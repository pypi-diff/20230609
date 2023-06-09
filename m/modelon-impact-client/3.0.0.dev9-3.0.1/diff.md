# Comparing `tmp/modelon_impact_client-3.0.0.dev9.tar.gz` & `tmp/modelon_impact_client-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelon_impact_client-3.0.0.dev9.tar", max compression
+gzip compressed data, was "modelon_impact_client-3.0.1.tar", max compression
```

## Comparing `modelon_impact_client-3.0.0.dev9.tar` & `modelon_impact_client-3.0.1.tar`

### file list

```diff
@@ -1,64 +1,81 @@
--rw-r--r--   0        0        0     1477 2023-01-24 18:43:55.104900 modelon_impact_client-3.0.0.dev9/LICENSE.md
--rw-r--r--   0        0        0     2748 2023-01-24 18:43:55.113901 modelon_impact_client-3.0.0.dev9/README.md
--rw-r--r--   0        0        0        0 2023-01-24 18:43:55.079899 modelon_impact_client-3.0.0.dev9/modelon/__init__.py
--rw-r--r--   0        0        0        0 2023-01-24 18:43:55.102900 modelon_impact_client-3.0.0.dev9/modelon/impact/__init__.py
--rw-r--r--   0        0        0      753 2023-01-24 18:43:55.098900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/__init__.py
--rw-r--r--   0        0        0    14534 2023-01-24 18:43:55.083899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/client.py
--rw-r--r--   0        0        0      787 2023-01-24 18:43:55.114901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/configuration.py
--rw-r--r--   0        0        0     1663 2023-01-24 18:43:55.084899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/credential_manager.py
--rw-r--r--   0        0        0      119 2023-01-24 18:43:55.094900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/__init__.py
--rw-r--r--   0        0        0      552 2023-01-24 18:43:55.076899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/asserts.py
--rw-r--r--   0        0        0    16640 2023-01-24 18:43:55.112901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/case.py
--rw-r--r--   0        0        0     5932 2023-01-24 18:43:55.124901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/content.py
--rw-r--r--   0        0        0     6385 2023-01-24 18:43:55.085899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/custom_function.py
--rw-r--r--   0        0        0    11124 2023-01-24 18:43:55.088899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/experiment.py
--rw-r--r--   0        0        0     1838 2023-01-24 18:43:55.076899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/external_result.py
--rw-r--r--   0        0        0      158 2023-01-24 18:43:55.095900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/log.py
--rw-r--r--   0        0        0    11249 2023-01-24 18:43:55.088899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/model.py
--rw-r--r--   0        0        0     8671 2023-01-24 18:43:55.081899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/model_executable.py
--rw-r--r--   0        0        0    10459 2023-01-24 18:43:55.121901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/project.py
--rw-r--r--   0        0        0     1555 2023-01-24 18:43:55.096900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/result.py
--rw-r--r--   0        0        0      775 2023-01-24 18:43:55.067899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/status.py
--rw-r--r--   0        0        0    20394 2023-01-24 18:43:55.117901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/workspace.py
--rw-r--r--   0        0        0     1093 2023-01-24 18:43:55.086899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-01-24 18:43:55.077899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/__init__.py
--rw-r--r--   0        0        0     3602 2023-01-24 18:43:55.130901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/asserts.py
--rw-r--r--   0        0        0    30259 2023-01-24 18:43:55.089899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/base.py
--rw-r--r--   0        0        0     3250 2023-01-24 18:43:55.083899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/expansion.py
--rw-r--r--   0        0        0     9643 2023-01-24 18:43:55.068899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/extension.py
--rw-r--r--   0        0        0     4642 2023-01-24 18:43:55.074899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/operators.py
--rw-r--r--   0        0        0      414 2023-01-24 18:43:55.076899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/util.py
--rw-r--r--   0        0        0       65 2023-01-24 18:43:55.128901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/jupyterhub/__init__.py
--rw-r--r--   0        0        0     1860 2023-01-24 18:43:55.107900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/jupyterhub/authorize.py
--rw-r--r--   0        0        0      281 2023-01-24 18:43:55.133901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/jupyterhub/exceptions.py
--rw-r--r--   0        0        0     2554 2023-01-24 18:43:55.086899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/jupyterhub/sal.py
--rw-r--r--   0        0        0       79 2023-01-24 18:43:55.078899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/__init__.py
--rw-r--r--   0        0        0     5002 2023-01-24 18:43:55.090900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/base.py
--rw-r--r--   0        0        0     2107 2023-01-24 18:43:55.097900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/case.py
--rw-r--r--   0        0        0     2363 2023-01-24 18:43:55.098900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/content_import.py
--rw-r--r--   0        0        0     2039 2023-01-24 18:43:55.077899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/experiment.py
--rw-r--r--   0        0        0     2244 2023-01-24 18:43:55.099900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/external_result.py
--rw-r--r--   0        0        0     5516 2023-01-24 18:43:55.128901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/model_executable.py
--rw-r--r--   0        0        0        0 2023-01-24 18:43:55.081899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/__init__.py
--rw-r--r--   0        0        0     2397 2023-01-24 18:43:55.129901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/conversion.py
--rw-r--r--   0        0        0     3081 2023-01-24 18:43:55.130901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/exports.py
--rw-r--r--   0        0        0     2464 2023-01-24 18:43:55.108900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/imports.py
--rw-r--r--   0        0        0     3397 2023-01-24 18:43:55.115901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/options.py
--rw-r--r--   0        0        0        0 2023-01-24 18:43:55.105900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/__init__.py
--rw-r--r--   0        0        0      123 2023-01-24 18:43:55.102900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/context.py
--rw-r--r--   0        0        0     1413 2023-01-24 18:43:55.091899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/custom_function.py
--rw-r--r--   0        0        0      723 2023-01-24 18:43:55.066898 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/exceptions.py
--rw-r--r--   0        0        0     5739 2023-01-24 18:43:55.108900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/experiment.py
--rw-r--r--   0        0        0      419 2023-01-24 18:43:55.084899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/export.py
--rw-r--r--   0        0        0     2715 2023-01-24 18:43:55.100900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/http.py
--rw-r--r--   0        0        0     2706 2023-01-24 18:43:55.115901 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/model_executable.py
--rw-r--r--   0        0        0     4023 2023-01-24 18:43:55.109900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/project.py
--rw-r--r--   0        0        0     3560 2023-01-24 18:43:55.085899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/request.py
--rw-r--r--   0        0        0     4509 2023-01-24 18:43:55.097900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/response.py
--rw-r--r--   0        0        0     3644 2023-01-24 18:43:55.077899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/service.py
--rw-r--r--   0        0        0      770 2023-01-24 18:43:55.069899 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/uri.py
--rw-r--r--   0        0        0      405 2023-01-24 18:43:55.094900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/users.py
--rw-r--r--   0        0        0     7467 2023-01-24 18:43:55.092900 modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/workspace.py
--rw-r--r--   0        0        0      970 2023-01-24 18:47:18.216913 modelon_impact_client-3.0.0.dev9/pyproject.toml
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 modelon_impact_client-3.0.0.dev9/setup.py
--rw-r--r--   0        0        0     3785 1970-01-01 00:00:00.000000 modelon_impact_client-3.0.0.dev9/PKG-INFO
+-rw-r--r--   0        0        0     1479 2023-06-09 06:58:12.992848 modelon_impact_client-3.0.1/LICENSE.md
+-rw-r--r--   0        0        0     2748 2023-06-09 06:58:12.999848 modelon_impact_client-3.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.954847 modelon_impact_client-3.0.1/modelon/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.988847 modelon_impact_client-3.0.1/modelon/impact/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-09 06:58:12.981847 modelon_impact_client-3.0.1/modelon/impact/client/__init__.py
+-rw-r--r--   0        0        0    24886 2023-06-09 06:58:12.957847 modelon_impact_client-3.0.1/modelon/impact/client/client.py
+-rw-r--r--   0        0        0      835 2023-06-09 06:58:13.000847 modelon_impact_client-3.0.1/modelon/impact/client/configuration.py
+-rw-r--r--   0        0        0     1938 2023-06-09 06:58:12.958847 modelon_impact_client-3.0.1/modelon/impact/client/credential_manager.py
+-rw-r--r--   0        0        0      119 2023-06-09 06:58:12.969847 modelon_impact_client-3.0.1/modelon/impact/client/entities/__init__.py
+-rw-r--r--   0        0        0      639 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/entities/asserts.py
+-rw-r--r--   0        0        0    24767 2023-06-09 06:58:12.999848 modelon_impact_client-3.0.1/modelon/impact/client/entities/case.py
+-rw-r--r--   0        0        0     2259 2023-06-09 06:58:13.010848 modelon_impact_client-3.0.1/modelon/impact/client/entities/content.py
+-rw-r--r--   0        0        0     6620 2023-06-09 06:58:12.959847 modelon_impact_client-3.0.1/modelon/impact/client/entities/custom_function.py
+-rw-r--r--   0        0        0    18419 2023-06-09 06:58:12.961847 modelon_impact_client-3.0.1/modelon/impact/client/entities/experiment.py
+-rw-r--r--   0        0        0     2511 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/entities/external_result.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:13.009848 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-09 06:58:12.948847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/case.py
+-rw-r--r--   0        0        0      200 2023-06-09 06:58:12.987847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/custom_function.py
+-rw-r--r--   0        0        0      366 2023-06-09 06:58:12.976847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/experiment.py
+-rw-r--r--   0        0        0      192 2023-06-09 06:58:12.982847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/external_result.py
+-rw-r--r--   0        0        0      186 2023-06-09 06:58:12.978847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/model.py
+-rw-r--r--   0        0        0      190 2023-06-09 06:58:12.969847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/model_executable.py
+-rw-r--r--   0        0        0      190 2023-06-09 06:58:12.953847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/workspace.py
+-rw-r--r--   0        0        0      156 2023-06-09 06:58:12.972847 modelon_impact_client-3.0.1/modelon/impact/client/entities/log.py
+-rw-r--r--   0        0        0    16840 2023-06-09 06:58:12.962847 modelon_impact_client-3.0.1/modelon/impact/client/entities/model.py
+-rw-r--r--   0        0        0    12110 2023-06-09 06:58:12.956847 modelon_impact_client-3.0.1/modelon/impact/client/entities/model_executable.py
+-rw-r--r--   0        0        0    12288 2023-06-09 06:58:13.007848 modelon_impact_client-3.0.1/modelon/impact/client/entities/project.py
+-rw-r--r--   0        0        0     1986 2023-06-09 06:58:12.977847 modelon_impact_client-3.0.1/modelon/impact/client/entities/result.py
+-rw-r--r--   0        0        0     1487 2023-06-09 06:58:12.948847 modelon_impact_client-3.0.1/modelon/impact/client/entities/status.py
+-rw-r--r--   0        0        0    20712 2023-06-09 06:58:13.004848 modelon_impact_client-3.0.1/modelon/impact/client/entities/workspace.py
+-rw-r--r--   0        0        0     1365 2023-06-09 06:58:12.959847 modelon_impact_client-3.0.1/modelon/impact/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/__init__.py
+-rw-r--r--   0        0        0     5284 2023-06-09 06:58:13.015848 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/asserts.py
+-rw-r--r--   0        0        0     3085 2023-06-09 06:58:12.957847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/expansion.py
+-rw-r--r--   0        0        0    10251 2023-06-09 06:58:12.949847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/extension.py
+-rw-r--r--   0        0        0    12659 2023-06-09 06:58:12.995848 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/fmu_based.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.990847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/__init__.py
+-rw-r--r--   0        0        0      506 2023-06-09 06:58:12.958847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/definition.py
+-rw-r--r--   0        0        0      409 2023-06-09 06:58:12.959847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/expansion.py
+-rw-r--r--   0        0        0      187 2023-06-09 06:58:12.945847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/extension.py
+-rw-r--r--   0        0        0    18576 2023-06-09 06:58:12.963847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/model_based.py
+-rw-r--r--   0        0        0     4704 2023-06-09 06:58:12.951847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/operators.py
+-rw-r--r--   0        0        0      641 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/util.py
+-rw-r--r--   0        0        0       65 2023-06-09 06:58:13.013848 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/__init__.py
+-rw-r--r--   0        0        0     3019 2023-06-09 06:58:12.994847 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/authorize.py
+-rw-r--r--   0        0        0      281 2023-06-09 06:58:13.018848 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/exceptions.py
+-rw-r--r--   0        0        0     2894 2023-06-09 06:58:12.960847 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/sal.py
+-rw-r--r--   0        0        0       79 2023-06-09 06:58:12.953847 modelon_impact_client-3.0.1/modelon/impact/client/operations/__init__.py
+-rw-r--r--   0        0        0     5804 2023-06-09 06:58:12.964847 modelon_impact_client-3.0.1/modelon/impact/client/operations/base.py
+-rw-r--r--   0        0        0     2439 2023-06-09 06:58:12.979847 modelon_impact_client-3.0.1/modelon/impact/client/operations/case.py
+-rw-r--r--   0        0        0     2502 2023-06-09 06:58:12.980847 modelon_impact_client-3.0.1/modelon/impact/client/operations/content_import.py
+-rw-r--r--   0        0        0     2243 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/operations/experiment.py
+-rw-r--r--   0        0        0     2408 2023-06-09 06:58:12.983847 modelon_impact_client-3.0.1/modelon/impact/client/operations/external_result_import.py
+-rw-r--r--   0        0        0     2719 2023-06-09 06:58:12.972847 modelon_impact_client-3.0.1/modelon/impact/client/operations/fmu_import.py
+-rw-r--r--   0        0        0     5845 2023-06-09 06:58:13.014848 modelon_impact_client-3.0.1/modelon/impact/client/operations/model_executable.py
+-rw-r--r--   0        0        0     2629 2023-06-09 06:58:13.024848 modelon_impact_client-3.0.1/modelon/impact/client/operations/project_import.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.956847 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-09 06:58:13.014848 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/conversion.py
+-rw-r--r--   0        0        0     3512 2023-06-09 06:58:13.015848 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/exports.py
+-rw-r--r--   0        0        0     2532 2023-06-09 06:58:12.996847 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/imports.py
+-rw-r--r--   0        0        0     3772 2023-06-09 06:58:13.001848 modelon_impact_client-3.0.1/modelon/impact/client/options.py
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.948847 modelon_impact_client-3.0.1/modelon/impact/client/py.typed
+-rw-r--r--   0        0        0        0 2023-06-09 06:58:12.993847 modelon_impact_client-3.0.1/modelon/impact/client/sal/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-09 06:58:12.989848 modelon_impact_client-3.0.1/modelon/impact/client/sal/context.py
+-rw-r--r--   0        0        0     1543 2023-06-09 06:58:12.965847 modelon_impact_client-3.0.1/modelon/impact/client/sal/custom_function.py
+-rw-r--r--   0        0        0      671 2023-06-09 06:58:12.947847 modelon_impact_client-3.0.1/modelon/impact/client/sal/exceptions.py
+-rw-r--r--   0        0        0     6785 2023-06-09 06:58:12.996847 modelon_impact_client-3.0.1/modelon/impact/client/sal/experiment.py
+-rw-r--r--   0        0        0      629 2023-06-09 06:58:12.957847 modelon_impact_client-3.0.1/modelon/impact/client/sal/exports.py
+-rw-r--r--   0        0        0     1475 2023-06-09 06:58:13.018848 modelon_impact_client-3.0.1/modelon/impact/client/sal/external_result.py
+-rw-r--r--   0        0        0     3124 2023-06-09 06:58:12.985847 modelon_impact_client-3.0.1/modelon/impact/client/sal/http.py
+-rw-r--r--   0        0        0      475 2023-06-09 06:58:13.023848 modelon_impact_client-3.0.1/modelon/impact/client/sal/imports.py
+-rw-r--r--   0        0        0     3083 2023-06-09 06:58:13.001848 modelon_impact_client-3.0.1/modelon/impact/client/sal/model_executable.py
+-rw-r--r--   0        0        0     4640 2023-06-09 06:58:12.996847 modelon_impact_client-3.0.1/modelon/impact/client/sal/project.py
+-rw-r--r--   0        0        0     4877 2023-06-09 06:58:12.958847 modelon_impact_client-3.0.1/modelon/impact/client/sal/request.py
+-rw-r--r--   0        0        0     5113 2023-06-09 06:58:12.978847 modelon_impact_client-3.0.1/modelon/impact/client/sal/response.py
+-rw-r--r--   0        0        0     5082 2023-06-09 06:58:12.953847 modelon_impact_client-3.0.1/modelon/impact/client/sal/service.py
+-rw-r--r--   0        0        0      884 2023-06-09 06:58:12.949847 modelon_impact_client-3.0.1/modelon/impact/client/sal/uri.py
+-rw-r--r--   0        0        0      453 2023-06-09 06:58:12.967847 modelon_impact_client-3.0.1/modelon/impact/client/sal/users.py
+-rw-r--r--   0        0        0     6995 2023-06-09 06:58:12.965847 modelon_impact_client-3.0.1/modelon/impact/client/sal/workspace.py
+-rw-r--r--   0        0        0     1359 2023-06-09 06:59:15.194490 modelon_impact_client-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.0.1/PKG-INFO
```

### Comparing `modelon_impact_client-3.0.0.dev9/LICENSE.md` & `modelon_impact_client-3.0.1/LICENSE.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Copyright 2020 Modelon AB
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
- 1. Redistributions of source code must retain the above copyright
+ 1. Re-distributions of source code must retain the above copyright
     notice, this list of conditions and the following disclaimer.
 
- 2. Redistributions in binary form must reproduce the above copyright
+ 2. Re-distributions in binary form must reproduce the above copyright
     notice, this list of conditions and the following disclaimer in the
     documentation and/or other materials provided with the distribution.
 
  3. Neither the name of the copyright holder nor the names of its
     contributors may be used to endorse or promote products derived from
     this software without specific prior written permission.
