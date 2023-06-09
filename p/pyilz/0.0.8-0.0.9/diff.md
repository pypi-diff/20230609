# Comparing `tmp/pyilz-0.0.8.tar.gz` & `tmp/pyilz-0.0.9.tar.gz`

## Comparing `pyilz-0.0.8.tar` & `pyilz-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.8/requirements.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.8/.github/workflows/main.yml
--rw-r--r--   0        0        0    29922 2020-02-02 00:00:00.000000 pyilz-0.0.8/images/access_tokens.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/__init__.py
--rw-r--r--   0        0        0   131677 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/buildings.json
--rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_buildings.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_device_id.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_game_state.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_timers.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_token.py
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/parse_land.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/refresh_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.8/tests/example_game_state.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.8/tests/test_e2e.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.8/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.8/LICENSE
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pyilz-0.0.8/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pyilz-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.9/requirements.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.9/.github/workflows/main.yml
+-rw-r--r--   0        0        0    29922 2020-02-02 00:00:00.000000 pyilz-0.0.9/images/access_tokens.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/__init__.py
+-rw-r--r--   0        0        0   131677 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/buildings.json
+-rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/get_buildings.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/get_device_id.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/get_game_state.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/get_timers.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/get_token.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/parse_land.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyilz/refresh_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.9/tests/example_game_state.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.9/tests/test_e2e.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pyilz-0.0.9/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pyilz-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pyilz-0.0.9/PKG-INFO
```

### Comparing `pyilz-0.0.8/.github/workflows/main.yml` & `pyilz-0.0.9/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/images/access_tokens.png` & `pyilz-0.0.9/images/access_tokens.png`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyilz/buildings.json` & `pyilz-0.0.9/pyilz/buildings.json`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyilz/get_buildings.py` & `pyilz-0.0.9/pyilz/get_buildings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 import json
 import math
-with open('./pyilz/buildings.json', 'r') as f:
-    buildings = json.load(f)['buildings']
+import importlib.resources
+import json
+
+with importlib.resources.open_text("pyilz", "buildings.json") as file:
+    buildings = json.load(file)['buildings']
 
 
 def get_active_output(name, level, tier, efficiency=100):
     name = name.lower().replace(' ', '').replace('_', '')
     land_tier_bonus_multiplier_percent = [0, 0, 33.33333333333, 100, 300, 900]
     for building in buildings:  # This should probably be a dict
         if building['nameId'] == name:
```

### Comparing `pyilz-0.0.8/pyilz/get_device_id.py` & `pyilz-0.0.9/pyilz/get_device_id.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyilz/get_game_state.py` & `pyilz-0.0.9/pyilz/get_game_state.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyilz/get_timers.py` & `pyilz-0.0.9/pyilz/get_timers.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyilz/parse_land.py` & `pyilz-0.0.9/pyilz/parse_land.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyilz/refresh_token.py` & `pyilz-0.0.9/pyilz/refresh_token.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/tests/example_game_state.json` & `pyilz-0.0.9/tests/example_game_state.json`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/.gitignore` & `pyilz-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/LICENSE` & `pyilz-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/README.md` & `pyilz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.8/pyproject.toml` & `pyilz-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyilz"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Nick Jordan", email="nickjordan289@gmail.com" },
 ]
 description = "A Python Library for Illuvium Zero Land Management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyilz-0.0.8/PKG-INFO` & `pyilz-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyilz
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Python Library for Illuvium Zero Land Management
 Project-URL: Homepage, https://github.com/NickJordan289/pyilz
 Project-URL: Bug Tracker, https://github.com/NickJordan289/pyilz/issues
 Author-email: Nick Jordan <nickjordan289@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

