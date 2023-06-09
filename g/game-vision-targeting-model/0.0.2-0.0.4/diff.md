# Comparing `tmp/game-vision-targeting-model-0.0.2.tar.gz` & `tmp/game_vision_targeting_model-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "game-vision-targeting-model-0.0.2.tar", last modified: Tue May 30 19:12:46 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `game-vision-targeting-model-0.0.2.tar` & `game_vision_targeting_model-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/models/map_classifier_v1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/preprocessing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/model_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/training_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-30 19:12:28.000000 game-vision-targeting-model-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 19:12:46.512616 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-30 19:12:45.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-30 19:12:46.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 19:12:45.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-30 19:12:46.000000 game-vision-targeting-model-0.0.2/src/game_vision_targeting_model.egg-info/top_level.txt
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.gitattributes
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/Changelog.md
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/License.md
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/requirements.txt
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.github/workflows/testing.yml
+-rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/notebooks/notebook.ipynb
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/__init__.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/setup_package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/__init__.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/__init__.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/__init__.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
+-rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
+-rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
+-rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/singletons/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/singletons/singletons.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/__init__.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/model_settings.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/normalise_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/training_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/configuration_test.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/map_classifier_test.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/pytest_test.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.gitignore
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/Readme.md
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/PKG-INFO
```

### Comparing `game-vision-targeting-model-0.0.2/src/GameVisionTargetingModel/variables/model_settings.py` & `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/model_settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,12 +64,19 @@
 
 
 def get_number_of_labels() -> int:
     global number_of_labels
     return number_of_labels
 
 
+def set_last_layer_multiplier(
+        value: int
+) -> None:
+    global last_layer_multiplier
+    last_layer_multiplier = value
+
+
 def set_number_of_labels(
         value: int
 ) -> None:
     global number_of_labels
     number_of_labels = value
```

