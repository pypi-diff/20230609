# Comparing `tmp/pyilz-0.0.7.tar.gz` & `tmp/pyilz-0.0.8.tar.gz`

## Comparing `pyilz-0.0.7.tar` & `pyilz-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.7/requirements.txt
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.7/.github/workflows/main.yml
--rw-r--r--   0        0        0    29922 2020-02-02 00:00:00.000000 pyilz-0.0.7/images/access_tokens.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/__init__.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/get_device_id.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/get_game_state.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/get_timers.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/get_token.py
--rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/parse_land.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyilz/refresh_token.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.7/tests/example_game_state.json
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.7/tests/test_e2e.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.7/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.7/LICENSE
--rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 pyilz-0.0.7/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 pyilz-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 pyilz-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 pyilz-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 pyilz-0.0.8/.github/workflows/main.yml
+-rw-r--r--   0        0        0    29922 2020-02-02 00:00:00.000000 pyilz-0.0.8/images/access_tokens.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/__init__.py
+-rw-r--r--   0        0        0   131677 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/buildings.json
+-rw-r--r--   0        0        0     2602 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_buildings.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_device_id.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_game_state.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_timers.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/get_token.py
+-rw-r--r--   0        0        0     5729 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/parse_land.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyilz/refresh_token.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyilz-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0   264324 2020-02-02 00:00:00.000000 pyilz-0.0.8/tests/example_game_state.json
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pyilz-0.0.8/tests/test_e2e.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 pyilz-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 pyilz-0.0.8/LICENSE
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 pyilz-0.0.8/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 pyilz-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 pyilz-0.0.8/PKG-INFO
```

### Comparing `pyilz-0.0.7/.github/workflows/main.yml` & `pyilz-0.0.8/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/images/access_tokens.png` & `pyilz-0.0.8/images/access_tokens.png`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/pyilz/get_device_id.py` & `pyilz-0.0.8/pyilz/get_device_id.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/pyilz/get_game_state.py` & `pyilz-0.0.8/pyilz/get_game_state.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/pyilz/get_timers.py` & `pyilz-0.0.8/pyilz/get_timers.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/pyilz/parse_land.py` & `pyilz-0.0.8/pyilz/parse_land.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/pyilz/refresh_token.py` & `pyilz-0.0.8/pyilz/refresh_token.py`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/tests/example_game_state.json` & `pyilz-0.0.8/tests/example_game_state.json`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/.gitignore` & `pyilz-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/LICENSE` & `pyilz-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyilz-0.0.7/README.md` & `pyilz-0.0.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,21 @@
 
 As the current Alpha version has no server-side authority the methods implemented only perform reads as to not break your gamestate.
 
 This library **CAN** be used while you have the game running as it uses your local machines **[device_id](/pyilz/get_device_id.py)**, without this your game client would log-out due to different devices running the same plot.
 
 *Currently only supports Windows as replicating the **[get_device_id](/pyilz/get_device_id.py)** implementation from the Unity game engine requires WMI.*
 
+# Installation
+
+Install using `pip`...
+
+    pip install pyilz
+
+
 # Requirements
 
 * Python 3.7+
 * Your Cognito access_token or refresh_token [*See below*](#acquiring-a-cognito-access_token)
 
 Tokens can either be passed into the [**get_game_state**](/pyilz/get_game_state.py) function or pulled from the environment variables if available.
 
@@ -31,20 +38,14 @@
 At the time of writing this there is no way of generating application scoped access tokens so the only way to authenticate against the gamestate APIs is by logging into https://play.illuvium.io/ and retrieving the tokens from local storage.
 
 **DO NOT** share your refresh_token or access_token, the refresh_token can generate new access_tokens for up to 30 days.
 
 ### Example of tokens in Chromium Local Storage
 ![access_tokens.png](/images/access_tokens.png)
 
-# Installation
-
-Install using `pip`...
-
-    pip install pyilz
-
 
 # Example
 ```py
 from pyilz.get_token import get_token
 from pyilz.get_game_state import get_game_state
 from pyilz.parse_land import parse_land
 from pyilz.get_timers import get_timers
```

### Comparing `pyilz-0.0.7/pyproject.toml` & `pyilz-0.0.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyilz"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Nick Jordan", email="nickjordan289@gmail.com" },
 ]
 description = "A Python Library for Illuvium Zero Land Management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
+    "Operating System :: Microsoft :: Windows",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/NickJordan289/pyilz"
 "Bug Tracker" = "https://github.com/NickJordan289/pyilz/issues"
```

### Comparing `pyilz-0.0.7/PKG-INFO` & `pyilz-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pyilz
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Python Library for Illuvium Zero Land Management
 Project-URL: Homepage, https://github.com/NickJordan289/pyilz
 Project-URL: Bug Tracker, https://github.com/NickJordan289/pyilz/issues
 Author-email: Nick Jordan <nickjordan289@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
+Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Pyilz - An Illuvium Zero Python library
 
 [![build-status-image]][build-status]
@@ -23,14 +23,21 @@
 
 As the current Alpha version has no server-side authority the methods implemented only perform reads as to not break your gamestate.
 
 This library **CAN** be used while you have the game running as it uses your local machines **[device_id](/pyilz/get_device_id.py)**, without this your game client would log-out due to different devices running the same plot.
 
 *Currently only supports Windows as replicating the **[get_device_id](/pyilz/get_device_id.py)** implementation from the Unity game engine requires WMI.*
 
+# Installation
+
+Install using `pip`...
+
+    pip install pyilz
+
+
 # Requirements
 
 * Python 3.7+
 * Your Cognito access_token or refresh_token [*See below*](#acquiring-a-cognito-access_token)
 
 Tokens can either be passed into the [**get_game_state**](/pyilz/get_game_state.py) function or pulled from the environment variables if available.
 
@@ -45,20 +52,14 @@
 At the time of writing this there is no way of generating application scoped access tokens so the only way to authenticate against the gamestate APIs is by logging into https://play.illuvium.io/ and retrieving the tokens from local storage.
 
 **DO NOT** share your refresh_token or access_token, the refresh_token can generate new access_tokens for up to 30 days.
 
 ### Example of tokens in Chromium Local Storage
 ![access_tokens.png](/images/access_tokens.png)
 
-# Installation
-
-Install using `pip`...
-
-    pip install pyilz
-
 
 # Example
 ```py
 from pyilz.get_token import get_token
 from pyilz.get_game_state import get_game_state
 from pyilz.parse_land import parse_land
 from pyilz.get_timers import get_timers
```

