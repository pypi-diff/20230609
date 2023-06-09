# Comparing `tmp/py-miraie-ac-0.0.5.tar.gz` & `tmp/py-miraie-ac-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.0.5.tar", last modified: Fri Jun  9 13:17:21 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.0.6.tar", last modified: Fri Jun  9 13:29:51 2023, max compression
```

## Comparing `py-miraie-ac-0.0.5.tar` & `py-miraie-ac-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 13:17:21.887318 py-miraie-ac-0.0.5/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1232 2023-06-09 13:17:21.887318 py-miraie-ac-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.5/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 07:29:23.000000 py-miraie-ac-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      744 2023-06-09 13:17:21.888328 py-miraie-ac-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 13:17:21.605459 py-miraie-ac-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 13:17:21.882318 py-miraie-ac-0.0.5/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6036 2023-06-05 04:01:19.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0     6210 2023-06-05 03:30:21.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/broker.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4494 2023-06-05 04:00:59.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      846 2023-06-05 03:53:39.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      470 2023-06-05 03:56:31.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-05 03:59:07.000000 py-miraie-ac-0.0.5/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-09 13:17:21.886322 py-miraie-ac-0.0.5/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1232 2023-06-09 13:17:21.000000 py-miraie-ac-0.0.5/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      505 2023-06-09 13:17:21.000000 py-miraie-ac-0.0.5/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 13:17:21.000000 py-miraie-ac-0.0.5/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-06-09 13:17:21.000000 py-miraie-ac-0.0.5/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.643589 py-miraie-ac-0.0.6/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1232 2023-06-09 13:29:51.643589 py-miraie-ac-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      625 2023-06-09 08:48:49.000000 py-miraie-ac-0.0.6/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 07:29:23.000000 py-miraie-ac-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      744 2023-06-09 13:29:51.645592 py-miraie-ac-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.621510 py-miraie-ac-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.638594 py-miraie-ac-0.0.6/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6172 2023-06-09 13:28:16.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6221 2023-06-09 13:28:36.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4542 2023-06-09 13:28:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      857 2023-06-09 13:29:04.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.0.6/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:29:51.643589 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1232 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      505 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-06-09 13:29:51.000000 py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.0.5/LICENSE` & `py-miraie-ac-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.5/PKG-INFO` & `py-miraie-ac-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.0.5/README.md` & `py-miraie-ac-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.5/setup.cfg` & `py-miraie-ac-0.0.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e35  .version = 0.0.5
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e36  .version = 0.0.6
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.0.5/src/py_miraie_ac/api.py` & `py-miraie-ac-0.0.6/src/py_miraie_ac/api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """The MirAIe API module"""
 
 import math
 import random
 import aiohttp
