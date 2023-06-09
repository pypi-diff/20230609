# Comparing `tmp/a2ml-1.0.92.tar.gz` & `tmp/a2ml-1.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a2ml-1.0.92.tar", last modified: Wed May 24 16:23:01 2023, max compression
+gzip compressed data, was "a2ml-1.0.93.tar", last modified: Fri Jun  9 17:13:38 2023, max compression
```

## Comparing `a2ml-1.0.92.tar` & `a2ml-1.0.93.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.489376 a2ml-1.0.92/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 16:22:56.000000 a2ml-1.0.92/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-24 16:23:01.489376 a2ml-1.0.92/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-24 16:22:56.000000 a2ml-1.0.92/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.469375 a2ml-1.0.92/a2ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.469375 a2ml-1.0.92/a2ml/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/a2ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/a2ml_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/a2ml_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/a2ml_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/a2ml_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/a2ml_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.473375 a2ml-1.0.92/a2ml/api/auger/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/a2ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/experiment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.473375 a2ml-1.0.92/a2ml/api/auger/impl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.473375 a2ml-1.0.92/a2ml/api/auger/impl/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/actual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/cluster_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/endpoint_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/experiment_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/org.py
--rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/pipeline_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/project_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/review_alert.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/review_alert_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/cloud/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.477376 a2ml-1.0.92/a2ml/api/auger/impl/mparts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/mparts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/mparts/actual.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/mparts/delete_actual.py
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/mparts/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/mparts/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/mparts/undeploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/impl/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/auger/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.477376 a2ml-1.0.92/a2ml/api/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/a2ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)    23693 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/azure/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/base_a2ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.477376 a2ml-1.0.92/a2ml/api/google/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/google/a2ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.477376 a2ml-1.0.92/a2ml/api/model_review/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21001 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/model_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    39353 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/model_review.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/probabilistic_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.477376 a2ml-1.0.92/a2ml/api/model_review/scores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/scores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/scores/classification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/model_review/scores/regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.477376 a2ml-1.0.92/a2ml/api/roi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/base_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/roi/var_names_fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.481376 a2ml-1.0.92/a2ml/api/stats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/stats/feature_divergence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.481376 a2ml-1.0.92/a2ml/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/base_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/config_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/crud_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/file_uploader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    15236 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/fsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/local_fsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/provider_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/remote_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/s3_fsclient.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/api/utils/show_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.481376 a2ml-1.0.92/a2ml/cmdl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/cmdl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.485376 a2ml-1.0.92/a2ml/cmdl/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_new.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_server.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/commands/cmd_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.485376 a2ml-1.0.92/a2ml/cmdl/template/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.485376 a2ml-1.0.92/a2ml/cmdl/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/cmdl/utils/test_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.485376 a2ml-1.0.92/a2ml/server/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/server/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/server/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/server/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.485376 a2ml-1.0.92/a2ml/tasks_queue/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/tasks_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/tasks_queue/celery_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/tasks_queue/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/tasks_queue/tasks_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25482 2023-05-24 16:22:56.000000 a2ml-1.0.92/a2ml/tasks_queue/tasks_hub_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.469375 a2ml-1.0.92/a2ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 16:23:01.000000 a2ml-1.0.92/a2ml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-24 16:23:01.489376 a2ml-1.0.92/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-05-24 16:22:56.000000 a2ml-1.0.92/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.485376 a2ml-1.0.92/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/_test_azure_a2ml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/_test_azure_auth_cmdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/_test_google_a2ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/_test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.489376 a2ml-1.0.92/tests/auger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/test_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/auger/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:23:01.489376 a2ml-1.0.92/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/integration/test_auger.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/integration/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/test_auger_auth_cmdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/test_cmdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/test_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/test_new_cmdl.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-24 16:22:56.000000 a2ml-1.0.92/tests/vcr_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.356168 a2ml-1.0.93/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 17:13:32.000000 a2ml-1.0.93/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-09 17:13:38.356168 a2ml-1.0.93/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-09 17:13:32.000000 a2ml-1.0.93/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.344168 a2ml-1.0.93/a2ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.344168 a2ml-1.0.93/a2ml/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22108 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/a2ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/a2ml_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/a2ml_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7759 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/a2ml_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/a2ml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6747 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/a2ml_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.344168 a2ml-1.0.93/a2ml/api/auger/
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/a2ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/experiment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.344168 a2ml-1.0.93/a2ml/api/auger/impl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/auger/impl/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/actual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7669 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/cluster_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9104 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/endpoint_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10026 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/experiment_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6018 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/pipeline_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4302 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/project_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/review_alert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/review_alert_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/cloud/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5273 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/auger/impl/mparts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/mparts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/mparts/actual.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/mparts/delete_actual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/mparts/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12751 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/mparts/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/mparts/undeploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/impl/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/auger/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/a2ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5224 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16584 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23693 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8620 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/azure/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/base_a2ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/google/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/google/a2ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/model_review/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21001 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/model_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39353 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/model_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/probabilistic_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/model_review/scores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/scores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/scores/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/model_review/scores/regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/roi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/base_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7694 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14581 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/roi/var_names_fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.348168 a2ml-1.0.93/a2ml/api/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/stats/feature_divergence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/base_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/config_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6124 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/crud_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25389 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/file_uploader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/fsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2340 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/local_fsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/provider_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/remote_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/s3_fsclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/api/utils/show_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/cmdl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/cmdl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/cmdl/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/commands/cmd_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/cmdl/template/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/cmdl/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/cmdl/utils/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/server/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/server/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/server/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/server/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/a2ml/tasks_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/tasks_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/tasks_queue/celery_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/tasks_queue/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/tasks_queue/tasks_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25482 2023-06-09 17:13:32.000000 a2ml-1.0.93/a2ml/tasks_queue/tasks_hub_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.344168 a2ml-1.0.93/a2ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 17:13:38.000000 a2ml-1.0.93/a2ml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-09 17:13:38.356168 a2ml-1.0.93/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-09 17:13:32.000000 a2ml-1.0.93/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/_test_azure_a2ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/_test_azure_auth_cmdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/_test_google_a2ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/_test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/tests/auger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/test_configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/auger/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:38.352168 a2ml-1.0.93/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/integration/test_auger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/integration/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/test_auger_auth_cmdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/test_cmdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/test_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/test_new_cmdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 17:13:32.000000 a2ml-1.0.93/tests/vcr_helper.py
```

### Comparing `a2ml-1.0.92/LICENSE` & `a2ml-1.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/PKG-INFO` & `a2ml-1.0.93/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2ml
-Version: 1.0.92
+Version: 1.0.93
 Summary: A powerful API to Automate Machine Learning workflows from multiple vendors.
 Home-page: https://a2ml.org
 Author: Auger AI
 Author-email: hello@auger.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://a2ml.org
 Project-URL: Changelog, https://github.com/augerai/a2ml/releases
