# Comparing `tmp/mlfoundry-0.8.1.tar.gz` & `tmp/mlfoundry-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlfoundry-0.8.1.tar", max compression
+gzip compressed data, was "mlfoundry-0.9.0rc1.tar", max compression
```

## Comparing `mlfoundry-0.8.1.tar` & `mlfoundry-0.9.0rc1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     3158 2023-05-31 16:00:16.854792 mlfoundry-0.8.1/README.md
--rw-r--r--   0        0        0      991 2023-05-31 16:00:16.866792 mlfoundry-0.8.1/mlfoundry/__init__.py
--rw-r--r--   0        0        0     1211 2023-05-31 16:00:16.866792 mlfoundry-0.8.1/mlfoundry/__main__.py
--rw-r--r--   0        0        0     3713 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/amplitude.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/artifact/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/artifact/truefoundry_artifact_repo.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/__init__.py
--rw-r--r--   0        0        0      287 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/events.py
--rw-r--r--   0        0        0     3032 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/interface.py
--rw-r--r--   0        0        0     4016 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/sender.py
--rw-r--r--   0        0        0     8756 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/system_metrics.py
--rw-r--r--   0        0        0     4028 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/background/utils.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/__init__.py
--rw-r--r--   0        0        0      918 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/cli_interface.py
--rw-r--r--   0        0        0      100 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0      731 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/commands/download.py
--rw-r--r--   0        0        0      739 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/cli/commands/login.py
--rw-r--r--   0        0        0     2724 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/constants.py
--rw-r--r--   0        0        0      103 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/__init__.py
--rw-r--r--   0        0        0     7854 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/dataset.py
--rw-r--r--   0        0        0     2255 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/schema.py
--rw-r--r--   0        0        0    13138 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/serde.py
--rw-r--r--   0        0        0     2028 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/serde_utils.py
--rw-r--r--   0        0        0     2078 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/stats.py
--rw-r--r--   0        0        0     1903 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/types.py
--rw-r--r--   0        0        0     2588 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/validation.py
--rw-r--r--   0        0        0       69 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/whylogs_types/__init__.py
--rw-r--r--   0        0        0     4025 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/dataset/whylogs_types/summary.py
--rw-r--r--   0        0        0     1392 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/enums.py
--rw-r--r--   0        0        0      325 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/env_vars.py
--rw-r--r--   0        0        0      365 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/exceptions.py
--rw-r--r--   0        0        0     2037 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/__init__.py
--rw-r--r--   0        0        0      301 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/base_registry.py
--rw-r--r--   0        0        0      718 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/fastai_registry.py
--rw-r--r--   0        0        0      892 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/gluon_registry.py
--rw-r--r--   0        0        0      700 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/h2o_registry.py
--rw-r--r--   0        0        0      712 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/keras_registry.py
--rw-r--r--   0        0        0      730 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/lightgbm_registry.py
--rw-r--r--   0        0        0      706 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/onnx_registry.py
--rw-r--r--   0        0        0      775 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/paddle_registry.py
--rw-r--r--   0        0        0      744 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/pytorch_registry.py
--rw-r--r--   0        0        0      724 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/sklearn_registry.py
--rw-r--r--   0        0        0      712 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/spacy_registry.py
--rw-r--r--   0        0        0      748 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/statsmodel_registry.py
--rw-r--r--   0        0        0     3077 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/tensorflow_registry.py
--rw-r--r--   0        0        0      774 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/transformers_registry.py
--rw-r--r--   0        0        0      724 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/frameworks/xgboost_registry.py
--rw-r--r--   0        0        0     2349 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/git_info.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/integrations/__init__.py
--rw-r--r--   0        0        0    15423 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/integrations/lightning.py
--rw-r--r--   0        0        0    22410 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/integrations/transformers.py
--rw-r--r--   0        0        0     1785 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/internal_namespace.py
--rw-r--r--   0        0        0      571 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/__init__.py
--rw-r--r--   0        0        0     7978 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/artifact.py
--rw-r--r--   0        0        0     1019 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/constants.py
--rw-r--r--   0        0        0     3072 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/general_artifact.py
--rw-r--r--   0        0        0    15275 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/model.py
--rw-r--r--   0        0        0     5983 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/artifacts/utils.py
--rw-r--r--   0        0        0     1281 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/dataset_artifact.py
--rw-r--r--   0        0        0      222 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/dataset_schema.py
--rw-r--r--   0        0        0      318 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/dataset_stats.py
--rw-r--r--   0        0        0       50 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/__init__.py
--rw-r--r--   0        0        0      255 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/constants.py
--rw-r--r--   0        0        0    11446 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/image.py
--rw-r--r--   0        0        0     2767 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/image_normalizer.py
--rw-r--r--   0        0        0     1566 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/image/types.py
--rw-r--r--   0        0        0      271 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/model_artifact.py
--rw-r--r--   0        0        0     7125 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/plot.py
--rw-r--r--   0        0        0     2486 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/pydantic_base.py
--rw-r--r--   0        0        0     1332 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/log_types/utils.py
--rw-r--r--   0        0        0      453 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/logger.py
--rw-r--r--   0        0        0     9286 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/login.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/__init__.py
--rw-r--r--   0        0        0     2080 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/base_metrics.py
--rw-r--r--   0        0        0     6852 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/binary_classification_metrics.py
--rw-r--r--   0        0        0     6736 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     4419 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/regression_metrics.py
--rw-r--r--   0        0        0     3976 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v1/timeseries_metrics.py
--rw-r--r--   0        0        0     1026 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/__init__.py
--rw-r--r--   0        0        0     1898 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/base_metrics.py
--rw-r--r--   0        0        0      566 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/custom_metric_types.py
--rw-r--r--   0        0        0     6192 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
--rw-r--r--   0        0        0     2718 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/regression_metrics.py
--rw-r--r--   0        0        0     2251 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/timeseries_metrics.py
--rw-r--r--   0        0        0      295 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/metrics/v2/utils.py
--rw-r--r--   0        0        0    44772 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/mlfoundry_api.py
--rw-r--r--   0        0        0    46176 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/mlfoundry_run.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/__init__.py
--rw-r--r--   0        0        0     1994 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/entities.py
--rw-r--r--   0        0        0       63 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/__init__.py
--rw-r--r--   0        0        0     6630 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/client.py
--rw-r--r--   0        0        0      169 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/constants.py
--rw-r--r--   0        0        0      336 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/__init__.py
--rw-r--r--   0        0        0     1351 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/dto.py
--rw-r--r--   0        0        0     6529 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
--rw-r--r--   0        0        0     2178 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/monitoring/store/worker.py
--rw-r--r--   0        0        0     4304 2023-05-31 16:00:16.870792 mlfoundry-0.8.1/mlfoundry/run_utils.py
--rw-r--r--   0        0        0      492 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/schema.py
--rw-r--r--   0        0        0    10031 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/session.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/__init__.py
--rw-r--r--   0        0        0     2766 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/auth_service.py
--rw-r--r--   0        0        0     2629 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/entities.py
--rw-r--r--   0        0        0     1175 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/servicefoundry_service.py
--rw-r--r--   0        0        0     4308 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/tracking/truefoundry_rest_store.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/vendor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/vendor/pynvml/__init__.py
--rw-r--r--   0        0        0    56147 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/vendor/pynvml/pynvml.py
--rw-r--r--   0        0        0      253 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/version.py
--rw-r--r--   0        0        0        0 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/webapp/__init__.py
--rw-r--r--   0        0        0       38 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/webapp/inputs.py
--rw-r--r--   0        0        0       39 2023-05-31 16:00:16.874792 mlfoundry-0.8.1/mlfoundry/webapp/outputs.py
--rw-r--r--   0        0        0     3548 2023-05-31 16:00:27.847129 mlfoundry-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     4925 1970-01-01 00:00:00.000000 mlfoundry-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     3158 2023-06-09 11:01:51.323648 mlfoundry-0.9.0rc1/README.md
+-rw-r--r--   0        0        0      991 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/__main__.py
+-rw-r--r--   0        0        0     3713 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/amplitude.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/artifact/__init__.py
+-rw-r--r--   0        0        0    20613 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/artifact/truefoundry_artifact_repo.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/__init__.py
+-rw-r--r--   0        0        0      287 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/events.py
+-rw-r--r--   0        0        0     3032 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/interface.py
+-rw-r--r--   0        0        0     4016 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/sender.py
+-rw-r--r--   0        0        0     8756 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/system_metrics.py
+-rw-r--r--   0        0        0     4028 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/background/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/__init__.py
+-rw-r--r--   0        0        0      918 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/cli_interface.py
+-rw-r--r--   0        0        0      100 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0      731 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/download.py
+-rw-r--r--   0        0        0      739 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/cli/commands/login.py
+-rw-r--r--   0        0        0     2724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/constants.py
+-rw-r--r--   0        0        0      103 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/__init__.py
+-rw-r--r--   0        0        0     7854 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/dataset.py
+-rw-r--r--   0        0        0     2255 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/schema.py
+-rw-r--r--   0        0        0    13138 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/serde.py
+-rw-r--r--   0        0        0     2028 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/serde_utils.py
+-rw-r--r--   0        0        0     2078 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/stats.py
+-rw-r--r--   0        0        0     1903 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/types.py
+-rw-r--r--   0        0        0     2588 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/validation.py
+-rw-r--r--   0        0        0       69 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/__init__.py
+-rw-r--r--   0        0        0     4025 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/summary.py
+-rw-r--r--   0        0        0     1392 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/enums.py
+-rw-r--r--   0        0        0      383 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/env_vars.py
+-rw-r--r--   0        0        0      365 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/exceptions.py
+-rw-r--r--   0        0        0     2037 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/__init__.py
+-rw-r--r--   0        0        0      301 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/base_registry.py
+-rw-r--r--   0        0        0      718 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/fastai_registry.py
+-rw-r--r--   0        0        0      892 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/gluon_registry.py
+-rw-r--r--   0        0        0      700 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/h2o_registry.py
+-rw-r--r--   0        0        0      712 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/keras_registry.py
+-rw-r--r--   0        0        0      730 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/lightgbm_registry.py
+-rw-r--r--   0        0        0      706 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/onnx_registry.py
+-rw-r--r--   0        0        0      775 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/paddle_registry.py
+-rw-r--r--   0        0        0      744 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/pytorch_registry.py
+-rw-r--r--   0        0        0      724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/sklearn_registry.py
+-rw-r--r--   0        0        0      712 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/spacy_registry.py
+-rw-r--r--   0        0        0      748 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/statsmodel_registry.py
+-rw-r--r--   0        0        0     3077 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/tensorflow_registry.py
+-rw-r--r--   0        0        0      774 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/transformers_registry.py
+-rw-r--r--   0        0        0      724 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/frameworks/xgboost_registry.py
+-rw-r--r--   0        0        0     2349 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/git_info.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/__init__.py
+-rw-r--r--   0        0        0    15423 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/lightning.py
+-rw-r--r--   0        0        0    22410 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/integrations/transformers.py
+-rw-r--r--   0        0        0     1785 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/internal_namespace.py
+-rw-r--r--   0        0        0      571 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/__init__.py
+-rw-r--r--   0        0        0     7978 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/artifact.py
+-rw-r--r--   0        0        0     1019 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/constants.py
+-rw-r--r--   0        0        0     3072 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/general_artifact.py
+-rw-r--r--   0        0        0    15275 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/model.py
+-rw-r--r--   0        0        0     5983 2023-06-09 11:01:51.347648 mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/utils.py
+-rw-r--r--   0        0        0     1281 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_artifact.py
+-rw-r--r--   0        0        0      222 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_schema.py
+-rw-r--r--   0        0        0      318 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_stats.py
+-rw-r--r--   0        0        0       50 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/__init__.py
+-rw-r--r--   0        0        0      255 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/constants.py
+-rw-r--r--   0        0        0    11446 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image.py
+-rw-r--r--   0        0        0     2767 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image_normalizer.py
+-rw-r--r--   0        0        0     1566 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/image/types.py
+-rw-r--r--   0        0        0      271 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/model_artifact.py
+-rw-r--r--   0        0        0     7125 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/plot.py
+-rw-r--r--   0        0        0     2486 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/pydantic_base.py
+-rw-r--r--   0        0        0     1332 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/log_types/utils.py
+-rw-r--r--   0        0        0      453 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/logger.py
+-rw-r--r--   0        0        0     9286 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/login.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/__init__.py
+-rw-r--r--   0        0        0     1065 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/__init__.py
+-rw-r--r--   0        0        0     2080 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/base_metrics.py
+-rw-r--r--   0        0        0     6852 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py
+-rw-r--r--   0        0        0     6736 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     4419 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/regression_metrics.py
+-rw-r--r--   0        0        0     3976 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py
+-rw-r--r--   0        0        0     1026 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/__init__.py
+-rw-r--r--   0        0        0     1898 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/base_metrics.py
+-rw-r--r--   0        0        0      566 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/custom_metric_types.py
+-rw-r--r--   0        0        0     6192 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py
+-rw-r--r--   0        0        0     2718 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/regression_metrics.py
+-rw-r--r--   0        0        0     2251 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py
+-rw-r--r--   0        0        0      295 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/utils.py
+-rw-r--r--   0        0        0    44772 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_api.py
+-rw-r--r--   0        0        0    46176 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_run.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/__init__.py
+-rw-r--r--   0        0        0     1994 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/entities.py
+-rw-r--r--   0        0        0       63 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/__init__.py
+-rw-r--r--   0        0        0     6630 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/client.py
+-rw-r--r--   0        0        0      169 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/constants.py
+-rw-r--r--   0        0        0      336 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/__init__.py
+-rw-r--r--   0        0        0     1351 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/dto.py
+-rw-r--r--   0        0        0     6529 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py
+-rw-r--r--   0        0        0     2178 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/worker.py
+-rw-r--r--   0        0        0     4304 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/run_utils.py
+-rw-r--r--   0        0        0      492 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/schema.py
+-rw-r--r--   0        0        0    10031 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/session.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/__init__.py
+-rw-r--r--   0        0        0     2766 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/auth_service.py
+-rw-r--r--   0        0        0     2629 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/entities.py
+-rw-r--r--   0        0        0     1175 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/servicefoundry_service.py
+-rw-r--r--   0        0        0     4308 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/tracking/truefoundry_rest_store.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/__init__.py
+-rw-r--r--   0        0        0    56147 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/pynvml.py
+-rw-r--r--   0        0        0      253 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/version.py
+-rw-r--r--   0        0        0        0 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/__init__.py
+-rw-r--r--   0        0        0       38 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/inputs.py
+-rw-r--r--   0        0        0       39 2023-06-09 11:01:51.351648 mlfoundry-0.9.0rc1/mlfoundry/webapp/outputs.py
+-rw-r--r--   0        0        0     3551 2023-06-09 11:02:10.840067 mlfoundry-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4928 1970-01-01 00:00:00.000000 mlfoundry-0.9.0rc1/PKG-INFO
```

### Comparing `mlfoundry-0.8.1/README.md` & `mlfoundry-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/__main__.py` & `mlfoundry-0.9.0rc1/mlfoundry/__main__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/amplitude.py` & `mlfoundry-0.9.0rc1/mlfoundry/amplitude.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/background/interface.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/background/sender.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/sender.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/background/system_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/system_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/background/utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/background/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/cli/cli_interface.py` & `mlfoundry-0.9.0rc1/mlfoundry/cli/cli_interface.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/cli/commands/download.py` & `mlfoundry-0.9.0rc1/mlfoundry/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/cli/commands/login.py` & `mlfoundry-0.9.0rc1/mlfoundry/cli/commands/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/constants.py` & `mlfoundry-0.9.0rc1/mlfoundry/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/dataset.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/schema.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/schema.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/serde.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/serde.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/serde_utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/serde_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/stats.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/stats.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/types.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/validation.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/validation.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/dataset/whylogs_types/summary.py` & `mlfoundry-0.9.0rc1/mlfoundry/dataset/whylogs_types/summary.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/enums.py` & `mlfoundry-0.9.0rc1/mlfoundry/enums.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/fastai_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/fastai_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/gluon_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/gluon_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/h2o_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/h2o_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/keras_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/keras_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/lightgbm_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/lightgbm_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/onnx_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/onnx_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/paddle_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/paddle_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/pytorch_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/pytorch_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/sklearn_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/sklearn_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/spacy_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/spacy_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/statsmodel_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/statsmodel_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/tensorflow_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/tensorflow_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/transformers_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/transformers_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/frameworks/xgboost_registry.py` & `mlfoundry-0.9.0rc1/mlfoundry/frameworks/xgboost_registry.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/git_info.py` & `mlfoundry-0.9.0rc1/mlfoundry/git_info.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/integrations/lightning.py` & `mlfoundry-0.9.0rc1/mlfoundry/integrations/lightning.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/integrations/transformers.py` & `mlfoundry-0.9.0rc1/mlfoundry/integrations/transformers.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/internal_namespace.py` & `mlfoundry-0.9.0rc1/mlfoundry/internal_namespace.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/artifact.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/constants.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/constants.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/general_artifact.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/general_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/model.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/model.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/artifacts/utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/artifacts/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/dataset_artifact.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/dataset_artifact.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/image/image.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/image/image_normalizer.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/image_normalizer.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/image/types.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/image/types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/plot.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/plot.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/pydantic_base.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/pydantic_base.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/log_types/utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/log_types/utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/login.py` & `mlfoundry-0.9.0rc1/mlfoundry/login.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v1/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v1/base_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v1/binary_classification_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/binary_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v1/multiclass_classification_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v1/regression_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v1/timeseries_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v1/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v2/__init__.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v2/base_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/base_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v2/custom_metric_types.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/custom_metric_types.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v2/multiclass_classification_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/multiclass_classification_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v2/regression_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/metrics/v2/timeseries_metrics.py` & `mlfoundry-0.9.0rc1/mlfoundry/metrics/v2/timeseries_metrics.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/mlfoundry_api.py` & `mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_api.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/mlfoundry_run.py` & `mlfoundry-0.9.0rc1/mlfoundry/mlfoundry_run.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/monitoring/entities.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/monitoring/store/client.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/client.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/dto.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/dto.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/repositories/rest_monitoring_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/monitoring/store/worker.py` & `mlfoundry-0.9.0rc1/mlfoundry/monitoring/store/worker.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/run_utils.py` & `mlfoundry-0.9.0rc1/mlfoundry/run_utils.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/session.py` & `mlfoundry-0.9.0rc1/mlfoundry/session.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/tracking/auth_service.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/auth_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/tracking/entities.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/entities.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/tracking/servicefoundry_service.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/servicefoundry_service.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/tracking/truefoundry_rest_store.py` & `mlfoundry-0.9.0rc1/mlfoundry/tracking/truefoundry_rest_store.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/mlfoundry/vendor/pynvml/pynvml.py` & `mlfoundry-0.9.0rc1/mlfoundry/vendor/pynvml/pynvml.py`

 * *Files identical despite different names*

### Comparing `mlfoundry-0.8.1/pyproject.toml` & `mlfoundry-0.9.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlfoundry"
-version = "0.8.1" # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.0rc1" # do not change, auto-generated by poetry-dynamic-versioning
 description = "Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/truefoundry/mlfoundry"
 repository = "https://github.com/truefoundry/mlfoundry"
 readme = "README.md"
 packages = [
     { include = "mlfoundry" },
@@ -31,15 +31,15 @@
 pydantic = ">=1.8.2,<2.0.0"
 scikit-learn = ">=0.24.2,<2.0.0"
 scipy = [
     # This is split into two because poetry will select a version which has no wheel on python >= 3.10 :/
     { version = ">=1.5.4,<2.0.0", python = "<3.10" },
     { version = ">=1.8.0,<2.0.0", python = ">=3.10" },
 ]
-tfy-mlflow-client = "0.0.31"
+tfy-mlflow-client = "0.0.32"
 # Check and try to eliminate libs below this comment
 boto3 = ">=1.14.1,<2.0.0"
 fastparquet = ">=0.8.0,<=2022.12.0"
 importlib-metadata = ">=4.11.3,<5.0.0"
 packaging = ">=20.0,<24.0"
 pyarrow = ">=5.0.0,<11.0.0"
 whylogs = [
```

### Comparing `mlfoundry-0.8.1/PKG-INFO` & `mlfoundry-0.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlfoundry
-Version: 0.8.1
+Version: 0.9.0rc1
 Summary: Truefoundry's Experiment Tracking, Model Registry and Model Monitoring Library
 Home-page: https://github.com/truefoundry/mlfoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -27,15 +27,15 @@
 Requires-Dist: protobuf (>=3.19.0,<3.21.0)
 Requires-Dist: psutil (>=5.9.0,<6.0.0)
 Requires-Dist: pyarrow (>=5.0.0,<11.0.0)
 Requires-Dist: pydantic (>=1.8.2,<2.0.0)
 Requires-Dist: scikit-learn (>=0.24.2,<2.0.0)
 Requires-Dist: scipy (>=1.5.4,<2.0.0) ; python_version < "3.10"
 Requires-Dist: scipy (>=1.8.0,<2.0.0) ; python_version >= "3.10"
-Requires-Dist: tfy-mlflow-client (==0.0.31)
+Requires-Dist: tfy-mlflow-client (==0.0.32)
 Requires-Dist: whylogs (>=0.6.15,<1.0.0) ; python_version < "3.10"
 Requires-Dist: whylogs (>=1.0.0,<2.0.0) ; python_version >= "3.10"
 Project-URL: Repository, https://github.com/truefoundry/mlfoundry
 Description-Content-Type: text/markdown
 
 # MlFoundry
```

