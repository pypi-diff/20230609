# Comparing `tmp/flytekit-1.6.2b0.tar.gz` & `tmp/flytekit-1.6.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.6.2b0.tar", last modified: Thu Jun  1 20:41:44 2023, max compression
+gzip compressed data, was "flytekit-1.6.2b1.tar", last modified: Thu Jun  8 23:49:31 2023, max compression
```

## Comparing `flytekit-1.6.2b0.tar` & `flytekit-1.6.2b1.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-01 20:41:42.000000 flytekit-1.6.2b0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23028 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.331650 flytekit-1.6.2b0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12783 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/backend/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extend/backend/external_plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.339650 flytekit-1.6.2b0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.343650 flytekit-1.6.2b0/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.347651 flytekit-1.6.2b0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.347651 flytekit-1.6.2b0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.347651 flytekit-1.6.2b0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.351651 flytekit-1.6.2b0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.327650 flytekit-1.6.2b0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 20:41:44.000000 flytekit-1.6.2b0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-01 20:41:31.000000 flytekit-1.6.2b0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-01 20:41:44.355651 flytekit-1.6.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-01 20:41:42.000000 flytekit-1.6.2b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.811171 flytekit-1.6.2b1/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-06-08 23:49:29.000000 flytekit-1.6.2b1/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.811171 flytekit-1.6.2b1/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23142 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.815171 flytekit-1.6.2b1/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.819171 flytekit-1.6.2b1/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.827171 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5469 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.827171 flytekit-1.6.2b1/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.835171 flytekit-1.6.2b1/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31002 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36384 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17833 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46442 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77072 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.835171 flytekit-1.6.2b1/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.839171 flytekit-1.6.2b1/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.843171 flytekit-1.6.2b1/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.847171 flytekit-1.6.2b1/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.847171 flytekit-1.6.2b1/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.847171 flytekit-1.6.2b1/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87310 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.851171 flytekit-1.6.2b1/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23925 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.811171 flytekit-1.6.2b1/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 23:49:31.000000 flytekit-1.6.2b1/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 23:49:15.000000 flytekit-1.6.2b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 23:49:31.855171 flytekit-1.6.2b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-08 23:49:29.000000 flytekit-1.6.2b1/setup.py
```

### Comparing `flytekit-1.6.2b0/LICENSE` & `flytekit-1.6.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/MANIFEST.in` & `flytekit-1.6.2b1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/PKG-INFO` & `flytekit-1.6.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.2b0/README.md` & `flytekit-1.6.2b1/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/__init__.py` & `flytekit-1.6.2b1/flytekit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,15 +238,15 @@
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.6.2b0"
+__version__ = "1.6.2b1"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
```

### Comparing `flytekit-1.6.2b0/flytekit/bin/entrypoint.py` & `flytekit-1.6.2b1/flytekit/bin/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from flytekit.core import utils
 from flytekit.core.base_task import IgnoreOutputs, PythonTask
 from flytekit.core.checkpointer import SyncCheckpoint
 from flytekit.core.context_manager import ExecutionParameters, ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.data_persistence import FileAccessProvider
 from flytekit.core.map_task import MapTaskResolver
 from flytekit.core.promise import VoidPromise
+from flytekit.deck.deck import _output_deck
 from flytekit.exceptions import scopes as _scoped_exceptions
 from flytekit.exceptions import scopes as _scopes
 from flytekit.interfaces.stats.taggable import get_stats as _get_stats
 from flytekit.loggers import entrypoint_logger as logger
 from flytekit.loggers import user_space_logger
 from flytekit.models import dynamic_job as _dynamic_job
 from flytekit.models import literals as _literal_models
@@ -153,14 +154,15 @@
         logger.error(exc_str)
         logger.error("!! End Error Captured by Flyte !!")
 
     for k, v in output_file_dict.items():
         utils.write_proto_to_file(v.to_flyte_idl(), os.path.join(ctx.execution_state.engine_dir, k))
 
     ctx.file_access.put_data(ctx.execution_state.engine_dir, output_prefix, is_multipart=True)
