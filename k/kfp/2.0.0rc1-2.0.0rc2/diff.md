# Comparing `tmp/kfp-2.0.0-rc.1.tar.gz` & `tmp/kfp-2.0.0-rc.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.PWxKLpYf/kfp-2.0.0rc1.tar", last modified: Tue May 16 18:50:52 2023, max compression
+gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.CNLWtm3Q/kfp-2.0.0rc2.tar", last modified: Fri Jun  9 18:10:48 2023, max compression
```

## Comparing `kfp-2.0.0-rc.1.tar` & `kfp-2.0.0-rc.2.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/MANIFEST.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3977 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2155 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/README.md
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      887 2023-05-16 18:47:57.000000 kfp-2.0.0rc1/kfp/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/cli_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5391 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/compile_.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/compile_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16072 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-03-14 22:48:17.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/dsl.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/cli/utils/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/parsing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/parsing_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/client/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66676 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/client/client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17294 2023-05-12 20:36:23.000000 kfp-2.0.0rc1/kfp/client/client_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/set_volume_credentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/set_volume_credentials_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/token_credentials_base.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/token_credentials_base_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3443 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   152313 2023-05-12 17:28:57.000000 kfp-2.0.0rc1/kfp/compiler/compiler_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    32534 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/compiler_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1965 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/compiler_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85354 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8163 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/read_write_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1321 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6055 2023-05-09 18:23:54.000000 kfp-2.0.0rc1/kfp/components/base_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5432 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/base_component_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5995 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5489 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/component_decorator_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25321 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/component_factory.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6726 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/component_factory_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/constants.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1516 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1997 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component_artifact_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1888 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component_artifact_channel_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1905 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4574 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/container_component_decorator_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15493 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/executor.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3649 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/executor_main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    43760 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/executor_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11014 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6428 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/for_loop_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3399 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1015 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/importer_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5510 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/importer_node.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7662 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/importer_node_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/kfp_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13634 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/pipeline_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5981 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/pipeline_channel_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6436 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/pipeline_context.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27154 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/pipeline_task.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12295 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/pipeline_task_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16441 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/placeholders.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    22066 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/placeholders_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1523 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/python_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    44307 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/components/structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    38004 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/structures_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/task_final_status.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7711 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/tasks_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2851 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/tasks_group_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/components/types/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2415 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/artifact_types_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8059 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/custom_artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16140 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/custom_artifact_types_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7647 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/type_annotations.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7717 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/type_annotations_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19843 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/components/types/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    26536 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/type_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3905 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3679 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1740 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/v1_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/v1_modelbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27893 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/v1_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4214 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/yaml_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4324 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/yaml_component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_local_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_runners.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/auth/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/auth/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/auth/_satvolumecredentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/auth/_tokencredentialsbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/aws.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/azure.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/components_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_rewriter.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_using_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_default_transformers.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_k8s_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_op_to_template.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compat.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compatible_compiler_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_airflow_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_component_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_data_passing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_dynamic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_key_value_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_naming.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_python_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_python_to_graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_yaml_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/modelbase.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/components/structures/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/structures/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/containers/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_build_image_api.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_cache.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_component_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_container_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_gcs_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_k8s_job_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint_utils.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_component_bridge.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_metadata.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_ops_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_param.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_resource_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_snapshot_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/artifact.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/artifact_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/data_passing_methods.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/kubernetes.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/io_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/gcp.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/notebook/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/notebook/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/notebook/_magic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/onprem.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7618 2023-05-16 00:14:24.000000 kfp-2.0.0rc1/kfp/dsl/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/registry/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/registry/context/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/context/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/context/default_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/context/kfp_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/registry_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/registry_client_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/v2/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/dsl.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3977 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7648 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/SOURCES.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/dependency_links.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/entry_points.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      449 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/requires.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/top_level.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1276 2023-05-16 18:47:57.000000 kfp-2.0.0rc1/requirements.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/setup.cfg
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/setup.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/tests/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-03-14 22:48:17.000000 kfp-2.0.0rc1/tests/test_kfp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3977 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2155 2023-06-05 22:53:03.000000 kfp-2.0.0rc2/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      887 2023-06-09 18:00:38.000000 kfp-2.0.0rc2/kfp/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/cli_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5391 2023-05-25 20:05:16.000000 kfp-2.0.0rc2/kfp/cli/compile_.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-05-25 20:05:16.000000 kfp-2.0.0rc2/kfp/cli/compile_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16072 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/component_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-03-14 22:48:17.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/dsl.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/cli/utils/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/aliased_plurals_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/aliased_plurals_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/deprecated_alias_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/deprecated_alias_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/parsing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/cli/utils/parsing_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/client/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/client/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/client/auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66676 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/client/client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17294 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/client/client_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/client/set_volume_credentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/client/set_volume_credentials_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/client/token_credentials_base.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/client/token_credentials_base_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-05-19 17:00:33.000000 kfp-2.0.0rc2/kfp/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3443 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   154348 2023-06-09 16:48:50.000000 kfp-2.0.0rc2/kfp/compiler/compiler_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    33924 2023-06-09 16:48:50.000000 kfp-2.0.0rc2/kfp/compiler/compiler_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1965 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/compiler/compiler_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85354 2023-06-08 23:25:22.000000 kfp-2.0.0rc2/kfp/compiler/pipeline_spec_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/compiler/pipeline_spec_builder_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8163 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/compiler/read_write_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1321 2023-05-25 20:05:16.000000 kfp-2.0.0rc2/kfp/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6055 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/base_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5432 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/components/base_component_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5995 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/component_decorator.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5489 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/component_decorator_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25321 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/component_factory.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6726 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/component_factory_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/constants.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1516 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/container_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1997 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/container_component_artifact_channel.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1888 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/container_component_artifact_channel_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1905 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/container_component_decorator.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4574 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/container_component_decorator_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15824 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/executor.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3649 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/executor_main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    44835 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/executor_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11014 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6428 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/for_loop_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3399 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1015 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/importer_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5510 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/importer_node.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7662 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/importer_node_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/components/kfp_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13634 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/pipeline_channel.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5981 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/pipeline_channel_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6436 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/pipeline_context.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27240 2023-06-09 16:48:50.000000 kfp-2.0.0rc2/kfp/components/pipeline_task.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12295 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/pipeline_task_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16441 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/placeholders.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    22066 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/placeholders_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1523 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/python_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    44307 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    38004 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/structures_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/task_final_status.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7711 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/tasks_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2851 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/tasks_group_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/components/types/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/types/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/artifact_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2415 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/artifact_types_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8059 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/custom_artifact_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16140 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/custom_artifact_types_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7858 2023-06-09 16:48:50.000000 kfp-2.0.0rc2/kfp/components/types/type_annotations.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7717 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/type_annotations_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19843 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    26536 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/components/types/type_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3905 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3679 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1740 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/v1_components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/components/v1_modelbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27893 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/components/v1_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4214 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/components/yaml_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4324 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/components/yaml_component_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/_auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-06-01 17:20:34.000000 kfp-2.0.0rc2/kfp/deprecated/_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/_local_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/_runners.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/auth/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/auth/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/auth/_satvolumecredentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/auth/_tokencredentialsbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/aws.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/azure.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/components_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/_data_passing_using_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/_default_transformers.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/_k8s_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/_op_to_template.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/v2_compat.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/compiler/v2_compatible_compiler_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_airflow_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_component_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_data_passing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_dynamic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_key_value_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_naming.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_python_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_python_to_graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/_yaml_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/modelbase.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/components/structures/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/structures/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/type_annotation_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/components/type_annotation_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/containers/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/_build_image_api.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/_cache.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/_component_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/_container_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/_gcs_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/_k8s_job_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/entrypoint.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/containers/entrypoint_utils.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_component_bridge.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_container_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_container_op_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_metadata.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_ops_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_pipeline_param.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_pipeline_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_resource_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_volume_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/_volume_snapshot_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/artifact.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/artifact_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/component_spec.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/component_spec_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/data_passing_methods.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/dsl_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/dsl_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/extensions/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/extensions/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/extensions/kubernetes.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/io_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/metrics_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/metrics_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/serialization_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/serialization_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/dsl/types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/gcp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/deprecated/notebook/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/notebook/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/notebook/_magic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/deprecated/onprem.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7618 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/kfp/dsl/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/registry/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-05-25 20:05:16.000000 kfp-2.0.0rc2/kfp/registry/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/registry/context/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/registry/context/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/registry/context/default_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/registry/context/kfp_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/registry/registry_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/registry/registry_client_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp/v2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2023-05-31 17:19:49.000000 kfp-2.0.0rc2/kfp/v2/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/v2/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/v2/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-05-17 17:25:59.000000 kfp-2.0.0rc2/kfp/v2/dsl.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3977 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7648 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/entry_points.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      449 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/kfp.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1276 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/requirements.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-06-05 22:53:04.000000 kfp-2.0.0rc2/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-06-09 18:10:48.000000 kfp-2.0.0rc2/tests/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-03-14 22:48:17.000000 kfp-2.0.0rc2/tests/test_kfp.py
```

### Comparing `kfp-2.0.0rc1/PKG-INFO` & `kfp-2.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
```

### Comparing `kfp-2.0.0rc1/README.md` & `kfp-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/__init__.py` & `kfp-2.0.0rc2/kfp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,13 +12,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # `kfp` is a namespace package.
 # https://packaging.python.org/guides/packaging-namespace-packages/#pkgutil-style-namespace-packages
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
-__version__ = '2.0.0-rc.1'
+__version__ = '2.0.0-rc.2'
 
 TYPE_CHECK = True
 
 from kfp import dsl
 from kfp.client import Client
