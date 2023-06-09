# Comparing `tmp/oasislmf-1.9.0.tar.gz` & `tmp/oasislmf-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/oasislmf-1.9.0.tar", last modified: Fri Jul 17 10:18:35 2020, max compression
+gzip compressed data, was "dist/oasislmf-1.9.1.tar", last modified: Tue Aug 18 16:24:35 2020, max compression
```

## Comparing `oasislmf-1.9.0.tar` & `oasislmf-1.9.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/
--rw-r--r--   0 root         (0) root         (0)      380 2020-07-17 10:18:35.000000 oasislmf-1.9.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      238 2020-07-17 10:16:47.000000 oasislmf-1.9.0/MANIFEST.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/utils/
--rw-r--r--   0 root         (0) root         (0)     8305 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/defaults.py
--rw-r--r--   0 root         (0) root         (0)       24 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3446 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/log.py
--rw-r--r--   0 root         (0) root         (0)     1154 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/diff.py
--rw-r--r--   0 root         (0) root         (0)     1333 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/compress.py
--rw-r--r--   0 root         (0) root         (0)      690 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/status.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/version_info.py
--rw-r--r--   0 root         (0) root         (0)     4885 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/profiles.py
--rw-r--r--   0 root         (0) root         (0)     4338 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/path.py
--rw-r--r--   0 root         (0) root         (0)     7099 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/deterministic_loss.py
--rw-r--r--   0 root         (0) root         (0)     1441 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/calc_rules.py
--rw-r--r--   0 root         (0) root         (0)     5089 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/fm.py
--rw-r--r--   0 root         (0) root         (0)      862 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/coverages.py
--rw-r--r--   0 root         (0) root         (0)      753 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    15936 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/peril.py
--rw-r--r--   0 root         (0) root         (0)    36238 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/utils/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/model_testing/
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2108 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_testing/validation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/cli/
--rw-r--r--   0 root         (0) root         (0)     1552 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/cleaners.py
--rw-r--r--   0 root         (0) root         (0)     1839 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/computation_command.py
--rw-r--r--   0 root         (0) root         (0)       34 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      375 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/version.py
--rw-r--r--   0 root         (0) root         (0)     4979 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/test.py
--rw-r--r--   0 root         (0) root         (0)     4881 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/exposure.py
--rw-r--r--   0 root         (0) root         (0)     3960 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/config.py
--rw-r--r--   0 root         (0) root         (0)     4919 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/inputs.py
--rw-r--r--   0 root         (0) root         (0)    29397 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/model.py
--rw-r--r--   0 root         (0) root         (0)     1514 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/root.py
--rw-r--r--   0 root         (0) root         (0)    10895 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/admin.py
--rw-r--r--   0 root         (0) root         (0)    13673 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/api.py
--rw-r--r--   0 root         (0) root         (0)     2451 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/cli/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/model_preparation/
--rw-r--r--   0 root         (0) root         (0)    19613 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/model_preparation/gul_inputs.py
--rw-r--r--   0 root         (0) root         (0)    42821 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/lookup.py
--rw-r--r--   0 root         (0) root         (0)    46131 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/model_preparation/il_inputs.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33821 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/summaries.py
--rw-r--r--   0 root         (0) root         (0)     4105 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/exposure_pre_analysis.py
--rw-r--r--   0 root         (0) root         (0)     3261 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/computation_step.py
--rw-r--r--   0 root         (0) root         (0)     2142 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/utils.py
--rw-r--r--   0 root         (0) root         (0)    39561 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/reinsurance_layer.py
--rw-r--r--   0 root         (0) root         (0)    18062 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_preparation/oed.py
--rw-r--r--   0 root         (0) root         (0)       22 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/api/
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7821 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/api/session.py
--rw-r--r--   0 root         (0) root         (0)    26368 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/api/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/_data/
--rw-r--r--   0 root         (0) root         (0)    15647 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/_data/calc_rules.csv
--rw-r--r--   0 root         (0) root         (0)    14607 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/default_loc_profile.json
--rw-r--r--   0 root         (0) root         (0)     2901 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/_data/default_fm_agg_profile.json
--rw-r--r--   0 root         (0) root         (0)    23493 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/default_combined_exposure_profile.json
--rw-r--r--   0 root         (0) root         (0)    42756 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/acc_dtypes.json
--rw-r--r--   0 root         (0) root         (0)     3038 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/default_step_policies_profile.json
--rw-r--r--   0 root         (0) root         (0)     1747 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/analysis_settings.json
--rw-r--r--   0 root         (0) root         (0)     7104 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/info_dtypes.json
--rw-r--r--   0 root         (0) root         (0)    44477 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/loc_dtypes.json
--rw-r--r--   0 root         (0) root         (0)      457 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/cookiecutter.json
--rw-r--r--   0 root         (0) root         (0)     2297 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/calc_rules_step.csv
--rw-r--r--   0 root         (0) root         (0)     1095 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/_data/default_fm_profile_field_values.json
--rw-r--r--   0 root         (0) root         (0)     5200 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/_data/default_acc_profile.json
--rw-r--r--   0 root         (0) root         (0)     3299 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/scope_dtypes.json
--rw-r--r--   0 root         (0) root         (0)     3265 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/_data/config_compatibility_profile.json
--rw-r--r--   0 root         (0) root         (0)    46186 2020-07-17 10:16:48.000000 oasislmf-1.9.0/oasislmf/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/model_execution/
--rw-r--r--   0 root         (0) root         (0)    48200 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/bash.py
--rw-r--r--   0 root         (0) root         (0)        0 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1254 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/complex_items_to_bin.py
--rw-r--r--   0 root         (0) root         (0)    16409 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/bin.py
--rw-r--r--   0 root         (0) root         (0)     1649 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/files.py
--rw-r--r--   0 root         (0) root         (0)     3656 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/runner.py
--rw-r--r--   0 root         (0) root         (0)     3035 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/conf.py
--rw-r--r--   0 root         (0) root         (0)     1592 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/model_execution/complex_items_to_csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf/schema/
--rw-r--r--   0 root         (0) root         (0)    11504 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/schema/analysis_settings.json
--rw-r--r--   0 root         (0) root         (0)     4871 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/schema/example_model_settings.json
--rw-r--r--   0 root         (0) root         (0)    33988 2020-07-17 10:16:47.000000 oasislmf-1.9.0/oasislmf/schema/model_settings.json
--rw-r--r--   0 root         (0) root         (0)    12509 2020-07-17 10:16:48.000000 oasislmf-1.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)    10834 2020-07-17 10:18:35.000000 oasislmf-1.9.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1530 2020-07-17 10:16:47.000000 oasislmf-1.9.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/bin/
--rwxr-xr-x   0 root         (0) root         (0)     5844 2020-07-17 10:16:47.000000 oasislmf-1.9.0/bin/completer_oasislmf
--rwxr-xr-x   0 root         (0) root         (0)      125 2020-07-17 10:16:47.000000 oasislmf-1.9.0/bin/oasislmf
--rwxr-xr-x   0 root         (0) root         (0)      962 2020-07-17 10:16:47.000000 oasislmf-1.9.0/bin/ktools_monitor.sh
--rw-r--r--   0 root         (0) root         (0)    19521 2020-07-17 10:16:48.000000 oasislmf-1.9.0/CHANGELOG.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      161 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)    10834 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      281 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     2680 2020-07-17 10:18:35.000000 oasislmf-1.9.0/oasislmf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      281 2020-07-17 10:16:47.000000 oasislmf-1.9.0/requirements-package.in
--rw-r--r--   0 root         (0) root         (0)     8718 2020-07-17 10:16:47.000000 oasislmf-1.9.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)      380 2020-08-18 16:24:35.000000 oasislmf-1.9.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      238 2020-08-18 16:22:53.000000 oasislmf-1.9.1/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/utils/
+-rw-r--r--   0 root         (0) root         (0)     8305 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/defaults.py
+-rw-r--r--   0 root         (0) root         (0)       24 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3446 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/log.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/diff.py
+-rw-r--r--   0 root         (0) root         (0)     1333 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/compress.py
+-rw-r--r--   0 root         (0) root         (0)      690 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/status.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/version_info.py
+-rw-r--r--   0 root         (0) root         (0)     4885 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/profiles.py
+-rw-r--r--   0 root         (0) root         (0)     4338 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/path.py
+-rw-r--r--   0 root         (0) root         (0)     7099 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/deterministic_loss.py
+-rw-r--r--   0 root         (0) root         (0)     1441 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/calc_rules.py
+-rw-r--r--   0 root         (0) root         (0)     5089 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/fm.py
+-rw-r--r--   0 root         (0) root         (0)      862 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/coverages.py
+-rw-r--r--   0 root         (0) root         (0)      753 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    15936 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/peril.py
+-rw-r--r--   0 root         (0) root         (0)    36238 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/utils/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/model_testing/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_testing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2108 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_testing/validation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/cli/
+-rw-r--r--   0 root         (0) root         (0)     1552 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/cleaners.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/computation_command.py
+-rw-r--r--   0 root         (0) root         (0)       34 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      375 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/version.py
+-rw-r--r--   0 root         (0) root         (0)     4979 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/test.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/exposure.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/config.py
+-rw-r--r--   0 root         (0) root         (0)     4919 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/inputs.py
+-rw-r--r--   0 root         (0) root         (0)    29397 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/model.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/root.py
+-rw-r--r--   0 root         (0) root         (0)    10895 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/admin.py
+-rw-r--r--   0 root         (0) root         (0)    13673 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/api.py
+-rw-r--r--   0 root         (0) root         (0)     2451 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/cli/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/model_preparation/
+-rw-r--r--   0 root         (0) root         (0)    19613 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/gul_inputs.py
+-rw-r--r--   0 root         (0) root         (0)    42821 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/lookup.py
+-rw-r--r--   0 root         (0) root         (0)    46131 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/il_inputs.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33821 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/summaries.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/exposure_pre_analysis.py
+-rw-r--r--   0 root         (0) root         (0)     3261 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/computation_step.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/utils.py
+-rw-r--r--   0 root         (0) root         (0)    39561 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/reinsurance_layer.py
+-rw-r--r--   0 root         (0) root         (0)    18062 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_preparation/oed.py
+-rw-r--r--   0 root         (0) root         (0)       22 2020-08-18 16:22:54.000000 oasislmf-1.9.1/oasislmf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7821 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/api/session.py
+-rw-r--r--   0 root         (0) root         (0)    26368 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/api/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/_data/
+-rw-r--r--   0 root         (0) root         (0)    15647 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/calc_rules.csv
+-rw-r--r--   0 root         (0) root         (0)    14607 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/default_loc_profile.json
+-rw-r--r--   0 root         (0) root         (0)     2901 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/default_fm_agg_profile.json
+-rw-r--r--   0 root         (0) root         (0)    23493 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/default_combined_exposure_profile.json
+-rw-r--r--   0 root         (0) root         (0)    42756 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/acc_dtypes.json
+-rw-r--r--   0 root         (0) root         (0)     3038 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/default_step_policies_profile.json
+-rw-r--r--   0 root         (0) root         (0)     1747 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/analysis_settings.json
+-rw-r--r--   0 root         (0) root         (0)     7104 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/info_dtypes.json
+-rw-r--r--   0 root         (0) root         (0)    44477 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/loc_dtypes.json
+-rw-r--r--   0 root         (0) root         (0)      457 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/cookiecutter.json
+-rw-r--r--   0 root         (0) root         (0)     2297 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/calc_rules_step.csv
+-rw-r--r--   0 root         (0) root         (0)     1095 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/default_fm_profile_field_values.json
+-rw-r--r--   0 root         (0) root         (0)     5200 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/default_acc_profile.json
+-rw-r--r--   0 root         (0) root         (0)     3299 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/scope_dtypes.json
+-rw-r--r--   0 root         (0) root         (0)     3265 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/_data/config_compatibility_profile.json
+-rw-r--r--   0 root         (0) root         (0)    46186 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/model_execution/
+-rw-r--r--   0 root         (0) root         (0)    49980 2020-08-18 16:22:54.000000 oasislmf-1.9.1/oasislmf/model_execution/bash.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1254 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/complex_items_to_bin.py
+-rw-r--r--   0 root         (0) root         (0)    16409 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/bin.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/files.py
+-rw-r--r--   0 root         (0) root         (0)     3656 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/runner.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/conf.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/model_execution/complex_items_to_csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf/schema/
+-rw-r--r--   0 root         (0) root         (0)    11504 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/schema/analysis_settings.json
+-rw-r--r--   0 root         (0) root         (0)     4871 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/schema/example_model_settings.json
+-rw-r--r--   0 root         (0) root         (0)    33988 2020-08-18 16:22:53.000000 oasislmf-1.9.1/oasislmf/schema/model_settings.json
+-rw-r--r--   0 root         (0) root         (0)    12509 2020-08-18 16:22:53.000000 oasislmf-1.9.1/setup.py
+-rw-r--r--   0 root         (0) root         (0)    10834 2020-08-18 16:24:35.000000 oasislmf-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1530 2020-08-18 16:22:53.000000 oasislmf-1.9.1/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/bin/
+-rwxr-xr-x   0 root         (0) root         (0)     5844 2020-08-18 16:22:53.000000 oasislmf-1.9.1/bin/completer_oasislmf
+-rwxr-xr-x   0 root         (0) root         (0)      125 2020-08-18 16:22:53.000000 oasislmf-1.9.1/bin/oasislmf
+-rwxr-xr-x   0 root         (0) root         (0)      962 2020-08-18 16:22:53.000000 oasislmf-1.9.1/bin/ktools_monitor.sh
+-rw-r--r--   0 root         (0) root         (0)    19734 2020-08-18 16:22:54.000000 oasislmf-1.9.1/CHANGELOG.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      161 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)    10834 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        9 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      281 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     2680 2020-08-18 16:24:35.000000 oasislmf-1.9.1/oasislmf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      281 2020-08-18 16:22:53.000000 oasislmf-1.9.1/requirements-package.in
+-rw-r--r--   0 root         (0) root         (0)     8718 2020-08-18 16:22:53.000000 oasislmf-1.9.1/README.md
```

### Comparing `oasislmf-1.9.0/oasislmf/utils/defaults.py` & `oasislmf-1.9.1/oasislmf/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/log.py` & `oasislmf-1.9.1/oasislmf/utils/log.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/diff.py` & `oasislmf-1.9.1/oasislmf/utils/diff.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/compress.py` & `oasislmf-1.9.1/oasislmf/utils/compress.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/status.py` & `oasislmf-1.9.1/oasislmf/utils/status.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/profiles.py` & `oasislmf-1.9.1/oasislmf/utils/profiles.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/path.py` & `oasislmf-1.9.1/oasislmf/utils/path.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/deterministic_loss.py` & `oasislmf-1.9.1/oasislmf/utils/deterministic_loss.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/calc_rules.py` & `oasislmf-1.9.1/oasislmf/utils/calc_rules.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/fm.py` & `oasislmf-1.9.1/oasislmf/utils/fm.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/coverages.py` & `oasislmf-1.9.1/oasislmf/utils/coverages.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/exceptions.py` & `oasislmf-1.9.1/oasislmf/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/peril.py` & `oasislmf-1.9.1/oasislmf/utils/peril.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/utils/data.py` & `oasislmf-1.9.1/oasislmf/utils/data.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_testing/validation.py` & `oasislmf-1.9.1/oasislmf/model_testing/validation.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/cleaners.py` & `oasislmf-1.9.1/oasislmf/cli/cleaners.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/computation_command.py` & `oasislmf-1.9.1/oasislmf/cli/computation_command.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/test.py` & `oasislmf-1.9.1/oasislmf/cli/test.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/exposure.py` & `oasislmf-1.9.1/oasislmf/cli/exposure.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/config.py` & `oasislmf-1.9.1/oasislmf/cli/config.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/inputs.py` & `oasislmf-1.9.1/oasislmf/cli/inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/model.py` & `oasislmf-1.9.1/oasislmf/cli/model.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/root.py` & `oasislmf-1.9.1/oasislmf/cli/root.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/admin.py` & `oasislmf-1.9.1/oasislmf/cli/admin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/api.py` & `oasislmf-1.9.1/oasislmf/cli/api.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/cli/base.py` & `oasislmf-1.9.1/oasislmf/cli/base.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/gul_inputs.py` & `oasislmf-1.9.1/oasislmf/model_preparation/gul_inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/lookup.py` & `oasislmf-1.9.1/oasislmf/model_preparation/lookup.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/il_inputs.py` & `oasislmf-1.9.1/oasislmf/model_preparation/il_inputs.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/summaries.py` & `oasislmf-1.9.1/oasislmf/model_preparation/summaries.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/exposure_pre_analysis.py` & `oasislmf-1.9.1/oasislmf/model_preparation/exposure_pre_analysis.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/computation_step.py` & `oasislmf-1.9.1/oasislmf/model_preparation/computation_step.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/utils.py` & `oasislmf-1.9.1/oasislmf/model_preparation/utils.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/reinsurance_layer.py` & `oasislmf-1.9.1/oasislmf/model_preparation/reinsurance_layer.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_preparation/oed.py` & `oasislmf-1.9.1/oasislmf/model_preparation/oed.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/api/session.py` & `oasislmf-1.9.1/oasislmf/api/session.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/api/client.py` & `oasislmf-1.9.1/oasislmf/api/client.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/calc_rules.csv` & `oasislmf-1.9.1/oasislmf/_data/calc_rules.csv`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/default_loc_profile.json` & `oasislmf-1.9.1/oasislmf/_data/default_loc_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/default_fm_agg_profile.json` & `oasislmf-1.9.1/oasislmf/_data/default_fm_agg_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/default_combined_exposure_profile.json` & `oasislmf-1.9.1/oasislmf/_data/default_combined_exposure_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/acc_dtypes.json` & `oasislmf-1.9.1/oasislmf/_data/acc_dtypes.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/default_step_policies_profile.json` & `oasislmf-1.9.1/oasislmf/_data/default_step_policies_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/analysis_settings.json` & `oasislmf-1.9.1/oasislmf/_data/analysis_settings.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/info_dtypes.json` & `oasislmf-1.9.1/oasislmf/_data/info_dtypes.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/loc_dtypes.json` & `oasislmf-1.9.1/oasislmf/_data/loc_dtypes.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/calc_rules_step.csv` & `oasislmf-1.9.1/oasislmf/_data/calc_rules_step.csv`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/default_fm_profile_field_values.json` & `oasislmf-1.9.1/oasislmf/_data/default_fm_profile_field_values.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/default_acc_profile.json` & `oasislmf-1.9.1/oasislmf/_data/default_acc_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/scope_dtypes.json` & `oasislmf-1.9.1/oasislmf/_data/scope_dtypes.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/_data/config_compatibility_profile.json` & `oasislmf-1.9.1/oasislmf/_data/config_compatibility_profile.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/manager.py` & `oasislmf-1.9.1/oasislmf/manager.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/bash.py` & `oasislmf-1.9.1/oasislmf/model_execution/bash.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import copy
 import io
 import os
 import random
 import re
 import string
 
 from collections import Counter
