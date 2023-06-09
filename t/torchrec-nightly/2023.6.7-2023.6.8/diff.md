# Comparing `tmp/torchrec_nightly-2023.6.7-py38-none-any.whl.zip` & `tmp/torchrec_nightly-2023.6.8-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,145 +1,145 @@
-Zip file size: 350610 bytes, number of entries: 143
--rw-r--r--  2.0 unx      811 b- defN 23-Jun-07 11:17 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-Jun-07 11:17 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jun-07 11:17 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Jun-07 11:17 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-Jun-07 11:17 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-Jun-07 11:17 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-Jun-07 11:17 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-Jun-07 11:17 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Jun-07 11:17 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jun-07 11:17 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jun-07 11:17 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Jun-07 11:17 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jun-07 11:17 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    37053 b- defN 23-Jun-07 11:17 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-Jun-07 11:17 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-Jun-07 11:17 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55918 b- defN 23-Jun-07 11:17 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    35580 b- defN 23-Jun-07 11:17 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    30257 b- defN 23-Jun-07 11:17 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     3872 b- defN 23-Jun-07 11:17 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    28994 b- defN 23-Jun-07 11:17 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    18564 b- defN 23-Jun-07 11:17 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    37089 b- defN 23-Jun-07 11:17 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15030 b- defN 23-Jun-07 11:17 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    35078 b- defN 23-Jun-07 11:17 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-Jun-07 11:17 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     5542 b- defN 23-Jun-07 11:17 torchrec/distributed/fp_embeddingbag.py
--rw-r--r--  2.0 unx     5273 b- defN 23-Jun-07 11:17 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5110 b- defN 23-Jun-07 11:17 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     1709 b- defN 23-Jun-07 11:17 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-Jun-07 11:17 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19520 b- defN 23-Jun-07 11:17 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    13729 b- defN 23-Jun-07 11:17 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    13343 b- defN 23-Jun-07 11:17 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    10931 b- defN 23-Jun-07 11:17 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Jun-07 11:17 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19411 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    34059 b- defN 23-Jun-07 11:17 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    24927 b- defN 23-Jun-07 11:17 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    11373 b- defN 23-Jun-07 11:17 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jun-07 11:17 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    10318 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12642 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      835 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    13288 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11134 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    40395 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    23617 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9125 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    13899 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jun-07 11:17 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2539 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx     9519 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     5041 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    12850 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3114 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7692 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16315 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19898 b- defN 23-Jun-07 11:17 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    10213 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34114 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11193 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25075 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Jun-07 11:17 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jun-07 11:17 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6477 b- defN 23-Jun-07 11:17 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4401 b- defN 23-Jun-07 11:17 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jun-07 11:17 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-Jun-07 11:17 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jun-07 11:17 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     8068 b- defN 23-Jun-07 11:17 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-Jun-07 11:17 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Jun-07 11:17 torchrec/metrics/accuracy.py
--rw-r--r--  2.0 unx    12549 b- defN 23-Jun-07 11:17 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-Jun-07 11:17 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-Jun-07 11:17 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-Jun-07 11:17 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17909 b- defN 23-Jun-07 11:17 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6778 b- defN 23-Jun-07 11:17 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3695 b- defN 23-Jun-07 11:17 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jun-07 11:17 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jun-07 11:17 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-Jun-07 11:17 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     6811 b- defN 23-Jun-07 11:17 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    31495 b- defN 23-Jun-07 11:17 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-Jun-07 11:17 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-Jun-07 11:17 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    10622 b- defN 23-Jun-07 11:17 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jun-07 11:17 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-Jun-07 11:17 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Jun-07 11:17 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-Jun-07 11:17 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    30000 b- defN 23-Jun-07 11:17 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-07 11:17 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9825 b- defN 23-Jun-07 11:17 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-Jun-07 11:17 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jun-07 11:17 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Jun-07 11:17 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    15163 b- defN 23-Jun-07 11:17 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-Jun-07 11:17 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     5537 b- defN 23-Jun-07 11:17 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Jun-07 11:17 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-Jun-07 11:17 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-Jun-07 11:17 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx     2169 b- defN 23-Jun-07 11:17 torchrec/modules/feature_processor_.py
--rw-r--r--  2.0 unx     3855 b- defN 23-Jun-07 11:17 torchrec/modules/fp_embedding_modules.py
--rw-r--r--  2.0 unx    31193 b- defN 23-Jun-07 11:17 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10696 b- defN 23-Jun-07 11:17 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-Jun-07 11:17 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     4022 b- defN 23-Jun-07 11:17 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jun-07 11:17 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jun-07 11:17 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Jun-07 11:17 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jun-07 11:17 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-Jun-07 11:17 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jun-07 11:17 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-Jun-07 11:17 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-Jun-07 11:17 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jun-07 11:17 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-Jun-07 11:17 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    22933 b- defN 23-Jun-07 11:17 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     4100 b- defN 23-Jun-07 11:17 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jun-07 11:17 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    55649 b- defN 23-Jun-07 11:17 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jun-07 11:17 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jun-07 11:17 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-Jun-07 11:22 torchrec_nightly-2023.6.7.dist-info/LICENSE
--rw-r--r--  2.0 unx     5011 b- defN 23-Jun-07 11:22 torchrec_nightly-2023.6.7.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jun-07 11:22 torchrec_nightly-2023.6.7.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-07 11:22 torchrec_nightly-2023.6.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13347 b- defN 23-Jun-07 11:22 torchrec_nightly-2023.6.7.dist-info/RECORD
-143 files, 1426435 bytes uncompressed, 329256 bytes compressed:  76.9%
+Zip file size: 351028 bytes, number of entries: 143
+-rw-r--r--  2.0 unx      811 b- defN 23-Jun-08 11:18 torchrec/__init__.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jun-08 11:18 torchrec/streamable.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jun-08 11:18 torchrec/types.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jun-08 11:18 torchrec/datasets/__init__.py
+-rw-r--r--  2.0 unx    41469 b- defN 23-Jun-08 11:18 torchrec/datasets/criteo.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jun-08 11:18 torchrec/datasets/movielens.py
+-rw-r--r--  2.0 unx     6539 b- defN 23-Jun-08 11:18 torchrec/datasets/random.py
+-rw-r--r--  2.0 unx    10909 b- defN 23-Jun-08 11:18 torchrec/datasets/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jun-08 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/datasets/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Jun-08 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Jun-08 11:18 torchrec/distributed/__init__.py
+-rw-r--r--  2.0 unx    37053 b- defN 23-Jun-08 11:18 torchrec/distributed/batched_embedding_kernel.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jun-08 11:18 torchrec/distributed/collective_utils.py
+-rw-r--r--  2.0 unx     4988 b- defN 23-Jun-08 11:18 torchrec/distributed/comm.py
+-rw-r--r--  2.0 unx    55918 b- defN 23-Jun-08 11:18 torchrec/distributed/comm_ops.py
+-rw-r--r--  2.0 unx    35580 b- defN 23-Jun-08 11:18 torchrec/distributed/dist_data.py
+-rw-r--r--  2.0 unx    31599 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding.py
+-rw-r--r--  2.0 unx     3872 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_kernel.py
+-rw-r--r--  2.0 unx    28994 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_lookup.py
+-rw-r--r--  2.0 unx    18564 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_sharding.py
+-rw-r--r--  2.0 unx    37089 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_tower_sharding.py
+-rw-r--r--  2.0 unx    15030 b- defN 23-Jun-08 11:18 torchrec/distributed/embedding_types.py
+-rw-r--r--  2.0 unx    35078 b- defN 23-Jun-08 11:18 torchrec/distributed/embeddingbag.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Jun-08 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-r--r--  2.0 unx     5542 b- defN 23-Jun-08 11:18 torchrec/distributed/fp_embeddingbag.py
+-rw-r--r--  2.0 unx     5273 b- defN 23-Jun-08 11:18 torchrec/distributed/fused_embedding.py
+-rw-r--r--  2.0 unx     5110 b- defN 23-Jun-08 11:18 torchrec/distributed/fused_embeddingbag.py
+-rw-r--r--  2.0 unx     1709 b- defN 23-Jun-08 11:18 torchrec/distributed/fused_params.py
+-rw-r--r--  2.0 unx     3807 b- defN 23-Jun-08 11:18 torchrec/distributed/grouped_position_weighted.py
+-rw-r--r--  2.0 unx    19786 b- defN 23-Jun-08 11:18 torchrec/distributed/model_parallel.py
+-rw-r--r--  2.0 unx    13729 b- defN 23-Jun-08 11:18 torchrec/distributed/quant_embedding.py
+-rw-r--r--  2.0 unx    13343 b- defN 23-Jun-08 11:18 torchrec/distributed/quant_embedding_kernel.py
+-rw-r--r--  2.0 unx    10931 b- defN 23-Jun-08 11:18 torchrec/distributed/quant_embeddingbag.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Jun-08 11:18 torchrec/distributed/shard.py
+-rw-r--r--  2.0 unx    19411 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding_plan.py
+-rw-r--r--  2.0 unx    34059 b- defN 23-Jun-08 11:18 torchrec/distributed/train_pipeline.py
+-rw-r--r--  2.0 unx    24927 b- defN 23-Jun-08 11:18 torchrec/distributed/types.py
+-rw-r--r--  2.0 unx    11873 b- defN 23-Jun-08 11:18 torchrec/distributed/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/distributed/composable/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jun-08 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/__init__.py
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/constants.py
+-rw-r--r--  2.0 unx    10318 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/enumerators.py
+-rw-r--r--  2.0 unx    12642 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/partitioners.py
+-rw-r--r--  2.0 unx      835 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/perf_models.py
+-rw-r--r--  2.0 unx    13288 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/planners.py
+-rw-r--r--  2.0 unx    11134 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/proposers.py
+-rw-r--r--  2.0 unx    40395 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/shard_estimators.py
+-rw-r--r--  2.0 unx    23617 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/stats.py
+-rw-r--r--  2.0 unx     9125 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/storage_reservations.py
+-rw-r--r--  2.0 unx    13899 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/types.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jun-08 11:18 torchrec/distributed/planner/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/__init__.py
+-rw-r--r--  2.0 unx     2539 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-r--r--  2.0 unx     9519 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/cw_sharding.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/dp_sharding.py
+-rw-r--r--  2.0 unx     5041 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-r--r--  2.0 unx    12850 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/rw_sharding.py
+-rw-r--r--  2.0 unx     3114 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/sequence_sharding.py
+-rw-r--r--  2.0 unx     7692 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-r--r--  2.0 unx    16315 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/tw_sharding.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/twcw_sharding.py
+-rw-r--r--  2.0 unx    19898 b- defN 23-Jun-08 11:18 torchrec/distributed/sharding/twrw_sharding.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/__init__.py
+-rw-r--r--  2.0 unx    10213 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/infer_utils.py
+-rw-r--r--  2.0 unx     4868 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/multi_process.py
+-rw-r--r--  2.0 unx    34246 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_model.py
+-rw-r--r--  2.0 unx    11193 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-r--r--  2.0 unx    25190 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jun-08 11:18 torchrec/distributed/test_utils/test_sharding.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jun-08 11:18 torchrec/fx/__init__.py
+-rw-r--r--  2.0 unx     6477 b- defN 23-Jun-08 11:18 torchrec/fx/tracer.py
+-rw-r--r--  2.0 unx     4401 b- defN 23-Jun-08 11:18 torchrec/fx/utils.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jun-08 11:18 torchrec/inference/__init__.py
+-rw-r--r--  2.0 unx     3614 b- defN 23-Jun-08 11:18 torchrec/inference/client.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jun-08 11:18 torchrec/inference/model_packager.py
+-rw-r--r--  2.0 unx     8068 b- defN 23-Jun-08 11:18 torchrec/inference/modules.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Jun-08 11:18 torchrec/inference/state_dict_transform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/metrics/__init__.py
+-rw-r--r--  2.0 unx     4168 b- defN 23-Jun-08 11:18 torchrec/metrics/accuracy.py
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jun-08 11:18 torchrec/metrics/auc.py
+-rw-r--r--  2.0 unx     3703 b- defN 23-Jun-08 11:18 torchrec/metrics/calibration.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jun-08 11:18 torchrec/metrics/ctr.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Jun-08 11:18 torchrec/metrics/mae.py
+-rw-r--r--  2.0 unx    17909 b- defN 23-Jun-08 11:18 torchrec/metrics/metric_module.py
+-rw-r--r--  2.0 unx     6778 b- defN 23-Jun-08 11:18 torchrec/metrics/metrics_config.py
+-rw-r--r--  2.0 unx     3695 b- defN 23-Jun-08 11:18 torchrec/metrics/metrics_namespace.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jun-08 11:18 torchrec/metrics/model_utils.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jun-08 11:18 torchrec/metrics/mse.py
+-rw-r--r--  2.0 unx     5605 b- defN 23-Jun-08 11:18 torchrec/metrics/multiclass_recall.py
+-rw-r--r--  2.0 unx     6811 b- defN 23-Jun-08 11:18 torchrec/metrics/ne.py
+-rw-r--r--  2.0 unx    31495 b- defN 23-Jun-08 11:18 torchrec/metrics/rec_metric.py
+-rw-r--r--  2.0 unx    10490 b- defN 23-Jun-08 11:18 torchrec/metrics/recall_session.py
+-rw-r--r--  2.0 unx     6057 b- defN 23-Jun-08 11:18 torchrec/metrics/throughput.py
+-rw-r--r--  2.0 unx    10622 b- defN 23-Jun-08 11:18 torchrec/metrics/tower_qps.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jun-08 11:18 torchrec/metrics/weighted_avg.py
+-rw-r--r--  2.0 unx    16441 b- defN 23-Jun-08 11:18 torchrec/metrics/test_utils/__init__.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Jun-08 11:18 torchrec/models/__init__.py
+-rw-r--r--  2.0 unx    11410 b- defN 23-Jun-08 11:18 torchrec/models/deepfm.py
+-rw-r--r--  2.0 unx    30000 b- defN 23-Jun-08 11:18 torchrec/models/dlrm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 11:18 torchrec/models/experimental/__init__.py
+-rw-r--r--  2.0 unx     9825 b- defN 23-Jun-08 11:18 torchrec/models/experimental/test_transformerdlrm.py
+-rw-r--r--  2.0 unx     7434 b- defN 23-Jun-08 11:18 torchrec/models/experimental/transformerdlrm.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jun-08 11:18 torchrec/modules/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jun-08 11:18 torchrec/modules/activation.py
+-rw-r--r--  2.0 unx    15163 b- defN 23-Jun-08 11:18 torchrec/modules/crossnet.py
+-rw-r--r--  2.0 unx     8415 b- defN 23-Jun-08 11:18 torchrec/modules/deepfm.py
+-rw-r--r--  2.0 unx     5537 b- defN 23-Jun-08 11:18 torchrec/modules/embedding_configs.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Jun-08 11:18 torchrec/modules/embedding_modules.py
+-rw-r--r--  2.0 unx     4858 b- defN 23-Jun-08 11:18 torchrec/modules/embedding_tower.py
+-rw-r--r--  2.0 unx    12360 b- defN 23-Jun-08 11:18 torchrec/modules/feature_processor.py
+-rw-r--r--  2.0 unx     2169 b- defN 23-Jun-08 11:18 torchrec/modules/feature_processor_.py
+-rw-r--r--  2.0 unx     3855 b- defN 23-Jun-08 11:18 torchrec/modules/fp_embedding_modules.py
+-rw-r--r--  2.0 unx    31193 b- defN 23-Jun-08 11:18 torchrec/modules/fused_embedding_modules.py
+-rw-r--r--  2.0 unx    10696 b- defN 23-Jun-08 11:18 torchrec/modules/lazy_extension.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jun-08 11:18 torchrec/modules/mlp.py
+-rw-r--r--  2.0 unx     4022 b- defN 23-Jun-08 11:18 torchrec/modules/utils.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jun-08 11:18 torchrec/optim/__init__.py
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jun-08 11:18 torchrec/optim/apply_optimizer_in_backward.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Jun-08 11:18 torchrec/optim/clipping.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jun-08 11:18 torchrec/optim/fused.py
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jun-08 11:18 torchrec/optim/keyed.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jun-08 11:18 torchrec/optim/optimizers.py
+-rw-r--r--  2.0 unx     7405 b- defN 23-Jun-08 11:18 torchrec/optim/rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4865 b- defN 23-Jun-08 11:18 torchrec/optim/warmup.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jun-08 11:18 torchrec/optim/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jun-08 11:18 torchrec/quant/__init__.py
+-rw-r--r--  2.0 unx    22933 b- defN 23-Jun-08 11:18 torchrec/quant/embedding_modules.py
+-rw-r--r--  2.0 unx     4100 b- defN 23-Jun-08 11:18 torchrec/quant/utils.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jun-08 11:18 torchrec/sparse/__init__.py
+-rw-r--r--  2.0 unx    55583 b- defN 23-Jun-08 11:18 torchrec/sparse/jagged_tensor.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jun-08 11:18 torchrec/sparse/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jun-08 11:18 torchrec/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5011 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13347 b- defN 23-Jun-08 11:22 torchrec_nightly-2023.6.8.dist-info/RECORD
+143 files, 1428724 bytes uncompressed, 329674 bytes compressed:  76.9%
```

## zipnote {}

```diff
@@ -408,23 +408,23 @@
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.6.7.dist-info/LICENSE
+Filename: torchrec_nightly-2023.6.8.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.6.7.dist-info/METADATA
+Filename: torchrec_nightly-2023.6.8.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.6.7.dist-info/WHEEL
+Filename: torchrec_nightly-2023.6.8.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.6.7.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.6.8.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.6.7.dist-info/RECORD
+Filename: torchrec_nightly-2023.6.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchrec/distributed/embedding.py

