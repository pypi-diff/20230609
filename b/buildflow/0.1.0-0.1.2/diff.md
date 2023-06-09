# Comparing `tmp/buildflow-0.1.0.tar.gz` & `tmp/buildflow-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildflow-0.1.0.tar", last modified: Wed Jun  7 20:41:11 2023, max compression
+gzip compressed data, was "buildflow-0.1.2.tar", last modified: Fri Jun  9 17:50:50 2023, max compression
```

## Comparing `buildflow-0.1.0.tar` & `buildflow-0.1.2.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-06-07 20:41:00.000000 buildflow-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-07 20:41:11.332065 buildflow-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-06-07 20:41:00.000000 buildflow-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.312064 buildflow-0.1.0/buildflow/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/api/
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/depends.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/infra.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/node.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/options.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/api/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/core/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.316065 buildflow-0.1.0/buildflow/core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/grid/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/grid/grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/infra/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/infra/actors/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/actors/pulumi_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2314 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/actors/setup_infra.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/infra/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/node/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/node/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8642 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/node/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/processor/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.320065 buildflow-0.1.0/buildflow/core/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/core/runtime/actors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/process_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    10263 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/pull_process_push.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/pull_process_push_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/actors/runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/autoscale.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/autoscale_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/core/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/io/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/io/depends/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/depends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/depends/depends.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.324065 buildflow-0.1.0/buildflow/io/providers/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/file_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/file_provider_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3280 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/bigquery_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9812 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcp_pub_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcp_pub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/gcp/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/utils/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/gcp/utils/setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/pulsing_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/pulsing_provider_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.328065 buildflow-0.1.0/buildflow/io/providers/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/providers/schemas/converters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/io/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/buildflow/migration/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/migration/beam_migrator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/buildflow/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/samples/csv_bigquery_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/samples/pubsub_walkthrough.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-07 20:41:00.000000 buildflow-0.1.0/buildflow/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.312064 buildflow-0.1.0/buildflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-07 20:41:11.000000 buildflow-0.1.0/buildflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.312064 buildflow-0.1.0/integration_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:41:11.332065 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 20:41:00.000000 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-07 20:41:00.000000 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_publish.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-07 20:41:00.000000 buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-07 20:41:00.000000 buildflow-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:41:11.332065 buildflow-0.1.0/setup.cfg
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.406174 buildflow-0.1.2/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    10480 2023-05-16 13:09:45.000000 buildflow-0.1.2/LICENSE
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3323 2023-06-09 17:50:50.406174 buildflow-0.1.2/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2703 2023-06-09 17:31:00.000000 buildflow-0.1.2/README.md
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       72 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/__init__.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/api/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      555 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      402 2023-05-25 01:31:40.000000 buildflow-0.1.2/buildflow/api/depends.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      733 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/grid.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      428 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/infra.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      610 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/infrastructure.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      531 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/io.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1653 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/node.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      792 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/options.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      993 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/processor.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1737 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/api/runtime.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/cli/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-05-25 01:31:40.000000 buildflow-0.1.2/buildflow/cli/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4252 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/cli/main.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      998 2023-05-25 01:31:40.000000 buildflow-0.1.2/buildflow/cli/utils.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      298 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/conftest.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/core/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      164 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/__init__.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/core/exceptions/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       39 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/exceptions/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      906 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/exceptions/exceptions.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/core/grid/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       35 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/grid/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1268 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/grid/grid.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/core/infra/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      163 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/infra/__init__.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow/core/infra/actors/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       99 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/infra/actors/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     7257 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/infra/actors/pulumi_infra.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2314 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/infra/actors/setup_infra.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      893 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/infra/config.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/core/node/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/node/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1444 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/node/_utils.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     8736 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/node/node.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/core/processor/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       35 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/processor/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      547 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/processor/base.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/core/runtime/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      208 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/__init__.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/core/runtime/actors/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/actors/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      161 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/actors/conftest.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     8631 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/actors/process_pool.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    10265 2023-06-09 17:31:00.000000 buildflow-0.1.2/buildflow/core/runtime/actors/pull_process_push.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4215 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/actors/pull_process_push_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     6186 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/actors/runtime.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1560 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/actors/runtime_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4812 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/autoscale.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    12903 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/autoscale_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2524 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/core/runtime/config.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      149 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/env.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/io/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       85 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/__init__.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/io/depends/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       74 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/depends/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      755 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/depends/depends.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/io/providers/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       73 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/__init__.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/io/providers/aws/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       15 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/aws/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3932 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/base.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2441 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/file_provider.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1802 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/file_provider_test.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/io/providers/gcp/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       57 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3280 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/bigquery.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     5231 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/bigquery_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     9812 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/gcp_pub_sub.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)    10405 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/gcp_pub_sub_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     6537 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/gcs_file_stream.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2498 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/gcs_file_stream_test.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.402174 buildflow-0.1.2/buildflow/io/providers/gcp/utils/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/utils/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2707 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/utils/clients.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3476 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/gcp/utils/setup_utils.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1408 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/pulsing_provider.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      770 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/pulsing_provider_test.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.406174 buildflow-0.1.2/buildflow/io/providers/schemas/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/schemas/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3093 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/schemas/bigquery_schemas.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4664 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/providers/schemas/bigquery_schemas_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     4213 2023-06-09 17:31:00.000000 buildflow-0.1.2/buildflow/io/providers/schemas/converters.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     5454 2023-06-09 17:31:00.000000 buildflow-0.1.2/buildflow/io/providers/schemas/converters_test.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3237 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/io/registry.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.406174 buildflow-0.1.2/buildflow/migration/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      197 2023-03-24 16:57:27.000000 buildflow-0.1.2/buildflow/migration/beam_migrator.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.406174 buildflow-0.1.2/buildflow/samples/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        0 2023-03-24 16:57:27.000000 buildflow-0.1.2/buildflow/samples/__init__.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2945 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/samples/csv_bigquery_walkthrough.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1698 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/samples/pubsub_walkthrough.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2360 2023-06-08 12:52:11.000000 buildflow-0.1.2/buildflow/utils.py
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/buildflow.egg-info/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3323 2023-06-09 17:50:50.000000 buildflow-0.1.2/buildflow.egg-info/PKG-INFO
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     3013 2023-06-09 17:50:50.000000 buildflow-0.1.2/buildflow.egg-info/SOURCES.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)        1 2023-06-09 17:50:50.000000 buildflow-0.1.2/buildflow.egg-info/dependency_links.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       54 2023-06-09 17:50:50.000000 buildflow-0.1.2/buildflow.egg-info/entry_points.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)      439 2023-06-09 17:50:50.000000 buildflow-0.1.2/buildflow.egg-info/requires.txt
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       39 2023-06-09 17:50:50.000000 buildflow-0.1.2/buildflow.egg-info/top_level.txt
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.398174 buildflow-0.1.2/integration_tests/
+drwxrwxr-x   0 caleb     (1000) caleb     (1000)        0 2023-06-09 17:50:50.406174 buildflow-0.1.2/integration_tests/pubsub_to_pubsub/
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1105 2023-06-08 12:52:11.000000 buildflow-0.1.2/integration_tests/pubsub_to_pubsub/pubsub_main.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1517 2023-06-08 12:52:11.000000 buildflow-0.1.2/integration_tests/pubsub_to_pubsub/pubsub_publish.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     1003 2023-06-08 12:52:11.000000 buildflow-0.1.2/integration_tests/pubsub_to_pubsub/pubsub_validation.py
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)     2308 2023-06-09 17:50:32.000000 buildflow-0.1.2/pyproject.toml
+-rw-rw-r--   0 caleb     (1000) caleb     (1000)       38 2023-06-09 17:50:50.406174 buildflow-0.1.2/setup.cfg
```

### Comparing `buildflow-0.1.0/LICENSE` & `buildflow-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/PKG-INFO` & `buildflow-0.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,63 @@
 Metadata-Version: 2.1
 Name: buildflow
