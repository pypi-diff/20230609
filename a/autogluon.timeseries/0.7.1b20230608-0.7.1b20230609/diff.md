# Comparing `tmp/autogluon.timeseries-0.7.1b20230608.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230609.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230608.tar", last modified: Thu Jun  8 09:04:28 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230609.tar", last modified: Fri Jun  9 09:04:12 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230608.tar` & `autogluon.timeseries-0.7.1b20230609.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.094242 autogluon.timeseries-0.7.1b20230608/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-08 09:04:28.094242 autogluon.timeseries-0.7.1b20230608/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:04:28.094242 autogluon.timeseries-0.7.1b20230608/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.082242 autogluon.timeseries-0.7.1b20230608/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.082242 autogluon.timeseries-0.7.1b20230608/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.086242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.086242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.086242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.086242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.086242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16983 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
--rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9167 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12144 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    49496 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.090242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48286 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.094242 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-08 09:03:43.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 09:04:27.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:04:28.086242 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:04:28.000000 autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:04:12.162212 autogluon.timeseries-0.7.1b20230609/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37746 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10323 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19507 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17083 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14835 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5284 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18929 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22184 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18117 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9326 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15975 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11905 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49409 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48405 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3063 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.158212 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-09 09:03:31.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 09:04:11.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:04:12.154212 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12561 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:04:12.000000 autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230608/PKG-INFO` & `autogluon.timeseries-0.7.1b20230609/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230608
+Version: 0.7.1b20230609
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230608/setup.py` & `autogluon.timeseries-0.7.1b20230609/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,22 @@
 submodule = "timeseries"
 install_requires = [
     # version ranges added in ag.get_dependency_version_ranges()
     "joblib>=1.1,<2",
     "numpy",  # version range defined in `core/_setup_utils.py`
     "scipy",  # version range defined in `core/_setup_utils.py`
     "pandas",  # version range defined in `core/_setup_utils.py`
-    "statsmodels>=0.13.0,<0.14",
+    "statsmodels>=0.13.0,<0.15",
     "gluonts>=0.13.1,<0.14",
     "torch>=1.9,<1.14",
     "pytorch-lightning>=1.7.4,<1.10.0",
     "networkx",  # version range defined in `core/_setup_utils.py`
+    # TODO: update statsforecast to v1.5.0 - resolve antlr4-python3-runtime depedency clash with multimodal
     "statsforecast>=1.4.0,<1.5",
-    "mlforecast>=0.7.0,<0.8.0",
+    "mlforecast>=0.7.0,<0.7.4",
     "tqdm",  # version range defined in `core/_setup_utils.py`
     "ujson>=5,<6",  # needed to silence GluonTS warning
     f"autogluon.core[raytune]=={version}",
     f"autogluon.common=={version}",
     f"autogluon.tabular[catboost,lightgbm,xgboost]=={version}",
 ]
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 
 TIMESERIES_PRESETS_CONFIGS = dict(
     best_quality={
         "hyperparameters": "best_quality",
         "hyperparameter_tune_kwargs": {
             "scheduler": "local",
             "searcher": "auto",
-            "num_trials": 10,
+            "num_trials": 3,
         },
     },
     high_quality={"hyperparameters": "high_quality"},
     medium_quality={"hyperparameters": "medium_quality"},
-    fast_training={"hyperparameters": "local_only"},
+    fast_training={"hyperparameters": "fast_training"},
 )
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/direct_tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from gluonts.time_feature import get_lags_for_frequency, time_features_from_frequency_str
 from joblib.parallel import Parallel, delayed
 
 import autogluon.core as ag
 from autogluon.tabular import TabularPredictor
 from autogluon.timeseries.dataset.ts_dataframe import ITEMID, TIMESTAMP, TimeSeriesDataFrame
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
+from autogluon.timeseries.models.local.abstract_local_model import AG_DEFAULT_N_JOBS
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 
 logger = logging.getLogger(__name__)
 
 
 class DirectTabularModel(AbstractTimeSeriesModel):
     """Predict future time series values using autogluon.tabular.TabularPredictor.
@@ -215,15 +216,15 @@
             name: str,
         ):
             """Generate lag features for all time series in the dataset.
 
             See the docstring of get_lags for the description of the parameters.
             """
             # TODO: Expose n_jobs to the user as a hyperparameter
-            lags_per_item = Parallel(n_jobs=-1)(
+            lags_per_item = Parallel(n_jobs=AG_DEFAULT_N_JOBS)(
                 delayed(get_lags)(
                     ts,
                     lag_indices,
                     prediction_length=prediction_length,
                     max_rows_per_item=max_rows_per_item,
                     mask=mask,
                 )
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/autogluon_tabular/utils.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/autogluon_tabular/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/__init__.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,18 @@
 from autogluon.timeseries.utils.forecast import get_forecast_horizon_index_ts_dataframe
 from autogluon.timeseries.utils.seasonality import get_seasonality
 from autogluon.timeseries.utils.warning_filters import statsmodels_joblib_warning_filter, statsmodels_warning_filter
 
 logger = logging.getLogger(__name__)
 
 
+# We use the same default n_jobs across AG-TS to ensure that Joblib reuses the process pool
+AG_DEFAULT_N_JOBS = max(int(cpu_count() * 0.5), 1)
+
+
 class AbstractLocalModel(AbstractTimeSeriesModel):
     """Abstract class for local forecasting models that are trained separately for each time series.
 
     Prediction is parallelized across CPU cores using joblib.Parallel.
 
     Attributes
     ----------