```

### Comparing `a2ml-1.0.92/README.md` & `a2ml-1.0.93/README.md`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/a2ml.py` & `a2ml-1.0.93/a2ml/api/a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/a2ml_credentials.py` & `a2ml-1.0.93/a2ml/api/a2ml_credentials.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/a2ml_dataset.py` & `a2ml-1.0.93/a2ml/api/a2ml_dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/a2ml_experiment.py` & `a2ml-1.0.93/a2ml/api/a2ml_experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/a2ml_model.py` & `a2ml-1.0.93/a2ml/api/a2ml_model.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/a2ml_project.py` & `a2ml-1.0.93/a2ml/api/a2ml_project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/a2ml.py` & `a2ml-1.0.93/a2ml/api/auger/a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/config.py` & `a2ml-1.0.93/a2ml/api/auger/config.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/credentials.py` & `a2ml-1.0.93/a2ml/api/auger/credentials.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/dataset.py` & `a2ml-1.0.93/a2ml/api/auger/dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/experiment.py` & `a2ml-1.0.93/a2ml/api/auger/experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/actual.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/actual.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/auth.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/auth.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/base.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/base.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/cluster.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/cluster.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/cluster_task.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/cluster_task.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/dataset.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/endpoint.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/endpoint.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/experiment.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/experiment_session.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/experiment_session.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/org.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/org.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/pipeline.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/pipeline.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/pipeline_file.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/pipeline_file.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/prediction.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/prediction.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/project.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/project_file.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/project_file.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/rest_api.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/rest_api.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/cloud/review_alert.py` & `a2ml-1.0.93/a2ml/api/auger/impl/cloud/review_alert.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/dataset.py` & `a2ml-1.0.93/a2ml/api/auger/impl/dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/decorators.py` & `a2ml-1.0.93/a2ml/api/auger/impl/decorators.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/experiment.py` & `a2ml-1.0.93/a2ml/api/auger/impl/experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/model.py` & `a2ml-1.0.93/a2ml/api/auger/impl/model.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/mparts/actual.py` & `a2ml-1.0.93/a2ml/api/auger/impl/mparts/actual.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/mparts/deploy.py` & `a2ml-1.0.93/a2ml/api/auger/impl/mparts/deploy.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/mparts/predict.py` & `a2ml-1.0.93/a2ml/api/auger/impl/mparts/predict.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/impl/mparts/undeploy.py` & `a2ml-1.0.93/a2ml/api/auger/impl/mparts/undeploy.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/model.py` & `a2ml-1.0.93/a2ml/api/auger/model.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/auger/project.py` & `a2ml-1.0.93/a2ml/api/auger/project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/azure/a2ml.py` & `a2ml-1.0.93/a2ml/api/azure/a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/azure/credentials.py` & `a2ml-1.0.93/a2ml/api/azure/credentials.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/azure/dataset.py` & `a2ml-1.0.93/a2ml/api/azure/dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/azure/experiment.py` & `a2ml-1.0.93/a2ml/api/azure/experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/azure/model.py` & `a2ml-1.0.93/a2ml/api/azure/model.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/azure/project.py` & `a2ml-1.0.93/a2ml/api/azure/project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/base_a2ml.py` & `a2ml-1.0.93/a2ml/api/base_a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/google/a2ml.py` & `a2ml-1.0.93/a2ml/api/google/a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/model_review/model_helper.py` & `a2ml-1.0.93/a2ml/api/model_review/model_helper.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/model_review/model_review.py` & `a2ml-1.0.93/a2ml/api/model_review/model_review.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/model_review/scores/classification.py` & `a2ml-1.0.93/a2ml/api/model_review/scores/classification.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/model_review/scores/regression.py` & `a2ml-1.0.93/a2ml/api/model_review/scores/regression.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/base_interpreter.py` & `a2ml-1.0.93/a2ml/api/roi/base_interpreter.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/calculator.py` & `a2ml-1.0.93/a2ml/api/roi/calculator.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/interpreter.py` & `a2ml-1.0.93/a2ml/api/roi/interpreter.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/lexer.py` & `a2ml-1.0.93/a2ml/api/roi/lexer.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/parser.py` & `a2ml-1.0.93/a2ml/api/roi/parser.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/validator.py` & `a2ml-1.0.93/a2ml/api/roi/validator.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/roi/var_names_fetcher.py` & `a2ml-1.0.93/a2ml/api/roi/var_names_fetcher.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/stats/feature_divergence.py` & `a2ml-1.0.93/a2ml/api/stats/feature_divergence.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/__init__.py` & `a2ml-1.0.93/a2ml/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/base_credentials.py` & `a2ml-1.0.93/a2ml/api/utils/base_credentials.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/config.py` & `a2ml-1.0.93/a2ml/api/utils/config.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/config_yaml.py` & `a2ml-1.0.93/a2ml/api/utils/config_yaml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/context.py` & `a2ml-1.0.93/a2ml/api/utils/context.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/crud_runner.py` & `a2ml-1.0.93/a2ml/api/utils/crud_runner.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/dataframe.py` & `a2ml-1.0.93/a2ml/api/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/decorators.py` & `a2ml-1.0.93/a2ml/api/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/file_uploader.py` & `a2ml-1.0.93/a2ml/api/utils/file_uploader.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/formatter.py` & `a2ml-1.0.93/a2ml/api/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/fsclient.py` & `a2ml-1.0.93/a2ml/api/utils/fsclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,20 @@
 def _get_fsclient_bypath(path):
     if is_s3_path(path):
         from .s3_fsclient import S3FSClient
         return S3FSClient()
     else:
         return LocalFSClient()
 
-def get_file_base_name(file_name):
+def get_file_base_name(file_name, last_ext=False):
     if '.' in file_name:
-        separator_index = file_name.index('.')
+        if last_ext:
+            separator_index = file_name.rindex('.')
+        else:
+            separator_index = file_name.index('.')    
         base_name = file_name[:separator_index]
         return base_name
     else:
         return file_name
 
 def get_path_base_name(path):
     file_name = os.path.basename(path)
```

