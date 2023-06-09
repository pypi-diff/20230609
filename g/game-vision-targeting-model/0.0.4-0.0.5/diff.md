# Comparing `tmp/game_vision_targeting_model-0.0.4.tar.gz` & `tmp/game-vision-targeting-model-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "game-vision-targeting-model-0.0.5.tar", last modified: Fri Jun  9 17:24:12 2023, max compression
```

## Comparing `game_vision_targeting_model-0.0.4.tar` & `game-vision-targeting-model-0.0.5.tar`

### file list

```diff
@@ -1,40 +1,57 @@
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.gitattributes
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/Changelog.md
--rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/License.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/requirements.txt
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.github/workflows/testing.yml
--rw-r--r--   0        0        0    11856 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/notebooks/notebook.ipynb
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/__init__.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/setup_package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/__init__.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/__init__.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/__init__.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
--rw-r--r--   0        0        0      654 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/singletons/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/singletons/singletons.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/__init__.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/model_settings.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/normalise_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/training_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/configuration_test.py
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/map_classifier_test.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/tests/pytest_test.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/.gitignore
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/Readme.md
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 game_vision_targeting_model-0.0.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/Changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/docs/License.md
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/docs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.864636 game-vision-targeting-model-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_input_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_output_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/setup_package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/singletons/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/singletons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/singletons/singletons.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.868636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/map_classifier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/tests/pytest_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/model_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/normalise_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 17:23:59.000000 game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/training_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 17:24:12.872636 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-09 17:24:12.000000 game-vision-targeting-model-0.0.5/src/game_vision_targeting_model.egg-info/top_level.txt
```

### Comparing `game_vision_targeting_model-0.0.4/License.md` & `game-vision-targeting-model-0.0.5/License.md`

 * *Files identical despite different names*

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/setup_package.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/setup_package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.GameVisionTargetingModel.variables \
+from GameVisionTargetingModel.variables \
     import \
     set_channels, \
     set_width, \
     set_height, \
     set_last_layer_multiplier, \
     set_number_of_labels
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/layers.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.GameVisionTargetingModel.models.classification.map.v1.setup \
+from GameVisionTargetingModel.models.classification.map.v1.setup \
     import                  \
     generate_input_layer,   \
     generate_output_layer,  \
     generate_middle_layer,  \
     generate_preprocessing_layers
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/map_classifier_v1.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras.models \
     import Sequential
 
 from tensorflow import compat, get_logger
 
-from src.GameVisionTargetingModel.models.classification.map.v1.layers \
+from GameVisionTargetingModel.models.classification.map.v1.layers \
     import generate_layers_for_map_classifier_v1
 
 from keras.losses \
     import SparseCategoricalCrossentropy
 
 from keras.metrics              \
     import                      \
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/setup_of_middle_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from src.GameVisionTargetingModel.models.classification.map.v1.setup.middle_layer\
+from GameVisionTargetingModel.models.classification.map.v1.setup.middle_layer\
     import                          \
     generate_first_middle_layer,    \
     generate_second_middle_layer,   \
     generate_third_middle_layer,    \
     generate_decision_middle_layer
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/decision.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras.layers \
     import \
     Conv2D, \
     GlobalAveragePooling2D
 
-from src.GameVisionTargetingModel.variables.model_settings \
+from GameVisionTargetingModel.variables.model_settings \
     import \
     get_channels
 
 
 def generate_decision_middle_layer(
         layers: list
 ):
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/first.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras.layers \
     import \
     Conv2D, \
     MaxPooling2D
 
-from src.GameVisionTargetingModel.variables.model_settings \
+from GameVisionTargetingModel.variables.model_settings \
     import \
     get_channels
 
 
 def generate_first_middle_layer(
         layers: list
 ):
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/second.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras.layers \
     import \
     Conv2D, \
     MaxPooling2D
 
-from src.GameVisionTargetingModel.variables.model_settings \
+from GameVisionTargetingModel.variables.model_settings \
     import \
     get_channels
 
 
 def generate_second_middle_layer(
         layers: list
 ):
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/models/classification/map/v1/setup/middle_layer/third.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from keras.layers \
     import \
     Conv2D, \
     MaxPooling2D
 
-from src.GameVisionTargetingModel.variables.model_settings \
+from GameVisionTargetingModel.variables.model_settings \
     import \
     get_channels
 
 
 def generate_third_middle_layer(
         layers: list
 ):
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/__init__.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-from src.GameVisionTargetingModel.variables.model_settings \
+from GameVisionTargetingModel.variables.model_settings \
     import                  \
     get_input_set,          \
     get_width,              \
     get_channels,           \
     get_height,             \
     get_number_of_labels,   \
     get_last_layer_multiplier
 
-from src.GameVisionTargetingModel.variables.model_settings \
+from GameVisionTargetingModel.variables.model_settings \
     import                  \
     set_width,              \
     set_height,             \
     set_channels,           \
     set_number_of_labels,   \
     set_last_layer_multiplier
 
-from src.GameVisionTargetingModel.variables.normalise_settings \
+from GameVisionTargetingModel.variables.normalise_settings \
     import \
     get_rescaling_multiplier, \
     set_rescaling_multiplier
```