```

### Comparing `kfp-2.0.0rc1/kfp/cli/__init__.py` & `kfp-2.0.0rc2/kfp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/__main__.py` & `kfp-2.0.0rc2/kfp/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/cli.py` & `kfp-2.0.0rc2/kfp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/cli_test.py` & `kfp-2.0.0rc2/kfp/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/compile_.py` & `kfp-2.0.0rc2/kfp/cli/compile_.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/compile_test.py` & `kfp-2.0.0rc2/kfp/cli/compile_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/component.py` & `kfp-2.0.0rc2/kfp/cli/component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/component_test.py` & `kfp-2.0.0rc2/kfp/cli/component_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/__init__.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env_test.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp_test.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/utility.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/utility.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me/utility_test.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me/utility_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/diagnose_me_cli.py` & `kfp-2.0.0rc2/kfp/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/dsl.py` & `kfp-2.0.0rc2/kfp/cli/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/experiment.py` & `kfp-2.0.0rc2/kfp/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/output.py` & `kfp-2.0.0rc2/kfp/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/pipeline.py` & `kfp-2.0.0rc2/kfp/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/recurring_run.py` & `kfp-2.0.0rc2/kfp/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/run.py` & `kfp-2.0.0rc2/kfp/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/__init__.py` & `kfp-2.0.0rc2/kfp/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group.py` & `kfp-2.0.0rc2/kfp/cli/utils/aliased_plurals_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group_test.py` & `kfp-2.0.0rc2/kfp/cli/utils/aliased_plurals_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group.py` & `kfp-2.0.0rc2/kfp/cli/utils/deprecated_alias_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group_test.py` & `kfp-2.0.0rc2/kfp/cli/utils/deprecated_alias_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/parsing.py` & `kfp-2.0.0rc2/kfp/cli/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/cli/utils/parsing_test.py` & `kfp-2.0.0rc2/kfp/cli/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/__init__.py` & `kfp-2.0.0rc2/kfp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/auth.py` & `kfp-2.0.0rc2/kfp/client/auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/client.py` & `kfp-2.0.0rc2/kfp/client/client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/client_test.py` & `kfp-2.0.0rc2/kfp/client/client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/set_volume_credentials.py` & `kfp-2.0.0rc2/kfp/client/set_volume_credentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/set_volume_credentials_test.py` & `kfp-2.0.0rc2/kfp/client/set_volume_credentials_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/token_credentials_base.py` & `kfp-2.0.0rc2/kfp/client/token_credentials_base.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/client/token_credentials_base_test.py` & `kfp-2.0.0rc2/kfp/client/token_credentials_base_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/compiler/__init__.py` & `kfp-2.0.0rc2/kfp/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/compiler/compiler.py` & `kfp-2.0.0rc2/kfp/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/compiler/compiler_test.py` & `kfp-2.0.0rc2/kfp/compiler/compiler_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -1818,14 +1818,72 @@
                         two = print_op(message='3').after(one)
 
             with tempfile.TemporaryDirectory() as tempdir:
                 package_path = os.path.join(tempdir, 'pipeline.yaml')
                 compiler.Compiler().compile(
                     pipeline_func=my_pipeline, package_path=package_path)
 