### Comparing `a2ml-1.0.92/a2ml/api/utils/json_utils.py` & `a2ml-1.0.93/a2ml/api/utils/json_utils.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/local_fsclient.py` & `a2ml-1.0.93/a2ml/api/utils/local_fsclient.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/provider_runner.py` & `a2ml-1.0.93/a2ml/api/utils/provider_runner.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/remote_runner.py` & `a2ml-1.0.93/a2ml/api/utils/remote_runner.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/s3_fsclient.py` & `a2ml-1.0.93/a2ml/api/utils/s3_fsclient.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/api/utils/show_result.py` & `a2ml-1.0.93/a2ml/api/utils/show_result.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/cmdl.py` & `a2ml-1.0.93/a2ml/cmdl/cmdl.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_auth.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_auth.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_dataset.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_deploy.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_deploy.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_evaluate.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_evaluate.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_experiment.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_import.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_import.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_model.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_model.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_new.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_new.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_predict.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_predict.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_project.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_server.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_server.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/cmdl/commands/cmd_worker.py` & `a2ml-1.0.93/a2ml/cmdl/commands/cmd_worker.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/server/config.py` & `a2ml-1.0.93/a2ml/server/config.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/server/notification.py` & `a2ml-1.0.93/a2ml/server/notification.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/server/server.py` & `a2ml-1.0.93/a2ml/server/server.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/tasks_queue/celery_app.py` & `a2ml-1.0.93/a2ml/tasks_queue/celery_app.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/tasks_queue/tasks_api.py` & `a2ml-1.0.93/a2ml/tasks_queue/tasks_api.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml/tasks_queue/tasks_hub_api.py` & `a2ml-1.0.93/a2ml/tasks_queue/tasks_hub_api.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml.egg-info/PKG-INFO` & `a2ml-1.0.93/a2ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a2ml
-Version: 1.0.92
+Version: 1.0.93
 Summary: A powerful API to Automate Machine Learning workflows from multiple vendors.
 Home-page: https://a2ml.org
 Author: Auger AI
 Author-email: hello@auger.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://a2ml.org
 Project-URL: Changelog, https://github.com/augerai/a2ml/releases