+    _output_deck(task_def.name.split(".")[-1], ctx.user_space_params)
     logger.info(f"Engine folder written successfully to the output prefix {output_prefix}")
     logger.debug("Finished _dispatch_execute")
 
     if os.environ.get("FLYTE_FAIL_ON_ERROR", "").lower() == "true" and _constants.ERROR_FILE_NAME in output_file_dict:
         # This env is set by the flytepropeller
         # AWS batch job get the status from the exit code, so once we catch the error,
         # we should return the error code here
```

### Comparing `flytekit-1.6.2b0/flytekit/clients/auth/auth_client.py` & `flytekit-1.6.2b1/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/auth/authenticator.py` & `flytekit-1.6.2b1/flytekit/clients/auth/authenticator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/auth/keyring.py` & `flytekit-1.6.2b1/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/auth/token_client.py` & `flytekit-1.6.2b1/flytekit/clients/auth/token_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/auth_helper.py` & `flytekit-1.6.2b1/flytekit/clients/auth_helper.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/friendly.py` & `flytekit-1.6.2b1/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.6.2b1/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.6.2b1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/helpers.py` & `flytekit-1.6.2b1/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clients/raw.py` & `flytekit-1.6.2b1/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.6.2b1/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/helpers.py` & `flytekit-1.6.2b1/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/build.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/run.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serialize.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/clis/sdk_in_container/serve.py` & `flytekit-1.6.2b1/flytekit/clis/sdk_in_container/serve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from concurrent import futures
 
 import click
 import grpc
-from flyteidl.service.external_plugin_service_pb2_grpc import add_ExternalPluginServiceServicer_to_server
+from flyteidl.service.agent_pb2_grpc import add_AsyncAgentServiceServicer_to_server
 
-from flytekit.extend.backend.external_plugin_service import BackendPluginServer
+from flytekit.extend.backend.agent_service import AgentService
 
-_serve_help = """Start a grpc server for the external plugin service."""
+_serve_help = """Start a grpc server for the agent service."""
 
 
 @click.command("serve", help=_serve_help)
 @click.option(
     "--port",
     default="8000",
     is_flag=False,
     type=int,
-    help="Grpc port for the external plugin service",
+    help="Grpc port for the agent service",
 )
 @click.option(
     "--worker",
     default="10",
     is_flag=False,
     type=int,
     help="Number of workers for the grpc server",
@@ -31,16 +31,16 @@
     type=int,
     help="It will wait for the specified number of seconds before shutting down grpc server. It should only be used "
     "for testing.",
 )
 @click.pass_context
 def serve(_: click.Context, port, worker, timeout):
     """
-    Start a grpc server for the external plugin service.
+    Start a grpc server for the agent service.
     """
-    click.secho("Starting the external plugin service...", fg="blue")
+    click.secho("Starting the agent service...", fg="blue")
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=worker))
-    add_ExternalPluginServiceServicer_to_server(BackendPluginServer(), server)
+    add_AsyncAgentServiceServicer_to_server(AgentService(), server)
 
     server.add_insecure_port(f"[::]:{port}")
     server.start()
     server.wait_for_termination(timeout=timeout)
