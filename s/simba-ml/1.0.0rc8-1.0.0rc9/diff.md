# Comparing `tmp/simba_ml-1.0.0rc8.tar.gz` & `tmp/simba_ml-1.0.0rc9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simba_ml-1.0.0rc8.tar", last modified: Thu Jun  8 13:17:19 2023, max compression
+gzip compressed data, was "simba_ml-1.0.0rc9.tar", last modified: Fri Jun  9 11:01:51 2023, max compression
```

## Comparing `simba_ml-1.0.0rc8.tar` & `simba_ml-1.0.0rc9.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.634576 simba_ml-1.0.0rc8/simba_ml/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-08 13:17:19.634576 simba_ml-1.0.0rc8/simba_ml/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.618576 simba_ml-1.0.0rc8/simba_ml/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/generate_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.618576 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/problem_viewer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/run_problem_viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/cli/start_prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4644 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/error_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/example_problems/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/constant_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/salt_and_brine_tanks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/sir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/sird.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/example_problems/trigonometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/logging/logging_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/logging/wandb_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/plugin_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/preprocessing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/config/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/config/steady_state_data_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/dataset_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/splits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/time_series_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/data_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/splits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/window_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.622576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/average_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/dense_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/last_value_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     7032 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/keep_species_sum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_in_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_truncator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.626576 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/derivative_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/beta_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/continuous_uniform_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/lognormal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/normal_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/distributions/vector_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/generators/
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/generator_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/pertubation_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/steady_state_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_points_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_series_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/additive_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/adjusting_mean_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/column_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/elastic_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multi_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multiplicative_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/no_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/noisers/sequential_noiser.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/random_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/constant_suffix_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/interval_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/no_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/random_sample_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/sequential_sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/sparsifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/species.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.630576 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:17:19.618576 simba_ml-1.0.0rc8/simba_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 13:17:19.000000 simba_ml-1.0.0rc8/simba_ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-08 13:13:29.000000 simba_ml-1.0.0rc8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/simba_ml/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-09 11:01:51.470151 simba_ml-1.0.0rc9/simba_ml/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.446151 simba_ml-1.0.0rc9/simba_ml/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/generate_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.446151 simba_ml-1.0.0rc9/simba_ml/cli/problem_viewer/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/problem_viewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/problem_viewer/problem_viewer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      693 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/problem_viewer/run_problem_viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/cli/start_prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/error_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.446151 simba_ml-1.0.0rc9/simba_ml/example_problems/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/example_problems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/example_problems/constant_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/example_problems/salt_and_brine_tanks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/example_problems/sir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/example_problems/sird.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/example_problems/trigonometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.446151 simba_ml-1.0.0rc9/simba_ml/prediction/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/logging/logging_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/logging/wandb_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/plugin_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/preprocessing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/config/steady_state_data_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/dataset_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/splits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.450151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/mixed_data_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/mixed_data_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/mixed_data_pipeline/data_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.454151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/synthetic_data_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/synthetic_data_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/synthetic_data_pipeline/data_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/time_series_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.454151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/transfer_learning_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/transfer_learning_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/transfer_learning_pipeline/data_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.454151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/splits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/window_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.454151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/metrics/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14058 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.454151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/average_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.458151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/dense_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/last_value_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.458151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7211 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.458151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2160 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/transfer_learning_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/transfer_learning_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.458151 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.458151 simba_ml-1.0.0rc9/simba_ml/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.458151 simba_ml-1.0.0rc9/simba_ml/simulation/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/constraints/keep_species_sum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/constraints/species_value_in_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/constraints/species_value_truncator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.462151 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/derivative_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.462151 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/beta_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/continuous_uniform_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/lognormal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/normal_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/distributions/vector_distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.462151 simba_ml-1.0.0rc9/simba_ml/simulation/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/generators/generator_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/generators/pertubation_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/generators/steady_state_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/generators/time_points_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/generators/time_series_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.462151 simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/additive_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/adjusting_mean_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/column_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/elastic_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/multi_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/multiplicative_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/no_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/noisers/sequential_noiser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/random_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4029 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/constant_suffix_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/interval_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/no_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/random_sample_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/sequential_sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/sparsifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/species.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.466151 simba_ml-1.0.0rc9/simba_ml/simulation/system_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/system_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11654 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/system_model/system_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/simba_ml/simulation/system_model/system_model_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:01:51.446151 simba_ml-1.0.0rc9/simba_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-06-09 11:01:51.000000 simba_ml-1.0.0rc9/simba_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-09 11:01:51.000000 simba_ml-1.0.0rc9/simba_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:01:51.000000 simba_ml-1.0.0rc9/simba_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 11:01:51.000000 simba_ml-1.0.0rc9/simba_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-09 11:01:51.000000 simba_ml-1.0.0rc9/simba_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 11:01:51.000000 simba_ml-1.0.0rc9/simba_ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-06-09 10:56:53.000000 simba_ml-1.0.0rc9/versioneer.py
```

### Comparing `simba_ml-1.0.0rc8/PKG-INFO` & `simba_ml-1.0.0rc9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simba_ml
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Simulation-Based Machine Learning
 Home-page: UNKNOWN
 Author: Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews
 Author-email: maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/DILiS-lab/SimbaML/issues
 Project-URL: Source Code, https://github.com/DILiS-lab/SimbaML