-Version: 0.1.0
+Version: 0.1.2
 Summary: buildflow is a unified **batch** and **streaming** framework that turns any python function into a scalable data pipeline that can read from our supported IO resources.
 Author-email: Caleb Van Dyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# BuildFlow
+# ⚒️ BuildFlow
 
 ![CI](https://github.com/launchflow/buildflow/actions/workflows/python_ci.yaml/badge.svg)
 ![GCP Tests](https://github.com/launchflow/buildflow/actions/workflows/gcp_integration.yaml/badge.svg)
+[![Python version](https://badge.fury.io/py/buildflow.svg)](https://pypi.org/project/buildflow)
+[![codecov](https://codecov.io/gh/launchflow/buildflow/branch/main/graph/badge.svg?token=AO0TP8XG7X)](https://codecov.io/gh/launchflow/buildflow)
 [![Discord Shield](https://discordapp.com/api/guilds/1082821064180117575/widget.png?style=shield)](https://discordapp.com/invite/wz7fjHyrCA)
 
-**BuildFlow**, is an open source framework that lets you build a data pipeline by simply attaching a decorator to a Python function. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. No configuration outside of the code is required.
 
-Key Features:
+## Overview
+**BuildFlow**, is an open source framework for building large scale systems using Python. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. **No configuration outside of the code is required**.
 
-- Unified **batch** and **streaming** [Processor API](https://www.buildflow.dev/docs/processors/overview)
-- Production-grade [IO connectors](https://www.buildflow.dev/docs/io-connectors/overview) for popular cloud services & storage systems
-- IO templates for common data pipelines (e.g. [file upload notifications](https://www.buildflow.dev/docs/io-connectors/gcs_notifications))
-- Automatic [resource creation / management](https://www.buildflow.dev/docs/resource-creation) for popular cloud resources
-- [Schema validation](https://www.buildflow.dev/docs/schema-validation) powered by Python dataclasses and type hints
-- Automatic parallelism powered by [Ray](https://ray.io)
+Key Features (all provided out-of-the-box):
 
-## Quick Links
-
-- **Docs**: https://www.buildflow.dev/docs
-- **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
-- **Discord**: https://discordapp.com/invite/wz7fjHyrCA
-
-## Quickstart
+- Automatic [resource creation / management](https://www.buildflow.dev/docs/features/resource-creation) (Infrastructure as Code) powered by [Pulumi](https://github.com/pulumi/pulumi)
+- Automatic [parallelism & concurrency](https://www.buildflow.dev/docs/features/parallelism) powered by [Ray](https://github.com/ray-project/ray)
+- [Dynamic autoscaling](https://www.buildflow.dev/docs/features/autoscaling): scale up during high traffic / reduce costs during low traffic
+- [Schema validation](https://www.buildflow.dev/docs/features/schema-validation) powered by Python dataclasses and type hints
 
-### Install
+## Installation
 
 ```bash
 pip install buildflow
 ```
 
-### Example Usage
+### Extra Dependencies
 
-```python
-# Import the buildflow package
-import buildflow
-from buildflow import Flow
-
-# Create the Flow object
-flow = Flow()
-
-# Define your input / output
-@flow.processor(
-   source=buildflow.PubSubSource(subscription='my_subscription'),
-   sink=buildflow.BigQuerySink(table_id='project.dataset.table'),
-)
-def stream_processor(pubsub_message):
-  # TODO(developer): Implement processing logic
-  ...
-  # The output is sent to the sink provider
-  return pubsub_message
+#### Pulumi Installation
 
-# Start the processor(s)
-flow.run().output()
-```
+BuildFlow uses Pulumi to manage resources used by your BuildFlow Nodes and Processors. To install Pulumi visit: https://www.pulumi.com/docs/install/
+
+Installing Pulumi unlocks:
+- allows BuildFlow to manage resource creation and destruction
+- full access to Pulumi API / CLI
+- fine-grained control over Pulumi Stacks & Resources
 
-For a more in depth tutorial see our [walkthroughs](https://www.buildflow.dev/docs/category/walk-throughs).
 
-## Windows Users
+## Quick Links
 
-Our runtime is built on [Ray](https://ray.io/), where Windows support is currently in beta. See the [Ray docs](https://docs.ray.io/en/latest/ray-overview/installation.html#windows-support) for more info.
+- **Docs**: https://www.buildflow.dev/docs
+- **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
+- **Discord**: https://discordapp.com/invite/wz7fjHyrCA
 
 ## Code Health Checks
 
 We use [black](https://github.com/psf/black) and [ruff](https://github.com/charliermarsh/ruff) with [pre-commit](https://pre-commit.com/) hooks to perform health checks.
 To setup these locally:
 
 - Clone the repo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildflow-0.1.0/README.md` & `buildflow-0.1.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,68 +1,49 @@
-# BuildFlow
+# ⚒️ BuildFlow
 
 ![CI](https://github.com/launchflow/buildflow/actions/workflows/python_ci.yaml/badge.svg)
 ![GCP Tests](https://github.com/launchflow/buildflow/actions/workflows/gcp_integration.yaml/badge.svg)
+[![Python version](https://badge.fury.io/py/buildflow.svg)](https://pypi.org/project/buildflow)
+[![codecov](https://codecov.io/gh/launchflow/buildflow/branch/main/graph/badge.svg?token=AO0TP8XG7X)](https://codecov.io/gh/launchflow/buildflow)
 [![Discord Shield](https://discordapp.com/api/guilds/1082821064180117575/widget.png?style=shield)](https://discordapp.com/invite/wz7fjHyrCA)
 
-**BuildFlow**, is an open source framework that lets you build a data pipeline by simply attaching a decorator to a Python function. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. No configuration outside of the code is required.
 
-Key Features:
+## Overview
+**BuildFlow**, is an open source framework for building large scale systems using Python. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. **No configuration outside of the code is required**.
 
-- Unified **batch** and **streaming** [Processor API](https://www.buildflow.dev/docs/processors/overview)
-- Production-grade [IO connectors](https://www.buildflow.dev/docs/io-connectors/overview) for popular cloud services & storage systems
-- IO templates for common data pipelines (e.g. [file upload notifications](https://www.buildflow.dev/docs/io-connectors/gcs_notifications))
-- Automatic [resource creation / management](https://www.buildflow.dev/docs/resource-creation) for popular cloud resources
-- [Schema validation](https://www.buildflow.dev/docs/schema-validation) powered by Python dataclasses and type hints
-- Automatic parallelism powered by [Ray](https://ray.io)
+Key Features (all provided out-of-the-box):
 
-## Quick Links
-
-- **Docs**: https://www.buildflow.dev/docs
-- **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
-- **Discord**: https://discordapp.com/invite/wz7fjHyrCA
-
-## Quickstart
+- Automatic [resource creation / management](https://www.buildflow.dev/docs/features/resource-creation) (Infrastructure as Code) powered by [Pulumi](https://github.com/pulumi/pulumi)
+- Automatic [parallelism & concurrency](https://www.buildflow.dev/docs/features/parallelism) powered by [Ray](https://github.com/ray-project/ray)
+- [Dynamic autoscaling](https://www.buildflow.dev/docs/features/autoscaling): scale up during high traffic / reduce costs during low traffic
+- [Schema validation](https://www.buildflow.dev/docs/features/schema-validation) powered by Python dataclasses and type hints
 
-### Install
+## Installation
 
 ```bash
 pip install buildflow
 ```
 
-### Example Usage
+### Extra Dependencies
 
-```python
-# Import the buildflow package
-import buildflow
-from buildflow import Flow
-
-# Create the Flow object
-flow = Flow()
-
-# Define your input / output
-@flow.processor(
-   source=buildflow.PubSubSource(subscription='my_subscription'),
-   sink=buildflow.BigQuerySink(table_id='project.dataset.table'),
-)
-def stream_processor(pubsub_message):
-  # TODO(developer): Implement processing logic
-  ...
-  # The output is sent to the sink provider
-  return pubsub_message
+#### Pulumi Installation
 
-# Start the processor(s)
-flow.run().output()
-```
+BuildFlow uses Pulumi to manage resources used by your BuildFlow Nodes and Processors. To install Pulumi visit: https://www.pulumi.com/docs/install/
+
+Installing Pulumi unlocks:
+- allows BuildFlow to manage resource creation and destruction
+- full access to Pulumi API / CLI
+- fine-grained control over Pulumi Stacks & Resources
 
-For a more in depth tutorial see our [walkthroughs](https://www.buildflow.dev/docs/category/walk-throughs).
 
-## Windows Users
+## Quick Links
 
-Our runtime is built on [Ray](https://ray.io/), where Windows support is currently in beta. See the [Ray docs](https://docs.ray.io/en/latest/ray-overview/installation.html#windows-support) for more info.
+- **Docs**: https://www.buildflow.dev/docs
+- **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
+- **Discord**: https://discordapp.com/invite/wz7fjHyrCA
 
 ## Code Health Checks
 
 We use [black](https://github.com/psf/black) and [ruff](https://github.com/charliermarsh/ruff) with [pre-commit](https://pre-commit.com/) hooks to perform health checks.
 To setup these locally:
 
 - Clone the repo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildflow-0.1.0/buildflow/api/__init__.py` & `buildflow-0.1.2/buildflow/api/__init__.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/grid.py` & `buildflow-0.1.2/buildflow/api/grid.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/infrastructure.py` & `buildflow-0.1.2/buildflow/api/infrastructure.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/io.py` & `buildflow-0.1.2/buildflow/api/io.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/node.py` & `buildflow-0.1.2/buildflow/api/node.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/options.py` & `buildflow-0.1.2/buildflow/api/options.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/processor.py` & `buildflow-0.1.2/buildflow/api/processor.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/api/runtime.py` & `buildflow-0.1.2/buildflow/api/runtime.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/cli/main.py` & `buildflow-0.1.2/buildflow/cli/main.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/cli/utils.py` & `buildflow-0.1.2/buildflow/cli/utils.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/exceptions/exceptions.py` & `buildflow-0.1.2/buildflow/core/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/grid/grid.py` & `buildflow-0.1.2/buildflow/core/grid/grid.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/infra/actors/pulumi_infra.py` & `buildflow-0.1.2/buildflow/core/infra/actors/pulumi_infra.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 @ray.remote
 class PulumiInfraActor(InfraAPI):
     def __init__(
         self,
         config: InfraConfig,
         *,
         # TODO: Support more pulumi options
+        stack_name: str,
         project_name: str = "buildflow-app",
-        stack_name: str = "buildflow-infra",
         passphrase: str = "",
         backend_url: str = f"file://{_PULUMI_DIR}",
     ) -> None:
         # NOTE: Ray actors run in their own process, so we need to configure
         # logging per actor / remote task.
         logging.getLogger().setLevel(config.log_level)
```

### Comparing `buildflow-0.1.0/buildflow/core/infra/actors/setup_infra.py` & `buildflow-0.1.2/buildflow/core/infra/actors/setup_infra.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/infra/config.py` & `buildflow-0.1.2/buildflow/core/infra/config.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/node/_utils.py` & `buildflow-0.1.2/buildflow/core/node/_utils.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/node/node.py` & `buildflow-0.1.2/buildflow/core/node/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,23 +228,27 @@
         return result
 
     def apply(self) -> NodeApplyResult:
         return asyncio.get_event_loop().run_until_complete(self._apply_async())
 
     async def _apply_async(self) -> NodeApplyResult:
         logging.info(f"Setting up infrastructure for Node({self.node_id})...")
-        infra_actor = PulumiInfraActor.remote(self._infra_config)
+        infra_actor = PulumiInfraActor.remote(
+            self._infra_config, stack_name=self.node_id
+        )
         result = await infra_actor.apply.remote(processors=self._processors)
         logging.info(f"...Finished setting up infrastructure for Node({self.node_id})")
         return result
 
     def destroy(self) -> NodeDestroyResult:
         return asyncio.get_event_loop().run_until_complete(self._destroy_async())
 
     async def _destroy_async(self) -> NodeDestroyResult:
         logging.info(f"Tearing down infrastructure for Node({self.node_id})...")
-        infra_actor = PulumiInfraActor.remote(self._infra_config)
+        infra_actor = PulumiInfraActor.remote(
+            self._infra_config, stack_name=self.node_id
+        )
         result = await infra_actor.destroy.remote(processors=self._processors)
         logging.info(
             f"...Finished tearing down infrastructure for Node({self.node_id})"
         )
         return result
```

### Comparing `buildflow-0.1.0/buildflow/core/processor/base.py` & `buildflow-0.1.2/buildflow/core/processor/base.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/actors/process_pool.py` & `buildflow-0.1.2/buildflow/core/runtime/actors/process_pool.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/actors/pull_process_push.py` & `buildflow-0.1.2/buildflow/core/runtime/actors/pull_process_push.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
     async def run(self):
         if self._status == RuntimeStatus.IDLE:
             logging.info("Starting PullProcessPushActor...")
             self._status = RuntimeStatus.RUNNING
         elif self._status == RuntimeStatus.DRAINING:
             raise RuntimeError("Cannot run a PullProcessPushActor that is draining.")
 
-        logging.info("Starting Thread...")
+        logging.debug("Starting Thread...")
         self._num_running_threads += 1
 
         raw_process_fn = self.processor.process
         full_arg_spec = inspect.getfullargspec(raw_process_fn)
         output_type = None
         input_type = None
         if "return" in full_arg_spec.annotations:
@@ -217,15 +217,15 @@
             self.total_time_gauge.set((time.time() - total_start_time) * 1000)
 
         self._num_running_threads -= 1
         if self._num_running_threads == 0:
             self._status = RuntimeStatus.IDLE
             logging.info("PullProcessPushActor Complete.")
 
-        logging.info("Thread Complete.")
+        logging.debug("Thread Complete.")
 
     async def status(self):
         # TODO: Have this method count the number of active threads
         return self._status
 
     async def drain(self):
         logging.info("Draining PullProcessPushActor...")
```

### Comparing `buildflow-0.1.0/buildflow/core/runtime/actors/pull_process_push_test.py` & `buildflow-0.1.2/buildflow/core/runtime/actors/pull_process_push_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/actors/runtime.py` & `buildflow-0.1.2/buildflow/core/runtime/actors/runtime.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/actors/runtime_test.py` & `buildflow-0.1.2/buildflow/core/runtime/actors/runtime_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/autoscale.py` & `buildflow-0.1.2/buildflow/core/runtime/autoscale.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/autoscale_test.py` & `buildflow-0.1.2/buildflow/core/runtime/autoscale_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/core/runtime/config.py` & `buildflow-0.1.2/buildflow/core/runtime/config.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/depends/depends.py` & `buildflow-0.1.2/buildflow/io/depends/depends.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/base.py` & `buildflow-0.1.2/buildflow/io/providers/base.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/file_provider.py` & `buildflow-0.1.2/buildflow/io/providers/file_provider.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/file_provider_test.py` & `buildflow-0.1.2/buildflow/io/providers/file_provider_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/bigquery.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/bigquery.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/bigquery_test.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/bigquery_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/gcp_pub_sub.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/gcp_pub_sub.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/gcp_pub_sub_test.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/gcp_pub_sub_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/gcs_file_stream.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/gcs_file_stream_test.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/gcs_file_stream_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/utils/clients.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/utils/clients.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/gcp/utils/setup_utils.py` & `buildflow-0.1.2/buildflow/io/providers/gcp/utils/setup_utils.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/pulsing_provider.py` & `buildflow-0.1.2/buildflow/io/providers/pulsing_provider.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/pulsing_provider_test.py` & `buildflow-0.1.2/buildflow/io/providers/pulsing_provider_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas.py` & `buildflow-0.1.2/buildflow/io/providers/schemas/bigquery_schemas.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/schemas/bigquery_schemas_test.py` & `buildflow-0.1.2/buildflow/io/providers/schemas/bigquery_schemas_test.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/io/providers/schemas/converters.py` & `buildflow-0.1.2/buildflow/io/providers/schemas/converters.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,28 +15,37 @@
 
 import datetime
 from dataclasses import is_dataclass
 import json
 from typing import Any, Dict, Callable, Optional, Type
 
 import dacite
+import pandas as pd
 
 from buildflow.core import exceptions
 
 
+def str_to_datetime(s: str) -> datetime.datetime:
+    return pd.Timestamp(s).to_pydatetime()
+
+
 def identity():
     return lambda x: x
 
 
 def bytes_to_dict() -> Callable[[bytes], Dict[str, Any]]:
     return lambda bytes_: json.loads(bytes_.decode())
 
 
 def bytes_to_dataclass(type_: Type) -> Callable[[bytes], Any]:
-    return lambda bytes_: dacite.from_dict(type_, json.loads(bytes_.decode()))
+    return lambda bytes_: dacite.from_dict(
+        type_,
+        json.loads(bytes_.decode()),
+        config=dacite.Config(type_hooks={datetime.datetime: str_to_datetime}),
+    )
 
 
 def _dataclass_to_json(dataclass_instance) -> Dict[str, Any]:
     # NOTE: we roll our own asdict instead of using dataclasses.asdict because
     # of an issue with dataclasses and cloudpickle.
     # https://github.com/cloudpipe/cloudpickle/issues/386
     # This also converts some field types that we know aren't serializable to
```

### Comparing `buildflow-0.1.0/buildflow/io/providers/schemas/converters_test.py` & `buildflow-0.1.2/buildflow/io/providers/schemas/converters_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from dataclasses import asdict, dataclass
+import datetime
 import json
 from typing import Dict, List, Optional, Set
 import unittest
 
 from buildflow.core import exceptions
 from buildflow.io.providers.schemas import converters
 
@@ -14,40 +15,52 @@
 
 @dataclass
 class InputDataClass:
     a: int
     b: int
     nested: Optional[Nested] = None
     nested_list: Optional[List[Nested]] = None
+    timestamp: Optional[datetime.datetime] = None
 
 
 class ConvertersTest(unittest.TestCase):
     def test_bytes_to_dict(self):
         expected_dict = {"a": 1, "b": 2}
         intput_bytes = json.dumps(expected_dict).encode("utf-8")
 
         converter = converters.bytes_to_dict()
 
         self.assertEqual(expected_dict, converter(intput_bytes))
 
     def test_bytes_to_dataclass(self):
         expected_output = InputDataClass(
-            a=1, b=2, nested=Nested(c=3), nested_list=[Nested(c=4)]
+            a=1,
+            b=2,
+            nested=Nested(c=3),
+            nested_list=[Nested(c=4)],
+            timestamp=datetime.datetime.now(),
         )
-        intput_bytes = json.dumps(asdict(expected_output)).encode("utf-8")
+        output_dict = asdict(expected_output)
+        output_dict["timestamp"] = output_dict["timestamp"].isoformat()
+        intput_bytes = json.dumps(output_dict).encode("utf-8")
 
         converter = converters.bytes_to_dataclass(InputDataClass)
 
         self.assertEqual(expected_output, converter(intput_bytes))
 
     def test_dataclass_to_json(self):
         input_class = InputDataClass(
-            a=1, b=2, nested=Nested(c=3), nested_list=[Nested(c=4)]
+            a=1,
+            b=2,
+            nested=Nested(c=3),
+            nested_list=[Nested(c=4)],
+            timestamp=datetime.datetime.now(),
         )
         expected_output = asdict(input_class)
+        expected_output["timestamp"] = expected_output["timestamp"].isoformat()
 
         converter = converters.dataclass_to_json()
 
         converted_json = converter(input_class)
         self.assertEqual(expected_output, converted_json)
 
     def test_json_push_converter_none(self):
```

### Comparing `buildflow-0.1.0/buildflow/io/registry.py` & `buildflow-0.1.2/buildflow/io/registry.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/samples/csv_bigquery_walkthrough.py` & `buildflow-0.1.2/buildflow/samples/csv_bigquery_walkthrough.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/samples/pubsub_walkthrough.py` & `buildflow-0.1.2/buildflow/samples/pubsub_walkthrough.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow/utils.py` & `buildflow-0.1.2/buildflow/utils.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/buildflow.egg-info/PKG-INFO` & `buildflow-0.1.2/buildflow.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,82 +1,63 @@
 Metadata-Version: 2.1
 Name: buildflow
-Version: 0.1.0
+Version: 0.1.2
 Summary: buildflow is a unified **batch** and **streaming** framework that turns any python function into a scalable data pipeline that can read from our supported IO resources.
 Author-email: Caleb Van Dyke <caleb@launchflow.com>, Josh Tanke <josh@launchflow.com>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
-# BuildFlow
+# ⚒️ BuildFlow
 
 ![CI](https://github.com/launchflow/buildflow/actions/workflows/python_ci.yaml/badge.svg)
 ![GCP Tests](https://github.com/launchflow/buildflow/actions/workflows/gcp_integration.yaml/badge.svg)
+[![Python version](https://badge.fury.io/py/buildflow.svg)](https://pypi.org/project/buildflow)
+[![codecov](https://codecov.io/gh/launchflow/buildflow/branch/main/graph/badge.svg?token=AO0TP8XG7X)](https://codecov.io/gh/launchflow/buildflow)
 [![Discord Shield](https://discordapp.com/api/guilds/1082821064180117575/widget.png?style=shield)](https://discordapp.com/invite/wz7fjHyrCA)
 
-**BuildFlow**, is an open source framework that lets you build a data pipeline by simply attaching a decorator to a Python function. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. No configuration outside of the code is required.
 
-Key Features:
+## Overview
+**BuildFlow**, is an open source framework for building large scale systems using Python. All you need to do is describe where your input is coming from and where your output should be written, and BuildFlow handles the rest. **No configuration outside of the code is required**.
 
-- Unified **batch** and **streaming** [Processor API](https://www.buildflow.dev/docs/processors/overview)
-- Production-grade [IO connectors](https://www.buildflow.dev/docs/io-connectors/overview) for popular cloud services & storage systems
-- IO templates for common data pipelines (e.g. [file upload notifications](https://www.buildflow.dev/docs/io-connectors/gcs_notifications))
-- Automatic [resource creation / management](https://www.buildflow.dev/docs/resource-creation) for popular cloud resources
-- [Schema validation](https://www.buildflow.dev/docs/schema-validation) powered by Python dataclasses and type hints
-- Automatic parallelism powered by [Ray](https://ray.io)
+Key Features (all provided out-of-the-box):
 
-## Quick Links
-
-- **Docs**: https://www.buildflow.dev/docs
-- **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
-- **Discord**: https://discordapp.com/invite/wz7fjHyrCA
-
-## Quickstart
+- Automatic [resource creation / management](https://www.buildflow.dev/docs/features/resource-creation) (Infrastructure as Code) powered by [Pulumi](https://github.com/pulumi/pulumi)
+- Automatic [parallelism & concurrency](https://www.buildflow.dev/docs/features/parallelism) powered by [Ray](https://github.com/ray-project/ray)
+- [Dynamic autoscaling](https://www.buildflow.dev/docs/features/autoscaling): scale up during high traffic / reduce costs during low traffic
+- [Schema validation](https://www.buildflow.dev/docs/features/schema-validation) powered by Python dataclasses and type hints
 
-### Install
+## Installation
 
 ```bash
 pip install buildflow
 ```
 
-### Example Usage
+### Extra Dependencies
 
-```python
-# Import the buildflow package
-import buildflow
-from buildflow import Flow
-
-# Create the Flow object
-flow = Flow()
-
-# Define your input / output
-@flow.processor(
-   source=buildflow.PubSubSource(subscription='my_subscription'),
-   sink=buildflow.BigQuerySink(table_id='project.dataset.table'),
-)
-def stream_processor(pubsub_message):
-  # TODO(developer): Implement processing logic
-  ...
-  # The output is sent to the sink provider
-  return pubsub_message
+#### Pulumi Installation
 
-# Start the processor(s)
-flow.run().output()
-```
+BuildFlow uses Pulumi to manage resources used by your BuildFlow Nodes and Processors. To install Pulumi visit: https://www.pulumi.com/docs/install/
+
+Installing Pulumi unlocks:
+- allows BuildFlow to manage resource creation and destruction
+- full access to Pulumi API / CLI
+- fine-grained control over Pulumi Stacks & Resources
 
-For a more in depth tutorial see our [walkthroughs](https://www.buildflow.dev/docs/category/walk-throughs).
 
-## Windows Users
+## Quick Links
 
-Our runtime is built on [Ray](https://ray.io/), where Windows support is currently in beta. See the [Ray docs](https://docs.ray.io/en/latest/ray-overview/installation.html#windows-support) for more info.
+- **Docs**: https://www.buildflow.dev/docs
+- **Walkthroughs**: https://www.buildflow.dev/docs/category/walk-throughs
+- **Discord**: https://discordapp.com/invite/wz7fjHyrCA
 
 ## Code Health Checks
 
 We use [black](https://github.com/psf/black) and [ruff](https://github.com/charliermarsh/ruff) with [pre-commit](https://pre-commit.com/) hooks to perform health checks.
 To setup these locally:
 
 - Clone the repo
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `buildflow-0.1.0/buildflow.egg-info/SOURCES.txt` & `buildflow-0.1.2/buildflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_main.py` & `buildflow-0.1.2/integration_tests/pubsub_to_pubsub/pubsub_main.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_publish.py` & `buildflow-0.1.2/integration_tests/pubsub_to_pubsub/pubsub_publish.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/integration_tests/pubsub_to_pubsub/pubsub_validation.py` & `buildflow-0.1.2/integration_tests/pubsub_to_pubsub/pubsub_validation.py`

 * *Files identical despite different names*

### Comparing `buildflow-0.1.0/pyproject.toml` & `buildflow-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "buildflow"
-version = "0.1.0"
+version = "0.1.2"
 authors = [
     { name = "Caleb Van Dyke", email = "caleb@launchflow.com" },
     { name = "Josh Tanke", email = "josh@launchflow.com" },
 ]
 description = "buildflow is a unified **batch** and **streaming** framework that turns any python function into a scalable data pipeline that can read from our supported IO resources."
 readme = "README.md"
 requires-python = ">=3.7"
```