+    def test_inner_parallelfor_can_iter_over_upstream_output(self):
+
+        @dsl.component
+        def str_to_list(string: str) -> List:
+            return [string]
+
+        @dsl.component
+        def identity(string: str) -> str:
+            return string
+
+        @dsl.pipeline
+        def my_pipeline():
+            with dsl.ParallelFor(['a', 'b', 'c']) as itema:
+                t1 = str_to_list(string=itema)
+                with dsl.ParallelFor(t1.output) as itemb:
+                    identity(string=itemb)
+
+        with tempfile.TemporaryDirectory() as tempdir:
+            package_path = os.path.join(tempdir, 'pipeline.yaml')
+            compiler.Compiler().compile(
+                pipeline_func=my_pipeline, package_path=package_path)
+
+    def test_permitted_nested_parallelfor_complex(self):
+
+        @dsl.component
+        def str_to_list(string: str) -> List:
+            return [string]
+
+        @dsl.component
+        def identity(string: str) -> str:
+            return string
+
+        @dsl.pipeline
+        def my_pipeline():
+
+            # for-loop-2
+            with dsl.ParallelFor(['a', 'b', 'c']) as itema:
+                t1 = str_to_list(string=itema)
+                t2 = str_to_list(string=itema)
+
+                sequential_task1 = identity(string=itema)
+                identity(string=sequential_task1.output)
+
+                # for-loop-3
+                with dsl.ParallelFor(t1.output) as itemb:
+                    t3 = str_to_list(string=itema)
+                    with dsl.ParallelFor(t3.output) as itemc:
+                        identity(string=itemc)
+                    with dsl.ParallelFor(t2.output) as itemd:
+                        identity(string=itemd)
+                with dsl.ParallelFor(t2.output) as iteme:
+                    identity(string=iteme)
+
+        with tempfile.TemporaryDirectory() as tempdir:
+            package_path = os.path.join(tempdir, 'pipeline.yaml')
+            compiler.Compiler().compile(
+                pipeline_func=my_pipeline, package_path=package_path)
+
     def test_downstream_in_condition_nested_in_a_for_loop(self):
 
         @dsl.pipeline()
         def my_pipeline():
             return_1_task = return_1()
 
             with dsl.ParallelFor([1, 2, 3]):
