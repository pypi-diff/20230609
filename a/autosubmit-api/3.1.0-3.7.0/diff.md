# Comparing `tmp/autosubmit_api-3.1.0.tar.gz` & `tmp/autosubmit_api-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/autosubmit_api-3.1.0.tar", last modified: Thu Jun  8 14:31:16 2023, max compression
+gzip compressed data, was "dist/autosubmit_api-3.7.0.tar", last modified: Fri Jun  9 09:05:24 2023, max compression
```

## Comparing `autosubmit_api-3.1.0.tar` & `autosubmit_api-3.7.0.tar`

### file list

```diff
@@ -1,200 +1,200 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    35147 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2261 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/
--rw-r--r--   0 root         (0) root         (0)       99 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18635 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/app.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164377 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/autosubmit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47503 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job.py
--rw-r--r--   0 root         (0) root         (0)     6512 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_common.py
--rw-r--r--   0 root         (0) root         (0)    16066 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_dict.py
--rw-rw-rw-   0 root         (0) root         (0)      989 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py
--rw-r--r--   0 root         (0) root         (0)    24369 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py
--rw-r--r--   0 root         (0) root         (0)   159761 2023-06-08 14:08:18.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list.py
--rw-r--r--   0 root         (0) root         (0)     5147 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py
--rw-r--r--   0 root         (0) root         (0)     3366 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py
--rw-r--r--   0 root         (0) root         (0)    21782 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packager.py
--rw-r--r--   0 root         (0) root         (0)    21025 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packages.py
--rw-r--r--   0 root         (0) root         (0)    16035 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33229 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py
--rw-r--r--   0 root         (0) root         (0)     7914 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5436 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py
--rw-rw-rw-   0 root         (0) root         (0)     4014 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py
--rw-rw-rw-   0 root         (0) root         (0)     7289 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py
--rw-rw-rw-   0 root         (0) root         (0)     2950 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py
--rw-rw-rw-   0 root         (0) root         (0)     3377 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py
--rw-rw-rw-   0 root         (0) root         (0)     2941 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py
--rw-rw-rw-   0 root         (0) root         (0)     3517 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py
--rw-rw-rw-   0 root         (0) root         (0)     6049 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py
--rw-r--r--   0 root         (0) root         (0)     5778 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py
--rw-r--r--   0 root         (0) root         (0)    37704 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py
--rw-r--r--   0 root         (0) root         (0)    24711 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py
--rw-r--r--   0 root         (0) root         (0)     7855 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py
--rw-r--r--   0 root         (0) root         (0)     3739 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py
--rw-r--r--   0 root         (0) root         (0)    10116 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/platform.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py
--rw-r--r--   0 root         (0) root         (0)    13130 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py
--rw-r--r--   0 root         (0) root         (0)     9152 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py
--rw-r--r--   0 root         (0) root         (0)     3184 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py
--rw-r--r--   0 root         (0) root         (0)     6945 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py
--rw-r--r--   0 root         (0) root         (0)     1296 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15542 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py
--rw-r--r--   0 root         (0) root         (0)     4971 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/builders/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/builders/__init__.py
--rw-r--r--   0 root         (0) root         (0)      558 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/basic_builder.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/configuration_facade_builder.py
--rw-r--r--   0 root         (0) root         (0)     3133 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/experiment_history_builder.py
--rw-r--r--   0 root         (0) root         (0)     2620 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/joblist_helper_builder.py
--rw-r--r--   0 root         (0) root         (0)     1515 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/joblist_loader_builder.py
--rw-r--r--   0 root         (0) root         (0)     2188 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/builders/pkl_organizer_builder.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/common/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7517 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/common/utils.py
--rw-rw-rw-   0 root         (0) root         (0)      596 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/common/utils_for_testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9174 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/configuration_facade.py
--rw-r--r--   0 root         (0) root         (0)     5969 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/pkl_organizer.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/experiment/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12506 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_factory.py
--rw-r--r--   0 root         (0) root         (0)     3121 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_support.py
--rw-r--r--   0 root         (0) root         (0)     3441 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_helper.py
--rw-r--r--   0 root         (0) root         (0)     8889 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_loader.py
--rw-r--r--   0 root         (0) root         (0)      637 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/test.py
--rw-r--r--   0 root         (0) root         (0)     5243 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/jobs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1321 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/edge.py
--rw-r--r--   0 root         (0) root         (0)    17156 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/graph.py
--rw-r--r--   0 root         (0) root         (0)     6891 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2669 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/test.py
--rw-r--r--   0 root         (0) root         (0)    13728 2023-06-08 14:08:18.000000 autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/tree.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/config/
--rw-r--r--   0 root         (0) root         (0)    19435 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/IConfigStrategy.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8268 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/basicConfig.py
--rw-r--r--   0 root         (0) root         (0)    49155 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/confConfigStrategy.py
--rw-r--r--   0 root         (0) root         (0)    24603 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/config_common.py
--rw-r--r--   0 root         (0) root         (0)    13398 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/config/ymlConfigStrategy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/database/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/database/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164539 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/autosubmit.py
--rw-r--r--   0 root         (0) root         (0)    24836 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_common.py
--rw-r--r--   0 root         (0) root         (0)    93216 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_jobdata.py
--rw-r--r--   0 root         (0) root         (0)     8229 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_manager.py
--rw-r--r--   0 root         (0) root         (0)     5331 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/database/db_structure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/__init__.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/as_times_db_manager.py
--rw-r--r--   0 root         (0) root         (0)    37090 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/common_db_requests.py
--rw-r--r--   0 root         (0) root         (0)    69844 2023-06-08 14:08:54.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/common_requests.py
--rw-r--r--   0 root         (0) root         (0)     5784 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_common.py
--rw-r--r--   0 root         (0) root         (0)     1904 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_db_manager.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/test.py
--rw-r--r--   0 root         (0) root         (0)      647 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/experiment/utils.py
--rw-r--r--   0 root         (0) root         (0)  2569500 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/get-pip.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/git/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/git/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8606 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/git/autosubmit_git.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7514 2023-06-08 14:08:18.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/experiment_run.py
--rw-r--r--   0 root         (0) root         (0)    11544 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/data_classes/job_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5781 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_manager.py
--rw-rw-rw-   0 root         (0) root         (0)     5197 2022-04-13 10:23:20.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_models.py
--rw-r--r--   0 root         (0) root         (0)    23160 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py
--rw-r--r--   0 root         (0) root         (0)     6721 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py
--rw-r--r--   0 root         (0) root         (0)    13582 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/database_managers/test.py
--rw-r--r--   0 root         (0) root         (0)    22104 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/experiment_history.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/experiment_status.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/experiment_status_manager.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/internal_logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_monitor.py
--rw-rw-rw-   0 root         (0) root         (0)     2315 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_utils.py
--rw-r--r--   0 root         (0) root         (0)     2195 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor.py
--rw-r--r--   0 root         (0) root         (0)     3429 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py
--rw-r--r--   0 root         (0) root         (0)     4427 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/test.py
--rw-r--r--   0 root         (0) root         (0)    10701 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/strategies.py
--rw-r--r--   0 root         (0) root         (0)    24841 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test.py
--rw-r--r--   0 root         (0) root         (0)     3470 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test_job_history.py
--rw-r--r--   0 root         (0) root         (0)     6630 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test_strategies.py
--rw-r--r--   0 root         (0) root         (0)     1116 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/history/test_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3090 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/history/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6293 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/diagram.py
--rw-r--r--   0 root         (0) root         (0)    20102 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/monitor.py
--rw-r--r--   0 root         (0) root         (0)     1408 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/monitor/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2435 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/mail_notifier.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/notifications/notifier.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/performance/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/performance/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7642 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/performance/performance_metrics.py
--rw-r--r--   0 root         (0) root         (0)     1606 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/performance/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:15.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/job_stat.py
--rw-r--r--   0 root         (0) root         (0)     6950 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/statistics.py
--rw-rw-rw-   0 root         (0) root         (0)     2565 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/stats_summary.py
--rw-r--r--   0 root         (0) root         (0)     3390 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/test.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/statistics/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14039 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/populate_times.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/business/process_graph_drawings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6359 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic.py
--rw-r--r--   0 root         (0) root         (0)     6782 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic_energy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4077 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/populate.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/test.py
--rw-r--r--   0 root         (0) root         (0)      212 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_details_db.py
--rw-r--r--   0 root         (0) root         (0)      249 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_graph.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_queue_run_times.py
--rw-r--r--   0 root         (0) root         (0)      307 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/populate_running_experiments.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/test.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/test_esarchive.py
--rw-r--r--   0 root         (0) root         (0)      184 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/autosubmit_api/workers/verify_complete.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      588 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7930 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      182 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-08 14:31:14.000000 autosubmit_api-3.1.0/autosubmit_api.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 14:31:16.000000 autosubmit_api-3.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1335 2023-01-24 10:12:43.000000 autosubmit_api-3.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35147 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2261 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18635 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/app.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164377 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/autosubmit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47503 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job.py
+-rw-r--r--   0 root         (0) root         (0)     6512 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_common.py
+-rw-r--r--   0 root         (0) root         (0)    16066 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_dict.py
+-rw-rw-rw-   0 root         (0) root         (0)      989 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    24369 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py
+-rw-r--r--   0 root         (0) root         (0)   159761 2023-06-08 14:08:18.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_list.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py
+-rw-r--r--   0 root         (0) root         (0)    21782 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_packager.py
+-rw-r--r--   0 root         (0) root         (0)    21025 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_packages.py
+-rw-r--r--   0 root         (0) root         (0)    16035 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33229 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)     7914 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5436 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     4014 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     1804 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     7289 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2950 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     3377 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2941 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     3517 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py
+-rw-rw-rw-   0 root         (0) root         (0)     6049 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py
+-rw-r--r--   0 root         (0) root         (0)     5778 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py
+-rw-r--r--   0 root         (0) root         (0)    37704 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py
+-rw-r--r--   0 root         (0) root         (0)    24711 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py
+-rw-r--r--   0 root         (0) root         (0)     7855 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     3739 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py
+-rw-r--r--   0 root         (0) root         (0)    10116 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/platform.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py
+-rw-r--r--   0 root         (0) root         (0)    13130 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py
+-rw-r--r--   0 root         (0) root         (0)     9152 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py
+-rw-r--r--   0 root         (0) root         (0)     6945 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py
+-rw-r--r--   0 root         (0) root         (0)     1296 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15542 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py
+-rw-r--r--   0 root         (0) root         (0)     4971 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/builders/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/builders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      558 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/builders/basic_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/builders/configuration_facade_builder.py
+-rw-r--r--   0 root         (0) root         (0)     3133 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/builders/experiment_history_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2620 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/builders/joblist_helper_builder.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/builders/joblist_loader_builder.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/builders/pkl_organizer_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/common/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7517 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/common/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      596 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/common/utils_for_testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/components/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/components/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/components/experiment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/components/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9174 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/components/experiment/configuration_facade.py
+-rw-r--r--   0 root         (0) root         (0)     5969 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/experiment/pkl_organizer.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/experiment/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12506 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/job_factory.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/job_support.py
+-rw-r--r--   0 root         (0) root         (0)     3441 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/joblist_helper.py
+-rw-r--r--   0 root         (0) root         (0)     8889 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/joblist_loader.py
+-rw-r--r--   0 root         (0) root         (0)      637 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/test.py
+-rw-r--r--   0 root         (0) root         (0)     5243 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/jobs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1321 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/edge.py
+-rw-r--r--   0 root         (0) root         (0)    17156 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/graph.py
+-rw-r--r--   0 root         (0) root         (0)     6891 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/tree/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/tree/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2669 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/tree/test.py
+-rw-r--r--   0 root         (0) root         (0)    13728 2023-06-08 14:08:18.000000 autosubmit_api-3.7.0/autosubmit_api/components/representations/tree/tree.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/config/
+-rw-r--r--   0 root         (0) root         (0)    19435 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/config/IConfigStrategy.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8268 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/config/basicConfig.py
+-rw-r--r--   0 root         (0) root         (0)    49155 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/config/confConfigStrategy.py
+-rw-r--r--   0 root         (0) root         (0)    24603 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/config/config_common.py
+-rw-r--r--   0 root         (0) root         (0)    13398 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/config/ymlConfigStrategy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/database/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/database/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164539 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/database/autosubmit.py
+-rw-r--r--   0 root         (0) root         (0)    24836 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/database/db_common.py
+-rw-r--r--   0 root         (0) root         (0)    93216 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/database/db_jobdata.py
+-rw-r--r--   0 root         (0) root         (0)     8229 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/database/db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5331 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/database/db_structure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      590 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/as_times_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)    37090 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/common_db_requests.py
+-rw-r--r--   0 root         (0) root         (0)    69844 2023-06-09 09:04:04.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/common_requests.py
+-rw-r--r--   0 root         (0) root         (0)     5784 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/experiment_common.py
+-rw-r--r--   0 root         (0) root         (0)     1904 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/experiment_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/test.py
+-rw-r--r--   0 root         (0) root         (0)      647 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/experiment/utils.py
+-rw-r--r--   0 root         (0) root         (0)  2569500 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/get-pip.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/git/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/git/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8606 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/git/autosubmit_git.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/history/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/history/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/history/data_classes/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/history/data_classes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7514 2023-06-08 14:08:18.000000 autosubmit_api-3.7.0/autosubmit_api/history/data_classes/experiment_run.py
+-rw-r--r--   0 root         (0) root         (0)    11544 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/data_classes/job_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5781 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/database_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     5197 2022-04-13 10:23:20.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/database_models.py
+-rw-r--r--   0 root         (0) root         (0)    23160 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)     6721 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py
+-rw-r--r--   0 root         (0) root         (0)    13582 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/database_managers/test.py
+-rw-r--r--   0 root         (0) root         (0)    22104 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/experiment_history.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/experiment_status.py
+-rw-r--r--   0 root         (0) root         (0)     3973 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/experiment_status_manager.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/internal_logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/platform_monitor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2315 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/platform_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2195 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/slurm_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     3429 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/test.py
+-rw-r--r--   0 root         (0) root         (0)    10701 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/strategies.py
+-rw-r--r--   0 root         (0) root         (0)    24841 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/test.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/test_job_history.py
+-rw-r--r--   0 root         (0) root         (0)     6630 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/test_strategies.py
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/history/test_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3090 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/history/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/monitor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/monitor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6293 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/monitor/diagram.py
+-rw-r--r--   0 root         (0) root         (0)    20102 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/monitor/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/monitor/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/notifications/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/notifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2435 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/notifications/mail_notifier.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/notifications/notifier.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/performance/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/performance/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7642 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/performance/performance_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/performance/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/job_stat.py
+-rw-r--r--   0 root         (0) root         (0)     6950 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/statistics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2565 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/stats_summary.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/test.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/statistics/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/workers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/workers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/workers/business/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/workers/business/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14039 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/business/populate_times.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/business/process_graph_drawings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/workers/deprecated/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/workers/deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/deprecated/fix_historic.py
+-rw-r--r--   0 root         (0) root         (0)     6782 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/deprecated/fix_historic_energy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_details/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-04-05 15:15:49.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_details/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4077 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_details/populate.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_details/test.py
+-rw-r--r--   0 root         (0) root         (0)      212 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_details_db.py
+-rw-r--r--   0 root         (0) root         (0)      249 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_graph.py
+-rw-r--r--   0 root         (0) root         (0)      220 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_queue_run_times.py
+-rw-r--r--   0 root         (0) root         (0)      307 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/populate_running_experiments.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/test.py
+-rw-r--r--   0 root         (0) root         (0)      158 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/test_esarchive.py
+-rw-r--r--   0 root         (0) root         (0)      184 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/autosubmit_api/workers/verify_complete.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/autosubmit_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-09 09:05:23.000000 autosubmit_api-3.7.0/autosubmit_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7930 2023-06-09 09:05:23.000000 autosubmit_api-3.7.0/autosubmit_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-09 09:05:23.000000 autosubmit_api-3.7.0/autosubmit_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      182 2023-06-09 09:05:23.000000 autosubmit_api-3.7.0/autosubmit_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-09 09:05:23.000000 autosubmit_api-3.7.0/autosubmit_api.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-09 09:05:24.000000 autosubmit_api-3.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1335 2023-01-24 10:12:43.000000 autosubmit_api-3.7.0/setup.py
```

### Comparing `autosubmit_api-3.1.0/LICENSE` & `autosubmit_api-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/PKG-INFO` & `autosubmit_api-3.7.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit_api
-Version: 3.1.0
+Version: 3.7.0
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/wuruchi/autosubmit_api
 Author: Wilmer Uruchi
 Author-email: wilmer.uruchi@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-3.1.0/README.md` & `autosubmit_api-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/app.py` & `autosubmit_api-3.7.0/autosubmit_api/app.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/autosubmit.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/autosubmit.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_common.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_dict.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_dict.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_exceptions.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_grouping.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_list.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_list_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_package_persistence.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packager.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_packager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_packages.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_packages.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/job/job_utils.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/job/job_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/ecmwf_adaptor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/ecplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_cca_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/ec_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/local_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/lsf_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs10_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs11_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/pbs12_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/ps_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/sge_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/headers/slurm_header.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/locplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/lsfplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/mn_adaptor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/paramiko_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/pbsplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/platform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/psplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/saga_platform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/saga_submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/sgeplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/slurmplatform.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/submitter.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py` & `autosubmit_api-3.7.0/autosubmit_api/autosubmit_legacy/platforms/wrappers/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/builders/basic_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/builders/basic_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/builders/configuration_facade_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/builders/configuration_facade_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/builders/experiment_history_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/builders/experiment_history_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/builders/joblist_helper_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/builders/joblist_helper_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/builders/joblist_loader_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/builders/joblist_loader_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/builders/pkl_organizer_builder.py` & `autosubmit_api-3.7.0/autosubmit_api/builders/pkl_organizer_builder.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/common/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/common/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/common/utils_for_testing.py` & `autosubmit_api-3.7.0/autosubmit_api/common/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/experiment/configuration_facade.py` & `autosubmit_api-3.7.0/autosubmit_api/components/experiment/configuration_facade.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/experiment/pkl_organizer.py` & `autosubmit_api-3.7.0/autosubmit_api/components/experiment/pkl_organizer.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/experiment/test.py` & `autosubmit_api-3.7.0/autosubmit_api/components/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_factory.py` & `autosubmit_api-3.7.0/autosubmit_api/components/jobs/job_factory.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/jobs/job_support.py` & `autosubmit_api-3.7.0/autosubmit_api/components/jobs/job_support.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_helper.py` & `autosubmit_api-3.7.0/autosubmit_api/components/jobs/joblist_helper.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/jobs/joblist_loader.py` & `autosubmit_api-3.7.0/autosubmit_api/components/jobs/joblist_loader.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/jobs/test.py` & `autosubmit_api-3.7.0/autosubmit_api/components/jobs/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/jobs/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/components/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/edge.py` & `autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/edge.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/graph.py` & `autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/graph.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/representations/graph/test.py` & `autosubmit_api-3.7.0/autosubmit_api/components/representations/graph/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/test.py` & `autosubmit_api-3.7.0/autosubmit_api/components/representations/tree/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/components/representations/tree/tree.py` & `autosubmit_api-3.7.0/autosubmit_api/components/representations/tree/tree.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/config/IConfigStrategy.py` & `autosubmit_api-3.7.0/autosubmit_api/config/IConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/config/basicConfig.py` & `autosubmit_api-3.7.0/autosubmit_api/config/basicConfig.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/config/confConfigStrategy.py` & `autosubmit_api-3.7.0/autosubmit_api/config/confConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/config/config_common.py` & `autosubmit_api-3.7.0/autosubmit_api/config/config_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/config/ymlConfigStrategy.py` & `autosubmit_api-3.7.0/autosubmit_api/config/ymlConfigStrategy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/database/autosubmit.py` & `autosubmit_api-3.7.0/autosubmit_api/database/autosubmit.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/database/db_common.py` & `autosubmit_api-3.7.0/autosubmit_api/database/db_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/database/db_jobdata.py` & `autosubmit_api-3.7.0/autosubmit_api/database/db_jobdata.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/database/db_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/database/db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/database/db_structure.py` & `autosubmit_api-3.7.0/autosubmit_api/database/db_structure.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/as_times_db_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/as_times_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/common_db_requests.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/common_db_requests.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/common_requests.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/common_requests.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_common.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/experiment_common.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/experiment_db_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/experiment_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/test.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/experiment/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/get-pip.py` & `autosubmit_api-3.7.0/autosubmit_api/get-pip.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/git/autosubmit_git.py` & `autosubmit_api-3.7.0/autosubmit_api/git/autosubmit_git.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/data_classes/experiment_run.py` & `autosubmit_api-3.7.0/autosubmit_api/history/data_classes/experiment_run.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/data_classes/job_data.py` & `autosubmit_api-3.7.0/autosubmit_api/history/data_classes/job_data.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/history/database_managers/database_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/database_models.py` & `autosubmit_api-3.7.0/autosubmit_api/history/database_managers/database_models.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/history/database_managers/experiment_history_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/history/database_managers/experiment_status_db_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/database_managers/test.py` & `autosubmit_api-3.7.0/autosubmit_api/history/database_managers/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/experiment_history.py` & `autosubmit_api-3.7.0/autosubmit_api/history/experiment_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/experiment_status.py` & `autosubmit_api-3.7.0/autosubmit_api/history/experiment_status.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/experiment_status_manager.py` & `autosubmit_api-3.7.0/autosubmit_api/history/experiment_status_manager.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/internal_logging.py` & `autosubmit_api-3.7.0/autosubmit_api/history/internal_logging.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_monitor.py` & `autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/platform_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/platform_utils.py` & `autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/platform_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor.py` & `autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/slurm_monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py` & `autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/slurm_monitor_item.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/platform_monitor/test.py` & `autosubmit_api-3.7.0/autosubmit_api/history/platform_monitor/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/strategies.py` & `autosubmit_api-3.7.0/autosubmit_api/history/strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/test.py` & `autosubmit_api-3.7.0/autosubmit_api/history/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/test_job_history.py` & `autosubmit_api-3.7.0/autosubmit_api/history/test_job_history.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/test_strategies.py` & `autosubmit_api-3.7.0/autosubmit_api/history/test_strategies.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/test_utils.py` & `autosubmit_api-3.7.0/autosubmit_api/history/test_utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/history/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/history/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/monitor/diagram.py` & `autosubmit_api-3.7.0/autosubmit_api/monitor/diagram.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/monitor/monitor.py` & `autosubmit_api-3.7.0/autosubmit_api/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/monitor/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/notifications/mail_notifier.py` & `autosubmit_api-3.7.0/autosubmit_api/notifications/mail_notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/notifications/notifier.py` & `autosubmit_api-3.7.0/autosubmit_api/notifications/notifier.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/performance/performance_metrics.py` & `autosubmit_api-3.7.0/autosubmit_api/performance/performance_metrics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/performance/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/performance/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/statistics/job_stat.py` & `autosubmit_api-3.7.0/autosubmit_api/statistics/job_stat.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/statistics/statistics.py` & `autosubmit_api-3.7.0/autosubmit_api/statistics/statistics.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/statistics/stats_summary.py` & `autosubmit_api-3.7.0/autosubmit_api/statistics/stats_summary.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/statistics/test.py` & `autosubmit_api-3.7.0/autosubmit_api/statistics/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/statistics/utils.py` & `autosubmit_api-3.7.0/autosubmit_api/statistics/utils.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/business/populate_times.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/business/populate_times.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/business/process_graph_drawings.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/business/process_graph_drawings.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/deprecated/fix_historic.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/deprecated/fix_historic_energy.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/deprecated/fix_historic_energy.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/populate.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/populate_details/populate.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/populate_details/test.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/populate_details/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api/workers/test.py` & `autosubmit_api-3.7.0/autosubmit_api/workers/test.py`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/autosubmit_api.egg-info/PKG-INFO` & `autosubmit_api-3.7.0/autosubmit_api.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autosubmit-api
-Version: 3.1.0
+Version: 3.7.0
 Summary: An extension to the Autosubmit package that serves its information as an API
 Home-page: https://earth.bsc.es/gitlab/wuruchi/autosubmit_api
 Author: Wilmer Uruchi
 Author-email: wilmer.uruchi@bsc.es
 License: GNU GPL
 Keywords: autosubmit,API
 Classifier: Development Status :: 4 - Beta
```

### Comparing `autosubmit_api-3.1.0/autosubmit_api.egg-info/SOURCES.txt` & `autosubmit_api-3.7.0/autosubmit_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autosubmit_api-3.1.0/setup.py` & `autosubmit_api-3.7.0/setup.py`

 * *Files identical despite different names*