```

### Comparing `flytekit-1.6.2b0/flytekit/configuration/__init__.py` & `flytekit-1.6.2b1/flytekit/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/configuration/default_images.py` & `flytekit-1.6.2b1/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/configuration/feature_flags.py` & `flytekit-1.6.2b1/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/configuration/file.py` & `flytekit-1.6.2b1/flytekit/configuration/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/configuration/internal.py` & `flytekit-1.6.2b1/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/annotation.py` & `flytekit-1.6.2b1/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/base_sql_task.py` & `flytekit-1.6.2b1/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/base_task.py` & `flytekit-1.6.2b1/flytekit/core/base_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -505,15 +505,14 @@
         * ``Literal Map`` is returned when the task returns either one more outputs in the declaration. Individual outputs
           may be none
         * ``DynamicJobSpec`` is returned when a dynamic workflow is executed
         """
 
         # Invoked before the task is executed
         new_user_params = self.pre_execute(ctx.user_space_params)
-        from flytekit.deck.deck import _output_deck
 
         # Create another execution context with the new user params, but let's keep the same working dir
         with FlyteContextManager.with_context(
             ctx.with_execution_state(
                 cast(ExecutionState, ctx.execution_state).with_params(user_space_params=new_user_params)
             )
             # type: ignore
@@ -598,16 +597,14 @@
                 for k, v in native_inputs.items():
                     input_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_input_var(k, v)))
 
                 output_deck = Deck(OUTPUT)
                 for k, v in native_outputs_as_map.items():
                     output_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_output_var(k, v)))
 
-                _output_deck(self.name.split(".")[-1], new_user_params)
-
             outputs_literal_map = _literal_models.LiteralMap(literals=literals)
             # After the execute has been successfully completed
             return outputs_literal_map
 
     def pre_execute(self, user_params: Optional[ExecutionParameters]) -> Optional[ExecutionParameters]:  # type: ignore
         """
         This is the method that will be invoked directly before executing the task method and before all the inputs
```

### Comparing `flytekit-1.6.2b0/flytekit/core/checkpointer.py` & `flytekit-1.6.2b1/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/class_based_resolver.py` & `flytekit-1.6.2b1/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/condition.py` & `flytekit-1.6.2b1/flytekit/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/constants.py` & `flytekit-1.6.2b1/flytekit/core/constants.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/container_task.py` & `flytekit-1.6.2b1/flytekit/core/container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/context_manager.py` & `flytekit-1.6.2b1/flytekit/core/context_manager.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/data_persistence.py` & `flytekit-1.6.2b1/flytekit/core/data_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,44 +283,43 @@
     def upload_directory(self, local_path: str, remote_path: str):
         """
         :param Text local_path:
         :param Text remote_path:
         """
         return self.put_data(local_path, remote_path, is_multipart=True)
 
-    @timeit("Download data to local from remote")
     def get_data(self, remote_path: str, local_path: str, is_multipart: bool = False):
         """
         :param remote_path:
         :param local_path:
         :param is_multipart:
         """
         try:
             pathlib.Path(local_path).parent.mkdir(parents=True, exist_ok=True)
-            self.get(remote_path, to_path=local_path, recursive=is_multipart)
+            with timeit(f"Download data to local from {remote_path}"):
+                self.get(remote_path, to_path=local_path, recursive=is_multipart)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to get data from {remote_path} to {local_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             )
 
-    @timeit("Upload data to remote")
     def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False, **kwargs):
         """
         The implication here is that we're always going to put data to the remote location, so we .remote to ensure
         we don't use the true local proxy if the remote path is a file://
 
         :param local_path:
         :param remote_path:
         :param is_multipart:
         """
         try:
             local_path = str(local_path)