```

### Comparing `kfp-2.0.0rc1/kfp/compiler/compiler_utils.py` & `kfp-2.0.0rc2/kfp/compiler/compiler_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -650,45 +650,70 @@
             )
 
             # uncommon upstream ancestor check
             uncommon_upstream_groups = deepcopy(upstream_groups)
             uncommon_upstream_groups.remove(
                 upstream_task.name
             )  # because a task's `upstream_groups` contains the task's name
+
+            # TODO: this logic can be simplified: the logic to check for consumption from a task in an upstream
+            # Condition and ExitHandler should be the same and can be unified with the ParallelFor checks
             if uncommon_upstream_groups:
                 dependent_group = group_name_to_group.get(
                     uncommon_upstream_groups[0], None)
 
                 if isinstance(dependent_group,
                               (tasks_group.Condition, tasks_group.ExitHandler)):
                     raise InvalidTopologyException(
                         f'{ILLEGAL_CROSS_DAG_ERROR_PREFIX} A downstream task cannot depend on an upstream task within a dsl.{dependent_group.__class__.__name__} context unless the downstream is within that context too. Found task {task.name} which depends on upstream task {upstream_task.name} within an uncommon dsl.{dependent_group.__class__.__name__} context.'
                     )
                 elif isinstance(dependent_group, tasks_group.ParallelFor):
                     raise InvalidTopologyException(
                         f'{ILLEGAL_CROSS_DAG_ERROR_PREFIX} A downstream task cannot depend on an upstream task within a dsl.{dependent_group.__class__.__name__} context unless the downstream is within that context too or the outputs are begin fanned-in to a list using dsl.{for_loop.Collected.__name__}. Found task {task.name} which depends on upstream task {upstream_task.name} within an uncommon dsl.{dependent_group.__class__.__name__} context.'
                     )
 
-            # ParralelFor Nested Check
-            # if there is a parrallelFor group type in the upstream parents tasks and there also exists a parallelFor in the uncommon_ancestors of downstream: this means a nested for loop exists in the DAG
-            # only check when upstream_task is a PipelineTask, since checking
-            # for TasksGroup results in catching dsl.Collected cases.
+            # tasks in a deeper part of a nested ParallelFor cannot depend directly on a task in a shallower part of the nested ParallelFor
+            # to check for this we need to know that:
+            # - the upstream task has at least one ParallelFor parent group
+            # - the downstream task has at least one ParallelFor parent group uncommon to the upstream task
+            # - the downstream consumes from the upstream or has an explicit dependency (.after) on it (a dependency transitively via the parent task group doesn't satisfy the error condition, since the ParallelFor should be permitted to iterate over the upstreams list output)
             if isinstance(upstream_task, pipeline_task.PipelineTask):
                 upstream_parent_tasks = task_name_to_parent_groups[
                     upstream_task.name]
 
