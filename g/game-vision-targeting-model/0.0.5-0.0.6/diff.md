# Comparing `tmp/game-vision-targeting-model-0.0.5.tar.gz` & `tmp/game-vision-targeting-model-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-vision-targeting-model-0.0.5.tar", last modified: Fri Jun  9 17:24:12 2023, max compression
+gzip compressed data, was "game-vision-targeting-model-0.0.6.tar", last modified: Fri Jun  9 17:38:21 2023, max compression
```

## Comparing `game-vision-targeting-model-0.0.5.tar` & `game-vision-targeting-model-0.0.6.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/Changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/License.md
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/docs/License.md
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/docs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.864636 game-vision-targeting-model-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/setup_package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/singletons/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/singletons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/singletons/singletons.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/map_classifier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/pytest_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/model_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/normalise_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/training_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/Changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-09 17:38:21.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.314159 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/singletons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/singletons/singletons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/map_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/tests/pytest_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/normalise_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/training_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/docs/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/docs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:38:21.318158 game-vision-targeting-model-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:38:08.000000 game-vision-targeting-model-0.0.6/setup.py
```

### Comparing `game-vision-targeting-model-0.0.5/License.md` & `game-vision-targeting-model-0.0.6/License.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/PKG-INFO` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/game_vision_targeting_model.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-vision-targeting-model
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
 License: Copyright 2023 Kent Vejrup Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
```

### Comparing `game-vision-targeting-model-0.0.5/Readme.md` & `game-vision-targeting-model-0.0.6/Readme.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/docs/License.md` & `game-vision-targeting-model-0.0.6/docs/License.md`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/pyproject.toml` & `game-vision-targeting-model-0.0.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 
 
 [project]
 name = "game-vision-targeting-model"
-version = "0.0.5"
+version = "0.0.6"
 
 authors = [
   { name="Kent vejrup Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
 
 description = "A small example package"
 readme = "Readme.md"
@@ -53,10 +53,9 @@
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
     "debug"
 ]
 
 [tool.setuptools.packages.find]
-where = ['src']
-include = ['GameVisionTargetingModel*']
+where = ['GameVisionTargetingModel']
 namespaces = true
```

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/layers.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/layers.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/setup_package.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/setup_package.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/__init__.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/model_settings.py` & `game-vision-targeting-model-0.0.6/GameVisionTargetingModel/variables/model_settings.py`

 * *Files identical despite different names*

### Comparing `game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/PKG-INFO` & `game-vision-targeting-model-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: game-vision-targeting-model
-Version: 0.0.5
+Version: 0.0.6
 Summary: A small example package
 Author-email: Kent vejrup Madsen <kent.vejrup.madsen@outlook.com>
 License: Copyright 2023 Kent Vejrup Madsen
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated 
         documentation files (the “Software”), to deal in the Software without restriction, including without limitation 
         the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
```