```

### Comparing `modelon_impact_client-3.0.0.dev9/README.md` & `modelon_impact_client-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/__init__.py` & `modelon_impact_client-3.0.1/modelon/impact/client/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from modelon.impact.client.client import Client
-from modelon.impact.client.experiment_definition.base import (
+from modelon.impact.client.experiment_definition.fmu_based import (
     SimpleFMUExperimentDefinition,
+)
+from modelon.impact.client.experiment_definition.model_based import (
     SimpleModelicaExperimentDefinition,
 )
 from modelon.impact.client.experiment_definition.extension import (
     SimpleExperimentExtension,
 )
 from modelon.impact.client.experiment_definition.operators import (
     Range,
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/configuration.py` & `modelon_impact_client-3.0.1/modelon/impact/client/configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import os
 import logging
 
 
 logger = logging.getLogger(__name__)
 
 
-def get_client_url():
-    """Returns the default URL the client will use if unspecified. Can be overridden
-    by the environment variable MODELON_IMPACT_CLIENT_URL."""
+def get_client_url() -> str:
+    """Returns the default URL the client will use if unspecified.
+
+    Can be overridden by the environment variable
+    MODELON_IMPACT_CLIENT_URL.
+
+    """
     url = os.environ.get("MODELON_IMPACT_CLIENT_URL")
     if url is None:
-        url = "http://localhost:8080/"
+        url = "https://impact.modelon.cloud/"
         logger.warning("No URL for client was specified, will use: {}".format(url))
     return url
 
 
-def get_client_interactive():
-    """Returns the default for if client will run interactive or not if unspecified.
-    Can be overridden by the environment variable MODELON_IMPACT_CLIENT_INTERACTIVE."""
+def get_client_interactive() -> bool:
+    """Returns the default for if client will run interactive or not if
+    unspecified.
+
+    Can be overridden by the environment variable
+    MODELON_IMPACT_CLIENT_INTERACTIVE.
+
+    """
     interactive_env = os.environ.get("MODELON_IMPACT_CLIENT_INTERACTIVE", "false")
     return interactive_env.lower() in ("1", "true")
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/case.py` & `modelon_impact_client-3.0.1/modelon/impact/client/entities/experiment.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,546 +1,574 @@
+from __future__ import annotations
 import logging
-from datetime import datetime
-from typing import Any, Dict, Tuple, Optional
-from modelon.impact.client.sal.service import Service
-from modelon.impact.client.sal.experiment import ResultFormat
-from modelon.impact.client.operations.case import CaseOperation
-from modelon.impact.client.entities.external_result import ExternalResult
-from modelon.impact.client.entities.log import Log
-from modelon.impact.client.entities.result import Result
-import modelon.impact.client.entities.model_executable
-from modelon.impact.client.entities.status import CaseStatus
-from modelon.impact.client.entities.asserts import assert_successful_operation
+import enum
+from typing import Any, List, Dict, Optional, Union, TYPE_CHECKING
+
+from modelon.impact.client.entities.interfaces.experiment import ExperimentInterface
+from modelon.impact.client.operations import experiment
+from modelon.impact.client.entities.case import Case
+from modelon.impact.client.entities.asserts import assert_variable_in_result
+from modelon.impact.client.entities.status import ExperimentStatus
+from modelon.impact.client.options import (
+    CompilerOptions,
+    SimulationOptions,
+    RuntimeOptions,
+    SolverOptions,
+)
 from modelon.impact.client import exceptions
 
-logger = logging.getLogger(__name__)
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import BaseOperation
 
+logger = logging.getLogger(__name__)
 
-def _assert_case_is_complete(status, operation_name="Operation"):
-    if status == CaseStatus.NOT_STARTED:
-        raise exceptions.OperationNotCompleteError.for_operation(operation_name, status)
-    elif status == CaseStatus.CANCELLED:
-        raise exceptions.OperationFailureError.for_operation(operation_name)
+ScalarValue = Union[float, int, str]
 
 
-def _datetime_from_unix_time(unix_time: Optional[int]):
-    if unix_time:
-        return datetime.fromtimestamp(unix_time / 1e3)
+@enum.unique
+class _TrajectoryResponseFormat(enum.Enum):
+    V1 = "application/vnd.impact.trajectories.v1+json"
+    V2 = "application/vnd.impact.trajectories.v2+json"
 
 
-class _CaseRunInfo:
-    """
-    Class containing Case run info.
-    """
+class ExperimentResultPoint:
+    """Value class with the single time instance data in a experiment."""
 
-    def __init__(
-        self,
-        status: CaseStatus,
-        consistent: bool,
-        datetime_started: Optional[datetime],
-        datetime_finished: Optional[datetime],
-    ):
-        self._status = status
-        self._consistent = consistent
-        self._datetime_started = datetime_started
-        self._datetime_finished = datetime_finished
+    def __init__(self, trajectories: List[Dict[str, Any]], variables: List[str]):
+        self._trajectories = trajectories
+        self._variables = variables
 
     @property
-    def status(self) -> CaseStatus:
-        """Status info for a Case, its type is CaseStatus."""
-        return self._status
+    def variables(self) -> List[str]:
+        """List of variables."""
+        return self._variables
 
     @property
-    def consistent(self) -> bool:
-        """True if the case has not been synced since it was executed,
-        false otherwise."""
-        return self._consistent
+    def cases(self) -> List[str]:
+        """List of case ids."""
+        return [case["caseId"] for case in self._trajectories]
 
-    @property
-    def started(self):
-        """
-        Case execution start time. Returns None if case execution hasn't started.
-        """
-        return self._datetime_started
+    def as_lists(self) -> List[Optional[List[Optional[ScalarValue]]]]:
+        """Return a list of results per case.
 
-    @property
-    def finished(self):
-        """
-        Case execution finish time. Returns None if case execution hasn't finished.
-        """
-        return self._datetime_finished
+        None indicates that the case was not run or failed. None value
+        for a variable indicated that the variable is not present in the
+        specific case output.
 
+        Example::
 
-class _CaseAnalysis:
-    """
-    Class containing Case analysis configuration.
-    """
+            result_data = result.as_lists()
 
-    def __init__(self, analysis: Dict[str, Any]):
-        self._analysis = analysis
+        """
+        return [
+            [item["trajectory"][0] if item else None for item in case_data["items"]]
+            for case_data in self._trajectories
+        ]
 
-    @property
-    def analysis_function(self) -> str:
-        """The name of the custom function"""
-        return self._analysis['analysis_function']
 
-    @property
-    def parameters(self) -> Dict[str, Any]:
-        """Parameters to the custom function
+@enum.unique
+class _Workflow(enum.Enum):
+    """Workflow type."""
 
-        Example::
-            {
-                "start_time": 0,
-                "final_time": 1
-            }
-        """
-        return self._analysis['parameters']
+    FMU_BASED = 'FMU_BASED'
+    CLASS_BASED = 'CLASS_BASED'
 
-    @parameters.setter
-    def parameters(self, parameters: Dict[str, Any]):
-        self._analysis['parameters'] = parameters
 
-    @property
-    def simulation_options(self) -> Dict[str, Any]:
-        """Key-value pairs of simulation options"""
-        return self._analysis['simulation_options']
+def _assert_experiment_is_complete(
+    status: ExperimentStatus, operation_name: str = "Operation"
+) -> None:
+    if status == ExperimentStatus.NOTSTARTED:
+        raise exceptions.OperationNotCompleteError.for_operation(operation_name, status)
+    elif status == ExperimentStatus.CANCELLED:
+        raise exceptions.OperationFailureError.for_operation(operation_name)
 
-    @simulation_options.setter
-    def simulation_options(self, simulation_options: Dict[str, Any]):
-        self._analysis['simulation_options'] = simulation_options
 
-    @property
-    def solver_options(self) -> Dict[str, Any]:
-        """Key-value pairs of solver options"""
-        return self._analysis['solver_options']
+class ExperimentRunInfo:
+    """Class containing experiment run information."""
 
-    @solver_options.setter
-    def solver_options(self, solver_options: Dict[str, Any]):
-        self._analysis['solver_options'] = solver_options
+    def __init__(
+        self,
+        status: ExperimentStatus,
+        errors: List[str],
+        failed: int,
+        successful: int,
+        cancelled: int,
+        not_started: int,
+    ):
+        self._status = status
+        self._errors = errors
+        self._failed = failed
+        self._successful = successful
+        self._cancelled = cancelled
+        self._not_started = not_started
 
     @property
-    def simulation_log_level(self) -> str:
-        """The simulation log level"""
-        return self._analysis['simulation_log_level']
+    def status(self) -> ExperimentStatus:
+        """Status info for an Experiment.
+
+        .. Note:: For tracing status changes of a running experiment execution,
+            the ExperimentOperation status property must be used and not
+            Experiment entities run info(ExperimentRunInfo) status property. See
+            example for usage.
 
-    @simulation_log_level.setter
-    def simulation_log_level(self, simulation_log_level: str):
-        self._analysis['simulation_log_level'] = simulation_log_level
+        Example::
 
+            # To get the case entity run info status
+            status = experiment.run_info.status
 
-class _CaseMeta:
-    """
-    Class containing Case meta
-    """
+            # To get the status updates of a running experiment execution
+            experiment_ops = experiment.execute()
+            status = experiment_ops.status
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
+        """
+        return self._status
 
     @property
-    def label(self) -> str:
-        """Label for the case."""
-        return self._data['label']
+    def errors(self) -> List[str]:
+        """A list of errors.
 
-    @label.setter
-    def label(self, label: str):
-        self._data['label'] = label
+        Is empty unless 'status' attribute is 'FAILED'
 
+        """
+        return self._errors
 
-class _CaseInput:
-    """
-    Class containing Case input
-    """
+    @property
+    def successful(self) -> int:
+        """Number of cases in experiment that are successful."""
+        return self._successful
 
-    def __init__(self, data: Dict[str, Any]):
-        self._data = data
+    @property
+    def failed(self) -> int:
+        """Number of cases in experiment thar have failed."""
+        return self._failed
 
     @property
-    def analysis(self) -> _CaseAnalysis:
-        return _CaseAnalysis(self._data['analysis'])
+    def cancelled(self) -> int:
+        """Number of cases in experiment that are cancelled."""
+        return self._cancelled
 
     @property
-    def parametrization(self) -> Dict[str, Any]:
-        """
-        Parameterization of the case, a list of key value pairs where key
-        is variable name and value is the value to use for that variable.
-        """
-        return self._data['parametrization']
+    def not_started(self) -> int:
+        """Number of cases in experiment that have not yet started."""
+        return self._not_started
 
-    @parametrization.setter
-    def parametrization(self, parameterization: Dict[str, Any]):
-        self._data['parametrization'] = parameterization
 
-    @property
-    def fmu_id(self) -> str:
-        """Reference ID to the compiled model used running the case."""
-        return self._data['fmu_id']
+class ExperimentMetaData:
+    """Class containing experiment metadata."""
+
+    def __init__(self, meta_data: Dict[str, Any]):
+        self._meta_data = meta_data
 
     @property
-    def structural_parametrization(self) -> Dict[str, Any]:
-        """
-        Structural parameterization of the case, a list of key value pairs where
-        key is variable name and value is the value to use for that variable.
-        These are values that cannot be applied to the FMU/Model after compilation.
-        """
-        return self._data['structural_parametrization']
+    def user_data(self) -> Dict[str, Any]:
+        """User data dictionary object attached to experiment, if any."""
+        return self._meta_data.get("user_data", {})
 
     @property
-    def fmu_base_parametrization(self) -> Dict[str, Any]:
-        """
-        This is some base parametrization that must be applied to the FMU for
-        it to be valid running this case. It often comes as a result from of
-        caching to reuse the FMU.
-        """
-        return self._data['fmu_base_parametrization']
+    def label(self) -> Optional[str]:
+        """Experiment label."""
+        return self._meta_data.get("label")
 
 
-class Case:
-    """
-    Class containing Case functionalities.
-    """
+class Experiment(ExperimentInterface):
+    """Class containing Experiment functionalities."""
 
     def __init__(
         self,
-        case_id: str,
         workspace_id: str,
         exp_id: str,
         service: Service,
-        info: Dict[str, Any],
+        info: Optional[Dict[str, Any]] = None,
     ):
-        self._case_id = case_id
-        self._workspace_id = workspace_id
         self._exp_id = exp_id
+        self._workspace_id = workspace_id
         self._sal = service
         self._info = info
+        self._fmu_info: Optional[Dict[str, Any]] = None
 
-    def __repr__(self):
-        return f"Case with id '{self._case_id}'"
+    def __eq__(self, obj: object) -> bool:
+        return isinstance(obj, Experiment) and obj._exp_id == self._exp_id
 
-    def __eq__(self, obj):
-        return isinstance(obj, Case) and obj._case_id == self._case_id
+    def __repr__(self) -> str:
+        return f"Experiment with id '{self._exp_id}'"
 
     @property
     def id(self) -> str:
-        """Case id"""
-        return self._case_id
-
-    @property
-    def experiment_id(self) -> str:
-        """Experiment id"""
+        """Experiment id."""
         return self._exp_id
 
-    @property
-    def info(self) -> Dict[str, Any]:
-        """Deprecated, use 'run_info' attribute"""
-        logger.warning("This attribute is deprectated, use 'run_info' instead")
+    def _get_info(self, cached: bool = True) -> Dict[str, Any]:
+        if not cached or self._info is None:
+            self._info = self._sal.workspace.experiment_get(
+                self._workspace_id, self._exp_id
+            )
+
         return self._info
 
     @property
-    def run_info(self) -> _CaseRunInfo:
-        """Case run information"""
-        run_info = self._info["run_info"]
-        started = _datetime_from_unix_time(run_info.get("datetime_started"))
-        finished = _datetime_from_unix_time(run_info.get("datetime_finished"))
-        return _CaseRunInfo(
-            CaseStatus(run_info["status"]), run_info["consistent"], started, finished
-        )
+    def run_info(self) -> ExperimentRunInfo:
+        """Experiment run information.
 
-    @property
-    def input(self) -> _CaseInput:
-        """Case input attributes
+        Returns:
+            A ExperimentRunInfo class object.
 
         Example::
 
-         case.input.analysis.parameters = {'start_time': 0, 'final_time': 90}
-         case.input.analysis.simulation_options = {'ncp': 600}
-         case.input.analysis.solver_options = {'atol': 1e-8}
-         case.input.parametrization = {'PI.k': 120}
-         case.sync()
+            status = experiment.run_info.status
 
-         help(case.input.analysis) # See help for attribute
-         dir(case.input) # See nested attributes
         """
-        return _CaseInput(self._info['input'])
+        run_info = self._get_info(cached=False)["run_info"]
+
+        status = ExperimentStatus(run_info["status"])
+        errors = run_info.get("errors", [])
+        failed = run_info.get("failed", 0)
+        successful = run_info.get("successful", 0)
+        cancelled = run_info.get("cancelled", 0)
+        not_started = run_info.get("not_started", 0)
+        return ExperimentRunInfo(
+            status, errors, failed, successful, cancelled, not_started
+        )
 
     @property
-    def meta(self) -> _CaseMeta:
-        """Case meta attributes
+    def metadata(self) -> ExperimentMetaData:
+        """Experiment metadata.
+
+        Returns:
+            A ExperimentMetaData class object.
 
         Example::
 
-         case.meta.label = 'Cruise condition'
-         case.sync()
+            user_data = experiment.metadata.user_data
 
-         help(case.meta) # See help for attribute
-         dir(case.input) # See nested attributes
         """
-        return _CaseMeta(self._info['meta'])
 
-    @property
-    def initialize_from_case(self) -> Optional['Case']:
-        init_from_dict = self._info['input'].get('initialize_from_case')
-        if init_from_dict is None:
-            return None
+        info = self._get_info(cached=False)
+        meta_data = info.get("meta_data", {})
+        return ExperimentMetaData(meta_data)
 
-        experiment_id = init_from_dict.get('experimentId')
-        case_id = init_from_dict.get('caseId')
+    @property
+    def info(self) -> Dict[str, Any]:
+        """Deprecated, use 'run_info' attribute."""
+        logger.warning("This attribute is deprectated, use 'run_info' instead")
+        return self._get_info(cached=False)
 
-        case_data = self._sal.experiment.case_get(
-            self._workspace_id, experiment_id, case_id
-        )
-        return Case(
-            case_data["id"], self._workspace_id, experiment_id, self._sal, case_data
-        )
+    def execute(
+        self, with_cases: Optional[List[Case]] = None, sync_case_changes: bool = True
+    ) -> experiment.ExperimentOperation:
+        """Executes an experiment. Returns an ExperimentOperation class object.
+
+        Args:
+            with_cases: A list of cases objects to execute.
+            sync_case_changes: Boolean specifying if to sync the cases given with the
+                'with_cases' argument against the server before executing the
+                experiment. Default is True.
 
-    @initialize_from_case.setter
-    def initialize_from_case(self, case: 'Case'):
-        if not isinstance(case, Case):
-            raise TypeError(
-                "The value must be an instance of modelon.impact.client.entities."
-                "case.Case"
-            )
-        self._assert_unique_case_initialization('initialize_from_external_result')
-        self._info['input']['initialize_from_case'] = {
-            'experimentId': case.experiment_id,
-            'caseId': case.id,
-        }
+        Returns:
+            An ExperimentOperation class object.
 
-    @property
-    def initialize_from_external_result(self) -> Optional[ExternalResult]:
-        init_from_dict = self._info['input'].get('initialize_from_external_result')
+        Example::
 
-        if init_from_dict is None:
-            return None
+            experiment = workspace.create_experiment(experiment_definition)
+            experiment_ops = experiment.execute()
+            experiment_ops.cancel()
+            experiment_ops.status
+            experiment_ops.wait()
 
-        result_id = init_from_dict.get('uploadId')
+            generate_cases = experiment.execute(with_cases=[]).wait()
+            cases_to_execute =  generate_cases.get_case('case_2')
+            experiment = experiment.execute(with_cases=[cases_to_execute]).wait()
 
-        return ExternalResult(result_id, self._sal)
+        """
+        if sync_case_changes and with_cases is not None:
+            for case in with_cases:
+                case.sync()
 
-    @initialize_from_external_result.setter
-    def initialize_from_external_result(self, result: ExternalResult):
-        if not isinstance(result, ExternalResult):
-            raise TypeError(
-                "The value must be an instance of "
-                "modelon.impact.client.entities.external_result.ExternalResult"
-            )
-        self._assert_unique_case_initialization('initialize_from_case')
-        self._info['input']['initialize_from_external_result'] = {"uploadId": result.id}
+        case_ids = [case.id for case in with_cases] if with_cases is not None else None
+        return experiment.ExperimentOperation[Experiment](
+            self._workspace_id,
+            self._sal.experiment.experiment_execute(
+                self._workspace_id, self._exp_id, case_ids
+            ),
+            self._sal,
+            Experiment.from_operation,
+        )
 
     def is_successful(self) -> bool:
-        """
-        Returns True if a case has completed successfully.
+        """Returns True if the Experiment is done and no cases has failed. Use
+        the 'run_info' attribute to get more info.
 
         Returns:
-
-            True -> If the case has executed successfully.
-            False -> If the case has failed execution.
+            True, if execution process has completed successfully. False, if
+            execution process has failed, is cancelled or still running.
 
         Example::
 
-            case.is_successful()
-        """
-        return self.run_info.status == CaseStatus.SUCCESSFUL
+            experiment.is_successful()
 
-    def get_log(self) -> Log:
         """
-        Returns the log class object for a finished case.
+        return (
+            self.run_info.status == ExperimentStatus.DONE
+            and self.run_info.failed == 0
+            and self.run_info.cancelled == 0
+        )
+
+    def get_variables(self) -> List[str]:
+        """Returns a list of variables available in the result.
 
         Returns:
+            An list of result variables.
 
-            log --
-                The case execution log class object.
+        Raises:
+            OperationNotCompleteError if simulation process is in progress.
+            OperationFailureError if simulation process has failed or was cancelled.
 
         Example::
 
-            log = case.get_log()
-            log.show()
+            experiment.get_variables()
+
         """
-        return Log(
-            self._sal.experiment.case_get_log(
-                self._workspace_id, self._exp_id, self._case_id
-            )
+        _assert_experiment_is_complete(self.run_info.status, "Simulation")
+        return self._sal.experiment.result_variables_get(
+            self._workspace_id, self._exp_id
         )
 
-    def get_result(self, format: str = 'mat') -> Tuple[bytes, str]:
-        """
-        Returns the result stream and the file name for a finished case.
+    def get_cases(self) -> List[Case]:
+        """Returns a list of case objects for an experiment.
 
-        Parameters:
+        Returns:
+            An list of case objects.
 
-            format --
-                The file format to download the result in. The only possible values
-                are 'mat' and 'csv'.
-                Default: 'mat'
+        Example::
 
-        Returns:
+            experiment.get_cases()
 
-            result --
-                The result byte stream.
+        """
+        resp = self._sal.experiment.cases_get(self._workspace_id, self._exp_id)
+        return [
+            Case(case["id"], self._workspace_id, self._exp_id, self._sal, case)
+            for case in resp["data"]["items"]
+        ]
 
-            filename --
-                The filename for the result. This name could be used to write the
-                result stream.
+    def get_case(self, case_id: str) -> Case:
+        """Returns a case object for a given case_id.
 
-        Raises:
+        Args:
+            case_id: The case_id for the case.
 
-            OperationNotCompleteError if simulation process is in progress.
-            OperationFailureError if simulation process has failed or was cancelled.
-            TypeError if the variable is not a list object.
-            ValueError if trajectory variable is not present in the result.
+        Returns:
+            An case object.
 
         Example::
 
-            result, file_name = case.get_result(format = 'csv')
-            with open(file_name, "w") as f:
-                f.write(result)
-        """
-        assert_successful_operation(self.is_successful(), self._case_id)
-        result_format = ResultFormat(format)
-        result, file_name = self._sal.experiment.case_result_get(
-            self._workspace_id, self._exp_id, self._case_id, result_format
-        )
-        return result, file_name
+            experiment.get_case('case_1')
 
-    def get_trajectories(self) -> Result:
         """
-        Returns result(Mapping) object containing the result trajectories.
-
-        Returns:
+        case_data = self._sal.experiment.case_get(
+            self._workspace_id, self._exp_id, case_id
+        )
+        return Case(
+            case_data["id"], self._workspace_id, self._exp_id, self._sal, case_data
+        )
 
-            trajectories --
-                A result trajectory dictionary object.
+    def get_cases_with_label(self, case_label: str) -> List[Case]:
+        """Returns a list of case objects for an experiment with the label.
 
-        Raises:
+        Args:
+            case_label: The case_label for the case.
 
-            OperationNotCompleteError if simulation process is in progress.
-            OperationFailureError if simulation process was cancelled.
+        Returns:
+            An list of case objects.
 
         Example::
 
-            result = case.get_trajectories()
-            result_variables = result.keys()
-            height = result['h']
-            time = res['time']
-        """
-        _assert_case_is_complete(self.run_info.status, "Simulation")
-        return Result(
-            self._sal.experiment.result_variables_get(self._workspace_id, self._exp_id),
-            self._case_id,
-            self._workspace_id,
-            self._exp_id,
-            self._sal,
-        )
+            experiment.get_cases_with_label('Cruise condition')
 
-    def get_artifact(self, artifact_id: str) -> Tuple[bytes, str]:
         """
-        Returns the artifact stream and the file name for a finished case.
+        return [case for case in self.get_cases() if case.meta.label == case_label]
 
-        Parameters:
+    def _validate_and_fetch_trajectories(
+        self,
+        variables: List[str],
+        only_last_point: bool = False,
+        format: _TrajectoryResponseFormat = _TrajectoryResponseFormat.V1,
+    ) -> Any:
+        if not isinstance(variables, list):
+            raise TypeError(
+                "Please specify the list of result keys for the trajectories of "
+                "intrest!"
+            )
+        _assert_experiment_is_complete(self.run_info.status, "Simulation")
+        assert_variable_in_result(variables, self.get_variables())
 
-            artifact_id --
-                The ID of the artifact.
+        return self._sal.experiment.trajectories_get(
+            self._workspace_id, self._exp_id, variables, only_last_point, format.value
+        )
 
-        Returns:
+    def get_trajectories(self, variables: List[str]) -> Dict[str, Any]:
+        """Returns a dictionary containing the result trajectories for a list
+        of result variables for all the cases.
 
-            artifact --
-                The artifact byte stream.
+        Args:
+            variables: A list of result variables to fecth trajectories for.
 
-            filename --
-                The filename for the artifact. This name could be used to write the
-                artifact stream.
+        Returns:
+            A dictionary object containing the result trajectories for all cases.
 
         Raises:
-
             OperationNotCompleteError if simulation process is in progress.
-            OperationFailureError if simulation process has failed or was cancelled.
+            OperationFailureError if simulation process was cancelled.
+            TypeError if the variable is not a list object.
+            ValueError if trajectory variable is not present in the result.
 
         Example::
 
-            result, file_name = case.get_artifact("ABCD")
-            with open(file_name, "wb") as f:
-                f.write(result)
+            result = experiment.get_trajectories(['h', 'time'])
+            height = result['case_1']['h']
+            time = result['case_1']['time']
+
         """
-        assert_successful_operation(self.is_successful(), self._case_id)
-        result, file_name = self._sal.experiment.case_artifact_get(
-            self._workspace_id, self._exp_id, self._case_id, artifact_id
+        response = self._validate_and_fetch_trajectories(
+            variables, only_last_point=False, format=_TrajectoryResponseFormat.V1
         )
 
-        return result, file_name
+        if response:
+            case_nbrs = range(len(response[0]))
+        else:
+            case_nbrs = range(len(self.get_cases()))
+
+        return {
+            f"case_{j + 1}": {
+                variable: response[i][j] for i, variable in enumerate(variables)
+            }
+            for j in case_nbrs
+        }
 
-    def get_fmu(self):
-        """
-        Returns the ModelExecutable class object simulated for the case.
+    def get_last_point(
+        self, variables: Optional[List[str]] = None
+    ) -> ExperimentResultPoint:
+        """Returns a ExperimentResultPoint class for a list of result variables
+        for all the cases.
+
+        Args:
+            variables: An optional list of result variables to fetch
+            trajectories for.
 
         Returns:
+            An ExperimentResultPoint class object.
 
-            FMU --
-                ModelExecutable class object.
+        Raises:
+            OperationNotCompleteError if simulation process is in progress.
+            OperationFailureError if simulation process was cancelled.
+            TypeError if the variable is not a list object.
+            ValueError if trajectory variable is not present in the result.
 
         Example::
 
-            case = experiment.get_case('case_1')
-            fmu = case.get_fmu()
-            fmus = set(case.get_fmu() for case in exp.get_cases())
-        """
-        fmu_id = self.input.fmu_id
+            result = experiment.get_last_point(['h', 'time'])
 
-        return modelon.impact.client.entities.model_executable.ModelExecutable(
-            self._workspace_id, fmu_id, self._sal
-        )
+            # Convert to Pandas data frame
+            df = pd.DataFrame(data=result.as_lists(), columns=result.variables,
+                index=result.cases)
+            df.index.name = "Cases"
+
+        """
+        format = _TrajectoryResponseFormat.V2
+        if variables is None:
+            variables = self.get_variables()
+            trajectories = self._sal.experiment.trajectories_get(
+                self._workspace_id,
+                self._exp_id,
+                variables,
+                last_point_only=True,
+                format=format.value,
+            )
+        else:
+            trajectories = self._validate_and_fetch_trajectories(
+                variables, only_last_point=True, format=format
+            )
+        return ExperimentResultPoint(trajectories["data"]["items"], variables)
 
-    def sync(self):
-        """Sync case state against server, pushing any changes that has been
-        done to the object client side.
+    def delete(self) -> None:
+        """Deletes an experiment.
 
         Example::
-            case.input.parametrization = {'PI.k': 120}
-            case.sync()
-        """
-        self._info = self._sal.experiment.case_put(
-            self._workspace_id, self._exp_id, self._case_id, self._info
-        )
-
-    def execute(self, sync_case_changes: bool = True) -> CaseOperation:
-        """Exceutes a case.
-        Returns an modelon.impact.client.operations.case.CaseOperation class object.
 
-        Parameters:
+            experiment.delete()
 
-            sync_case_changes --
-                Boolean specifying if to sync case changes against the server
-                before executing the case. Default is True.
+        """
+        self._sal.experiment.experiment_delete(self._workspace_id, self._exp_id)
 
+    def set_label(self, label: str) -> None:
+        """Sets a label (string) for an experiment to distinguish it.
 
-        Returns:
+        Example::
 
-            case_ops --
-                An modelon.impact.client.operations.case.CaseOperation class object.
+            experiment.set_label("Engine run with Oil type B")
 
-        Example::
-            case = experiment.get_case('case_1')
-            case.input.parametrization = {'PI.k': 120}
-            case.sync()
-            case_ops = case.execute()
-            case_ops.cancel()
-            case_ops.status()
-            case_ops.wait()
         """
-        if sync_case_changes:
-            self.sync()
+        self._sal.experiment.experiment_set_label(
+            self._workspace_id, self._exp_id, label
+        )
 
-        return CaseOperation(
-            self._workspace_id,
-            self._sal.experiment.experiment_execute(
-                self._workspace_id, self._exp_id, [self._case_id]
-            ),
-            self._case_id,
-            self._sal,
+    @classmethod
+    def from_operation(
+        cls, operation: BaseOperation[Experiment], **kwargs: Any
+    ) -> Experiment:
+        assert isinstance(operation, experiment.ExperimentOperation)
+        return cls(**kwargs, service=operation._sal)
+
+    @property
+    def custom_function(self) -> str:
+        """Returns the custom function name."""
+        return self._get_info()["experiment"]["base"]["analysis"]["type"]
+
+    def _get_fmu_info(self, fmu_id: str) -> Dict[str, Any]:
+        if self._fmu_info is None:
+            self._fmu_info = self._sal.workspace.fmu_get(self._workspace_id, fmu_id)
+
+        return self._fmu_info
+
+    def _get_workflow(self) -> _Workflow:
+        model = self._get_info()["experiment"]["base"]["model"]
+        return _Workflow.CLASS_BASED if model.get("modelica") else _Workflow.FMU_BASED
+
+    def get_class_name(self) -> str:
+        """Return the model class name."""
+        model = self._get_info()["experiment"]["base"]["model"]
+        if self._get_workflow() == _Workflow.CLASS_BASED:
+            return model["modelica"]["className"]
+        return self._get_fmu_info(model["fmu"]["id"])['input']["class_name"]
+
+    def get_compiler_options(self) -> CompilerOptions:
+        """Return a CompilerOptions object."""
+        model = self._get_info()["experiment"]["base"]["model"]
+        if self._get_workflow() == _Workflow.CLASS_BASED:
+            return CompilerOptions(
+                model["modelica"].get("compilerOptions", {}), self.custom_function
+            )
+        fmu_info = self._get_fmu_info(model["fmu"]["id"])['input']
+        return CompilerOptions(
+            fmu_info.get("compiler_options", {}), self.custom_function
         )
 
-    def _assert_unique_case_initialization(self, unsupported_init):
-        if self._info['input'][unsupported_init]:
-            raise ValueError(
-                "A case cannot use both 'initialize_from_case' and "
-                "'initialize_from_external_result' to specify what to initialize from! "
-                f"To resolve this, set the '{unsupported_init}' attribute "
-                "to None and re-try."
+    def get_runtime_options(self) -> RuntimeOptions:
+        """Return a RuntimeOptions object."""
+        model = self._get_info()["experiment"]["base"]["model"]
+        if self._get_workflow() == _Workflow.CLASS_BASED:
+            return RuntimeOptions(
+                model["modelica"].get("runtimeOptions", {}), self.custom_function
             )
+        fmu_info = self._get_fmu_info(model["fmu"]["id"])['input']
+        return RuntimeOptions(fmu_info.get("runtime_options", {}), self.custom_function)
+
+    def get_simulation_options(self) -> SimulationOptions:
+        """Return a SimulationOptions object."""
+        analysis = self._get_info()["experiment"]["base"]["analysis"]
+        return SimulationOptions(
+            analysis.get("simulationOptions", {}), self.custom_function
+        )
+
+    def get_solver_options(self) -> SolverOptions:
+        """Return a SolverOptions object."""
+        analysis = self._get_info()["experiment"]["base"]["analysis"]
+        return SolverOptions(analysis.get("solverOptions", {}), self.custom_function)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/custom_function.py` & `modelon_impact_client-3.0.1/modelon/impact/client/entities/custom_function.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+from __future__ import annotations
 import logging
-from typing import Any, List, Dict, Optional
+from typing import Any, List, Dict, Optional, TYPE_CHECKING
+
+from modelon.impact.client.entities.interfaces.custom_function import (
+    CustomFunctionInterface,
+)
 from modelon.impact.client.sal.service import Service
 from modelon.impact.client.options import ProjectExecutionOptions
 
+if TYPE_CHECKING:
+    from modelon.impact.client.options import (
+        CompilerOptions,
+        RuntimeOptions,
+        SimulationOptions,
+        SolverOptions,
+    )
+
 logger = logging.getLogger(__name__)
 
 
 class _Parameter:
+    __slots__ = ['_name', '_value', '_value_type', '_valid_values']
+
     _JSON_2_PY_TYPE = {
         "Number": (
             float,
             int,
         ),
         "String": (str,),
         "Boolean": (bool,),
@@ -24,37 +39,35 @@
         self._valid_values = valid_values
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
-    def value(self):
+    def value(self) -> Any:
         return self._value
 
     @value.setter
-    def value(self, value):
+    def value(self, value: Any) -> None:
         if not isinstance(value, self._JSON_2_PY_TYPE[self._value_type]):
             raise ValueError(
                 f"Cannot set {self._name} to {value}, its type is {self._value_type}"
             )
 
         if self._value_type == "Enumeration" and value not in self._valid_values:
             raise ValueError(
                 f"Cannot set enumeration '{self._name}' to '{value}', "
                 f"must be one of {self._valid_values}"
             )
 
         self._value = value
 
 
-class CustomFunction:
-    """
-    Class containing CustomFunction functionalities.
-    """
+class CustomFunction(CustomFunctionInterface):
+    """Class containing CustomFunction functionalities."""
 
     def __init__(
         self,
         workspace_id: str,
         name: str,
         parameter_data: List[Dict[str, Any]],
         service: Service,
@@ -69,37 +82,36 @@
                 p["type"],
                 p.get("values", []),
             )
             for p in parameter_data
         }
         self._sal = service
 
-    def __repr__(self):
-        return f"Custom function '{self._name}'"
-
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return isinstance(obj, CustomFunction) and obj._name == self._name
 
+    def __repr__(self) -> str:
+        return f"Custom function '{self._name}'"
+
     @property
     def name(self) -> str:
         "Custom function name"
         return self._name
 
-    def with_parameters(self, **modified) -> 'CustomFunction':
+    def with_parameters(self, **modified: Any) -> CustomFunction:
         """Sets/updates the custom_function parameters for an experiment.
 
-        Parameters:
-
-            parameters --
-                A keyworded, variable-length argument list of custom_function
+        Args:
+            parameters: A keyworded, variable-length argument list of custom_function
                 parameters.
 
         Example::
 
             custom_function.with_parameters(start_time=0.0, final_time=2.0)
+
         """
         new = CustomFunction(
             self._workspace_id, self._name, self._parameter_data, self._sal
         )
         for name, value in modified.items():
             if name not in new._param_by_name:
                 raise ValueError(
@@ -110,104 +122,106 @@
             parameter = new._param_by_name[name]
             parameter.value = value
 
         return new
 
     @property
     def parameter_values(self) -> Dict[str, Any]:
-        """Custom_function parameters and value as a dictionary"""
+        """Custom_function parameters and value as a dictionary."""
         return {p.name: p.value for p in self._param_by_name.values()}
 
-    def get_options(self, use_defaults: Optional[bool] = False):
+    def get_options(
+        self, use_defaults: Optional[bool] = False
+    ) -> ProjectExecutionOptions:
         """Get project execution option.
 
-        Parameters:
-
-            use_defaults --
+        Args:
+            use_defaults:
                 If true, default compiler options are used.
 
         Example::
+
             opts = custom_function.get_compiler_options()
             opts_2 = opts.compiler_options.with_values(c_compiler='gcc')
+
         """
         if use_defaults:
             options = self._sal.custom_function.custom_function_default_options_get(
                 self._workspace_id, self._name
             )
         else:
             options = self._sal.custom_function.custom_function_options_get(
                 self._workspace_id, self._name
             )
         return ProjectExecutionOptions(options, self.name)
 
-    def get_compiler_options(self, use_defaults: bool = False):
-        """
-        Return a modelon.impact.client.options.CompilerOptions object.
+    def get_compiler_options(self, use_defaults: bool = False) -> CompilerOptions:
+        """Return a modelon.impact.client.options.CompilerOptions object.
 
-        Returns:
+        Args:
+            use_defaults:
+                If True, default compiler options are used.
 
-            compiler_options --
-                A modelon.impact.client.options.CompilerOptions object.
+        Returns:
+            A CompilerOptions object.
 
-            use_defaults --
-                If true, default compiler options are used.
         Example::
 
             opts = custom_function.get_compiler_options()
             compiler_options = opts.with_values(c_compiler='gcc')
+
         """
         return self.get_options(use_defaults=use_defaults).compiler_options
 
-    def get_runtime_options(self, use_defaults: bool = False):
-        """
-        Return a modelon.impact.client.options.RuntimeOptions object.
+    def get_runtime_options(self, use_defaults: bool = False) -> RuntimeOptions:
+        """Return a RuntimeOptions object.
 
-        Returns:
+        Args:
+            use_defaults:
+                If True, default compiler options are used.
 
-            runtime_options --
-                A modelon.impact.client.options.RuntimeOptions object.
+        Returns:
+            A RuntimeOptions object.
 
-            use_defaults --
-                If true, default runtime options are used.
         Example::
 
             opts = custom_function.get_runtime_options()
             opts_2 = opts.with_values(cs_solver=0)
+
         """
         return self.get_options(use_defaults=use_defaults).runtime_options
 
-    def get_solver_options(self, use_defaults: bool = False):
-        """
-        Return a modelon.impact.client.options.SolverOptions object.
+    def get_solver_options(self, use_defaults: bool = False) -> SolverOptions:
+        """Return a modelon.impact.client.options.SolverOptions object.
 
-        Returns:
+        Args:
+            use_defaults:
+                If True, default compiler options are used.
 
-            solver_options --
-                A modelon.impact.client.options.SolverOptions object.
-
-            use_defaults --
-                If true, default solver options are used.
+        Returns:
+            A SolverOptions object.
 
         Example::
 
             opts = custom_function.get_solver_options()
             opts_2 = opts.with_values(rtol=1e-7)
+
         """
         return self.get_options(use_defaults=use_defaults).solver_options
 
-    def get_simulation_options(self, use_defaults: bool = False):
-        """
-        Return a modelon.impact.client.options.SimulationOptions object.
+    def get_simulation_options(self, use_defaults: bool = False) -> SimulationOptions:
+        """Return a SimulationOptions object.
 
-        Returns:
+        Args:
+            use_defaults:
+                If True, default compiler options are used.
 
-            simulation_options --
-                A modelon.impact.client.options.SimulationOptions object.
+        Returns:
+            A SimulationOptions object.
 
-            use_defaults --
-                If true, default simulation options are used.
         Example::
 
             opts = custom_function.get_simulation_options()
             opts_2 = opts.with_values(ncp=500)
+
         """
         return self.get_options(use_defaults=use_defaults).simulation_options
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/experiment.py` & `modelon_impact_client-3.0.1/modelon/impact/client/entities/model_executable.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,372 +1,363 @@
+from __future__ import annotations
 import logging
-from typing import Any, List, Dict, Optional
-from modelon.impact.client.sal.service import Service
-from modelon.impact.client.operations import experiment
-from modelon.impact.client.entities.case import Case
-from modelon.impact.client.entities.asserts import assert_variable_in_result
-from modelon.impact.client.entities.status import ExperimentStatus
+import os
+import tempfile
+from typing import Any, List, Dict, Optional, Union, TYPE_CHECKING
+
+from modelon.impact.client.entities.interfaces.model_executable import (
+    ModelExecutableInterface,
+)
+from modelon.impact.client.entities.asserts import assert_successful_operation
+from modelon.impact.client.entities.log import Log
+from modelon.impact.client.entities.status import ModelExecutableStatus
+from modelon.impact.client.experiment_definition.fmu_based import (
+    SimpleFMUExperimentDefinition,
+)
 from modelon.impact.client import exceptions
+from modelon.impact.client.operations.model_executable import (
+    ModelExecutableOperation,
+    CachedModelExecutableOperation,
+)
+
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.entities.custom_function import CustomFunction
+    from modelon.impact.client.options import SimulationOptions, SolverOptions
+    from modelon.impact.client.operations.base import BaseOperation
+
+    SimulationOptionsOrDict = Union[SimulationOptions, Dict[str, Any]]
+    SolverOptionsOrDict = Union[SolverOptions, Dict[str, Any]]
 
 logger = logging.getLogger(__name__)
 
 
-def _assert_experiment_is_complete(status, operation_name="Operation"):
-    if status == ExperimentStatus.NOTSTARTED:
+def _assert_compilation_is_complete(
+    status: ModelExecutableStatus, operation_name: str = "Operation"
+) -> None:
+    if status == ModelExecutableStatus.NOTSTARTED:
         raise exceptions.OperationNotCompleteError.for_operation(operation_name, status)
-    elif status == ExperimentStatus.CANCELLED:
+    elif status == ModelExecutableStatus.CANCELLED:
         raise exceptions.OperationFailureError.for_operation(operation_name)
 
 
-class _ExperimentRunInfo:
-    def __init__(
-        self,
-        status: ExperimentStatus,
-        errors: List[str],
-        failed: int,
-        successful: int,
-        cancelled: int,
-        not_started: int,
-    ):
+class ModelDescription(str):
+    """ModelDescription class inheriting from string object."""
+
+    def show(self) -> str:
+        """Prints the formatted xml."""
+        return self
+
+    def download(self, path: Optional[str] = None) -> str:
+        """Downloads the formatted xml.
+
+        Args:
+            path: The local path to store the downloaded model description.
+                Default: None. If no path is given, model description will
+                be downloaded in a temporary directory.
+
+        Returns:
+            Local path to the model description file.
+
+        Example::
+
+            model_description = fmu.get_model_description()
+            model_description.show()
+            model_description.download()
+
+        """
+        if path is None:
+            path = os.path.join(tempfile.gettempdir(), "impact-downloads")
+        os.makedirs(path, exist_ok=True)
+        artifact_path = os.path.join(path, 'modelDescription.xml')
+        with open(artifact_path, mode="w", encoding="utf-8") as f:
+            f.write(self)
+        return artifact_path
+
+
+class ModelExecutableRunInfo:
+    def __init__(self, status: ModelExecutableStatus, errors: List[str]):
         self._status = status
         self._errors = errors
-        self._failed = failed
-        self._successful = successful
-        self._cancelled = cancelled
-        self._not_started = not_started
 
     @property
-    def status(self):
-        """Status info for an Experiment"""
-        return self._status
+    def status(self) -> ModelExecutableStatus:
+        """Status info for a Model-Executable.
 
-    @property
-    def errors(self):
-        """A list of errors. Is empty unless 'status' attribute is 'FAILED'"""
-        return self._errors
+        .. Note:: For tracing status changes of a running
+            compilation, the ModelExecutableOperation status
+            property must be used and not ModelExecutable
+            entities run info(ModelExecutableRunInfo) status
+            property. See example for usage.
 
-    @property
-    def successful(self):
-        """Number of cases in experiment that are successful"""
-        return self._successful
+        Example::
 
-    @property
-    def failed(self):
-        """Number of cases in experiment thar have failed"""
-        return self._failed
+            # To get the case entity run info status
+            status = fmu.run_info.status
 
-    @property
-    def cancelled(self):
-        """Number of cases in experiment that are cancelled"""
-        return self._cancelled
+            # To get the status updates of a running compilation
+            compile_ops = = model.compile()
+            status = compile_ops.status
 
-    @property
-    def not_started(self):
-        """Number of cases in experiment that have not yet started"""
-        return self._not_started
+        """
+        return self._status
 
+    @property
+    def errors(self) -> List[str]:
+        """A list of errors.
 
-class _ExperimentMetaData:
-    def __init__(self, user_data: Dict[str, Any]):
-        self._user_data = user_data
+        Is empty unless 'status' attribute is 'FAILED'
 
-    @property
-    def user_data(self) -> Dict[str, Any]:
-        """User data dictionary object attached to experiment, if any"""
-        return self._user_data
+        """
+        return self._errors
 
 
-class Experiment:
-    """
-    Class containing Experiment functionalities.
-    """
+class ModelExecutable(ModelExecutableInterface):
+    """Class containing ModelExecutable functionalities."""
 
     def __init__(
         self,
         workspace_id: str,
-        exp_id: str,
+        fmu_id: str,
         service: Service,
         info: Optional[Dict[str, Any]] = None,
+        modifiers: Optional[Dict[str, Any]] = None,
     ):
+        self._fmu_id = fmu_id
         self._workspace_id = workspace_id
-        self._exp_id = exp_id
         self._sal = service
         self._info = info
+        self._modifiers = modifiers
 
-    def __repr__(self):
-        return f"Experiment with id '{self._exp_id}'"
+    def __eq__(self, obj: object) -> bool:
+        return isinstance(obj, ModelExecutable) and obj._fmu_id == self._fmu_id
 
-    def __eq__(self, obj):
-        return isinstance(obj, Experiment) and obj._exp_id == self._exp_id
+    def __repr__(self) -> str:
+        return f"FMU with id '{self._fmu_id}'"
 
-    @property
-    def id(self) -> str:
-        """Experiment id"""
-        return self._exp_id
+    def __hash__(self) -> int:
+        return self._fmu_id.__hash__()
 
-    def _get_info(self) -> Dict[str, Any]:
-        if self._info is None:
-            self._info = self._sal.workspace.experiment_get(
-                self._workspace_id, self._exp_id
-            )
+    def _variable_modifiers(self) -> Dict[str, Any]:
+        return {} if self._modifiers is None else self._modifiers
 
-        return self._info
-
-    @property
-    def run_info(self) -> _ExperimentRunInfo:
-        """Experiment run information"""
-        run_info = self._get_info()["run_info"]
+    def _get_info(self, cached: bool = True) -> Dict[str, Any]:
+        if not cached or self._info is None:
+            self._info = self._sal.workspace.fmu_get(self._workspace_id, self._fmu_id)
 
-        status = ExperimentStatus(run_info["status"])
-        errors = run_info.get("errors", [])
-        failed = run_info.get("failed", 0)
-        successful = run_info.get("successful", 0)
-        cancelled = run_info.get("cancelled", 0)
-        not_started = run_info.get("not_started", 0)
-        return _ExperimentRunInfo(
-            status, errors, failed, successful, cancelled, not_started
-        )
+        return self._info
 
     @property
-    def metadata(self) -> Optional[_ExperimentMetaData]:
-        """Experiment metadata. Returns custom user_data dictionary object attached
-        to the experiment, if any."""
-
-        info = self._get_info()
-        meta_data = info.get("meta_data")
-        if meta_data is not None:
-            user_data = meta_data.get("user_data")
-            if user_data is not None:
-                return _ExperimentMetaData(user_data)
-
-        return None
+    def id(self) -> str:
+        """FMU id."""
+        return self._fmu_id
 
     @property
     def info(self) -> Dict[str, Any]:
-        """Deprecated, use 'run_info' attribute"""
+        """Deprecated, use 'run_info' attribute."""
         logger.warning("This attribute is deprectated, use 'run_info' instead")
-        return self._get_info()
+        return self._get_info(cached=False)
 
-    def execute(
-        self, with_cases: Optional[List[Case]] = None, sync_case_changes: bool = True
-    ):
-        """Exceutes an experiment.
-        Returns an modelon.impact.client.operations.experiment.ExperimentOperation class
-        object.
-
-        Parameters:
-
-            with_cases --
-                A list of cases objects to execute.
-            sync_case_changes --
-                Boolean specifying if to sync the cases given with the 'with_cases'
-                argument against the server before executing the experiment.
-                Default is True.
+    @property
+    def run_info(self) -> ModelExecutableRunInfo:
+        """Compilation run information."""
+        run_info = self._get_info(cached=False)["run_info"]
+        status = ModelExecutableStatus(run_info["status"])
+        errors = run_info.get("errors", [])
+        return ModelExecutableRunInfo(status, errors)
 
-        Returns:
+    @property
+    def metadata(self) -> Dict[str, Any]:
+        """FMU metadata.
 
-            experiment_ops --
-                An modelon.impact.client.operations.experiment.ExperimentOperation
-                class object.
+        Returns the 'iteration_variable_count' and
+        'residual_variable_count' only for steady state model compiled
+        as an FMU
 
-        Example::
-            experiment = workspace.create_experiment(experiment_definition)
-            experiment_ops = experiment.execute()
-            experiment_ops.cancel()
-            experiment_ops.status()
-            experiment_ops.wait()
-
-            generate_cases = experiment.execute(with_cases=[]).wait()
-            cases_to_execute =  generate_cases.get_case('case_2')
-            experiment = experiment.execute(with_cases=[cases_to_execute]).wait()
-        """
-        if sync_case_changes and with_cases is not None:
-            for case in with_cases:
-                case.sync()
-
-        case_ids = [case.id for case in with_cases] if with_cases is not None else None
-        return experiment.ExperimentOperation(
-            self._workspace_id,
-            self._sal.experiment.experiment_execute(
-                self._workspace_id, self._exp_id, case_ids
-            ),
-            self._sal,
+        """
+        assert_successful_operation(self.is_successful(), "Compilation")
+        parameter_state = {"parameterState": self._variable_modifiers()}
+        return self._sal.model_executable.ss_fmu_metadata_get(
+            self._workspace_id, self._fmu_id, parameter_state
         )
 
+    def get_class_name(self) -> str:
+        """Return the model class name."""
+        return self._get_info()["input"]["class_name"]
+
     def is_successful(self) -> bool:
-        """
-        Returns True if the Experiment is done and no cases has failed.
-        Use the 'run_info' attribute to get more info.
+        """Returns True if the model has compiled successfully. Use the
+        'run_info' attribute to get more info.
 
         Returns:
-
-            True -> If execution process has completed successfully.
-            False -> If execution process has failed, is cancelled or still running.
+            True, if model has compiled successfully. False, if compilation
+            process has failed, is running or is cancelled.
 
         Example::
 
-            experiment.is_successful()
-        """
-        return (
-            self.run_info.status == ExperimentStatus.DONE
-            and self.run_info.failed == 0
-            and self.run_info.cancelled == 0
-        )
+            fmu.is_successful()
 
-    def get_variables(self) -> List[str]:
         """
-        Returns a list of variables available in the result.
+        return self.run_info.status == ModelExecutableStatus.SUCCESSFUL
 
-        Returns:
+    def get_log(self) -> Log:
+        """Returns the compilation log object.
 
-            variables --
-                An list of result variables.
+        Returns:
+            The compilation log object.
 
         Raises:
-
-            OperationNotCompleteError if simulation process is in progress.
-            OperationFailureError if simulation process has failed or was cancelled.
+            OperationNotCompleteError if compilation process is in progress.
+            OperationFailureError if compilation process was cancelled.
 
         Example::
 
-            experiment.get_variables()
+            log = fmu.get_log()
+            log.show()
+
         """
-        _assert_experiment_is_complete(self.run_info.status, "Simulation")
-        return self._sal.experiment.result_variables_get(
-            self._workspace_id, self._exp_id
+        _assert_compilation_is_complete(self.run_info.status, "Compilation")
+        return Log(
+            self._sal.model_executable.compile_log(self._workspace_id, self._fmu_id)
         )
 
-    def get_cases(self) -> List[Case]:
-        """
-        Returns a list of case objects for an experiment.
+    def get_model_description(self) -> ModelDescription:
+        """Returns the model description object.
 
         Returns:
-
-            cases --
-                An list of case objects.
+            The compilation log object.
 
         Example::
 
-            experiment.get_cases()
-        """
-        resp = self._sal.experiment.cases_get(self._workspace_id, self._exp_id)
-        return [
-            Case(case["id"], self._workspace_id, self._exp_id, self._sal, case)
-            for case in resp["data"]["items"]
-        ]
-
-    def get_case(self, case_id: str) -> Case:
-        """
-        Returns a case object for a given case_id.
-
-        Parameters:
+            model_description = fmu.get_model_description()
 
-            case_id --
-                The case_id for the case.
+            # Print the formatted xml
+            model_description.show()
 
-        Returns:
+            # Download the formatted xml
+            model_description.download()
 
-            cases --
-                An case object.
+            # Parse the xml
+            from xml.etree import ElementTree
 
-        Example::
+            tree = ElementTree.fromstring(model_description)
+            model_variables =tree.find('ModelVariables')
+            variable_names = [child.attrib.get('name') for child in model_variables]
 
-            experiment.get_case('case_1')
         """
-        case_data = self._sal.experiment.case_get(
-            self._workspace_id, self._exp_id, case_id
-        )
-        return Case(
-            case_data["id"], self._workspace_id, self._exp_id, self._sal, case_data
+        return ModelDescription(
+            self._sal.model_executable.model_description_get(
+                self._workspace_id, self._fmu_id
+            )
         )
 
-    def get_cases_with_label(self, case_label: str) -> List[Case]:
-        """
-        Returns a list of case objects for an experiment with the label.
-
-        Parameters:
-
-            case_label --
-                The case_label for the case.
-
-        Returns:
-
-            cases --
-                An list of case objects.
+    def delete(self) -> None:
+        """Deletes an FMU.
 
         Example::
 
-            experiment.get_cases_with_label('Cruise condition')
-        """
-        return [case for case in self.get_cases() if case.meta.label == case_label]
+            fmu.delete()
 
-    def get_trajectories(self, variables: List[str]) -> Dict[str, Any]:
         """
-        Returns a dictionary containing the result trajectories
-        for a list of result variables for all the cases.
-
-        Parameters:
+        self._sal.model_executable.fmu_delete(self._workspace_id, self._fmu_id)
 
-            variables --
-                A list of result variables to fecth trajectories for.
+    def get_settable_parameters(self) -> List[str]:
+        """Returns a list of settable parameters for the FMU.
 
         Returns:
-
-            trajectory --
-                A dictionary object containing the result trajectories for all cases.
+            A list of parameters that can be set on the FMU.
 
         Raises:
-
-            OperationNotCompleteError if simulation process is in progress.
-            OperationFailureError if simulation process was cancelled.
-            TypeError if the variable is not a list object.
-            ValueError if trajectory variable is not present in the result.
+            OperationNotCompleteError if compilation process is in progress.
+            OperationFailureError if compilation process has failed or was cancelled.
 
         Example::
 
-            result = experiment.get_trajectories(['h', 'time'])
-            height = result['case_1']['h']
-            time = result['case_1']['time']
-        """
-        if not isinstance(variables, list):
-            raise TypeError(
-                "Please specify the list of result keys for the trajectories of "
-                "intrest!"
-            )
-        _assert_experiment_is_complete(self.run_info.status, "Simulation")
-        assert_variable_in_result(variables, self.get_variables())
+            fmu.get_settable_parameters()
 
-        response = self._sal.experiment.trajectories_get(
-            self._workspace_id, self._exp_id, variables
+        """
+        assert_successful_operation(self.is_successful(), "Compilation")
+        return self._sal.model_executable.settable_parameters_get(
+            self._workspace_id, self._fmu_id
         )
 
-        if response:
-            case_nbrs = range(len(response[0]))
-        else:
-            case_nbrs = range(len(self.get_cases()))
-
-        return {
-            f"case_{j + 1}": {
-                variable: response[i][j] for i, variable in enumerate(variables)
-            }
-            for j in case_nbrs
-        }
-
-    def delete(self):
-        """Deletes an experiment.
+    def new_experiment_definition(
+        self,
+        custom_function: CustomFunction,
+        solver_options: Optional[SolverOptionsOrDict] = None,
+        simulation_options: Optional[SimulationOptionsOrDict] = None,
+        simulation_log_level: str = "WARNING",
+    ) -> SimpleFMUExperimentDefinition:
+        """Returns a new experiment definition using this FMU.
+
+        Args:
+            custom_function: The custom function to use for this experiment.
+            solver_options: The solver options to use for this experiment. By default
+                the options is set to None, which means the default options for the
+                custom_function input is used.
+            simulation_options: The simulation_options to use for this experiment.
+                By default the options is set to None, which means the default options
+                for the custom_function input is used.
+            simulation_log_level: Simulation log level for this experiment. Default
+                is 'WARNING'.
 
         Example::
 
-            experiment.delete()
-        """
-        self._sal.experiment.experiment_delete(self._workspace_id, self._exp_id)
+            fmu = model.compile().wait()
+            dynamic = workspace.get_custom_function('dynamic')
+            solver_options = {'atol':1e-8}
+            simulation_options = dynamic.get_simulation_options().
+            with_values(ncp=500)
+            experiment_definition = fmu.new_experiment_definition(
+                dynamic, solver_options, simulation_options)
+            experiment = workspace.execute(experiment_definition).wait()
+
+        """
+        return SimpleFMUExperimentDefinition(
+            self,
+            custom_function,
+            solver_options,
+            simulation_options,
+            simulation_log_level,
+        )
 
-    def set_label(self, label: str):
-        """Sets a label (string) for an experiment to distinguish it.
+    def download(self, path: Optional[str] = None) -> str:
+        """Downloads an FMU binary that is compiled. Returns the local path to
+        the downloaded FMU archive.
+
+        Args:
+            path: The local path to store the downloaded FMU. Default: None.
+                If no path is given, FMU will be downloaded in a temporary directory.
+
+        Returns:
+            Local path to the downloaded FMU.
+
+        Raises:
+            OperationNotCompleteError if compilation process is in progress.
+            OperationFailureError if compilation process has failed or was cancelled.
 
         Example::
 
-            experiment.set_label("Engine run with Oil type B")
-        """
-        self._sal.experiment.experiment_set_label(
-            self._workspace_id, self._exp_id, label
+            fmu =  model.compile().wait()
+            if fmu.is_successful():
+                fmu_path = fmu.download()
+                fmu_path = fmu.download('~/Downloads')
+
+        """
+        assert_successful_operation(self.is_successful(), "Compilation")
+        data = self._sal.workspace.fmu_download(self._workspace_id, self._fmu_id)
+        if path is None:
+            path = os.path.join(tempfile.gettempdir(), "impact-downloads")
+        os.makedirs(path, exist_ok=True)
+        fmu_path = os.path.join(path, self._fmu_id + ".fmu")
+        with open(fmu_path, "wb") as f:
+            f.write(data)
+        return fmu_path
+
+    @classmethod
+    def from_operation(
+        cls, operation: BaseOperation[ModelExecutable], **kwargs: Any
+    ) -> ModelExecutable:
+        assert isinstance(
+            operation, (ModelExecutableOperation, CachedModelExecutableOperation)
         )
+        return cls(**kwargs, service=operation._sal)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/project.py` & `modelon_impact_client-3.0.1/modelon/impact/client/entities/project.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-#
-# Copyright (c) 2022 Modelon AB
-#
+from __future__ import annotations
 import enum
 import logging
 from pathlib import Path
 from dataclasses import dataclass
-from typing import Optional, Union
+from typing import Optional, Union, List, Dict, Any, Iterable, TYPE_CHECKING
 from modelon.impact.client.options import ProjectExecutionOptions
 from modelon.impact.client.entities.content import ContentType, ProjectContent
 from modelon.impact.client.operations.content_import import ContentImportOperation
+from modelon.impact.client.operations.project_import import ProjectImportOperation
 from modelon.impact.client.entities.custom_function import CustomFunction
 from modelon.impact.client.sal.service import Service
 
+if TYPE_CHECKING:
+    from modelon.impact.client.operations.base import BaseOperation
+
 logger = logging.getLogger(__name__)
 RepoURL = Union['GitRepoURL', 'SvnRepoURL']
 
 
 @enum.unique
 class ProjectType(enum.Enum):
     """Type of project."""
@@ -23,62 +25,62 @@
     LOCAL = 'LOCAL'
     RELEASED = 'RELEASED'
     SYSTEM = 'SYSTEM'
 
 
 @dataclass
 class GitRepoURL:
-    """GitRepoURL represents a project referenced in a git repo
-    String representation is url[@[refname][:sha1]]
-    """
+    """GitRepoURL represents a project referenced in a git repo String
+    representation is url[@[refname][:sha1]]"""
 
     url: str
-    """ URL without protocol part, e.g., gitlab.modelon.com/group/project/repo """
+    """URL without protocol part, e.g.,
+    gitlab.modelon.com/group/project/repo."""
 
     refname: str = ""
-    """ Reference name (branch, tag or similar) """
+    """Reference name (branch, tag or similar)"""
 
     sha1: str = ""
-    """ Commit hash """
+    """Commit hash."""
 
-    def __str__(self):
+    def __str__(self) -> str:
         repo_url = self.url
         if self.refname or self.sha1:
             repo_url += '@'
         if self.refname:
             repo_url += self.refname
         if self.sha1:
             repo_url += ':' + self.sha1
         return repo_url
 
     @classmethod
-    def from_dict(cls, data):
+    def from_dict(cls, data: Any) -> GitRepoURL:
         return cls(
             url=data.get("url"), refname=data.get("refname"), sha1=data.get("sha1")
         )
 
 
 @dataclass
 class SvnRepoURL:
-    """SvnRepoURL represents a project referenced in a Subversion repo
-    String representation is url/trunk/subdir[@[rev]]
-    """
+    """SvnRepoURL represents a project referenced in a Subversion repo String
+    representation is url/trunk/subdir[@[rev]]"""
 
     root_url: str
-    """ URL without protocol part up to branch part, e.g., svn.modelon.com/PNNN/ """
+    """URL without protocol part up to branch part, e.g.,
+    svn.modelon.com/PNNN/"""
 
     branch: str = ""
-    """ Non-empty if it's standard layout and can be either
-        trunk or branches/name or tags/name """
+    """Non-empty if it's standard layout and can be either trunk or
+    branches/name or tags/name."""
 
     url_from_root: str = ""
-    """ URL segment after branch (could be saved in subdir as well) """
+    """URL segment after branch (could be saved in subdir as well)"""
 
     rev: str = ""
-    """ Revision number or empty (means HEAD) """
+    """Revision number or empty (means HEAD)"""
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, SvnRepoURL):
             return False
         return (
             self.get_rev() == other.get_rev()
             and self.root_url == other.root_url
@@ -88,27 +90,27 @@
 
     def get_rev(self) -> str:
         rev = self.rev
         if rev == "":
             return 'HEAD'
         return rev
 
-    def __str__(self):
+    def __str__(self) -> str:
         segments = [self.root_url]
         if self.branch:
             segments.append(self.branch)
         if self.url_from_root:
             segments.append(self.url_from_root)
         repo_url = '/'.join(segments)
         if self.rev:
             repo_url += '@' + self.rev
         return repo_url
 
     @classmethod
-    def from_dict(cls, data):
+    def from_dict(cls, data: Any) -> SvnRepoURL:
         return cls(
             root_url=data.get("rootUrl"),
             branch=data.get("branch"),
             url_from_root=data.get("urlFromRoot"),
             rev=data.get("rev"),
         )
 
@@ -117,262 +119,302 @@
 class VcsUri:
     service_kind: str
     service_url: str
     repourl: RepoURL
     protocol: str
     subdir: str
 
-    def __str__(self):
+    def __str__(self) -> str:
         uri = f"{self.service_kind.lower()}+{self.protocol}://{self.repourl}"
         subdir = self.subdir
         if subdir not in ["", "."]:
             uri = uri + "#" + subdir
         return uri
 
     @classmethod
-    def from_dict(cls, data):
+    def from_dict(cls, data: Any) -> VcsUri:
         repo_url = data.get("repoUrl")
         service_kind = data.get("serviceKind")
         return cls(
             service_kind=service_kind,
             service_url=data.get("serviceUrl"),
             repourl=GitRepoURL.from_dict(repo_url)
             if service_kind.lower() == 'git'
             else SvnRepoURL.from_dict(repo_url),
             protocol=data.get("protocol"),
             subdir=data.get("subdir"),
         )
 
 
 class ProjectDependency:
-    """Dependency entry for a project"""
+    """Dependency entry for a project."""
 
-    def __init__(self, data):
+    def __init__(self, data: Dict[str, Any]):
         self._data = data
 
     @property
-    def name(self):
-        """The name of the project dependency"""
+    def name(self) -> Optional[str]:
+        """The name of the project dependency."""
         return self._data.get('name')
 
     @property
-    def version_specifier(self):
-        """Version specifier"""
+    def version_specifier(self) -> Optional[str]:
+        """Version specifier."""
         return self._data.get('versionSpecifier')
 
 
 class ProjectDefinition:
-    """
-    Impact project definition.
-    """
+    """Impact project definition."""
 
-    def __init__(self, data):
+    def __init__(self, data: Dict[str, Any]):
         self._data = data
 
     @property
-    def name(self):
-        return self._data.get("name")
+    def name(self) -> str:
+        return self._data["name"]
 
     @property
-    def version(self):
+    def version(self) -> Optional[str]:
         return self._data.get("version")
 
     @property
-    def format(self):
-        return self._data.get("format")
+    def format(self) -> str:
+        return self._data["format"]
 
     @property
-    def dependencies(self):
+    def dependencies(self) -> List[ProjectDependency]:
         dependencies = self._data.get('dependencies', [])
         return [ProjectDependency(dependency) for dependency in dependencies]
 
     @property
-    def content(self):
+    def content(self) -> list:
         return self._data.get('content', [])
 
     @property
-    def execution_options(self):
+    def execution_options(self) -> List[ProjectExecutionOptions]:
         execution_options = self._data.get('executionOptions', [])
         return [
             ProjectExecutionOptions(
                 execution_option, execution_option['customFunction']
             )
             for execution_option in execution_options
         ]
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         return self._data
 
 
 class Project:
-    """
-    Class containing Project functionalities.
-    """
+    """Class containing Project functionalities."""
 
     def __init__(
         self,
         project_id: str,
-        project_definition: ProjectDefinition,
-        project_type: ProjectType,
+        project_definition: Union[ProjectDefinition, Dict[str, Any]],
+        project_type: Union[ProjectType, str],
         vcs_uri: Optional[VcsUri],
         service: Service,
     ):
         self._project_id = project_id
-        self._project_definition = project_definition
+        self._project_definition = (
+            ProjectDefinition(project_definition)
+            if isinstance(project_definition, dict)
+            else project_definition
+        )
         self._vcs_uri = vcs_uri or None
-        self._project_type = project_type
+        self._project_type = (
+            ProjectType(project_type) if isinstance(project_type, str) else project_type
+        )
         self._sal = service
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Project with id '{self._project_id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return isinstance(obj, Project) and obj._project_id == self._project_id
 
     @property
     def id(self) -> str:
-        """Project id"""
+        """Project id."""
         return self._project_id
 
     @property
-    def definition(self):
+    def name(self) -> str:
+        """Project name."""
+        return self.definition.name
+
+    @property
+    def size(self) -> float:
+        """Project size in bytes."""
+        return self._sal.project.project_get(self.id, vcs_info=False, size_info=True)[
+            'size'
+        ]
+
+    @property
+    def definition(self) -> ProjectDefinition:
         return self._project_definition
 
     @property
     def vcs_uri(self) -> Optional[VcsUri]:
-        """Project vcs uri"""
+        """Project vcs uri."""
         return self._vcs_uri
 
     @property
-    def project_type(self):
+    def project_type(self) -> ProjectType:
         return self._project_type
 
-    def delete(self):
+    def delete(self) -> None:
         """Deletes a project.
 
         Example::
 
             project.delete()
+
         """
         self._sal.project.project_delete(self._project_id)
 
-    def _get_project_content(self, content):
+    def _get_project_content(self, content: Dict[str, str]) -> ProjectContent:
         return ProjectContent(content, self._project_id, self._sal)
 
-    def get_contents(self):
+    def get_contents(self) -> Iterable[ProjectContent]:
         """Get project contents.
 
         Example::
 
             project.get_contents()
+
         """
         return [
             self._get_project_content(content)
             for content in self._project_definition.content
         ]
 
+    def get_content(self, content_id: str) -> ProjectContent:
+        """Gets the project content with the given ID.
+
+        Args:
+            content_id: The ID of the workspace.
+
+        Example::
+
+            project.get_content("79sd8-3n2a4-e3t24")
+
+        """
+        resp = self._sal.project.project_content_get(self.id, content_id)
+        return ProjectContent(resp, self.id, self._sal)
+
     def get_content_by_name(
         self, name: str, content_type: Optional[ContentType] = None
     ) -> Optional[ProjectContent]:
         """Gets the first matching project content with the given name.
 
-        Parameters:
+        Args:
+            name: The name of the content.
 
-            name --
-                The name of the content.
+            content_type: The type of the project content.
 
-            content_type --
-                The type of the project content.
         Example::
+
             from modelon.impact.client import ContentType
             project.get_content_by_name(name, ContentType.MODELICA)
+
         """
         contents = self.get_contents()
         if content_type:
             contents = (c for c in contents if c.content_type == content_type)
         try:
             return next(c for c in contents if c.name == name)
         except StopIteration:
             return None
 
     def get_modelica_library_by_name(self, name: str) -> Optional[ProjectContent]:
-        """Gets the first matching modelica library with the given name.
+        """Gets the first matching Modelica library with the given name.
 
-        Parameters:
+        Args:
 
-            name --
-                The modelica library name.
+            name: The Modelica library name.
 
         Example::
 
             project.get_content_by_name(name)
+
         """
         return self.get_content_by_name(name, ContentType.MODELICA)
 
-    def upload_content(self, path_to_content: str, content_type: ContentType):
+    def import_content(
+        self, path_to_content: str, content_type: ContentType
+    ) -> ContentImportOperation:
         """Upload content to a project.
 
-        Parameters:
+        Args:
 
-            path_to_content --
-                The path for the content to be imported.
+            path_to_content: The path for the content to be imported.
 
-            content_type --
-                The type of the imported content.
+            content_type: The type of the imported content.
 
         Example::
+
             from modelon.impact.client import ContentType
 
-            project.upload_content('/home/test.mo', ContentType.MODELICA).wait()
+            project.import_content('/home/test.mo', ContentType.MODELICA).wait()
+
         """
         resp = self._sal.project.project_content_upload(
             path_to_content, self._project_id, content_type.value
         )
-        return ContentImportOperation(resp['data']['location'], self._sal)
-
-    def upload_modelica_library(self, path_to_lib: str):
-        """Uploads/adds a non-encrypted modelica library or a modelica model to the project.
+        return ContentImportOperation[ProjectContent](
+            resp['data']['location'], self._sal, ProjectContent.from_operation
+        )
 
-        Parameters:
+    def import_modelica_library(self, path_to_lib: str) -> ContentImportOperation:
+        """Uploads/adds a non-encrypted Modelica library or a Modelica model to
+        the project.
 
-            path_to_lib --
+        Args:
+            path_to_lib:
                 The path for the library to be imported. Only '.mo' or '.zip' file
                 extension are supported for upload.
 
         Example::
 
-            project.upload_model_library('C:/A.mo')
-            project.upload_model_library('C:/B.zip')
+            content  = project.import_modelica_library('A.mo').wait()
+            content  = project.import_modelica_library('B.zip').wait()
+
         """
         if Path(path_to_lib).suffix.lower() not in ['.mo', '.zip']:
             raise ValueError(
                 "Only '.mo' or '.zip' file extension are supported for uploading "
                 "Modelica content into project."
             )
-        return self.upload_content(path_to_lib, ContentType.MODELICA)
+        return self.import_content(path_to_lib, ContentType.MODELICA)
 
     def get_options(
         self, custom_function: CustomFunction, use_defaults: Optional[bool] = False
-    ):
+    ) -> ProjectExecutionOptions:
         """Get project execution option.
 
-        Parameters:
-
-            custom_function --
-                The CustomFunction class object.
-
-            use_defaults --
-                If true, default options are used.
+        Args:
+            custom_function: The CustomFunction class object.
+            use_defaults: If true, default options are used.
 
         Example::
+
             dynamic = workspace.get_custom_function('dynamic')
             project.get_options(dynamic)
+
         """
         if use_defaults:
             options = self._sal.project.project_default_options_get(
-                self._project_id, custom_function=custom_function.name
+                custom_function._workspace_id, custom_function.name
             )
         else:
             options = self._sal.project.project_options_get(
-                self._project_id, custom_function=custom_function.name
+                self._project_id, custom_function._workspace_id, custom_function.name
             )
         return ProjectExecutionOptions(options, custom_function.name)
+
+    @classmethod
+    def from_operation(
+        cls, operation: BaseOperation[Project], **kwargs: Any
+    ) -> Project:
+        assert isinstance(operation, ProjectImportOperation)
+        return cls(**kwargs, vcs_uri=None, service=operation._sal)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/entities/workspace.py` & `modelon_impact_client-3.0.1/modelon/impact/client/entities/workspace.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,46 @@
+from __future__ import annotations
 from dataclasses import dataclass
 import logging
 import os
 import json
-from typing import Any, List, Dict, Optional, Union
+from typing import Any, List, Dict, Optional, Union, Type, TYPE_CHECKING
+
+from modelon.impact.client.entities.interfaces.workspace import WorkspaceInterface
 from modelon.impact.client.sal.service import Service
-from modelon.impact.client.experiment_definition.base import (
-    SimpleModelicaExperimentDefinition,
-    SimpleFMUExperimentDefinition,
+from modelon.impact.client.experiment_definition.interfaces.definition import (
+    BaseExperimentDefinition,
 )
 from modelon.impact.client.entities.custom_function import CustomFunction
-from modelon.impact.client.operations.workspace.exports import WorkspaceExportOperation
+from modelon.impact.client.operations.workspace.exports import (
+    WorkspaceExportOperation,
+    Export,
+)
+from modelon.impact.client.operations.workspace.imports import WorkspaceImportOperation
+from modelon.impact.client.operations.workspace.conversion import (
+    WorkspaceConversionOperation,
+)
+from modelon.impact.client.operations.project_import import ProjectImportOperation
 from modelon.impact.client.operations.experiment import ExperimentOperation
-from modelon.impact.client.operations.external_result import (
-    ExternalResultUploadOperation,
+from modelon.impact.client.operations.external_result_import import (
+    ExternalResultImportOperation,
 )
-import modelon.impact.client.entities.model
+from modelon.impact.client.entities.model import Model
+from modelon.impact.client.entities.external_result import ExternalResult
 from modelon.impact.client.entities.model_executable import ModelExecutable
 from modelon.impact.client.entities.experiment import Experiment
-from modelon.impact.client.entities.project import Project, ProjectDefinition, VcsUri
+from modelon.impact.client.entities.project import Project, VcsUri
 
+if TYPE_CHECKING:
+    from modelon.impact.client.operations.base import BaseOperation
 
 logger = logging.getLogger(__name__)
 
 ExperimentDefinition = Union[
-    SimpleModelicaExperimentDefinition,
-    SimpleFMUExperimentDefinition,
+    Type[BaseExperimentDefinition],
     Dict[str, Any],
 ]
 
 
 @dataclass
 class Reference:
     id: str
@@ -44,51 +56,53 @@
 
 @dataclass
 class VcsReference:
     id: str
     vcs_uri: str
 
 
-def _get_project_entry_reference(reference):
+def _get_project_entry_reference(
+    reference: Any,
+) -> Union[ReleasedProjectReference, VcsReference, Reference]:
     if "name" in reference:
         return ReleasedProjectReference(
             id=reference.get('id'),
             name=reference.get('name'),
             version=reference.get('version'),
             build=reference.get('build'),
         )
     elif "vcsUri" in reference:
         return VcsReference(id=reference.get('id'), vcs_uri=reference.get('vcsUri'))
     else:
         return Reference(id=reference.get('id'))
 
 
 class ProjectEntry:
-    def __init__(self, data) -> None:
+    def __init__(self, data: Any) -> None:
         self._data = data
 
     @property
-    def reference(self):
+    def reference(self) -> Union[ReleasedProjectReference, VcsReference, Reference]:
         return _get_project_entry_reference(self._data.get('reference'))
 
     @property
-    def id(self):
+    def id(self) -> str:
         return self.reference.id
 
     @property
-    def disabled(self):
+    def disabled(self) -> bool:
         return self._data.get('disabled')
 
     @property
-    def disabled_content(self):
+    def disabled_content(self) -> bool:
         return self._data.get('disabledContent')
 
 
 class WorkspaceDefinition:
-    def __init__(self, data) -> None:
+    def __init__(self, data: Any) -> None:
         self._data = data
 
     @property
     def name(self) -> str:
         return self._data.get('name')
 
     @property
@@ -121,550 +135,543 @@
         os.makedirs(path, exist_ok=True)
         definition_path = os.path.join(path, self.name + ".json")
         with open(definition_path, "w", encoding='utf-8') as f:
             json.dump(self._data, f, indent=4)
         return definition_path
 
     @classmethod
-    def from_file(cls, path: str):
+    def from_file(cls, path: str) -> WorkspaceDefinition:
         with open(path) as json_file:
             data = json.load(json_file)
         return cls(data)
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         return self._data
 
 
-class Workspace:
-    """
-    Class containing Workspace functionalities.
-    """
+class Workspace(WorkspaceInterface):
+    """Class containing Workspace functionalities."""
 
     def __init__(
         self,
         workspace_id: str,
-        workspace_definition: WorkspaceDefinition,
+        workspace_definition: Union[WorkspaceDefinition, Dict[str, Any]],
         service: Service,
     ):
         self._workspace_id = workspace_id
-        self._workspace_definition = workspace_definition
+        self._workspace_definition = (
+            WorkspaceDefinition(workspace_definition)
+            if isinstance(workspace_definition, dict)
+            else workspace_definition
+        )
         self._sal = service
 
-    def __repr__(self):
-        return f"Workspace with id '{self._workspace_id}'"
-
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return isinstance(obj, Workspace) and obj._workspace_id == self._workspace_id
 
+    def __repr__(self) -> str:
+        return f"Workspace with id '{self._workspace_id}'"
+
     @property
     def id(self) -> str:
-        """Workspace id"""
+        """Workspace id."""
         return self._workspace_id
 
     @property
-    def definition(self):
+    def size(self) -> float:
+        """Workspace size in bytes."""
+        return self._sal.workspace.workspace_get(workspace_id=self.id, size_info=True)[
+            "sizeInfo"
+        ]["total"]
+
+    @property
+    def definition(self) -> WorkspaceDefinition:
         return self._workspace_definition
 
     def get_custom_function(self, name: str) -> CustomFunction:
-        """
-        Returns a CustomFunction class object.
+        """Returns a CustomFunction class object.
 
-        Parameters:
-
-            name --
-                The name of the custom function.
+        Args:
+            name: The name of the custom function.
 
         Returns:
-
-            custom_function --
-                The CustomFunction class object.
+            The CustomFunction class object.
 
         Example::
 
             workspace.get_custom_function('dynamic')
+
         """
         custom_function = self._sal.custom_function.custom_function_get(
             self._workspace_id, name
         )
         return CustomFunction(
             self._workspace_id,
             custom_function["name"],
             custom_function["parameters"],
             self._sal,
         )
 
     def get_custom_functions(self) -> List[CustomFunction]:
-        """
-        Returns a list of CustomFunctions class objects.
+        """Returns a list of CustomFunctions class objects.
 
         Returns:
-
-            custom_functions --
-                A list of CustomFunction class objects.
+            A list of CustomFunction class objects.
 
         Example::
 
             workspace.get_custom_functions()
+
         """
         custom_functions = self._sal.custom_function.custom_functions_get(
             self._workspace_id
         )
         return [
             CustomFunction(
                 self._workspace_id,
                 custom_function["name"],
                 custom_function["parameters"],
                 self._sal,
             )
             for custom_function in custom_functions["data"]["items"]
         ]
 
-    def delete(self):
+    def delete(self) -> None:
         """Deletes a workspace.
 
         Example::
 
             workspace.delete()
+
         """
         self._sal.workspace.workspace_delete(self._workspace_id)
 
     def upload_result(
         self,
         path_to_result: str,
         label: Optional[str] = None,
         description: Optional[str] = None,
-    ) -> ExternalResultUploadOperation:
+    ) -> ExternalResultImportOperation:
         """Uploads a '.mat' result file to the workspace.
 
-        Parameters:
-
-            path_to_result --
-                The path for the result file to be imported.
-
-            label --
-                The label of the result file. Default: None.
-
-            description --
-                The description of the result file. Default: None.
+        Args:
+            path_to_result: The path for the result file to be imported.
+            label: The label of the result file. Default: None.
+            description: The description of the result file. Default: None.
 
         Example::
 
-            workspace.upload_result('C:/A.mat')
-            workspace.upload_result('C:/B.mat', label = "result_for_PID.mat",
+            workspace.upload_result('A.mat')
+            workspace.upload_result('B.mat', label = "result_for_PID.mat",
             description = "This is a result file for PID controller")
+
         """
-        resp = self._sal.workspace.result_upload(
+        resp = self._sal.external_result.result_upload(
             self._workspace_id, path_to_result, label=label, description=description
         )
-        return ExternalResultUploadOperation(resp["data"]["id"], self._sal)
+        return ExternalResultImportOperation[ExternalResult](
+            resp["data"]["location"], self._sal, ExternalResult.from_operation
+        )
 
-    def export(self, options: Dict[str, Any]):
+    def export(self) -> WorkspaceExportOperation:
         """Exports the workspace as a binary compressed archive. Similar to
         :obj:`~modelon.impact.client.entities.workspace.Workspace.download`,
         but gives more control for getting the workspace async.
-        Returns an modelon.impact.client.operations.workspace
+        Returns an modelon.impact.client.operations.workspace.exports
         .WorkspaceExportOperation class object.
 
-        Parameters:
-
-            options --
-                The definition of what workspace resources to include when
-                exporting the workspace.
-
         Returns:
-
-            WorkspaceExportOperation --
-                An modelon.impact.client.operations.workspace.WorkspaceExportOperation
-                 class object.
+            An WorkspaceExportOperation class object.
 
         Example::
 
-            options = {
-                "contents": {
-                    "libraries": [
-                        {"name": "LiquidCooling", "resources_to_exclude": []},
-                        {
-                            "name": "Workspace",
-                            "resources_to_exclude": ["my_plot.png", "my_sheet.csv"],
-                        },
-                    ],
-                    "experiment_ids": [
-                        "_nics_multibody_examples_elementary_doublependulum_20191029",
-                        "modelica_blocks_examples_pid_controller_20191023_151659_f32a30d",
-                    ],
-                    "fmu_ids": [
-                        "_nics_multibody_examples_elementary_doublependulum_20191029_089",
-                        "modelica_blocks_examples_pid_controller_20191023_151659_f32a30d",
-                    ],
-                }
-            }
-            path = workspace.export(options).wait().download_as('/home/workspace.zip')
-        """
-        options["workspaceId"] = self._workspace_id
-        resp = self._sal.workspace.workspace_export_setup(self._workspace_id, options)
-        return WorkspaceExportOperation(resp["data"]["location"], self._sal)
-
-    def download(self, options: Dict[str, Any], path: str):
-        """Downloads the workspace as a binary compressed archive.
-        Returns the local path to the downloaded workspace archive.
-        Similar to :obj:`~modelon.impact.client.entities.workspace.Workspace.export`,
-        but does the entire setup and download in one go.
-
-        Parameters:
-
-            options --
-                The definition of what workspace resources to include when
-                exporting the workspace.
-
-            path --
-                The local path to store the downloaded workspace.
+            path = workspace.export().wait().download_as('/home/workspace.zip')
+        """
+        resp = self._sal.workspace.workspace_export_setup(self._workspace_id)
+        return WorkspaceExportOperation[Workspace](
+            resp["data"]["location"], self._sal, Export.from_operation
+        )
 
-        Returns:
+    def download(self, path: str) -> str:
+        """Downloads the workspace as a binary compressed archive. Returns the
+        local path to the downloaded workspace archive. Similar to
+        :obj:`~modelon.impact.client.entities.workspace.Workspace.export`, but
+        does the entire setup and download in one go.
 
-            path --
-                Local path to the downloaded workspace archive.
+        Args:
 
-        Example::
-
-            options = {
-                "contents": {
-                    "libraries": [
-                        {"name": "LiquidCooling", "resources_to_exclude": []},
-                        {
-                            "name": "Workspace",
-                            "resources_to_exclude": ["my_plot.png", "my_sheet.csv"],
-                        },
-                    ],
-                    "experiment_ids": [
-                        "_nics_multibody_examples_elementary_doublependulum_20191029_0",
-                        "modelica_blocks_examples_pid_controller_20191023_151659_f32a30d",
-                    ],
-                    "fmu_ids": [
-                        "_nics_multibody_examples_elementary_doublependulum_20191029_08",
-                        "modelica_blocks_examples_pid_controller_20191023_151659_f32a30d",
-                    ],
-                }
-            }
-            workspace.download(options, path)
-        """
-        ws_path = os.path.join(path, self._workspace_id + ".zip")
-        ops = self.export(options).wait()
-        return ops.download_as(ws_path)
-
-    def clone(self) -> 'Workspace':
-        """Clones the workspace.
-        Returns a clone Workspace class object.
+            path: The local path to store the downloaded workspace.
 
         Returns:
-
-            workspace_clone --
-                Clones workspace class object.
+            Local path to the downloaded workspace archive.
 
         Example::
 
-            workspace.clone()
-        """
-        resp = self._sal.workspace.workspace_clone(self._workspace_id)
-        return Workspace(
-            resp["workspace_id"], WorkspaceDefinition(resp["definition"]), self._sal
-        )
+            workspace.download(path)
 
-    def get_model(self, class_name: str, project: Optional[Project] = None):
         """
-        Returns a Model class object.
-
-        Parameters:
+        ws_path = os.path.join(path, self._workspace_id + ".zip")
+        ops = self.export().wait()
+        return ops.download_as(ws_path)
 
-            class_name --
-                The modelica class path of the model.
+    def get_model(self, class_name: str, project: Optional[Project] = None) -> Model:
+        """Returns a Model class object.
 
-            project --
-                Project class object
+        Args:
+            class_name: The Modelica class path of the model.
+            project: Project class object
 
         Returns:
-
-            model --
-                Model class object.
+            Model class object.
 
         Example::
 
             workspace.get_model(class_name)
+
         """
         project = project or self.get_default_project()
-        return modelon.impact.client.entities.model.Model(
-            class_name, self._workspace_id, project.id, self._sal
-        )
+        return Model(class_name, self._workspace_id, project.id, self._sal)
 
     def get_fmus(self) -> List[ModelExecutable]:
-        """
-        Returns a list of ModelExecutable class objects.
+        """Returns a list of ModelExecutable class objects.
 
         Returns:
-
-            FMUs --
-                List of ModelExecutable class objects.
+            List of ModelExecutable class objects.
 
         Example::
 
             workspace.get_fmus()
+
         """
         resp = self._sal.workspace.fmus_get(self._workspace_id)
         return [
             ModelExecutable(self._workspace_id, item["id"], self._sal, item)
             for item in resp["data"]["items"]
         ]
 
     def get_fmu(self, fmu_id: str) -> ModelExecutable:
-        """
-        Returns a ModelExecutable class object.
+        """Returns a ModelExecutable class object.
 
         Returns:
-
-            FMU --
-                ModelExecutable class object.
+            ModelExecutable class object.
 
         Example::
 
             workspace.get_fmu(fmu_id)
+
         """
         resp = self._sal.workspace.fmu_get(self._workspace_id, fmu_id)
         return ModelExecutable(self._workspace_id, resp["id"], self._sal, resp)
 
-    def get_experiments(self) -> List[Experiment]:
-        """
-        Returns a list of Experiment class objects.
+    def get_experiments(self, class_path: Optional[str] = None) -> List[Experiment]:
+        """Returns a list of Experiment class objects.
 
-        Returns:
+        Parameters:
 
-            experiment --
-                List of Experiment class objects.
+            class_path --
+                The modelica class path. If given, only the experiments
+                generated for model with the specified class path
+                are returned.
+
+        Returns:
+            List of Experiment class objects.
 
         Example::
 
             workspace.get_experiments()
+
         """
-        resp = self._sal.workspace.experiments_get(self._workspace_id)
+        resp = self._sal.workspace.experiments_get(self._workspace_id, class_path)
         return [
             Experiment(self._workspace_id, item["id"], self._sal, item)
             for item in resp["data"]["items"]
         ]
 
     def get_experiment(self, experiment_id: str) -> Experiment:
-        """
-        Returns an Experiment class object.
+        """Returns an Experiment class object.
 
-        Parameters:
-
-            experiment_id --
+        Args:
+            experiment_id:
                 The ID of the experiment.
 
         Returns:
-
-            experiment --
-                Experiment class object.
+            Experiment class object.
 
         Example::
 
             workspace.get_experiment(experiment_id)
+
         """
         resp = self._sal.workspace.experiment_get(self._workspace_id, experiment_id)
         return Experiment(self._workspace_id, resp["id"], self._sal, resp)
 
     def create_experiment(
         self,
         definition: ExperimentDefinition,
         user_data: Optional[Dict[str, Any]] = None,
     ) -> Experiment:
-        """Creates an experiment.
-        Returns an Experiment class object.
+        """Creates an experiment. Returns an Experiment class object.
 
-        Parameters:
-
-            definition --
-                An parametrized experiment definition class of type
-                modelon.impact.client.experiment_definition.base.SimpleModelicaExperimentDefinition
-                or
-                modelon.impact.client.experiment_definition.base.SimpleFMUExperimentDefinition.
-            user_data --
+        Args:
+            definition: A parametrized experiment definition class of type
+                SimpleModelicaExperimentDefinition or SimpleFMUExperimentDefinition.
+            user_data:
                 Optional dictionary object with custom data to attach to the experiment.
 
         Returns:
-
-            experiment --
-                Experiment class object.
+            Experiment class object.
 
         Example::
 
             workspace.create_experiment(definition)
+
         """
         if isinstance(
             definition,
-            (SimpleFMUExperimentDefinition, SimpleModelicaExperimentDefinition),
+            BaseExperimentDefinition,
         ):
             definition_as_dict = definition.to_dict()
         elif isinstance(definition, dict):
             definition_as_dict = definition
         else:
             raise TypeError(
                 "Definition object must either be a dictionary or an instance of either"
-                "modelon.impact.client.experiment_definition.base."
-                "SimpleModelicaExperimentDefinition class or modelon.impact.client."
-                "experiment_definition.base.SimpleFMUExperimentDefinition.!"
+                "SimpleModelicaExperimentDefinition or SimpleFMUExperimentDefinition"
+                "class!"
             )
         resp = self._sal.workspace.experiment_create(
             self._workspace_id, definition_as_dict, user_data
         )
         return Experiment(self._workspace_id, resp["experiment_id"], self._sal)
 
     def execute(
         self,
         definition: ExperimentDefinition,
         user_data: Optional[Dict[str, Any]] = None,
     ) -> ExperimentOperation:
-        """Exceutes an experiment.
-        Returns an modelon.impact.client.operations.experiment.ExperimentOperation
-        class object.
+        """Executes an experiment.
 
-        Parameters:
-
-            definition --
+        Args:
+            definition:
                 An experiment definition class instance of
-                modelon.impact.client.experiment_definition.base.SimpleFMUExperimentDefinition
-                or
-                modelon.impact.client.experiment_definition.base.SimpleModelicaExperimentDefinition
-                or
-                a dictionary object containing the definition.
-            user_data --
+                SimpleFMUExperimentDefinition
+                or SimpleModelicaExperimentDefinition
+                or a dictionary object containing the definition.
+            user_data:
                 Optional dictionary object with custom data to attach to the experiment.
 
 
         Returns:
-
-            experiment_ops --
-                An modelon.impact.client.operations.experiment.ExperimentOperation
-                class object.
+            An ExperimentOperation class object.
 
         Example::
 
             experiment_ops = workspace.execute(definition)
             experiment_ops.cancel()
-            experiment_ops.status()
+            experiment_ops.status
             experiment_ops.wait()
+
         """
         exp_id = self.create_experiment(definition, user_data).id
-        return ExperimentOperation(
+        return ExperimentOperation[Experiment](
             self._workspace_id,
             self._sal.experiment.experiment_execute(self._workspace_id, exp_id),
             self._sal,
+            Experiment.from_operation,
         )
 
-    def get_projects(self, vcs_info: bool = True, include_disabled: bool = False):
+    def get_projects(
+        self, vcs_info: bool = True, include_disabled: bool = False
+    ) -> List[Project]:
         """Return the list of projects for a workspace.
 
-        Returns:
+        Args:
+            vcs_info: If True, the versioning details are returned for the
+            project(if under version control).
+            include_disabled: If True, projects disabled in the workspace
+            are also lsited.
 
-            projects --
-                A list of modelon.impact.client.entities.project.Project
-                class object.
+        Returns:
+            A list of Project class objects.
 
         Example::
 
             projects = workspace.get_projects()
+
         """
         resp = self._sal.workspace.projects_get(
             self._workspace_id, vcs_info=vcs_info, include_disabled=include_disabled
         )
         projects = [
             Project(
                 item["id"],
-                ProjectDefinition(item['definition']),
+                item['definition'],
                 item["projectType"],
                 VcsUri.from_dict(item["vcsUri"]) if item.get("vcsUri") else None,
                 self._sal,
             )
             for item in resp["data"]["items"]
         ]
         return projects
 
-    def get_dependencies(self, vcs_info: bool = True, include_disabled: bool = False):
+    def get_dependencies(
+        self, vcs_info: bool = True, include_disabled: bool = False
+    ) -> List[Project]:
         """Return the list of project dependencies for a workspace.
 
-        Returns:
+        Args:
+            vcs_info: If True, the versioning details are returned for the
+            project(if under version control).
+            include_disabled: If True, projects disabled in the workspace
+            are also lsited.
 
-            dependencies --
-                A list of modelon.impact.client.entities.project.Project
-                class object.
+        Returns:
+            A list of Project class object.
 
         Example::
 
             dependencies = workspace.get_dependencies()
+
         """
         resp = self._sal.workspace.dependencies_get(
             self._workspace_id, vcs_info, include_disabled
         )
         return [
             Project(
                 item["id"],
-                ProjectDefinition(item['definition']),
+                item['definition'],
                 item["projectType"],
                 VcsUri.from_dict(item["vcsUri"]) if item.get("vcsUri") else None,
                 self._sal,
             )
             for item in resp["data"]["items"]
         ]
 
-    def create_project(self, name: str):
+    def create_project(self, name: str) -> Project:
         """Creates a new project in the workspace.
 
         Returns:
-
-            project --
-                An modelon.impact.client.entities.project.Project
-                class object.
+            A Project class object.
 
         Example::
 
             project = workspace.create_project("test")
+
         """
         resp = self._sal.workspace.project_create(self._workspace_id, name)
         return Project(
             resp["id"],
-            ProjectDefinition(resp['definition']),
+            resp['definition'],
             resp["projectType"],
             VcsUri.from_dict(resp["vcsUri"]) if resp.get("vcsUri") else None,
             self._sal,
         )
 
-    def get_default_project(self):
+    def get_default_project(self) -> Project:
         """Return the default project for a workspace.
 
         Returns:
-
-            project --
-                An modelon.impact.client.entities.project.Project
-                class object.
+            An Project class object.
 
         Example::
 
             project = workspace.get_default_project()
+
         """
         if not self._workspace_definition.default_project_id:
             raise ValueError(
                 f'No default project exists for the workspace {self._workspace_id}!'
             )
         resp = self._sal.project.project_get(
-            self._workspace_definition.default_project_id, vcs_info=True
+            self._workspace_definition.default_project_id,
+            vcs_info=True,
+            size_info=False,
         )
         return Project(
             resp["id"],
-            ProjectDefinition(resp["definition"]),
+            resp["definition"],
             resp["projectType"],
             VcsUri.from_dict(resp["vcsUri"]) if resp.get("vcsUri") else None,
             self._sal,
         )
 
-    def get_shared_definition(self, strict: bool = False):
+    def get_shared_definition(self, strict: bool = False) -> WorkspaceDefinition:
+        """Return the shared definition for a workspace.
+
+        Args:
+            strict: If True, the version control URIs for workspace projects and
+                dependencies are to specific commits or not.
+
+        Returns:
+            An WorkspaceDefinition class object.
+
+        Example::
+
+            definition = workspace.get_shared_definition()
+
+        """
         return WorkspaceDefinition(
             self._sal.workspace.shared_definition_get(
                 self._workspace_id, strict=strict
             )["definition"]
         )
+
+    def import_project_from_zip(self, path_to_project: str) -> ProjectImportOperation:
+        """Imports a Project from a compressed(.zip) project file and adds it
+        to the workspace. Returns the project class object.
+
+        Args:
+            path_to_project: The path for the compressed project(.zip) to be uploaded.
+
+        Returns:
+            A ProjectImportOperation class object.
+
+        Example::
+
+            workspace.import_project_from_zip(path_to_project).wait()
+
+        """
+        resp = self._sal.workspace.import_project_from_zip(
+            self._workspace_id, path_to_project
+        )
+        return ProjectImportOperation[Project](
+            resp["data"]["location"], self._sal, Project.from_operation
+        )
+
+    def import_dependency_from_zip(
+        self, path_to_dependency: str
+    ) -> ProjectImportOperation:
+        """Imports a Project dependency from a compressed(.zip) project file
+        and adds it to the workspace. Returns the project class object.
+
+        Args:
+            path_to_dependency: The path for the compressed project(.zip) to be
+            uploaded.
+
+        Returns:
+            An ProjectImportOperation class object.
+
+        Example::
+
+            workspace.import_dependency_from_zip(path_to_project).wait()
+
+        """
+        resp = self._sal.workspace.import_dependency_from_zip(
+            self._workspace_id, path_to_dependency
+        )
+        return ProjectImportOperation[Project](
+            resp["data"]["location"], self._sal, Project.from_operation
+        )
+
+    @classmethod
+    def from_import_operation(
+        cls, operation: BaseOperation[Workspace], **kwargs: Any
+    ) -> Workspace:
+        assert isinstance(operation, WorkspaceImportOperation)
+        return cls(**kwargs, service=operation._sal)
+
+    @classmethod
+    def from_conversion_operation(
+        cls, operation: BaseOperation[Workspace], **kwargs: Any
+    ) -> Workspace:
+        assert isinstance(operation, WorkspaceConversionOperation)
+        return cls(**kwargs, service=operation._sal)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/exceptions.py` & `modelon_impact_client-3.0.1/modelon/impact/client/exceptions.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+from __future__ import annotations
+from typing import Any
+
+
 class Error(Exception):
     pass
 
 
 class UnsupportedSemanticVersionError(Error):
     pass
 
@@ -12,35 +16,41 @@
 
 class OperationTimeOutError(Error):
     pass
 
 
 class OperationFailureError(Error):
     @classmethod
-    def for_operation(cls, operation_name: str):
+    def for_operation(cls, operation_name: str) -> OperationFailureError:
         return cls(
             f"{operation_name} was cancelled before completion! "
             f"Log file generated for cancelled {operation_name} is empty!"
         )
 
 
 class OperationNotCompleteError(Error):
     @classmethod
-    def for_operation(cls, operation_name: str, status):
+    def for_operation(
+        cls, operation_name: str, status: Any
+    ) -> OperationNotCompleteError:
         return cls(
             f"{operation_name} is still in progress! Status : {status}."
             f" Please call the wait() method on the {operation_name} operation"
             " to wait until completion!"
         )
 
 
 class OperationCompleteError(Error):
     pass
 
 
+class IllegalProjectImport(Error):
+    pass
+
+
 class IllegalWorkspaceImport(Error):
     pass
 
 
 class IllegalWorkspaceExport(Error):
     pass
 
@@ -49,9 +59,17 @@
     pass
 
 
 class IllegalContentImport(Error):
     pass
 
 
+class IllegalFMUImport(Error):
+    pass
+
+
 class ExternalResultUploadError(Error):
     pass
+
+
+class NoSuchCustomArtifactError(Error):
+    pass
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/expansion.py` & `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/expansion.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,106 +1,92 @@
-from dataclasses import dataclass, asdict
-from abc import abstractmethod, ABC
-from typing import Optional
 import logging
+from dataclasses import dataclass, asdict
+from typing import Optional, Dict, Any
 
+from modelon.impact.client.experiment_definition.interfaces.expansion import (
+    ExpansionAlgorithm,
+)
 
 logger = logging.getLogger(__name__)
 
 
-class ExpansionAlgorithm(ABC):
-    """
-    Base class for an expansion algorithm.
-    """
-
-    @abstractmethod
-    def __str__(self):
-        "Returns a string representation of the expansion algorithm"
-
-    @abstractmethod
-    def get_parameters_as_dict(self):
-        "Returns parameters as a dictionary"
-
-
 @dataclass
 class LatinHypercube(ExpansionAlgorithm):
-    """LatinHypercube expansion class.
+    """LatinHypercube expansion class. Produces <samples> cases, picks a random
+    value from each Modifier expression for each case. The resulting cases are
+    ortogonal, i.e., the values of a given Modifier expression do not repeat.
+    The exception are singular Modifiers, e.g., Modifier('name', 1), these
+    result in the same value for all cases. Singular Modifiers do not affect
+    the result (with respect to the seed) in the resulting Experiment.
 
     Args:
-        samples (int) --
+        samples (int):
             Positive integer; number of cases the Experiment will produce.
-        seed (int)  --
+        seed (int) :
             Using the same seed will result in the same output for an Experiment with
             the same modifiers. If not set or None: picks a random seed. Must be a
             non-negative integer. Default: None.
 
-        Produces <samples> cases, picks a random value from each Modifier expression
-        for each case. The resulting cases are ortogonal, i.e., the values of a given
-        Modifier expression do not repeat. The exception are singular Modifiers, e.g.,
-        Modifier('name', 1), these result in the same value for all cases. Singular
-        Modifiers do not affect the result (with respect to the seed) in the resulting
-        Experiment.
-
     """
 
     samples: int
     seed: Optional[int] = None
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "LATINHYPERCUBE"
 
-    def get_parameters_as_dict(self):
+    def get_parameters_as_dict(self) -> Optional[Dict[str, Any]]:
         return asdict(self)
 
 
 class FullFactorial(ExpansionAlgorithm):
-    """Full-factorial expansion class.
-    Creates experiment with all possible combinations of the input Modifiers
-    expressions.
-
-    Supported Modifier expressions:
-        Range
-        Choices
-        Singular Modifiers, e.g., Modifier('name', 1), Modifier('name', 'a')
-
-    Will return a single empty case if no Modifiers provided in Experiment.
-
-    Observe that the size of an Experiment with FullFactorial expansion is the product
-    of the Modifier lenghts. This number can grow very rapidly if using a lot of
-    Modifiers.
+    """Full-factorial expansion class. Creates experiment with all possible
+    combinations of the input Modifiers expressions.
+
+    Supported Modifier expressions:     Range     Choices     Singular
+    Modifiers, e.g., Modifier('name', 1), Modifier('name', 'a')
+
+    Will return a single empty case if no Modifiers provided in
+    Experiment.
+
+    Observe that the size of an Experiment with FullFactorial expansion
+    is the product of the Modifier lenghts. This number can grow very
+    rapidly if using a lot of Modifiers.
+
     """
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "FULLFACTORIAL"
 
-    def get_parameters_as_dict(self):
+    def get_parameters_as_dict(self) -> Optional[Dict[str, Any]]:
         return None
 
 
 @dataclass
 class Sobol(ExpansionAlgorithm):
-    """Expansion method based on the Sobol sequence.
-    The Sobol sequence is a minimal discrepancy quasi-random
-    sampling methods and suitable for achieving a good coverage of the design space.
+    """Expansion method based on the Sobol sequence. The Sobol sequence is a
+    minimal discrepancy quasi-random sampling methods and suitable for
+    achieving a good coverage of the design space.
 
     Args:
-        samples (int) --
+        samples (int):
             Positive integer; number of cases the Experiment will produce.
             Expansions where the number of samples is a power of 2 yield
             additional balances properties.
 
         Produces <samples> cases, based on the Sobol sequence.
         The points of the Sobol sequence are "extendible".
         I.e., given two Experiments with Expansions of different sample size, the larger
         Experiment contains all cases of the smaller one.
 
         Singular Modifiers, e.g., Modifier('name', 1), do not affect the result in the
         resulting Experiment.
+
     """
 
     samples: int
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "SOBOL"
 
-    def get_parameters_as_dict(self):
+    def get_parameters_as_dict(self) -> Optional[Dict[str, Any]]:
         return asdict(self)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/extension.py` & `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/extension.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,67 @@
+from __future__ import annotations
 import logging
-from abc import ABC
+from typing import Optional, Dict, Any, Union, TYPE_CHECKING
 
+from modelon.impact.client.experiment_definition.interfaces.extension import (
+    BaseExperimentExtension,
+)
 from modelon.impact.client.experiment_definition.operators import Operator
-from modelon.impact.client.entities.external_result import ExternalResult
+from modelon.impact.client.entities.interfaces.experiment import ExperimentInterface
+from modelon.impact.client.entities.interfaces.case import CaseInterface
 from modelon.impact.client.experiment_definition.util import (
     get_options,
     case_to_identifier_dict,
 )
-from modelon.impact.client.experiment_definition.asserts import (
-    validate_and_set_initialize_from,
-    assert_unique_exp_initialization,
-)
+
+if TYPE_CHECKING:
+    from modelon.impact.client.entities.case import Case
+    from modelon.impact.client.entities.experiment import Experiment
+
+    CaseOrExperiment = Union[Case, Experiment]
 
 logger = logging.getLogger(__name__)
 
 
-class BaseExperimentExtension(ABC):
-    """
-    Base class for an experiment extension class.
-    """
+def _validate_initialize_from(entity: Optional[CaseOrExperiment]) -> None:
+    if not entity:
+        return
+    if entity and not isinstance(entity, (ExperimentInterface, CaseInterface)):
+        raise TypeError(
+            "It is only supported to specify initialize from either Experiment "
+            "or Case for experiment extensions"
+        )
+    if isinstance(entity, ExperimentInterface) and len(entity.get_cases()) > 1:
+        raise ValueError(
+            "Cannot initialize from an experiment containing multiple"
+            " cases! Please specify a case object instead."
+        )
 
 
 class SimpleExperimentExtension(BaseExperimentExtension):
-    """
-    A simple experiment extension class for defining experiement extensions.
+    """A simple experiment extension class for defining experiement extensions.
 
-    Parameters:
-
-        parameter_modifiers --
-            The custom function parameters passes as a dictionary. By default, the
-            parameter_modifier is set to None, which means the options set in
-            the experiment definition will be used.
-
-        solver_options --
-            A solver options class instance of
-            modelon.impact.client.options.SolverOptions or
+    Args:
+        parameter_modifiers: The custom function parameters passes as a dictionary.
+            By default, the parameter_modifier is set to None, which means the options
+            set in the experiment definition will be used.
+        solver_options: A solver options class instance of SolverOptions or
             a dictionary object containing the solver options. By
             default, the options is set to None, which means an empty dictionary
             is passed in the experiment extension.
-
-        simulation_options --
-            A simulation options class instance of
-            modelon.impact.client.options.SimulationOptions or
+        simulation_options: A simulation options class instance of SimulationOptions or
             a dictionary object containing the simulation options. By
             default, the options is set to None, which means an empty dictionary
             is passed in the experiment extension.
+        simulation_log_level: Simulation log level for this experiment.
+            Default: 'WARNING'.
+        initialize_from: Optional entity to initialize from. An instance of
+            Case or Experiment. Default: None
 
-        simulation_log_level --
-            Simulation log level for this experiment. Default: 'WARNING'.
-
-    Examples::
+    Example::
 
         fmu = model.compile().wait()
         simulation_options = custom_function.get_simulation_options()
         .with_values(ncp=500)
         solver_options = {'atol':1e-8}
         simulate_def = fmu.new_experiment_definition(
             custom_function,
@@ -63,41 +71,43 @@
         simulate_ext = SimpleExperimentExtension(
         {'start_time': 0.0, 'final_time': 4.0},
         solver_options,
         simulation_options.with_values(ncp=600)
         ).with_modifiers({'PI.k': 40})
         simulate_def = simulate_def.with_extensions(simulate_ext)
         simulate_def.to_dict()
+
     """
 
     def __init__(
         self,
-        parameter_modifiers=None,
-        solver_options=None,
-        simulation_options=None,
-        simulation_log_level=None,
+        parameter_modifiers: Optional[Dict[str, Any]] = None,
+        solver_options: Optional[Dict[str, Any]] = None,
+        simulation_options: Optional[Dict[str, Any]] = None,
+        simulation_log_level: Optional[str] = None,
+        initialize_from: Optional[CaseOrExperiment] = None,
     ):
+        _validate_initialize_from(initialize_from)
         self._parameter_modifiers = (
             {} if parameter_modifiers is None else parameter_modifiers
         )
         self._solver_options = get_options(dict, solver_options)
         self._simulation_options = get_options(dict, simulation_options)
         self._simulation_log_level = simulation_log_level
-        self._variable_modifiers = {}
-        self._initialize_from_experiment = None
-        self._initialize_from_case = None
-        self._case_label = None
-
-    def with_modifiers(self, modifiers=None, **modifiers_kwargs):
+        self._variable_modifiers: Dict[str, Any] = {}
+        self._initialize_from = initialize_from
+        self._case_label: Optional[str] = None
+
+    def with_modifiers(
+        self, modifiers: Optional[Dict[str, Any]] = None, **modifiers_kwargs: Any
+    ) -> SimpleExperimentExtension:
         """Sets the modifiers variables for an experiment extension.
 
-        Parameters:
-
-            modifiers --
-                A dictionary of variable modifiers.
+        Args:
+            modifiers: A dictionary of variable modifiers.
 
         Example::
 
             simulation_options = custom_function.get_simulation_options()
             .with_values(ncp=500)
             solver_options = {'atol':1e-8}
             simulate_ext = SimpleExperimentExtension().with_modifiers({'PI.k': 40})
@@ -117,125 +127,119 @@
         modifiers = {} if modifiers is None else modifiers
         modifiers_aggregate = {**modifiers, **modifiers_kwargs}
         new = SimpleExperimentExtension(
             self._parameter_modifiers,
             self._solver_options,
             self._simulation_options,
             self._simulation_log_level,
+            self._initialize_from,
         )
-        new._initialize_from_experiment = self._initialize_from_experiment
-        new._initialize_from_case = self._initialize_from_case
         new._case_label = self._case_label
         for variable, value in modifiers_aggregate.items():
             if isinstance(value, Operator):
                 raise ValueError(
                     "Range operator is not supported when using extentions"
                     " in the experiment"
                 )
             new._variable_modifiers[variable] = value
         return new
 
-    def with_case_label(self, case_label):
+    def with_case_label(self, case_label: str) -> SimpleExperimentExtension:
         """Sets the case label for an experiment extension.
 
-        Parameters:
-
-            case_label --
-                A case label string.
+        Args:
+            case_label: A case label string.
 
         Example::
 
             simulation_options = custom_function.get_simulation_options()
             .with_values(ncp=500)
             solver_options = {'atol':1e-8}
             simulate_ext = SimpleExperimentExtension().with_case_label(
             'Cruise condition')
             simulate_ext = SimpleExperimentExtension(
             {'start_time': 0.0, 'final_time': 4.0},
             solver_options,
             simulation_options
             ).with_case_label('Cruise condition')
+
         """
         new = SimpleExperimentExtension(
             self._parameter_modifiers,
             self._solver_options,
             self._simulation_options,
             self._simulation_log_level,
+            self._initialize_from,
         )
-        new._initialize_from_experiment = self._initialize_from_experiment
-        new._initialize_from_case = self._initialize_from_case
         new._variable_modifiers = self._variable_modifiers
         new._case_label = case_label
 
         return new
 
-    def initialize_from(self, entity):
-        """Sets the experiment or case to initialize from for an experiment extension.
-
-        Parameters:
+    @property
+    def initialize_from(self) -> Optional[CaseOrExperiment]:
+        return self._initialize_from
+
+    def with_initialize_from(
+        self, entity: Optional[CaseOrExperiment] = None
+    ) -> SimpleExperimentExtension:
+        """Sets the experiment or case to initialize from for an experiment
+        extension.
 
-            entity --
-                "An instance of modelon.impact.client.entities.case.Case or "
-                "modelon.impact.client.entities.experiment.Experiment."
+        Args:
+            entity: An instance of Case or Experiment classes.
 
         Example::
+
             experiment = workspace.get_experiment(experiment_id)
-            simulate_ext = SimpleExperimentExtension().initialize_from(experiment)
+            simulate_ext = SimpleExperimentExtension()
+            simulate_ext.with_initialize_from(experiment)
 
             experiment = workspace.get_experiment(experiment_id)
             case = experiment.get_case('case_1')
-            simulate_ext = SimpleExperimentExtension().initialize_from(case)
+            simulate_ext = SimpleExperimentExtension()
+            simulate_ext.with_initialize_from(case)
+
         """
+        _validate_initialize_from(entity)
         new = SimpleExperimentExtension(
             self._parameter_modifiers,
             self._solver_options,
             self._simulation_options,
             self._simulation_log_level,
-        )
-        if isinstance(entity, ExternalResult):
-            raise TypeError(
-                "It is not supported to specify initialize from external result for "
-                "experiment extensions"
-            )
-
-        new._initialize_from_experiment = self._initialize_from_experiment
-        new._initialize_from_case = self._initialize_from_case
-        validate_and_set_initialize_from(entity, new)
-        assert_unique_exp_initialization(
-            new._initialize_from_experiment,
-            new._initialize_from_case,
+            entity,
         )
         new._variable_modifiers = self._variable_modifiers
         new._case_label = self._case_label
         return new
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         """Returns the experiment extensions as a dictionary.
 
         Returns:
-
-            extensions_dict --
-                A dictionary containing the experiment extensions.
+            A dictionary containing the experiment extensions.
 
         Example::
 
             fmu = model.compile().wait()
             simulation_options = custom_function.get_simulation_options()
                 .with_values(ncp=500)
             solver_options = {'atol':1e-8}
             simulate_ext = SimpleExperimentExtension(
             {'start_time': 0.0, 'final_time': 4.0},
             solver_options,
             simulation_options,
             ).with_modifiers({'PI.k': 40})
             simulate_ext.to_dict()
+
         """
-        ext_dict = {}
+        ext_dict: Dict[str, Any] = {}
         if self._variable_modifiers:
-            ext_dict["modifiers"] = {"variables": self._variable_modifiers}
+            ext_dict.setdefault("modifiers", {})
+            ext_dict["modifiers"]["variables"] = self._variable_modifiers
 
         if self._parameter_modifiers:
             ext_dict.setdefault("analysis", {})
             ext_dict["analysis"]["parameters"] = self._parameter_modifiers
 
         if self._solver_options:
             ext_dict.setdefault("analysis", {})
@@ -245,20 +249,19 @@
             ext_dict.setdefault("analysis", {})
             ext_dict["analysis"]["simulationOptions"] = self._simulation_options
 
         if self._simulation_log_level:
             ext_dict.setdefault("analysis", {})
             ext_dict["analysis"]["simulationLogLevel"] = self._simulation_log_level
 
-        if self._initialize_from_experiment:
-            ext_dict["modifiers"][
-                "initializeFrom"
-            ] = self._initialize_from_experiment.id
-
-        elif self._initialize_from_case:
+        if isinstance(self.initialize_from, ExperimentInterface):
+            ext_dict.setdefault("modifiers", {})
+            ext_dict["modifiers"]["initializeFrom"] = self.initialize_from.id
+        elif isinstance(self.initialize_from, CaseInterface):
             ext_dict["modifiers"]["initializeFromCase"] = case_to_identifier_dict(
-                self._initialize_from_case
+                self.initialize_from
             )
+
         if self._case_label:
             ext_dict["caseData"] = [{"label": self._case_label}]
 
         return ext_dict
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/experiment_definition/operators.py` & `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/operators.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,180 +1,160 @@
 """This module contains operators for parametrizing batch runs."""
-
+from typing import Any
 from abc import abstractmethod
 from dataclasses import dataclass
 
 
 class Operator:
-    """
-    Base class for an Operator.
-    """
+    """Base class for an Operator."""
 
     @abstractmethod
-    def __str__(self):
+    def __str__(self) -> str:
         "Returns a string representation of the operator"
 
 
 @dataclass
 class Range(Operator):
-    """
-    Range operator class for parameterizing batch runs.
-
-    Parameters:
-
-        start_value --
-            The start value for the sweep parameter.
-
-        end_value --
-            The end value for the sweep parameter.
+    """Range operator class for parameterizing batch runs. Range(a, b, c)
+    represents c linearly spaced values in the (real) interval [a, b]; b >= a.
+    The functionality is analogous to numpy.linspace.
+
+    Args:
+        start_value: The start value for the sweep parameter.
+        end_value: The end value for the sweep parameter.
+        no_of_steps: The number of steps to intermediate steps
+        to take between start_value and end_value.
 
-        no_of_steps --
-            The number of steps to intermediate steps to take between start_value
-            and end_value.
-
-    Examples::
+    Example::
 
         from modelon.impact.client import Range
 
         fmu = model.compile().wait()
         experiment_definition = fmu.new_experiment_definition(
             custom_function).with_modifiers({'inertia1.J': 2,
             'inertia2.J': Range(0.1, 0.5, 3)})
+
     """
 
     start_value: float
     end_value: float
     no_of_steps: int
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"range({self.start_value},{self.end_value},{self.no_of_steps})"
 
 
 class Choices(Operator):
-    """
-    Choices operator class for parameterizing batch runs.
-
-    Parameters:
+    """Choices operator class for parameterizing batch runs. Choices defines a
+    list of specified values a Modifier expression can take.
 
-        values --
-            Variable number of numerical arguments to sweep.
+    Args:
+        values: Variable number of numerical arguments to sweep.
 
-    Examples::
+    Example::
 
         from modelon.impact.client import Choices
 
         fmu = model.compile().wait()
         experiment_definition = fmu.new_experiment_definition(
             custom_function).with_modifiers({'inertia1.J': 2,
             'inertia2.J': Choices(0.1, 0.5)})
+
     """
 
-    def __init__(self, *values):
+    def __init__(self, *values: Any):
         self.values = values
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"choices({', '.join(map(str, self.values))})"
 
 
 @dataclass
 class Uniform(Operator):
-    """
-    Uniform distribution class for parameterizing batch runs.For mathematical
-    background, see e.g., https://en.wikipedia.org/wiki/Continuous_uniform_distribution
-
-    Parameters:
+    """Uniform distribution class for parameterizing batch runs.For
+    mathematical background, see e.g.,
+    https://en.wikipedia.org/wiki/Continuous_uniform_distribution.
+
+    Args:
+        start (float): Starting value of the interval.
+        end (float): End value of the interval. Requires start <= end.
 
-        start (float) --
-            Starting value of the interval.
-
-        end   (float) --
-            End value of the interval. Requires start <= end.
-
-    Examples::
+    Example::
 
         from modelon.impact.client import Uniform
 
         fmu = model.compile().wait()
         experiment_definition = fmu.new_experiment_definition(
             custom_function).with_modifiers({'inertia1.J': 2,
             'inertia2.J': Uniform(0.1, 0.5)})
+
     """
 
     start: float
     end: float
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"uniform({self.start},{self.end})"
 
 
 @dataclass
 class Beta(Operator):
-    """
-    Beta distribution class for parameterizing batch runs. For mathematical
+    """Beta distribution class for parameterizing batch runs. For mathematical
     background, see e.g., https://en.wikipedia.org/wiki/Beta_distribution.
 
-    Parameters:
+    Args:
+        alpha (float): 'alpha' resp. 'a' parameter of beta distribution, requires
+            alpha > 0
+        beta (float): 'beta' resp. 'b' parameter of beta distribution, requires
+            beta > 0
 
-        alpha  (float) --
-            'alpha' resp. 'a' parameter of beta distribution, requires alpha > 0
-
-        beta   (float) --
-            'beta' resp. 'b' parameter of beta distribution, requires beta > 0
-
-    Examples::
+    Example::
 
         from modelon.impact.client import Beta
 
         fmu = model.compile().wait()
         experiment_definition = fmu.new_experiment_definition(
             custom_function).with_modifiers({'inertia1.J': 2,
             'inertia2.J': Beta(0.1, 0.5, 3)})
+
     """
 
     alpha: float
     beta: float
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"beta({self.alpha},{self.alpha})"
 
 
 @dataclass
 class Normal(Operator):
-    """
-    Normal distribution class for parameterizing batch runs.For mathematical
+    """Normal distribution class for parameterizing batch runs.For mathematical
     background, see e.g., https://en.wikipedia.org/wiki/Normal_distribution
-    https://en.wikipedia.org/wiki/Truncated_normal_distribution
-    Supports both the standard and truncated Normal distribution.
-    The standard Normal distribution is the default, add additional start &
-    end parameters for truncation.
-
-    Parameters:
-
-        mean     (float) --
-            Mean resp. location of the distribution.
-
-        variance (float) --
-            Variance of the normal distribution. Requires var > 0.
+    https://en.wikipedia.org/wiki/Truncated_normal_distribution Supports both
+    the standard and truncated Normal distribution. The standard Normal
+    distribution is the default, add additional start & end parameters for
+    truncation.
+
+    Args:
+        mean (float): Mean resp. location of the distribution.
+        variance (float): Variance of the normal distribution. Requires var > 0.
+        start (float): Lower bound. Default: -inf
+        end (float): Upper bound, requires end > start. Default: inf
 
-        start    (float) --
-            Lower bound. Default: -inf
-
-        end      (float)
-            Upper bound, requires end > start. Default: inf
-
-    Examples::
+    Example::
 
         from modelon.impact.client import Normal
 
         fmu = model.compile().wait()
         experiment_definition = fmu.new_experiment_definition(
             custom_function).with_modifiers({'inertia1.J': 2,
             'inertia2.J': Normal(0.1, 0.5)})
+
     """
 
     mean: float
     variance: float
     start: float = float('-inf')
     end: float = float('inf')
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"normal({self.mean},{self.variance},{self.start},{self.end})"
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/jupyterhub/authorize.py` & `modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/authorize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,83 @@
 import logging
-
+import os
+from typing import Optional, Tuple
 from modelon.impact.client.credential_manager import CredentialManager
 from modelon.impact.client.jupyterhub import exceptions
 from modelon.impact.client.jupyterhub import sal
-
+from modelon.impact.client.sal.context import Context
+from modelon.impact.client.sal.uri import URI
 
 logger = logging.getLogger(__name__)
 
 
-def _get_jupyter_token(credential_manager, interactive, context=None):
+def _get_jupyter_token(credential_manager: CredentialManager, interactive: bool) -> str:
     jupyter_token = credential_manager.get_key(interactive=interactive)
     if not jupyter_token:
         raise exceptions.NoJupyterHubTokenError("No JupyterHub API token is given")
 
     return jupyter_token
 
 
-def authorize(uri, interactive, context=None, credential_manager=None, service=None):
+def _running_in_jupyterhub_environment() -> bool:
+    return os.environ.get("JUPYTERHUB_SERVICE_PREFIX") is not None
+
+
+def _running_with_same_jupyterhub_server(uri: URI) -> bool:
+    return str(uri) in os.environ.get('IMPACT_URL', '')
+
+
+def authorize(
+    uri: URI,
+    interactive: bool,
+    context: Optional[Context] = None,
+    credential_manager: Optional[CredentialManager] = None,
+    service: Optional[sal.JupyterHubService] = None,
+) -> Tuple[URI, sal.JupyterContext]:
+
+    jupyter_context = sal.JupyterContext(base=context)
+    service = service or sal.JupyterHubService()
+
+    if _running_in_jupyterhub_environment() and _running_with_same_jupyterhub_server(
+        uri
+    ):
+        jupyter_context.token = os.environ.get('JUPYTERHUB_API_TOKEN', '')
+        server = os.environ.get('JUPYTERHUB_SERVICE_PREFIX')
+        user = service.get_user_data(uri, jupyter_context, server)
+        return user.impact_server_uri(uri), jupyter_context
+
+    help_text = f"Enter JupyterHub API token (can be generated at {uri / 'token'}):"
     credential_manager = credential_manager or CredentialManager(
         file_id="jupyterhub-api.key",
-        env_name="MODELON_IMPACT_JUPYTERHUB_CLIENT_API_TOKEN",
-        interactive_help_text="Enter JupyterHub API token:",
+        env_names=[
+            "JUPYTERHUB_API_TOKEN",
+            "MODELON_IMPACT_JUPYTERHUB_CLIENT_API_TOKEN",
+        ],
+        interactive_help_text=help_text,
     )
-    context = sal.JupyterContext(base=context)
-    service = service or sal.JupyterHubService()
 
     try:
-        context.token = _get_jupyter_token(credential_manager, interactive)
-        user = service.get_user_data(uri, context)
+        jupyter_context.token = _get_jupyter_token(credential_manager, interactive)
+        user = service.get_user_data(uri, jupyter_context)
     except exceptions.JupyterHubAuthrizationError:
         if interactive:
             logger.warning(
                 "Could not authorize with the provided JupyterHub API token, "
                 "please enter a new token"
             )
-            context.token = credential_manager.get_key_from_prompt()
-            user = service.get_user_data(uri, context)
+            jupyter_context.token = credential_manager.get_key_from_prompt()
+            user = service.get_user_data(uri, jupyter_context)
         else:
             raise
 
-    if interactive:
-        credential_manager.write_key_to_file(context.token)
+    jupyter_token = jupyter_context.token
+    if interactive and jupyter_token:
+        credential_manager.write_key_to_file(jupyter_token)
 
     if not user.server_running():
         uri_to_start_server = uri / 'hub/home'
         raise exceptions.NoJupyterHubServerRunningError(
             "The user does not have a server running. "
             f"Go to {uri_to_start_server} and start a server."
         )
 
-    return user.impact_server_uri(uri), context
+    return user.impact_server_uri(uri), jupyter_context
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/jupyterhub/sal.py` & `modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/sal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,83 @@
 import json.decoder
-
+from typing import Optional
 import requests
 
 from modelon.impact.client.jupyterhub import exceptions
 from modelon.impact.client.sal.context import Context
+from modelon.impact.client.sal.uri import URI
 
 
 class JupyterContext:
-    def __init__(self, base=None):
+    __slots__ = ['_base', '_token']
+
+    def __init__(self, base: Optional[Context] = None):
         self._base = base if base else Context()
-        self._token = None
+        self._token: Optional[str] = None
 
     @property
-    def session(self):
+    def session(self) -> requests.Session:
         return self._base.session
 
     @property
-    def token(self):
+    def token(self) -> Optional[str]:
         return self._token
 
     @token.setter
-    def token(self, token):
+    def token(self, token: str) -> None:
         self._token = token
         self.session.headers.update({'Authorization': 'token %s' % token})
 
 
 class JupyterUser:
-    def __init__(self, user_id, server):
+    def __init__(self, user_id: str, server: Optional[str]):
         self.id = user_id
         self._server = server
 
-    def server_running(self):
+    def server_running(self) -> bool:
         return self._server is not None
 
-    def impact_server_uri(self, jupyterhub_uri):
+    def impact_server_uri(self, jupyterhub_uri: URI) -> URI:
         return jupyterhub_uri / f'user/{self.id}/impact'
 
 
 class JupyterHubService:
     @classmethod
-    def get_user_data(cls, uri, context):
+    def get_user_data(
+        cls, uri: URI, context: JupyterContext, server: Optional[str] = None
+    ) -> JupyterUser:
         auth_token_url = (
             uri / f'hub/api/authorizations/token/{context.token}'
         ).resolve()
 
         try:
-            user_respons = context.session.get(auth_token_url)
+            user_response = context.session.get(auth_token_url)
         except requests.exceptions.RequestException as e:
             raise exceptions.NotAJupyterHubUrl(
                 f"Did not get a response from {uri}, is the URL correct?"
             ) from e
 
-        if not user_respons.ok:
-            if user_respons.status_code == 403:
+        if not user_response.ok:
+            if user_response.status_code == 403:
                 raise exceptions.JupyterHubAuthrizationError(
                     "Could not authorize against JupyterHub, is the token correct?"
                 )
-            elif user_respons.status_code == 404:
+            elif user_response.status_code == 404:
                 raise exceptions.NotAJupyterHubUrl(
                     f"Missing resource '{auth_token_url}'. Possible errors are "
                     f"that the URL '{uri}' don't points to a JupyterHub or "
                     "that the user of the API key as been deleted."
                 )
             else:
                 raise exceptions.UnknownJupyterHubError(
                     "Something went wrong calling JupyterHub. Got the response "
-                    f"'{user_respons}' with content '{user_respons.content}'"
+                    f"'{user_response}' with content '{str(user_response.content)}'"
                 )
 
         try:
-            user_data = user_respons.json()
-            return JupyterUser(user_data['name'], user_data['server'])
+            user_data = user_response.json()
+            return JupyterUser(user_data['name'], user_data.get('server', server))
         except (KeyError, json.decoder.JSONDecodeError) as e:
             raise exceptions.NotAJupyterHubUrl(
                 "User response data is not correct, "
                 f"is the URL '{uri}' for a JupyterHub?"
             ) from e
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/base.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,193 +1,197 @@
+from __future__ import annotations
 import enum
 import time
 import logging
 
-from abc import ABC, abstractmethod
-from typing import Any, Optional
+from abc import abstractmethod
+from typing import Any, Optional, TypeVar, Protocol, Generic
 from modelon.impact.client import exceptions
 
 logger = logging.getLogger(__name__)
+Entity = TypeVar("Entity")
+
+
+class EntityFromOperation(Protocol[Entity]):
+    def __call__(self, operation: BaseOperation[Entity], **kwargs: Any) -> Entity:
+        ...
 
 
 @enum.unique
 class Status(enum.Enum):
-    """
-    Class representing an enumeration for the possible
-    operation states.
-    """
+    """Class representing an enumeration for the possible operation states."""
 
     PENDING = "pending"
+    """Status for an operation that is pending."""
+
     RUNNING = "running"
+    """Status for an operation that is running."""
+
     STOPPING = "stopping"
+    """Status for an operation that has been cancelled and is stopping."""
+
     CANCELLED = "cancelled"
+    """Status for an operation that has been cancelled."""
+
     DONE = "done"
+    """Status for an operation that has been completed."""
 
 
 @enum.unique
 class AsyncOperationStatus(enum.Enum):
-    """
-    Defines all states for import
-    """
+    """Defines all states for import."""
 
     RUNNING = 'running'
+    """Status for an async operation that is running."""
+
     READY = 'ready'
+    """Status for an async operation that is ready."""
+
     ERROR = 'error'
+    """Status for an async operation that has errors."""
 
-    def done(self):
+    def done(self) -> bool:
         return self in [AsyncOperationStatus.READY, AsyncOperationStatus.ERROR]
 
 
-class BaseOperation(ABC):
-    """
-    Abstract base operation class.
-    """
+class BaseOperation(Generic[Entity]):
+    """Abstract base operation class."""
+
+    def __init__(self, create_entity: EntityFromOperation):
+        self._create_entity = create_entity
 
     @abstractmethod
-    def data(self):
-        """
-        Returns the operation class.
-        """
+    def data(self) -> Entity:
+        """Returns the Entity class."""
         pass
 
+    @property
     @abstractmethod
-    def status(self):
-        """
-        Returns the operation status as an enumeration.
-        """
+    def status(self) -> Any:
+        """Returns the operation status as an enumeration."""
         pass
 
     @abstractmethod
-    def cancel(self):
-        """
-        Terminates the operation.
-        """
+    def cancel(self) -> Any:
+        """Terminates the operation."""
         pass
 
     @property
     @abstractmethod
     def name(self) -> str:
-        """
-        Name of the operation.
-        """
+        """Name of the operation."""
         pass
 
     @abstractmethod
-    def wait(self, timeout):
-        """
-        Waits for the operation to finish.
-        """
+    def wait(self, timeout: Optional[float]) -> Entity:
+        """Waits for the operation to finish."""
         pass
 
 
-class AsyncOperation(BaseOperation):
-    """
-    File operation class containing base functionality.
-    """
-
-    def wait(self, timeout: Optional[float] = None) -> Any:
-        """Waits until the operation completes.
-        Returns the operation class instance if operation completes.
+class AsyncOperation(BaseOperation[Entity]):
+    """File operation class containing base functionality."""
 
-        Parameters:
+    def wait(self, timeout: Optional[float] = None) -> Entity:
+        """Waits until the operation completes. Returns the operation class
+        instance if operation completes.
 
-            timeout --
-                Time to wait in seconds for achieving the status. By default
+        Args:
+            timeout: Time to wait in seconds for achieving the status. By default
                 the timeout is set to 'None', which signifies an infinite time
                 to wait until the status is achieved.
 
         Returns:
 
-            Operation class instance if operation completes.
+            Entity class instance if operation completes.
 
         Raises:
-
             OperationTimeOutError if time exceeds set timeout.
 
         Example::
 
-            workspace.upload_result('C:/A.mat').wait(timeout = 120)
+            workspace.upload_result('A.mat').wait(timeout = 120)
+
         """
         start_t = time.time()
         while True:
-            logger.info(f"{self.name} in progress! Status : {self.status().name}")
-            if self.status().done():
-                logger.info(f"{self.name} completed! Status : {self.status().name}")
+            logger.info(f"{self.name} in progress! Status : {self.status.name}")
+            if self.status.done():
+                logger.info(f"{self.name} completed! Status : {self.status.name}")
                 return self.data()
 
             current_t = time.time()
             if timeout and current_t - start_t > timeout:
                 raise exceptions.OperationTimeOutError(
                     f"Time exceeded the set timeout - {timeout}s! "
-                    f"Present status of operation is {self.status().name}!"
+                    f"Present status of operation is {self.status.name}!"
                 )
 
             time.sleep(0.5)
 
+    def cancel(self) -> None:
+        raise NotImplementedError('Cancel is not supported for this operation')
 
-class ExecutionOperation(BaseOperation):
-    """
-    Execution operation class containing base functionality.
-    """
+
+class ExecutionOperation(BaseOperation[Entity]):
+    """Execution operation class containing base functionality."""
 
     def is_complete(self) -> bool:
-        """
-        Returns True if the operation has completed.
+        """Returns True if the operation has completed.
 
         Returns:
-
-            True -> If operation has completed.
-            False -> If operation has not completed.
+            True, if operation has completed.False, if operation has
+            not completed.
 
         Example::
 
            model.compile(options).is_complete()
            workspace.execute(definition).is_complete()
-        """
-        return self.status() == Status.DONE
 
-    def wait(self, timeout: Optional[float] = None, status: Status = Status.DONE):
-        """Waits until the operation achieves the set status.
-        Returns the operation class instance if the set status is achieved.
+        """
+        return self.status == Status.DONE
 
-        Parameters:
+    def wait(
+        self, timeout: Optional[float] = None, status: Status = Status.DONE
+    ) -> Entity:
+        """Waits until the operation achieves the set status. Returns the
+        operation class instance if the set status is achieved.
 
-            timeout --
-                Time to wait in seconds for achieving the status. By default
+        Args:
+            timeout: Time to wait in seconds for achieving the status. By default
                 the timeout is set to 'None', which signifies an infinite time
                 to wait until the status is achieved.
 
-            status --
+            status:
                 Operation status to be achieved.
                 Default: Status.DONE
 
         Returns:
 
-            Operation class instance if the set status is achieved.
+            Entity class instance if the set status is achieved.
 
         Raises:
-
             OperationTimeOutError if time exceeds set timeout.
 
         Example::
 
            model.compile(compile_options).wait(
                timeout = 120,
                status = Status.CANCELLED
            )
            workspace.execute(experiment_definition).wait(timeout = 120)
+
         """
         start_t = time.time()
         while True:
-            logger.info(f"{self.name} in progress! Status : {self.status().name}")
-            if self.status() == status:
-                logger.info(f"{self.name} completed! Status : {self.status().name}")
+            logger.info(f"{self.name} in progress! Status : {self.status.name}")
+            if self.status == status:
+                logger.info(f"{self.name} completed! Status : {self.status.name}")
                 return self.data()
 
             current_t = time.time()
             if timeout and current_t - start_t > timeout:
                 raise exceptions.OperationTimeOutError(
                     f"Time exceeded the set timeout - {timeout}s! "
-                    f"Present status of operation is {self.status().name}!"
+                    f"Present status of operation is {self.status.name}!"
                 )
 
             time.sleep(0.5)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/case.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/experiment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,79 +1,81 @@
-from modelon.impact.client.entities import case
-from modelon.impact.client.operations.base import ExecutionOperation, Status
-from modelon.impact.client.sal.service import Service
-
-
-class CaseOperation(ExecutionOperation):
-    """
-    An operation class for the modelon.impact.client.entities.Case class.
-    """
-
-    def __init__(self, workspace_id, exp_id, case_id, service: Service):
-        super().__init__()
+from __future__ import annotations
+from typing import TYPE_CHECKING
+from modelon.impact.client.operations.base import ExecutionOperation, Entity, Status
+
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import EntityFromOperation
+
+
+class ExperimentOperation(ExecutionOperation[Entity]):
+    """An operation class for the Experiment class."""
+
+    def __init__(
+        self,
+        workspace_id: str,
+        exp_id: str,
+        service: Service,
+        create_entity: EntityFromOperation,
+    ):
+        super().__init__(create_entity)
         self._workspace_id = workspace_id
         self._exp_id = exp_id
-        self._case_id = case_id
         self._sal = service
+        self._create_entity = create_entity
 
-    def __repr__(self):
-        return f"Case operation for id '{self._case_id}'"
+    def __repr__(self) -> str:
+        return f"Experiment operation for id '{self._exp_id}'"
 
-    def __eq__(self, obj):
-        return isinstance(obj, CaseOperation) and obj._case_id == self._case_id
+    def __eq__(self, obj: object) -> bool:
+        return isinstance(obj, ExperimentOperation) and obj._exp_id == self._exp_id
 
     @property
-    def id(self):
-        """Case id"""
-        return self._case_id
+    def id(self) -> str:
+        """Experiment id."""
+        return self._exp_id
 
     @property
-    def name(self):
-        """Return the name of operation"""
+    def name(self) -> str:
+        """Return the name of operation."""
         return "Execution"
 
-    def data(self):
-        """
-        Returns a new Case class instance.
+    def data(self) -> Entity:
+        """Returns a new Experiment class instance.
 
         Returns:
+            An experiment class instance.
 
-            experiment --
-                An Case class instance.
         """
-        case_data = self._sal.experiment.case_get(
-            self._workspace_id, self._exp_id, self._case_id
-        )
-        return case.Case(
-            self._case_id, self._workspace_id, self._exp_id, self._sal, case_data
+        return self._create_entity(
+            self, workspace_id=self._workspace_id, exp_id=self._exp_id
         )
 
-    def status(self):
-        """
-        Returns the execution status as an enumeration.
+    @property
+    def status(self) -> Status:
+        """Returns the execution status as an enumeration.
 
         Returns:
-
-            status --
-                The execution status enum. The status can have the enum values
-                Status.PENDING, Status.RUNNING, Status.STOPPING, Status.CANCELLED
-                or Status.DONE
+            The execution status enum. The status can have the enum values
+            Status.PENDING, Status.RUNNING, Status.STOPPING, Status.CANCELLED
+            or Status.DONE
 
         Example::
 
-            case.execute().status()
+            workspace.execute(definition).status
+
         """
         return Status(
             self._sal.experiment.execute_status(self._workspace_id, self._exp_id)[
                 "status"
             ]
         )
 
-    def cancel(self):
-        """
-        Terminates the execution process.
+    def cancel(self) -> None:
+        """Terminates the execution process.
 
         Example::
 
-            case.execute().cancel()
+            workspace.execute(definition).cancel()
+
         """
         self._sal.experiment.execute_cancel(self._workspace_id, self._exp_id)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/content_import.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/project_import.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,83 @@
+from __future__ import annotations
+from typing import Dict, Any, TYPE_CHECKING
 from modelon.impact.client.sal.service import Service
-from modelon.impact.client.operations.base import AsyncOperation, AsyncOperationStatus
+from modelon.impact.client.operations.base import (
+    AsyncOperation,
+    AsyncOperationStatus,
+    Entity,
+)
 from modelon.impact.client import exceptions
-from modelon.impact.client.entities.content import ProjectContent
 
+if TYPE_CHECKING:
+    from modelon.impact.client.operations.base import EntityFromOperation
 
-class ContentImportOperation(AsyncOperation):
-    """
-    An operation class for the modelon.impact.client.entities.project.ProjectContent
-    class.
-    """
 
-    def __init__(self, location: str, service: Service):
-        super().__init__()
+class ProjectImportOperation(AsyncOperation[Entity]):
+    """An import operation class for the Project class."""
+
+    def __init__(
+        self, location: str, service: Service, create_entity: EntityFromOperation
+    ):
+        super().__init__(create_entity)
         self._location = location
         self._sal = service
+        self._create_entity = create_entity
 
-    def __repr__(self):
-        return f"Content import operations for id '{self.id}'"
+    def __repr__(self) -> str:
+        return f"Project import operations for id '{self.id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return (
-            isinstance(obj, ContentImportOperation) and obj._location == self._location
+            isinstance(obj, ProjectImportOperation) and obj._location == self._location
         )
 
     @property
-    def id(self):
-        """Content import id"""
+    def id(self) -> str:
+        """Project import id."""
         return self._location.split('/')[-1]
 
     @property
-    def name(self):
-        """Return the name of operation"""
-        return "Content import"
-
-    def cancel(self):
-        raise NotImplementedError('Cancel is not supported for this operation')
+    def name(self) -> str:
+        """Return the name of operation."""
+        return "Project import"
 
-    def _info(self):
-        return self._sal.project.project_content_upload_status(self._location)["data"]
+    def _info(self) -> Dict[str, Any]:
+        return self._sal.imports.get_import_status(self._location)["data"]
 
-    def data(self):
-        """
-        Returns a new Workspace class instance.
+    def data(self) -> Entity:
+        """Returns a new Project class instance.
 
         Returns:
+            A Project class instance.
 
-            workspace --
-                A Workspace class instance.
         """
         info = self._info()
         if info['status'] == AsyncOperationStatus.ERROR.value:
-            raise exceptions.IllegalContentImport(
-                f"Content import failed! Cause: {info['error'].get('message')}"
+            raise exceptions.IllegalProjectImport(
+                f"Project import failed! Cause: {info['error'].get('message')}"
             )
         project_id = info["data"]["projectId"]
-        content_id = info["data"]["contentId"]
-        resp = self._sal.project.project_content_get(project_id, content_id)
-        return ProjectContent(resp, project_id, self._sal)
+        resp = self._sal.project.project_get(project_id, False, False)
+        return self._create_entity(
+            self,
+            project_id=resp["id"],
+            project_definition=resp["definition"],
+            project_type=resp["projectType"],
+        )
 
-    def status(self):
-        """
-        Returns the upload status as an enumeration.
+    @property
+    def status(self) -> AsyncOperationStatus:
+        """Returns the upload status as an enumeration.
 
         Returns:
-
-            upload_status --
-                The AsyncOperationStatus enum. The status can have the enum values
-                AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
-                AsyncOperationStatus.ERROR
+            The AsyncOperationStatus enum. The status can have the enum values
+            AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
+            AsyncOperationStatus.ERROR
 
         Example::
 
-            project.upload_content('path/to/model.mo').status()
+            status = client.import_project_from_zip(path_to_project).status
+            status = workspace.import_project_from_zip(path_to_project).status
+
         """
         return AsyncOperationStatus(self._info()["status"])
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/external_result.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/external_result_import.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-from modelon.impact.client import exceptions
-from modelon.impact.client.entities.external_result import ExternalResult
-from modelon.impact.client.sal.service import Service
-from modelon.impact.client.operations.base import AsyncOperation, AsyncOperationStatus
-
+from __future__ import annotations
+from typing import Dict, Any, TYPE_CHECKING
 
-class ExternalResultUploadOperation(AsyncOperation):
-    """
-    An operation class for the modelon.impact.client.entities.
-    external_result.ExternalResult class.
-    """
-
-    def __init__(self, result_id: str, service: Service):
-        super().__init__()
-        self._result_id = result_id
+from modelon.impact.client import exceptions
+from modelon.impact.client.operations.base import (
+    AsyncOperation,
+    AsyncOperationStatus,
+    Entity,
+)
+
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import EntityFromOperation
+
+
+class ExternalResultImportOperation(AsyncOperation[Entity]):
+    """An operation class for the ExternalResult class."""
+
+    def __init__(
+        self, location: str, service: Service, create_entity: EntityFromOperation
+    ):
+        super().__init__(create_entity)
+        self._location = location
         self._sal = service
+        self._create_entity = create_entity
 
-    def __repr__(self):
-        return f"Result upload operations for id '{self._result_id}'"
+    def __repr__(self) -> str:
+        return f"Result import operations for id '{self.id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return (
-            isinstance(obj, ExternalResultUploadOperation)
-            and obj._result_id == self._result_id
+            isinstance(obj, ExternalResultImportOperation)
+            and obj._location == self._location
         )
 
     @property
-    def id(self):
-        """Result id"""
-        return self._result_id
+    def id(self) -> str:
+        """Result import id."""
+        return self._location.split('/')[-1]
 
     @property
-    def name(self):
-        """Return the name of operation"""
-        return "Result upload"
+    def name(self) -> str:
+        """Return the name of operation."""
+        return "Result import"
 
-    def cancel(self):
-        raise NotImplementedError('Cancel is not supported for this operation')
+    def _info(self) -> Dict[str, Any]:
+        return self._sal.imports.get_import_status(self._location)["data"]
 
-    def _info(self):
-        return self._sal.workspace.get_result_upload_status(self._result_id)["data"]
-
-    def data(self):
-        """
-        Returns a new ExternalResult class instance.
+    def data(self) -> Entity:
+        """Returns a new ExternalResult class instance.
 
         Returns:
+            A ExternalResult class instance.
 
-            external_result --
-                A ExternalResult class instance.
         """
         info = self._info()
         if info['status'] == AsyncOperationStatus.ERROR.value:
             raise exceptions.ExternalResultUploadError(
                 f"External result upload failed! Cause: {info['error'].get('message')}"
             )
+        resp = self._sal.external_result.get_uploaded_result(self.id)
+        return self._create_entity(self, result_id=resp['data']['id'])
 
-        return ExternalResult(self._result_id, self._sal)
-
-    def status(self):
-        """
-        Returns the upload status as an enumeration.
+    @property
+    def status(self) -> AsyncOperationStatus:
+        """Returns the upload status as an enumeration.
 
         Returns:
-
-            upload_status --
-                The AsyncOperationStatus enum. The status can have the enum values
-                AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
-                AsyncOperationStatus.ERROR
+            The AsyncOperationStatus enum. The status can have the enum values
+            AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
+            AsyncOperationStatus.ERROR
 
         Example::
 
-            workspace.upload_result('C:/A.mat').status()
+            workspace.upload_result('A.mat').status
+
         """
         return AsyncOperationStatus(self._info()["status"])
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/model_executable.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/model_executable.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,193 +1,201 @@
+from __future__ import annotations
 import logging
-from typing import Dict, Optional, Any
-from modelon.impact.client.entities.model_executable import ModelExecutable
-from modelon.impact.client.sal.service import Service
-from modelon.impact.client.operations.base import ExecutionOperation, Status
+from typing import Dict, Optional, Any, TYPE_CHECKING
+
+from modelon.impact.client.operations.base import ExecutionOperation, Status, Entity
 from modelon.impact.client import exceptions
 
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import EntityFromOperation
+
 logger = logging.getLogger(__name__)
 
 
-class CachedModelExecutableOperation(ExecutionOperation):
-    """
-    An operation class for a cached modelon.impact.client.entities.
-    model_executable.ModelExecutable class.
-    """
+class CachedModelExecutableOperation(ExecutionOperation[Entity]):
+    """An operation class for a cached ModelExecutable class."""
 
     def __init__(
         self,
         workspace_id: str,
         fmu_id: str,
         service: Service,
+        create_entity: EntityFromOperation,
         info: Optional[Dict[str, Any]] = None,
         modifiers: Optional[Dict[str, Any]] = None,
     ):
-        super().__init__()
+        super().__init__(create_entity)
         self._workspace_id = workspace_id
         self._fmu_id = fmu_id
         self._sal = service
         self._info = info
         self._modifiers = modifiers
+        self._create_entity = create_entity
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Cached model executable operations for id '{self._fmu_id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return (
             isinstance(obj, CachedModelExecutableOperation)
             and obj._fmu_id == self._fmu_id
         )
 
     @property
-    def id(self):
-        """FMU id"""
+    def id(self) -> str:
+        """FMU id."""
         return self._fmu_id
 
     @property
-    def name(self):
-        """Return the name of operation"""
+    def name(self) -> str:
+        """Return the name of operation."""
         return "Looking for cached FMU"
 
-    def data(self):
-        """
-        Returns a new ModelExecutable class instance.
+    def data(self) -> Entity:
+        """Returns a new ModelExecutable class instance.
 
         Returns:
+            A model_executable class instance.
 
-            model_executable --
-                A model_executable class instance.
         """
-        return ModelExecutable(
-            self._workspace_id, self._fmu_id, self._sal, self._info, self._modifiers
+        return self._create_entity(
+            self,
+            workspace_id=self._workspace_id,
+            fmu_id=self._fmu_id,
+            info=self._info,
+            modifiers=self._modifiers,
         )
 
-    def status(self):
-        """
-        Returns the compilation status as an enumeration.
+    @property
+    def status(self) -> Status:
+        """Returns the compilation status as an enumeration.
 
         Returns:
-
-            status --
-                The compilation status enum. The status has the enum value
-                Status.DONE as a cached FMU is only possible for a
-                successfully finished compilation.
+            The compilation status enum. The status has the enum value
+            Status.DONE as a cached FMU is only possible for a
+            successfully finished compilation.
 
         Example::
 
-            model.compile(options).status()
+            model.compile(options).status
+
         """
         return Status.DONE
 
-    def cancel(self):
+    def cancel(self) -> None:
         raise NotImplementedError(
             "Cancel is not supported for CachedModelExecutableOperation class"
         )
 
-    def wait(self, timeout=None, status=Status.DONE):
-        """Waits until the operation achieves the set status.
-        Returns the operation class instance if the set status is achieved.
-
-        Parameters:
+    def wait(
+        self, timeout: Optional[float] = None, status: Status = Status.DONE
+    ) -> Entity:
+        """Waits until the operation achieves the set status. Returns the
+        operation class instance if the set status is achieved.
 
-            timeout --
-                Time to wait in seconds for achieving the status.This argument is
+        Args:
+            timeout: Time to wait in seconds for achieving the status.This argument is
                 not accounted for the CachedModelExecutableOperation class as the
                 model has a successfully compiled status(Status.DONE) in this class.
 
-            status --
+            status:
                 Operation status to be achieved. The only possible status for the
                 CachedModelExecutableOperation class is Status.DONE as cached FMU
-                is only avaiable for a successfully compiled model.
+                is only available for a successfully compiled model.
 
         Returns:
 
-            Operation class instance if the set status is achieved.
+            Entity class instance if the set status is achieved.
 
         Raises:
 
             OperationTimeOutError if operation status is not set as Status.DONE.
 
         Example::
 
            model.compile(compile_options).wait()
+
         """
 
-        if self.status() != status:
+        if self.status != status:
             raise exceptions.OperationTimeOutError(
-                f"The operation '{self.name}' has the status '{self.status().name}'"
+                f"The operation '{self.name}' has the status '{self.status.name}'"
                 f", it will never get the status '{status.name}'!"
             )
 
         logger.info("Cached FMU found! Using the cached FMU!")
         return self.data()
 
 
-class ModelExecutableOperation(ExecutionOperation):
-    """
-    An operation class for the modelon.impact.client.entities.
-    model_executable.ModelExecutable class.
-    """
+class ModelExecutableOperation(ExecutionOperation[Entity]):
+    """An operation class for the ModelExecutable class."""
 
-    def __init__(self, workspace_id: str, fmu_id: str, service: Service):
-        super().__init__()
+    def __init__(
+        self,
+        workspace_id: str,
+        fmu_id: str,
+        service: Service,
+        create_entity: EntityFromOperation,
+    ):
+        super().__init__(create_entity)
         self._workspace_id = workspace_id
         self._fmu_id = fmu_id
         self._sal = service
+        self._create_entity = create_entity
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Model executable operations for id '{self._fmu_id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return isinstance(obj, ModelExecutableOperation) and obj._fmu_id == self._fmu_id
 
     @property
-    def id(self):
-        """FMU id"""
+    def id(self) -> str:
+        """FMU id."""
         return self._fmu_id
 
     @property
-    def name(self):
-        """Return the name of operation"""
+    def name(self) -> str:
+        """Return the name of operation."""
         return "Compilation"
 
-    def data(self):
-        """
-        Returns a new ModelExecutable class instance.
+    def data(self) -> Entity:
+        """Returns a new ModelExecutable class instance.
 
         Returns:
+            A ModelExecutable class instance.
 
-            model_executable --
-                A model_executable class instance.
         """
-        return ModelExecutable(self._workspace_id, self._fmu_id, self._sal)
+        return self._create_entity(
+            self, workspace_id=self._workspace_id, fmu_id=self._fmu_id
+        )
 
-    def status(self):
-        """
-        Returns the compilation status as an enumeration.
+    @property
+    def status(self) -> Status:
+        """Returns the compilation status as an enumeration.
 
         Returns:
-
-            status --
-                The compilation status enum. The status can have the enum values
-                Status.PENDING, Status.RUNNING, Status.STOPPING, Status.CANCELLED
-                or Status.DONE
+            The compilation status enum. The status can have the enum values
+            Status.PENDING, Status.RUNNING, Status.STOPPING, Status.CANCELLED
+            or Status.DONE
 
         Example::
 
-            model.compile(options).status()
+            model.compile(options).status
+
         """
         return Status(
             self._sal.model_executable.compile_status(self._workspace_id, self._fmu_id)[
                 "status"
             ]
         )
 
-    def cancel(self):
-        """
-        Terminates the compilation process.
+    def cancel(self) -> None:
+        """Terminates the compilation process.
 
         Example::
 
             model.compile(options).cancel()
+
         """
         self._sal.model_executable.compile_cancel(self._workspace_id, self._fmu_id)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/conversion.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/imports.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,76 +1,81 @@
+from __future__ import annotations
+from typing import Dict, Any, TYPE_CHECKING
+
+from modelon.impact.client.operations.base import (
+    AsyncOperation,
+    AsyncOperationStatus,
+    Entity,
+)
 from modelon.impact.client import exceptions
-from modelon.impact.client.entities.workspace import Workspace, WorkspaceDefinition
-from modelon.impact.client.operations.base import AsyncOperation, AsyncOperationStatus
-from modelon.impact.client.sal.service import Service
 
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import EntityFromOperation
 
-class WorkspaceConversionOperation(AsyncOperation):
-    """
-    An conversion operation class for the modelon.impact.client.entities.workspace.
-    Workspace class.
-    """
 
-    def __init__(self, location: str, service: Service):
-        super().__init__()
+class WorkspaceImportOperation(AsyncOperation[Entity]):
+    """An import operation class for the Workspace class."""
+
+    def __init__(
+        self, location: str, service: Service, create_entity: EntityFromOperation
+    ):
+        super().__init__(create_entity)
         self._location = location
         self._sal = service
+        self._create_entity = create_entity
 
-    def __repr__(self):
-        return f"Workspace conversion operations for id '{self.id}'"
+    def __repr__(self) -> str:
+        return f"Workspace import operations for id '{self.id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return (
-            isinstance(obj, WorkspaceConversionOperation)
+            isinstance(obj, WorkspaceImportOperation)
             and obj._location == self._location
         )
 
     @property
-    def id(self):
-        """Workspace conversion id"""
+    def id(self) -> str:
+        """Workspace import id."""
         return self._location.split('/')[-1]
 
     @property
-    def name(self):
-        """Return the name of operation"""
-        return "Workspace conversion"
-
-    def cancel(self):
-        raise NotImplementedError('Cancel is not supported for this operation')
-
-    def _info(self):
-        return self._sal.workspace.get_workspace_conversion_status(self._location)[
-            "data"
-        ]
+    def name(self) -> str:
+        """Return the name of operation."""
+        return "Workspace import"
 
-    def data(self):
-        """
-        Returns a Workspace class instance of the converted workspace.
+    def _info(self) -> Dict[str, Any]:
+        return self._sal.imports.get_import_status(self._location)["data"]
+
+    def data(self) -> Entity:
+        """Returns a new Workspace class instance.
 
         Returns:
+            A Workspace class instance.
 
-            An Workspace class instance.
         """
         info = self._info()
         if info['status'] == AsyncOperationStatus.ERROR.value:
-            raise exceptions.IllegalWorkspaceConversion(
-                f"Workspace conversion failed! Cause: {info['error'].get('message')}"
+            raise exceptions.IllegalWorkspaceImport(
+                f"Workspace import failed! Cause: {info['error'].get('message')}"
             )
-
         workspace_id = info["data"]["workspaceId"]
-        resp = self._sal.workspace.workspace_get(workspace_id)
-        return Workspace(resp["id"], WorkspaceDefinition(resp["definition"]), self._sal)
+        resp = self._sal.workspace.workspace_get(workspace_id, False)
+        return self._create_entity(
+            self, workspace_id=resp["id"], workspace_definition=resp["definition"]
+        )
 
-    def status(self):
-        """
-        Returns the conversion status as an enumeration.
+    @property
+    def status(self) -> AsyncOperationStatus:
+        """Returns the upload status as an enumeration.
 
         Returns:
             The AsyncOperationStatus enum. The status can have the enum values
             AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
             AsyncOperationStatus.ERROR
 
         Example::
 
-            client.convert_workspace(workspace_id).status()
+            client.import_workspace_from_shared_definition(definition, False).status
+
         """
         return AsyncOperationStatus(self._info()["status"])
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/exports.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/exports.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,111 @@
+from __future__ import annotations
 import os
-from modelon.impact.client.sal.service import Service
-from modelon.impact.client.operations.base import AsyncOperation, AsyncOperationStatus
+from typing import Dict, Any, TYPE_CHECKING
+from modelon.impact.client.operations.base import (
+    AsyncOperation,
+    AsyncOperationStatus,
+    Entity,
+    BaseOperation,
+)
 from modelon.impact.client import exceptions
 
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.exports import ExportService
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import EntityFromOperation
+
 
 class Export:
-    def __init__(self, export_service, download_uri):
+    def __init__(self, export_service: ExportService, download_uri: str):
         self._export_sal = export_service
         self._download_uri = download_uri
 
-    def download_as(self, path_to_download):
-        """Writes the binary archive to a file.
-        Returns the path to downloaded archive.
-
-        Parameters:
+    def download_as(self, path_to_download: str) -> str:
+        """Writes the binary archive to a file. Returns the path to downloaded
+        archive.
 
-            path_to_download --
-                The path to store the downloaded workspace.
+        Args:
+            path_to_download: The path to store the downloaded workspace.
 
         Returns:
-
-            path --
-                Local path to the downloaded archive.
+            local path to the downloaded archive.
 
         Example::
 
-            path = workspace.export(options).wait().download_as('/home/workspace.zip')
-            path = workspace.export(options).wait().download_as('workspace.zip')
+            path = workspace.export().wait().download_as('/home/workspace.zip')
+            path = workspace.export().wait().download_as('workspace.zip')
+
         """
         data = self._export_sal.export_download(self._download_uri)
         os.makedirs(os.path.dirname(path_to_download), exist_ok=True)
         with open(path_to_download, "wb") as f:
             f.write(data)
         return path_to_download
 
+    @classmethod
+    def from_operation(cls, operation: BaseOperation[Export], **kwargs: Any) -> Export:
+        assert isinstance(operation, WorkspaceExportOperation)
+        return cls(**kwargs, export_service=operation._sal.exports)
 
-class WorkspaceExportOperation(AsyncOperation):
-    """
-    An export operation class for the modelon.impact.client.entities.workspace.
-    Workspace class.
-    """
 
-    def __init__(self, location: str, service: Service):
-        super().__init__()
+class WorkspaceExportOperation(AsyncOperation[Entity]):
+    """An export operation class for the Workspace class."""
+
+    def __init__(
+        self, location: str, service: Service, create_entity: EntityFromOperation
+    ):
+        super().__init__(create_entity)
         self._location = location
         self._sal = service
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"Workspace export operations for id '{self.id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return (
             isinstance(obj, WorkspaceExportOperation)
             and obj._location == self._location
         )
 
     @property
-    def id(self):
-        """Workspace export id"""
+    def id(self) -> str:
+        """Workspace export id."""
         return self._location.split('/')[-1]
 
     @property
-    def name(self):
-        """Return the name of operation"""
+    def name(self) -> str:
+        """Return the name of operation."""
         return "Workspace export"
 
-    def cancel(self):
-        raise NotImplementedError('Cancel is not supported for this operation')
-
-    def _info(self):
-        return self._sal.workspace.get_workspace_export_status(self._location)["data"]
+    def _info(self) -> Dict[str, Any]:
+        return self._sal.exports.get_export_status(self._location)["data"]
 
-    def data(self):
-        """
-        Returns a Export class instance.
+    def data(self) -> Entity:
+        """Returns a Export class instance.
 
         Returns:
-
             An Export class instance.
+
         """
         info = self._info()
         if info['status'] == AsyncOperationStatus.ERROR.value:
             raise exceptions.IllegalWorkspaceExport(
                 f"Workspace export failed! Cause: {info['error'].get('message')}"
             )
-        return Export(self._sal.export, info["data"]["downloadUri"])
+        return self._create_entity(self, download_uri=info["data"]["downloadUri"])
 
-    def status(self):
-        """
-        Returns the upload status as an enumeration.
+    @property
+    def status(self) -> AsyncOperationStatus:
+        """Returns the upload status as an enumeration.
 
         Returns:
-
-            upload_status --
-                The AsyncOperationStatus enum. The status can have the enum values
-                AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
-                AsyncOperationStatus.ERROR
+            The AsyncOperationStatus enum. The status can have the enum values
+            AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
+            AsyncOperationStatus.ERROR
 
         Example::
 
-            workspace.download(definition, False).status()
+            workspace.download().status
+
         """
         return AsyncOperationStatus(self._info()["status"])
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/operations/workspace/imports.py` & `modelon_impact_client-3.0.1/modelon/impact/client/operations/content_import.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,79 @@
-from modelon.impact.client.entities.workspace import Workspace, WorkspaceDefinition
-from modelon.impact.client.sal.service import Service
-from modelon.impact.client.operations.base import AsyncOperation, AsyncOperationStatus
+from __future__ import annotations
+from typing import Dict, Any, TYPE_CHECKING
+
+from modelon.impact.client.operations.base import (
+    AsyncOperation,
+    AsyncOperationStatus,
+    Entity,
+)
 from modelon.impact.client import exceptions
 
+if TYPE_CHECKING:
+    from modelon.impact.client.sal.service import Service
+    from modelon.impact.client.operations.base import EntityFromOperation
+
 
-class WorkspaceImportOperation(AsyncOperation):
-    """
-    An import operation class for the modelon.impact.client.entities.workspace.
-    Workspace class.
-    """
+class ContentImportOperation(AsyncOperation[Entity]):
+    """An operation class for the ProjectContent class."""
 
     def __init__(
-        self,
-        location: str,
-        workspace_definition: WorkspaceDefinition,
-        service: Service,
+        self, location: str, service: Service, create_entity: EntityFromOperation
     ):
-        super().__init__()
+        super().__init__(create_entity)
         self._location = location
-        self._workspace_definition = workspace_definition
         self._sal = service
+        self._create_entity = create_entity
 
-    def __repr__(self):
-        return f"Workspace import operations for id '{self.id}'"
+    def __repr__(self) -> str:
+        return f"Content import operations for id '{self.id}'"
 
-    def __eq__(self, obj):
+    def __eq__(self, obj: object) -> bool:
         return (
-            isinstance(obj, WorkspaceImportOperation)
-            and obj._location == self._location
+            isinstance(obj, ContentImportOperation) and obj._location == self._location
         )
 
     @property
-    def id(self):
-        """Workspace import id"""
+    def id(self) -> str:
+        """Content import id."""
         return self._location.split('/')[-1]
 
     @property
-    def name(self):
-        """Return the name of operation"""
-        return "Workspace import"
+    def name(self) -> str:
+        """Return the name of operation."""
+        return "Project content import"
 
-    def cancel(self):
-        raise NotImplementedError('Cancel is not supported for this operation')
+    def _info(self) -> Dict[str, Any]:
+        return self._sal.imports.get_import_status(self._location)["data"]
 
-    def _info(self):
-        return self._sal.workspace.get_workspace_upload_status(self._location)["data"]
-
-    def data(self):
-        """
-        Returns a new Workspace class instance.
+    def data(self) -> Entity:
+        """Returns a new ProjectContent class instance.
 
         Returns:
+            A ProjectContent class instance.
 
-            workspace --
-                A Workspace class instance.
         """
         info = self._info()
         if info['status'] == AsyncOperationStatus.ERROR.value:
-            raise exceptions.IllegalWorkspaceImport(
-                f"Workspace import failed! Cause: {info['error'].get('message')}"
+            raise exceptions.IllegalContentImport(
+                f"Content import failed! Cause: {info['error'].get('message')}"
             )
-        workspace_id = info["data"]["workspaceId"]
-        return Workspace(workspace_id, self._workspace_definition, self._sal)
+        project_id = self._location.split('/')[-3]
+        content_id = info["data"]["contentId"]
+        resp = self._sal.project.project_content_get(project_id, content_id)
+        return self._create_entity(self, content=resp, project_id=project_id)
 
-    def status(self):
-        """
-        Returns the upload status as an enumeration.
+    @property
+    def status(self) -> AsyncOperationStatus:
+        """Returns the upload status as an enumeration.
 
         Returns:
-
-            upload_status --
-                The AsyncOperationStatus enum. The status can have the enum values
-                AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
-                AsyncOperationStatus.ERROR
+            The AsyncOperationStatus enum. The status can have the enum values
+            AsyncOperationStatus.READY, AsyncOperationStatus.RUNNING or
+            AsyncOperationStatus.ERROR
 
         Example::
 
-            client.import_from_shared_definition(definition, False).status()
+            project.import_content('path/to/model.mo').status
+
         """
         return AsyncOperationStatus(self._info()["status"])
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/options.py` & `modelon_impact_client-3.0.1/modelon/impact/client/options.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,57 +1,56 @@
+from __future__ import annotations
 from copy import deepcopy
 from collections.abc import Mapping
-from typing import Union, List, Dict, Any
+from typing import List, Dict, Any, Iterator
 from abc import ABC
 
 
-def _set_options(options, **modified):
+def _set_options(options: Dict[str, Any], **modified: Any) -> Dict[str, Any]:
     opts = deepcopy(options)
     for name, value in modified.items():
         opts[name] = value
     return opts
 
 
 class BaseExecutionOptions(Mapping, ABC):
-    """
-    Base class for the simulation, compiler, solver and runtime options settings.
-    """
+    """Base class for the simulation, compiler, solver and runtime options
+    settings."""
 
     def __init__(self, values: Dict[str, Any], custom_function_name: str):
         self._values = values
         self._custom_function_name = custom_function_name
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"{type(self).__name__} for '{self._custom_function_name}'"
 
-    def __getitem__(self, key):
+    def __getitem__(self, key: str) -> Any:
         return self._values[key]
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[Any]:
         return self._values.__iter__()
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self._values.__len__()
 
-    def with_values(self, **modified):
+    def with_values(self, **modified: Any) -> Any:
         """Sets/updates the options.
 
-        Parameters:
-
-            parameters --
-                A keyworded, variable-length argument list of options.
+        Args:
+            parameters: A keyworded, variable-length argument list of options.
 
         Example::
 
             cmp_opts = custom_function.get_compiler_options().with_values(
                 c_compiler='gcc')
             runtime_opts = custom_function.get_runtime_options().with_values(
                 cs_solver=0)
             sol_opts = custom_function.get_solver_options().with_values(rtol=1e-7)
             sim_opts = custom_function.get_simulation_options().with_values(ncp=500)
+
         """
         values = _set_options(self._values, **modified)
         return self.__class__(values, self._custom_function_name)
 
 
 class CompilerOptions(BaseExecutionOptions):
     pass
@@ -62,56 +61,60 @@
 
 
 class SolverOptions(BaseExecutionOptions):
     pass
 
 
 class SimulationOptions(BaseExecutionOptions):
-    def with_result_filter(self, pattern: Union[str, List[str]]):
+    def with_result_filter(self, filter: List[str]) -> SimulationOptions:
         """Sets the variable filter for results.
 
-        Parameters:
-
-            pattern --
-                A filter pattern for choosing which variables to actually store
-            result for. The syntax can be found in
-            http://en.wikipedia.org/wiki/Glob_%28programming%29 . An
-            example is filter = "*der" , stores all variables ending with
-            'der'. Can also be a list.
+        Args:
+            filter:
+                A list of filter patterns for choosing which variables to actually
+                store result for. The syntax can be found in
+                https://en.wikipedia.org/wiki/Glob_(programming).
+                An example for filter is `*der`, which would stores all
+                variables ending with `der`.
 
         Example::
 
             sim_opts = custom_function.get_simulation_options().with_result_filter(
-                pattern = ["*.phi"])
+                filter = ["*.phi"])
+
         """
-        if not isinstance(pattern, str):
-            pattern = str(pattern)
-        return self.with_values(filter=pattern)
+        if not isinstance(filter, list) or [
+            p for p in filter if not isinstance(p, str)
+        ]:
+            raise ValueError(
+                "The filter must be specified as a list of pattern strings!"
+            )
+        return self.with_values(filter=str(filter))
 
 
 class ProjectExecutionOptions:
     def __init__(self, data: Dict[str, Any], name: str):
         self._data = data
         self._name = name
 
     @property
-    def custom_function(self):
+    def custom_function(self) -> str:
         return self._name
 
     @property
-    def compiler_options(self):
+    def compiler_options(self) -> CompilerOptions:
         return CompilerOptions(self._data.get("compiler", {}), self.custom_function)
 
     @property
-    def runtime_options(self):
+    def runtime_options(self) -> RuntimeOptions:
         return RuntimeOptions(self._data.get("runtime", {}), self.custom_function)
 
     @property
-    def simulation_options(self):
+    def simulation_options(self) -> SimulationOptions:
         return SimulationOptions(self._data.get("simulation", {}), self.custom_function)
 
     @property
-    def solver_options(self):
+    def solver_options(self) -> SolverOptions:
         return SolverOptions(self._data.get("solver", {}), self.custom_function)
 
-    def to_dict(self):
+    def to_dict(self) -> Dict[str, Any]:
         return {"customFunction": self._name, **self._data}
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/custom_function.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/custom_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,45 @@
-"""Custom function service module"""
+"""Custom function service module."""
+from typing import Dict, Any
 from modelon.impact.client.sal.http import HTTPClient
 from modelon.impact.client.sal.uri import URI
 
 
 class CustomFunctionService:
     def __init__(self, uri: URI, http_client: HTTPClient):
         self._base_uri = uri
         self._http_client = http_client
 
-    def custom_function_get(self, workspace_id: str, custom_function: str):
+    def custom_function_get(
+        self, workspace_id: str, custom_function: str
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/custom-functions/{custom_function}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def custom_functions_get(self, workspace_id: str):
+    def custom_functions_get(self, workspace_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/custom-functions"
         ).resolve()
         return self._http_client.get_json(url)
 
     def custom_function_default_options_get(
         self, workspace_id: str, custom_function: str
-    ):
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/custom-functions/{custom_function}"
             "/default-options"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def custom_function_options_get(self, workspace_id: str, custom_function: str):
+    def custom_function_options_get(
+        self, workspace_id: str, custom_function: str
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/custom-functions/{custom_function}"
             "/options"
         ).resolve()
         return self._http_client.get_json(url)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/exceptions.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/exceptions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Service access layer exceptions"""
+"""Service access layer exceptions."""
 
 
 class ServiceAccessError(Exception):
     pass
 
 
 class CommunicationError(ServiceAccessError):
@@ -18,26 +18,22 @@
 
 
 class UnauthorizedError(ServiceAccessError):
     pass
 
 
 class HTTPError(ServiceAccessError):
-    def __init__(self, message, status_code):
+    def __init__(self, message: str, status_code: int):
         self.status_code = status_code
         super().__init__(message)
 
 
 class ErrorBodyIsNotJSONError(ServiceAccessError):
     pass
 
 
 class ErrorJSONInvalidFormatError(ServiceAccessError):
     pass
 
 
 class NoResponseFetchVersionError(ServiceAccessError):
     pass
-
-
-class AccessingJupyterHubError(ServiceAccessError):
-    pass
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/experiment.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/experiment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
-"""Experiment service module"""
+"""Experiment service module."""
+from __future__ import annotations
 import enum
-from typing import Any, Optional, List, Dict
+from typing import Any, Optional, List, Dict, Union, Text, Tuple
 from modelon.impact.client.sal.http import HTTPClient
 from modelon.impact.client.sal.uri import URI
 
 
 @enum.unique
 class ResultFormat(enum.Enum):
-    """
-    Class representing an enumeration for the possible
-    formats avaiable for downloading results.
-    """
+    """Class representing an enumeration for the possible formats available for
+    downloading results."""
 
     MAT = "mat"
     CSV = "csv"
 
     @classmethod
-    def _missing_(cls, value):
+    def _missing_(cls, value: Any) -> Any:
         if cls not in ['mat', 'csv']:
             raise ValueError(
                 "Invalid result format! Allowed formats are 'mat' and 'csv."
             )
         return cls(value)
 
 
@@ -36,128 +35,157 @@
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{exp_id}/execution"
         ).resolve()
         self._http_client.post_json_no_response_body(url, body=body)
         return exp_id
 
-    def experiment_delete(self, workspace_id: str, exp_id: str):
+    def experiment_delete(self, workspace_id: str, exp_id: str) -> None:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/experiments/{exp_id}"
         ).resolve()
         self._http_client.delete_json(url)
 
-    def experiment_set_label(self, workspace_id: str, exp_id: str, label: str):
+    def experiment_set_label(self, workspace_id: str, exp_id: str, label: str) -> None:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/experiments/{exp_id}"
         ).resolve()
         return self._http_client.put_json_no_response_body(url, body={"label": label})
 
-    def execute_status(self, workspace_id: str, experiment_id: str):
+    def execute_status(self, workspace_id: str, experiment_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/execution"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def execute_cancel(self, workspace_id: str, experiment_id: str):
+    def execute_cancel(self, workspace_id: str, experiment_id: str) -> None:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/execution"
         ).resolve()
         return self._http_client.delete_json(url)
 
-    def result_variables_get(self, workspace_id: str, experiment_id: str):
+    def result_variables_get(self, workspace_id: str, experiment_id: str) -> List[str]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/variables"
         ).resolve()
         return self._http_client.get_json(url)
 
     def trajectories_get(
-        self, workspace_id: str, experiment_id: str, variables: List[str]
-    ):
-        body = {"variable_names": variables}
+        self,
+        workspace_id: str,
+        experiment_id: str,
+        variables: List[str],
+        last_point_only: bool,
+        format: Optional[str] = None,
+    ) -> Any:
+        body = {
+            "variable_names": variables,
+            "filter": {"lastPointOnly": last_point_only},
+        }
+        headers = {"Accept": format or "application/vnd.impact.trajectories.v1+json"}
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/trajectories"
         ).resolve()
-        return self._http_client.post_json(url, body=body)
+        return self._http_client.post_json(url, body=body, headers=headers)
 
-    def cases_get(self, workspace_id: str, experiment_id: str):
+    def cases_get(self, workspace_id: str, experiment_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def case_get(self, workspace_id: str, experiment_id: str, case_id: str):
+    def case_get(
+        self, workspace_id: str, experiment_id: str, case_id: str
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}"
         ).resolve()
         return self._http_client.get_json(url)
 
     def case_put(
         self,
         workspace_id: str,
         experiment_id: str,
         case_id: str,
         case_data: Dict[str, Any],
-    ):
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}"
         ).resolve()
         return self._http_client.put_json(url, body=case_data)
 
-    def case_get_log(self, workspace_id: str, experiment_id: str, case_id: str):
+    def case_get_log(self, workspace_id: str, experiment_id: str, case_id: str) -> str:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}/log"
         ).resolve()
         return self._http_client.get_text(url)
 
     def case_result_get(
         self,
         workspace_id: str,
         experiment_id: str,
         case_id: str,
         result_format: ResultFormat = ResultFormat.MAT,
-    ):
+    ) -> Tuple[Union[Text, bytes], str]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}/result"
         ).resolve()
         if result_format == ResultFormat.CSV:
             headers = {'Accept': 'text/csv'}
             csv_resp = self._http_client.get_csv(url, headers=headers)
             return csv_resp.stream, csv_resp.file_name
         headers = {'Accept': 'application/vnd.impact.mat.v1+octet-stream'}
         mat_resp = self._http_client.get_mat(url, headers=headers)
         return mat_resp.stream, mat_resp.file_name
 
     def case_trajectories_get(
-        self, workspace_id: str, experiment_id: str, case_id: str, variables: List[str]
-    ):
-        body = {"variable_names": variables}
+        self,
+        workspace_id: str,
+        experiment_id: str,
+        case_id: str,
+        variables: List[str],
+        last_point_only: bool,
+    ) -> List[str]:
+        body = {
+            "variable_names": variables,
+            "filter": {"lastPointOnly": last_point_only},
+        }
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}/trajectories"
         ).resolve()
         return self._http_client.post_json(url, body=body)
 
     def case_artifact_get(
         self, workspace_id: str, experiment_id: str, case_id: str, artifact_id: str
-    ):
+    ) -> Tuple[bytes, str]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
             f"{case_id}/custom-artifacts/{artifact_id}"
         ).resolve()
         resp = self._http_client.get_octet_response(url)
         return resp.stream, resp.file_name
+
+    def case_artifacts_meta_get(
+        self, workspace_id: str, experiment_id: str, case_id: str
+    ) -> Dict[str, Any]:
+        url = (
+            self._base_uri
+            / f"api/workspaces/{workspace_id}/experiments/{experiment_id}/cases/"
+            f"{case_id}/custom-artifacts"
+        ).resolve()
+        return self._http_client.get_json(url)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/http.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/http.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-"""HTTP client class"""
-from typing import Optional, Dict, Any
+"""HTTP client class."""
+from typing import Optional, Dict, Any, Union
 from modelon.impact.client.sal.request import (
     RequestCSV,
     RequestJSON,
     RequestMatStream,
     RequestOctetStream,
     RequestText,
     RequestZip,
+    RequestXML,
 )
 from modelon.impact.client.sal.response import (
     JSONResponse,
     CSVResponse,
     MatStreamResponse,
     OctetStreamResponse,
 )
 from modelon.impact.client.sal.context import Context
+from modelon.impact.client.jupyterhub.sal import JupyterContext
 
 
 class HTTPClient:
-    def __init__(self, context: Optional[Context] = None):
+    def __init__(self, context: Optional[Union[Context, JupyterContext]] = None):
         self._context = context if context else Context()
 
-    def get_json(self, url: str, headers: Optional[Dict[str, Any]] = None):
+    def get_json(self, url: str, headers: Optional[Dict[str, Any]] = None) -> Any:
         return self.get_json_response(url, headers=headers).data
 
     def get_json_response(
         self, url: str, headers: Optional[Dict[str, Any]] = None
     ) -> JSONResponse:
         request = RequestJSON(self._context, "GET", url, headers=headers)
         return request.execute()
 
-    def get_text(self, url: str) -> Dict[str, Any]:
+    def get_text(self, url: str) -> str:
         request = RequestText(self._context, "GET", url)
         return request.execute().data
 
     def get_csv(
         self, url: str, headers: Optional[Dict[str, Any]] = None
     ) -> CSVResponse:
         request = RequestCSV(self._context, "GET", url, headers=headers)
         return request.execute()
 
+    def get_xml(self, url: str, headers: Optional[Dict[str, Any]] = None) -> str:
+        request = RequestXML(self._context, "GET", url, headers=headers)
+        return request.execute().data
+
     def get_mat(
         self, url: str, headers: Optional[Dict[str, Any]] = None
     ) -> MatStreamResponse:
         request = RequestMatStream(self._context, "GET", url, headers=headers)
         return request.execute()
 
     def get_octet_response(self, url: str) -> OctetStreamResponse:
@@ -51,30 +57,32 @@
         return request.execute()
 
     def get_zip(self, url: str) -> bytes:
         request = RequestZip(self._context, "GET", url)
         return request.execute().data
 
     def post_json(
-        self, url: str, body: Optional[Dict[str, Any]] = None, files=None
-    ) -> Dict[str, Any]:
-        request = RequestJSON(self._context, "POST", url, body, files)
+        self,
+        url: str,
+        body: Optional[Dict[str, Any]] = None,
+        files: Optional[Dict[str, Any]] = None,
+        headers: Optional[Dict[str, Any]] = None,
+    ) -> Any:
+        request = RequestJSON(self._context, "POST", url, body, files, headers=headers)
         return request.execute().data
 
     def post_json_no_response_body(
         self, url: str, body: Optional[Dict[str, Any]] = None
-    ):
+    ) -> None:
         RequestJSON(self._context, "POST", url, body).execute()
 
-    def delete_json(self, url: str, body: Optional[Dict[str, Any]] = None):
+    def delete_json(self, url: str, body: Optional[Dict[str, Any]] = None) -> None:
         RequestJSON(self._context, "DELETE", url, body).execute()
 
     def put_json_no_response_body(
         self, url: str, body: Optional[Dict[str, Any]] = None
-    ):
+    ) -> None:
         RequestJSON(self._context, "PUT", url, body).execute()
 
-    def put_json(
-        self, url: str, body: Optional[Dict[str, Any]] = None
-    ) -> Dict[str, Any]:
+    def put_json(self, url: str, body: Optional[Dict[str, Any]] = None) -> Any:
         request = RequestJSON(self._context, "PUT", url, body)
         return request.execute().data
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/model_executable.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/model_executable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-"""Model executable service module"""
-from typing import Any, Dict, Tuple
+"""Model executable service module."""
+from typing import Any, Dict, Tuple, List
 from modelon.impact.client.sal.http import HTTPClient
 from modelon.impact.client.sal.uri import URI
 
 
 class ModelExecutableService:
     def __init__(self, uri: URI, http_client: HTTPClient):
         self._base_uri = uri
@@ -15,59 +15,67 @@
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/model-executables"
             f"?getCached={'true' if get_cached else 'false'}"
         ).resolve()
         resp = self._http_client.post_json(url, body=options)
         return resp["id"], resp["parameters"]
 
-    def compile_model(self, workspace_id, fmu_id: str) -> str:
+    def compile_model(self, workspace_id: str, fmu_id: str) -> str:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/compilation"
         ).resolve()
         self._http_client.post_json_no_response_body(url)
         return fmu_id
 
-    def compile_log(self, workspace_id: str, fmu_id: str):
+    def compile_log(self, workspace_id: str, fmu_id: str) -> str:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/compilation/"
             "log"
         ).resolve()
         return self._http_client.get_text(url)
 
-    def fmu_delete(self, workspace_id: str, fmu_id: str):
+    def model_description_get(self, workspace_id: str, fmu_id: str) -> str:
+        url = (
+            self._base_uri
+            / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/"
+            "model-description"
+        ).resolve()
+        return self._http_client.get_xml(url)
+
+    def fmu_delete(self, workspace_id: str, fmu_id: str) -> None:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}"
         ).resolve()
         self._http_client.delete_json(url)
 
-    def compile_status(self, workspace_id: str, fmu_id: str):
+    def compile_status(self, workspace_id: str, fmu_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/compilation"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def compile_cancel(self, workspace_id: str, fmu_id: str):
+    def compile_cancel(self, workspace_id: str, fmu_id: str) -> None:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/compilation"
         ).resolve()
         return self._http_client.delete_json(url)
 
-    def settable_parameters_get(self, workspace_id: str, fmu_id: str):
+    def settable_parameters_get(self, workspace_id: str, fmu_id: str) -> List[str]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/"
             "settable-parameters"
         ).resolve()
         return self._http_client.get_json(url)
 
     def ss_fmu_metadata_get(
         self, workspace_id: str, fmu_id: str, parameter_state: Dict[str, Any]
-    ):
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}"
             "/steady-state-metadata"
         ).resolve()
         return self._http_client.post_json(url, body=parameter_state)
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/project.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/project.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,96 +1,105 @@
-"""Project service module"""
+"""Project service module."""
+from __future__ import annotations
 import json
-from typing import Dict, Any, Optional, Union, List
+from typing import Dict, Any, Optional, Union, List, TYPE_CHECKING
 from modelon.impact.client.sal.http import HTTPClient
 from modelon.impact.client.sal.uri import URI
 
+if TYPE_CHECKING:
+    from modelon.impact.client.entities.project import ProjectType
+
 
 class ProjectService:
     def __init__(self, uri: URI, http_client: HTTPClient):
         self._base_uri = uri
         self._http_client = http_client
 
-    def projects_get(self, vcs_info: bool):
-        url = (self._base_uri / f"api/projects?vcsInfo={vcs_info}").resolve()
+    def projects_get(
+        self, vcs_info: bool, project_type: Optional[ProjectType] = None
+    ) -> Dict[str, Any]:
+        prj_type = '&type=' + str(project_type) if project_type else ""
+        url = (self._base_uri / f"api/projects?vcsInfo={vcs_info}{prj_type}").resolve()
         return self._http_client.get_json(url)
 
-    def project_get(self, project_id: str, vcs_info: bool):
+    def project_get(
+        self, project_id: str, vcs_info: bool, size_info: bool
+    ) -> Dict[str, Any]:
         url = (
-            self._base_uri / f"api/projects/{project_id}?vcsInfo={vcs_info}"
+            self._base_uri
+            / f"api/projects/{project_id}?vcsInfo={vcs_info}&sizeInfo={size_info}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def project_delete(self, project_id: str):
+    def project_delete(self, project_id: str) -> None:
         url = (self._base_uri / f"api/projects/{project_id}").resolve()
         self._http_client.delete_json(url)
 
-    def project_put(self, project_id: str, project_data: Dict[str, Any]):
+    def project_put(self, project_id: str, project_data: Dict[str, Any]) -> None:
         url = (self._base_uri / f"api/projects/{project_id}").resolve()
         self._http_client.put_json(url, body=project_data)
 
-    def project_options_get(self, project_id: str, custom_function: str):
+    def project_options_get(
+        self, project_id: str, workspace_id: str, custom_function: str
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
-            / f"api/projects/{project_id}/custom-functions/{custom_function}/options"
+            / f"api/workspaces/{workspace_id}/projects/{project_id}/custom-functions/"
+            f"{custom_function}/options"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def project_default_options_get(self, project_id: str, custom_function: str):
+    def project_default_options_get(
+        self, workspace_id: str, custom_function: str
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
-            / f"api/projects/{project_id}/custom-functions/{custom_function}/"
-            "default-options"
+            / f"api/workspaces/{workspace_id}/custom-functions/{custom_function}"
+            "/default-options"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def project_content_delete(self, project_id: str, content_id: str):
+    def project_content_delete(self, project_id: str, content_id: str) -> None:
         url = (
             self._base_uri / f"api/projects/{project_id}/content/{content_id}"
         ).resolve()
         self._http_client.delete_json(url)
 
     def project_content_upload(
         self, path_to_result: str, project_id: str, content_type: str
-    ):
+    ) -> Dict[str, Any]:
         url = (self._base_uri / f"/api/projects/{project_id}/content-imports").resolve()
         with open(path_to_result, "rb") as f:
             multipart_form_data = {
                 'file': f,
                 'options': json.dumps({'contentType': content_type}),
             }
             return self._http_client.post_json(url, files=multipart_form_data)
 
-    def project_content_upload_status(self, location: str):
-        url = (self._base_uri / location).resolve()
-        return self._http_client.get_json(url)
-
-    def project_content_get(self, project_id: str, content_id: str):
+    def project_content_get(self, project_id: str, content_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri / f"/api/projects/{project_id}/content/{content_id}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def fmu_upload(
+    def fmu_import(
         self,
-        workspace_id: str,
         project_id: str,
         content_id: str,
         fmu_path: str,
         class_name: str,
         overwrite: bool = False,
         include_patterns: Optional[Union[str, List[str]]] = None,
         exclude_patterns: Optional[Union[str, List[str]]] = None,
         top_level_inputs: Optional[Union[str, List[str]]] = None,
         step_size: float = 0.0,
-    ):
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
-            / f"api/workspaces/{workspace_id}/projects/{project_id}/content/"
-            f"{content_id}/models"
+            / f"api/projects/{project_id}/content/{content_id}/fmu-imports"
         ).resolve()
         options = {
             "className": class_name,
             "overwrite": overwrite,
             "stepSize": step_size,
         }
 
@@ -103,7 +112,12 @@
 
         with open(fmu_path, "rb") as f:
             multipart_form_data = {
                 'file': f,
                 'options': json.dumps(options),
             }
             return self._http_client.post_json(url, files=multipart_form_data)
+
+    def import_from_zip(self, path_to_project: str) -> Dict[str, Any]:
+        url = (self._base_uri / "api/project-imports").resolve()
+        with open(path_to_project, "rb") as f:
+            return self._http_client.post_json(url, files={"file": f})
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/response.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Response class"""
+"""Response class."""
 import re
-from typing import Text, Union, Dict, Any
+from typing import Text, Dict, Any
 from modelon.impact.client.sal import exceptions
 
 
 class ResponseError:
     def __init__(self, message: str, code: int):
         self.message = message
         self.code = code
 
 
 class Response:
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         self._resp_obj = resp_obj
 
     def _is_json(self) -> bool:
         return "application/json" in self._resp_obj.headers.get("content-type")
 
     @property
     def status_code(self) -> int:
@@ -42,15 +42,15 @@
             )
 
         error = json["error"]
         return ResponseError(error["message"], error["code"])
 
 
 class JSONResponse(Response):
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         super().__init__(resp_obj)
 
     @property
     def data(self) -> Dict[str, Any]:
         if not self._resp_obj.ok:
             raise exceptions.HTTPError(self.error.message, self._resp_obj.status_code)
 
@@ -63,15 +63,15 @@
 
     @property
     def headers(self) -> Dict[str, Any]:
         return self._resp_obj.headers
 
 
 class TextResponse(Response):
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         super().__init__(resp_obj)
 
     def _is_txt(self) -> bool:
         return "text/plain" in self._resp_obj.headers.get("content-type")
 
     @property
     def data(self) -> Text:
@@ -82,16 +82,36 @@
             raise exceptions.InvalidContentTypeError(
                 "Incorrect content type on response, expected text"
             )
 
         return self._resp_obj.text
 
 
+class XMLResponse(Response):
+    def __init__(self, resp_obj: Any):
+        super().__init__(resp_obj)
+
+    def _is_xml(self) -> bool:
+        return "application/xml" in self._resp_obj.headers.get("content-type")
+
+    @property
+    def data(self) -> Text:
+        if not self._resp_obj.ok:
+            raise exceptions.HTTPError(self.error.message, self._resp_obj.status_code)
+
+        if not self._is_xml():
+            raise exceptions.InvalidContentTypeError(
+                "Incorrect content type on response, expected XML"
+            )
+
+        return self._resp_obj.text
+
+
 class ZIPResponse(Response):
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         super().__init__(resp_obj)
 
     def _is_zip(self) -> bool:
         return "application/zip" in self._resp_obj.headers.get("content-type")
 
     @property
     def data(self) -> bytes:
@@ -104,23 +124,23 @@
                 "compressed archive"
             )
 
         return self._resp_obj.content
 
 
 class FileResponse(Response):
-    def __init__(self, resp_obj, content_type: str):
+    def __init__(self, resp_obj: Any, content_type: str):
         super().__init__(resp_obj)
         self.content_type = content_type
 
     def _is_expected_content_type(self) -> bool:
         return self.content_type in self._resp_obj.headers.get("content-type")
 
     @property
-    def stream(self) -> Union[Text, bytes]:
+    def stream(self) -> bytes:
         if not self._resp_obj.ok:
             raise exceptions.HTTPError(self.error.message, self._resp_obj.status_code)
 
         if not self._is_expected_content_type():
             raise exceptions.InvalidContentTypeError(
                 f"Incorrect content type on response, expected {self.content_type}"
             )
@@ -138,19 +158,19 @@
     @property
     def file_name(self) -> str:
         d = self.headers["content-disposition"]
         return re.findall("filename=(.+)", d)[0].strip('"')
 
 
 class CSVResponse(FileResponse):
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         super().__init__(resp_obj, "text/csv")
 
 
 class OctetStreamResponse(FileResponse):
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         super().__init__(resp_obj, "application/octet-stream")
 
 
 class MatStreamResponse(FileResponse):
-    def __init__(self, resp_obj):
+    def __init__(self, resp_obj: Any):
         super().__init__(resp_obj, "application/vnd.impact.mat.v1+octet-stream")
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/uri.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/uri.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-"""URI class"""
+"""URI class."""
+from __future__ import annotations
+from typing import Any
 import sys
 import urllib.parse
 
 
 class URI:
     def __init__(self, content: str):
         # If running on Windows you can get a lot of overhead using 'localhost'
         if sys.platform.startswith("win32") and content.startswith("http://localhost:"):
             content = content.replace("http://localhost:", "http://127.0.0.1:")
 
         self.content = content
 
-    def resolve(self, **kwargs):
+    def resolve(self, **kwargs: Any) -> str:
         return self.content.format(**kwargs)
 
-    def _with_path(self, path):
+    def _with_path(self, path: str) -> URI:
         return URI(urllib.parse.urljoin(self.content + "/", path.lstrip('/')))
 
-    def __floordiv__(self, other):
+    def __floordiv__(self, other: str) -> URI:
         return self._with_path(other)
 
-    def __truediv__(self, other):
+    def __truediv__(self, other: str) -> URI:
         return self._with_path(other)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return self.content
```

### Comparing `modelon_impact_client-3.0.0.dev9/modelon/impact/client/sal/workspace.py` & `modelon_impact_client-3.0.1/modelon/impact/client/sal/workspace.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,186 +1,173 @@
-"""Workspace service module"""
-import json
+"""Workspace service module."""
 from typing import Optional, Dict, Any, List
 from modelon.impact.client.sal.http import HTTPClient
 from modelon.impact.client.sal.uri import URI
 
 
 class WorkspaceService:
     def __init__(self, uri: URI, http_client: HTTPClient):
         self._base_uri = uri
         self._http_client = http_client
 
-    def workspace_create(self, name: str):
+    def workspace_create(self, name: str) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspaces").resolve()
         return self._http_client.post_json(url, body={"new": {"name": name}})
 
-    def workspace_delete(self, workspace_id: str):
+    def workspace_delete(self, workspace_id: str) -> None:
         url = (self._base_uri / f"api/workspaces/{workspace_id}").resolve()
         self._http_client.delete_json(url)
 
-    def workspaces_get(self):
+    def workspace_get(self, workspace_id: str, size_info: bool) -> Dict[str, Any]:
+        url = (
+            self._base_uri / f"api/workspaces/{workspace_id}?sizeInfo={size_info}"
+        ).resolve()
+        return self._http_client.get_json(url)
+
+    def workspaces_get(self) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspaces").resolve()
         return self._http_client.get_json(url)
 
-    def projects_get(self, workspace_id: str, vcs_info: bool, include_disabled: bool):
+    def projects_get(
+        self, workspace_id: str, vcs_info: bool, include_disabled: bool
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/projects?vcsInfo={vcs_info}"
             f"&includeDisabled={include_disabled}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def project_create(self, workspace_id: str, name: str):
+    def project_create(self, workspace_id: str, name: str) -> Dict[str, Any]:
         url = (self._base_uri / f"api/workspaces/{workspace_id}/projects").resolve()
         return self._http_client.post_json(url, body={"new": {"name": name}})
 
     def dependencies_get(
         self, workspace_id: str, vcs_info: bool, include_disabled: bool
-    ):
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/dependencies?vcsInfo={vcs_info}"
             f"&includeDisabled={include_disabled}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def workspace_get(self, workspace_id: str):
-        url = (self._base_uri / f"api/workspaces/{workspace_id}").resolve()
-        return self._http_client.get_json(url)
-
-    def workspace_upload(self, path_to_workspace: str):
-        url = (self._base_uri / "api/workspaces").resolve()
-        with open(path_to_workspace, "rb") as f:
-            return self._http_client.post_json(url, files={"file": f})
-
-    def result_upload(
-        self,
-        workspace_id: str,
-        path_to_result: str,
-        label: Optional[str] = None,
-        description: Optional[str] = None,
-    ):
-        url = (self._base_uri / "api/uploads/results").resolve()
-        options: Dict[str, Any] = {
-            "context": {"workspaceId": workspace_id},
-        }
-        if label:
-            options["name"] = label
-        if description:
-            options["description"] = description
-        with open(path_to_result, "rb") as f:
-            multipart_form_data = {
-                'file': f,
-                'options': json.dumps(options),
-            }
-            return self._http_client.post_json(url, files=multipart_form_data)
-
-    def get_result_upload_status(self, upload_id: str):
-        url = (self._base_uri / f"api/uploads/results/{upload_id}").resolve()
-        return self._http_client.get_json(url)
-
-    def get_uploaded_result_meta(self, upload_id: str):
-        url = (self._base_uri / f"api/external-result/{upload_id}").resolve()
-        return self._http_client.get_json(url)
-
-    def delete_uploaded_result(self, upload_id: str):
-        url = (self._base_uri / f"api/external-result/{upload_id}").resolve()
-        return self._http_client.delete_json(url)
-
-    def workspace_export_setup(self, workspace_id: str, options: Dict[str, Any]):
+    def workspace_export_setup(self, workspace_id: str) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-exports").resolve()
-        options["workspaceId"] = workspace_id
-        return self._http_client.post_json(url, body=options)
-
-    def get_workspace_export_status(self, location: str):
-        url = (self._base_uri / location).resolve()
-        return self._http_client.get_json(url)
+        body = {"workspaceId": workspace_id}
+        return self._http_client.post_json(url, body=body)
 
-    def workspace_conversion_setup(self, workspace_id: str, backup_name: Optional[str]):
+    def workspace_conversion_setup(
+        self, workspace_id: str, backup_name: Optional[str]
+    ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-conversions").resolve()
         backup_data = {'backup': {'name': backup_name}} if backup_name else {}
         body: Dict[str, Any] = {'data': {'workspaceId': workspace_id, **backup_data}}
         return self._http_client.post_json(url, body=body)
 
-    def get_workspace_conversion_status(self, location: str):
+    def get_workspace_conversion_status(self, location: str) -> Dict[str, Any]:
         url = (self._base_uri / location).resolve()
         return self._http_client.get_json(url)
 
-    def workspace_clone(self, workspace_id: str):
-        url = (self._base_uri / f"api/workspaces/{workspace_id}/clone").resolve()
-        return self._http_client.post_json(url)
-
-    def fmus_get(self, workspace_id: str):
+    def fmus_get(self, workspace_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/model-executables"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def fmu_get(self, workspace_id: str, fmu_id: str):
+    def fmu_get(self, workspace_id: str, fmu_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}"
         ).resolve()
         return self._http_client.get_json(url)
 
-    def fmu_download(self, workspace_id: str, fmu_id: str):
+    def fmu_download(self, workspace_id: str, fmu_id: str) -> bytes:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/model-executables/{fmu_id}/binary"
         ).resolve()
         return self._http_client.get_zip(url)
 
-    def experiments_get(self, workspace_id: str):
-        url = (self._base_uri / f"api/workspaces/{workspace_id}/experiments").resolve()
+    def experiments_get(
+        self, workspace_id: str, class_path: Optional[str] = None
+    ) -> Dict[str, Any]:
+        class_path_query = f"?classPath={class_path}" if class_path else ""
+        url = (
+            self._base_uri
+            / f"api/workspaces/{workspace_id}/experiments{class_path_query}"
+        ).resolve()
         return self._http_client.get_json(
             url, headers={"Accept": "application/vnd.impact.experiment.v2+json"}
         )
 
-    def experiment_get(self, workspace_id: str, experiment_id: str):
+    def experiment_get(self, workspace_id: str, experiment_id: str) -> Dict[str, Any]:
         url = (
             self._base_uri
             / f"api/workspaces/{workspace_id}/experiments/{experiment_id}"
         ).resolve()
         return self._http_client.get_json(
             url, headers={"Accept": "application/vnd.impact.experiment.v2+json"}
         )
 
     def experiment_create(
         self,
         workspace_id: str,
         definition: Dict[str, Any],
         user_data: Optional[Dict[str, Any]] = None,
-    ):
+    ) -> Dict[str, Any]:
         url = (self._base_uri / f"api/workspaces/{workspace_id}/experiments").resolve()
         body = {
             **definition,
             **({"userData": user_data} if user_data is not None else {}),
         }
         return self._http_client.post_json(url, body=body)
 
-    def shared_definition_get(self, workspace_id: str, strict: bool = False):
+    def shared_definition_get(
+        self, workspace_id: str, strict: bool = False
+    ) -> Dict[str, Any]:
         url = (
             self._base_uri / f"api/workspaces/{workspace_id}/"
             f"sharing-definition?strict={'true' if strict else 'false'}"
         ).resolve()
         return self._http_client.get_json(url)
 
+    def import_from_zip(self, path_to_workspace: str) -> Dict[str, Any]:
+        url = (self._base_uri / "api/workspace-imports").resolve()
+        with open(path_to_workspace, "rb") as f:
+            return self._http_client.post_json(url, files={"file": f})
+
     def import_from_shared_definition(
         self,
         shared_definition: Dict[str, Any],
         selected_matchings: Optional[List[Dict[str, Any]]] = None,
-    ):
+    ) -> Dict[str, Any]:
         if selected_matchings:
             shared_definition = {
                 **shared_definition,
                 **{"selectedMatchings": {"entries": selected_matchings}},
             }
         url = (self._base_uri / "api/workspace-imports").resolve()
         return self._http_client.post_json(url, body=shared_definition)
 
-    def get_workspace_upload_status(self, location: str):
-        url = (self._base_uri / location).resolve()
-        return self._http_client.get_json(url)
-
-    def get_project_matchings(self, shared_definition: Dict[str, Any]):
+    def get_project_matchings(
+        self, shared_definition: Dict[str, Any]
+    ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-imports-matchings").resolve()
         return self._http_client.post_json(url, body=shared_definition)
+
+    def import_project_from_zip(
+        self, workspace_id: str, path_to_project: str
+    ) -> Dict[str, Any]:
+        url = (
+            self._base_uri / f"api/workspaces/{workspace_id}/project-imports"
+        ).resolve()
+        with open(path_to_project, "rb") as f:
+            return self._http_client.post_json(url, files={"file": f})
+
+    def import_dependency_from_zip(
+        self, workspace_id: str, path_to_project: str
+    ) -> Dict[str, Any]:
+        url = (
+            self._base_uri / f"api/workspaces/{workspace_id}/dependency-imports"
+        ).resolve()
+        with open(path_to_project, "rb") as f:
+            return self._http_client.post_json(url, files={"file": f})
```

### Comparing `modelon_impact_client-3.0.0.dev9/pyproject.toml` & `modelon_impact_client-3.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modelon-impact-client"
 packages = [
     { include = "modelon" },
 ]
-version = "3.0.0-dev.9"
+version = "3.0.1"
 description = "Client library for easy scripting against Modelon Impact"
 readme = "README.md"
 homepage = "https://www.modelon.com/modelon-impact"
 repository = "https://github.com/modelon-community/impact-client-python"
 documentation = "https://modelon-impact-client.readthedocs.io"
 license = "BSD"
 authors = [
@@ -17,25 +17,38 @@
     "Programming Language :: Python :: 3.7"
 ]
 include = [
 ]
 keywords = ["impact", "client", "API"]
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.9.0"
 requests = "^2.23"
 semantic_version = "^2.8.5"
 types-requests = "^2.27.30"
+# Do not use urllib3 2.0, it only supports OpenSSL 1.1.1+, CentOS 7 have 1.0.2k-fips
+urllib3 = "^1.26.15"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 flake8 = "4.0.1"
 mypy = "*"
 pytest-watch = "^4.2.0"
 black = "^22.10.0"
 click = "^8.1.3"
 requests_mock = "^1.10"
-sphinx = "^4.0.0"
-sphinx-rtd-theme = "^1.1.1"
-sphinx-copybutton = "^0.5.1"
 pytest-cov = "^4.0.0"
 pylint = "^2.13.4"
+docformatter = {extras = ["tomli"], version = "^1.5.1"}
+
+[tool.poetry.group.docs.dependencies]
+sphinx = "^6.0.0"
+sphinx-rtd-theme = "^1.1.1"
+sphinx-copybutton = "^0.5.1"
+sphinxcontrib-napoleon = "^0.7"
+sphinxcontrib-spelling = "^7.7.0"
+readthedocs-sphinx-search = "^0.3.1"
+sphinx-autodoc-typehints = "^1.22"
+
+[tool.docformatter]
+recursive = true
+blank = true
```

### Comparing `modelon_impact_client-3.0.0.dev9/setup.py` & `modelon_impact_client-3.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,105 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['modelon',
- 'modelon.impact',
- 'modelon.impact.client',
- 'modelon.impact.client.entities',
- 'modelon.impact.client.experiment_definition',
- 'modelon.impact.client.jupyterhub',
- 'modelon.impact.client.operations',
- 'modelon.impact.client.operations.workspace',
- 'modelon.impact.client.sal']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['requests>=2.23,<3.0',
- 'semantic_version>=2.8.5,<3.0.0',
- 'types-requests>=2.27.30,<3.0.0']
-
-setup_kwargs = {
-    'name': 'modelon-impact-client',
-    'version': '3.0.0.dev9',
-    'description': 'Client library for easy scripting against Modelon Impact',
-    'long_description': '# Modelon-impact-client\nClient library for easy scripting against Modelon Impact\n\n## Installation\n\nFor installation instructions and requirements, please refer to the [documentation](https://modelon-impact-client.readthedocs.io).\n\n## Develop\n\n### Devcontainer\nIf you are developing with VS Code you can use the devcontainer which gives gives you a ready to use environment for development. Just click the "Reopen in Container" button after opening the project in VS Code.\n\n#### Tips and tricks\nIt is possible to run the \'make\' commands listed bellow using the devcontainer. It will detect being in a container and bypass Docker parts of the commands.\n\nYou can open a project with the dev-container directly without having to open and then re-load. Standing in the project directory you can run:\n```\ndevcontainer open .\n```\nNote that this requires the [devcontainer-cli](https://code.visualstudio.com/docs/remote/devcontainer-cli).\n\nYou can add your own extensions to devcontainers. These extensions will be added for all devcontainers. First open your \'settings\' as JSON. Then, to add for example the "GitLens" extension, put the following at the bottom of the settings:\n```\n    ...\n    "remote.containers.defaultExtensions": ["eamodio.gitlens"]\n}\n```\nVS Code also have a `\'Install Local Extensions in \'Remote\'` command, but it must be repeated for each devcontainer and everytime a devcontainer is re-built.\n\n### Creating a shell\nModelon-impact-client is developed using a Docker container for all build tools.\nYou can get a shell into said container by running:\n\n```\nmake shell\n```\n\n### Manage dependencies\nDependencies are managed by poetry. Add dependencies by running \n`poetry add <package>`  or `poetry add <package> --dev` inside the shell\n\n### Running tests\n\nTests are executed by running `make test`. You can also run `make test-watch` to get a watcher\nthat continuously re-runs the tests.\n\n### Running lint\n```\nmake lint\n```\n\n## Build\n\nBuilding modelon-impact-client is done by running\n\n```\nmake wheel\n```\n\n## Release\n\nThe modelon-impact-client build process is a fully automated using `Semantic-release`.\n\nAutomation is enabled for:\n- Bumping version\n- Generate changelog\n\nThis is done based on git commit semantics as described here: https://semantic-release.gitbook.io/semantic-release/\n\nTo make a new release simply run:\n```\nmake publish\n```\n\nThis command will detect what branch you are on and your git history and make a appropriate release.\n\nCurrent configuration can be found in `.releaserc` and specifies that commits to branch `master` should be released and\ncommits to branch `beta` should be released as a `pre-release`.\n\nThis workflow make sure that no administrative time needs to be put into managing the release workflow.\n',
-    'author': 'WEP',
-    'author_email': 'impact@modelon.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://www.modelon.com/modelon-impact',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.0,<4.0.0',
+Metadata-Version: 2.1
+Name: modelon-impact-client
+Version: 3.0.1
+Summary: Client library for easy scripting against Modelon Impact
+Home-page: https://www.modelon.com/modelon-impact
+License: BSD
+Keywords: impact,client,API
+Author: WEP
+Author-email: impact@modelon.com
+Requires-Python: >=3.9.0,<4.0.0
+Classifier: License :: Other/Proprietary License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Requires-Dist: requests (>=2.23,<3.0)
+Requires-Dist: semantic_version (>=2.8.5,<3.0.0)
+Requires-Dist: types-requests (>=2.27.30,<3.0.0)
+Requires-Dist: urllib3 (>=1.26.15,<2.0.0)
+Project-URL: Documentation, https://modelon-impact-client.readthedocs.io
+Project-URL: Repository, https://github.com/modelon-community/impact-client-python
+Description-Content-Type: text/markdown
+
+# Modelon-impact-client
+Client library for easy scripting against Modelon Impact
+
+## Installation
+
+For installation instructions and requirements, please refer to the [documentation](https://modelon-impact-client.readthedocs.io).
+
+## Develop
+
+### Devcontainer
+If you are developing with VS Code you can use the devcontainer which gives gives you a ready to use environment for development. Just click the "Reopen in Container" button after opening the project in VS Code.
+
+#### Tips and tricks
+It is possible to run the 'make' commands listed bellow using the devcontainer. It will detect being in a container and bypass Docker parts of the commands.
+
+You can open a project with the dev-container directly without having to open and then re-load. Standing in the project directory you can run:
+```
+devcontainer open .
+```
+Note that this requires the [devcontainer-cli](https://code.visualstudio.com/docs/remote/devcontainer-cli).
+
+You can add your own extensions to devcontainers. These extensions will be added for all devcontainers. First open your 'settings' as JSON. Then, to add for example the "GitLens" extension, put the following at the bottom of the settings:
+```
+    ...
+    "remote.containers.defaultExtensions": ["eamodio.gitlens"]
 }
+```
+VS Code also have a `'Install Local Extensions in 'Remote'` command, but it must be repeated for each devcontainer and everytime a devcontainer is re-built.
+
+### Creating a shell
+Modelon-impact-client is developed using a Docker container for all build tools.
+You can get a shell into said container by running:
+
+```
+make shell
+```
+
+### Manage dependencies
+Dependencies are managed by poetry. Add dependencies by running 
+`poetry add <package>`  or `poetry add <package> --dev` inside the shell
+
+### Running tests
+
+Tests are executed by running `make test`. You can also run `make test-watch` to get a watcher
+that continuously re-runs the tests.
+
+### Running lint
+```
+make lint
+```
+
+## Build
+
+Building modelon-impact-client is done by running
+
+```
+make wheel
+```
+
+## Release
+
+The modelon-impact-client build process is a fully automated using `Semantic-release`.
+
+Automation is enabled for:
+- Bumping version
+- Generate changelog
+
+This is done based on git commit semantics as described here: https://semantic-release.gitbook.io/semantic-release/
+
+To make a new release simply run:
+```
+make publish
+```
+
+This command will detect what branch you are on and your git history and make a appropriate release.
+
+Current configuration can be found in `.releaserc` and specifies that commits to branch `master` should be released and
+commits to branch `beta` should be released as a `pre-release`.
 
+This workflow make sure that no administrative time needs to be put into managing the release workflow.
 
-setup(**setup_kwargs)
```