@@ -110,14 +111,29 @@
 
 def do_fifos_exec(runtype, max_process_id, filename, fifo_dir, action='mkfifo'):
     for process_id in range(1, max_process_id + 1):
         print_command(filename, '{} {}{}_P{}'.format(action, fifo_dir, runtype, process_id))
     print_command(filename, '')
 
 
+def do_fifos_exec_full_correlation(
+    runtype, max_process_id, filename, fifo_dir, action='mkfifo'
+):
+    for process_id in range(1, max_process_id + 1):
+        print_command(filename, '{} {}{}_sumcalc_P{}'.format(
+            action, fifo_dir, runtype, process_id
+        ))
+    print_command(filename, '')
+    for process_id in range(1, max_process_id + 1):
+        print_command(filename, '{} {}{}_fmcalc_P{}'.format(
+            action, fifo_dir, runtype, process_id
+        ))
+    print_command(filename, '')
+
+
 def do_fifos_calc(runtype, analysis_settings, max_process_id,
                   filename, fifo_dir='fifo/', action='mkfifo'):
 
     summaries = analysis_settings.get('{}_summaries'.format(runtype))
     if not summaries:
         return
 
@@ -255,14 +271,15 @@
     analysis_settings,
     process_id,
     filename,
     fifo_dir='fifo/',
     stderr_guard=True,
     num_reinsurance_iterations=0,
     gul_legacy_stream=None,
