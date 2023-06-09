# Comparing `tmp/servicefoundry-0.9.5.tar.gz` & `tmp/servicefoundry-0.9.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "servicefoundry-0.9.5.tar", max compression
+gzip compressed data, was "servicefoundry-0.9.6rc1.tar", max compression
```

## Comparing `servicefoundry-0.9.5.tar` & `servicefoundry-0.9.6rc1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0      672 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/README.md
--rw-r--r--   0        0        0     2116 2023-06-07 11:33:27.644514 servicefoundry-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     1365 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/__init__.py
--rw-r--r--   0        0        0    39576 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/auto_gen/models.py
--rw-r--r--   0        0        0     4294 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/__init__.py
--rw-r--r--   0        0        0      632 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/builders/__init__.py
--rw-r--r--   0        0        0     1364 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/builders/dockerfile.py
--rw-r--r--   0        0        0     1317 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
--rw-r--r--   0        0        0     1369 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     1357 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
--rw-r--r--   0        0        0     6496 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
--rw-r--r--   0        0        0     6480 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/builder/docker_service.py
--rw-r--r--   0        0        0       66 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/__init__.py
--rw-r--r--   0        0        0      494 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/__main__.py
--rw-r--r--   0        0        0     3089 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/cli_main.py
--rw-r--r--   0        0        0      958 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/__init__.py
--rw-r--r--   0        0        0     1042 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/build_command.py
--rw-r--r--   0        0        0     2788 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/build_logs_command.py
--rw-r--r--   0        0        0     1834 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/create_command.py
--rw-r--r--   0        0        0     2358 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/delete_command.py
--rw-r--r--   0        0        0     1227 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/deploy_v2_command.py
--rw-r--r--   0        0        0     3536 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/get_command.py
--rw-r--r--   0        0        0     2944 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/infra_bootstrap.py
--rw-r--r--   0        0        0     4462 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/list_command.py
--rw-r--r--   0        0        0      938 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/login_command.py
--rw-r--r--   0        0        0      534 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/logout_command.py
--rw-r--r--   0        0        0     4134 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/logs_command.py
--rw-r--r--   0        0        0     1670 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/patch_command.py
--rw-r--r--   0        0        0     1020 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/redeploy_command.py
--rw-r--r--   0        0        0     2752 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/commands/trigger_command.py
--rw-r--r--   0        0        0      206 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/config.py
--rw-r--r--   0        0        0      242 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/console.py
--rw-r--r--   0        0        0      510 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/const.py
--rw-r--r--   0        0        0     2970 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/display_util.py
--rw-r--r--   0        0        0     2500 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/cli/util.py
--rw-r--r--   0        0        0      132 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/core/__init__.py
--rw-r--r--   0        0        0      232 2023-06-07 11:33:16.768414 servicefoundry-0.9.5/servicefoundry/core/login.py
--rw-r--r--   0        0        0       76 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/core/logout.py
--rw-r--r--   0        0        0      188 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/__init__.py
--rw-r--r--   0        0        0      775 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/__main__.py
--rw-r--r--   0        0        0     2857 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/app.py
--rw-r--r--   0        0        0     1844 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/build.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
--rw-r--r--   0        0        0      673 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
--rw-r--r--   0        0        0      185 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
--rw-r--r--   0        0        0      600 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
--rw-r--r--   0        0        0      297 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
--rw-r--r--   0        0        0     1772 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
--rw-r--r--   0        0        0      369 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/model.py
--rw-r--r--   0        0        0     1513 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
--rw-r--r--   0        0        0      153 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/utils.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
--rw-r--r--   0        0        0      406 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
--rw-r--r--   0        0        0      518 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
--rw-r--r--   0        0        0      191 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/remote/__init__.py
--rw-r--r--   0        0        0       67 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/remote/context.py
--rw-r--r--   0        0        0     1875 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/remote/method.py
--rw-r--r--   0        0        0     4210 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/remote/remote.py
--rw-r--r--   0        0        0     4494 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/route.py
--rw-r--r--   0        0        0     4139 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/service.py
--rw-r--r--   0        0        0     1231 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/function_service/utils.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/internal/__init__.py
--rw-r--r--   0        0        0      960 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/internal/experimental.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/io/__init__.py
--rw-r--r--   0        0        0      604 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/io/output_callback.py
--rw-r--r--   0        0        0      825 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/io/rich_output_callback.py
--rw-r--r--   0        0        0      175 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/json_util.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/__init__.py
--rw-r--r--   0        0        0     2906 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/auth/auth_service_client.py
--rw-r--r--   0        0        0     4228 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/auth/credential_file_manager.py
--rw-r--r--   0        0        0     4268 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/auth/credential_provider.py
--rw-r--r--   0        0        0     1854 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/auth/servicefoundry_session.py
--rw-r--r--   0        0        0     7447 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/binarydownloader.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/__init__.py
--rw-r--r--   0        0        0      671 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/cookiecutter_client.py
--rw-r--r--   0        0        0     2563 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/git_client.py
--rw-r--r--   0        0        0    25229 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/service_foundry_client.py
--rw-r--r--   0        0        0      455 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/shell_client.py
--rw-r--r--   0        0        0     1455 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/terragrunt_client.py
--rw-r--r--   0        0        0     1122 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/clients/utils.py
--rw-r--r--   0        0        0     1331 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/config/config_manager.py
--rw-r--r--   0        0        0     2237 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/config/dict_questionaire.py
--rw-r--r--   0        0        0    10594 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/config/infra_config.py
--rw-r--r--   0        0        0     1886 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/config/installation_config.py
--rw-r--r--   0        0        0     1752 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/const.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/dao/__init__.py
--rw-r--r--   0        0        0     6485 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/dao/application.py
--rw-r--r--   0        0        0     1123 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/dao/version.py
--rw-r--r--   0        0        0     2344 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/dao/workspace.py
--rw-r--r--   0        0        0      588 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/exceptions.py
--rw-r--r--   0        0        0      288 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/argo-secrets.mustache
--rw-r--r--   0        0        0      918 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/argo-ubermold.mustache
--rw-r--r--   0        0        0    23708 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/install_truefoundry.py
--rw-r--r--   0        0        0     1411 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/nats-bootstrap.sh
--rw-r--r--   0        0        0      328 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/tfy-agent.mustache
--rw-r--r--   0        0        0     1137 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/tfy-control-plane.mustache
--rw-r--r--   0        0        0     6290 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/infra/utils.py
--rw-r--r--   0        0        0     1463 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/logs_utils.py
--rw-r--r--   0        0        0      861 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/messages.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/model/__init__.py
--rw-r--r--   0        0        0    10866 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/model/entity.py
--rw-r--r--   0        0        0     5208 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/session.py
--rw-r--r--   0        0        0     1664 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/util.py
--rw-r--r--   0        0        0     4995 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/lib/win32.py
--rw-r--r--   0        0        0      688 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/logger.py
--rw-r--r--   0        0        0        0 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/__init__.py
--rw-r--r--   0        0        0      517 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/deploy.py
--rw-r--r--   0        0        0      305 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/main.py
--rw-r--r--   0        0        0      303 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      441 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
--rw-r--r--   0        0        0      524 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
--rw-r--r--   0        0        0      639 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/model_deployment/hf/deploy.py
--rw-r--r--   0        0        0      190 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
--rw-r--r--   0        0        0      579 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
--rw-r--r--   0        0        0      313 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
--rw-r--r--   0        0        0      764 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/service_deployment/deploy.py
--rw-r--r--   0        0        0      117 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/service_deployment/main.py
--rw-r--r--   0        0        0      482 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
--rw-r--r--   0        0        0      188 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/lib/__init__.py
--rw-r--r--   0        0        0    10072 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/lib/deploy.py
--rw-r--r--   0        0        0     1876 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/lib/deployable_patched_models.py
--rw-r--r--   0        0        0     1105 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/lib/models.py
--rw-r--r--   0        0        0     5396 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/lib/patched_models.py
--rw-r--r--   0        0        0     8988 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/v2/lib/source.py
--rw-r--r--   0        0        0      130 2023-06-07 11:33:16.772414 servicefoundry-0.9.5/servicefoundry/version.py
--rw-r--r--   0        0        0     2440 1970-01-01 00:00:00.000000 servicefoundry-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0      672 2023-06-09 12:16:06.846536 servicefoundry-0.9.6rc1/README.md
+-rw-r--r--   0        0        0     2119 2023-06-09 12:16:18.582633 servicefoundry-0.9.6rc1/pyproject.toml
+-rw-r--r--   0        0        0     1365 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/__init__.py
+-rw-r--r--   0        0        0    40084 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/auto_gen/models.py
+-rw-r--r--   0        0        0     4294 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/__init__.py
+-rw-r--r--   0        0        0      632 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/builders/__init__.py
+-rw-r--r--   0        0        0     1506 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/builders/dockerfile.py
+-rw-r--r--   0        0        0     1317 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py
+-rw-r--r--   0        0        0     1369 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     1357 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py
+-rw-r--r--   0        0        0     6496 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py
+-rw-r--r--   0        0        0     6972 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/builder/docker_service.py
+-rw-r--r--   0        0        0       66 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/__init__.py
+-rw-r--r--   0        0        0      494 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/__main__.py
+-rw-r--r--   0        0        0     3089 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/cli_main.py
+-rw-r--r--   0        0        0      958 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1232 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/build_command.py
+-rw-r--r--   0        0        0     2788 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/build_logs_command.py
+-rw-r--r--   0        0        0     1834 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/create_command.py
+-rw-r--r--   0        0        0     2358 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/delete_command.py
+-rw-r--r--   0        0        0     1227 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/deploy_v2_command.py
+-rw-r--r--   0        0        0     3536 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/get_command.py
+-rw-r--r--   0        0        0     2944 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/infra_bootstrap.py
+-rw-r--r--   0        0        0     4462 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/list_command.py
+-rw-r--r--   0        0        0      938 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/login_command.py
+-rw-r--r--   0        0        0      534 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/logout_command.py
+-rw-r--r--   0        0        0     4134 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/logs_command.py
+-rw-r--r--   0        0        0     1670 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/patch_command.py
+-rw-r--r--   0        0        0     1020 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/redeploy_command.py
+-rw-r--r--   0        0        0     2752 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/commands/trigger_command.py
+-rw-r--r--   0        0        0      206 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/config.py
+-rw-r--r--   0        0        0      242 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/console.py
+-rw-r--r--   0        0        0      510 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/const.py
+-rw-r--r--   0        0        0     2970 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/display_util.py
+-rw-r--r--   0        0        0     2500 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/cli/util.py
+-rw-r--r--   0        0        0      132 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/core/__init__.py
+-rw-r--r--   0        0        0      232 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/core/login.py
+-rw-r--r--   0        0        0       76 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/core/logout.py
+-rw-r--r--   0        0        0      188 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/__init__.py
+-rw-r--r--   0        0        0      775 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/__main__.py
+-rw-r--r--   0        0        0     2857 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/app.py
+-rw-r--r--   0        0        0     1844 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/build.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/class_deployment/__init__.py
+-rw-r--r--   0        0        0      673 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py
+-rw-r--r--   0        0        0      185 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/class_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/function_deployment/__init__.py
+-rw-r--r--   0        0        0      600 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py
+-rw-r--r--   0        0        0      297 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/function_deployment/my_module.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/__init__.py
+-rw-r--r--   0        0        0     1772 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py
+-rw-r--r--   0        0        0      369 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/model.py
+-rw-r--r--   0        0        0     1513 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py
+-rw-r--r--   0        0        0      153 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/deployment.py
+-rw-r--r--   0        0        0      518 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py
+-rw-r--r--   0        0        0      191 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/remote/__init__.py
+-rw-r--r--   0        0        0       67 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/remote/context.py
+-rw-r--r--   0        0        0     1875 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/remote/method.py
+-rw-r--r--   0        0        0     4210 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/remote/remote.py
+-rw-r--r--   0        0        0     4494 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/route.py
+-rw-r--r--   0        0        0     4139 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/service.py
+-rw-r--r--   0        0        0     1231 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/function_service/utils.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/internal/__init__.py
+-rw-r--r--   0        0        0      960 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/internal/experimental.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/io/__init__.py
+-rw-r--r--   0        0        0      604 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/io/output_callback.py
+-rw-r--r--   0        0        0      825 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/io/rich_output_callback.py
+-rw-r--r--   0        0        0      175 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/json_util.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/__init__.py
+-rw-r--r--   0        0        0     2906 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/auth/auth_service_client.py
+-rw-r--r--   0        0        0     4228 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/auth/credential_file_manager.py
+-rw-r--r--   0        0        0     4268 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/auth/credential_provider.py
+-rw-r--r--   0        0        0     1854 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/auth/servicefoundry_session.py
+-rw-r--r--   0        0        0     7447 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/binarydownloader.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/__init__.py
+-rw-r--r--   0        0        0      671 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/cookiecutter_client.py
+-rw-r--r--   0        0        0     2563 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/git_client.py
+-rw-r--r--   0        0        0    25229 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/service_foundry_client.py
+-rw-r--r--   0        0        0      455 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/shell_client.py
+-rw-r--r--   0        0        0     1455 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/terragrunt_client.py
+-rw-r--r--   0        0        0     1122 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/clients/utils.py
+-rw-r--r--   0        0        0     1331 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/config/config_manager.py
+-rw-r--r--   0        0        0     2237 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/config/dict_questionaire.py
+-rw-r--r--   0        0        0    10594 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/config/infra_config.py
+-rw-r--r--   0        0        0     1886 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/config/installation_config.py
+-rw-r--r--   0        0        0     1752 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/const.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/dao/__init__.py
+-rw-r--r--   0        0        0     6485 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/dao/application.py
+-rw-r--r--   0        0        0     1123 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/dao/version.py
+-rw-r--r--   0        0        0     2344 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/dao/workspace.py
+-rw-r--r--   0        0        0      588 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/exceptions.py
+-rw-r--r--   0        0        0      288 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/argo-secrets.mustache
+-rw-r--r--   0        0        0      918 2023-06-09 12:16:06.850536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/argo-ubermold.mustache
+-rw-r--r--   0        0        0    23708 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/install_truefoundry.py
+-rw-r--r--   0        0        0     1411 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/nats-bootstrap.sh
+-rw-r--r--   0        0        0      328 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/tfy-agent.mustache
+-rw-r--r--   0        0        0     1137 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/tfy-control-plane.mustache
+-rw-r--r--   0        0        0     6290 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/infra/utils.py
+-rw-r--r--   0        0        0     1463 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/logs_utils.py
+-rw-r--r--   0        0        0      861 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/messages.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/model/__init__.py
+-rw-r--r--   0        0        0    10866 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/model/entity.py
+-rw-r--r--   0        0        0     5208 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/session.py
+-rw-r--r--   0        0        0     1664 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/util.py
+-rw-r--r--   0        0        0     4995 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/lib/win32.py
+-rw-r--r--   0        0        0      688 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/logger.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/__init__.py
+-rw-r--r--   0        0        0      517 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/deploy.py
+-rw-r--r--   0        0        0      305 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/main.py
+-rw-r--r--   0        0        0      303 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      441 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_manual.yaml
+-rw-r--r--   0        0        0      524 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml
+-rw-r--r--   0        0        0      639 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py
+-rw-r--r--   0        0        0      190 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/model_deployment/hf/servicefoundry.yaml
+-rw-r--r--   0        0        0      579 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py
+-rw-r--r--   0        0        0      313 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/servicefoundry.yaml
+-rw-r--r--   0        0        0      764 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/service_deployment/deploy.py
+-rw-r--r--   0        0        0      117 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/service_deployment/main.py
+-rw-r--r--   0        0        0      482 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/examples/service_deployment/servicefoundry.yaml
+-rw-r--r--   0        0        0      188 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/lib/__init__.py
+-rw-r--r--   0        0        0    10072 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/lib/deploy.py
+-rw-r--r--   0        0        0     1876 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/lib/deployable_patched_models.py
+-rw-r--r--   0        0        0     1105 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/lib/models.py
+-rw-r--r--   0        0        0     5491 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/lib/patched_models.py
+-rw-r--r--   0        0        0     8988 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/v2/lib/source.py
+-rw-r--r--   0        0        0      130 2023-06-09 12:16:06.854536 servicefoundry-0.9.6rc1/servicefoundry/version.py
+-rw-r--r--   0        0        0     2443 1970-01-01 00:00:00.000000 servicefoundry-0.9.6rc1/PKG-INFO
```

### Comparing `servicefoundry-0.9.5/README.md` & `servicefoundry-0.9.6rc1/README.md`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/pyproject.toml` & `servicefoundry-0.9.6rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "servicefoundry"
-version = "0.9.5"  # do not change, auto-generated by poetry-dynamic-versioning
+version = "0.9.6rc1"  # do not change, auto-generated by poetry-dynamic-versioning
 description = "Generate deployed services from code"
 authors = ["Abhishek Choudhary <abhichoudhary06@gmail.com>"]
 homepage = "https://github.com/innoavator/servicefoundry"
 repository = "https://github.com/innoavator/servicefoundry"
 readme = "README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `servicefoundry-0.9.5/servicefoundry/__init__.py` & `servicefoundry-0.9.6rc1/servicefoundry/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/auto_gen/models.py` & `servicefoundry-0.9.6rc1/servicefoundry/auto_gen/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  application.json