@@ -32,15 +36,15 @@
         Default number of CPU cores used to train models. If float, this fraction of CPU cores will be used.
     init_time_in_seconds : int
         Time that it takes to initialize the model in seconds (e.g., because of JIT compilation by Numba).
         If time_limit is below this number, model won't be trained.
     """
 
     allowed_local_model_args: List[str] = []
-    default_n_jobs: Union[int, float] = 0.5
+    default_n_jobs: Union[int, float] = AG_DEFAULT_N_JOBS
     init_time_in_seconds: int = 0
 
     def __init__(
         self,
         freq: Optional[str] = None,
         prediction_length: int = 1,
         path: Optional[str] = None,
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/models/presets.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,26 +73,28 @@
         )
     )
 
 DEFAULT_MODEL_NAMES = {v: k for k, v in MODEL_TYPES.items()}
 DEFAULT_MODEL_PRIORITY = dict(
     Naive=100,
     SeasonalNaive=100,
-    ETS=90,
     Theta=90,
-    RecursiveTabular=80,
-    ARIMA=70,
-    DirectTabular=70,
+    AutoETS=80,
+    ETS=80,
+    RecursiveTabular=70,
     DeepAR=60,
     TemporalFusionTransformer=50,
-    SimpleFeedForward=40,
-    AutoARIMA=50,
-    AutoETS=70,
-    DynamicOptimizedTheta=60,
+    PatchTST=50,
+    DirectTabular=40,
+    AutoARIMA=30,
     # Models below are not included in any presets
+    ARIMA=30,
+    ThetaStatsmodels=90,
+    SimpleFeedForward=30,
+    DynamicOptimizedTheta=30,
     DeepARMXNet=50,
     SimpleFeedForwardMXNet=30,
     TemporalFusionTransformerMXNet=50,
     TransformerMXNet=30,
     MQCNNMXNet=10,
     MQRNNMXNet=10,
 )
@@ -103,71 +105,61 @@
     "name_prefix",
     "name_suffix",
 }
 
 
 def get_default_hps(key):
     default_model_hps = {
-        "local_only": {
+        "fast_training": {
             "Naive": {},
             "SeasonalNaive": {},
-            "ARIMA": {},
             "ETS": {},
             "Theta": {},
             "RecursiveTabular": {"max_num_samples": 100_000},
         },
         "medium_quality": {
             "Naive": {},
             "SeasonalNaive": {},
-            "ARIMA": {},
-            "ETS": {},
             "AutoETS": {},
             "Theta": {},
             "RecursiveTabular": {},
-            "DirectTabular": {},
             "DeepAR": {},
         },
         "high_quality": {
             "Naive": {},
             "SeasonalNaive": {},
-            "ARIMA": {},
-            "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
             "Theta": {},
             "RecursiveTabular": {},
             "DirectTabular": {},
             "DeepAR": {},
-            "SimpleFeedForward": {},
             "TemporalFusionTransformer": {},
+            "PatchTST": {},
         },
         "best_quality": {
             "Naive": {},
             "SeasonalNaive": {},
-            "ARIMA": {},
-            "ETS": {},
             "AutoETS": {},
             "AutoARIMA": {},
-            "DynamicOptimizedTheta": {},
             "Theta": {},
+            # TODO: Define separate model for each tabular submodel?
             "RecursiveTabular": {
                 "tabular_hyperparameters": {
                     "NN_TORCH": {"proc.impute_strategy": "constant"},
                     "GBM": [{}, {"extra_trees": True, "ag_args": {"name_suffix": "XT"}}],
                 },
             },
             "DirectTabular": {},
+            "TemporalFusionTransformer": {},
+            "PatchTST": {},
             "DeepAR": {
                 "num_layers": space.Int(1, 3, default=2),
                 "hidden_size": space.Int(40, 80, default=40),
             },
-            "SimpleFeedForward": {
-                "hidden_dimensions": space.Categorical([40], [40, 40], [120]),
-            },
-            "TemporalFusionTransformer": {},
         },
     }
 
     # For backwards compatibility
     default_model_hps["default"] = default_model_hps["medium_quality"]
     default_model_hps["default_hpo"] = default_model_hps["best_quality"]
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,18 +358,18 @@
             to get a high-accuracy predictor, or set ``presets="fast_training"`` to quickly fit multiple simple
             statistical models.
             Any user-specified arguments in :meth:`~autogluon.timeseries.TimeSeriesPredictor.fit` will
             override the values used by presets.
 
             Available presets:
 
-            - ``"fast_training"``: fit simple "local" statistical models (``ETS``, ``ARIMA``, ``Theta``, ``Naive``, ``SeasonalNaive``). These models are fast to train, but cannot capture more complex patterns in the data.
-            - ``"medium_quality"``: all models mentioned above + tree-based model ``DirectTabular`` + deep learning model ``DeepAR``. Default setting that produces good forecasts with reasonable training time.
-            - ``"high_quality"``: all models mentioned above + hyperparameter optimization for local statistical models + deep learning models ``TemporalFusionTransformerMXNet`` (if MXNet is available) and ``SimpleFeedForward``. Usually more accurate than ``medium_quality``, but takes longer to train.
-            - ``"best_quality"``: all models mentioned above + deep learning model ``TransformerMXNet`` (if MXNet is available) + hyperparameter optimization for deep learning models. Usually better than ``high_quality``, but takes much longer to train.
+            - ``"fast_training"``: fit simple statistical models (``ETS``, ``Theta``, ``Naive``, ``SeasonalNaive``) + fast tree-based model ``RecursiveTabular``. These models are fast to train but may not be very accurate.
+            - ``"medium_quality"``: all models mentioned above + deep learning model ``DeepAR``. Default setting that produces good forecasts with reasonable training time.
+            - ``"high_quality"``: all models mentioned above + automatically tuned statistical models (``AutoETS``, ``AutoARIMA``) + tree-based model ``DirectTabular`` + deep learning models ``TemporalFusionTransformer`` and ``PatchTST`` . Much more accurate than ``medium_quality``, but takes longer to train.
+            - ``"best_quality"``: all models mentioned above + more tabular models + training multiple copies of ``DeepAR``. Usually better than ``high_quality``, but takes even longer to train.
 
             Details for these presets can be found in ``autogluon/timeseries/configs/presets_configs.py``. If not
             provided, user-provided values for ``hyperparameters`` and ``hyperparameter_tune_kwargs`` will be used
             (defaulting to their default values specified below).
         hyperparameters : str or dict, default = "medium_quality"
             Determines what models are trained and what hyperparameters are used by each model.
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 import networkx as nx
 import pandas as pd
 from tqdm import tqdm
 
 from autogluon.common.utils.log_utils import set_logger_verbosity
+from autogluon.common.utils.path_converter import PathConverter
 from autogluon.common.utils.utils import hash_pandas_df
 from autogluon.core.models import AbstractModel
 from autogluon.core.utils.exceptions import TimeLimitExceeded
 from autogluon.core.utils.loaders import load_pkl
 from autogluon.core.utils.savers import save_json, save_pkl
 from autogluon.timeseries import TimeSeriesDataFrame, TimeSeriesEvaluator
 from autogluon.timeseries.models.abstract import AbstractTimeSeriesModel
@@ -34,14 +35,15 @@
 class SimpleAbstractTrainer:
     trainer_file_name = "trainer.pkl"
     trainer_info_name = "info.pkl"
     trainer_info_json_name = "info.json"
 
     def __init__(self, path: str, low_memory: bool, save_data: bool, *args, **kwargs):
         self.path = path
+        self.path = PathConverter.to_relative(self.path)
         self.reset_paths = False
 
         self.low_memory = low_memory
         self.save_data = save_data
 
         self.models = {}
         self.model_graph = nx.DiGraph()
@@ -537,15 +539,14 @@
         hyperparameters: Optional[Union[str, Dict]] = None,
         models: Optional[List[AbstractTimeSeriesModel]] = None,
         val_data: Optional[TimeSeriesDataFrame] = None,
         hyperparameter_tune_kwargs: Optional[Union[str, dict]] = None,
         excluded_model_types: Optional[List[str]] = None,
         time_limit: Optional[float] = None,
     ) -> List[str]:
-
         logger.info(f"\nStarting training. Start time is {time.strftime('%Y-%m-%d %H:%M:%S')}")
 
         time_start = time.time()
         if hyperparameters is not None:
             hyperparameters = copy.deepcopy(hyperparameters)
         else:
             if models is None:
@@ -1042,15 +1043,14 @@
 
     def refit_single_full(
         self,
         train_data: Optional[TimeSeriesDataFrame] = None,
         val_data: Optional[TimeSeriesDataFrame] = None,
         models: List[str] = None,
     ) -> List[str]:
-
         train_data = train_data or self.load_train_data()
         val_data = val_data or self.load_val_data()
         refit_full_data = self._merge_refit_full_data(train_data, val_data)
 
         if models is None:
             models = self.get_model_names()
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         Parameters
         ----------
         train_data: TimeSeriesDataFrame
             Training data for fitting time series timeseries models.
         hyperparameters: str or Dict
             A dictionary mapping selected model names, model classes or model factory to hyperparameter
             settings. Model names should be present in `trainer.presets.DEFAULT_MODEL_NAMES`. Optionally,
-            the user may provide one of "local_only", "default", "default_hpo" to specify presets.
+            the user may provide one of "fast_training", "default", "default_hpo" to specify presets.
         val_data: TimeSeriesDataFrame
             Optional validation data set to report validation scores on.
         hyperparameter_tune_kwargs
             Args for hyperparameter tuning
         excluded_model_types
             Names of models that should not be trained, even if listed in `hyperparameters`.
         time_limit
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230609/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230608
+Version: 0.7.1b20230609
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230608/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230609/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