```

### Comparing `simba_ml-1.0.0rc8/README.md` & `simba_ml-1.0.0rc9/README.md`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/setup.cfg` & `simba_ml-1.0.0rc9/setup.cfg`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/setup.py` & `simba_ml-1.0.0rc9/setup.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/cli/generate_data.py` & `simba_ml-1.0.0rc9/simba_ml/cli/generate_data.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/problem_viewer.py` & `simba_ml-1.0.0rc9/simba_ml/cli/problem_viewer/problem_viewer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/cli/problem_viewer/run_problem_viewer.py` & `simba_ml-1.0.0rc9/simba_ml/cli/problem_viewer/run_problem_viewer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/cli/start_prediction.py` & `simba_ml-1.0.0rc9/simba_ml/cli/start_prediction.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/error_handler.py` & `simba_ml-1.0.0rc9/simba_ml/error_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,49 +59,47 @@
         TypeError: If sequence contains other data types than float and int.
     """
     if not all(isinstance(v, (float, int)) for v in sequence_):
         raise TypeError(f"All values of {param_name} must be float or int.")
 
 
 def confirm_number_is_greater_or_equal_to_0(
-    number: typing.Union[int, float], param_name: str = "param"
+    number: float, param_name: str = "param"
 ) -> None:
     """Checks that a number is greater or equal to 0.
 
     Args:
         number: The number that gets confirmed.
         param_name: Optional name to display in the error message.
 
     Raises:
         ValueError: If param is < 0.
     """
     if number < 0:
         raise ValueError(f"{param_name} must be >= 0, not {number}.")
 
 
-def confirm_number_is_greater_than_0(
-    number: typing.Union[int, float], param_name: str = "param"
-) -> None:
+def confirm_number_is_greater_than_0(number: float, param_name: str = "param") -> None:
     """Checks that a number is greater than 0.
 
     Args:
         number: The number that gets confirmed.
         param_name: Optional name to display in the error message.
 
     Raises:
         ValueError: If param <= 0.
     """
     if number <= 0:
         raise ValueError(f"{param_name} must be > 0, not {number}.")
 
 
 def confirm_number_is_in_interval(
-    number: typing.Union[int, float],
-    start_value: typing.Union[int, float],
-    end_value: typing.Union[int, float],
+    number: float,
+    start_value: float,
+    end_value: float,
     include_left: bool = True,
     include_right: bool = True,
     param_name: str = "param",
 ) -> None:
     """Checks that a number lays in an intervall.
 
     Args:
@@ -119,15 +117,15 @@
     right = number <= end_value if include_right else number < end_value
 
     if not (left and right):
         interval_type_left = "inclusive" if include_left else "exclusive"
         interval_type_right = "inclusive" if include_right else "exclusive"
         raise ValueError(
             f"{param_name} must be a value between {start_value} ({interval_type_left})"
-            f"and {end_value} ({interval_type_right}), not {str(number)}."
+            f"and {end_value} ({interval_type_right}), not {number}."
         )
 
 
 def confirm_sequence_is_not_empty(
     sequence_: collections.abc.Sequence[typing.Any], param_name: str = "param"
 ) -> None:
     """Checks that a sequence in not empty.
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/example_problems/constant_function.py` & `simba_ml-1.0.0rc9/simba_ml/example_problems/constant_function.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/example_problems/salt_and_brine_tanks.py` & `simba_ml-1.0.0rc9/simba_ml/example_problems/salt_and_brine_tanks.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/example_problems/sir.py` & `simba_ml-1.0.0rc9/simba_ml/example_problems/sir.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/example_problems/sird.py` & `simba_ml-1.0.0rc9/simba_ml/example_problems/sird.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/example_problems/trigonometry.py` & `simba_ml-1.0.0rc9/simba_ml/example_problems/trigonometry.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/export.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/export.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/logging/wandb_logger.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/logging/wandb_logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 P = typing.ParamSpec("P")
 T = typing.TypeVar("T")
 
 
 class WandbLogger:
     """Wrapper for wandb logging."""
 
-    def __init__(self, config: typing.Optional[logging_config.LoggingConfig]) -> None:
+    def __init__(self, config: logging_config.LoggingConfig | None) -> None:
         """Initializes the wandb logger.
 
         Args:
             config: The config of the wandb logger.
         """
         self.config = config
 
@@ -29,30 +29,26 @@
         """
         if self.config is None:
             return
         wandb.init(
             *args, **kwargs, project=self.config.project, entity=self.config.entity
         )
 
