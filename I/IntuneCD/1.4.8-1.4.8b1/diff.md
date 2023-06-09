# Comparing `tmp/IntuneCD-1.4.8.tar.gz` & `tmp/IntuneCD-1.4.8b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IntuneCD-1.4.8.tar", last modified: Fri Jun  9 07:59:21 2023, max compression
+gzip compressed data, was "IntuneCD-1.4.8b1.tar", last modified: Wed Jun  7 14:15:04 2023, max compression
```

## Comparing `IntuneCD-1.4.8.tar` & `IntuneCD-1.4.8b1.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:59:21.182539 IntuneCD-1.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-09 07:59:21.182539 IntuneCD-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-09 07:59:21.182539 IntuneCD-1.4.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:59:21.158539 IntuneCD-1.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:59:21.174539 IntuneCD-1.4.8/src/IntuneCD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/assignment_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_AppProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_apns.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_assignmentFilters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_autopilotDevices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_compliancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_deviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_managedGPlay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_managementPartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_remoteAssistancePartner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_vppTokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/backup_windowsEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/get_accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/run_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/run_documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/run_update.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_appConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_appProtection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_appleEnrollmentProfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_assignmentFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_conditionalAccess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_configurationPolicies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_customAttributeShellScript.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_deviceCategories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_deviceManagementSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_enrollmentConfigurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_enrollmentStatusPage.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_groupPolicyConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_managementIntents.py
--rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_notificationTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_powershellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_proactiveRemediation.py
--rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_profiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_shellScripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/src/IntuneCD/update_windowsEnrollmentProfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:59:21.178539 IntuneCD-1.4.8/src/IntuneCD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3488 2023-06-09 07:59:21.000000 IntuneCD-1.4.8/src/IntuneCD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-09 07:59:21.000000 IntuneCD-1.4.8/src/IntuneCD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:59:21.000000 IntuneCD-1.4.8/src/IntuneCD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-09 07:59:21.000000 IntuneCD-1.4.8/src/IntuneCD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 07:59:21.000000 IntuneCD-1.4.8/src/IntuneCD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 07:59:21.000000 IntuneCD-1.4.8/src/IntuneCD.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:59:21.182539 IntuneCD-1.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_check_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_clean_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_diff_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_documentation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_get_added_removed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_get_authparams.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_graph_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_graph_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_group_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_load_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_match.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_remove_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_save_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-09 07:59:06.000000 IntuneCD-1.4.8/tests/test_update_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.645342 IntuneCD-1.4.8b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.653342 IntuneCD-1.4.8b1/src/IntuneCD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/assignment_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_AppProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_apns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_assignmentFilters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_autopilotDevices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_compliancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_managedGPlay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_managementPartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_remoteAssistancePartner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_vppTokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/backup_windowsEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/get_accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7753 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12500 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/run_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/run_documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11212 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/run_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8154 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_appConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_appProtection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_appleEnrollmentProfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_assignmentFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9372 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7193 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_conditionalAccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_configurationPolicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8929 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_customAttributeShellScript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_deviceCategories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_deviceManagementSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentConfigurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentStatusPage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24286 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_groupPolicyConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9069 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_managementIntents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8066 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_notificationTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8428 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_powershellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10612 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_proactiveRemediation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16118 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_profiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_shellScripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7197 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/src/IntuneCD/update_windowsEnrollmentProfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.653342 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 14:15:04.000000 IntuneCD-1.4.8b1/src/IntuneCD.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 14:15:04.657343 IntuneCD-1.4.8b1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_check_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_clean_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_diff_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_documentation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_get_added_removed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_get_authparams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_graph_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17428 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_graph_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_group_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_load_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_remove_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_save_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-07 14:14:51.000000 IntuneCD-1.4.8b1/tests/test_update_frontend.py
```

### Comparing `IntuneCD-1.4.8/LICENSE` & `IntuneCD-1.4.8b1/LICENSE`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/PKG-INFO` & `IntuneCD-1.4.8b1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.8
+Version: 1.4.8b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,19 +25,19 @@
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/204297420-4b5373a8-4864-4710-a4a5-802ea4ec08d5.png#gh-dark-mode-only" width="500" height="300">
 </p>
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/204501041-a7cc2321-8991-4abb-a622-97f72f19051f.png#gh-light-mode-only" width="500" height="300">
 </p>
 
-IntuneCD, short for Intune Continuous Delivery, is a powerful Python package designed to facilitate the backup and update of configurations in Intune. With a primary focus on seamless integration with pipelines, it enables users to maintain a comprehensive history of configuration changes and track specific setting modifications.
+IntuneCD or, Intune Continuous Delivery as it stands for is a Python package that is used to back up and update configurations in Intune. It was created with running it from a pipeline in mind. Using this approach we get complete history of which configurations have been changed and what setting has been changed.
 
-The core functionality of IntuneCD revolves around securely backing up Intune configurations to a Git repository within a DEV environment. It goes beyond simple backup capabilities by automatically detecting any alterations made to configurations and efficiently propagating those changes to the PROD Intune environment.
+The main function is to back up configurations from Intune to a Git repository from a DEV environment and if any configurations has changed, push them to PROD Intune environment.
 
-By leveraging IntuneCD, users can streamline their configuration management workflow, ensuring smooth and consistent deployment of settings while maintaining an auditable history of changes.
+The package can also be run standalone outside a pipeline, or in one to only backup data.
 
 # Exciting news 📣
 The front end for IntuneCD has now been released. Check it out [here](https://github.com/almenscorner/intunecd-monitor)
 
 ***
 
 ### Getting started
```

