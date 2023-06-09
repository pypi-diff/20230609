# Comparing `tmp/game-vision-targeting-model-0.0.6.tar.gz` & `tmp/game-vision-targeting-model-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-vision-targeting-model-0.0.6.tar", last modified: Fri Jun  9 17:38:21 2023, max compression
+gzip compressed data, was "game-vision-targeting-model-0.0.7.tar", last modified: Fri Jun  9 17:59:05 2023, max compression
```

## Comparing `game-vision-targeting-model-0.0.6.tar` & `game-vision-targeting-model-0.0.7.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/Changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/singletons/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/singletons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/singletons/singletons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/map_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/pytest_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/model_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/normalise_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/training_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/License.md
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/docs/License.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/docs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.825696 game-vision-targeting-model-0.0.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/docs/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/docs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.821696 game-vision-targeting-model-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.825696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.825696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.825696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.825696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.829696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.829696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.829696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/singletons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/singletons/singletons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/tests/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/tests/map_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/tests/pytest_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/normalise_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:58:51.000000 game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/training_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:59:05.833696 game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-09 17:59:05.000000 game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-09 17:59:05.000000 game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:59:05.000000 game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 17:59:05.000000 game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 17:59:05.000000 game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/top_level.txt
```

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/PKG-INFO` & `game-vision-targeting-model-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-vision-targeting-model
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
 License: Copyright 2023 Kent Vejrup Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
@@ -20,17 +20,20 @@
 Project-URL: Changelog, https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/Changelog.md
 Project-URL: Homepage, https://github.com/KentVejrupMadsen/gv-targeting-model
 Project-URL: Issues, https://github.com/KentVejrupMadsen/gv-targeting-model/issues
 Project-URL: License, https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/License.md
 Project-URL: Requirements, https://raw.githubusercontent.com/KentVejrupMadsen/gv-targeting-model/main/requirements.txt
 Keywords: game,vision,machine,learning
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: notebook
 
 # Game targeting model
 ## Status
 ### Test & Publishing 
 [![Python package](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/testing.yml/badge.svg)](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/testing.yml)
 [![Upload Python Package](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/publish.yml/badge.svg)](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/publish.yml)
```

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/layers.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/layers.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/setup_package.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/setup_package.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/__init__.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/model_settings.py` & `game-vision-targeting-model-0.0.7/src/GameVisionTargetingModel/variables/model_settings.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/License.md` & `game-vision-targeting-model-0.0.7/License.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/PKG-INFO` & `game-vision-targeting-model-0.0.7/src/game_vision_targeting_model.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-vision-targeting-model
-Version: 0.0.6
+Version: 0.0.7
 Summary: A small example package
 Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
 License: Copyright 2023 Kent Vejrup Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, 
@@ -20,17 +20,20 @@
 Project-URL: Changelog, https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/Changelog.md
 Project-URL: Homepage, https://github.com/KentVejrupMadsen/gv-targeting-model
 Project-URL: Issues, https://github.com/KentVejrupMadsen/gv-targeting-model/issues
 Project-URL: License, https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/License.md
 Project-URL: Requirements, https://raw.githubusercontent.com/KentVejrupMadsen/gv-targeting-model/main/requirements.txt
 Keywords: game,vision,machine,learning
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+Provides-Extra: notebook
 
 # Game targeting model
 ## Status
 ### Test & Publishing 
 [![Python package](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/testing.yml/badge.svg)](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/testing.yml)
 [![Upload Python Package](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/publish.yml/badge.svg)](https://github.com/KentVejrupMadsen/gv-targeting-model/actions/workflows/publish.yml)
```

### Comparing `game-vision-targeting-model-0.0.6/Readme.md` & `game-vision-targeting-model-0.0.7/Readme.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/docs/License.md` & `game-vision-targeting-model-0.0.7/docs/License.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.6/pyproject.toml` & `game-vision-targeting-model-0.0.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "game-vision-targeting-model"
-version = "0.0.6"
+version = "0.0.7"
 
 authors = [
   { name="Kent vejrup Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
 
 description = "A small example package"
 readme = "Readme.md"
@@ -23,28 +23,34 @@
     "tensorflow",
     "numpy"
 ]
 
 license = { file='License.md' }
 
 classifiers = [
-    "Programming Language :: Python :: 3"
+    "Programming Language :: Python :: 3",
+    "Development Status :: 2 - Pre-Alpha",
+    "License :: OSI Approved :: MIT License"
 ]
 
 keywords = [
     "game", "vision", "machine", "learning"
 ]
 
 
 
 [project.optional-dependencies]
 dev = [
     'pytest'
 ]
 
+notebook = [
+    'jupyterlab'
+]
+
 [project.urls]
 "Changelog"     = "https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/Changelog.md"
 "Homepage"      = "https://github.com/KentVejrupMadsen/gv-targeting-model"
 "Issues"        = "https://github.com/KentVejrupMadsen/gv-targeting-model/issues"
 "License"       = "https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/License.md"
 "Requirements"  = "https://raw.githubusercontent.com/KentVejrupMadsen/gv-targeting-model/main/requirements.txt"
 
@@ -53,9 +59,9 @@
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
     "debug"
 ]
 
 [tool.setuptools.packages.find]
-where = ['GameVisionTargetingModel']
+where = ['src']
 namespaces = true
```