-    def __getattr__(self, name: str) -> typing.Callable[..., typing.Optional[T]]:
+    def __getattr__(self, name: str) -> typing.Callable[..., T | None]:
         """Passes the message to wandb if wandb logging is enabled.
 
         Args:
             name: The name of the wandb function to call.
 
         Returns:
             A function that calls the corresponding wandb function
             if wandb logging is enabled.
         """
         func = getattr(wandb, name)
 
-        def outer(
-            func: typing.Callable[..., T]
-        ) -> typing.Callable[..., typing.Optional[T]]:
-            def pass_message(
-                *args: typing.Any, **kwargs: typing.Any
-            ) -> typing.Optional[T]:
+        def outer(func: typing.Callable[..., T]) -> typing.Callable[..., T | None]:
+            def pass_message(*args: typing.Any, **kwargs: typing.Any) -> T | None:
                 return func(*args, **kwargs) if self.config is not None else None
 
             return pass_message
 
         return outer(func)
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/normalizer.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/normalizer.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/plugin_loader.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/preprocessing.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/preprocessing.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/dataset_generator.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/dataset_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/mixed_data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module provides the dataloader."""
 import os
-from typing import Optional, Tuple
+from typing import Tuple
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
 from simba_ml.prediction import preprocessing
 from simba_ml.prediction.steady_state.config import steady_state_data_config
@@ -18,16 +18,16 @@
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets,
             one for each ratio of synthethic to observed data.
     """
 
     config: steady_state_data_config.DataConfig
-    __X_test: Optional[npt.NDArray[np.float64]] = None
-    __y_test: Optional[npt.NDArray[np.float64]] = None
+    __X_test: npt.NDArray[np.float64] | None = None
+    __y_test: npt.NDArray[np.float64] | None = None
     __list_of_train_validation_sets: list[
         list[dict[str, list[npt.NDArray[np.float64]]]]
     ] = []
 
     def __init__(self, config: steady_state_data_config.DataConfig) -> None:
         """Inits the DataLoader.
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/steady_state/data_loader/splits.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/steady_state/data_loader/splits.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/mixed_data_pipeline/pipeline_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Provides the configuration for the pipeline."""
-import typing
 import dataclasses
 
 from simba_ml.prediction.time_series.config.mixed_data_pipeline import (
     data_config,
 )
 from simba_ml.prediction.logging import logging_config
 from simba_ml.prediction.time_series.metrics import factory as metrics_factory
@@ -15,15 +14,15 @@
     """Config for the Pipeline."""
 
     models: list[dict[str, object]]
     metrics: list[str]
     data: data_config.DataConfig
     plugins: list[str] = dataclasses.field(default_factory=list)
     metric_functions: dict[str, metrics_module.Metric] = dataclasses.field(init=False)
-    logging: typing.Optional[logging_config.LoggingConfig] = None
+    logging: logging_config.LoggingConfig | None = None
     seed: int = 42
 
     def __post_init__(self) -> None:
         """Inits the PipelineConfig.
 
         Creates a dict mapping the given metric_ids to their respective functions.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/synthetic_data_pipeline/pipeline_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Provides the configuration for the pipeline."""