+    gul_full_correlation=False
 ):
 
     summaries = analysis_settings.get('{}_summaries'.format(runtype))
     if not summaries:
         return
 
     if process_id == 1:
@@ -278,21 +295,27 @@
             summarycalc_switch = '-i'
 
     summarycalc_directory_switch = ""
     if runtype == RUNTYPE_REINSURANCE_LOSS:
         i = num_reinsurance_iterations
         summarycalc_directory_switch = "-p RI_{0}".format(i)
 
+    input_filename_component = ''
+    if gul_full_correlation:
+        input_filename_component = '_sumcalc'
+
     cmd = 'summarycalc {} {}'.format(summarycalc_switch, summarycalc_directory_switch)
     for summary in summaries:
         if 'id' in summary:
             summary_set = summary['id']
             cmd = '{0} -{1} {4}{2}_S{1}_summary_P{3}'.format(cmd, summary_set, runtype, process_id, fifo_dir)
 
-    cmd = '{0} < {1}{2}_P{3}'.format(cmd, fifo_dir, runtype, process_id)
+    cmd = '{0} < {1}{2}{3}_P{4}'.format(
+        cmd, fifo_dir, runtype, input_filename_component, process_id
+    )
     cmd = '( {0} ) 2>> log/stderror.err  &'.format(cmd) if stderr_guard else '{0} &'.format(cmd)      # Wrap in subshell and pipe stderr to file
     print_command(filename, cmd)
 
 
 def do_tees(runtype, analysis_settings, process_id, filename, process_counter, fifo_dir='fifo/', work_dir='work/'):
     summaries = analysis_settings.get('{}_summaries'.format(runtype))
     if not summaries:
@@ -322,14 +345,48 @@
             if summary.get('lec_output') and leccalc_enabled(summary['leccalc']):
                 cmd = '{} {}{}_S{}_summaryleccalc/P{}.bin'.format(cmd, work_dir, runtype, summary_set, process_id)
 
             cmd = '{} > /dev/null & pid{}=$!'.format(cmd, process_counter['pid_monitor_count'])
             print_command(filename, cmd)
 
 
+def do_tees_fc_sumcalc_fmcalc(process_id, filename, correlated_output_stems):
+
+    if process_id == 1:
+        print_command(filename, '')
+
+    cmd = 'tee < {0}{1}'.format(
+        correlated_output_stems['gulcalc_output'], process_id
+    )
+    cmd = '{0} {1}{3} {2}{3} > /dev/null &'.format(
+        cmd,
+        correlated_output_stems['sumcalc_input'], 
+        correlated_output_stems['fmcalc_input'],
+        process_id
+    )
+
+    print_command(filename, cmd)
+
+
+def get_correlated_output_stems(fifo_dir):
+
+    correlated_output_stems = {}
+    correlated_output_stems['gulcalc_output'] = '{0}{1}_P'.format(
+        fifo_dir, RUNTYPE_GROUNDUP_LOSS
+    )
+    correlated_output_stems['fmcalc_input'] = '{0}{1}_fmcalc_P'.format(
+        fifo_dir, RUNTYPE_GROUNDUP_LOSS
+    )
+    correlated_output_stems['sumcalc_input'] = '{0}{1}_sumcalc_P'.format(
+        fifo_dir, RUNTYPE_GROUNDUP_LOSS
+    )
+
+    return correlated_output_stems
+
+
 def do_any(runtype, analysis_settings, process_id, filename, process_counter, fifo_dir='fifo/', work_dir='work/'):
     summaries = analysis_settings.get('{}_summaries'.format(runtype))
     if not summaries:
         return
 
     if process_id == 1:
         print_command(filename, '')
