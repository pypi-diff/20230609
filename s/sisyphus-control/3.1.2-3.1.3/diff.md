# Comparing `tmp/sisyphus_control-3.1.2-py3-none-any.whl.zip` & `tmp/sisyphus_control-3.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 12073 bytes, number of entries: 14
--rw-r--r--  2.0 unx      243 b- defN 20-Aug-31 01:46 sisyphus_control/__init__.py
--rw-r--r--  2.0 unx     4106 b- defN 21-Oct-20 19:49 sisyphus_control/data.py
--rw-r--r--  2.0 unx      638 b- defN 21-Oct-20 19:34 sisyphus_control/log.py
--rw-r--r--  2.0 unx     3279 b- defN 21-Oct-21 21:05 sisyphus_control/playlist.py
--rw-r--r--  2.0 unx        0 b- defN 21-Oct-20 02:07 sisyphus_control/py.typed
--rw-r--r--  2.0 unx       60 b- defN 21-Oct-20 18:12 sisyphus_control/sisbot_json.py
--rw-r--r--  2.0 unx    11434 b- defN 21-Oct-21 21:10 sisyphus_control/table.py
--rw-r--r--  2.0 unx     2093 b- defN 21-Oct-21 21:16 sisyphus_control/track.py
--rw-r--r--  2.0 unx     2951 b- defN 21-Oct-22 01:08 sisyphus_control/transport.py
--rw-r--r--  2.0 unx     1295 b- defN 21-Dec-13 17:42 sisyphus_control-3.1.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     2959 b- defN 21-Dec-13 17:42 sisyphus_control-3.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Dec-13 17:42 sisyphus_control-3.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 21-Dec-13 17:42 sisyphus_control-3.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1176 b- defN 21-Dec-13 17:42 sisyphus_control-3.1.2.dist-info/RECORD
-14 files, 30343 bytes uncompressed, 10103 bytes compressed:  66.7%
+Zip file size: 12351 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      243 b- defN 23-Jun-08 23:42 sisyphus_control/__init__.py
+-rw-r--r--  2.0 unx     4141 b- defN 23-Jun-08 23:56 sisyphus_control/data.py
+-rw-r--r--  2.0 unx      638 b- defN 23-Jun-08 23:42 sisyphus_control/log.py
+-rw-r--r--  2.0 unx     3279 b- defN 23-Jun-08 23:42 sisyphus_control/playlist.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 23:42 sisyphus_control/py.typed
+-rw-r--r--  2.0 unx       60 b- defN 23-Jun-08 23:42 sisyphus_control/sisbot_json.py
+-rw-r--r--  2.0 unx    11468 b- defN 23-Jun-08 23:57 sisyphus_control/table.py
+-rw-r--r--  2.0 unx     2093 b- defN 23-Jun-08 23:42 sisyphus_control/track.py
+-rw-r--r--  2.0 unx     2951 b- defN 23-Jun-08 23:42 sisyphus_control/transport.py
+-rw-r--r--  2.0 unx      228 b- defN 23-Jun-08 23:56 sisyphus_control/util.py
+-rw-r--r--  2.0 unx     1295 b- defN 23-Jun-09 00:13 sisyphus_control-3.1.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2922 b- defN 23-Jun-09 00:13 sisyphus_control-3.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 00:13 sisyphus_control-3.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-Jun-09 00:13 sisyphus_control-3.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1256 b- defN 23-Jun-09 00:13 sisyphus_control-3.1.3.dist-info/RECORD
+15 files, 30683 bytes uncompressed, 10257 bytes compressed:  66.6%
```

## zipnote {}

```diff
@@ -21,23 +21,26 @@
 
 Filename: sisyphus_control/track.py
 Comment: 
 
 Filename: sisyphus_control/transport.py
 Comment: 
 
-Filename: sisyphus_control-3.1.2.dist-info/LICENSE
+Filename: sisyphus_control/util.py
 Comment: 
 
-Filename: sisyphus_control-3.1.2.dist-info/METADATA
+Filename: sisyphus_control-3.1.3.dist-info/LICENSE
 Comment: 
 
-Filename: sisyphus_control-3.1.2.dist-info/WHEEL
+Filename: sisyphus_control-3.1.3.dist-info/METADATA
 Comment: 
 
-Filename: sisyphus_control-3.1.2.dist-info/top_level.txt
+Filename: sisyphus_control-3.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: sisyphus_control-3.1.2.dist-info/RECORD
+Filename: sisyphus_control-3.1.3.dist-info/top_level.txt
+Comment: 
+
+Filename: sisyphus_control-3.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sisyphus_control/data.py

```diff
@@ -1,11 +1,13 @@
 import asyncio
 from collections import UserDict
 from typing import TYPE_CHECKING, Any, Awaitable, Callable, Dict, List, Union
 
+from .util import ensure_coroutine
+
 CollectionListener = Union[Callable[[], None], Callable[[], Awaitable[None]]]
 
 
 class Model(UserDict):
     """Holds the data about one entity in a collection."""
 
     def __init__(self, data: Dict[str, Any]):
@@ -50,15 +52,15 @@
 
     def remove_listener(self, listener: CollectionListener) -> None:
         self._listeners.remove(listener)
 
     async def _notify_listeners(self) -> None:
         listeners = list(self._listeners)
         for listener in listeners:
-            await asyncio.coroutine(listener)()  # type: ignore
+            await ensure_coroutine(listener)()  # type: ignore
 
 
 if __name__ == "__main__":
     import aiounittest
     import unittest
     from unittest.mock import MagicMock
```

