# Comparing `tmp/modelon_impact_client-3.0.1.tar.gz` & `tmp/modelon_impact_client-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelon_impact_client-3.0.1.tar", max compression
+gzip compressed data, was "modelon_impact_client-3.0.2.tar", max compression
```

## Comparing `modelon_impact_client-3.0.1.tar` & `modelon_impact_client-3.0.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1479 2023-06-09 06:58:12.992848 modelon_impact_client-3.0.1/LICENSE.md
--rw-r--r--   0        0        0     2748 2023-06-09 06:58:12.999848 modelon_impact_client-3.0.1/README.md
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.954847 modelon_impact_client-3.0.1/modelon/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.988847 modelon_impact_client-3.0.1/modelon/impact/__init__.py
--rw-r--r--   0        0        0      830 2023-06-09 06:58:12.981847 modelon_impact_client-3.0.1/modelon/impact/client/__init__.py
--rw-r--r--   0        0        0    24886 2023-06-09 06:58:12.957847 modelon_impact_client-3.0.1/modelon/impact/client/client.py
--rw-r--r--   0        0        0      835 2023-06-09 06:58:13.000847 modelon_impact_client-3.0.1/modelon/impact/client/configuration.py
--rw-r--r--   0        0        0     1938 2023-06-09 06:58:12.958847 modelon_impact_client-3.0.1/modelon/impact/client/credential_manager.py
--rw-r--r--   0        0        0      119 2023-06-09 06:58:12.969847 modelon_impact_client-3.0.1/modelon/impact/client/entities/__init__.py
--rw-r--r--   0        0        0      639 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/entities/asserts.py
--rw-r--r--   0        0        0    24767 2023-06-09 06:58:12.999848 modelon_impact_client-3.0.1/modelon/impact/client/entities/case.py
--rw-r--r--   0        0        0     2259 2023-06-09 06:58:13.010848 modelon_impact_client-3.0.1/modelon/impact/client/entities/content.py
--rw-r--r--   0        0        0     6620 2023-06-09 06:58:12.959847 modelon_impact_client-3.0.1/modelon/impact/client/entities/custom_function.py
--rw-r--r--   0        0        0    18419 2023-06-09 06:58:12.961847 modelon_impact_client-3.0.1/modelon/impact/client/entities/experiment.py
--rw-r--r--   0        0        0     2511 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/entities/external_result.py
--rw-r--r--   0        0        0        0 2023-06-09 06:58:13.009848 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/__init__.py
--rw-r--r--   0        0        0      180 2023-06-09 06:58:12.948847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/case.py
--rw-r--r--   0        0        0      200 2023-06-09 06:58:12.987847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/custom_function.py
--rw-r--r--   0        0        0      366 2023-06-09 06:58:12.976847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/experiment.py
--rw-r--r--   0        0        0      192 2023-06-09 06:58:12.982847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/external_result.py
--rw-r--r--   0        0        0      186 2023-06-09 06:58:12.978847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/model.py
--rw-r--r--   0        0        0      190 2023-06-09 06:58:12.969847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/model_executable.py
--rw-r--r--   0        0        0      190 2023-06-09 06:58:12.953847 modelon_impact_client-3.0.1/modelon/impact/client/entities/interfaces/workspace.py
--rw-r--r--   0        0        0      156 2023-06-09 06:58:12.972847 modelon_impact_client-3.0.1/modelon/impact/client/entities/log.py
--rw-r--r--   0        0        0    16840 2023-06-09 06:58:12.962847 modelon_impact_client-3.0.1/modelon/impact/client/entities/model.py
--rw-r--r--   0        0        0    12110 2023-06-09 06:58:12.956847 modelon_impact_client-3.0.1/modelon/impact/client/entities/model_executable.py
--rw-r--r--   0        0        0    12288 2023-06-09 06:58:13.007848 modelon_impact_client-3.0.1/modelon/impact/client/entities/project.py
--rw-r--r--   0        0        0     1986 2023-06-09 06:58:12.977847 modelon_impact_client-3.0.1/modelon/impact/client/entities/result.py
--rw-r--r--   0        0        0     1487 2023-06-09 06:58:12.948847 modelon_impact_client-3.0.1/modelon/impact/client/entities/status.py
--rw-r--r--   0        0        0    20712 2023-06-09 06:58:13.004848 modelon_impact_client-3.0.1/modelon/impact/client/entities/workspace.py
--rw-r--r--   0        0        0     1365 2023-06-09 06:58:12.959847 modelon_impact_client-3.0.1/modelon/impact/client/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/__init__.py
--rw-r--r--   0        0        0     5284 2023-06-09 06:58:13.015848 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/asserts.py
--rw-r--r--   0        0        0     3085 2023-06-09 06:58:12.957847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/expansion.py
--rw-r--r--   0        0        0    10251 2023-06-09 06:58:12.949847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/extension.py
--rw-r--r--   0        0        0    12659 2023-06-09 06:58:12.995848 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/fmu_based.py
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.990847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/__init__.py
--rw-r--r--   0        0        0      506 2023-06-09 06:58:12.958847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/definition.py
--rw-r--r--   0        0        0      409 2023-06-09 06:58:12.959847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/expansion.py
--rw-r--r--   0        0        0      187 2023-06-09 06:58:12.945847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/interfaces/extension.py
--rw-r--r--   0        0        0    18576 2023-06-09 06:58:12.963847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/model_based.py
--rw-r--r--   0        0        0     4704 2023-06-09 06:58:12.951847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/operators.py
--rw-r--r--   0        0        0      641 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/util.py
--rw-r--r--   0        0        0       65 2023-06-09 06:58:13.013848 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/__init__.py
--rw-r--r--   0        0        0     3019 2023-06-09 06:58:12.994847 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/authorize.py
--rw-r--r--   0        0        0      281 2023-06-09 06:58:13.018848 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/exceptions.py
--rw-r--r--   0        0        0     2894 2023-06-09 06:58:12.960847 modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/sal.py
--rw-r--r--   0        0        0       79 2023-06-09 06:58:12.953847 modelon_impact_client-3.0.1/modelon/impact/client/operations/__init__.py
--rw-r--r--   0        0        0     5804 2023-06-09 06:58:12.964847 modelon_impact_client-3.0.1/modelon/impact/client/operations/base.py
--rw-r--r--   0        0        0     2439 2023-06-09 06:58:12.979847 modelon_impact_client-3.0.1/modelon/impact/client/operations/case.py
--rw-r--r--   0        0        0     2502 2023-06-09 06:58:12.980847 modelon_impact_client-3.0.1/modelon/impact/client/operations/content_import.py
--rw-r--r--   0        0        0     2243 2023-06-09 06:58:12.952847 modelon_impact_client-3.0.1/modelon/impact/client/operations/experiment.py
--rw-r--r--   0        0        0     2408 2023-06-09 06:58:12.983847 modelon_impact_client-3.0.1/modelon/impact/client/operations/external_result_import.py
--rw-r--r--   0        0        0     2719 2023-06-09 06:58:12.972847 modelon_impact_client-3.0.1/modelon/impact/client/operations/fmu_import.py
--rw-r--r--   0        0        0     5845 2023-06-09 06:58:13.014848 modelon_impact_client-3.0.1/modelon/impact/client/operations/model_executable.py
--rw-r--r--   0        0        0     2629 2023-06-09 06:58:13.024848 modelon_impact_client-3.0.1/modelon/impact/client/operations/project_import.py
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.956847 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/__init__.py
--rw-r--r--   0        0        0     2599 2023-06-09 06:58:13.014848 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/conversion.py
--rw-r--r--   0        0        0     3512 2023-06-09 06:58:13.015848 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/exports.py
--rw-r--r--   0        0        0     2532 2023-06-09 06:58:12.996847 modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/imports.py
--rw-r--r--   0        0        0     3772 2023-06-09 06:58:13.001848 modelon_impact_client-3.0.1/modelon/impact/client/options.py
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.948847 modelon_impact_client-3.0.1/modelon/impact/client/py.typed
--rw-r--r--   0        0        0        0 2023-06-09 06:58:12.993847 modelon_impact_client-3.0.1/modelon/impact/client/sal/__init__.py
--rw-r--r--   0        0        0      132 2023-06-09 06:58:12.989848 modelon_impact_client-3.0.1/modelon/impact/client/sal/context.py
--rw-r--r--   0        0        0     1543 2023-06-09 06:58:12.965847 modelon_impact_client-3.0.1/modelon/impact/client/sal/custom_function.py
--rw-r--r--   0        0        0      671 2023-06-09 06:58:12.947847 modelon_impact_client-3.0.1/modelon/impact/client/sal/exceptions.py
--rw-r--r--   0        0        0     6785 2023-06-09 06:58:12.996847 modelon_impact_client-3.0.1/modelon/impact/client/sal/experiment.py
--rw-r--r--   0        0        0      629 2023-06-09 06:58:12.957847 modelon_impact_client-3.0.1/modelon/impact/client/sal/exports.py
--rw-r--r--   0        0        0     1475 2023-06-09 06:58:13.018848 modelon_impact_client-3.0.1/modelon/impact/client/sal/external_result.py
--rw-r--r--   0        0        0     3124 2023-06-09 06:58:12.985847 modelon_impact_client-3.0.1/modelon/impact/client/sal/http.py
--rw-r--r--   0        0        0      475 2023-06-09 06:58:13.023848 modelon_impact_client-3.0.1/modelon/impact/client/sal/imports.py
--rw-r--r--   0        0        0     3083 2023-06-09 06:58:13.001848 modelon_impact_client-3.0.1/modelon/impact/client/sal/model_executable.py
--rw-r--r--   0        0        0     4640 2023-06-09 06:58:12.996847 modelon_impact_client-3.0.1/modelon/impact/client/sal/project.py
--rw-r--r--   0        0        0     4877 2023-06-09 06:58:12.958847 modelon_impact_client-3.0.1/modelon/impact/client/sal/request.py
--rw-r--r--   0        0        0     5113 2023-06-09 06:58:12.978847 modelon_impact_client-3.0.1/modelon/impact/client/sal/response.py
--rw-r--r--   0        0        0     5082 2023-06-09 06:58:12.953847 modelon_impact_client-3.0.1/modelon/impact/client/sal/service.py
--rw-r--r--   0        0        0      884 2023-06-09 06:58:12.949847 modelon_impact_client-3.0.1/modelon/impact/client/sal/uri.py
--rw-r--r--   0        0        0      453 2023-06-09 06:58:12.967847 modelon_impact_client-3.0.1/modelon/impact/client/sal/users.py
--rw-r--r--   0        0        0     6995 2023-06-09 06:58:12.965847 modelon_impact_client-3.0.1/modelon/impact/client/sal/workspace.py
--rw-r--r--   0        0        0     1359 2023-06-09 06:59:15.194490 modelon_impact_client-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1479 2023-06-09 07:05:31.710359 modelon_impact_client-3.0.2/LICENSE.md
+-rw-r--r--   0        0        0     2748 2023-06-09 07:05:31.717359 modelon_impact_client-3.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.686359 modelon_impact_client-3.0.2/modelon/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.708359 modelon_impact_client-3.0.2/modelon/impact/__init__.py
+-rw-r--r--   0        0        0      830 2023-06-09 07:05:31.705359 modelon_impact_client-3.0.2/modelon/impact/client/__init__.py
+-rw-r--r--   0        0        0    24886 2023-06-09 07:05:31.690359 modelon_impact_client-3.0.2/modelon/impact/client/client.py
+-rw-r--r--   0        0        0      835 2023-06-09 07:05:31.717359 modelon_impact_client-3.0.2/modelon/impact/client/configuration.py
+-rw-r--r--   0        0        0     1938 2023-06-09 07:05:31.690359 modelon_impact_client-3.0.2/modelon/impact/client/credential_manager.py
+-rw-r--r--   0        0        0      119 2023-06-09 07:05:31.700359 modelon_impact_client-3.0.2/modelon/impact/client/entities/__init__.py
+-rw-r--r--   0        0        0      639 2023-06-09 07:05:31.683359 modelon_impact_client-3.0.2/modelon/impact/client/entities/asserts.py
+-rw-r--r--   0        0        0    24767 2023-06-09 07:05:31.716359 modelon_impact_client-3.0.2/modelon/impact/client/entities/case.py
+-rw-r--r--   0        0        0     2259 2023-06-09 07:05:31.732360 modelon_impact_client-3.0.2/modelon/impact/client/entities/content.py
+-rw-r--r--   0        0        0     6620 2023-06-09 07:05:31.692359 modelon_impact_client-3.0.2/modelon/impact/client/entities/custom_function.py
+-rw-r--r--   0        0        0    18419 2023-06-09 07:05:31.695359 modelon_impact_client-3.0.2/modelon/impact/client/entities/experiment.py
+-rw-r--r--   0        0        0     2511 2023-06-09 07:05:31.683359 modelon_impact_client-3.0.2/modelon/impact/client/entities/external_result.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.730359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/__init__.py
+-rw-r--r--   0        0        0      180 2023-06-09 07:05:31.678359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/case.py
+-rw-r--r--   0        0        0      200 2023-06-09 07:05:31.708359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/custom_function.py
+-rw-r--r--   0        0        0      366 2023-06-09 07:05:31.704359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/experiment.py
+-rw-r--r--   0        0        0      192 2023-06-09 07:05:31.705359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/external_result.py
+-rw-r--r--   0        0        0      186 2023-06-09 07:05:31.704359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/model.py
+-rw-r--r--   0        0        0      190 2023-06-09 07:05:31.700359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/model_executable.py
+-rw-r--r--   0        0        0      190 2023-06-09 07:05:31.685359 modelon_impact_client-3.0.2/modelon/impact/client/entities/interfaces/workspace.py
+-rw-r--r--   0        0        0      156 2023-06-09 07:05:31.702359 modelon_impact_client-3.0.2/modelon/impact/client/entities/log.py
+-rw-r--r--   0        0        0    16840 2023-06-09 07:05:31.695359 modelon_impact_client-3.0.2/modelon/impact/client/entities/model.py
+-rw-r--r--   0        0        0    12111 2023-06-09 07:05:31.688359 modelon_impact_client-3.0.2/modelon/impact/client/entities/model_executable.py
+-rw-r--r--   0        0        0    12288 2023-06-09 07:05:31.725359 modelon_impact_client-3.0.2/modelon/impact/client/entities/project.py
+-rw-r--r--   0        0        0     1986 2023-06-09 07:05:31.704359 modelon_impact_client-3.0.2/modelon/impact/client/entities/result.py
+-rw-r--r--   0        0        0     1487 2023-06-09 07:05:31.679359 modelon_impact_client-3.0.2/modelon/impact/client/entities/status.py
+-rw-r--r--   0        0        0    20712 2023-06-09 07:05:31.720359 modelon_impact_client-3.0.2/modelon/impact/client/entities/workspace.py
+-rw-r--r--   0        0        0     1365 2023-06-09 07:05:31.692359 modelon_impact_client-3.0.2/modelon/impact/client/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.684359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/__init__.py
+-rw-r--r--   0        0        0     5284 2023-06-09 07:05:31.739359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/asserts.py
+-rw-r--r--   0        0        0     3085 2023-06-09 07:05:31.690359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/expansion.py
+-rw-r--r--   0        0        0    10251 2023-06-09 07:05:31.680359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/extension.py
+-rw-r--r--   0        0        0    12659 2023-06-09 07:05:31.713359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/fmu_based.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.708359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/interfaces/__init__.py
+-rw-r--r--   0        0        0      506 2023-06-09 07:05:31.691359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/interfaces/definition.py
+-rw-r--r--   0        0        0      409 2023-06-09 07:05:31.692359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/interfaces/expansion.py
+-rw-r--r--   0        0        0      187 2023-06-09 07:05:31.676359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/interfaces/extension.py
+-rw-r--r--   0        0        0    18576 2023-06-09 07:05:31.696359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/model_based.py
+-rw-r--r--   0        0        0     4704 2023-06-09 07:05:31.682359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/operators.py
+-rw-r--r--   0        0        0      641 2023-06-09 07:05:31.684359 modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/util.py
+-rw-r--r--   0        0        0       65 2023-06-09 07:05:31.736359 modelon_impact_client-3.0.2/modelon/impact/client/jupyterhub/__init__.py
+-rw-r--r--   0        0        0     3019 2023-06-09 07:05:31.712359 modelon_impact_client-3.0.2/modelon/impact/client/jupyterhub/authorize.py
+-rw-r--r--   0        0        0      281 2023-06-09 07:05:31.743360 modelon_impact_client-3.0.2/modelon/impact/client/jupyterhub/exceptions.py
+-rw-r--r--   0        0        0     2894 2023-06-09 07:05:31.693359 modelon_impact_client-3.0.2/modelon/impact/client/jupyterhub/sal.py
+-rw-r--r--   0        0        0       79 2023-06-09 07:05:31.685359 modelon_impact_client-3.0.2/modelon/impact/client/operations/__init__.py
+-rw-r--r--   0        0        0     5804 2023-06-09 07:05:31.697359 modelon_impact_client-3.0.2/modelon/impact/client/operations/base.py
+-rw-r--r--   0        0        0     2439 2023-06-09 07:05:31.705359 modelon_impact_client-3.0.2/modelon/impact/client/operations/case.py
+-rw-r--r--   0        0        0     2502 2023-06-09 07:05:31.705359 modelon_impact_client-3.0.2/modelon/impact/client/operations/content_import.py
+-rw-r--r--   0        0        0     2243 2023-06-09 07:05:31.684359 modelon_impact_client-3.0.2/modelon/impact/client/operations/experiment.py
+-rw-r--r--   0        0        0     2408 2023-06-09 07:05:31.706359 modelon_impact_client-3.0.2/modelon/impact/client/operations/external_result_import.py
+-rw-r--r--   0        0        0     2719 2023-06-09 07:05:31.701359 modelon_impact_client-3.0.2/modelon/impact/client/operations/fmu_import.py
+-rw-r--r--   0        0        0     5845 2023-06-09 07:05:31.737360 modelon_impact_client-3.0.2/modelon/impact/client/operations/model_executable.py
+-rw-r--r--   0        0        0     2629 2023-06-09 07:05:31.747360 modelon_impact_client-3.0.2/modelon/impact/client/operations/project_import.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.688359 modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/__init__.py
+-rw-r--r--   0        0        0     2599 2023-06-09 07:05:31.737360 modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/conversion.py
+-rw-r--r--   0        0        0     3512 2023-06-09 07:05:31.740360 modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/exports.py
+-rw-r--r--   0        0        0     2532 2023-06-09 07:05:31.713359 modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/imports.py
+-rw-r--r--   0        0        0     3772 2023-06-09 07:05:31.718359 modelon_impact_client-3.0.2/modelon/impact/client/options.py
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.679359 modelon_impact_client-3.0.2/modelon/impact/client/py.typed
+-rw-r--r--   0        0        0        0 2023-06-09 07:05:31.711359 modelon_impact_client-3.0.2/modelon/impact/client/sal/__init__.py
+-rw-r--r--   0        0        0      132 2023-06-09 07:05:31.708359 modelon_impact_client-3.0.2/modelon/impact/client/sal/context.py
+-rw-r--r--   0        0        0     1543 2023-06-09 07:05:31.698359 modelon_impact_client-3.0.2/modelon/impact/client/sal/custom_function.py
+-rw-r--r--   0        0        0      671 2023-06-09 07:05:31.677359 modelon_impact_client-3.0.2/modelon/impact/client/sal/exceptions.py
+-rw-r--r--   0        0        0     6785 2023-06-09 07:05:31.713359 modelon_impact_client-3.0.2/modelon/impact/client/sal/experiment.py
+-rw-r--r--   0        0        0      629 2023-06-09 07:05:31.689359 modelon_impact_client-3.0.2/modelon/impact/client/sal/exports.py
+-rw-r--r--   0        0        0     1475 2023-06-09 07:05:31.744360 modelon_impact_client-3.0.2/modelon/impact/client/sal/external_result.py
+-rw-r--r--   0        0        0     3124 2023-06-09 07:05:31.706359 modelon_impact_client-3.0.2/modelon/impact/client/sal/http.py
+-rw-r--r--   0        0        0      475 2023-06-09 07:05:31.747360 modelon_impact_client-3.0.2/modelon/impact/client/sal/imports.py
+-rw-r--r--   0        0        0     3083 2023-06-09 07:05:31.718359 modelon_impact_client-3.0.2/modelon/impact/client/sal/model_executable.py
+-rw-r--r--   0        0        0     4640 2023-06-09 07:05:31.714359 modelon_impact_client-3.0.2/modelon/impact/client/sal/project.py
+-rw-r--r--   0        0        0     4877 2023-06-09 07:05:31.691359 modelon_impact_client-3.0.2/modelon/impact/client/sal/request.py
+-rw-r--r--   0        0        0     5113 2023-06-09 07:05:31.704359 modelon_impact_client-3.0.2/modelon/impact/client/sal/response.py
+-rw-r--r--   0        0        0     5082 2023-06-09 07:05:31.685359 modelon_impact_client-3.0.2/modelon/impact/client/sal/service.py
+-rw-r--r--   0        0        0      884 2023-06-09 07:05:31.680359 modelon_impact_client-3.0.2/modelon/impact/client/sal/uri.py
+-rw-r--r--   0        0        0      453 2023-06-09 07:05:31.699359 modelon_impact_client-3.0.2/modelon/impact/client/sal/users.py
+-rw-r--r--   0        0        0     6995 2023-06-09 07:05:31.698359 modelon_impact_client-3.0.2/modelon/impact/client/sal/workspace.py
+-rw-r--r--   0        0        0     1359 2023-06-09 07:06:29.836957 modelon_impact_client-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.0.2/PKG-INFO
```

### Comparing `modelon_impact_client-3.0.1/LICENSE.md` & `modelon_impact_client-3.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/README.md` & `modelon_impact_client-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/__init__.py` & `modelon_impact_client-3.0.2/modelon/impact/client/__init__.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/client.py` & `modelon_impact_client-3.0.2/modelon/impact/client/client.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/configuration.py` & `modelon_impact_client-3.0.2/modelon/impact/client/configuration.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/credential_manager.py` & `modelon_impact_client-3.0.2/modelon/impact/client/credential_manager.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/asserts.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/case.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/content.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/content.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/custom_function.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/experiment.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/external_result.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/model.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/model.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/model_executable.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/model_executable.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
     elif status == ModelExecutableStatus.CANCELLED:
         raise exceptions.OperationFailureError.for_operation(operation_name)
 
 
 class ModelDescription(str):
     """ModelDescription class inheriting from string object."""
 