@@ -417,18 +474,16 @@
 def do_gul(
     analysis_settings,
     max_process_id,
     filename,
     process_counter,
     fifo_dir='fifo/',
     work_dir='work/',
-    gul_alloc_rule=None,
     gul_legacy_stream=None,
-    stderr_guard=True,
-    full_correlation=False
+    stderr_guard=True
 ):
 
     for process_id in range(1, max_process_id + 1):
         do_any(RUNTYPE_GROUNDUP_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir)
 
     for process_id in range(1, max_process_id + 1):
         do_tees(RUNTYPE_GROUNDUP_LOSS, analysis_settings, process_id, filename, process_counter, fifo_dir, work_dir)
@@ -441,14 +496,40 @@
             filename=filename,
             gul_legacy_stream=gul_legacy_stream,
             fifo_dir=fifo_dir,
             stderr_guard=stderr_guard
         )
 
 
+def do_gul_full_correlation(
+    analysis_settings,
+    max_process_id,
+    filename,
+    process_counter,
+    fifo_dir='fifo/full_correlation/',
+    work_dir='work/full_correlation/',
+    gul_legacy_stream=None,
+    stderr_guard=None
+):
+
+    for process_id in range(1, max_process_id + 1):
+        do_any(
+            RUNTYPE_GROUNDUP_LOSS, analysis_settings, process_id, filename,
+            process_counter, fifo_dir, work_dir
+        )
+
+    for process_id in range(1, max_process_id + 1):
+        do_tees(
+            RUNTYPE_GROUNDUP_LOSS, analysis_settings, process_id, filename,
+            process_counter, fifo_dir, work_dir
+        )
+
+    print_command(filename, '')
+
+
 def do_waits(wait_variable, wait_count, filename):
     """
     Add waits to the script
 
     :param wait_variable: The type of wait
     :type wait_variable: str
 
@@ -491,21 +572,14 @@
 def do_kwaits(filename, process_counter):
     """
     Add kwaits to the script
     """
     do_waits('kpid', process_counter['kpid_monitor_count'], filename)
 
 
-def do_fcwaits(filename, process_counter):
-    """
-    Add fcwaits to the script
-    """
-    do_waits('fcpid', process_counter['fcpid_monitor_count'], filename)
-
-
 def get_getmodel_itm_cmd(
         number_of_samples, gul_threshold, use_random_number_file,
         gul_alloc_rule, item_output,
         process_id, max_process_id, correlated_output, **kwargs):
     """
     Gets the getmodel ktools command (3.1.0+) Gulcalc item stream
     :param number_of_samples: The number of samples to run
@@ -569,16 +643,15 @@
     process_id,
     il_output,
     il_alloc_rule,
     ri_alloc_rule,
     num_reinsurance_iterations,
     fifo_dir='fifo/',
     stderr_guard=True,
-    full_correlation=False,
-    process_counter=None
+    full_correlation=False
 ):
     """
     Gets the fmcalc ktools command reinsurance stream
     :param cmd: either gulcalc command stream or correlated output file
     :type cmd: str
     :param process_id: ID corresponding to thread
     :type process_id: int
@@ -613,31 +686,25 @@
     for i in range(1, num_reinsurance_iterations + 1):
         main_cmd = "{0} | fmcalc -a{2} -n -p RI_{1}".format(
             main_cmd, i, ri_alloc_rule
         )
 
     main_cmd = "{0} > {1}ri_P{2}".format(main_cmd, fifo_dir, process_id)
     main_cmd = '( {0} ) 2>> log/stderror.err &'.format(main_cmd) if stderr_guard else '{0} &'.format(main_cmd)
-    if full_correlation:
-        process_counter['fcpid_monitor_count'] += 1
-        main_cmd = '{0} fcpid{1}=$!'.format(
-            main_cmd, process_counter['fcpid_monitor_count']
-        )
 
     return main_cmd
 
 
 def get_main_cmd_il_stream(
     cmd,
     process_id,
     il_alloc_rule,
     fifo_dir='fifo/',
     stderr_guard=True,
-    full_correlation=False,
-    process_counter=None
+    full_correlation=False
 ):
     """
     Gets the fmcalc ktools command insured losses stream
     :param cmd: either gulcalc command stream or correlated output file
     :type cmd: str
     :param process_id: ID corresponding to thread
     :type process_id: int