-import typing
 import dataclasses
 
 from simba_ml.prediction.time_series.config.synthetic_data_pipeline import (
     data_config,
 )
 from simba_ml.prediction.logging import (
     logging_config,
@@ -17,15 +16,15 @@
     """Config for the Pipeline."""
 
     models: list[dict[str, object]]
     metrics: list[str]
     data: data_config.DataConfig
     plugins: list[str] = dataclasses.field(default_factory=list)
     metric_functions: dict[str, metrics_module.Metric] = dataclasses.field(init=False)
-    logging: typing.Optional[logging_config.LoggingConfig] = None
+    logging: logging_config.LoggingConfig | None = None
     seed: int = 42
 
     def __post_init__(self) -> None:
         """Inits the PipelineConfig.
 
         Creates a dict mapping the given metric_ids to their respective functions.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/config/transfer_learning_pipeline/pipeline_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Provides the configuration for the pipeline."""
 import dataclasses
-import typing
 
 from simba_ml.prediction.time_series.config.transfer_learning_pipeline import (
     data_config,
 )
 from simba_ml.prediction.logging import (
     logging_config,
 )
@@ -15,15 +14,15 @@
 @dataclasses.dataclass
 class PipelineConfig:
     """Config for the Pipeline."""
 
     models: list[dict[str, object]]
     metrics: list[str]
     data: data_config.DataConfig
-    logging: typing.Optional[logging_config.LoggingConfig] = None
+    logging: logging_config.LoggingConfig | None = None
     plugins: list[str] = dataclasses.field(default_factory=list)
     metric_functions: dict[str, metrics_module.Metric] = dataclasses.field(init=False)
     seed: int = 42
 
     def __post_init__(self) -> None:
         """Inits the PipelineConfig.
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/mixed_data_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module provides the dataloader."""
 import os
-from typing import Optional, Tuple
+from typing import Tuple
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
 from simba_ml.prediction.time_series.config.mixed_data_pipeline import (
     data_config,
@@ -21,17 +21,17 @@
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets, one for each ratio of
             synthethic to observed data
     """
 
     config: data_config.DataConfig
-    __X_test: Optional[npt.NDArray[np.float64]] = None
-    __y_test: Optional[npt.NDArray[np.float64]] = None
-    __train_sets: Optional[dict[float, list[npt.NDArray[np.float64]]]] = None
+    __X_test: npt.NDArray[np.float64] | None = None
+    __y_test: npt.NDArray[np.float64] | None = None
+    __train_sets: dict[float, list[npt.NDArray[np.float64]]] | None = None
 
     def __init__(self, config: data_config.DataConfig) -> None:
         """Inits the DataLoader.
 
         Args:
             config: the data configuration.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/splits.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/splits.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/synthetic_data_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """This module provides the dataloader."""
 import os
-from typing import Optional
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
 from simba_ml.prediction.time_series.config.synthetic_data_pipeline import (
     data_config,
@@ -21,17 +20,17 @@
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets, one for each ratio of
             synthethic to observed data
     """
 
     config: data_config.DataConfig
-    __X_test: Optional[npt.NDArray[np.float64]] = None
-    __y_test: Optional[npt.NDArray[np.float64]] = None
-    __train: Optional[list[npt.NDArray[np.float64]]] = None
+    __X_test: npt.NDArray[np.float64] | None = None
+    __y_test: npt.NDArray[np.float64] | None = None
+    __train: list[npt.NDArray[np.float64]] | None = None
 
     def __init__(self, config: data_config.DataConfig) -> None:
         """Inits the DataLoader.
 
         Args:
             config: the data configuration.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/transfer_learning_data_loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """This module provides the dataloader."""
 import os
-from typing import Optional, Tuple
+from typing import Tuple
 
 import pandas as pd
 import numpy as np
 from numpy import typing as npt
 
 from simba_ml.prediction.time_series.config.transfer_learning_pipeline import (
     data_config,
@@ -21,18 +21,18 @@
         X_test: the input of the test data
         y_test: the labels for the test data
         train_validation_sets: list of validations sets, one for each ratio of
             synthethic to observed data
     """
 
     config: data_config.DataConfig
-    __X_test: Optional[npt.NDArray[np.float64]] = None
-    __y_test: Optional[npt.NDArray[np.float64]] = None
-    __train_observed: Optional[list[npt.NDArray[np.float64]]] = None
-    __train_synthetic: Optional[list[npt.NDArray[np.float64]]] = None
+    __X_test: npt.NDArray[np.float64] | None = None
+    __y_test: npt.NDArray[np.float64] | None = None
+    __train_observed: list[npt.NDArray[np.float64]] | None = None
+    __train_synthetic: list[npt.NDArray[np.float64]] | None = None
 
     def __init__(self, config: data_config.DataConfig) -> None:
         """Inits the DataLoader.
 
         Args:
             config: the data configuration.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/data_loader/window_generator.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/data_loader/window_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/factory.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/metrics/factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/metrics/metrics.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/average_predictor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/average_predictor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/factory.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/dense_neural_network.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/dense_neural_network.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/keras/keras_model.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/keras/keras_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/last_value_predictor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/last_value_predictor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/model_to_transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/dense_neural_network.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/pytorch_lightning/pytorch_lightning_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Provides a model that predicts next timesteps from with a\
      pytorch lightning architecture."""
 import abc
 import dataclasses
-import typing
 
 import torch
 from torch import utils
 import numpy as np
 import numpy.typing as npt
 import pandas as pd
 
@@ -50,17 +49,18 @@
 
     patience: int = 5
     batch_size: int = 32
     validation_split: float = 0.2
     verbose: int = 0
     accelerator: str = "auto"
     learning_rate: float = 0.001
-    finetuning_learning_rate: typing.Optional[float] = None
+    finetuning_learning_rate: float | None = None
     epochs: int = 10
-    finetuning_epochs: typing.Optional[int] = None
+    finetuning_epochs: int | None = None
+    show_progress_bar: bool = True
 
 
 @dataclasses.dataclass
 class PytorchLightningModelConfig(model.ModelConfig):
     """Defines the configuration for the PytorchLightningModel."""
 
     name: str = "Pytorch Lightning Model"
@@ -162,20 +162,22 @@
         """
         if self.model_params.finetuning:
             check_finetuning_params(self.model_params)
             trainer = pl.Trainer(
                 max_epochs=self.model_params.training_params.finetuning_epochs,
                 log_every_n_steps=len(train_loader) // 2,
                 accelerator=self.model_params.training_params.accelerator,
+                enable_progress_bar=self.model_params.training_params.show_progress_bar,
             )
         else:
             trainer = pl.Trainer(
                 max_epochs=self.model_params.training_params.epochs,
                 log_every_n_steps=len(train_loader) // 2,
                 accelerator=self.model_params.training_params.accelerator,
+                enable_progress_bar=self.model_params.training_params.show_progress_bar,
             )
         trainer.fit(self.model, train_loader)
 
     def predict(self, data: npt.NDArray[np.float64]) -> npt.NDArray[np.float64]:
         """Predicts the next timestamps for every row (time series).
 
         Args:
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/decision_tree_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/linear_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """Provides a model, which predicts next timesteps from with a linear regressor."""
-import typing
 import dataclasses
 
 import sklearn as sk
 from sklearn import linear_model
 
 from simba_ml.prediction.time_series.models.sk_learn import sk_learn_model
 from simba_ml.prediction.time_series.config import (
@@ -19,15 +18,15 @@
         name: name of the model.
         criterion: the function to measure the quality of a split.
         splitter: the strategy used to choose the split at each node.
     """
 
     name: str = "Linear Regressor"
     fit_intercept: bool = True
-    n_jobs: typing.Optional[int] = None
+    n_jobs: int | None = None
     positive: bool = False
 
 
 class LinearRegressorModel(sk_learn_model.SkLearnModel):
     """Defines a model, which uses a Linear Regressor to predict the next timestamps."""
 
     def __init__(
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/nearest_neighbors_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/random_forest_regressor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Provides a model, which predicts next timesteps with a random forest regressor."""
 import enum
 import dataclasses
-import typing
 import sklearn as sk
 from sklearn import ensemble
 
 from simba_ml.prediction.time_series.models.sk_learn import sk_learn_model
 from simba_ml.prediction.time_series.config import (
     time_series_config,
 )
@@ -45,15 +44,15 @@
         criterion: the function to measure the quality of a split.
         splitter: the strategy used to choose the split at each node.
     """
 
     name: str = "Random Forest Regressor"
     criterion: Criterion = Criterion.squared_error
     n_estimators: int = 100
-    max_depth: typing.Optional[int] = None
+    max_depth: int | None = None
     min_samples_split: int = 2
     min_samples_leaf: int = 1
     min_weight_fraction_leaf: float = 0.0
 
 
 class RandomForestRegressorModel(sk_learn_model.SkLearnModel):
     """Defines a model, which uses a Random Forest regressor."""
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/sk_learn_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/sk_learn/support_vector_machine_regressor.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_factory.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/transfer_learning_factory.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/models/transfer_learning_model.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/models/transfer_learning_model.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/mixed_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/synthetic_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py` & `simba_ml-1.0.0rc9/simba_ml/prediction/time_series/pipelines/transfer_learning_pipeline.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/constraint.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/constraints/constraint.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/keep_species_sum.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/constraints/keep_species_sum.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Provides a constranit, which does nothing."""
-from typing import Optional
 import math
 import pandas as pd
 from simba_ml.simulation.constraints import constraint
 from simba_ml.simulation.system_model import system_model_interface
 
 
 class KeepSpeciesSum(constraint.Constraint):
     """Keeps the sum of specieses constant at every timestep."""
 
     def __init__(
         self,
         sm: system_model_interface.SystemModelInterface,
-        specieses_to_hold_sum: Optional[list[str]] = None,
-        species_sum: Optional[int] = None,
+        specieses_to_hold_sum: list[str] | None = None,
+        species_sum: int | None = None,
     ):
         """Inits `KeepSpeciesSum`.
 
         Args:
             sm: A SystemModel, on which the constraint will be applied.
             specieses_to_hold_sum: The specieses, for which the sum has to be constant.
                 If None, all specieses will be taken into account.
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_in_range.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/constraints/species_value_in_range.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/constraints/species_value_truncator.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/constraints/species_value_truncator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/additive_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/derivative_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/derivative_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/multi_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/multiplicative_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/no_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/derivative_noiser/sequential_deriv_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/beta_distribution.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/beta_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Defines Beta Distribution."""
 
-import typing
-
 from scipy import stats
 
 from simba_ml import error_handler
 
 from simba_ml.simulation import random_generator
 
 
@@ -19,17 +17,15 @@
     Raises:
         TypeError: If alpha is not float or int.
         TypeError: If beta is not float or int.
         ValueError: If alpha <= 0.
         ValueError: If beta <= 0.
     """
 
-    def __init__(
-        self, alpha: typing.Union[float, int], beta: typing.Union[float, int]
-    ) -> None:
+    def __init__(self, alpha: float, beta: float) -> None:
         """Inits `BetaDistribution` with the provided arguments.
 
         Args:
             alpha: Alpha parameter of the distributions.
             beta: Beta parameter of the distributions.
         """
         self.alpha = alpha
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/constant.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/constant.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/continuous_uniform_distribution.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/continuous_uniform_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Defines Continuous Uniform Distribution."""
 
-import typing
-
 import numpy as np
 
 from simba_ml import error_handler
 from simba_ml.simulation import random_generator
 
 
 class ContinuousUniformDistribution:
@@ -16,17 +14,15 @@
         max_value: the maximal value of the distributions.
 
     Raises:
         TypeError: If min_value is not float or int.
         TypeError: If max_value is not float or int.
     """
 
-    def __init__(
-        self, min_value: typing.Union[float, int], max_value: typing.Union[float, int]
-    ) -> None:
+    def __init__(self, min_value: float, max_value: float) -> None:
         """Inits ContinuousUniformDistribution with the provided arguments.
 
         Args:
             min_value: the minimal value of the distributions.
             max_value: the maximal value of the distributions.
         """
         self.min_value = min_value
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/distribution.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/distribution.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/helper_functions.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/lognormal_distribution.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/lognormal_distribution.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Defines Lognormal Distribution."""
 
-import typing
-
 from scipy import stats
 
 from simba_ml import error_handler
 from simba_ml.simulation import random_generator
 
 
 class LogNormalDistribution:
@@ -18,17 +16,15 @@
 
     Raises:
         ValueError: If sigma < 0.
         TypeError: If mu is not float or int.
         TypeError: If sigma is not float or int.
     """
 
-    def __init__(
-        self, mu: typing.Union[float, int], sigma: typing.Union[float, int]
-    ) -> None:
+    def __init__(self, mu: float, sigma: float) -> None:
         """Inits LogNormalDistribution with the provided arguments.
 
         Args:
             mu: Mean ("centre") of the distributions.
             sigma: Standard deviation (spread or "width") of the distributions.
                 Must be non-negative.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/normal_distribution.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/normal_distribution.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Defines the Normal Distribution."""
 
-import typing
-
 from scipy import stats
 
 from simba_ml import error_handler
 from simba_ml.simulation import random_generator
 
 
 class NormalDistribution:
@@ -18,17 +16,15 @@
 
     Raises:
         ValueError: If sigma < 0.
         TypeError: If mu is not float or int.
         TypeError: If sigma is not float or int.
     """
 
-    def __init__(
-        self, mu: typing.Union[float, int], sigma: typing.Union[float, int]
-    ) -> None:
+    def __init__(self, mu: float, sigma: float) -> None:
         """Inits NormalDistribution with the provided arguments.
 
         Args:
             mu: Mean ("centre") of the distributions.
             sigma: Standard deviation (spread or "width") of the distributions.
                 Must be non-negative.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/distributions/vector_distribution.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/distributions/vector_distribution.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Defines Vector Distribution."""
 
-import typing
-
 from simba_ml import error_handler
 from simba_ml.simulation import random_generator
 
 
 class VectorDistribution:
     """An object which samples values from a list of numbers.
 
@@ -13,15 +11,15 @@
         values: A list containing values.
 
     Raises:
         IndexError: If values is empty.
         TypeError: If values contains a value which is not a float or int.
     """
 
-    def __init__(self, values: list[typing.Union[float, int]]) -> None:
+    def __init__(self, values: list[float]) -> None:
         """Inits VectorDistribution with the provided arguments.
 
         Args:
             values: A list containing all the valid values.
         """
         self.values = values
         error_handler.confirm_sequence_is_not_empty(self.values, "values")
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/generators/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/generators/generator_interface.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/generators/generator_interface.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/generators/pertubation_generator.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/generators/pertubation_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     and a table containing the concrete start values for the species, arguments and
     the according steady-states is returned.
     """
 
     def __init__(
         self,
         sm: system_model_interface.SystemModelInterface,
-        species_start_values_noiser: typing.Optional[noisers.Noiser] = None,
-        kinetic_parameters_noiser: typing.Optional[noisers.Noiser] = None,
+        species_start_values_noiser: noisers.Noiser | None = None,
+        kinetic_parameters_noiser: noisers.Noiser | None = None,
     ):
         """Initializes the `PertubationGenerator`.
 
         Note:
             Only the use of a constant_kinetic_parameter is allowed.
 
         Args:
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/generators/steady_state_generator.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/generators/steady_state_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_points_generator.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/generators/time_points_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/generators/time_series_generator.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/generators/time_series_generator.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/constant_kinetic_parameter.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     Attributes:
         samples: The kinetic parameters for each run (time series)
             of the current simulation.
         distribution: The distribution for possible values of the kinetic parameter.
     """
 
-    samples: typing.Optional[list[T]] = None
+    samples: list[T] | None = None
 
     def __init__(self, distribution: distribution_module.Distribution[T]):
         """Initializes a constant kinetic parameter.
 
         Args:
             distribution: The distribution for possible values of the kinetic parameter.
         """
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/dict_based_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/function_based_kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/kinetic_parameters/kinetic_parameter.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/additive_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/additive_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/adjusting_mean_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/adjusting_mean_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/column_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/column_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/elastic_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/elastic_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multi_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/multi_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/multiplicative_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/multiplicative_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/noisers/sequential_noiser.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/noisers/sequential_noiser.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/__init__.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/__init__.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/constant_suffix_remover.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/constant_suffix_remover.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/interval_sparsifier.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/interval_sparsifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 """Removes a given relative amount of samples from a signal."""
-import typing
-
 import pandas as pd
 
 from simba_ml.simulation.sparsifier import sparsifier as sparsifier_module
 
 
 class IntervalSparsifier(sparsifier_module.Sparsifier):
     """A `Sparsifier` that sparsifies intervals with different `Sparsifier`.
 
     The `IntervalSparsifier` takes sparsifiers and interval endings as arguments.
     The sparsifiers are applied to the according intervals.
     """
 
     def __init__(
         self,
-        *kinetic_parameters: tuple[
-            sparsifier_module.Sparsifier, typing.Union[int, str]
-        ],
+        *kinetic_parameters: tuple[sparsifier_module.Sparsifier, int | str],
     ) -> None:
         """Inits the `IntervalSparsifier`.
 
         Args:
             *kinetic_parameters: Pairs of (sparsifier, end_of_interval) where the
                 end_of_interval is the last timestep, where the sparsifier should
                 be applied. end_of_interval can either be represented explicit as
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/keep_extreme_values_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/no_sparsifier.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/no_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/random_sample_sparsifier.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/random_sample_sparsifier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Removes a given relative amount of samples from a signal."""
-import typing
-
 import pandas as pd
 
 from simba_ml import error_handler
 from simba_ml.simulation.sparsifier import sparsifier
 
 
 class RandomSampleSparsifier(sparsifier.Sparsifier):
@@ -15,23 +13,23 @@
             0 <= frac <= 1.
 
     Raises:
         TypeError: If frac is not a float.
         ValueError: If frac not in the interval [0, 1].
     """
 
-    def __init__(self, frac: typing.Union[float, int] = 0.5) -> None:
+    def __init__(self, frac: float = 0.5) -> None:
         """Inits the `RandomSampleSparsiier`.
 
         Args:
             frac: The relative amount of samples to keep from the incoming signal.
         """
         error_handler.confirm_param_is_float_or_int(frac, "frac")
         error_handler.confirm_number_is_in_interval(frac, 0, 1, param_name="frac")
-        self.frac = float(frac)
+        self.frac = frac
 
     def sparsify(self, signal: pd.DataFrame) -> pd.DataFrame:
         """Removes some (`1-frac`) samples chosen with a uniform random distributions.
 
         Args:
             signal: The signal to sparsify.
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/sparsifier/sequential_sparsifier.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/sparsifier/sequential_sparsifier.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/species.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/species.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     """
 
     def __init__(
         self,
         name: str,
         distribution: distributions.Distribution[float],
         contained_in_output: bool = True,
-        min_value: typing.Optional[float] = None,
-        max_value: typing.Optional[float] = None,
+        min_value: float | None = None,
+        max_value: float | None = None,
     ) -> None:
         """Inits Species with the provided params.
 
         Args:
             name: The name of the variable.
             distribution: A condition determining the value of the parameter
                 at the start.
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/system_model/system_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,20 +88,18 @@
         specieses: list[species.Species],
         kinetic_parameters: dict[
             str, kinetic_parameters_module.KineticParameter[KineticParameterType]
         ],
         deriv: typing.Callable[
             [float, list[float], dict[str, KineticParameterType]], tuple[float, ...]
         ],
-        sparsifier: typing.Optional[abstract_sparsifier.Sparsifier] = None,
-        noiser: typing.Optional[noisers.Noiser] = None,
-        deriv_noiser: typing.Optional[
-            derivative_noiser.DerivNoiser[KineticParameterType]
-        ] = None,
-        timestamps: typing.Optional[distributions.Distribution[float]] = None,
+        sparsifier: abstract_sparsifier.Sparsifier | None = None,
+        noiser: noisers.Noiser | None = None,
+        deriv_noiser: derivative_noiser.DerivNoiser[KineticParameterType] | None = None,
+        timestamps: distributions.Distribution[float] | None = None,
         solver_method: str = "LSODA",
     ):
         """Inits PredictionTask with the provided params.
 
         Args:
             name: The name of the problem.
             specieses: A list of specieses.
@@ -127,17 +125,15 @@
         self.sparsifier = sparsifier or no_sparsifier.NoSparsifier()
         self.noiser = noiser or noisers.NoNoiser()
         self.deriv_noiser = deriv_noiser or derivative_noiser.NoDerivNoiser()
         self.timestamps = timestamps or distributions.Constant(1500.0)
         self.__deriv = deriv
         self.solver_method = solver_method
 
-    def __get_t(
-        self, timestamps: typing.Optional[int] = None
-    ) -> np.typing.NDArray[np.float64]:
+    def __get_t(self, timestamps: int | None = None) -> np.typing.NDArray[np.float64]:
         """Returns an array of timestamps in range `[0, timestamps)`.
 
         Args:
             timestamps(int): The number of timestamps.
                 If None, the number of timestamps is sampled ramdomly.
 
         Returns:
```

### Comparing `simba_ml-1.0.0rc8/simba_ml/simulation/system_model/system_model_interface.py` & `simba_ml-1.0.0rc9/simba_ml/simulation/system_model/system_model_interface.py`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/simba_ml.egg-info/PKG-INFO` & `simba_ml-1.0.0rc9/simba_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simba-ml
-Version: 1.0.0rc8
+Version: 1.0.0rc9
 Summary: Simulation-Based Machine Learning
 Home-page: UNKNOWN
 Author: Maximilian Kleissl, Björn Heyder, Julian Zabbarov, Lukas Drews
 Author-email: maximilian.kleissl@student.hpi.de,bjoern.heyder@student.hpi.de,julian.zabbarov@student.hpi.de,lukas.drews@student.hpi.de
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/DILiS-lab/SimbaML/issues
 Project-URL: Source Code, https://github.com/DILiS-lab/SimbaML
```

### Comparing `simba_ml-1.0.0rc8/simba_ml.egg-info/SOURCES.txt` & `simba_ml-1.0.0rc9/simba_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simba_ml-1.0.0rc8/versioneer.py` & `simba_ml-1.0.0rc9/versioneer.py`

 * *Files identical despite different names*