-                for group in downstream_groups:
+                downstream_parallelfor_parents = [
+                    group_name_to_group.get(group, None)
+                    for group in downstream_groups
+                    if isinstance(
+                        group_name_to_group.get(group, None),
+                        tasks_group.ParallelFor)
+                ]
+                downstream_in_parallelfor = bool(downstream_parallelfor_parents)
+
+                upstream_parallelfor_parents = [
+                    parent_group for parent_group in upstream_parent_tasks
                     if isinstance(
-                            group_name_to_group.get(group, None),
-                            tasks_group.ParallelFor):
-                        for parent_task in upstream_parent_tasks:
-                            if isinstance(
-                                    group_name_to_group.get(parent_task, None),
-                                    tasks_group.ParallelFor):
-
-                                raise InvalidTopologyException(
-                                    f'{ILLEGAL_CROSS_DAG_ERROR_PREFIX} Downstream tasks in a nested {tasks_group.ParallelFor.__name__} group cannot depend on an upstream task in a shallower {tasks_group.ParallelFor.__name__} group. Task {task.name} depends on upstream task {upstream_task.name}, while {group} is nested in {parent_task}.'
-                                )
+                        group_name_to_group.get(parent_group, None),
+                        tasks_group.ParallelFor)
+                ]
+                upstream_in_parallelfor = bool(upstream_parallelfor_parents)
+
+                downstream_consumes_from_upstream = bool([
+                    inp.name
+                    for inp in task._task_spec.inputs.values()
+                    if isinstance(inp, pipeline_channel.PipelineChannel) and
+                    inp.name == upstream_task.name
+                ])
+
+                after_called_on_upstream = upstream_task.name in task._run_after
+
+                if downstream_in_parallelfor and upstream_in_parallelfor and (
+                        downstream_consumes_from_upstream or
+                        after_called_on_upstream):
+
+                    raise InvalidTopologyException(
+                        f'{ILLEGAL_CROSS_DAG_ERROR_PREFIX} Downstream tasks in a nested {tasks_group.ParallelFor.__name__} group cannot depend on an upstream task in a shallower {tasks_group.ParallelFor.__name__} group. Task {task.name} depends on upstream task {upstream_task.name}, while {downstream_parallelfor_parents[0]} is nested in {upstream_parallelfor_parents[0]}.'
+                    )
 
             dependencies[downstream_groups[0]].add(upstream_groups[0])
 
     return dependencies
```

### Comparing `kfp-2.0.0rc1/kfp/compiler/compiler_utils_test.py` & `kfp-2.0.0rc2/kfp/compiler/compiler_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder.py` & `kfp-2.0.0rc2/kfp/compiler/pipeline_spec_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder_test.py` & `kfp-2.0.0rc2/kfp/compiler/pipeline_spec_builder_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/compiler/read_write_test.py` & `kfp-2.0.0rc2/kfp/compiler/read_write_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/__init__.py` & `kfp-2.0.0rc2/kfp/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/base_component.py` & `kfp-2.0.0rc2/kfp/components/base_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/base_component_test.py` & `kfp-2.0.0rc2/kfp/components/base_component_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/component_decorator.py` & `kfp-2.0.0rc2/kfp/components/component_decorator.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/component_decorator_test.py` & `kfp-2.0.0rc2/kfp/components/component_decorator_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/component_factory.py` & `kfp-2.0.0rc2/kfp/components/component_factory.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/component_factory_test.py` & `kfp-2.0.0rc2/kfp/components/component_factory_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/constants.py` & `kfp-2.0.0rc2/kfp/components/constants.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/container_component.py` & `kfp-2.0.0rc2/kfp/components/container_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/container_component_artifact_channel.py` & `kfp-2.0.0rc2/kfp/components/container_component_artifact_channel.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/container_component_artifact_channel_test.py` & `kfp-2.0.0rc2/kfp/components/container_component_artifact_channel_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/container_component_decorator.py` & `kfp-2.0.0rc2/kfp/components/container_component_decorator.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/container_component_decorator_test.py` & `kfp-2.0.0rc2/kfp/components/container_component_decorator_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/executor.py` & `kfp-2.0.0rc2/kfp/components/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,24 +219,30 @@
         return False
 
     def _handle_single_return_value(self, output_name: str,
                                     annotation_type: Any, return_value: Any):
         if self._is_parameter(annotation_type):
             origin_type = getattr(annotation_type, '__origin__',
                                   None) or annotation_type
-            if not isinstance(return_value, origin_type):
+            # relax float-typed return to allow both int and float.
+            if origin_type == float:
+                accepted_types = (int, float)
+            # TODO: relax str-typed return to allow all primitive types?
+            else:
+                accepted_types = origin_type
+            if not isinstance(return_value, accepted_types):
                 raise ValueError(
                     f'Function `{self._func.__name__}` returned value of type {type(return_value)}; want type {origin_type}'
                 )
             self._write_output_parameter_value(output_name, return_value)
         elif self._is_artifact(annotation_type):
             self._write_output_artifact_payload(output_name, return_value)
         else:
             raise RuntimeError(
-                f'Unknown return type: {annotation_type}. Must be one of `str`, `int`, `float`, or a subclass of `Artifact`'
+                f'Unknown return type: {annotation_type}. Must be one of the supported data types: https://www.kubeflow.org/docs/components/pipelines/v2/data-types/'
             )
 
     def _write_executor_output(self, func_output: Optional[Any] = None):
         if self._output_artifacts:
             self._executor_output['artifacts'] = {}
 
         for name, artifact in self._output_artifacts.items():