@@ -656,19 +723,14 @@
 
     if full_correlation:
         fm_cmd = 'fmcalc -a{2} < {1} > {3}il_P{0}'
     else:
         fm_cmd = '{1} | fmcalc -a{2} > {3}il_P{0} '
     main_cmd = fm_cmd.format(process_id, cmd, il_alloc_rule, fifo_dir)
     main_cmd = '( {0} ) 2>> log/stderror.err &'.format(main_cmd) if stderr_guard else '{0} &'.format(main_cmd)
-    if full_correlation:
-        process_counter['fcpid_monitor_count'] += 1
-        main_cmd = '{0} fcpid{1}=$!'.format(
-            main_cmd, process_counter['fcpid_monitor_count']
-        )
 
     return main_cmd
 
 
 def get_main_cmd_gul_stream(
     cmd,
     process_id,
@@ -790,14 +852,20 @@
             full_correlation = analysis_settings['full_correlation']
 
     # Output depends on being enabled AND having at lease one summaries section
     gul_output = analysis_settings.get('gul_output', False) and (len(analysis_settings.get('gul_summaries', [])) > 0)
     il_output = analysis_settings.get('il_output', False) and (len(analysis_settings.get('il_summaries', [])) > 0)
     ri_output = analysis_settings.get('ri_output', False) and (len(analysis_settings.get('ri_summaries', [])) > 0)
 
+    # Determine whether GUL output only
+    # This is used for full correlation
+    gul_output_only = False
+    if gul_output and not il_output and not ri_output:
+        gul_output_only = True
+
     print_command(filename, '#!/bin/bash')
     print_command(filename, 'SCRIPT=$(readlink -f "$0") && cd $(dirname "$SCRIPT")')
     print_command(filename, '')
 
     print_command(filename, '# --- Script Init ---')
     print_command(filename, '')
     print_command(filename, 'set -e')
@@ -926,14 +994,34 @@
     if ri_output:
         do_fifos_calc(RUNTYPE_REINSURANCE_LOSS, analysis_settings,
                       max_process_id, filename, fifo_queue_dir)
 
     # Create Full correlation FIFO
     if full_correlation:
         if gul_output:
+            do_fifos_exec(
+                RUNTYPE_GROUNDUP_LOSS, max_process_id, filename,
+                fifo_full_correlation_dir
+            )
+            if not gul_output_only:
+                do_fifos_exec_full_correlation(
+                    RUNTYPE_GROUNDUP_LOSS, max_process_id, filename,
+                    fifo_full_correlation_dir
+                )
+        if il_output:
+            do_fifos_exec(
+                RUNTYPE_INSURED_LOSS, max_process_id, filename,
+                fifo_full_correlation_dir
+            )
+        if ri_output:
+            do_fifos_exec(
+                RUNTYPE_REINSURANCE_LOSS, max_process_id, filename,
+                fifo_full_correlation_dir
+            )
+        if gul_output:
             do_fifos_calc(
                 RUNTYPE_GROUNDUP_LOSS, analysis_settings,
                 max_process_id, filename, fifo_full_correlation_dir
             )
         if il_output:
             do_fifos_calc(
                 RUNTYPE_INSURED_LOSS, analysis_settings,
@@ -959,14 +1047,19 @@
                 'num_reinsurance_iterations': num_reinsurance_iterations,
                 'fifo_dir': fifo_queue_dir,
                 'work_dir': work_dir,
                 'stderr_guard': stderr_guard
             }
         }
         compute_outputs.append(ri_computes)
+        if full_correlation:
+            ri_fc_computes = copy.deepcopy(ri_computes)
+            ri_fc_computes['compute_args']['fifo_dir'] = fifo_full_correlation_dir
+            ri_fc_computes['compute_args']['work_dir'] = work_full_correlation_dir
+            compute_outputs.append(ri_fc_computes)
 
     if il_output:
         il_computes = {
             'loss_type': 'insured',
             'compute_fun': il,
             'compute_args': {
                 'analysis_settings': analysis_settings,
@@ -975,43 +1068,116 @@
                 'process_counter': process_counter,
                 'fifo_dir': fifo_queue_dir,
                 'work_dir': work_dir,
                 'stderr_guard': stderr_guard
             }
         }
         compute_outputs.append(il_computes)
+        if full_correlation:
+            il_fc_computes = copy.deepcopy(il_computes)
+            il_fc_computes['compute_args']['fifo_dir'] = fifo_full_correlation_dir
+            il_fc_computes['compute_args']['work_dir'] = work_full_correlation_dir
+            compute_outputs.append(il_fc_computes)
 
     if gul_output:
         gul_computes = {
             'loss_type': 'ground up',
             'compute_fun': do_gul,
             'compute_args': {
                 'analysis_settings': analysis_settings,
                 'max_process_id': max_process_id,
                 'filename': filename,
                 'process_counter': process_counter,
                 'fifo_dir': fifo_queue_dir,
                 'work_dir': work_dir,
-                'gul_alloc_rule': gul_alloc_rule,
                 'gul_legacy_stream': gul_legacy_stream,
                 'stderr_guard': stderr_guard
             }
         }
         compute_outputs.append(gul_computes)
 
     do_computes(compute_outputs)
 
     print_command(filename, '')
 
