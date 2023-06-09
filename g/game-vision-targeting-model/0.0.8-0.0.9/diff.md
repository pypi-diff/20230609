# Comparing `tmp/game-vision-targeting-model-0.0.8.tar.gz` & `tmp/game-vision-targeting-model-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-vision-targeting-model-0.0.8.tar", last modified: Fri Jun  9 19:04:11 2023, max compression
+gzip compressed data, was "game-vision-targeting-model-0.0.9.tar", last modified: Fri Jun  9 19:32:01 2023, max compression
```

## Comparing `game-vision-targeting-model-0.0.8.tar` & `game-vision-targeting-model-0.0.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.747437 game-vision-targeting-model-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/License.md
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-09 19:04:11.743437 game-vision-targeting-model-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/docs/License.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/docs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:04:11.747437 game-vision-targeting-model-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.735437 game-vision-targeting-model-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.739437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.743437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.743437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/singletons/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/singletons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/singletons/singletons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.743437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/tests/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/tests/map_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/tests/pytest_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.743437 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/model_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/normalise_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:03:58.000000 game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/training_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:04:11.743437 game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-09 19:04:11.000000 game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-09 19:04:11.000000 game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:04:11.000000 game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 19:04:11.000000 game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 19:04:11.000000 game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/docs/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/docs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.884498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/singletons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/singletons/singletons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/tests/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/tests/map_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/tests/pytest_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/normalise_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 19:31:49.000000 game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/training_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 19:32:01.888498 game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-09 19:32:01.000000 game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-06-09 19:32:01.000000 game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 19:32:01.000000 game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 19:32:01.000000 game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 19:32:01.000000 game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/top_level.txt
```

### Comparing `game-vision-targeting-model-0.0.8/License.md` & `game-vision-targeting-model-0.0.9/License.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/PKG-INFO` & `game-vision-targeting-model-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-vision-targeting-model
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
 License: Copyright 2023 Kent Vejrup Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
```

### Comparing `game-vision-targeting-model-0.0.8/Readme.md` & `game-vision-targeting-model-0.0.9/Readme.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/docs/License.md` & `game-vision-targeting-model-0.0.9/docs/License.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/pyproject.toml` & `game-vision-targeting-model-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "game-vision-targeting-model"
-version = "0.0.8"
+version = "0.0.9"
 
 authors = [
   { name="Kent vejrup Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
 
 description = "A small example package"
 readme = "Readme.md"
```

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/layers.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/layers.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from keras.models \
     import Sequential
 
-from tensorflow import compat, get_logger
+from tensorflow \
+    import get_logger
 
 from GameVisionTargetingModel.models.classification.map.v1.layers \
     import generate_layers_for_map_classifier_v1
 
 from keras.losses \
     import SparseCategoricalCrossentropy
 
@@ -15,15 +16,14 @@
     SparseCategoricalAccuracy
 
 from logging \
     import ERROR
 
 
 def tensorflow_settings():
-    compat.v1.disable_eager_execution()
     get_logger().setLevel(
         ERROR
     )
 
 
 class MapClassifier(
     Sequential
```

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/setup_package.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/setup_package.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/singletons/singletons.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/singletons/singletons.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/tests/configuration_test.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/tests/configuration_test.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/__init__.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/GameVisionTargetingModel/variables/model_settings.py` & `game-vision-targeting-model-0.0.9/src/GameVisionTargetingModel/variables/model_settings.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/PKG-INFO` & `game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-vision-targeting-model
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small example package
 Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
 License: Copyright 2023 Kent Vejrup Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
```

### Comparing `game-vision-targeting-model-0.0.8/src/game_vision_targeting_model.egg-info/SOURCES.txt` & `game-vision-targeting-model-0.0.9/src/game_vision_targeting_model.egg-info/SOURCES.txt`

 * *Files identical despite different names*