```diff
@@ -399,36 +399,67 @@
                     process_group=env.process_group,
                     gradient_as_bucket_view=True,
                     broadcast_buffers=True,
                     static_graph=True,
                 )
         self._initialize_torch_state()
 
+        if module.device != torch.device("meta"):
+            self.load_state_dict(module.state_dict())
+
     @staticmethod
     def _pre_load_state_dict_hook(
         self: "ShardedEmbeddingCollection",
         state_dict: Dict[str, Any],
         prefix: str,
         *args: Any,
     ) -> None:
         """
         Modify the destination state_dict for model parallel
         to transform from ShardedTensors into tensors
         """
-        for table_name in self._model_parallel_name_to_local_shards.keys():
+        for (
+            table_name,
+            model_shards,
+        ) in self._model_parallel_name_to_local_shards.items():
             key = f"{prefix}embeddings.{table_name}.weight"
-            local_shards = state_dict[key].local_shards()
-            if len(local_shards) == 0:
-                state_dict[key] = torch.empty(0)
+
+            # If state_dict[key] is already a ShardedTensor, use its local shards
+            if isinstance(state_dict[key], ShardedTensor):
+                local_shards = state_dict[key].local_shards()
+                # If no local shards, create an empty tensor
+                if len(local_shards) == 0:
+                    state_dict[key] = torch.empty(0)
+                else:
+                    dim = state_dict[key].metadata().shards_metadata[0].shard_sizes[1]
+                    # CW multiple shards are merged
+                    state_dict[key] = torch.cat(
+                        [shard.tensor.view(-1) for shard in local_shards], dim=0
+                    ).view(-1, dim)
             else:
-                dim = state_dict[key].metadata().shards_metadata[0].shard_sizes[1]
-                # CW multiple shards are merged
-                state_dict[key] = torch.cat(
-                    [s.tensor.view(-1) for s in local_shards], dim=0
-                ).view(-1, dim)
+                local_shards = []
+                for shard in model_shards:
+                    # Extract shard size and offsets for splicing
+                    shard_sizes = shard.metadata.shard_sizes
+                    shard_offsets = shard.metadata.shard_offsets
+
+                    # Prepare tensor by splicing and placing on appropriate device
+                    spliced_tensor = state_dict[key][
+                        shard_offsets[0] : shard_offsets[0] + shard_sizes[0],
+                        shard_offsets[1] : shard_offsets[1] + shard_sizes[1],
+                    ].to(shard.tensor.get_device())
+
+                    # Append spliced tensor into local shards
+                    local_shards.append(spliced_tensor)
+
+                state_dict[key] = (
+                    torch.empty(0)
+                    if not local_shards
+                    else torch.cat(local_shards, dim=0)
+                )
 
     def _initialize_torch_state(self) -> None:  # noqa
         """
         This provides consistency between this class and the EmbeddingCollection's
         nn.Module API calls (state_dict, named_modules, etc)
         """
```