### Comparing `game_vision_targeting_model-0.0.4/src/GameVisionTargetingModel/variables/model_settings.py` & `game-vision-targeting-model-0.0.5/src/GameVisionTargetingModel/variables/model_settings.py`

 * *Files identical despite different names*

### Comparing `game_vision_targeting_model-0.0.4/Readme.md` & `game-vision-targeting-model-0.0.5/Readme.md`

 * *Files identical despite different names*

### Comparing `game_vision_targeting_model-0.0.4/pyproject.toml` & `game-vision-targeting-model-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,62 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
+requires = ["setuptools", "setuptools-scm"]
+build-backend = "setuptools.build_meta"
+
+
 
 [project]
 name = "game-vision-targeting-model"
-version = "0.0.4"
+version = "0.0.5"
 
 authors = [
   { name="Kent vejrup Madsen", email="kent.vejrup.madsen@outlook.com" },
 ]
 
 description = "A small example package"
 readme = "Readme.md"
 
 requires-python = ">=3.7"
+
+dependencies = [
+    "wheel",
+    "keras",
+    "tensorflow",
+    "numpy"
+]
+
+license = { file='License.md' }
+
 classifiers = [
     "Programming Language :: Python :: 3"
 ]
 
 keywords = [
     "game", "vision", "machine", "learning"
 ]
 
-dependencies = [
-    "wheel",
-    "keras",
-    "tensorflow",
-    "numpy"
-]
+
 
 [project.optional-dependencies]
-test = [
+dev = [
     'pytest'
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/KentVejrupMadsen/gv-targeting-model"
-"Bug Tracker" = "https://github.com/KentVejrupMadsen/gv-targeting-model/issues"
-"License" = "https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/License.md"
-"Change logs" = "https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/Changelog.md"
-"requirements" = "https://raw.githubusercontent.com/KentVejrupMadsen/gv-targeting-model/main/requirements.txt"
+"Changelog"     = "https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/Changelog.md"
+"Homepage"      = "https://github.com/KentVejrupMadsen/gv-targeting-model"
+"Issues"        = "https://github.com/KentVejrupMadsen/gv-targeting-model/issues"
+"License"       = "https://github.com/KentVejrupMadsen/gv-targeting-model/blob/main/License.md"
+"Requirements"  = "https://raw.githubusercontent.com/KentVejrupMadsen/gv-targeting-model/main/requirements.txt"
 
 
 [tool.pytest.ini_options]
 markers = [
     "slow: marks tests as slow (deselect with '-m \"not slow\"')",
     "serial",
     "debug"
 ]
 
+[tool.setuptools.packages.find]
+where = ['src']
+include = ['GameVisionTargetingModel*']
+namespaces = true
```