### Comparing `IntuneCD-1.4.8/README.md` & `IntuneCD-1.4.8b1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/204297420-4b5373a8-4864-4710-a4a5-802ea4ec08d5.png#gh-dark-mode-only" width="500" height="300">
 </p>
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/204501041-a7cc2321-8991-4abb-a622-97f72f19051f.png#gh-light-mode-only" width="500" height="300">
 </p>
 
-IntuneCD, short for Intune Continuous Delivery, is a powerful Python package designed to facilitate the backup and update of configurations in Intune. With a primary focus on seamless integration with pipelines, it enables users to maintain a comprehensive history of configuration changes and track specific setting modifications.
+IntuneCD or, Intune Continuous Delivery as it stands for is a Python package that is used to back up and update configurations in Intune. It was created with running it from a pipeline in mind. Using this approach we get complete history of which configurations have been changed and what setting has been changed.
 
-The core functionality of IntuneCD revolves around securely backing up Intune configurations to a Git repository within a DEV environment. It goes beyond simple backup capabilities by automatically detecting any alterations made to configurations and efficiently propagating those changes to the PROD Intune environment.
+The main function is to back up configurations from Intune to a Git repository from a DEV environment and if any configurations has changed, push them to PROD Intune environment.
 
-By leveraging IntuneCD, users can streamline their configuration management workflow, ensuring smooth and consistent deployment of settings while maintaining an auditable history of changes.
+The package can also be run standalone outside a pipeline, or in one to only backup data.
 
 # Exciting news 📣
 The front end for IntuneCD has now been released. Check it out [here](https://github.com/almenscorner/intunecd-monitor)
 
 ***
 
 ### Getting started
```

### Comparing `IntuneCD-1.4.8/setup.cfg` & `IntuneCD-1.4.8b1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = IntuneCD
-version = 1.4.8
+version = 1.4.8.beta1
 author = Tobias Almén
 author_email = almenscorner@outlook.com
 description = Tool to backup and update configurations in Intune
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/almenscorner/IntuneCD
 project_urls =
```

### Comparing `IntuneCD-1.4.8/src/IntuneCD/archive.py` & `IntuneCD-1.4.8b1/src/IntuneCD/archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/assignment_report.py` & `IntuneCD-1.4.8b1/src/IntuneCD/assignment_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_AppProtection.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_AppProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_apns.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_apns.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_appConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_appleEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_applications.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_applications.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_assignmentFilters.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_assignmentFilters.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_autopilotDevices.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_autopilotDevices.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_compliance.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_compliancePartner.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_compliancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_conditionalAccess.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_configurationPolicies.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_customAttributeShellScript.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_deviceCategories.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceCategories.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_deviceManagementSettings.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_enrollmentConfigurations.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_enrollmentStatusPage.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_groupPolicyConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_managedGPlay.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_managedGPlay.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_managementIntents.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_managementPartner.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_managementPartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_notificationTemplate.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_powershellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_powershellScripts.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,21 +32,27 @@
     configpath = path + "/" + "Scripts/Powershell/"
     data = makeapirequest(ENDPOINT, token)
     if data["value"]:
         script_ids = []
         for script in data["value"]:
             script_ids.append(script["id"])
 
-        assignment_responses = batch_assignment(data, "deviceManagement/deviceManagementScripts/", "/assignments", token)
-        script_data_responses = batch_request(script_ids, "deviceManagement/deviceManagementScripts/", "", token)
+        assignment_responses = batch_assignment(
+            data, "deviceManagement/deviceManagementScripts/", "/assignments", token
+        )
+        script_data_responses = batch_request(
+            script_ids, "deviceManagement/deviceManagementScripts/", "", token
+        )
 
         for script_data in script_data_responses:
             results["config_count"] += 1
             if "assignments" not in exclude:
-                assignments = get_object_assignment(script_data["id"], assignment_responses)
+                assignments = get_object_assignment(
+                    script_data["id"], assignment_responses
+                )
                 if assignments:
                     script_data["assignments"] = assignments
 
             script_data = remove_keys(script_data)
 
             print("Backing up Powershell script: " + script_data["displayName"])
 
@@ -55,15 +61,14 @@
             # Save Powershell script as JSON or YAML depending on configured value
             # in "-o"
             save_output(output, configpath, fname, script_data)
 
             results["outputs"].append(fname)
 
             # Save Powershell script data to the script data folder
-            if script_data.get("scriptContent"):
-                if not os.path.exists(configpath + "Script Data/"):
-                    os.makedirs(configpath + "Script Data/")
-                decoded = base64.b64decode(script_data["scriptContent"]).decode("utf-8")
-                f = open(configpath + "Script Data/" + script_data["fileName"], "w")
-                f.write(decoded)
+            if not os.path.exists(configpath + "Script Data/"):
+                os.makedirs(configpath + "Script Data/")
+            decoded = base64.b64decode(script_data["scriptContent"]).decode("utf-8")
+            f = open(configpath + "Script Data/" + script_data["fileName"], "w")
+            f.write(decoded)
 
     return results
```

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_proactiveRemediation.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_profiles.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_remoteAssistancePartner.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_remoteAssistancePartner.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_shellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_vppTokens.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_vppTokens.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/backup_windowsEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/backup_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/check_file.py` & `IntuneCD-1.4.8b1/src/IntuneCD/check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/clean_filename.py` & `IntuneCD-1.4.8b1/src/IntuneCD/clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/diff_summary.py` & `IntuneCD-1.4.8b1/src/IntuneCD/diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/documentation_functions.py` & `IntuneCD-1.4.8b1/src/IntuneCD/documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/get_accesstoken.py` & `IntuneCD-1.4.8b1/src/IntuneCD/get_accesstoken.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/get_authparams.py` & `IntuneCD-1.4.8b1/src/IntuneCD/get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/graph_batch.py` & `IntuneCD-1.4.8b1/src/IntuneCD/graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/graph_request.py` & `IntuneCD-1.4.8b1/src/IntuneCD/graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/load_file.py` & `IntuneCD-1.4.8b1/src/IntuneCD/load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/remove_keys.py` & `IntuneCD-1.4.8b1/src/IntuneCD/remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/run_backup.py` & `IntuneCD-1.4.8b1/src/IntuneCD/run_backup.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/run_documentation.py` & `IntuneCD-1.4.8b1/src/IntuneCD/run_documentation.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,29 +413,29 @@
         )
 
         if jsondata:
             json_dict = json.loads(jsondata)
             if "title" in json_dict:
                 title = json_dict["title"]
             else:
-                title = "Intune Documentation"
+                title = "MEM Documentation"
             if "intro" in json_dict:
                 intro = json_dict["intro"]
             else:
                 intro = args.intro
             if "tenant" in json_dict:
                 tenant = json_dict["tenant"]
             else:
                 tenant = f"**Tenant:** {tenantname}"
             if "updated" in json_dict:
                 updated = json_dict["updated"]
             else:
                 updated = f"**Document updated on:**"
         else:
-            title = "Intune Documentation"
+            title = "MEM Documentation"
             intro = args.intro
             tenant = f"**Tenant:** {tenantname}"
             updated = f"**Document updated on:**"
 
         if split:
             files = get_md_files(configpath)
             index_md = f"{configpath}/index.md"
```

### Comparing `IntuneCD-1.4.8/src/IntuneCD/run_update.py` & `IntuneCD-1.4.8b1/src/IntuneCD/run_update.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/save_output.py` & `IntuneCD-1.4.8b1/src/IntuneCD/save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_appConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_appConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_appProtection.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_appProtection.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_appleEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_appleEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_assignment.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_assignment.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_assignmentFilter.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_assignmentFilter.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_compliance.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_compliance.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_conditionalAccess.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_conditionalAccess.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_configurationPolicies.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_configurationPolicies.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_customAttributeShellScript.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_customAttributeShellScript.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_deviceCategories.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_deviceCategories.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_deviceManagementSettings.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_deviceManagementSettings.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_enrollmentConfigurations.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentConfigurations.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_enrollmentStatusPage.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_enrollmentStatusPage.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_frontend.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_frontend.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_groupPolicyConfiguration.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_groupPolicyConfiguration.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_managementIntents.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_managementIntents.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_notificationTemplate.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_notificationTemplate.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_powershellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_powershellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_proactiveRemediation.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_proactiveRemediation.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_profiles.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_profiles.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_shellScripts.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_shellScripts.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD/update_windowsEnrollmentProfile.py` & `IntuneCD-1.4.8b1/src/IntuneCD/update_windowsEnrollmentProfile.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/src/IntuneCD.egg-info/PKG-INFO` & `IntuneCD-1.4.8b1/src/IntuneCD.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IntuneCD
-Version: 1.4.8
+Version: 1.4.8b1
 Summary: Tool to backup and update configurations in Intune
 Home-page: https://github.com/almenscorner/IntuneCD
 Author: Tobias Almén
 Author-email: almenscorner@outlook.com
 Project-URL: Bug Tracker, https://github.com/almenscorner/IntuneCD/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -25,19 +25,19 @@
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/204297420-4b5373a8-4864-4710-a4a5-802ea4ec08d5.png#gh-dark-mode-only" width="500" height="300">
 </p>
 <p align="center">
   <img src="https://user-images.githubusercontent.com/78877636/204501041-a7cc2321-8991-4abb-a622-97f72f19051f.png#gh-light-mode-only" width="500" height="300">
 </p>
 
-IntuneCD, short for Intune Continuous Delivery, is a powerful Python package designed to facilitate the backup and update of configurations in Intune. With a primary focus on seamless integration with pipelines, it enables users to maintain a comprehensive history of configuration changes and track specific setting modifications.
+IntuneCD or, Intune Continuous Delivery as it stands for is a Python package that is used to back up and update configurations in Intune. It was created with running it from a pipeline in mind. Using this approach we get complete history of which configurations have been changed and what setting has been changed.
 
-The core functionality of IntuneCD revolves around securely backing up Intune configurations to a Git repository within a DEV environment. It goes beyond simple backup capabilities by automatically detecting any alterations made to configurations and efficiently propagating those changes to the PROD Intune environment.
+The main function is to back up configurations from Intune to a Git repository from a DEV environment and if any configurations has changed, push them to PROD Intune environment.
 
-By leveraging IntuneCD, users can streamline their configuration management workflow, ensuring smooth and consistent deployment of settings while maintaining an auditable history of changes.
+The package can also be run standalone outside a pipeline, or in one to only backup data.
 
 # Exciting news 📣
 The front end for IntuneCD has now been released. Check it out [here](https://github.com/almenscorner/intunecd-monitor)
 
 ***
 
 ### Getting started
```

### Comparing `IntuneCD-1.4.8/src/IntuneCD.egg-info/SOURCES.txt` & `IntuneCD-1.4.8b1/src/IntuneCD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_archive.py` & `IntuneCD-1.4.8b1/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_check_file.py` & `IntuneCD-1.4.8b1/tests/test_check_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_clean_filename.py` & `IntuneCD-1.4.8b1/tests/test_clean_filename.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_diff_summary.py` & `IntuneCD-1.4.8b1/tests/test_diff_summary.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_documentation_functions.py` & `IntuneCD-1.4.8b1/tests/test_documentation_functions.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_get_added_removed.py` & `IntuneCD-1.4.8b1/tests/test_get_added_removed.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_get_authparams.py` & `IntuneCD-1.4.8b1/tests/test_get_authparams.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_graph_batch.py` & `IntuneCD-1.4.8b1/tests/test_graph_batch.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_graph_request.py` & `IntuneCD-1.4.8b1/tests/test_graph_request.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_group_report.py` & `IntuneCD-1.4.8b1/tests/test_group_report.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_load_file.py` & `IntuneCD-1.4.8b1/tests/test_load_file.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_match.py` & `IntuneCD-1.4.8b1/tests/test_match.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_remove_keys.py` & `IntuneCD-1.4.8b1/tests/test_remove_keys.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_save_output.py` & `IntuneCD-1.4.8b1/tests/test_save_output.py`

 * *Files identical despite different names*

### Comparing `IntuneCD-1.4.8/tests/test_update_frontend.py` & `IntuneCD-1.4.8b1/tests/test_update_frontend.py`

 * *Files identical despite different names*