## torchrec/distributed/model_parallel.py

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import abc
+import copy
 from collections import OrderedDict
 from typing import Any, cast, Dict, Iterator, List, Optional, Tuple, Type
 
 import torch
 import torch.distributed as dist
 from torch import nn
 from torch.distributed.fsdp import FullyShardedDataParallel
@@ -22,23 +23,23 @@
     sharder_name,
     Topology,
 )
 from torchrec.distributed.sharding_plan import get_default_sharders
 from torchrec.distributed.types import (
     ModuleSharder,
     ShardedModule,
-    ShardedTensor,
     ShardingEnv,
     ShardingPlan,
 )
 from torchrec.distributed.utils import (
     add_prefix_to_state_dict,
     append_prefix,
     copy_to_device,
     filter_state_dict,
+    sharded_model_copy,
 )
 from torchrec.optim.fused import FusedOptimizerModule
 from torchrec.optim.keyed import CombinedOptimizer, KeyedOptimizer
 
 try:
     torch.ops.load_library("//deeplearning/fbgemm/fbgemm_gpu:sparse_ops")
     torch.ops.load_library("//deeplearning/fbgemm/fbgemm_gpu:sparse_ops_cpu")
@@ -282,16 +283,23 @@
     ) -> "DistributedModelParallel":
         """
         Recursively copy submodules to new device by calling per-module customized copy
         process, since some modules needs to use the original references (like
         `ShardedModule` for inference).
         """
         assert isinstance(device, torch.device)
