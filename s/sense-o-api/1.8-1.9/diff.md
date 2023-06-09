# Comparing `tmp/sense_o_api-1.8.tar.gz` & `tmp/sense_o_api-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sense_o_api-1.8.tar", last modified: Wed Aug 11 14:38:28 2021, max compression
+gzip compressed data, was "sense_o_api-1.9.tar", last modified: Tue Aug 24 14:16:20 2021, max compression
```

## Comparing `sense_o_api-1.8.tar` & `sense_o_api-1.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.508201 sense_o_api-1.8/
--rw-r--r--   0 xiyang     (502) staff       (20)     1095 2021-08-04 15:03:48.000000 sense_o_api-1.8/LICENSE.txt
--rw-r--r--   0 xiyang     (502) staff       (20)      480 2021-08-11 14:38:28.507918 sense_o_api-1.8/PKG-INFO
--rw-r--r--   0 xiyang     (502) staff       (20)      471 2021-08-09 03:53:59.000000 sense_o_api-1.8/README.md
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.486281 sense_o_api-1.8/sense/
--rw-r--r--   0 xiyang     (502) staff       (20)       21 2021-08-11 14:38:14.000000 sense_o_api-1.8/sense/__init__.py
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.489266 sense_o_api-1.8/sense/client/
--rw-r--r--   0 xiyang     (502) staff       (20)        0 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/client/__init__.py
--rw-r--r--   0 xiyang     (502) staff       (20)     2464 2021-08-09 03:53:59.000000 sense_o_api-1.8/sense/client/apiclient.py
--rw-r--r--   0 xiyang     (502) staff       (20)    17216 2021-06-29 13:21:06.000000 sense_o_api-1.8/sense/client/discover_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)    36817 2021-08-09 03:53:59.000000 sense_o_api-1.8/sense/client/instance_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)     6328 2021-08-09 03:53:59.000000 sense_o_api-1.8/sense/client/intent_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)    14688 2021-08-09 03:53:59.000000 sense_o_api-1.8/sense/client/logging_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)    24197 2021-06-29 19:30:33.000000 sense_o_api-1.8/sense/client/profile_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3529 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/client/requestwrapper.py
--rw-r--r--   0 xiyang     (502) staff       (20)    24069 2021-08-09 15:30:52.000000 sense_o_api-1.8/sense/client/workflow_combined_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)    26701 2021-08-09 03:53:59.000000 sense_o_api-1.8/sense/client/workflow_phased_api.py
--rw-r--r--   0 xiyang     (502) staff       (20)      486 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/common.py
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.502412 sense_o_api-1.8/sense/models/
--rw-r--r--   0 xiyang     (502) staff       (20)     2439 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/__init__.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4267 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/bandwidth.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3686 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/capability_description.py
--rw-r--r--   0 xiyang     (502) staff       (20)     7320 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/connection.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4387 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/connection_bandwidth.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4490 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/connection_path_tprofile.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4623 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/connection_schedule.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4547 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/connection_suggest_ip_range.py
--rw-r--r--   0 xiyang     (502) staff       (20)     7378 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/connection_terminals.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3642 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/delta.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4732 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/discover_description.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3870 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/discover_description_end_points.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4130 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/dnc_schema.py
--rw-r--r--   0 xiyang     (502) staff       (20)     5163 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/dnc_schema_data.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4425 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/domain_description.py
--rw-r--r--   0 xiyang     (502) staff       (20)     5399 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/domain_description_edge_points.py
--rw-r--r--   0 xiyang     (502) staff       (20)    11207 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/full_profile.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4817 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/inline_response200.py
--rw-r--r--   0 xiyang     (502) staff       (20)     7794 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/intent.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3304 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/intent_expanded.py
--rw-r--r--   0 xiyang     (502) staff       (20)     9425 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/log.py
--rw-r--r--   0 xiyang     (502) staff       (20)     2527 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/log_level.py
--rw-r--r--   0 xiyang     (502) staff       (20)     7708 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/logging_configuration.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4220 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/logging_configuration_loggers.py
--rw-r--r--   0 xiyang     (502) staff       (20)     2446 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/one_of_service_intent_data.py
--rw-r--r--   0 xiyang     (502) staff       (20)     2765 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/operation.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3043 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/path.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4902 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/profile_edit.py
--rw-r--r--   0 xiyang     (502) staff       (20)     5611 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/profile_license.py
--rw-r--r--   0 xiyang     (502) staff       (20)     6184 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/profile_manifest.py
--rw-r--r--   0 xiyang     (502) staff       (20)     5724 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/service_description.py
--rw-r--r--   0 xiyang     (502) staff       (20)     6987 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/service_intent.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3761 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/service_intent_queries.py
--rw-r--r--   0 xiyang     (502) staff       (20)     5522 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/service_intent_response.py
--rw-r--r--   0 xiyang     (502) staff       (20)     9565 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/slim_profile.py
--rw-r--r--   0 xiyang     (502) staff       (20)     5035 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/terminal.py
--rw-r--r--   0 xiyang     (502) staff       (20)    10851 2021-06-17 12:42:40.000000 sense_o_api-1.8/sense/models/verification_result.py
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.504398 sense_o_api-1.8/sense_o_api.egg-info/
--rw-r--r--   0 xiyang     (502) staff       (20)      480 2021-08-11 14:38:28.000000 sense_o_api-1.8/sense_o_api.egg-info/PKG-INFO
--rw-r--r--   0 xiyang     (502) staff       (20)     1928 2021-08-11 14:38:28.000000 sense_o_api-1.8/sense_o_api.egg-info/SOURCES.txt
--rw-r--r--   0 xiyang     (502) staff       (20)        1 2021-08-11 14:38:28.000000 sense_o_api-1.8/sense_o_api.egg-info/dependency_links.txt
--rw-r--r--   0 xiyang     (502) staff       (20)       27 2021-08-11 14:38:28.000000 sense_o_api-1.8/sense_o_api.egg-info/requires.txt
--rw-r--r--   0 xiyang     (502) staff       (20)       11 2021-08-11 14:38:28.000000 sense_o_api-1.8/sense_o_api.egg-info/top_level.txt
--rw-r--r--   0 xiyang     (502) staff       (20)       38 2021-08-11 14:38:28.508320 sense_o_api-1.8/setup.cfg
--rw-r--r--   0 xiyang     (502) staff       (20)      803 2021-08-09 03:53:59.000000 sense_o_api-1.8/setup.py
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.507070 sense_o_api-1.8/test/
--rw-r--r--   0 xiyang     (502) staff       (20)        0 2021-06-17 12:42:40.000000 sense_o_api-1.8/test/__init__.py
--rw-r--r--   0 xiyang     (502) staff       (20)     2033 2021-06-29 19:24:18.000000 sense_o_api-1.8/test/test_discover.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3816 2021-06-21 15:13:17.000000 sense_o_api-1.8/test/test_instance.py
--rw-r--r--   0 xiyang     (502) staff       (20)     1350 2021-06-29 19:38:05.000000 sense_o_api-1.8/test/test_intent.py
--rw-r--r--   0 xiyang     (502) staff       (20)     3028 2021-06-29 13:21:06.000000 sense_o_api-1.8/test/test_logging.py
--rw-r--r--   0 xiyang     (502) staff       (20)     4100 2021-06-29 19:36:46.000000 sense_o_api-1.8/test/test_profile.py
--rw-r--r--   0 xiyang     (502) staff       (20)    13102 2021-07-01 21:23:05.000000 sense_o_api-1.8/test/test_workflow.py
-drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-11 14:38:28.507515 sense_o_api-1.8/util/
--rw-r--r--   0 xiyang     (502) staff       (20)     6764 2021-08-11 14:36:16.000000 sense_o_api-1.8/util/sense_util.py
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.327215 sense_o_api-1.9/
+-rw-r--r--   0 xiyang     (502) staff       (20)     1095 2021-08-04 15:03:48.000000 sense_o_api-1.9/LICENSE.txt
+-rw-r--r--   0 xiyang     (502) staff       (20)      480 2021-08-24 14:16:20.326963 sense_o_api-1.9/PKG-INFO
+-rw-r--r--   0 xiyang     (502) staff       (20)      471 2021-08-09 03:53:59.000000 sense_o_api-1.9/README.md
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.295795 sense_o_api-1.9/sense/
+-rw-r--r--   0 xiyang     (502) staff       (20)       21 2021-08-24 14:15:32.000000 sense_o_api-1.9/sense/__init__.py
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.301437 sense_o_api-1.9/sense/client/
+-rw-r--r--   0 xiyang     (502) staff       (20)        0 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/client/__init__.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     2425 2021-08-24 13:55:13.000000 sense_o_api-1.9/sense/client/apiclient.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    17216 2021-08-17 20:37:09.000000 sense_o_api-1.9/sense/client/discover_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    36817 2021-08-09 03:53:59.000000 sense_o_api-1.9/sense/client/instance_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     6328 2021-08-09 03:53:59.000000 sense_o_api-1.9/sense/client/intent_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    14688 2021-08-09 03:53:59.000000 sense_o_api-1.9/sense/client/logging_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    24197 2021-06-29 19:30:33.000000 sense_o_api-1.9/sense/client/profile_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3661 2021-08-24 14:14:53.000000 sense_o_api-1.9/sense/client/requestwrapper.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    24069 2021-08-09 15:30:52.000000 sense_o_api-1.9/sense/client/workflow_combined_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    26701 2021-08-09 03:53:59.000000 sense_o_api-1.9/sense/client/workflow_phased_api.py
+-rw-r--r--   0 xiyang     (502) staff       (20)      486 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/common.py
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.320645 sense_o_api-1.9/sense/models/
+-rw-r--r--   0 xiyang     (502) staff       (20)     2439 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/__init__.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4267 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/bandwidth.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3686 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/capability_description.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     7320 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/connection.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4387 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/connection_bandwidth.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4490 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/connection_path_tprofile.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4623 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/connection_schedule.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4547 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/connection_suggest_ip_range.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     7378 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/connection_terminals.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3642 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/delta.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4732 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/discover_description.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3870 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/discover_description_end_points.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4130 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/dnc_schema.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     5163 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/dnc_schema_data.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4425 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/domain_description.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     5399 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/domain_description_edge_points.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    11207 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/full_profile.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4817 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/inline_response200.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     7794 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/intent.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3304 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/intent_expanded.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     9425 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/log.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     2527 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/log_level.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     7708 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/logging_configuration.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4220 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/logging_configuration_loggers.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     2446 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/one_of_service_intent_data.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     2765 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/operation.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3043 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/path.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4902 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/profile_edit.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     5611 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/profile_license.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     6184 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/profile_manifest.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     5724 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/service_description.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     6987 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/service_intent.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3761 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/service_intent_queries.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     5522 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/service_intent_response.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     9565 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/slim_profile.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     5035 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/terminal.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    10851 2021-06-17 12:42:40.000000 sense_o_api-1.9/sense/models/verification_result.py
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.322604 sense_o_api-1.9/sense_o_api.egg-info/
+-rw-r--r--   0 xiyang     (502) staff       (20)      480 2021-08-24 14:16:20.000000 sense_o_api-1.9/sense_o_api.egg-info/PKG-INFO
+-rw-r--r--   0 xiyang     (502) staff       (20)     1928 2021-08-24 14:16:20.000000 sense_o_api-1.9/sense_o_api.egg-info/SOURCES.txt
+-rw-r--r--   0 xiyang     (502) staff       (20)        1 2021-08-24 14:16:20.000000 sense_o_api-1.9/sense_o_api.egg-info/dependency_links.txt
+-rw-r--r--   0 xiyang     (502) staff       (20)       27 2021-08-24 14:16:20.000000 sense_o_api-1.9/sense_o_api.egg-info/requires.txt
+-rw-r--r--   0 xiyang     (502) staff       (20)       11 2021-08-24 14:16:20.000000 sense_o_api-1.9/sense_o_api.egg-info/top_level.txt
+-rw-r--r--   0 xiyang     (502) staff       (20)       38 2021-08-24 14:16:20.327364 sense_o_api-1.9/setup.cfg
+-rw-r--r--   0 xiyang     (502) staff       (20)      803 2021-08-09 03:53:59.000000 sense_o_api-1.9/setup.py
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.325524 sense_o_api-1.9/test/
+-rw-r--r--   0 xiyang     (502) staff       (20)        0 2021-06-17 12:42:40.000000 sense_o_api-1.9/test/__init__.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     2033 2021-08-17 20:46:11.000000 sense_o_api-1.9/test/test_discover.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3816 2021-08-18 14:08:56.000000 sense_o_api-1.9/test/test_instance.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     1350 2021-06-29 19:38:05.000000 sense_o_api-1.9/test/test_intent.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     3028 2021-06-29 13:21:06.000000 sense_o_api-1.9/test/test_logging.py
+-rw-r--r--   0 xiyang     (502) staff       (20)     4100 2021-06-29 19:36:46.000000 sense_o_api-1.9/test/test_profile.py
+-rw-r--r--   0 xiyang     (502) staff       (20)    13102 2021-07-01 21:23:05.000000 sense_o_api-1.9/test/test_workflow.py
+drwxr-xr-x   0 xiyang     (502) staff       (20)        0 2021-08-24 14:16:20.326300 sense_o_api-1.9/util/
+-rw-r--r--   0 xiyang     (502) staff       (20)     6764 2021-08-11 14:36:16.000000 sense_o_api-1.9/util/sense_util.py
```

### Comparing `sense_o_api-1.8/LICENSE.txt` & `sense_o_api-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/apiclient.py` & `sense_o_api-1.9/sense/client/apiclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 import json
 import requests
 from yaml import load as yload
 from yaml import FullLoader
 