-
-            self.put(cast(str, local_path), remote_path, recursive=is_multipart, **kwargs)
+            with timeit(f"Upload data to {remote_path}"):
+                self.put(cast(str, local_path), remote_path, recursive=is_multipart, **kwargs)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to put data from {local_path} to {remote_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             ) from ex
```

### Comparing `flytekit-1.6.2b0/flytekit/core/docstring.py` & `flytekit-1.6.2b1/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.6.2b1/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/gate.py` & `flytekit-1.6.2b1/flytekit/core/gate.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/interface.py` & `flytekit-1.6.2b1/flytekit/core/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/launch_plan.py` & `flytekit-1.6.2b1/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/local_cache.py` & `flytekit-1.6.2b1/flytekit/core/local_cache.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/map_task.py` & `flytekit-1.6.2b1/flytekit/core/map_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/mock_stats.py` & `flytekit-1.6.2b1/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/node.py` & `flytekit-1.6.2b1/flytekit/core/node.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/node_creation.py` & `flytekit-1.6.2b1/flytekit/core/node_creation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/notification.py` & `flytekit-1.6.2b1/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/pod_template.py` & `flytekit-1.6.2b1/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/promise.py` & `flytekit-1.6.2b1/flytekit/core/promise.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/python_auto_container.py` & `flytekit-1.6.2b1/flytekit/core/python_auto_container.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/python_customized_container_task.py` & `flytekit-1.6.2b1/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/python_function_task.py` & `flytekit-1.6.2b1/flytekit/core/python_function_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/reference.py` & `flytekit-1.6.2b1/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/reference_entity.py` & `flytekit-1.6.2b1/flytekit/core/reference_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/resources.py` & `flytekit-1.6.2b1/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/schedule.py` & `flytekit-1.6.2b1/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/shim_task.py` & `flytekit-1.6.2b1/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/task.py` & `flytekit-1.6.2b1/flytekit/core/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/testing.py` & `flytekit-1.6.2b1/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/tracker.py` & `flytekit-1.6.2b1/flytekit/core/tracker.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/type_engine.py` & `flytekit-1.6.2b1/flytekit/core/type_engine.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/type_helpers.py` & `flytekit-1.6.2b1/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/utils.py` & `flytekit-1.6.2b1/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/core/workflow.py` & `flytekit-1.6.2b1/flytekit/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/deck/deck.py` & `flytekit-1.6.2b1/flytekit/deck/deck.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/deck/html/template.html` & `flytekit-1.6.2b1/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/deck/renderer.py` & `flytekit-1.6.2b1/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/exceptions/scopes.py` & `flytekit-1.6.2b1/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/exceptions/system.py` & `flytekit-1.6.2b1/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/exceptions/user.py` & `flytekit-1.6.2b1/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extend/__init__.py` & `flytekit-1.6.2b1/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extend/backend/base_plugin.py` & `flytekit-1.6.2b1/flytekit/extend/backend/base_agent.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 import typing
 from abc import ABC, abstractmethod
 
 import grpc
-from flyteidl.core.tasks_pb2 import TaskTemplate
-from flyteidl.service.external_plugin_service_pb2 import (
+from flyteidl.admin.agent_pb2 import (
     RETRYABLE_FAILURE,
     RUNNING,
     SUCCEEDED,
+    CreateTaskResponse,
+    DeleteTaskResponse,
+    GetTaskResponse,
     State,
-    TaskCreateResponse,
-    TaskDeleteResponse,
-    TaskGetResponse,
 )
+from flyteidl.core.tasks_pb2 import TaskTemplate
 
 from flytekit import logger
 from flytekit.models.literals import LiteralMap
 
 
-class BackendPluginBase(ABC):
+class AgentBase(ABC):
     """
-    This is the base class for all backend plugins. It defines the interface that all plugins must implement.
-    The external plugins service will be run either locally or in a pod, and will be responsible for
-    invoking backend plugins. The propeller will communicate with the external plugins service
+    This is the base class for all agents. It defines the interface that all agents must implement.
+    The agent service will be run either locally or in a pod, and will be responsible for
+    invoking agents. The propeller will communicate with the agent service
     to create tasks, get the status of tasks, and delete tasks.
 
-    All the backend plugins should be registered in the BackendPluginRegistry. External plugins service
-    will look up the plugin based on the task type. Every task type can only have one plugin.
+    All the agents should be registered in the AgentRegistry. Agent Service
+    will look up the agent based on the task type. Every task type can only have one agent.
     """
 
     def __init__(self, task_type: str):
         self._task_type = task_type
 
     @property
     def task_type(self) -> str:
         """
-        task_type is the name of the task type that this plugin supports.
+        task_type is the name of the task type that this agent supports.
         """
         return self._task_type
 
     @abstractmethod
     def create(
         self,
         context: grpc.ServicerContext,
         output_prefix: str,
         task_template: TaskTemplate,
         inputs: typing.Optional[LiteralMap] = None,
-    ) -> TaskCreateResponse:
+    ) -> CreateTaskResponse:
         """
         Return a Unique ID for the task that was created. It should return error code if the task creation failed.
         """
         pass
 
     @abstractmethod