+    if full_correlation:
+        correlated_output_stems = get_correlated_output_stems(
+            fifo_full_correlation_dir
+        )
+        if gul_output:
+            gul_fc_computes = copy.deepcopy(gul_computes)
+            gul_fc_computes['compute_args']['fifo_dir'] = fifo_full_correlation_dir
+            gul_fc_computes['compute_args']['work_dir'] = work_full_correlation_dir
+            do_gul_full_correlation(**gul_fc_computes['compute_args'])
+
+        for process_id in range(1, max_process_id + 1):
+            # Set up file name for full correlation file
+            correlated_output_file = '{0}{1}'.format(
+                correlated_output_stems['fmcalc_input'], process_id
+            )
+
+            if num_reinsurance_iterations > 0 and ri_output:
+                main_cmd = get_main_cmd_ri_stream(
+                    correlated_output_file,
+                    process_id,
+                    il_output,
+                    il_alloc_rule,
+                    ri_alloc_rule,
+                    num_reinsurance_iterations,
+                    fifo_full_correlation_dir,
+                    stderr_guard,
+                    full_correlation
+                )
+
+                print_command(filename, main_cmd)
+            elif gul_output and il_output:
+                main_cmd = get_main_cmd_il_stream(
+                    correlated_output_file, process_id, il_alloc_rule,
+                    fifo_full_correlation_dir, stderr_guard, full_correlation
+                )
+                print_command(filename, main_cmd)
+            else:
+                if il_output and 'il_summaries' in analysis_settings:
+
+                    main_cmd = get_main_cmd_il_stream(
+                        correlated_output_file, process_id, il_alloc_rule,
+                        fifo_full_correlation_dir, stderr_guard,
+                        full_correlation
+                    )
+                    print_command(filename, main_cmd)
+
+        gul_full_correlation = True
+        if gul_output_only:
+            gul_full_correlation = False
+        for process_id in range(1, max_process_id + 1):
+            do_summarycalcs(
+                runtype=RUNTYPE_GROUNDUP_LOSS,
+                analysis_settings=analysis_settings,
+                process_id=process_id,
+                filename=filename,
+                gul_legacy_stream=gul_legacy_stream,
+                fifo_dir=fifo_full_correlation_dir,
+                stderr_guard=stderr_guard,
+                gul_full_correlation=gul_full_correlation
+            )
+
+        if not gul_output_only:
+            for process_id in range(1, max_process_id + 1):
+                do_tees_fc_sumcalc_fmcalc(
+                    process_id, filename, correlated_output_stems
+                )
+
+        print_command(filename, '')
+
+
     for process_id in range(1, max_process_id + 1):
         # gulcalc output file for fully correlated output
         if full_correlation:
