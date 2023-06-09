# Comparing `tmp/homewizard_climate_ws-0.0.21.tar.gz` & `tmp/homewizard_climate_ws-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homewizard_climate_ws-0.0.21.tar", last modified: Fri Jun  9 08:01:27 2023, max compression
+gzip compressed data, was "homewizard_climate_ws-0.0.9.tar", last modified: Sun Jan 22 18:13:04 2023, max compression
```

## Comparing `homewizard_climate_ws-0.0.21.tar` & `homewizard_climate_ws-0.0.9.tar`

### file list

```diff
@@ -1,44 +1,43 @@
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.857241 homewizard_climate_ws-0.0.21/
--rw-r--r--   0 JongD      (502) staff       (20)     1622 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/CONTRIBUTING.md
--rw-r--r--   0 JongD      (502) staff       (20)     1064 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/LICENSE
--rw-r--r--   0 JongD      (502) staff       (20)      260 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/MANIFEST.in
--rw-r--r--   0 JongD      (502) staff       (20)     2834 2023-06-09 08:01:27.857298 homewizard_climate_ws-0.0.21/PKG-INFO
--rw-r--r--   0 JongD      (502) staff       (20)     1979 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/README.md
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.853215 homewizard_climate_ws-0.0.21/docs/
--rw-r--r--   0 JongD      (502) staff       (20)      629 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/docs/Makefile
--rwxr-xr-x   0 JongD      (502) staff       (20)     5580 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/docs/conf.py
--rw-r--r--   0 JongD      (502) staff       (20)       34 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/docs/contributing.rst
--rw-r--r--   0 JongD      (502) staff       (20)      370 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/docs/index.rst
--rw-r--r--   0 JongD      (502) staff       (20)     1266 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/docs/installation.rst
--rw-r--r--   0 JongD      (502) staff       (20)      826 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/docs/make.bat
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.854082 homewizard_climate_ws-0.0.21/homewizard_climate_ws/
--rw-r--r--   0 JongD      (502) staff       (20)      299 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/__init__.py
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.855363 homewizard_climate_ws-0.0.21/homewizard_climate_ws/api/
--rw-r--r--   0 JongD      (502) staff       (20)        0 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/api/__init__.py
--rw-r--r--   0 JongD      (502) staff       (20)     2943 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/api/api.py
--rw-r--r--   0 JongD      (502) staff       (20)      157 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/const.py
--rw-r--r--   0 JongD      (502) staff       (20)     1616 2023-05-18 12:38:33.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/debug.py
--rw-r--r--   0 JongD      (502) staff       (20)      607 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/main.py
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.855775 homewizard_climate_ws-0.0.21/homewizard_climate_ws/model/
--rw-r--r--   0 JongD      (502) staff       (20)        0 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/model/__init__.py
--rw-r--r--   0 JongD      (502) staff       (20)      657 2023-06-09 08:00:52.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/model/climate_device.py
--rw-r--r--   0 JongD      (502) staff       (20)     1785 2023-05-19 09:21:30.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/model/climate_device_state.py
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.856316 homewizard_climate_ws-0.0.21/homewizard_climate_ws/ws/
--rw-r--r--   0 JongD      (502) staff       (20)        0 2023-05-18 11:46:21.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/ws/__init__.py
--rw-r--r--   0 JongD      (502) staff       (20)     9829 2023-05-18 12:36:59.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/ws/hw_websocket.py
--rw-r--r--   0 JongD      (502) staff       (20)     5638 2023-05-18 12:34:47.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws/ws/hw_websocket_payloads.py
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.855086 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/
--rw-r--r--   0 JongD      (502) staff       (20)     2834 2023-06-09 08:01:27.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/PKG-INFO
--rw-r--r--   0 JongD      (502) staff       (20)      982 2023-06-09 08:01:27.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/SOURCES.txt
--rw-r--r--   0 JongD      (502) staff       (20)        1 2023-06-09 08:01:27.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/dependency_links.txt
--rw-r--r--   0 JongD      (502) staff       (20)        1 2023-05-18 11:47:43.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/not-zip-safe
--rw-r--r--   0 JongD      (502) staff       (20)      853 2023-06-09 08:01:27.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/requires.txt
--rw-r--r--   0 JongD      (502) staff       (20)       22 2023-06-09 08:01:27.000000 homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/top_level.txt
--rw-r--r--   0 JongD      (502) staff       (20)      488 2023-06-09 08:01:27.857535 homewizard_climate_ws-0.0.21/setup.cfg
--rw-r--r--   0 JongD      (502) staff       (20)     2442 2023-06-09 08:01:11.000000 homewizard_climate_ws-0.0.21/setup.py
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.856919 homewizard_climate_ws-0.0.21/tests/
--rw-r--r--   0 JongD      (502) staff       (20)       83 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/tests/__init__.py
--rw-r--r--   0 JongD      (502) staff       (20)     1387 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/tests/conftest.py
-drwxr-xr-x   0 JongD      (502) staff       (20)        0 2023-06-09 08:01:27.857089 homewizard_climate_ws-0.0.21/tests/data/
--rw-r--r--   0 JongD      (502) staff       (20)       42 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/tests/data/example_values.json
--rw-r--r--   0 JongD      (502) staff       (20)       58 2023-01-14 12:59:20.000000 homewizard_climate_ws-0.0.21/tests/test_dummy.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     1622 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/CONTRIBUTING.md
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     1064 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/LICENSE
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      260 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/MANIFEST.in
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     2576 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/PKG-INFO
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     1702 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/README.md
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/docs/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      629 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/docs/Makefile
+-rwxrwxr-x   0 dennis    (1000) dennis    (1000)     5608 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/docs/conf.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)       34 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/docs/contributing.rst
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      370 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/docs/index.rst
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     1266 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/docs/installation.rst
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      826 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/docs/make.bat
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/homewizard_climate_ws/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      299 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/__init__.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/homewizard_climate_ws/api/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)        0 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/api/__init__.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     3112 2023-01-14 09:36:28.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/api/api.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      157 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/const.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      621 2023-01-14 09:36:28.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/main.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/homewizard_climate_ws/model/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)        0 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/model/__init__.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      559 2023-01-22 17:43:23.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/model/climate_device.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     1397 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/model/climate_device_state.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/homewizard_climate_ws/ws/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)        0 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/ws/__init__.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     9112 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/ws/hw_websocket.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     3580 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws/ws/hw_websocket_payloads.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     2576 2023-01-22 18:13:04.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/PKG-INFO
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      951 2023-01-22 18:13:04.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/SOURCES.txt
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)        1 2023-01-22 18:13:04.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/dependency_links.txt
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)        1 2023-01-22 17:47:58.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/not-zip-safe
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      891 2023-01-22 18:13:04.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/requires.txt
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)       22 2023-01-22 18:13:04.000000 homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/top_level.txt
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)      494 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/setup.cfg
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     2448 2023-01-22 18:11:06.000000 homewizard_climate_ws-0.0.9/setup.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/tests/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)       83 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/tests/__init__.py
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)     1387 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/tests/conftest.py
+drwxrwxr-x   0 dennis    (1000) dennis    (1000)        0 2023-01-22 18:13:04.111498 homewizard_climate_ws-0.0.9/tests/data/
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)       42 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/tests/data/example_values.json
+-rw-rw-r--   0 dennis    (1000) dennis    (1000)       58 2023-01-13 19:20:50.000000 homewizard_climate_ws-0.0.9/tests/test_dummy.py
```

### Comparing `homewizard_climate_ws-0.0.21/CONTRIBUTING.md` & `homewizard_climate_ws-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `homewizard_climate_ws-0.0.21/LICENSE` & `homewizard_climate_ws-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `homewizard_climate_ws-0.0.21/PKG-INFO` & `homewizard_climate_ws-0.0.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: homewizard_climate_ws
-Version: 0.0.21
+Version: 0.0.9
 Summary: API/Websocket to control Homewizard Climate devices
 Home-page: https://github.com/dennis1804/homewizard-climate-websocket
 Author: Dennis1804
 Author-email: dennis@de-jong.frl
 License: MIT license
 Keywords: homewizard_climate_ws
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: setup
 Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 # homewizard-climate-websocket
 
 API/Websocket to control Homewizard Climate devices
 
 ---
 
 This library allows you to control your Homewizard Climate devices. There are a multitude of brands that use Homewizard apps for their smart controls.
 