-        copy_dmp = copy_to_device(self, self.device, device)
-        return cast(DistributedModelParallel, copy_dmp)
+        # dmp code deep copy
+        with sharded_model_copy(device=None):
+            copy_dmp = copy.deepcopy(self)
+        # tensor resident module deep copy
+        copy_dmp_wrapped_module = copy_to_device(
+            self._dmp_wrapped_module, self.device, device
+        )
+        copy_dmp._dmp_wrapped_module = copy_dmp_wrapped_module
+        return copy_dmp
 
     def _init_dmp(self, module: nn.Module) -> nn.Module:
         return self._shard_modules_impl(module)
 
     def _init_optim(self, module: nn.Module) -> CombinedOptimizer:
         # pyre-ignore [6]
         return CombinedOptimizer(self._fused_optim_impl(module, []))
```

## torchrec/distributed/utils.py

```diff
@@ -224,15 +224,26 @@
         if tensor.device == current_device:
             return tensor.to(to_device)
         return tensor
 
     # if this is a sharded module, customize the copy
     if isinstance(copy_module, CopyMixIn):
         return copy_module.copy(to_device)
-
+    copied_param = {
+        name: torch.nn.Parameter(_copy_if_device_match(param.data))
+        for name, param in copy_module.named_parameters(recurse=False)
+    }
+    copied_buffer = {
+        name: _copy_if_device_match(buffer)
+        for name, buffer in copy_module.named_buffers(recurse=False)
+    }
+    for name, param in copied_param.items():
+        copy_module.register_parameter(name, param)
+    for name, buffer in copied_buffer.items():
+        copy_module.register_buffer(name, buffer)
     for child_name, child in copy_module.named_children():
         if not any([isinstance(submodule, CopyMixIn) for submodule in child.modules()]):
             child_copy = child._apply(_copy_if_device_match)
         else:
             child_copy = copy_to_device(child, current_device, to_device)
         copy_module.register_module(child_name, child_copy)
     return copy_module