-#   timestamp: 2023-06-06T08:33:20+00:00
+#   timestamp: 2023-06-09T11:30:15+00:00
 
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, Field, confloat, conint, constr
@@ -80,14 +80,18 @@
         "./",
         description="+label=Path to build context\n+usage=Build context path for the Dockerfile relative to project root path.",
     )
     command: Optional[Union[str, List[str]]] = Field(
         None,
         description="+label=Entrypoint Override\n+usage=Override the command to run when the container starts\nWhen deploying a Job, the command can be templatized by defining `params` and referencing them in command\nE.g. `python main.py --learning_rate {{learning_rate}}`",
     )
+    build_args: Optional[Dict[str, str]] = Field(
+        None,
+        description="+label=Build Args\n+usage=Build arguments to pass to `docker build`.",
+    )
 
 
 class Endpoint(BaseModel):
     host: constr(
         regex=r"^(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-]*[a-zA-Z0-9])\.)(([a-zA-Z0-9]|[a-zA-Z0-9][a-zA-Z0-9\-]*[a-zA-Z0-9])\.)*([A-Za-z0-9]|[A-Za-z0-9][A-Za-z0-9\-]*[A-Za-z0-9])$"
     ) = Field(
         ...,
@@ -238,15 +242,16 @@
     spot_fallback_on_demand = "spot_fallback_on_demand"
     spot = "spot"
     on_demand = "on_demand"
 
 
 class NodeSelector(BaseModel):
     """
-    +label=Node selector
+        +label=Node selector
+    +usage=Constraints to select a Node - Specific GPU / Instance Families, On-Demand/Spot.
     """
 
     type: Literal["node_selector"] = Field(..., description="+value=node_selector")
     gpu_type: Optional[str] = Field(
         None,
         description="+label=GPU Type\n+usage=Name of the Nvidia GPU. One of [K80, P4, P100, V100, T4, A10G, A100_40GB, A100_80GB]\nOne instance of the card contains the following amount of memory -\nK80: 12 GB, P4: 8 GB, P100: 16 GB, V100: 16 GB, T4: 16 GB, A10G: 24 GB, A100_40GB: 40GB, A100_80GB: 80 GB",
     )
@@ -258,15 +263,16 @@
         None,
         description='+label=Capacity Type\n+usage=Configure what type of nodes to run the app. By default no placement logic is applied.\n"spot_fallback_on_demand" will try to place the application on spot nodes but will fallback to on-demand when spot nodes are not available.\n"spot" will strictly place the application on spot nodes.\n"on_demand" will strictly place the application on on-demand nodes.',
     )
 
 
 class NodepoolSelector(BaseModel):
     """
-    +label=Node pool selector
+        +label=Nodepool selector
+    +usage=Specify one or more nodepools to run your application on.
     """
 
     type: Literal["nodepool_selector"] = Field(
         ..., description="+value=nodepool_selector"
     )
     nodepools: Optional[List[str]] = Field(
         None,
@@ -375,19 +381,19 @@
     )
     requirements_path: Optional[str] = Field(
         None,
         description="`Path to build context`\n+label=Path to requirements\n+usage=Path to `requirements.txt` relative to\n`Path to build context`",
     )
     pip_packages: Optional[List[str]] = Field(
         None,
-        description="+label=Pip packages to install\n+usage=Define pip package requirements.",
+        description='+label=Pip packages to install\n+usage=Define pip package requirements.\nIn Python/YAML E.g. ["fastapi>=0.90,<1.0", "uvicorn"]\n+placeholder=Enter a pip package name E.g. fastapi>=0.90,<1.0',
     )
     apt_packages: Optional[List[str]] = Field(
         None,
-        description='+label=Debian packages to install via apt.\n+usage=Define Debian packages to install via apt.\nE.g. `["ffmpeg", "libsm6", "libxext6"]',
+        description='+label=List of Debian packages to install.\n+usage=Debian packages to install via `apt get`.\nIn Python/YAML E.g. ["git", "ffmpeg", "htop"]\n+placeholder=Enter a debian package name E.g. ffmpeg',
     )
     command: Union[str, List[str]] = Field(
         ...,
         description="Command will be set as the Entrypoint of the generated\nimage.\n+label=Command\n+usage=Command to run when the container starts.\nCommand will be set as the Entrypoint of the generated image.\nWhen deploying a Job, the command can be templatized by defining `params` and referencing them in command\nE.g. `python main.py --learning_rate {{learning_rate}}`",
     )
     cuda_version: Optional[
         constr(
```

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/__init__.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/builders/__init__.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/builders/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/builders/dockerfile.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/builders/dockerfile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Optional
+from typing import Any, Dict, Optional
 
 from servicefoundry.auto_gen.models import DockerFileBuild
 from servicefoundry.builder.docker_service import build_docker_image
 from servicefoundry.logger import logger
 
 __all__ = ["build"]
 
@@ -12,27 +12,29 @@
     return os.path.abspath(os.path.expanduser(path))
 
 
 def _build_docker_image(
     tag: str,
     path: str = ".",
     file: Optional[str] = None,
+    build_args: Optional[Dict[str, str]] = None,
     cache_from: Optional[str] = None,
 ):
     path = _get_expanded_and_absolute_path(path)
 
     if file:
         file = _get_expanded_and_absolute_path(file)
 
     build_docker_image(
         path=path,
         tag=tag,
         # TODO: can we pick target platform(s) picked from cluster
         platform="linux/amd64",
         dockerfile=file,
+        build_args=build_args,
         cache_from=[cache_from],
     )
 
 
 def build(
     tag: str,
     build_configuration: DockerFileBuild,
@@ -46,9 +48,10 @@
         logger.info("Dockerfile content:-")
         logger.info(dockerfile_content)
 
     _build_docker_image(
         tag=tag,
         path=build_configuration.build_context_path,
         file=build_configuration.dockerfile_path,
+        build_args=build_configuration.build_args,
         cache_from=cache_from,
     )
```

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_notebook_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_python_buildpack/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/builders/tfy_python_buildpack/dockerfile_template.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/builder/docker_service.py` & `servicefoundry-0.9.6rc1/servicefoundry/builder/docker_service.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import collections
 import os
-from typing import Any, Dict, Iterator, List
+from typing import Any, Dict, Iterator, List, Optional
 
 import docker
 from docker.errors import APIError, BuildError
 from pydantic import BaseModel
 from rich.console import Console
 
 from servicefoundry.lib.clients.shell_client import Shell
@@ -79,14 +79,20 @@
                 line = str(value)
                 if line.strip():
                     parts.append(line.rstrip())
         if parts:
             console.print(" ".join(parts))
 
 
+def _get_build_args_string(build_args: Optional[Dict[str, str]] = None) -> str:
+    if not build_args:
+        return None
+    return ",".join([f"{param}={value}" for param, value in build_args.items()])
+
+
 def _get_docker_client():
     try:
         return docker.from_env()
     except Exception as ex:
         raise Exception("Could not connect to Docker") from ex
 
 
@@ -107,47 +113,55 @@
         if line.get("error") is not None:
             raise Exception(
                 f'Failed to push to registry with message \'{line.get("error")}\''
             )
 
 
 def build_docker_image(
-    path: str, tag: str, platform: str, dockerfile: str, cache_from: List[str]
+    path: str,
+    tag: str,
+    platform: str,
+    dockerfile: str,
+    cache_from: List[str],
+    build_args: Optional[Dict[str, str]] = None,
 ):
     use_depot = bool(os.environ.get("USE_DEPOT"))
     depot_project_id = os.environ.get("DEPOT_PROJECT_KEY")
     logger.info("Starting docker build...")
     if use_depot and depot_project_id:
         try:
-            Shell().execute_shell_command(
-                [
-                    "depot",
-                    "build",
-                    "--project",
-                    depot_project_id,
-                    "-f",
-                    dockerfile,
-                    "-t",
-                    tag,
-                    path,
-                    "--push",
-                ]
-            )
+            command = [
+                "depot",
+                "build",
+                "--project",
+                depot_project_id,
+                "-f",
+                dockerfile,
+                "-t",
+                tag,
+                path,
+            ]
+            final_build_args = _get_build_args_string(build_args=build_args)
+            if final_build_args:
+                command.extend(["--build-arg", final_build_args])
+            command.append("--push")  # keep push at last
+            Shell().execute_shell_command(command=command)
         except Exception as e:
             raise Exception("Error while building Docker image using Depot") from e
     else:
         try:
             # TODO (chiragjn): Maybe consider using client.images.build
             build_logs = _get_docker_client().api.build(
                 decode=True,
                 path=path,
                 tag=tag,
                 platform=platform,
                 dockerfile=dockerfile,
                 cache_from=cache_from,
+                buildargs=build_args,
             )
             _stream_docker_build_logs(build_logs)
         except (BuildError, APIError) as e:
             raise Exception("Error while building Docker image") from e
 
 
 def push_docker_image(
```

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/cli_main.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/cli_main.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/__init__.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/build_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/build_command.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import json
 
 import rich_click as click
 
 from servicefoundry import builder
+from servicefoundry.cli.console import console
 from servicefoundry.cli.const import GROUP_CLS
 from servicefoundry.cli.util import handle_exception_wrapper
+from servicefoundry.version import __version__ as servicefoundry_version
 
 
 @click.group(
     name="build",
     cls=GROUP_CLS,
     invoke_without_command=True,
     help="Build docker image locally from Truefoundry spec",
@@ -31,15 +33,15 @@
     type=click.STRING,
     default=None,
     help="Docker repository to use as a cache to pull layers from",
 )
 @handle_exception_wrapper
 def build_command(name, cache, build_config):
     if build_config:
+        console.print(rf"\[build] Servicefoundry version: {servicefoundry_version}")
         builder.build(
             build_configuration=json.loads(build_config), tag=name, cache_from=cache
         )
-        return
 
 
 def get_build_command():
     return build_command
```

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/build_logs_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/build_logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/create_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/create_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/delete_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/delete_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/deploy_v2_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/deploy_v2_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/get_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/get_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/infra_bootstrap.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/infra_bootstrap.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/list_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/list_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/login_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/login_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/logout_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/logout_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/logs_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/logs_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/patch_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/patch_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/redeploy_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/redeploy_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/commands/trigger_command.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/commands/trigger_command.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/display_util.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/display_util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/cli/util.py` & `servicefoundry-0.9.6rc1/servicefoundry/cli/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/__main__.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/__main__.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/app.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/app.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/build.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/build.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/class_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/function_deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/deployment.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/deployment.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/model_composition/model_composition.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/deployment_examples/one_service_calling_another/my_module.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/remote/method.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/remote/method.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/remote/remote.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/remote/remote.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/route.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/route.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/service.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/service.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/function_service/utils.py` & `servicefoundry-0.9.6rc1/servicefoundry/function_service/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/internal/experimental.py` & `servicefoundry-0.9.6rc1/servicefoundry/internal/experimental.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/io/output_callback.py` & `servicefoundry-0.9.6rc1/servicefoundry/io/output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/io/rich_output_callback.py` & `servicefoundry-0.9.6rc1/servicefoundry/io/rich_output_callback.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/auth/auth_service_client.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/auth/auth_service_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/auth/credential_file_manager.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/auth/credential_file_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/auth/credential_provider.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/auth/credential_provider.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/auth/servicefoundry_session.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/auth/servicefoundry_session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/binarydownloader.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/binarydownloader.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/clients/cookiecutter_client.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/clients/cookiecutter_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/clients/git_client.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/clients/git_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/clients/service_foundry_client.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/clients/service_foundry_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/clients/terragrunt_client.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/clients/terragrunt_client.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/clients/utils.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/clients/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/config/config_manager.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/config/config_manager.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/config/dict_questionaire.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/config/dict_questionaire.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/config/infra_config.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/config/infra_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/config/installation_config.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/config/installation_config.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/const.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/const.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/dao/application.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/dao/application.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/dao/version.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/dao/version.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/dao/workspace.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/dao/workspace.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/exceptions.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/infra/argo-ubermold.mustache` & `servicefoundry-0.9.6rc1/servicefoundry/lib/infra/argo-ubermold.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/infra/install_truefoundry.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/infra/install_truefoundry.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/infra/nats-bootstrap.sh` & `servicefoundry-0.9.6rc1/servicefoundry/lib/infra/nats-bootstrap.sh`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/infra/tfy-control-plane.mustache` & `servicefoundry-0.9.6rc1/servicefoundry/lib/infra/tfy-control-plane.mustache`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/infra/utils.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/infra/utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/logs_utils.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/logs_utils.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/messages.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/messages.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/model/entity.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/model/entity.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/session.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/session.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/util.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/util.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/lib/win32.py` & `servicefoundry-0.9.6rc1/servicefoundry/lib/win32.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/logger.py` & `servicefoundry-0.9.6rc1/servicefoundry/logger.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/deploy.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml` & `servicefoundry-0.9.6rc1/servicefoundry/v2/examples/job_deployment/servicefoundry_schedule.yaml`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/examples/model_deployment/hf/deploy.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/examples/model_deployment/hf/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/examples/model_deployment/mlfoundry/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/examples/service_deployment/deploy.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/examples/service_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/lib/deploy.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/lib/deploy.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/lib/deployable_patched_models.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/lib/deployable_patched_models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/lib/models.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/lib/models.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/lib/patched_models.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/lib/patched_models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import enum
 import re
-from typing import Optional, Union
+from typing import Dict, Optional, Union
 
 from pydantic import Field, constr, root_validator
 from typing_extensions import Literal
 
 from servicefoundry.auto_gen import models
 
 # TODO (chiragjn): Setup a base class for auto_gen.models to make `extra = "forbid"` default
@@ -38,14 +38,15 @@
 
 
 class DockerFileBuild(models.DockerFileBuild):
     class Config:
         extra = "forbid"
 
     type: constr(regex=r"dockerfile") = "dockerfile"
+    build_args: Optional[Dict[constr(min_length=1), constr(min_length=1)]] = Field(None)
 
 
 class PythonBuild(models.PythonBuild):
     class Config:
         extra = "forbid"
 
     type: constr(regex=r"tfy-python-buildpack") = "tfy-python-buildpack"
```

### Comparing `servicefoundry-0.9.5/servicefoundry/v2/lib/source.py` & `servicefoundry-0.9.6rc1/servicefoundry/v2/lib/source.py`

 * *Files identical despite different names*

### Comparing `servicefoundry-0.9.5/PKG-INFO` & `servicefoundry-0.9.6rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicefoundry
-Version: 0.9.5
+Version: 0.9.6rc1
 Summary: Generate deployed services from code
 Home-page: https://github.com/innoavator/servicefoundry
 Author: Abhishek Choudhary
 Author-email: abhichoudhary06@gmail.com
 Requires-Python: >=3.7,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