-This was developed in order to be used in a [Home Assistant](https://www.home-assistant.io/) integration. It has not been thoroughly tested or worked with as a standalone code.
+This was developed in oder to be used in a [Home Assistant](https://www.home-assistant.io/) integration. It has not been thoroughly tested or worked with as a standalone code.
 
 ### Supported Devices
 This library is in an early stage of development and only works for the following device types returned from the Homewizard Climate API:
 
 - `heaterfan`
-- `infraredheater`
-- `heater`
 
 It has been tested on the following devices (even though it might work on others too):
 - [Princess Smart Heating and Cooling Tower (01.347000.01.001)](https://www.princesshome.eu/en-gb/princess-01-347000-01-001-smart-heating-and-01.347000.01.001)
-- [Princess Smart Infrared Panel Heater 350 (01.343350.02.001)](https://www.princesshome.eu/en-gb/princess-01-343350-02-001-smart-infrared-panel-01.343350.02.001)
-- [Princess Smart Glass Panel Heater (01.342001.09.001)](https://www.princesshome.eu/en-gb/princess-01-342001-09-001-smart-glass-panel-heater-01.342001.09.001)
+
+![](https://www.princesshome.eu/product/image/large/01.347000.01.001_3.jpg)
 
 ## Quick start
 There's no separate `requirements.txt` file, the dependencies can be found and installed in `setup.py`
 
 ```
 username = os.environ["HW_CLIMATE_USERNAME"]
 password = os.environ["HW_CLIMATE_PASSWORD"]
@@ -64,7 +63,9 @@
 **Stable Release (PyPi):** `pip install homewizard_climate_websocket`<br>
 **Local Development:** `pip install .`
 
 ## Development
 Any help to increase the number of supported devices is much appreciated as I only had access to the one mentioned above.
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
+
+
```

### Comparing `homewizard_climate_ws-0.0.21/README.md` & `homewizard_climate_ws-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 
 API/Websocket to control Homewizard Climate devices
 
 ---
 
 This library allows you to control your Homewizard Climate devices. There are a multitude of brands that use Homewizard apps for their smart controls.
 
-This was developed in order to be used in a [Home Assistant](https://www.home-assistant.io/) integration. It has not been thoroughly tested or worked with as a standalone code.
+This was developed in oder to be used in a [Home Assistant](https://www.home-assistant.io/) integration. It has not been thoroughly tested or worked with as a standalone code.
 
 ### Supported Devices
 This library is in an early stage of development and only works for the following device types returned from the Homewizard Climate API:
 
 - `heaterfan`
-- `infraredheater`
-- `heater`
 
 It has been tested on the following devices (even though it might work on others too):
 - [Princess Smart Heating and Cooling Tower (01.347000.01.001)](https://www.princesshome.eu/en-gb/princess-01-347000-01-001-smart-heating-and-01.347000.01.001)
-- [Princess Smart Infrared Panel Heater 350 (01.343350.02.001)](https://www.princesshome.eu/en-gb/princess-01-343350-02-001-smart-infrared-panel-01.343350.02.001)
-- [Princess Smart Glass Panel Heater (01.342001.09.001)](https://www.princesshome.eu/en-gb/princess-01-342001-09-001-smart-glass-panel-heater-01.342001.09.001)
+
+![](https://www.princesshome.eu/product/image/large/01.347000.01.001_3.jpg)
 
 ## Quick start
 There's no separate `requirements.txt` file, the dependencies can be found and installed in `setup.py`
 
 ```
 username = os.environ["HW_CLIMATE_USERNAME"]
 password = os.environ["HW_CLIMATE_PASSWORD"]
```

### Comparing `homewizard_climate_ws-0.0.21/docs/Makefile` & `homewizard_climate_ws-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `homewizard_climate_ws-0.0.21/docs/conf.py` & `homewizard_climate_ws-0.0.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,17 @@
 # absolute, like shown here.
 #
 import os
 import sys
 
 import sphinx_rtd_theme
 
-import homewizard_climate_ws
+import homewizard_climate_websocket
 
-sys.path.insert(0, os.path.abspath("../homewizard_climate_ws"))
+sys.path.insert(0, os.path.abspath("../homewizard_climate_websocket"))
 
 
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = "1.0"
@@ -74,17 +74,17 @@
 author = "Mepla"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = homewizard_climate_ws.__version__
+version = homewizard_climate_websocket.__version__
 # The full version, including alpha/beta/rc tags.
-release = homewizard_climate_ws.__version__
+release = homewizard_climate_websocket.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `homewizard_climate_ws-0.0.21/docs/installation.rst` & `homewizard_climate_ws-0.0.9/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `homewizard_climate_ws-0.0.21/docs/make.bat` & `homewizard_climate_ws-0.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws/api/api.py` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws/api/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 
 import requests
 
-from homewizard_climate_ws.const import API_LOGIN, API_V1_PATH, API_DEVICES
-from homewizard_climate_ws.model.climate_device import (
+from homewizard_climate_websocket.const import API_LOGIN, API_V1_PATH, API_DEVICES
+from homewizard_climate_websocket.model.climate_device import (
     HomeWizardClimateDevice,
     HomeWizardClimateDeviceType,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -35,47 +35,50 @@
         _LOGGER.debug(f"Logging in to {login_path} with username {self._username}")
 
         resp = requests.get(login_path, auth=(self._username, self._password))
         _LOGGER.debug(f"Login ({self._username}) status code: {resp.status_code}")
 
         if (
             resp.status_code == 200
-            and "application/json" in resp.headers.get("content-type")
+            and resp.headers.get("content-type") == "application/json"
             and "token" in resp.json()
         ):
             self._token = resp.json().get("token")
             _LOGGER.debug(f"Login successful with token for username {self._username}")
             return self._token
         else:
             _LOGGER.error(
                 f"Login failed for username {self._username}, response was: {resp}"
             )
             raise InvalidHomewizardAuth()
 
-    def get_devices(self) -> list:
+    def get_devices(self) -> list[HomeWizardClimateDevice]:
         resp = requests.get(
             os.path.join(API_V1_PATH, API_DEVICES),
             auth=(self._username, self._password),
         )
         if (
             resp.status_code == 200
-            and "application/json" in resp.headers.get("content-type")
+            and resp.headers.get("content-type") == "application/json"
             and "devices" in resp.json()
         ):
             supported_device_types = [t.value for t in HomeWizardClimateDeviceType]
             _LOGGER.debug(
                 f'Received {len(resp.json().get("devices"))} device(s) for user '
                 f"({self._username}), filtering the supported ones. "
                 f"supported_device_types: {supported_device_types}"
             )
             devices_list = list(
                 map(
                     HomeWizardClimateDevice.from_dict,
                     # Filter only known device types in: HomeWizardClimateDeviceType
-                    resp.json().get("devices"),
+                    filter(
+                        lambda x: x.get("type") in supported_device_types,
+                        resp.json().get("devices"),
+                    ),
                 )
             )
             _LOGGER.debug(
                 f"Creating {len(devices_list)} device(s) for user "
                 f"({self._username}): {[x.identifier for x in devices_list]}"
             )
             return devices_list
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws/main.py` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import os
 import time
 
-from homewizard_climate_ws.api.api import HomeWizardClimateApi
-from homewizard_climate_ws.ws.hw_websocket import HomeWizardClimateWebSocket
+from homewizard_climate_websocket.api.api import HomeWizardClimateApi
+from homewizard_climate_websocket.ws.hw_websocket import HomeWizardClimateWebSocket
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def main():
     username = os.environ["HW_CLIMATE_USERNAME"]
     password = os.environ["HW_CLIMATE_PASSWORD"]
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws/model/climate_device.py` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws/model/climate_device.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,19 +8,16 @@
 class HomeWizardClimateDeviceType(Enum):
     """Only devices with these defined types will be picked
     up by the API function get_devices"""
 
     HEATERFAN = "heaterfan"
     INFRAREDHEATER = "infraredheater"
     HEATER = "heater"
-    FAN = "fan"
-    DEHUMIDIFIER = "dehumidifier"
-    AIRCONDITIONER = "airconditioner"
 
 @dataclass_json
 @dataclass
 class HomeWizardClimateDevice:
     name: Optional[str]
     identifier: str
     grants: Optional[list]
-    type: Optional[HomeWizardClimateDeviceType]
+    type: HomeWizardClimateDeviceType
     endpoint: Optional[str]
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws/model/climate_device_state.py` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws/model/climate_device_state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,69 +1,58 @@
 from dataclasses import dataclass
-from typing import Optional
-from dataclasses_json import dataclass_json, Undefined
 
+from dataclasses_json import dataclass_json
 
-@dataclass_json(undefined=Undefined.EXCLUDE)
+
+@dataclass_json
 @dataclass
 class HomeWizardClimateDeviceState:
     power_on: bool
-    mode: Optional[str]
+    mode: str
     current_temperature: int
     target_temperature: int
-    target_humidity: int
-    current_humidity: int
     fan_speed: int
     oscillate: bool
-    oscillation: bool
     timer: int
-    speed: int
     error: list[str]
     heat_status: str
     vent_heat: bool
     silent: bool
     heater: bool
-    swing: bool
     ext_mode: list[str]
     ext_current_temperature: int
     ext_target_temperature: int
 
 
 def default_state():
     return HomeWizardClimateDeviceState.from_dict(
         {
             "power_on": False,
             "mode": "normal",
             "current_temperature": 0,
             "target_temperature": 0,
-            "target_humidity": 0,
-            "current_humidity": 0,
             "fan_speed": 0,
             "oscillate": False,
-            "oscillation": False,
             "timer": 0,
-            "speed": 1,
             "ext_mode": [],
             "heat_status": "idle",
             "vent_heat": False,
             "silent": False,
             "heater": False,
-            "swing": False,
             "error": [],
             "ext_current_temperature": 0,
             "ext_target_temperature": 0,
         }
     )
 
 
 def diff_states(
     first_state: HomeWizardClimateDeviceState,
     second_state: HomeWizardClimateDeviceState,
 ) -> str:
     result = ""
     for k, v in first_state.to_dict().items():
-        if k in second_state.to_dict():
-            second_value = second_state.to_dict().get(k)
-            if v != second_value:
-                result += f"{k}: {v} -> {second_value}, "
+        second_value = second_state.to_dict().get(k)
+        if v != second_value:
+            result += f"{k}: {v} -> {second_value}, "
 
     return result
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws/ws/hw_websocket.py` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws/ws/hw_websocket.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from collections.abc import Callable
 from dataclasses import replace
 from enum import Enum
 
 import websocket
 from websocket._exceptions import WebSocketConnectionClosedException
 
-from homewizard_climate_ws.api.api import HomeWizardClimateApi
-from homewizard_climate_ws.const import API_WS_PATH
-from homewizard_climate_ws.model.climate_device import (
+from homewizard_climate_websocket.api.api import HomeWizardClimateApi
+from homewizard_climate_websocket.const import API_WS_PATH
+from homewizard_climate_websocket.model.climate_device import (
     HomeWizardClimateDevice,
 )
-from homewizard_climate_ws.model.climate_device_state import (
+from homewizard_climate_websocket.model.climate_device_state import (
     HomeWizardClimateDeviceState,
     default_state,
     diff_states,
 )
-from homewizard_climate_ws.ws.hw_websocket_payloads import (
+from homewizard_climate_websocket.ws.hw_websocket_payloads import (
     HomeWizardClimateWSPayloads,
 )
 
 
 class SocketStatus(Enum):
     PRE_INITIALIZATION = 0
     INITIALIZING = 1
@@ -119,30 +119,14 @@
 
     def set_fan_speed(self, speed: int) -> None:
         self._send_message(self._payloads.set_fan_speed(speed))
 
     def set_target_temperature(self, temp: int) -> None:
         self._send_message(self._payloads.set_target_temperature(temp))
 
-
-    def set_mode(self, mode: str) -> None:
-        self._send_message(self._payloads.set_mode(mode))
-
-    def set_timer(self, timer: int) -> None:
-        self._send_message(self._payloads.set_timer(timer))
-
-    def set_target_humidity(self, humidity: int) -> None:
-        self._send_message(self._payloads.set_target_humidity(humidity))
-
-    def set_speed(self, speed: int) -> None:
-        self._send_message(self._payloads.set_speed(speed))
-
-    def set_swing(self, swing: bool) -> None:
-        self._send_message(self._payloads.set_swing(swing))
-
     def turn_on_heater(self) -> None:
         self._send_message(self._payloads.set_heater())
 
     def turn_on_cooler(self) -> None:
         self._send_message(self._payloads.set_cooler())
 
     def turn_on_oscillation(self) -> None:
@@ -213,21 +197,16 @@
         if self._socket_status == SocketStatus.INITIALIZING:
             self._socket_status = SocketStatus.INITIALIZED
             self._LOGGER.debug("Socket initialized.")
             if self._on_initialized:
                 self._on_initialized(self._device)
 
         self._LOGGER.debug(f"Received full device update: {received_message}")
-        state = received_message.get("state")
-        # Fill-in missing state entries using default values
-        for k, v in default_state().to_dict().items():
-            if k not in state:
-                state[k] = v
         self._update_last_state(
-            HomeWizardClimateDeviceState.from_dict(state)
+            HomeWizardClimateDeviceState.from_dict(received_message.get("state"))
         )
 
     def _handle_state_update(self, received_message: dict) -> None:
         if received_message.get("patch"):
             kw = {}
             for patch in received_message.get("patch"):
                 if patch.get("op", "") == "replace":
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws/ws/hw_websocket_payloads.py` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws/ws/hw_websocket_payloads.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import json
 from enum import Enum
 
-from homewizard_climate_ws.api.api import HomeWizardClimateApi
-from homewizard_climate_ws.model.climate_device import (
-        HomeWizardClimateDevice,
-        HomeWizardClimateDeviceType
-    )
+from homewizard_climate_websocket.api.api import HomeWizardClimateApi
+from homewizard_climate_websocket.model.climate_device import HomeWizardClimateDevice
+
 
 class HomeWizardClimateWSPayloads:
     def __init__(self, api: HomeWizardClimateApi, device: HomeWizardClimateDevice):
         self._device = device
         self._api = api
 
     def hello(self) -> str:
@@ -81,107 +79,41 @@
                         "path": "/state/target_temperature",
                         "value": temp,
                     }
                 ],
             }
         )
 
-    def set_target_humidity(self, humidity: int) -> str:
-        return json.dumps(
-            {
-                "device": self._device.identifier,
-                "type": "json_patch",
-                "patch": [
-                    {
-                        "op": "replace",
-                        "path": "/state/target_humidity",
-                        "value": humidity,
-                    }
-                ],
-            }
-        )
-
     def set_fan_speed(self, speed: int) -> str:
         return json.dumps(
             {
                 "device": self._device.identifier,
                 "type": "json_patch",
                 "patch": [
                     {"op": "replace", "path": "/state/fan_speed", "value": speed}
                 ],
             }
         )
-    
-    def set_speed(self, speed: int) -> str:
-        return json.dumps(
-            {
-                "device": self._device.identifier,
-                "type": "json_patch",
-                "patch": [
-                    {"op": "replace", "path": "/state/speed", "value": speed}
-                ],
-            }
-        )
-
-    def set_timer(self, timer: int) -> str:
-        return json.dumps(
-            {
-                "device": self._device.identifier,
-                "type": "json_patch",
-                "patch": [
-                    {"op": "replace", "path": "/state/timer", "value": timer}
-                ],
-            }
-        )
-
-    def set_mode(self, mode: str) -> str:
-        return json.dumps(
-            {
-                "device": self._device.identifier,
-                "type": "json_patch",
-                "patch": [
-                    {"op": "replace", "path": "/state/mode", "value": mode}
-                ],
-            }
-        )
-
-    def set_swing(self, value: bool) -> str:
-        return json.dumps(
-            {
-                "device": self._device.identifier,
-                "type": "json_patch",
-                "patch": [
-                    {"op": "replace", "path": "/state/swing", "value": value}
-                ],
-            }
-        )
 
     def turn_on_oscillate(self) -> str:
-        path = "/state/oscillate"
-        print(self._device.type)
-        if self._device.type == HomeWizardClimateDeviceType.FAN:
-            path = "/state/oscillation"
         return json.dumps(
             {
                 "device": self._device.identifier,
                 "type": "json_patch",
-                "patch": [{"op": "replace", "path": path, "value": True}],
+                "patch": [{"op": "replace", "path": "/state/oscillate", "value": True}],
             }
         )
 
     def turn_off_oscillate(self) -> str:
-        path = "/state/oscillate"
-        if self._device.type == HomeWizardClimateDeviceType.FAN:
-            path = "/state/oscillation"
         return json.dumps(
             {
                 "device": self._device.identifier,
                 "type": "json_patch",
                 "patch": [
-                    {"op": "replace", "path": path, "value": False}
+                    {"op": "replace", "path": "/state/oscillate", "value": False}
                 ],
             }
         )
 
 
 class HomeWizardClimateStatePath(Enum):
     CURRENT_TEMP = "/state/current_temperature"
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/PKG-INFO` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: homewizard-climate-ws
-Version: 0.0.21
+Version: 0.0.9
 Summary: API/Websocket to control Homewizard Climate devices
 Home-page: https://github.com/dennis1804/homewizard-climate-websocket
 Author: Dennis1804
 Author-email: dennis@de-jong.frl
 License: MIT license
 Keywords: homewizard_climate_ws
+Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: setup
 Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 # homewizard-climate-websocket
 
 API/Websocket to control Homewizard Climate devices
 
 ---
 
 This library allows you to control your Homewizard Climate devices. There are a multitude of brands that use Homewizard apps for their smart controls.
 
-This was developed in order to be used in a [Home Assistant](https://www.home-assistant.io/) integration. It has not been thoroughly tested or worked with as a standalone code.
+This was developed in oder to be used in a [Home Assistant](https://www.home-assistant.io/) integration. It has not been thoroughly tested or worked with as a standalone code.
 
 ### Supported Devices
 This library is in an early stage of development and only works for the following device types returned from the Homewizard Climate API:
 
 - `heaterfan`
-- `infraredheater`
-- `heater`
 
 It has been tested on the following devices (even though it might work on others too):
 - [Princess Smart Heating and Cooling Tower (01.347000.01.001)](https://www.princesshome.eu/en-gb/princess-01-347000-01-001-smart-heating-and-01.347000.01.001)
-- [Princess Smart Infrared Panel Heater 350 (01.343350.02.001)](https://www.princesshome.eu/en-gb/princess-01-343350-02-001-smart-infrared-panel-01.343350.02.001)
-- [Princess Smart Glass Panel Heater (01.342001.09.001)](https://www.princesshome.eu/en-gb/princess-01-342001-09-001-smart-glass-panel-heater-01.342001.09.001)
+
+![](https://www.princesshome.eu/product/image/large/01.347000.01.001_3.jpg)
 
 ## Quick start
 There's no separate `requirements.txt` file, the dependencies can be found and installed in `setup.py`
 
 ```
 username = os.environ["HW_CLIMATE_USERNAME"]
 password = os.environ["HW_CLIMATE_PASSWORD"]
@@ -64,7 +63,9 @@
 **Stable Release (PyPi):** `pip install homewizard_climate_websocket`<br>
 **Local Development:** `pip install .`
 
 ## Development
 Any help to increase the number of supported devices is much appreciated as I only had access to the one mentioned above.
 
 See [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
+
+
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/SOURCES.txt` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 homewizard_climate_ws/__init__.py
 homewizard_climate_ws/const.py
-homewizard_climate_ws/debug.py
 homewizard_climate_ws/main.py
 homewizard_climate_ws.egg-info/PKG-INFO
 homewizard_climate_ws.egg-info/SOURCES.txt
 homewizard_climate_ws.egg-info/dependency_links.txt
 homewizard_climate_ws.egg-info/not-zip-safe
 homewizard_climate_ws.egg-info/requires.txt
 homewizard_climate_ws.egg-info/top_level.txt
```

### Comparing `homewizard_climate_ws-0.0.21/homewizard_climate_ws.egg-info/requires.txt` & `homewizard_climate_ws-0.0.9/homewizard_climate_ws.egg-info/requires.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 dataclasses-json>=0.5.7
 requests>=2.28.0
 websocket-client>=1.1.0
 
 [all]
-dataclasses-json>=0.5.7
-requests>=2.28.0
-websocket-client>=1.1.0
-pytest-runner>=5.2
+Sphinx>=3.4.3
 black>=19.10b0
-codecov>=2.1.4
-flake8>=3.8.3
-flake8-debugger>=3.2.1
-pytest>=5.4.3
-pytest-cov>=2.9.0
-pytest-raises>=0.11
 bump2version>=1.0.1
+codecov>=2.1.4
 coverage>=5.1
+dataclasses-json>=0.5.7
+flake8-debugger>=3.2.1
+flake8>=3.8.3
 ipython>=7.15.0
 m2r2>=0.2.7
-Sphinx>=3.4.3
+pytest-cov>=2.9.0
+pytest-raises>=0.11
+pytest-runner>=5.2
+pytest-runner>=5.2
+pytest>=5.4.3
+requests>=2.28.0
 sphinx_rtd_theme>=0.5.1
 tox>=3.15.2
 twine>=3.1.1
+websocket-client>=1.1.0
 wheel>=0.34.2
 
 [dev]
-pytest-runner>=5.2
+Sphinx>=3.4.3
 black>=19.10b0
-codecov>=2.1.4
-flake8>=3.8.3
-flake8-debugger>=3.2.1
-pytest>=5.4.3
-pytest-cov>=2.9.0
-pytest-raises>=0.11
 bump2version>=1.0.1
+codecov>=2.1.4
 coverage>=5.1
+flake8-debugger>=3.2.1
+flake8>=3.8.3
 ipython>=7.15.0
 m2r2>=0.2.7
-Sphinx>=3.4.3
+pytest-cov>=2.9.0
+pytest-raises>=0.11
+pytest-runner>=5.2
+pytest-runner>=5.2
+pytest>=5.4.3
 sphinx_rtd_theme>=0.5.1
 tox>=3.15.2
 twine>=3.1.1
 wheel>=0.34.2
 
 [setup]
 pytest-runner>=5.2
 
 [test]
 black>=19.10b0
 codecov>=2.1.4
-flake8>=3.8.3
 flake8-debugger>=3.2.1
-pytest>=5.4.3
+flake8>=3.8.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
+pytest>=5.4.3
```

### Comparing `homewizard_climate_ws-0.0.21/setup.py` & `homewizard_climate_ws-0.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -78,16 +78,16 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="homewizard_climate_ws",
     name="homewizard_climate_ws",
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*"]),
     python_requires=">=3.7",
     setup_requires=setup_requirements,
-    test_suite="homewizard_climate_ws/tests",
+    test_suite="homewizard_climate_websocket/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/dennis1804/homewizard-climate-websocket",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="0.0.21",
+    version="0.0.9",
     zip_safe=False,
 )
```

### Comparing `homewizard_climate_ws-0.0.21/tests/conftest.py` & `homewizard_climate_ws-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