-            correlated_output_file = '{0}gul_P{1}'.format(
-                fifo_full_correlation_dir,
-                process_id
+            correlated_output_file = '{0}{1}'.format(
+                correlated_output_stems['gulcalc_output'], process_id
             )
         else:
             correlated_output_file = ''
 
         getmodel_args = {
             'number_of_samples': number_of_samples,
             'gul_threshold': gul_threshold,
@@ -1089,121 +1255,14 @@
                 )
                 print_command(filename, main_cmd)
 
     print_command(filename, '')
 
     do_pwaits(filename, process_counter)
 
-    if full_correlation:
-        print_command(
-            filename, '# --- Do computes for fully correlated output ---'
-        )
-        print_command(filename, '')
-
-        for process_id in range(1, max_process_id + 1):
-            # Set up file name for full correlation file
-            correlated_output_file = '{0}gul_P{1}'.format(
-                fifo_full_correlation_dir,
-                process_id
-            )
-
-            if num_reinsurance_iterations > 0 and ri_output:
-                main_cmd = get_main_cmd_ri_stream(
-                    correlated_output_file,
-                    process_id,
-                    il_output,
-                    il_alloc_rule,
-                    ri_alloc_rule,
-                    num_reinsurance_iterations,
-                    fifo_full_correlation_dir,
-                    stderr_guard,
-                    full_correlation,
-                    process_counter
-                )
-
-                print_command(filename, main_cmd)
-            elif gul_output and il_output:
-                main_cmd = get_main_cmd_il_stream(
-                    correlated_output_file, process_id, il_alloc_rule,
-                    fifo_full_correlation_dir, stderr_guard, full_correlation,
-                    process_counter
-                )
-                print_command(filename, main_cmd)
-            else:
-                if il_output and 'il_summaries' in analysis_settings:
-
-                    main_cmd = get_main_cmd_il_stream(
-                        correlated_output_file, process_id, il_alloc_rule,
-                        fifo_full_correlation_dir, stderr_guard,
-                        full_correlation, process_counter
-                    )
-                    print_command(filename, main_cmd)
-
-        print_command(filename, '')
-
-        do_fcwaits(filename, process_counter)
-
-        process_counter['pid_monitor_count'] = 0
-        compute_outputs = []
-        if ri_output:
-            ri_computes = {
-                'loss_type': 'reinsurance',
-                'compute_fun': ri,
-                'compute_args': {
-                    'analysis_settings': analysis_settings,
-                    'max_process_id': max_process_id,
-                    'filename': filename,
-                    'process_counter': process_counter,
-                    'num_reinsurance_iterations': num_reinsurance_iterations,
-                    'fifo_dir': fifo_full_correlation_dir,
-                    'work_dir': work_full_correlation_dir,
-                    'stderr_guard': stderr_guard
-                }
-            }
-            compute_outputs.append(ri_computes)
-        if il_output:
-            il_computes = {
-                'loss_type': 'insured',
-                'compute_fun': il,
-                'compute_args': {
-                    'analysis_settings': analysis_settings,
-                    'max_process_id': max_process_id,
-                    'filename': filename,
-                    'process_counter': process_counter,
-                    'fifo_dir': fifo_full_correlation_dir,
-                    'work_dir': work_full_correlation_dir,
-                    'stderr_guard': stderr_guard
-                }
-            }
-            compute_outputs.append(il_computes)
-        if gul_output:
-            gul_computes = {
-                'loss_type': 'ground up',
-                'compute_fun': do_gul,
-                'compute_args': {
-                    'analysis_settings': analysis_settings,
-                    'max_process_id': max_process_id,
-                    'filename': filename,
-                    'process_counter': process_counter,
-                    'fifo_dir': fifo_full_correlation_dir,
-                    'work_dir': work_full_correlation_dir,
-                    'gul_alloc_rule': gul_alloc_rule,
-                    'gul_legacy_stream': gul_legacy_stream,
-                    'stderr_guard': stderr_guard,
-                    'full_correlation': full_correlation
-                }
-            }
-            compute_outputs.append(gul_computes)
-
-        do_computes(compute_outputs)
-
-        print_command(filename, '')
-
-        do_pwaits(filename, process_counter)
-
     if ri_output:
         print_command(filename, '')
         print_command(filename, '# --- Do reinsurance loss kats ---')
         print_command(filename, '')
         do_kats(
             RUNTYPE_REINSURANCE_LOSS, analysis_settings, max_process_id,
             filename, process_counter, work_kat_dir, output_dir
```

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/complex_items_to_bin.py` & `oasislmf-1.9.1/oasislmf/model_execution/complex_items_to_bin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/bin.py` & `oasislmf-1.9.1/oasislmf/model_execution/bin.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/files.py` & `oasislmf-1.9.1/oasislmf/model_execution/files.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/runner.py` & `oasislmf-1.9.1/oasislmf/model_execution/runner.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/conf.py` & `oasislmf-1.9.1/oasislmf/model_execution/conf.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/model_execution/complex_items_to_csv.py` & `oasislmf-1.9.1/oasislmf/model_execution/complex_items_to_csv.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/schema/analysis_settings.json` & `oasislmf-1.9.1/oasislmf/schema/analysis_settings.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/schema/example_model_settings.json` & `oasislmf-1.9.1/oasislmf/schema/example_model_settings.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/oasislmf/schema/model_settings.json` & `oasislmf-1.9.1/oasislmf/schema/model_settings.json`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/setup.py` & `oasislmf-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/PKG-INFO` & `oasislmf-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasislmf
-Version: 1.9.0
+Version: 1.9.1
 Summary: Core loss modelling framework.
 Home-page: https://github.com/OasisLMF/oasislmf
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: BSD 3-Clause
 Description: <img src="https://oasislmf.org/packages/oasis_theme_package/themes/oasis_theme/assets/src/oasis-lmf-colour.png" alt="Oasis LMF logo" width="250"/>
```

### Comparing `oasislmf-1.9.0/LICENSE` & `oasislmf-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/bin/completer_oasislmf` & `oasislmf-1.9.1/bin/completer_oasislmf`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/bin/ktools_monitor.sh` & `oasislmf-1.9.1/bin/ktools_monitor.sh`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/CHANGELOG.rst` & `oasislmf-1.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 OasisLMF Changelog
 ==================
 
-`1.9.0`_
+`1.9.1`_
 --------
 .. start_latest_release
+* [#630](https://github.com/OasisLMF/OasisLMF/issues/630) - full_correlation gulcalc option creates large output files.
+.. end_latest_release
+
+
+`1.9.0`_
+--------
 * [#566](https://github.com/OasisLMF/OasisLMF/issues/566) - Handle unlimited LayerLimit without large default value
 * [#574](https://github.com/OasisLMF/OasisLMF/issues/574) - Use LayerNumber to identify unique policy layers in gross fm file generation 
 * [#578](https://github.com/OasisLMF/OasisLMF/issues/578) - Added missing combination of terms in calcrules
 * [#603](https://github.com/OasisLMF/OasisLMF/issues/603) - Add type 2 financial terms tests for multi-peril to regression test
 * [PR 600](https://github.com/OasisLMF/OasisLMF/pull/600) - Added Scripts for generated example model data for testing.
-.. end_latest_release
 
 `1.8.3`_
 --------
 * [#601](https://github.com/OasisLMF/OasisLMF/issues/601) - Fix calculations for type 2 deductibles and limits in multi-peril models
 
 `1.8.2`_
 --------
@@ -419,14 +424,15 @@
   exposures manager generate keys error files by default
 
 `1.0.1`_ (beta)
 ---------------
 
 * Add console logging
 
+.. _`1.9.1`:  https://github.com/OasisLMF/OasisLMF/compare/1.9.0...1.9.1
 .. _`1.9.0`:  https://github.com/OasisLMF/OasisLMF/compare/1.8.3...1.9.0
 .. _`1.8.3`:  https://github.com/OasisLMF/OasisLMF/compare/1.8.2...1.8.3
 .. _`1.8.2`:  https://github.com/OasisLMF/OasisLMF/compare/1.8.1...1.8.2
 .. _`1.8.1`:  https://github.com/OasisLMF/OasisLMF/compare/1.8.0...1.8.1
 .. _`1.8.0`:  https://github.com/OasisLMF/OasisLMF/compare/1.7.1...1.8.0
 .. _`1.7.1`:  https://github.com/OasisLMF/OasisLMF/compare/1.7.0...1.7.1
 .. _`1.7.0`:  https://github.com/OasisLMF/OasisLMF/compare/1.6.0...1.7.0
```

### Comparing `oasislmf-1.9.0/oasislmf.egg-info/PKG-INFO` & `oasislmf-1.9.1/oasislmf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oasislmf
-Version: 1.9.0
+Version: 1.9.1
 Summary: Core loss modelling framework.
 Home-page: https://github.com/OasisLMF/oasislmf
 Author: Oasis LMF
 Author-email: support@oasislmf.org
 License: BSD 3-Clause
 Description: <img src="https://oasislmf.org/packages/oasis_theme_package/themes/oasis_theme/assets/src/oasis-lmf-colour.png" alt="Oasis LMF logo" width="250"/>
```

### Comparing `oasislmf-1.9.0/oasislmf.egg-info/SOURCES.txt` & `oasislmf-1.9.1/oasislmf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oasislmf-1.9.0/README.md` & `oasislmf-1.9.1/README.md`

 * *Files identical despite different names*

