# Comparing `tmp/transformers-4.9.1.tar.gz` & `tmp/transformers-4.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transformers-4.9.1.tar", last modified: Mon Jul 26 14:23:37 2021, max compression
+gzip compressed data, was "dist/transformers-4.9.2.tar", last modified: Mon Aug  9 14:24:42 2021, max compression
```

## Comparing `transformers-4.9.1.tar` & `transformers-4.9.2.tar`

### file list

```diff
@@ -1,624 +1,625 @@
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11418 2021-07-13 20:46:01.000000 transformers-4.9.1/LICENSE
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)       16 2020-09-19 03:12:34.000000 transformers-4.9.1/MANIFEST.in
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    43096 2021-07-26 14:23:37.000000 transformers-4.9.1/PKG-INFO
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    38681 2021-07-26 14:17:21.000000 transformers-4.9.1/README.md
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)       57 2021-07-13 20:46:01.000000 transformers-4.9.1/pyproject.toml
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      737 2021-07-26 14:23:37.000000 transformers-4.9.1/setup.cfg
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12613 2021-07-26 14:21:24.000000 transformers-4.9.1/setup.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   118787 2021-07-26 14:21:24.000000 transformers-4.9.1/src/transformers/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3537 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/activations.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2766 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/activations_tf.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/benchmark/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)        0 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10613 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/benchmark.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3777 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/benchmark_args.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4573 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/benchmark_args_tf.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5895 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/benchmark_args_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12924 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/benchmark_tf.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    37265 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/benchmark/benchmark_utils.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/commands/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      923 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9393 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/add_new_model.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7555 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/commands/convert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1860 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/download.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3223 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/env.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7951 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/lfs.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4316 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/run.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8088 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/serving.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6371 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/train.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1837 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/transformers_cli.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    15582 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/commands/user.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    40373 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/configuration_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    18640 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/convert_graph_to_onnx.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    16607 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/convert_pytorch_checkpoint_to_tf2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    29938 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/convert_slow_tokenizer.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     4955 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/convert_slow_tokenizers_checkpoints_to_fast.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2899 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/data/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1271 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    36353 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/data_collator.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/data/datasets/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1080 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/datasets/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6139 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/datasets/glue.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    22637 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/datasets/language_modeling.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9042 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/datasets/squad.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/data/metrics/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3783 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/metrics/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    29617 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/metrics/squad_metrics.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/data/processors/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1185 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/processors/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    23289 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/processors/glue.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    33283 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/processors/squad.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13833 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/processors/utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3290 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/processors/xnli.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3438 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/data/test_generation_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12950 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/debug_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    17035 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/deepspeed.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1772 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/dependency_versions_check.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2501 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/dependency_versions_table.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    15734 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/feature_extraction_sequence_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    21973 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/feature_extraction_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    80956 2021-07-21 16:40:49.000000 transformers-4.9.1/src/transformers/file_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    17536 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/generation_beam_search.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11805 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/generation_flax_logits_process.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    37887 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/generation_flax_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    26683 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/generation_logits_process.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5383 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/generation_stopping_criteria.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    91769 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/generation_tf_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   143441 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/generation_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7325 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/hf_api.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10711 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/hf_argparser.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8871 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/image_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    33602 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/integrations.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    29548 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/modelcard.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    38385 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/modeling_flax_outputs.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10482 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/modeling_flax_pytorch_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    25432 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/modeling_flax_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    52392 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/modeling_outputs.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    42017 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/modeling_tf_outputs.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    17997 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/modeling_tf_pytorch_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    77670 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/modeling_tf_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   105294 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/modeling_utils.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1656 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/__init__.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/albert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3549 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/albert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8984 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/albert/configuration_albert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2155 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    56453 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/albert/modeling_albert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    70275 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/albert/modeling_tf_albert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14513 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/albert/tokenization_albert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10552 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/albert/tokenization_albert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/auto/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8313 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/auto/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    27603 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/auto/auto_factory.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    22776 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/auto/configuration_auto.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8260 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/auto/feature_extraction_auto.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    33274 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/auto/modeling_auto.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9806 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/auto/modeling_flax_auto.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    21745 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/auto/modeling_tf_auto.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    27427 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/auto/tokenization_auto.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/bart/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3116 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10106 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/configuration_bart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5647 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    83415 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/modeling_bart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    72353 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/bart/modeling_flax_bart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    70569 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/modeling_tf_bart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3052 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/tokenization_bart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3942 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bart/tokenization_bart_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/barthez/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1475 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/barthez/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12497 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/barthez/tokenization_barthez.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8748 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/barthez/tokenization_barthez_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/bert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4611 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10322 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/bert/configuration_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10253 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2131 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4101 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    78800 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/bert/modeling_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    42177 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/bert/modeling_flax_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    82409 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/bert/modeling_tf_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    24552 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert/tokenization_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14323 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert/tokenization_bert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/bert_generation/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1908 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert_generation/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6324 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert_generation/configuration_bert_generation.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    27566 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert_generation/modeling_bert_generation.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6513 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert_generation/tokenization_bert_generation.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/bert_japanese/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1214 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bert_japanese/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13227 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/bert_japanese/tokenization_bert_japanese.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/bertweet/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1120 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bertweet/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    27394 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bertweet/tokenization_bertweet.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/big_bird/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3590 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/big_bird/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8037 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/big_bird/configuration_big_bird.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2466 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   135005 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/big_bird/modeling_big_bird.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    85524 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/big_bird/modeling_flax_big_bird.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12261 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/big_bird/tokenization_big_bird.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11146 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/big_bird/tokenization_big_bird_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/bigbird_pegasus/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2072 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bigbird_pegasus/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9748 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6295 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   142054 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/blenderbot/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2331 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8590 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/blenderbot/configuration_blenderbot.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3678 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    74735 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/blenderbot/modeling_blenderbot.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    73218 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot/modeling_tf_blenderbot.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4134 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot/tokenization_blenderbot.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2490 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8603 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/configuration_blenderbot_small.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    73753 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/modeling_blenderbot_small.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    72131 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8679 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/tokenization_blenderbot_small.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4063 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/byt5/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1103 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/byt5/__init__.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2107 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11475 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/byt5/tokenization_byt5.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/camembert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3303 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/camembert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1499 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/camembert/configuration_camembert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5734 2021-07-13 20:46:01.000000 transformers-4.9.1/src/transformers/models/camembert/modeling_camembert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6327 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/camembert/modeling_tf_camembert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12909 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/camembert/tokenization_camembert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8554 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/camembert/tokenization_camembert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/canine/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2146 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/canine/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6959 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/canine/configuration_canine.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2118 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    70648 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/canine/modeling_canine.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9435 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/canine/tokenization_canine.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/clip/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2995 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13419 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/configuration_clip.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5234 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/convert_clip_original_pytorch_to_hf.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9548 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/feature_extraction_clip.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    43692 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/clip/modeling_clip.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    44715 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/clip/modeling_flax_clip.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9021 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/processing_clip.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14668 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/tokenization_clip.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7022 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/clip/tokenization_clip_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/convbert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3380 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/convbert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6767 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/convbert/configuration_convbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2080 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    54697 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/convbert/modeling_convbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    58768 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/convbert/modeling_tf_convbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2216 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/convbert/tokenization_convbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2422 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/convbert/tokenization_convbert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/cpm/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1100 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/cpm/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5653 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/cpm/tokenization_cpm.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/ctrl/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2314 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ctrl/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5824 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ctrl/configuration_ctrl.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    29015 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ctrl/modeling_ctrl.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    38193 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ctrl/modeling_tf_ctrl.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8504 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ctrl/tokenization_ctrl.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/deberta/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2248 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deberta/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7628 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deberta/configuration_deberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    54099 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/deberta/modeling_deberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10346 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deberta/tokenization_deberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9082 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deberta/tokenization_deberta_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/deberta_v2/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2073 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deberta_v2/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7372 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deberta_v2/configuration_deberta_v2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    60591 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/deberta_v2/modeling_deberta_v2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    21489 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/deberta_v2/tokenization_deberta_v2.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/deit/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1947 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deit/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5379 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deit/configuration_deit.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9000 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deit/convert_deit_timm_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7516 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/deit/feature_extraction_deit.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    31573 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/deit/modeling_deit.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/detr/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1900 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/detr/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9986 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/detr/configuration_detr.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13304 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    40828 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/detr/feature_extraction_detr.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   107836 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/detr/modeling_detr.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/dialogpt/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)        0 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dialogpt/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1542 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/distilbert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3469 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/distilbert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7276 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/distilbert/configuration_distilbert.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    39882 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/distilbert/modeling_distilbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    49790 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/distilbert/modeling_tf_distilbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3035 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/distilbert/tokenization_distilbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4056 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/distilbert/tokenization_distilbert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/dpr/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3826 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dpr/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6939 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dpr/configuration_dpr.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6043 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    28713 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/dpr/modeling_dpr.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    37860 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dpr/modeling_tf_dpr.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    20037 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dpr/tokenization_dpr.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    20519 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/dpr/tokenization_dpr_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/electra/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4186 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/electra/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9202 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/electra/configuration_electra.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2845 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    61975 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/electra/modeling_electra.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    42701 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/electra/modeling_flax_electra.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    63334 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/electra/modeling_tf_electra.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2932 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/electra/tokenization_electra.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3958 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/electra/tokenization_electra_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/encoder_decoder/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1360 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/encoder_decoder/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5040 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/encoder_decoder/configuration_encoder_decoder.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    26150 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/encoder_decoder/modeling_encoder_decoder.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/flaubert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3000 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/flaubert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8932 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/flaubert/configuration_flaubert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    17590 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/flaubert/modeling_flaubert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    40272 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/flaubert/modeling_tf_flaubert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5634 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/flaubert/tokenization_flaubert.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/fsmt/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1549 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/fsmt/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10332 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/fsmt/configuration_fsmt.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    11261 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    53914 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/fsmt/modeling_fsmt.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    19528 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/fsmt/tokenization_fsmt.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/funnel/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3479 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/funnel/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9492 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/funnel/configuration_funnel.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2346 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    66858 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/funnel/modeling_funnel.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    78480 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/funnel/modeling_tf_funnel.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5374 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/funnel/tokenization_funnel.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6927 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/funnel/tokenization_funnel_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/gpt2/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3123 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11777 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/configuration_gpt2.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2539 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    25996 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/modeling_flax_gpt2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    57110 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/modeling_gpt2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    45855 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/modeling_tf_gpt2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12364 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/tokenization_gpt2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8131 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt2/tokenization_gpt2_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/gpt_neo/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2146 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt_neo/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8477 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt_neo/configuration_gpt_neo.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2555 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    27203 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt_neo/modeling_flax_gpt_neo.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    48638 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/gpt_neo/modeling_gpt_neo.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/herbert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1353 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/herbert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3318 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/herbert/tokenization_herbert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6637 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/herbert/tokenization_herbert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/hubert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2081 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/hubert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12793 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/hubert/configuration_hubert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10289 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    46180 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/hubert/modeling_hubert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    69660 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/hubert/modeling_tf_hubert.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/ibert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1931 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ibert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6985 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ibert/configuration_ibert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    55422 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ibert/modeling_ibert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    30518 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/ibert/quant_modules.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/layoutlm/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3074 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/layoutlm/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6160 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/layoutlm/configuration_layoutlm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    50874 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/layoutlm/modeling_layoutlm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    58199 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/layoutlm/modeling_tf_layoutlm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2088 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/layoutlm/tokenization_layoutlm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2550 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/layoutlm/tokenization_layoutlm_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/led/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2361 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/led/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8324 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/led/configuration_led.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   134093 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/led/modeling_led.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   120358 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/led/modeling_tf_led.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1864 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/led/tokenization_led.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2031 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/led/tokenization_led_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/longformer/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3549 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/longformer/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4123 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/longformer/configuration_longformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3027 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   110628 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/longformer/modeling_longformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   127235 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/longformer/modeling_tf_longformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3160 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/longformer/tokenization_longformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4188 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/longformer/tokenization_longformer_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/luke/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1897 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/luke/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6702 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/luke/configuration_luke.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6719 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    63091 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/luke/modeling_luke.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    78060 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/luke/tokenization_luke.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/lxmert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2749 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9843 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/configuration_lxmert.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2120 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    64442 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/modeling_lxmert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    66786 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/modeling_tf_lxmert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1736 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/tokenization_lxmert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2098 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/lxmert/tokenization_lxmert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/m2m_100/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1828 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/m2m_100/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7857 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/m2m_100/configuration_m2m_100.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3118 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    63602 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/m2m_100/modeling_m2m_100.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    16130 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/m2m_100/tokenization_m2m_100.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/marian/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2531 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/marian/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8388 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/marian/configuration_marian.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    33875 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    23461 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/marian/convert_marian_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    63842 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/marian/modeling_flax_marian.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    73840 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/marian/modeling_marian.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    73427 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/marian/modeling_tf_marian.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    15286 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/marian/tokenization_marian.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/mbart/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3526 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8333 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/configuration_mbart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3035 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    74350 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/mbart/modeling_flax_mbart.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    84451 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/modeling_mbart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    72804 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/modeling_tf_mbart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9967 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    16070 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart50.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12145 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart50_fast.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9921 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/megatron_bert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2380 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/megatron_bert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6956 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/megatron_bert/configuration_megatron_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9641 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    78672 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/megatron_bert/modeling_megatron_bert.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/mmbt/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1360 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mmbt/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1654 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mmbt/configuration_mmbt.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    19250 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mmbt/modeling_mmbt.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/mobilebert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3847 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mobilebert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7804 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/mobilebert/configuration_mobilebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2172 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    66006 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/mobilebert/modeling_mobilebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    76628 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/mobilebert/modeling_tf_mobilebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1729 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mobilebert/tokenization_mobilebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2094 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mobilebert/tokenization_mobilebert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/mpnet/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3224 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mpnet/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5659 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mpnet/configuration_mpnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    41065 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mpnet/modeling_mpnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    55732 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mpnet/modeling_tf_mpnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    22284 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/mpnet/tokenization_mpnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9053 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mpnet/tokenization_mpnet_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/mt5/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2221 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mt5/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5595 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mt5/configuration_mt5.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4250 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mt5/modeling_mt5.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3614 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/mt5/modeling_tf_mt5.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/openai/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3011 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8395 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/configuration_openai.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2673 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    35876 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/modeling_openai.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    41855 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/modeling_tf_openai.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8507 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/tokenization_openai.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3085 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/openai/tokenization_openai_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/pegasus/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2575 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/pegasus/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8344 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/pegasus/configuration_pegasus.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5362 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    73813 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/pegasus/modeling_pegasus.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    73429 2021-07-14 14:24:49.000000 transformers-4.9.1/src/transformers/models/pegasus/modeling_tf_pegasus.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13079 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/pegasus/tokenization_pegasus.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9639 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/pegasus/tokenization_pegasus_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/phobert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1116 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/phobert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13718 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/phobert/tokenization_phobert.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/prophetnet/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2031 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/prophetnet/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8652 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/prophetnet/configuration_prophetnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7055 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   113056 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/prophetnet/modeling_prophetnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12509 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/prophetnet/tokenization_prophetnet.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/rag/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2052 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/rag/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9289 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/rag/configuration_rag.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    89845 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/rag/modeling_rag.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    97101 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/rag/modeling_tf_rag.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    29159 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/rag/retrieval_rag.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4898 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/rag/tokenization_rag.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/reformer/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2499 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/reformer/__init__.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    13521 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/reformer/configuration_reformer.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     7790 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   110884 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/reformer/modeling_reformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6679 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/reformer/tokenization_reformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4552 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/reformer/tokenization_reformer_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/retribert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1976 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/retribert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5357 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/retribert/configuration_retribert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9449 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/retribert/modeling_retribert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1884 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/retribert/tokenization_retribert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2264 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/retribert/tokenization_retribert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/roberta/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4054 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roberta/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3454 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roberta/configuration_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8002 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    37120 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/roberta/modeling_flax_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    67588 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/roberta/modeling_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    59857 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/roberta/modeling_tf_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12006 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roberta/tokenization_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10916 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roberta/tokenization_roberta_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/roformer/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3512 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7442 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/configuration_roformer.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2212 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    67008 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/modeling_roformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    67531 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/modeling_tf_roformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14478 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/roformer/tokenization_roformer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8273 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/tokenization_roformer_fast.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2651 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/roformer/tokenization_utils.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/speech_to_text/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2527 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/speech_to_text/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9928 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/speech_to_text/configuration_speech_to_text.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4071 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10108 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/speech_to_text/feature_extraction_speech_to_text.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    64733 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/speech_to_text/modeling_speech_to_text.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6929 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/speech_to_text/processing_speech_to_text.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10949 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/speech_to_text/tokenization_speech_to_text.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/squeezebert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2510 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/squeezebert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7210 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/squeezebert/configuration_squeezebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    44244 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/squeezebert/modeling_squeezebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2337 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/squeezebert/tokenization_squeezebert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2989 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/squeezebert/tokenization_squeezebert_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/t5/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3042 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/t5/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8940 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/t5/configuration_t5.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2107 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    68939 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/t5/modeling_flax_t5.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    81418 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/t5/modeling_t5.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    74076 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/t5/modeling_tf_t5.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13155 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/t5/tokenization_t5.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8622 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/t5/tokenization_t5_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/tapas/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1879 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/tapas/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13459 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/tapas/configuration_tapas.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5093 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   106883 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/tapas/modeling_tapas.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   119284 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/tapas/tokenization_tapas.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/transfo_xl/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2808 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8128 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/configuration_transfo_xl.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     4923 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    48370 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/modeling_tf_transfo_xl.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7588 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    53495 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/modeling_transfo_xl.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10694 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    30667 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/transfo_xl/tokenization_transfo_xl.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/visual_bert/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2116 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/visual_bert/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8153 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/visual_bert/configuration_visual_bert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5158 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    67162 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/visual_bert/modeling_visual_bert.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/vit/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2159 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/vit/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5272 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/vit/configuration_vit.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9959 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/vit/convert_vit_timm_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6646 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/vit/feature_extraction_vit.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    22844 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/vit/modeling_flax_vit.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    24782 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/vit/modeling_vit.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/wav2vec2/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3145 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/wav2vec2/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    15046 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/wav2vec2/configuration_wav2vec2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    10612 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9625 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/models/wav2vec2/feature_extraction_wav2vec2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    50889 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/models/wav2vec2/modeling_flax_wav2vec2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    68358 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/wav2vec2/modeling_tf_wav2vec2.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    66594 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/models/wav2vec2/modeling_wav2vec2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7492 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/wav2vec2/processing_wav2vec2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    24737 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/wav2vec2/tokenization_wav2vec2.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/xlm/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2886 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11891 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm/configuration_xlm.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     2981 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    59142 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm/modeling_tf_xlm.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    53247 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm/modeling_xlm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    34429 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm/tokenization_xlm.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/xlm_prophetnet/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1360 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_prophetnet/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1262 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7309 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    13840 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3477 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2620 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/configuration_xlm_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6353 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5877 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/modeling_xlm_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14051 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/tokenization_xlm_roberta.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9965 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/models/xlnet/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3421 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    11248 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/configuration_xlnet.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)     3695 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    81280 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/modeling_tf_xlnet.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    91661 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/modeling_xlnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14406 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/tokenization_xlnet.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9944 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/models/xlnet/tokenization_xlnet_fast.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/onnx/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      829 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/onnx/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5822 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/onnx/__main__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7860 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/onnx/config.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8698 2021-07-21 10:41:17.000000 transformers-4.9.1/src/transformers/onnx/convert.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2377 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/onnx/utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    27375 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/optimization.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    15890 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/optimization_tf.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/pipelines/
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)    24467 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6526 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/automatic_speech_recognition.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    30282 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/pipelines/base.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14841 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/conversational.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3684 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/feature_extraction.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8780 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/fill_mask.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5155 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/image_classification.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    24463 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/question_answering.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14037 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/table_question_answering.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14756 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/text2text_generation.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3194 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/text_classification.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8974 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/text_generation.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    19373 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/token_classification.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8455 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/pipelines/zero_shot_classification.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/sagemaker/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      901 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/sagemaker/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1044 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/sagemaker/trainer_sm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4926 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/sagemaker/training_args_sm.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    42795 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/testing_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    32397 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/tokenization_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)   165870 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/tokenization_utils_base.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    32188 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/tokenization_utils_fast.py
--rwxr-xr-x   0 sgugger   (1000) sgugger   (1000)   126345 2021-07-23 04:42:24.000000 transformers-4.9.1/src/transformers/trainer.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    23488 2021-07-21 14:20:39.000000 transformers-4.9.1/src/transformers/trainer_callback.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    44264 2021-07-14 14:26:49.000000 transformers-4.9.1/src/transformers/trainer_pt_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9744 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/trainer_seq2seq.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    34959 2021-07-14 17:53:55.000000 transformers-4.9.1/src/transformers/trainer_tf.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    15414 2021-07-21 16:40:52.000000 transformers-4.9.1/src/transformers/trainer_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    57088 2021-07-26 14:21:07.000000 transformers-4.9.1/src/transformers/training_args.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1754 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/training_args_seq2seq.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14909 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/training_args_tf.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers/utils/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1520 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1715 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/coco_classes.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    19181 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_flax_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    88488 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/utils/dummy_pt_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      376 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_sentencepiece_and_speech_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      278 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_sentencepiece_and_tokenizers_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4089 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/utils/dummy_sentencepiece_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      241 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_speech_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    47447 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/utils/dummy_tf_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1108 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_timm_and_vision_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      810 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_timm_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     8684 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/utils/dummy_tokenizers_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      916 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/dummy_vision_objects.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14869 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/fx.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4971 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/hp_naming.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    33616 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/imagenet_classes.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     7701 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/logging.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2186 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/model_parallel_utils.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    16415 2021-07-26 14:17:21.000000 transformers-4.9.1/src/transformers/utils/modeling_auto_mapping.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    14431 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/notebook.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    39607 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/sentencepiece_model_pb2.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     4381 2021-07-13 20:46:02.000000 transformers-4.9.1/src/transformers/utils/versions.py
-drwxr-xr-x   0 sgugger   (1000) sgugger   (1000)        0 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    43096 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/PKG-INFO
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    28260 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/SOURCES.txt
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)        1 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/dependency_links.txt
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)       82 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/entry_points.txt
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3024 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/requires.txt
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)       13 2021-07-26 14:23:37.000000 transformers-4.9.1/src/transformers.egg-info/top_level.txt
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.698037 transformers-4.9.2/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11418 2021-07-12 07:26:47.000000 transformers-4.9.2/LICENSE
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)       16 2020-11-27 00:13:10.000000 transformers-4.9.2/MANIFEST.in
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    43096 2021-08-09 14:24:42.698037 transformers-4.9.2/PKG-INFO
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    38681 2021-08-09 14:23:38.000000 transformers-4.9.2/README.md
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)       57 2021-06-28 07:40:59.000000 transformers-4.9.2/pyproject.toml
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      737 2021-08-09 14:24:42.698037 transformers-4.9.2/setup.cfg
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12613 2021-08-09 14:23:38.000000 transformers-4.9.2/setup.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.638038 transformers-4.9.2/src/
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.648037 transformers-4.9.2/src/transformers/
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   118787 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3537 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/activations.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2766 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/activations_tf.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.648037 transformers-4.9.2/src/transformers/benchmark/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)        0 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/benchmark/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10613 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/benchmark/benchmark.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3777 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/benchmark/benchmark_args.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4573 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/benchmark/benchmark_args_tf.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5895 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/benchmark/benchmark_args_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12924 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/benchmark/benchmark_tf.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    37265 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/benchmark/benchmark_utils.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.648037 transformers-4.9.2/src/transformers/commands/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      923 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/commands/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9393 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/add_new_model.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7555 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/commands/convert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1860 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/commands/download.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3223 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/env.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7951 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/lfs.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4316 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/run.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8088 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/serving.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6371 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/train.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1837 2021-07-14 08:25:45.000000 transformers-4.9.2/src/transformers/commands/transformers_cli.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15582 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/commands/user.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    40373 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/configuration_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    18640 2021-07-14 09:14:58.000000 transformers-4.9.2/src/transformers/convert_graph_to_onnx.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    16607 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/convert_pytorch_checkpoint_to_tf2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    29938 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/convert_slow_tokenizer.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     4955 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/convert_slow_tokenizers_checkpoints_to_fast.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2899 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.648037 transformers-4.9.2/src/transformers/data/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1271 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/data/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    36353 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/data/data_collator.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.648037 transformers-4.9.2/src/transformers/data/datasets/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1080 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/data/datasets/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6139 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/datasets/glue.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    22637 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/datasets/language_modeling.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9042 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/datasets/squad.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/data/metrics/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3783 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/metrics/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    29617 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/metrics/squad_metrics.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/data/processors/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1185 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/data/processors/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    23289 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/processors/glue.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    33283 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/processors/squad.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13833 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/processors/utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3290 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/data/processors/xnli.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3438 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/data/test_generation_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12950 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/debug_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    17035 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/deepspeed.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1772 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/dependency_versions_check.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2501 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/dependency_versions_table.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15734 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/feature_extraction_sequence_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    21973 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/feature_extraction_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    81311 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/file_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    17536 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/generation_beam_search.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11805 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/generation_flax_logits_process.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    37887 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/generation_flax_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    26683 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/generation_logits_process.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5383 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/generation_stopping_criteria.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    91769 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/generation_tf_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   143441 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/generation_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7325 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/hf_api.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10711 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/hf_argparser.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8871 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/image_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    33602 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/integrations.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    29548 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/modelcard.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    38385 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/modeling_flax_outputs.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10482 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/modeling_flax_pytorch_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    25432 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/modeling_flax_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    52392 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/modeling_outputs.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    42017 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/modeling_tf_outputs.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    17997 2021-07-24 10:50:44.000000 transformers-4.9.2/src/transformers/modeling_tf_pytorch_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    77670 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/modeling_tf_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   105419 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/modeling_utils.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/models/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1656 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/__init__.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/models/albert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3549 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/albert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8984 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/albert/configuration_albert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2155 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    56499 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/albert/modeling_albert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    70275 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/albert/modeling_tf_albert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14513 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/albert/tokenization_albert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10552 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/albert/tokenization_albert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/models/auto/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8313 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/auto/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    27603 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/auto_factory.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    22776 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/configuration_auto.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8260 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/feature_extraction_auto.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    33274 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/modeling_auto.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9806 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/modeling_flax_auto.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    21745 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/modeling_tf_auto.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    27427 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/auto/tokenization_auto.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/models/bart/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3116 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bart/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10106 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bart/configuration_bart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5647 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    83415 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bart/modeling_bart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    72353 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/bart/modeling_flax_bart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    70569 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bart/modeling_tf_bart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3052 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/bart/tokenization_bart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3942 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/bart/tokenization_bart_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.651371 transformers-4.9.2/src/transformers/models/barthez/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1475 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/barthez/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12497 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/barthez/tokenization_barthez.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8748 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/barthez/tokenization_barthez_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.654704 transformers-4.9.2/src/transformers/models/bert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4611 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10322 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/bert/configuration_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10253 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2131 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4101 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    78800 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/bert/modeling_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    42177 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/bert/modeling_flax_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    82409 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/bert/modeling_tf_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    24552 2021-08-04 13:06:53.000000 transformers-4.9.2/src/transformers/models/bert/tokenization_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14323 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/bert/tokenization_bert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.654704 transformers-4.9.2/src/transformers/models/bert_generation/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1908 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bert_generation/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6324 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/bert_generation/configuration_bert_generation.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    27600 2021-08-09 13:53:05.000000 transformers-4.9.2/src/transformers/models/bert_generation/modeling_bert_generation.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6513 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bert_generation/tokenization_bert_generation.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.654704 transformers-4.9.2/src/transformers/models/bert_japanese/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1214 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bert_japanese/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13227 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bert_japanese/tokenization_bert_japanese.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.654704 transformers-4.9.2/src/transformers/models/bertweet/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1120 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bertweet/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    27394 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bertweet/tokenization_bertweet.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.654704 transformers-4.9.2/src/transformers/models/big_bird/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3590 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/big_bird/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8037 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/big_bird/configuration_big_bird.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2466 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   135005 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/big_bird/modeling_big_bird.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    85524 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/big_bird/modeling_flax_big_bird.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12261 2021-07-12 13:49:39.000000 transformers-4.9.2/src/transformers/models/big_bird/tokenization_big_bird.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11146 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/big_bird/tokenization_big_bird_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.658037 transformers-4.9.2/src/transformers/models/bigbird_pegasus/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2072 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/bigbird_pegasus/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9748 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6295 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   142054 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.658037 transformers-4.9.2/src/transformers/models/blenderbot/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2331 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8590 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot/configuration_blenderbot.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3678 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    74735 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot/modeling_blenderbot.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    73218 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot/modeling_tf_blenderbot.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4134 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/blenderbot/tokenization_blenderbot.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.658037 transformers-4.9.2/src/transformers/models/blenderbot_small/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2490 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot_small/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8603 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/blenderbot_small/configuration_blenderbot_small.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    73753 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot_small/modeling_blenderbot_small.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    72131 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8679 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/blenderbot_small/tokenization_blenderbot_small.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4063 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.658037 transformers-4.9.2/src/transformers/models/byt5/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1103 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/byt5/__init__.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2107 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11475 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/byt5/tokenization_byt5.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.658037 transformers-4.9.2/src/transformers/models/camembert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3303 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/camembert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1499 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/camembert/configuration_camembert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5734 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/camembert/modeling_camembert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6327 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/camembert/modeling_tf_camembert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12909 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/camembert/tokenization_camembert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8554 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/camembert/tokenization_camembert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.658037 transformers-4.9.2/src/transformers/models/canine/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2146 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/canine/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6959 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/canine/configuration_canine.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2118 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    70648 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/canine/modeling_canine.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9435 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/canine/tokenization_canine.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/clip/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2995 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/clip/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13419 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/clip/configuration_clip.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5234 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/clip/convert_clip_original_pytorch_to_hf.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9548 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/clip/feature_extraction_clip.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    43692 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/clip/modeling_clip.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    44715 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/clip/modeling_flax_clip.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9021 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/clip/processing_clip.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14668 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/clip/tokenization_clip.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7022 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/clip/tokenization_clip_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/convbert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3380 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/convbert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6767 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/convbert/configuration_convbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2080 2021-07-12 12:32:19.000000 transformers-4.9.2/src/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    54697 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/convbert/modeling_convbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    58768 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/convbert/modeling_tf_convbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2216 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/convbert/tokenization_convbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2422 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/convbert/tokenization_convbert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/cpm/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1100 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/cpm/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5653 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/cpm/tokenization_cpm.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/ctrl/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2314 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/ctrl/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5824 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/ctrl/configuration_ctrl.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    29015 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/ctrl/modeling_ctrl.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    38193 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/ctrl/modeling_tf_ctrl.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8504 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/ctrl/tokenization_ctrl.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/deberta/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2248 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/deberta/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7628 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/deberta/configuration_deberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    54099 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/deberta/modeling_deberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10346 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/deberta/tokenization_deberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9082 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/deberta/tokenization_deberta_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/deberta_v2/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2073 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/deberta_v2/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7372 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/deberta_v2/configuration_deberta_v2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    60591 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/deberta_v2/modeling_deberta_v2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    21489 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/deberta_v2/tokenization_deberta_v2.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.661371 transformers-4.9.2/src/transformers/models/deit/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1947 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/deit/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5379 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/deit/configuration_deit.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9000 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/deit/convert_deit_timm_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7516 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/deit/feature_extraction_deit.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    31573 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/deit/modeling_deit.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/detr/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1900 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/detr/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9986 2021-07-13 14:17:19.000000 transformers-4.9.2/src/transformers/models/detr/configuration_detr.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13304 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    40828 2021-07-13 14:17:19.000000 transformers-4.9.2/src/transformers/models/detr/feature_extraction_detr.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   107836 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/detr/modeling_detr.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/dialogpt/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)        0 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/dialogpt/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1542 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/distilbert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3469 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/distilbert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7276 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/distilbert/configuration_distilbert.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    39882 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/distilbert/modeling_distilbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    49790 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/distilbert/modeling_tf_distilbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3035 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/distilbert/tokenization_distilbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4056 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/distilbert/tokenization_distilbert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/dpr/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3826 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/dpr/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6939 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/dpr/configuration_dpr.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6043 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    28713 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/dpr/modeling_dpr.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    37860 2021-07-24 15:36:09.000000 transformers-4.9.2/src/transformers/models/dpr/modeling_tf_dpr.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    20037 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/dpr/tokenization_dpr.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    20519 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/dpr/tokenization_dpr_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/electra/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4186 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/electra/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9202 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/electra/configuration_electra.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2845 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    61975 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/electra/modeling_electra.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    42701 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/electra/modeling_flax_electra.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    63334 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/electra/modeling_tf_electra.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2932 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/electra/tokenization_electra.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3958 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/electra/tokenization_electra_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/encoder_decoder/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1360 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/encoder_decoder/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5040 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/encoder_decoder/configuration_encoder_decoder.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    26150 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/encoder_decoder/modeling_encoder_decoder.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.664704 transformers-4.9.2/src/transformers/models/flaubert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3000 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/flaubert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8932 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/flaubert/configuration_flaubert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    17590 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/flaubert/modeling_flaubert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    40272 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/flaubert/modeling_tf_flaubert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5634 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/flaubert/tokenization_flaubert.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/fsmt/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1549 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/fsmt/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10332 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/fsmt/configuration_fsmt.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    11261 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    53914 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/fsmt/modeling_fsmt.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    19528 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/fsmt/tokenization_fsmt.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/funnel/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3479 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/funnel/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9492 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/funnel/configuration_funnel.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2346 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    66858 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/funnel/modeling_funnel.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    78480 2021-07-24 15:36:09.000000 transformers-4.9.2/src/transformers/models/funnel/modeling_tf_funnel.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5374 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/funnel/tokenization_funnel.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6927 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/funnel/tokenization_funnel_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/gpt2/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3123 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/gpt2/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11777 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/gpt2/configuration_gpt2.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2539 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    25996 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/gpt2/modeling_flax_gpt2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    57110 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/gpt2/modeling_gpt2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    45855 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/gpt2/modeling_tf_gpt2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12364 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/gpt2/tokenization_gpt2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8131 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/gpt2/tokenization_gpt2_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/gpt_neo/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2184 2021-08-09 13:50:44.000000 transformers-4.9.2/src/transformers/models/gpt_neo/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15188 2021-08-09 13:50:58.000000 transformers-4.9.2/src/transformers/models/gpt_neo/configuration_gpt_neo.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2555 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    27203 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/gpt_neo/modeling_flax_gpt_neo.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    48645 2021-08-09 13:50:44.000000 transformers-4.9.2/src/transformers/models/gpt_neo/modeling_gpt_neo.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/herbert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1353 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/herbert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3318 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/herbert/tokenization_herbert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6637 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/herbert/tokenization_herbert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/hubert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2081 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/hubert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12793 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/hubert/configuration_hubert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10289 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    46180 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/hubert/modeling_hubert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    69660 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/hubert/modeling_tf_hubert.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.668037 transformers-4.9.2/src/transformers/models/ibert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1931 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/ibert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6985 2021-07-12 12:32:19.000000 transformers-4.9.2/src/transformers/models/ibert/configuration_ibert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    55456 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/ibert/modeling_ibert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    30518 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/ibert/quant_modules.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.671371 transformers-4.9.2/src/transformers/models/layoutlm/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3074 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/layoutlm/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6160 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/layoutlm/configuration_layoutlm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    50874 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/layoutlm/modeling_layoutlm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    58199 2021-07-24 15:36:09.000000 transformers-4.9.2/src/transformers/models/layoutlm/modeling_tf_layoutlm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2088 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/layoutlm/tokenization_layoutlm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2550 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/layoutlm/tokenization_layoutlm_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.671371 transformers-4.9.2/src/transformers/models/led/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2361 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/led/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8324 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/led/configuration_led.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   134093 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/led/modeling_led.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   120358 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/led/modeling_tf_led.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1864 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/led/tokenization_led.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2031 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/led/tokenization_led_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.671371 transformers-4.9.2/src/transformers/models/longformer/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3549 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/longformer/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4123 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/longformer/configuration_longformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3027 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   110662 2021-08-09 13:53:05.000000 transformers-4.9.2/src/transformers/models/longformer/modeling_longformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   127235 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/longformer/modeling_tf_longformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3160 2021-07-12 12:37:52.000000 transformers-4.9.2/src/transformers/models/longformer/tokenization_longformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4188 2021-07-12 12:37:52.000000 transformers-4.9.2/src/transformers/models/longformer/tokenization_longformer_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.671371 transformers-4.9.2/src/transformers/models/luke/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1897 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/luke/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6702 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/luke/configuration_luke.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6719 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    63091 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/luke/modeling_luke.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    78060 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/luke/tokenization_luke.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.671371 transformers-4.9.2/src/transformers/models/lxmert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2749 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/lxmert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9843 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/lxmert/configuration_lxmert.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2120 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    64442 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/lxmert/modeling_lxmert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    66786 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/lxmert/modeling_tf_lxmert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1736 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/lxmert/tokenization_lxmert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2098 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/lxmert/tokenization_lxmert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.671371 transformers-4.9.2/src/transformers/models/m2m_100/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1828 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/m2m_100/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7857 2021-07-12 12:32:19.000000 transformers-4.9.2/src/transformers/models/m2m_100/configuration_m2m_100.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3118 2021-07-12 12:32:19.000000 transformers-4.9.2/src/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    63602 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/m2m_100/modeling_m2m_100.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    16130 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/m2m_100/tokenization_m2m_100.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.674704 transformers-4.9.2/src/transformers/models/marian/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2531 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/marian/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8388 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/marian/configuration_marian.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    33875 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    23461 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/marian/convert_marian_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    63842 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/marian/modeling_flax_marian.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    73840 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/marian/modeling_marian.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    73427 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/marian/modeling_tf_marian.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15286 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/marian/tokenization_marian.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.674704 transformers-4.9.2/src/transformers/models/mbart/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3562 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mbart/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9398 2021-08-09 13:52:07.000000 transformers-4.9.2/src/transformers/models/mbart/configuration_mbart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3035 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    74350 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mbart/modeling_flax_mbart.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    84451 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/mbart/modeling_mbart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    72804 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/mbart/modeling_tf_mbart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9967 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    16070 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart50.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12145 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart50_fast.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9921 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.674704 transformers-4.9.2/src/transformers/models/megatron_bert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2380 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/megatron_bert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6956 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/megatron_bert/configuration_megatron_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9641 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    78672 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/megatron_bert/modeling_megatron_bert.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.674704 transformers-4.9.2/src/transformers/models/mmbt/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1360 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/mmbt/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1654 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/mmbt/configuration_mmbt.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    19250 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/mmbt/modeling_mmbt.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.674704 transformers-4.9.2/src/transformers/models/mobilebert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3847 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/mobilebert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7804 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mobilebert/configuration_mobilebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2172 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    66006 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mobilebert/modeling_mobilebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    76628 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mobilebert/modeling_tf_mobilebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1729 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/mobilebert/tokenization_mobilebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2094 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/mobilebert/tokenization_mobilebert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.674704 transformers-4.9.2/src/transformers/models/mpnet/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3224 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/mpnet/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5659 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/mpnet/configuration_mpnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    41065 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mpnet/modeling_mpnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    55732 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/mpnet/modeling_tf_mpnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    22284 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/mpnet/tokenization_mpnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9053 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/mpnet/tokenization_mpnet_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.678037 transformers-4.9.2/src/transformers/models/mt5/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2221 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/mt5/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5595 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/mt5/configuration_mt5.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4250 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/mt5/modeling_mt5.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3614 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/mt5/modeling_tf_mt5.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.678037 transformers-4.9.2/src/transformers/models/openai/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3011 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/openai/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8395 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/openai/configuration_openai.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2673 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    35876 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/openai/modeling_openai.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    41855 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/openai/modeling_tf_openai.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8507 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/openai/tokenization_openai.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3085 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/openai/tokenization_openai_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.678037 transformers-4.9.2/src/transformers/models/pegasus/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2575 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/pegasus/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8344 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/pegasus/configuration_pegasus.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5362 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    73813 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/pegasus/modeling_pegasus.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    73429 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/pegasus/modeling_tf_pegasus.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13079 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/pegasus/tokenization_pegasus.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9639 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/pegasus/tokenization_pegasus_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.678037 transformers-4.9.2/src/transformers/models/phobert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1116 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/phobert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13718 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/phobert/tokenization_phobert.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.678037 transformers-4.9.2/src/transformers/models/prophetnet/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2031 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/prophetnet/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8652 2021-07-12 12:32:19.000000 transformers-4.9.2/src/transformers/models/prophetnet/configuration_prophetnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7055 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   113056 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/prophetnet/modeling_prophetnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12509 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/prophetnet/tokenization_prophetnet.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.678037 transformers-4.9.2/src/transformers/models/rag/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2052 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/rag/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9289 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/rag/configuration_rag.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    89845 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/rag/modeling_rag.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    97101 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/rag/modeling_tf_rag.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    29159 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/rag/retrieval_rag.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4898 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/rag/tokenization_rag.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.681371 transformers-4.9.2/src/transformers/models/reformer/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2499 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/reformer/__init__.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    13521 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/reformer/configuration_reformer.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     7790 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   110930 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/reformer/modeling_reformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6679 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/reformer/tokenization_reformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4552 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/reformer/tokenization_reformer_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.681371 transformers-4.9.2/src/transformers/models/retribert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1976 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/retribert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5357 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/retribert/configuration_retribert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9449 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/retribert/modeling_retribert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1884 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/retribert/tokenization_retribert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2264 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/retribert/tokenization_retribert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.681371 transformers-4.9.2/src/transformers/models/roberta/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4054 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roberta/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3454 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roberta/configuration_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8002 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    37120 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/roberta/modeling_flax_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    67622 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/roberta/modeling_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    59857 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/roberta/modeling_tf_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    12006 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/roberta/tokenization_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10916 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/roberta/tokenization_roberta_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.681371 transformers-4.9.2/src/transformers/models/roformer/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3512 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roformer/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7442 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roformer/configuration_roformer.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2212 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    67008 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/roformer/modeling_roformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    67531 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roformer/modeling_tf_roformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14478 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roformer/tokenization_roformer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8273 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roformer/tokenization_roformer_fast.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2651 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/roformer/tokenization_utils.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.681371 transformers-4.9.2/src/transformers/models/speech_to_text/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2527 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/speech_to_text/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9928 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/speech_to_text/configuration_speech_to_text.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4071 2021-07-12 12:37:05.000000 transformers-4.9.2/src/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10108 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/speech_to_text/feature_extraction_speech_to_text.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    64733 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/speech_to_text/modeling_speech_to_text.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6929 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/speech_to_text/processing_speech_to_text.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10949 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/speech_to_text/tokenization_speech_to_text.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.684704 transformers-4.9.2/src/transformers/models/squeezebert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2510 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/squeezebert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7210 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/squeezebert/configuration_squeezebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    44244 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/squeezebert/modeling_squeezebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2337 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/squeezebert/tokenization_squeezebert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2989 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/squeezebert/tokenization_squeezebert_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.684704 transformers-4.9.2/src/transformers/models/t5/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3042 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/t5/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10613 2021-08-09 13:50:58.000000 transformers-4.9.2/src/transformers/models/t5/configuration_t5.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2107 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    68939 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/t5/modeling_flax_t5.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    81385 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/t5/modeling_t5.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    74076 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/t5/modeling_tf_t5.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13155 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/t5/tokenization_t5.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8622 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/t5/tokenization_t5_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.684704 transformers-4.9.2/src/transformers/models/tapas/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1879 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/tapas/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13459 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/tapas/configuration_tapas.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5093 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   106883 2021-08-05 06:50:06.000000 transformers-4.9.2/src/transformers/models/tapas/modeling_tapas.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   119284 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/tapas/tokenization_tapas.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.684704 transformers-4.9.2/src/transformers/models/transfo_xl/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2808 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/transfo_xl/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8128 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/transfo_xl/configuration_transfo_xl.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     4923 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    48370 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/transfo_xl/modeling_tf_transfo_xl.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7588 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    53495 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/transfo_xl/modeling_transfo_xl.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10694 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    30667 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/transfo_xl/tokenization_transfo_xl.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.684704 transformers-4.9.2/src/transformers/models/visual_bert/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2116 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/visual_bert/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8153 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/visual_bert/configuration_visual_bert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5158 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    67162 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/visual_bert/modeling_visual_bert.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.688037 transformers-4.9.2/src/transformers/models/vit/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2159 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/vit/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5272 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/vit/configuration_vit.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9959 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/vit/convert_vit_timm_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6646 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/vit/feature_extraction_vit.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    22844 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/vit/modeling_flax_vit.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    24782 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/vit/modeling_vit.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.688037 transformers-4.9.2/src/transformers/models/wav2vec2/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3145 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/wav2vec2/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15046 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/wav2vec2/configuration_wav2vec2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    10612 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9625 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/wav2vec2/feature_extraction_wav2vec2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    50889 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/wav2vec2/modeling_flax_wav2vec2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    68358 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/wav2vec2/modeling_tf_wav2vec2.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    66594 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/wav2vec2/modeling_wav2vec2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7492 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/wav2vec2/processing_wav2vec2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    24737 2021-07-12 14:16:40.000000 transformers-4.9.2/src/transformers/models/wav2vec2/tokenization_wav2vec2.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.691370 transformers-4.9.2/src/transformers/models/xlm/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2886 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlm/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11891 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/xlm/configuration_xlm.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     2981 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    59142 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlm/modeling_tf_xlm.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    53247 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlm/modeling_xlm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    34429 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlm/tokenization_xlm.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.691370 transformers-4.9.2/src/transformers/models/xlm_prophetnet/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1360 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/xlm_prophetnet/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1262 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7309 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    13840 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.691370 transformers-4.9.2/src/transformers/models/xlm_roberta/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3477 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlm_roberta/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2620 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlm_roberta/configuration_xlm_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6353 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5877 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/xlm_roberta/modeling_xlm_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14051 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlm_roberta/tokenization_xlm_roberta.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9965 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.691370 transformers-4.9.2/src/transformers/models/xlnet/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3421 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/models/xlnet/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11248 2021-06-28 07:40:59.000000 transformers-4.9.2/src/transformers/models/xlnet/configuration_xlnet.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)     3695 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    81280 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlnet/modeling_tf_xlnet.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    91661 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/models/xlnet/modeling_xlnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14406 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/models/xlnet/tokenization_xlnet.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9944 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/models/xlnet/tokenization_xlnet_fast.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.691370 transformers-4.9.2/src/transformers/onnx/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      843 2021-08-09 13:50:44.000000 transformers-4.9.2/src/transformers/onnx/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2884 2021-08-09 13:50:44.000000 transformers-4.9.2/src/transformers/onnx/__main__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    11662 2021-08-09 13:50:58.000000 transformers-4.9.2/src/transformers/onnx/config.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9370 2021-08-09 13:50:58.000000 transformers-4.9.2/src/transformers/onnx/convert.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5872 2021-08-09 13:52:07.000000 transformers-4.9.2/src/transformers/onnx/features.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1748 2021-08-09 13:50:58.000000 transformers-4.9.2/src/transformers/onnx/utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    27375 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/optimization.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15890 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/optimization_tf.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.694704 transformers-4.9.2/src/transformers/pipelines/
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)    24467 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/pipelines/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     6526 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/automatic_speech_recognition.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    30282 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/pipelines/base.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14841 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/conversational.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3684 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/pipelines/feature_extraction.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8780 2021-08-06 08:00:14.000000 transformers-4.9.2/src/transformers/pipelines/fill_mask.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     5155 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/image_classification.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    24463 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/question_answering.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14037 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/table_question_answering.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14756 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/text2text_generation.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3194 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/pipelines/text_classification.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8974 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/text_generation.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    19373 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/pipelines/token_classification.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8455 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/pipelines/zero_shot_classification.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.694704 transformers-4.9.2/src/transformers/sagemaker/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      901 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/sagemaker/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1044 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/sagemaker/trainer_sm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4926 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/sagemaker/training_args_sm.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    42812 2021-08-09 13:52:07.000000 transformers-4.9.2/src/transformers/testing_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    32397 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/tokenization_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)   165870 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/tokenization_utils_base.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    32188 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/tokenization_utils_fast.py
+-rwxr-xr-x   0 lysandre  (1000) lysandre  (1000)   126822 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/trainer.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    23488 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/trainer_callback.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    44264 2021-08-04 12:33:45.000000 transformers-4.9.2/src/transformers/trainer_pt_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     9744 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/trainer_seq2seq.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    34959 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/trainer_tf.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    15414 2021-08-04 12:34:04.000000 transformers-4.9.2/src/transformers/trainer_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    57088 2021-08-09 12:30:01.000000 transformers-4.9.2/src/transformers/training_args.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1754 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/training_args_seq2seq.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14909 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/training_args_tf.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.698037 transformers-4.9.2/src/transformers/utils/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1520 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/__init__.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1715 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/coco_classes.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    19181 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/dummy_flax_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    88488 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/dummy_pt_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      376 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/dummy_sentencepiece_and_speech_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      278 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/dummy_sentencepiece_and_tokenizers_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4089 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/dummy_sentencepiece_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      241 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/dummy_speech_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    47447 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/dummy_tf_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     1108 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/dummy_timm_and_vision_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      810 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/dummy_timm_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     8684 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/dummy_tokenizers_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)      916 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/dummy_vision_objects.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14869 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/fx.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4971 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/utils/hp_naming.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    33616 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/imagenet_classes.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     7701 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/logging.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     2186 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/utils/model_parallel_utils.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    16415 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/modeling_auto_mapping.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    14431 2021-08-09 14:23:38.000000 transformers-4.9.2/src/transformers/utils/notebook.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    39607 2021-07-12 07:26:47.000000 transformers-4.9.2/src/transformers/utils/sentencepiece_model_pb2.py
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     4381 2021-07-12 12:57:15.000000 transformers-4.9.2/src/transformers/utils/versions.py
+drwxr-xr-x   0 lysandre  (1000) lysandre  (1000)        0 2021-08-09 14:24:42.648037 transformers-4.9.2/src/transformers.egg-info/
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    43096 2021-08-09 14:24:42.000000 transformers-4.9.2/src/transformers.egg-info/PKG-INFO
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)    28294 2021-08-09 14:24:42.000000 transformers-4.9.2/src/transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)        1 2021-08-09 14:24:42.000000 transformers-4.9.2/src/transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)       82 2021-08-09 14:24:42.000000 transformers-4.9.2/src/transformers.egg-info/entry_points.txt
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)     3024 2021-08-09 14:24:42.000000 transformers-4.9.2/src/transformers.egg-info/requires.txt
+-rw-r--r--   0 lysandre  (1000) lysandre  (1000)       13 2021-08-09 14:24:42.000000 transformers-4.9.2/src/transformers.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `transformers-4.9.1/LICENSE` & `transformers-4.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/PKG-INFO` & `transformers-4.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers
-Version: 4.9.1
+Version: 4.9.2
 Summary: State-of-the-art Natural Language Processing for TensorFlow 2.0 and PyTorch
 Home-page: https://github.com/huggingface/transformers
 Author: Thomas Wolf, Lysandre Debut, Victor Sanh, Julien Chaumond, Sam Shleifer, Patrick von Platen, Sylvain Gugger, Suraj Patil, Stas Bekman, Google AI Language Team Authors, Open AI team Authors, Facebook AI Authors, Carnegie Mellon University Authors
 Author-email: thomas@huggingface.co
 License: Apache
 Description: <!---
         Copyright 2020 The HuggingFace Team. All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transformers Version: 4.9.1 Summary: State-of-the-
+Metadata-Version: 2.1 Name: transformers Version: 4.9.2 Summary: State-of-the-
 art Natural Language Processing for TensorFlow 2.0 and PyTorch Home-page:
 https://github.com/huggingface/transformers Author: Thomas Wolf, Lysandre
 Debut, Victor Sanh, Julien Chaumond, Sam Shleifer, Patrick von Platen, Sylvain
 Gugger, Suraj Patil, Stas Bekman, Google AI Language Team Authors, Open AI team
 Authors, Facebook AI Authors, Carnegie Mellon University Authors Author-email:
 thomas@huggingface.co License: Apache Description:
```

### Comparing `transformers-4.9.1/README.md` & `transformers-4.9.2/README.md`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/setup.cfg` & `transformers-4.9.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/setup.py` & `transformers-4.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
     deps["sacremoses"],  # for XLM
     deps["tokenizers"],
     deps["tqdm"],  # progress bars in model download and training scripts
 ]
 
 setup(
     name="transformers",
-    version="4.9.1",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
+    version="4.9.2",  # expected format is one of x.y.z.dev0, or x.y.z.rc1 or x.y.z (no to dashes, yes to dots)
     author="Thomas Wolf, Lysandre Debut, Victor Sanh, Julien Chaumond, Sam Shleifer, Patrick von Platen, Sylvain Gugger, Suraj Patil, Stas Bekman, Google AI Language Team Authors, Open AI team Authors, Facebook AI Authors, Carnegie Mellon University Authors",
     author_email="thomas@huggingface.co",
     description="State-of-the-art Natural Language Processing for TensorFlow 2.0 and PyTorch",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="NLP deep learning transformer pytorch tensorflow BERT GPT GPT-2 google openai CMU",
     license="Apache",
```

### Comparing `transformers-4.9.1/src/transformers/__init__.py` & `transformers-4.9.2/src/transformers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 # When adding a new object to this init, remember to add it twice: once inside the `_import_structure` dictionary and
 # once inside the `if TYPE_CHECKING` branch. The `TYPE_CHECKING` should have import statements as usual, but they are
 # only there for type checking. The `_import_structure` is a dictionary submodule to list of object names, and is used
 # to defer the actual importing for when the objects are requested. This way `import transformers` provides the names
 # in the namespace without actually importing anything (and especially none of the backends).
 
-__version__ = "4.9.1"
+__version__ = "4.9.2"
 
 # Work around to update TensorFlow's absl.logging threshold which alters the
 # default Python logging output behavior when present.
 # see: https://github.com/abseil/abseil-py/issues/99
 # and: https://github.com/tensorflow/tensorflow/issues/26691#issuecomment-500369493
 try:
     import absl.logging
```

### Comparing `transformers-4.9.1/src/transformers/activations.py` & `transformers-4.9.2/src/transformers/activations.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/activations_tf.py` & `transformers-4.9.2/src/transformers/activations_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/benchmark/benchmark.py` & `transformers-4.9.2/src/transformers/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/benchmark/benchmark_args.py` & `transformers-4.9.2/src/transformers/benchmark/benchmark_args.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/benchmark/benchmark_args_tf.py` & `transformers-4.9.2/src/transformers/benchmark/benchmark_args_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/benchmark/benchmark_args_utils.py` & `transformers-4.9.2/src/transformers/benchmark/benchmark_args_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/benchmark/benchmark_tf.py` & `transformers-4.9.2/src/transformers/benchmark/benchmark_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/benchmark/benchmark_utils.py` & `transformers-4.9.2/src/transformers/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/__init__.py` & `transformers-4.9.2/src/transformers/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/add_new_model.py` & `transformers-4.9.2/src/transformers/commands/add_new_model.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/convert.py` & `transformers-4.9.2/src/transformers/commands/convert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/download.py` & `transformers-4.9.2/src/transformers/commands/download.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/env.py` & `transformers-4.9.2/src/transformers/commands/env.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/lfs.py` & `transformers-4.9.2/src/transformers/commands/lfs.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/run.py` & `transformers-4.9.2/src/transformers/commands/run.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/serving.py` & `transformers-4.9.2/src/transformers/commands/serving.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/train.py` & `transformers-4.9.2/src/transformers/commands/train.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/transformers_cli.py` & `transformers-4.9.2/src/transformers/commands/transformers_cli.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/commands/user.py` & `transformers-4.9.2/src/transformers/commands/user.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/configuration_utils.py` & `transformers-4.9.2/src/transformers/configuration_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/convert_graph_to_onnx.py` & `transformers-4.9.2/src/transformers/convert_graph_to_onnx.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/convert_pytorch_checkpoint_to_tf2.py` & `transformers-4.9.2/src/transformers/convert_pytorch_checkpoint_to_tf2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/convert_slow_tokenizer.py` & `transformers-4.9.2/src/transformers/convert_slow_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/convert_slow_tokenizers_checkpoints_to_fast.py` & `transformers-4.9.2/src/transformers/convert_slow_tokenizers_checkpoints_to_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py` & `transformers-4.9.2/src/transformers/convert_tf_hub_seq_to_seq_bert_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/__init__.py` & `transformers-4.9.2/src/transformers/data/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/data_collator.py` & `transformers-4.9.2/src/transformers/data/data_collator.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/datasets/__init__.py` & `transformers-4.9.2/src/transformers/data/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/datasets/glue.py` & `transformers-4.9.2/src/transformers/data/datasets/glue.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/datasets/language_modeling.py` & `transformers-4.9.2/src/transformers/data/datasets/language_modeling.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/datasets/squad.py` & `transformers-4.9.2/src/transformers/data/datasets/squad.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/metrics/__init__.py` & `transformers-4.9.2/src/transformers/data/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/metrics/squad_metrics.py` & `transformers-4.9.2/src/transformers/data/metrics/squad_metrics.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/processors/__init__.py` & `transformers-4.9.2/src/transformers/data/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/processors/glue.py` & `transformers-4.9.2/src/transformers/data/processors/glue.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/processors/squad.py` & `transformers-4.9.2/src/transformers/data/processors/squad.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/processors/utils.py` & `transformers-4.9.2/src/transformers/data/processors/utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/processors/xnli.py` & `transformers-4.9.2/src/transformers/data/processors/xnli.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/data/test_generation_utils.py` & `transformers-4.9.2/src/transformers/data/test_generation_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/debug_utils.py` & `transformers-4.9.2/src/transformers/debug_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/deepspeed.py` & `transformers-4.9.2/src/transformers/deepspeed.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/dependency_versions_check.py` & `transformers-4.9.2/src/transformers/dependency_versions_check.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/dependency_versions_table.py` & `transformers-4.9.2/src/transformers/dependency_versions_table.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/feature_extraction_sequence_utils.py` & `transformers-4.9.2/src/transformers/feature_extraction_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/feature_extraction_utils.py` & `transformers-4.9.2/src/transformers/feature_extraction_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/file_utils.py` & `transformers-4.9.2/src/transformers/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,16 +270,17 @@
 HUGGINGFACE_CO_PREFIX = HUGGINGFACE_CO_RESOLVE_ENDPOINT + "/{model_id}/resolve/{revision}/{filename}"
 
 PRESET_MIRROR_DICT = {
     "tuna": "https://mirrors.tuna.tsinghua.edu.cn/hugging-face-models",
     "bfsu": "https://mirrors.bfsu.edu.cn/hugging-face-models",
 }
 
-# This is the version of torch required to run torch.fx features.
+# This is the version of torch required to run torch.fx features and torch.onnx with dictionary inputs.
 TORCH_FX_REQUIRED_VERSION = version.parse("1.8")
+TORCH_ONNX_DICT_INPUTS_MINIMUM_VERSION = version.parse("1.8")
 
 _is_offline_mode = True if os.environ.get("TRANSFORMERS_OFFLINE", "0").upper() in ENV_VARS_TRUE_VALUES else False
 
 
 def is_offline_mode():
     return _is_offline_mode
 
@@ -293,27 +294,33 @@
         import torch
 
         return torch.cuda.is_available()
     else:
         return False
 
 
-_torch_fx_available = False
+_torch_fx_available = _torch_onnx_dict_inputs_support_available = False
 if _torch_available:
     torch_version = version.parse(importlib_metadata.version("torch"))
     _torch_fx_available = (torch_version.major, torch_version.minor) == (
         TORCH_FX_REQUIRED_VERSION.major,
         TORCH_FX_REQUIRED_VERSION.minor,
     )
 
+    _torch_onnx_dict_inputs_support_available = torch_version >= TORCH_ONNX_DICT_INPUTS_MINIMUM_VERSION
+
 
 def is_torch_fx_available():
     return _torch_fx_available
 
 
+def is_torch_onnx_dict_inputs_support_available():
+    return _torch_onnx_dict_inputs_support_available
+
+
 def is_tf_available():
     return _tf_available
 
 
 def is_coloredlogs_available():
     return _coloredlogs_available
```

### Comparing `transformers-4.9.1/src/transformers/generation_beam_search.py` & `transformers-4.9.2/src/transformers/generation_beam_search.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/generation_flax_logits_process.py` & `transformers-4.9.2/src/transformers/generation_flax_logits_process.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/generation_flax_utils.py` & `transformers-4.9.2/src/transformers/generation_flax_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/generation_logits_process.py` & `transformers-4.9.2/src/transformers/generation_logits_process.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/generation_stopping_criteria.py` & `transformers-4.9.2/src/transformers/generation_stopping_criteria.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/generation_tf_utils.py` & `transformers-4.9.2/src/transformers/generation_tf_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/generation_utils.py` & `transformers-4.9.2/src/transformers/generation_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/hf_api.py` & `transformers-4.9.2/src/transformers/hf_api.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/hf_argparser.py` & `transformers-4.9.2/src/transformers/hf_argparser.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/image_utils.py` & `transformers-4.9.2/src/transformers/image_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/integrations.py` & `transformers-4.9.2/src/transformers/integrations.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modelcard.py` & `transformers-4.9.2/src/transformers/modelcard.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_flax_outputs.py` & `transformers-4.9.2/src/transformers/modeling_flax_outputs.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_flax_pytorch_utils.py` & `transformers-4.9.2/src/transformers/modeling_flax_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_flax_utils.py` & `transformers-4.9.2/src/transformers/modeling_flax_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_outputs.py` & `transformers-4.9.2/src/transformers/modeling_outputs.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_tf_outputs.py` & `transformers-4.9.2/src/transformers/modeling_tf_outputs.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_tf_pytorch_utils.py` & `transformers-4.9.2/src/transformers/modeling_tf_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_tf_utils.py` & `transformers-4.9.2/src/transformers/modeling_tf_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/modeling_utils.py` & `transformers-4.9.2/src/transformers/modeling_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -590,14 +590,18 @@
             self._tie_or_clone_weights(output_embeddings, self.get_input_embeddings())
 
         if self.config.is_encoder_decoder and self.config.tie_encoder_decoder:
             if hasattr(self, self.base_model_prefix):
                 self = getattr(self, self.base_model_prefix)
             self._tie_encoder_decoder_weights(self.encoder, self.decoder, self.base_model_prefix)
 
+        for module in self.modules():
+            if hasattr(module, "_tie_weights"):
+                module._tie_weights()
+
     @staticmethod
     def _tie_encoder_decoder_weights(encoder: nn.Module, decoder: nn.Module, base_model_prefix: str):
         uninitialized_encoder_weights: List[str] = []
         if decoder.__class__ != encoder.__class__:
             logger.info(
                 f"{decoder.__class__} and {encoder.__class__} are not equal. In this case make sure that all encoder weights are correctly initialized."
             )
```

### Comparing `transformers-4.9.1/src/transformers/models/__init__.py` & `transformers-4.9.2/src/transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/albert/__init__.py` & `transformers-4.9.2/src/transformers/models/albert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/albert/configuration_albert.py` & `transformers-4.9.2/src/transformers/models/albert/configuration_albert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/albert/convert_albert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/albert/modeling_albert.py` & `transformers-4.9.2/src/transformers/models/albert/modeling_albert.py`

 * *Files 0% similar despite different names*

```diff
@@ -856,28 +856,30 @@
         super().__init__()
 
         self.LayerNorm = nn.LayerNorm(config.embedding_size)
         self.bias = nn.Parameter(torch.zeros(config.vocab_size))
         self.dense = nn.Linear(config.hidden_size, config.embedding_size)
         self.decoder = nn.Linear(config.embedding_size, config.vocab_size)
         self.activation = ACT2FN[config.hidden_act]
-
-        # Need a link between the two variables so that the bias is correctly resized with `resize_token_embeddings`
         self.decoder.bias = self.bias
 
     def forward(self, hidden_states):
         hidden_states = self.dense(hidden_states)
         hidden_states = self.activation(hidden_states)
         hidden_states = self.LayerNorm(hidden_states)
         hidden_states = self.decoder(hidden_states)
 
         prediction_scores = hidden_states
 
         return prediction_scores
 
+    def _tie_weights(self):
+        # To tie those two weights if they get disconnected (on TPU or when the bias is resized)
+        self.bias = self.decoder.bias
+
 
 class AlbertSOPHead(nn.Module):
     def __init__(self, config):
         super().__init__()
 
         self.dropout = nn.Dropout(config.classifier_dropout_prob)
         self.classifier = nn.Linear(config.hidden_size, config.num_labels)
```

### Comparing `transformers-4.9.1/src/transformers/models/albert/modeling_tf_albert.py` & `transformers-4.9.2/src/transformers/models/albert/modeling_tf_albert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/albert/tokenization_albert.py` & `transformers-4.9.2/src/transformers/models/albert/tokenization_albert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/albert/tokenization_albert_fast.py` & `transformers-4.9.2/src/transformers/models/albert/tokenization_albert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/__init__.py` & `transformers-4.9.2/src/transformers/models/auto/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/auto_factory.py` & `transformers-4.9.2/src/transformers/models/auto/auto_factory.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/configuration_auto.py` & `transformers-4.9.2/src/transformers/models/auto/configuration_auto.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/feature_extraction_auto.py` & `transformers-4.9.2/src/transformers/models/auto/feature_extraction_auto.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/modeling_auto.py` & `transformers-4.9.2/src/transformers/models/auto/modeling_auto.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/modeling_flax_auto.py` & `transformers-4.9.2/src/transformers/models/auto/modeling_flax_auto.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/modeling_tf_auto.py` & `transformers-4.9.2/src/transformers/models/auto/modeling_tf_auto.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/auto/tokenization_auto.py` & `transformers-4.9.2/src/transformers/models/auto/tokenization_auto.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/__init__.py` & `transformers-4.9.2/src/transformers/models/bart/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/configuration_bart.py` & `transformers-4.9.2/src/transformers/models/bart/configuration_bart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/bart/convert_bart_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/modeling_bart.py` & `transformers-4.9.2/src/transformers/models/bart/modeling_bart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/modeling_flax_bart.py` & `transformers-4.9.2/src/transformers/models/bart/modeling_flax_bart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/modeling_tf_bart.py` & `transformers-4.9.2/src/transformers/models/bart/modeling_tf_bart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/tokenization_bart.py` & `transformers-4.9.2/src/transformers/models/bart/tokenization_bart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bart/tokenization_bart_fast.py` & `transformers-4.9.2/src/transformers/models/bart/tokenization_bart_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/barthez/__init__.py` & `transformers-4.9.2/src/transformers/models/barthez/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/barthez/tokenization_barthez.py` & `transformers-4.9.2/src/transformers/models/barthez/tokenization_barthez.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/barthez/tokenization_barthez_fast.py` & `transformers-4.9.2/src/transformers/models/barthez/tokenization_barthez_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/__init__.py` & `transformers-4.9.2/src/transformers/models/bert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/configuration_bert.py` & `transformers-4.9.2/src/transformers/models/bert/configuration_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/bert/convert_bert_original_tf2_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/bert/convert_bert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py` & `transformers-4.9.2/src/transformers/models/bert/convert_bert_pytorch_checkpoint_to_original_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/modeling_bert.py` & `transformers-4.9.2/src/transformers/models/bert/modeling_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/modeling_flax_bert.py` & `transformers-4.9.2/src/transformers/models/bert/modeling_flax_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/modeling_tf_bert.py` & `transformers-4.9.2/src/transformers/models/bert/modeling_tf_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/tokenization_bert.py` & `transformers-4.9.2/src/transformers/models/bert/tokenization_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert/tokenization_bert_fast.py` & `transformers-4.9.2/src/transformers/models/bert/tokenization_bert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert_generation/__init__.py` & `transformers-4.9.2/src/transformers/models/bert_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert_generation/configuration_bert_generation.py` & `transformers-4.9.2/src/transformers/models/bert_generation/configuration_bert_generation.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert_generation/modeling_bert_generation.py` & `transformers-4.9.2/src/transformers/models/bert_generation/modeling_bert_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -426,24 +426,26 @@
             cross_attentions=encoder_outputs.cross_attentions,
         )
 
 
 class BertGenerationOnlyLMHead(nn.Module):
     def __init__(self, config):
         super().__init__()
-        self.decoder = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
+        self.decoder = nn.Linear(config.hidden_size, config.vocab_size)
         self.bias = nn.Parameter(torch.zeros(config.vocab_size))
-
-        # Need a link between the two variables so that the bias is correctly resized with `resize_token_embeddings`
         self.decoder.bias = self.bias
 
     def forward(self, hidden_states):
         logits = self.decoder(hidden_states)
         return logits
 
+    def _tie_weights(self):
+        # To tie those two weights if they get disconnected (on TPU or when the bias is resized)
+        self.bias = self.decoder.bias
+
 
 @add_start_docstrings(
     """BertGeneration Model with a `language modeling` head on top for CLM fine-tuning. """,
     BERT_GENERATION_START_DOCSTRING,
 )
 class BertGenerationDecoder(BertGenerationPreTrainedModel):
     def __init__(self, config):
```

### Comparing `transformers-4.9.1/src/transformers/models/bert_generation/tokenization_bert_generation.py` & `transformers-4.9.2/src/transformers/models/bert_generation/tokenization_bert_generation.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert_japanese/__init__.py` & `transformers-4.9.2/src/transformers/models/bert_japanese/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bert_japanese/tokenization_bert_japanese.py` & `transformers-4.9.2/src/transformers/models/bert_japanese/tokenization_bert_japanese.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bertweet/__init__.py` & `transformers-4.9.2/src/transformers/models/bertweet/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bertweet/tokenization_bertweet.py` & `transformers-4.9.2/src/transformers/models/bertweet/tokenization_bertweet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/__init__.py` & `transformers-4.9.2/src/transformers/models/big_bird/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/configuration_big_bird.py` & `transformers-4.9.2/src/transformers/models/big_bird/configuration_big_bird.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/big_bird/convert_bigbird_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/modeling_big_bird.py` & `transformers-4.9.2/src/transformers/models/big_bird/modeling_big_bird.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/modeling_flax_big_bird.py` & `transformers-4.9.2/src/transformers/models/big_bird/modeling_flax_big_bird.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/tokenization_big_bird.py` & `transformers-4.9.2/src/transformers/models/big_bird/tokenization_big_bird.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/big_bird/tokenization_big_bird_fast.py` & `transformers-4.9.2/src/transformers/models/big_bird/tokenization_big_bird_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bigbird_pegasus/__init__.py` & `transformers-4.9.2/src/transformers/models/bigbird_pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py` & `transformers-4.9.2/src/transformers/models/bigbird_pegasus/configuration_bigbird_pegasus.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/bigbird_pegasus/convert_bigbird_pegasus_tf_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py` & `transformers-4.9.2/src/transformers/models/bigbird_pegasus/modeling_bigbird_pegasus.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot/__init__.py` & `transformers-4.9.2/src/transformers/models/blenderbot/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot/configuration_blenderbot.py` & `transformers-4.9.2/src/transformers/models/blenderbot/configuration_blenderbot.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/blenderbot/convert_blenderbot_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot/modeling_blenderbot.py` & `transformers-4.9.2/src/transformers/models/blenderbot/modeling_blenderbot.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot/modeling_tf_blenderbot.py` & `transformers-4.9.2/src/transformers/models/blenderbot/modeling_tf_blenderbot.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot/tokenization_blenderbot.py` & `transformers-4.9.2/src/transformers/models/blenderbot/tokenization_blenderbot.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot_small/__init__.py` & `transformers-4.9.2/src/transformers/models/blenderbot_small/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot_small/configuration_blenderbot_small.py` & `transformers-4.9.2/src/transformers/models/blenderbot_small/configuration_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot_small/modeling_blenderbot_small.py` & `transformers-4.9.2/src/transformers/models/blenderbot_small/modeling_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py` & `transformers-4.9.2/src/transformers/models/blenderbot_small/modeling_tf_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot_small/tokenization_blenderbot_small.py` & `transformers-4.9.2/src/transformers/models/blenderbot_small/tokenization_blenderbot_small.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py` & `transformers-4.9.2/src/transformers/models/blenderbot_small/tokenization_blenderbot_small_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/byt5/__init__.py` & `transformers-4.9.2/src/transformers/models/byt5/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/byt5/convert_byt5_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/byt5/tokenization_byt5.py` & `transformers-4.9.2/src/transformers/models/byt5/tokenization_byt5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/camembert/__init__.py` & `transformers-4.9.2/src/transformers/models/camembert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/camembert/configuration_camembert.py` & `transformers-4.9.2/src/transformers/models/camembert/configuration_camembert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/camembert/modeling_camembert.py` & `transformers-4.9.2/src/transformers/models/camembert/modeling_camembert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/camembert/modeling_tf_camembert.py` & `transformers-4.9.2/src/transformers/models/camembert/modeling_tf_camembert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/camembert/tokenization_camembert.py` & `transformers-4.9.2/src/transformers/models/camembert/tokenization_camembert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/camembert/tokenization_camembert_fast.py` & `transformers-4.9.2/src/transformers/models/camembert/tokenization_camembert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/canine/__init__.py` & `transformers-4.9.2/src/transformers/models/canine/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/canine/configuration_canine.py` & `transformers-4.9.2/src/transformers/models/canine/configuration_canine.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/canine/convert_canine_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/canine/modeling_canine.py` & `transformers-4.9.2/src/transformers/models/canine/modeling_canine.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/canine/tokenization_canine.py` & `transformers-4.9.2/src/transformers/models/canine/tokenization_canine.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/__init__.py` & `transformers-4.9.2/src/transformers/models/clip/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/configuration_clip.py` & `transformers-4.9.2/src/transformers/models/clip/configuration_clip.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/convert_clip_original_pytorch_to_hf.py` & `transformers-4.9.2/src/transformers/models/clip/convert_clip_original_pytorch_to_hf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/feature_extraction_clip.py` & `transformers-4.9.2/src/transformers/models/clip/feature_extraction_clip.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/modeling_clip.py` & `transformers-4.9.2/src/transformers/models/clip/modeling_clip.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/modeling_flax_clip.py` & `transformers-4.9.2/src/transformers/models/clip/modeling_flax_clip.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/processing_clip.py` & `transformers-4.9.2/src/transformers/models/clip/processing_clip.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/tokenization_clip.py` & `transformers-4.9.2/src/transformers/models/clip/tokenization_clip.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/clip/tokenization_clip_fast.py` & `transformers-4.9.2/src/transformers/models/clip/tokenization_clip_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/__init__.py` & `transformers-4.9.2/src/transformers/models/convbert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/configuration_convbert.py` & `transformers-4.9.2/src/transformers/models/convbert/configuration_convbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py` & `transformers-4.9.2/src/transformers/models/convbert/convert_convbert_original_tf1_checkpoint_to_pytorch_and_tf2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/modeling_convbert.py` & `transformers-4.9.2/src/transformers/models/convbert/modeling_convbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/modeling_tf_convbert.py` & `transformers-4.9.2/src/transformers/models/convbert/modeling_tf_convbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/tokenization_convbert.py` & `transformers-4.9.2/src/transformers/models/convbert/tokenization_convbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/convbert/tokenization_convbert_fast.py` & `transformers-4.9.2/src/transformers/models/convbert/tokenization_convbert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/cpm/__init__.py` & `transformers-4.9.2/src/transformers/models/cpm/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/cpm/tokenization_cpm.py` & `transformers-4.9.2/src/transformers/models/cpm/tokenization_cpm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ctrl/__init__.py` & `transformers-4.9.2/src/transformers/models/ctrl/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ctrl/configuration_ctrl.py` & `transformers-4.9.2/src/transformers/models/ctrl/configuration_ctrl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ctrl/modeling_ctrl.py` & `transformers-4.9.2/src/transformers/models/ctrl/modeling_ctrl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ctrl/modeling_tf_ctrl.py` & `transformers-4.9.2/src/transformers/models/ctrl/modeling_tf_ctrl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ctrl/tokenization_ctrl.py` & `transformers-4.9.2/src/transformers/models/ctrl/tokenization_ctrl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta/__init__.py` & `transformers-4.9.2/src/transformers/models/deberta/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta/configuration_deberta.py` & `transformers-4.9.2/src/transformers/models/deberta/configuration_deberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta/modeling_deberta.py` & `transformers-4.9.2/src/transformers/models/deberta/modeling_deberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta/tokenization_deberta.py` & `transformers-4.9.2/src/transformers/models/deberta/tokenization_deberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta/tokenization_deberta_fast.py` & `transformers-4.9.2/src/transformers/models/deberta/tokenization_deberta_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta_v2/__init__.py` & `transformers-4.9.2/src/transformers/models/deberta_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta_v2/configuration_deberta_v2.py` & `transformers-4.9.2/src/transformers/models/deberta_v2/configuration_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta_v2/modeling_deberta_v2.py` & `transformers-4.9.2/src/transformers/models/deberta_v2/modeling_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deberta_v2/tokenization_deberta_v2.py` & `transformers-4.9.2/src/transformers/models/deberta_v2/tokenization_deberta_v2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deit/__init__.py` & `transformers-4.9.2/src/transformers/models/deit/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deit/configuration_deit.py` & `transformers-4.9.2/src/transformers/models/deit/configuration_deit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deit/convert_deit_timm_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/deit/convert_deit_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deit/feature_extraction_deit.py` & `transformers-4.9.2/src/transformers/models/deit/feature_extraction_deit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/deit/modeling_deit.py` & `transformers-4.9.2/src/transformers/models/deit/modeling_deit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/detr/__init__.py` & `transformers-4.9.2/src/transformers/models/detr/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/detr/configuration_detr.py` & `transformers-4.9.2/src/transformers/models/detr/configuration_detr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/detr/convert_detr_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/detr/feature_extraction_detr.py` & `transformers-4.9.2/src/transformers/models/detr/feature_extraction_detr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/detr/modeling_detr.py` & `transformers-4.9.2/src/transformers/models/detr/modeling_detr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/dialogpt/convert_dialogpt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/distilbert/__init__.py` & `transformers-4.9.2/src/transformers/models/distilbert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/distilbert/configuration_distilbert.py` & `transformers-4.9.2/src/transformers/models/distilbert/configuration_distilbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/distilbert/modeling_distilbert.py` & `transformers-4.9.2/src/transformers/models/distilbert/modeling_distilbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/distilbert/modeling_tf_distilbert.py` & `transformers-4.9.2/src/transformers/models/distilbert/modeling_tf_distilbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/distilbert/tokenization_distilbert.py` & `transformers-4.9.2/src/transformers/models/distilbert/tokenization_distilbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/distilbert/tokenization_distilbert_fast.py` & `transformers-4.9.2/src/transformers/models/distilbert/tokenization_distilbert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/__init__.py` & `transformers-4.9.2/src/transformers/models/dpr/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/configuration_dpr.py` & `transformers-4.9.2/src/transformers/models/dpr/configuration_dpr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/dpr/convert_dpr_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/modeling_dpr.py` & `transformers-4.9.2/src/transformers/models/dpr/modeling_dpr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/modeling_tf_dpr.py` & `transformers-4.9.2/src/transformers/models/dpr/modeling_tf_dpr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/tokenization_dpr.py` & `transformers-4.9.2/src/transformers/models/dpr/tokenization_dpr.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/dpr/tokenization_dpr_fast.py` & `transformers-4.9.2/src/transformers/models/dpr/tokenization_dpr_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/__init__.py` & `transformers-4.9.2/src/transformers/models/electra/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/configuration_electra.py` & `transformers-4.9.2/src/transformers/models/electra/configuration_electra.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/electra/convert_electra_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/modeling_electra.py` & `transformers-4.9.2/src/transformers/models/electra/modeling_electra.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/modeling_flax_electra.py` & `transformers-4.9.2/src/transformers/models/electra/modeling_flax_electra.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/modeling_tf_electra.py` & `transformers-4.9.2/src/transformers/models/electra/modeling_tf_electra.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/tokenization_electra.py` & `transformers-4.9.2/src/transformers/models/electra/tokenization_electra.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/electra/tokenization_electra_fast.py` & `transformers-4.9.2/src/transformers/models/electra/tokenization_electra_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/encoder_decoder/__init__.py` & `transformers-4.9.2/src/transformers/models/encoder_decoder/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/encoder_decoder/configuration_encoder_decoder.py` & `transformers-4.9.2/src/transformers/models/encoder_decoder/configuration_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/encoder_decoder/modeling_encoder_decoder.py` & `transformers-4.9.2/src/transformers/models/encoder_decoder/modeling_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/flaubert/__init__.py` & `transformers-4.9.2/src/transformers/models/flaubert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/flaubert/configuration_flaubert.py` & `transformers-4.9.2/src/transformers/models/flaubert/configuration_flaubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/flaubert/modeling_flaubert.py` & `transformers-4.9.2/src/transformers/models/flaubert/modeling_flaubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/flaubert/modeling_tf_flaubert.py` & `transformers-4.9.2/src/transformers/models/flaubert/modeling_tf_flaubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/flaubert/tokenization_flaubert.py` & `transformers-4.9.2/src/transformers/models/flaubert/tokenization_flaubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/fsmt/__init__.py` & `transformers-4.9.2/src/transformers/models/fsmt/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/fsmt/configuration_fsmt.py` & `transformers-4.9.2/src/transformers/models/fsmt/configuration_fsmt.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/fsmt/convert_fsmt_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/fsmt/modeling_fsmt.py` & `transformers-4.9.2/src/transformers/models/fsmt/modeling_fsmt.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/fsmt/tokenization_fsmt.py` & `transformers-4.9.2/src/transformers/models/fsmt/tokenization_fsmt.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/__init__.py` & `transformers-4.9.2/src/transformers/models/funnel/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/configuration_funnel.py` & `transformers-4.9.2/src/transformers/models/funnel/configuration_funnel.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/funnel/convert_funnel_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/modeling_funnel.py` & `transformers-4.9.2/src/transformers/models/funnel/modeling_funnel.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/modeling_tf_funnel.py` & `transformers-4.9.2/src/transformers/models/funnel/modeling_tf_funnel.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/tokenization_funnel.py` & `transformers-4.9.2/src/transformers/models/funnel/tokenization_funnel.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/funnel/tokenization_funnel_fast.py` & `transformers-4.9.2/src/transformers/models/funnel/tokenization_funnel_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/__init__.py` & `transformers-4.9.2/src/transformers/models/gpt2/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/configuration_gpt2.py` & `transformers-4.9.2/src/transformers/models/gpt2/configuration_gpt2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/gpt2/convert_gpt2_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/modeling_flax_gpt2.py` & `transformers-4.9.2/src/transformers/models/gpt2/modeling_flax_gpt2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/modeling_gpt2.py` & `transformers-4.9.2/src/transformers/models/gpt2/modeling_gpt2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/modeling_tf_gpt2.py` & `transformers-4.9.2/src/transformers/models/gpt2/modeling_tf_gpt2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/tokenization_gpt2.py` & `transformers-4.9.2/src/transformers/models/gpt2/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt2/tokenization_gpt2_fast.py` & `transformers-4.9.2/src/transformers/models/gpt2/tokenization_gpt2_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt_neo/__init__.py` & `transformers-4.9.2/src/transformers/models/gpt_neo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 # limitations under the License.
 from typing import TYPE_CHECKING
 
 from ...file_utils import _LazyModule, is_flax_available, is_torch_available
 
 
 _import_structure = {
-    "configuration_gpt_neo": ["GPT_NEO_PRETRAINED_CONFIG_ARCHIVE_MAP", "GPTNeoConfig"],
+    "configuration_gpt_neo": ["GPT_NEO_PRETRAINED_CONFIG_ARCHIVE_MAP", "GPTNeoConfig", "GPTNeoOnnxConfig"],
 }
 
 if is_torch_available():
     _import_structure["modeling_gpt_neo"] = [
         "GPT_NEO_PRETRAINED_MODEL_ARCHIVE_LIST",
         "GPTNeoForCausalLM",
         "GPTNeoForSequenceClassification",
@@ -39,15 +39,15 @@
         "FlaxGPTNeoForCausalLM",
         "FlaxGPTNeoModel",
         "FlaxGPTNeoPreTrainedModel",
     ]
 
 
 if TYPE_CHECKING:
-    from .configuration_gpt_neo import GPT_NEO_PRETRAINED_CONFIG_ARCHIVE_MAP, GPTNeoConfig
+    from .configuration_gpt_neo import GPT_NEO_PRETRAINED_CONFIG_ARCHIVE_MAP, GPTNeoConfig, GPTNeoOnnxConfig
 
     if is_torch_available():
         from .modeling_gpt_neo import (
             GPT_NEO_PRETRAINED_MODEL_ARCHIVE_LIST,
             GPTNeoForCausalLM,
             GPTNeoForSequenceClassification,
             GPTNeoModel,
```

### Comparing `transformers-4.9.1/src/transformers/models/gpt_neo/configuration_gpt_neo.py` & `transformers-4.9.2/src/transformers/models/openai/configuration_openai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,175 +1,176 @@
 # coding=utf-8
-# Copyright 2021 The HuggingFace Inc. team. All rights reserved.
+# Copyright 2018 The OpenAI Team Authors and HuggingFace Inc. team.
+# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" GPT Neo model configuration """
+""" OpenAI GPT configuration """
 
 from ...configuration_utils import PretrainedConfig
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)
 
-GPT_NEO_PRETRAINED_CONFIG_ARCHIVE_MAP = {
-    "EleutherAI/gpt-neo-1.3B": "https://huggingface.co/EleutherAI/gpt-neo-1.3B/resolve/main/config.json",
-    # See all GPTNeo models at https://huggingface.co/models?filter=gpt_neo
-}
+OPENAI_GPT_PRETRAINED_CONFIG_ARCHIVE_MAP = {"openai-gpt": "https://huggingface.co/openai-gpt/resolve/main/config.json"}
 
 
-class GPTNeoConfig(PretrainedConfig):
-    r"""
-    This is the configuration class to store the configuration of a :class:`~transformers.GPTNeoModel`. It is used to
-    instantiate a GPT Neo model according to the specified arguments, defining the model architecture. Instantiating a
-    configuration with the defaults will yield a similar configuration to that of the GPTNeo `gpt-neo-1.3B
-    <https://huggingface.co/EleutherAI/gpt-neo-1.3B>`__ architecture.
+class OpenAIGPTConfig(PretrainedConfig):
+    """
+    This is the configuration class to store the configuration of a :class:`~transformers.OpenAIGPTModel` or a
+    :class:`~transformers.TFOpenAIGPTModel`. It is used to instantiate a GPT model according to the specified
+    arguments, defining the model architecture. Instantiating a configuration with the defaults will yield a similar
+    configuration to that of the `GPT <https://huggingface.co/openai-gpt>`__ architecture from OpenAI.
 
     Configuration objects inherit from :class:`~transformers.PretrainedConfig` and can be used to control the model
     outputs. Read the documentation from :class:`~transformers.PretrainedConfig` for more information.
 
-
     Args:
-        vocab_size (:obj:`int`, `optional`, defaults to 50257):
-            Vocabulary size of the GPT Neo model. Defines the number of different tokens that can be represented by the
-            :obj:`inputs_ids` passed when calling :class:`~transformers.GPTNeoModel`. Vocabulary size of the model.
-            Defines the different tokens that can be represented by the `inputs_ids` passed to the forward method of
-            :class:`~transformers.GPTNeoModel`.
-        attention_types (:obj:`List`, `optional`, defaults to :obj:`[[["global", "local"], 12]]`):
-            The type of attention for each layer in a :obj:`List` of the following format :obj:`[[["attention_type"],
-            num_layerss]]` e.g. for a 24 layer model :obj:`[[["global"], 24]]` or :obj:`[[["global", "local"], 12]]`
-            Choose the value of ``attention_type`` from :obj:`["global", "local"]`
-        hidden_size (:obj:`int`, `optional`, defaults to 2048):
-            Dimensionality of the encoder layers and the pooler layer.
-        num_layers (:obj:`int`, `optional`, defaults to 24):
+        vocab_size (:obj:`int`, `optional`, defaults to 40478):
+            Vocabulary size of the GPT-2 model. Defines the number of different tokens that can be represented by the
+            :obj:`inputs_ids` passed when calling :class:`~transformers.OpenAIGPTModel` or
+            :class:`~transformers.TFOpenAIGPTModel`.
+        n_positions (:obj:`int`, `optional`, defaults to 512):
+            The maximum sequence length that this model might ever be used with. Typically set this to something large
+            just in case (e.g., 512 or 1024 or 2048).
+        n_ctx (:obj:`int`, `optional`, defaults to 512):
+            Dimensionality of the causal mask (usually same as n_positions).
+        n_embd (:obj:`int`, `optional`, defaults to 768):
+            Dimensionality of the embeddings and hidden states.
+        n_layer (:obj:`int`, `optional`, defaults to 12):
             Number of hidden layers in the Transformer encoder.
-        num_heads (:obj:`int`, `optional`, defaults to 16):
+        n_head (:obj:`int`, `optional`, defaults to 12):
             Number of attention heads for each attention layer in the Transformer encoder.
-        intermediate_size (:obj:`int`, `optional`, defaults to 8192):
-            Dimensionality of the "intermediate" (i.e., feed-forward) layer in the Transformer encoder.
-        activation_function (:obj:`str` or :obj:`function`, `optional`, defaults to :obj:`"gelu_new"`):
+        afn (:obj:`str` or :obj:`Callable`, `optional`, defaults to :obj:`"gelu"`):
             The non-linear activation function (function or string) in the encoder and pooler. If string,
-            :obj:`"gelu"`, :obj:`"relu"`, :obj:`"selu"` and :obj:`"gelu_new"` are supported.
-        embed_dropout (:obj:`float`, `optional`, defaults to 0.0):
-            The dropout probabilitiy for all fully connected layers in the embeddings, encoder, and pooler.
-        attention_dropout (:obj:`float`, `optional`, defaults to 0.0):
-            The dropout ratio for the attention probabilities.
-        max_position_embeddings (:obj:`int`, `optional`, defaults to 2048):
-            The maximum sequence length that this model might ever be used with. Typically set this to something large
-            just in case (e.g., 512 or 1024 or 2048).
-        type_vocab_size (:obj:`int`, `optional`, defaults to 2):
-            The vocabulary size of the :obj:`token_type_ids` passed when calling :class:`~transformers.GPTNeoModel`.
+            :obj:`"gelu"`, :obj:`"relu"`, :obj:`"silu"` and :obj:`"gelu_new"` are supported.
+        resid_pdrop (:obj:`float`, `optional`, defaults to 0.1):
+            The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
+        embd_pdrop (:obj:`int`, `optional`, defaults to 0.1):
+            The dropout ratio for the embeddings.
+        attn_pdrop (:obj:`float`, `optional`, defaults to 0.1):
+            The dropout ratio for the attention.
+        layer_norm_epsilon (:obj:`float`, `optional`, defaults to 1e-5):
+            The epsilon to use in the layer normalization layers
         initializer_range (:obj:`float`, `optional`, defaults to 0.02):
             The standard deviation of the truncated_normal_initializer for initializing all weight matrices.
-        layer_norm_epsilon (:obj:`float`, `optional`, defaults to 1e-5):
-            The epsilon used by the layer normalization layers.
+        predict_special_tokens (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Whether or not special tokens should be predicted when the model has a language modeling head.
+        summary_type (:obj:`str`, `optional`, defaults to :obj:`"cls_index"`):
+            Argument used when doing sequence summary, used in the models
+            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+
+            Has to be one of the following options:
+
+                - :obj:`"last"`: Take the last token hidden state (like XLNet).
+                - :obj:`"first"`: Take the first token hidden state (like BERT).
+                - :obj:`"mean"`: Take the mean of all tokens hidden states.
+                - :obj:`"cls_index"`: Supply a Tensor of classification token position (like GPT/GPT-2).
+                - :obj:`"attn"`: Not implemented now, use multi-head attention.
+        summary_use_proj (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Argument used when doing sequence summary, used in the models
+            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+
+            Whether or not to add a projection after the vector extraction.
+        summary_activation (:obj:`str`, `optional`):
+            Argument used when doing sequence summary, used in the models
+            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+
+            Pass :obj:`"tanh"` for a tanh activation to the output, any other value will result in no activation.
+        summary_proj_to_labels (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Argument used when doing sequence summary, used in the models
+            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+
+            Whether the projection outputs should have :obj:`config.num_labels` or :obj:`config.hidden_size` classes.
+        summary_first_dropout (:obj:`float`, `optional`, defaults to 0.1):
+            Argument used when doing sequence summary, used in the models
+            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+
+            The dropout ratio to be used after the projection and activation.
         use_cache (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Whether or not the model should return the last key/values attentions (not used by all models). Only
-            relevant if ``config.is_decoder=True``.
-        gradient_checkpointing (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            If True, use gradient checkpointing to save memory at the expense of slower backward pass.
+            Whether or not the model should return the last key/values attentions (not used by all models).
 
-        Example::
 
-            >>> from transformers import GPTNeoModel, GPTNeoConfig
+    Examples::
 
-            >>> # Initializing a GPTNeo EleutherAI/gpt-neo-1.3B style configuration
-            >>> configuration = GPTNeoConfig()
+        >>> from transformers import OpenAIGPTConfig, OpenAIGPTModel
 
-            >>> # Initializing a model from the EleutherAI/gpt-neo-1.3B style configuration
-            >>> model = GPTNeoModel(configuration)
+        >>> # Initializing a GPT configuration
+        >>> configuration = OpenAIGPTConfig()
 
-            >>> # Accessing the model configuration
-            >>> configuration = model.config
+        >>> # Initializing a model from the configuration
+        >>> model = OpenAIGPTModel(configuration)
+
+        >>> # Accessing the model configuration
+        >>> configuration = model.config
     """
-    model_type = "gpt_neo"
+
+    model_type = "openai-gpt"
 
     def __init__(
         self,
-        vocab_size=50257,
-        max_position_embeddings=2048,
-        hidden_size=2048,
-        num_layers=24,
-        attention_types=[[["global", "local"], 12]],
-        num_heads=16,
-        intermediate_size=None,
-        window_size=256,
-        activation_function="gelu_new",
-        resid_dropout=0.0,
-        embed_dropout=0.0,
-        attention_dropout=0.0,
+        vocab_size=40478,
+        n_positions=512,
+        n_ctx=512,
+        n_embd=768,
+        n_layer=12,
+        n_head=12,
+        afn="gelu",
+        resid_pdrop=0.1,
+        embd_pdrop=0.1,
+        attn_pdrop=0.1,
         layer_norm_epsilon=1e-5,
         initializer_range=0.02,
+        predict_special_tokens=True,
         summary_type="cls_index",
         summary_use_proj=True,
         summary_activation=None,
         summary_proj_to_labels=True,
         summary_first_dropout=0.1,
-        gradient_checkpointing=False,
-        use_cache=True,
-        bos_token_id=50256,
-        eos_token_id=50256,
         **kwargs
     ):
-        super().__init__(bos_token_id=bos_token_id, eos_token_id=eos_token_id, **kwargs)
+        super().__init__(**kwargs)
 
         self.vocab_size = vocab_size
-        self.max_position_embeddings = max_position_embeddings
-        self.hidden_size = hidden_size
-        self.num_layers = num_layers
-        self.num_heads = num_heads
-        self.intermediate_size = intermediate_size
-        self.window_size = window_size
-        self.activation_function = activation_function
-        self.resid_dropout = resid_dropout
-        self.embed_dropout = embed_dropout
-        self.attention_dropout = attention_dropout
+        self.n_ctx = n_ctx
+        self.n_positions = n_positions
+        self.n_embd = n_embd
+        self.n_layer = n_layer
+        self.n_head = n_head
+        self.afn = afn
+        self.resid_pdrop = resid_pdrop
+        self.embd_pdrop = embd_pdrop
+        self.attn_pdrop = attn_pdrop
         self.layer_norm_epsilon = layer_norm_epsilon
         self.initializer_range = initializer_range
+        self.predict_special_tokens = predict_special_tokens
         self.summary_type = summary_type
         self.summary_use_proj = summary_use_proj
         self.summary_activation = summary_activation
         self.summary_first_dropout = summary_first_dropout
         self.summary_proj_to_labels = summary_proj_to_labels
-        self.gradient_checkpointing = gradient_checkpointing
-        self.use_cache = use_cache
 
-        self.bos_token_id = bos_token_id
-        self.eos_token_id = eos_token_id
-
-        self.attention_types = attention_types
-        self.attention_layers = self.expand_attention_types_params(attention_types)
+    @property
+    def max_position_embeddings(self):
+        return self.n_positions
 
-        if len(self.attention_layers) != self.num_layers:
-            raise ValueError(
-                "Configuration for convolutional module is incorrect."
-                "It is required that `len(config.attention_layers)` == `config.num_layers`"
-                f"but is `len(config.attention_layers) = {len(self.attention_layers)}`,"
-                f"`config.num_layers = {self.num_layers}`."
-                "`config.attention_layers` is prepared using `config.attention_types`."
-                "Please verify the value of `config.attention_types` argument."
-            )
-
-    @staticmethod
-    def expand_attention_types_params(attention_types):
-        attentions = []
-        for item in attention_types:
-            for _ in range(item[1]):
-                attentions.extend(item[0])
-        return attentions
+    @property
+    def hidden_size(self):
+        return self.n_embd
 
     @property
     def num_attention_heads(self):
-        return self.num_heads
+        return self.n_head
 
     @property
     def num_hidden_layers(self):
-        return self.num_layers
+        return self.n_layer
```

### Comparing `transformers-4.9.1/src/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/gpt_neo/convert_gpt_neo_mesh_tf_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt_neo/modeling_flax_gpt_neo.py` & `transformers-4.9.2/src/transformers/models/gpt_neo/modeling_flax_gpt_neo.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/gpt_neo/modeling_gpt_neo.py` & `transformers-4.9.2/src/transformers/models/gpt_neo/modeling_gpt_neo.py`

 * *Files 0% similar despite different names*

```diff
@@ -1117,15 +1117,15 @@
             else:
                 sequence_lengths = -1
                 logger.warning(
                     f"{self.__class__.__name__} will not detect padding tokens in `inputs_embeds`. Results may be "
                     f"unexpected if using padding tokens in conjunction with `inputs_embeds.`"
                 )
 
-        pooled_logits = logits[range(batch_size), sequence_lengths]
+        pooled_logits = logits[torch.arange(batch_size), sequence_lengths]
 
         loss = None
         if labels is not None:
             if self.num_labels == 1:
                 #  We are doing regression
                 loss_fct = MSELoss()
                 loss = loss_fct(pooled_logits.view(-1), labels.to(self.dtype).view(-1))
```

### Comparing `transformers-4.9.1/src/transformers/models/herbert/__init__.py` & `transformers-4.9.2/src/transformers/models/herbert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/herbert/tokenization_herbert.py` & `transformers-4.9.2/src/transformers/models/herbert/tokenization_herbert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/herbert/tokenization_herbert_fast.py` & `transformers-4.9.2/src/transformers/models/herbert/tokenization_herbert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/hubert/__init__.py` & `transformers-4.9.2/src/transformers/models/hubert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/hubert/configuration_hubert.py` & `transformers-4.9.2/src/transformers/models/hubert/configuration_hubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/hubert/convert_hubert_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/hubert/modeling_hubert.py` & `transformers-4.9.2/src/transformers/models/hubert/modeling_hubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/hubert/modeling_tf_hubert.py` & `transformers-4.9.2/src/transformers/models/hubert/modeling_tf_hubert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ibert/__init__.py` & `transformers-4.9.2/src/transformers/models/ibert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ibert/configuration_ibert.py` & `transformers-4.9.2/src/transformers/models/ibert/configuration_ibert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/ibert/modeling_ibert.py` & `transformers-4.9.2/src/transformers/models/ibert/modeling_ibert.py`

 * *Files 1% similar despite different names*

```diff
@@ -944,30 +944,32 @@
     """I-BERT Head for masked language modeling."""
 
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Linear(config.hidden_size, config.hidden_size)
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
-        self.decoder = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
+        self.decoder = nn.Linear(config.hidden_size, config.vocab_size)
         self.bias = nn.Parameter(torch.zeros(config.vocab_size))
-
-        # Need a link between the two variables so that the bias is correctly resized with `resize_token_embeddings`
         self.decoder.bias = self.bias
 
     def forward(self, features, **kwargs):
         x = self.dense(features)
         x = gelu(x)
         x = self.layer_norm(x)
 
         # project back to size of vocabulary with bias
         x = self.decoder(x)
 
         return x
 
+    def _tie_weights(self):
+        # To tie those two weights if they get disconnected (on TPU or when the bias is resized)
+        self.bias = self.decoder.bias
+
 
 @add_start_docstrings(
     """
     I-BERT Model transformer with a sequence classification/regression head on top (a linear layer on top of the pooled
     output) e.g. for GLUE tasks.
     """,
     IBERT_START_DOCSTRING,
```

### Comparing `transformers-4.9.1/src/transformers/models/ibert/quant_modules.py` & `transformers-4.9.2/src/transformers/models/ibert/quant_modules.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/layoutlm/__init__.py` & `transformers-4.9.2/src/transformers/models/layoutlm/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/layoutlm/configuration_layoutlm.py` & `transformers-4.9.2/src/transformers/models/layoutlm/configuration_layoutlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/layoutlm/modeling_layoutlm.py` & `transformers-4.9.2/src/transformers/models/layoutlm/modeling_layoutlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/layoutlm/modeling_tf_layoutlm.py` & `transformers-4.9.2/src/transformers/models/layoutlm/modeling_tf_layoutlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/layoutlm/tokenization_layoutlm.py` & `transformers-4.9.2/src/transformers/models/layoutlm/tokenization_layoutlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/layoutlm/tokenization_layoutlm_fast.py` & `transformers-4.9.2/src/transformers/models/layoutlm/tokenization_layoutlm_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/led/__init__.py` & `transformers-4.9.2/src/transformers/models/led/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/led/configuration_led.py` & `transformers-4.9.2/src/transformers/models/led/configuration_led.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/led/modeling_led.py` & `transformers-4.9.2/src/transformers/models/led/modeling_led.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/led/modeling_tf_led.py` & `transformers-4.9.2/src/transformers/models/led/modeling_tf_led.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/led/tokenization_led.py` & `transformers-4.9.2/src/transformers/models/led/tokenization_led.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/led/tokenization_led_fast.py` & `transformers-4.9.2/src/transformers/models/led/tokenization_led_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/longformer/__init__.py` & `transformers-4.9.2/src/transformers/models/longformer/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/longformer/configuration_longformer.py` & `transformers-4.9.2/src/transformers/models/longformer/configuration_longformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/longformer/convert_longformer_original_pytorch_lightning_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/longformer/modeling_longformer.py` & `transformers-4.9.2/src/transformers/models/longformer/modeling_longformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1332,30 +1332,32 @@
     """Longformer Head for masked language modeling."""
 
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Linear(config.hidden_size, config.hidden_size)
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
-        self.decoder = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
+        self.decoder = nn.Linear(config.hidden_size, config.vocab_size)
         self.bias = nn.Parameter(torch.zeros(config.vocab_size))
-
-        # Need a link between the two variables so that the bias is correctly resized with `resize_token_embeddings`
         self.decoder.bias = self.bias
 
     def forward(self, features, **kwargs):
         x = self.dense(features)
         x = gelu(x)
         x = self.layer_norm(x)
 
         # project back to size of vocabulary with bias
         x = self.decoder(x)
 
         return x
 
+    def _tie_weights(self):
+        # To tie those two weights if they get disconnected (on TPU or when the bias is resized)
+        self.bias = self.decoder.bias
+
 
 class LongformerPreTrainedModel(PreTrainedModel):
     """
     An abstract class to handle weights initialization and a simple interface for downloading and loading pretrained
     models.
     """
```

### Comparing `transformers-4.9.1/src/transformers/models/longformer/modeling_tf_longformer.py` & `transformers-4.9.2/src/transformers/models/longformer/modeling_tf_longformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/longformer/tokenization_longformer.py` & `transformers-4.9.2/src/transformers/models/longformer/tokenization_longformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/longformer/tokenization_longformer_fast.py` & `transformers-4.9.2/src/transformers/models/longformer/tokenization_longformer_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/luke/__init__.py` & `transformers-4.9.2/src/transformers/models/luke/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/luke/configuration_luke.py` & `transformers-4.9.2/src/transformers/models/luke/configuration_luke.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/luke/convert_luke_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/luke/modeling_luke.py` & `transformers-4.9.2/src/transformers/models/luke/modeling_luke.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/luke/tokenization_luke.py` & `transformers-4.9.2/src/transformers/models/luke/tokenization_luke.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/__init__.py` & `transformers-4.9.2/src/transformers/models/lxmert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/configuration_lxmert.py` & `transformers-4.9.2/src/transformers/models/lxmert/configuration_lxmert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/lxmert/convert_lxmert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/modeling_lxmert.py` & `transformers-4.9.2/src/transformers/models/lxmert/modeling_lxmert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/modeling_tf_lxmert.py` & `transformers-4.9.2/src/transformers/models/lxmert/modeling_tf_lxmert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/tokenization_lxmert.py` & `transformers-4.9.2/src/transformers/models/lxmert/tokenization_lxmert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/lxmert/tokenization_lxmert_fast.py` & `transformers-4.9.2/src/transformers/models/lxmert/tokenization_lxmert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/m2m_100/__init__.py` & `transformers-4.9.2/src/transformers/models/m2m_100/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/m2m_100/configuration_m2m_100.py` & `transformers-4.9.2/src/transformers/models/m2m_100/configuration_m2m_100.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/m2m_100/convert_m2m100_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/m2m_100/modeling_m2m_100.py` & `transformers-4.9.2/src/transformers/models/m2m_100/modeling_m2m_100.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/m2m_100/tokenization_m2m_100.py` & `transformers-4.9.2/src/transformers/models/m2m_100/tokenization_m2m_100.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/__init__.py` & `transformers-4.9.2/src/transformers/models/marian/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/configuration_marian.py` & `transformers-4.9.2/src/transformers/models/marian/configuration_marian.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/marian/convert_marian_tatoeba_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/convert_marian_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/marian/convert_marian_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/modeling_flax_marian.py` & `transformers-4.9.2/src/transformers/models/marian/modeling_flax_marian.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/modeling_marian.py` & `transformers-4.9.2/src/transformers/models/marian/modeling_marian.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/modeling_tf_marian.py` & `transformers-4.9.2/src/transformers/models/marian/modeling_tf_marian.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/marian/tokenization_marian.py` & `transformers-4.9.2/src/transformers/models/marian/tokenization_marian.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/__init__.py` & `transformers-4.9.2/src/transformers/models/mbart/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     is_tf_available,
     is_tokenizers_available,
     is_torch_available,
 )
 
 
 _import_structure = {
-    "configuration_mbart": ["MBART_PRETRAINED_CONFIG_ARCHIVE_MAP", "MBartConfig"],
+    "configuration_mbart": ["MBART_PRETRAINED_CONFIG_ARCHIVE_MAP", "MBartConfig", "MBartOnnxConfig"],
 }
 
 if is_sentencepiece_available():
     _import_structure["tokenization_mbart"] = ["MBartTokenizer"]
     _import_structure["tokenization_mbart50"] = ["MBart50Tokenizer"]
 
 if is_tokenizers_available():
@@ -64,15 +64,15 @@
         "FlaxMBartForSequenceClassification",
         "FlaxMBartModel",
         "FlaxMBartPreTrainedModel",
     ]
 
 
 if TYPE_CHECKING:
-    from .configuration_mbart import MBART_PRETRAINED_CONFIG_ARCHIVE_MAP, MBartConfig
+    from .configuration_mbart import MBART_PRETRAINED_CONFIG_ARCHIVE_MAP, MBartConfig, MBartOnnxConfig
 
     if is_sentencepiece_available():
         from .tokenization_mbart import MBartTokenizer
         from .tokenization_mbart50 import MBart50Tokenizer
 
     if is_tokenizers_available():
         from .tokenization_mbart50_fast import MBart50TokenizerFast
```

### Comparing `transformers-4.9.1/src/transformers/models/mbart/configuration_mbart.py` & `transformers-4.9.2/src/transformers/models/pegasus/configuration_pegasus.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # coding=utf-8
-# Copyright 2021, The Facebook AI Research Team and The HuggingFace Inc. team. All rights reserved.
+# Copyright 2021, Google and The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" MBART model configuration """
+""" PEGASUS model configuration """
 
 from ...configuration_utils import PretrainedConfig
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)
 
-MBART_PRETRAINED_CONFIG_ARCHIVE_MAP = {
-    "facebook/mbart-large-cc25": "https://huggingface.co/facebook/mbart-large-cc25/resolve/main/config.json",
-    # See all MBART models at https://huggingface.co/models?filter=mbart
+PEGASUS_PRETRAINED_CONFIG_ARCHIVE_MAP = {
+    "google/pegasus-large": "https://huggingface.co/google/pegasus-large/resolve/main/config.json",
+    # See all PEGASUS models at https://huggingface.co/models?filter=pegasus
 }
 
 
-class MBartConfig(PretrainedConfig):
+class PegasusConfig(PretrainedConfig):
     r"""
-    This is the configuration class to store the configuration of a :class:`~transformers.MBartModel`. It is used to
-    instantiate an MBART model according to the specified arguments, defining the model architecture. Instantiating a
-    configuration with the defaults will yield a similar configuration to that of the MBART `facebook/mbart-large-cc25
-    <https://huggingface.co/facebook/mbart-large-cc25>`__ architecture.
+    This is the configuration class to store the configuration of a :class:`~transformers.PegasusModel`. It is used to
+    instantiate an PEGASUS model according to the specified arguments, defining the model architecture. Instantiating a
+    configuration with the defaults will yield a similar configuration to that of the PEGASUS `google/pegasus-large
+    <https://huggingface.co/google/pegasus-large>`__ architecture.
 
     Configuration objects inherit from :class:`~transformers.PretrainedConfig` and can be used to control the model
     outputs. Read the documentation from :class:`~transformers.PretrainedConfig` for more information.
 
 
     Args:
         vocab_size (:obj:`int`, `optional`, defaults to 50265):
-            Vocabulary size of the MBART model. Defines the number of different tokens that can be represented by the
-            :obj:`inputs_ids` passed when calling :class:`~transformers.MBartModel` or
-            :class:`~transformers.TFMBartModel`.
+            Vocabulary size of the PEGASUS model. Defines the number of different tokens that can be represented by the
+            :obj:`inputs_ids` passed when calling :class:`~transformers.PegasusModel` or
+            :class:`~transformers.TFPegasusModel`.
         d_model (:obj:`int`, `optional`, defaults to 1024):
             Dimensionality of the layers and the pooler layer.
         encoder_layers (:obj:`int`, `optional`, defaults to 12):
             Number of encoder layers.
         decoder_layers (:obj:`int`, `optional`, defaults to 12):
             Number of decoder layers.
         encoder_attention_heads (:obj:`int`, `optional`, defaults to 16):
@@ -80,32 +80,32 @@
             https://arxiv.org/abs/1909.11556>`__ for more details.
         gradient_checkpointing (:obj:`bool`, `optional`, defaults to :obj:`False`):
             If True, use gradient checkpointing to save memory at the expense of slower backward pass.
         scale_embedding (:obj:`bool`, `optional`, defaults to :obj:`False`):
             Scale embeddings by diving by sqrt(d_model).
         use_cache (:obj:`bool`, `optional`, defaults to :obj:`True`):
             Whether or not the model should return the last key/values attentions (not used by all models)
-        forced_eos_token_id (:obj:`int`, `optional`, defaults to 2):
+        forced_eos_token_id (:obj:`int`, `optional`, defaults to 1):
             The id of the token to force as the last generated token when :obj:`max_length` is reached. Usually set to
             :obj:`eos_token_id`.
 
     Example::
 
-        >>> from transformers import MBartModel, MBartConfig
+        >>> from transformers import PegasusModel, PegasusConfig
 
-        >>> # Initializing a MBART facebook/mbart-large-cc25 style configuration
-        >>> configuration = MBartConfig()
+        >>> # Initializing a PEGASUS google/pegasus-large style configuration
+        >>> configuration = PegasusConfig()
 
-        >>> # Initializing a model from the facebook/mbart-large-cc25 style configuration
-        >>> model = MBartModel(configuration)
+        >>> # Initializing a model from the google/pegasus-large style configuration
+        >>> model = PegasusModel(configuration)
 
         >>> # Accessing the model configuration
         >>> configuration = model.config
     """
-    model_type = "mbart"
+    model_type = "pegasus"
     keys_to_ignore_at_inference = ["past_key_values"]
 
     def __init__(
         self,
         vocab_size=50265,
         max_position_embeddings=1024,
         encoder_layers=12,
@@ -120,28 +120,28 @@
         is_encoder_decoder=True,
         activation_function="gelu",
         d_model=1024,
         dropout=0.1,
         attention_dropout=0.0,
         activation_dropout=0.0,
         init_std=0.02,
+        decoder_start_token_id=0,
         classifier_dropout=0.0,
         scale_embedding=False,
         gradient_checkpointing=False,
-        pad_token_id=1,
-        bos_token_id=0,
-        eos_token_id=2,
-        forced_eos_token_id=2,
+        pad_token_id=0,
+        eos_token_id=1,
+        forced_eos_token_id=1,
         **kwargs
     ):
         super().__init__(
             pad_token_id=pad_token_id,
-            bos_token_id=bos_token_id,
             eos_token_id=eos_token_id,
             is_encoder_decoder=is_encoder_decoder,
+            decoder_start_token_id=decoder_start_token_id,
             forced_eos_token_id=forced_eos_token_id,
             **kwargs,
         )
 
         self.vocab_size = vocab_size
         self.max_position_embeddings = max_position_embeddings
         self.d_model = d_model
```

### Comparing `transformers-4.9.1/src/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/mbart/convert_mbart_original_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/modeling_flax_mbart.py` & `transformers-4.9.2/src/transformers/models/mbart/modeling_flax_mbart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/modeling_mbart.py` & `transformers-4.9.2/src/transformers/models/mbart/modeling_mbart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/modeling_tf_mbart.py` & `transformers-4.9.2/src/transformers/models/mbart/modeling_tf_mbart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart.py` & `transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart50.py` & `transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart50.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart50_fast.py` & `transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart50_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mbart/tokenization_mbart_fast.py` & `transformers-4.9.2/src/transformers/models/mbart/tokenization_mbart_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/megatron_bert/__init__.py` & `transformers-4.9.2/src/transformers/models/megatron_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/megatron_bert/configuration_megatron_bert.py` & `transformers-4.9.2/src/transformers/models/megatron_bert/configuration_megatron_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py` & `transformers-4.9.2/src/transformers/models/megatron_bert/convert_megatron_bert_checkpoint.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/megatron_bert/modeling_megatron_bert.py` & `transformers-4.9.2/src/transformers/models/megatron_bert/modeling_megatron_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mmbt/__init__.py` & `transformers-4.9.2/src/transformers/models/mmbt/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mmbt/configuration_mmbt.py` & `transformers-4.9.2/src/transformers/models/mmbt/configuration_mmbt.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mmbt/modeling_mmbt.py` & `transformers-4.9.2/src/transformers/models/mmbt/modeling_mmbt.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/__init__.py` & `transformers-4.9.2/src/transformers/models/mobilebert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/configuration_mobilebert.py` & `transformers-4.9.2/src/transformers/models/mobilebert/configuration_mobilebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/mobilebert/convert_mobilebert_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/modeling_mobilebert.py` & `transformers-4.9.2/src/transformers/models/mobilebert/modeling_mobilebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/modeling_tf_mobilebert.py` & `transformers-4.9.2/src/transformers/models/mobilebert/modeling_tf_mobilebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/tokenization_mobilebert.py` & `transformers-4.9.2/src/transformers/models/mobilebert/tokenization_mobilebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mobilebert/tokenization_mobilebert_fast.py` & `transformers-4.9.2/src/transformers/models/mobilebert/tokenization_mobilebert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mpnet/__init__.py` & `transformers-4.9.2/src/transformers/models/mpnet/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mpnet/configuration_mpnet.py` & `transformers-4.9.2/src/transformers/models/mpnet/configuration_mpnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mpnet/modeling_mpnet.py` & `transformers-4.9.2/src/transformers/models/mpnet/modeling_mpnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mpnet/modeling_tf_mpnet.py` & `transformers-4.9.2/src/transformers/models/mpnet/modeling_tf_mpnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mpnet/tokenization_mpnet.py` & `transformers-4.9.2/src/transformers/models/mpnet/tokenization_mpnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mpnet/tokenization_mpnet_fast.py` & `transformers-4.9.2/src/transformers/models/mpnet/tokenization_mpnet_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mt5/__init__.py` & `transformers-4.9.2/src/transformers/models/mt5/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mt5/configuration_mt5.py` & `transformers-4.9.2/src/transformers/models/mt5/configuration_mt5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mt5/modeling_mt5.py` & `transformers-4.9.2/src/transformers/models/mt5/modeling_mt5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/mt5/modeling_tf_mt5.py` & `transformers-4.9.2/src/transformers/models/mt5/modeling_tf_mt5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/openai/__init__.py` & `transformers-4.9.2/src/transformers/models/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/openai/configuration_openai.py` & `transformers-4.9.2/src/transformers/models/xlm/configuration_xlm.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,176 +1,242 @@
 # coding=utf-8
-# Copyright 2018 The OpenAI Team Authors and HuggingFace Inc. team.
-# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
+# Copyright 2019-present, Facebook, Inc and the HuggingFace Inc. team.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" OpenAI GPT configuration """
+""" XLM configuration """
 
 from ...configuration_utils import PretrainedConfig
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)
 
-OPENAI_GPT_PRETRAINED_CONFIG_ARCHIVE_MAP = {"openai-gpt": "https://huggingface.co/openai-gpt/resolve/main/config.json"}
+XLM_PRETRAINED_CONFIG_ARCHIVE_MAP = {
+    "xlm-mlm-en-2048": "https://huggingface.co/xlm-mlm-en-2048/resolve/main/config.json",
+    "xlm-mlm-ende-1024": "https://huggingface.co/xlm-mlm-ende-1024/resolve/main/config.json",
+    "xlm-mlm-enfr-1024": "https://huggingface.co/xlm-mlm-enfr-1024/resolve/main/config.json",
+    "xlm-mlm-enro-1024": "https://huggingface.co/xlm-mlm-enro-1024/resolve/main/config.json",
+    "xlm-mlm-tlm-xnli15-1024": "https://huggingface.co/xlm-mlm-tlm-xnli15-1024/resolve/main/config.json",
+    "xlm-mlm-xnli15-1024": "https://huggingface.co/xlm-mlm-xnli15-1024/resolve/main/config.json",
+    "xlm-clm-enfr-1024": "https://huggingface.co/xlm-clm-enfr-1024/resolve/main/config.json",
+    "xlm-clm-ende-1024": "https://huggingface.co/xlm-clm-ende-1024/resolve/main/config.json",
+    "xlm-mlm-17-1280": "https://huggingface.co/xlm-mlm-17-1280/resolve/main/config.json",
+    "xlm-mlm-100-1280": "https://huggingface.co/xlm-mlm-100-1280/resolve/main/config.json",
+}
 
 
-class OpenAIGPTConfig(PretrainedConfig):
+class XLMConfig(PretrainedConfig):
     """
-    This is the configuration class to store the configuration of a :class:`~transformers.OpenAIGPTModel` or a
-    :class:`~transformers.TFOpenAIGPTModel`. It is used to instantiate a GPT model according to the specified
-    arguments, defining the model architecture. Instantiating a configuration with the defaults will yield a similar
-    configuration to that of the `GPT <https://huggingface.co/openai-gpt>`__ architecture from OpenAI.
+    This is the configuration class to store the configuration of a :class:`~transformers.XLMModel` or a
+    :class:`~transformers.TFXLMModel`. It is used to instantiate a XLM model according to the specified arguments,
+    defining the model architecture. Instantiating a configuration with the defaults will yield a similar configuration
+    to that of the `xlm-mlm-en-2048 <https://huggingface.co/xlm-mlm-en-2048>`__ architecture.
 
     Configuration objects inherit from :class:`~transformers.PretrainedConfig` and can be used to control the model
     outputs. Read the documentation from :class:`~transformers.PretrainedConfig` for more information.
 
     Args:
-        vocab_size (:obj:`int`, `optional`, defaults to 40478):
-            Vocabulary size of the GPT-2 model. Defines the number of different tokens that can be represented by the
-            :obj:`inputs_ids` passed when calling :class:`~transformers.OpenAIGPTModel` or
-            :class:`~transformers.TFOpenAIGPTModel`.
-        n_positions (:obj:`int`, `optional`, defaults to 512):
-            The maximum sequence length that this model might ever be used with. Typically set this to something large
-            just in case (e.g., 512 or 1024 or 2048).
-        n_ctx (:obj:`int`, `optional`, defaults to 512):
-            Dimensionality of the causal mask (usually same as n_positions).
-        n_embd (:obj:`int`, `optional`, defaults to 768):
-            Dimensionality of the embeddings and hidden states.
+        vocab_size (:obj:`int`, `optional`, defaults to 30145):
+            Vocabulary size of the BERT model. Defines the number of different tokens that can be represented by the
+            :obj:`inputs_ids` passed when calling :class:`~transformers.XLMModel` or :class:`~transformers.TFXLMModel`.
+        emb_dim (:obj:`int`, `optional`, defaults to 2048):
+            Dimensionality of the encoder layers and the pooler layer.
         n_layer (:obj:`int`, `optional`, defaults to 12):
             Number of hidden layers in the Transformer encoder.
-        n_head (:obj:`int`, `optional`, defaults to 12):
+        n_head (:obj:`int`, `optional`, defaults to 16):
             Number of attention heads for each attention layer in the Transformer encoder.
-        afn (:obj:`str` or :obj:`Callable`, `optional`, defaults to :obj:`"gelu"`):
-            The non-linear activation function (function or string) in the encoder and pooler. If string,
-            :obj:`"gelu"`, :obj:`"relu"`, :obj:`"silu"` and :obj:`"gelu_new"` are supported.
-        resid_pdrop (:obj:`float`, `optional`, defaults to 0.1):
+        dropout (:obj:`float`, `optional`, defaults to 0.1):
             The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
-        embd_pdrop (:obj:`int`, `optional`, defaults to 0.1):
-            The dropout ratio for the embeddings.
-        attn_pdrop (:obj:`float`, `optional`, defaults to 0.1):
-            The dropout ratio for the attention.
-        layer_norm_epsilon (:obj:`float`, `optional`, defaults to 1e-5):
-            The epsilon to use in the layer normalization layers
-        initializer_range (:obj:`float`, `optional`, defaults to 0.02):
-            The standard deviation of the truncated_normal_initializer for initializing all weight matrices.
-        predict_special_tokens (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Whether or not special tokens should be predicted when the model has a language modeling head.
-        summary_type (:obj:`str`, `optional`, defaults to :obj:`"cls_index"`):
-            Argument used when doing sequence summary, used in the models
-            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+        attention_dropout (:obj:`float`, `optional`, defaults to 0.1):
+            The dropout probability for the attention mechanism
+        gelu_activation (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Whether or not to use `gelu` for the activations instead of `relu`.
+        sinusoidal_embeddings (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            Whether or not to use sinusoidal positional embeddings instead of absolute positional embeddings.
+        causal (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            Whether or not the model should behave in a causal manner. Causal models use a triangular attention mask in
+            order to only attend to the left-side context instead if a bidirectional context.
+        asm (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            Whether or not to use an adaptive log softmax projection layer instead of a linear layer for the prediction
+            layer.
+        n_langs (:obj:`int`, `optional`, defaults to 1):
+            The number of languages the model handles. Set to 1 for monolingual models.
+        use_lang_emb (:obj:`bool`, `optional`, defaults to :obj:`True`)
+            Whether to use language embeddings. Some models use additional language embeddings, see `the multilingual
+            models page <http://huggingface.co/transformers/multilingual.html#xlm-language-embeddings>`__ for
+            information on how to use them.
+        max_position_embeddings (:obj:`int`, `optional`, defaults to 512):
+            The maximum sequence length that this model might ever be used with. Typically set this to something large
+            just in case (e.g., 512 or 1024 or 2048).
+        embed_init_std (:obj:`float`, `optional`, defaults to 2048^-0.5):
+            The standard deviation of the truncated_normal_initializer for initializing the embedding matrices.
+        init_std (:obj:`int`, `optional`, defaults to 50257):
+            The standard deviation of the truncated_normal_initializer for initializing all weight matrices except the
+            embedding matrices.
+        layer_norm_eps (:obj:`float`, `optional`, defaults to 1e-12):
+            The epsilon used by the layer normalization layers.
+        bos_index (:obj:`int`, `optional`, defaults to 0):
+            The index of the beginning of sentence token in the vocabulary.
+        eos_index (:obj:`int`, `optional`, defaults to 1):
+            The index of the end of sentence token in the vocabulary.
+        pad_index (:obj:`int`, `optional`, defaults to 2):
+            The index of the padding token in the vocabulary.
+        unk_index (:obj:`int`, `optional`, defaults to 3):
+            The index of the unknown token in the vocabulary.
+        mask_index (:obj:`int`, `optional`, defaults to 5):
+            The index of the masking token in the vocabulary.
+        is_encoder(:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Whether or not the initialized model should be a transformer encoder or decoder as seen in Vaswani et al.
+        summary_type (:obj:`string`, `optional`, defaults to "first"):
+            Argument used when doing sequence summary. Used in the sequence classification and multiple choice models.
 
             Has to be one of the following options:
 
                 - :obj:`"last"`: Take the last token hidden state (like XLNet).
                 - :obj:`"first"`: Take the first token hidden state (like BERT).
                 - :obj:`"mean"`: Take the mean of all tokens hidden states.
                 - :obj:`"cls_index"`: Supply a Tensor of classification token position (like GPT/GPT-2).
                 - :obj:`"attn"`: Not implemented now, use multi-head attention.
         summary_use_proj (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Argument used when doing sequence summary, used in the models
-            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+            Argument used when doing sequence summary. Used in the sequence classification and multiple choice models.
 
             Whether or not to add a projection after the vector extraction.
         summary_activation (:obj:`str`, `optional`):
-            Argument used when doing sequence summary, used in the models
-            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+            Argument used when doing sequence summary. Used in the sequence classification and multiple choice models.
 
             Pass :obj:`"tanh"` for a tanh activation to the output, any other value will result in no activation.
         summary_proj_to_labels (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Argument used when doing sequence summary, used in the models
-            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+            Used in the sequence classification and multiple choice models.
 
             Whether the projection outputs should have :obj:`config.num_labels` or :obj:`config.hidden_size` classes.
         summary_first_dropout (:obj:`float`, `optional`, defaults to 0.1):
-            Argument used when doing sequence summary, used in the models
-            :class:`~transformers.OpenAIGPTDoubleHeadsModel` and :class:`~transformers.OpenAIGPTDoubleHeadsModel`.
+            Used in the sequence classification and multiple choice models.
 
             The dropout ratio to be used after the projection and activation.
-        use_cache (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Whether or not the model should return the last key/values attentions (not used by all models).
-
+        start_n_top (:obj:`int`, `optional`, defaults to 5):
+            Used in the SQuAD evaluation script.
+        end_n_top (:obj:`int`, `optional`, defaults to 5):
+            Used in the SQuAD evaluation script.
+        mask_token_id (:obj:`int`, `optional`, defaults to 0):
+            Model agnostic parameter to identify masked tokens when generating text in an MLM context.
+        lang_id (:obj:`int`, `optional`, defaults to 1):
+            The ID of the language used by the model. This parameter is used when generating text in a given language.
 
     Examples::
 
-        >>> from transformers import OpenAIGPTConfig, OpenAIGPTModel
+        >>> from transformers import XLMConfig, XLMModel
 
-        >>> # Initializing a GPT configuration
-        >>> configuration = OpenAIGPTConfig()
+        >>> # Initializing a XLM configuration
+        >>> configuration = XLMConfig()
 
         >>> # Initializing a model from the configuration
-        >>> model = OpenAIGPTModel(configuration)
+        >>> model = XLMModel(configuration)
 
         >>> # Accessing the model configuration
         >>> configuration = model.config
     """
 
-    model_type = "openai-gpt"
+    model_type = "xlm"
 
     def __init__(
         self,
-        vocab_size=40478,
-        n_positions=512,
-        n_ctx=512,
-        n_embd=768,
-        n_layer=12,
-        n_head=12,
-        afn="gelu",
-        resid_pdrop=0.1,
-        embd_pdrop=0.1,
-        attn_pdrop=0.1,
-        layer_norm_epsilon=1e-5,
-        initializer_range=0.02,
-        predict_special_tokens=True,
-        summary_type="cls_index",
+        vocab_size=30145,
+        emb_dim=2048,
+        n_layers=12,
+        n_heads=16,
+        dropout=0.1,
+        attention_dropout=0.1,
+        gelu_activation=True,
+        sinusoidal_embeddings=False,
+        causal=False,
+        asm=False,
+        n_langs=1,
+        use_lang_emb=True,
+        max_position_embeddings=512,
+        embed_init_std=2048 ** -0.5,
+        layer_norm_eps=1e-12,
+        init_std=0.02,
+        bos_index=0,
+        eos_index=1,
+        pad_index=2,
+        unk_index=3,
+        mask_index=5,
+        is_encoder=True,
+        summary_type="first",
         summary_use_proj=True,
         summary_activation=None,
         summary_proj_to_labels=True,
         summary_first_dropout=0.1,
+        start_n_top=5,
+        end_n_top=5,
+        mask_token_id=0,
+        lang_id=0,
+        pad_token_id=2,
+        bos_token_id=0,
         **kwargs
     ):
-        super().__init__(**kwargs)
-
+        """Constructs XLMConfig."""
+        super().__init__(pad_token_id=pad_token_id, bos_token_id=bos_token_id, **kwargs)
         self.vocab_size = vocab_size
-        self.n_ctx = n_ctx
-        self.n_positions = n_positions
-        self.n_embd = n_embd
-        self.n_layer = n_layer
-        self.n_head = n_head
-        self.afn = afn
-        self.resid_pdrop = resid_pdrop
-        self.embd_pdrop = embd_pdrop
-        self.attn_pdrop = attn_pdrop
-        self.layer_norm_epsilon = layer_norm_epsilon
-        self.initializer_range = initializer_range
-        self.predict_special_tokens = predict_special_tokens
+        self.emb_dim = emb_dim
+        self.n_layers = n_layers
+        self.n_heads = n_heads
+        self.dropout = dropout
+        self.attention_dropout = attention_dropout
+        self.gelu_activation = gelu_activation
+        self.sinusoidal_embeddings = sinusoidal_embeddings
+        self.causal = causal
+        self.asm = asm
+        self.n_langs = n_langs
+        self.use_lang_emb = use_lang_emb
+        self.layer_norm_eps = layer_norm_eps
+        self.bos_index = bos_index
+        self.eos_index = eos_index
+        self.pad_index = pad_index
+        self.unk_index = unk_index
+        self.mask_index = mask_index
+        self.is_encoder = is_encoder
+        self.max_position_embeddings = max_position_embeddings
+        self.embed_init_std = embed_init_std
+        self.init_std = init_std
         self.summary_type = summary_type
         self.summary_use_proj = summary_use_proj
         self.summary_activation = summary_activation
-        self.summary_first_dropout = summary_first_dropout
         self.summary_proj_to_labels = summary_proj_to_labels
+        self.summary_first_dropout = summary_first_dropout
+        self.start_n_top = start_n_top
+        self.end_n_top = end_n_top
+        self.mask_token_id = mask_token_id
+        self.lang_id = lang_id
+
+        if "n_words" in kwargs:
+            self.n_words = kwargs["n_words"]
 
     @property
-    def max_position_embeddings(self):
-        return self.n_positions
+    def n_words(self):  # For backward compatibility
+        return self.vocab_size
+
+    @n_words.setter
+    def n_words(self, value):  # For backward compatibility
+        self.vocab_size = value
 
     @property
     def hidden_size(self):
-        return self.n_embd
+        return self.emb_dim
 
     @property
     def num_attention_heads(self):
-        return self.n_head
+        return self.n_heads
 
     @property
     def num_hidden_layers(self):
-        return self.n_layer
+        return self.n_layers
```

### Comparing `transformers-4.9.1/src/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/openai/convert_openai_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/openai/modeling_openai.py` & `transformers-4.9.2/src/transformers/models/openai/modeling_openai.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/openai/modeling_tf_openai.py` & `transformers-4.9.2/src/transformers/models/openai/modeling_tf_openai.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/openai/tokenization_openai.py` & `transformers-4.9.2/src/transformers/models/openai/tokenization_openai.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/openai/tokenization_openai_fast.py` & `transformers-4.9.2/src/transformers/models/openai/tokenization_openai_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/__init__.py` & `transformers-4.9.2/src/transformers/models/pegasus/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/configuration_pegasus.py` & `transformers-4.9.2/src/transformers/models/mbart/configuration_mbart.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,55 @@
 # coding=utf-8
-# Copyright 2021, Google and The HuggingFace Inc. team. All rights reserved.
+# Copyright 2021, The Facebook AI Research Team and The HuggingFace Inc. team. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" PEGASUS model configuration """
+""" MBART model configuration """
+from collections import OrderedDict
+from typing import Mapping
+
+from transformers.onnx import OnnxConfigWithPast
 
 from ...configuration_utils import PretrainedConfig
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)
 
-PEGASUS_PRETRAINED_CONFIG_ARCHIVE_MAP = {
-    "google/pegasus-large": "https://huggingface.co/google/pegasus-large/resolve/main/config.json",
-    # See all PEGASUS models at https://huggingface.co/models?filter=pegasus
+MBART_PRETRAINED_CONFIG_ARCHIVE_MAP = {
+    "facebook/mbart-large-cc25": "https://huggingface.co/facebook/mbart-large-cc25/resolve/main/config.json",
+    # See all MBART models at https://huggingface.co/models?filter=mbart
 }
 
 
-class PegasusConfig(PretrainedConfig):
+class MBartConfig(PretrainedConfig):
     r"""
-    This is the configuration class to store the configuration of a :class:`~transformers.PegasusModel`. It is used to
-    instantiate an PEGASUS model according to the specified arguments, defining the model architecture. Instantiating a
-    configuration with the defaults will yield a similar configuration to that of the PEGASUS `google/pegasus-large
-    <https://huggingface.co/google/pegasus-large>`__ architecture.
+    This is the configuration class to store the configuration of a :class:`~transformers.MBartModel`. It is used to
+    instantiate an MBART model according to the specified arguments, defining the model architecture. Instantiating a
+    configuration with the defaults will yield a similar configuration to that of the MBART `facebook/mbart-large-cc25
+    <https://huggingface.co/facebook/mbart-large-cc25>`__ architecture.
 
     Configuration objects inherit from :class:`~transformers.PretrainedConfig` and can be used to control the model
     outputs. Read the documentation from :class:`~transformers.PretrainedConfig` for more information.
 
 
     Args:
         vocab_size (:obj:`int`, `optional`, defaults to 50265):
-            Vocabulary size of the PEGASUS model. Defines the number of different tokens that can be represented by the
-            :obj:`inputs_ids` passed when calling :class:`~transformers.PegasusModel` or
-            :class:`~transformers.TFPegasusModel`.
+            Vocabulary size of the MBART model. Defines the number of different tokens that can be represented by the
+            :obj:`inputs_ids` passed when calling :class:`~transformers.MBartModel` or
+            :class:`~transformers.TFMBartModel`.
         d_model (:obj:`int`, `optional`, defaults to 1024):
             Dimensionality of the layers and the pooler layer.
         encoder_layers (:obj:`int`, `optional`, defaults to 12):
             Number of encoder layers.
         decoder_layers (:obj:`int`, `optional`, defaults to 12):
             Number of decoder layers.
         encoder_attention_heads (:obj:`int`, `optional`, defaults to 16):
@@ -80,32 +84,32 @@
             https://arxiv.org/abs/1909.11556>`__ for more details.
         gradient_checkpointing (:obj:`bool`, `optional`, defaults to :obj:`False`):
             If True, use gradient checkpointing to save memory at the expense of slower backward pass.
         scale_embedding (:obj:`bool`, `optional`, defaults to :obj:`False`):
             Scale embeddings by diving by sqrt(d_model).
         use_cache (:obj:`bool`, `optional`, defaults to :obj:`True`):
             Whether or not the model should return the last key/values attentions (not used by all models)
-        forced_eos_token_id (:obj:`int`, `optional`, defaults to 1):
+        forced_eos_token_id (:obj:`int`, `optional`, defaults to 2):
             The id of the token to force as the last generated token when :obj:`max_length` is reached. Usually set to
             :obj:`eos_token_id`.
 
     Example::
 
-        >>> from transformers import PegasusModel, PegasusConfig
+        >>> from transformers import MBartModel, MBartConfig
 
-        >>> # Initializing a PEGASUS google/pegasus-large style configuration
-        >>> configuration = PegasusConfig()
+        >>> # Initializing a MBART facebook/mbart-large-cc25 style configuration
+        >>> configuration = MBartConfig()
 
-        >>> # Initializing a model from the google/pegasus-large style configuration
-        >>> model = PegasusModel(configuration)
+        >>> # Initializing a model from the facebook/mbart-large-cc25 style configuration
+        >>> model = MBartModel(configuration)
 
         >>> # Accessing the model configuration
         >>> configuration = model.config
     """
-    model_type = "pegasus"
+    model_type = "mbart"
     keys_to_ignore_at_inference = ["past_key_values"]
 
     def __init__(
         self,
         vocab_size=50265,
         max_position_embeddings=1024,
         encoder_layers=12,
@@ -120,28 +124,28 @@
         is_encoder_decoder=True,
         activation_function="gelu",
         d_model=1024,
         dropout=0.1,
         attention_dropout=0.0,
         activation_dropout=0.0,
         init_std=0.02,
-        decoder_start_token_id=0,
         classifier_dropout=0.0,
         scale_embedding=False,
         gradient_checkpointing=False,
-        pad_token_id=0,
-        eos_token_id=1,
-        forced_eos_token_id=1,
+        pad_token_id=1,
+        bos_token_id=0,
+        eos_token_id=2,
+        forced_eos_token_id=2,
         **kwargs
     ):
         super().__init__(
             pad_token_id=pad_token_id,
+            bos_token_id=bos_token_id,
             eos_token_id=eos_token_id,
             is_encoder_decoder=is_encoder_decoder,
-            decoder_start_token_id=decoder_start_token_id,
             forced_eos_token_id=forced_eos_token_id,
             **kwargs,
         )
 
         self.vocab_size = vocab_size
         self.max_position_embeddings = max_position_embeddings
         self.d_model = d_model
@@ -167,7 +171,36 @@
     @property
     def num_attention_heads(self) -> int:
         return self.encoder_attention_heads
 
     @property
     def hidden_size(self) -> int:
         return self.d_model
+
+
+class MBartOnnxConfig(OnnxConfigWithPast):
+    @property
+    def inputs(self) -> Mapping[str, Mapping[int, str]]:
+        return OrderedDict(
+            [
+                ("input_ids", {0: "batch", 1: "sequence"}),
+                ("attention_mask", {0: "batch", 1: "sequence"}),
+            ]
+        )
+
+    @property
+    def outputs(self) -> Mapping[str, Mapping[int, str]]:
+        if self.use_past:
+            return OrderedDict(
+                [
+                    ("last_hidden_state", {0: "batch", 1: "sequence"}),
+                    ("past_keys", {0: "batch", 2: "sequence"}),
+                    ("encoder_last_hidden_state", {0: "batch", 1: "sequence"}),
+                ]
+            )
+        else:
+            return OrderedDict(
+                [
+                    ("last_hidden_state", {0: "batch", 1: "sequence"}),
+                    ("encoder_last_hidden_state", {0: "batch", 1: "sequence"}),
+                ]
+            )
```

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/pegasus/convert_pegasus_tf_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/modeling_pegasus.py` & `transformers-4.9.2/src/transformers/models/pegasus/modeling_pegasus.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/modeling_tf_pegasus.py` & `transformers-4.9.2/src/transformers/models/pegasus/modeling_tf_pegasus.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/tokenization_pegasus.py` & `transformers-4.9.2/src/transformers/models/pegasus/tokenization_pegasus.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/pegasus/tokenization_pegasus_fast.py` & `transformers-4.9.2/src/transformers/models/pegasus/tokenization_pegasus_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/phobert/__init__.py` & `transformers-4.9.2/src/transformers/models/phobert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/phobert/tokenization_phobert.py` & `transformers-4.9.2/src/transformers/models/phobert/tokenization_phobert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/prophetnet/__init__.py` & `transformers-4.9.2/src/transformers/models/prophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/prophetnet/configuration_prophetnet.py` & `transformers-4.9.2/src/transformers/models/prophetnet/configuration_prophetnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/prophetnet/convert_prophetnet_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/prophetnet/modeling_prophetnet.py` & `transformers-4.9.2/src/transformers/models/prophetnet/modeling_prophetnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/prophetnet/tokenization_prophetnet.py` & `transformers-4.9.2/src/transformers/models/prophetnet/tokenization_prophetnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/rag/__init__.py` & `transformers-4.9.2/src/transformers/models/rag/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/rag/configuration_rag.py` & `transformers-4.9.2/src/transformers/models/rag/configuration_rag.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/rag/modeling_rag.py` & `transformers-4.9.2/src/transformers/models/rag/modeling_rag.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/rag/modeling_tf_rag.py` & `transformers-4.9.2/src/transformers/models/rag/modeling_tf_rag.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/rag/retrieval_rag.py` & `transformers-4.9.2/src/transformers/models/rag/retrieval_rag.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/rag/tokenization_rag.py` & `transformers-4.9.2/src/transformers/models/rag/tokenization_rag.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/reformer/__init__.py` & `transformers-4.9.2/src/transformers/models/reformer/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/reformer/configuration_reformer.py` & `transformers-4.9.2/src/transformers/models/reformer/configuration_reformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/reformer/convert_reformer_trax_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/reformer/modeling_reformer.py` & `transformers-4.9.2/src/transformers/models/reformer/modeling_reformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -4586,2346 +4586,2349 @@
 00011e90: 6967 2e68 6964 6465 6e5f 7369 7a65 2c20  ig.hidden_size, 
 00011ea0: 636f 6e66 6967 2e76 6f63 6162 5f73 697a  config.vocab_siz
 00011eb0: 652c 2062 6961 733d 4661 6c73 6529 0a20  e, bias=False). 
 00011ec0: 2020 2020 2020 2073 656c 662e 6269 6173         self.bias
 00011ed0: 203d 206e 6e2e 5061 7261 6d65 7465 7228   = nn.Parameter(
 00011ee0: 746f 7263 682e 7a65 726f 7328 636f 6e66  torch.zeros(conf
 00011ef0: 6967 2e76 6f63 6162 5f73 697a 6529 290a  ig.vocab_size)).
-00011f00: 0a20 2020 2020 2020 2023 204e 6565 6420  .        # Need 
-00011f10: 6120 6c69 6e6b 2062 6574 7765 656e 2074  a link between t
-00011f20: 6865 2074 776f 2076 6172 6961 626c 6573  he two variables
-00011f30: 2073 6f20 7468 6174 2074 6865 2062 6961   so that the bia
-00011f40: 7320 6973 2063 6f72 7265 6374 6c79 2072  s is correctly r
-00011f50: 6573 697a 6564 2077 6974 6820 6072 6573  esized with `res
-00011f60: 697a 655f 746f 6b65 6e5f 656d 6265 6464  ize_token_embedd
-00011f70: 696e 6773 600a 2020 2020 2020 2020 7365  ings`.        se
-00011f80: 6c66 2e64 6563 6f64 6572 2e62 6961 7320  lf.decoder.bias 
-00011f90: 3d20 7365 6c66 2e62 6961 730a 0a20 2020  = self.bias..   
-00011fa0: 2064 6566 2066 6f72 7761 7264 2873 656c   def forward(sel
-00011fb0: 662c 2068 6964 6465 6e5f 7374 6174 6573  f, hidden_states
-00011fc0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00011fd0: 6e20 6170 706c 795f 6368 756e 6b69 6e67  n apply_chunking
-00011fe0: 5f74 6f5f 666f 7277 6172 6428 7365 6c66  _to_forward(self
-00011ff0: 2e66 6f72 7761 7264 5f63 6875 6e6b 2c20  .forward_chunk, 
-00012000: 7365 6c66 2e63 6875 6e6b 5f73 697a 655f  self.chunk_size_
-00012010: 6c6d 5f68 6561 642c 2073 656c 662e 7365  lm_head, self.se
-00012020: 715f 6c65 6e5f 6469 6d2c 2068 6964 6465  q_len_dim, hidde
-00012030: 6e5f 7374 6174 6573 290a 0a20 2020 2064  n_states)..    d
-00012040: 6566 2066 6f72 7761 7264 5f63 6875 6e6b  ef forward_chunk
-00012050: 2873 656c 662c 2068 6964 6465 6e5f 7374  (self, hidden_st
-00012060: 6174 6573 293a 0a20 2020 2020 2020 2068  ates):.        h
-00012070: 6964 6465 6e5f 7374 6174 6573 203d 2073  idden_states = s
-00012080: 656c 662e 6465 636f 6465 7228 6869 6464  elf.decoder(hidd
-00012090: 656e 5f73 7461 7465 7329 0a20 2020 2020  en_states).     
-000120a0: 2020 2072 6574 7572 6e20 6869 6464 656e     return hidden
-000120b0: 5f73 7461 7465 730a 0a0a 636c 6173 7320  _states...class 
-000120c0: 5265 666f 726d 6572 5072 6554 7261 696e  ReformerPreTrain
-000120d0: 6564 4d6f 6465 6c28 5072 6554 7261 696e  edModel(PreTrain
-000120e0: 6564 4d6f 6465 6c29 3a0a 2020 2020 2222  edModel):.    ""
-000120f0: 220a 2020 2020 416e 2061 6273 7472 6163  ".    An abstrac
-00012100: 7420 636c 6173 7320 746f 2068 616e 646c  t class to handl
-00012110: 6520 7765 6967 6874 7320 696e 6974 6961  e weights initia
-00012120: 6c69 7a61 7469 6f6e 2061 6e64 2061 2073  lization and a s
-00012130: 696d 706c 6520 696e 7465 7266 6163 6520  imple interface 
-00012140: 666f 7220 646f 776e 6c6f 6164 696e 6720  for downloading 
-00012150: 616e 6420 6c6f 6164 696e 6720 7072 6574  and loading pret
-00012160: 7261 696e 6564 0a20 2020 206d 6f64 656c  rained.    model
-00012170: 732e 0a20 2020 2022 2222 0a0a 2020 2020  s..    """..    
-00012180: 636f 6e66 6967 5f63 6c61 7373 203d 2052  config_class = R
-00012190: 6566 6f72 6d65 7243 6f6e 6669 670a 2020  eformerConfig.  
-000121a0: 2020 6261 7365 5f6d 6f64 656c 5f70 7265    base_model_pre
-000121b0: 6669 7820 3d20 2272 6566 6f72 6d65 7222  fix = "reformer"
-000121c0: 0a0a 2020 2020 4070 726f 7065 7274 790a  ..    @property.
-000121d0: 2020 2020 6465 6620 6475 6d6d 795f 696e      def dummy_in
-000121e0: 7075 7473 2873 656c 6629 3a0a 2020 2020  puts(self):.    
-000121f0: 2020 2020 696e 7075 745f 6964 7320 3d20      input_ids = 
-00012200: 746f 7263 682e 7465 6e73 6f72 2844 554d  torch.tensor(DUM
-00012210: 4d59 5f49 4e50 5554 5329 0a20 2020 2020  MY_INPUTS).     
-00012220: 2020 2069 6e70 7574 5f6d 6173 6b20 3d20     input_mask = 
-00012230: 746f 7263 682e 7465 6e73 6f72 2844 554d  torch.tensor(DUM
-00012240: 4d59 5f4d 4153 4b29 0a20 2020 2020 2020  MY_MASK).       
-00012250: 2064 756d 6d79 5f69 6e70 7574 7320 3d20   dummy_inputs = 
-00012260: 7b0a 2020 2020 2020 2020 2020 2020 2269  {.            "i
-00012270: 6e70 7574 5f69 6473 223a 2069 6e70 7574  nput_ids": input
-00012280: 5f69 6473 2c0a 2020 2020 2020 2020 2020  _ids,.          
-00012290: 2020 2261 7474 656e 7469 6f6e 5f6d 6173    "attention_mas
-000122a0: 6b22 3a20 696e 7075 745f 6d61 736b 2c0a  k": input_mask,.
-000122b0: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
-000122c0: 2020 7265 7475 726e 2064 756d 6d79 5f69    return dummy_i
-000122d0: 6e70 7574 730a 0a20 2020 2064 6566 205f  nputs..    def _
-000122e0: 696e 6974 5f77 6569 6768 7473 2873 656c  init_weights(sel
-000122f0: 662c 206d 6f64 756c 6529 3a0a 2020 2020  f, module):.    
-00012300: 2020 2020 2222 2249 6e69 7469 616c 697a      """Initializ
-00012310: 6520 7468 6520 7765 6967 6874 7322 2222  e the weights"""
-00012320: 0a20 2020 2020 2020 2069 6620 6973 696e  .        if isin
-00012330: 7374 616e 6365 286d 6f64 756c 652c 2041  stance(module, A
-00012340: 7869 616c 506f 7369 7469 6f6e 456d 6265  xialPositionEmbe
-00012350: 6464 696e 6773 293a 0a20 2020 2020 2020  ddings):.       
-00012360: 2020 2020 2066 6f72 2077 6569 6768 7420       for weight 
-00012370: 696e 206d 6f64 756c 652e 7765 6967 6874  in module.weight
-00012380: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00012390: 2020 206e 6e2e 696e 6974 2e6e 6f72 6d61     nn.init.norma
-000123a0: 6c5f 2877 6569 6768 742c 2073 7464 3d73  l_(weight, std=s
-000123b0: 656c 662e 636f 6e66 6967 2e61 7869 616c  elf.config.axial
-000123c0: 5f6e 6f72 6d5f 7374 6429 0a20 2020 2020  _norm_std).     
-000123d0: 2020 2065 6c69 6620 6973 696e 7374 616e     elif isinstan
-000123e0: 6365 286d 6f64 756c 652c 206e 6e2e 456d  ce(module, nn.Em
-000123f0: 6265 6464 696e 6729 3a0a 2020 2020 2020  bedding):.      
-00012400: 2020 2020 2020 6d6f 6475 6c65 2e77 6569        module.wei
-00012410: 6768 742e 6461 7461 2e6e 6f72 6d61 6c5f  ght.data.normal_
-00012420: 286d 6561 6e3d 302e 302c 2073 7464 3d73  (mean=0.0, std=s
-00012430: 656c 662e 636f 6e66 6967 2e69 6e69 7469  elf.config.initi
-00012440: 616c 697a 6572 5f72 616e 6765 290a 2020  alizer_range).  
-00012450: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-00012460: 756c 652e 7061 6464 696e 675f 6964 7820  ule.padding_idx 
-00012470: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00012480: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00012490: 756c 652e 7765 6967 6874 2e64 6174 615b  ule.weight.data[
-000124a0: 6d6f 6475 6c65 2e70 6164 6469 6e67 5f69  module.padding_i
-000124b0: 6478 5d2e 7a65 726f 5f28 290a 2020 2020  dx].zero_().    
-000124c0: 2020 2020 656c 6966 2069 7369 6e73 7461      elif isinsta
-000124d0: 6e63 6528 6d6f 6475 6c65 2c20 6e6e 2e4c  nce(module, nn.L
-000124e0: 696e 6561 7229 3a0a 2020 2020 2020 2020  inear):.        
-000124f0: 2020 2020 2320 536c 6967 6874 6c79 2064      # Slightly d
-00012500: 6966 6665 7265 6e74 2066 726f 6d20 7468  ifferent from th
-00012510: 6520 5446 2076 6572 7369 6f6e 2077 6869  e TF version whi
-00012520: 6368 2075 7365 7320 7472 756e 6361 7465  ch uses truncate
-00012530: 645f 6e6f 726d 616c 2066 6f72 2069 6e69  d_normal for ini
-00012540: 7469 616c 697a 6174 696f 6e0a 2020 2020  tialization.    
-00012550: 2020 2020 2020 2020 2320 6366 2068 7474          # cf htt
-00012560: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00012570: 7079 746f 7263 682f 7079 746f 7263 682f  pytorch/pytorch/
-00012580: 7075 6c6c 2f35 3631 370a 2020 2020 2020  pull/5617.      
-00012590: 2020 2020 2020 6d6f 6475 6c65 2e77 6569        module.wei
-000125a0: 6768 742e 6461 7461 2e6e 6f72 6d61 6c5f  ght.data.normal_
-000125b0: 286d 6561 6e3d 302e 302c 2073 7464 3d73  (mean=0.0, std=s
-000125c0: 656c 662e 636f 6e66 6967 2e69 6e69 7469  elf.config.initi
-000125d0: 616c 697a 6572 5f72 616e 6765 290a 2020  alizer_range).  
-000125e0: 2020 2020 2020 2020 2020 6966 206d 6f64            if mod
-000125f0: 756c 652e 6269 6173 2069 7320 6e6f 7420  ule.bias is not 
-00012600: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00012610: 2020 2020 2020 6d6f 6475 6c65 2e62 6961        module.bia
-00012620: 732e 6461 7461 2e7a 6572 6f5f 2829 0a20  s.data.zero_(). 
-00012630: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-00012640: 7374 616e 6365 286d 6f64 756c 652c 206e  stance(module, n
-00012650: 6e2e 4c61 7965 724e 6f72 6d29 3a0a 2020  n.LayerNorm):.  
-00012660: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
-00012670: 2e62 6961 732e 6461 7461 2e7a 6572 6f5f  .bias.data.zero_
-00012680: 2829 0a20 2020 2020 2020 2020 2020 206d  ().            m
-00012690: 6f64 756c 652e 7765 6967 6874 2e64 6174  odule.weight.dat
-000126a0: 612e 6669 6c6c 5f28 312e 3029 0a0a 0a40  a.fill_(1.0)...@
-000126b0: 6461 7461 636c 6173 730a 636c 6173 7320  dataclass.class 
-000126c0: 5265 666f 726d 6572 4d6f 6465 6c4f 7574  ReformerModelOut
-000126d0: 7075 7428 4d6f 6465 6c4f 7574 7075 7429  put(ModelOutput)
-000126e0: 3a0a 2020 2020 2222 220a 2020 2020 4f75  :.    """.    Ou
-000126f0: 7470 7574 2074 7970 6520 6f66 203a 636c  tput type of :cl
-00012700: 6173 733a 607e 7472 616e 7366 6f72 6d65  ass:`~transforme
-00012710: 7273 2e52 6566 6f72 6d65 724d 6f64 656c  rs.ReformerModel
-00012720: 602e 0a0a 2020 2020 4172 6773 3a0a 2020  `...    Args:.  
-00012730: 2020 2020 2020 6c61 7374 5f68 6964 6465        last_hidde
-00012740: 6e5f 7374 6174 6520 283a 6f62 6a3a 6074  n_state (:obj:`t
-00012750: 6f72 6368 2e46 6c6f 6174 5465 6e73 6f72  orch.FloatTensor
-00012760: 6020 6f66 2073 6861 7065 203a 6f62 6a3a  ` of shape :obj:
-00012770: 6028 6261 7463 685f 7369 7a65 2c20 6e75  `(batch_size, nu
-00012780: 6d5f 7072 6564 6963 742c 2068 6964 6465  m_predict, hidde
-00012790: 6e5f 7369 7a65 2960 293a 0a20 2020 2020  n_size)`):.     
-000127a0: 2020 2020 2020 2053 6571 7565 6e63 6520         Sequence 
-000127b0: 6f66 2068 6964 6465 6e2d 7374 6174 6573  of hidden-states
-000127c0: 2061 7420 7468 6520 6c61 7374 206c 6179   at the last lay
-000127d0: 6572 206f 6620 7468 6520 6d6f 6465 6c2e  er of the model.
-000127e0: 0a0a 2020 2020 2020 2020 2020 2020 6060  ..            ``
-000127f0: 6e75 6d5f 7072 6564 6963 7460 6020 636f  num_predict`` co
-00012800: 7272 6573 706f 6e64 7320 746f 2060 6074  rresponds to ``t
-00012810: 6172 6765 745f 6d61 7070 696e 672e 7368  arget_mapping.sh
-00012820: 6170 655b 315d 6060 2e20 4966 2060 6074  ape[1]``. If ``t
-00012830: 6172 6765 745f 6d61 7070 696e 6760 6020  arget_mapping`` 
-00012840: 6973 2060 604e 6f6e 6560 602c 2074 6865  is ``None``, the
-00012850: 6e0a 2020 2020 2020 2020 2020 2020 6060  n.            ``
-00012860: 6e75 6d5f 7072 6564 6963 7460 6020 636f  num_predict`` co
-00012870: 7272 6573 706f 6e64 7320 746f 2060 6073  rresponds to ``s
-00012880: 6571 7565 6e63 655f 6c65 6e67 7468 6060  equence_length``
-00012890: 2e0a 2020 2020 2020 2020 7061 7374 5f62  ..        past_b
-000128a0: 7563 6b65 7473 5f73 7461 7465 7320 283a  uckets_states (:
-000128b0: 6f62 6a3a 604c 6973 745b 5475 706c 6528  obj:`List[Tuple(
-000128c0: 746f 7263 682e 4c6f 6e67 5465 6e73 6f72  torch.LongTensor
-000128d0: 2c20 746f 7263 682e 466c 6f61 7454 656e  , torch.FloatTen
-000128e0: 736f 7229 5d60 2c20 606f 7074 696f 6e61  sor)]`, `optiona
-000128f0: 6c60 2c20 7265 7475 726e 6564 2077 6865  l`, returned whe
-00012900: 6e20 6060 7573 655f 6361 6368 653d 5472  n ``use_cache=Tr
-00012910: 7565 6060 2069 7320 7061 7373 6564 206f  ue`` is passed o
-00012920: 7220 7768 656e 2060 6063 6f6e 6669 672e  r when ``config.
-00012930: 7573 655f 6361 6368 653d 5472 7565 6060  use_cache=True``
-00012940: 293a 0a20 2020 2020 2020 2020 2020 204c  ):.            L
-00012950: 6973 7420 6f66 203a 6f62 6a3a 6054 7570  ist of :obj:`Tup
-00012960: 6c65 2874 6f72 6368 2e4c 6f6e 6754 656e  le(torch.LongTen
-00012970: 736f 722c 2074 6f72 6368 2e46 6c6f 6174  sor, torch.Float
-00012980: 5465 6e73 6f72 6020 6f66 206c 656e 6774  Tensor` of lengt
-00012990: 6820 3a6f 626a 3a60 636f 6e66 6967 2e6e  h :obj:`config.n
-000129a0: 5f6c 6179 6572 7360 2c20 7769 7468 2074  _layers`, with t
-000129b0: 6865 2066 6972 7374 0a20 2020 2020 2020  he first.       
-000129c0: 2020 2020 2065 6c65 6d65 6e74 2062 6569       element bei
-000129d0: 6e67 2074 6865 2070 7265 7669 6f75 7320  ng the previous 
-000129e0: 6062 7563 6b65 7473 6020 6f66 2073 6861  `buckets` of sha
-000129f0: 7065 203a 6f62 6a3a 6028 6261 7463 685f  pe :obj:`(batch_
-00012a00: 7369 7a65 2c20 6e75 6d5f 6865 6164 732c  size, num_heads,
-00012a10: 206e 756d 5f68 6173 6865 732c 2073 6571   num_hashes, seq
-00012a20: 7565 6e63 655f 6c65 6e67 7468 2960 290a  uence_length)`).
-00012a30: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00012a40: 7468 6520 7365 636f 6e64 2062 6569 6e67  the second being
-00012a50: 2074 6865 2070 7265 7669 6f75 7320 6068   the previous `h
-00012a60: 6964 6465 6e5f 7374 6174 6573 6020 6f66  idden_states` of
-00012a70: 2073 6861 7065 203a 6f62 6a3a 6028 6261   shape :obj:`(ba
-00012a80: 7463 685f 7369 7a65 2c20 7365 7175 656e  tch_size, sequen
-00012a90: 6365 5f6c 656e 6774 682c 0a20 2020 2020  ce_length,.     
-00012aa0: 2020 2020 2020 2068 6964 6465 6e5f 7369         hidden_si
-00012ab0: 7a65 2960 292e 0a0a 2020 2020 2020 2020  ze)`)...        
-00012ac0: 2020 2020 436f 6e74 6169 6e73 2070 7265      Contains pre
-00012ad0: 636f 6d70 7574 6564 2062 7563 6b65 7473  computed buckets
-00012ae0: 2061 6e64 2068 6964 6465 6e2d 7374 6174   and hidden-stat
-00012af0: 6573 2074 6861 7420 6361 6e20 6265 2075  es that can be u
-00012b00: 7365 6420 2873 6565 2060 6070 6173 745f  sed (see ``past_
-00012b10: 6275 636b 6574 735f 7374 6174 6573 6060  buckets_states``
-00012b20: 2069 6e70 7574 2920 746f 0a20 2020 2020   input) to.     
-00012b30: 2020 2020 2020 2073 7065 6564 2075 7020         speed up 
-00012b40: 7365 7175 656e 7469 616c 2064 6563 6f64  sequential decod
-00012b50: 696e 672e 0a20 2020 2020 2020 2068 6964  ing..        hid
-00012b60: 6465 6e5f 7374 6174 6573 2028 3a6f 626a  den_states (:obj
-00012b70: 3a60 7475 706c 6528 746f 7263 682e 466c  :`tuple(torch.Fl
-00012b80: 6f61 7454 656e 736f 7229 602c 2060 6f70  oatTensor)`, `op
-00012b90: 7469 6f6e 616c 602c 2072 6574 7572 6e65  tional`, returne
-00012ba0: 6420 7768 656e 2060 606f 7574 7075 745f  d when ``output_
-00012bb0: 6869 6464 656e 5f73 7461 7465 733d 5472  hidden_states=Tr
-00012bc0: 7565 6060 2069 7320 7061 7373 6564 206f  ue`` is passed o
-00012bd0: 7220 7768 656e 2060 6063 6f6e 6669 672e  r when ``config.
-00012be0: 6f75 7470 7574 5f68 6964 6465 6e5f 7374  output_hidden_st
-00012bf0: 6174 6573 3d54 7275 6560 6029 3a0a 2020  ates=True``):.  
-00012c00: 2020 2020 2020 2020 2020 5475 706c 6520            Tuple 
-00012c10: 6f66 203a 6f62 6a3a 6074 6f72 6368 2e46  of :obj:`torch.F
-00012c20: 6c6f 6174 5465 6e73 6f72 6020 286f 6e65  loatTensor` (one
-00012c30: 2066 6f72 2074 6865 206f 7574 7075 7420   for the output 
-00012c40: 6f66 2074 6865 2065 6d62 6564 6469 6e67  of the embedding
-00012c50: 7320 616e 6420 6f6e 6520 666f 7220 7468  s and one for th
-00012c60: 6520 6f75 7470 7574 206f 6620 6561 6368  e output of each
-00012c70: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00012c80: 6572 2920 6f66 2073 6861 7065 203a 6f62  er) of shape :ob
-00012c90: 6a3a 6028 6261 7463 685f 7369 7a65 2c20  j:`(batch_size, 
-00012ca0: 7365 7175 656e 6365 5f6c 656e 6774 682c  sequence_length,
-00012cb0: 2068 6964 6465 6e5f 7369 7a65 2960 2e0a   hidden_size)`..
-00012cc0: 0a20 2020 2020 2020 2020 2020 2048 6964  .            Hid
-00012cd0: 6465 6e2d 7374 6174 6573 206f 6620 7468  den-states of th
-00012ce0: 6520 6d6f 6465 6c20 6174 2074 6865 206f  e model at the o
-00012cf0: 7574 7075 7420 6f66 2065 6163 6820 6c61  utput of each la
-00012d00: 7965 7220 706c 7573 2074 6865 2069 6e69  yer plus the ini
-00012d10: 7469 616c 2065 6d62 6564 6469 6e67 206f  tial embedding o
-00012d20: 7574 7075 7473 2e0a 2020 2020 2020 2020  utputs..        
-00012d30: 6174 7465 6e74 696f 6e73 2028 3a6f 626a  attentions (:obj
-00012d40: 3a60 7475 706c 6528 746f 7263 682e 466c  :`tuple(torch.Fl
-00012d50: 6f61 7454 656e 736f 7229 602c 2060 6f70  oatTensor)`, `op
-00012d60: 7469 6f6e 616c 602c 2072 6574 7572 6e65  tional`, returne
-00012d70: 6420 7768 656e 2060 606f 7574 7075 745f  d when ``output_
-00012d80: 6174 7465 6e74 696f 6e73 3d54 7275 6560  attentions=True`
-00012d90: 6020 6973 2070 6173 7365 6420 6f72 2077  ` is passed or w
-00012da0: 6865 6e20 6060 636f 6e66 6967 2e6f 7574  hen ``config.out
-00012db0: 7075 745f 6174 7465 6e74 696f 6e73 3d54  put_attentions=T
-00012dc0: 7275 6560 6029 3a0a 2020 2020 2020 2020  rue``):.        
-00012dd0: 2020 2020 5475 706c 6520 6f66 203a 6f62      Tuple of :ob
-00012de0: 6a3a 6074 6f72 6368 2e46 6c6f 6174 5465  j:`torch.FloatTe
-00012df0: 6e73 6f72 6020 286f 6e65 2066 6f72 2065  nsor` (one for e
-00012e00: 6163 6820 6c61 7965 7229 206f 6620 7368  ach layer) of sh
-00012e10: 6170 6520 3a6f 626a 3a60 2862 6174 6368  ape :obj:`(batch
-00012e20: 5f73 697a 652c 206e 756d 5f68 6561 6473  _size, num_heads
-00012e30: 2c0a 2020 2020 2020 2020 2020 2020 7365  ,.            se
-00012e40: 7175 656e 6365 5f6c 656e 6774 682c 2073  quence_length, s
-00012e50: 6571 7565 6e63 655f 6c65 6e67 7468 2960  equence_length)`
-00012e60: 2e0a 0a20 2020 2020 2020 2020 2020 2041  ...            A
-00012e70: 7474 656e 7469 6f6e 7320 7765 6967 6874  ttentions weight
-00012e80: 7320 6166 7465 7220 7468 6520 6174 7465  s after the atte
-00012e90: 6e74 696f 6e20 736f 6674 6d61 782c 2075  ntion softmax, u
-00012ea0: 7365 6420 746f 2063 6f6d 7075 7465 2074  sed to compute t
-00012eb0: 6865 2077 6569 6768 7465 6420 6176 6572  he weighted aver
-00012ec0: 6167 6520 696e 2074 6865 2073 656c 662d  age in the self-
-00012ed0: 6174 7465 6e74 696f 6e0a 2020 2020 2020  attention.      
-00012ee0: 2020 2020 2020 6865 6164 732e 0a20 2020        heads..   
-00012ef0: 2022 2222 0a0a 2020 2020 6c61 7374 5f68   """..    last_h
-00012f00: 6964 6465 6e5f 7374 6174 653a 2074 6f72  idden_state: tor
-00012f10: 6368 2e46 6c6f 6174 5465 6e73 6f72 0a20  ch.FloatTensor. 
-00012f20: 2020 2070 6173 745f 6275 636b 6574 735f     past_buckets_
-00012f30: 7374 6174 6573 3a20 4f70 7469 6f6e 616c  states: Optional
-00012f40: 5b4c 6973 745b 5475 706c 655b 746f 7263  [List[Tuple[torc
-00012f50: 682e 4c6f 6e67 5465 6e73 6f72 2c20 746f  h.LongTensor, to
-00012f60: 7263 682e 466c 6f61 7454 656e 736f 725d  rch.FloatTensor]
-00012f70: 5d5d 203d 204e 6f6e 650a 2020 2020 6869  ]] = None.    hi
-00012f80: 6464 656e 5f73 7461 7465 733a 204f 7074  dden_states: Opt
-00012f90: 696f 6e61 6c5b 5475 706c 655b 746f 7263  ional[Tuple[torc
-00012fa0: 682e 466c 6f61 7454 656e 736f 725d 5d20  h.FloatTensor]] 
-00012fb0: 3d20 4e6f 6e65 0a20 2020 2061 7474 656e  = None.    atten
-00012fc0: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-00012fd0: 5475 706c 655b 746f 7263 682e 466c 6f61  Tuple[torch.Floa
-00012fe0: 7454 656e 736f 725d 5d20 3d20 4e6f 6e65  tTensor]] = None
-00012ff0: 0a0a 0a40 6461 7461 636c 6173 730a 636c  ...@dataclass.cl
-00013000: 6173 7320 5265 666f 726d 6572 4d6f 6465  ass ReformerMode
-00013010: 6c57 6974 684c 4d48 6561 644f 7574 7075  lWithLMHeadOutpu
-00013020: 7428 4d6f 6465 6c4f 7574 7075 7429 3a0a  t(ModelOutput):.
-00013030: 2020 2020 2222 220a 2020 2020 4f75 7470      """.    Outp
-00013040: 7574 2074 7970 6520 6f66 203a 636c 6173  ut type of :clas
-00013050: 733a 607e 7472 616e 7366 6f72 6d65 7273  s:`~transformers
-00013060: 2e52 6566 6f72 6d65 724d 6f64 656c 5769  .ReformerModelWi
-00013070: 7468 4c4d 4865 6164 602e 0a0a 2020 2020  thLMHead`...    
-00013080: 4172 6773 3a0a 2020 2020 2020 2020 6c6f  Args:.        lo
-00013090: 7373 2028 3a6f 626a 3a60 746f 7263 682e  ss (:obj:`torch.
-000130a0: 466c 6f61 7454 656e 736f 7260 206f 6620  FloatTensor` of 
-000130b0: 7368 6170 6520 6028 312c 2960 2c20 606f  shape `(1,)`, `o
-000130c0: 7074 696f 6e61 6c60 2c20 7265 7475 726e  ptional`, return
-000130d0: 6564 2077 6865 6e20 6060 6c61 6265 6c73  ed when ``labels
-000130e0: 6060 2069 7320 7072 6f76 6964 6564 290a  `` is provided).
-000130f0: 2020 2020 2020 2020 2020 2020 4c61 6e67              Lang
-00013100: 7561 6765 206d 6f64 656c 696e 6720 6c6f  uage modeling lo
-00013110: 7373 2028 666f 7220 6e65 7874 2d74 6f6b  ss (for next-tok
-00013120: 656e 2070 7265 6469 6374 696f 6e29 2e0a  en prediction)..
-00013130: 2020 2020 2020 2020 6c6f 6769 7473 2028          logits (
-00013140: 3a6f 626a 3a60 746f 7263 682e 466c 6f61  :obj:`torch.Floa
-00013150: 7454 656e 736f 7260 206f 6620 7368 6170  tTensor` of shap
-00013160: 6520 3a6f 626a 3a60 2862 6174 6368 5f73  e :obj:`(batch_s
-00013170: 697a 652c 206e 756d 5f70 7265 6469 6374  ize, num_predict
-00013180: 2c20 636f 6e66 6967 2e76 6f63 6162 5f73  , config.vocab_s
-00013190: 697a 6529 6029 3a0a 2020 2020 2020 2020  ize)`):.        
-000131a0: 2020 2020 5072 6564 6963 7469 6f6e 2073      Prediction s
-000131b0: 636f 7265 7320 6f66 2074 6865 206c 616e  cores of the lan
-000131c0: 6775 6167 6520 6d6f 6465 6c69 6e67 2068  guage modeling h
-000131d0: 6561 6420 2873 636f 7265 7320 666f 7220  ead (scores for 
-000131e0: 6561 6368 2076 6f63 6162 756c 6172 7920  each vocabulary 
-000131f0: 746f 6b65 6e20 6265 666f 7265 2053 6f66  token before Sof
-00013200: 744d 6178 292e 0a0a 2020 2020 2020 2020  tMax)...        
-00013210: 2020 2020 6060 6e75 6d5f 7072 6564 6963      ``num_predic
-00013220: 7460 6020 636f 7272 6573 706f 6e64 7320  t`` corresponds 
-00013230: 746f 2060 6074 6172 6765 745f 6d61 7070  to ``target_mapp
-00013240: 696e 672e 7368 6170 655b 315d 6060 2e20  ing.shape[1]``. 
-00013250: 4966 2060 6074 6172 6765 745f 6d61 7070  If ``target_mapp
-00013260: 696e 6760 6020 6973 2060 604e 6f6e 6560  ing`` is ``None`
-00013270: 602c 2074 6865 6e0a 2020 2020 2020 2020  `, then.        
-00013280: 2020 2020 6060 6e75 6d5f 7072 6564 6963      ``num_predic
-00013290: 7460 6020 636f 7272 6573 706f 6e64 7320  t`` corresponds 
-000132a0: 746f 2060 6073 6571 7565 6e63 655f 6c65  to ``sequence_le
-000132b0: 6e67 7468 6060 2e0a 2020 2020 2020 2020  ngth``..        
-000132c0: 7061 7374 5f62 7563 6b65 7473 5f73 7461  past_buckets_sta
-000132d0: 7465 7320 283a 6f62 6a3a 604c 6973 745b  tes (:obj:`List[
-000132e0: 5475 706c 6528 746f 7263 682e 4c6f 6e67  Tuple(torch.Long
-000132f0: 5465 6e73 6f72 2c20 746f 7263 682e 466c  Tensor, torch.Fl
-00013300: 6f61 7454 656e 736f 7229 5d60 2c20 606f  oatTensor)]`, `o
-00013310: 7074 696f 6e61 6c60 2c20 7265 7475 726e  ptional`, return
-00013320: 6564 2077 6865 6e20 6060 7573 655f 6361  ed when ``use_ca
-00013330: 6368 653d 5472 7565 6060 2069 7320 7061  che=True`` is pa
-00013340: 7373 6564 206f 7220 7768 656e 2060 6063  ssed or when ``c
-00013350: 6f6e 6669 672e 7573 655f 6361 6368 653d  onfig.use_cache=
-00013360: 5472 7565 6060 293a 0a20 2020 2020 2020  True``):.       
-00013370: 2020 2020 204c 6973 7420 6f66 203a 6f62       List of :ob
-00013380: 6a3a 6054 7570 6c65 2874 6f72 6368 2e4c  j:`Tuple(torch.L
-00013390: 6f6e 6754 656e 736f 722c 2074 6f72 6368  ongTensor, torch
-000133a0: 2e46 6c6f 6174 5465 6e73 6f72 6020 6f66  .FloatTensor` of
-000133b0: 206c 656e 6774 6820 3a6f 626a 3a60 636f   length :obj:`co
-000133c0: 6e66 6967 2e6e 5f6c 6179 6572 7360 2c20  nfig.n_layers`, 
-000133d0: 7769 7468 2074 6865 2066 6972 7374 0a20  with the first. 
-000133e0: 2020 2020 2020 2020 2020 2065 6c65 6d65             eleme
-000133f0: 6e74 2062 6569 6e67 2074 6865 2070 7265  nt being the pre
-00013400: 7669 6f75 7320 6062 7563 6b65 7473 6020  vious `buckets` 
-00013410: 6f66 2073 6861 7065 203a 6f62 6a3a 6028  of shape :obj:`(
-00013420: 6261 7463 685f 7369 7a65 2c20 6e75 6d5f  batch_size, num_
-00013430: 6865 6164 732c 206e 756d 5f68 6173 6865  heads, num_hashe
-00013440: 732c 2073 6571 7565 6e63 655f 6c65 6e67  s, sequence_leng
-00013450: 7468 2960 290a 2020 2020 2020 2020 2020  th)`).          
-00013460: 2020 616e 6420 7468 6520 7365 636f 6e64    and the second
-00013470: 2062 6569 6e67 2074 6865 2070 7265 7669   being the previ
-00013480: 6f75 7320 6068 6964 6465 6e5f 7374 6174  ous `hidden_stat
-00013490: 6573 6020 6f66 2073 6861 7065 203a 6f62  es` of shape :ob
-000134a0: 6a3a 6028 6261 7463 685f 7369 7a65 2c20  j:`(batch_size, 
-000134b0: 7365 7175 656e 6365 5f6c 656e 6774 682c  sequence_length,
-000134c0: 0a20 2020 2020 2020 2020 2020 2068 6964  .            hid
-000134d0: 6465 6e5f 7369 7a65 2960 292e 0a0a 2020  den_size)`)...  
-000134e0: 2020 2020 2020 2020 2020 436f 6e74 6169            Contai
-000134f0: 6e73 2070 7265 636f 6d70 7574 6564 2062  ns precomputed b
-00013500: 7563 6b65 7473 2061 6e64 2068 6964 6465  uckets and hidde
-00013510: 6e2d 7374 6174 6573 2074 6861 7420 6361  n-states that ca
-00013520: 6e20 6265 2075 7365 6420 2873 6565 2060  n be used (see `
-00013530: 6070 6173 745f 6275 636b 6574 735f 7374  `past_buckets_st
-00013540: 6174 6573 6060 2069 6e70 7574 2920 746f  ates`` input) to
-00013550: 0a20 2020 2020 2020 2020 2020 2073 7065  .            spe
-00013560: 6564 2075 7020 7365 7175 656e 7469 616c  ed up sequential
-00013570: 2064 6563 6f64 696e 672e 0a20 2020 2020   decoding..     
-00013580: 2020 2068 6964 6465 6e5f 7374 6174 6573     hidden_states
-00013590: 2028 3a6f 626a 3a60 7475 706c 6528 746f   (:obj:`tuple(to
-000135a0: 7263 682e 466c 6f61 7454 656e 736f 7229  rch.FloatTensor)
-000135b0: 602c 2060 6f70 7469 6f6e 616c 602c 2072  `, `optional`, r
-000135c0: 6574 7572 6e65 6420 7768 656e 2060 606f  eturned when ``o
-000135d0: 7574 7075 745f 6869 6464 656e 5f73 7461  utput_hidden_sta
-000135e0: 7465 733d 5472 7565 6060 2069 7320 7061  tes=True`` is pa
-000135f0: 7373 6564 206f 7220 7768 656e 2060 6063  ssed or when ``c
-00013600: 6f6e 6669 672e 6f75 7470 7574 5f68 6964  onfig.output_hid
-00013610: 6465 6e5f 7374 6174 6573 3d54 7275 6560  den_states=True`
-00013620: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-00013630: 5454 7570 6c65 206f 6620 3a6f 626a 3a60  TTuple of :obj:`
-00013640: 746f 7263 682e 466c 6f61 7454 656e 736f  torch.FloatTenso
-00013650: 7260 2028 6f6e 6520 666f 7220 7468 6520  r` (one for the 
-00013660: 6f75 7470 7574 206f 6620 7468 6520 656d  output of the em
-00013670: 6265 6464 696e 6773 2061 6e64 206f 6e65  beddings and one
-00013680: 2066 6f72 2074 6865 206f 7574 7075 7420   for the output 
-00013690: 6f66 2065 6163 680a 2020 2020 2020 2020  of each.        
-000136a0: 2020 2020 6c61 7965 7229 206f 6620 7368      layer) of sh
-000136b0: 6170 6520 3a6f 626a 3a60 2862 6174 6368  ape :obj:`(batch
-000136c0: 5f73 697a 652c 2073 6571 7565 6e63 655f  _size, sequence_
-000136d0: 6c65 6e67 7468 2c20 6869 6464 656e 5f73  length, hidden_s
-000136e0: 697a 6529 602e 0a0a 2020 2020 2020 2020  ize)`...        
-000136f0: 2020 2020 4869 6464 656e 2d73 7461 7465      Hidden-state
-00013700: 7320 6f66 2074 6865 206d 6f64 656c 2061  s of the model a
-00013710: 7420 7468 6520 6f75 7470 7574 206f 6620  t the output of 
-00013720: 6561 6368 206c 6179 6572 2070 6c75 7320  each layer plus 
-00013730: 7468 6520 696e 6974 6961 6c20 656d 6265  the initial embe
-00013740: 6464 696e 6720 6f75 7470 7574 732e 0a20  dding outputs.. 
-00013750: 2020 2020 2020 2061 7474 656e 7469 6f6e         attention
-00013760: 7320 283a 6f62 6a3a 6074 7570 6c65 2874  s (:obj:`tuple(t
-00013770: 6f72 6368 2e46 6c6f 6174 5465 6e73 6f72  orch.FloatTensor
-00013780: 2960 2c20 606f 7074 696f 6e61 6c60 2c20  )`, `optional`, 
-00013790: 7265 7475 726e 6564 2077 6865 6e20 6060  returned when ``
-000137a0: 6f75 7470 7574 5f61 7474 656e 7469 6f6e  output_attention
-000137b0: 733d 5472 7565 6060 2069 7320 7061 7373  s=True`` is pass
-000137c0: 6564 206f 7220 7768 656e 2060 6063 6f6e  ed or when ``con
-000137d0: 6669 672e 6f75 7470 7574 5f61 7474 656e  fig.output_atten
-000137e0: 7469 6f6e 733d 5472 7565 6060 293a 0a20  tions=True``):. 
-000137f0: 2020 2020 2020 2020 2020 2054 7570 6c65             Tuple
-00013800: 206f 6620 3a6f 626a 3a60 746f 7263 682e   of :obj:`torch.
-00013810: 466c 6f61 7454 656e 736f 7260 2028 6f6e  FloatTensor` (on
-00013820: 6520 666f 7220 6561 6368 206c 6179 6572  e for each layer
-00013830: 2920 6f66 2073 6861 7065 203a 6f62 6a3a  ) of shape :obj:
-00013840: 6028 6261 7463 685f 7369 7a65 2c20 6e75  `(batch_size, nu
-00013850: 6d5f 6865 6164 732c 0a20 2020 2020 2020  m_heads,.       
-00013860: 2020 2020 2073 6571 7565 6e63 655f 6c65       sequence_le
-00013870: 6e67 7468 2c20 7365 7175 656e 6365 5f6c  ngth, sequence_l
-00013880: 656e 6774 6829 602e 0a0a 2020 2020 2020  ength)`...      
-00013890: 2020 2020 2020 4174 7465 6e74 696f 6e73        Attentions
-000138a0: 2077 6569 6768 7473 2061 6674 6572 2074   weights after t
-000138b0: 6865 2061 7474 656e 7469 6f6e 2073 6f66  he attention sof
-000138c0: 746d 6178 2c20 7573 6564 2074 6f20 636f  tmax, used to co
-000138d0: 6d70 7574 6520 7468 6520 7765 6967 6874  mpute the weight
-000138e0: 6564 2061 7665 7261 6765 2069 6e20 7468  ed average in th
-000138f0: 6520 7365 6c66 2d61 7474 656e 7469 6f6e  e self-attention
-00013900: 0a20 2020 2020 2020 2020 2020 2068 6561  .            hea
-00013910: 6473 2e0a 2020 2020 2222 220a 0a20 2020  ds..    """..   
-00013920: 206c 6f73 733a 204f 7074 696f 6e61 6c5b   loss: Optional[
-00013930: 746f 7263 682e 466c 6f61 7454 656e 736f  torch.FloatTenso
-00013940: 725d 203d 204e 6f6e 650a 2020 2020 6c6f  r] = None.    lo
-00013950: 6769 7473 3a20 746f 7263 682e 466c 6f61  gits: torch.Floa
-00013960: 7454 656e 736f 7220 3d20 4e6f 6e65 0a20  tTensor = None. 
-00013970: 2020 2070 6173 745f 6275 636b 6574 735f     past_buckets_
-00013980: 7374 6174 6573 3a20 4f70 7469 6f6e 616c  states: Optional
-00013990: 5b4c 6973 745b 5475 706c 655b 746f 7263  [List[Tuple[torc
-000139a0: 682e 4c6f 6e67 5465 6e73 6f72 2c20 746f  h.LongTensor, to
-000139b0: 7263 682e 466c 6f61 7454 656e 736f 725d  rch.FloatTensor]
-000139c0: 5d5d 203d 204e 6f6e 650a 2020 2020 6869  ]] = None.    hi
-000139d0: 6464 656e 5f73 7461 7465 733a 204f 7074  dden_states: Opt
-000139e0: 696f 6e61 6c5b 5475 706c 655b 746f 7263  ional[Tuple[torc
-000139f0: 682e 466c 6f61 7454 656e 736f 725d 5d20  h.FloatTensor]] 
-00013a00: 3d20 4e6f 6e65 0a20 2020 2061 7474 656e  = None.    atten
-00013a10: 7469 6f6e 733a 204f 7074 696f 6e61 6c5b  tions: Optional[
-00013a20: 5475 706c 655b 746f 7263 682e 466c 6f61  Tuple[torch.Floa
-00013a30: 7454 656e 736f 725d 5d20 3d20 4e6f 6e65  tTensor]] = None
-00013a40: 0a0a 0a52 4546 4f52 4d45 525f 5354 4152  ...REFORMER_STAR
-00013a50: 545f 444f 4353 5452 494e 4720 3d20 7222  T_DOCSTRING = r"
-00013a60: 2222 0a20 2020 2052 6566 6f72 6d65 7220  "".    Reformer 
-00013a70: 7761 7320 7072 6f70 6f73 6564 2069 6e20  was proposed in 
-00013a80: 6052 6566 6f72 6d65 723a 2054 6865 2045  `Reformer: The E
-00013a90: 6666 6963 6965 6e74 2054 7261 6e73 666f  fficient Transfo
-00013aa0: 726d 6572 203c 6874 7470 733a 2f2f 6172  rmer <https://ar
-00013ab0: 7869 762e 6f72 672f 6162 732f 3230 3031  xiv.org/abs/2001
-00013ac0: 2e30 3434 3531 3e60 5f5f 2062 7920 4e69  .04451>`__ by Ni
-00013ad0: 6b69 7461 0a20 2020 204b 6974 6165 762c  kita.    Kitaev,
-00013ae0: 20c5 8175 6b61 737a 204b 6169 7365 722c   ..ukasz Kaiser,
-00013af0: 2041 6e73 656c 6d20 4c65 7673 6b61 7961   Anselm Levskaya
-00013b00: 2e0a 0a20 2020 2054 6869 7320 6d6f 6465  ...    This mode
-00013b10: 6c20 696e 6865 7269 7473 2066 726f 6d20  l inherits from 
-00013b20: 3a63 6c61 7373 3a60 7e74 7261 6e73 666f  :class:`~transfo
-00013b30: 726d 6572 732e 5072 6554 7261 696e 6564  rmers.PreTrained
-00013b40: 4d6f 6465 6c60 2e20 4368 6563 6b20 7468  Model`. Check th
-00013b50: 6520 7375 7065 7263 6c61 7373 2064 6f63  e superclass doc
-00013b60: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
-00013b70: 6865 2067 656e 6572 6963 0a20 2020 206d  he generic.    m
-00013b80: 6574 686f 6473 2074 6865 206c 6962 7261  ethods the libra
-00013b90: 7279 2069 6d70 6c65 6d65 6e74 7320 666f  ry implements fo
-00013ba0: 7220 616c 6c20 6974 7320 6d6f 6465 6c20  r all its model 
-00013bb0: 2873 7563 6820 6173 2064 6f77 6e6c 6f61  (such as downloa
-00013bc0: 6469 6e67 206f 7220 7361 7669 6e67 2c20  ding or saving, 
-00013bd0: 7265 7369 7a69 6e67 2074 6865 2069 6e70  resizing the inp
-00013be0: 7574 2065 6d62 6564 6469 6e67 732c 0a20  ut embeddings,. 
-00013bf0: 2020 2070 7275 6e69 6e67 2068 6561 6473     pruning heads
-00013c00: 2065 7463 2e29 0a0a 2020 2020 5468 6973   etc.)..    This
-00013c10: 206d 6f64 656c 2069 7320 616c 736f 2061   model is also a
-00013c20: 2050 7954 6f72 6368 2060 746f 7263 682e   PyTorch `torch.
-00013c30: 6e6e 2e4d 6f64 756c 6520 3c68 7474 7073  nn.Module <https
-00013c40: 3a2f 2f70 7974 6f72 6368 2e6f 7267 2f64  ://pytorch.org/d
-00013c50: 6f63 732f 7374 6162 6c65 2f6e 6e2e 6874  ocs/stable/nn.ht
-00013c60: 6d6c 2374 6f72 6368 2e6e 6e2e 4d6f 6475  ml#torch.nn.Modu
-00013c70: 6c65 3e60 5f5f 0a20 2020 2073 7562 636c  le>`__.    subcl
-00013c80: 6173 732e 2055 7365 2069 7420 6173 2061  ass. Use it as a
-00013c90: 2072 6567 756c 6172 2050 7954 6f72 6368   regular PyTorch
-00013ca0: 204d 6f64 756c 6520 616e 6420 7265 6665   Module and refe
-00013cb0: 7220 746f 2074 6865 2050 7954 6f72 6368  r to the PyTorch
-00013cc0: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
-00013cd0: 6f72 2061 6c6c 206d 6174 7465 7220 7265  or all matter re
-00013ce0: 6c61 7465 6420 746f 0a20 2020 2067 656e  lated to.    gen
-00013cf0: 6572 616c 2075 7361 6765 2061 6e64 2062  eral usage and b
-00013d00: 6568 6176 696f 722e 0a0a 2020 2020 5061  ehavior...    Pa
-00013d10: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00013d20: 2020 636f 6e66 6967 2028 3a63 6c61 7373    config (:class
-00013d30: 3a60 7e74 7261 6e73 666f 726d 6572 732e  :`~transformers.
-00013d40: 5265 666f 726d 6572 436f 6e66 6967 6029  ReformerConfig`)
-00013d50: 3a20 4d6f 6465 6c20 636f 6e66 6967 7572  : Model configur
-00013d60: 6174 696f 6e20 636c 6173 7320 7769 7468  ation class with
-00013d70: 2061 6c6c 2074 6865 2070 6172 616d 6574   all the paramet
-00013d80: 6572 7320 6f66 2074 6865 206d 6f64 656c  ers of the model
-00013d90: 2e0a 2020 2020 2020 2020 2020 2020 496e  ..            In
-00013da0: 6974 6961 6c69 7a69 6e67 2077 6974 6820  itializing with 
-00013db0: 6120 636f 6e66 6967 2066 696c 6520 646f  a config file do
-00013dc0: 6573 206e 6f74 206c 6f61 6420 7468 6520  es not load the 
-00013dd0: 7765 6967 6874 7320 6173 736f 6369 6174  weights associat
-00013de0: 6564 2077 6974 6820 7468 6520 6d6f 6465  ed with the mode
-00013df0: 6c2c 206f 6e6c 7920 7468 650a 2020 2020  l, only the.    
-00013e00: 2020 2020 2020 2020 636f 6e66 6967 7572          configur
-00013e10: 6174 696f 6e2e 2043 6865 636b 206f 7574  ation. Check out
-00013e20: 2074 6865 203a 6d65 7468 3a60 7e74 7261   the :meth:`~tra
-00013e30: 6e73 666f 726d 6572 732e 5072 6554 7261  nsformers.PreTra
-00013e40: 696e 6564 4d6f 6465 6c2e 6672 6f6d 5f70  inedModel.from_p
-00013e50: 7265 7472 6169 6e65 6460 206d 6574 686f  retrained` metho
-00013e60: 6420 746f 206c 6f61 6420 7468 6520 6d6f  d to load the mo
-00013e70: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00013e80: 7765 6967 6874 732e 0a22 2222 0a0a 5245  weights.."""..RE
-00013e90: 464f 524d 4552 5f49 4e50 5554 535f 444f  FORMER_INPUTS_DO
-00013ea0: 4353 5452 494e 4720 3d20 7222 2222 0a20  CSTRING = r""". 
-00013eb0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00013ec0: 2069 6e70 7574 5f69 6473 2028 3a6f 626a   input_ids (:obj
-00013ed0: 3a60 746f 7263 682e 4c6f 6e67 5465 6e73  :`torch.LongTens
-00013ee0: 6f72 6020 6f66 2073 6861 7065 203a 6f62  or` of shape :ob
-00013ef0: 6a3a 6028 6261 7463 685f 7369 7a65 2c20  j:`(batch_size, 
-00013f00: 7365 7175 656e 6365 5f6c 656e 6774 6829  sequence_length)
-00013f10: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-00013f20: 496e 6469 6365 7320 6f66 2069 6e70 7574  Indices of input
-00013f30: 2073 6571 7565 6e63 6520 746f 6b65 6e73   sequence tokens
-00013f40: 2069 6e20 7468 6520 766f 6361 6275 6c61   in the vocabula
-00013f50: 7279 2e20 4475 7269 6e67 2074 7261 696e  ry. During train
-00013f60: 696e 6720 7468 6520 696e 7075 745f 6964  ing the input_id
-00013f70: 7320 7365 7175 656e 6365 5f6c 656e 6774  s sequence_lengt
-00013f80: 6820 6861 7320 746f 2062 650a 2020 2020  h has to be.    
-00013f90: 2020 2020 2020 2020 6120 6d75 6c74 6970          a multip
-00013fa0: 6c65 206f 6620 7468 6520 7265 6c65 7661  le of the releva
-00013fb0: 6e74 206d 6f64 656c 2773 2063 6875 6e6b  nt model's chunk
-00013fc0: 206c 656e 6774 6873 2028 6c73 6827 732c   lengths (lsh's,
-00013fd0: 206c 6f63 616c 2773 206f 7220 626f 7468   local's or both
-00013fe0: 292e 2044 7572 696e 6720 6576 616c 7561  ). During evalua
-00013ff0: 7469 6f6e 2c20 7468 6520 696e 6469 6365  tion, the indice
-00014000: 730a 2020 2020 2020 2020 2020 2020 6172  s.            ar
-00014010: 6520 6175 746f 6d61 7469 6361 6c6c 7920  e automatically 
-00014020: 7061 6464 6564 2074 6f20 6265 2061 206d  padded to be a m
-00014030: 756c 7469 706c 6520 6f66 2074 6865 2063  ultiple of the c
-00014040: 6875 6e6b 206c 656e 6774 682e 0a0a 2020  hunk length...  
-00014050: 2020 2020 2020 2020 2020 496e 6469 6365            Indice
-00014060: 7320 6361 6e20 6265 206f 6274 6169 6e65  s can be obtaine
-00014070: 6420 7573 696e 6720 3a63 6c61 7373 3a60  d using :class:`
-00014080: 7e74 7261 6e73 666f 726d 6572 732e 5265  ~transformers.Re
-00014090: 666f 726d 6572 546f 6b65 6e69 7a65 7260  formerTokenizer`
-000140a0: 2e20 5365 650a 2020 2020 2020 2020 2020  . See.          
-000140b0: 2020 3a6d 6574 683a 6074 7261 6e73 666f    :meth:`transfo
-000140c0: 726d 6572 732e 5072 6554 7261 696e 6564  rmers.PreTrained
-000140d0: 546f 6b65 6e69 7a65 722e 656e 636f 6465  Tokenizer.encode
-000140e0: 6020 616e 6420 3a6d 6574 683a 6074 7261  ` and :meth:`tra
-000140f0: 6e73 666f 726d 6572 732e 5072 6554 7261  nsformers.PreTra
-00014100: 696e 6564 546f 6b65 6e69 7a65 722e 5f5f  inedTokenizer.__
-00014110: 6361 6c6c 5f5f 6020 666f 720a 2020 2020  call__` for.    
-00014120: 2020 2020 2020 2020 6465 7461 696c 732e          details.
-00014130: 0a0a 2020 2020 2020 2020 2020 2020 6057  ..            `W
-00014140: 6861 7420 6172 6520 696e 7075 7420 4944  hat are input ID
-00014150: 733f 203c 2e2e 2f67 6c6f 7373 6172 792e  s? <../glossary.
-00014160: 6874 6d6c 2369 6e70 7574 2d69 6473 3e60  html#input-ids>`
-00014170: 5f5f 0a20 2020 2020 2020 2061 7474 656e  __.        atten
-00014180: 7469 6f6e 5f6d 6173 6b20 283a 6f62 6a3a  tion_mask (:obj:
-00014190: 6074 6f72 6368 2e46 6c6f 6174 5465 6e73  `torch.FloatTens
-000141a0: 6f72 6020 6f66 2073 6861 7065 203a 6f62  or` of shape :ob
-000141b0: 6a3a 6028 6261 7463 685f 7369 7a65 2c20  j:`(batch_size, 
-000141c0: 7365 7175 656e 6365 5f6c 656e 6774 6829  sequence_length)
-000141d0: 602c 2060 6f70 7469 6f6e 616c 6029 3a0a  `, `optional`):.
-000141e0: 2020 2020 2020 2020 2020 2020 4d61 736b              Mask
-000141f0: 2074 6f20 6176 6f69 6420 7065 7266 6f72   to avoid perfor
-00014200: 6d69 6e67 2061 7474 656e 7469 6f6e 206f  ming attention o
-00014210: 6e20 7061 6464 696e 6720 746f 6b65 6e20  n padding token 
-00014220: 696e 6469 6365 732e 204d 6173 6b20 7661  indices. Mask va
-00014230: 6c75 6573 2073 656c 6563 7465 6420 696e  lues selected in
-00014240: 2060 605b 302c 2031 5d60 603a 0a0a 2020   ``[0, 1]``:..  
-00014250: 2020 2020 2020 2020 2020 2d20 3120 666f            - 1 fo
-00014260: 7220 746f 6b65 6e73 2074 6861 7420 6172  r tokens that ar
-00014270: 6520 2a2a 6e6f 7420 6d61 736b 6564 2a2a  e **not masked**
-00014280: 2c0a 2020 2020 2020 2020 2020 2020 2d20  ,.            - 
-00014290: 3020 666f 7220 746f 6b65 6e73 2074 6861  0 for tokens tha
-000142a0: 7420 6172 6520 2a2a 6d61 736b 6564 2a2a  t are **masked**
-000142b0: 2e0a 0a20 2020 2020 2020 2020 2020 2060  ...            `
-000142c0: 5768 6174 2061 7265 2061 7474 656e 7469  What are attenti
-000142d0: 6f6e 206d 6173 6b73 3f20 3c2e 2e2f 676c  on masks? <../gl
-000142e0: 6f73 7361 7279 2e68 746d 6c23 6174 7465  ossary.html#atte
-000142f0: 6e74 696f 6e2d 6d61 736b 3e60 5f5f 0a20  ntion-mask>`__. 
-00014300: 2020 2020 2020 2070 6f73 6974 696f 6e5f         position_
-00014310: 6964 7320 283a 6f62 6a3a 6074 6f72 6368  ids (:obj:`torch
-00014320: 2e4c 6f6e 6754 656e 736f 7260 206f 6620  .LongTensor` of 
-00014330: 7368 6170 6520 3a6f 626a 3a60 2862 6174  shape :obj:`(bat
-00014340: 6368 5f73 697a 652c 2073 6571 7565 6e63  ch_size, sequenc
-00014350: 655f 6c65 6e67 7468 2960 2c20 606f 7074  e_length)`, `opt
-00014360: 696f 6e61 6c60 293a 0a20 2020 2020 2020  ional`):.       
-00014370: 2020 2020 2049 6e64 6963 6573 206f 6620       Indices of 
-00014380: 706f 7369 7469 6f6e 7320 6f66 2065 6163  positions of eac
-00014390: 6820 696e 7075 7420 7365 7175 656e 6365  h input sequence
-000143a0: 2074 6f6b 656e 7320 696e 2074 6865 2070   tokens in the p
-000143b0: 6f73 6974 696f 6e20 656d 6265 6464 696e  osition embeddin
-000143c0: 6773 2e20 5365 6c65 6374 6564 2069 6e20  gs. Selected in 
-000143d0: 7468 6520 7261 6e67 6520 6060 5b30 2c0a  the range ``[0,.
-000143e0: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-000143f0: 6967 2e6d 6178 5f70 6f73 6974 696f 6e5f  ig.max_position_
-00014400: 656d 6265 6464 696e 6773 202d 2031 5d60  embeddings - 1]`
-00014410: 602e 0a0a 2020 2020 2020 2020 2020 2020  `...            
-00014420: 6057 6861 7420 6172 6520 706f 7369 7469  `What are positi
-00014430: 6f6e 2049 4473 3f20 3c2e 2e2f 676c 6f73  on IDs? <../glos
-00014440: 7361 7279 2e68 746d 6c23 706f 7369 7469  sary.html#positi
-00014450: 6f6e 2d69 6473 3e60 5f5f 0a20 2020 2020  on-ids>`__.     
-00014460: 2020 2068 6561 645f 6d61 736b 2028 3a6f     head_mask (:o
-00014470: 626a 3a60 746f 7263 682e 466c 6f61 7454  bj:`torch.FloatT
-00014480: 656e 736f 7260 206f 6620 7368 6170 6520  ensor` of shape 
-00014490: 3a6f 626a 3a60 286e 756d 5f68 6561 6473  :obj:`(num_heads
-000144a0: 2c29 6020 6f72 203a 6f62 6a3a 6028 6e75  ,)` or :obj:`(nu
-000144b0: 6d5f 6c61 7965 7273 2c20 6e75 6d5f 6865  m_layers, num_he
-000144c0: 6164 7329 602c 2060 6f70 7469 6f6e 616c  ads)`, `optional
-000144d0: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-000144e0: 4d61 736b 2074 6f20 6e75 6c6c 6966 7920  Mask to nullify 
-000144f0: 7365 6c65 6374 6564 2068 6561 6473 206f  selected heads o
-00014500: 6620 7468 6520 7365 6c66 2d61 7474 656e  f the self-atten
-00014510: 7469 6f6e 206d 6f64 756c 6573 2e20 4d61  tion modules. Ma
-00014520: 736b 2076 616c 7565 7320 7365 6c65 6374  sk values select
-00014530: 6564 2069 6e20 6060 5b30 2c20 315d 6060  ed in ``[0, 1]``
-00014540: 3a0a 0a20 2020 2020 2020 2020 2020 202d  :..            -
-00014550: 2031 2069 6e64 6963 6174 6573 2074 6865   1 indicates the
-00014560: 2068 6561 6420 6973 202a 2a6e 6f74 206d   head is **not m
-00014570: 6173 6b65 642a 2a2c 0a20 2020 2020 2020  asked**,.       
-00014580: 2020 2020 202d 2030 2069 6e64 6963 6174       - 0 indicat
-00014590: 6573 2074 6865 2068 6561 6420 6973 202a  es the head is *
-000145a0: 2a6d 6173 6b65 642a 2a2e 0a0a 2020 2020  *masked**...    
-000145b0: 2020 2020 696e 7075 7473 5f65 6d62 6564      inputs_embed
-000145c0: 7320 283a 6f62 6a3a 6074 6f72 6368 2e46  s (:obj:`torch.F
-000145d0: 6c6f 6174 5465 6e73 6f72 6020 6f66 2073  loatTensor` of s
-000145e0: 6861 7065 203a 6f62 6a3a 6028 6261 7463  hape :obj:`(batc
-000145f0: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
-00014600: 5f6c 656e 6774 682c 2068 6964 6465 6e5f  _length, hidden_
-00014610: 7369 7a65 2960 2c20 606f 7074 696f 6e61  size)`, `optiona
-00014620: 6c60 293a 0a20 2020 2020 2020 2020 2020  l`):.           
-00014630: 204f 7074 696f 6e61 6c6c 792c 2069 6e73   Optionally, ins
-00014640: 7465 6164 206f 6620 7061 7373 696e 6720  tead of passing 
-00014650: 3a6f 626a 3a60 696e 7075 745f 6964 7360  :obj:`input_ids`
-00014660: 2079 6f75 2063 616e 2063 686f 6f73 6520   you can choose 
-00014670: 746f 2064 6972 6563 746c 7920 7061 7373  to directly pass
-00014680: 2061 6e20 656d 6265 6464 6564 2072 6570   an embedded rep
-00014690: 7265 7365 6e74 6174 696f 6e2e 0a20 2020  resentation..   
-000146a0: 2020 2020 2020 2020 2054 6869 7320 6973           This is
-000146b0: 2075 7365 6675 6c20 6966 2079 6f75 2077   useful if you w
-000146c0: 616e 7420 6d6f 7265 2063 6f6e 7472 6f6c  ant more control
-000146d0: 206f 7665 7220 686f 7720 746f 2063 6f6e   over how to con
-000146e0: 7665 7274 203a 6f62 6a3a 6069 6e70 7574  vert :obj:`input
-000146f0: 5f69 6473 6020 696e 6469 6365 7320 696e  _ids` indices in
-00014700: 746f 2061 7373 6f63 6961 7465 640a 2020  to associated.  
-00014710: 2020 2020 2020 2020 2020 7665 6374 6f72            vector
-00014720: 7320 7468 616e 2074 6865 206d 6f64 656c  s than the model
-00014730: 2773 2069 6e74 6572 6e61 6c20 656d 6265  's internal embe
-00014740: 6464 696e 6720 6c6f 6f6b 7570 206d 6174  dding lookup mat
-00014750: 7269 782e 0a20 2020 2020 2020 206e 756d  rix..        num
-00014760: 5f68 6173 6865 7320 283a 6f62 6a3a 6069  _hashes (:obj:`i
-00014770: 6e74 602c 2060 6f70 7469 6f6e 616c 6029  nt`, `optional`)
-00014780: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
-00014790: 6520 6e75 6d62 6572 206f 6620 6861 7368  e number of hash
-000147a0: 696e 6720 726f 756e 6473 2074 6861 7420  ing rounds that 
-000147b0: 7368 6f75 6c64 2062 6520 7065 7266 6f72  should be perfor
-000147c0: 6d65 6420 6475 7269 6e67 2062 7563 6b65  med during bucke
-000147d0: 7469 6e67 2e20 5365 7474 696e 6720 7468  ting. Setting th
-000147e0: 6973 2061 7267 756d 656e 7420 6f76 6572  is argument over
-000147f0: 7772 6974 6573 0a20 2020 2020 2020 2020  writes.         
-00014800: 2020 2074 6865 2064 6566 6175 6c74 2064     the default d
-00014810: 6566 696e 6564 2069 6e20 3a6f 626a 3a60  efined in :obj:`
-00014820: 636f 6e66 6967 2e6e 756d 5f68 6173 6865  config.num_hashe
-00014830: 7360 2e0a 0a20 2020 2020 2020 2020 2020  s`...           
-00014840: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
-00014850: 6174 696f 6e2c 2073 6565 203a 6f62 6a3a  ation, see :obj:
-00014860: 606e 756d 5f68 6173 6865 7360 2069 6e20  `num_hashes` in 
-00014870: 3a63 6c61 7373 3a60 7e74 7261 6e73 666f  :class:`~transfo
-00014880: 726d 6572 732e 5265 666f 726d 6572 436f  rmers.ReformerCo
-00014890: 6e66 6967 602e 0a20 2020 2020 2020 2070  nfig`..        p
-000148a0: 6173 745f 6275 636b 6574 735f 7374 6174  ast_buckets_stat
-000148b0: 6573 2028 3a6f 626a 3a60 4c69 7374 5b54  es (:obj:`List[T
-000148c0: 7570 6c65 2874 6f72 6368 2e4c 6f6e 6754  uple(torch.LongT
-000148d0: 656e 736f 722c 2074 6f72 6368 2e46 6c6f  ensor, torch.Flo
-000148e0: 6174 5465 6e73 6f72 295d 602c 2060 6f70  atTensor)]`, `op
-000148f0: 7469 6f6e 616c 6029 3a0a 2020 2020 2020  tional`):.      
-00014900: 2020 2020 2020 4c69 7374 206f 6620 3a6f        List of :o
-00014910: 626a 3a60 5475 706c 6528 746f 7263 682e  bj:`Tuple(torch.
-00014920: 4c6f 6e67 5465 6e73 6f72 2c20 746f 7263  LongTensor, torc
-00014930: 682e 466c 6f61 7454 656e 736f 7260 206f  h.FloatTensor` o
-00014940: 6620 6c65 6e67 7468 203a 6f62 6a3a 6063  f length :obj:`c
-00014950: 6f6e 6669 672e 6e5f 6c61 7965 7273 602c  onfig.n_layers`,
-00014960: 2077 6974 6820 7468 6520 6669 7273 740a   with the first.
-00014970: 2020 2020 2020 2020 2020 2020 656c 656d              elem
-00014980: 656e 7420 6265 696e 6720 7468 6520 7072  ent being the pr
-00014990: 6576 696f 7573 2060 6275 636b 6574 7360  evious `buckets`
-000149a0: 206f 6620 7368 6170 6520 3a6f 626a 3a60   of shape :obj:`
-000149b0: 2862 6174 6368 5f73 697a 652c 206e 756d  (batch_size, num
-000149c0: 5f68 6561 6473 2c20 6e75 6d5f 6861 7368  _heads, num_hash
-000149d0: 6573 2c20 7365 7175 656e 6365 5f6c 656e  es, sequence_len
-000149e0: 6774 6829 6029 0a20 2020 2020 2020 2020  gth)`).         
-000149f0: 2020 2061 6e64 2074 6865 2073 6563 6f6e     and the secon
-00014a00: 6420 6265 696e 6720 7468 6520 7072 6576  d being the prev
-00014a10: 696f 7573 2060 6869 6464 656e 5f73 7461  ious `hidden_sta
-00014a20: 7465 7360 206f 6620 7368 6170 6520 3a6f  tes` of shape :o
-00014a30: 626a 3a60 2862 6174 6368 5f73 697a 652c  bj:`(batch_size,
-00014a40: 2073 6571 7565 6e63 655f 6c65 6e67 7468   sequence_length
-00014a50: 2c0a 2020 2020 2020 2020 2020 2020 6869  ,.            hi
-00014a60: 6464 656e 5f73 697a 6529 6029 2e0a 0a20  dden_size)`)... 
-00014a70: 2020 2020 2020 2020 2020 2043 6f6e 7461             Conta
-00014a80: 696e 7320 7072 6563 6f6d 7075 7465 6420  ins precomputed 
-00014a90: 6869 6464 656e 2d73 7461 7465 7320 616e  hidden-states an
-00014aa0: 6420 6275 636b 6574 7320 286f 6e6c 7920  d buckets (only 
-00014ab0: 7265 6c65 7661 6e74 2066 6f72 204c 5348  relevant for LSH
-00014ac0: 2053 656c 662d 4174 7465 6e74 696f 6e29   Self-Attention)
-00014ad0: 2e20 4361 6e20 6265 2075 7365 6420 746f  . Can be used to
-00014ae0: 2073 7065 6564 0a20 2020 2020 2020 2020   speed.         
-00014af0: 2020 2075 7020 7365 7175 656e 7469 616c     up sequential
-00014b00: 2064 6563 6f64 696e 672e 0a20 2020 2020   decoding..     
-00014b10: 2020 2075 7365 5f63 6163 6865 2028 3a6f     use_cache (:o
-00014b20: 626a 3a60 626f 6f6c 602c 2060 6f70 7469  bj:`bool`, `opti
-00014b30: 6f6e 616c 6029 3a0a 2020 2020 2020 2020  onal`):.        
-00014b40: 2020 2020 4966 2073 6574 2074 6f20 3a6f      If set to :o
-00014b50: 626a 3a60 5472 7565 602c 203a 6f62 6a3a  bj:`True`, :obj:
-00014b60: 6070 6173 745f 6b65 795f 7661 6c75 6573  `past_key_values
-00014b70: 6020 6b65 7920 7661 6c75 6520 7374 6174  ` key value stat
-00014b80: 6573 2061 7265 2072 6574 7572 6e65 6420  es are returned 
-00014b90: 616e 6420 6361 6e20 6265 2075 7365 6420  and can be used 
-00014ba0: 746f 2073 7065 6564 2075 700a 2020 2020  to speed up.    
-00014bb0: 2020 2020 2020 2020 6465 636f 6469 6e67          decoding
-00014bc0: 2028 7365 6520 3a6f 626a 3a60 7061 7374   (see :obj:`past
-00014bd0: 5f6b 6579 5f76 616c 7565 7360 292e 0a20  _key_values`).. 
-00014be0: 2020 2020 2020 206f 7574 7075 745f 6174         output_at
-00014bf0: 7465 6e74 696f 6e73 2028 3a6f 626a 3a60  tentions (:obj:`
-00014c00: 626f 6f6c 602c 2060 6f70 7469 6f6e 616c  bool`, `optional
-00014c10: 6029 3a0a 2020 2020 2020 2020 2020 2020  `):.            
-00014c20: 5768 6574 6865 7220 6f72 206e 6f74 2074  Whether or not t
-00014c30: 6f20 7265 7475 726e 2074 6865 2061 7474  o return the att
-00014c40: 656e 7469 6f6e 7320 7465 6e73 6f72 7320  entions tensors 
-00014c50: 6f66 2061 6c6c 2061 7474 656e 7469 6f6e  of all attention
-00014c60: 206c 6179 6572 732e 2053 6565 2060 6061   layers. See ``a
-00014c70: 7474 656e 7469 6f6e 7360 6020 756e 6465  ttentions`` unde
-00014c80: 7220 7265 7475 726e 6564 0a20 2020 2020  r returned.     
-00014c90: 2020 2020 2020 2074 656e 736f 7273 2066         tensors f
-00014ca0: 6f72 206d 6f72 6520 6465 7461 696c 2e0a  or more detail..
-00014cb0: 2020 2020 2020 2020 6f75 7470 7574 5f68          output_h
-00014cc0: 6964 6465 6e5f 7374 6174 6573 2028 3a6f  idden_states (:o
-00014cd0: 626a 3a60 626f 6f6c 602c 2060 6f70 7469  bj:`bool`, `opti
-00014ce0: 6f6e 616c 6029 3a0a 2020 2020 2020 2020  onal`):.        
-00014cf0: 2020 2020 5768 6574 6865 7220 6f72 206e      Whether or n
-00014d00: 6f74 2074 6f20 7265 7475 726e 2074 6865  ot to return the
-00014d10: 2068 6964 6465 6e20 7374 6174 6573 206f   hidden states o
-00014d20: 6620 616c 6c20 6c61 7965 7273 2e20 5365  f all layers. Se
-00014d30: 6520 6060 6869 6464 656e 5f73 7461 7465  e ``hidden_state
-00014d40: 7360 6020 756e 6465 7220 7265 7475 726e  s`` under return
-00014d50: 6564 2074 656e 736f 7273 2066 6f72 0a20  ed tensors for. 
-00014d60: 2020 2020 2020 2020 2020 206d 6f72 6520             more 
-00014d70: 6465 7461 696c 2e0a 2020 2020 2020 2020  detail..        
-00014d80: 7265 7475 726e 5f64 6963 7420 283a 6f62  return_dict (:ob
-00014d90: 6a3a 6062 6f6f 6c60 2c20 606f 7074 696f  j:`bool`, `optio
-00014da0: 6e61 6c60 293a 0a20 2020 2020 2020 2020  nal`):.         
-00014db0: 2020 2057 6865 7468 6572 206f 7220 6e6f     Whether or no
-00014dc0: 7420 746f 2072 6574 7572 6e20 6120 3a63  t to return a :c
-00014dd0: 6c61 7373 3a60 7e74 7261 6e73 666f 726d  lass:`~transform
-00014de0: 6572 732e 6669 6c65 5f75 7469 6c73 2e4d  ers.file_utils.M
-00014df0: 6f64 656c 4f75 7470 7574 6020 696e 7374  odelOutput` inst
-00014e00: 6561 6420 6f66 2061 2070 6c61 696e 2074  ead of a plain t
-00014e10: 7570 6c65 2e0a 2222 220a 0a0a 4061 6464  uple.."""...@add
-00014e20: 5f73 7461 7274 5f64 6f63 7374 7269 6e67  _start_docstring
-00014e30: 7328 0a20 2020 2022 5468 6520 6261 7265  s(.    "The bare
-00014e40: 2052 6566 6f72 6d65 7220 4d6f 6465 6c20   Reformer Model 
-00014e50: 7472 616e 7366 6f72 6d65 7220 6f75 7470  transformer outp
-00014e60: 7574 7469 6e67 2072 6177 2068 6964 6465  utting raw hidde
-00014e70: 6e2d 7374 6174 6573 2220 2277 6974 686f  n-states" "witho
-00014e80: 7574 2061 6e79 2073 7065 6369 6669 6320  ut any specific 
-00014e90: 6865 6164 206f 6e20 746f 702e 222c 0a20  head on top.",. 
-00014ea0: 2020 2052 4546 4f52 4d45 525f 5354 4152     REFORMER_STAR
-00014eb0: 545f 444f 4353 5452 494e 472c 0a29 0a63  T_DOCSTRING,.).c
-00014ec0: 6c61 7373 2052 6566 6f72 6d65 724d 6f64  lass ReformerMod
-00014ed0: 656c 2852 6566 6f72 6d65 7250 7265 5472  el(ReformerPreTr
-00014ee0: 6169 6e65 644d 6f64 656c 293a 0a20 2020  ainedModel):.   
-00014ef0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00014f00: 6c66 2c20 636f 6e66 6967 293a 0a20 2020  lf, config):.   
-00014f10: 2020 2020 2073 7570 6572 2829 2e5f 5f69       super().__i
-00014f20: 6e69 745f 5f28 636f 6e66 6967 290a 2020  nit__(config).  
-00014f30: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
-00014f40: 6720 3d20 636f 6e66 6967 0a20 2020 2020  g = config.     
-00014f50: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-00014f60: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-00014f70: 6669 672e 6e75 6d5f 6869 6464 656e 5f6c  fig.num_hidden_l
-00014f80: 6179 6572 7320 3e20 300a 2020 2020 2020  ayers > 0.      
-00014f90: 2020 292c 2022 6063 6f6e 6669 672e 6174    ), "`config.at
-00014fa0: 746e 5f6c 6179 6572 7360 2069 7320 656d  tn_layers` is em
-00014fb0: 7074 792e 2053 656c 6563 7420 6174 206c  pty. Select at l
-00014fc0: 6561 7374 206f 6e65 2061 7474 6e20 6c61  east one attn la
-00014fd0: 7965 7220 666f 726d 205b 276c 7368 272c  yer form ['lsh',
-00014fe0: 2027 6c6f 6361 6c27 5d22 0a0a 2020 2020   'local']"..    
-00014ff0: 2020 2020 7365 6c66 2e65 6d62 6564 6469      self.embeddi
-00015000: 6e67 7320 3d20 5265 666f 726d 6572 456d  ngs = ReformerEm
-00015010: 6265 6464 696e 6773 2863 6f6e 6669 6729  beddings(config)
-00015020: 0a20 2020 2020 2020 2073 656c 662e 656e  .        self.en
-00015030: 636f 6465 7220 3d20 5265 666f 726d 6572  coder = Reformer
-00015040: 456e 636f 6465 7228 636f 6e66 6967 290a  Encoder(config).
-00015050: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
-00015060: 6974 5f77 6569 6768 7473 2829 0a0a 2020  it_weights()..  
-00015070: 2020 6465 6620 6765 745f 696e 7075 745f    def get_input_
-00015080: 656d 6265 6464 696e 6773 2873 656c 6629  embeddings(self)
-00015090: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000150a0: 2073 656c 662e 656d 6265 6464 696e 6773   self.embeddings
-000150b0: 2e77 6f72 645f 656d 6265 6464 696e 6773  .word_embeddings
-000150c0: 0a0a 2020 2020 6465 6620 7365 745f 696e  ..    def set_in
-000150d0: 7075 745f 656d 6265 6464 696e 6773 2873  put_embeddings(s
-000150e0: 656c 662c 2076 616c 7565 293a 0a20 2020  elf, value):.   
-000150f0: 2020 2020 2073 656c 662e 656d 6265 6464       self.embedd
-00015100: 696e 6773 2e77 6f72 645f 656d 6265 6464  ings.word_embedd
-00015110: 696e 6773 203d 2076 616c 7565 0a0a 2020  ings = value..  
-00015120: 2020 6465 6620 5f70 7275 6e65 5f68 6561    def _prune_hea
-00015130: 6473 2873 656c 662c 2068 6561 6473 5f74  ds(self, heads_t
-00015140: 6f5f 7072 756e 6529 3a0a 2020 2020 2020  o_prune):.      
-00015150: 2020 2222 220a 2020 2020 2020 2020 5072    """.        Pr
-00015160: 756e 6573 2068 6561 6473 206f 6620 7468  unes heads of th
-00015170: 6520 6d6f 6465 6c2e 2068 6561 6473 5f74  e model. heads_t
-00015180: 6f5f 7072 756e 653a 2064 6963 7420 6f66  o_prune: dict of
-00015190: 207b 6c61 7965 725f 6e75 6d3a 206c 6973   {layer_num: lis
-000151a0: 7420 6f66 2068 6561 6473 2074 6f20 7072  t of heads to pr
-000151b0: 756e 6520 696e 2074 6869 7320 6c61 7965  une in this laye
-000151c0: 727d 2053 6565 2062 6173 650a 2020 2020  r} See base.    
-000151d0: 2020 2020 636c 6173 7320 5072 6554 7261      class PreTra
-000151e0: 696e 6564 4d6f 6465 6c0a 2020 2020 2020  inedModel.      
-000151f0: 2020 2222 220a 2020 2020 2020 2020 666f    """.        fo
-00015200: 7220 6c61 7965 722c 2068 6561 6473 2069  r layer, heads i
-00015210: 6e20 6865 6164 735f 746f 5f70 7275 6e65  n heads_to_prune
-00015220: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00015230: 2020 2020 2020 7365 6c66 2e65 6e63 6f64        self.encod
-00015240: 6572 2e6c 6179 6572 5b6c 6179 6572 5d2e  er.layer[layer].
-00015250: 6174 7465 6e74 696f 6e2e 7072 756e 655f  attention.prune_
-00015260: 6865 6164 7328 6865 6164 7329 0a0a 2020  heads(heads)..  
-00015270: 2020 4061 6464 5f73 7461 7274 5f64 6f63    @add_start_doc
-00015280: 7374 7269 6e67 735f 746f 5f6d 6f64 656c  strings_to_model
-00015290: 5f66 6f72 7761 7264 2852 4546 4f52 4d45  _forward(REFORME
-000152a0: 525f 494e 5055 5453 5f44 4f43 5354 5249  R_INPUTS_DOCSTRI
-000152b0: 4e47 290a 2020 2020 4061 6464 5f63 6f64  NG).    @add_cod
-000152c0: 655f 7361 6d70 6c65 5f64 6f63 7374 7269  e_sample_docstri
-000152d0: 6e67 7328 0a20 2020 2020 2020 2074 6f6b  ngs(.        tok
-000152e0: 656e 697a 6572 5f63 6c61 7373 3d5f 544f  enizer_class=_TO
-000152f0: 4b45 4e49 5a45 525f 464f 525f 444f 432c  KENIZER_FOR_DOC,
-00015300: 0a20 2020 2020 2020 2063 6865 636b 706f  .        checkpo
-00015310: 696e 743d 5f43 4845 434b 504f 494e 545f  int=_CHECKPOINT_
-00015320: 464f 525f 444f 432c 0a20 2020 2020 2020  FOR_DOC,.       
-00015330: 206f 7574 7075 745f 7479 7065 3d52 6566   output_type=Ref
-00015340: 6f72 6d65 724d 6f64 656c 4f75 7470 7574  ormerModelOutput
-00015350: 2c0a 2020 2020 2020 2020 636f 6e66 6967  ,.        config
-00015360: 5f63 6c61 7373 3d5f 434f 4e46 4947 5f46  _class=_CONFIG_F
-00015370: 4f52 5f44 4f43 2c0a 2020 2020 290a 2020  OR_DOC,.    ).  
-00015380: 2020 6465 6620 666f 7277 6172 6428 0a20    def forward(. 
-00015390: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
-000153a0: 2020 2020 2069 6e70 7574 5f69 6473 3d4e       input_ids=N
-000153b0: 6f6e 652c 0a20 2020 2020 2020 2061 7474  one,.        att
-000153c0: 656e 7469 6f6e 5f6d 6173 6b3d 4e6f 6e65  ention_mask=None
-000153d0: 2c0a 2020 2020 2020 2020 706f 7369 7469  ,.        positi
-000153e0: 6f6e 5f69 6473 3d4e 6f6e 652c 0a20 2020  on_ids=None,.   
-000153f0: 2020 2020 2068 6561 645f 6d61 736b 3d4e       head_mask=N
-00015400: 6f6e 652c 0a20 2020 2020 2020 2069 6e70  one,.        inp
-00015410: 7574 735f 656d 6265 6473 3d4e 6f6e 652c  uts_embeds=None,
-00015420: 0a20 2020 2020 2020 206e 756d 5f68 6173  .        num_has
-00015430: 6865 733d 4e6f 6e65 2c0a 2020 2020 2020  hes=None,.      
-00015440: 2020 7061 7374 5f62 7563 6b65 7473 5f73    past_buckets_s
-00015450: 7461 7465 733d 4e6f 6e65 2c0a 2020 2020  tates=None,.    
-00015460: 2020 2020 7573 655f 6361 6368 653d 4e6f      use_cache=No
-00015470: 6e65 2c0a 2020 2020 2020 2020 6f75 7470  ne,.        outp
-00015480: 7574 5f68 6964 6465 6e5f 7374 6174 6573  ut_hidden_states
-00015490: 3d4e 6f6e 652c 0a20 2020 2020 2020 206f  =None,.        o
-000154a0: 7574 7075 745f 6174 7465 6e74 696f 6e73  utput_attentions
-000154b0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2072  =None,.        r
-000154c0: 6574 7572 6e5f 6469 6374 3d4e 6f6e 652c  eturn_dict=None,
-000154d0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000154e0: 7573 655f 6361 6368 6520 3d20 7573 655f  use_cache = use_
-000154f0: 6361 6368 6520 6966 2075 7365 5f63 6163  cache if use_cac
-00015500: 6865 2069 7320 6e6f 7420 4e6f 6e65 2065  he is not None e
-00015510: 6c73 6520 7365 6c66 2e63 6f6e 6669 672e  lse self.config.
-00015520: 7573 655f 6361 6368 650a 2020 2020 2020  use_cache.      
-00015530: 2020 6f75 7470 7574 5f61 7474 656e 7469    output_attenti
-00015540: 6f6e 7320 3d20 6f75 7470 7574 5f61 7474  ons = output_att
-00015550: 656e 7469 6f6e 7320 6966 206f 7574 7075  entions if outpu
-00015560: 745f 6174 7465 6e74 696f 6e73 2069 7320  t_attentions is 
-00015570: 6e6f 7420 4e6f 6e65 2065 6c73 6520 7365  not None else se
-00015580: 6c66 2e63 6f6e 6669 672e 6f75 7470 7574  lf.config.output
-00015590: 5f61 7474 656e 7469 6f6e 730a 2020 2020  _attentions.    
-000155a0: 2020 2020 6f75 7470 7574 5f68 6964 6465      output_hidde
-000155b0: 6e5f 7374 6174 6573 203d 2028 0a20 2020  n_states = (.   
-000155c0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
-000155d0: 6869 6464 656e 5f73 7461 7465 7320 6966  hidden_states if
-000155e0: 206f 7574 7075 745f 6869 6464 656e 5f73   output_hidden_s
-000155f0: 7461 7465 7320 6973 206e 6f74 204e 6f6e  tates is not Non
-00015600: 6520 656c 7365 2073 656c 662e 636f 6e66  e else self.conf
-00015610: 6967 2e6f 7574 7075 745f 6869 6464 656e  ig.output_hidden
-00015620: 5f73 7461 7465 730a 2020 2020 2020 2020  _states.        
-00015630: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00015640: 5f64 6963 7420 3d20 7265 7475 726e 5f64  _dict = return_d
-00015650: 6963 7420 6966 2072 6574 7572 6e5f 6469  ict if return_di
-00015660: 6374 2069 7320 6e6f 7420 4e6f 6e65 2065  ct is not None e
-00015670: 6c73 6520 7365 6c66 2e63 6f6e 6669 672e  lse self.config.
-00015680: 7573 655f 7265 7475 726e 5f64 6963 740a  use_return_dict.
-00015690: 0a20 2020 2020 2020 2069 6620 696e 7075  .        if inpu
-000156a0: 745f 6964 7320 6973 206e 6f74 204e 6f6e  t_ids is not Non
-000156b0: 6520 616e 6420 696e 7075 7473 5f65 6d62  e and inputs_emb
-000156c0: 6564 7320 6973 206e 6f74 204e 6f6e 653a  eds is not None:
-000156d0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-000156e0: 7365 2056 616c 7565 4572 726f 7228 2259  se ValueError("Y
-000156f0: 6f75 2063 616e 6e6f 7420 7370 6563 6966  ou cannot specif
-00015700: 7920 626f 7468 2069 6e70 7574 5f69 6473  y both input_ids
-00015710: 2061 6e64 2069 6e70 7574 735f 656d 6265   and inputs_embe
-00015720: 6473 2061 7420 7468 6520 7361 6d65 2074  ds at the same t
-00015730: 696d 6522 290a 2020 2020 2020 2020 656c  ime").        el
-00015740: 6966 2069 6e70 7574 5f69 6473 2069 7320  if input_ids is 
-00015750: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00015760: 2020 2020 2020 696e 7075 745f 7368 6170        input_shap
-00015770: 6520 3d20 696e 7075 745f 6964 732e 7369  e = input_ids.si
-00015780: 7a65 2829 2020 2320 6e6f 7161 3a20 4638  ze()  # noqa: F8
-00015790: 3431 0a20 2020 2020 2020 2020 2020 2064  41.            d
-000157a0: 6576 6963 6520 3d20 696e 7075 745f 6964  evice = input_id
-000157b0: 732e 6465 7669 6365 0a20 2020 2020 2020  s.device.       
-000157c0: 2065 6c69 6620 696e 7075 7473 5f65 6d62   elif inputs_emb
-000157d0: 6564 7320 6973 206e 6f74 204e 6f6e 653a  eds is not None:
-000157e0: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-000157f0: 7574 5f73 6861 7065 203d 2069 6e70 7574  ut_shape = input
-00015800: 735f 656d 6265 6473 2e73 697a 6528 295b  s_embeds.size()[
-00015810: 3a2d 315d 2020 2320 6e6f 7161 3a20 4638  :-1]  # noqa: F8
-00015820: 3431 0a20 2020 2020 2020 2020 2020 2064  41.            d
-00015830: 6576 6963 6520 3d20 696e 7075 7473 5f65  evice = inputs_e
-00015840: 6d62 6564 732e 6465 7669 6365 0a20 2020  mbeds.device.   
-00015850: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00015860: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-00015870: 7565 4572 726f 7228 2259 6f75 2068 6176  ueError("You hav
-00015880: 6520 746f 2073 7065 6369 6679 2065 6974  e to specify eit
-00015890: 6865 7220 696e 7075 745f 6964 7320 6f72  her input_ids or
-000158a0: 2069 6e70 7574 735f 656d 6265 6473 2229   inputs_embeds")
-000158b0: 0a0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000158c0: 2028 0a20 2020 2020 2020 2020 2020 206c   (.            l
-000158d0: 656e 2869 6e70 7574 5f73 6861 7065 2920  en(input_shape) 
-000158e0: 3d3d 2032 0a20 2020 2020 2020 2029 2c20  == 2.        ), 
-000158f0: 6622 6069 6e70 7574 5f69 6473 6020 6861  f"`input_ids` ha
-00015900: 7665 2062 6520 6f66 2073 6861 7065 2060  ve be of shape `
-00015910: 5b62 6174 6368 5f73 697a 652c 2073 6571  [batch_size, seq
-00015920: 7565 6e63 655f 6c65 6e67 7468 5d60 2c20  uence_length]`, 
-00015930: 6275 7420 676f 7420 7368 6170 653a 207b  but got shape: {
-00015940: 696e 7075 745f 7368 6170 657d 220a 0a20  input_shape}".. 
-00015950: 2020 2020 2020 2069 6620 7061 7374 5f62         if past_b
-00015960: 7563 6b65 7473 5f73 7461 7465 7320 6973  uckets_states is
-00015970: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00015980: 2020 2020 2020 2061 7373 6572 7420 6e6f         assert no
-00015990: 7420 7365 6c66 2e74 7261 696e 696e 672c  t self.training,
-000159a0: 2022 6070 6173 745f 6275 636b 6574 735f   "`past_buckets_
-000159b0: 7374 6174 6573 6020 6361 6e20 6f6e 6c79  states` can only
-000159c0: 2062 6520 7573 6564 2066 6f72 2069 6e66   be used for inf
-000159d0: 6572 656e 6365 2c20 6e6f 7420 666f 7220  erence, not for 
-000159e0: 7472 6169 6e69 6e67 602e 220a 0a20 2020  training`."..   
-000159f0: 2020 2020 2023 2070 7265 7061 7265 2068       # prepare h
-00015a00: 6561 6420 6d61 736b 0a20 2020 2020 2020  ead mask.       
-00015a10: 2068 6561 645f 6d61 736b 203d 2073 656c   head_mask = sel
-00015a20: 662e 6765 745f 6865 6164 5f6d 6173 6b28  f.get_head_mask(
-00015a30: 6865 6164 5f6d 6173 6b2c 2073 656c 662e  head_mask, self.
-00015a40: 636f 6e66 6967 2e6e 756d 5f68 6964 6465  config.num_hidde
-00015a50: 6e5f 6c61 7965 7273 2c20 6973 5f61 7474  n_layers, is_att
-00015a60: 656e 7469 6f6e 5f63 6875 6e6b 6564 3d54  ention_chunked=T
-00015a70: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
-00015a80: 6f72 6967 696e 616c 2073 6571 7565 6e63  original sequenc
-00015a90: 6520 6c65 6e67 7468 2066 6f72 2070 6164  e length for pad
-00015aa0: 6469 6e67 0a20 2020 2020 2020 206f 7269  ding.        ori
-00015ab0: 675f 7365 7175 656e 6365 5f6c 656e 6774  g_sequence_lengt
-00015ac0: 6820 3d20 696e 7075 745f 7368 6170 655b  h = input_shape[
-00015ad0: 2d31 5d0a 0a20 2020 2020 2020 2023 2069  -1]..        # i
-00015ae0: 6620 6e65 6564 7320 7061 6464 696e 670a  f needs padding.
-00015af0: 2020 2020 2020 2020 6c65 6173 745f 636f          least_co
-00015b00: 6d6d 6f6e 5f6d 756c 745f 6368 756e 6b5f  mmon_mult_chunk_
-00015b10: 6c65 6e67 7468 203d 205f 6765 745f 6c65  length = _get_le
-00015b20: 6173 745f 636f 6d6d 6f6e 5f6d 756c 745f  ast_common_mult_
-00015b30: 6368 756e 6b5f 6c65 6e28 7365 6c66 2e63  chunk_len(self.c
-00015b40: 6f6e 6669 6729 0a20 2020 2020 2020 206d  onfig).        m
-00015b50: 696e 5f63 6875 6e6b 5f6c 656e 6774 6820  in_chunk_length 
-00015b60: 3d20 5f67 6574 5f6d 696e 5f63 6875 6e6b  = _get_min_chunk
-00015b70: 5f6c 656e 2873 656c 662e 636f 6e66 6967  _len(self.config
-00015b80: 290a 0a20 2020 2020 2020 206d 7573 745f  )..        must_
-00015b90: 7061 645f 746f 5f6d 6174 6368 5f63 6875  pad_to_match_chu
-00015ba0: 6e6b 5f6c 656e 6774 6820 3d20 280a 2020  nk_length = (.  
-00015bb0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
-00015bc0: 7368 6170 655b 2d31 5d20 2520 6c65 6173  shape[-1] % leas
-00015bd0: 745f 636f 6d6d 6f6e 5f6d 756c 745f 6368  t_common_mult_ch
-00015be0: 756e 6b5f 6c65 6e67 7468 2021 3d20 300a  unk_length != 0.
-00015bf0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00015c00: 696e 7075 745f 7368 6170 655b 2d31 5d20  input_shape[-1] 
-00015c10: 3e20 6d69 6e5f 6368 756e 6b5f 6c65 6e67  > min_chunk_leng
-00015c20: 7468 0a20 2020 2020 2020 2020 2020 2061  th.            a
-00015c30: 6e64 2070 6173 745f 6275 636b 6574 735f  nd past_buckets_
-00015c40: 7374 6174 6573 2069 7320 4e6f 6e65 0a20  states is None. 
-00015c50: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00015c60: 2020 6966 206d 7573 745f 7061 645f 746f    if must_pad_to
-00015c70: 5f6d 6174 6368 5f63 6875 6e6b 5f6c 656e  _match_chunk_len
-00015c80: 6774 683a 0a20 2020 2020 2020 2020 2020  gth:.           
-00015c90: 2070 6164 6469 6e67 5f6c 656e 6774 6820   padding_length 
-00015ca0: 3d20 6c65 6173 745f 636f 6d6d 6f6e 5f6d  = least_common_m
-00015cb0: 756c 745f 6368 756e 6b5f 6c65 6e67 7468  ult_chunk_length
-00015cc0: 202d 2069 6e70 7574 5f73 6861 7065 5b2d   - input_shape[-
-00015cd0: 315d 2025 206c 6561 7374 5f63 6f6d 6d6f  1] % least_commo
-00015ce0: 6e5f 6d75 6c74 5f63 6875 6e6b 5f6c 656e  n_mult_chunk_len
-00015cf0: 6774 680a 0a20 2020 2020 2020 2020 2020  gth..           
-00015d00: 2069 6620 7365 6c66 2e74 7261 696e 696e   if self.trainin
-00015d10: 6720 6973 2054 7275 653a 0a20 2020 2020  g is True:.     
-00015d20: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00015d30: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00015d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015d50: 2066 2249 6620 7472 6169 6e69 6e67 2c20   f"If training, 
-00015d60: 7365 7175 656e 6365 206c 656e 6774 6820  sequence length 
-00015d70: 7b69 6e70 7574 5f73 6861 7065 5b2d 315d  {input_shape[-1]
-00015d80: 7d20 6861 7320 746f 2062 6520 6120 6d75  } has to be a mu
-00015d90: 6c74 6970 6c65 206f 6620 6c65 6173 7420  ltiple of least 
-00015da0: 636f 6d6d 6f6e 206d 756c 7469 706c 6520  common multiple 
-00015db0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00015dc0: 2020 2020 2020 6622 6368 756e 6b5f 6c65        f"chunk_le
-00015dd0: 6e67 7468 207b 6c65 6173 745f 636f 6d6d  ngth {least_comm
-00015de0: 6f6e 5f6d 756c 745f 6368 756e 6b5f 6c65  on_mult_chunk_le
-00015df0: 6e67 7468 7d2e 2050 6c65 6173 6520 636f  ngth}. Please co
-00015e00: 6e73 6964 6572 2070 6164 6469 6e67 2074  nsider padding t
-00015e10: 6865 2069 6e70 7574 2074 6f20 6120 6c65  he input to a le
-00015e20: 6e67 7468 2022 0a20 2020 2020 2020 2020  ngth ".         
-00015e30: 2020 2020 2020 2020 2020 2066 226f 6620             f"of 
-00015e40: 7b69 6e70 7574 5f73 6861 7065 5b2d 315d  {input_shape[-1]
-00015e50: 202b 2070 6164 6469 6e67 5f6c 656e 6774   + padding_lengt
-00015e60: 687d 2e22 0a20 2020 2020 2020 2020 2020  h}.".           
-00015e70: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00015e80: 2020 2020 2320 7061 6420 696e 7075 740a      # pad input.
-00015e90: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-00015ea0: 745f 6964 732c 2069 6e70 7574 735f 656d  t_ids, inputs_em
-00015eb0: 6265 6473 2c20 6174 7465 6e74 696f 6e5f  beds, attention_
-00015ec0: 6d61 736b 2c20 706f 7369 7469 6f6e 5f69  mask, position_i
-00015ed0: 6473 2c20 696e 7075 745f 7368 6170 6520  ds, input_shape 
-00015ee0: 3d20 7365 6c66 2e5f 7061 645f 746f 5f6d  = self._pad_to_m
-00015ef0: 756c 745f 6f66 5f63 6875 6e6b 5f6c 656e  ult_of_chunk_len
-00015f00: 6774 6828 0a20 2020 2020 2020 2020 2020  gth(.           
-00015f10: 2020 2020 2069 6e70 7574 5f69 6473 2c0a       input_ids,.
-00015f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015f30: 696e 7075 7473 5f65 6d62 6564 733d 696e  inputs_embeds=in
-00015f40: 7075 7473 5f65 6d62 6564 732c 0a20 2020  puts_embeds,.   
-00015f50: 2020 2020 2020 2020 2020 2020 2061 7474               att
-00015f60: 656e 7469 6f6e 5f6d 6173 6b3d 6174 7465  ention_mask=atte
-00015f70: 6e74 696f 6e5f 6d61 736b 2c0a 2020 2020  ntion_mask,.    
-00015f80: 2020 2020 2020 2020 2020 2020 706f 7369              posi
-00015f90: 7469 6f6e 5f69 6473 3d70 6f73 6974 696f  tion_ids=positio
-00015fa0: 6e5f 6964 732c 0a20 2020 2020 2020 2020  n_ids,.         
-00015fb0: 2020 2020 2020 2069 6e70 7574 5f73 6861         input_sha
-00015fc0: 7065 3d69 6e70 7574 5f73 6861 7065 2c0a  pe=input_shape,.
-00015fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015fe0: 7061 6464 696e 675f 6c65 6e67 7468 3d70  padding_length=p
-00015ff0: 6164 6469 6e67 5f6c 656e 6774 682c 0a20  adding_length,. 
-00016000: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00016010: 6164 6465 645f 7365 715f 6c65 6e67 7468  added_seq_length
-00016020: 3d6c 6561 7374 5f63 6f6d 6d6f 6e5f 6d75  =least_common_mu
-00016030: 6c74 5f63 6875 6e6b 5f6c 656e 6774 682c  lt_chunk_length,
-00016040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016050: 2064 6576 6963 653d 6465 7669 6365 2c0a   device=device,.
-00016060: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
-00016070: 2020 2020 2020 2023 2073 7461 7274 2069         # start i
-00016080: 6e64 6578 2066 6f72 2070 6f73 6974 696f  ndex for positio
-00016090: 6e20 656e 636f 6469 6e67 2064 6570 656e  n encoding depen
-000160a0: 6473 206f 6e20 696e 6372 656d 656e 7461  ds on incrementa
-000160b0: 6c20 6465 636f 6469 6e67 0a20 2020 2020  l decoding.     
-000160c0: 2020 2069 6620 7061 7374 5f62 7563 6b65     if past_bucke
-000160d0: 7473 5f73 7461 7465 7320 6973 206e 6f74  ts_states is not
-000160e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000160f0: 2020 2073 7461 7274 5f69 6478 5f70 6f73     start_idx_pos
-00016100: 5f65 6e63 6f64 696e 6773 203d 2070 6173  _encodings = pas
-00016110: 745f 6275 636b 6574 735f 7374 6174 6573  t_buckets_states
-00016120: 5b30 5d5b 315d 2e73 6861 7065 5b31 5d0a  [0][1].shape[1].
-00016130: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00016140: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-00016150: 6964 785f 706f 735f 656e 636f 6469 6e67  idx_pos_encoding
-00016160: 7320 3d20 300a 0a20 2020 2020 2020 2065  s = 0..        e
-00016170: 6d62 6564 6469 6e67 5f6f 7574 7075 7420  mbedding_output 
-00016180: 3d20 7365 6c66 2e65 6d62 6564 6469 6e67  = self.embedding
-00016190: 7328 0a20 2020 2020 2020 2020 2020 2069  s(.            i
-000161a0: 6e70 7574 5f69 6473 3d69 6e70 7574 5f69  nput_ids=input_i
-000161b0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-000161c0: 706f 7369 7469 6f6e 5f69 6473 3d70 6f73  position_ids=pos
-000161d0: 6974 696f 6e5f 6964 732c 0a20 2020 2020  ition_ids,.     
-000161e0: 2020 2020 2020 2069 6e70 7574 735f 656d         inputs_em
-000161f0: 6265 6473 3d69 6e70 7574 735f 656d 6265  beds=inputs_embe
-00016200: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00016210: 7374 6172 745f 6964 785f 706f 735f 656e  start_idx_pos_en
-00016220: 636f 6469 6e67 733d 7374 6172 745f 6964  codings=start_id
-00016230: 785f 706f 735f 656e 636f 6469 6e67 732c  x_pos_encodings,
-00016240: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00016250: 2020 2020 656e 636f 6465 725f 6f75 7470      encoder_outp
-00016260: 7574 7320 3d20 7365 6c66 2e65 6e63 6f64  uts = self.encod
-00016270: 6572 280a 2020 2020 2020 2020 2020 2020  er(.            
-00016280: 6869 6464 656e 5f73 7461 7465 733d 656d  hidden_states=em
-00016290: 6265 6464 696e 675f 6f75 7470 7574 2c0a  bedding_output,.
-000162a0: 2020 2020 2020 2020 2020 2020 6865 6164              head
-000162b0: 5f6d 6173 6b3d 6865 6164 5f6d 6173 6b2c  _mask=head_mask,
-000162c0: 0a20 2020 2020 2020 2020 2020 2061 7474  .            att
-000162d0: 656e 7469 6f6e 5f6d 6173 6b3d 6174 7465  ention_mask=atte
-000162e0: 6e74 696f 6e5f 6d61 736b 2c0a 2020 2020  ntion_mask,.    
-000162f0: 2020 2020 2020 2020 6e75 6d5f 6861 7368          num_hash
-00016300: 6573 3d6e 756d 5f68 6173 6865 732c 0a20  es=num_hashes,. 
-00016310: 2020 2020 2020 2020 2020 2070 6173 745f             past_
-00016320: 6275 636b 6574 735f 7374 6174 6573 3d70  buckets_states=p
-00016330: 6173 745f 6275 636b 6574 735f 7374 6174  ast_buckets_stat
-00016340: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
-00016350: 7573 655f 6361 6368 653d 7573 655f 6361  use_cache=use_ca
-00016360: 6368 652c 0a20 2020 2020 2020 2020 2020  che,.           
-00016370: 206f 7269 675f 7365 7175 656e 6365 5f6c   orig_sequence_l
-00016380: 656e 6774 683d 6f72 6967 5f73 6571 7565  ength=orig_seque
-00016390: 6e63 655f 6c65 6e67 7468 2c0a 2020 2020  nce_length,.    
-000163a0: 2020 2020 2020 2020 6f75 7470 7574 5f68          output_h
-000163b0: 6964 6465 6e5f 7374 6174 6573 3d6f 7574  idden_states=out
-000163c0: 7075 745f 6869 6464 656e 5f73 7461 7465  put_hidden_state
-000163d0: 732c 0a20 2020 2020 2020 2020 2020 206f  s,.            o
-000163e0: 7574 7075 745f 6174 7465 6e74 696f 6e73  utput_attentions
-000163f0: 3d6f 7574 7075 745f 6174 7465 6e74 696f  =output_attentio
-00016400: 6e73 2c0a 2020 2020 2020 2020 290a 2020  ns,.        ).  
-00016410: 2020 2020 2020 7365 7175 656e 6365 5f6f        sequence_o
-00016420: 7574 7075 7420 3d20 656e 636f 6465 725f  utput = encoder_
-00016430: 6f75 7470 7574 732e 6869 6464 656e 5f73  outputs.hidden_s
-00016440: 7461 7465 730a 0a20 2020 2020 2020 2023  tates..        #
-00016450: 2069 6620 7061 6464 696e 6720 7761 7320   if padding was 
-00016460: 6170 706c 6965 640a 2020 2020 2020 2020  applied.        
-00016470: 6966 206d 7573 745f 7061 645f 746f 5f6d  if must_pad_to_m
-00016480: 6174 6368 5f63 6875 6e6b 5f6c 656e 6774  atch_chunk_lengt
-00016490: 683a 0a20 2020 2020 2020 2020 2020 2073  h:.            s
-000164a0: 6571 7565 6e63 655f 6f75 7470 7574 203d  equence_output =
-000164b0: 2073 6571 7565 6e63 655f 6f75 7470 7574   sequence_output
-000164c0: 5b3a 2c20 3a6f 7269 675f 7365 7175 656e  [:, :orig_sequen
-000164d0: 6365 5f6c 656e 6774 685d 0a0a 2020 2020  ce_length]..    
-000164e0: 2020 2020 7061 7374 5f62 7563 6b65 7473      past_buckets
-000164f0: 5f73 7461 7465 7320 3d20 656e 636f 6465  _states = encode
-00016500: 725f 6f75 7470 7574 732e 7061 7374 5f62  r_outputs.past_b
-00016510: 7563 6b65 7473 5f73 7461 7465 7320 6966  uckets_states if
-00016520: 2075 7365 5f63 6163 6865 2065 6c73 6520   use_cache else 
-00016530: 4e6f 6e65 0a20 2020 2020 2020 2068 6964  None.        hid
-00016540: 6465 6e5f 7374 6174 6573 203d 2065 6e63  den_states = enc
-00016550: 6f64 6572 5f6f 7574 7075 7473 2e61 6c6c  oder_outputs.all
-00016560: 5f68 6964 6465 6e5f 7374 6174 6573 2069  _hidden_states i
-00016570: 6620 6f75 7470 7574 5f68 6964 6465 6e5f  f output_hidden_
-00016580: 7374 6174 6573 2065 6c73 6520 4e6f 6e65  states else None
-00016590: 0a20 2020 2020 2020 2061 7474 656e 7469  .        attenti
-000165a0: 6f6e 7320 3d20 656e 636f 6465 725f 6f75  ons = encoder_ou
-000165b0: 7470 7574 732e 616c 6c5f 6174 7465 6e74  tputs.all_attent
-000165c0: 696f 6e73 2069 6620 6f75 7470 7574 5f61  ions if output_a
-000165d0: 7474 656e 7469 6f6e 7320 656c 7365 204e  ttentions else N
-000165e0: 6f6e 650a 0a20 2020 2020 2020 2069 6620  one..        if 
-000165f0: 6e6f 7420 7265 7475 726e 5f64 6963 743a  not return_dict:
-00016600: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016610: 7572 6e20 7475 706c 6528 7620 666f 7220  urn tuple(v for 
-00016620: 7620 696e 205b 7365 7175 656e 6365 5f6f  v in [sequence_o
-00016630: 7574 7075 742c 2070 6173 745f 6275 636b  utput, past_buck
-00016640: 6574 735f 7374 6174 6573 2c20 6869 6464  ets_states, hidd
-00016650: 656e 5f73 7461 7465 732c 2061 7474 656e  en_states, atten
-00016660: 7469 6f6e 735d 2069 6620 7620 6973 206e  tions] if v is n
-00016670: 6f74 204e 6f6e 6529 0a20 2020 2020 2020  ot None).       
-00016680: 2072 6574 7572 6e20 5265 666f 726d 6572   return Reformer
-00016690: 4d6f 6465 6c4f 7574 7075 7428 0a20 2020  ModelOutput(.   
-000166a0: 2020 2020 2020 2020 206c 6173 745f 6869           last_hi
-000166b0: 6464 656e 5f73 7461 7465 3d73 6571 7565  dden_state=seque
-000166c0: 6e63 655f 6f75 7470 7574 2c0a 2020 2020  nce_output,.    
-000166d0: 2020 2020 2020 2020 7061 7374 5f62 7563          past_buc
-000166e0: 6b65 7473 5f73 7461 7465 733d 7061 7374  kets_states=past
-000166f0: 5f62 7563 6b65 7473 5f73 7461 7465 732c  _buckets_states,
-00016700: 0a20 2020 2020 2020 2020 2020 2068 6964  .            hid
-00016710: 6465 6e5f 7374 6174 6573 3d68 6964 6465  den_states=hidde
-00016720: 6e5f 7374 6174 6573 2c0a 2020 2020 2020  n_states,.      
-00016730: 2020 2020 2020 6174 7465 6e74 696f 6e73        attentions
-00016740: 3d61 7474 656e 7469 6f6e 732c 0a20 2020  =attentions,.   
-00016750: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-00016760: 5f70 6164 5f74 6f5f 6d75 6c74 5f6f 665f  _pad_to_mult_of_
-00016770: 6368 756e 6b5f 6c65 6e67 7468 280a 2020  chunk_length(.  
-00016780: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
-00016790: 2020 2020 696e 7075 745f 6964 732c 0a20      input_ids,. 
-000167a0: 2020 2020 2020 2069 6e70 7574 735f 656d         inputs_em
-000167b0: 6265 6473 3d4e 6f6e 652c 0a20 2020 2020  beds=None,.     
-000167c0: 2020 2061 7474 656e 7469 6f6e 5f6d 6173     attention_mas
-000167d0: 6b3d 4e6f 6e65 2c0a 2020 2020 2020 2020  k=None,.        
-000167e0: 706f 7369 7469 6f6e 5f69 6473 3d4e 6f6e  position_ids=Non
-000167f0: 652c 0a20 2020 2020 2020 2069 6e70 7574  e,.        input
-00016800: 5f73 6861 7065 3d4e 6f6e 652c 0a20 2020  _shape=None,.   
-00016810: 2020 2020 2070 6164 6469 6e67 5f6c 656e       padding_len
-00016820: 6774 683d 4e6f 6e65 2c0a 2020 2020 2020  gth=None,.      
-00016830: 2020 7061 6464 6564 5f73 6571 5f6c 656e    padded_seq_len
-00016840: 6774 683d 4e6f 6e65 2c0a 2020 2020 2020  gth=None,.      
-00016850: 2020 6465 7669 6365 3d4e 6f6e 652c 0a20    device=None,. 
-00016860: 2020 2029 3a0a 2020 2020 2020 2020 6c6f     ):.        lo
-00016870: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-00016880: 2020 2020 2020 2066 2249 6e70 7574 2069         f"Input i
-00016890: 6473 2061 7265 2061 7574 6f6d 6174 6963  ds are automatic
-000168a0: 616c 6c79 2070 6164 6465 6420 6672 6f6d  ally padded from
-000168b0: 207b 696e 7075 745f 7368 6170 655b 2d31   {input_shape[-1
-000168c0: 5d7d 2074 6f20 7b69 6e70 7574 5f73 6861  ]} to {input_sha
-000168d0: 7065 5b2d 315d 202b 2070 6164 6469 6e67  pe[-1] + padding
-000168e0: 5f6c 656e 6774 687d 2074 6f20 6265 2061  _length} to be a
-000168f0: 2022 0a20 2020 2020 2020 2020 2020 2066   ".            f
-00016900: 226d 756c 7469 706c 6520 6f66 2060 636f  "multiple of `co
-00016910: 6e66 6967 2e63 6875 6e6b 5f6c 656e 6774  nfig.chunk_lengt
-00016920: 6860 3a20 7b70 6164 6465 645f 7365 715f  h`: {padded_seq_
-00016930: 6c65 6e67 7468 7d22 0a20 2020 2020 2020  length}".       
-00016940: 2029 0a0a 2020 2020 2020 2020 7061 6464   )..        padd
-00016950: 6564 5f69 6e70 7574 5f69 6473 203d 2074  ed_input_ids = t
-00016960: 6f72 6368 2e66 756c 6c28 0a20 2020 2020  orch.full(.     
-00016970: 2020 2020 2020 2028 696e 7075 745f 7368         (input_sh
-00016980: 6170 655b 305d 2c20 7061 6464 696e 675f  ape[0], padding_
-00016990: 6c65 6e67 7468 292c 0a20 2020 2020 2020  length),.       
-000169a0: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-000169b0: 2e70 6164 5f74 6f6b 656e 5f69 642c 0a20  .pad_token_id,. 
-000169c0: 2020 2020 2020 2020 2020 2064 6576 6963             devic
-000169d0: 653d 6465 7669 6365 2c0a 2020 2020 2020  e=device,.      
-000169e0: 2020 2020 2020 6474 7970 653d 746f 7263        dtype=torc
-000169f0: 682e 6c6f 6e67 2c0a 2020 2020 2020 2020  h.long,.        
-00016a00: 290a 0a20 2020 2020 2020 2023 2045 7874  )..        # Ext
-00016a10: 656e 6420 6061 7474 656e 7469 6f6e 5f6d  end `attention_m
-00016a20: 6173 6b60 0a20 2020 2020 2020 2069 6620  ask`.        if 
-00016a30: 6174 7465 6e74 696f 6e5f 6d61 736b 2069  attention_mask i
-00016a40: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00016a50: 2020 2020 2020 2020 7061 645f 6174 7465          pad_atte
-00016a60: 6e74 696f 6e5f 6d61 736b 203d 2074 6f72  ntion_mask = tor
-00016a70: 6368 2e7a 6572 6f73 2869 6e70 7574 5f73  ch.zeros(input_s
-00016a80: 6861 7065 5b30 5d2c 2070 6164 6469 6e67  hape[0], padding
-00016a90: 5f6c 656e 6774 682c 2064 6576 6963 653d  _length, device=
-00016aa0: 6465 7669 6365 2c20 6474 7970 653d 6174  device, dtype=at
-00016ab0: 7465 6e74 696f 6e5f 6d61 736b 2e64 7479  tention_mask.dty
-00016ac0: 7065 290a 0a20 2020 2020 2020 2020 2020  pe)..           
-00016ad0: 2061 7474 656e 7469 6f6e 5f6d 6173 6b20   attention_mask 
-00016ae0: 3d20 746f 7263 682e 6361 7428 5b61 7474  = torch.cat([att
-00016af0: 656e 7469 6f6e 5f6d 6173 6b2c 2070 6164  ention_mask, pad
-00016b00: 5f61 7474 656e 7469 6f6e 5f6d 6173 6b5d  _attention_mask]
-00016b10: 2c20 6469 6d3d 2d31 290a 2020 2020 2020  , dim=-1).      
-00016b20: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00016b30: 2020 2020 6174 7465 6e74 696f 6e5f 6d61      attention_ma
-00016b40: 736b 203d 2074 6f72 6368 2e63 6174 280a  sk = torch.cat(.
-00016b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016b60: 5b0a 2020 2020 2020 2020 2020 2020 2020  [.              
-00016b70: 2020 2020 2020 746f 7263 682e 6f6e 6573        torch.ones
-00016b80: 2869 6e70 7574 5f73 6861 7065 2c20 6465  (input_shape, de
-00016b90: 7669 6365 3d64 6576 6963 652c 2064 7479  vice=device, dty
-00016ba0: 7065 3d74 6f72 6368 2e75 696e 7438 292c  pe=torch.uint8),
-00016bb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016bc0: 2020 2020 2074 6f72 6368 2e7a 6572 6f73       torch.zeros
-00016bd0: 2828 696e 7075 745f 7368 6170 655b 305d  ((input_shape[0]
-00016be0: 2c20 7061 6464 696e 675f 6c65 6e67 7468  , padding_length
-00016bf0: 292c 2064 6576 6963 653d 6465 7669 6365  ), device=device
-00016c00: 2c20 6474 7970 653d 746f 7263 682e 7569  , dtype=torch.ui
-00016c10: 6e74 3829 2c0a 2020 2020 2020 2020 2020  nt8),.          
-00016c20: 2020 2020 2020 5d2c 0a20 2020 2020 2020        ],.       
-00016c30: 2020 2020 2020 2020 2064 696d 3d2d 312c           dim=-1,
-00016c40: 0a20 2020 2020 2020 2020 2020 2029 0a0a  .            )..
-00016c50: 2020 2020 2020 2020 2320 4578 7465 6e64          # Extend
-00016c60: 2060 696e 7075 745f 6964 7360 2077 6974   `input_ids` wit
-00016c70: 6820 7061 6464 696e 6720 746f 206d 6174  h padding to mat
-00016c80: 6368 206c 6561 7374 2063 6f6d 6d6f 6e20  ch least common 
-00016c90: 6d75 6c74 6970 6c65 2063 6875 6e6b 5f6c  multiple chunk_l
-00016ca0: 656e 6774 680a 2020 2020 2020 2020 6966  ength.        if
-00016cb0: 2069 6e70 7574 5f69 6473 2069 7320 6e6f   input_ids is no
-00016cc0: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00016cd0: 2020 2020 696e 7075 745f 6964 7320 3d20      input_ids = 
-00016ce0: 746f 7263 682e 6361 7428 5b69 6e70 7574  torch.cat([input
-00016cf0: 5f69 6473 2c20 7061 6464 6564 5f69 6e70  _ids, padded_inp
-00016d00: 7574 5f69 6473 5d2c 2064 696d 3d2d 3129  ut_ids], dim=-1)
-00016d10: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
-00016d20: 7574 5f73 6861 7065 203d 2069 6e70 7574  ut_shape = input
-00016d30: 5f69 6473 2e73 697a 6528 290a 0a20 2020  _ids.size()..   
-00016d40: 2020 2020 2020 2020 2023 2050 6164 2070           # Pad p
-00016d50: 6f73 6974 696f 6e20 6964 7320 6966 2067  osition ids if g
-00016d60: 6976 656e 0a20 2020 2020 2020 2020 2020  iven.           
-00016d70: 2069 6620 706f 7369 7469 6f6e 5f69 6473   if position_ids
-00016d80: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00016d90: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00016da0: 6464 6564 5f70 6f73 6974 696f 6e5f 6964  dded_position_id
-00016db0: 7320 3d20 746f 7263 682e 6172 616e 6765  s = torch.arange
-00016dc0: 2869 6e70 7574 5f73 6861 7065 5b2d 315d  (input_shape[-1]
-00016dd0: 2c20 7061 6464 6564 5f73 6571 5f6c 656e  , padded_seq_len
-00016de0: 6774 682c 2064 7479 7065 3d74 6f72 6368  gth, dtype=torch
-00016df0: 2e6c 6f6e 672c 2064 6576 6963 653d 6465  .long, device=de
-00016e00: 7669 6365 290a 2020 2020 2020 2020 2020  vice).          
-00016e10: 2020 2020 2020 7061 6464 6564 5f70 6f73        padded_pos
-00016e20: 6974 696f 6e5f 6964 7320 3d20 706f 7369  ition_ids = posi
-00016e30: 7469 6f6e 5f69 6473 2e75 6e73 7175 6565  tion_ids.unsquee
-00016e40: 7a65 2830 292e 6578 7061 6e64 2869 6e70  ze(0).expand(inp
-00016e50: 7574 5f73 6861 7065 5b30 5d2c 2070 6164  ut_shape[0], pad
-00016e60: 6469 6e67 5f6c 656e 6774 6829 0a20 2020  ding_length).   
-00016e70: 2020 2020 2020 2020 2020 2020 2070 6f73               pos
-00016e80: 6974 696f 6e5f 6964 7320 3d20 746f 7263  ition_ids = torc
-00016e90: 682e 6361 7428 5b70 6f73 6974 696f 6e5f  h.cat([position_
-00016ea0: 6964 732c 2070 6164 6465 645f 706f 7369  ids, padded_posi
-00016eb0: 7469 6f6e 5f69 6473 5d2c 2064 696d 3d2d  tion_ids], dim=-
-00016ec0: 3129 0a0a 2020 2020 2020 2020 2320 4578  1)..        # Ex
-00016ed0: 7465 6e64 2060 696e 7075 7473 5f65 6d62  tend `inputs_emb
-00016ee0: 6564 7360 2077 6974 6820 7061 6464 696e  eds` with paddin
-00016ef0: 6720 746f 206d 6174 6368 206c 6561 7374  g to match least
-00016f00: 2063 6f6d 6d6f 6e20 6d75 6c74 6970 6c65   common multiple
-00016f10: 2063 6875 6e6b 5f6c 656e 6774 680a 2020   chunk_length.  
-00016f20: 2020 2020 2020 6966 2069 6e70 7574 735f        if inputs_
-00016f30: 656d 6265 6473 2069 7320 6e6f 7420 4e6f  embeds is not No
-00016f40: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00016f50: 7061 6464 6564 5f69 6e70 7574 735f 656d  padded_inputs_em
-00016f60: 6265 6473 203d 2073 656c 662e 656d 6265  beds = self.embe
-00016f70: 6464 696e 6773 2870 6164 6465 645f 696e  ddings(padded_in
-00016f80: 7075 745f 6964 732c 2070 6f73 6974 696f  put_ids, positio
-00016f90: 6e5f 6964 7329 0a20 2020 2020 2020 2020  n_ids).         
-00016fa0: 2020 2069 6e70 7574 735f 656d 6265 6473     inputs_embeds
-00016fb0: 203d 2074 6f72 6368 2e63 6174 285b 696e   = torch.cat([in
-00016fc0: 7075 7473 5f65 6d62 6564 732c 2070 6164  puts_embeds, pad
-00016fd0: 6465 645f 696e 7075 7473 5f65 6d62 6564  ded_inputs_embed
-00016fe0: 735d 2c20 6469 6d3d 2d32 290a 2020 2020  s], dim=-2).    
-00016ff0: 2020 2020 2020 2020 696e 7075 745f 7368          input_sh
-00017000: 6170 6520 3d20 696e 7075 7473 5f65 6d62  ape = inputs_emb
-00017010: 6564 732e 7369 7a65 2829 0a20 2020 2020  eds.size().     
-00017020: 2020 2072 6574 7572 6e20 696e 7075 745f     return input_
-00017030: 6964 732c 2069 6e70 7574 735f 656d 6265  ids, inputs_embe
-00017040: 6473 2c20 6174 7465 6e74 696f 6e5f 6d61  ds, attention_ma
-00017050: 736b 2c20 706f 7369 7469 6f6e 5f69 6473  sk, position_ids
-00017060: 2c20 696e 7075 745f 7368 6170 650a 0a0a  , input_shape...
-00017070: 4061 6464 5f73 7461 7274 5f64 6f63 7374  @add_start_docst
-00017080: 7269 6e67 7328 2222 2252 6566 6f72 6d65  rings("""Reforme
-00017090: 7220 4d6f 6465 6c20 7769 7468 2061 2060  r Model with a `
-000170a0: 6c61 6e67 7561 6765 206d 6f64 656c 696e  language modelin
-000170b0: 6760 2068 6561 6420 6f6e 2074 6f70 2e20  g` head on top. 
-000170c0: 2222 222c 2052 4546 4f52 4d45 525f 5354  """, REFORMER_ST
-000170d0: 4152 545f 444f 4353 5452 494e 4729 0a63  ART_DOCSTRING).c
-000170e0: 6c61 7373 2052 6566 6f72 6d65 724d 6f64  lass ReformerMod
-000170f0: 656c 5769 7468 4c4d 4865 6164 2852 6566  elWithLMHead(Ref
-00017100: 6f72 6d65 7250 7265 5472 6169 6e65 644d  ormerPreTrainedM
-00017110: 6f64 656c 293a 0a20 2020 2064 6566 205f  odel):.    def _
-00017120: 5f69 6e69 745f 5f28 7365 6c66 2c20 636f  _init__(self, co
-00017130: 6e66 6967 293a 0a20 2020 2020 2020 2073  nfig):.        s
-00017140: 7570 6572 2829 2e5f 5f69 6e69 745f 5f28  uper().__init__(
-00017150: 636f 6e66 6967 290a 2020 2020 2020 2020  config).        
-00017160: 6173 7365 7274 2063 6f6e 6669 672e 6973  assert config.is
-00017170: 5f64 6563 6f64 6572 2c20 2249 6620 796f  _decoder, "If yo
-00017180: 7520 7761 6e74 2074 6f20 7573 6520 6052  u want to use `R
-00017190: 6566 6f72 6d65 724d 6f64 656c 5769 7468  eformerModelWith
-000171a0: 4c4d 4865 6164 6020 6d61 6b65 2073 7572  LMHead` make sur
-000171b0: 6520 7468 6174 2060 6973 5f64 6563 6f64  e that `is_decod
-000171c0: 6572 3d54 7275 6560 2e22 0a20 2020 2020  er=True`.".     
-000171d0: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-000171e0: 2020 2020 2020 2020 226c 6f63 616c 2220          "local" 
-000171f0: 6e6f 7420 696e 2073 656c 662e 636f 6e66  not in self.conf
-00017200: 6967 2e61 7474 6e5f 6c61 7965 7273 206f  ig.attn_layers o
-00017210: 7220 636f 6e66 6967 2e6c 6f63 616c 5f6e  r config.local_n
-00017220: 756d 5f63 6875 6e6b 735f 6166 7465 7220  um_chunks_after 
-00017230: 3d3d 2030 0a20 2020 2020 2020 2029 2c20  == 0.        ), 
-00017240: 6622 4966 2063 6175 7361 6c20 6d61 736b  f"If causal mask
-00017250: 2069 7320 656e 6162 6c65 642c 206d 616b   is enabled, mak
-00017260: 6520 7375 7265 2074 6861 7420 6063 6f6e  e sure that `con
-00017270: 6669 672e 6c6f 6361 6c5f 6e75 6d5f 6368  fig.local_num_ch
-00017280: 756e 6b73 5f61 6674 6572 6020 6973 2073  unks_after` is s
-00017290: 6574 2074 6f20 3020 616e 6420 6e6f 7420  et to 0 and not 
-000172a0: 7b63 6f6e 6669 672e 6c6f 6361 6c5f 6e75  {config.local_nu
-000172b0: 6d5f 6368 756e 6b73 5f61 6674 6572 7d2e  m_chunks_after}.
-000172c0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-000172d0: 2028 0a20 2020 2020 2020 2020 2020 2022   (.            "
-000172e0: 6c73 6822 206e 6f74 2069 6e20 7365 6c66  lsh" not in self
-000172f0: 2e63 6f6e 6669 672e 6174 746e 5f6c 6179  .config.attn_lay
-00017300: 6572 7320 6f72 2063 6f6e 6669 672e 6c73  ers or config.ls
-00017310: 685f 6e75 6d5f 6368 756e 6b73 5f61 6674  h_num_chunks_aft
-00017320: 6572 203d 3d20 300a 2020 2020 2020 2020  er == 0.        
-00017330: 292c 2066 2249 6620 6361 7573 616c 206d  ), f"If causal m
-00017340: 6173 6b20 6973 2065 6e61 626c 6564 2c20  ask is enabled, 
-00017350: 6d61 6b65 2073 7572 6520 7468 6174 2060  make sure that `
-00017360: 636f 6e66 6967 2e6c 7368 5f6e 756d 5f63  config.lsh_num_c
-00017370: 6875 6e6b 735f 6166 7465 7260 2069 7320  hunks_after` is 
-00017380: 7365 7420 746f 2031 2061 6e64 206e 6f74  set to 1 and not
-00017390: 207b 636f 6e66 6967 2e6c 7368 5f6e 756d   {config.lsh_num
-000173a0: 5f63 6875 6e6b 735f 6166 7465 727d 2e22  _chunks_after}."
-000173b0: 0a0a 2020 2020 2020 2020 7365 6c66 2e72  ..        self.r
-000173c0: 6566 6f72 6d65 7220 3d20 5265 666f 726d  eformer = Reform
-000173d0: 6572 4d6f 6465 6c28 636f 6e66 6967 290a  erModel(config).
-000173e0: 2020 2020 2020 2020 7365 6c66 2e6c 6d5f          self.lm_
-000173f0: 6865 6164 203d 2052 6566 6f72 6d65 724f  head = ReformerO
-00017400: 6e6c 794c 4d48 6561 6428 636f 6e66 6967  nlyLMHead(config
-00017410: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00017420: 696e 6974 5f77 6569 6768 7473 2829 0a0a  init_weights()..
-00017430: 2020 2020 6465 6620 6765 745f 6f75 7470      def get_outp
-00017440: 7574 5f65 6d62 6564 6469 6e67 7328 7365  ut_embeddings(se
-00017450: 6c66 293a 0a20 2020 2020 2020 2072 6574  lf):.        ret
-00017460: 7572 6e20 7365 6c66 2e6c 6d5f 6865 6164  urn self.lm_head
-00017470: 2e64 6563 6f64 6572 0a0a 2020 2020 6465  .decoder..    de
-00017480: 6620 7365 745f 6f75 7470 7574 5f65 6d62  f set_output_emb
-00017490: 6564 6469 6e67 7328 7365 6c66 2c20 6e65  eddings(self, ne
-000174a0: 775f 656d 6265 6464 696e 6773 293a 0a20  w_embeddings):. 
-000174b0: 2020 2020 2020 2073 656c 662e 6c6d 5f68         self.lm_h
-000174c0: 6561 642e 6465 636f 6465 7220 3d20 6e65  ead.decoder = ne
-000174d0: 775f 656d 6265 6464 696e 6773 0a0a 2020  w_embeddings..  
-000174e0: 2020 4061 6464 5f73 7461 7274 5f64 6f63    @add_start_doc
-000174f0: 7374 7269 6e67 735f 746f 5f6d 6f64 656c  strings_to_model
-00017500: 5f66 6f72 7761 7264 2852 4546 4f52 4d45  _forward(REFORME
-00017510: 525f 494e 5055 5453 5f44 4f43 5354 5249  R_INPUTS_DOCSTRI
-00017520: 4e47 290a 2020 2020 4061 6464 5f63 6f64  NG).    @add_cod
-00017530: 655f 7361 6d70 6c65 5f64 6f63 7374 7269  e_sample_docstri
-00017540: 6e67 7328 0a20 2020 2020 2020 2074 6f6b  ngs(.        tok
-00017550: 656e 697a 6572 5f63 6c61 7373 3d5f 544f  enizer_class=_TO
-00017560: 4b45 4e49 5a45 525f 464f 525f 444f 432c  KENIZER_FOR_DOC,
-00017570: 0a20 2020 2020 2020 2063 6865 636b 706f  .        checkpo
-00017580: 696e 743d 5f43 4845 434b 504f 494e 545f  int=_CHECKPOINT_
-00017590: 464f 525f 444f 432c 0a20 2020 2020 2020  FOR_DOC,.       
-000175a0: 206f 7574 7075 745f 7479 7065 3d43 6175   output_type=Cau
-000175b0: 7361 6c4c 4d4f 7574 7075 742c 0a20 2020  salLMOutput,.   
-000175c0: 2020 2020 2063 6f6e 6669 675f 636c 6173       config_clas
-000175d0: 733d 5f43 4f4e 4649 475f 464f 525f 444f  s=_CONFIG_FOR_DO
-000175e0: 432c 0a20 2020 2029 0a20 2020 2064 6566  C,.    ).    def
-000175f0: 2066 6f72 7761 7264 280a 2020 2020 2020   forward(.      
-00017600: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00017610: 696e 7075 745f 6964 733d 4e6f 6e65 2c0a  input_ids=None,.
-00017620: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
-00017630: 5f69 6473 3d4e 6f6e 652c 0a20 2020 2020  _ids=None,.     
-00017640: 2020 2061 7474 656e 7469 6f6e 5f6d 6173     attention_mas
-00017650: 6b3d 4e6f 6e65 2c0a 2020 2020 2020 2020  k=None,.        
-00017660: 6865 6164 5f6d 6173 6b3d 4e6f 6e65 2c0a  head_mask=None,.
-00017670: 2020 2020 2020 2020 696e 7075 7473 5f65          inputs_e
-00017680: 6d62 6564 733d 4e6f 6e65 2c0a 2020 2020  mbeds=None,.    
-00017690: 2020 2020 6e75 6d5f 6861 7368 6573 3d4e      num_hashes=N
-000176a0: 6f6e 652c 0a20 2020 2020 2020 2070 6173  one,.        pas
-000176b0: 745f 6275 636b 6574 735f 7374 6174 6573  t_buckets_states
-000176c0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2075  =None,.        u
-000176d0: 7365 5f63 6163 6865 3d4e 6f6e 652c 0a20  se_cache=None,. 
-000176e0: 2020 2020 2020 206f 7574 7075 745f 6869         output_hi
-000176f0: 6464 656e 5f73 7461 7465 733d 4e6f 6e65  dden_states=None
-00017700: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
-00017710: 5f61 7474 656e 7469 6f6e 733d 4e6f 6e65  _attentions=None
-00017720: 2c0a 2020 2020 2020 2020 7265 7475 726e  ,.        return
-00017730: 5f64 6963 743d 4e6f 6e65 2c0a 2020 2020  _dict=None,.    
-00017740: 2020 2020 6c61 6265 6c73 3d4e 6f6e 652c      labels=None,
-00017750: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00017760: 7222 2222 0a20 2020 2020 2020 206c 6162  r""".        lab
-00017770: 656c 7320 283a 6f62 6a3a 6074 6f72 6368  els (:obj:`torch
-00017780: 2e4c 6f6e 6754 656e 736f 7260 206f 6620  .LongTensor` of 
-00017790: 7368 6170 6520 3a6f 626a 3a60 2862 6174  shape :obj:`(bat
-000177a0: 6368 5f73 697a 652c 2960 2c20 606f 7074  ch_size,)`, `opt
-000177b0: 696f 6e61 6c60 293a 0a20 2020 2020 2020  ional`):.       
-000177c0: 2020 2020 2020 2020 204c 6162 656c 7320           Labels 
-000177d0: 666f 7220 636f 6d70 7574 696e 6720 7468  for computing th
-000177e0: 6520 7365 7175 656e 6365 2063 6c61 7373  e sequence class
-000177f0: 6966 6963 6174 696f 6e2f 7265 6772 6573  ification/regres
-00017800: 7369 6f6e 206c 6f73 732e 2049 6e64 6963  sion loss. Indic
-00017810: 6573 2073 686f 756c 6420 6265 2069 6e20  es should be in 
-00017820: 3a6f 626a 3a60 5b2d 3130 302c 2030 2c0a  :obj:`[-100, 0,.
-00017830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00017840: 2e2e 2e2c 2063 6f6e 6669 672e 766f 6361  ..., config.voca
-00017850: 625f 7369 7a65 202d 2031 5d60 2e20 416c  b_size - 1]`. Al
-00017860: 6c20 6c61 6265 6c73 2073 6574 2074 6f20  l labels set to 
-00017870: 6060 2d31 3030 6060 2061 7265 2069 676e  ``-100`` are ign
-00017880: 6f72 6564 2028 6d61 736b 6564 292c 2074  ored (masked), t
-00017890: 6865 206c 6f73 7320 6973 206f 6e6c 790a  he loss is only.
-000178a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000178b0: 636f 6d70 7574 6564 2066 6f72 206c 6162  computed for lab
-000178c0: 656c 7320 696e 2060 605b 302c 202e 2e2e  els in ``[0, ...
-000178d0: 2c20 636f 6e66 6967 2e76 6f63 6162 5f73  , config.vocab_s
-000178e0: 697a 655d 6060 0a20 2020 2020 2020 2022  ize]``.        "
-000178f0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-00017900: 6e5f 6469 6374 203d 2072 6574 7572 6e5f  n_dict = return_
-00017910: 6469 6374 2069 6620 7265 7475 726e 5f64  dict if return_d
-00017920: 6963 7420 6973 206e 6f74 204e 6f6e 6520  ict is not None 
-00017930: 656c 7365 2073 656c 662e 636f 6e66 6967  else self.config
-00017940: 2e75 7365 5f72 6574 7572 6e5f 6469 6374  .use_return_dict
-00017950: 0a0a 2020 2020 2020 2020 7265 666f 726d  ..        reform
-00017960: 6572 5f6f 7574 7075 7473 203d 2073 656c  er_outputs = sel
-00017970: 662e 7265 666f 726d 6572 280a 2020 2020  f.reformer(.    
-00017980: 2020 2020 2020 2020 696e 7075 745f 6964          input_id
-00017990: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
-000179a0: 6f73 6974 696f 6e5f 6964 733d 706f 7369  osition_ids=posi
-000179b0: 7469 6f6e 5f69 6473 2c0a 2020 2020 2020  tion_ids,.      
-000179c0: 2020 2020 2020 6174 7465 6e74 696f 6e5f        attention_
-000179d0: 6d61 736b 3d61 7474 656e 7469 6f6e 5f6d  mask=attention_m
-000179e0: 6173 6b2c 0a20 2020 2020 2020 2020 2020  ask,.           
-000179f0: 2068 6561 645f 6d61 736b 3d68 6561 645f   head_mask=head_
-00017a00: 6d61 736b 2c0a 2020 2020 2020 2020 2020  mask,.          
-00017a10: 2020 696e 7075 7473 5f65 6d62 6564 733d    inputs_embeds=
-00017a20: 696e 7075 7473 5f65 6d62 6564 732c 0a20  inputs_embeds,. 
-00017a30: 2020 2020 2020 2020 2020 206e 756d 5f68             num_h
-00017a40: 6173 6865 733d 6e75 6d5f 6861 7368 6573  ashes=num_hashes
-00017a50: 2c0a 2020 2020 2020 2020 2020 2020 7061  ,.            pa
-00017a60: 7374 5f62 7563 6b65 7473 5f73 7461 7465  st_buckets_state
-00017a70: 733d 7061 7374 5f62 7563 6b65 7473 5f73  s=past_buckets_s
-00017a80: 7461 7465 732c 0a20 2020 2020 2020 2020  tates,.         
-00017a90: 2020 2075 7365 5f63 6163 6865 3d75 7365     use_cache=use
-00017aa0: 5f63 6163 6865 2c0a 2020 2020 2020 2020  _cache,.        
-00017ab0: 2020 2020 6f75 7470 7574 5f68 6964 6465      output_hidde
-00017ac0: 6e5f 7374 6174 6573 3d6f 7574 7075 745f  n_states=output_
-00017ad0: 6869 6464 656e 5f73 7461 7465 732c 0a20  hidden_states,. 
-00017ae0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-00017af0: 745f 6174 7465 6e74 696f 6e73 3d6f 7574  t_attentions=out
-00017b00: 7075 745f 6174 7465 6e74 696f 6e73 2c0a  put_attentions,.
-00017b10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00017b20: 726e 5f64 6963 743d 7265 7475 726e 5f64  rn_dict=return_d
-00017b30: 6963 742c 0a20 2020 2020 2020 2029 0a0a  ict,.        )..
-00017b40: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
-00017b50: 5f6f 7574 7075 7420 3d20 7265 666f 726d  _output = reform
-00017b60: 6572 5f6f 7574 7075 7473 5b30 5d0a 2020  er_outputs[0].  
-00017b70: 2020 2020 2020 6c6f 6769 7473 203d 2073        logits = s
-00017b80: 656c 662e 6c6d 5f68 6561 6428 7365 7175  elf.lm_head(sequ
-00017b90: 656e 6365 5f6f 7574 7075 7429 0a0a 2020  ence_output)..  
-00017ba0: 2020 2020 2020 6c6f 7373 203d 204e 6f6e        loss = Non
-00017bb0: 650a 2020 2020 2020 2020 6966 206c 6162  e.        if lab
-00017bc0: 656c 7320 6973 206e 6f74 204e 6f6e 653a  els is not None:
-00017bd0: 0a20 2020 2020 2020 2020 2020 2023 2053  .            # S
-00017be0: 6869 6674 2073 6f20 7468 6174 2074 6f6b  hift so that tok
-00017bf0: 656e 7320 3c20 6e20 7072 6564 6963 7420  ens < n predict 
-00017c00: 6e0a 2020 2020 2020 2020 2020 2020 7368  n.            sh
-00017c10: 6966 745f 6c6f 6769 7473 203d 206c 6f67  ift_logits = log
-00017c20: 6974 735b 2e2e 2e2c 203a 2d31 2c20 3a5d  its[..., :-1, :]
-00017c30: 2e63 6f6e 7469 6775 6f75 7328 290a 2020  .contiguous().  
-00017c40: 2020 2020 2020 2020 2020 7368 6966 745f            shift_
-00017c50: 6c61 6265 6c73 203d 206c 6162 656c 735b  labels = labels[
-00017c60: 2e2e 2e2c 2031 3a5d 2e63 6f6e 7469 6775  ..., 1:].contigu
-00017c70: 6f75 7328 290a 2020 2020 2020 2020 2020  ous().          
-00017c80: 2020 2320 466c 6174 7465 6e20 7468 6520    # Flatten the 
-00017c90: 746f 6b65 6e73 0a20 2020 2020 2020 2020  tokens.         
-00017ca0: 2020 206c 6f73 735f 6663 7420 3d20 4372     loss_fct = Cr
-00017cb0: 6f73 7345 6e74 726f 7079 4c6f 7373 2829  ossEntropyLoss()
-00017cc0: 0a20 2020 2020 2020 2020 2020 206c 6f73  .            los
-00017cd0: 7320 3d20 6c6f 7373 5f66 6374 2873 6869  s = loss_fct(shi
-00017ce0: 6674 5f6c 6f67 6974 732e 7669 6577 282d  ft_logits.view(-
-00017cf0: 312c 2073 656c 662e 636f 6e66 6967 2e76  1, self.config.v
-00017d00: 6f63 6162 5f73 697a 6529 2c20 7368 6966  ocab_size), shif
-00017d10: 745f 6c61 6265 6c73 2e76 6965 7728 2d31  t_labels.view(-1
-00017d20: 2929 0a0a 2020 2020 2020 2020 6966 206e  ))..        if n
-00017d30: 6f74 2072 6574 7572 6e5f 6469 6374 3a0a  ot return_dict:.
-00017d40: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
-00017d50: 7574 203d 2028 6c6f 6769 7473 2c29 202b  ut = (logits,) +
-00017d60: 2072 6566 6f72 6d65 725f 6f75 7470 7574   reformer_output
-00017d70: 735b 313a 5d0a 2020 2020 2020 2020 2020  s[1:].          
-00017d80: 2020 7265 7475 726e 2028 286c 6f73 732c    return ((loss,
-00017d90: 2920 2b20 6f75 7470 7574 2920 6966 206c  ) + output) if l
-00017da0: 6f73 7320 6973 206e 6f74 204e 6f6e 6520  oss is not None 
-00017db0: 656c 7365 206f 7574 7075 740a 0a20 2020  else output..   
-00017dc0: 2020 2020 2072 6574 7572 6e20 5265 666f       return Refo
-00017dd0: 726d 6572 4d6f 6465 6c57 6974 684c 4d48  rmerModelWithLMH
-00017de0: 6561 644f 7574 7075 7428 0a20 2020 2020  eadOutput(.     
-00017df0: 2020 2020 2020 206c 6f73 733d 6c6f 7373         loss=loss
-00017e00: 2c0a 2020 2020 2020 2020 2020 2020 6c6f  ,.            lo
-00017e10: 6769 7473 3d6c 6f67 6974 732c 0a20 2020  gits=logits,.   
-00017e20: 2020 2020 2020 2020 2070 6173 745f 6275           past_bu
-00017e30: 636b 6574 735f 7374 6174 6573 3d72 6566  ckets_states=ref
-00017e40: 6f72 6d65 725f 6f75 7470 7574 732e 7061  ormer_outputs.pa
-00017e50: 7374 5f62 7563 6b65 7473 5f73 7461 7465  st_buckets_state
-00017e60: 732c 0a20 2020 2020 2020 2020 2020 2068  s,.            h
-00017e70: 6964 6465 6e5f 7374 6174 6573 3d72 6566  idden_states=ref
-00017e80: 6f72 6d65 725f 6f75 7470 7574 732e 6869  ormer_outputs.hi
-00017e90: 6464 656e 5f73 7461 7465 732c 0a20 2020  dden_states,.   
-00017ea0: 2020 2020 2020 2020 2061 7474 656e 7469           attenti
-00017eb0: 6f6e 733d 7265 666f 726d 6572 5f6f 7574  ons=reformer_out
-00017ec0: 7075 7473 2e61 7474 656e 7469 6f6e 732c  puts.attentions,
-00017ed0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00017ee0: 6465 6620 7072 6570 6172 655f 696e 7075  def prepare_inpu
-00017ef0: 7473 5f66 6f72 5f67 656e 6572 6174 696f  ts_for_generatio
-00017f00: 6e28 7365 6c66 2c20 696e 7075 745f 6964  n(self, input_id
-00017f10: 732c 2070 6173 743d 4e6f 6e65 2c20 7573  s, past=None, us
-00017f20: 655f 6361 6368 653d 4e6f 6e65 2c20 6e75  e_cache=None, nu
-00017f30: 6d5f 6861 7368 6573 3d4e 6f6e 652c 202a  m_hashes=None, *
-00017f40: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00017f50: 2020 2320 6f6e 6c79 206c 6173 7420 746f    # only last to
-00017f60: 6b65 6e20 666f 7220 696e 7075 7473 5f69  ken for inputs_i
-00017f70: 6473 2069 6620 7061 7374 2069 7320 6465  ds if past is de
-00017f80: 6669 6e65 6420 696e 206b 7761 7267 730a  fined in kwargs.
-00017f90: 2020 2020 2020 2020 6966 2070 6173 7420          if past 
-00017fa0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00017fb0: 2020 2020 2020 2020 2069 6e70 7574 5f69           input_i
-00017fc0: 6473 203d 2069 6e70 7574 5f69 6473 5b3a  ds = input_ids[:
-00017fd0: 2c20 2d31 3a5d 0a0a 2020 2020 2020 2020  , -1:]..        
-00017fe0: 696e 7075 7473 5f64 6963 7420 3d20 7b0a  inputs_dict = {.
-00017ff0: 2020 2020 2020 2020 2020 2020 2269 6e70              "inp
-00018000: 7574 5f69 6473 223a 2069 6e70 7574 5f69  ut_ids": input_i
-00018010: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00018020: 2270 6173 745f 6275 636b 6574 735f 7374  "past_buckets_st
-00018030: 6174 6573 223a 2070 6173 742c 0a20 2020  ates": past,.   
-00018040: 2020 2020 2020 2020 2022 7573 655f 6361           "use_ca
-00018050: 6368 6522 3a20 7573 655f 6361 6368 652c  che": use_cache,
-00018060: 0a20 2020 2020 2020 2020 2020 2022 6e75  .            "nu
-00018070: 6d5f 6861 7368 6573 223a 206e 756d 5f68  m_hashes": num_h
-00018080: 6173 6865 732c 0a20 2020 2020 2020 207d  ashes,.        }
-00018090: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000180a0: 2069 6e70 7574 735f 6469 6374 0a0a 2020   inputs_dict..  
-000180b0: 2020 6465 6620 5f72 656f 7264 6572 5f63    def _reorder_c
-000180c0: 6163 6865 2873 656c 662c 2070 6173 742c  ache(self, past,
-000180d0: 2062 6561 6d5f 6964 7829 3a0a 2020 2020   beam_idx):.    
-000180e0: 2020 2020 7265 6f72 645f 7061 7374 5f62      reord_past_b
-000180f0: 7563 6b65 7473 5f73 7461 7465 7320 3d20  uckets_states = 
-00018100: 5b5d 0a20 2020 2020 2020 2066 6f72 206c  [].        for l
-00018110: 6179 6572 5f70 6173 7420 696e 2070 6173  ayer_past in pas
-00018120: 743a 0a20 2020 2020 2020 2020 2020 2023  t:.            #
-00018130: 2062 7563 6b65 7473 0a20 2020 2020 2020   buckets.       
-00018140: 2020 2020 2069 6620 6c61 7965 725f 7061       if layer_pa
-00018150: 7374 5b30 5d20 6973 206e 6f74 204e 6f6e  st[0] is not Non
-00018160: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00018170: 2020 2072 656f 7264 5f62 7563 6b65 7473     reord_buckets
-00018180: 203d 206c 6179 6572 5f70 6173 745b 305d   = layer_past[0]
-00018190: 2e69 6e64 6578 5f73 656c 6563 7428 302c  .index_select(0,
-000181a0: 2062 6561 6d5f 6964 7829 0a20 2020 2020   beam_idx).     
-000181b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000181c0: 2020 2020 2020 2020 2020 2020 2072 656f               reo
-000181d0: 7264 5f62 7563 6b65 7473 203d 204e 6f6e  rd_buckets = Non
-000181e0: 650a 0a20 2020 2020 2020 2020 2020 2023  e..            #
-000181f0: 2068 6964 6465 6e20 7374 6174 6573 0a20   hidden states. 
-00018200: 2020 2020 2020 2020 2020 2072 656f 7264             reord
-00018210: 5f68 6964 6465 6e5f 7374 6174 6573 203d  _hidden_states =
-00018220: 206c 6179 6572 5f70 6173 745b 315d 2e69   layer_past[1].i
-00018230: 6e64 6578 5f73 656c 6563 7428 302c 2062  ndex_select(0, b
-00018240: 6561 6d5f 6964 7829 0a20 2020 2020 2020  eam_idx).       
-00018250: 2020 2020 2072 656f 7264 5f70 6173 745f       reord_past_
-00018260: 6275 636b 6574 735f 7374 6174 6573 2e61  buckets_states.a
-00018270: 7070 656e 6428 2872 656f 7264 5f62 7563  ppend((reord_buc
-00018280: 6b65 7473 2c20 7265 6f72 645f 6869 6464  kets, reord_hidd
-00018290: 656e 5f73 7461 7465 7329 290a 2020 2020  en_states)).    
-000182a0: 2020 2020 7265 7475 726e 2072 656f 7264      return reord
-000182b0: 5f70 6173 745f 6275 636b 6574 735f 7374  _past_buckets_st
-000182c0: 6174 6573 0a0a 0a40 6164 645f 7374 6172  ates...@add_star
-000182d0: 745f 646f 6373 7472 696e 6773 2822 2222  t_docstrings("""
-000182e0: 5265 666f 726d 6572 204d 6f64 656c 2077  Reformer Model w
-000182f0: 6974 6820 6120 606c 616e 6775 6167 6520  ith a `language 
-00018300: 6d6f 6465 6c69 6e67 6020 6865 6164 206f  modeling` head o
-00018310: 6e20 746f 702e 2022 2222 2c20 5245 464f  n top. """, REFO
-00018320: 524d 4552 5f53 5441 5254 5f44 4f43 5354  RMER_START_DOCST
-00018330: 5249 4e47 290a 636c 6173 7320 5265 666f  RING).class Refo
-00018340: 726d 6572 466f 724d 6173 6b65 644c 4d28  rmerForMaskedLM(
-00018350: 5265 666f 726d 6572 5072 6554 7261 696e  ReformerPreTrain
-00018360: 6564 4d6f 6465 6c29 3a0a 2020 2020 6465  edModel):.    de
-00018370: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-00018380: 2063 6f6e 6669 6729 3a0a 2020 2020 2020   config):.      
-00018390: 2020 7375 7065 7228 292e 5f5f 696e 6974    super().__init
-000183a0: 5f5f 2863 6f6e 6669 6729 0a20 2020 2020  __(config).     
-000183b0: 2020 2061 7373 6572 7420 280a 2020 2020     assert (.    
-000183c0: 2020 2020 2020 2020 6e6f 7420 636f 6e66          not conf
-000183d0: 6967 2e69 735f 6465 636f 6465 720a 2020  ig.is_decoder.  
-000183e0: 2020 2020 2020 292c 2022 4966 2079 6f75        ), "If you
-000183f0: 2077 616e 7420 746f 2075 7365 2060 5265   want to use `Re
-00018400: 666f 726d 6572 466f 724d 6173 6b65 644c  formerForMaskedL
-00018410: 4d60 206d 616b 6520 7375 7265 2060 636f  M` make sure `co
-00018420: 6e66 6967 2e69 735f 6465 636f 6465 723d  nfig.is_decoder=
-00018430: 4661 6c73 6560 2066 6f72 2062 692d 6469  False` for bi-di
-00018440: 7265 6374 696f 6e61 6c20 7365 6c66 2d61  rectional self-a
-00018450: 7474 656e 7469 6f6e 2e22 0a20 2020 2020  ttention.".     
-00018460: 2020 2073 656c 662e 7265 666f 726d 6572     self.reformer
-00018470: 203d 2052 6566 6f72 6d65 724d 6f64 656c   = ReformerModel
-00018480: 2863 6f6e 6669 6729 0a20 2020 2020 2020  (config).       
-00018490: 2073 656c 662e 6c6d 5f68 6561 6420 3d20   self.lm_head = 
-000184a0: 5265 666f 726d 6572 4f6e 6c79 4c4d 4865  ReformerOnlyLMHe
-000184b0: 6164 2863 6f6e 6669 6729 0a0a 2020 2020  ad(config)..    
-000184c0: 2020 2020 7365 6c66 2e69 6e69 745f 7765      self.init_we
-000184d0: 6967 6874 7328 290a 0a20 2020 2064 6566  ights()..    def
-000184e0: 2067 6574 5f6f 7574 7075 745f 656d 6265   get_output_embe
-000184f0: 6464 696e 6773 2873 656c 6629 3a0a 2020  ddings(self):.  
-00018500: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00018510: 662e 6c6d 5f68 6561 642e 6465 636f 6465  f.lm_head.decode
-00018520: 720a 0a20 2020 2064 6566 2073 6574 5f6f  r..    def set_o
-00018530: 7574 7075 745f 656d 6265 6464 696e 6773  utput_embeddings
-00018540: 2873 656c 662c 206e 6577 5f65 6d62 6564  (self, new_embed
-00018550: 6469 6e67 7329 3a0a 2020 2020 2020 2020  dings):.        
-00018560: 7365 6c66 2e6c 6d5f 6865 6164 2e64 6563  self.lm_head.dec
-00018570: 6f64 6572 203d 206e 6577 5f65 6d62 6564  oder = new_embed
-00018580: 6469 6e67 730a 0a20 2020 2040 6164 645f  dings..    @add_
-00018590: 7374 6172 745f 646f 6373 7472 696e 6773  start_docstrings
-000185a0: 5f74 6f5f 6d6f 6465 6c5f 666f 7277 6172  _to_model_forwar
-000185b0: 6428 5245 464f 524d 4552 5f49 4e50 5554  d(REFORMER_INPUT
-000185c0: 535f 444f 4353 5452 494e 4729 0a20 2020  S_DOCSTRING).   
-000185d0: 2040 6164 645f 636f 6465 5f73 616d 706c   @add_code_sampl
-000185e0: 655f 646f 6373 7472 696e 6773 280a 2020  e_docstrings(.  
-000185f0: 2020 2020 2020 746f 6b65 6e69 7a65 725f        tokenizer_
-00018600: 636c 6173 733d 5f54 4f4b 454e 495a 4552  class=_TOKENIZER
-00018610: 5f46 4f52 5f44 4f43 2c0a 2020 2020 2020  _FOR_DOC,.      
-00018620: 2020 6368 6563 6b70 6f69 6e74 3d5f 4348    checkpoint=_CH
-00018630: 4543 4b50 4f49 4e54 5f46 4f52 5f44 4f43  ECKPOINT_FOR_DOC
-00018640: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
-00018650: 5f74 7970 653d 4d61 736b 6564 4c4d 4f75  _type=MaskedLMOu
-00018660: 7470 7574 2c0a 2020 2020 2020 2020 636f  tput,.        co
-00018670: 6e66 6967 5f63 6c61 7373 3d5f 434f 4e46  nfig_class=_CONF
-00018680: 4947 5f46 4f52 5f44 4f43 2c0a 2020 2020  IG_FOR_DOC,.    
-00018690: 290a 2020 2020 6465 6620 666f 7277 6172  ).    def forwar
-000186a0: 6428 0a20 2020 2020 2020 2073 656c 662c  d(.        self,
-000186b0: 0a20 2020 2020 2020 2069 6e70 7574 5f69  .        input_i
-000186c0: 6473 3d4e 6f6e 652c 0a20 2020 2020 2020  ds=None,.       
-000186d0: 2070 6f73 6974 696f 6e5f 6964 733d 4e6f   position_ids=No
-000186e0: 6e65 2c0a 2020 2020 2020 2020 6174 7465  ne,.        atte
-000186f0: 6e74 696f 6e5f 6d61 736b 3d4e 6f6e 652c  ntion_mask=None,
-00018700: 0a20 2020 2020 2020 2068 6561 645f 6d61  .        head_ma
-00018710: 736b 3d4e 6f6e 652c 0a20 2020 2020 2020  sk=None,.       
-00018720: 2069 6e70 7574 735f 656d 6265 6473 3d4e   inputs_embeds=N
-00018730: 6f6e 652c 0a20 2020 2020 2020 206e 756d  one,.        num
-00018740: 5f68 6173 6865 733d 4e6f 6e65 2c0a 2020  _hashes=None,.  
-00018750: 2020 2020 2020 6c61 6265 6c73 3d4e 6f6e        labels=Non
-00018760: 652c 0a20 2020 2020 2020 206f 7574 7075  e,.        outpu
-00018770: 745f 6869 6464 656e 5f73 7461 7465 733d  t_hidden_states=
-00018780: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f75  None,.        ou
-00018790: 7470 7574 5f61 7474 656e 7469 6f6e 733d  tput_attentions=
-000187a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 7265  None,.        re
-000187b0: 7475 726e 5f64 6963 743d 4e6f 6e65 2c0a  turn_dict=None,.
-000187c0: 2020 2020 293a 0a20 2020 2020 2020 2072      ):.        r
-000187d0: 2222 220a 2020 2020 2020 2020 6c61 6265  """.        labe
-000187e0: 6c73 2028 3a6f 626a 3a60 746f 7263 682e  ls (:obj:`torch.
-000187f0: 4c6f 6e67 5465 6e73 6f72 6020 6f66 2073  LongTensor` of s
-00018800: 6861 7065 203a 6f62 6a3a 6028 6261 7463  hape :obj:`(batc
-00018810: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
-00018820: 5f6c 656e 6774 6829 602c 2060 6f70 7469  _length)`, `opti
-00018830: 6f6e 616c 6029 3a0a 2020 2020 2020 2020  onal`):.        
-00018840: 2020 2020 2020 2020 4c61 6265 6c73 2066          Labels f
-00018850: 6f72 2063 6f6d 7075 7469 6e67 2074 6865  or computing the
-00018860: 206d 6173 6b65 6420 6c61 6e67 7561 6765   masked language
-00018870: 206d 6f64 656c 696e 6720 6c6f 7373 2e20   modeling loss. 
-00018880: 496e 6469 6365 7320 7368 6f75 6c64 2062  Indices should b
-00018890: 6520 696e 2060 605b 2d31 3030 2c20 302c  e in ``[-100, 0,
-000188a0: 202e 2e2e 2c0a 2020 2020 2020 2020 2020   ...,.          
-000188b0: 2020 2020 2020 636f 6e66 6967 2e76 6f63        config.voc
-000188c0: 6162 5f73 697a 655d 6060 2028 7365 6520  ab_size]`` (see 
-000188d0: 6060 696e 7075 745f 6964 7360 6020 646f  ``input_ids`` do
-000188e0: 6373 7472 696e 6729 2054 6f6b 656e 7320  cstring) Tokens 
-000188f0: 7769 7468 2069 6e64 6963 6573 2073 6574  with indices set
-00018900: 2074 6f20 6060 2d31 3030 6060 2061 7265   to ``-100`` are
-00018910: 2069 676e 6f72 6564 0a20 2020 2020 2020   ignored.       
-00018920: 2020 2020 2020 2020 2028 6d61 736b 6564           (masked
-00018930: 292c 2074 6865 206c 6f73 7320 6973 206f  ), the loss is o
-00018940: 6e6c 7920 636f 6d70 7574 6564 2066 6f72  nly computed for
-00018950: 2074 6865 2074 6f6b 656e 7320 7769 7468   the tokens with
-00018960: 206c 6162 656c 730a 2020 2020 2020 2020   labels.        
-00018970: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
-00018980: 726e 5f64 6963 7420 3d20 7265 7475 726e  rn_dict = return
-00018990: 5f64 6963 7420 6966 2072 6574 7572 6e5f  _dict if return_
-000189a0: 6469 6374 2069 7320 6e6f 7420 4e6f 6e65  dict is not None
-000189b0: 2065 6c73 6520 7365 6c66 2e63 6f6e 6669   else self.confi
-000189c0: 672e 7573 655f 7265 7475 726e 5f64 6963  g.use_return_dic
-000189d0: 740a 0a20 2020 2020 2020 2072 6566 6f72  t..        refor
-000189e0: 6d65 725f 6f75 7470 7574 7320 3d20 7365  mer_outputs = se
-000189f0: 6c66 2e72 6566 6f72 6d65 7228 0a20 2020  lf.reformer(.   
-00018a00: 2020 2020 2020 2020 2069 6e70 7574 5f69           input_i
-00018a10: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
-00018a20: 706f 7369 7469 6f6e 5f69 6473 3d70 6f73  position_ids=pos
-00018a30: 6974 696f 6e5f 6964 732c 0a20 2020 2020  ition_ids,.     
-00018a40: 2020 2020 2020 2061 7474 656e 7469 6f6e         attention
-00018a50: 5f6d 6173 6b3d 6174 7465 6e74 696f 6e5f  _mask=attention_
-00018a60: 6d61 736b 2c0a 2020 2020 2020 2020 2020  mask,.          
-00018a70: 2020 6865 6164 5f6d 6173 6b3d 6865 6164    head_mask=head
-00018a80: 5f6d 6173 6b2c 0a20 2020 2020 2020 2020  _mask,.         
-00018a90: 2020 2069 6e70 7574 735f 656d 6265 6473     inputs_embeds
-00018aa0: 3d69 6e70 7574 735f 656d 6265 6473 2c0a  =inputs_embeds,.
-00018ab0: 2020 2020 2020 2020 2020 2020 6e75 6d5f              num_
-00018ac0: 6861 7368 6573 3d6e 756d 5f68 6173 6865  hashes=num_hashe
-00018ad0: 732c 0a20 2020 2020 2020 2020 2020 2075  s,.            u
-00018ae0: 7365 5f63 6163 6865 3d46 616c 7365 2c20  se_cache=False, 
-00018af0: 2023 206e 6f20 6361 7573 616c 206d 6173   # no causal mas
-00018b00: 6b0a 2020 2020 2020 2020 2020 2020 6f75  k.            ou
-00018b10: 7470 7574 5f68 6964 6465 6e5f 7374 6174  tput_hidden_stat
-00018b20: 6573 3d6f 7574 7075 745f 6869 6464 656e  es=output_hidden
-00018b30: 5f73 7461 7465 732c 0a20 2020 2020 2020  _states,.       
-00018b40: 2020 2020 206f 7574 7075 745f 6174 7465       output_atte
-00018b50: 6e74 696f 6e73 3d6f 7574 7075 745f 6174  ntions=output_at
-00018b60: 7465 6e74 696f 6e73 2c0a 2020 2020 2020  tentions,.      
-00018b70: 2020 2020 2020 7265 7475 726e 5f64 6963        return_dic
-00018b80: 743d 7265 7475 726e 5f64 6963 742c 0a20  t=return_dict,. 
-00018b90: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00018ba0: 2020 7365 7175 656e 6365 5f6f 7574 7075    sequence_outpu
-00018bb0: 7420 3d20 7265 666f 726d 6572 5f6f 7574  t = reformer_out
-00018bc0: 7075 7473 5b30 5d0a 2020 2020 2020 2020  puts[0].        
-00018bd0: 6c6f 6769 7473 203d 2073 656c 662e 6c6d  logits = self.lm
-00018be0: 5f68 6561 6428 7365 7175 656e 6365 5f6f  _head(sequence_o
-00018bf0: 7574 7075 7429 0a0a 2020 2020 2020 2020  utput)..        
-00018c00: 6d61 736b 6564 5f6c 6d5f 6c6f 7373 203d  masked_lm_loss =
-00018c10: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-00018c20: 206c 6162 656c 7320 6973 206e 6f74 204e   labels is not N
-00018c30: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-00018c40: 206c 6f73 735f 6663 7420 3d20 4372 6f73   loss_fct = Cros
-00018c50: 7345 6e74 726f 7079 4c6f 7373 2829 2020  sEntropyLoss()  
-00018c60: 2320 2d31 3030 2069 6e64 6578 203d 2070  # -100 index = p
-00018c70: 6164 6469 6e67 2074 6f6b 656e 0a20 2020  adding token.   
-00018c80: 2020 2020 2020 2020 206d 6173 6b65 645f           masked_
-00018c90: 6c6d 5f6c 6f73 7320 3d20 6c6f 7373 5f66  lm_loss = loss_f
-00018ca0: 6374 286c 6f67 6974 732e 7669 6577 282d  ct(logits.view(-
-00018cb0: 312c 2073 656c 662e 636f 6e66 6967 2e76  1, self.config.v
-00018cc0: 6f63 6162 5f73 697a 6529 2c20 6c61 6265  ocab_size), labe
-00018cd0: 6c73 2e76 6965 7728 2d31 2929 0a0a 2020  ls.view(-1))..  
-00018ce0: 2020 2020 2020 6966 206e 6f74 2072 6574        if not ret
-00018cf0: 7572 6e5f 6469 6374 3a0a 2020 2020 2020  urn_dict:.      
-00018d00: 2020 2020 2020 6f75 7470 7574 203d 2028        output = (
-00018d10: 6c6f 6769 7473 2c29 202b 2072 6566 6f72  logits,) + refor
-00018d20: 6d65 725f 6f75 7470 7574 735b 313a 5d0a  mer_outputs[1:].
-00018d30: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00018d40: 726e 2028 286d 6173 6b65 645f 6c6d 5f6c  rn ((masked_lm_l
-00018d50: 6f73 732c 2920 2b20 6f75 7470 7574 2920  oss,) + output) 
-00018d60: 6966 206d 6173 6b65 645f 6c6d 5f6c 6f73  if masked_lm_los
-00018d70: 7320 6973 206e 6f74 204e 6f6e 6520 656c  s is not None el
-00018d80: 7365 206f 7574 7075 740a 0a20 2020 2020  se output..     
-00018d90: 2020 2072 6574 7572 6e20 4d61 736b 6564     return Masked
-00018da0: 4c4d 4f75 7470 7574 280a 2020 2020 2020  LMOutput(.      
-00018db0: 2020 2020 2020 6c6f 7373 3d6d 6173 6b65        loss=maske
-00018dc0: 645f 6c6d 5f6c 6f73 732c 0a20 2020 2020  d_lm_loss,.     
-00018dd0: 2020 2020 2020 206c 6f67 6974 733d 6c6f         logits=lo
-00018de0: 6769 7473 2c0a 2020 2020 2020 2020 2020  gits,.          
-00018df0: 2020 6869 6464 656e 5f73 7461 7465 733d    hidden_states=
-00018e00: 7265 666f 726d 6572 5f6f 7574 7075 7473  reformer_outputs
-00018e10: 2e68 6964 6465 6e5f 7374 6174 6573 2c0a  .hidden_states,.
-00018e20: 2020 2020 2020 2020 2020 2020 6174 7465              atte
-00018e30: 6e74 696f 6e73 3d72 6566 6f72 6d65 725f  ntions=reformer_
-00018e40: 6f75 7470 7574 732e 6174 7465 6e74 696f  outputs.attentio
-00018e50: 6e73 2c0a 2020 2020 2020 2020 290a 0a0a  ns,.        )...
-00018e60: 4061 6464 5f73 7461 7274 5f64 6f63 7374  @add_start_docst
-00018e70: 7269 6e67 7328 0a20 2020 2022 2222 0a20  rings(.    """. 
-00018e80: 2020 2052 6566 6f72 6d65 7220 4d6f 6465     Reformer Mode
-00018e90: 6c20 7472 616e 7366 6f72 6d65 7220 7769  l transformer wi
-00018ea0: 7468 2061 2073 6571 7565 6e63 6520 636c  th a sequence cl
-00018eb0: 6173 7369 6669 6361 7469 6f6e 2f72 6567  assification/reg
-00018ec0: 7265 7373 696f 6e20 6865 6164 206f 6e20  ression head on 
-00018ed0: 746f 7020 2861 206c 696e 6561 7220 6c61  top (a linear la
-00018ee0: 7965 7220 6f6e 2074 6f70 206f 6620 7468  yer on top of th
-00018ef0: 650a 2020 2020 706f 6f6c 6564 206f 7574  e.    pooled out
-00018f00: 7075 7429 2065 2e67 2e20 666f 7220 474c  put) e.g. for GL
-00018f10: 5545 2074 6173 6b73 2e0a 2020 2020 2222  UE tasks..    ""
-00018f20: 222c 0a20 2020 2052 4546 4f52 4d45 525f  ",.    REFORMER_
-00018f30: 5354 4152 545f 444f 4353 5452 494e 472c  START_DOCSTRING,
-00018f40: 0a29 0a63 6c61 7373 2052 6566 6f72 6d65  .).class Reforme
-00018f50: 7246 6f72 5365 7175 656e 6365 436c 6173  rForSequenceClas
-00018f60: 7369 6669 6361 7469 6f6e 2852 6566 6f72  sification(Refor
-00018f70: 6d65 7250 7265 5472 6169 6e65 644d 6f64  merPreTrainedMod
-00018f80: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
-00018f90: 6e69 745f 5f28 7365 6c66 2c20 636f 6e66  nit__(self, conf
-00018fa0: 6967 293a 0a20 2020 2020 2020 2073 7570  ig):.        sup
-00018fb0: 6572 2829 2e5f 5f69 6e69 745f 5f28 636f  er().__init__(co
-00018fc0: 6e66 6967 290a 2020 2020 2020 2020 7365  nfig).        se
-00018fd0: 6c66 2e6e 756d 5f6c 6162 656c 7320 3d20  lf.num_labels = 
-00018fe0: 636f 6e66 6967 2e6e 756d 5f6c 6162 656c  config.num_label
-00018ff0: 730a 2020 2020 2020 2020 7365 6c66 2e63  s.        self.c
-00019000: 6f6e 6669 6720 3d20 636f 6e66 6967 0a0a  onfig = config..
-00019010: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
-00019020: 6f72 6d65 7220 3d20 5265 666f 726d 6572  ormer = Reformer
-00019030: 4d6f 6465 6c28 636f 6e66 6967 290a 2020  Model(config).  
-00019040: 2020 2020 2020 7365 6c66 2e63 6c61 7373        self.class
-00019050: 6966 6965 7220 3d20 5265 666f 726d 6572  ifier = Reformer
-00019060: 436c 6173 7369 6669 6361 7469 6f6e 4865  ClassificationHe
-00019070: 6164 2863 6f6e 6669 6729 0a20 2020 2020  ad(config).     
-00019080: 2020 2069 6620 636f 6e66 6967 2e69 735f     if config.is_
-00019090: 6465 636f 6465 7220 6973 2054 7275 653a  decoder is True:
-000190a0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-000190b0: 6765 722e 7761 726e 696e 6728 2259 6f75  ger.warning("You
-000190c0: 206d 6967 6874 2077 616e 7420 746f 2064   might want to d
-000190d0: 6973 6162 6c65 2063 6175 7361 6c20 6d61  isable causal ma
-000190e0: 736b 696e 6720 666f 7220 7365 7175 656e  sking for sequen
-000190f0: 6365 2063 6c61 7373 6966 6963 6174 696f  ce classificatio
-00019100: 6e22 290a 0a20 2020 2020 2020 2073 656c  n")..        sel
-00019110: 662e 696e 6974 5f77 6569 6768 7473 2829  f.init_weights()
-00019120: 0a0a 2020 2020 4061 6464 5f73 7461 7274  ..    @add_start
-00019130: 5f64 6f63 7374 7269 6e67 735f 746f 5f6d  _docstrings_to_m
-00019140: 6f64 656c 5f66 6f72 7761 7264 2852 4546  odel_forward(REF
-00019150: 4f52 4d45 525f 494e 5055 5453 5f44 4f43  ORMER_INPUTS_DOC
-00019160: 5354 5249 4e47 290a 2020 2020 4061 6464  STRING).    @add
-00019170: 5f63 6f64 655f 7361 6d70 6c65 5f64 6f63  _code_sample_doc
-00019180: 7374 7269 6e67 7328 0a20 2020 2020 2020  strings(.       
-00019190: 2074 6f6b 656e 697a 6572 5f63 6c61 7373   tokenizer_class
-000191a0: 3d5f 544f 4b45 4e49 5a45 525f 464f 525f  =_TOKENIZER_FOR_
-000191b0: 444f 432c 0a20 2020 2020 2020 2063 6865  DOC,.        che
-000191c0: 636b 706f 696e 743d 5f43 4845 434b 504f  ckpoint=_CHECKPO
-000191d0: 494e 545f 464f 525f 444f 432c 0a20 2020  INT_FOR_DOC,.   
-000191e0: 2020 2020 206f 7574 7075 745f 7479 7065       output_type
-000191f0: 3d53 6571 7565 6e63 6543 6c61 7373 6966  =SequenceClassif
-00019200: 6965 724f 7574 7075 742c 0a20 2020 2020  ierOutput,.     
-00019210: 2020 2063 6f6e 6669 675f 636c 6173 733d     config_class=
-00019220: 5f43 4f4e 4649 475f 464f 525f 444f 432c  _CONFIG_FOR_DOC,
-00019230: 0a20 2020 2029 0a20 2020 2064 6566 2066  .    ).    def f
-00019240: 6f72 7761 7264 280a 2020 2020 2020 2020  orward(.        
-00019250: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
-00019260: 7075 745f 6964 733d 4e6f 6e65 2c0a 2020  put_ids=None,.  
-00019270: 2020 2020 2020 706f 7369 7469 6f6e 5f69        position_i
-00019280: 6473 3d4e 6f6e 652c 0a20 2020 2020 2020  ds=None,.       
-00019290: 2061 7474 656e 7469 6f6e 5f6d 6173 6b3d   attention_mask=
-000192a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 6865  None,.        he
-000192b0: 6164 5f6d 6173 6b3d 4e6f 6e65 2c0a 2020  ad_mask=None,.  
-000192c0: 2020 2020 2020 696e 7075 7473 5f65 6d62        inputs_emb
-000192d0: 6564 733d 4e6f 6e65 2c0a 2020 2020 2020  eds=None,.      
-000192e0: 2020 6e75 6d5f 6861 7368 6573 3d4e 6f6e    num_hashes=Non
-000192f0: 652c 0a20 2020 2020 2020 206c 6162 656c  e,.        label
+00011f00: 2020 2020 2020 2020 7365 6c66 2e64 6563          self.dec
+00011f10: 6f64 6572 2e62 6961 7320 3d20 7365 6c66  oder.bias = self
+00011f20: 2e62 6961 730a 0a20 2020 2064 6566 2066  .bias..    def f
+00011f30: 6f72 7761 7264 2873 656c 662c 2068 6964  orward(self, hid
+00011f40: 6465 6e5f 7374 6174 6573 293a 0a20 2020  den_states):.   
+00011f50: 2020 2020 2072 6574 7572 6e20 6170 706c       return appl
+00011f60: 795f 6368 756e 6b69 6e67 5f74 6f5f 666f  y_chunking_to_fo
+00011f70: 7277 6172 6428 7365 6c66 2e66 6f72 7761  rward(self.forwa
+00011f80: 7264 5f63 6875 6e6b 2c20 7365 6c66 2e63  rd_chunk, self.c
+00011f90: 6875 6e6b 5f73 697a 655f 6c6d 5f68 6561  hunk_size_lm_hea
+00011fa0: 642c 2073 656c 662e 7365 715f 6c65 6e5f  d, self.seq_len_
+00011fb0: 6469 6d2c 2068 6964 6465 6e5f 7374 6174  dim, hidden_stat
+00011fc0: 6573 290a 0a20 2020 2064 6566 2066 6f72  es)..    def for
+00011fd0: 7761 7264 5f63 6875 6e6b 2873 656c 662c  ward_chunk(self,
+00011fe0: 2068 6964 6465 6e5f 7374 6174 6573 293a   hidden_states):
+00011ff0: 0a20 2020 2020 2020 2068 6964 6465 6e5f  .        hidden_
+00012000: 7374 6174 6573 203d 2073 656c 662e 6465  states = self.de
+00012010: 636f 6465 7228 6869 6464 656e 5f73 7461  coder(hidden_sta
+00012020: 7465 7329 0a20 2020 2020 2020 2072 6574  tes).        ret
+00012030: 7572 6e20 6869 6464 656e 5f73 7461 7465  urn hidden_state
+00012040: 730a 0a20 2020 2064 6566 205f 7469 655f  s..    def _tie_
+00012050: 7765 6967 6874 7328 7365 6c66 293a 0a20  weights(self):. 
+00012060: 2020 2020 2020 2023 2054 6f20 7469 6520         # To tie 
+00012070: 7468 6f73 6520 7477 6f20 7765 6967 6874  those two weight
+00012080: 7320 6966 2074 6865 7920 6765 7420 6469  s if they get di
+00012090: 7363 6f6e 6e65 6374 6564 2028 6f6e 2054  sconnected (on T
+000120a0: 5055 206f 7220 7768 656e 2074 6865 2062  PU or when the b
+000120b0: 6961 7320 6973 2072 6573 697a 6564 290a  ias is resized).
+000120c0: 2020 2020 2020 2020 7365 6c66 2e62 6961          self.bia
+000120d0: 7320 3d20 7365 6c66 2e64 6563 6f64 6572  s = self.decoder
+000120e0: 2e62 6961 730a 0a0a 636c 6173 7320 5265  .bias...class Re
+000120f0: 666f 726d 6572 5072 6554 7261 696e 6564  formerPreTrained
+00012100: 4d6f 6465 6c28 5072 6554 7261 696e 6564  Model(PreTrained
+00012110: 4d6f 6465 6c29 3a0a 2020 2020 2222 220a  Model):.    """.
+00012120: 2020 2020 416e 2061 6273 7472 6163 7420      An abstract 
+00012130: 636c 6173 7320 746f 2068 616e 646c 6520  class to handle 
+00012140: 7765 6967 6874 7320 696e 6974 6961 6c69  weights initiali
+00012150: 7a61 7469 6f6e 2061 6e64 2061 2073 696d  zation and a sim
+00012160: 706c 6520 696e 7465 7266 6163 6520 666f  ple interface fo
+00012170: 7220 646f 776e 6c6f 6164 696e 6720 616e  r downloading an
+00012180: 6420 6c6f 6164 696e 6720 7072 6574 7261  d loading pretra
+00012190: 696e 6564 0a20 2020 206d 6f64 656c 732e  ined.    models.
+000121a0: 0a20 2020 2022 2222 0a0a 2020 2020 636f  .    """..    co
+000121b0: 6e66 6967 5f63 6c61 7373 203d 2052 6566  nfig_class = Ref
+000121c0: 6f72 6d65 7243 6f6e 6669 670a 2020 2020  ormerConfig.    
+000121d0: 6261 7365 5f6d 6f64 656c 5f70 7265 6669  base_model_prefi
+000121e0: 7820 3d20 2272 6566 6f72 6d65 7222 0a0a  x = "reformer"..
+000121f0: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00012200: 2020 6465 6620 6475 6d6d 795f 696e 7075    def dummy_inpu
+00012210: 7473 2873 656c 6629 3a0a 2020 2020 2020  ts(self):.      
+00012220: 2020 696e 7075 745f 6964 7320 3d20 746f    input_ids = to
+00012230: 7263 682e 7465 6e73 6f72 2844 554d 4d59  rch.tensor(DUMMY
+00012240: 5f49 4e50 5554 5329 0a20 2020 2020 2020  _INPUTS).       
+00012250: 2069 6e70 7574 5f6d 6173 6b20 3d20 746f   input_mask = to
+00012260: 7263 682e 7465 6e73 6f72 2844 554d 4d59  rch.tensor(DUMMY
+00012270: 5f4d 4153 4b29 0a20 2020 2020 2020 2064  _MASK).        d
+00012280: 756d 6d79 5f69 6e70 7574 7320 3d20 7b0a  ummy_inputs = {.
+00012290: 2020 2020 2020 2020 2020 2020 2269 6e70              "inp
+000122a0: 7574 5f69 6473 223a 2069 6e70 7574 5f69  ut_ids": input_i
+000122b0: 6473 2c0a 2020 2020 2020 2020 2020 2020  ds,.            
+000122c0: 2261 7474 656e 7469 6f6e 5f6d 6173 6b22  "attention_mask"
+000122d0: 3a20 696e 7075 745f 6d61 736b 2c0a 2020  : input_mask,.  
+000122e0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+000122f0: 7265 7475 726e 2064 756d 6d79 5f69 6e70  return dummy_inp
+00012300: 7574 730a 0a20 2020 2064 6566 205f 696e  uts..    def _in
+00012310: 6974 5f77 6569 6768 7473 2873 656c 662c  it_weights(self,
+00012320: 206d 6f64 756c 6529 3a0a 2020 2020 2020   module):.      
+00012330: 2020 2222 2249 6e69 7469 616c 697a 6520    """Initialize 
+00012340: 7468 6520 7765 6967 6874 7322 2222 0a20  the weights""". 
+00012350: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00012360: 616e 6365 286d 6f64 756c 652c 2041 7869  ance(module, Axi
+00012370: 616c 506f 7369 7469 6f6e 456d 6265 6464  alPositionEmbedd
+00012380: 696e 6773 293a 0a20 2020 2020 2020 2020  ings):.         
+00012390: 2020 2066 6f72 2077 6569 6768 7420 696e     for weight in
+000123a0: 206d 6f64 756c 652e 7765 6967 6874 733a   module.weights:
+000123b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000123c0: 206e 6e2e 696e 6974 2e6e 6f72 6d61 6c5f   nn.init.normal_
+000123d0: 2877 6569 6768 742c 2073 7464 3d73 656c  (weight, std=sel
+000123e0: 662e 636f 6e66 6967 2e61 7869 616c 5f6e  f.config.axial_n
+000123f0: 6f72 6d5f 7374 6429 0a20 2020 2020 2020  orm_std).       
+00012400: 2065 6c69 6620 6973 696e 7374 616e 6365   elif isinstance
+00012410: 286d 6f64 756c 652c 206e 6e2e 456d 6265  (module, nn.Embe
+00012420: 6464 696e 6729 3a0a 2020 2020 2020 2020  dding):.        
+00012430: 2020 2020 6d6f 6475 6c65 2e77 6569 6768      module.weigh
+00012440: 742e 6461 7461 2e6e 6f72 6d61 6c5f 286d  t.data.normal_(m
+00012450: 6561 6e3d 302e 302c 2073 7464 3d73 656c  ean=0.0, std=sel
+00012460: 662e 636f 6e66 6967 2e69 6e69 7469 616c  f.config.initial
+00012470: 697a 6572 5f72 616e 6765 290a 2020 2020  izer_range).    
+00012480: 2020 2020 2020 2020 6966 206d 6f64 756c          if modul
+00012490: 652e 7061 6464 696e 675f 6964 7820 6973  e.padding_idx is
+000124a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+000124b0: 2020 2020 2020 2020 2020 206d 6f64 756c             modul
+000124c0: 652e 7765 6967 6874 2e64 6174 615b 6d6f  e.weight.data[mo
+000124d0: 6475 6c65 2e70 6164 6469 6e67 5f69 6478  dule.padding_idx
+000124e0: 5d2e 7a65 726f 5f28 290a 2020 2020 2020  ].zero_().      
+000124f0: 2020 656c 6966 2069 7369 6e73 7461 6e63    elif isinstanc
+00012500: 6528 6d6f 6475 6c65 2c20 6e6e 2e4c 696e  e(module, nn.Lin
+00012510: 6561 7229 3a0a 2020 2020 2020 2020 2020  ear):.          
+00012520: 2020 2320 536c 6967 6874 6c79 2064 6966    # Slightly dif
+00012530: 6665 7265 6e74 2066 726f 6d20 7468 6520  ferent from the 
+00012540: 5446 2076 6572 7369 6f6e 2077 6869 6368  TF version which
+00012550: 2075 7365 7320 7472 756e 6361 7465 645f   uses truncated_
+00012560: 6e6f 726d 616c 2066 6f72 2069 6e69 7469  normal for initi
+00012570: 616c 697a 6174 696f 6e0a 2020 2020 2020  alization.      
+00012580: 2020 2020 2020 2320 6366 2068 7474 7073        # cf https
+00012590: 3a2f 2f67 6974 6875 622e 636f 6d2f 7079  ://github.com/py
+000125a0: 746f 7263 682f 7079 746f 7263 682f 7075  torch/pytorch/pu
+000125b0: 6c6c 2f35 3631 370a 2020 2020 2020 2020  ll/5617.        
+000125c0: 2020 2020 6d6f 6475 6c65 2e77 6569 6768      module.weigh
+000125d0: 742e 6461 7461 2e6e 6f72 6d61 6c5f 286d  t.data.normal_(m
+000125e0: 6561 6e3d 302e 302c 2073 7464 3d73 656c  ean=0.0, std=sel
+000125f0: 662e 636f 6e66 6967 2e69 6e69 7469 616c  f.config.initial
+00012600: 697a 6572 5f72 616e 6765 290a 2020 2020  izer_range).    
+00012610: 2020 2020 2020 2020 6966 206d 6f64 756c          if modul
+00012620: 652e 6269 6173 2069 7320 6e6f 7420 4e6f  e.bias is not No
+00012630: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00012640: 2020 2020 6d6f 6475 6c65 2e62 6961 732e      module.bias.
+00012650: 6461 7461 2e7a 6572 6f5f 2829 0a20 2020  data.zero_().   
+00012660: 2020 2020 2065 6c69 6620 6973 696e 7374       elif isinst
+00012670: 616e 6365 286d 6f64 756c 652c 206e 6e2e  ance(module, nn.
+00012680: 4c61 7965 724e 6f72 6d29 3a0a 2020 2020  LayerNorm):.    
+00012690: 2020 2020 2020 2020 6d6f 6475 6c65 2e62          module.b
+000126a0: 6961 732e 6461 7461 2e7a 6572 6f5f 2829  ias.data.zero_()
+000126b0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+000126c0: 756c 652e 7765 6967 6874 2e64 6174 612e  ule.weight.data.
+000126d0: 6669 6c6c 5f28 312e 3029 0a0a 0a40 6461  fill_(1.0)...@da
+000126e0: 7461 636c 6173 730a 636c 6173 7320 5265  taclass.class Re
+000126f0: 666f 726d 6572 4d6f 6465 6c4f 7574 7075  formerModelOutpu
+00012700: 7428 4d6f 6465 6c4f 7574 7075 7429 3a0a  t(ModelOutput):.
+00012710: 2020 2020 2222 220a 2020 2020 4f75 7470      """.    Outp
+00012720: 7574 2074 7970 6520 6f66 203a 636c 6173  ut type of :clas
+00012730: 733a 607e 7472 616e 7366 6f72 6d65 7273  s:`~transformers
+00012740: 2e52 6566 6f72 6d65 724d 6f64 656c 602e  .ReformerModel`.
+00012750: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00012760: 2020 2020 6c61 7374 5f68 6964 6465 6e5f      last_hidden_
+00012770: 7374 6174 6520 283a 6f62 6a3a 6074 6f72  state (:obj:`tor
+00012780: 6368 2e46 6c6f 6174 5465 6e73 6f72 6020  ch.FloatTensor` 
+00012790: 6f66 2073 6861 7065 203a 6f62 6a3a 6028  of shape :obj:`(
+000127a0: 6261 7463 685f 7369 7a65 2c20 6e75 6d5f  batch_size, num_
+000127b0: 7072 6564 6963 742c 2068 6964 6465 6e5f  predict, hidden_
+000127c0: 7369 7a65 2960 293a 0a20 2020 2020 2020  size)`):.       
+000127d0: 2020 2020 2053 6571 7565 6e63 6520 6f66       Sequence of
+000127e0: 2068 6964 6465 6e2d 7374 6174 6573 2061   hidden-states a
+000127f0: 7420 7468 6520 6c61 7374 206c 6179 6572  t the last layer
+00012800: 206f 6620 7468 6520 6d6f 6465 6c2e 0a0a   of the model...
+00012810: 2020 2020 2020 2020 2020 2020 6060 6e75              ``nu
+00012820: 6d5f 7072 6564 6963 7460 6020 636f 7272  m_predict`` corr
+00012830: 6573 706f 6e64 7320 746f 2060 6074 6172  esponds to ``tar
+00012840: 6765 745f 6d61 7070 696e 672e 7368 6170  get_mapping.shap
+00012850: 655b 315d 6060 2e20 4966 2060 6074 6172  e[1]``. If ``tar
+00012860: 6765 745f 6d61 7070 696e 6760 6020 6973  get_mapping`` is
+00012870: 2060 604e 6f6e 6560 602c 2074 6865 6e0a   ``None``, then.
+00012880: 2020 2020 2020 2020 2020 2020 6060 6e75              ``nu
+00012890: 6d5f 7072 6564 6963 7460 6020 636f 7272  m_predict`` corr
+000128a0: 6573 706f 6e64 7320 746f 2060 6073 6571  esponds to ``seq
+000128b0: 7565 6e63 655f 6c65 6e67 7468 6060 2e0a  uence_length``..
+000128c0: 2020 2020 2020 2020 7061 7374 5f62 7563          past_buc
+000128d0: 6b65 7473 5f73 7461 7465 7320 283a 6f62  kets_states (:ob
+000128e0: 6a3a 604c 6973 745b 5475 706c 6528 746f  j:`List[Tuple(to
+000128f0: 7263 682e 4c6f 6e67 5465 6e73 6f72 2c20  rch.LongTensor, 
+00012900: 746f 7263 682e 466c 6f61 7454 656e 736f  torch.FloatTenso
+00012910: 7229 5d60 2c20 606f 7074 696f 6e61 6c60  r)]`, `optional`
+00012920: 2c20 7265 7475 726e 6564 2077 6865 6e20  , returned when 
+00012930: 6060 7573 655f 6361 6368 653d 5472 7565  ``use_cache=True
+00012940: 6060 2069 7320 7061 7373 6564 206f 7220  `` is passed or 
+00012950: 7768 656e 2060 6063 6f6e 6669 672e 7573  when ``config.us
+00012960: 655f 6361 6368 653d 5472 7565 6060 293a  e_cache=True``):
+00012970: 0a20 2020 2020 2020 2020 2020 204c 6973  .            Lis
+00012980: 7420 6f66 203a 6f62 6a3a 6054 7570 6c65  t of :obj:`Tuple
+00012990: 2874 6f72 6368 2e4c 6f6e 6754 656e 736f  (torch.LongTenso
+000129a0: 722c 2074 6f72 6368 2e46 6c6f 6174 5465  r, torch.FloatTe
+000129b0: 6e73 6f72 6020 6f66 206c 656e 6774 6820  nsor` of length 
+000129c0: 3a6f 626a 3a60 636f 6e66 6967 2e6e 5f6c  :obj:`config.n_l
+000129d0: 6179 6572 7360 2c20 7769 7468 2074 6865  ayers`, with the
+000129e0: 2066 6972 7374 0a20 2020 2020 2020 2020   first.         
+000129f0: 2020 2065 6c65 6d65 6e74 2062 6569 6e67     element being
+00012a00: 2074 6865 2070 7265 7669 6f75 7320 6062   the previous `b
+00012a10: 7563 6b65 7473 6020 6f66 2073 6861 7065  uckets` of shape
+00012a20: 203a 6f62 6a3a 6028 6261 7463 685f 7369   :obj:`(batch_si
+00012a30: 7a65 2c20 6e75 6d5f 6865 6164 732c 206e  ze, num_heads, n
+00012a40: 756d 5f68 6173 6865 732c 2073 6571 7565  um_hashes, seque
+00012a50: 6e63 655f 6c65 6e67 7468 2960 290a 2020  nce_length)`).  
+00012a60: 2020 2020 2020 2020 2020 616e 6420 7468            and th
+00012a70: 6520 7365 636f 6e64 2062 6569 6e67 2074  e second being t
+00012a80: 6865 2070 7265 7669 6f75 7320 6068 6964  he previous `hid
+00012a90: 6465 6e5f 7374 6174 6573 6020 6f66 2073  den_states` of s
+00012aa0: 6861 7065 203a 6f62 6a3a 6028 6261 7463  hape :obj:`(batc
+00012ab0: 685f 7369 7a65 2c20 7365 7175 656e 6365  h_size, sequence
+00012ac0: 5f6c 656e 6774 682c 0a20 2020 2020 2020  _length,.       
+00012ad0: 2020 2020 2068 6964 6465 6e5f 7369 7a65       hidden_size
+00012ae0: 2960 292e 0a0a 2020 2020 2020 2020 2020  )`)...          
+00012af0: 2020 436f 6e74 6169 6e73 2070 7265 636f    Contains preco
+00012b00: 6d70 7574 6564 2062 7563 6b65 7473 2061  mputed buckets a
+00012b10: 6e64 2068 6964 6465 6e2d 7374 6174 6573  nd hidden-states
+00012b20: 2074 6861 7420 6361 6e20 6265 2075 7365   that can be use
+00012b30: 6420 2873 6565 2060 6070 6173 745f 6275  d (see ``past_bu
+00012b40: 636b 6574 735f 7374 6174 6573 6060 2069  ckets_states`` i
+00012b50: 6e70 7574 2920 746f 0a20 2020 2020 2020  nput) to.       
+00012b60: 2020 2020 2073 7065 6564 2075 7020 7365       speed up se
+00012b70: 7175 656e 7469 616c 2064 6563 6f64 696e  quential decodin
+00012b80: 672e 0a20 2020 2020 2020 2068 6964 6465  g..        hidde
+00012b90: 6e5f 7374 6174 6573 2028 3a6f 626a 3a60  n_states (:obj:`
+00012ba0: 7475 706c 6528 746f 7263 682e 466c 6f61  tuple(torch.Floa
+00012bb0: 7454 656e 736f 7229 602c 2060 6f70 7469  tTensor)`, `opti
+00012bc0: 6f6e 616c 602c 2072 6574 7572 6e65 6420  onal`, returned 
+00012bd0: 7768 656e 2060 606f 7574 7075 745f 6869  when ``output_hi
+00012be0: 6464 656e 5f73 7461 7465 733d 5472 7565  dden_states=True
+00012bf0: 6060 2069 7320 7061 7373 6564 206f 7220  `` is passed or 
+00012c00: 7768 656e 2060 6063 6f6e 6669 672e 6f75  when ``config.ou
+00012c10: 7470 7574 5f68 6964 6465 6e5f 7374 6174  tput_hidden_stat
+00012c20: 6573 3d54 7275 6560 6029 3a0a 2020 2020  es=True``):.    
+00012c30: 2020 2020 2020 2020 5475 706c 6520 6f66          Tuple of
+00012c40: 203a 6f62 6a3a 6074 6f72 6368 2e46 6c6f   :obj:`torch.Flo
+00012c50: 6174 5465 6e73 6f72 6020 286f 6e65 2066  atTensor` (one f
+00012c60: 6f72 2074 6865 206f 7574 7075 7420 6f66  or the output of
+00012c70: 2074 6865 2065 6d62 6564 6469 6e67 7320   the embeddings 
+00012c80: 616e 6420 6f6e 6520 666f 7220 7468 6520  and one for the 
+00012c90: 6f75 7470 7574 206f 6620 6561 6368 0a20  output of each. 
+00012ca0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+00012cb0: 2920 6f66 2073 6861 7065 203a 6f62 6a3a  ) of shape :obj:
+00012cc0: 6028 6261 7463 685f 7369 7a65 2c20 7365  `(batch_size, se
+00012cd0: 7175 656e 6365 5f6c 656e 6774 682c 2068  quence_length, h
+00012ce0: 6964 6465 6e5f 7369 7a65 2960 2e0a 0a20  idden_size)`... 
+00012cf0: 2020 2020 2020 2020 2020 2048 6964 6465             Hidde
+00012d00: 6e2d 7374 6174 6573 206f 6620 7468 6520  n-states of the 
+00012d10: 6d6f 6465 6c20 6174 2074 6865 206f 7574  model at the out
+00012d20: 7075 7420 6f66 2065 6163 6820 6c61 7965  put of each laye
+00012d30: 7220 706c 7573 2074 6865 2069 6e69 7469  r plus the initi
+00012d40: 616c 2065 6d62 6564 6469 6e67 206f 7574  al embedding out
+00012d50: 7075 7473 2e0a 2020 2020 2020 2020 6174  puts..        at
+00012d60: 7465 6e74 696f 6e73 2028 3a6f 626a 3a60  tentions (:obj:`
+00012d70: 7475 706c 6528 746f 7263 682e 466c 6f61  tuple(torch.Floa
+00012d80: 7454 656e 736f 7229 602c 2060 6f70 7469  tTensor)`, `opti
+00012d90: 6f6e 616c 602c 2072 6574 7572 6e65 6420  onal`, returned 
+00012da0: 7768 656e 2060 606f 7574 7075 745f 6174  when ``output_at
+00012db0: 7465 6e74 696f 6e73 3d54 7275 6560 6020  tentions=True`` 
+00012dc0: 6973 2070 6173 7365 6420 6f72 2077 6865  is passed or whe
+00012dd0: 6e20 6060 636f 6e66 6967 2e6f 7574 7075  n ``config.outpu
+00012de0: 745f 6174 7465 6e74 696f 6e73 3d54 7275  t_attentions=Tru
+00012df0: 6560 6029 3a0a 2020 2020 2020 2020 2020  e``):.          
+00012e00: 2020 5475 706c 6520 6f66 203a 6f62 6a3a    Tuple of :obj:
+00012e10: 6074 6f72 6368 2e46 6c6f 6174 5465 6e73  `torch.FloatTens
+00012e20: 6f72 6020 286f 6e65 2066 6f72 2065 6163  or` (one for eac
+00012e30: 6820 6c61 7965 7229 206f 6620 7368 6170  h layer) of shap
+00012e40: 6520 3a6f 626a 3a60 2862 6174 6368 5f73  e :obj:`(batch_s
+00012e50: 697a 652c 206e 756d 5f68 6561 6473 2c0a  ize, num_heads,.
+00012e60: 2020 2020 2020 2020 2020 2020 7365 7175              sequ
+00012e70: 656e 6365 5f6c 656e 6774 682c 2073 6571  ence_length, seq
+00012e80: 7565 6e63 655f 6c65 6e67 7468 2960 2e0a  uence_length)`..
+00012e90: 0a20 2020 2020 2020 2020 2020 2041 7474  .            Att
+00012ea0: 656e 7469 6f6e 7320 7765 6967 6874 7320  entions weights 
+00012eb0: 6166 7465 7220 7468 6520 6174 7465 6e74  after the attent
+00012ec0: 696f 6e20 736f 6674 6d61 782c 2075 7365  ion softmax, use
+00012ed0: 6420 746f 2063 6f6d 7075 7465 2074 6865  d to compute the
+00012ee0: 2077 6569 6768 7465 6420 6176 6572 6167   weighted averag
+00012ef0: 6520 696e 2074 6865 2073 656c 662d 6174  e in the self-at
+00012f00: 7465 6e74 696f 6e0a 2020 2020 2020 2020  tention.        
+00012f10: 2020 2020 6865 6164 732e 0a20 2020 2022      heads..    "
+00012f20: 2222 0a0a 2020 2020 6c61 7374 5f68 6964  ""..    last_hid
+00012f30: 6465 6e5f 7374 6174 653a 2074 6f72 6368  den_state: torch
+00012f40: 2e46 6c6f 6174 5465 6e73 6f72 0a20 2020  .FloatTensor.   
+00012f50: 2070 6173 745f 6275 636b 6574 735f 7374   past_buckets_st
+00012f60: 6174 6573 3a20 4f70 7469 6f6e 616c 5b4c  ates: Optional[L
+00012f70: 6973 745b 5475 706c 655b 746f 7263 682e  ist[Tuple[torch.
+00012f80: 4c6f 6e67 5465 6e73 6f72 2c20 746f 7263  LongTensor, torc
+00012f90: 682e 466c 6f61 7454 656e 736f 725d 5d5d  h.FloatTensor]]]
+00012fa0: 203d 204e 6f6e 650a 2020 2020 6869 6464   = None.    hidd
+00012fb0: 656e 5f73 7461 7465 733a 204f 7074 696f  en_states: Optio
+00012fc0: 6e61 6c5b 5475 706c 655b 746f 7263 682e  nal[Tuple[torch.
+00012fd0: 466c 6f61 7454 656e 736f 725d 5d20 3d20  FloatTensor]] = 
+00012fe0: 4e6f 6e65 0a20 2020 2061 7474 656e 7469  None.    attenti
+00012ff0: 6f6e 733a 204f 7074 696f 6e61 6c5b 5475  ons: Optional[Tu
+00013000: 706c 655b 746f 7263 682e 466c 6f61 7454  ple[torch.FloatT
+00013010: 656e 736f 725d 5d20 3d20 4e6f 6e65 0a0a  ensor]] = None..
+00013020: 0a40 6461 7461 636c 6173 730a 636c 6173  .@dataclass.clas
+00013030: 7320 5265 666f 726d 6572 4d6f 6465 6c57  s ReformerModelW
+00013040: 6974 684c 4d48 6561 644f 7574 7075 7428  ithLMHeadOutput(
+00013050: 4d6f 6465 6c4f 7574 7075 7429 3a0a 2020  ModelOutput):.  
+00013060: 2020 2222 220a 2020 2020 4f75 7470 7574    """.    Output
+00013070: 2074 7970 6520 6f66 203a 636c 6173 733a   type of :class:
+00013080: 607e 7472 616e 7366 6f72 6d65 7273 2e52  `~transformers.R
+00013090: 6566 6f72 6d65 724d 6f64 656c 5769 7468  eformerModelWith
+000130a0: 4c4d 4865 6164 602e 0a0a 2020 2020 4172  LMHead`...    Ar
+000130b0: 6773 3a0a 2020 2020 2020 2020 6c6f 7373  gs:.        loss
+000130c0: 2028 3a6f 626a 3a60 746f 7263 682e 466c   (:obj:`torch.Fl
+000130d0: 6f61 7454 656e 736f 7260 206f 6620 7368  oatTensor` of sh
+000130e0: 6170 6520 6028 312c 2960 2c20 606f 7074  ape `(1,)`, `opt
+000130f0: 696f 6e61 6c60 2c20 7265 7475 726e 6564  ional`, returned
+00013100: 2077 6865 6e20 6060 6c61 6265 6c73 6060   when ``labels``
+00013110: 2069 7320 7072 6f76 6964 6564 290a 2020   is provided).  
+00013120: 2020 2020 2020 2020 2020 4c61 6e67 7561            Langua
+00013130: 6765 206d 6f64 656c 696e 6720 6c6f 7373  ge modeling loss
+00013140: 2028 666f 7220 6e65 7874 2d74 6f6b 656e   (for next-token
+00013150: 2070 7265 6469 6374 696f 6e29 2e0a 2020   prediction)..  
+00013160: 2020 2020 2020 6c6f 6769 7473 2028 3a6f        logits (:o
+00013170: 626a 3a60 746f 7263 682e 466c 6f61 7454  bj:`torch.FloatT
+00013180: 656e 736f 7260 206f 6620 7368 6170 6520  ensor` of shape 
+00013190: 3a6f 626a 3a60 2862 6174 6368 5f73 697a  :obj:`(batch_siz
+000131a0: 652c 206e 756d 5f70 7265 6469 6374 2c20  e, num_predict, 
+000131b0: 636f 6e66 6967 2e76 6f63 6162 5f73 697a  config.vocab_siz
+000131c0: 6529 6029 3a0a 2020 2020 2020 2020 2020  e)`):.          
+000131d0: 2020 5072 6564 6963 7469 6f6e 2073 636f    Prediction sco
+000131e0: 7265 7320 6f66 2074 6865 206c 616e 6775  res of the langu
+000131f0: 6167 6520 6d6f 6465 6c69 6e67 2068 6561  age modeling hea
+00013200: 6420 2873 636f 7265 7320 666f 7220 6561  d (scores for ea
+00013210: 6368 2076 6f63 6162 756c 6172 7920 746f  ch vocabulary to
+00013220: 6b65 6e20 6265 666f 7265 2053 6f66 744d  ken before SoftM
+00013230: 6178 292e 0a0a 2020 2020 2020 2020 2020  ax)...          
+00013240: 2020 6060 6e75 6d5f 7072 6564 6963 7460    ``num_predict`
+00013250: 6020 636f 7272 6573 706f 6e64 7320 746f  ` corresponds to
+00013260: 2060 6074 6172 6765 745f 6d61 7070 696e   ``target_mappin
+00013270: 672e 7368 6170 655b 315d 6060 2e20 4966  g.shape[1]``. If
+00013280: 2060 6074 6172 6765 745f 6d61 7070 696e   ``target_mappin
+00013290: 6760 6020 6973 2060 604e 6f6e 6560 602c  g`` is ``None``,
+000132a0: 2074 6865 6e0a 2020 2020 2020 2020 2020   then.          
+000132b0: 2020 6060 6e75 6d5f 7072 6564 6963 7460    ``num_predict`
+000132c0: 6020 636f 7272 6573 706f 6e64 7320 746f  ` corresponds to
+000132d0: 2060 6073 6571 7565 6e63 655f 6c65 6e67   ``sequence_leng
+000132e0: 7468 6060 2e0a 2020 2020 2020 2020 7061  th``..        pa
+000132f0: 7374 5f62 7563 6b65 7473 5f73 7461 7465  st_buckets_state
+00013300: 7320 283a 6f62 6a3a 604c 6973 745b 5475  s (:obj:`List[Tu
+00013310: 706c 6528 746f 7263 682e 4c6f 6e67 5465  ple(torch.LongTe
+00013320: 6e73 6f72 2c20 746f 7263 682e 466c 6f61  nsor, torch.Floa
+00013330: 7454 656e 736f 7229 5d60 2c20 606f 7074  tTensor)]`, `opt
+00013340: 696f 6e61 6c60 2c20 7265 7475 726e 6564  ional`, returned
+00013350: 2077 6865 6e20 6060 7573 655f 6361 6368   when ``use_cach
+00013360: 653d 5472 7565 6060 2069 7320 7061 7373  e=True`` is pass
+00013370: 6564 206f 7220 7768 656e 2060 6063 6f6e  ed or when ``con
+00013380: 6669 672e 7573 655f 6361 6368 653d 5472  fig.use_cache=Tr
+00013390: 7565 6060 293a 0a20 2020 2020 2020 2020  ue``):.         
+000133a0: 2020 204c 6973 7420 6f66 203a 6f62 6a3a     List of :obj:
+000133b0: 6054 7570 6c65 2874 6f72 6368 2e4c 6f6e  `Tuple(torch.Lon
+000133c0: 6754 656e 736f 722c 2074 6f72 6368 2e46  gTensor, torch.F
+000133d0: 6c6f 6174 5465 6e73 6f72 6020 6f66 206c  loatTensor` of l
+000133e0: 656e 6774 6820 3a6f 626a 3a60 636f 6e66  ength :obj:`conf
+000133f0: 6967 2e6e 5f6c 6179 6572 7360 2c20 7769  ig.n_layers`, wi
+00013400: 7468 2074 6865 2066 6972 7374 0a20 2020  th the first.   
+00013410: 2020 2020 2020 2020 2065 6c65 6d65 6e74           element
+00013420: 2062 6569 6e67 2074 6865 2070 7265 7669   being the previ
+00013430: 6f75 7320 6062 7563 6b65 7473 6020 6f66  ous `buckets` of
+00013440: 2073 6861 7065 203a 6f62 6a3a 6028 6261   shape :obj:`(ba
+00013450: 7463 685f 7369 7a65 2c20 6e75 6d5f 6865  tch_size, num_he
+00013460: 6164 732c 206e 756d 5f68 6173 6865 732c  ads, num_hashes,
+00013470: 2073 6571 7565 6e63 655f 6c65 6e67 7468   sequence_length
+00013480: 2960 290a 2020 2020 2020 2020 2020 2020  )`).            
+00013490: 616e 6420 7468 6520 7365 636f 6e64 2062  and the second b
+000134a0: 6569 6e67 2074 6865 2070 7265 7669 6f75  eing the previou
+000134b0: 7320 6068 6964 6465 6e5f 7374 6174 6573  s `hidden_states
+000134c0: 6020 6f66 2073 6861 7065 203a 6f62 6a3a  ` of shape :obj:
+000134d0: 6028 6261 7463 685f 7369 7a65 2c20 7365  `(batch_size, se
+000134e0: 7175 656e 6365 5f6c 656e 6774 682c 0a20  quence_length,. 
+000134f0: 2020 2020 2020 2020 2020 2068 6964 6465             hidde
+00013500: 6e5f 7369 7a65 2960 292e 0a0a 2020 2020  n_size)`)...    
+00013510: 2020 2020 2020 2020 436f 6e74 6169 6e73          Contains
+00013520: 2070 7265 636f 6d70 7574 6564 2062 7563   precomputed buc
+00013530: 6b65 7473 2061 6e64 2068 6964 6465 6e2d  kets and hidden-
+00013540: 7374 6174 6573 2074 6861 7420 6361 6e20  states that can 
+00013550: 6265 2075 7365 6420 2873 6565 2060 6070  be used (see ``p
+00013560: 6173 745f 6275 636b 6574 735f 7374 6174  ast_buckets_stat
+00013570: 6573 6060 2069 6e70 7574 2920 746f 0a20  es`` input) to. 
+00013580: 2020 2020 2020 2020 2020 2073 7065 6564             speed
+00013590: 2075 7020 7365 7175 656e 7469 616c 2064   up sequential d
+000135a0: 6563 6f64 696e 672e 0a20 2020 2020 2020  ecoding..       
+000135b0: 2068 6964 6465 6e5f 7374 6174 6573 2028   hidden_states (
+000135c0: 3a6f 626a 3a60 7475 706c 6528 746f 7263  :obj:`tuple(torc
+000135d0: 682e 466c 6f61 7454 656e 736f 7229 602c  h.FloatTensor)`,
+000135e0: 2060 6f70 7469 6f6e 616c 602c 2072 6574   `optional`, ret
+000135f0: 7572 6e65 6420 7768 656e 2060 606f 7574  urned when ``out
+00013600: 7075 745f 6869 6464 656e 5f73 7461 7465  put_hidden_state
+00013610: 733d 5472 7565 6060 2069 7320 7061 7373  s=True`` is pass
+00013620: 6564 206f 7220 7768 656e 2060 6063 6f6e  ed or when ``con
+00013630: 6669 672e 6f75 7470 7574 5f68 6964 6465  fig.output_hidde
+00013640: 6e5f 7374 6174 6573 3d54 7275 6560 6029  n_states=True``)
+00013650: 3a0a 2020 2020 2020 2020 2020 2020 5454  :.            TT
+00013660: 7570 6c65 206f 6620 3a6f 626a 3a60 746f  uple of :obj:`to
+00013670: 7263 682e 466c 6f61 7454 656e 736f 7260  rch.FloatTensor`
+00013680: 2028 6f6e 6520 666f 7220 7468 6520 6f75   (one for the ou
+00013690: 7470 7574 206f 6620 7468 6520 656d 6265  tput of the embe
+000136a0: 6464 696e 6773 2061 6e64 206f 6e65 2066  ddings and one f
+000136b0: 6f72 2074 6865 206f 7574 7075 7420 6f66  or the output of
+000136c0: 2065 6163 680a 2020 2020 2020 2020 2020   each.          
+000136d0: 2020 6c61 7965 7229 206f 6620 7368 6170    layer) of shap
+000136e0: 6520 3a6f 626a 3a60 2862 6174 6368 5f73  e :obj:`(batch_s
+000136f0: 697a 652c 2073 6571 7565 6e63 655f 6c65  ize, sequence_le
+00013700: 6e67 7468 2c20 6869 6464 656e 5f73 697a  ngth, hidden_siz
+00013710: 6529 602e 0a0a 2020 2020 2020 2020 2020  e)`...          
+00013720: 2020 4869 6464 656e 2d73 7461 7465 7320    Hidden-states 
+00013730: 6f66 2074 6865 206d 6f64 656c 2061 7420  of the model at 
+00013740: 7468 6520 6f75 7470 7574 206f 6620 6561  the output of ea
+00013750: 6368 206c 6179 6572 2070 6c75 7320 7468  ch layer plus th
+00013760: 6520 696e 6974 6961 6c20 656d 6265 6464  e initial embedd
+00013770: 696e 6720 6f75 7470 7574 732e 0a20 2020  ing outputs..   
+00013780: 2020 2020 2061 7474 656e 7469 6f6e 7320       attentions 
+00013790: 283a 6f62 6a3a 6074 7570 6c65 2874 6f72  (:obj:`tuple(tor
+000137a0: 6368 2e46 6c6f 6174 5465 6e73 6f72 2960  ch.FloatTensor)`
+000137b0: 2c20 606f 7074 696f 6e61 6c60 2c20 7265  , `optional`, re
+000137c0: 7475 726e 6564 2077 6865 6e20 6060 6f75  turned when ``ou
+000137d0: 7470 7574 5f61 7474 656e 7469 6f6e 733d  tput_attentions=
+000137e0: 5472 7565 6060 2069 7320 7061 7373 6564  True`` is passed
+000137f0: 206f 7220 7768 656e 2060 6063 6f6e 6669   or when ``confi
+00013800: 672e 6f75 7470 7574 5f61 7474 656e 7469  g.output_attenti
+00013810: 6f6e 733d 5472 7565 6060 293a 0a20 2020  ons=True``):.   
+00013820: 2020 2020 2020 2020 2054 7570 6c65 206f           Tuple o
+00013830: 6620 3a6f 626a 3a60 746f 7263 682e 466c  f :obj:`torch.Fl
+00013840: 6f61 7454 656e 736f 7260 2028 6f6e 6520  oatTensor` (one 
+00013850: 666f 7220 6561 6368 206c 6179 6572 2920  for each layer) 
+00013860: 6f66 2073 6861 7065 203a 6f62 6a3a 6028  of shape :obj:`(
+00013870: 6261 7463 685f 7369 7a65 2c20 6e75 6d5f  batch_size, num_
+00013880: 6865 6164 732c 0a20 2020 2020 2020 2020  heads,.         
+00013890: 2020 2073 6571 7565 6e63 655f 6c65 6e67     sequence_leng
+000138a0: 7468 2c20 7365 7175 656e 6365 5f6c 656e  th, sequence_len
+000138b0: 6774 6829 602e 0a0a 2020 2020 2020 2020  gth)`...        
+000138c0: 2020 2020 4174 7465 6e74 696f 6e73 2077      Attentions w
+000138d0: 6569 6768 7473 2061 6674 6572 2074 6865  eights after the
+000138e0: 2061 7474 656e 7469 6f6e 2073 6f66 746d   attention softm
+000138f0: 6178 2c20 7573 6564 2074 6f20 636f 6d70  ax, used to comp
+00013900: 7574 6520 7468 6520 7765 6967 6874 6564  ute the weighted
+00013910: 2061 7665 7261 6765 2069 6e20 7468 6520   average in the 
+00013920: 7365 6c66 2d61 7474 656e 7469 6f6e 0a20  self-attention. 
+00013930: 2020 2020 2020 2020 2020 2068 6561 6473             heads
+00013940: 2e0a 2020 2020 2222 220a 0a20 2020 206c  ..    """..    l
+00013950: 6f73 733a 204f 7074 696f 6e61 6c5b 746f  oss: Optional[to
+00013960: 7263 682e 466c 6f61 7454 656e 736f 725d  rch.FloatTensor]
+00013970: 203d 204e 6f6e 650a 2020 2020 6c6f 6769   = None.    logi
+00013980: 7473 3a20 746f 7263 682e 466c 6f61 7454  ts: torch.FloatT
+00013990: 656e 736f 7220 3d20 4e6f 6e65 0a20 2020  ensor = None.   
+000139a0: 2070 6173 745f 6275 636b 6574 735f 7374   past_buckets_st
+000139b0: 6174 6573 3a20 4f70 7469 6f6e 616c 5b4c  ates: Optional[L
+000139c0: 6973 745b 5475 706c 655b 746f 7263 682e  ist[Tuple[torch.
+000139d0: 4c6f 6e67 5465 6e73 6f72 2c20 746f 7263  LongTensor, torc
+000139e0: 682e 466c 6f61 7454 656e 736f 725d 5d5d  h.FloatTensor]]]
+000139f0: 203d 204e 6f6e 650a 2020 2020 6869 6464   = None.    hidd
+00013a00: 656e 5f73 7461 7465 733a 204f 7074 696f  en_states: Optio
+00013a10: 6e61 6c5b 5475 706c 655b 746f 7263 682e  nal[Tuple[torch.
+00013a20: 466c 6f61 7454 656e 736f 725d 5d20 3d20  FloatTensor]] = 
+00013a30: 4e6f 6e65 0a20 2020 2061 7474 656e 7469  None.    attenti
+00013a40: 6f6e 733a 204f 7074 696f 6e61 6c5b 5475  ons: Optional[Tu
+00013a50: 706c 655b 746f 7263 682e 466c 6f61 7454  ple[torch.FloatT
+00013a60: 656e 736f 725d 5d20 3d20 4e6f 6e65 0a0a  ensor]] = None..
+00013a70: 0a52 4546 4f52 4d45 525f 5354 4152 545f  .REFORMER_START_
+00013a80: 444f 4353 5452 494e 4720 3d20 7222 2222  DOCSTRING = r"""
+00013a90: 0a20 2020 2052 6566 6f72 6d65 7220 7761  .    Reformer wa
+00013aa0: 7320 7072 6f70 6f73 6564 2069 6e20 6052  s proposed in `R
+00013ab0: 6566 6f72 6d65 723a 2054 6865 2045 6666  eformer: The Eff
+00013ac0: 6963 6965 6e74 2054 7261 6e73 666f 726d  icient Transform
+00013ad0: 6572 203c 6874 7470 733a 2f2f 6172 7869  er <https://arxi
+00013ae0: 762e 6f72 672f 6162 732f 3230 3031 2e30  v.org/abs/2001.0
+00013af0: 3434 3531 3e60 5f5f 2062 7920 4e69 6b69  4451>`__ by Niki
+00013b00: 7461 0a20 2020 204b 6974 6165 762c 20c5  ta.    Kitaev, .
+00013b10: 8175 6b61 737a 204b 6169 7365 722c 2041  .ukasz Kaiser, A
+00013b20: 6e73 656c 6d20 4c65 7673 6b61 7961 2e0a  nselm Levskaya..
+00013b30: 0a20 2020 2054 6869 7320 6d6f 6465 6c20  .    This model 
+00013b40: 696e 6865 7269 7473 2066 726f 6d20 3a63  inherits from :c
+00013b50: 6c61 7373 3a60 7e74 7261 6e73 666f 726d  lass:`~transform
+00013b60: 6572 732e 5072 6554 7261 696e 6564 4d6f  ers.PreTrainedMo
+00013b70: 6465 6c60 2e20 4368 6563 6b20 7468 6520  del`. Check the 
+00013b80: 7375 7065 7263 6c61 7373 2064 6f63 756d  superclass docum
+00013b90: 656e 7461 7469 6f6e 2066 6f72 2074 6865  entation for the
+00013ba0: 2067 656e 6572 6963 0a20 2020 206d 6574   generic.    met
+00013bb0: 686f 6473 2074 6865 206c 6962 7261 7279  hods the library
+00013bc0: 2069 6d70 6c65 6d65 6e74 7320 666f 7220   implements for 
+00013bd0: 616c 6c20 6974 7320 6d6f 6465 6c20 2873  all its model (s
+00013be0: 7563 6820 6173 2064 6f77 6e6c 6f61 6469  uch as downloadi
+00013bf0: 6e67 206f 7220 7361 7669 6e67 2c20 7265  ng or saving, re
+00013c00: 7369 7a69 6e67 2074 6865 2069 6e70 7574  sizing the input
+00013c10: 2065 6d62 6564 6469 6e67 732c 0a20 2020   embeddings,.   
+00013c20: 2070 7275 6e69 6e67 2068 6561 6473 2065   pruning heads e
+00013c30: 7463 2e29 0a0a 2020 2020 5468 6973 206d  tc.)..    This m
+00013c40: 6f64 656c 2069 7320 616c 736f 2061 2050  odel is also a P
+00013c50: 7954 6f72 6368 2060 746f 7263 682e 6e6e  yTorch `torch.nn
+00013c60: 2e4d 6f64 756c 6520 3c68 7474 7073 3a2f  .Module <https:/
+00013c70: 2f70 7974 6f72 6368 2e6f 7267 2f64 6f63  /pytorch.org/doc
+00013c80: 732f 7374 6162 6c65 2f6e 6e2e 6874 6d6c  s/stable/nn.html
+00013c90: 2374 6f72 6368 2e6e 6e2e 4d6f 6475 6c65  #torch.nn.Module
+00013ca0: 3e60 5f5f 0a20 2020 2073 7562 636c 6173  >`__.    subclas
+00013cb0: 732e 2055 7365 2069 7420 6173 2061 2072  s. Use it as a r
+00013cc0: 6567 756c 6172 2050 7954 6f72 6368 204d  egular PyTorch M
+00013cd0: 6f64 756c 6520 616e 6420 7265 6665 7220  odule and refer 
+00013ce0: 746f 2074 6865 2050 7954 6f72 6368 2064  to the PyTorch d
+00013cf0: 6f63 756d 656e 7461 7469 6f6e 2066 6f72  ocumentation for
+00013d00: 2061 6c6c 206d 6174 7465 7220 7265 6c61   all matter rela
+00013d10: 7465 6420 746f 0a20 2020 2067 656e 6572  ted to.    gener
+00013d20: 616c 2075 7361 6765 2061 6e64 2062 6568  al usage and beh
+00013d30: 6176 696f 722e 0a0a 2020 2020 5061 7261  avior...    Para
+00013d40: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
+00013d50: 636f 6e66 6967 2028 3a63 6c61 7373 3a60  config (:class:`
+00013d60: 7e74 7261 6e73 666f 726d 6572 732e 5265  ~transformers.Re
+00013d70: 666f 726d 6572 436f 6e66 6967 6029 3a20  formerConfig`): 
+00013d80: 4d6f 6465 6c20 636f 6e66 6967 7572 6174  Model configurat
+00013d90: 696f 6e20 636c 6173 7320 7769 7468 2061  ion class with a
+00013da0: 6c6c 2074 6865 2070 6172 616d 6574 6572  ll the parameter
+00013db0: 7320 6f66 2074 6865 206d 6f64 656c 2e0a  s of the model..
+00013dc0: 2020 2020 2020 2020 2020 2020 496e 6974              Init
+00013dd0: 6961 6c69 7a69 6e67 2077 6974 6820 6120  ializing with a 
+00013de0: 636f 6e66 6967 2066 696c 6520 646f 6573  config file does
+00013df0: 206e 6f74 206c 6f61 6420 7468 6520 7765   not load the we
+00013e00: 6967 6874 7320 6173 736f 6369 6174 6564  ights associated
+00013e10: 2077 6974 6820 7468 6520 6d6f 6465 6c2c   with the model,
+00013e20: 206f 6e6c 7920 7468 650a 2020 2020 2020   only the.      
+00013e30: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
+00013e40: 696f 6e2e 2043 6865 636b 206f 7574 2074  ion. Check out t
+00013e50: 6865 203a 6d65 7468 3a60 7e74 7261 6e73  he :meth:`~trans
+00013e60: 666f 726d 6572 732e 5072 6554 7261 696e  formers.PreTrain
+00013e70: 6564 4d6f 6465 6c2e 6672 6f6d 5f70 7265  edModel.from_pre
+00013e80: 7472 6169 6e65 6460 206d 6574 686f 6420  trained` method 
+00013e90: 746f 206c 6f61 6420 7468 6520 6d6f 6465  to load the mode
+00013ea0: 6c0a 2020 2020 2020 2020 2020 2020 7765  l.            we
+00013eb0: 6967 6874 732e 0a22 2222 0a0a 5245 464f  ights.."""..REFO
+00013ec0: 524d 4552 5f49 4e50 5554 535f 444f 4353  RMER_INPUTS_DOCS
+00013ed0: 5452 494e 4720 3d20 7222 2222 0a20 2020  TRING = r""".   
+00013ee0: 2041 7267 733a 0a20 2020 2020 2020 2069   Args:.        i
+00013ef0: 6e70 7574 5f69 6473 2028 3a6f 626a 3a60  nput_ids (:obj:`
+00013f00: 746f 7263 682e 4c6f 6e67 5465 6e73 6f72  torch.LongTensor
+00013f10: 6020 6f66 2073 6861 7065 203a 6f62 6a3a  ` of shape :obj:
+00013f20: 6028 6261 7463 685f 7369 7a65 2c20 7365  `(batch_size, se
+00013f30: 7175 656e 6365 5f6c 656e 6774 6829 6029  quence_length)`)
+00013f40: 3a0a 2020 2020 2020 2020 2020 2020 496e  :.            In
+00013f50: 6469 6365 7320 6f66 2069 6e70 7574 2073  dices of input s
+00013f60: 6571 7565 6e63 6520 746f 6b65 6e73 2069  equence tokens i
+00013f70: 6e20 7468 6520 766f 6361 6275 6c61 7279  n the vocabulary
+00013f80: 2e20 4475 7269 6e67 2074 7261 696e 696e  . During trainin
+00013f90: 6720 7468 6520 696e 7075 745f 6964 7320  g the input_ids 
+00013fa0: 7365 7175 656e 6365 5f6c 656e 6774 6820  sequence_length 
+00013fb0: 6861 7320 746f 2062 650a 2020 2020 2020  has to be.      
+00013fc0: 2020 2020 2020 6120 6d75 6c74 6970 6c65        a multiple
+00013fd0: 206f 6620 7468 6520 7265 6c65 7661 6e74   of the relevant
+00013fe0: 206d 6f64 656c 2773 2063 6875 6e6b 206c   model's chunk l
+00013ff0: 656e 6774 6873 2028 6c73 6827 732c 206c  engths (lsh's, l
+00014000: 6f63 616c 2773 206f 7220 626f 7468 292e  ocal's or both).
+00014010: 2044 7572 696e 6720 6576 616c 7561 7469   During evaluati
+00014020: 6f6e 2c20 7468 6520 696e 6469 6365 730a  on, the indices.
+00014030: 2020 2020 2020 2020 2020 2020 6172 6520              are 
+00014040: 6175 746f 6d61 7469 6361 6c6c 7920 7061  automatically pa
+00014050: 6464 6564 2074 6f20 6265 2061 206d 756c  dded to be a mul
+00014060: 7469 706c 6520 6f66 2074 6865 2063 6875  tiple of the chu
+00014070: 6e6b 206c 656e 6774 682e 0a0a 2020 2020  nk length...    
+00014080: 2020 2020 2020 2020 496e 6469 6365 7320          Indices 
+00014090: 6361 6e20 6265 206f 6274 6169 6e65 6420  can be obtained 
+000140a0: 7573 696e 6720 3a63 6c61 7373 3a60 7e74  using :class:`~t
+000140b0: 7261 6e73 666f 726d 6572 732e 5265 666f  ransformers.Refo
+000140c0: 726d 6572 546f 6b65 6e69 7a65 7260 2e20  rmerTokenizer`. 
+000140d0: 5365 650a 2020 2020 2020 2020 2020 2020  See.            
+000140e0: 3a6d 6574 683a 6074 7261 6e73 666f 726d  :meth:`transform
+000140f0: 6572 732e 5072 6554 7261 696e 6564 546f  ers.PreTrainedTo
+00014100: 6b65 6e69 7a65 722e 656e 636f 6465 6020  kenizer.encode` 
+00014110: 616e 6420 3a6d 6574 683a 6074 7261 6e73  and :meth:`trans
+00014120: 666f 726d 6572 732e 5072 6554 7261 696e  formers.PreTrain
+00014130: 6564 546f 6b65 6e69 7a65 722e 5f5f 6361  edTokenizer.__ca
+00014140: 6c6c 5f5f 6020 666f 720a 2020 2020 2020  ll__` for.      
+00014150: 2020 2020 2020 6465 7461 696c 732e 0a0a        details...
+00014160: 2020 2020 2020 2020 2020 2020 6057 6861              `Wha
+00014170: 7420 6172 6520 696e 7075 7420 4944 733f  t are input IDs?
+00014180: 203c 2e2e 2f67 6c6f 7373 6172 792e 6874   <../glossary.ht
+00014190: 6d6c 2369 6e70 7574 2d69 6473 3e60 5f5f  ml#input-ids>`__
+000141a0: 0a20 2020 2020 2020 2061 7474 656e 7469  .        attenti
+000141b0: 6f6e 5f6d 6173 6b20 283a 6f62 6a3a 6074  on_mask (:obj:`t
+000141c0: 6f72 6368 2e46 6c6f 6174 5465 6e73 6f72  orch.FloatTensor
+000141d0: 6020 6f66 2073 6861 7065 203a 6f62 6a3a  ` of shape :obj:
+000141e0: 6028 6261 7463 685f 7369 7a65 2c20 7365  `(batch_size, se
+000141f0: 7175 656e 6365 5f6c 656e 6774 6829 602c  quence_length)`,
+00014200: 2060 6f70 7469 6f6e 616c 6029 3a0a 2020   `optional`):.  
+00014210: 2020 2020 2020 2020 2020 4d61 736b 2074            Mask t
+00014220: 6f20 6176 6f69 6420 7065 7266 6f72 6d69  o avoid performi
+00014230: 6e67 2061 7474 656e 7469 6f6e 206f 6e20  ng attention on 
+00014240: 7061 6464 696e 6720 746f 6b65 6e20 696e  padding token in
+00014250: 6469 6365 732e 204d 6173 6b20 7661 6c75  dices. Mask valu
+00014260: 6573 2073 656c 6563 7465 6420 696e 2060  es selected in `
+00014270: 605b 302c 2031 5d60 603a 0a0a 2020 2020  `[0, 1]``:..    
+00014280: 2020 2020 2020 2020 2d20 3120 666f 7220          - 1 for 
+00014290: 746f 6b65 6e73 2074 6861 7420 6172 6520  tokens that are 
+000142a0: 2a2a 6e6f 7420 6d61 736b 6564 2a2a 2c0a  **not masked**,.
+000142b0: 2020 2020 2020 2020 2020 2020 2d20 3020              - 0 
+000142c0: 666f 7220 746f 6b65 6e73 2074 6861 7420  for tokens that 
+000142d0: 6172 6520 2a2a 6d61 736b 6564 2a2a 2e0a  are **masked**..
+000142e0: 0a20 2020 2020 2020 2020 2020 2060 5768  .            `Wh
+000142f0: 6174 2061 7265 2061 7474 656e 7469 6f6e  at are attention
+00014300: 206d 6173 6b73 3f20 3c2e 2e2f 676c 6f73   masks? <../glos
+00014310: 7361 7279 2e68 746d 6c23 6174 7465 6e74  sary.html#attent
+00014320: 696f 6e2d 6d61 736b 3e60 5f5f 0a20 2020  ion-mask>`__.   
+00014330: 2020 2020 2070 6f73 6974 696f 6e5f 6964       position_id
+00014340: 7320 283a 6f62 6a3a 6074 6f72 6368 2e4c  s (:obj:`torch.L
+00014350: 6f6e 6754 656e 736f 7260 206f 6620 7368  ongTensor` of sh
+00014360: 6170 6520 3a6f 626a 3a60 2862 6174 6368  ape :obj:`(batch
+00014370: 5f73 697a 652c 2073 6571 7565 6e63 655f  _size, sequence_
+00014380: 6c65 6e67 7468 2960 2c20 606f 7074 696f  length)`, `optio
+00014390: 6e61 6c60 293a 0a20 2020 2020 2020 2020  nal`):.         
+000143a0: 2020 2049 6e64 6963 6573 206f 6620 706f     Indices of po
+000143b0: 7369 7469 6f6e 7320 6f66 2065 6163 6820  sitions of each 
+000143c0: 696e 7075 7420 7365 7175 656e 6365 2074  input sequence t
+000143d0: 6f6b 656e 7320 696e 2074 6865 2070 6f73  okens in the pos
+000143e0: 6974 696f 6e20 656d 6265 6464 696e 6773  ition embeddings
+000143f0: 2e20 5365 6c65 6374 6564 2069 6e20 7468  . Selected in th
+00014400: 6520 7261 6e67 6520 6060 5b30 2c0a 2020  e range ``[0,.  
+00014410: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+00014420: 2e6d 6178 5f70 6f73 6974 696f 6e5f 656d  .max_position_em
+00014430: 6265 6464 696e 6773 202d 2031 5d60 602e  beddings - 1]``.
+00014440: 0a0a 2020 2020 2020 2020 2020 2020 6057  ..            `W
+00014450: 6861 7420 6172 6520 706f 7369 7469 6f6e  hat are position
+00014460: 2049 4473 3f20 3c2e 2e2f 676c 6f73 7361   IDs? <../glossa
+00014470: 7279 2e68 746d 6c23 706f 7369 7469 6f6e  ry.html#position
+00014480: 2d69 6473 3e60 5f5f 0a20 2020 2020 2020  -ids>`__.       
+00014490: 2068 6561 645f 6d61 736b 2028 3a6f 626a   head_mask (:obj
+000144a0: 3a60 746f 7263 682e 466c 6f61 7454 656e  :`torch.FloatTen
+000144b0: 736f 7260 206f 6620 7368 6170 6520 3a6f  sor` of shape :o
+000144c0: 626a 3a60 286e 756d 5f68 6561 6473 2c29  bj:`(num_heads,)
+000144d0: 6020 6f72 203a 6f62 6a3a 6028 6e75 6d5f  ` or :obj:`(num_
+000144e0: 6c61 7965 7273 2c20 6e75 6d5f 6865 6164  layers, num_head
+000144f0: 7329 602c 2060 6f70 7469 6f6e 616c 6029  s)`, `optional`)
+00014500: 3a0a 2020 2020 2020 2020 2020 2020 4d61  :.            Ma
+00014510: 736b 2074 6f20 6e75 6c6c 6966 7920 7365  sk to nullify se
+00014520: 6c65 6374 6564 2068 6561 6473 206f 6620  lected heads of 
+00014530: 7468 6520 7365 6c66 2d61 7474 656e 7469  the self-attenti
+00014540: 6f6e 206d 6f64 756c 6573 2e20 4d61 736b  on modules. Mask
+00014550: 2076 616c 7565 7320 7365 6c65 6374 6564   values selected
+00014560: 2069 6e20 6060 5b30 2c20 315d 6060 3a0a   in ``[0, 1]``:.
+00014570: 0a20 2020 2020 2020 2020 2020 202d 2031  .            - 1
+00014580: 2069 6e64 6963 6174 6573 2074 6865 2068   indicates the h
+00014590: 6561 6420 6973 202a 2a6e 6f74 206d 6173  ead is **not mas
+000145a0: 6b65 642a 2a2c 0a20 2020 2020 2020 2020  ked**,.         
+000145b0: 2020 202d 2030 2069 6e64 6963 6174 6573     - 0 indicates
+000145c0: 2074 6865 2068 6561 6420 6973 202a 2a6d   the head is **m
+000145d0: 6173 6b65 642a 2a2e 0a0a 2020 2020 2020  asked**...      
+000145e0: 2020 696e 7075 7473 5f65 6d62 6564 7320    inputs_embeds 
+000145f0: 283a 6f62 6a3a 6074 6f72 6368 2e46 6c6f  (:obj:`torch.Flo
+00014600: 6174 5465 6e73 6f72 6020 6f66 2073 6861  atTensor` of sha
+00014610: 7065 203a 6f62 6a3a 6028 6261 7463 685f  pe :obj:`(batch_
+00014620: 7369 7a65 2c20 7365 7175 656e 6365 5f6c  size, sequence_l
+00014630: 656e 6774 682c 2068 6964 6465 6e5f 7369  ength, hidden_si
+00014640: 7a65 2960 2c20 606f 7074 696f 6e61 6c60  ze)`, `optional`
+00014650: 293a 0a20 2020 2020 2020 2020 2020 204f  ):.            O
+00014660: 7074 696f 6e61 6c6c 792c 2069 6e73 7465  ptionally, inste
+00014670: 6164 206f 6620 7061 7373 696e 6720 3a6f  ad of passing :o
+00014680: 626a 3a60 696e 7075 745f 6964 7360 2079  bj:`input_ids` y
+00014690: 6f75 2063 616e 2063 686f 6f73 6520 746f  ou can choose to
+000146a0: 2064 6972 6563 746c 7920 7061 7373 2061   directly pass a
+000146b0: 6e20 656d 6265 6464 6564 2072 6570 7265  n embedded repre
+000146c0: 7365 6e74 6174 696f 6e2e 0a20 2020 2020  sentation..     
+000146d0: 2020 2020 2020 2054 6869 7320 6973 2075         This is u
+000146e0: 7365 6675 6c20 6966 2079 6f75 2077 616e  seful if you wan
+000146f0: 7420 6d6f 7265 2063 6f6e 7472 6f6c 206f  t more control o
+00014700: 7665 7220 686f 7720 746f 2063 6f6e 7665  ver how to conve
+00014710: 7274 203a 6f62 6a3a 6069 6e70 7574 5f69  rt :obj:`input_i
+00014720: 6473 6020 696e 6469 6365 7320 696e 746f  ds` indices into
+00014730: 2061 7373 6f63 6961 7465 640a 2020 2020   associated.    
+00014740: 2020 2020 2020 2020 7665 6374 6f72 7320          vectors 
+00014750: 7468 616e 2074 6865 206d 6f64 656c 2773  than the model's
+00014760: 2069 6e74 6572 6e61 6c20 656d 6265 6464   internal embedd
+00014770: 696e 6720 6c6f 6f6b 7570 206d 6174 7269  ing lookup matri
+00014780: 782e 0a20 2020 2020 2020 206e 756d 5f68  x..        num_h
+00014790: 6173 6865 7320 283a 6f62 6a3a 6069 6e74  ashes (:obj:`int
+000147a0: 602c 2060 6f70 7469 6f6e 616c 6029 3a0a  `, `optional`):.
+000147b0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+000147c0: 6e75 6d62 6572 206f 6620 6861 7368 696e  number of hashin
+000147d0: 6720 726f 756e 6473 2074 6861 7420 7368  g rounds that sh
+000147e0: 6f75 6c64 2062 6520 7065 7266 6f72 6d65  ould be performe
+000147f0: 6420 6475 7269 6e67 2062 7563 6b65 7469  d during bucketi
+00014800: 6e67 2e20 5365 7474 696e 6720 7468 6973  ng. Setting this
+00014810: 2061 7267 756d 656e 7420 6f76 6572 7772   argument overwr
+00014820: 6974 6573 0a20 2020 2020 2020 2020 2020  ites.           
+00014830: 2074 6865 2064 6566 6175 6c74 2064 6566   the default def
+00014840: 696e 6564 2069 6e20 3a6f 626a 3a60 636f  ined in :obj:`co
+00014850: 6e66 6967 2e6e 756d 5f68 6173 6865 7360  nfig.num_hashes`
+00014860: 2e0a 0a20 2020 2020 2020 2020 2020 2046  ...            F
+00014870: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00014880: 696f 6e2c 2073 6565 203a 6f62 6a3a 606e  ion, see :obj:`n
+00014890: 756d 5f68 6173 6865 7360 2069 6e20 3a63  um_hashes` in :c
+000148a0: 6c61 7373 3a60 7e74 7261 6e73 666f 726d  lass:`~transform
+000148b0: 6572 732e 5265 666f 726d 6572 436f 6e66  ers.ReformerConf
+000148c0: 6967 602e 0a20 2020 2020 2020 2070 6173  ig`..        pas
+000148d0: 745f 6275 636b 6574 735f 7374 6174 6573  t_buckets_states
+000148e0: 2028 3a6f 626a 3a60 4c69 7374 5b54 7570   (:obj:`List[Tup
+000148f0: 6c65 2874 6f72 6368 2e4c 6f6e 6754 656e  le(torch.LongTen
+00014900: 736f 722c 2074 6f72 6368 2e46 6c6f 6174  sor, torch.Float
+00014910: 5465 6e73 6f72 295d 602c 2060 6f70 7469  Tensor)]`, `opti
+00014920: 6f6e 616c 6029 3a0a 2020 2020 2020 2020  onal`):.        
+00014930: 2020 2020 4c69 7374 206f 6620 3a6f 626a      List of :obj
+00014940: 3a60 5475 706c 6528 746f 7263 682e 4c6f  :`Tuple(torch.Lo
+00014950: 6e67 5465 6e73 6f72 2c20 746f 7263 682e  ngTensor, torch.
+00014960: 466c 6f61 7454 656e 736f 7260 206f 6620  FloatTensor` of 
+00014970: 6c65 6e67 7468 203a 6f62 6a3a 6063 6f6e  length :obj:`con
+00014980: 6669 672e 6e5f 6c61 7965 7273 602c 2077  fig.n_layers`, w
+00014990: 6974 6820 7468 6520 6669 7273 740a 2020  ith the first.  
+000149a0: 2020 2020 2020 2020 2020 656c 656d 656e            elemen
+000149b0: 7420 6265 696e 6720 7468 6520 7072 6576  t being the prev
+000149c0: 696f 7573 2060 6275 636b 6574 7360 206f  ious `buckets` o
+000149d0: 6620 7368 6170 6520 3a6f 626a 3a60 2862  f shape :obj:`(b
+000149e0: 6174 6368 5f73 697a 652c 206e 756d 5f68  atch_size, num_h
+000149f0: 6561 6473 2c20 6e75 6d5f 6861 7368 6573  eads, num_hashes
+00014a00: 2c20 7365 7175 656e 6365 5f6c 656e 6774  , sequence_lengt
+00014a10: 6829 6029 0a20 2020 2020 2020 2020 2020  h)`).           
+00014a20: 2061 6e64 2074 6865 2073 6563 6f6e 6420   and the second 
+00014a30: 6265 696e 6720 7468 6520 7072 6576 696f  being the previo
+00014a40: 7573 2060 6869 6464 656e 5f73 7461 7465  us `hidden_state
+00014a50: 7360 206f 6620 7368 6170 6520 3a6f 626a  s` of shape :obj
+00014a60: 3a60 2862 6174 6368 5f73 697a 652c 2073  :`(batch_size, s
+00014a70: 6571 7565 6e63 655f 6c65 6e67 7468 2c0a  equence_length,.
+00014a80: 2020 2020 2020 2020 2020 2020 6869 6464              hidd
+00014a90: 656e 5f73 697a 6529 6029 2e0a 0a20 2020  en_size)`)...   
+00014aa0: 2020 2020 2020 2020 2043 6f6e 7461 696e           Contain
+00014ab0: 7320 7072 6563 6f6d 7075 7465 6420 6869  s precomputed hi
+00014ac0: 6464 656e 2d73 7461 7465 7320 616e 6420  dden-states and 
+00014ad0: 6275 636b 6574 7320 286f 6e6c 7920 7265  buckets (only re
+00014ae0: 6c65 7661 6e74 2066 6f72 204c 5348 2053  levant for LSH S
+00014af0: 656c 662d 4174 7465 6e74 696f 6e29 2e20  elf-Attention). 
+00014b00: 4361 6e20 6265 2075 7365 6420 746f 2073  Can be used to s
+00014b10: 7065 6564 0a20 2020 2020 2020 2020 2020  peed.           
+00014b20: 2075 7020 7365 7175 656e 7469 616c 2064   up sequential d
+00014b30: 6563 6f64 696e 672e 0a20 2020 2020 2020  ecoding..       
+00014b40: 2075 7365 5f63 6163 6865 2028 3a6f 626a   use_cache (:obj
+00014b50: 3a60 626f 6f6c 602c 2060 6f70 7469 6f6e  :`bool`, `option
+00014b60: 616c 6029 3a0a 2020 2020 2020 2020 2020  al`):.          
+00014b70: 2020 4966 2073 6574 2074 6f20 3a6f 626a    If set to :obj
+00014b80: 3a60 5472 7565 602c 203a 6f62 6a3a 6070  :`True`, :obj:`p
+00014b90: 6173 745f 6b65 795f 7661 6c75 6573 6020  ast_key_values` 
+00014ba0: 6b65 7920 7661 6c75 6520 7374 6174 6573  key value states
+00014bb0: 2061 7265 2072 6574 7572 6e65 6420 616e   are returned an
+00014bc0: 6420 6361 6e20 6265 2075 7365 6420 746f  d can be used to
+00014bd0: 2073 7065 6564 2075 700a 2020 2020 2020   speed up.      
+00014be0: 2020 2020 2020 6465 636f 6469 6e67 2028        decoding (
+00014bf0: 7365 6520 3a6f 626a 3a60 7061 7374 5f6b  see :obj:`past_k
+00014c00: 6579 5f76 616c 7565 7360 292e 0a20 2020  ey_values`)..   
+00014c10: 2020 2020 206f 7574 7075 745f 6174 7465       output_atte
+00014c20: 6e74 696f 6e73 2028 3a6f 626a 3a60 626f  ntions (:obj:`bo
+00014c30: 6f6c 602c 2060 6f70 7469 6f6e 616c 6029  ol`, `optional`)
+00014c40: 3a0a 2020 2020 2020 2020 2020 2020 5768  :.            Wh
+00014c50: 6574 6865 7220 6f72 206e 6f74 2074 6f20  ether or not to 
+00014c60: 7265 7475 726e 2074 6865 2061 7474 656e  return the atten
+00014c70: 7469 6f6e 7320 7465 6e73 6f72 7320 6f66  tions tensors of
+00014c80: 2061 6c6c 2061 7474 656e 7469 6f6e 206c   all attention l
+00014c90: 6179 6572 732e 2053 6565 2060 6061 7474  ayers. See ``att
+00014ca0: 656e 7469 6f6e 7360 6020 756e 6465 7220  entions`` under 
+00014cb0: 7265 7475 726e 6564 0a20 2020 2020 2020  returned.       
+00014cc0: 2020 2020 2074 656e 736f 7273 2066 6f72       tensors for
+00014cd0: 206d 6f72 6520 6465 7461 696c 2e0a 2020   more detail..  
+00014ce0: 2020 2020 2020 6f75 7470 7574 5f68 6964        output_hid
+00014cf0: 6465 6e5f 7374 6174 6573 2028 3a6f 626a  den_states (:obj
+00014d00: 3a60 626f 6f6c 602c 2060 6f70 7469 6f6e  :`bool`, `option
+00014d10: 616c 6029 3a0a 2020 2020 2020 2020 2020  al`):.          
+00014d20: 2020 5768 6574 6865 7220 6f72 206e 6f74    Whether or not
+00014d30: 2074 6f20 7265 7475 726e 2074 6865 2068   to return the h
+00014d40: 6964 6465 6e20 7374 6174 6573 206f 6620  idden states of 
+00014d50: 616c 6c20 6c61 7965 7273 2e20 5365 6520  all layers. See 
+00014d60: 6060 6869 6464 656e 5f73 7461 7465 7360  ``hidden_states`
+00014d70: 6020 756e 6465 7220 7265 7475 726e 6564  ` under returned
+00014d80: 2074 656e 736f 7273 2066 6f72 0a20 2020   tensors for.   
+00014d90: 2020 2020 2020 2020 206d 6f72 6520 6465           more de
+00014da0: 7461 696c 2e0a 2020 2020 2020 2020 7265  tail..        re
+00014db0: 7475 726e 5f64 6963 7420 283a 6f62 6a3a  turn_dict (:obj:
+00014dc0: 6062 6f6f 6c60 2c20 606f 7074 696f 6e61  `bool`, `optiona
+00014dd0: 6c60 293a 0a20 2020 2020 2020 2020 2020  l`):.           
+00014de0: 2057 6865 7468 6572 206f 7220 6e6f 7420   Whether or not 
+00014df0: 746f 2072 6574 7572 6e20 6120 3a63 6c61  to return a :cla
+00014e00: 7373 3a60 7e74 7261 6e73 666f 726d 6572  ss:`~transformer
+00014e10: 732e 6669 6c65 5f75 7469 6c73 2e4d 6f64  s.file_utils.Mod
+00014e20: 656c 4f75 7470 7574 6020 696e 7374 6561  elOutput` instea
+00014e30: 6420 6f66 2061 2070 6c61 696e 2074 7570  d of a plain tup
+00014e40: 6c65 2e0a 2222 220a 0a0a 4061 6464 5f73  le.."""...@add_s
+00014e50: 7461 7274 5f64 6f63 7374 7269 6e67 7328  tart_docstrings(
+00014e60: 0a20 2020 2022 5468 6520 6261 7265 2052  .    "The bare R
+00014e70: 6566 6f72 6d65 7220 4d6f 6465 6c20 7472  eformer Model tr
+00014e80: 616e 7366 6f72 6d65 7220 6f75 7470 7574  ansformer output
+00014e90: 7469 6e67 2072 6177 2068 6964 6465 6e2d  ting raw hidden-
+00014ea0: 7374 6174 6573 2220 2277 6974 686f 7574  states" "without
+00014eb0: 2061 6e79 2073 7065 6369 6669 6320 6865   any specific he
+00014ec0: 6164 206f 6e20 746f 702e 222c 0a20 2020  ad on top.",.   
+00014ed0: 2052 4546 4f52 4d45 525f 5354 4152 545f   REFORMER_START_
+00014ee0: 444f 4353 5452 494e 472c 0a29 0a63 6c61  DOCSTRING,.).cla
+00014ef0: 7373 2052 6566 6f72 6d65 724d 6f64 656c  ss ReformerModel
+00014f00: 2852 6566 6f72 6d65 7250 7265 5472 6169  (ReformerPreTrai
+00014f10: 6e65 644d 6f64 656c 293a 0a20 2020 2064  nedModel):.    d
+00014f20: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
+00014f30: 2c20 636f 6e66 6967 293a 0a20 2020 2020  , config):.     
+00014f40: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
+00014f50: 745f 5f28 636f 6e66 6967 290a 2020 2020  t__(config).    
+00014f60: 2020 2020 7365 6c66 2e63 6f6e 6669 6720      self.config 
+00014f70: 3d20 636f 6e66 6967 0a20 2020 2020 2020  = config.       
+00014f80: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+00014f90: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+00014fa0: 672e 6e75 6d5f 6869 6464 656e 5f6c 6179  g.num_hidden_lay
+00014fb0: 6572 7320 3e20 300a 2020 2020 2020 2020  ers > 0.        
+00014fc0: 292c 2022 6063 6f6e 6669 672e 6174 746e  ), "`config.attn
+00014fd0: 5f6c 6179 6572 7360 2069 7320 656d 7074  _layers` is empt
+00014fe0: 792e 2053 656c 6563 7420 6174 206c 6561  y. Select at lea
+00014ff0: 7374 206f 6e65 2061 7474 6e20 6c61 7965  st one attn laye
+00015000: 7220 666f 726d 205b 276c 7368 272c 2027  r form ['lsh', '
+00015010: 6c6f 6361 6c27 5d22 0a0a 2020 2020 2020  local']"..      
+00015020: 2020 7365 6c66 2e65 6d62 6564 6469 6e67    self.embedding
+00015030: 7320 3d20 5265 666f 726d 6572 456d 6265  s = ReformerEmbe
+00015040: 6464 696e 6773 2863 6f6e 6669 6729 0a20  ddings(config). 
+00015050: 2020 2020 2020 2073 656c 662e 656e 636f         self.enco
+00015060: 6465 7220 3d20 5265 666f 726d 6572 456e  der = ReformerEn
+00015070: 636f 6465 7228 636f 6e66 6967 290a 0a20  coder(config).. 
+00015080: 2020 2020 2020 2073 656c 662e 696e 6974         self.init
+00015090: 5f77 6569 6768 7473 2829 0a0a 2020 2020  _weights()..    
+000150a0: 6465 6620 6765 745f 696e 7075 745f 656d  def get_input_em
+000150b0: 6265 6464 696e 6773 2873 656c 6629 3a0a  beddings(self):.
+000150c0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000150d0: 656c 662e 656d 6265 6464 696e 6773 2e77  elf.embeddings.w
+000150e0: 6f72 645f 656d 6265 6464 696e 6773 0a0a  ord_embeddings..
+000150f0: 2020 2020 6465 6620 7365 745f 696e 7075      def set_inpu
+00015100: 745f 656d 6265 6464 696e 6773 2873 656c  t_embeddings(sel
+00015110: 662c 2076 616c 7565 293a 0a20 2020 2020  f, value):.     
+00015120: 2020 2073 656c 662e 656d 6265 6464 696e     self.embeddin
+00015130: 6773 2e77 6f72 645f 656d 6265 6464 696e  gs.word_embeddin
+00015140: 6773 203d 2076 616c 7565 0a0a 2020 2020  gs = value..    
+00015150: 6465 6620 5f70 7275 6e65 5f68 6561 6473  def _prune_heads
+00015160: 2873 656c 662c 2068 6561 6473 5f74 6f5f  (self, heads_to_
+00015170: 7072 756e 6529 3a0a 2020 2020 2020 2020  prune):.        
+00015180: 2222 220a 2020 2020 2020 2020 5072 756e  """.        Prun
+00015190: 6573 2068 6561 6473 206f 6620 7468 6520  es heads of the 
+000151a0: 6d6f 6465 6c2e 2068 6561 6473 5f74 6f5f  model. heads_to_
+000151b0: 7072 756e 653a 2064 6963 7420 6f66 207b  prune: dict of {
+000151c0: 6c61 7965 725f 6e75 6d3a 206c 6973 7420  layer_num: list 
+000151d0: 6f66 2068 6561 6473 2074 6f20 7072 756e  of heads to prun
+000151e0: 6520 696e 2074 6869 7320 6c61 7965 727d  e in this layer}
+000151f0: 2053 6565 2062 6173 650a 2020 2020 2020   See base.      
+00015200: 2020 636c 6173 7320 5072 6554 7261 696e    class PreTrain
+00015210: 6564 4d6f 6465 6c0a 2020 2020 2020 2020  edModel.        
+00015220: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
+00015230: 6c61 7965 722c 2068 6561 6473 2069 6e20  layer, heads in 
+00015240: 6865 6164 735f 746f 5f70 7275 6e65 2e69  heads_to_prune.i
+00015250: 7465 6d73 2829 3a0a 2020 2020 2020 2020  tems():.        
+00015260: 2020 2020 7365 6c66 2e65 6e63 6f64 6572      self.encoder
+00015270: 2e6c 6179 6572 5b6c 6179 6572 5d2e 6174  .layer[layer].at
+00015280: 7465 6e74 696f 6e2e 7072 756e 655f 6865  tention.prune_he
+00015290: 6164 7328 6865 6164 7329 0a0a 2020 2020  ads(heads)..    
+000152a0: 4061 6464 5f73 7461 7274 5f64 6f63 7374  @add_start_docst
+000152b0: 7269 6e67 735f 746f 5f6d 6f64 656c 5f66  rings_to_model_f
+000152c0: 6f72 7761 7264 2852 4546 4f52 4d45 525f  orward(REFORMER_
+000152d0: 494e 5055 5453 5f44 4f43 5354 5249 4e47  INPUTS_DOCSTRING
+000152e0: 290a 2020 2020 4061 6464 5f63 6f64 655f  ).    @add_code_
+000152f0: 7361 6d70 6c65 5f64 6f63 7374 7269 6e67  sample_docstring
+00015300: 7328 0a20 2020 2020 2020 2074 6f6b 656e  s(.        token
+00015310: 697a 6572 5f63 6c61 7373 3d5f 544f 4b45  izer_class=_TOKE
+00015320: 4e49 5a45 525f 464f 525f 444f 432c 0a20  NIZER_FOR_DOC,. 
+00015330: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
+00015340: 743d 5f43 4845 434b 504f 494e 545f 464f  t=_CHECKPOINT_FO
+00015350: 525f 444f 432c 0a20 2020 2020 2020 206f  R_DOC,.        o
+00015360: 7574 7075 745f 7479 7065 3d52 6566 6f72  utput_type=Refor
+00015370: 6d65 724d 6f64 656c 4f75 7470 7574 2c0a  merModelOutput,.
+00015380: 2020 2020 2020 2020 636f 6e66 6967 5f63          config_c
+00015390: 6c61 7373 3d5f 434f 4e46 4947 5f46 4f52  lass=_CONFIG_FOR
+000153a0: 5f44 4f43 2c0a 2020 2020 290a 2020 2020  _DOC,.    ).    
+000153b0: 6465 6620 666f 7277 6172 6428 0a20 2020  def forward(.   
+000153c0: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+000153d0: 2020 2069 6e70 7574 5f69 6473 3d4e 6f6e     input_ids=Non
+000153e0: 652c 0a20 2020 2020 2020 2061 7474 656e  e,.        atten
+000153f0: 7469 6f6e 5f6d 6173 6b3d 4e6f 6e65 2c0a  tion_mask=None,.
+00015400: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
+00015410: 5f69 6473 3d4e 6f6e 652c 0a20 2020 2020  _ids=None,.     
+00015420: 2020 2068 6561 645f 6d61 736b 3d4e 6f6e     head_mask=Non
+00015430: 652c 0a20 2020 2020 2020 2069 6e70 7574  e,.        input
+00015440: 735f 656d 6265 6473 3d4e 6f6e 652c 0a20  s_embeds=None,. 
+00015450: 2020 2020 2020 206e 756d 5f68 6173 6865         num_hashe
+00015460: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+00015470: 7061 7374 5f62 7563 6b65 7473 5f73 7461  past_buckets_sta
+00015480: 7465 733d 4e6f 6e65 2c0a 2020 2020 2020  tes=None,.      
+00015490: 2020 7573 655f 6361 6368 653d 4e6f 6e65    use_cache=None
+000154a0: 2c0a 2020 2020 2020 2020 6f75 7470 7574  ,.        output
+000154b0: 5f68 6964 6465 6e5f 7374 6174 6573 3d4e  _hidden_states=N
+000154c0: 6f6e 652c 0a20 2020 2020 2020 206f 7574  one,.        out
+000154d0: 7075 745f 6174 7465 6e74 696f 6e73 3d4e  put_attentions=N
+000154e0: 6f6e 652c 0a20 2020 2020 2020 2072 6574  one,.        ret
+000154f0: 7572 6e5f 6469 6374 3d4e 6f6e 652c 0a20  urn_dict=None,. 
+00015500: 2020 2029 3a0a 2020 2020 2020 2020 7573     ):.        us
+00015510: 655f 6361 6368 6520 3d20 7573 655f 6361  e_cache = use_ca
+00015520: 6368 6520 6966 2075 7365 5f63 6163 6865  che if use_cache
+00015530: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+00015540: 6520 7365 6c66 2e63 6f6e 6669 672e 7573  e self.config.us
+00015550: 655f 6361 6368 650a 2020 2020 2020 2020  e_cache.        
+00015560: 6f75 7470 7574 5f61 7474 656e 7469 6f6e  output_attention
+00015570: 7320 3d20 6f75 7470 7574 5f61 7474 656e  s = output_atten
+00015580: 7469 6f6e 7320 6966 206f 7574 7075 745f  tions if output_
+00015590: 6174 7465 6e74 696f 6e73 2069 7320 6e6f  attentions is no
+000155a0: 7420 4e6f 6e65 2065 6c73 6520 7365 6c66  t None else self
+000155b0: 2e63 6f6e 6669 672e 6f75 7470 7574 5f61  .config.output_a
+000155c0: 7474 656e 7469 6f6e 730a 2020 2020 2020  ttentions.      
+000155d0: 2020 6f75 7470 7574 5f68 6964 6465 6e5f    output_hidden_
+000155e0: 7374 6174 6573 203d 2028 0a20 2020 2020  states = (.     
+000155f0: 2020 2020 2020 206f 7574 7075 745f 6869         output_hi
+00015600: 6464 656e 5f73 7461 7465 7320 6966 206f  dden_states if o
+00015610: 7574 7075 745f 6869 6464 656e 5f73 7461  utput_hidden_sta
+00015620: 7465 7320 6973 206e 6f74 204e 6f6e 6520  tes is not None 
+00015630: 656c 7365 2073 656c 662e 636f 6e66 6967  else self.config
+00015640: 2e6f 7574 7075 745f 6869 6464 656e 5f73  .output_hidden_s
+00015650: 7461 7465 730a 2020 2020 2020 2020 290a  tates.        ).
+00015660: 2020 2020 2020 2020 7265 7475 726e 5f64          return_d
+00015670: 6963 7420 3d20 7265 7475 726e 5f64 6963  ict = return_dic
+00015680: 7420 6966 2072 6574 7572 6e5f 6469 6374  t if return_dict
+00015690: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+000156a0: 6520 7365 6c66 2e63 6f6e 6669 672e 7573  e self.config.us
+000156b0: 655f 7265 7475 726e 5f64 6963 740a 0a20  e_return_dict.. 
+000156c0: 2020 2020 2020 2069 6620 696e 7075 745f         if input_
+000156d0: 6964 7320 6973 206e 6f74 204e 6f6e 6520  ids is not None 
+000156e0: 616e 6420 696e 7075 7473 5f65 6d62 6564  and inputs_embed
+000156f0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00015700: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00015710: 2056 616c 7565 4572 726f 7228 2259 6f75   ValueError("You
+00015720: 2063 616e 6e6f 7420 7370 6563 6966 7920   cannot specify 
+00015730: 626f 7468 2069 6e70 7574 5f69 6473 2061  both input_ids a
+00015740: 6e64 2069 6e70 7574 735f 656d 6265 6473  nd inputs_embeds
+00015750: 2061 7420 7468 6520 7361 6d65 2074 696d   at the same tim
+00015760: 6522 290a 2020 2020 2020 2020 656c 6966  e").        elif
+00015770: 2069 6e70 7574 5f69 6473 2069 7320 6e6f   input_ids is no
+00015780: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00015790: 2020 2020 696e 7075 745f 7368 6170 6520      input_shape 
+000157a0: 3d20 696e 7075 745f 6964 732e 7369 7a65  = input_ids.size
+000157b0: 2829 2020 2320 6e6f 7161 3a20 4638 3431  ()  # noqa: F841
+000157c0: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
+000157d0: 6963 6520 3d20 696e 7075 745f 6964 732e  ice = input_ids.
+000157e0: 6465 7669 6365 0a20 2020 2020 2020 2065  device.        e
+000157f0: 6c69 6620 696e 7075 7473 5f65 6d62 6564  lif inputs_embed
+00015800: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00015810: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00015820: 5f73 6861 7065 203d 2069 6e70 7574 735f  _shape = inputs_
+00015830: 656d 6265 6473 2e73 697a 6528 295b 3a2d  embeds.size()[:-
+00015840: 315d 2020 2320 6e6f 7161 3a20 4638 3431  1]  # noqa: F841
+00015850: 0a20 2020 2020 2020 2020 2020 2064 6576  .            dev
+00015860: 6963 6520 3d20 696e 7075 7473 5f65 6d62  ice = inputs_emb
+00015870: 6564 732e 6465 7669 6365 0a20 2020 2020  eds.device.     
+00015880: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00015890: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+000158a0: 4572 726f 7228 2259 6f75 2068 6176 6520  Error("You have 
+000158b0: 746f 2073 7065 6369 6679 2065 6974 6865  to specify eithe
+000158c0: 7220 696e 7075 745f 6964 7320 6f72 2069  r input_ids or i
+000158d0: 6e70 7574 735f 656d 6265 6473 2229 0a0a  nputs_embeds")..
+000158e0: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+000158f0: 0a20 2020 2020 2020 2020 2020 206c 656e  .            len
+00015900: 2869 6e70 7574 5f73 6861 7065 2920 3d3d  (input_shape) ==
+00015910: 2032 0a20 2020 2020 2020 2029 2c20 6622   2.        ), f"
+00015920: 6069 6e70 7574 5f69 6473 6020 6861 7665  `input_ids` have
+00015930: 2062 6520 6f66 2073 6861 7065 2060 5b62   be of shape `[b
+00015940: 6174 6368 5f73 697a 652c 2073 6571 7565  atch_size, seque
+00015950: 6e63 655f 6c65 6e67 7468 5d60 2c20 6275  nce_length]`, bu
+00015960: 7420 676f 7420 7368 6170 653a 207b 696e  t got shape: {in
+00015970: 7075 745f 7368 6170 657d 220a 0a20 2020  put_shape}"..   
+00015980: 2020 2020 2069 6620 7061 7374 5f62 7563       if past_buc
+00015990: 6b65 7473 5f73 7461 7465 7320 6973 206e  kets_states is n
+000159a0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000159b0: 2020 2020 2061 7373 6572 7420 6e6f 7420       assert not 
+000159c0: 7365 6c66 2e74 7261 696e 696e 672c 2022  self.training, "
+000159d0: 6070 6173 745f 6275 636b 6574 735f 7374  `past_buckets_st
+000159e0: 6174 6573 6020 6361 6e20 6f6e 6c79 2062  ates` can only b
+000159f0: 6520 7573 6564 2066 6f72 2069 6e66 6572  e used for infer
+00015a00: 656e 6365 2c20 6e6f 7420 666f 7220 7472  ence, not for tr
+00015a10: 6169 6e69 6e67 602e 220a 0a20 2020 2020  aining`."..     
+00015a20: 2020 2023 2070 7265 7061 7265 2068 6561     # prepare hea
+00015a30: 6420 6d61 736b 0a20 2020 2020 2020 2068  d mask.        h
+00015a40: 6561 645f 6d61 736b 203d 2073 656c 662e  ead_mask = self.
+00015a50: 6765 745f 6865 6164 5f6d 6173 6b28 6865  get_head_mask(he
+00015a60: 6164 5f6d 6173 6b2c 2073 656c 662e 636f  ad_mask, self.co
+00015a70: 6e66 6967 2e6e 756d 5f68 6964 6465 6e5f  nfig.num_hidden_
+00015a80: 6c61 7965 7273 2c20 6973 5f61 7474 656e  layers, is_atten
+00015a90: 7469 6f6e 5f63 6875 6e6b 6564 3d54 7275  tion_chunked=Tru
+00015aa0: 6529 0a0a 2020 2020 2020 2020 2320 6f72  e)..        # or
+00015ab0: 6967 696e 616c 2073 6571 7565 6e63 6520  iginal sequence 
+00015ac0: 6c65 6e67 7468 2066 6f72 2070 6164 6469  length for paddi
+00015ad0: 6e67 0a20 2020 2020 2020 206f 7269 675f  ng.        orig_
+00015ae0: 7365 7175 656e 6365 5f6c 656e 6774 6820  sequence_length 
+00015af0: 3d20 696e 7075 745f 7368 6170 655b 2d31  = input_shape[-1
+00015b00: 5d0a 0a20 2020 2020 2020 2023 2069 6620  ]..        # if 
+00015b10: 6e65 6564 7320 7061 6464 696e 670a 2020  needs padding.  
+00015b20: 2020 2020 2020 6c65 6173 745f 636f 6d6d        least_comm
+00015b30: 6f6e 5f6d 756c 745f 6368 756e 6b5f 6c65  on_mult_chunk_le
+00015b40: 6e67 7468 203d 205f 6765 745f 6c65 6173  ngth = _get_leas
+00015b50: 745f 636f 6d6d 6f6e 5f6d 756c 745f 6368  t_common_mult_ch
+00015b60: 756e 6b5f 6c65 6e28 7365 6c66 2e63 6f6e  unk_len(self.con
+00015b70: 6669 6729 0a20 2020 2020 2020 206d 696e  fig).        min
+00015b80: 5f63 6875 6e6b 5f6c 656e 6774 6820 3d20  _chunk_length = 
+00015b90: 5f67 6574 5f6d 696e 5f63 6875 6e6b 5f6c  _get_min_chunk_l
+00015ba0: 656e 2873 656c 662e 636f 6e66 6967 290a  en(self.config).
+00015bb0: 0a20 2020 2020 2020 206d 7573 745f 7061  .        must_pa
+00015bc0: 645f 746f 5f6d 6174 6368 5f63 6875 6e6b  d_to_match_chunk
+00015bd0: 5f6c 656e 6774 6820 3d20 280a 2020 2020  _length = (.    
+00015be0: 2020 2020 2020 2020 696e 7075 745f 7368          input_sh
+00015bf0: 6170 655b 2d31 5d20 2520 6c65 6173 745f  ape[-1] % least_
+00015c00: 636f 6d6d 6f6e 5f6d 756c 745f 6368 756e  common_mult_chun
+00015c10: 6b5f 6c65 6e67 7468 2021 3d20 300a 2020  k_length != 0.  
+00015c20: 2020 2020 2020 2020 2020 616e 6420 696e            and in
+00015c30: 7075 745f 7368 6170 655b 2d31 5d20 3e20  put_shape[-1] > 
+00015c40: 6d69 6e5f 6368 756e 6b5f 6c65 6e67 7468  min_chunk_length
+00015c50: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
+00015c60: 2070 6173 745f 6275 636b 6574 735f 7374   past_buckets_st
+00015c70: 6174 6573 2069 7320 4e6f 6e65 0a20 2020  ates is None.   
+00015c80: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00015c90: 6966 206d 7573 745f 7061 645f 746f 5f6d  if must_pad_to_m
+00015ca0: 6174 6368 5f63 6875 6e6b 5f6c 656e 6774  atch_chunk_lengt
+00015cb0: 683a 0a20 2020 2020 2020 2020 2020 2070  h:.            p
+00015cc0: 6164 6469 6e67 5f6c 656e 6774 6820 3d20  adding_length = 
+00015cd0: 6c65 6173 745f 636f 6d6d 6f6e 5f6d 756c  least_common_mul
+00015ce0: 745f 6368 756e 6b5f 6c65 6e67 7468 202d  t_chunk_length -
+00015cf0: 2069 6e70 7574 5f73 6861 7065 5b2d 315d   input_shape[-1]
+00015d00: 2025 206c 6561 7374 5f63 6f6d 6d6f 6e5f   % least_common_
+00015d10: 6d75 6c74 5f63 6875 6e6b 5f6c 656e 6774  mult_chunk_lengt
+00015d20: 680a 0a20 2020 2020 2020 2020 2020 2069  h..            i
+00015d30: 6620 7365 6c66 2e74 7261 696e 696e 6720  f self.training 
+00015d40: 6973 2054 7275 653a 0a20 2020 2020 2020  is True:.       
+00015d50: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00015d60: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+00015d70: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00015d80: 2249 6620 7472 6169 6e69 6e67 2c20 7365  "If training, se
+00015d90: 7175 656e 6365 206c 656e 6774 6820 7b69  quence length {i
+00015da0: 6e70 7574 5f73 6861 7065 5b2d 315d 7d20  nput_shape[-1]} 
+00015db0: 6861 7320 746f 2062 6520 6120 6d75 6c74  has to be a mult
+00015dc0: 6970 6c65 206f 6620 6c65 6173 7420 636f  iple of least co
+00015dd0: 6d6d 6f6e 206d 756c 7469 706c 6520 220a  mmon multiple ".
+00015de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015df0: 2020 2020 6622 6368 756e 6b5f 6c65 6e67      f"chunk_leng
+00015e00: 7468 207b 6c65 6173 745f 636f 6d6d 6f6e  th {least_common
+00015e10: 5f6d 756c 745f 6368 756e 6b5f 6c65 6e67  _mult_chunk_leng
+00015e20: 7468 7d2e 2050 6c65 6173 6520 636f 6e73  th}. Please cons
+00015e30: 6964 6572 2070 6164 6469 6e67 2074 6865  ider padding the
+00015e40: 2069 6e70 7574 2074 6f20 6120 6c65 6e67   input to a leng
+00015e50: 7468 2022 0a20 2020 2020 2020 2020 2020  th ".           
+00015e60: 2020 2020 2020 2020 2066 226f 6620 7b69           f"of {i
+00015e70: 6e70 7574 5f73 6861 7065 5b2d 315d 202b  nput_shape[-1] +
+00015e80: 2070 6164 6469 6e67 5f6c 656e 6774 687d   padding_length}
+00015e90: 2e22 0a20 2020 2020 2020 2020 2020 2020  .".             
+00015ea0: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00015eb0: 2020 2320 7061 6420 696e 7075 740a 2020    # pad input.  
+00015ec0: 2020 2020 2020 2020 2020 696e 7075 745f            input_
+00015ed0: 6964 732c 2069 6e70 7574 735f 656d 6265  ids, inputs_embe
+00015ee0: 6473 2c20 6174 7465 6e74 696f 6e5f 6d61  ds, attention_ma
+00015ef0: 736b 2c20 706f 7369 7469 6f6e 5f69 6473  sk, position_ids
+00015f00: 2c20 696e 7075 745f 7368 6170 6520 3d20  , input_shape = 
+00015f10: 7365 6c66 2e5f 7061 645f 746f 5f6d 756c  self._pad_to_mul
+00015f20: 745f 6f66 5f63 6875 6e6b 5f6c 656e 6774  t_of_chunk_lengt
+00015f30: 6828 0a20 2020 2020 2020 2020 2020 2020  h(.             
+00015f40: 2020 2069 6e70 7574 5f69 6473 2c0a 2020     input_ids,.  
+00015f50: 2020 2020 2020 2020 2020 2020 2020 696e                in
+00015f60: 7075 7473 5f65 6d62 6564 733d 696e 7075  puts_embeds=inpu
+00015f70: 7473 5f65 6d62 6564 732c 0a20 2020 2020  ts_embeds,.     
+00015f80: 2020 2020 2020 2020 2020 2061 7474 656e             atten
+00015f90: 7469 6f6e 5f6d 6173 6b3d 6174 7465 6e74  tion_mask=attent
+00015fa0: 696f 6e5f 6d61 736b 2c0a 2020 2020 2020  ion_mask,.      
+00015fb0: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+00015fc0: 6f6e 5f69 6473 3d70 6f73 6974 696f 6e5f  on_ids=position_
+00015fd0: 6964 732c 0a20 2020 2020 2020 2020 2020  ids,.           
+00015fe0: 2020 2020 2069 6e70 7574 5f73 6861 7065       input_shape
+00015ff0: 3d69 6e70 7574 5f73 6861 7065 2c0a 2020  =input_shape,.  
+00016000: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+00016010: 6464 696e 675f 6c65 6e67 7468 3d70 6164  dding_length=pad
+00016020: 6469 6e67 5f6c 656e 6774 682c 0a20 2020  ding_length,.   
+00016030: 2020 2020 2020 2020 2020 2020 2070 6164               pad
+00016040: 6465 645f 7365 715f 6c65 6e67 7468 3d6c  ded_seq_length=l
+00016050: 6561 7374 5f63 6f6d 6d6f 6e5f 6d75 6c74  east_common_mult
+00016060: 5f63 6875 6e6b 5f6c 656e 6774 682c 0a20  _chunk_length,. 
+00016070: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00016080: 6576 6963 653d 6465 7669 6365 2c0a 2020  evice=device,.  
+00016090: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+000160a0: 2020 2020 2023 2073 7461 7274 2069 6e64       # start ind
+000160b0: 6578 2066 6f72 2070 6f73 6974 696f 6e20  ex for position 
+000160c0: 656e 636f 6469 6e67 2064 6570 656e 6473  encoding depends
+000160d0: 206f 6e20 696e 6372 656d 656e 7461 6c20   on incremental 
+000160e0: 6465 636f 6469 6e67 0a20 2020 2020 2020  decoding.       
+000160f0: 2069 6620 7061 7374 5f62 7563 6b65 7473   if past_buckets
+00016100: 5f73 7461 7465 7320 6973 206e 6f74 204e  _states is not N
+00016110: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00016120: 2073 7461 7274 5f69 6478 5f70 6f73 5f65   start_idx_pos_e
+00016130: 6e63 6f64 696e 6773 203d 2070 6173 745f  ncodings = past_
+00016140: 6275 636b 6574 735f 7374 6174 6573 5b30  buckets_states[0
+00016150: 5d5b 315d 2e73 6861 7065 5b31 5d0a 2020  ][1].shape[1].  
+00016160: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00016170: 2020 2020 2020 2020 7374 6172 745f 6964          start_id
+00016180: 785f 706f 735f 656e 636f 6469 6e67 7320  x_pos_encodings 
+00016190: 3d20 300a 0a20 2020 2020 2020 2065 6d62  = 0..        emb
+000161a0: 6564 6469 6e67 5f6f 7574 7075 7420 3d20  edding_output = 
+000161b0: 7365 6c66 2e65 6d62 6564 6469 6e67 7328  self.embeddings(
+000161c0: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+000161d0: 7574 5f69 6473 3d69 6e70 7574 5f69 6473  ut_ids=input_ids
+000161e0: 2c0a 2020 2020 2020 2020 2020 2020 706f  ,.            po
+000161f0: 7369 7469 6f6e 5f69 6473 3d70 6f73 6974  sition_ids=posit
+00016200: 696f 6e5f 6964 732c 0a20 2020 2020 2020  ion_ids,.       
+00016210: 2020 2020 2069 6e70 7574 735f 656d 6265       inputs_embe
+00016220: 6473 3d69 6e70 7574 735f 656d 6265 6473  ds=inputs_embeds
+00016230: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
+00016240: 6172 745f 6964 785f 706f 735f 656e 636f  art_idx_pos_enco
+00016250: 6469 6e67 733d 7374 6172 745f 6964 785f  dings=start_idx_
+00016260: 706f 735f 656e 636f 6469 6e67 732c 0a20  pos_encodings,. 
+00016270: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
+00016280: 2020 656e 636f 6465 725f 6f75 7470 7574    encoder_output
+00016290: 7320 3d20 7365 6c66 2e65 6e63 6f64 6572  s = self.encoder
+000162a0: 280a 2020 2020 2020 2020 2020 2020 6869  (.            hi
+000162b0: 6464 656e 5f73 7461 7465 733d 656d 6265  dden_states=embe
+000162c0: 6464 696e 675f 6f75 7470 7574 2c0a 2020  dding_output,.  
+000162d0: 2020 2020 2020 2020 2020 6865 6164 5f6d            head_m
+000162e0: 6173 6b3d 6865 6164 5f6d 6173 6b2c 0a20  ask=head_mask,. 
+000162f0: 2020 2020 2020 2020 2020 2061 7474 656e             atten
+00016300: 7469 6f6e 5f6d 6173 6b3d 6174 7465 6e74  tion_mask=attent
+00016310: 696f 6e5f 6d61 736b 2c0a 2020 2020 2020  ion_mask,.      
+00016320: 2020 2020 2020 6e75 6d5f 6861 7368 6573        num_hashes
+00016330: 3d6e 756d 5f68 6173 6865 732c 0a20 2020  =num_hashes,.   
+00016340: 2020 2020 2020 2020 2070 6173 745f 6275           past_bu
+00016350: 636b 6574 735f 7374 6174 6573 3d70 6173  ckets_states=pas
+00016360: 745f 6275 636b 6574 735f 7374 6174 6573  t_buckets_states
+00016370: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
+00016380: 655f 6361 6368 653d 7573 655f 6361 6368  e_cache=use_cach
+00016390: 652c 0a20 2020 2020 2020 2020 2020 206f  e,.            o
+000163a0: 7269 675f 7365 7175 656e 6365 5f6c 656e  rig_sequence_len
+000163b0: 6774 683d 6f72 6967 5f73 6571 7565 6e63  gth=orig_sequenc
+000163c0: 655f 6c65 6e67 7468 2c0a 2020 2020 2020  e_length,.      
+000163d0: 2020 2020 2020 6f75 7470 7574 5f68 6964        output_hid
+000163e0: 6465 6e5f 7374 6174 6573 3d6f 7574 7075  den_states=outpu
+000163f0: 745f 6869 6464 656e 5f73 7461 7465 732c  t_hidden_states,
+00016400: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
+00016410: 7075 745f 6174 7465 6e74 696f 6e73 3d6f  put_attentions=o
+00016420: 7574 7075 745f 6174 7465 6e74 696f 6e73  utput_attentions
+00016430: 2c0a 2020 2020 2020 2020 290a 2020 2020  ,.        ).    
+00016440: 2020 2020 7365 7175 656e 6365 5f6f 7574      sequence_out
+00016450: 7075 7420 3d20 656e 636f 6465 725f 6f75  put = encoder_ou
+00016460: 7470 7574 732e 6869 6464 656e 5f73 7461  tputs.hidden_sta
+00016470: 7465 730a 0a20 2020 2020 2020 2023 2069  tes..        # i
+00016480: 6620 7061 6464 696e 6720 7761 7320 6170  f padding was ap
+00016490: 706c 6965 640a 2020 2020 2020 2020 6966  plied.        if
+000164a0: 206d 7573 745f 7061 645f 746f 5f6d 6174   must_pad_to_mat
+000164b0: 6368 5f63 6875 6e6b 5f6c 656e 6774 683a  ch_chunk_length:
+000164c0: 0a20 2020 2020 2020 2020 2020 2073 6571  .            seq
+000164d0: 7565 6e63 655f 6f75 7470 7574 203d 2073  uence_output = s
+000164e0: 6571 7565 6e63 655f 6f75 7470 7574 5b3a  equence_output[:
+000164f0: 2c20 3a6f 7269 675f 7365 7175 656e 6365  , :orig_sequence
+00016500: 5f6c 656e 6774 685d 0a0a 2020 2020 2020  _length]..      
+00016510: 2020 7061 7374 5f62 7563 6b65 7473 5f73    past_buckets_s
+00016520: 7461 7465 7320 3d20 656e 636f 6465 725f  tates = encoder_
+00016530: 6f75 7470 7574 732e 7061 7374 5f62 7563  outputs.past_buc
+00016540: 6b65 7473 5f73 7461 7465 7320 6966 2075  kets_states if u
+00016550: 7365 5f63 6163 6865 2065 6c73 6520 4e6f  se_cache else No
+00016560: 6e65 0a20 2020 2020 2020 2068 6964 6465  ne.        hidde
+00016570: 6e5f 7374 6174 6573 203d 2065 6e63 6f64  n_states = encod
+00016580: 6572 5f6f 7574 7075 7473 2e61 6c6c 5f68  er_outputs.all_h
+00016590: 6964 6465 6e5f 7374 6174 6573 2069 6620  idden_states if 
+000165a0: 6f75 7470 7574 5f68 6964 6465 6e5f 7374  output_hidden_st
+000165b0: 6174 6573 2065 6c73 6520 4e6f 6e65 0a20  ates else None. 
+000165c0: 2020 2020 2020 2061 7474 656e 7469 6f6e         attention
+000165d0: 7320 3d20 656e 636f 6465 725f 6f75 7470  s = encoder_outp
+000165e0: 7574 732e 616c 6c5f 6174 7465 6e74 696f  uts.all_attentio
+000165f0: 6e73 2069 6620 6f75 7470 7574 5f61 7474  ns if output_att
+00016600: 656e 7469 6f6e 7320 656c 7365 204e 6f6e  entions else Non
+00016610: 650a 0a20 2020 2020 2020 2069 6620 6e6f  e..        if no
+00016620: 7420 7265 7475 726e 5f64 6963 743a 0a20  t return_dict:. 
+00016630: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00016640: 6e20 7475 706c 6528 7620 666f 7220 7620  n tuple(v for v 
+00016650: 696e 205b 7365 7175 656e 6365 5f6f 7574  in [sequence_out
+00016660: 7075 742c 2070 6173 745f 6275 636b 6574  put, past_bucket
+00016670: 735f 7374 6174 6573 2c20 6869 6464 656e  s_states, hidden
+00016680: 5f73 7461 7465 732c 2061 7474 656e 7469  _states, attenti
+00016690: 6f6e 735d 2069 6620 7620 6973 206e 6f74  ons] if v is not
+000166a0: 204e 6f6e 6529 0a20 2020 2020 2020 2072   None).        r
+000166b0: 6574 7572 6e20 5265 666f 726d 6572 4d6f  eturn ReformerMo
+000166c0: 6465 6c4f 7574 7075 7428 0a20 2020 2020  delOutput(.     
+000166d0: 2020 2020 2020 206c 6173 745f 6869 6464         last_hidd
+000166e0: 656e 5f73 7461 7465 3d73 6571 7565 6e63  en_state=sequenc
+000166f0: 655f 6f75 7470 7574 2c0a 2020 2020 2020  e_output,.      
+00016700: 2020 2020 2020 7061 7374 5f62 7563 6b65        past_bucke
+00016710: 7473 5f73 7461 7465 733d 7061 7374 5f62  ts_states=past_b
+00016720: 7563 6b65 7473 5f73 7461 7465 732c 0a20  uckets_states,. 
+00016730: 2020 2020 2020 2020 2020 2068 6964 6465             hidde
+00016740: 6e5f 7374 6174 6573 3d68 6964 6465 6e5f  n_states=hidden_
+00016750: 7374 6174 6573 2c0a 2020 2020 2020 2020  states,.        
+00016760: 2020 2020 6174 7465 6e74 696f 6e73 3d61      attentions=a
+00016770: 7474 656e 7469 6f6e 732c 0a20 2020 2020  ttentions,.     
+00016780: 2020 2029 0a0a 2020 2020 6465 6620 5f70     )..    def _p
+00016790: 6164 5f74 6f5f 6d75 6c74 5f6f 665f 6368  ad_to_mult_of_ch
+000167a0: 756e 6b5f 6c65 6e67 7468 280a 2020 2020  unk_length(.    
+000167b0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+000167c0: 2020 696e 7075 745f 6964 732c 0a20 2020    input_ids,.   
+000167d0: 2020 2020 2069 6e70 7574 735f 656d 6265       inputs_embe
+000167e0: 6473 3d4e 6f6e 652c 0a20 2020 2020 2020  ds=None,.       
+000167f0: 2061 7474 656e 7469 6f6e 5f6d 6173 6b3d   attention_mask=
+00016800: 4e6f 6e65 2c0a 2020 2020 2020 2020 706f  None,.        po
+00016810: 7369 7469 6f6e 5f69 6473 3d4e 6f6e 652c  sition_ids=None,
+00016820: 0a20 2020 2020 2020 2069 6e70 7574 5f73  .        input_s
+00016830: 6861 7065 3d4e 6f6e 652c 0a20 2020 2020  hape=None,.     
+00016840: 2020 2070 6164 6469 6e67 5f6c 656e 6774     padding_lengt
+00016850: 683d 4e6f 6e65 2c0a 2020 2020 2020 2020  h=None,.        
+00016860: 7061 6464 6564 5f73 6571 5f6c 656e 6774  padded_seq_lengt
+00016870: 683d 4e6f 6e65 2c0a 2020 2020 2020 2020  h=None,.        
+00016880: 6465 7669 6365 3d4e 6f6e 652c 0a20 2020  device=None,.   
+00016890: 2029 3a0a 2020 2020 2020 2020 6c6f 6767   ):.        logg
+000168a0: 6572 2e69 6e66 6f28 0a20 2020 2020 2020  er.info(.       
+000168b0: 2020 2020 2066 2249 6e70 7574 2069 6473       f"Input ids
+000168c0: 2061 7265 2061 7574 6f6d 6174 6963 616c   are automatical
+000168d0: 6c79 2070 6164 6465 6420 6672 6f6d 207b  ly padded from {
+000168e0: 696e 7075 745f 7368 6170 655b 2d31 5d7d  input_shape[-1]}
+000168f0: 2074 6f20 7b69 6e70 7574 5f73 6861 7065   to {input_shape
+00016900: 5b2d 315d 202b 2070 6164 6469 6e67 5f6c  [-1] + padding_l
+00016910: 656e 6774 687d 2074 6f20 6265 2061 2022  ength} to be a "
+00016920: 0a20 2020 2020 2020 2020 2020 2066 226d  .            f"m
+00016930: 756c 7469 706c 6520 6f66 2060 636f 6e66  ultiple of `conf
+00016940: 6967 2e63 6875 6e6b 5f6c 656e 6774 6860  ig.chunk_length`
+00016950: 3a20 7b70 6164 6465 645f 7365 715f 6c65  : {padded_seq_le
+00016960: 6e67 7468 7d22 0a20 2020 2020 2020 2029  ngth}".        )
+00016970: 0a0a 2020 2020 2020 2020 7061 6464 6564  ..        padded
+00016980: 5f69 6e70 7574 5f69 6473 203d 2074 6f72  _input_ids = tor
+00016990: 6368 2e66 756c 6c28 0a20 2020 2020 2020  ch.full(.       
+000169a0: 2020 2020 2028 696e 7075 745f 7368 6170       (input_shap
+000169b0: 655b 305d 2c20 7061 6464 696e 675f 6c65  e[0], padding_le
+000169c0: 6e67 7468 292c 0a20 2020 2020 2020 2020  ngth),.         
+000169d0: 2020 2073 656c 662e 636f 6e66 6967 2e70     self.config.p
+000169e0: 6164 5f74 6f6b 656e 5f69 642c 0a20 2020  ad_token_id,.   
+000169f0: 2020 2020 2020 2020 2064 6576 6963 653d           device=
+00016a00: 6465 7669 6365 2c0a 2020 2020 2020 2020  device,.        
+00016a10: 2020 2020 6474 7970 653d 746f 7263 682e      dtype=torch.
+00016a20: 6c6f 6e67 2c0a 2020 2020 2020 2020 290a  long,.        ).
+00016a30: 0a20 2020 2020 2020 2023 2045 7874 656e  .        # Exten
+00016a40: 6420 6061 7474 656e 7469 6f6e 5f6d 6173  d `attention_mas
+00016a50: 6b60 0a20 2020 2020 2020 2069 6620 6174  k`.        if at
+00016a60: 7465 6e74 696f 6e5f 6d61 736b 2069 7320  tention_mask is 
+00016a70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00016a80: 2020 2020 2020 7061 645f 6174 7465 6e74        pad_attent
+00016a90: 696f 6e5f 6d61 736b 203d 2074 6f72 6368  ion_mask = torch
+00016aa0: 2e7a 6572 6f73 2869 6e70 7574 5f73 6861  .zeros(input_sha
+00016ab0: 7065 5b30 5d2c 2070 6164 6469 6e67 5f6c  pe[0], padding_l
+00016ac0: 656e 6774 682c 2064 6576 6963 653d 6465  ength, device=de
+00016ad0: 7669 6365 2c20 6474 7970 653d 6174 7465  vice, dtype=atte
+00016ae0: 6e74 696f 6e5f 6d61 736b 2e64 7479 7065  ntion_mask.dtype
+00016af0: 290a 0a20 2020 2020 2020 2020 2020 2061  )..            a
+00016b00: 7474 656e 7469 6f6e 5f6d 6173 6b20 3d20  ttention_mask = 
+00016b10: 746f 7263 682e 6361 7428 5b61 7474 656e  torch.cat([atten
+00016b20: 7469 6f6e 5f6d 6173 6b2c 2070 6164 5f61  tion_mask, pad_a
+00016b30: 7474 656e 7469 6f6e 5f6d 6173 6b5d 2c20  ttention_mask], 
+00016b40: 6469 6d3d 2d31 290a 2020 2020 2020 2020  dim=-1).        
+00016b50: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00016b60: 2020 6174 7465 6e74 696f 6e5f 6d61 736b    attention_mask
+00016b70: 203d 2074 6f72 6368 2e63 6174 280a 2020   = torch.cat(.  
+00016b80: 2020 2020 2020 2020 2020 2020 2020 5b0a                [.
+00016b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016ba0: 2020 2020 746f 7263 682e 6f6e 6573 2869      torch.ones(i
+00016bb0: 6e70 7574 5f73 6861 7065 2c20 6465 7669  nput_shape, devi
+00016bc0: 6365 3d64 6576 6963 652c 2064 7479 7065  ce=device, dtype
+00016bd0: 3d74 6f72 6368 2e75 696e 7438 292c 0a20  =torch.uint8),. 
+00016be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016bf0: 2020 2074 6f72 6368 2e7a 6572 6f73 2828     torch.zeros((
+00016c00: 696e 7075 745f 7368 6170 655b 305d 2c20  input_shape[0], 
+00016c10: 7061 6464 696e 675f 6c65 6e67 7468 292c  padding_length),
+00016c20: 2064 6576 6963 653d 6465 7669 6365 2c20   device=device, 
+00016c30: 6474 7970 653d 746f 7263 682e 7569 6e74  dtype=torch.uint
+00016c40: 3829 2c0a 2020 2020 2020 2020 2020 2020  8),.            
+00016c50: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00016c60: 2020 2020 2020 2064 696d 3d2d 312c 0a20         dim=-1,. 
+00016c70: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00016c80: 2020 2020 2020 2320 4578 7465 6e64 2060        # Extend `
+00016c90: 696e 7075 745f 6964 7360 2077 6974 6820  input_ids` with 
+00016ca0: 7061 6464 696e 6720 746f 206d 6174 6368  padding to match
+00016cb0: 206c 6561 7374 2063 6f6d 6d6f 6e20 6d75   least common mu
+00016cc0: 6c74 6970 6c65 2063 6875 6e6b 5f6c 656e  ltiple chunk_len
+00016cd0: 6774 680a 2020 2020 2020 2020 6966 2069  gth.        if i
+00016ce0: 6e70 7574 5f69 6473 2069 7320 6e6f 7420  nput_ids is not 
+00016cf0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00016d00: 2020 696e 7075 745f 6964 7320 3d20 746f    input_ids = to
+00016d10: 7263 682e 6361 7428 5b69 6e70 7574 5f69  rch.cat([input_i
+00016d20: 6473 2c20 7061 6464 6564 5f69 6e70 7574  ds, padded_input
+00016d30: 5f69 6473 5d2c 2064 696d 3d2d 3129 0a20  _ids], dim=-1). 
+00016d40: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+00016d50: 5f73 6861 7065 203d 2069 6e70 7574 5f69  _shape = input_i
+00016d60: 6473 2e73 697a 6528 290a 0a20 2020 2020  ds.size()..     
+00016d70: 2020 2020 2020 2023 2050 6164 2070 6f73         # Pad pos
+00016d80: 6974 696f 6e20 6964 7320 6966 2067 6976  ition ids if giv
+00016d90: 656e 0a20 2020 2020 2020 2020 2020 2069  en.            i
+00016da0: 6620 706f 7369 7469 6f6e 5f69 6473 2069  f position_ids i
+00016db0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00016dc0: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+00016dd0: 6564 5f70 6f73 6974 696f 6e5f 6964 7320  ed_position_ids 
+00016de0: 3d20 746f 7263 682e 6172 616e 6765 2869  = torch.arange(i
+00016df0: 6e70 7574 5f73 6861 7065 5b2d 315d 2c20  nput_shape[-1], 
+00016e00: 7061 6464 6564 5f73 6571 5f6c 656e 6774  padded_seq_lengt
+00016e10: 682c 2064 7479 7065 3d74 6f72 6368 2e6c  h, dtype=torch.l
+00016e20: 6f6e 672c 2064 6576 6963 653d 6465 7669  ong, device=devi
+00016e30: 6365 290a 2020 2020 2020 2020 2020 2020  ce).            
+00016e40: 2020 2020 7061 6464 6564 5f70 6f73 6974      padded_posit
+00016e50: 696f 6e5f 6964 7320 3d20 706f 7369 7469  ion_ids = positi
+00016e60: 6f6e 5f69 6473 2e75 6e73 7175 6565 7a65  on_ids.unsqueeze
+00016e70: 2830 292e 6578 7061 6e64 2869 6e70 7574  (0).expand(input
+00016e80: 5f73 6861 7065 5b30 5d2c 2070 6164 6469  _shape[0], paddi
+00016e90: 6e67 5f6c 656e 6774 6829 0a20 2020 2020  ng_length).     
+00016ea0: 2020 2020 2020 2020 2020 2070 6f73 6974             posit
+00016eb0: 696f 6e5f 6964 7320 3d20 746f 7263 682e  ion_ids = torch.
+00016ec0: 6361 7428 5b70 6f73 6974 696f 6e5f 6964  cat([position_id
+00016ed0: 732c 2070 6164 6465 645f 706f 7369 7469  s, padded_positi
+00016ee0: 6f6e 5f69 6473 5d2c 2064 696d 3d2d 3129  on_ids], dim=-1)
+00016ef0: 0a0a 2020 2020 2020 2020 2320 4578 7465  ..        # Exte
+00016f00: 6e64 2060 696e 7075 7473 5f65 6d62 6564  nd `inputs_embed
+00016f10: 7360 2077 6974 6820 7061 6464 696e 6720  s` with padding 
+00016f20: 746f 206d 6174 6368 206c 6561 7374 2063  to match least c
+00016f30: 6f6d 6d6f 6e20 6d75 6c74 6970 6c65 2063  ommon multiple c
+00016f40: 6875 6e6b 5f6c 656e 6774 680a 2020 2020  hunk_length.    
+00016f50: 2020 2020 6966 2069 6e70 7574 735f 656d      if inputs_em
+00016f60: 6265 6473 2069 7320 6e6f 7420 4e6f 6e65  beds is not None
+00016f70: 3a0a 2020 2020 2020 2020 2020 2020 7061  :.            pa
+00016f80: 6464 6564 5f69 6e70 7574 735f 656d 6265  dded_inputs_embe
+00016f90: 6473 203d 2073 656c 662e 656d 6265 6464  ds = self.embedd
+00016fa0: 696e 6773 2870 6164 6465 645f 696e 7075  ings(padded_inpu
+00016fb0: 745f 6964 732c 2070 6f73 6974 696f 6e5f  t_ids, position_
+00016fc0: 6964 7329 0a20 2020 2020 2020 2020 2020  ids).           
+00016fd0: 2069 6e70 7574 735f 656d 6265 6473 203d   inputs_embeds =
+00016fe0: 2074 6f72 6368 2e63 6174 285b 696e 7075   torch.cat([inpu
+00016ff0: 7473 5f65 6d62 6564 732c 2070 6164 6465  ts_embeds, padde
+00017000: 645f 696e 7075 7473 5f65 6d62 6564 735d  d_inputs_embeds]
+00017010: 2c20 6469 6d3d 2d32 290a 2020 2020 2020  , dim=-2).      
+00017020: 2020 2020 2020 696e 7075 745f 7368 6170        input_shap
+00017030: 6520 3d20 696e 7075 7473 5f65 6d62 6564  e = inputs_embed
+00017040: 732e 7369 7a65 2829 0a20 2020 2020 2020  s.size().       
+00017050: 2072 6574 7572 6e20 696e 7075 745f 6964   return input_id
+00017060: 732c 2069 6e70 7574 735f 656d 6265 6473  s, inputs_embeds
+00017070: 2c20 6174 7465 6e74 696f 6e5f 6d61 736b  , attention_mask
+00017080: 2c20 706f 7369 7469 6f6e 5f69 6473 2c20  , position_ids, 
+00017090: 696e 7075 745f 7368 6170 650a 0a0a 4061  input_shape...@a
+000170a0: 6464 5f73 7461 7274 5f64 6f63 7374 7269  dd_start_docstri
+000170b0: 6e67 7328 2222 2252 6566 6f72 6d65 7220  ngs("""Reformer 
+000170c0: 4d6f 6465 6c20 7769 7468 2061 2060 6c61  Model with a `la
+000170d0: 6e67 7561 6765 206d 6f64 656c 696e 6760  nguage modeling`
+000170e0: 2068 6561 6420 6f6e 2074 6f70 2e20 2222   head on top. ""
+000170f0: 222c 2052 4546 4f52 4d45 525f 5354 4152  ", REFORMER_STAR
+00017100: 545f 444f 4353 5452 494e 4729 0a63 6c61  T_DOCSTRING).cla
+00017110: 7373 2052 6566 6f72 6d65 724d 6f64 656c  ss ReformerModel
+00017120: 5769 7468 4c4d 4865 6164 2852 6566 6f72  WithLMHead(Refor
+00017130: 6d65 7250 7265 5472 6169 6e65 644d 6f64  merPreTrainedMod
+00017140: 656c 293a 0a20 2020 2064 6566 205f 5f69  el):.    def __i
+00017150: 6e69 745f 5f28 7365 6c66 2c20 636f 6e66  nit__(self, conf
+00017160: 6967 293a 0a20 2020 2020 2020 2073 7570  ig):.        sup
+00017170: 6572 2829 2e5f 5f69 6e69 745f 5f28 636f  er().__init__(co
+00017180: 6e66 6967 290a 2020 2020 2020 2020 6173  nfig).        as
+00017190: 7365 7274 2063 6f6e 6669 672e 6973 5f64  sert config.is_d
+000171a0: 6563 6f64 6572 2c20 2249 6620 796f 7520  ecoder, "If you 
+000171b0: 7761 6e74 2074 6f20 7573 6520 6052 6566  want to use `Ref
+000171c0: 6f72 6d65 724d 6f64 656c 5769 7468 4c4d  ormerModelWithLM
+000171d0: 4865 6164 6020 6d61 6b65 2073 7572 6520  Head` make sure 
+000171e0: 7468 6174 2060 6973 5f64 6563 6f64 6572  that `is_decoder
+000171f0: 3d54 7275 6560 2e22 0a20 2020 2020 2020  =True`.".       
+00017200: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+00017210: 2020 2020 2020 226c 6f63 616c 2220 6e6f        "local" no
+00017220: 7420 696e 2073 656c 662e 636f 6e66 6967  t in self.config
+00017230: 2e61 7474 6e5f 6c61 7965 7273 206f 7220  .attn_layers or 
+00017240: 636f 6e66 6967 2e6c 6f63 616c 5f6e 756d  config.local_num
+00017250: 5f63 6875 6e6b 735f 6166 7465 7220 3d3d  _chunks_after ==
+00017260: 2030 0a20 2020 2020 2020 2029 2c20 6622   0.        ), f"
+00017270: 4966 2063 6175 7361 6c20 6d61 736b 2069  If causal mask i
+00017280: 7320 656e 6162 6c65 642c 206d 616b 6520  s enabled, make 
+00017290: 7375 7265 2074 6861 7420 6063 6f6e 6669  sure that `confi
+000172a0: 672e 6c6f 6361 6c5f 6e75 6d5f 6368 756e  g.local_num_chun
+000172b0: 6b73 5f61 6674 6572 6020 6973 2073 6574  ks_after` is set
+000172c0: 2074 6f20 3020 616e 6420 6e6f 7420 7b63   to 0 and not {c
+000172d0: 6f6e 6669 672e 6c6f 6361 6c5f 6e75 6d5f  onfig.local_num_
+000172e0: 6368 756e 6b73 5f61 6674 6572 7d2e 220a  chunks_after}.".
+000172f0: 2020 2020 2020 2020 6173 7365 7274 2028          assert (
+00017300: 0a20 2020 2020 2020 2020 2020 2022 6c73  .            "ls
+00017310: 6822 206e 6f74 2069 6e20 7365 6c66 2e63  h" not in self.c
+00017320: 6f6e 6669 672e 6174 746e 5f6c 6179 6572  onfig.attn_layer
+00017330: 7320 6f72 2063 6f6e 6669 672e 6c73 685f  s or config.lsh_
+00017340: 6e75 6d5f 6368 756e 6b73 5f61 6674 6572  num_chunks_after
+00017350: 203d 3d20 300a 2020 2020 2020 2020 292c   == 0.        ),
+00017360: 2066 2249 6620 6361 7573 616c 206d 6173   f"If causal mas
+00017370: 6b20 6973 2065 6e61 626c 6564 2c20 6d61  k is enabled, ma
+00017380: 6b65 2073 7572 6520 7468 6174 2060 636f  ke sure that `co
+00017390: 6e66 6967 2e6c 7368 5f6e 756d 5f63 6875  nfig.lsh_num_chu
+000173a0: 6e6b 735f 6166 7465 7260 2069 7320 7365  nks_after` is se
+000173b0: 7420 746f 2031 2061 6e64 206e 6f74 207b  t to 1 and not {
+000173c0: 636f 6e66 6967 2e6c 7368 5f6e 756d 5f63  config.lsh_num_c
+000173d0: 6875 6e6b 735f 6166 7465 727d 2e22 0a0a  hunks_after}."..
+000173e0: 2020 2020 2020 2020 7365 6c66 2e72 6566          self.ref
+000173f0: 6f72 6d65 7220 3d20 5265 666f 726d 6572  ormer = Reformer
+00017400: 4d6f 6465 6c28 636f 6e66 6967 290a 2020  Model(config).  
+00017410: 2020 2020 2020 7365 6c66 2e6c 6d5f 6865        self.lm_he
+00017420: 6164 203d 2052 6566 6f72 6d65 724f 6e6c  ad = ReformerOnl
+00017430: 794c 4d48 6561 6428 636f 6e66 6967 290a  yLMHead(config).
+00017440: 0a20 2020 2020 2020 2073 656c 662e 696e  .        self.in
+00017450: 6974 5f77 6569 6768 7473 2829 0a0a 2020  it_weights()..  
+00017460: 2020 6465 6620 6765 745f 6f75 7470 7574    def get_output
+00017470: 5f65 6d62 6564 6469 6e67 7328 7365 6c66  _embeddings(self
+00017480: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00017490: 6e20 7365 6c66 2e6c 6d5f 6865 6164 2e64  n self.lm_head.d
+000174a0: 6563 6f64 6572 0a0a 2020 2020 6465 6620  ecoder..    def 
+000174b0: 7365 745f 6f75 7470 7574 5f65 6d62 6564  set_output_embed
+000174c0: 6469 6e67 7328 7365 6c66 2c20 6e65 775f  dings(self, new_
+000174d0: 656d 6265 6464 696e 6773 293a 0a20 2020  embeddings):.   
+000174e0: 2020 2020 2073 656c 662e 6c6d 5f68 6561       self.lm_hea
+000174f0: 642e 6465 636f 6465 7220 3d20 6e65 775f  d.decoder = new_
+00017500: 656d 6265 6464 696e 6773 0a0a 2020 2020  embeddings..    
+00017510: 4061 6464 5f73 7461 7274 5f64 6f63 7374  @add_start_docst
+00017520: 7269 6e67 735f 746f 5f6d 6f64 656c 5f66  rings_to_model_f
+00017530: 6f72 7761 7264 2852 4546 4f52 4d45 525f  orward(REFORMER_
+00017540: 494e 5055 5453 5f44 4f43 5354 5249 4e47  INPUTS_DOCSTRING
+00017550: 290a 2020 2020 4061 6464 5f63 6f64 655f  ).    @add_code_
+00017560: 7361 6d70 6c65 5f64 6f63 7374 7269 6e67  sample_docstring
+00017570: 7328 0a20 2020 2020 2020 2074 6f6b 656e  s(.        token
+00017580: 697a 6572 5f63 6c61 7373 3d5f 544f 4b45  izer_class=_TOKE
+00017590: 4e49 5a45 525f 464f 525f 444f 432c 0a20  NIZER_FOR_DOC,. 
+000175a0: 2020 2020 2020 2063 6865 636b 706f 696e         checkpoin
+000175b0: 743d 5f43 4845 434b 504f 494e 545f 464f  t=_CHECKPOINT_FO
+000175c0: 525f 444f 432c 0a20 2020 2020 2020 206f  R_DOC,.        o
+000175d0: 7574 7075 745f 7479 7065 3d43 6175 7361  utput_type=Causa
+000175e0: 6c4c 4d4f 7574 7075 742c 0a20 2020 2020  lLMOutput,.     
+000175f0: 2020 2063 6f6e 6669 675f 636c 6173 733d     config_class=
+00017600: 5f43 4f4e 4649 475f 464f 525f 444f 432c  _CONFIG_FOR_DOC,
+00017610: 0a20 2020 2029 0a20 2020 2064 6566 2066  .    ).    def f
+00017620: 6f72 7761 7264 280a 2020 2020 2020 2020  orward(.        
+00017630: 7365 6c66 2c0a 2020 2020 2020 2020 696e  self,.        in
+00017640: 7075 745f 6964 733d 4e6f 6e65 2c0a 2020  put_ids=None,.  
+00017650: 2020 2020 2020 706f 7369 7469 6f6e 5f69        position_i
+00017660: 6473 3d4e 6f6e 652c 0a20 2020 2020 2020  ds=None,.       
+00017670: 2061 7474 656e 7469 6f6e 5f6d 6173 6b3d   attention_mask=
+00017680: 4e6f 6e65 2c0a 2020 2020 2020 2020 6865  None,.        he
+00017690: 6164 5f6d 6173 6b3d 4e6f 6e65 2c0a 2020  ad_mask=None,.  
+000176a0: 2020 2020 2020 696e 7075 7473 5f65 6d62        inputs_emb
+000176b0: 6564 733d 4e6f 6e65 2c0a 2020 2020 2020  eds=None,.      
+000176c0: 2020 6e75 6d5f 6861 7368 6573 3d4e 6f6e    num_hashes=Non
+000176d0: 652c 0a20 2020 2020 2020 2070 6173 745f  e,.        past_
+000176e0: 6275 636b 6574 735f 7374 6174 6573 3d4e  buckets_states=N
+000176f0: 6f6e 652c 0a20 2020 2020 2020 2075 7365  one,.        use
+00017700: 5f63 6163 6865 3d4e 6f6e 652c 0a20 2020  _cache=None,.   
+00017710: 2020 2020 206f 7574 7075 745f 6869 6464       output_hidd
+00017720: 656e 5f73 7461 7465 733d 4e6f 6e65 2c0a  en_states=None,.
+00017730: 2020 2020 2020 2020 6f75 7470 7574 5f61          output_a
+00017740: 7474 656e 7469 6f6e 733d 4e6f 6e65 2c0a  ttentions=None,.
+00017750: 2020 2020 2020 2020 7265 7475 726e 5f64          return_d
+00017760: 6963 743d 4e6f 6e65 2c0a 2020 2020 2020  ict=None,.      
+00017770: 2020 6c61 6265 6c73 3d4e 6f6e 652c 0a20    labels=None,. 
+00017780: 2020 2029 3a0a 2020 2020 2020 2020 7222     ):.        r"
+00017790: 2222 0a20 2020 2020 2020 206c 6162 656c  "".        label
+000177a0: 7320 283a 6f62 6a3a 6074 6f72 6368 2e4c  s (:obj:`torch.L
+000177b0: 6f6e 6754 656e 736f 7260 206f 6620 7368  ongTensor` of sh
+000177c0: 6170 6520 3a6f 626a 3a60 2862 6174 6368  ape :obj:`(batch
+000177d0: 5f73 697a 652c 2960 2c20 606f 7074 696f  _size,)`, `optio
+000177e0: 6e61 6c60 293a 0a20 2020 2020 2020 2020  nal`):.         
+000177f0: 2020 2020 2020 204c 6162 656c 7320 666f         Labels fo
+00017800: 7220 636f 6d70 7574 696e 6720 7468 6520  r computing the 
+00017810: 7365 7175 656e 6365 2063 6c61 7373 6966  sequence classif
+00017820: 6963 6174 696f 6e2f 7265 6772 6573 7369  ication/regressi
+00017830: 6f6e 206c 6f73 732e 2049 6e64 6963 6573  on loss. Indices
+00017840: 2073 686f 756c 6420 6265 2069 6e20 3a6f   should be in :o
+00017850: 626a 3a60 5b2d 3130 302c 2030 2c0a 2020  bj:`[-100, 0,.  
+00017860: 2020 2020 2020 2020 2020 2020 2020 2e2e                ..
+00017870: 2e2c 2063 6f6e 6669 672e 766f 6361 625f  ., config.vocab_
+00017880: 7369 7a65 202d 2031 5d60 2e20 416c 6c20  size - 1]`. All 
+00017890: 6c61 6265 6c73 2073 6574 2074 6f20 6060  labels set to ``
+000178a0: 2d31 3030 6060 2061 7265 2069 676e 6f72  -100`` are ignor
+000178b0: 6564 2028 6d61 736b 6564 292c 2074 6865  ed (masked), the
+000178c0: 206c 6f73 7320 6973 206f 6e6c 790a 2020   loss is only.  
+000178d0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000178e0: 6d70 7574 6564 2066 6f72 206c 6162 656c  mputed for label
+000178f0: 7320 696e 2060 605b 302c 202e 2e2e 2c20  s in ``[0, ..., 
+00017900: 636f 6e66 6967 2e76 6f63 6162 5f73 697a  config.vocab_siz
+00017910: 655d 6060 0a20 2020 2020 2020 2022 2222  e]``.        """
+00017920: 0a20 2020 2020 2020 2072 6574 7572 6e5f  .        return_
+00017930: 6469 6374 203d 2072 6574 7572 6e5f 6469  dict = return_di
+00017940: 6374 2069 6620 7265 7475 726e 5f64 6963  ct if return_dic
+00017950: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
+00017960: 7365 2073 656c 662e 636f 6e66 6967 2e75  se self.config.u
+00017970: 7365 5f72 6574 7572 6e5f 6469 6374 0a0a  se_return_dict..
+00017980: 2020 2020 2020 2020 7265 666f 726d 6572          reformer
+00017990: 5f6f 7574 7075 7473 203d 2073 656c 662e  _outputs = self.
+000179a0: 7265 666f 726d 6572 280a 2020 2020 2020  reformer(.      
+000179b0: 2020 2020 2020 696e 7075 745f 6964 732c        input_ids,
+000179c0: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
+000179d0: 6974 696f 6e5f 6964 733d 706f 7369 7469  ition_ids=positi
+000179e0: 6f6e 5f69 6473 2c0a 2020 2020 2020 2020  on_ids,.        
+000179f0: 2020 2020 6174 7465 6e74 696f 6e5f 6d61      attention_ma
+00017a00: 736b 3d61 7474 656e 7469 6f6e 5f6d 6173  sk=attention_mas
+00017a10: 6b2c 0a20 2020 2020 2020 2020 2020 2068  k,.            h
+00017a20: 6561 645f 6d61 736b 3d68 6561 645f 6d61  ead_mask=head_ma
+00017a30: 736b 2c0a 2020 2020 2020 2020 2020 2020  sk,.            
+00017a40: 696e 7075 7473 5f65 6d62 6564 733d 696e  inputs_embeds=in
+00017a50: 7075 7473 5f65 6d62 6564 732c 0a20 2020  puts_embeds,.   
+00017a60: 2020 2020 2020 2020 206e 756d 5f68 6173           num_has
+00017a70: 6865 733d 6e75 6d5f 6861 7368 6573 2c0a  hes=num_hashes,.
+00017a80: 2020 2020 2020 2020 2020 2020 7061 7374              past
+00017a90: 5f62 7563 6b65 7473 5f73 7461 7465 733d  _buckets_states=
+00017aa0: 7061 7374 5f62 7563 6b65 7473 5f73 7461  past_buckets_sta
+00017ab0: 7465 732c 0a20 2020 2020 2020 2020 2020  tes,.           
+00017ac0: 2075 7365 5f63 6163 6865 3d75 7365 5f63   use_cache=use_c
+00017ad0: 6163 6865 2c0a 2020 2020 2020 2020 2020  ache,.          
+00017ae0: 2020 6f75 7470 7574 5f68 6964 6465 6e5f    output_hidden_
+00017af0: 7374 6174 6573 3d6f 7574 7075 745f 6869  states=output_hi
+00017b00: 6464 656e 5f73 7461 7465 732c 0a20 2020  dden_states,.   
+00017b10: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+00017b20: 6174 7465 6e74 696f 6e73 3d6f 7574 7075  attentions=outpu
+00017b30: 745f 6174 7465 6e74 696f 6e73 2c0a 2020  t_attentions,.  
+00017b40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00017b50: 5f64 6963 743d 7265 7475 726e 5f64 6963  _dict=return_dic
+00017b60: 742c 0a20 2020 2020 2020 2029 0a0a 2020  t,.        )..  
+00017b70: 2020 2020 2020 7365 7175 656e 6365 5f6f        sequence_o
+00017b80: 7574 7075 7420 3d20 7265 666f 726d 6572  utput = reformer
+00017b90: 5f6f 7574 7075 7473 5b30 5d0a 2020 2020  _outputs[0].    
+00017ba0: 2020 2020 6c6f 6769 7473 203d 2073 656c      logits = sel
+00017bb0: 662e 6c6d 5f68 6561 6428 7365 7175 656e  f.lm_head(sequen
+00017bc0: 6365 5f6f 7574 7075 7429 0a0a 2020 2020  ce_output)..    
+00017bd0: 2020 2020 6c6f 7373 203d 204e 6f6e 650a      loss = None.
+00017be0: 2020 2020 2020 2020 6966 206c 6162 656c          if label
+00017bf0: 7320 6973 206e 6f74 204e 6f6e 653a 0a20  s is not None:. 
+00017c00: 2020 2020 2020 2020 2020 2023 2053 6869             # Shi
+00017c10: 6674 2073 6f20 7468 6174 2074 6f6b 656e  ft so that token
+00017c20: 7320 3c20 6e20 7072 6564 6963 7420 6e0a  s < n predict n.
+00017c30: 2020 2020 2020 2020 2020 2020 7368 6966              shif
+00017c40: 745f 6c6f 6769 7473 203d 206c 6f67 6974  t_logits = logit
+00017c50: 735b 2e2e 2e2c 203a 2d31 2c20 3a5d 2e63  s[..., :-1, :].c
+00017c60: 6f6e 7469 6775 6f75 7328 290a 2020 2020  ontiguous().    
+00017c70: 2020 2020 2020 2020 7368 6966 745f 6c61          shift_la
+00017c80: 6265 6c73 203d 206c 6162 656c 735b 2e2e  bels = labels[..
+00017c90: 2e2c 2031 3a5d 2e63 6f6e 7469 6775 6f75  ., 1:].contiguou
+00017ca0: 7328 290a 2020 2020 2020 2020 2020 2020  s().            
+00017cb0: 2320 466c 6174 7465 6e20 7468 6520 746f  # Flatten the to
+00017cc0: 6b65 6e73 0a20 2020 2020 2020 2020 2020  kens.           
+00017cd0: 206c 6f73 735f 6663 7420 3d20 4372 6f73   loss_fct = Cros
+00017ce0: 7345 6e74 726f 7079 4c6f 7373 2829 0a20  sEntropyLoss(). 
+00017cf0: 2020 2020 2020 2020 2020 206c 6f73 7320             loss 
+00017d00: 3d20 6c6f 7373 5f66 6374 2873 6869 6674  = loss_fct(shift
+00017d10: 5f6c 6f67 6974 732e 7669 6577 282d 312c  _logits.view(-1,
+00017d20: 2073 656c 662e 636f 6e66 6967 2e76 6f63   self.config.voc
+00017d30: 6162 5f73 697a 6529 2c20 7368 6966 745f  ab_size), shift_
+00017d40: 6c61 6265 6c73 2e76 6965 7728 2d31 2929  labels.view(-1))
+00017d50: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+00017d60: 2072 6574 7572 6e5f 6469 6374 3a0a 2020   return_dict:.  
+00017d70: 2020 2020 2020 2020 2020 6f75 7470 7574            output
+00017d80: 203d 2028 6c6f 6769 7473 2c29 202b 2072   = (logits,) + r
+00017d90: 6566 6f72 6d65 725f 6f75 7470 7574 735b  eformer_outputs[
+00017da0: 313a 5d0a 2020 2020 2020 2020 2020 2020  1:].            
+00017db0: 7265 7475 726e 2028 286c 6f73 732c 2920  return ((loss,) 
+00017dc0: 2b20 6f75 7470 7574 2920 6966 206c 6f73  + output) if los
+00017dd0: 7320 6973 206e 6f74 204e 6f6e 6520 656c  s is not None el
+00017de0: 7365 206f 7574 7075 740a 0a20 2020 2020  se output..     
+00017df0: 2020 2072 6574 7572 6e20 5265 666f 726d     return Reform
+00017e00: 6572 4d6f 6465 6c57 6974 684c 4d48 6561  erModelWithLMHea
+00017e10: 644f 7574 7075 7428 0a20 2020 2020 2020  dOutput(.       
+00017e20: 2020 2020 206c 6f73 733d 6c6f 7373 2c0a       loss=loss,.
+00017e30: 2020 2020 2020 2020 2020 2020 6c6f 6769              logi
+00017e40: 7473 3d6c 6f67 6974 732c 0a20 2020 2020  ts=logits,.     
+00017e50: 2020 2020 2020 2070 6173 745f 6275 636b         past_buck
+00017e60: 6574 735f 7374 6174 6573 3d72 6566 6f72  ets_states=refor
+00017e70: 6d65 725f 6f75 7470 7574 732e 7061 7374  mer_outputs.past
+00017e80: 5f62 7563 6b65 7473 5f73 7461 7465 732c  _buckets_states,
+00017e90: 0a20 2020 2020 2020 2020 2020 2068 6964  .            hid
+00017ea0: 6465 6e5f 7374 6174 6573 3d72 6566 6f72  den_states=refor
+00017eb0: 6d65 725f 6f75 7470 7574 732e 6869 6464  mer_outputs.hidd
+00017ec0: 656e 5f73 7461 7465 732c 0a20 2020 2020  en_states,.     
+00017ed0: 2020 2020 2020 2061 7474 656e 7469 6f6e         attention
+00017ee0: 733d 7265 666f 726d 6572 5f6f 7574 7075  s=reformer_outpu
+00017ef0: 7473 2e61 7474 656e 7469 6f6e 732c 0a20  ts.attentions,. 
+00017f00: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00017f10: 6620 7072 6570 6172 655f 696e 7075 7473  f prepare_inputs
+00017f20: 5f66 6f72 5f67 656e 6572 6174 696f 6e28  _for_generation(
+00017f30: 7365 6c66 2c20 696e 7075 745f 6964 732c  self, input_ids,
+00017f40: 2070 6173 743d 4e6f 6e65 2c20 7573 655f   past=None, use_
+00017f50: 6361 6368 653d 4e6f 6e65 2c20 6e75 6d5f  cache=None, num_
+00017f60: 6861 7368 6573 3d4e 6f6e 652c 202a 2a6b  hashes=None, **k
+00017f70: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00017f80: 2320 6f6e 6c79 206c 6173 7420 746f 6b65  # only last toke
+00017f90: 6e20 666f 7220 696e 7075 7473 5f69 6473  n for inputs_ids
+00017fa0: 2069 6620 7061 7374 2069 7320 6465 6669   if past is defi
+00017fb0: 6e65 6420 696e 206b 7761 7267 730a 2020  ned in kwargs.  
+00017fc0: 2020 2020 2020 6966 2070 6173 7420 6973        if past is
+00017fd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
+00017fe0: 2020 2020 2020 2069 6e70 7574 5f69 6473         input_ids
+00017ff0: 203d 2069 6e70 7574 5f69 6473 5b3a 2c20   = input_ids[:, 
+00018000: 2d31 3a5d 0a0a 2020 2020 2020 2020 696e  -1:]..        in
+00018010: 7075 7473 5f64 6963 7420 3d20 7b0a 2020  puts_dict = {.  
+00018020: 2020 2020 2020 2020 2020 2269 6e70 7574            "input
+00018030: 5f69 6473 223a 2069 6e70 7574 5f69 6473  _ids": input_ids
+00018040: 2c0a 2020 2020 2020 2020 2020 2020 2270  ,.            "p
+00018050: 6173 745f 6275 636b 6574 735f 7374 6174  ast_buckets_stat
+00018060: 6573 223a 2070 6173 742c 0a20 2020 2020  es": past,.     
+00018070: 2020 2020 2020 2022 7573 655f 6361 6368         "use_cach
+00018080: 6522 3a20 7573 655f 6361 6368 652c 0a20  e": use_cache,. 
+00018090: 2020 2020 2020 2020 2020 2022 6e75 6d5f             "num_
+000180a0: 6861 7368 6573 223a 206e 756d 5f68 6173  hashes": num_has
+000180b0: 6865 732c 0a20 2020 2020 2020 207d 0a0a  hes,.        }..
+000180c0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
+000180d0: 6e70 7574 735f 6469 6374 0a0a 2020 2020  nputs_dict..    
+000180e0: 6465 6620 5f72 656f 7264 6572 5f63 6163  def _reorder_cac
+000180f0: 6865 2873 656c 662c 2070 6173 742c 2062  he(self, past, b
+00018100: 6561 6d5f 6964 7829 3a0a 2020 2020 2020  eam_idx):.      
+00018110: 2020 7265 6f72 645f 7061 7374 5f62 7563    reord_past_buc
+00018120: 6b65 7473 5f73 7461 7465 7320 3d20 5b5d  kets_states = []
+00018130: 0a20 2020 2020 2020 2066 6f72 206c 6179  .        for lay
+00018140: 6572 5f70 6173 7420 696e 2070 6173 743a  er_past in past:
+00018150: 0a20 2020 2020 2020 2020 2020 2023 2062  .            # b
+00018160: 7563 6b65 7473 0a20 2020 2020 2020 2020  uckets.         
+00018170: 2020 2069 6620 6c61 7965 725f 7061 7374     if layer_past
+00018180: 5b30 5d20 6973 206e 6f74 204e 6f6e 653a  [0] is not None:
+00018190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000181a0: 2072 656f 7264 5f62 7563 6b65 7473 203d   reord_buckets =
+000181b0: 206c 6179 6572 5f70 6173 745b 305d 2e69   layer_past[0].i
+000181c0: 6e64 6578 5f73 656c 6563 7428 302c 2062  ndex_select(0, b
+000181d0: 6561 6d5f 6964 7829 0a20 2020 2020 2020  eam_idx).       
+000181e0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000181f0: 2020 2020 2020 2020 2020 2072 656f 7264             reord
+00018200: 5f62 7563 6b65 7473 203d 204e 6f6e 650a  _buckets = None.
+00018210: 0a20 2020 2020 2020 2020 2020 2023 2068  .            # h
+00018220: 6964 6465 6e20 7374 6174 6573 0a20 2020  idden states.   
+00018230: 2020 2020 2020 2020 2072 656f 7264 5f68           reord_h
+00018240: 6964 6465 6e5f 7374 6174 6573 203d 206c  idden_states = l
+00018250: 6179 6572 5f70 6173 745b 315d 2e69 6e64  ayer_past[1].ind
+00018260: 6578 5f73 656c 6563 7428 302c 2062 6561  ex_select(0, bea
+00018270: 6d5f 6964 7829 0a20 2020 2020 2020 2020  m_idx).         
+00018280: 2020 2072 656f 7264 5f70 6173 745f 6275     reord_past_bu
+00018290: 636b 6574 735f 7374 6174 6573 2e61 7070  ckets_states.app
+000182a0: 656e 6428 2872 656f 7264 5f62 7563 6b65  end((reord_bucke
+000182b0: 7473 2c20 7265 6f72 645f 6869 6464 656e  ts, reord_hidden
+000182c0: 5f73 7461 7465 7329 290a 2020 2020 2020  _states)).      
+000182d0: 2020 7265 7475 726e 2072 656f 7264 5f70    return reord_p
+000182e0: 6173 745f 6275 636b 6574 735f 7374 6174  ast_buckets_stat
+000182f0: 6573 0a0a 0a40 6164 645f 7374 6172 745f  es...@add_start_
+00018300: 646f 6373 7472 696e 6773 2822 2222 5265  docstrings("""Re
+00018310: 666f 726d 6572 204d 6f64 656c 2077 6974  former Model wit
+00018320: 6820 6120 606c 616e 6775 6167 6520 6d6f  h a `language mo
+00018330: 6465 6c69 6e67 6020 6865 6164 206f 6e20  deling` head on 
+00018340: 746f 702e 2022 2222 2c20 5245 464f 524d  top. """, REFORM
+00018350: 4552 5f53 5441 5254 5f44 4f43 5354 5249  ER_START_DOCSTRI
+00018360: 4e47 290a 636c 6173 7320 5265 666f 726d  NG).class Reform
+00018370: 6572 466f 724d 6173 6b65 644c 4d28 5265  erForMaskedLM(Re
+00018380: 666f 726d 6572 5072 6554 7261 696e 6564  formerPreTrained
+00018390: 4d6f 6465 6c29 3a0a 2020 2020 6465 6620  Model):.    def 
+000183a0: 5f5f 696e 6974 5f5f 2873 656c 662c 2063  __init__(self, c
+000183b0: 6f6e 6669 6729 3a0a 2020 2020 2020 2020  onfig):.        
+000183c0: 7375 7065 7228 292e 5f5f 696e 6974 5f5f  super().__init__
+000183d0: 2863 6f6e 6669 6729 0a20 2020 2020 2020  (config).       
+000183e0: 2061 7373 6572 7420 280a 2020 2020 2020   assert (.      
+000183f0: 2020 2020 2020 6e6f 7420 636f 6e66 6967        not config
+00018400: 2e69 735f 6465 636f 6465 720a 2020 2020  .is_decoder.    
+00018410: 2020 2020 292c 2022 4966 2079 6f75 2077      ), "If you w
+00018420: 616e 7420 746f 2075 7365 2060 5265 666f  ant to use `Refo
+00018430: 726d 6572 466f 724d 6173 6b65 644c 4d60  rmerForMaskedLM`
+00018440: 206d 616b 6520 7375 7265 2060 636f 6e66   make sure `conf
+00018450: 6967 2e69 735f 6465 636f 6465 723d 4661  ig.is_decoder=Fa
+00018460: 6c73 6560 2066 6f72 2062 692d 6469 7265  lse` for bi-dire
+00018470: 6374 696f 6e61 6c20 7365 6c66 2d61 7474  ctional self-att
+00018480: 656e 7469 6f6e 2e22 0a20 2020 2020 2020  ention.".       
+00018490: 2073 656c 662e 7265 666f 726d 6572 203d   self.reformer =
+000184a0: 2052 6566 6f72 6d65 724d 6f64 656c 2863   ReformerModel(c
+000184b0: 6f6e 6669 6729 0a20 2020 2020 2020 2073  onfig).        s
+000184c0: 656c 662e 6c6d 5f68 6561 6420 3d20 5265  elf.lm_head = Re
+000184d0: 666f 726d 6572 4f6e 6c79 4c4d 4865 6164  formerOnlyLMHead
+000184e0: 2863 6f6e 6669 6729 0a0a 2020 2020 2020  (config)..      
+000184f0: 2020 7365 6c66 2e69 6e69 745f 7765 6967    self.init_weig
+00018500: 6874 7328 290a 0a20 2020 2064 6566 2067  hts()..    def g
+00018510: 6574 5f6f 7574 7075 745f 656d 6265 6464  et_output_embedd
+00018520: 696e 6773 2873 656c 6629 3a0a 2020 2020  ings(self):.    
+00018530: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00018540: 6c6d 5f68 6561 642e 6465 636f 6465 720a  lm_head.decoder.
+00018550: 0a20 2020 2064 6566 2073 6574 5f6f 7574  .    def set_out
+00018560: 7075 745f 656d 6265 6464 696e 6773 2873  put_embeddings(s
+00018570: 656c 662c 206e 6577 5f65 6d62 6564 6469  elf, new_embeddi
+00018580: 6e67 7329 3a0a 2020 2020 2020 2020 7365  ngs):.        se
+00018590: 6c66 2e6c 6d5f 6865 6164 2e64 6563 6f64  lf.lm_head.decod
+000185a0: 6572 203d 206e 6577 5f65 6d62 6564 6469  er = new_embeddi
+000185b0: 6e67 730a 0a20 2020 2040 6164 645f 7374  ngs..    @add_st
+000185c0: 6172 745f 646f 6373 7472 696e 6773 5f74  art_docstrings_t
+000185d0: 6f5f 6d6f 6465 6c5f 666f 7277 6172 6428  o_model_forward(
+000185e0: 5245 464f 524d 4552 5f49 4e50 5554 535f  REFORMER_INPUTS_
+000185f0: 444f 4353 5452 494e 4729 0a20 2020 2040  DOCSTRING).    @
+00018600: 6164 645f 636f 6465 5f73 616d 706c 655f  add_code_sample_
+00018610: 646f 6373 7472 696e 6773 280a 2020 2020  docstrings(.    
+00018620: 2020 2020 746f 6b65 6e69 7a65 725f 636c      tokenizer_cl
+00018630: 6173 733d 5f54 4f4b 454e 495a 4552 5f46  ass=_TOKENIZER_F
+00018640: 4f52 5f44 4f43 2c0a 2020 2020 2020 2020  OR_DOC,.        
+00018650: 6368 6563 6b70 6f69 6e74 3d5f 4348 4543  checkpoint=_CHEC
+00018660: 4b50 4f49 4e54 5f46 4f52 5f44 4f43 2c0a  KPOINT_FOR_DOC,.
+00018670: 2020 2020 2020 2020 6f75 7470 7574 5f74          output_t
+00018680: 7970 653d 4d61 736b 6564 4c4d 4f75 7470  ype=MaskedLMOutp
+00018690: 7574 2c0a 2020 2020 2020 2020 636f 6e66  ut,.        conf
+000186a0: 6967 5f63 6c61 7373 3d5f 434f 4e46 4947  ig_class=_CONFIG
+000186b0: 5f46 4f52 5f44 4f43 2c0a 2020 2020 290a  _FOR_DOC,.    ).
+000186c0: 2020 2020 6465 6620 666f 7277 6172 6428      def forward(
+000186d0: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+000186e0: 2020 2020 2020 2069 6e70 7574 5f69 6473         input_ids
+000186f0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2070  =None,.        p
+00018700: 6f73 6974 696f 6e5f 6964 733d 4e6f 6e65  osition_ids=None
+00018710: 2c0a 2020 2020 2020 2020 6174 7465 6e74  ,.        attent
+00018720: 696f 6e5f 6d61 736b 3d4e 6f6e 652c 0a20  ion_mask=None,. 
+00018730: 2020 2020 2020 2068 6561 645f 6d61 736b         head_mask
+00018740: 3d4e 6f6e 652c 0a20 2020 2020 2020 2069  =None,.        i
+00018750: 6e70 7574 735f 656d 6265 6473 3d4e 6f6e  nputs_embeds=Non
+00018760: 652c 0a20 2020 2020 2020 206e 756d 5f68  e,.        num_h
+00018770: 6173 6865 733d 4e6f 6e65 2c0a 2020 2020  ashes=None,.    
+00018780: 2020 2020 6c61 6265 6c73 3d4e 6f6e 652c      labels=None,
+00018790: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+000187a0: 6869 6464 656e 5f73 7461 7465 733d 4e6f  hidden_states=No
+000187b0: 6e65 2c0a 2020 2020 2020 2020 6f75 7470  ne,.        outp
+000187c0: 7574 5f61 7474 656e 7469 6f6e 733d 4e6f  ut_attentions=No
+000187d0: 6e65 2c0a 2020 2020 2020 2020 7265 7475  ne,.        retu
+000187e0: 726e 5f64 6963 743d 4e6f 6e65 2c0a 2020  rn_dict=None,.  
+000187f0: 2020 293a 0a20 2020 2020 2020 2072 2222    ):.        r""
+00018800: 220a 2020 2020 2020 2020 6c61 6265 6c73  ".        labels
+00018810: 2028 3a6f 626a 3a60 746f 7263 682e 4c6f   (:obj:`torch.Lo
+00018820: 6e67 5465 6e73 6f72 6020 6f66 2073 6861  ngTensor` of sha
+00018830: 7065 203a 6f62 6a3a 6028 6261 7463 685f  pe :obj:`(batch_
+00018840: 7369 7a65 2c20 7365 7175 656e 6365 5f6c  size, sequence_l
+00018850: 656e 6774 6829 602c 2060 6f70 7469 6f6e  ength)`, `option
+00018860: 616c 6029 3a0a 2020 2020 2020 2020 2020  al`):.          
+00018870: 2020 2020 2020 4c61 6265 6c73 2066 6f72        Labels for
+00018880: 2063 6f6d 7075 7469 6e67 2074 6865 206d   computing the m
+00018890: 6173 6b65 6420 6c61 6e67 7561 6765 206d  asked language m
+000188a0: 6f64 656c 696e 6720 6c6f 7373 2e20 496e  odeling loss. In
+000188b0: 6469 6365 7320 7368 6f75 6c64 2062 6520  dices should be 
+000188c0: 696e 2060 605b 2d31 3030 2c20 302c 202e  in ``[-100, 0, .
+000188d0: 2e2e 2c0a 2020 2020 2020 2020 2020 2020  ..,.            
+000188e0: 2020 2020 636f 6e66 6967 2e76 6f63 6162      config.vocab
+000188f0: 5f73 697a 655d 6060 2028 7365 6520 6060  _size]`` (see ``
+00018900: 696e 7075 745f 6964 7360 6020 646f 6373  input_ids`` docs
+00018910: 7472 696e 6729 2054 6f6b 656e 7320 7769  tring) Tokens wi
+00018920: 7468 2069 6e64 6963 6573 2073 6574 2074  th indices set t
+00018930: 6f20 6060 2d31 3030 6060 2061 7265 2069  o ``-100`` are i
+00018940: 676e 6f72 6564 0a20 2020 2020 2020 2020  gnored.         
+00018950: 2020 2020 2020 2028 6d61 736b 6564 292c         (masked),
+00018960: 2074 6865 206c 6f73 7320 6973 206f 6e6c   the loss is onl
+00018970: 7920 636f 6d70 7574 6564 2066 6f72 2074  y computed for t
+00018980: 6865 2074 6f6b 656e 7320 7769 7468 206c  he tokens with l
+00018990: 6162 656c 730a 2020 2020 2020 2020 2222  abels.        ""
+000189a0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000189b0: 5f64 6963 7420 3d20 7265 7475 726e 5f64  _dict = return_d
+000189c0: 6963 7420 6966 2072 6574 7572 6e5f 6469  ict if return_di
+000189d0: 6374 2069 7320 6e6f 7420 4e6f 6e65 2065  ct is not None e
+000189e0: 6c73 6520 7365 6c66 2e63 6f6e 6669 672e  lse self.config.
+000189f0: 7573 655f 7265 7475 726e 5f64 6963 740a  use_return_dict.
+00018a00: 0a20 2020 2020 2020 2072 6566 6f72 6d65  .        reforme
+00018a10: 725f 6f75 7470 7574 7320 3d20 7365 6c66  r_outputs = self
+00018a20: 2e72 6566 6f72 6d65 7228 0a20 2020 2020  .reformer(.     
+00018a30: 2020 2020 2020 2069 6e70 7574 5f69 6473         input_ids
+00018a40: 2c0a 2020 2020 2020 2020 2020 2020 706f  ,.            po
+00018a50: 7369 7469 6f6e 5f69 6473 3d70 6f73 6974  sition_ids=posit
+00018a60: 696f 6e5f 6964 732c 0a20 2020 2020 2020  ion_ids,.       
+00018a70: 2020 2020 2061 7474 656e 7469 6f6e 5f6d       attention_m
+00018a80: 6173 6b3d 6174 7465 6e74 696f 6e5f 6d61  ask=attention_ma
+00018a90: 736b 2c0a 2020 2020 2020 2020 2020 2020  sk,.            
+00018aa0: 6865 6164 5f6d 6173 6b3d 6865 6164 5f6d  head_mask=head_m
+00018ab0: 6173 6b2c 0a20 2020 2020 2020 2020 2020  ask,.           
+00018ac0: 2069 6e70 7574 735f 656d 6265 6473 3d69   inputs_embeds=i
+00018ad0: 6e70 7574 735f 656d 6265 6473 2c0a 2020  nputs_embeds,.  
+00018ae0: 2020 2020 2020 2020 2020 6e75 6d5f 6861            num_ha
+00018af0: 7368 6573 3d6e 756d 5f68 6173 6865 732c  shes=num_hashes,
+00018b00: 0a20 2020 2020 2020 2020 2020 2075 7365  .            use
+00018b10: 5f63 6163 6865 3d46 616c 7365 2c20 2023  _cache=False,  #
+00018b20: 206e 6f20 6361 7573 616c 206d 6173 6b0a   no causal mask.
+00018b30: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00018b40: 7574 5f68 6964 6465 6e5f 7374 6174 6573  ut_hidden_states
+00018b50: 3d6f 7574 7075 745f 6869 6464 656e 5f73  =output_hidden_s
+00018b60: 7461 7465 732c 0a20 2020 2020 2020 2020  tates,.         
+00018b70: 2020 206f 7574 7075 745f 6174 7465 6e74     output_attent
+00018b80: 696f 6e73 3d6f 7574 7075 745f 6174 7465  ions=output_atte
+00018b90: 6e74 696f 6e73 2c0a 2020 2020 2020 2020  ntions,.        
+00018ba0: 2020 2020 7265 7475 726e 5f64 6963 743d      return_dict=
+00018bb0: 7265 7475 726e 5f64 6963 742c 0a20 2020  return_dict,.   
+00018bc0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00018bd0: 7365 7175 656e 6365 5f6f 7574 7075 7420  sequence_output 
+00018be0: 3d20 7265 666f 726d 6572 5f6f 7574 7075  = reformer_outpu
+00018bf0: 7473 5b30 5d0a 2020 2020 2020 2020 6c6f  ts[0].        lo
+00018c00: 6769 7473 203d 2073 656c 662e 6c6d 5f68  gits = self.lm_h
+00018c10: 6561 6428 7365 7175 656e 6365 5f6f 7574  ead(sequence_out
+00018c20: 7075 7429 0a0a 2020 2020 2020 2020 6d61  put)..        ma
+00018c30: 736b 6564 5f6c 6d5f 6c6f 7373 203d 204e  sked_lm_loss = N
+00018c40: 6f6e 650a 2020 2020 2020 2020 6966 206c  one.        if l
+00018c50: 6162 656c 7320 6973 206e 6f74 204e 6f6e  abels is not Non
+00018c60: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
+00018c70: 6f73 735f 6663 7420 3d20 4372 6f73 7345  oss_fct = CrossE
+00018c80: 6e74 726f 7079 4c6f 7373 2829 2020 2320  ntropyLoss()  # 
+00018c90: 2d31 3030 2069 6e64 6578 203d 2070 6164  -100 index = pad
+00018ca0: 6469 6e67 2074 6f6b 656e 0a20 2020 2020  ding token.     
+00018cb0: 2020 2020 2020 206d 6173 6b65 645f 6c6d         masked_lm
+00018cc0: 5f6c 6f73 7320 3d20 6c6f 7373 5f66 6374  _loss = loss_fct
+00018cd0: 286c 6f67 6974 732e 7669 6577 282d 312c  (logits.view(-1,
+00018ce0: 2073 656c 662e 636f 6e66 6967 2e76 6f63   self.config.voc
+00018cf0: 6162 5f73 697a 6529 2c20 6c61 6265 6c73  ab_size), labels
+00018d00: 2e76 6965 7728 2d31 2929 0a0a 2020 2020  .view(-1))..    
+00018d10: 2020 2020 6966 206e 6f74 2072 6574 7572      if not retur
+00018d20: 6e5f 6469 6374 3a0a 2020 2020 2020 2020  n_dict:.        
+00018d30: 2020 2020 6f75 7470 7574 203d 2028 6c6f      output = (lo
+00018d40: 6769 7473 2c29 202b 2072 6566 6f72 6d65  gits,) + reforme
+00018d50: 725f 6f75 7470 7574 735b 313a 5d0a 2020  r_outputs[1:].  
+00018d60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00018d70: 2028 286d 6173 6b65 645f 6c6d 5f6c 6f73   ((masked_lm_los
+00018d80: 732c 2920 2b20 6f75 7470 7574 2920 6966  s,) + output) if
+00018d90: 206d 6173 6b65 645f 6c6d 5f6c 6f73 7320   masked_lm_loss 
+00018da0: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
+00018db0: 206f 7574 7075 740a 0a20 2020 2020 2020   output..       
+00018dc0: 2072 6574 7572 6e20 4d61 736b 6564 4c4d   return MaskedLM
+00018dd0: 4f75 7470 7574 280a 2020 2020 2020 2020  Output(.        
+00018de0: 2020 2020 6c6f 7373 3d6d 6173 6b65 645f      loss=masked_
+00018df0: 6c6d 5f6c 6f73 732c 0a20 2020 2020 2020  lm_loss,.       
+00018e00: 2020 2020 206c 6f67 6974 733d 6c6f 6769       logits=logi
+00018e10: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+00018e20: 6869 6464 656e 5f73 7461 7465 733d 7265  hidden_states=re
+00018e30: 666f 726d 6572 5f6f 7574 7075 7473 2e68  former_outputs.h
+00018e40: 6964 6465 6e5f 7374 6174 6573 2c0a 2020  idden_states,.  
+00018e50: 2020 2020 2020 2020 2020 6174 7465 6e74            attent
+00018e60: 696f 6e73 3d72 6566 6f72 6d65 725f 6f75  ions=reformer_ou
+00018e70: 7470 7574 732e 6174 7465 6e74 696f 6e73  tputs.attentions
+00018e80: 2c0a 2020 2020 2020 2020 290a 0a0a 4061  ,.        )...@a
+00018e90: 6464 5f73 7461 7274 5f64 6f63 7374 7269  dd_start_docstri
+00018ea0: 6e67 7328 0a20 2020 2022 2222 0a20 2020  ngs(.    """.   
+00018eb0: 2052 6566 6f72 6d65 7220 4d6f 6465 6c20   Reformer Model 
+00018ec0: 7472 616e 7366 6f72 6d65 7220 7769 7468  transformer with
+00018ed0: 2061 2073 6571 7565 6e63 6520 636c 6173   a sequence clas
+00018ee0: 7369 6669 6361 7469 6f6e 2f72 6567 7265  sification/regre
+00018ef0: 7373 696f 6e20 6865 6164 206f 6e20 746f  ssion head on to
+00018f00: 7020 2861 206c 696e 6561 7220 6c61 7965  p (a linear laye
+00018f10: 7220 6f6e 2074 6f70 206f 6620 7468 650a  r on top of the.
+00018f20: 2020 2020 706f 6f6c 6564 206f 7574 7075      pooled outpu
+00018f30: 7429 2065 2e67 2e20 666f 7220 474c 5545  t) e.g. for GLUE
+00018f40: 2074 6173 6b73 2e0a 2020 2020 2222 222c   tasks..    """,
+00018f50: 0a20 2020 2052 4546 4f52 4d45 525f 5354  .    REFORMER_ST
+00018f60: 4152 545f 444f 4353 5452 494e 472c 0a29  ART_DOCSTRING,.)
+00018f70: 0a63 6c61 7373 2052 6566 6f72 6d65 7246  .class ReformerF
+00018f80: 6f72 5365 7175 656e 6365 436c 6173 7369  orSequenceClassi
+00018f90: 6669 6361 7469 6f6e 2852 6566 6f72 6d65  fication(Reforme
+00018fa0: 7250 7265 5472 6169 6e65 644d 6f64 656c  rPreTrainedModel
+00018fb0: 293a 0a20 2020 2064 6566 205f 5f69 6e69  ):.    def __ini
+00018fc0: 745f 5f28 7365 6c66 2c20 636f 6e66 6967  t__(self, config
+00018fd0: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
+00018fe0: 2829 2e5f 5f69 6e69 745f 5f28 636f 6e66  ().__init__(conf
+00018ff0: 6967 290a 2020 2020 2020 2020 7365 6c66  ig).        self
+00019000: 2e6e 756d 5f6c 6162 656c 7320 3d20 636f  .num_labels = co
+00019010: 6e66 6967 2e6e 756d 5f6c 6162 656c 730a  nfig.num_labels.
+00019020: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00019030: 6669 6720 3d20 636f 6e66 6967 0a0a 2020  fig = config..  
+00019040: 2020 2020 2020 7365 6c66 2e72 6566 6f72        self.refor
+00019050: 6d65 7220 3d20 5265 666f 726d 6572 4d6f  mer = ReformerMo
+00019060: 6465 6c28 636f 6e66 6967 290a 2020 2020  del(config).    
+00019070: 2020 2020 7365 6c66 2e63 6c61 7373 6966      self.classif
+00019080: 6965 7220 3d20 5265 666f 726d 6572 436c  ier = ReformerCl
+00019090: 6173 7369 6669 6361 7469 6f6e 4865 6164  assificationHead
+000190a0: 2863 6f6e 6669 6729 0a20 2020 2020 2020  (config).       
+000190b0: 2069 6620 636f 6e66 6967 2e69 735f 6465   if config.is_de
+000190c0: 636f 6465 7220 6973 2054 7275 653a 0a20  coder is True:. 
+000190d0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+000190e0: 722e 7761 726e 696e 6728 2259 6f75 206d  r.warning("You m
+000190f0: 6967 6874 2077 616e 7420 746f 2064 6973  ight want to dis
+00019100: 6162 6c65 2063 6175 7361 6c20 6d61 736b  able causal mask
+00019110: 696e 6720 666f 7220 7365 7175 656e 6365  ing for sequence
+00019120: 2063 6c61 7373 6966 6963 6174 696f 6e22   classification"
+00019130: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00019140: 696e 6974 5f77 6569 6768 7473 2829 0a0a  init_weights()..
+00019150: 2020 2020 4061 6464 5f73 7461 7274 5f64      @add_start_d
+00019160: 6f63 7374 7269 6e67 735f 746f 5f6d 6f64  ocstrings_to_mod
+00019170: 656c 5f66 6f72 7761 7264 2852 4546 4f52  el_forward(REFOR
+00019180: 4d45 525f 494e 5055 5453 5f44 4f43 5354  MER_INPUTS_DOCST
+00019190: 5249 4e47 290a 2020 2020 4061 6464 5f63  RING).    @add_c
+000191a0: 6f64 655f 7361 6d70 6c65 5f64 6f63 7374  ode_sample_docst
+000191b0: 7269 6e67 7328 0a20 2020 2020 2020 2074  rings(.        t
+000191c0: 6f6b 656e 697a 6572 5f63 6c61 7373 3d5f  okenizer_class=_
+000191d0: 544f 4b45 4e49 5a45 525f 464f 525f 444f  TOKENIZER_FOR_DO
+000191e0: 432c 0a20 2020 2020 2020 2063 6865 636b  C,.        check
+000191f0: 706f 696e 743d 5f43 4845 434b 504f 494e  point=_CHECKPOIN
+00019200: 545f 464f 525f 444f 432c 0a20 2020 2020  T_FOR_DOC,.     
+00019210: 2020 206f 7574 7075 745f 7479 7065 3d53     output_type=S
+00019220: 6571 7565 6e63 6543 6c61 7373 6966 6965  equenceClassifie
+00019230: 724f 7574 7075 742c 0a20 2020 2020 2020  rOutput,.       
+00019240: 2063 6f6e 6669 675f 636c 6173 733d 5f43   config_class=_C
+00019250: 4f4e 4649 475f 464f 525f 444f 432c 0a20  ONFIG_FOR_DOC,. 
+00019260: 2020 2029 0a20 2020 2064 6566 2066 6f72     ).    def for
+00019270: 7761 7264 280a 2020 2020 2020 2020 7365  ward(.        se
+00019280: 6c66 2c0a 2020 2020 2020 2020 696e 7075  lf,.        inpu
+00019290: 745f 6964 733d 4e6f 6e65 2c0a 2020 2020  t_ids=None,.    
+000192a0: 2020 2020 706f 7369 7469 6f6e 5f69 6473      position_ids
+000192b0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2061  =None,.        a
+000192c0: 7474 656e 7469 6f6e 5f6d 6173 6b3d 4e6f  ttention_mask=No
+000192d0: 6e65 2c0a 2020 2020 2020 2020 6865 6164  ne,.        head
+000192e0: 5f6d 6173 6b3d 4e6f 6e65 2c0a 2020 2020  _mask=None,.    
+000192f0: 2020 2020 696e 7075 7473 5f65 6d62 6564      inputs_embed
 00019300: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00019310: 6f75 7470 7574 5f68 6964 6465 6e5f 7374  output_hidden_st
-00019320: 6174 6573 3d4e 6f6e 652c 0a20 2020 2020  ates=None,.     
-00019330: 2020 206f 7574 7075 745f 6174 7465 6e74     output_attent
-00019340: 696f 6e73 3d4e 6f6e 652c 0a20 2020 2020  ions=None,.     
-00019350: 2020 2072 6574 7572 6e5f 6469 6374 3d4e     return_dict=N
-00019360: 6f6e 652c 0a20 2020 2029 3a0a 2020 2020  one,.    ):.    
-00019370: 2020 2020 7222 2222 0a20 2020 2020 2020      r""".       
-00019380: 206c 6162 656c 7320 283a 6f62 6a3a 6074   labels (:obj:`t
-00019390: 6f72 6368 2e4c 6f6e 6754 656e 736f 7260  orch.LongTensor`
-000193a0: 206f 6620 7368 6170 6520 3a6f 626a 3a60   of shape :obj:`
-000193b0: 2862 6174 6368 5f73 697a 652c 2960 2c20  (batch_size,)`, 
-000193c0: 606f 7074 696f 6e61 6c60 293a 0a20 2020  `optional`):.   
-000193d0: 2020 2020 2020 2020 204c 6162 656c 7320           Labels 
-000193e0: 666f 7220 636f 6d70 7574 696e 6720 7468  for computing th
-000193f0: 6520 7365 7175 656e 6365 2063 6c61 7373  e sequence class
-00019400: 6966 6963 6174 696f 6e2f 7265 6772 6573  ification/regres
-00019410: 7369 6f6e 206c 6f73 732e 2049 6e64 6963  sion loss. Indic
-00019420: 6573 2073 686f 756c 6420 6265 2069 6e20  es should be in 
-00019430: 3a6f 626a 3a60 5b30 2c20 2e2e 2e2c 0a20  :obj:`[0, ...,. 
-00019440: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
-00019450: 672e 6e75 6d5f 6c61 6265 6c73 202d 2031  g.num_labels - 1
-00019460: 5d60 2e20 4966 203a 6f62 6a3a 6063 6f6e  ]`. If :obj:`con
-00019470: 6669 672e 6e75 6d5f 6c61 6265 6c73 203d  fig.num_labels =
-00019480: 3d20 3160 2061 2072 6567 7265 7373 696f  = 1` a regressio
-00019490: 6e20 6c6f 7373 2069 7320 636f 6d70 7574  n loss is comput
-000194a0: 6564 2028 4d65 616e 2d53 7175 6172 6520  ed (Mean-Square 
-000194b0: 6c6f 7373 292c 0a20 2020 2020 2020 2020  loss),.         
-000194c0: 2020 2049 6620 3a6f 626a 3a60 636f 6e66     If :obj:`conf
-000194d0: 6967 2e6e 756d 5f6c 6162 656c 7320 3e20  ig.num_labels > 
-000194e0: 3160 2061 2063 6c61 7373 6966 6963 6174  1` a classificat
-000194f0: 696f 6e20 6c6f 7373 2069 7320 636f 6d70  ion loss is comp
-00019500: 7574 6564 2028 4372 6f73 732d 456e 7472  uted (Cross-Entr
-00019510: 6f70 7929 2e0a 2020 2020 2020 2020 2222  opy)..        ""
-00019520: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00019530: 5f64 6963 7420 3d20 7265 7475 726e 5f64  _dict = return_d
-00019540: 6963 7420 6966 2072 6574 7572 6e5f 6469  ict if return_di
-00019550: 6374 2069 7320 6e6f 7420 4e6f 6e65 2065  ct is not None e
-00019560: 6c73 6520 7365 6c66 2e63 6f6e 6669 672e  lse self.config.
-00019570: 7573 655f 7265 7475 726e 5f64 6963 740a  use_return_dict.
-00019580: 0a20 2020 2020 2020 206f 7574 7075 7473  .        outputs
-00019590: 203d 2073 656c 662e 7265 666f 726d 6572   = self.reformer
-000195a0: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-000195b0: 7075 745f 6964 732c 0a20 2020 2020 2020  put_ids,.       
-000195c0: 2020 2020 2070 6f73 6974 696f 6e5f 6964       position_id
-000195d0: 733d 706f 7369 7469 6f6e 5f69 6473 2c0a  s=position_ids,.
-000195e0: 2020 2020 2020 2020 2020 2020 6174 7465              atte
-000195f0: 6e74 696f 6e5f 6d61 736b 3d61 7474 656e  ntion_mask=atten
-00019600: 7469 6f6e 5f6d 6173 6b2c 0a20 2020 2020  tion_mask,.     
-00019610: 2020 2020 2020 2068 6561 645f 6d61 736b         head_mask
-00019620: 3d68 6561 645f 6d61 736b 2c0a 2020 2020  =head_mask,.    
-00019630: 2020 2020 2020 2020 696e 7075 7473 5f65          inputs_e
-00019640: 6d62 6564 733d 696e 7075 7473 5f65 6d62  mbeds=inputs_emb
-00019650: 6564 732c 0a20 2020 2020 2020 2020 2020  eds,.           
-00019660: 206e 756d 5f68 6173 6865 733d 6e75 6d5f   num_hashes=num_
-00019670: 6861 7368 6573 2c0a 2020 2020 2020 2020  hashes,.        
-00019680: 2020 2020 6f75 7470 7574 5f68 6964 6465      output_hidde
-00019690: 6e5f 7374 6174 6573 3d6f 7574 7075 745f  n_states=output_
-000196a0: 6869 6464 656e 5f73 7461 7465 732c 0a20  hidden_states,. 
-000196b0: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
-000196c0: 745f 6174 7465 6e74 696f 6e73 3d6f 7574  t_attentions=out
-000196d0: 7075 745f 6174 7465 6e74 696f 6e73 2c0a  put_attentions,.
-000196e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000196f0: 726e 5f64 6963 743d 7265 7475 726e 5f64  rn_dict=return_d
-00019700: 6963 742c 0a20 2020 2020 2020 2029 0a0a  ict,.        )..
-00019710: 2020 2020 2020 2020 7365 7175 656e 6365          sequence
-00019720: 5f6f 7574 7075 7420 3d20 6f75 7470 7574  _output = output
-00019730: 735b 305d 0a20 2020 2020 2020 206c 6f67  s[0].        log
-00019740: 6974 7320 3d20 7365 6c66 2e63 6c61 7373  its = self.class
-00019750: 6966 6965 7228 7365 7175 656e 6365 5f6f  ifier(sequence_o
-00019760: 7574 7075 7429 0a0a 2020 2020 2020 2020  utput)..        
-00019770: 6c6f 7373 203d 204e 6f6e 650a 2020 2020  loss = None.    
-00019780: 2020 2020 6966 206c 6162 656c 7320 6973      if labels is
-00019790: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000197a0: 2020 2020 2020 2069 6620 7365 6c66 2e63         if self.c
-000197b0: 6f6e 6669 672e 7072 6f62 6c65 6d5f 7479  onfig.problem_ty
-000197c0: 7065 2069 7320 4e6f 6e65 3a0a 2020 2020  pe is None:.    
-000197d0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-000197e0: 656c 662e 6e75 6d5f 6c61 6265 6c73 203d  elf.num_labels =
-000197f0: 3d20 313a 0a20 2020 2020 2020 2020 2020  = 1:.           
-00019800: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-00019810: 6e66 6967 2e70 726f 626c 656d 5f74 7970  nfig.problem_typ
-00019820: 6520 3d20 2272 6567 7265 7373 696f 6e22  e = "regression"
-00019830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019840: 2065 6c69 6620 7365 6c66 2e6e 756d 5f6c   elif self.num_l
-00019850: 6162 656c 7320 3e20 3120 616e 6420 286c  abels > 1 and (l
-00019860: 6162 656c 732e 6474 7970 6520 3d3d 2074  abels.dtype == t
-00019870: 6f72 6368 2e6c 6f6e 6720 6f72 206c 6162  orch.long or lab
-00019880: 656c 732e 6474 7970 6520 3d3d 2074 6f72  els.dtype == tor
-00019890: 6368 2e69 6e74 293a 0a20 2020 2020 2020  ch.int):.       
-000198a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000198b0: 662e 636f 6e66 6967 2e70 726f 626c 656d  f.config.problem
-000198c0: 5f74 7970 6520 3d20 2273 696e 676c 655f  _type = "single_
-000198d0: 6c61 6265 6c5f 636c 6173 7369 6669 6361  label_classifica
-000198e0: 7469 6f6e 220a 2020 2020 2020 2020 2020  tion".          
-000198f0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00019900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019910: 7365 6c66 2e63 6f6e 6669 672e 7072 6f62  self.config.prob
-00019920: 6c65 6d5f 7479 7065 203d 2022 6d75 6c74  lem_type = "mult
-00019930: 695f 6c61 6265 6c5f 636c 6173 7369 6669  i_label_classifi
-00019940: 6361 7469 6f6e 220a 0a20 2020 2020 2020  cation"..       
-00019950: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
-00019960: 6669 672e 7072 6f62 6c65 6d5f 7479 7065  fig.problem_type
-00019970: 203d 3d20 2272 6567 7265 7373 696f 6e22   == "regression"
-00019980: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00019990: 2020 6c6f 7373 5f66 6374 203d 204d 5345    loss_fct = MSE
-000199a0: 4c6f 7373 2829 0a20 2020 2020 2020 2020  Loss().         
-000199b0: 2020 2020 2020 2069 6620 7365 6c66 2e6e         if self.n
-000199c0: 756d 5f6c 6162 656c 7320 3d3d 2031 3a0a  um_labels == 1:.
-000199d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000199e0: 2020 2020 6c6f 7373 203d 206c 6f73 735f      loss = loss_
-000199f0: 6663 7428 6c6f 6769 7473 2e73 7175 6565  fct(logits.squee
-00019a00: 7a65 2829 2c20 6c61 6265 6c73 2e73 7175  ze(), labels.squ
-00019a10: 6565 7a65 2829 290a 2020 2020 2020 2020  eeze()).        
-00019a20: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00019a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019a40: 2020 6c6f 7373 203d 206c 6f73 735f 6663    loss = loss_fc
-00019a50: 7428 6c6f 6769 7473 2c20 6c61 6265 6c73  t(logits, labels
-00019a60: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-00019a70: 6966 2073 656c 662e 636f 6e66 6967 2e70  if self.config.p
-00019a80: 726f 626c 656d 5f74 7970 6520 3d3d 2022  roblem_type == "
-00019a90: 7369 6e67 6c65 5f6c 6162 656c 5f63 6c61  single_label_cla
-00019aa0: 7373 6966 6963 6174 696f 6e22 3a0a 2020  ssification":.  
-00019ab0: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00019ac0: 7373 5f66 6374 203d 2043 726f 7373 456e  ss_fct = CrossEn
-00019ad0: 7472 6f70 794c 6f73 7328 290a 2020 2020  tropyLoss().    
+00019310: 6e75 6d5f 6861 7368 6573 3d4e 6f6e 652c  num_hashes=None,
+00019320: 0a20 2020 2020 2020 206c 6162 656c 733d  .        labels=
+00019330: 4e6f 6e65 2c0a 2020 2020 2020 2020 6f75  None,.        ou
+00019340: 7470 7574 5f68 6964 6465 6e5f 7374 6174  tput_hidden_stat
+00019350: 6573 3d4e 6f6e 652c 0a20 2020 2020 2020  es=None,.       
+00019360: 206f 7574 7075 745f 6174 7465 6e74 696f   output_attentio
+00019370: 6e73 3d4e 6f6e 652c 0a20 2020 2020 2020  ns=None,.       
+00019380: 2072 6574 7572 6e5f 6469 6374 3d4e 6f6e   return_dict=Non
+00019390: 652c 0a20 2020 2029 3a0a 2020 2020 2020  e,.    ):.      
+000193a0: 2020 7222 2222 0a20 2020 2020 2020 206c    r""".        l
+000193b0: 6162 656c 7320 283a 6f62 6a3a 6074 6f72  abels (:obj:`tor
+000193c0: 6368 2e4c 6f6e 6754 656e 736f 7260 206f  ch.LongTensor` o
+000193d0: 6620 7368 6170 6520 3a6f 626a 3a60 2862  f shape :obj:`(b
+000193e0: 6174 6368 5f73 697a 652c 2960 2c20 606f  atch_size,)`, `o
+000193f0: 7074 696f 6e61 6c60 293a 0a20 2020 2020  ptional`):.     
+00019400: 2020 2020 2020 204c 6162 656c 7320 666f         Labels fo
+00019410: 7220 636f 6d70 7574 696e 6720 7468 6520  r computing the 
+00019420: 7365 7175 656e 6365 2063 6c61 7373 6966  sequence classif
+00019430: 6963 6174 696f 6e2f 7265 6772 6573 7369  ication/regressi
+00019440: 6f6e 206c 6f73 732e 2049 6e64 6963 6573  on loss. Indices
+00019450: 2073 686f 756c 6420 6265 2069 6e20 3a6f   should be in :o
+00019460: 626a 3a60 5b30 2c20 2e2e 2e2c 0a20 2020  bj:`[0, ...,.   
+00019470: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
+00019480: 6e75 6d5f 6c61 6265 6c73 202d 2031 5d60  num_labels - 1]`
+00019490: 2e20 4966 203a 6f62 6a3a 6063 6f6e 6669  . If :obj:`confi
+000194a0: 672e 6e75 6d5f 6c61 6265 6c73 203d 3d20  g.num_labels == 
+000194b0: 3160 2061 2072 6567 7265 7373 696f 6e20  1` a regression 
+000194c0: 6c6f 7373 2069 7320 636f 6d70 7574 6564  loss is computed
+000194d0: 2028 4d65 616e 2d53 7175 6172 6520 6c6f   (Mean-Square lo
+000194e0: 7373 292c 0a20 2020 2020 2020 2020 2020  ss),.           
+000194f0: 2049 6620 3a6f 626a 3a60 636f 6e66 6967   If :obj:`config
+00019500: 2e6e 756d 5f6c 6162 656c 7320 3e20 3160  .num_labels > 1`
+00019510: 2061 2063 6c61 7373 6966 6963 6174 696f   a classificatio
+00019520: 6e20 6c6f 7373 2069 7320 636f 6d70 7574  n loss is comput
+00019530: 6564 2028 4372 6f73 732d 456e 7472 6f70  ed (Cross-Entrop
+00019540: 7929 2e0a 2020 2020 2020 2020 2222 220a  y)..        """.
+00019550: 2020 2020 2020 2020 7265 7475 726e 5f64          return_d
+00019560: 6963 7420 3d20 7265 7475 726e 5f64 6963  ict = return_dic
+00019570: 7420 6966 2072 6574 7572 6e5f 6469 6374  t if return_dict
+00019580: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+00019590: 6520 7365 6c66 2e63 6f6e 6669 672e 7573  e self.config.us
+000195a0: 655f 7265 7475 726e 5f64 6963 740a 0a20  e_return_dict.. 
+000195b0: 2020 2020 2020 206f 7574 7075 7473 203d         outputs =
+000195c0: 2073 656c 662e 7265 666f 726d 6572 280a   self.reformer(.
+000195d0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+000195e0: 745f 6964 732c 0a20 2020 2020 2020 2020  t_ids,.         
+000195f0: 2020 2070 6f73 6974 696f 6e5f 6964 733d     position_ids=
+00019600: 706f 7369 7469 6f6e 5f69 6473 2c0a 2020  position_ids,.  
+00019610: 2020 2020 2020 2020 2020 6174 7465 6e74            attent
+00019620: 696f 6e5f 6d61 736b 3d61 7474 656e 7469  ion_mask=attenti
+00019630: 6f6e 5f6d 6173 6b2c 0a20 2020 2020 2020  on_mask,.       
+00019640: 2020 2020 2068 6561 645f 6d61 736b 3d68       head_mask=h
+00019650: 6561 645f 6d61 736b 2c0a 2020 2020 2020  ead_mask,.      
+00019660: 2020 2020 2020 696e 7075 7473 5f65 6d62        inputs_emb
+00019670: 6564 733d 696e 7075 7473 5f65 6d62 6564  eds=inputs_embed
+00019680: 732c 0a20 2020 2020 2020 2020 2020 206e  s,.            n
+00019690: 756d 5f68 6173 6865 733d 6e75 6d5f 6861  um_hashes=num_ha
+000196a0: 7368 6573 2c0a 2020 2020 2020 2020 2020  shes,.          
+000196b0: 2020 6f75 7470 7574 5f68 6964 6465 6e5f    output_hidden_
+000196c0: 7374 6174 6573 3d6f 7574 7075 745f 6869  states=output_hi
+000196d0: 6464 656e 5f73 7461 7465 732c 0a20 2020  dden_states,.   
+000196e0: 2020 2020 2020 2020 206f 7574 7075 745f           output_
+000196f0: 6174 7465 6e74 696f 6e73 3d6f 7574 7075  attentions=outpu
+00019700: 745f 6174 7465 6e74 696f 6e73 2c0a 2020  t_attentions,.  
+00019710: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00019720: 5f64 6963 743d 7265 7475 726e 5f64 6963  _dict=return_dic
+00019730: 742c 0a20 2020 2020 2020 2029 0a0a 2020  t,.        )..  
+00019740: 2020 2020 2020 7365 7175 656e 6365 5f6f        sequence_o
+00019750: 7574 7075 7420 3d20 6f75 7470 7574 735b  utput = outputs[
+00019760: 305d 0a20 2020 2020 2020 206c 6f67 6974  0].        logit
+00019770: 7320 3d20 7365 6c66 2e63 6c61 7373 6966  s = self.classif
+00019780: 6965 7228 7365 7175 656e 6365 5f6f 7574  ier(sequence_out
+00019790: 7075 7429 0a0a 2020 2020 2020 2020 6c6f  put)..        lo
+000197a0: 7373 203d 204e 6f6e 650a 2020 2020 2020  ss = None.      
+000197b0: 2020 6966 206c 6162 656c 7320 6973 206e    if labels is n
+000197c0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+000197d0: 2020 2020 2069 6620 7365 6c66 2e63 6f6e       if self.con
+000197e0: 6669 672e 7072 6f62 6c65 6d5f 7479 7065  fig.problem_type
+000197f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00019800: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00019810: 662e 6e75 6d5f 6c61 6265 6c73 203d 3d20  f.num_labels == 
+00019820: 313a 0a20 2020 2020 2020 2020 2020 2020  1:.             
+00019830: 2020 2020 2020 2073 656c 662e 636f 6e66         self.conf
+00019840: 6967 2e70 726f 626c 656d 5f74 7970 6520  ig.problem_type 
+00019850: 3d20 2272 6567 7265 7373 696f 6e22 0a20  = "regression". 
+00019860: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+00019870: 6c69 6620 7365 6c66 2e6e 756d 5f6c 6162  lif self.num_lab
+00019880: 656c 7320 3e20 3120 616e 6420 286c 6162  els > 1 and (lab
+00019890: 656c 732e 6474 7970 6520 3d3d 2074 6f72  els.dtype == tor
+000198a0: 6368 2e6c 6f6e 6720 6f72 206c 6162 656c  ch.long or label
+000198b0: 732e 6474 7970 6520 3d3d 2074 6f72 6368  s.dtype == torch
+000198c0: 2e69 6e74 293a 0a20 2020 2020 2020 2020  .int):.         
+000198d0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+000198e0: 636f 6e66 6967 2e70 726f 626c 656d 5f74  config.problem_t
+000198f0: 7970 6520 3d20 2273 696e 676c 655f 6c61  ype = "single_la
+00019900: 6265 6c5f 636c 6173 7369 6669 6361 7469  bel_classificati
+00019910: 6f6e 220a 2020 2020 2020 2020 2020 2020  on".            
+00019920: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00019930: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00019940: 6c66 2e63 6f6e 6669 672e 7072 6f62 6c65  lf.config.proble
+00019950: 6d5f 7479 7065 203d 2022 6d75 6c74 695f  m_type = "multi_
+00019960: 6c61 6265 6c5f 636c 6173 7369 6669 6361  label_classifica
+00019970: 7469 6f6e 220a 0a20 2020 2020 2020 2020  tion"..         
+00019980: 2020 2069 6620 7365 6c66 2e63 6f6e 6669     if self.confi
+00019990: 672e 7072 6f62 6c65 6d5f 7479 7065 203d  g.problem_type =
+000199a0: 3d20 2272 6567 7265 7373 696f 6e22 3a0a  = "regression":.
+000199b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000199c0: 6c6f 7373 5f66 6374 203d 204d 5345 4c6f  loss_fct = MSELo
+000199d0: 7373 2829 0a20 2020 2020 2020 2020 2020  ss().           
+000199e0: 2020 2020 2069 6620 7365 6c66 2e6e 756d       if self.num
+000199f0: 5f6c 6162 656c 7320 3d3d 2031 3a0a 2020  _labels == 1:.  
+00019a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a10: 2020 6c6f 7373 203d 206c 6f73 735f 6663    loss = loss_fc
+00019a20: 7428 6c6f 6769 7473 2e73 7175 6565 7a65  t(logits.squeeze
+00019a30: 2829 2c20 6c61 6265 6c73 2e73 7175 6565  (), labels.squee
+00019a40: 7a65 2829 290a 2020 2020 2020 2020 2020  ze()).          
+00019a50: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00019a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019a70: 6c6f 7373 203d 206c 6f73 735f 6663 7428  loss = loss_fct(
+00019a80: 6c6f 6769 7473 2c20 6c61 6265 6c73 290a  logits, labels).
+00019a90: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+00019aa0: 2073 656c 662e 636f 6e66 6967 2e70 726f   self.config.pro
+00019ab0: 626c 656d 5f74 7970 6520 3d3d 2022 7369  blem_type == "si
+00019ac0: 6e67 6c65 5f6c 6162 656c 5f63 6c61 7373  ngle_label_class
+00019ad0: 6966 6963 6174 696f 6e22 3a0a 2020 2020  ification":.    
 00019ae0: 2020 2020 2020 2020 2020 2020 6c6f 7373              loss
-00019af0: 203d 206c 6f73 735f 6663 7428 6c6f 6769   = loss_fct(logi
-00019b00: 7473 2e76 6965 7728 2d31 2c20 7365 6c66  ts.view(-1, self
-00019b10: 2e6e 756d 5f6c 6162 656c 7329 2c20 6c61  .num_labels), la
-00019b20: 6265 6c73 2e76 6965 7728 2d31 2929 0a20  bels.view(-1)). 
-00019b30: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-00019b40: 7365 6c66 2e63 6f6e 6669 672e 7072 6f62  self.config.prob
-00019b50: 6c65 6d5f 7479 7065 203d 3d20 226d 756c  lem_type == "mul
-00019b60: 7469 5f6c 6162 656c 5f63 6c61 7373 6966  ti_label_classif
-00019b70: 6963 6174 696f 6e22 3a0a 2020 2020 2020  ication":.      
-00019b80: 2020 2020 2020 2020 2020 6c6f 7373 5f66            loss_f
-00019b90: 6374 203d 2042 4345 5769 7468 4c6f 6769  ct = BCEWithLogi
-00019ba0: 7473 4c6f 7373 2829 0a20 2020 2020 2020  tsLoss().       
-00019bb0: 2020 2020 2020 2020 206c 6f73 7320 3d20           loss = 
-00019bc0: 6c6f 7373 5f66 6374 286c 6f67 6974 732c  loss_fct(logits,
-00019bd0: 206c 6162 656c 7329 0a0a 2020 2020 2020   labels)..      
-00019be0: 2020 6966 206e 6f74 2072 6574 7572 6e5f    if not return_
-00019bf0: 6469 6374 3a0a 2020 2020 2020 2020 2020  dict:.          
-00019c00: 2020 6f75 7470 7574 203d 2028 6c6f 6769    output = (logi
-00019c10: 7473 2c29 202b 206f 7574 7075 7473 5b32  ts,) + outputs[2
-00019c20: 3a5d 0a20 2020 2020 2020 2020 2020 2072  :].            r
-00019c30: 6574 7572 6e20 2828 6c6f 7373 2c29 202b  eturn ((loss,) +
-00019c40: 206f 7574 7075 7429 2069 6620 6c6f 7373   output) if loss
-00019c50: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
-00019c60: 6520 6f75 7470 7574 0a0a 2020 2020 2020  e output..      
-00019c70: 2020 7265 7475 726e 2053 6571 7565 6e63    return Sequenc
-00019c80: 6543 6c61 7373 6966 6965 724f 7574 7075  eClassifierOutpu
-00019c90: 7428 0a20 2020 2020 2020 2020 2020 206c  t(.            l
-00019ca0: 6f73 733d 6c6f 7373 2c0a 2020 2020 2020  oss=loss,.      
-00019cb0: 2020 2020 2020 6c6f 6769 7473 3d6c 6f67        logits=log
-00019cc0: 6974 732c 0a20 2020 2020 2020 2020 2020  its,.           
-00019cd0: 2068 6964 6465 6e5f 7374 6174 6573 3d6f   hidden_states=o
-00019ce0: 7574 7075 7473 2e68 6964 6465 6e5f 7374  utputs.hidden_st
-00019cf0: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
-00019d00: 2020 6174 7465 6e74 696f 6e73 3d6f 7574    attentions=out
-00019d10: 7075 7473 2e61 7474 656e 7469 6f6e 732c  puts.attentions,
-00019d20: 0a20 2020 2020 2020 2029 0a0a 0a63 6c61  .        )...cla
-00019d30: 7373 2052 6566 6f72 6d65 7243 6c61 7373  ss ReformerClass
-00019d40: 6966 6963 6174 696f 6e48 6561 6428 6e6e  ificationHead(nn
-00019d50: 2e4d 6f64 756c 6529 3a0a 2020 2020 2222  .Module):.    ""
-00019d60: 2248 6561 6420 666f 7220 7365 6e74 656e  "Head for senten
-00019d70: 6365 2d6c 6576 656c 2063 6c61 7373 6966  ce-level classif
-00019d80: 6963 6174 696f 6e20 7461 736b 732e 2222  ication tasks.""
-00019d90: 220a 0a20 2020 2064 6566 205f 5f69 6e69  "..    def __ini
-00019da0: 745f 5f28 7365 6c66 2c20 636f 6e66 6967  t__(self, config
-00019db0: 293a 0a20 2020 2020 2020 2073 7570 6572  ):.        super
-00019dc0: 2829 2e5f 5f69 6e69 745f 5f28 290a 2020  ().__init__().  
-00019dd0: 2020 2020 2020 7365 6c66 2e64 656e 7365        self.dense
-00019de0: 203d 206e 6e2e 4c69 6e65 6172 2832 202a   = nn.Linear(2 *
-00019df0: 2063 6f6e 6669 672e 6869 6464 656e 5f73   config.hidden_s
-00019e00: 697a 652c 2063 6f6e 6669 672e 6869 6464  ize, config.hidd
-00019e10: 656e 5f73 697a 6529 0a20 2020 2020 2020  en_size).       
-00019e20: 2073 656c 662e 6472 6f70 6f75 7420 3d20   self.dropout = 
-00019e30: 6e6e 2e44 726f 706f 7574 2863 6f6e 6669  nn.Dropout(confi
-00019e40: 672e 6869 6464 656e 5f64 726f 706f 7574  g.hidden_dropout
-00019e50: 5f70 726f 6229 0a20 2020 2020 2020 2073  _prob).        s
-00019e60: 656c 662e 6f75 745f 7072 6f6a 203d 206e  elf.out_proj = n
-00019e70: 6e2e 4c69 6e65 6172 2863 6f6e 6669 672e  n.Linear(config.
-00019e80: 6869 6464 656e 5f73 697a 652c 2063 6f6e  hidden_size, con
-00019e90: 6669 672e 6e75 6d5f 6c61 6265 6c73 290a  fig.num_labels).
-00019ea0: 0a20 2020 2064 6566 2066 6f72 7761 7264  .    def forward
-00019eb0: 2873 656c 662c 2068 6964 6465 6e5f 7374  (self, hidden_st
-00019ec0: 6174 6573 2c20 2a2a 6b77 6172 6773 293a  ates, **kwargs):
-00019ed0: 0a20 2020 2020 2020 2068 6964 6465 6e5f  .        hidden_
-00019ee0: 7374 6174 6573 203d 2068 6964 6465 6e5f  states = hidden_
-00019ef0: 7374 6174 6573 5b3a 2c20 302c 203a 5d20  states[:, 0, :] 
-00019f00: 2023 2074 616b 6520 3c73 3e20 746f 6b65   # take <s> toke
-00019f10: 6e20 2865 7175 6976 2e20 746f 205b 434c  n (equiv. to [CL
-00019f20: 535d 290a 2020 2020 2020 2020 6869 6464  S]).        hidd
-00019f30: 656e 5f73 7461 7465 7320 3d20 7365 6c66  en_states = self
-00019f40: 2e64 726f 706f 7574 2868 6964 6465 6e5f  .dropout(hidden_
-00019f50: 7374 6174 6573 290a 2020 2020 2020 2020  states).        
-00019f60: 6869 6464 656e 5f73 7461 7465 7320 3d20  hidden_states = 
-00019f70: 7365 6c66 2e64 656e 7365 2868 6964 6465  self.dense(hidde
-00019f80: 6e5f 7374 6174 6573 290a 2020 2020 2020  n_states).      
-00019f90: 2020 6869 6464 656e 5f73 7461 7465 7320    hidden_states 
-00019fa0: 3d20 746f 7263 682e 7461 6e68 2868 6964  = torch.tanh(hid
-00019fb0: 6465 6e5f 7374 6174 6573 290a 2020 2020  den_states).    
-00019fc0: 2020 2020 6869 6464 656e 5f73 7461 7465      hidden_state
-00019fd0: 7320 3d20 7365 6c66 2e64 726f 706f 7574  s = self.dropout
-00019fe0: 2868 6964 6465 6e5f 7374 6174 6573 290a  (hidden_states).
-00019ff0: 2020 2020 2020 2020 6869 6464 656e 5f73          hidden_s
-0001a000: 7461 7465 7320 3d20 7365 6c66 2e6f 7574  tates = self.out
-0001a010: 5f70 726f 6a28 6869 6464 656e 5f73 7461  _proj(hidden_sta
-0001a020: 7465 7329 0a20 2020 2020 2020 2072 6574  tes).        ret
-0001a030: 7572 6e20 6869 6464 656e 5f73 7461 7465  urn hidden_state
-0001a040: 730a 0a0a 4061 6464 5f73 7461 7274 5f64  s...@add_start_d
-0001a050: 6f63 7374 7269 6e67 7328 0a20 2020 2022  ocstrings(.    "
-0001a060: 2222 0a20 2020 2052 6566 6f72 6d65 7220  "".    Reformer 
-0001a070: 4d6f 6465 6c20 7769 7468 2061 2073 7061  Model with a spa
-0001a080: 6e20 636c 6173 7369 6669 6361 7469 6f6e  n classification
-0001a090: 2068 6561 6420 6f6e 2074 6f70 2066 6f72   head on top for
-0001a0a0: 2065 7874 7261 6374 6976 6520 7175 6573   extractive ques
-0001a0b0: 7469 6f6e 2d61 6e73 7765 7269 6e67 2074  tion-answering t
-0001a0c0: 6173 6b73 206c 696b 6520 5351 7541 4420  asks like SQuAD 
-0001a0d0: 2f20 5472 6976 6961 5141 0a20 2020 2028  / TriviaQA.    (
-0001a0e0: 2061 206c 696e 6561 7220 6c61 7965 7220   a linear layer 
-0001a0f0: 6f6e 2074 6f70 206f 6620 6869 6464 656e  on top of hidden
-0001a100: 2d73 7461 7465 7320 6f75 7470 7574 2074  -states output t
-0001a110: 6f20 636f 6d70 7574 6520 6073 7061 6e20  o compute `span 
-0001a120: 7374 6172 7420 6c6f 6769 7473 6020 616e  start logits` an
-0001a130: 6420 6073 7061 6e20 656e 6420 6c6f 6769  d `span end logi
-0001a140: 7473 602e 0a20 2020 2022 2222 2c0a 2020  ts`..    """,.  
-0001a150: 2020 5245 464f 524d 4552 5f53 5441 5254    REFORMER_START
-0001a160: 5f44 4f43 5354 5249 4e47 2c0a 290a 636c  _DOCSTRING,.).cl
-0001a170: 6173 7320 5265 666f 726d 6572 466f 7251  ass ReformerForQ
-0001a180: 7565 7374 696f 6e41 6e73 7765 7269 6e67  uestionAnswering
-0001a190: 2852 6566 6f72 6d65 7250 7265 5472 6169  (ReformerPreTrai
-0001a1a0: 6e65 644d 6f64 656c 293a 0a20 2020 2064  nedModel):.    d
-0001a1b0: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-0001a1c0: 2c20 636f 6e66 6967 293a 0a20 2020 2020  , config):.     
-0001a1d0: 2020 2073 7570 6572 2829 2e5f 5f69 6e69     super().__ini
-0001a1e0: 745f 5f28 636f 6e66 6967 290a 2020 2020  t__(config).    
-0001a1f0: 2020 2020 7365 6c66 2e6e 756d 5f6c 6162      self.num_lab
-0001a200: 656c 7320 3d20 636f 6e66 6967 2e6e 756d  els = config.num
-0001a210: 5f6c 6162 656c 730a 0a20 2020 2020 2020  _labels..       
-0001a220: 2073 656c 662e 7265 666f 726d 6572 203d   self.reformer =
-0001a230: 2052 6566 6f72 6d65 724d 6f64 656c 2863   ReformerModel(c
-0001a240: 6f6e 6669 6729 0a20 2020 2020 2020 2023  onfig).        #
-0001a250: 2032 202a 2063 6f6e 6669 672e 6869 6464   2 * config.hidd
-0001a260: 656e 5f73 697a 6520 6265 6361 7573 6520  en_size because 
-0001a270: 7765 2075 7365 2072 6576 6572 7369 626c  we use reversibl
-0001a280: 6520 7265 7369 6475 616c 206c 6179 6572  e residual layer
-0001a290: 730a 2020 2020 2020 2020 7365 6c66 2e71  s.        self.q
-0001a2a0: 615f 6f75 7470 7574 7320 3d20 6e6e 2e4c  a_outputs = nn.L
-0001a2b0: 696e 6561 7228 3220 2a20 636f 6e66 6967  inear(2 * config
-0001a2c0: 2e68 6964 6465 6e5f 7369 7a65 2c20 636f  .hidden_size, co
-0001a2d0: 6e66 6967 2e6e 756d 5f6c 6162 656c 7329  nfig.num_labels)
-0001a2e0: 0a0a 2020 2020 2020 2020 7365 6c66 2e69  ..        self.i
-0001a2f0: 6e69 745f 7765 6967 6874 7328 290a 0a20  nit_weights().. 
-0001a300: 2020 2040 6164 645f 7374 6172 745f 646f     @add_start_do
-0001a310: 6373 7472 696e 6773 5f74 6f5f 6d6f 6465  cstrings_to_mode
-0001a320: 6c5f 666f 7277 6172 6428 5245 464f 524d  l_forward(REFORM
-0001a330: 4552 5f49 4e50 5554 535f 444f 4353 5452  ER_INPUTS_DOCSTR
-0001a340: 494e 4729 0a20 2020 2040 6164 645f 636f  ING).    @add_co
-0001a350: 6465 5f73 616d 706c 655f 646f 6373 7472  de_sample_docstr
-0001a360: 696e 6773 280a 2020 2020 2020 2020 746f  ings(.        to
-0001a370: 6b65 6e69 7a65 725f 636c 6173 733d 5f54  kenizer_class=_T
-0001a380: 4f4b 454e 495a 4552 5f46 4f52 5f44 4f43  OKENIZER_FOR_DOC
-0001a390: 2c0a 2020 2020 2020 2020 6368 6563 6b70  ,.        checkp
-0001a3a0: 6f69 6e74 3d5f 4348 4543 4b50 4f49 4e54  oint=_CHECKPOINT
-0001a3b0: 5f46 4f52 5f44 4f43 2c0a 2020 2020 2020  _FOR_DOC,.      
-0001a3c0: 2020 6f75 7470 7574 5f74 7970 653d 5175    output_type=Qu
-0001a3d0: 6573 7469 6f6e 416e 7377 6572 696e 674d  estionAnsweringM
-0001a3e0: 6f64 656c 4f75 7470 7574 2c0a 2020 2020  odelOutput,.    
-0001a3f0: 2020 2020 636f 6e66 6967 5f63 6c61 7373      config_class
-0001a400: 3d5f 434f 4e46 4947 5f46 4f52 5f44 4f43  =_CONFIG_FOR_DOC
-0001a410: 2c0a 2020 2020 290a 2020 2020 6465 6620  ,.    ).    def 
-0001a420: 666f 7277 6172 6428 0a20 2020 2020 2020  forward(.       
-0001a430: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
-0001a440: 6e70 7574 5f69 6473 3d4e 6f6e 652c 0a20  nput_ids=None,. 
-0001a450: 2020 2020 2020 2070 6f73 6974 696f 6e5f         position_
-0001a460: 6964 733d 4e6f 6e65 2c0a 2020 2020 2020  ids=None,.      
-0001a470: 2020 6174 7465 6e74 696f 6e5f 6d61 736b    attention_mask
-0001a480: 3d4e 6f6e 652c 0a20 2020 2020 2020 2068  =None,.        h
-0001a490: 6561 645f 6d61 736b 3d4e 6f6e 652c 0a20  ead_mask=None,. 
-0001a4a0: 2020 2020 2020 2069 6e70 7574 735f 656d         inputs_em
-0001a4b0: 6265 6473 3d4e 6f6e 652c 0a20 2020 2020  beds=None,.     
-0001a4c0: 2020 206e 756d 5f68 6173 6865 733d 4e6f     num_hashes=No
-0001a4d0: 6e65 2c0a 2020 2020 2020 2020 7374 6172  ne,.        star
-0001a4e0: 745f 706f 7369 7469 6f6e 733d 4e6f 6e65  t_positions=None
-0001a4f0: 2c0a 2020 2020 2020 2020 656e 645f 706f  ,.        end_po
-0001a500: 7369 7469 6f6e 733d 4e6f 6e65 2c0a 2020  sitions=None,.  
-0001a510: 2020 2020 2020 6f75 7470 7574 5f68 6964        output_hid
-0001a520: 6465 6e5f 7374 6174 6573 3d4e 6f6e 652c  den_states=None,
-0001a530: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-0001a540: 6174 7465 6e74 696f 6e73 3d4e 6f6e 652c  attentions=None,
-0001a550: 0a20 2020 2020 2020 2072 6574 7572 6e5f  .        return_
-0001a560: 6469 6374 3d4e 6f6e 652c 0a20 2020 2029  dict=None,.    )
-0001a570: 3a0a 2020 2020 2020 2020 7222 2222 0a20  :.        r""". 
-0001a580: 2020 2020 2020 2073 7461 7274 5f70 6f73         start_pos
-0001a590: 6974 696f 6e73 2028 3a6f 626a 3a60 746f  itions (:obj:`to
-0001a5a0: 7263 682e 4c6f 6e67 5465 6e73 6f72 6020  rch.LongTensor` 
-0001a5b0: 6f66 2073 6861 7065 203a 6f62 6a3a 6028  of shape :obj:`(
-0001a5c0: 6261 7463 685f 7369 7a65 2c29 602c 2060  batch_size,)`, `
-0001a5d0: 6f70 7469 6f6e 616c 6029 3a0a 2020 2020  optional`):.    
-0001a5e0: 2020 2020 2020 2020 4c61 6265 6c73 2066          Labels f
-0001a5f0: 6f72 2070 6f73 6974 696f 6e20 2869 6e64  or position (ind
-0001a600: 6578 2920 6f66 2074 6865 2073 7461 7274  ex) of the start
-0001a610: 206f 6620 7468 6520 6c61 6265 6c6c 6564   of the labelled
-0001a620: 2073 7061 6e20 666f 7220 636f 6d70 7574   span for comput
-0001a630: 696e 6720 7468 6520 746f 6b65 6e20 636c  ing the token cl
-0001a640: 6173 7369 6669 6361 7469 6f6e 206c 6f73  assification los
-0001a650: 732e 0a20 2020 2020 2020 2020 2020 2050  s..            P
-0001a660: 6f73 6974 696f 6e73 2061 7265 2063 6c61  ositions are cla
-0001a670: 6d70 6564 2074 6f20 7468 6520 6c65 6e67  mped to the leng
-0001a680: 7468 206f 6620 7468 6520 7365 7175 656e  th of the sequen
-0001a690: 6365 2028 3a6f 626a 3a60 7365 7175 656e  ce (:obj:`sequen
-0001a6a0: 6365 5f6c 656e 6774 6860 292e 2050 6f73  ce_length`). Pos
-0001a6b0: 6974 696f 6e20 6f75 7473 6964 6520 6f66  ition outside of
-0001a6c0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0001a6d0: 2073 6571 7565 6e63 6520 6172 6520 6e6f   sequence are no
-0001a6e0: 7420 7461 6b65 6e20 696e 746f 2061 6363  t taken into acc
-0001a6f0: 6f75 6e74 2066 6f72 2063 6f6d 7075 7469  ount for computi
-0001a700: 6e67 2074 6865 206c 6f73 732e 0a20 2020  ng the loss..   
-0001a710: 2020 2020 2065 6e64 5f70 6f73 6974 696f       end_positio
-0001a720: 6e73 2028 3a6f 626a 3a60 746f 7263 682e  ns (:obj:`torch.
-0001a730: 4c6f 6e67 5465 6e73 6f72 6020 6f66 2073  LongTensor` of s
-0001a740: 6861 7065 203a 6f62 6a3a 6028 6261 7463  hape :obj:`(batc
-0001a750: 685f 7369 7a65 2c29 602c 2060 6f70 7469  h_size,)`, `opti
-0001a760: 6f6e 616c 6029 3a0a 2020 2020 2020 2020  onal`):.        
-0001a770: 2020 2020 4c61 6265 6c73 2066 6f72 2070      Labels for p
-0001a780: 6f73 6974 696f 6e20 2869 6e64 6578 2920  osition (index) 
-0001a790: 6f66 2074 6865 2065 6e64 206f 6620 7468  of the end of th
-0001a7a0: 6520 6c61 6265 6c6c 6564 2073 7061 6e20  e labelled span 
-0001a7b0: 666f 7220 636f 6d70 7574 696e 6720 7468  for computing th
-0001a7c0: 6520 746f 6b65 6e20 636c 6173 7369 6669  e token classifi
-0001a7d0: 6361 7469 6f6e 206c 6f73 732e 0a20 2020  cation loss..   
-0001a7e0: 2020 2020 2020 2020 2050 6f73 6974 696f           Positio
-0001a7f0: 6e73 2061 7265 2063 6c61 6d70 6564 2074  ns are clamped t
-0001a800: 6f20 7468 6520 6c65 6e67 7468 206f 6620  o the length of 
-0001a810: 7468 6520 7365 7175 656e 6365 2028 3a6f  the sequence (:o
-0001a820: 626a 3a60 7365 7175 656e 6365 5f6c 656e  bj:`sequence_len
-0001a830: 6774 6860 292e 2050 6f73 6974 696f 6e20  gth`). Position 
-0001a840: 6f75 7473 6964 6520 6f66 2074 6865 0a20  outside of the. 
-0001a850: 2020 2020 2020 2020 2020 2073 6571 7565             seque
-0001a860: 6e63 6520 6172 6520 6e6f 7420 7461 6b65  nce are not take
-0001a870: 6e20 696e 746f 2061 6363 6f75 6e74 2066  n into account f
-0001a880: 6f72 2063 6f6d 7075 7469 6e67 2074 6865  or computing the
-0001a890: 206c 6f73 732e 0a20 2020 2020 2020 2022   loss..        "
-0001a8a0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-0001a8b0: 6e5f 6469 6374 203d 2072 6574 7572 6e5f  n_dict = return_
-0001a8c0: 6469 6374 2069 6620 7265 7475 726e 5f64  dict if return_d
-0001a8d0: 6963 7420 6973 206e 6f74 204e 6f6e 6520  ict is not None 
-0001a8e0: 656c 7365 2073 656c 662e 636f 6e66 6967  else self.config
-0001a8f0: 2e75 7365 5f72 6574 7572 6e5f 6469 6374  .use_return_dict
-0001a900: 0a0a 2020 2020 2020 2020 7265 666f 726d  ..        reform
-0001a910: 6572 5f6f 7574 7075 7473 203d 2073 656c  er_outputs = sel
-0001a920: 662e 7265 666f 726d 6572 280a 2020 2020  f.reformer(.    
-0001a930: 2020 2020 2020 2020 696e 7075 745f 6964          input_id
-0001a940: 732c 0a20 2020 2020 2020 2020 2020 2070  s,.            p
-0001a950: 6f73 6974 696f 6e5f 6964 733d 706f 7369  osition_ids=posi
-0001a960: 7469 6f6e 5f69 6473 2c0a 2020 2020 2020  tion_ids,.      
-0001a970: 2020 2020 2020 6174 7465 6e74 696f 6e5f        attention_
-0001a980: 6d61 736b 3d61 7474 656e 7469 6f6e 5f6d  mask=attention_m
-0001a990: 6173 6b2c 0a20 2020 2020 2020 2020 2020  ask,.           
-0001a9a0: 2068 6561 645f 6d61 736b 3d68 6561 645f   head_mask=head_
-0001a9b0: 6d61 736b 2c0a 2020 2020 2020 2020 2020  mask,.          
-0001a9c0: 2020 696e 7075 7473 5f65 6d62 6564 733d    inputs_embeds=
-0001a9d0: 696e 7075 7473 5f65 6d62 6564 732c 0a20  inputs_embeds,. 
-0001a9e0: 2020 2020 2020 2020 2020 206e 756d 5f68             num_h
-0001a9f0: 6173 6865 733d 6e75 6d5f 6861 7368 6573  ashes=num_hashes
-0001aa00: 2c0a 2020 2020 2020 2020 2020 2020 7573  ,.            us
-0001aa10: 655f 6361 6368 653d 4661 6c73 652c 2020  e_cache=False,  
-0001aa20: 2320 6e6f 2063 6175 7361 6c20 6d61 736b  # no causal mask
-0001aa30: 0a20 2020 2020 2020 2020 2020 206f 7574  .            out
-0001aa40: 7075 745f 6869 6464 656e 5f73 7461 7465  put_hidden_state
-0001aa50: 733d 6f75 7470 7574 5f68 6964 6465 6e5f  s=output_hidden_
-0001aa60: 7374 6174 6573 2c0a 2020 2020 2020 2020  states,.        
-0001aa70: 2020 2020 6f75 7470 7574 5f61 7474 656e      output_atten
-0001aa80: 7469 6f6e 733d 6f75 7470 7574 5f61 7474  tions=output_att
-0001aa90: 656e 7469 6f6e 732c 0a20 2020 2020 2020  entions,.       
-0001aaa0: 2020 2020 2072 6574 7572 6e5f 6469 6374       return_dict
-0001aab0: 3d72 6574 7572 6e5f 6469 6374 2c0a 2020  =return_dict,.  
-0001aac0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0001aad0: 2073 6571 7565 6e63 655f 6f75 7470 7574   sequence_output
-0001aae0: 203d 2072 6566 6f72 6d65 725f 6f75 7470   = reformer_outp
-0001aaf0: 7574 735b 305d 0a0a 2020 2020 2020 2020  uts[0]..        
-0001ab00: 6c6f 6769 7473 203d 2073 656c 662e 7161  logits = self.qa
-0001ab10: 5f6f 7574 7075 7473 2873 6571 7565 6e63  _outputs(sequenc
-0001ab20: 655f 6f75 7470 7574 290a 2020 2020 2020  e_output).      
-0001ab30: 2020 7374 6172 745f 6c6f 6769 7473 2c20    start_logits, 
-0001ab40: 656e 645f 6c6f 6769 7473 203d 206c 6f67  end_logits = log
-0001ab50: 6974 732e 7370 6c69 7428 312c 2064 696d  its.split(1, dim
-0001ab60: 3d2d 3129 0a20 2020 2020 2020 2073 7461  =-1).        sta
-0001ab70: 7274 5f6c 6f67 6974 7320 3d20 7374 6172  rt_logits = star
-0001ab80: 745f 6c6f 6769 7473 2e73 7175 6565 7a65  t_logits.squeeze
-0001ab90: 282d 3129 2e63 6f6e 7469 6775 6f75 7328  (-1).contiguous(
-0001aba0: 290a 2020 2020 2020 2020 656e 645f 6c6f  ).        end_lo
-0001abb0: 6769 7473 203d 2065 6e64 5f6c 6f67 6974  gits = end_logit
-0001abc0: 732e 7371 7565 657a 6528 2d31 292e 636f  s.squeeze(-1).co
-0001abd0: 6e74 6967 756f 7573 2829 0a0a 2020 2020  ntiguous()..    
-0001abe0: 2020 2020 746f 7461 6c5f 6c6f 7373 203d      total_loss =
-0001abf0: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
-0001ac00: 2073 7461 7274 5f70 6f73 6974 696f 6e73   start_positions
-0001ac10: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-0001ac20: 2065 6e64 5f70 6f73 6974 696f 6e73 2069   end_positions i
-0001ac30: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0001ac40: 2020 2020 2020 2020 2320 4966 2077 6520          # If we 
-0001ac50: 6172 6520 6f6e 206d 756c 7469 2d47 5055  are on multi-GPU
-0001ac60: 2c20 7370 6c69 7420 6164 6420 6120 6469  , split add a di
-0001ac70: 6d65 6e73 696f 6e0a 2020 2020 2020 2020  mension.        
-0001ac80: 2020 2020 6966 206c 656e 2873 7461 7274      if len(start
-0001ac90: 5f70 6f73 6974 696f 6e73 2e73 697a 6528  _positions.size(
-0001aca0: 2929 203e 2031 3a0a 2020 2020 2020 2020  )) > 1:.        
-0001acb0: 2020 2020 2020 2020 7374 6172 745f 706f          start_po
-0001acc0: 7369 7469 6f6e 7320 3d20 7374 6172 745f  sitions = start_
-0001acd0: 706f 7369 7469 6f6e 732e 7371 7565 657a  positions.squeez
-0001ace0: 6528 2d31 290a 2020 2020 2020 2020 2020  e(-1).          
-0001acf0: 2020 6966 206c 656e 2865 6e64 5f70 6f73    if len(end_pos
-0001ad00: 6974 696f 6e73 2e73 697a 6528 2929 203e  itions.size()) >
-0001ad10: 2031 3a0a 2020 2020 2020 2020 2020 2020   1:.            
-0001ad20: 2020 2020 656e 645f 706f 7369 7469 6f6e      end_position
-0001ad30: 7320 3d20 656e 645f 706f 7369 7469 6f6e  s = end_position
-0001ad40: 732e 7371 7565 657a 6528 2d31 290a 2020  s.squeeze(-1).  
-0001ad50: 2020 2020 2020 2020 2020 2320 736f 6d65            # some
-0001ad60: 7469 6d65 7320 7468 6520 7374 6172 742f  times the start/
-0001ad70: 656e 6420 706f 7369 7469 6f6e 7320 6172  end positions ar
-0001ad80: 6520 6f75 7473 6964 6520 6f75 7220 6d6f  e outside our mo
-0001ad90: 6465 6c20 696e 7075 7473 2c20 7765 2069  del inputs, we i
-0001ada0: 676e 6f72 6520 7468 6573 6520 7465 726d  gnore these term
-0001adb0: 730a 2020 2020 2020 2020 2020 2020 6967  s.            ig
-0001adc0: 6e6f 7265 645f 696e 6465 7820 3d20 7374  nored_index = st
-0001add0: 6172 745f 6c6f 6769 7473 2e73 697a 6528  art_logits.size(
-0001ade0: 3129 0a20 2020 2020 2020 2020 2020 2073  1).            s
-0001adf0: 7461 7274 5f70 6f73 6974 696f 6e73 203d  tart_positions =
-0001ae00: 2073 7461 7274 5f70 6f73 6974 696f 6e73   start_positions
-0001ae10: 2e63 6c61 6d70 2830 2c20 6967 6e6f 7265  .clamp(0, ignore
-0001ae20: 645f 696e 6465 7829 0a20 2020 2020 2020  d_index).       
-0001ae30: 2020 2020 2065 6e64 5f70 6f73 6974 696f       end_positio
-0001ae40: 6e73 203d 2065 6e64 5f70 6f73 6974 696f  ns = end_positio
-0001ae50: 6e73 2e63 6c61 6d70 2830 2c20 6967 6e6f  ns.clamp(0, igno
-0001ae60: 7265 645f 696e 6465 7829 0a0a 2020 2020  red_index)..    
-0001ae70: 2020 2020 2020 2020 6c6f 7373 5f66 6374          loss_fct
-0001ae80: 203d 2043 726f 7373 456e 7472 6f70 794c   = CrossEntropyL
-0001ae90: 6f73 7328 6967 6e6f 7265 5f69 6e64 6578  oss(ignore_index
-0001aea0: 3d69 676e 6f72 6564 5f69 6e64 6578 290a  =ignored_index).
-0001aeb0: 2020 2020 2020 2020 2020 2020 7374 6172              star
-0001aec0: 745f 6c6f 7373 203d 206c 6f73 735f 6663  t_loss = loss_fc
-0001aed0: 7428 7374 6172 745f 6c6f 6769 7473 2c20  t(start_logits, 
-0001aee0: 7374 6172 745f 706f 7369 7469 6f6e 7329  start_positions)
-0001aef0: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
-0001af00: 5f6c 6f73 7320 3d20 6c6f 7373 5f66 6374  _loss = loss_fct
-0001af10: 2865 6e64 5f6c 6f67 6974 732c 2065 6e64  (end_logits, end
-0001af20: 5f70 6f73 6974 696f 6e73 290a 2020 2020  _positions).    
-0001af30: 2020 2020 2020 2020 746f 7461 6c5f 6c6f          total_lo
-0001af40: 7373 203d 2028 7374 6172 745f 6c6f 7373  ss = (start_loss
-0001af50: 202b 2065 6e64 5f6c 6f73 7329 202f 2032   + end_loss) / 2
-0001af60: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0001af70: 2072 6574 7572 6e5f 6469 6374 3a0a 2020   return_dict:.  
-0001af80: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-0001af90: 203d 2028 7374 6172 745f 6c6f 6769 7473   = (start_logits
-0001afa0: 2c20 656e 645f 6c6f 6769 7473 2920 2b20  , end_logits) + 
-0001afb0: 7265 666f 726d 6572 5f6f 7574 7075 7473  reformer_outputs
-0001afc0: 5b31 3a5d 0a20 2020 2020 2020 2020 2020  [1:].           
-0001afd0: 2072 6574 7572 6e20 2828 746f 7461 6c5f   return ((total_
-0001afe0: 6c6f 7373 2c29 202b 206f 7574 7075 7429  loss,) + output)
-0001aff0: 2069 6620 746f 7461 6c5f 6c6f 7373 2069   if total_loss i
-0001b000: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
-0001b010: 6f75 7470 7574 0a0a 2020 2020 2020 2020  output..        
-0001b020: 7265 7475 726e 2051 7565 7374 696f 6e41  return QuestionA
-0001b030: 6e73 7765 7269 6e67 4d6f 6465 6c4f 7574  nsweringModelOut
-0001b040: 7075 7428 0a20 2020 2020 2020 2020 2020  put(.           
-0001b050: 206c 6f73 733d 746f 7461 6c5f 6c6f 7373   loss=total_loss
-0001b060: 2c0a 2020 2020 2020 2020 2020 2020 7374  ,.            st
-0001b070: 6172 745f 6c6f 6769 7473 3d73 7461 7274  art_logits=start
-0001b080: 5f6c 6f67 6974 732c 0a20 2020 2020 2020  _logits,.       
-0001b090: 2020 2020 2065 6e64 5f6c 6f67 6974 733d       end_logits=
-0001b0a0: 656e 645f 6c6f 6769 7473 2c0a 2020 2020  end_logits,.    
-0001b0b0: 2020 2020 2020 2020 6869 6464 656e 5f73          hidden_s
-0001b0c0: 7461 7465 733d 7265 666f 726d 6572 5f6f  tates=reformer_o
-0001b0d0: 7574 7075 7473 2e68 6964 6465 6e5f 7374  utputs.hidden_st
-0001b0e0: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
-0001b0f0: 2020 6174 7465 6e74 696f 6e73 3d72 6566    attentions=ref
-0001b100: 6f72 6d65 725f 6f75 7470 7574 732e 6174  ormer_outputs.at
-0001b110: 7465 6e74 696f 6e73 2c0a 2020 2020 2020  tentions,.      
-0001b120: 2020 290a                                  ).
+00019af0: 5f66 6374 203d 2043 726f 7373 456e 7472  _fct = CrossEntr
+00019b00: 6f70 794c 6f73 7328 290a 2020 2020 2020  opyLoss().      
+00019b10: 2020 2020 2020 2020 2020 6c6f 7373 203d            loss =
+00019b20: 206c 6f73 735f 6663 7428 6c6f 6769 7473   loss_fct(logits
+00019b30: 2e76 6965 7728 2d31 2c20 7365 6c66 2e6e  .view(-1, self.n
+00019b40: 756d 5f6c 6162 656c 7329 2c20 6c61 6265  um_labels), labe
+00019b50: 6c73 2e76 6965 7728 2d31 2929 0a20 2020  ls.view(-1)).   
+00019b60: 2020 2020 2020 2020 2065 6c69 6620 7365           elif se
+00019b70: 6c66 2e63 6f6e 6669 672e 7072 6f62 6c65  lf.config.proble
+00019b80: 6d5f 7479 7065 203d 3d20 226d 756c 7469  m_type == "multi
+00019b90: 5f6c 6162 656c 5f63 6c61 7373 6966 6963  _label_classific
+00019ba0: 6174 696f 6e22 3a0a 2020 2020 2020 2020  ation":.        
+00019bb0: 2020 2020 2020 2020 6c6f 7373 5f66 6374          loss_fct
+00019bc0: 203d 2042 4345 5769 7468 4c6f 6769 7473   = BCEWithLogits
+00019bd0: 4c6f 7373 2829 0a20 2020 2020 2020 2020  Loss().         
+00019be0: 2020 2020 2020 206c 6f73 7320 3d20 6c6f         loss = lo
+00019bf0: 7373 5f66 6374 286c 6f67 6974 732c 206c  ss_fct(logits, l
+00019c00: 6162 656c 7329 0a0a 2020 2020 2020 2020  abels)..        
+00019c10: 6966 206e 6f74 2072 6574 7572 6e5f 6469  if not return_di
+00019c20: 6374 3a0a 2020 2020 2020 2020 2020 2020  ct:.            
+00019c30: 6f75 7470 7574 203d 2028 6c6f 6769 7473  output = (logits
+00019c40: 2c29 202b 206f 7574 7075 7473 5b32 3a5d  ,) + outputs[2:]
+00019c50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00019c60: 7572 6e20 2828 6c6f 7373 2c29 202b 206f  urn ((loss,) + o
+00019c70: 7574 7075 7429 2069 6620 6c6f 7373 2069  utput) if loss i
+00019c80: 7320 6e6f 7420 4e6f 6e65 2065 6c73 6520  s not None else 
+00019c90: 6f75 7470 7574 0a0a 2020 2020 2020 2020  output..        
+00019ca0: 7265 7475 726e 2053 6571 7565 6e63 6543  return SequenceC
+00019cb0: 6c61 7373 6966 6965 724f 7574 7075 7428  lassifierOutput(
+00019cc0: 0a20 2020 2020 2020 2020 2020 206c 6f73  .            los
+00019cd0: 733d 6c6f 7373 2c0a 2020 2020 2020 2020  s=loss,.        
+00019ce0: 2020 2020 6c6f 6769 7473 3d6c 6f67 6974      logits=logit
+00019cf0: 732c 0a20 2020 2020 2020 2020 2020 2068  s,.            h
+00019d00: 6964 6465 6e5f 7374 6174 6573 3d6f 7574  idden_states=out
+00019d10: 7075 7473 2e68 6964 6465 6e5f 7374 6174  puts.hidden_stat
+00019d20: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+00019d30: 6174 7465 6e74 696f 6e73 3d6f 7574 7075  attentions=outpu
+00019d40: 7473 2e61 7474 656e 7469 6f6e 732c 0a20  ts.attentions,. 
+00019d50: 2020 2020 2020 2029 0a0a 0a63 6c61 7373         )...class
+00019d60: 2052 6566 6f72 6d65 7243 6c61 7373 6966   ReformerClassif
+00019d70: 6963 6174 696f 6e48 6561 6428 6e6e 2e4d  icationHead(nn.M
+00019d80: 6f64 756c 6529 3a0a 2020 2020 2222 2248  odule):.    """H
+00019d90: 6561 6420 666f 7220 7365 6e74 656e 6365  ead for sentence
+00019da0: 2d6c 6576 656c 2063 6c61 7373 6966 6963  -level classific
+00019db0: 6174 696f 6e20 7461 736b 732e 2222 220a  ation tasks.""".
+00019dc0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+00019dd0: 5f28 7365 6c66 2c20 636f 6e66 6967 293a  _(self, config):
+00019de0: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00019df0: 2e5f 5f69 6e69 745f 5f28 290a 2020 2020  .__init__().    
+00019e00: 2020 2020 7365 6c66 2e64 656e 7365 203d      self.dense =
+00019e10: 206e 6e2e 4c69 6e65 6172 2832 202a 2063   nn.Linear(2 * c
+00019e20: 6f6e 6669 672e 6869 6464 656e 5f73 697a  onfig.hidden_siz
+00019e30: 652c 2063 6f6e 6669 672e 6869 6464 656e  e, config.hidden
+00019e40: 5f73 697a 6529 0a20 2020 2020 2020 2073  _size).        s
+00019e50: 656c 662e 6472 6f70 6f75 7420 3d20 6e6e  elf.dropout = nn
+00019e60: 2e44 726f 706f 7574 2863 6f6e 6669 672e  .Dropout(config.
+00019e70: 6869 6464 656e 5f64 726f 706f 7574 5f70  hidden_dropout_p
+00019e80: 726f 6229 0a20 2020 2020 2020 2073 656c  rob).        sel
+00019e90: 662e 6f75 745f 7072 6f6a 203d 206e 6e2e  f.out_proj = nn.
+00019ea0: 4c69 6e65 6172 2863 6f6e 6669 672e 6869  Linear(config.hi
+00019eb0: 6464 656e 5f73 697a 652c 2063 6f6e 6669  dden_size, confi
+00019ec0: 672e 6e75 6d5f 6c61 6265 6c73 290a 0a20  g.num_labels).. 
+00019ed0: 2020 2064 6566 2066 6f72 7761 7264 2873     def forward(s
+00019ee0: 656c 662c 2068 6964 6465 6e5f 7374 6174  elf, hidden_stat
+00019ef0: 6573 2c20 2a2a 6b77 6172 6773 293a 0a20  es, **kwargs):. 
+00019f00: 2020 2020 2020 2068 6964 6465 6e5f 7374         hidden_st
+00019f10: 6174 6573 203d 2068 6964 6465 6e5f 7374  ates = hidden_st
+00019f20: 6174 6573 5b3a 2c20 302c 203a 5d20 2023  ates[:, 0, :]  #
+00019f30: 2074 616b 6520 3c73 3e20 746f 6b65 6e20   take <s> token 
+00019f40: 2865 7175 6976 2e20 746f 205b 434c 535d  (equiv. to [CLS]
+00019f50: 290a 2020 2020 2020 2020 6869 6464 656e  ).        hidden
+00019f60: 5f73 7461 7465 7320 3d20 7365 6c66 2e64  _states = self.d
+00019f70: 726f 706f 7574 2868 6964 6465 6e5f 7374  ropout(hidden_st
+00019f80: 6174 6573 290a 2020 2020 2020 2020 6869  ates).        hi
+00019f90: 6464 656e 5f73 7461 7465 7320 3d20 7365  dden_states = se
+00019fa0: 6c66 2e64 656e 7365 2868 6964 6465 6e5f  lf.dense(hidden_
+00019fb0: 7374 6174 6573 290a 2020 2020 2020 2020  states).        
+00019fc0: 6869 6464 656e 5f73 7461 7465 7320 3d20  hidden_states = 
+00019fd0: 746f 7263 682e 7461 6e68 2868 6964 6465  torch.tanh(hidde
+00019fe0: 6e5f 7374 6174 6573 290a 2020 2020 2020  n_states).      
+00019ff0: 2020 6869 6464 656e 5f73 7461 7465 7320    hidden_states 
+0001a000: 3d20 7365 6c66 2e64 726f 706f 7574 2868  = self.dropout(h
+0001a010: 6964 6465 6e5f 7374 6174 6573 290a 2020  idden_states).  
+0001a020: 2020 2020 2020 6869 6464 656e 5f73 7461        hidden_sta
+0001a030: 7465 7320 3d20 7365 6c66 2e6f 7574 5f70  tes = self.out_p
+0001a040: 726f 6a28 6869 6464 656e 5f73 7461 7465  roj(hidden_state
+0001a050: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+0001a060: 6e20 6869 6464 656e 5f73 7461 7465 730a  n hidden_states.
+0001a070: 0a0a 4061 6464 5f73 7461 7274 5f64 6f63  ..@add_start_doc
+0001a080: 7374 7269 6e67 7328 0a20 2020 2022 2222  strings(.    """
+0001a090: 0a20 2020 2052 6566 6f72 6d65 7220 4d6f  .    Reformer Mo
+0001a0a0: 6465 6c20 7769 7468 2061 2073 7061 6e20  del with a span 
+0001a0b0: 636c 6173 7369 6669 6361 7469 6f6e 2068  classification h
+0001a0c0: 6561 6420 6f6e 2074 6f70 2066 6f72 2065  ead on top for e
+0001a0d0: 7874 7261 6374 6976 6520 7175 6573 7469  xtractive questi
+0001a0e0: 6f6e 2d61 6e73 7765 7269 6e67 2074 6173  on-answering tas
+0001a0f0: 6b73 206c 696b 6520 5351 7541 4420 2f20  ks like SQuAD / 
+0001a100: 5472 6976 6961 5141 0a20 2020 2028 2061  TriviaQA.    ( a
+0001a110: 206c 696e 6561 7220 6c61 7965 7220 6f6e   linear layer on
+0001a120: 2074 6f70 206f 6620 6869 6464 656e 2d73   top of hidden-s
+0001a130: 7461 7465 7320 6f75 7470 7574 2074 6f20  tates output to 
+0001a140: 636f 6d70 7574 6520 6073 7061 6e20 7374  compute `span st
+0001a150: 6172 7420 6c6f 6769 7473 6020 616e 6420  art logits` and 
+0001a160: 6073 7061 6e20 656e 6420 6c6f 6769 7473  `span end logits
+0001a170: 602e 0a20 2020 2022 2222 2c0a 2020 2020  `..    """,.    
+0001a180: 5245 464f 524d 4552 5f53 5441 5254 5f44  REFORMER_START_D
+0001a190: 4f43 5354 5249 4e47 2c0a 290a 636c 6173  OCSTRING,.).clas
+0001a1a0: 7320 5265 666f 726d 6572 466f 7251 7565  s ReformerForQue
+0001a1b0: 7374 696f 6e41 6e73 7765 7269 6e67 2852  stionAnswering(R
+0001a1c0: 6566 6f72 6d65 7250 7265 5472 6169 6e65  eformerPreTraine
+0001a1d0: 644d 6f64 656c 293a 0a20 2020 2064 6566  dModel):.    def
+0001a1e0: 205f 5f69 6e69 745f 5f28 7365 6c66 2c20   __init__(self, 
+0001a1f0: 636f 6e66 6967 293a 0a20 2020 2020 2020  config):.       
+0001a200: 2073 7570 6572 2829 2e5f 5f69 6e69 745f   super().__init_
+0001a210: 5f28 636f 6e66 6967 290a 2020 2020 2020  _(config).      
+0001a220: 2020 7365 6c66 2e6e 756d 5f6c 6162 656c    self.num_label
+0001a230: 7320 3d20 636f 6e66 6967 2e6e 756d 5f6c  s = config.num_l
+0001a240: 6162 656c 730a 0a20 2020 2020 2020 2073  abels..        s
+0001a250: 656c 662e 7265 666f 726d 6572 203d 2052  elf.reformer = R
+0001a260: 6566 6f72 6d65 724d 6f64 656c 2863 6f6e  eformerModel(con
+0001a270: 6669 6729 0a20 2020 2020 2020 2023 2032  fig).        # 2
+0001a280: 202a 2063 6f6e 6669 672e 6869 6464 656e   * config.hidden
+0001a290: 5f73 697a 6520 6265 6361 7573 6520 7765  _size because we
+0001a2a0: 2075 7365 2072 6576 6572 7369 626c 6520   use reversible 
+0001a2b0: 7265 7369 6475 616c 206c 6179 6572 730a  residual layers.
+0001a2c0: 2020 2020 2020 2020 7365 6c66 2e71 615f          self.qa_
+0001a2d0: 6f75 7470 7574 7320 3d20 6e6e 2e4c 696e  outputs = nn.Lin
+0001a2e0: 6561 7228 3220 2a20 636f 6e66 6967 2e68  ear(2 * config.h
+0001a2f0: 6964 6465 6e5f 7369 7a65 2c20 636f 6e66  idden_size, conf
+0001a300: 6967 2e6e 756d 5f6c 6162 656c 7329 0a0a  ig.num_labels)..
+0001a310: 2020 2020 2020 2020 7365 6c66 2e69 6e69          self.ini
+0001a320: 745f 7765 6967 6874 7328 290a 0a20 2020  t_weights()..   
+0001a330: 2040 6164 645f 7374 6172 745f 646f 6373   @add_start_docs
+0001a340: 7472 696e 6773 5f74 6f5f 6d6f 6465 6c5f  trings_to_model_
+0001a350: 666f 7277 6172 6428 5245 464f 524d 4552  forward(REFORMER
+0001a360: 5f49 4e50 5554 535f 444f 4353 5452 494e  _INPUTS_DOCSTRIN
+0001a370: 4729 0a20 2020 2040 6164 645f 636f 6465  G).    @add_code
+0001a380: 5f73 616d 706c 655f 646f 6373 7472 696e  _sample_docstrin
+0001a390: 6773 280a 2020 2020 2020 2020 746f 6b65  gs(.        toke
+0001a3a0: 6e69 7a65 725f 636c 6173 733d 5f54 4f4b  nizer_class=_TOK
+0001a3b0: 454e 495a 4552 5f46 4f52 5f44 4f43 2c0a  ENIZER_FOR_DOC,.
+0001a3c0: 2020 2020 2020 2020 6368 6563 6b70 6f69          checkpoi
+0001a3d0: 6e74 3d5f 4348 4543 4b50 4f49 4e54 5f46  nt=_CHECKPOINT_F
+0001a3e0: 4f52 5f44 4f43 2c0a 2020 2020 2020 2020  OR_DOC,.        
+0001a3f0: 6f75 7470 7574 5f74 7970 653d 5175 6573  output_type=Ques
+0001a400: 7469 6f6e 416e 7377 6572 696e 674d 6f64  tionAnsweringMod
+0001a410: 656c 4f75 7470 7574 2c0a 2020 2020 2020  elOutput,.      
+0001a420: 2020 636f 6e66 6967 5f63 6c61 7373 3d5f    config_class=_
+0001a430: 434f 4e46 4947 5f46 4f52 5f44 4f43 2c0a  CONFIG_FOR_DOC,.
+0001a440: 2020 2020 290a 2020 2020 6465 6620 666f      ).    def fo
+0001a450: 7277 6172 6428 0a20 2020 2020 2020 2073  rward(.        s
+0001a460: 656c 662c 0a20 2020 2020 2020 2069 6e70  elf,.        inp
+0001a470: 7574 5f69 6473 3d4e 6f6e 652c 0a20 2020  ut_ids=None,.   
+0001a480: 2020 2020 2070 6f73 6974 696f 6e5f 6964       position_id
+0001a490: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
+0001a4a0: 6174 7465 6e74 696f 6e5f 6d61 736b 3d4e  attention_mask=N
+0001a4b0: 6f6e 652c 0a20 2020 2020 2020 2068 6561  one,.        hea
+0001a4c0: 645f 6d61 736b 3d4e 6f6e 652c 0a20 2020  d_mask=None,.   
+0001a4d0: 2020 2020 2069 6e70 7574 735f 656d 6265       inputs_embe
+0001a4e0: 6473 3d4e 6f6e 652c 0a20 2020 2020 2020  ds=None,.       
+0001a4f0: 206e 756d 5f68 6173 6865 733d 4e6f 6e65   num_hashes=None
+0001a500: 2c0a 2020 2020 2020 2020 7374 6172 745f  ,.        start_
+0001a510: 706f 7369 7469 6f6e 733d 4e6f 6e65 2c0a  positions=None,.
+0001a520: 2020 2020 2020 2020 656e 645f 706f 7369          end_posi
+0001a530: 7469 6f6e 733d 4e6f 6e65 2c0a 2020 2020  tions=None,.    
+0001a540: 2020 2020 6f75 7470 7574 5f68 6964 6465      output_hidde
+0001a550: 6e5f 7374 6174 6573 3d4e 6f6e 652c 0a20  n_states=None,. 
+0001a560: 2020 2020 2020 206f 7574 7075 745f 6174         output_at
+0001a570: 7465 6e74 696f 6e73 3d4e 6f6e 652c 0a20  tentions=None,. 
+0001a580: 2020 2020 2020 2072 6574 7572 6e5f 6469         return_di
+0001a590: 6374 3d4e 6f6e 652c 0a20 2020 2029 3a0a  ct=None,.    ):.
+0001a5a0: 2020 2020 2020 2020 7222 2222 0a20 2020          r""".   
+0001a5b0: 2020 2020 2073 7461 7274 5f70 6f73 6974       start_posit
+0001a5c0: 696f 6e73 2028 3a6f 626a 3a60 746f 7263  ions (:obj:`torc
+0001a5d0: 682e 4c6f 6e67 5465 6e73 6f72 6020 6f66  h.LongTensor` of
+0001a5e0: 2073 6861 7065 203a 6f62 6a3a 6028 6261   shape :obj:`(ba
+0001a5f0: 7463 685f 7369 7a65 2c29 602c 2060 6f70  tch_size,)`, `op
+0001a600: 7469 6f6e 616c 6029 3a0a 2020 2020 2020  tional`):.      
+0001a610: 2020 2020 2020 4c61 6265 6c73 2066 6f72        Labels for
+0001a620: 2070 6f73 6974 696f 6e20 2869 6e64 6578   position (index
+0001a630: 2920 6f66 2074 6865 2073 7461 7274 206f  ) of the start o
+0001a640: 6620 7468 6520 6c61 6265 6c6c 6564 2073  f the labelled s
+0001a650: 7061 6e20 666f 7220 636f 6d70 7574 696e  pan for computin
+0001a660: 6720 7468 6520 746f 6b65 6e20 636c 6173  g the token clas
+0001a670: 7369 6669 6361 7469 6f6e 206c 6f73 732e  sification loss.
+0001a680: 0a20 2020 2020 2020 2020 2020 2050 6f73  .            Pos
+0001a690: 6974 696f 6e73 2061 7265 2063 6c61 6d70  itions are clamp
+0001a6a0: 6564 2074 6f20 7468 6520 6c65 6e67 7468  ed to the length
+0001a6b0: 206f 6620 7468 6520 7365 7175 656e 6365   of the sequence
+0001a6c0: 2028 3a6f 626a 3a60 7365 7175 656e 6365   (:obj:`sequence
+0001a6d0: 5f6c 656e 6774 6860 292e 2050 6f73 6974  _length`). Posit
+0001a6e0: 696f 6e20 6f75 7473 6964 6520 6f66 2074  ion outside of t
+0001a6f0: 6865 0a20 2020 2020 2020 2020 2020 2073  he.            s
+0001a700: 6571 7565 6e63 6520 6172 6520 6e6f 7420  equence are not 
+0001a710: 7461 6b65 6e20 696e 746f 2061 6363 6f75  taken into accou
+0001a720: 6e74 2066 6f72 2063 6f6d 7075 7469 6e67  nt for computing
+0001a730: 2074 6865 206c 6f73 732e 0a20 2020 2020   the loss..     
+0001a740: 2020 2065 6e64 5f70 6f73 6974 696f 6e73     end_positions
+0001a750: 2028 3a6f 626a 3a60 746f 7263 682e 4c6f   (:obj:`torch.Lo
+0001a760: 6e67 5465 6e73 6f72 6020 6f66 2073 6861  ngTensor` of sha
+0001a770: 7065 203a 6f62 6a3a 6028 6261 7463 685f  pe :obj:`(batch_
+0001a780: 7369 7a65 2c29 602c 2060 6f70 7469 6f6e  size,)`, `option
+0001a790: 616c 6029 3a0a 2020 2020 2020 2020 2020  al`):.          
+0001a7a0: 2020 4c61 6265 6c73 2066 6f72 2070 6f73    Labels for pos
+0001a7b0: 6974 696f 6e20 2869 6e64 6578 2920 6f66  ition (index) of
+0001a7c0: 2074 6865 2065 6e64 206f 6620 7468 6520   the end of the 
+0001a7d0: 6c61 6265 6c6c 6564 2073 7061 6e20 666f  labelled span fo
+0001a7e0: 7220 636f 6d70 7574 696e 6720 7468 6520  r computing the 
+0001a7f0: 746f 6b65 6e20 636c 6173 7369 6669 6361  token classifica
+0001a800: 7469 6f6e 206c 6f73 732e 0a20 2020 2020  tion loss..     
+0001a810: 2020 2020 2020 2050 6f73 6974 696f 6e73         Positions
+0001a820: 2061 7265 2063 6c61 6d70 6564 2074 6f20   are clamped to 
+0001a830: 7468 6520 6c65 6e67 7468 206f 6620 7468  the length of th
+0001a840: 6520 7365 7175 656e 6365 2028 3a6f 626a  e sequence (:obj
+0001a850: 3a60 7365 7175 656e 6365 5f6c 656e 6774  :`sequence_lengt
+0001a860: 6860 292e 2050 6f73 6974 696f 6e20 6f75  h`). Position ou
+0001a870: 7473 6964 6520 6f66 2074 6865 0a20 2020  tside of the.   
+0001a880: 2020 2020 2020 2020 2073 6571 7565 6e63           sequenc
+0001a890: 6520 6172 6520 6e6f 7420 7461 6b65 6e20  e are not taken 
+0001a8a0: 696e 746f 2061 6363 6f75 6e74 2066 6f72  into account for
+0001a8b0: 2063 6f6d 7075 7469 6e67 2074 6865 206c   computing the l
+0001a8c0: 6f73 732e 0a20 2020 2020 2020 2022 2222  oss..        """
+0001a8d0: 0a20 2020 2020 2020 2072 6574 7572 6e5f  .        return_
+0001a8e0: 6469 6374 203d 2072 6574 7572 6e5f 6469  dict = return_di
+0001a8f0: 6374 2069 6620 7265 7475 726e 5f64 6963  ct if return_dic
+0001a900: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
+0001a910: 7365 2073 656c 662e 636f 6e66 6967 2e75  se self.config.u
+0001a920: 7365 5f72 6574 7572 6e5f 6469 6374 0a0a  se_return_dict..
+0001a930: 2020 2020 2020 2020 7265 666f 726d 6572          reformer
+0001a940: 5f6f 7574 7075 7473 203d 2073 656c 662e  _outputs = self.
+0001a950: 7265 666f 726d 6572 280a 2020 2020 2020  reformer(.      
+0001a960: 2020 2020 2020 696e 7075 745f 6964 732c        input_ids,
+0001a970: 0a20 2020 2020 2020 2020 2020 2070 6f73  .            pos
+0001a980: 6974 696f 6e5f 6964 733d 706f 7369 7469  ition_ids=positi
+0001a990: 6f6e 5f69 6473 2c0a 2020 2020 2020 2020  on_ids,.        
+0001a9a0: 2020 2020 6174 7465 6e74 696f 6e5f 6d61      attention_ma
+0001a9b0: 736b 3d61 7474 656e 7469 6f6e 5f6d 6173  sk=attention_mas
+0001a9c0: 6b2c 0a20 2020 2020 2020 2020 2020 2068  k,.            h
+0001a9d0: 6561 645f 6d61 736b 3d68 6561 645f 6d61  ead_mask=head_ma
+0001a9e0: 736b 2c0a 2020 2020 2020 2020 2020 2020  sk,.            
+0001a9f0: 696e 7075 7473 5f65 6d62 6564 733d 696e  inputs_embeds=in
+0001aa00: 7075 7473 5f65 6d62 6564 732c 0a20 2020  puts_embeds,.   
+0001aa10: 2020 2020 2020 2020 206e 756d 5f68 6173           num_has
+0001aa20: 6865 733d 6e75 6d5f 6861 7368 6573 2c0a  hes=num_hashes,.
+0001aa30: 2020 2020 2020 2020 2020 2020 7573 655f              use_
+0001aa40: 6361 6368 653d 4661 6c73 652c 2020 2320  cache=False,  # 
+0001aa50: 6e6f 2063 6175 7361 6c20 6d61 736b 0a20  no causal mask. 
+0001aa60: 2020 2020 2020 2020 2020 206f 7574 7075             outpu
+0001aa70: 745f 6869 6464 656e 5f73 7461 7465 733d  t_hidden_states=
+0001aa80: 6f75 7470 7574 5f68 6964 6465 6e5f 7374  output_hidden_st
+0001aa90: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
+0001aaa0: 2020 6f75 7470 7574 5f61 7474 656e 7469    output_attenti
+0001aab0: 6f6e 733d 6f75 7470 7574 5f61 7474 656e  ons=output_atten
+0001aac0: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+0001aad0: 2020 2072 6574 7572 6e5f 6469 6374 3d72     return_dict=r
+0001aae0: 6574 7572 6e5f 6469 6374 2c0a 2020 2020  eturn_dict,.    
+0001aaf0: 2020 2020 290a 0a20 2020 2020 2020 2073      )..        s
+0001ab00: 6571 7565 6e63 655f 6f75 7470 7574 203d  equence_output =
+0001ab10: 2072 6566 6f72 6d65 725f 6f75 7470 7574   reformer_output
+0001ab20: 735b 305d 0a0a 2020 2020 2020 2020 6c6f  s[0]..        lo
+0001ab30: 6769 7473 203d 2073 656c 662e 7161 5f6f  gits = self.qa_o
+0001ab40: 7574 7075 7473 2873 6571 7565 6e63 655f  utputs(sequence_
+0001ab50: 6f75 7470 7574 290a 2020 2020 2020 2020  output).        
+0001ab60: 7374 6172 745f 6c6f 6769 7473 2c20 656e  start_logits, en
+0001ab70: 645f 6c6f 6769 7473 203d 206c 6f67 6974  d_logits = logit
+0001ab80: 732e 7370 6c69 7428 312c 2064 696d 3d2d  s.split(1, dim=-
+0001ab90: 3129 0a20 2020 2020 2020 2073 7461 7274  1).        start
+0001aba0: 5f6c 6f67 6974 7320 3d20 7374 6172 745f  _logits = start_
+0001abb0: 6c6f 6769 7473 2e73 7175 6565 7a65 282d  logits.squeeze(-
+0001abc0: 3129 2e63 6f6e 7469 6775 6f75 7328 290a  1).contiguous().
+0001abd0: 2020 2020 2020 2020 656e 645f 6c6f 6769          end_logi
+0001abe0: 7473 203d 2065 6e64 5f6c 6f67 6974 732e  ts = end_logits.
+0001abf0: 7371 7565 657a 6528 2d31 292e 636f 6e74  squeeze(-1).cont
+0001ac00: 6967 756f 7573 2829 0a0a 2020 2020 2020  iguous()..      
+0001ac10: 2020 746f 7461 6c5f 6c6f 7373 203d 204e    total_loss = N
+0001ac20: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+0001ac30: 7461 7274 5f70 6f73 6974 696f 6e73 2069  tart_positions i
+0001ac40: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2065  s not None and e
+0001ac50: 6e64 5f70 6f73 6974 696f 6e73 2069 7320  nd_positions is 
+0001ac60: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0001ac70: 2020 2020 2020 2320 4966 2077 6520 6172        # If we ar
+0001ac80: 6520 6f6e 206d 756c 7469 2d47 5055 2c20  e on multi-GPU, 
+0001ac90: 7370 6c69 7420 6164 6420 6120 6469 6d65  split add a dime
+0001aca0: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
+0001acb0: 2020 6966 206c 656e 2873 7461 7274 5f70    if len(start_p
+0001acc0: 6f73 6974 696f 6e73 2e73 697a 6528 2929  ositions.size())
+0001acd0: 203e 2031 3a0a 2020 2020 2020 2020 2020   > 1:.          
+0001ace0: 2020 2020 2020 7374 6172 745f 706f 7369        start_posi
+0001acf0: 7469 6f6e 7320 3d20 7374 6172 745f 706f  tions = start_po
+0001ad00: 7369 7469 6f6e 732e 7371 7565 657a 6528  sitions.squeeze(
+0001ad10: 2d31 290a 2020 2020 2020 2020 2020 2020  -1).            
+0001ad20: 6966 206c 656e 2865 6e64 5f70 6f73 6974  if len(end_posit
+0001ad30: 696f 6e73 2e73 697a 6528 2929 203e 2031  ions.size()) > 1
+0001ad40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0001ad50: 2020 656e 645f 706f 7369 7469 6f6e 7320    end_positions 
+0001ad60: 3d20 656e 645f 706f 7369 7469 6f6e 732e  = end_positions.
+0001ad70: 7371 7565 657a 6528 2d31 290a 2020 2020  squeeze(-1).    
+0001ad80: 2020 2020 2020 2020 2320 736f 6d65 7469          # someti
+0001ad90: 6d65 7320 7468 6520 7374 6172 742f 656e  mes the start/en
+0001ada0: 6420 706f 7369 7469 6f6e 7320 6172 6520  d positions are 
+0001adb0: 6f75 7473 6964 6520 6f75 7220 6d6f 6465  outside our mode
+0001adc0: 6c20 696e 7075 7473 2c20 7765 2069 676e  l inputs, we ign
+0001add0: 6f72 6520 7468 6573 6520 7465 726d 730a  ore these terms.
+0001ade0: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
+0001adf0: 7265 645f 696e 6465 7820 3d20 7374 6172  red_index = star
+0001ae00: 745f 6c6f 6769 7473 2e73 697a 6528 3129  t_logits.size(1)
+0001ae10: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+0001ae20: 7274 5f70 6f73 6974 696f 6e73 203d 2073  rt_positions = s
+0001ae30: 7461 7274 5f70 6f73 6974 696f 6e73 2e63  tart_positions.c
+0001ae40: 6c61 6d70 2830 2c20 6967 6e6f 7265 645f  lamp(0, ignored_
+0001ae50: 696e 6465 7829 0a20 2020 2020 2020 2020  index).         
+0001ae60: 2020 2065 6e64 5f70 6f73 6974 696f 6e73     end_positions
+0001ae70: 203d 2065 6e64 5f70 6f73 6974 696f 6e73   = end_positions
+0001ae80: 2e63 6c61 6d70 2830 2c20 6967 6e6f 7265  .clamp(0, ignore
+0001ae90: 645f 696e 6465 7829 0a0a 2020 2020 2020  d_index)..      
+0001aea0: 2020 2020 2020 6c6f 7373 5f66 6374 203d        loss_fct =
+0001aeb0: 2043 726f 7373 456e 7472 6f70 794c 6f73   CrossEntropyLos
+0001aec0: 7328 6967 6e6f 7265 5f69 6e64 6578 3d69  s(ignore_index=i
+0001aed0: 676e 6f72 6564 5f69 6e64 6578 290a 2020  gnored_index).  
+0001aee0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
+0001aef0: 6c6f 7373 203d 206c 6f73 735f 6663 7428  loss = loss_fct(
+0001af00: 7374 6172 745f 6c6f 6769 7473 2c20 7374  start_logits, st
+0001af10: 6172 745f 706f 7369 7469 6f6e 7329 0a20  art_positions). 
+0001af20: 2020 2020 2020 2020 2020 2065 6e64 5f6c             end_l
+0001af30: 6f73 7320 3d20 6c6f 7373 5f66 6374 2865  oss = loss_fct(e
+0001af40: 6e64 5f6c 6f67 6974 732c 2065 6e64 5f70  nd_logits, end_p
+0001af50: 6f73 6974 696f 6e73 290a 2020 2020 2020  ositions).      
+0001af60: 2020 2020 2020 746f 7461 6c5f 6c6f 7373        total_loss
+0001af70: 203d 2028 7374 6172 745f 6c6f 7373 202b   = (start_loss +
+0001af80: 2065 6e64 5f6c 6f73 7329 202f 2032 0a0a   end_loss) / 2..
+0001af90: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
+0001afa0: 6574 7572 6e5f 6469 6374 3a0a 2020 2020  eturn_dict:.    
+0001afb0: 2020 2020 2020 2020 6f75 7470 7574 203d          output =
+0001afc0: 2028 7374 6172 745f 6c6f 6769 7473 2c20   (start_logits, 
+0001afd0: 656e 645f 6c6f 6769 7473 2920 2b20 7265  end_logits) + re
+0001afe0: 666f 726d 6572 5f6f 7574 7075 7473 5b31  former_outputs[1
+0001aff0: 3a5d 0a20 2020 2020 2020 2020 2020 2072  :].            r
+0001b000: 6574 7572 6e20 2828 746f 7461 6c5f 6c6f  eturn ((total_lo
+0001b010: 7373 2c29 202b 206f 7574 7075 7429 2069  ss,) + output) i
+0001b020: 6620 746f 7461 6c5f 6c6f 7373 2069 7320  f total_loss is 
+0001b030: 6e6f 7420 4e6f 6e65 2065 6c73 6520 6f75  not None else ou
+0001b040: 7470 7574 0a0a 2020 2020 2020 2020 7265  tput..        re
+0001b050: 7475 726e 2051 7565 7374 696f 6e41 6e73  turn QuestionAns
+0001b060: 7765 7269 6e67 4d6f 6465 6c4f 7574 7075  weringModelOutpu
+0001b070: 7428 0a20 2020 2020 2020 2020 2020 206c  t(.            l
+0001b080: 6f73 733d 746f 7461 6c5f 6c6f 7373 2c0a  oss=total_loss,.
+0001b090: 2020 2020 2020 2020 2020 2020 7374 6172              star
+0001b0a0: 745f 6c6f 6769 7473 3d73 7461 7274 5f6c  t_logits=start_l
+0001b0b0: 6f67 6974 732c 0a20 2020 2020 2020 2020  ogits,.         
+0001b0c0: 2020 2065 6e64 5f6c 6f67 6974 733d 656e     end_logits=en
+0001b0d0: 645f 6c6f 6769 7473 2c0a 2020 2020 2020  d_logits,.      
+0001b0e0: 2020 2020 2020 6869 6464 656e 5f73 7461        hidden_sta
+0001b0f0: 7465 733d 7265 666f 726d 6572 5f6f 7574  tes=reformer_out
+0001b100: 7075 7473 2e68 6964 6465 6e5f 7374 6174  puts.hidden_stat
+0001b110: 6573 2c0a 2020 2020 2020 2020 2020 2020  es,.            
+0001b120: 6174 7465 6e74 696f 6e73 3d72 6566 6f72  attentions=refor
+0001b130: 6d65 725f 6f75 7470 7574 732e 6174 7465  mer_outputs.atte
+0001b140: 6e74 696f 6e73 2c0a 2020 2020 2020 2020  ntions,.        
+0001b150: 290a                                     ).
```

### Comparing `transformers-4.9.1/src/transformers/models/reformer/tokenization_reformer.py` & `transformers-4.9.2/src/transformers/models/reformer/tokenization_reformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/reformer/tokenization_reformer_fast.py` & `transformers-4.9.2/src/transformers/models/reformer/tokenization_reformer_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/retribert/__init__.py` & `transformers-4.9.2/src/transformers/models/retribert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/retribert/configuration_retribert.py` & `transformers-4.9.2/src/transformers/models/retribert/configuration_retribert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/retribert/modeling_retribert.py` & `transformers-4.9.2/src/transformers/models/retribert/modeling_retribert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/retribert/tokenization_retribert.py` & `transformers-4.9.2/src/transformers/models/retribert/tokenization_retribert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/retribert/tokenization_retribert_fast.py` & `transformers-4.9.2/src/transformers/models/retribert/tokenization_retribert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/__init__.py` & `transformers-4.9.2/src/transformers/models/roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/configuration_roberta.py` & `transformers-4.9.2/src/transformers/models/roberta/configuration_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/roberta/convert_roberta_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/modeling_flax_roberta.py` & `transformers-4.9.2/src/transformers/models/roberta/modeling_flax_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/modeling_roberta.py` & `transformers-4.9.2/src/transformers/models/roberta/modeling_roberta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1120,30 +1120,32 @@
     """Roberta Head for masked language modeling."""
 
     def __init__(self, config):
         super().__init__()
         self.dense = nn.Linear(config.hidden_size, config.hidden_size)
         self.layer_norm = nn.LayerNorm(config.hidden_size, eps=config.layer_norm_eps)
 
-        self.decoder = nn.Linear(config.hidden_size, config.vocab_size, bias=False)
+        self.decoder = nn.Linear(config.hidden_size, config.vocab_size)
         self.bias = nn.Parameter(torch.zeros(config.vocab_size))
-
-        # Need a link between the two variables so that the bias is correctly resized with `resize_token_embeddings`
         self.decoder.bias = self.bias
 
     def forward(self, features, **kwargs):
         x = self.dense(features)
         x = gelu(x)
         x = self.layer_norm(x)
 
         # project back to size of vocabulary with bias
         x = self.decoder(x)
 
         return x
 
+    def _tie_weights(self):
+        # To tie those two weights if they get disconnected (on TPU or when the bias is resized)
+        self.bias = self.decoder.bias
+
 
 @add_start_docstrings(
     """
     RoBERTa Model transformer with a sequence classification/regression head on top (a linear layer on top of the
     pooled output) e.g. for GLUE tasks.
     """,
     ROBERTA_START_DOCSTRING,
```

### Comparing `transformers-4.9.1/src/transformers/models/roberta/modeling_tf_roberta.py` & `transformers-4.9.2/src/transformers/models/roberta/modeling_tf_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/tokenization_roberta.py` & `transformers-4.9.2/src/transformers/models/roberta/tokenization_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roberta/tokenization_roberta_fast.py` & `transformers-4.9.2/src/transformers/models/roberta/tokenization_roberta_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/__init__.py` & `transformers-4.9.2/src/transformers/models/roformer/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/configuration_roformer.py` & `transformers-4.9.2/src/transformers/models/roformer/configuration_roformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/roformer/convert_roformer_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/modeling_roformer.py` & `transformers-4.9.2/src/transformers/models/roformer/modeling_roformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/modeling_tf_roformer.py` & `transformers-4.9.2/src/transformers/models/roformer/modeling_tf_roformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/tokenization_roformer.py` & `transformers-4.9.2/src/transformers/models/roformer/tokenization_roformer.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/tokenization_roformer_fast.py` & `transformers-4.9.2/src/transformers/models/roformer/tokenization_roformer_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/roformer/tokenization_utils.py` & `transformers-4.9.2/src/transformers/models/roformer/tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/__init__.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/configuration_speech_to_text.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/configuration_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/convert_s2t_fairseq_to_tfms.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/feature_extraction_speech_to_text.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/feature_extraction_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/modeling_speech_to_text.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/modeling_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/processing_speech_to_text.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/processing_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/speech_to_text/tokenization_speech_to_text.py` & `transformers-4.9.2/src/transformers/models/speech_to_text/tokenization_speech_to_text.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/squeezebert/__init__.py` & `transformers-4.9.2/src/transformers/models/squeezebert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/squeezebert/configuration_squeezebert.py` & `transformers-4.9.2/src/transformers/models/squeezebert/configuration_squeezebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/squeezebert/modeling_squeezebert.py` & `transformers-4.9.2/src/transformers/models/squeezebert/modeling_squeezebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/squeezebert/tokenization_squeezebert.py` & `transformers-4.9.2/src/transformers/models/squeezebert/tokenization_squeezebert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/squeezebert/tokenization_squeezebert_fast.py` & `transformers-4.9.2/src/transformers/models/squeezebert/tokenization_squeezebert_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/t5/__init__.py` & `transformers-4.9.2/src/transformers/models/t5/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/t5/configuration_t5.py` & `transformers-4.9.2/src/transformers/models/t5/configuration_t5.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ T5 model configuration """
 from collections import OrderedDict
-from typing import Any, Mapping, Optional
+from typing import Any, Dict, Iterable, Mapping, Optional
 
 from transformers import PreTrainedTokenizer, TensorType
 
+from ... import is_torch_available
 from ...configuration_utils import PretrainedConfig
 from ...onnx import OnnxConfigWithPast
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)
 
@@ -136,67 +137,104 @@
 
     @property
     def num_hidden_layers(self):
         return self.num_layers
 
 
 class T5OnnxConfig(OnnxConfigWithPast):
-    def __init__(self, config: PretrainedConfig, use_past: bool = False):
-        super().__init__(config, use_past)
-
     @property
     def inputs(self) -> Mapping[str, Mapping[int, str]]:
         common_inputs = OrderedDict(
             [
                 ("input_ids", {0: "batch", 1: "encoder_sequence"}),
                 ("attention_mask", {0: "batch", 1: "encoder_sequence"}),
                 ("decoder_input_ids", {0: "batch"}),
                 ("decoder_attention_mask", {0: "batch"}),
             ]
         )
 
         if self.use_past:
-            for i in range(self._config.num_layers):
-                common_inputs[f"past_key_values.{i}.decoder.0"] = ({0: "batch", 2: "past_sequence"},)
-                common_inputs[f"past_key_values.{i}.decoder.1"] = ({0: "batch", 2: "past_sequence"},)
-                common_inputs[f"past_key_values.{i}.encoder.0"] = ({0: "batch", 2: "past_sequence"},)
-                common_inputs[f"past_key_values.{i}.encoder.1"] = ({0: "batch", 2: "past_sequence"},)
+            for i in range(0, self._config.num_layers):
+                common_inputs[f"past_key_values.{i}.decoder.key"] = {0: "batch", 2: "past_sequence"}
+                common_inputs[f"past_key_values.{i}.decoder.value"] = {0: "batch", 2: "past_sequence"}
+                common_inputs[f"past_key_values.{i}.encoder.key"] = {0: "batch", 2: "past_sequence"}
+                common_inputs[f"past_key_values.{i}.encoder.value"] = {0: "batch", 2: "past_sequence"}
 
         return common_inputs
 
     @property
     def outputs(self) -> Mapping[str, Mapping[int, str]]:
-        common_outputs = OrderedDict(
-            [
-                ("last_hidden_state", {0: "batch", 1: "decoder_sequence"}),
-                ("encoder_last_hidden_state", {0: "batch", 2: "encoder_sequence"}),
-            ]
-        )
+        common_outputs = super().outputs
+
+        if "last_hidden_state" in common_outputs:
+            common_outputs["last_hidden_state"] = {0: "batch", 1: "decoder_sequence"}
 
         if self.use_past:
             for i in range(self._config.num_layers):
-                common_outputs[f"past_key_values.{i}.decoder.0"] = ({0: "batch", 2: "decoder_sequence"},)
-                common_outputs[f"past_key_values.{i}.decoder.1"] = ({0: "batch", 2: "decoder_sequence"},)
-                common_outputs[f"past_key_values.{i}.encoder.0"] = ({0: "batch", 2: "encoder_sequence"},)
-                common_outputs[f"past_key_values.{i}.encoder.1"] = ({0: "batch", 2: "encoder_sequence"},)
+                common_outputs[f"present.{i}.decoder.key"] = {0: "batch", 2: "decoder_sequence"}
+                common_outputs[f"present.{i}.decoder.value"] = {0: "batch", 2: "decoder_sequence"}
+                common_outputs[f"present.{i}.encoder.key"] = {0: "batch", 2: "encoder_sequence"}
+                common_outputs[f"present.{i}.encoder.value"] = {0: "batch", 2: "encoder_sequence"}
+
+        if self.task == "default":
+            common_outputs["encoder_last_hidden_state"] = {0: "batch", 2: "encoder_sequence"}
 
         return common_outputs
 
     def generate_dummy_inputs(
         self,
         tokenizer: PreTrainedTokenizer,
         batch_size: int = -1,
         seq_length: int = -1,
         is_pair: bool = False,
         framework: Optional[TensorType] = None,
     ) -> Mapping[str, Any]:
-        if self.use_past:
-            raise NotImplementedError()
 
         # Generate encoder inputs
         encoder_inputs = super().generate_dummy_inputs(tokenizer, batch_size, seq_length, is_pair, framework)
 
         # Generate decoder inputs
         decoder_inputs = super().generate_dummy_inputs(tokenizer, batch_size, 1, is_pair, framework)
         decoder_inputs = {f"decoder_{name}": tensor for name, tensor in decoder_inputs.items()}
 
-        return dict(**encoder_inputs, **decoder_inputs)
+        ordered_inputs = dict(**encoder_inputs, **decoder_inputs)
+        if self.use_past:
+            if not is_torch_available():
+                raise ValueError("Cannot generate dummy past_keys inputs without PyTorch installed.")
+            else:
+                import torch
+            batch = encoder_inputs["input_ids"].shape[0]
+            encoder_seq_length = encoder_inputs["input_ids"].shape[1]
+            encoder_shape = (
+                batch,
+                self._config.num_heads,
+                encoder_seq_length,
+                self._config.hidden_size // self._config.num_heads,
+            )
+            decoder_shape = (batch, self._config.num_heads, 1, self._config.hidden_size // self._config.num_heads)
+
+            ordered_inputs["past_key_values"] = []
+            for _ in range(self._config.num_layers):
+                ordered_inputs["past_key_values"].append(
+                    (
+                        torch.zeros(decoder_shape),
+                        torch.zeros(decoder_shape),
+                        torch.zeros(encoder_shape),
+                        torch.zeros(encoder_shape),
+                    )
+                )
+
+        return ordered_inputs
+
+    @staticmethod
+    def flatten_output_collection_property(name: str, field: Iterable[Any]) -> Dict[str, Any]:
+        if name in ["present", "past_key_values"]:
+            flatten_output = {}
+            for idx, t in enumerate(field):
+                flatten_output[f"{name}.{idx}.decoder.key"] = t[0]
+                flatten_output[f"{name}.{idx}.decoder.value"] = t[1]
+                flatten_output[f"{name}.{idx}.encoder.key"] = t[2]
+                flatten_output[f"{name}.{idx}.encoder.value"] = t[3]
+
+            return flatten_output
+
+        return super().flatten_output_collection_property(name, field)
```

### Comparing `transformers-4.9.1/src/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/t5/convert_t5_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/t5/modeling_flax_t5.py` & `transformers-4.9.2/src/transformers/models/t5/modeling_flax_t5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/t5/modeling_t5.py` & `transformers-4.9.2/src/transformers/models/t5/modeling_t5.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,16 +422,14 @@
         Self-attention (if key_value_states is None) or attention over source sentence (provided by key_value_states).
         """
         # Input is (batch_size, seq_length, dim)
         # Mask is (batch_size, key_length) (non-causal) or (batch_size, key_length, key_length)
         # past_key_value[0] is (batch_size, n_heads, q_len - 1, dim_per_head)
         batch_size, seq_length = hidden_states.shape[:2]
 
-        int_seq_length = int(seq_length)
-
         real_seq_length = seq_length
 
         if past_key_value is not None:
             assert (
                 len(past_key_value) == 2
             ), f"past_key_value should have 2 past states: keys and values. Got { len(past_key_value)} past states"
             real_seq_length += past_key_value[0].shape[2] if query_length is None else query_length
@@ -492,15 +490,15 @@
                     position_bias.requires_grad = True
             else:
                 position_bias = self.compute_bias(real_seq_length, key_length)
 
             # if key and values are already calculated
             # we want only the last query position bias
             if past_key_value is not None:
-                position_bias = position_bias[:, :, -int_seq_length:, :]
+                position_bias = position_bias[:, :, -hidden_states.size(1) :, :]
 
             if mask is not None:
                 position_bias = position_bias + mask  # (batch_size, n_heads, seq_length, key_length)
 
         scores += position_bias
         attn_weights = nn.functional.softmax(scores.float(), dim=-1).type_as(
             scores
@@ -622,15 +620,15 @@
         if past_key_value is not None:
             assert self.is_decoder, "Only decoder can use `past_key_values`"
             expected_num_past_key_values = 2 if encoder_hidden_states is None else 4
 
             if len(past_key_value) != expected_num_past_key_values:
                 raise ValueError(
                     f"There should be {expected_num_past_key_values} past states. "
-                    f"{'2 (past / key) for cross attention' if expected_num_past_key_values == 4 else ''}."
+                    f"{'2 (past / key) for cross attention. ' if expected_num_past_key_values == 4 else ''}"
                     f"Got {len(past_key_value)} past key / value states"
                 )
 
             self_attn_past_key_value = past_key_value[:2]
             cross_attn_past_key_value = past_key_value[2:]
         else:
             self_attn_past_key_value, cross_attn_past_key_value = None, None
```

### Comparing `transformers-4.9.1/src/transformers/models/t5/modeling_tf_t5.py` & `transformers-4.9.2/src/transformers/models/t5/modeling_tf_t5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/t5/tokenization_t5.py` & `transformers-4.9.2/src/transformers/models/t5/tokenization_t5.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/t5/tokenization_t5_fast.py` & `transformers-4.9.2/src/transformers/models/t5/tokenization_t5_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/tapas/__init__.py` & `transformers-4.9.2/src/transformers/models/tapas/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/tapas/configuration_tapas.py` & `transformers-4.9.2/src/transformers/models/tapas/configuration_tapas.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/tapas/convert_tapas_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/tapas/modeling_tapas.py` & `transformers-4.9.2/src/transformers/models/tapas/modeling_tapas.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/tapas/tokenization_tapas.py` & `transformers-4.9.2/src/transformers/models/tapas/tokenization_tapas.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/__init__.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/configuration_transfo_xl.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/configuration_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/convert_transfo_xl_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/modeling_tf_transfo_xl.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/modeling_tf_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/modeling_tf_transfo_xl_utilities.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/modeling_transfo_xl.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/modeling_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/modeling_transfo_xl_utilities.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/transfo_xl/tokenization_transfo_xl.py` & `transformers-4.9.2/src/transformers/models/transfo_xl/tokenization_transfo_xl.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/visual_bert/__init__.py` & `transformers-4.9.2/src/transformers/models/visual_bert/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/visual_bert/configuration_visual_bert.py` & `transformers-4.9.2/src/transformers/models/visual_bert/configuration_visual_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/visual_bert/convert_visual_bert_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/visual_bert/modeling_visual_bert.py` & `transformers-4.9.2/src/transformers/models/visual_bert/modeling_visual_bert.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/vit/__init__.py` & `transformers-4.9.2/src/transformers/models/vit/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/vit/configuration_vit.py` & `transformers-4.9.2/src/transformers/models/vit/configuration_vit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/vit/convert_vit_timm_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/vit/convert_vit_timm_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/vit/feature_extraction_vit.py` & `transformers-4.9.2/src/transformers/models/vit/feature_extraction_vit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/vit/modeling_flax_vit.py` & `transformers-4.9.2/src/transformers/models/vit/modeling_flax_vit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/vit/modeling_vit.py` & `transformers-4.9.2/src/transformers/models/vit/modeling_vit.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/__init__.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/configuration_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/configuration_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/convert_wav2vec2_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/feature_extraction_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/feature_extraction_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/modeling_flax_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/modeling_flax_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/modeling_tf_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/modeling_tf_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/modeling_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/modeling_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/processing_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/processing_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/wav2vec2/tokenization_wav2vec2.py` & `transformers-4.9.2/src/transformers/models/wav2vec2/tokenization_wav2vec2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm/__init__.py` & `transformers-4.9.2/src/transformers/models/xlm/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm/configuration_xlm.py` & `transformers-4.9.2/src/transformers/models/xlnet/configuration_xlnet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,88 @@
 # coding=utf-8
-# Copyright 2019-present, Facebook, Inc and the HuggingFace Inc. team.
+# Copyright 2018 Google AI, Google Brain and Carnegie Mellon University Authors and the HuggingFace Inc. team.
+# Copyright (c) 2018, NVIDIA CORPORATION.  All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-""" XLM configuration """
+""" XLNet configuration """
+
+import warnings
 
 from ...configuration_utils import PretrainedConfig
 from ...utils import logging
 
 
 logger = logging.get_logger(__name__)
 
-XLM_PRETRAINED_CONFIG_ARCHIVE_MAP = {
-    "xlm-mlm-en-2048": "https://huggingface.co/xlm-mlm-en-2048/resolve/main/config.json",
-    "xlm-mlm-ende-1024": "https://huggingface.co/xlm-mlm-ende-1024/resolve/main/config.json",
-    "xlm-mlm-enfr-1024": "https://huggingface.co/xlm-mlm-enfr-1024/resolve/main/config.json",
-    "xlm-mlm-enro-1024": "https://huggingface.co/xlm-mlm-enro-1024/resolve/main/config.json",
-    "xlm-mlm-tlm-xnli15-1024": "https://huggingface.co/xlm-mlm-tlm-xnli15-1024/resolve/main/config.json",
-    "xlm-mlm-xnli15-1024": "https://huggingface.co/xlm-mlm-xnli15-1024/resolve/main/config.json",
-    "xlm-clm-enfr-1024": "https://huggingface.co/xlm-clm-enfr-1024/resolve/main/config.json",
-    "xlm-clm-ende-1024": "https://huggingface.co/xlm-clm-ende-1024/resolve/main/config.json",
-    "xlm-mlm-17-1280": "https://huggingface.co/xlm-mlm-17-1280/resolve/main/config.json",
-    "xlm-mlm-100-1280": "https://huggingface.co/xlm-mlm-100-1280/resolve/main/config.json",
+XLNET_PRETRAINED_CONFIG_ARCHIVE_MAP = {
+    "xlnet-base-cased": "https://huggingface.co/xlnet-base-cased/resolve/main/config.json",
+    "xlnet-large-cased": "https://huggingface.co/xlnet-large-cased/resolve/main/config.json",
 }
 
 
-class XLMConfig(PretrainedConfig):
+class XLNetConfig(PretrainedConfig):
     """
-    This is the configuration class to store the configuration of a :class:`~transformers.XLMModel` or a
-    :class:`~transformers.TFXLMModel`. It is used to instantiate a XLM model according to the specified arguments,
+    This is the configuration class to store the configuration of a :class:`~transformers.XLNetModel` or a
+    :class:`~transformers.TFXLNetModel`. It is used to instantiate a XLNet model according to the specified arguments,
     defining the model architecture. Instantiating a configuration with the defaults will yield a similar configuration
-    to that of the `xlm-mlm-en-2048 <https://huggingface.co/xlm-mlm-en-2048>`__ architecture.
+    to that of the `xlnet-large-cased <https://huggingface.co/xlnet-large-cased>`__ architecture.
 
     Configuration objects inherit from :class:`~transformers.PretrainedConfig` and can be used to control the model
     outputs. Read the documentation from :class:`~transformers.PretrainedConfig` for more information.
 
     Args:
-        vocab_size (:obj:`int`, `optional`, defaults to 30145):
-            Vocabulary size of the BERT model. Defines the number of different tokens that can be represented by the
-            :obj:`inputs_ids` passed when calling :class:`~transformers.XLMModel` or :class:`~transformers.TFXLMModel`.
-        emb_dim (:obj:`int`, `optional`, defaults to 2048):
+        vocab_size (:obj:`int`, `optional`, defaults to 32000):
+            Vocabulary size of the XLNet model. Defines the number of different tokens that can be represented by the
+            :obj:`inputs_ids` passed when calling :class:`~transformers.XLNetModel` or
+            :class:`~transformers.TFXLNetModel`.
+        d_model (:obj:`int`, `optional`, defaults to 1024):
             Dimensionality of the encoder layers and the pooler layer.
-        n_layer (:obj:`int`, `optional`, defaults to 12):
+        n_layer (:obj:`int`, `optional`, defaults to 24):
             Number of hidden layers in the Transformer encoder.
         n_head (:obj:`int`, `optional`, defaults to 16):
             Number of attention heads for each attention layer in the Transformer encoder.
-        dropout (:obj:`float`, `optional`, defaults to 0.1):
-            The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
-        attention_dropout (:obj:`float`, `optional`, defaults to 0.1):
-            The dropout probability for the attention mechanism
-        gelu_activation (:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Whether or not to use `gelu` for the activations instead of `relu`.
-        sinusoidal_embeddings (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            Whether or not to use sinusoidal positional embeddings instead of absolute positional embeddings.
-        causal (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            Whether or not the model should behave in a causal manner. Causal models use a triangular attention mask in
-            order to only attend to the left-side context instead if a bidirectional context.
-        asm (:obj:`bool`, `optional`, defaults to :obj:`False`):
-            Whether or not to use an adaptive log softmax projection layer instead of a linear layer for the prediction
-            layer.
-        n_langs (:obj:`int`, `optional`, defaults to 1):
-            The number of languages the model handles. Set to 1 for monolingual models.
-        use_lang_emb (:obj:`bool`, `optional`, defaults to :obj:`True`)
-            Whether to use language embeddings. Some models use additional language embeddings, see `the multilingual
-            models page <http://huggingface.co/transformers/multilingual.html#xlm-language-embeddings>`__ for
-            information on how to use them.
-        max_position_embeddings (:obj:`int`, `optional`, defaults to 512):
-            The maximum sequence length that this model might ever be used with. Typically set this to something large
-            just in case (e.g., 512 or 1024 or 2048).
-        embed_init_std (:obj:`float`, `optional`, defaults to 2048^-0.5):
-            The standard deviation of the truncated_normal_initializer for initializing the embedding matrices.
-        init_std (:obj:`int`, `optional`, defaults to 50257):
-            The standard deviation of the truncated_normal_initializer for initializing all weight matrices except the
-            embedding matrices.
+        d_inner (:obj:`int`, `optional`, defaults to 4096):
+            Dimensionality of the "intermediate" (often named feed-forward) layer in the Transformer encoder.
+        ff_activation (:obj:`str` or :obj:`Callable`, `optional`, defaults to :obj:`"gelu"`):
+            The non-linear activation function (function or string) in the If string, :obj:`"gelu"`, :obj:`"relu"`,
+            :obj:`"silu"` and :obj:`"gelu_new"` are supported.
+        untie_r (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Whether or not to untie relative position biases
+        attn_type (:obj:`str`, `optional`, defaults to :obj:`"bi"`):
+            The attention type used by the model. Set :obj:`"bi"` for XLNet, :obj:`"uni"` for Transformer-XL.
+        initializer_range (:obj:`float`, `optional`, defaults to 0.02):
+            The standard deviation of the truncated_normal_initializer for initializing all weight matrices.
         layer_norm_eps (:obj:`float`, `optional`, defaults to 1e-12):
             The epsilon used by the layer normalization layers.
-        bos_index (:obj:`int`, `optional`, defaults to 0):
-            The index of the beginning of sentence token in the vocabulary.
-        eos_index (:obj:`int`, `optional`, defaults to 1):
-            The index of the end of sentence token in the vocabulary.
-        pad_index (:obj:`int`, `optional`, defaults to 2):
-            The index of the padding token in the vocabulary.
-        unk_index (:obj:`int`, `optional`, defaults to 3):
-            The index of the unknown token in the vocabulary.
-        mask_index (:obj:`int`, `optional`, defaults to 5):
-            The index of the masking token in the vocabulary.
-        is_encoder(:obj:`bool`, `optional`, defaults to :obj:`True`):
-            Whether or not the initialized model should be a transformer encoder or decoder as seen in Vaswani et al.
-        summary_type (:obj:`string`, `optional`, defaults to "first"):
+        dropout (:obj:`float`, `optional`, defaults to 0.1):
+            The dropout probability for all fully connected layers in the embeddings, encoder, and pooler.
+        mem_len (:obj:`int` or :obj:`None`, `optional`):
+            The number of tokens to cache. The key/value pairs that have already been pre-computed in a previous
+            forward pass won't be re-computed. See the `quickstart
+            <https://huggingface.co/transformers/quickstart.html#using-the-past>`__ for more information.
+        reuse_len (:obj:`int`, `optional`):
+            The number of tokens in the current batch to be cached and reused in the future.
+        bi_data (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            Whether or not to use bidirectional input pipeline. Usually set to :obj:`True` during pretraining and
+            :obj:`False` during finetuning.
+        clamp_len (:obj:`int`, `optional`, defaults to -1):
+            Clamp all relative distances larger than clamp_len. Setting this attribute to -1 means no clamping.
+        same_length (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            Whether or not to use the same attention length for each token.
+        summary_type (:obj:`str`, `optional`, defaults to "last"):
             Argument used when doing sequence summary. Used in the sequence classification and multiple choice models.
 
             Has to be one of the following options:
 
                 - :obj:`"last"`: Take the last token hidden state (like XLNet).
                 - :obj:`"first"`: Take the first token hidden state (like BERT).
                 - :obj:`"mean"`: Take the mean of all tokens hidden states.
@@ -110,133 +92,151 @@
             Argument used when doing sequence summary. Used in the sequence classification and multiple choice models.
 
             Whether or not to add a projection after the vector extraction.
         summary_activation (:obj:`str`, `optional`):
             Argument used when doing sequence summary. Used in the sequence classification and multiple choice models.
 
             Pass :obj:`"tanh"` for a tanh activation to the output, any other value will result in no activation.
-        summary_proj_to_labels (:obj:`bool`, `optional`, defaults to :obj:`True`):
+        summary_proj_to_labels (:obj:`boo`, `optional`, defaults to :obj:`True`):
             Used in the sequence classification and multiple choice models.
 
             Whether the projection outputs should have :obj:`config.num_labels` or :obj:`config.hidden_size` classes.
-        summary_first_dropout (:obj:`float`, `optional`, defaults to 0.1):
+        summary_last_dropout (:obj:`float`, `optional`, defaults to 0.1):
             Used in the sequence classification and multiple choice models.
 
             The dropout ratio to be used after the projection and activation.
         start_n_top (:obj:`int`, `optional`, defaults to 5):
             Used in the SQuAD evaluation script.
         end_n_top (:obj:`int`, `optional`, defaults to 5):
             Used in the SQuAD evaluation script.
-        mask_token_id (:obj:`int`, `optional`, defaults to 0):
-            Model agnostic parameter to identify masked tokens when generating text in an MLM context.
-        lang_id (:obj:`int`, `optional`, defaults to 1):
-            The ID of the language used by the model. This parameter is used when generating text in a given language.
+        use_mems_eval (:obj:`bool`, `optional`, defaults to :obj:`True`):
+            Whether or not the model should make use of the recurrent memory mechanism in evaluation mode.
+        use_mems_train (:obj:`bool`, `optional`, defaults to :obj:`False`):
+            Whether or not the model should make use of the recurrent memory mechanism in train mode.
+
+            .. note::
+                For pretraining, it is recommended to set ``use_mems_train`` to :obj:`True`. For fine-tuning, it is
+                recommended to set ``use_mems_train`` to :obj:`False` as discussed `here
+                <https://github.com/zihangdai/xlnet/issues/41#issuecomment-505102587>`__. If ``use_mems_train`` is set
+                to :obj:`True`, one has to make sure that the train batches are correctly pre-processed, `e.g.`
+                :obj:`batch_1 = [[This line is], [This is the]]` and :obj:`batch_2 = [[ the first line], [ second
+                line]]` and that all batches are of equal size.
 
     Examples::
 
-        >>> from transformers import XLMConfig, XLMModel
+        >>> from transformers import XLNetConfig, XLNetModel
 
-        >>> # Initializing a XLM configuration
-        >>> configuration = XLMConfig()
+        >>> # Initializing a XLNet configuration
+        >>> configuration = XLNetConfig()
 
         >>> # Initializing a model from the configuration
-        >>> model = XLMModel(configuration)
+        >>> model = XLNetModel(configuration)
 
         >>> # Accessing the model configuration
         >>> configuration = model.config
     """
 
-    model_type = "xlm"
+    model_type = "xlnet"
+    keys_to_ignore_at_inference = ["mems"]
 
     def __init__(
         self,
-        vocab_size=30145,
-        emb_dim=2048,
-        n_layers=12,
-        n_heads=16,
-        dropout=0.1,
-        attention_dropout=0.1,
-        gelu_activation=True,
-        sinusoidal_embeddings=False,
-        causal=False,
-        asm=False,
-        n_langs=1,
-        use_lang_emb=True,
-        max_position_embeddings=512,
-        embed_init_std=2048 ** -0.5,
+        vocab_size=32000,
+        d_model=1024,
+        n_layer=24,
+        n_head=16,
+        d_inner=4096,
+        ff_activation="gelu",
+        untie_r=True,
+        attn_type="bi",
+        initializer_range=0.02,
         layer_norm_eps=1e-12,
-        init_std=0.02,
-        bos_index=0,
-        eos_index=1,
-        pad_index=2,
-        unk_index=3,
-        mask_index=5,
-        is_encoder=True,
-        summary_type="first",
+        dropout=0.1,
+        mem_len=512,
+        reuse_len=None,
+        use_mems_eval=True,
+        use_mems_train=False,
+        bi_data=False,
+        clamp_len=-1,
+        same_length=False,
+        summary_type="last",
         summary_use_proj=True,
-        summary_activation=None,
-        summary_proj_to_labels=True,
-        summary_first_dropout=0.1,
+        summary_activation="tanh",
+        summary_last_dropout=0.1,
         start_n_top=5,
         end_n_top=5,
-        mask_token_id=0,
-        lang_id=0,
-        pad_token_id=2,
-        bos_token_id=0,
+        pad_token_id=5,
+        bos_token_id=1,
+        eos_token_id=2,
         **kwargs
     ):
-        """Constructs XLMConfig."""
-        super().__init__(pad_token_id=pad_token_id, bos_token_id=bos_token_id, **kwargs)
+        """Constructs XLNetConfig."""
+        super().__init__(pad_token_id=pad_token_id, bos_token_id=bos_token_id, eos_token_id=eos_token_id, **kwargs)
         self.vocab_size = vocab_size
-        self.emb_dim = emb_dim
-        self.n_layers = n_layers
-        self.n_heads = n_heads
-        self.dropout = dropout
-        self.attention_dropout = attention_dropout
-        self.gelu_activation = gelu_activation
-        self.sinusoidal_embeddings = sinusoidal_embeddings
-        self.causal = causal
-        self.asm = asm
-        self.n_langs = n_langs
-        self.use_lang_emb = use_lang_emb
+        self.d_model = d_model
+        self.n_layer = n_layer
+        self.n_head = n_head
+        assert d_model % n_head == 0
+        if "d_head" in kwargs:
+            assert (
+                kwargs["d_head"] == d_model // n_head
+            ), f"`d_head` ({kwargs['d_head']}) should be equal to `d_model // n_head` ({d_model // n_head})"
+        self.d_head = d_model // n_head
+        self.ff_activation = ff_activation
+        self.d_inner = d_inner
+        self.untie_r = untie_r
+        self.attn_type = attn_type
+
+        self.initializer_range = initializer_range
         self.layer_norm_eps = layer_norm_eps
-        self.bos_index = bos_index
-        self.eos_index = eos_index
-        self.pad_index = pad_index
-        self.unk_index = unk_index
-        self.mask_index = mask_index
-        self.is_encoder = is_encoder
-        self.max_position_embeddings = max_position_embeddings
-        self.embed_init_std = embed_init_std
-        self.init_std = init_std
+
+        self.dropout = dropout
+        self.mem_len = mem_len
+        self.reuse_len = reuse_len
+        self.bi_data = bi_data
+        self.clamp_len = clamp_len
+        self.same_length = same_length
+
         self.summary_type = summary_type
         self.summary_use_proj = summary_use_proj
         self.summary_activation = summary_activation
-        self.summary_proj_to_labels = summary_proj_to_labels
-        self.summary_first_dropout = summary_first_dropout
+        self.summary_last_dropout = summary_last_dropout
         self.start_n_top = start_n_top
         self.end_n_top = end_n_top
-        self.mask_token_id = mask_token_id
-        self.lang_id = lang_id
 
-        if "n_words" in kwargs:
-            self.n_words = kwargs["n_words"]
+        self.bos_token_id = bos_token_id
+        self.pad_token_id = pad_token_id
+        self.eos_token_id = eos_token_id
+
+        if "use_cache" in kwargs:
+            warnings.warn(
+                "The `use_cache` argument is deprecated and will be removed in a future version, use `use_mems_eval` instead.",
+                FutureWarning,
+            )
+            use_mems_eval = kwargs["use_cache"]
+
+        self.use_mems_eval = use_mems_eval
+        self.use_mems_train = use_mems_train
+
+    @property
+    def max_position_embeddings(self):
+        return -1
 
     @property
-    def n_words(self):  # For backward compatibility
+    def n_token(self):  # Backward compatibility
         return self.vocab_size
 
-    @n_words.setter
-    def n_words(self, value):  # For backward compatibility
+    @n_token.setter
+    def n_token(self, value):  # Backward compatibility
         self.vocab_size = value
 
     @property
     def hidden_size(self):
-        return self.emb_dim
+        return self.d_model
 
     @property
     def num_attention_heads(self):
-        return self.n_heads
+        return self.n_head
 
     @property
     def num_hidden_layers(self):
-        return self.n_layers
+        return self.n_layer
```

### Comparing `transformers-4.9.1/src/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/xlm/convert_xlm_original_pytorch_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm/modeling_tf_xlm.py` & `transformers-4.9.2/src/transformers/models/xlm/modeling_tf_xlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm/modeling_xlm.py` & `transformers-4.9.2/src/transformers/models/xlm/modeling_xlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm/tokenization_xlm.py` & `transformers-4.9.2/src/transformers/models/xlm/tokenization_xlm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_prophetnet/__init__.py` & `transformers-4.9.2/src/transformers/models/xlm_prophetnet/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py` & `transformers-4.9.2/src/transformers/models/xlm_prophetnet/configuration_xlm_prophetnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py` & `transformers-4.9.2/src/transformers/models/xlm_prophetnet/modeling_xlm_prophetnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py` & `transformers-4.9.2/src/transformers/models/xlm_prophetnet/tokenization_xlm_prophetnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_roberta/__init__.py` & `transformers-4.9.2/src/transformers/models/xlm_roberta/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_roberta/configuration_xlm_roberta.py` & `transformers-4.9.2/src/transformers/models/xlm_roberta/configuration_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py` & `transformers-4.9.2/src/transformers/models/xlm_roberta/modeling_tf_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_roberta/modeling_xlm_roberta.py` & `transformers-4.9.2/src/transformers/models/xlm_roberta/modeling_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_roberta/tokenization_xlm_roberta.py` & `transformers-4.9.2/src/transformers/models/xlm_roberta/tokenization_xlm_roberta.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py` & `transformers-4.9.2/src/transformers/models/xlm_roberta/tokenization_xlm_roberta_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlnet/__init__.py` & `transformers-4.9.2/src/transformers/models/xlnet/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py` & `transformers-4.9.2/src/transformers/models/xlnet/convert_xlnet_original_tf_checkpoint_to_pytorch.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlnet/modeling_tf_xlnet.py` & `transformers-4.9.2/src/transformers/models/xlnet/modeling_tf_xlnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlnet/modeling_xlnet.py` & `transformers-4.9.2/src/transformers/models/xlnet/modeling_xlnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlnet/tokenization_xlnet.py` & `transformers-4.9.2/src/transformers/models/xlnet/tokenization_xlnet.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/models/xlnet/tokenization_xlnet_fast.py` & `transformers-4.9.2/src/transformers/models/xlnet/tokenization_xlnet_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/onnx/__init__.py` & `transformers-4.9.2/src/transformers/onnx/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,10 +9,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .config import EXTERNAL_DATA_FORMAT_SIZE_LIMIT, OnnxConfig, OnnxConfigWithPast
+from .config import EXTERNAL_DATA_FORMAT_SIZE_LIMIT, OnnxConfig, OnnxConfigWithPast, PatchingSpec
 from .convert import export, validate_model_outputs
 from .utils import ParameterFormat, compute_serialized_parameters_size
```

### Comparing `transformers-4.9.1/src/transformers/onnx/config.py` & `transformers-4.9.2/src/transformers/pipelines/text_generation.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,223 +1,191 @@
-# Copyright 2021 The HuggingFace Team. All rights reserved.
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-from abc import ABC, abstractmethod
-from collections import OrderedDict
-from typing import Any, Mapping, Optional
-
-from transformers import PretrainedConfig, PreTrainedTokenizer, TensorType
-
-from .utils import ParameterFormat, compute_effective_axis_dimension, compute_serialized_parameters_size
+from ..file_utils import add_end_docstrings
+from .base import PIPELINE_INIT_ARGS, Pipeline
 
 
-DEFAULT_ONNX_OPSET = 11
-
-# 2 Gb
-EXTERNAL_DATA_FORMAT_SIZE_LIMIT = 2 * 1024 * 1024 * 1024
-
-
-class OnnxConfig(ABC):
-    """
-    Base class for ONNX exportable model describing metadata on how to export the model through the ONNX format.
+@add_end_docstrings(PIPELINE_INIT_ARGS)
+class TextGenerationPipeline(Pipeline):
     """
+    Language generation pipeline using any :obj:`ModelWithLMHead`. This pipeline predicts the words that will follow a
+    specified text prompt.
 
-    DEFAULT_FIXED_BATCH = 2
-    DEFAULT_FIXED_SEQUENCE = 8
-
-    def __init__(self, config: PretrainedConfig):
-        self._config = config
-
-    @classmethod
-    def default(cls, config: PretrainedConfig) -> "OnnxConfig":
-        """
-        Instantiate a OnnxConfig for a specific model
-
-        Args:
-            config: The model's configuration to use when exporting to ONNX
-
-        Returns:
-            OnnxConfig for this model
-        """
-        return cls(config)
-
-    @property
-    @abstractmethod
-    def inputs(self) -> Mapping[str, Mapping[int, str]]:
-        """
-        Mapping containing the axis definition of the input tensors to provide to the model
-
-        Returns:
-            For each input: its name associated to the axes symbolic name and the axis position within the tensor
-        """
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def outputs(self) -> Mapping[str, Mapping[int, str]]:
-        """
-        Mapping containing the axis definition of the output tensors to provide to the model
-
-        Returns:
-            For each output: its name associated to the axes symbolic name and the axis position within the tensor
-        """
-        raise NotImplementedError()
-
-    @property
-    def values_override(self) -> Optional[Mapping[str, Any]]:
-        """
-        Dictionary of keys to override in the model's config before exporting
-
-        Returns:
-            Dictionary with the keys (and their corresponding values) to override
-        """
-        if hasattr(self._config, "use_cache"):
-            return {"use_cache": False}
-
-        return None
-
-    @property
-    def default_batch_size(self) -> int:
-        """
-        The default batch size to use if no other indication
+    This language generation pipeline can currently be loaded from :func:`~transformers.pipeline` using the following
+    task identifier: :obj:`"text-generation"`.
 
-        Returns:
-            Integer > 0
-        """
-        # Using 2 avoid ONNX making assumption about single sample batch
-        return OnnxConfig.DEFAULT_FIXED_BATCH
-
-    @property
-    def default_sequence_length(self) -> int:
-        """
-        The default sequence length to use if no other indication
-
-        Returns:
-            Integer > 0
-        """
-        return OnnxConfig.DEFAULT_FIXED_SEQUENCE
-
-    @property
-    def default_onnx_opset(self) -> int:
-        """
-        Which onnx opset to use when exporting the model
-
-        Returns:
-            Integer ONNX Opset version
-        """
-        return DEFAULT_ONNX_OPSET
-
-    @staticmethod
-    def use_external_data_format(num_parameters: int) -> bool:
-        """
-        Flag indicating if the model requires using external data format
+    The models that this pipeline can use are models that have been trained with an autoregressive language modeling
+    objective, which includes the uni-directional models in the library (e.g. gpt2). See the list of available models
+    on `huggingface.co/models <https://huggingface.co/models?filter=causal-lm>`__.
+    """
 
-        Args:
-            num_parameters: Number of parameter on the model
+    # Prefix text to help Transformer-XL and XLNet with short prompts as proposed by Aman Rusia
+    # in https://github.com/rusiaaman/XLNet-gen#methodology
+    # and https://medium.com/@amanrusia/xlnet-speaks-comparison-to-gpt-2-ea1a4e9ba39e
+
+    XL_PREFIX = """
+    In 1991, the remains of Russian Tsar Nicholas II and his family (except for Alexei and Maria) are discovered. The
+    voice of Nicholas's young son, Tsarevich Alexei Nikolaevich, narrates the remainder of the story. 1883 Western
+    Siberia, a young Grigori Rasputin is asked by his father and a group of men to perform magic. Rasputin has a vision
+    and denounces one of the men as a horse thief. Although his father initially slaps him for making such an
+    accusation, Rasputin watches as the man is chased outside and beaten. Twenty years later, Rasputin sees a vision of
+    the Virgin Mary, prompting him to become a priest. Rasputin quickly becomes famous, with people, even a bishop,
+    begging for his blessing. <eod> </s> <eos>
+    """
 
-        Returns:
-            True if model.num_parameters() * size_of(float32) >= 2Gb False otherwise
-        """
+    ALLOWED_MODELS = [
+        "XLNetLMHeadModel",
+        "TransfoXLLMHeadModel",
+        "ReformerModelWithLMHead",
+        "GPT2LMHeadModel",
+        "GPTNeoForCausalLM",
+        "OpenAIGPTLMHeadModel",
+        "CTRLLMHeadModel",
+        "TFXLNetLMHeadModel",
+        "TFTransfoXLLMHeadModel",
+        "TFGPT2LMHeadModel",
+        "TFOpenAIGPTLMHeadModel",
+        "TFCTRLLMHeadModel",
+    ]
+
+    def __init__(self, *args, return_full_text=True, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.check_model_type(self.ALLOWED_MODELS)
+        self.return_full_text = return_full_text
+
+    # overriding _parse_and_tokenize to allow for unusual language-modeling tokenizer arguments
+    def _parse_and_tokenize(self, *args, **kwargs):
+        """
+        Parse arguments and tokenize
+        """
+        # Parse arguments
+        if self.model.__class__.__name__ in ["TransfoXLLMHeadModel"]:
+            kwargs.update({"add_space_before_punct_symbol": True})
 
-        return (
-            compute_serialized_parameters_size(num_parameters, ParameterFormat.Float)
-            >= EXTERNAL_DATA_FORMAT_SIZE_LIMIT
-        )
+        return super()._parse_and_tokenize(*args, **kwargs)
 
-    def generate_dummy_inputs(
+    def __call__(
         self,
-        tokenizer: PreTrainedTokenizer,
-        batch_size: int = -1,
-        seq_length: int = -1,
-        is_pair: bool = False,
-        framework: Optional[TensorType] = None,
-    ) -> Mapping[str, Any]:
-        """
-        Generate inputs to provide to the ONNX exporter for the specific framework
-
-        Args:
-            tokenizer: The tokenizer associated with this model configuration
-            batch_size: The batch size (int) to export the model for (-1 means dynamic axis)
-            seq_length: The sequence length (int) to export the model for (-1 means dynamic axis)
-            is_pair: Indicate if the input is a pair (sentence 1, sentence 2)
-            framework: The framework (optional) the tokenizer will generate tensor for
-
-        Returns:
-            Mapping[str, Tensor] holding the kwargs to provide to the model's forward function
+        text_inputs,
+        return_tensors=False,
+        return_text=True,
+        return_full_text=None,
+        clean_up_tokenization_spaces=False,
+        prefix=None,
+        **generate_kwargs
+    ):
         """
-
-        # If dynamic axis (-1) we forward with a fixed dimension of 2 samples to avoid optimizations made by ONNX
-        batch_size = compute_effective_axis_dimension(
-            batch_size, fixed_dimension=OnnxConfig.DEFAULT_FIXED_BATCH, num_token_to_add=0
-        )
-
-        # If dynamic axis (-1) we forward with a fixed dimension of 8 tokens to avoid optimizations made by ONNX
-        token_to_add = tokenizer.num_special_tokens_to_add(is_pair)
-        seq_length = compute_effective_axis_dimension(
-            seq_length, fixed_dimension=OnnxConfig.DEFAULT_FIXED_SEQUENCE, num_token_to_add=token_to_add
-        )
-
-        # Generate dummy inputs according to compute batch and sequence
-        dummy_input = [" ".join([tokenizer.unk_token]) * seq_length] * batch_size
-        return dict(tokenizer(dummy_input, return_tensors=framework))
-
-
-class OnnxConfigWithPast(OnnxConfig, ABC):
-    def __init__(self, config: PretrainedConfig, use_past: bool = False):
-        super().__init__(config)
-        self.use_past = use_past
-
-    @classmethod
-    def with_past(cls, config: PretrainedConfig) -> "OnnxConfigWithPast":
-        """
-        Instantiate a OnnxConfig with `use_past` attribute set to True
+        Complete the prompt(s) given as inputs.
 
         Args:
-            config: The underlying model's config to use when exporting to ONNX
+            args (:obj:`str` or :obj:`List[str]`):
+                One or several prompts (or one list of prompts) to complete.
+            return_tensors (:obj:`bool`, `optional`, defaults to :obj:`False`):
+                Whether or not to include the tensors of predictions (as token indices) in the outputs.
+            return_text (:obj:`bool`, `optional`, defaults to :obj:`True`):
+                Whether or not to include the decoded texts in the outputs.
+            return_full_text (:obj:`bool`, `optional`, defaults to :obj:`True`):
+                If set to :obj:`False` only added text is returned, otherwise the full text is returned Only meaningful
+                if `return_text` is set to True.
+            clean_up_tokenization_spaces (:obj:`bool`, `optional`, defaults to :obj:`False`):
+                Whether or not to clean up the potential extra spaces in the text output.
+            prefix (:obj:`str`, `optional`):
+                Prefix added to prompt.
+            generate_kwargs:
+                Additional keyword arguments to pass along to the generate method of the model (see the generate method
+                corresponding to your framework `here <./model.html#generative-models>`__).
+
+        Return:
+            A list or a list of list of :obj:`dict`: Each result comes as a dictionary with the following keys:
+
+            - **generated_text** (:obj:`str`, present when ``return_text=True``) -- The generated text.
+            - **generated_token_ids** (:obj:`torch.Tensor` or :obj:`tf.Tensor`, present when ``return_tensors=True``)
+              -- The token ids of the generated text.
+        """
+        prefix = prefix if prefix is not None else self.model.config.prefix
+        return_full_text = return_full_text if return_full_text is not None else self.return_full_text
+
+        if isinstance(text_inputs, str):
+            text_inputs = [text_inputs]
+        results = []
+        for prompt_text in text_inputs:
+            # Manage correct placement of the tensors
+            with self.device_placement():
+                if prefix is None and self.model.__class__.__name__ in [
+                    "XLNetLMHeadModel",
+                    "TransfoXLLMHeadModel",
+                    "TFXLNetLMHeadModel",
+                    "TFTransfoXLLMHeadModel",
+                ]:
+                    # For XLNet and TransformerXL we add an article to the prompt to give more state to the model.
+                    prefix = self.XL_PREFIX
+
+                if prefix:
+                    prefix_inputs = self._parse_and_tokenize(prefix, padding=False, add_special_tokens=False)
+                    # This impacts max_length and min_length argument that need adjusting.
+                    prefix_length = prefix_inputs["input_ids"].shape[-1]
+                    if generate_kwargs.get("max_length", None) is not None:
+                        generate_kwargs["max_length"] += prefix_length
+                    if generate_kwargs.get("min_length", None) is not None:
+                        generate_kwargs["min_length"] += prefix_length
+
+                prefix = prefix or ""
+                inputs = self._parse_and_tokenize(prefix + prompt_text, padding=False, add_special_tokens=False)
+
+                # set input_ids to None to allow empty prompt
+                if inputs["input_ids"].shape[-1] == 0:
+                    inputs["input_ids"] = None
+                    inputs["attention_mask"] = None
+
+                if self.framework == "pt" and inputs["input_ids"] is not None:
+                    inputs = self.ensure_tensor_on_device(**inputs)
+
+                input_ids = inputs["input_ids"]
+
+                # Ensure that batch size = 1 (batch generation not allowed for now)
+                assert (
+                    input_ids is None or input_ids.shape[0] == 1
+                ), "Batch generation is currently not supported. See https://github.com/huggingface/transformers/issues/3021 for more information."
+
+                output_sequences = self.model.generate(input_ids=input_ids, **generate_kwargs)  # BS x SL
+
+            result = []
+            for generated_sequence in output_sequences:
+                if self.framework == "pt" and generated_sequence is not None:
+                    generated_sequence = generated_sequence.cpu()
+                generated_sequence = generated_sequence.numpy().tolist()
+                record = {}
+                if return_tensors:
+                    record["generated_token_ids"] = generated_sequence
+                if return_text:
+                    # Decode text
+                    text = self.tokenizer.decode(
+                        generated_sequence,
+                        skip_special_tokens=True,
+                        clean_up_tokenization_spaces=clean_up_tokenization_spaces,
+                    )
+
+                    # Remove PADDING prompt of the sequence if XLNet or Transfo-XL model is used
+                    if input_ids is None:
+                        prompt_length = 0
+                    else:
+                        prompt_length = len(
+                            self.tokenizer.decode(
+                                input_ids[0],
+                                skip_special_tokens=True,
+                                clean_up_tokenization_spaces=clean_up_tokenization_spaces,
+                            )
+                        )
+
+                    if return_full_text:
+                        all_text = prompt_text + text[prompt_length:]
+                    else:
+                        all_text = text[prompt_length:]
+
+                    record["generated_text"] = all_text
 
-        Returns:
-            OnnxConfig with `.use_past = True`
-        """
-        return cls(config, use_past=True)
-
-    @property
-    def values_override(self) -> Optional[Mapping[str, Any]]:
-        if hasattr(self._config, "use_cache"):
-            return {"use_cache": self.use_past}
+                result.append(record)
+            results += [result]
 
-        return None
+        if len(results) == 1:
+            return results[0]
 
-    def generate_dummy_inputs(
-        self,
-        tokenizer: PreTrainedTokenizer,
-        batch_size: int = -1,
-        seq_length: int = -1,
-        is_pair: bool = False,
-        framework: Optional[TensorType] = None,
-    ) -> Mapping[str, Any]:
-        # If dynamic axis (-1) we forward with a fixed dimension of 2 samples to avoid optimizations made by ONNX
-        batch_size = compute_effective_axis_dimension(
-            batch_size, fixed_dimension=self.default_batch_size, num_token_to_add=0
-        )
-
-        # If dynamic axis (-1) we forward with a fixed dimension of 8 tokens to avoid optimizations made by ONNX
-        token_to_add = tokenizer.num_special_tokens_to_add(is_pair)
-
-        # When use_past the caching mechanism requires inputs to be only 1 single token
-        fixed_sequence_length = 1 if self.use_past else self.default_sequence_length
-        seq_length = compute_effective_axis_dimension(
-            seq_length, fixed_dimension=fixed_sequence_length, num_token_to_add=token_to_add
-        )
-
-        # Generate dummy inputs according to compute batch and sequence
-        dummy_input = [" ".join([tokenizer.unk_token]) * seq_length] * batch_size
-        return OrderedDict(dict(tokenizer(dummy_input, return_tensors=framework)))
+        return results
```

### Comparing `transformers-4.9.1/src/transformers/onnx/convert.py` & `transformers-4.9.2/src/transformers/onnx/convert.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 from pathlib import Path
 from typing import Iterable, List, Tuple, Union
 
 import numpy as np
 from packaging.version import Version, parse
 
 from .. import PreTrainedModel, PreTrainedTokenizer, TensorType, TFPreTrainedModel, is_torch_available
+from ..file_utils import is_torch_onnx_dict_inputs_support_available
 from ..utils import logging
 from .config import OnnxConfig
-from .utils import flatten_output_collection_property
 
 
 logger = logging.get_logger(__name__)  # pylint: disable=invalid-name
 
 
 # This is the minimal required version to support some ONNX Runtime features
 ORT_QUANTIZE_MINIMUM_VERSION = parse("1.4.0")
@@ -75,19 +75,24 @@
         opset:
         output:
 
     Returns:
 
     """
     if not is_torch_available():
-        raise Exception("Cannot convert because PyTorch is not installed. Please install torch first.")
+        raise ImportError("Cannot convert because PyTorch is not installed. Please install torch first.")
 
     import torch
     from torch.onnx import export
 
+    from ..file_utils import torch_version
+
+    if not is_torch_onnx_dict_inputs_support_available():
+        raise AssertionError(f"Unsupported PyTorch version, minimum required is 1.8.0, got: {torch_version}")
+
     logger.info(f"Using framework PyTorch: {torch.__version__}")
     torch.set_grad_enabled(False)
     model.config.return_dict = True
     model.eval()
 
     # Check if we need to override certain configuration item
     if config.values_override is not None:
@@ -101,28 +106,32 @@
     model_inputs = config.generate_dummy_inputs(tokenizer, framework=TensorType.PYTORCH)
     inputs_match, matched_inputs = ensure_model_and_config_inputs_match(model, model_inputs.keys())
     onnx_outputs = list(config.outputs.keys())
 
     if not inputs_match:
         raise ValueError("Model and config inputs doesn't match")
 
+    config.patch_ops()
+
     # export can works with named args but the dict containing named args as to be last element of the args tuple
     export(
         model,
         (model_inputs,),
         f=output.as_posix(),
         input_names=list(config.inputs.keys()),
         output_names=onnx_outputs,
         dynamic_axes={name: axes for name, axes in chain(config.inputs.items(), config.outputs.items())},
         do_constant_folding=True,
         use_external_data_format=config.use_external_data_format(model.num_parameters()),
         enable_onnx_checker=True,
         opset_version=opset,
     )
 
+    config.restore_ops()
+
     return matched_inputs, onnx_outputs
 
 
 def validate_model_outputs(
     config: OnnxConfig,
     tokenizer: PreTrainedTokenizer,
     reference_model: Union[PreTrainedModel, TFPreTrainedModel],
@@ -130,37 +139,43 @@
     onnx_named_outputs: List[str],
     atol: float,
 ):
     from onnxruntime import InferenceSession, SessionOptions
 
     logger.info("Validating ONNX model...")
 
+    # TODO: generate inputs with a different batch_size and seq_len that was used for conversion to properly test
+    # dynamic input shapes.
     reference_model_inputs = config.generate_dummy_inputs(tokenizer, framework=TensorType.PYTORCH)
 
     # Create ONNX Runtime session
     options = SessionOptions()
     session = InferenceSession(onnx_model.as_posix(), options)
 
     # Compute outputs from the reference model
     ref_outputs = reference_model(**reference_model_inputs)
     ref_outputs_dict = {}
 
     # We flatten potential collection of outputs (i.e. past_keys) to a flat structure
     for name, value in ref_outputs.items():
+        # Overwriting the output name as "present" since it is the name used for the ONNX ouputs
+        # ("past_key_values" being taken for the ONNX inputs)
+        if name == "past_key_values":
+            name = "present"
         if isinstance(value, (list, tuple)):
-            value = flatten_output_collection_property(name, value)
+            value = config.flatten_output_collection_property(name, value)
             ref_outputs_dict.update(value)
         else:
             ref_outputs_dict[name] = value
 
     # We flatten potential collection of inputs (i.e. past_keys)
     onnx_inputs = {}
     for name, value in reference_model_inputs.items():
         if isinstance(value, (list, tuple)):
-            value = flatten_output_collection_property(name, value)
+            value = config.flatten_output_collection_property(name, value)
             onnx_inputs.update({tensor_name: pt_tensor.numpy() for tensor_name, pt_tensor in value.items()})
         else:
             onnx_inputs[name] = value.numpy()
 
     # Compute outputs from the ONNX model
     onnx_outputs = session.run(onnx_named_outputs, onnx_inputs)
 
@@ -176,26 +191,26 @@
             f"{onnx_outputs_set.difference(ref_outputs_set)}"
         )
     else:
         logger.info(f"\t-[✓] ONNX model outputs' name match reference model ({onnx_outputs_set}")
 
     # Check the shape and values match
     for name, ort_value in zip(onnx_named_outputs, onnx_outputs):
-        ref_value = ref_outputs_dict[name].numpy()
+        ref_value = ref_outputs_dict[name].detach().numpy()
         logger.info(f'\t- Validating ONNX Model output "{name}":')
 
         # Shape
         if not ort_value.shape == ref_value.shape:
             logger.info(f"\t\t-[x] shape {ort_value.shape} doesn't match {ref_value.shape}")
             raise ValueError(
                 "Outputs shape doesn't match between reference model and ONNX exported model: "
                 f"Got {ref_value.shape} (reference) and {ort_value.shape} (ONNX)"
             )
         else:
-            logger.info(f"\t\t-[✓] {ort_value.shape} matchs {ref_value.shape}")
+            logger.info(f"\t\t-[✓] {ort_value.shape} matches {ref_value.shape}")
 
         # Values
         if not np.allclose(ref_value, ort_value, atol=atol):
             logger.info(f"\t\t-[x] values not close enough (atol: {atol})")
             raise ValueError(
                 "Outputs values doesn't match between reference model and ONNX exported model: "
                 f"Got max absolute difference of: {np.amax(np.abs(ref_value - ort_value))}"
```

### Comparing `transformers-4.9.1/src/transformers/optimization.py` & `transformers-4.9.2/src/transformers/optimization.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/optimization_tf.py` & `transformers-4.9.2/src/transformers/optimization_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/__init__.py` & `transformers-4.9.2/src/transformers/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/automatic_speech_recognition.py` & `transformers-4.9.2/src/transformers/pipelines/automatic_speech_recognition.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/base.py` & `transformers-4.9.2/src/transformers/pipelines/base.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/conversational.py` & `transformers-4.9.2/src/transformers/pipelines/conversational.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/feature_extraction.py` & `transformers-4.9.2/src/transformers/pipelines/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/fill_mask.py` & `transformers-4.9.2/src/transformers/pipelines/fill_mask.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/image_classification.py` & `transformers-4.9.2/src/transformers/pipelines/image_classification.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/question_answering.py` & `transformers-4.9.2/src/transformers/pipelines/question_answering.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/table_question_answering.py` & `transformers-4.9.2/src/transformers/pipelines/table_question_answering.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/text2text_generation.py` & `transformers-4.9.2/src/transformers/pipelines/text2text_generation.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/text_classification.py` & `transformers-4.9.2/src/transformers/pipelines/text_classification.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/token_classification.py` & `transformers-4.9.2/src/transformers/pipelines/token_classification.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/pipelines/zero_shot_classification.py` & `transformers-4.9.2/src/transformers/pipelines/zero_shot_classification.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/sagemaker/__init__.py` & `transformers-4.9.2/src/transformers/sagemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/sagemaker/trainer_sm.py` & `transformers-4.9.2/src/transformers/sagemaker/trainer_sm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/sagemaker/training_args_sm.py` & `transformers-4.9.2/src/transformers/sagemaker/training_args_sm.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/testing_utils.py` & `transformers-4.9.2/src/transformers/testing_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import sys
 import tempfile
 import unittest
 from distutils.util import strtobool
 from io import StringIO
 from pathlib import Path
 from typing import Iterator, Union
+from unittest import mock
 
 from transformers import logging as transformers_logging
 
 from .deepspeed import is_deepspeed_available
 from .file_utils import (
     is_datasets_available,
     is_faiss_available,
@@ -1003,15 +1004,15 @@
 
     @mockenv(RUN_SLOW=True, USE_TF=False)
     def test_something():
         run_slow = os.getenv("RUN_SLOW", False)
         use_tf = os.getenv("USE_TF", False)
 
     """
-    return unittest.mock.patch.dict(os.environ, kwargs)
+    return mock.patch.dict(os.environ, kwargs)
 
 
 # from https://stackoverflow.com/a/34333710/9201239
 @contextlib.contextmanager
 def mockenv_context(*remove, **update):
     """
     Temporarily updates the ``os.environ`` dictionary in-place. Similar to mockenv
```

### Comparing `transformers-4.9.1/src/transformers/tokenization_utils.py` & `transformers-4.9.2/src/transformers/tokenization_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/tokenization_utils_base.py` & `transformers-4.9.2/src/transformers/tokenization_utils_base.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/tokenization_utils_fast.py` & `transformers-4.9.2/src/transformers/tokenization_utils_fast.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/trainer.py` & `transformers-4.9.2/src/transformers/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         default_collator = default_data_collator if tokenizer is None else DataCollatorWithPadding(tokenizer)
         self.data_collator = data_collator if data_collator is not None else default_collator
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.tokenizer = tokenizer
 
         if self.place_model_on_device:
-            model = model.to(args.device)
+            self._move_model_to_device(model, args.device)
 
         # Force n_gpu to 1 to avoid DataParallel as MP will manage the GPUs
         if self.is_model_parallel:
             self.args._n_gpu = 1
 
         # later use `self.model is self.model_wrapped` to check if it's wrapped or not
         self.model_wrapped = model
@@ -501,14 +501,20 @@
         Args:
            callback (:obj:`type` or :class:`~transformer.TrainerCallback`):
                A :class:`~transformer.TrainerCallback` class or an instance of a :class:`~transformer.TrainerCallback`.
                In the first case, will remove the first member of that class found in the list of callbacks.
         """
         self.callback_handler.remove_callback(callback)
 
+    def _move_model_to_device(self, model, device):
+        model = model.to(device)
+        # Moving a model to an XLA device disconnects the tied weights, so we have to retie them.
+        if self.args.parallel_mode == ParallelMode.TPU and hasattr(model, "tie_weights"):
+            model.tie_weights()
+
     def _remove_unused_columns(self, dataset: "datasets.Dataset", description: Optional[str] = None):
         if not self.args.remove_unused_columns:
             return dataset
         if self._signature_columns is None:
             # Inspect model forward signature to keep only the arguments it accepts.
             signature = inspect.signature(self.model.forward)
             self._signature_columns = list(signature.parameters.keys())
@@ -1012,15 +1018,15 @@
         args = self.args
 
         self.is_in_train = True
 
         # do_train is not a reliable argument, as it might not be set and .train() still called, so
         # the following is a workaround:
         if args.fp16_full_eval and not args.do_train:
-            self.model = self.model.to(args.device)
+            self._move_model_to_device(self.model, args.device)
 
         if "model_path" in kwargs:
             resume_from_checkpoint = kwargs.pop("model_path")
             warnings.warn(
                 "`model_path` is deprecated and will be removed in a future version. Use `resume_from_checkpoint` "
                 "instead.",
                 FutureWarning,
@@ -1073,15 +1079,15 @@
 
                 # release memory
                 del state_dict
 
         # If model was re-initialized, put it on the right device and update self.model_wrapped
         if model_reloaded:
             if self.place_model_on_device:
-                self.model = self.model.to(args.device)
+                self._move_model_to_device(self.model, args.device)
             self.model_wrapped = self.model
 
         # Keeping track whether we can can len() on the dataset or not
         train_dataset_is_sized = isinstance(self.train_dataset, collections.abc.Sized)
 
         # Data loader and number of training steps
         train_dataloader = self.get_train_dataloader()
@@ -2511,18 +2517,19 @@
                 Message to commit while pushing.
             kwargs:
                 Additional keyword arguments passed along to :meth:`~transformers.Trainer.create_model_card`.
 
         Returns:
             The url of the commit of your model in the given repository.
         """
-        if not self.args.should_save:
-            return
 
-        self.create_model_card(model_name=self.args.push_to_hub_model_id, **kwargs)
+        if self.args.should_save:
+            self.create_model_card(model_name=self.args.push_to_hub_model_id, **kwargs)
+        # Needs to be executed on all processes for TPU training, but will only save on the processed determined by
+        # self.args.should_save.
         self.save_model()
 
         # Only push from one node.
         if not self.is_world_process_zero():
             return
 
         return self.repo.push_to_hub(commit_message=commit_message)
```

### Comparing `transformers-4.9.1/src/transformers/trainer_callback.py` & `transformers-4.9.2/src/transformers/trainer_callback.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/trainer_pt_utils.py` & `transformers-4.9.2/src/transformers/trainer_pt_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/trainer_seq2seq.py` & `transformers-4.9.2/src/transformers/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/trainer_tf.py` & `transformers-4.9.2/src/transformers/trainer_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/trainer_utils.py` & `transformers-4.9.2/src/transformers/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/training_args.py` & `transformers-4.9.2/src/transformers/training_args.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/training_args_seq2seq.py` & `transformers-4.9.2/src/transformers/training_args_seq2seq.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/training_args_tf.py` & `transformers-4.9.2/src/transformers/training_args_tf.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/__init__.py` & `transformers-4.9.2/src/transformers/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/coco_classes.py` & `transformers-4.9.2/src/transformers/utils/coco_classes.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_flax_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_flax_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_pt_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_pt_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_sentencepiece_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_sentencepiece_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_tf_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_tf_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_timm_and_vision_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_timm_and_vision_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_timm_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_timm_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_tokenizers_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_tokenizers_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/dummy_vision_objects.py` & `transformers-4.9.2/src/transformers/utils/dummy_vision_objects.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/fx.py` & `transformers-4.9.2/src/transformers/utils/fx.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/hp_naming.py` & `transformers-4.9.2/src/transformers/utils/hp_naming.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/imagenet_classes.py` & `transformers-4.9.2/src/transformers/utils/imagenet_classes.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/logging.py` & `transformers-4.9.2/src/transformers/utils/logging.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/model_parallel_utils.py` & `transformers-4.9.2/src/transformers/utils/model_parallel_utils.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/modeling_auto_mapping.py` & `transformers-4.9.2/src/transformers/utils/modeling_auto_mapping.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/notebook.py` & `transformers-4.9.2/src/transformers/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/sentencepiece_model_pb2.py` & `transformers-4.9.2/src/transformers/utils/sentencepiece_model_pb2.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers/utils/versions.py` & `transformers-4.9.2/src/transformers/utils/versions.py`

 * *Files identical despite different names*

### Comparing `transformers-4.9.1/src/transformers.egg-info/PKG-INFO` & `transformers-4.9.2/src/transformers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: transformers
-Version: 4.9.1
+Version: 4.9.2
 Summary: State-of-the-art Natural Language Processing for TensorFlow 2.0 and PyTorch
 Home-page: https://github.com/huggingface/transformers
 Author: Thomas Wolf, Lysandre Debut, Victor Sanh, Julien Chaumond, Sam Shleifer, Patrick von Platen, Sylvain Gugger, Suraj Patil, Stas Bekman, Google AI Language Team Authors, Open AI team Authors, Facebook AI Authors, Carnegie Mellon University Authors
 Author-email: thomas@huggingface.co
 License: Apache
 Description: <!---
         Copyright 2020 The HuggingFace Team. All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: transformers Version: 4.9.1 Summary: State-of-the-
+Metadata-Version: 2.1 Name: transformers Version: 4.9.2 Summary: State-of-the-
 art Natural Language Processing for TensorFlow 2.0 and PyTorch Home-page:
 https://github.com/huggingface/transformers Author: Thomas Wolf, Lysandre
 Debut, Victor Sanh, Julien Chaumond, Sam Shleifer, Patrick von Platen, Sylvain
 Gugger, Suraj Patil, Stas Bekman, Google AI Language Team Authors, Open AI team
 Authors, Facebook AI Authors, Carnegie Mellon University Authors Author-email:
 thomas@huggingface.co License: Apache Description:
```

### Comparing `transformers-4.9.1/src/transformers.egg-info/SOURCES.txt` & `transformers-4.9.2/src/transformers.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -492,14 +492,15 @@
 src/transformers/models/xlnet/modeling_xlnet.py
 src/transformers/models/xlnet/tokenization_xlnet.py
 src/transformers/models/xlnet/tokenization_xlnet_fast.py
 src/transformers/onnx/__init__.py
 src/transformers/onnx/__main__.py
 src/transformers/onnx/config.py
 src/transformers/onnx/convert.py
+src/transformers/onnx/features.py
 src/transformers/onnx/utils.py
 src/transformers/pipelines/__init__.py
 src/transformers/pipelines/automatic_speech_recognition.py
 src/transformers/pipelines/base.py
 src/transformers/pipelines/conversational.py
 src/transformers/pipelines/feature_extraction.py
 src/transformers/pipelines/fill_mask.py
```

### Comparing `transformers-4.9.1/src/transformers.egg-info/requires.txt` & `transformers-4.9.2/src/transformers.egg-info/requires.txt`

 * *Files identical despite different names*