-    def get(self, context: grpc.ServicerContext, job_id: str) -> TaskGetResponse:
+    def get(self, context: grpc.ServicerContext, resource_meta: bytes) -> GetTaskResponse:
         """
         Return the status of the task, and return the outputs in some cases. For example, bigquery job
         can't write the structured dataset to the output location, so it returns the output literals to the propeller,
         and the propeller will write the structured dataset to the blob store.
         """
         pass
 
     @abstractmethod
-    def delete(self, context: grpc.ServicerContext, job_id: str) -> TaskDeleteResponse:
+    def delete(self, context: grpc.ServicerContext, resource_meta: bytes) -> DeleteTaskResponse:
         """
         Delete the task. This call should be idempotent.
         """
         pass
 
 
-class BackendPluginRegistry(object):
+class AgentRegistry(object):
     """
-    This is the registry for all backend plugins. The external plugins service will look up the plugin
+    This is the registry for all agents. The agent service will look up the agent
     based on the task type.
     """
 
-    _REGISTRY: typing.Dict[str, BackendPluginBase] = {}
+    _REGISTRY: typing.Dict[str, AgentBase] = {}
 
     @staticmethod
-    def register(plugin: BackendPluginBase):
-        if plugin.task_type in BackendPluginRegistry._REGISTRY:
-            raise ValueError(f"Duplicate plugin for task type {plugin.task_type}")
-        BackendPluginRegistry._REGISTRY[plugin.task_type] = plugin
-        logger.info(f"Registering backend plugin for task type {plugin.task_type}")
+    def register(agent: AgentBase):
+        if agent.task_type in AgentRegistry._REGISTRY:
+            raise ValueError(f"Duplicate agent for task type {agent.task_type}")
+        AgentRegistry._REGISTRY[agent.task_type] = agent
+        logger.info(f"Registering an agent for task type {agent.task_type}")
 
     @staticmethod
-    def get_plugin(context: grpc.ServicerContext, task_type: str) -> typing.Optional[BackendPluginBase]:
-        if task_type not in BackendPluginRegistry._REGISTRY:
-            logger.error(f"Cannot find backend plugin for task type [{task_type}]")
+    def get_agent(context: grpc.ServicerContext, task_type: str) -> typing.Optional[AgentBase]:
+        if task_type not in AgentRegistry._REGISTRY:
+            logger.error(f"Cannot find agent for task type [{task_type}]")
             context.set_code(grpc.StatusCode.NOT_FOUND)
-            context.set_details(f"Cannot find backend plugin for task type [{task_type}]")
+            context.set_details(f"Cannot find the agent for task type [{task_type}]")
             return None
-        return BackendPluginRegistry._REGISTRY[task_type]
+        return AgentRegistry._REGISTRY[task_type]
 
 
 def convert_to_flyte_state(state: str) -> State:
     """
-    Convert the state from the backend plugin to the state in flyte.
+    Convert the state from the agent to the state in flyte.
     """
     state = state.lower()
     if state in ["failed"]:
         return RETRYABLE_FAILURE
     elif state in ["done", "succeeded"]:
         return SUCCEEDED
     elif state in ["running"]:
```

### Comparing `flytekit-1.6.2b0/flytekit/extend/backend/external_plugin_service.py` & `flytekit-1.6.2b1/flytekit/extend/backend/agent_service.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 import grpc
-from flyteidl.service.external_plugin_service_pb2 import (
+from flyteidl.admin.agent_pb2 import (
     PERMANENT_FAILURE,
-    TaskCreateRequest,
-    TaskCreateResponse,
-    TaskDeleteRequest,
-    TaskDeleteResponse,
-    TaskGetRequest,
-    TaskGetResponse,
+    CreateTaskRequest,
+    CreateTaskResponse,
+    DeleteTaskRequest,
+    DeleteTaskResponse,
+    GetTaskRequest,
+    GetTaskResponse,
+    Resource,
 )
-from flyteidl.service.external_plugin_service_pb2_grpc import ExternalPluginServiceServicer
+from flyteidl.service.agent_pb2_grpc import AsyncAgentServiceServicer
 
 from flytekit import logger
-from flytekit.extend.backend.base_plugin import BackendPluginRegistry
+from flytekit.extend.backend.base_agent import AgentRegistry
 from flytekit.models.literals import LiteralMap
 from flytekit.models.task import TaskTemplate
 
 
-class BackendPluginServer(ExternalPluginServiceServicer):
-    def CreateTask(self, request: TaskCreateRequest, context: grpc.ServicerContext) -> TaskCreateResponse:
+class AgentService(AsyncAgentServiceServicer):
+    def CreateTask(self, request: CreateTaskRequest, context: grpc.ServicerContext) -> CreateTaskResponse:
         try:
             tmp = TaskTemplate.from_flyte_idl(request.template)
             inputs = LiteralMap.from_flyte_idl(request.inputs) if request.inputs else None
-            plugin = BackendPluginRegistry.get_plugin(context, tmp.type)
-            if plugin is None:
-                return TaskCreateResponse()
-            return plugin.create(context=context, inputs=inputs, output_prefix=request.output_prefix, task_template=tmp)
+            agent = AgentRegistry.get_agent(context, tmp.type)
+            if agent is None:
+                return CreateTaskResponse()
+            return agent.create(context=context, inputs=inputs, output_prefix=request.output_prefix, task_template=tmp)
         except Exception as e:
             logger.error(f"failed to create task with error {e}")
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(f"failed to create task with error {e}")
 
-    def GetTask(self, request: TaskGetRequest, context: grpc.ServicerContext) -> TaskGetResponse:
+    def GetTask(self, request: GetTaskRequest, context: grpc.ServicerContext) -> GetTaskResponse:
         try:
-            plugin = BackendPluginRegistry.get_plugin(context, request.task_type)
-            if plugin is None:
-                return TaskGetResponse(state=PERMANENT_FAILURE)
-            return plugin.get(context=context, job_id=request.job_id)
+            agent = AgentRegistry.get_agent(context, request.task_type)
+            if agent is None:
+                return GetTaskResponse(resource=Resource(state=PERMANENT_FAILURE))
+            return agent.get(context=context, resource_meta=request.resource_meta)
         except Exception as e:
             logger.error(f"failed to get task with error {e}")
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(f"failed to get task with error {e}")
 
-    def DeleteTask(self, request: TaskDeleteRequest, context: grpc.ServicerContext) -> TaskDeleteResponse:
+    def DeleteTask(self, request: DeleteTaskRequest, context: grpc.ServicerContext) -> DeleteTaskResponse:
         try:
-            plugin = BackendPluginRegistry.get_plugin(context, request.task_type)
-            if plugin is None:
-                return TaskDeleteResponse()
-            return plugin.delete(context=context, job_id=request.job_id)
+            agent = AgentRegistry.get_agent(context, request.task_type)
+            if agent is None:
+                return DeleteTaskResponse()
+            return agent.delete(context=context, resource_meta=request.resource_meta)
         except Exception as e:
             logger.error(f"failed to delete task with error {e}")
             context.set_code(grpc.StatusCode.INTERNAL)
             context.set_details(f"failed to delete task with error {e}")
```

### Comparing `flytekit-1.6.2b0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.6.2b1/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.6.2b1/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.6.2b1/flytekit/extras/pytorch/checkpoint.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/pytorch/native.py` & `flytekit-1.6.2b1/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.6.2b1/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/sklearn/native.py` & `flytekit-1.6.2b1/flytekit/extras/sklearn/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/sqlite3/task.py` & `flytekit-1.6.2b1/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/tasks/shell.py` & `flytekit-1.6.2b1/flytekit/extras/tasks/shell.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.6.2b1/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/tensorflow/model.py` & `flytekit-1.6.2b1/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/extras/tensorflow/record.py` & `flytekit-1.6.2b1/flytekit/extras/tensorflow/record.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/image_spec/image_spec.py` & `flytekit-1.6.2b1/flytekit/image_spec/image_spec.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/interaction/parse_stdin.py` & `flytekit-1.6.2b1/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.6.2b1/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/interfaces/random.py` & `flytekit-1.6.2b1/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/interfaces/stats/client.py` & `flytekit-1.6.2b1/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.6.2b1/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/lazy_import/lazy_module.py` & `flytekit-1.6.2b1/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/loggers.py` & `flytekit-1.6.2b1/flytekit/loggers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/admin/common.py` & `flytekit-1.6.2b1/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/admin/task_execution.py` & `flytekit-1.6.2b1/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/admin/workflow.py` & `flytekit-1.6.2b1/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/annotation.py` & `flytekit-1.6.2b1/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/array_job.py` & `flytekit-1.6.2b1/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/common.py` & `flytekit-1.6.2b1/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/catalog.py` & `flytekit-1.6.2b1/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/compiler.py` & `flytekit-1.6.2b1/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/condition.py` & `flytekit-1.6.2b1/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/errors.py` & `flytekit-1.6.2b1/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/execution.py` & `flytekit-1.6.2b1/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/identifier.py` & `flytekit-1.6.2b1/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/types.py` & `flytekit-1.6.2b1/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/core/workflow.py` & `flytekit-1.6.2b1/flytekit/models/core/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/documentation.py` & `flytekit-1.6.2b1/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/dynamic_job.py` & `flytekit-1.6.2b1/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/execution.py` & `flytekit-1.6.2b1/flytekit/models/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/filters.py` & `flytekit-1.6.2b1/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/interface.py` & `flytekit-1.6.2b1/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/launch_plan.py` & `flytekit-1.6.2b1/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/literals.py` & `flytekit-1.6.2b1/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/matchable_resource.py` & `flytekit-1.6.2b1/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/named_entity.py` & `flytekit-1.6.2b1/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/node_execution.py` & `flytekit-1.6.2b1/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/presto.py` & `flytekit-1.6.2b1/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/project.py` & `flytekit-1.6.2b1/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/qubole.py` & `flytekit-1.6.2b1/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/schedule.py` & `flytekit-1.6.2b1/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/security.py` & `flytekit-1.6.2b1/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/task.py` & `flytekit-1.6.2b1/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/types.py` & `flytekit-1.6.2b1/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/models/workflow_closure.py` & `flytekit-1.6.2b1/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/__init__.py` & `flytekit-1.6.2b1/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/backfill.py` & `flytekit-1.6.2b1/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/entities.py` & `flytekit-1.6.2b1/flytekit/remote/entities.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/executions.py` & `flytekit-1.6.2b1/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/lazy_entity.py` & `flytekit-1.6.2b1/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/remote.py` & `flytekit-1.6.2b1/flytekit/remote/remote.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/remote/remote_callable.py` & `flytekit-1.6.2b1/flytekit/remote/remote_callable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/testing/__init__.py` & `flytekit-1.6.2b1/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/fast_registration.py` & `flytekit-1.6.2b1/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/ignore.py` & `flytekit-1.6.2b1/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/module_loader.py` & `flytekit-1.6.2b1/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/repo.py` & `flytekit-1.6.2b1/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/script_mode.py` & `flytekit-1.6.2b1/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/serialize_helpers.py` & `flytekit-1.6.2b1/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/subprocess.py` & `flytekit-1.6.2b1/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/tools/translator.py` & `flytekit-1.6.2b1/flytekit/tools/translator.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/directory/__init__.py` & `flytekit-1.6.2b1/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/directory/types.py` & `flytekit-1.6.2b1/flytekit/types/directory/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/file/__init__.py` & `flytekit-1.6.2b1/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/file/file.py` & `flytekit-1.6.2b1/flytekit/types/file/file.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/numpy/ndarray.py` & `flytekit-1.6.2b1/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/pickle/pickle.py` & `flytekit-1.6.2b1/flytekit/types/pickle/pickle.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/schema/types.py` & `flytekit-1.6.2b1/flytekit/types/schema/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/schema/types_pandas.py` & `flytekit-1.6.2b1/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/structured/__init__.py` & `flytekit-1.6.2b1/flytekit/types/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.6.2b1/flytekit/types/structured/basic_dfs.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/structured/bigquery.py` & `flytekit-1.6.2b1/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.6.2b1/flytekit/types/structured/structured_dataset.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/flytekit.egg-info/PKG-INFO` & `flytekit-1.6.2b1/flytekit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.6.2b0
+Version: 1.6.2b1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.6.2b1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.6.2b0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.6.2b1/flytekit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -104,16 +104,16 @@
 flytekit/exceptions/__init__.py
 flytekit/exceptions/base.py
 flytekit/exceptions/scopes.py
 flytekit/exceptions/system.py
 flytekit/exceptions/user.py
 flytekit/extend/__init__.py
 flytekit/extend/backend/__init__.py
-flytekit/extend/backend/base_plugin.py
-flytekit/extend/backend/external_plugin_service.py
+flytekit/extend/backend/agent_service.py
+flytekit/extend/backend/base_agent.py
 flytekit/extras/__init__.py
 flytekit/extras/cloud_pickle_resolver.py
 flytekit/extras/pytorch/__init__.py
 flytekit/extras/pytorch/checkpoint.py
 flytekit/extras/pytorch/native.py
 flytekit/extras/sklearn/__init__.py
 flytekit/extras/sklearn/native.py
```

### Comparing `flytekit-1.6.2b0/flytekit.egg-info/requires.txt` & `flytekit-1.6.2b1/flytekit.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 googleapis-common-protos>=1.57
-flyteidl>=1.5.6
+flyteidl>=1.5.10
 wheel<1.0.0,>=0.30.0
 pandas<2.0.0,>=1.0.0
 pyarrow<11.0.0,>=4.0.0
 click<9.0,>=6.6
 croniter<4.0.0,>=0.3.20
 deprecated<2.0,>=1.0
 docker<7.0.0,>=4.0.0
```

### Comparing `flytekit-1.6.2b0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.6.2b1/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.6.2b0/setup.py` & `flytekit-1.6.2b1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.6.2b0"
+__version__ = "1.6.2b1"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -25,15 +25,15 @@
             "pyflyte-map-execute=flytekit.bin.entrypoint:map_execute_task_cmd",
             "pyflyte=flytekit.clis.sdk_in_container.pyflyte:main",
             "flyte-cli=flytekit.clis.flyte_cli.main:_flyte_cli",
         ]
     },
     install_requires=[
         "googleapis-common-protos>=1.57",
-        "flyteidl>=1.5.6",
+        "flyteidl>=1.5.10",
         "wheel>=0.30.0,<1.0.0",
         "pandas>=1.0.0,<2.0.0",
         "pyarrow>=4.0.0,<11.0.0",
         "click>=6.6,<9.0",
         "croniter>=0.3.20,<4.0.0",
         "deprecated>=1.0,<2.0",
         "docker>=4.0.0,<7.0.0",
```