-# TODO: config file path as init param
 class ApiClient(object):
     def __init__(self):
         # For now only pass config file; Later all params
         self.token, self.config = None, None
         self.getConfig()
         self._getToken()
         pass
```

### Comparing `sense_o_api-1.8/sense/client/discover_api.py` & `sense_o_api-1.9/sense/client/discover_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/instance_api.py` & `sense_o_api-1.9/sense/client/instance_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/intent_api.py` & `sense_o_api-1.9/sense/client/intent_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/logging_api.py` & `sense_o_api-1.9/sense/client/logging_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/profile_api.py` & `sense_o_api-1.9/sense/client/profile_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/requestwrapper.py` & `sense_o_api-1.9/sense/client/requestwrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
                            params=params)
         if out.status_code == 401:
             self._refreshToken()
             out = requests.get(url,
                                headers=self.config['headers'],
                                verify=self.config['verify'],
                                params=params)
+            out.raise_for_status()
         return out.text
 
     def _put(self, api_path, data, params):
         url = self.config['REST_API'] + api_path
         out = requests.put(url,
                            headers=self.config['headers'],
                            verify=self.config['verify'],
@@ -33,14 +34,15 @@
         if out.status_code == 401:
             self._refreshToken()
             out = requests.put(url,
                                headers=self.config['headers'],
                                verify=self.config['verify'],
                                data=data,
                                params=params)
+        out.raise_for_status()
         return out.text
 
     def _post(self, api_path, data, params):
         url = self.config['REST_API'] + api_path
         out = requests.post(url,
                             headers=self.config['headers'],
                             verify=self.config['verify'],
@@ -49,28 +51,30 @@
         if out.status_code == 401:
             self._refreshToken()
             out = requests.post(url,
                                 headers=self.config['headers'],
                                 verify=self.config['verify'],
                                 data=data,
                                 params=params)
+        out.raise_for_status()
         return out.text
 
     def _delete(self, api_path, params):
         url = self.config['REST_API'] + api_path
         out = requests.delete(url,
                               headers=self.config['headers'],
                               verify=self.config['verify'],
                               params=params)
         if out.status_code == 401:
             self._refreshToken()
             out = requests.delete(url,
                                   headers=self.config['headers'],
                                   verify=self.config['verify'],
                                   params=params)
+        out.raise_for_status()
         return out.text
 
     def request(self, call_type, api_path, **kwargs):
         params = None
         if kwargs.get('query_params'):
             params = kwargs.get('query_params')
```

### Comparing `sense_o_api-1.8/sense/client/workflow_combined_api.py` & `sense_o_api-1.9/sense/client/workflow_combined_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/client/workflow_phased_api.py` & `sense_o_api-1.9/sense/client/workflow_phased_api.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/__init__.py` & `sense_o_api-1.9/sense/models/__init__.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/bandwidth.py` & `sense_o_api-1.9/sense/models/bandwidth.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/capability_description.py` & `sense_o_api-1.9/sense/models/capability_description.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/connection.py` & `sense_o_api-1.9/sense/models/connection.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/connection_bandwidth.py` & `sense_o_api-1.9/sense/models/connection_bandwidth.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/connection_path_tprofile.py` & `sense_o_api-1.9/sense/models/connection_path_tprofile.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/connection_schedule.py` & `sense_o_api-1.9/sense/models/connection_schedule.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/connection_suggest_ip_range.py` & `sense_o_api-1.9/sense/models/connection_suggest_ip_range.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/connection_terminals.py` & `sense_o_api-1.9/sense/models/connection_terminals.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/delta.py` & `sense_o_api-1.9/sense/models/delta.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/discover_description.py` & `sense_o_api-1.9/sense/models/discover_description.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/discover_description_end_points.py` & `sense_o_api-1.9/sense/models/discover_description_end_points.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/dnc_schema.py` & `sense_o_api-1.9/sense/models/dnc_schema.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/dnc_schema_data.py` & `sense_o_api-1.9/sense/models/dnc_schema_data.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/domain_description.py` & `sense_o_api-1.9/sense/models/domain_description.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/domain_description_edge_points.py` & `sense_o_api-1.9/sense/models/domain_description_edge_points.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/full_profile.py` & `sense_o_api-1.9/sense/models/full_profile.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/inline_response200.py` & `sense_o_api-1.9/sense/models/inline_response200.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/intent.py` & `sense_o_api-1.9/sense/models/intent.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/intent_expanded.py` & `sense_o_api-1.9/sense/models/intent_expanded.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/log.py` & `sense_o_api-1.9/sense/models/log.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/log_level.py` & `sense_o_api-1.9/sense/models/log_level.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/logging_configuration.py` & `sense_o_api-1.9/sense/models/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/logging_configuration_loggers.py` & `sense_o_api-1.9/sense/models/logging_configuration_loggers.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/one_of_service_intent_data.py` & `sense_o_api-1.9/sense/models/one_of_service_intent_data.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/operation.py` & `sense_o_api-1.9/sense/models/operation.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/path.py` & `sense_o_api-1.9/sense/models/path.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/profile_edit.py` & `sense_o_api-1.9/sense/models/profile_edit.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/profile_license.py` & `sense_o_api-1.9/sense/models/profile_license.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/profile_manifest.py` & `sense_o_api-1.9/sense/models/profile_manifest.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/service_description.py` & `sense_o_api-1.9/sense/models/service_description.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/service_intent.py` & `sense_o_api-1.9/sense/models/service_intent.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/service_intent_queries.py` & `sense_o_api-1.9/sense/models/service_intent_queries.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/service_intent_response.py` & `sense_o_api-1.9/sense/models/service_intent_response.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/slim_profile.py` & `sense_o_api-1.9/sense/models/slim_profile.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/terminal.py` & `sense_o_api-1.9/sense/models/terminal.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense/models/verification_result.py` & `sense_o_api-1.9/sense/models/verification_result.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/sense_o_api.egg-info/SOURCES.txt` & `sense_o_api-1.9/sense_o_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/setup.py` & `sense_o_api-1.9/setup.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/test/test_discover.py` & `sense_o_api-1.9/test/test_discover.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/test/test_instance.py` & `sense_o_api-1.9/test/test_instance.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/test/test_intent.py` & `sense_o_api-1.9/test/test_intent.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/test/test_logging.py` & `sense_o_api-1.9/test/test_logging.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/test/test_profile.py` & `sense_o_api-1.9/test/test_profile.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/test/test_workflow.py` & `sense_o_api-1.9/test/test_workflow.py`

 * *Files identical despite different names*

### Comparing `sense_o_api-1.8/util/sense_util.py` & `sense_o_api-1.9/util/sense_util.py`

 * *Files identical despite different names*