```

### Comparing `kfp-2.0.0rc1/kfp/components/executor_main.py` & `kfp-2.0.0rc2/kfp/components/executor_main.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/executor_test.py` & `kfp-2.0.0rc2/kfp/components/executor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from kfp.components.types.artifact_types import Model
 from kfp.components.types.type_annotations import InputPath
 from kfp.components.types.type_annotations import OutputPath
 from kfp.dsl import Input
 from kfp.dsl import Output
 
 
-class ExecutorTest(unittest.TestCase):
+class ExecutorTest(parameterized.TestCase):
 
     @classmethod
     def setUp(cls):
         cls.maxDiff = None
         cls._test_dir = tempfile.mkdtemp()
         artifact_types._GCS_LOCAL_MOUNT_PREFIX = cls._test_dir + '/'
         artifact_types._MINIO_LOCAL_MOUNT_PREFIX = cls._test_dir + '/minio/'
@@ -383,45 +383,78 @@
             test_func, executor_input)
         self.assertDictEqual(output_metadata, {
             'parameterValues': {
                 'Output': 42
             },
         })
 
-    def test_function_with_float_output(self):
-        executor_input = """\
-    {
-      "inputs": {
-        "parameterValues": {
-          "first": 0.0,
-          "second": 1.2
-        }
-      },
-      "outputs": {
-        "parameters": {
-          "Output": {
-            "outputFile": "gs://some-bucket/output"
-          }
+    @parameterized.parameters(
+        {
+            'executor_input':
+                """\
+            {
+              "inputs": {
+                "parameterValues": {
+                  "first": 0.0,
+                  "second": 1.2
+                }
+              },
+              "outputs": {
+                "parameters": {
+                  "Output": {
+                    "outputFile": "gs://some-bucket/output"
+                  }
+                },
+                "outputFile": "%(test_dir)s/output_metadata.json"
+              }
+            }
+            """,
+            'expected_output_metadata': {
+                'parameterValues': {
+                    'Output': 1.2
+                },
+            },
         },
-        "outputFile": "%(test_dir)s/output_metadata.json"
-      }
-    }
-    """
+        {
+            'executor_input':
+                """\
+            {
+              "inputs": {
+                "parameterValues": {
+                  "first": 1,
+                  "second": 2
+                }
+              },
+              "outputs": {
+                "parameters": {
+                  "Output": {
+                    "outputFile": "gs://some-bucket/output"
+                  }
+                },
+                "outputFile": "%(test_dir)s/output_metadata.json"
+              }
+            }
+            """,
+            'expected_output_metadata': {
+                'parameterValues': {
+                    'Output': 3
+                },
+            },
+        },
+    )
+    def test_function_with_float_output(self, executor_input,
+                                        expected_output_metadata):
 
         def test_func(first: float, second: float) -> float:
             return first + second
 
         output_metadata = self.execute_and_load_output_metadata(
             test_func, executor_input)
 
-        self.assertDictEqual(output_metadata, {
-            'parameterValues': {
-                'Output': 1.2
-            },
-        })
+        self.assertDictEqual(output_metadata, expected_output_metadata)
 
     def test_function_with_list_output(self):
         executor_input = """\
     {
       "inputs": {
         "parameterValues": {
           "first": 40,
```

### Comparing `kfp-2.0.0rc1/kfp/components/for_loop.py` & `kfp-2.0.0rc2/kfp/components/for_loop.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/for_loop_test.py` & `kfp-2.0.0rc2/kfp/components/for_loop_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/graph_component.py` & `kfp-2.0.0rc2/kfp/components/graph_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/importer_component.py` & `kfp-2.0.0rc2/kfp/components/importer_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/importer_node.py` & `kfp-2.0.0rc2/kfp/components/importer_node.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/importer_node_test.py` & `kfp-2.0.0rc2/kfp/components/importer_node_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/kfp_config.py` & `kfp-2.0.0rc2/kfp/components/kfp_config.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/pipeline_channel.py` & `kfp-2.0.0rc2/kfp/components/pipeline_channel.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/pipeline_channel_test.py` & `kfp-2.0.0rc2/kfp/components/pipeline_channel_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/pipeline_context.py` & `kfp-2.0.0rc2/kfp/components/pipeline_context.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/pipeline_task.py` & `kfp-2.0.0rc2/kfp/components/pipeline_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,14 +95,15 @@
 
         self._task_spec = structures.TaskSpec(
             name=self._register_task_handler(),
             inputs=dict(args.items()),
             dependent_tasks=[],
             component_ref=component_spec.name,
             enable_caching=True)
+        self._run_after: List[str] = []
 
         self.importer_spec = None
         self.container_spec = None
         self.pipeline_spec = None
         self._ignore_upstream_failure_tag = False
         # platform_config for this primitive task; empty if task is for a graph component
         self.platform_config = {}
@@ -571,14 +572,15 @@
 
             @dsl.pipeline(name='my-pipeline')
             def my_pipeline():
                 task1 = my_component(text='1st task')
                 task2 = my_component(text='2nd task').after(task1)
         """
         for task in tasks:
+            self._run_after.append(task.name)
             self._task_spec.dependent_tasks.append(task.name)
         return self
 
     def ignore_upstream_failure(self) -> 'PipelineTask':
         """If called, the pipeline task will run when any specified upstream
         tasks complete, even if unsuccessful.
```

### Comparing `kfp-2.0.0rc1/kfp/components/pipeline_task_test.py` & `kfp-2.0.0rc2/kfp/components/pipeline_task_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/placeholders.py` & `kfp-2.0.0rc2/kfp/components/placeholders.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/placeholders_test.py` & `kfp-2.0.0rc2/kfp/components/placeholders_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/python_component.py` & `kfp-2.0.0rc2/kfp/components/python_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/structures.py` & `kfp-2.0.0rc2/kfp/components/structures.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/structures_test.py` & `kfp-2.0.0rc2/kfp/components/structures_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/task_final_status.py` & `kfp-2.0.0rc2/kfp/components/task_final_status.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/tasks_group.py` & `kfp-2.0.0rc2/kfp/components/tasks_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/tasks_group_test.py` & `kfp-2.0.0rc2/kfp/components/tasks_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/__init__.py` & `kfp-2.0.0rc2/kfp/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/artifact_types.py` & `kfp-2.0.0rc2/kfp/components/types/artifact_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/artifact_types_test.py` & `kfp-2.0.0rc2/kfp/components/types/artifact_types_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/custom_artifact_types.py` & `kfp-2.0.0rc2/kfp/components/types/custom_artifact_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/custom_artifact_types_test.py` & `kfp-2.0.0rc2/kfp/components/types/custom_artifact_types_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/type_annotations.py` & `kfp-2.0.0rc2/kfp/components/types/type_annotations.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,10 +233,13 @@
 
 
 def is_list_of_artifacts(
     type_var: Union[Type[List[artifact_types.Artifact]],
                     Type[artifact_types.Artifact]]
 ) -> bool:
     # the type annotation for this function's `type_var` parameter may not actually be a subclass of the KFP SDK's Artifact class for custom artifact types
-    return getattr(type_var, '__origin__',
-                   None) == list and type_annotations.is_artifact_class(
-                       type_var.__args__[0])
+    is_list_or_list_generic = getattr(type_var, '__origin__', None) == list
+    # in >= python3.9, List wont have .__args__ if it's used as `-> List` with no inner type argument
+    contains_artifact = hasattr(
+        type_var, '__args__') and type_annotations.is_artifact_class(
+            type_var.__args__[0])
+    return is_list_or_list_generic and contains_artifact
```

### Comparing `kfp-2.0.0rc1/kfp/components/types/type_annotations_test.py` & `kfp-2.0.0rc2/kfp/components/types/type_annotations_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/type_utils.py` & `kfp-2.0.0rc2/kfp/components/types/type_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/types/type_utils_test.py` & `kfp-2.0.0rc2/kfp/components/types/type_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/utils.py` & `kfp-2.0.0rc2/kfp/components/utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/utils_test.py` & `kfp-2.0.0rc2/kfp/components/utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/v1_components.py` & `kfp-2.0.0rc2/kfp/components/v1_components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/v1_modelbase.py` & `kfp-2.0.0rc2/kfp/components/v1_modelbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/v1_structures.py` & `kfp-2.0.0rc2/kfp/components/v1_structures.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/yaml_component.py` & `kfp-2.0.0rc2/kfp/components/yaml_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/components/yaml_component_test.py` & `kfp-2.0.0rc2/kfp/components/yaml_component_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/__main__.py` & `kfp-2.0.0rc2/kfp/deprecated/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/_auth.py` & `kfp-2.0.0rc2/kfp/deprecated/_auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/_client.py` & `kfp-2.0.0rc2/kfp/deprecated/_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/_config.py` & `kfp-2.0.0rc2/kfp/deprecated/_config.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/_local_client.py` & `kfp-2.0.0rc2/kfp/deprecated/_local_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/_runners.py` & `kfp-2.0.0rc2/kfp/deprecated/_runners.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/auth/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/auth/_satvolumecredentials.py` & `kfp-2.0.0rc2/kfp/deprecated/auth/_satvolumecredentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/auth/_tokencredentialsbase.py` & `kfp-2.0.0rc2/kfp/deprecated/auth/_tokencredentialsbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/aws.py` & `kfp-2.0.0rc2/kfp/deprecated/aws.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/azure.py` & `kfp-2.0.0rc2/kfp/deprecated/azure.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/cli.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/components.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/components_test.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/components_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env_test.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp_test.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/utility.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility_test.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me/utility_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me_cli.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/experiment.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/output.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/pipeline.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/recurring_run.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/cli/run.py` & `kfp-2.0.0rc2/kfp/deprecated/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_rewriter.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_using_volume.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/_data_passing_using_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/_default_transformers.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/_default_transformers.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/_k8s_helper.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/_op_to_template.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/compiler.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/main.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/main.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compat.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/v2_compat.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compatible_compiler_test.py` & `kfp-2.0.0rc2/kfp/deprecated/compiler/v2_compatible_compiler_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_airflow_op.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_airflow_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_component_store.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_component_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_components.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_data_passing.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_data_passing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_dynamic.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_dynamic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_key_value_store.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_key_value_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_naming.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_naming.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_python_op.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_python_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_python_to_graph_component.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_python_to_graph_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_structures.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_structures.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/_yaml_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/components/_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/modelbase.py` & `kfp-2.0.0rc2/kfp/deprecated/components/modelbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/components/type_annotation_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils_test.py` & `kfp-2.0.0rc2/kfp/deprecated/components/type_annotation_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/_build_image_api.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/_build_image_api.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/_cache.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/_cache.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/_component_builder.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/_component_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/_container_builder.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/_container_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/_gcs_helper.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/_gcs_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/_k8s_job_helper.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/_k8s_job_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/entrypoint.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/containers/entrypoint_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_component.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_component_bridge.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_component_bridge.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_container_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op_test.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_container_op_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_for_loop.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_for_loop.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_metadata.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_metadata.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_ops_group.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_ops_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_param.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_pipeline_param.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_volume.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_pipeline_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_resource_op.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_resource_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_op.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_volume_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_snapshot_op.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/_volume_snapshot_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/artifact.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/artifact.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/artifact_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/component_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec_test.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/component_spec_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/data_passing_methods.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/data_passing_methods.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/dsl_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils_test.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/dsl_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/kubernetes.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/extensions/kubernetes.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/io_types.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/io_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils_test.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/metrics_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils_test.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/serialization_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/type_utils.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/type_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/dsl/types.py` & `kfp-2.0.0rc2/kfp/deprecated/dsl/types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/gcp.py` & `kfp-2.0.0rc2/kfp/deprecated/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/notebook/__init__.py` & `kfp-2.0.0rc2/kfp/deprecated/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/notebook/_magic.py` & `kfp-2.0.0rc2/kfp/deprecated/notebook/_magic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/deprecated/onprem.py` & `kfp-2.0.0rc2/kfp/deprecated/onprem.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/dsl/__init__.py` & `kfp-2.0.0rc2/kfp/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/registry/__init__.py` & `kfp-2.0.0rc2/kfp/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/registry/context/__init__.py` & `kfp-2.0.0rc2/kfp/registry/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/registry/context/default_pkg_dev.json` & `kfp-2.0.0rc2/kfp/registry/context/default_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/registry/context/kfp_pkg_dev.json` & `kfp-2.0.0rc2/kfp/registry/context/kfp_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/registry/registry_client.py` & `kfp-2.0.0rc2/kfp/registry/registry_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/registry/registry_client_test.py` & `kfp-2.0.0rc2/kfp/registry/registry_client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/v2/__init__.py` & `kfp-2.0.0rc2/kfp/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/v2/compiler.py` & `kfp-2.0.0rc2/kfp/v2/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/v2/components.py` & `kfp-2.0.0rc2/kfp/v2/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp/v2/dsl.py` & `kfp-2.0.0rc2/kfp/v2/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/kfp.egg-info/PKG-INFO` & `kfp-2.0.0rc2/kfp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
```

### Comparing `kfp-2.0.0rc1/kfp.egg-info/SOURCES.txt` & `kfp-2.0.0rc2/kfp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0rc1/requirements.in` & `kfp-2.0.0rc2/requirements.in`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # pin kfp-pipeline-spec to an exact version, since this is the contract between a given KFP SDK version and the BE. we don't want old version of the SDK to write new fields and to have the BE reject the new unsupported field (even if the new field backward compatible from a proto perspective)
 kfp-pipeline-spec==0.2.2
 # Update the upper version whenever a new major version of the
 # kfp-server-api package is released.
 # Update the lower version when kfp sdk depends on new apis/fields in
 # kfp-server-api.
 kfp-server-api==2.0.0-rc.1
-kubernetes>=8.0.0,<24
+kubernetes>=8.0.0,<27
 protobuf>=3.13.0,<4
 PyYAML>=5.3,<7
 requests-toolbelt>=0.8.0,<1
 tabulate>=0.8.6,<1
 urllib3<2.0.0
 
 ## standard library backports ##
```

### Comparing `kfp-2.0.0rc1/setup.py` & `kfp-2.0.0rc2/setup.py`

 * *Files identical despite different names*