## sisyphus_control/table.py

```diff
@@ -9,14 +9,15 @@
 
 from .data import Collection, Model
 from .log import log_data_change
 from .playlist import Playlist
 from .sisbot_json import parse_bool
 from .track import Track
 from .transport import TableTransport, post
+from .util import ensure_coroutine
 
 
 _LOGGER = logging.getLogger("sisyphus-control")
 
 TableListenerType = Union[Callable[[], None], Callable[[], Awaitable[None]]]
 
 
@@ -279,15 +280,15 @@
 
     def remove_listener(self, listener: TableListenerType) -> None:
         self._listeners.remove(listener)
 
     async def _notify_listeners(self) -> None:
         listeners = list(self._listeners)
         for listener in listeners:
-            await asyncio.coroutine(listener)()  # type: ignore
+            await ensure_coroutine(listener)()  # type: ignore
         self._updated.set()
 
     def _get_transport(self) -> TableTransport:
         if self._transport is not None:
             return self._transport
 
         raise Exception("Table not connected")
```

## Comparing `sisyphus_control-3.1.2.dist-info/LICENSE` & `sisyphus_control-3.1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sisyphus_control-3.1.2.dist-info/METADATA` & `sisyphus_control-3.1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: sisyphus-control
-Version: 3.1.2
+Version: 3.1.3
 Summary: Control your Sisyphus kinetic art tables (sisyphus-industries.com)
 Home-page: https://github.com/jkeljo/sisyphus-control
 Author: Jonathan Keljo
-License: UNKNOWN
 Keywords: sisyphus
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Home Automation
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 License-File: LICENSE
@@ -82,9 +80,7 @@
 The following features would be reasonable to include; I'll happily accept pull requests:
 
 * Playlist editing
 * Upload tracks to table
 * Track thumbnail rendering
 * Table administration (wifi settings, etc.)
 * Interactions with Sisyphus cloud
-
-
```

## Comparing `sisyphus_control-3.1.2.dist-info/RECORD` & `sisyphus_control-3.1.3.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 sisyphus_control/__init__.py,sha256=aaa5Mp24pQ41Sr6pbiwJTnP5npL4xLc-50nECZ5Qk-0,243
-sisyphus_control/data.py,sha256=OE-ELLzChCIVx1PvjgCFyotiSTXGmCQWsaPck5NXDOk,4106
+sisyphus_control/data.py,sha256=6t5eP4d3F6TPov4vfZ392UeZriVu2ctVDT7CZrJt2xA,4141
 sisyphus_control/log.py,sha256=vvmUM53EkaMXJOCK9GnsA3mfiXlnHQ2dvI4EV-cVnIM,638
 sisyphus_control/playlist.py,sha256=otBm5sXOfvuqyiyoVSIbD207VfLfYk5aH1a0w3WtPcc,3279
 sisyphus_control/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sisyphus_control/sisbot_json.py,sha256=fYG2A8idSraJQ5LcTpfgG4PldUm_F8j8f41LlOztFCI,60
-sisyphus_control/table.py,sha256=YeaBR8rrRxx1sm0EqY1rY9Ge2S1D4yd2rGh7v84Qauw,11434
+sisyphus_control/table.py,sha256=mJE79H1S2Q0AYQngJQOojiTpRz5g3gU3sW546nG9gB4,11468
 sisyphus_control/track.py,sha256=oIbxfi3CQ6AoHtXLXsymCI5eByJy2XqrxjMsPN7rXWw,2093
 sisyphus_control/transport.py,sha256=IcqMqjyMSOn6ptADL0D_tYESwnY2Xw1u5XrbM9PxbvQ,2951
-sisyphus_control-3.1.2.dist-info/LICENSE,sha256=_sElxuLOa94e6FIeoGn52iXFn9LheCKNEkfezQlmbD4,1295
-sisyphus_control-3.1.2.dist-info/METADATA,sha256=MQwJmjorNYdsCWZGeV_I2EgRWeG_I8M39wIjQv9yODI,2959
-sisyphus_control-3.1.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
-sisyphus_control-3.1.2.dist-info/top_level.txt,sha256=TkeHhrFR5rfo1p_tifTHmz0Zo5kwt5p1yUlJ8n2Bd2I,17
-sisyphus_control-3.1.2.dist-info/RECORD,,
+sisyphus_control/util.py,sha256=MOea71X1PgTkAmGegtZ4RY5Qo2Q7C92PVqw5ky0159o,228
+sisyphus_control-3.1.3.dist-info/LICENSE,sha256=_sElxuLOa94e6FIeoGn52iXFn9LheCKNEkfezQlmbD4,1295
+sisyphus_control-3.1.3.dist-info/METADATA,sha256=kO8pTGF_BxpMKMkjin6xBhhmOJ9wF3xyLLgj52ZR1Sk,2922
+sisyphus_control-3.1.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sisyphus_control-3.1.3.dist-info/top_level.txt,sha256=TkeHhrFR5rfo1p_tifTHmz0Zo5kwt5p1yUlJ8n2Bd2I,17
+sisyphus_control-3.1.3.dist-info/RECORD,,
```

