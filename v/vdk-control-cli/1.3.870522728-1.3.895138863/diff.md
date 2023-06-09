# Comparing `tmp/vdk-control-cli-1.3.870522728.tar.gz` & `tmp/vdk-control-cli-1.3.895138863.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vdk-control-cli-1.3.870522728.tar", last modified: Thu May 18 10:11:44 2023, max compression
+gzip compressed data, was "dist/vdk-control-cli-1.3.895138863.tar", last modified: Fri Jun  9 13:38:08 2023, max compression
```

## Comparing `vdk-control-cli-1.3.870522728.tar` & `vdk-control-cli-1.3.895138863.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     5153 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4192 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1747 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      460 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)      717 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/markers.py
--rw-rw-rw-   0 root         (0) root         (0)     1423 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/specs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/common_group/
--rw-rw-rw-   0 root         (0) root         (0)     2284 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/common_group/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/info_group/
--rw-rw-rw-   0 root         (0) root         (0)     1868 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/info_group/info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/
--rw-rw-rw-   0 root         (0) root         (0)    11236 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/create.py
--rw-rw-rw-   0 root         (0) root         (0)     2121 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/delete.py
--rw-rw-rw-   0 root         (0) root         (0)     7121 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli.py
--rw-rw-rw-   0 root         (0) root         (0)    14329 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
--rw-rw-rw-   0 root         (0) root         (0)     5129 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_job.py
--rw-rw-rw-   0 root         (0) root         (0)     2678 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_key.py
--rw-rw-rw-   0 root         (0) root         (0)    12200 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/execute.py
--rw-rw-rw-   0 root         (0) root         (0)     8735 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/list.py
--rw-rw-rw-   0 root         (0) root         (0)    12040 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/properties.py
--rw-rw-rw-   0 root         (0) root         (0)     3403 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/show.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/login_group/
--rw-rw-rw-   0 root         (0) root         (0)     6510 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/login_group/login.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/logout_group/
--rw-rw-rw-   0 root         (0) root         (0)      410 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/logout_group/logout.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/version_group/
--rw-rw-rw-   0 root         (0) root         (0)      772 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/version_group/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/
--rw-rw-rw-   0 root         (0) root         (0)      424 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/default_options.py
--rw-rw-rw-   0 root         (0) root         (0)     1221 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/defaults_config.py
--rw-rw-rw-   0 root         (0) root         (0)     2272 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/log_config.py
--rw-rw-rw-   0 root         (0) root         (0)     9834 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/vdk_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/exception/
--rw-rw-rw-   0 root         (0) root         (0)      649 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/exception/vdk_exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_archive.py
--rw-rw-rw-   0 root         (0) root         (0)     4871 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/
--rw-rw-rw-   0 root         (0) root         (0)      579 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/10_sql_step.sql
--rw-rw-rw-   0 root         (0) root         (0)      816 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/20_python_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/README.md
--rw-rw-rw-   0 root         (0) root         (0)     2902 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/config.ini
--rw-rw-rw-   0 root         (0) root         (0)      243 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     3553 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/plugin/
--rw-rw-rw-   0 root         (0) root         (0)     3715 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/plugin/control_plugin_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/
--rw-rw-rw-   0 root         (0) root         (0)     3077 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/factory.py
--rw-rw-rw-   0 root         (0) root         (0)     3845 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/rest_client_errors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/
--rw-rw-rw-   0 root         (0) root         (0)     7297 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/cli_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1413 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/control_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/output_printer.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-05-18 10:11:28.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/version_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-05-18 10:11:33.000000 vdk-control-cli-1.3.870522728/src/vdk/internal/control/vdk_control_build_info.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5153 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2371 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-18 10:11:44.000000 vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       14 2023-05-18 10:11:33.000000 vdk-control-cli-1.3.870522728/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4192 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      460 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)      717 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/markers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1423 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/specs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/common_group/
+-rw-rw-rw-   0 root         (0) root         (0)     2284 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/common_group/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/info_group/
+-rw-rw-rw-   0 root         (0) root         (0)     1868 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/info_group/info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/
+-rw-rw-rw-   0 root         (0) root         (0)    11236 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/create.py
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/delete.py
+-rw-rw-rw-   0 root         (0) root         (0)     7121 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    14343 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5129 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_job.py
+-rw-rw-rw-   0 root         (0) root         (0)     2678 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_key.py
+-rw-rw-rw-   0 root         (0) root         (0)    12207 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/execute.py
+-rw-rw-rw-   0 root         (0) root         (0)     8735 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/list.py
+-rw-rw-rw-   0 root         (0) root         (0)    12040 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/properties.py
+-rw-rw-rw-   0 root         (0) root         (0)     3403 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/show.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/login_group/
+-rw-rw-rw-   0 root         (0) root         (0)     6510 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/login_group/login.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/logout_group/
+-rw-rw-rw-   0 root         (0) root         (0)      410 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/logout_group/logout.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/version_group/
+-rw-rw-rw-   0 root         (0) root         (0)      772 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/version_group/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      424 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/default_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1221 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/defaults_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2272 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/log_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     9834 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/vdk_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/exception/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/exception/vdk_exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_archive.py
+-rw-rw-rw-   0 root         (0) root         (0)     4871 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/
+-rw-rw-rw-   0 root         (0) root         (0)      579 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/10_sql_step.sql
+-rw-rw-rw-   0 root         (0) root         (0)      816 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/20_python_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     2902 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/config.ini
+-rw-rw-rw-   0 root         (0) root         (0)      243 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     3553 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/plugin/
+-rw-rw-rw-   0 root         (0) root         (0)     3715 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/plugin/control_plugin_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/
+-rw-rw-rw-   0 root         (0) root         (0)     3077 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3845 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/rest_client_errors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     7297 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/cli_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1413 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/control_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/output_printer.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-06-09 13:37:51.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/version_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-06-09 13:37:55.000000 vdk-control-cli-1.3.895138863/src/vdk/internal/control/vdk_control_build_info.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5153 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2371 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       57 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-09 13:38:08.000000 vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       14 2023-06-09 13:37:55.000000 vdk-control-cli-1.3.895138863/version.txt
```

### Comparing `vdk-control-cli-1.3.870522728/PKG-INFO` & `vdk-control-cli-1.3.895138863/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.870522728
+Version: 1.3.895138863
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.870522728/README.md` & `vdk-control-cli-1.3.895138863/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/setup.cfg` & `vdk-control-cli-1.3.895138863/setup.cfg`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/markers.py` & `vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/markers.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/api/control/plugin/specs.py` & `vdk-control-cli-1.3.895138863/src/vdk/api/control/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/common_group/default.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/common_group/default.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/info_group/info.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/info_group/info.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/create.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/create.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/delete.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/delete.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/deploy_cli_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     ) -> None:
         job: DataJob = self.__read_data_job(name, team)
         local_config = JobConfig(job_path)
         schedule = local_config.get_schedule_cron()
         if len(schedule) == 0:
             log.warning(
                 "You have provided no schedule for your Data Job. "
-                "Note that your deployed job will not be scheduled and will only run when manually executed."
+                "Note that your deployed job will not be scheduled and will only run when triggered manually or otherwise."
             )
         contacts = DataJobContacts(
             notified_on_job_failure_user_error=local_config.get_contacts_notified_on_job_failure_user_error(),
             notified_on_job_failure_platform_error=local_config.get_contacts_notified_on_job_failure_platform_error(),
             notified_on_job_success=local_config.get_contacts_notified_on_job_success(),
             notified_on_job_deploy=local_config.get_contacts_notified_on_job_deploy(),
         )
```

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_job.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_job.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/download_key.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/download_key.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/execute.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             raise vdk_ex
 
     @ApiClientErrorDecorator()
     def start(
         self, name: str, team: str, output_format: OutputFormat, arguments: str
     ) -> None:
         execution_request = DataJobExecutionRequest(
-            started_by=f"vdk-control-cli",
+            started_by=f"manual/vdk-control-cli",
             args=self.__validate_and_parse_args(arguments),
         )
         log.debug(f"Starting job with request {execution_request}")
         headers = self.__execution_api.data_job_execution_start_with_http_info(
             team_name=team,
             job_name=name,
             deployment_id="production",  # TODO
```

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/list.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/list.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/properties.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/properties.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/job/show.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/job/show.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/login_group/login.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/login_group/login.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/command_groups/version_group/version.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/command_groups/version_group/version.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/defaults_config.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/defaults_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/log_config.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/log_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/configuration/vdk_config.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/configuration/vdk_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/exception/vdk_exception.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/exception/vdk_exception.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_archive.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_archive.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/job_config.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/job_config.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/10_sql_step.sql` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/10_sql_step.sql`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/20_python_step.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/20_python_step.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/README.md` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/README.md`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/job/sample_job/config.ini` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/job/sample_job/config.ini`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/main.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/main.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/plugin/control_plugin_manager.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/plugin/control_plugin_manager.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/factory.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/factory.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/rest_lib/rest_client_errors.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/rest_lib/rest_client_errors.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/cli_utils.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/control_utils.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/control_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/output_printer.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/output_printer.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk/internal/control/utils/version_utils.py` & `vdk-control-cli-1.3.895138863/src/vdk/internal/control/utils/version_utils.py`

 * *Files identical despite different names*

### Comparing `vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/PKG-INFO` & `vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vdk-control-cli
-Version: 1.3.870522728
+Version: 1.3.895138863
 Summary: VDK Control CLI allows user to create, delete, manage and their Data Jobs in Kubernetes runtime.
 Home-page: https://github.com/vmware/versatile-data-kit
 Author: VMware Inc.
 Author-email: aivanov@vmware.com
 Project-URL: Documentation, https://github.com/vmware/versatile-data-kit/wiki
 Project-URL: Source, https://github.com/vmware/versatile-data-kit/projects/vdk-control-cli
 Platform: any
```

### Comparing `vdk-control-cli-1.3.870522728/src/vdk_control_cli.egg-info/SOURCES.txt` & `vdk-control-cli-1.3.895138863/src/vdk_control_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