-    def show(self) -> str:
+    def show(self) -> None:
         """Prints the formatted xml."""
-        return self
+        print(self)
 
     def download(self, path: Optional[str] = None) -> str:
         """Downloads the formatted xml.
 
         Args:
             path: The local path to store the downloaded model description.
                 Default: None. If no path is given, model description will
```

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/project.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/result.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/status.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/status.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/entities/workspace.py` & `modelon_impact_client-3.0.2/modelon/impact/client/entities/workspace.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/exceptions.py` & `modelon_impact_client-3.0.2/modelon/impact/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/asserts.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/expansion.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/expansion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/extension.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/extension.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/fmu_based.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/fmu_based.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/model_based.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/model_based.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/operators.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/operators.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/experiment_definition/util.py` & `modelon_impact_client-3.0.2/modelon/impact/client/experiment_definition/util.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/authorize.py` & `modelon_impact_client-3.0.2/modelon/impact/client/jupyterhub/authorize.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/jupyterhub/sal.py` & `modelon_impact_client-3.0.2/modelon/impact/client/jupyterhub/sal.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/base.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/base.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/case.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/content_import.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/content_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/experiment.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/external_result_import.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/external_result_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/fmu_import.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/fmu_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/model_executable.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/project_import.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/project_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/conversion.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/conversion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/exports.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/operations/workspace/imports.py` & `modelon_impact_client-3.0.2/modelon/impact/client/operations/workspace/imports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/options.py` & `modelon_impact_client-3.0.2/modelon/impact/client/options.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/custom_function.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/exceptions.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/experiment.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/exports.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/external_result.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/http.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/http.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/model_executable.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/project.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/request.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/request.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/response.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/response.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/service.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/service.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/uri.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/uri.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/modelon/impact/client/sal/workspace.py` & `modelon_impact_client-3.0.2/modelon/impact/client/sal/workspace.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.0.1/pyproject.toml` & `modelon_impact_client-3.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modelon-impact-client"
 packages = [
     { include = "modelon" },
 ]
-version = "3.0.1"
+version = "3.0.2"
 description = "Client library for easy scripting against Modelon Impact"
 readme = "README.md"
 homepage = "https://www.modelon.com/modelon-impact"
 repository = "https://github.com/modelon-community/impact-client-python"
 documentation = "https://modelon-impact-client.readthedocs.io"
 license = "BSD"
 authors = [
```

### Comparing `modelon_impact_client-3.0.1/PKG-INFO` & `modelon_impact_client-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelon-impact-client
-Version: 3.0.1
+Version: 3.0.2
 Summary: Client library for easy scripting against Modelon Impact
 Home-page: https://www.modelon.com/modelon-impact
 License: BSD
 Keywords: impact,client,API
 Author: WEP
 Author-email: impact@modelon.com
 Requires-Python: >=3.9.0,<4.0.0
```