-from broker import MirAIeBroker
-import constants
-from device import Device
-from deviceStatus import DeviceStatus
-from enums import (
+from py_miraie_ac.constants import DEVICE_DETAILS_URL, HOMES_URL,HTTP_CLIENT_ID,LOGIN_URL,STATUS_URL
+from py_miraie_ac.broker import MirAIeBroker
+from py_miraie_ac.device import Device
+from py_miraie_ac.deviceStatus import DeviceStatus
+from py_miraie_ac.enums import (
     AuthType,
     DisplayState,
     FanMode,
     HVACMode,
     PowerMode,
     PresetMode,
     SwingMode,
 )
-from exceptions import AuthException
-from home import Home
-from user import User
-from utils import to_float
-
+from py_miraie_ac.exceptions import AuthException
+from py_miraie_ac.home import Home
+from py_miraie_ac.user import User
+from py_miraie_ac.utils import to_float
 
 class MirAIeAPI:
     """The MirAIe API class"""
     __auth_type: str
     __login_id: str
     __password: str
     __http_session: aiohttp.ClientSession
@@ -62,36 +61,36 @@
     async def reconnect_broker(self):
         """Authenticates with MirAIe and reconnects to MQTT server with the new credentials"""
         self.__user = await self.__login()
         self.__broker.reconnect(self.__user.access_token)
 
     async def __login(self):
         data = {
-            "clientId": constants.HTTP_CLIENT_ID,
+            "clientId": HTTP_CLIENT_ID,
             "password": self.__password,
             "scope": self.__get_scope(),
         }
 
         data[self.__auth_type] = self.__login_id
-        response = await self.__http_session.post(constants.LOGIN_URL, json=data)
+        response = await self.__http_session.post(LOGIN_URL, json=data)
 
         if response.status == 200:
             json = await response.json()
             return User(
                 access_token=json["accessToken"],
                 refresh_token=json["refreshToken"],
                 user_id=json["userId"],
                 expires_in=json["expiresIn"],
             )
 
         raise AuthException("Authentication failed")
 
     async def __get_home_details(self):
         response = await self.__http_session.get(
-            constants.HOMES_URL, headers=self.__build_http_headers()
+            HOMES_URL, headers=self.__build_http_headers()
         )
         resp = await response.json()
         return await self.__parse_home_details(resp[0])
 
     async def __parse_home_details(self, json_response):
         devices: list[Device] = []
 
@@ -123,29 +122,29 @@
                 self.__topics.append(device.status_topic)
                 self.__topics.append(device.connection_status_topic)
                 devices.append(device)
 
         return Home(home_id=json_response["homeId"], devices=devices)
 
     async def __get_device_details(self, device_id: str):
-        url = f"{constants.DEVICE_DETAILS_URL}/{device_id}"
+        url = f"{DEVICE_DETAILS_URL}/{device_id}"
 
         response = await self.__http_session.get(
             url,
             headers=self.__build_http_headers(),
         )
 
         json = await response.json()
         return json[0]
 
     async def __get_device_status(self, device_id: str):
         status: DeviceStatus
 
         response = await self.__http_session.get(
-            constants.STATUS_URL.replace("{deviceId}", device_id),
+            STATUS_URL.replace("{deviceId}", device_id),
             headers=self.__build_http_headers(),
         )
 
         json = await response.json()
         status = DeviceStatus(
             is_online=json["onlineStatus"] == "true",
             temperature=to_float(json["actmp"]),
```

### Comparing `py-miraie-ac-0.0.5/src/py_miraie_ac/broker.py` & `py-miraie-ac-0.0.6/src/py_miraie_ac/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 
 import json
 import math
 import random
 import ssl
 from paho.mqtt import client as paho
 
-from enums import FanMode, HVACMode, PowerMode, PresetMode, SwingMode
-
+from py_miraie_ac.enums import FanMode, HVACMode, PowerMode, PresetMode, SwingMode
 
 class MirAIeBroker:
     """The MirAIe Broker class"""
 
     __host: str = "mqtt.miraie.in"
     __port: int = 8883
     __username: str
```

### Comparing `py-miraie-ac-0.0.5/src/py_miraie_ac/device.py` & `py-miraie-ac-0.0.6/src/py_miraie_ac/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """The MirAIe device"""
 from typing import Callable
-from broker import MirAIeBroker
-from deviceStatus import DeviceStatus
-from enums import DisplayState, FanMode, HVACMode, PowerMode, PresetMode, SwingMode
-from utils import to_float
-
-
+from py_miraie_ac.broker import MirAIeBroker
+from py_miraie_ac.deviceStatus import DeviceStatus
+from py_miraie_ac.enums import DisplayState, FanMode, HVACMode, PowerMode, PresetMode, SwingMode
+from py_miraie_ac.utils import to_float
 
 class Device:
     """The MirAIe device class"""
 
     __broker: MirAIeBroker
 
     def __init__(
```

### Comparing `py-miraie-ac-0.0.5/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.0.6/src/py_miraie_ac/deviceStatus.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Represents the status of a device"""
-from enums import DisplayState, FanMode, HVACMode, PowerMode, PresetMode, SwingMode
-
+from py_miraie_ac.enums import DisplayState, FanMode, HVACMode, PowerMode, PresetMode, SwingMode
 
 class DeviceStatus:
     """The Device Status class"""
     def __init__(
         self,
         is_online: bool,
         temperature: float,
```

### Comparing `py-miraie-ac-0.0.5/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.0.6/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.0.5/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.0.6/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