```

### Comparing `a2ml-1.0.92/a2ml.egg-info/SOURCES.txt` & `a2ml-1.0.93/a2ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/a2ml.egg-info/requires.txt` & `a2ml-1.0.93/a2ml.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -44,21 +44,21 @@
 [docs]
 sphinx
 
 [google]
 google-cloud-automl
 
 [predict]
-auger.ai.predict[all]==1.0.110
+auger.ai.predict[all]==1.1.001
 
 [predict_no_cat_lgbm]
-auger.ai.predict[no_cat_lgbm]==1.0.110
+auger.ai.predict[no_cat_lgbm]==1.1.001
 
 [predict_no_lgbm]
-auger.ai.predict[no_cat_lgbm]==1.0.110
+auger.ai.predict[no_cat_lgbm]==1.1.001
 catboost
 
 [server]
 aioredis
 celery==5.2.7
 fastapi==0.85
 gevent
```

### Comparing `a2ml-1.0.92/setup.cfg` & `a2ml-1.0.93/setup.cfg`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/setup.py` & `a2ml-1.0.93/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -82,21 +82,21 @@
         #this needs to move to setup.azure.py and do not include default
         'azureml-sdk[automl]==1.29.0'
     ],
     'google': [
         'google-cloud-automl'
     ],
     'predict': [
-        'auger.ai.predict[all]==1.0.110'
+        'auger.ai.predict[all]==1.1.001'
     ],
     'predict_no_cat_lgbm': [
-        'auger.ai.predict[no_cat_lgbm]==1.0.110'
+        'auger.ai.predict[no_cat_lgbm]==1.1.001'
     ],
     'predict_no_lgbm': [
-        'auger.ai.predict[no_cat_lgbm]==1.0.110',
+        'auger.ai.predict[no_cat_lgbm]==1.1.001',
         'catboost'
     ]    
 }
 
 # Meta dependency groups.
 all_deps = []
 for group_name in extras:
```

### Comparing `a2ml-1.0.92/tests/_test_azure_a2ml.py` & `a2ml-1.0.93/tests/_test_azure_a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/_test_azure_auth_cmdl.py` & `a2ml-1.0.93/tests/_test_azure_auth_cmdl.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/_test_google_a2ml.py` & `a2ml-1.0.93/tests/_test_google_a2ml.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/_test_local.py` & `a2ml-1.0.93/tests/_test_local.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/conftest.py` & `a2ml-1.0.93/tests/auger/conftest.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/test_configs.py` & `a2ml-1.0.93/tests/auger/test_configs.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/test_dataset.py` & `a2ml-1.0.93/tests/auger/test_dataset.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/test_experiment.py` & `a2ml-1.0.93/tests/auger/test_experiment.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/test_model.py` & `a2ml-1.0.93/tests/auger/test_model.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/test_project.py` & `a2ml-1.0.93/tests/auger/test_project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/auger/utils.py` & `a2ml-1.0.93/tests/auger/utils.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/conftest.py` & `a2ml-1.0.93/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/integration/conftest.py` & `a2ml-1.0.93/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/integration/test_auger.py` & `a2ml-1.0.93/tests/integration/test_auger.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/integration/test_project.py` & `a2ml-1.0.93/tests/integration/test_project.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/test_auger_auth_cmdl.py` & `a2ml-1.0.93/tests/test_auger_auth_cmdl.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/test_cmdl.py` & `a2ml-1.0.93/tests/test_cmdl.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/test_facade.py` & `a2ml-1.0.93/tests/test_facade.py`

 * *Files identical despite different names*

### Comparing `a2ml-1.0.92/tests/test_new_cmdl.py` & `a2ml-1.0.93/tests/test_new_cmdl.py`

 * *Files identical despite different names*