```

## torchrec/distributed/test_utils/test_model.py

```diff
@@ -574,25 +574,29 @@
         self.sparse = TestSparseArch(
             tables,
             weighted_tables,
             sparse_device,
             max_feature_lengths_list if max_feature_lengths_list is not None else None,
         )
         self.over = TestOverArch(tables, weighted_tables, dense_device)
+        self.register_buffer(
+            "dummy_ones",
+            torch.ones(1, device=dense_device),
+        )
 
     def forward(
         self,
         input: ModelInput,
     ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         dense_r = self.dense(input.float_features)
         sparse_r = self.sparse(
             input.idlist_features, input.idscore_features, input.float_features.size(0)
         )
         over_r = self.over(dense_r, sparse_r)
-        pred = torch.sigmoid(torch.mean(over_r, dim=1))
+        pred = torch.sigmoid(torch.mean(over_r, dim=1)) + self.dummy_ones
         if self.training:
             return (
                 torch.nn.functional.binary_cross_entropy_with_logits(pred, input.label),
                 pred,
             )
         else:
             return pred
```

## torchrec/distributed/test_utils/test_model_parallel_base.py

```diff
@@ -639,38 +639,39 @@
         loss1, pred1 = m1(batch)
         loss2, pred2 = m2(batch)
         self.assertTrue(torch.equal(loss1, loss2))
         self.assertTrue(torch.equal(pred1, pred2))
 
         sd1 = m1.state_dict()
         for key, value in m2.state_dict().items():
-            table_name = key.split(".")[-2]
-            v2 = sd1[key]
-            if isinstance(value, ShardedTensor):
-                self.assertEqual(
-                    len(value.local_shards()), num_cw_shards_per_table[table_name]
-                )
-                dst = value.local_shards()[0].tensor
-            else:
-                dst = value
-
-            if isinstance(v2, ShardedTensor):
-                self.assertEqual(
-                    len(value.local_shards()), num_cw_shards_per_table[table_name]
-                )
+            if "." in key:
+                table_name = key.split(".")[-2]
+                v2 = sd1[key]
+                if isinstance(value, ShardedTensor):
+                    self.assertEqual(
+                        len(value.local_shards()), num_cw_shards_per_table[table_name]
+                    )
+                    dst = value.local_shards()[0].tensor
+                else:
+                    dst = value
 
-                for src_local_shard, dst_local_shard in zip(
-                    value.local_shards(), v2.local_shards()
-                ):
-                    self.assertTrue(
-                        torch.equal(src_local_shard.tensor, dst_local_shard.tensor)
+                if isinstance(v2, ShardedTensor):
+                    self.assertEqual(
+                        len(value.local_shards()), num_cw_shards_per_table[table_name]
                     )
-            else:
-                src = v2
-                self.assertTrue(torch.equal(src, dst))
+
+                    for src_local_shard, dst_local_shard in zip(
+                        value.local_shards(), v2.local_shards()
+                    ):
+                        self.assertTrue(
+                            torch.equal(src_local_shard.tensor, dst_local_shard.tensor)
+                        )
+                else:
+                    src = v2
+                    self.assertTrue(torch.equal(src, dst))
 
         for param_name, dst_param_group in dst_optimizer_state_dict.items():
             src_param_group = src_optimizer_state_dict[param_name]
 
             for state_key, dst_opt_state in dst_param_group.items():
                 table_name = state_key.split(".")[-2]
                 src_opt_state = src_param_group[state_key]
```

## torchrec/sparse/jagged_tensor.py

```diff
@@ -1008,27 +1008,28 @@
         Essentially, the lengths Tensor inferred by this function
         would be [2, 1, 1, 1, 3] indicating variable batch_size
         dim_1 violates the existing assumption / precondition
         that KeyedJaggedTensor's should have fixed batch_size dimension.
 
         """
         kjt_keys = list(jt_dict.keys())
-        kjt_vals = torch.concat(tuple(jt.values() for jt in jt_dict.values()))
-        kjt_lens = torch.concat(tuple(jt.lengths() for jt in jt_dict.values()))
-        kjt_weights = tuple(
-            jt.weights_or_none()
-            for jt in jt_dict.values()
-            if jt.weights_or_none() is not None
+        kjt_vals_list: List[torch.Tensor] = []
+        kjt_lens_list: List[torch.Tensor] = []
+        kjt_weights_list: List[torch.Tensor] = []
+        for jt in jt_dict.values():
+            kjt_vals_list.append(jt.values())
+            kjt_lens_list.append(jt.lengths())
+            weight = jt.weights_or_none()
+            if weight is not None:
+                kjt_weights_list.append(weight)
+        kjt_vals = torch.concat(kjt_vals_list)
+        kjt_lens = torch.concat(kjt_lens_list)
+        kjt_weights = (
+            torch.concat(kjt_weights_list) if len(kjt_weights_list) > 0 else None
         )
-        # pyre-ignore[6]: Incompatible parameter type [6]:
-        # In call `torch._C._VariableFunctions.concat`,
-        # for 1st positional only parameter
-        # expected `Union[List[Tensor], typing.Tuple[Tensor, ...]]`
-        # but got `typing.Tuple[Optional[Tensor], ...]`
-        kjt_weights = torch.concat(kjt_weights) if kjt_weights else None
         kjt = KeyedJaggedTensor(
             keys=kjt_keys,
             values=kjt_vals,
             weights=kjt_weights,
             lengths=kjt_lens,
         ).sync()
         return kjt
```

## Comparing `torchrec_nightly-2023.6.7.dist-info/LICENSE` & `torchrec_nightly-2023.6.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.6.7.dist-info/METADATA` & `torchrec_nightly-2023.6.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.6.7.dist-info/RECORD` & `torchrec_nightly-2023.6.8.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 torchrec/datasets/test_utils/criteo_test_utils.py,sha256=Ob2fJniGOsfbWNF_Gy2RJhrGAVnLAFPSlUTJOp2kay4,5308
 torchrec/distributed/__init__.py,sha256=VCy8GKOM-1dejxUWNSA3gozG3HQ4x5-Y9c9-WFbAMGg,1912
 torchrec/distributed/batched_embedding_kernel.py,sha256=_LWPI3zO_rObQgg0J0f-iojtpmazMfDfgHHg63hr_tE,37053
 torchrec/distributed/collective_utils.py,sha256=r7Aawq-KSVC-HjjEd6U8k0vNnRMx_-8_sAhYdElGaJw,2069
 torchrec/distributed/comm.py,sha256=21Std9n_HJCF3Nsw9O4yQQOJuL2DUVzZzoRhH3M6my8,4988
 torchrec/distributed/comm_ops.py,sha256=C63THNJOnJWkfRYGuNw5opFyKsdlpZs9_23u-DHSrAQ,55918
 torchrec/distributed/dist_data.py,sha256=pWuAzn98i5O4lNHmv2wMGa4gksYEh_DOJT4rzRp_nYg,35580
-torchrec/distributed/embedding.py,sha256=it9ImgDu3u42W94lOolqXAtI-duxPVu45dGGPi6NOIU,30257
+torchrec/distributed/embedding.py,sha256=U59gMHspqHedq1X4yb3DTLFTTxGn0YPjKd-CTDOu25g,31599
 torchrec/distributed/embedding_kernel.py,sha256=SNpvTbW1V4HtjSmAzPPa5imrUzSOe7zuQDkK3GFudHc,3872
 torchrec/distributed/embedding_lookup.py,sha256=1D7xO_ljztKkIIZJ7iziCI5mF65-S-l9hZ4Z6RAc1rY,28994
 torchrec/distributed/embedding_sharding.py,sha256=Kp8zJRIuBo_3XswENCCym9vnVId28Zh0HMoVqmcEoJI,18564
 torchrec/distributed/embedding_tower_sharding.py,sha256=ypr4JbTZUh_35dYUoKWoOSJNEVG3c6gV9g5gt-fs6lQ,37089
 torchrec/distributed/embedding_types.py,sha256=QbDVqeT2wb1RpnGZxrFtFdHYDsOHKW7SH8fLWmN_d0E,15030
 torchrec/distributed/embeddingbag.py,sha256=JffPXLKq_K0HAeSe8R3W3PrQuKowtdPTyHHez3qgdBs,35078
 torchrec/distributed/fbgemm_qcomm_codec.py,sha256=StYltKC6Eq6SE_YiX6GsVW3ZF0VyqTcGHXuCYmPAFlU,7373
 torchrec/distributed/fp_embeddingbag.py,sha256=tbwvTzBZXCBo_SSlyd7JnQOW6qWx1jdjmdeqnAnOaWM,5542
 torchrec/distributed/fused_embedding.py,sha256=uIgeaoEPujTgkcq8S2OPRYBe03J4TUF04uOOy_iRsMk,5273
 torchrec/distributed/fused_embeddingbag.py,sha256=7DIMc5sHdsDAgqCnNomcPo6V4aIH1wlkzyshHeJB3pc,5110
 torchrec/distributed/fused_params.py,sha256=THLZYo_6mErDx2DGMB3Fi_VFPpLKCrq6Amvg8CckjsA,1709
 torchrec/distributed/grouped_position_weighted.py,sha256=q-QE0U306BiPkXIAlJGIQ80EUDZj-FXTbWwjz3EyvLI,3807
-torchrec/distributed/model_parallel.py,sha256=GiDEkZ89gFUBE_7psmbpEVGqQ17UkryIGlxEXWSxnyk,19520
+torchrec/distributed/model_parallel.py,sha256=YzXWgCmmeA_ccHtqfzeDM5ZTnnFUXfYCtocx1pKHV7Q,19786
 torchrec/distributed/quant_embedding.py,sha256=tbUP4_-iVvfAZlJ7gCf5ZJb6snH35EFLeJrZhATUZD8,13729
 torchrec/distributed/quant_embedding_kernel.py,sha256=FNEKKje7yvnOI28ODg5POQy2pmeKWNmPvf193JF8iEw,13343
 torchrec/distributed/quant_embeddingbag.py,sha256=MxFdFDn4HAJ9PRc3ko_6q4O0KuWkh3_Y1BHajX0E9aY,10931
 torchrec/distributed/shard.py,sha256=4Dr5ixWCoMEFEuL5WN4fL2gIdl9wmSUjZWsiF-kdCdQ,9261
 torchrec/distributed/sharding_plan.py,sha256=vVQhmXy2w4FmXyuJa1t6PyfaqEEVSxoLZ5ChWlc7TbU,19411
 torchrec/distributed/train_pipeline.py,sha256=0twZDc4PIt2Sz6q2DEvyaz6P6jHb7-fmj_bTiA7ir7E,34059
 torchrec/distributed/types.py,sha256=tNd_B5PXjaOqPmUXxSZLXB3a71sjU8LBtSY9kuGxe7I,24927
-torchrec/distributed/utils.py,sha256=isPXbyPhHlbjiA0280ZY0V_wPUBuvDvvH4w6ziP5XA8,11373
+torchrec/distributed/utils.py,sha256=PbVfo9_QBugfSOvwmySdjXlhWOAYSl9eGpYYH0d0SqI,11873
 torchrec/distributed/composable/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/composable/table_batched_embedding_slice.py,sha256=x439M8TTXQtzoihan1OKKbmGYkqJlAxxTHCDz5295RY,3207
 torchrec/distributed/planner/__init__.py,sha256=UWnxb-SuE211uJGdwtSkKRVADT3plQozB2l6fvs6Ve0,1025
 torchrec/distributed/planner/constants.py,sha256=MkeVqYO2QGg57i6fs29lZb2dScaaR9mdQVsee4NxyFc,3135
 torchrec/distributed/planner/enumerators.py,sha256=hZzhnfMrOz65lBoddxTKBb01hm43R_5tdpysJFSzCLE,10318
 torchrec/distributed/planner/partitioners.py,sha256=k-rzm6oMZ_sLpGHT8yAu2tIMkMumhJMvAFeY0cdNirk,12642
 torchrec/distributed/planner/perf_models.py,sha256=vYIjVr0NG6sZItfxVuRWF7AS8lGGtbRn66O0flNJpoU,835
@@ -65,17 +65,17 @@
 torchrec/distributed/sharding/tw_sequence_sharding.py,sha256=SR_G_rniSZx_DBnrWW14HEMoeqwRnMPN3LdQlnptLL8,7692
 torchrec/distributed/sharding/tw_sharding.py,sha256=JtI2GW9YR-eg1VuQDwDa6qaR6sOgBAzGx3Y3XkEOBZM,16315
 torchrec/distributed/sharding/twcw_sharding.py,sha256=LyOowcADWmRdkRn-eEW6QB0b0xYi0vM-Ubrr6N2zwwA,1284
 torchrec/distributed/sharding/twrw_sharding.py,sha256=k69AX5oKj3ep38tM_RI_NkwyZ4z_U8kVQpLtDjRYPKI,19898
 torchrec/distributed/test_utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 torchrec/distributed/test_utils/infer_utils.py,sha256=v3OLVjfmy612aSSDPpFeu8m7K9omDAO9JFWQ08NHcZI,10213
 torchrec/distributed/test_utils/multi_process.py,sha256=6AxYe2cO44EGdw-Lt5YNwqmWZW8Ldu7bVGTluIIOFbA,4868
-torchrec/distributed/test_utils/test_model.py,sha256=x4DxsGp6YfBBJMyrkBwOZTFpotm6VB8V6tLxuanHNFM,34114
+torchrec/distributed/test_utils/test_model.py,sha256=ACqCdD3bcxX74JihIg7jTcLvBsV8U-Bvwvy9-Pbj7nI,34246
 torchrec/distributed/test_utils/test_model_parallel.py,sha256=oN_fl-QOaAarrZwnr7q5Lz4f9xiqxxof9Bk_4PM13hM,11193
-torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=05SOQyzfHS5jyZkSzUNmhGa3sT43cX2M_w_FiWrZhBw,25075
+torchrec/distributed/test_utils/test_model_parallel_base.py,sha256=gny2CZ7n4GUzIwAAKw6Iuq0lgd7LL5mhwKKR_gvG9uE,25190
 torchrec/distributed/test_utils/test_sharding.py,sha256=DlB6N5-qlRp-xQfEEFElDkNffnEX6LO4vOrDCGp8VkQ,15367
 torchrec/fx/__init__.py,sha256=TxNjllMWlB_rpDy4SNSA_e-xbZbhxGGTb9AxpZGcaFk,422
 torchrec/fx/tracer.py,sha256=iXfWWgPNdFlRs89RbA18Nel0Tl9z8UprRWPfTQbLx5k,6477
 torchrec/fx/utils.py,sha256=N50AfwlUhyS9r1Sv21fSbqRxiOk4KRX0MX9sDjCaQcA,4401
 torchrec/inference/__init__.py,sha256=vi2C_o1Bvsp6hS3_uVZTL7kShgxw5qFZp248Svee2Og,1223
 torchrec/inference/client.py,sha256=jS6ldQxBRY3Bp_LwDLUNSlPt2VYMc-Hsd4iKKoHfDVU,3614
 torchrec/inference/model_packager.py,sha256=HxOEbnqXB2K4uUB9dBBJAL49ZYJME4xTFyVzKjpsjy4,3957
@@ -129,15 +129,15 @@
 torchrec/optim/rowwise_adagrad.py,sha256=jHpCZDFWRrXbwlKiwROg2dl0qK1lG2uXMJkTtbZ_uSg,7405
 torchrec/optim/warmup.py,sha256=QaMcWU-jMZbDOfRHEH_x9r7EsjtI_LRgOGAmEgzJWSQ,4865
 torchrec/optim/test_utils/__init__.py,sha256=mkNZr5iNV3kseuamPBnnAeknjbv4ELPFMGyJ1lWiJGU,560
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
 torchrec/quant/embedding_modules.py,sha256=RLuYVywThBXgLEZeHrH2F1sGEA1XydzBg4S9v2rivgY,22933
 torchrec/quant/utils.py,sha256=PkgXn7wnnBIqJ5JAidJMvpAVre1YL8oiYGiPuV_gU2c,4100
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
-torchrec/sparse/jagged_tensor.py,sha256=t0QsLwPZ9l2M5by3FpGOPXL6KeSWQqOp7hLayDF-DAc,55649
+torchrec/sparse/jagged_tensor.py,sha256=3874Ka-1XE6nsvHIVu8iGM6l3nNlSF7PQW-fM5rnl4c,55583
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.6.7.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.6.7.dist-info/METADATA,sha256=x1noP6QhxigUnv0YlJoJ2G4cszwwJmHhqws3anadwdY,5011
-torchrec_nightly-2023.6.7.dist-info/WHEEL,sha256=LFkqBJk4I7hCv0noSqfZr_dqF1ghJkoTPb1XzfEVHuI,93
-torchrec_nightly-2023.6.7.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.6.7.dist-info/RECORD,,
+torchrec_nightly-2023.6.8.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.6.8.dist-info/METADATA,sha256=BwIzJWdT-QmzyTfPYoxkWS7MlNvibruyLtEneEF3c-s,5011
+torchrec_nightly-2023.6.8.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
+torchrec_nightly-2023.6.8.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.6.8.dist-info/RECORD,,
```

