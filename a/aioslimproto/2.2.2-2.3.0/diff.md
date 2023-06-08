# Comparing `tmp/aioslimproto-2.2.2.tar.gz` & `tmp/aioslimproto-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioslimproto-2.2.2.tar", last modified: Wed May 31 11:54:06 2023, max compression
+gzip compressed data, was "aioslimproto-2.3.0.tar", last modified: Thu Jun  8 22:39:48 2023, max compression
```

## Comparing `aioslimproto-2.2.2.tar` & `aioslimproto-2.3.0.tar`

### file list

```diff
@@ -1,24 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:54:06.436145 aioslimproto-2.2.2/aioslimproto/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30608 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/aioslimproto/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/aioslimproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:54:06.000000 aioslimproto-2.2.2/aioslimproto.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-31 11:54:06.440146 aioslimproto-2.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-31 11:53:54.000000 aioslimproto-2.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.537163 aioslimproto-2.3.0/aioslimproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34338 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/aioslimproto/font/
+-rw-r--r--   0 runner    (1001) docker     (123)   480716 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   540048 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   448868 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   499228 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   438596 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   504492 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Condensed.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   309664 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-ExtraLight.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   201752 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Bold-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   289124 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   209552 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   303604 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Mono.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   475244 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans-Oblique.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   569008 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/font/DejaVu-Sans.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/visualisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/aioslimproto/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:39:48.537163 aioslimproto-2.3.0/aioslimproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:39:48.000000 aioslimproto-2.3.0/aioslimproto.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-08 22:39:48.545163 aioslimproto-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-08 22:39:37.000000 aioslimproto-2.3.0/setup.py
```

### Comparing `aioslimproto-2.2.2/LICENSE` & `aioslimproto-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.2/PKG-INFO` & `aioslimproto-2.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.2.2
+Version: 2.3.0
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.2.2/aioslimproto/cli.py` & `aioslimproto-2.3.0/aioslimproto/cli.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.2/aioslimproto/client.py` & `aioslimproto-2.3.0/aioslimproto/client.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,29 +3,33 @@
 
 Large parts of this code are based on code by Doug Winter, all rights reserved.
 https://github.com/winjer/squeal/blob/master/src/squeal/net/slimproto.py
 """
 from __future__ import annotations
 
 import asyncio
+import ipaddress
 import logging
 import socket
 import struct
 import time
 from asyncio import StreamReader, StreamWriter, create_task
-from collections import deque
-from enum import Enum
+from enum import Enum, IntEnum
 from typing import Callable, Dict, List, TypedDict
 from urllib.parse import parse_qsl, urlparse
 
 from async_timeout import timeout
 
-from .const import EventType
+from aioslimproto.display import SlimProtoDisplay
+
+from .const import FALLBACK_CODECS, EventType
 from .errors import UnsupportedContentType
 from .util import parse_capabilities, parse_headers
+from .visualisation import SpectrumAnalyser, VisualisationType
+from .volume import SlimProtoVolume
 
 # from http://wiki.slimdevices.com/index.php/SlimProtoTCPProtocol#HELO
 DEVICE_TYPE = {
     2: "squeezebox",
     3: "softsqueeze",
     4: "squeezebox2",
     5: "transporter",
@@ -42,26 +46,85 @@
 class PlayerState(Enum):
     """Enum with the possible player states."""
 
     PLAYING = "playing"
     STOPPED = "stopped"
     PAUSED = "paused"
     BUFFERING = "buffering"
+    BUFFER_READY = "buffer_ready"
 
 
 class TransitionType(Enum):
     """Transition type enum."""
 
     NONE = b"0"
     CROSSFADE = b"1"
     FADE_IN = b"2"
     FADE_OUT = b"3"
     FADE_IN_OUT = b"4"
 
 
+class RemoteCode(IntEnum):
+    """Enum with all (known) remote ir codes."""
+
+    SLEEP = 1988737095
+    POWER = 1988706495
+    REWIND = 1988739135
+    PAUSE = 1988698335
+    FORWARD = 1988730975
+    ADD = 1988714655
+    PLAY = 1988694255
+    UP = 1988747295
+    DOWN = 1988735055
+    LEFT = 1988726895
+    RIGHT = 1988743215
+    VOLUME_UP = 1988722815
+    VOLUME_DOWN = 1988690175
+    NUM_1 = 1988751375
+    NUM_2 = 1988692215
+    NUM_3 = 1988724855
+    NUM_4 = 1988708535
+    NUM_5 = 1988741175
+    NUM_6 = 1988700375
+    NUM_7 = 1988733015
+    NUM_8 = 1988716695
+    NUM_9 = 1988749335
+    NUM_0 = 1988728935
+    FAVORITES = 1988696295
+    SEARCH = 1988712615
+    BROWSE = 1988718735
+    SHUFFLE = 1988745255
+    REPEAT = 1988704455
+    NOW_PLAYING = 1988720775
+    SIZE = 1988753415
+    BRIGHTNESS = 1988691195
+
+
+class ButtonCode(IntEnum):
+    """Enum with all (known) button codes."""
+
+    POWER = 65546
+    PRESET_1 = 131104
+    PRESET_2 = 131105
+    PRESET_3 = 131106
+    PRESET_4 = 131107
+    PRESET_5 = 131108
+    PRESET_6 = 131109
+    BACK = 131085
+    PLAY = 131090
+    ADD = 131091
+    UP = 131083
+    OK = 131086
+    REWIND = 131088
+    PAUSE = 131095
+    FORWARD = 131101
+    VOLUME_DOWN = 131081
+    VOLUME_UP = 131082
+
+
 PCM_SAMPLE_SIZE = {
     # Map with sample sizes used in slimproto."""
     8: b"0",
     16: b"1",
     20: b"2",
     32: b"3",
     24: b"4",
@@ -121,15 +184,14 @@
     "dsf": b"p",
     "dff": b"p",
     "aif": b"p",
 }
 
 FALLBACK_MODEL = "Squeezebox"
 FALLLBACK_FIRMWARE = "Unknown"
-FALLBACK_CODECS = ["pcm"]
 FALLBACK_SAMPLE_RATE = 96000
 HEARTBEAT_INTERVAL = 5
 
 
 class Metadata(TypedDict):
     """Optional metadata for playback."""
 
@@ -156,32 +218,35 @@
         self.current_metadata: Metadata | None = None
         self._reader = reader
         self._writer = writer
         self._player_id: str = ""
         self._device_type: str = ""
         self._capabilities: Dict[str, str] = {}
         self._device_name: str = ""
-        self._volume_control = PySqueezeVolume()
+        self._volume_control = SlimProtoVolume()
+        self._display_control = SlimProtoDisplay()
         self._powered: bool = False
         self._muted: bool = False
         self._state = PlayerState.STOPPED
+        self._jiffies: int = 0
         self._last_timestamp: float = 0
         self._elapsed_milliseconds: float = 0
         self._next_url: str | None = None
         self._next_metadata: Metadata | None = None
         self._connected: bool = False
-        self._last_heartbeat = (0, 0)
-        self._packet_latency = deque(maxlen=10)
+        self._last_heartbeat = 0
         self._reader_task = create_task(self._socket_reader())
-        self._send_heartbeat()
+        self._heartbeat_task: asyncio.Task | None = None
 
     def disconnect(self) -> None:
         """Disconnect and/or cleanup socket client."""
         if self._reader_task and not self._reader_task.done():
             self._reader_task.cancel()
+        if self._heartbeat_task and not self._heartbeat_task.done():
+            self._heartbeat_task.cancel()
 
         if self._connected:
             self._connected = False
             if self._writer.can_write_eof():
                 self._writer.write_eof()
             self._writer.close()
 
@@ -268,53 +333,98 @@
         # if the player is playing we return a very accurate timestamp
         # which in turn can be used by consumers to sync players etc.
         return self._elapsed_milliseconds + int(
             (time.time() - self._last_timestamp) * 1000
         )
 
     @property
-    def packet_latency(self) -> float:
-        """Return (averaged) packet latency in seconds."""
-        if not self._packet_latency:
-            return 5  # return a safe default of 5ms
-        return sum(self._packet_latency) / len(self._packet_latency)
+    def jiffies(self) -> int:
+        """Return (realtime) epoch timestamp from player."""
+        return self._jiffies + int((time.time() - self._last_timestamp) * 1000)
 
     async def stop(self) -> None:
         """Send stop command to player."""
-        await self.send_strm(b"q")
+        await self.send_strm(b"q", flags=0)
+        await self.set_display()
+        # some players do not update their state by event so we force it here
+        if self._state != PlayerState.STOPPED:
+            self._state = PlayerState.STOPPED
+            self.callback(EventType.PLAYER_UPDATED, self)
 
     async def play(self) -> None:
         """Send play/unpause command to player."""
-        await self.send_strm(b"u")
+        await self.send_strm(b"u", flags=0)
+        # some players do not update their state by event so we force it here
+        if self._state == PlayerState.PAUSED:
+            self._state = PlayerState.PLAYING
+            self.callback(EventType.PLAYER_UPDATED, self)
 
     async def pause(self) -> None:
         """Send pause command to player."""
         await self.send_strm(b"p")
+        # some players do not update their state by event so we force it here
+        if self._state == PlayerState.PLAYING:
+            self._state = PlayerState.PAUSED
+            self.callback(EventType.PLAYER_UPDATED, self)
+
+    async def toggle_pause(self) -> None:
+        """Toggle play/pause command."""
+        if self.state == PlayerState.PLAYING:
+            await self.pause()
+        else:
+            await self.play()
 
     async def power(self, powered: bool = True) -> None:
         """Send power command to player."""
         # mute is the same as power
         if not powered:
             await self.stop()
         power_int = 1 if powered else 0
         await self._send_frame(b"aude", struct.pack("2B", power_int, 1))
         self._powered = powered
         self.callback(EventType.PLAYER_UPDATED, self)
+        await self.set_display()
+
+    async def toggle_power(self) -> None:
+        """Toggle power command."""
+        await self.power(not self.powered)
 
     async def volume_set(self, volume_level: int) -> None:
         """Send new volume level command to player."""
         self._volume_control.volume = volume_level
         old_gain = self._volume_control.old_gain()
         new_gain = self._volume_control.new_gain()
         await self._send_frame(
             b"audg",
             struct.pack("!LLBBLL", old_gain, old_gain, 1, 255, new_gain, new_gain),
         )
         self.callback(EventType.PLAYER_UPDATED, self)
 
+    async def volume_up(self) -> None:
+        """Send volume up command to player."""
+        self._volume_control.increment()
+        old_gain = self._volume_control.old_gain()
+        new_gain = self._volume_control.new_gain()
+        await self._send_frame(
+            b"audg",
+            struct.pack("!LLBBLL", old_gain, old_gain, 1, 255, new_gain, new_gain),
+        )
+        self.callback(EventType.PLAYER_UPDATED, self)
+
+    async def volume_down(self) -> None:
+        """Send volume down command to player."""
+        self._volume_control.decrement()
+        old_gain = self._volume_control.old_gain()
+        new_gain = self._volume_control.new_gain()
+        await self._send_frame(
+            b"audg",
+            struct.pack("!LLBBLL", old_gain, old_gain, 1, 255, new_gain, new_gain),
+        )
+        self.callback(EventType.PLAYER_UPDATED, self)
+
     async def mute(self, muted: bool = False) -> None:
         """Send mute command to player."""
         muted_int = 0 if muted else 1
         await self._send_frame(b"aude", struct.pack("2B", muted_int, 0))
         self._muted = muted
         self.callback(EventType.PLAYER_UPDATED, self)
 
@@ -322,14 +432,15 @@
         self,
         url: str,
         mime_type: str | None = None,
         metadata: Metadata | None = None,
         send_flush: bool = True,
         transition: TransitionType = TransitionType.NONE,
         transition_duration: int = 0,
+        autostart: bool = True,
     ) -> None:
         """Request player to start playing a single url."""
         self.logger.debug("play url: %s", url)
         if not url.startswith("http"):
             raise UnsupportedContentType(f"Invalid URL: {url}")
 
         if send_flush:
@@ -349,15 +460,14 @@
         host = parsed_uri.hostname
         port = parsed_uri.port
         path = parsed_uri.path
         if parsed_uri.query:
             path += f"?{parsed_uri.query}"
 
         ipaddr = socket.gethostbyname(host)
-        ipaddr_b = socket.inet_aton(ipaddr)
 
         if port is None and scheme == "https":
             port = 443
         elif port is None:
             port = 80
 
         if scheme == "https" and not self._capabilities.get("CanHTTPS"):
@@ -372,19 +482,15 @@
 
         if mime_type is None:
             # try to get the audio format from file extension
             ext = f'audio/{url.split(".")[-1]}'
             if ext in CODEC_MAPPING:
                 mime_type = ext
 
-        codec = CODEC_MAPPING.get(mime_type)
-        if codec is not None and codec not in self.supported_codecs:
-            raise UnsupportedContentType(
-                f"Player does not support content type: {mime_type}"
-            )
+        codec_details = self._parse_codc(mime_type)
 
         if port not in (80, 443, "80", "443"):
             host += f":{port}"
         httpreq = (
             b"GET %s HTTP/1.0\r\n"
             b"Host: %s\r\n"
             b"Connection: close\r\n"
@@ -393,35 +499,87 @@
             b"User-Agent: VLC/3.0.9 LibVLC/3.0.9\r\n"
             b"Range: bytes=0-\r\n"
             b"\r\n" % (path.encode(), host.encode())
         )
 
         await self.send_strm(
             command=b"s",
-            formatbyte=FORMAT_BYTE.get(codec, b"?"),
-            autostart=b"3",
+            codec_details=codec_details,
+            autostart=b"1" if autostart else b"0",
             server_port=port,
-            server_ip=ipaddr_b,
+            server_ip=int(ipaddress.ip_address(ipaddr)),
             threshold=200,
             output_threshold=10,
             trans_duration=transition_duration,
             trans_type=transition.value,
             flags=0x20 if scheme == "https" else 0x00,
             httpreq=httpreq,
         )
+        await self.set_display()
+
+    async def set_brightness(self, level=4):
+        """Set brightness command on (supported) display."""
+        assert 0 <= level <= 4
+        await self._send_frame(b"grfb", struct.pack("!H", level))
 
-    def _send_heartbeat(self) -> None:
-        """Send heartbeat message to player."""
+    async def set_visualisation(
+        self, visualisation: VisualisationType | None = None
+    ) -> None:
+        """Set Visualisation engine on player."""
+        if visualisation is None:
+            visualisation = SpectrumAnalyser()
 
-        async def async_send_heartbeat():
-            heartbeat_id = self._last_heartbeat[0] + 1
-            self._last_heartbeat = (heartbeat_id, time.time())
-            await self.send_strm(b"t", flags=0, replay_gain=heartbeat_id)
+        def _handle():
+            return visualisation.pack()
 
-        asyncio.create_task(async_send_heartbeat())
+        data = await asyncio.get_running_loop().run_in_executor(None, _handle)
+        await self._send_frame(b"visu", data)
+
+    async def render(
+        self,
+        text: str,
+        size: int = 16,
+        position: tuple[int, int] = (0, 0),
+        font: str = "DejaVu-Sans",
+    ) -> None:
+        """Render given text on display of (supported) slimproto client."""
+
+        def _render():
+            self._display_control.clear()
+            self._display_control.renderText(text, font, size, position)
+            return self._display_control.frame()
+
+        bitmap = await asyncio.get_running_loop().run_in_executor(None, _render)
+        await self._update_display(bitmap)
+
+    async def set_display(self) -> None:
+        """Render default text on player display."""
+        await self.set_visualisation()
+        if not self.powered:
+            await self.render("")
+        elif self._next_metadata and "title" in self._next_metadata:
+            await self.render(self._next_metadata["title"])
+        else:
+            await self.render(self.name)
+
+    async def _update_display(
+        self, bitmap: bytes, transition: str = "c", offset: int = 0, param: int = 0
+    ) -> None:
+        """Update display of (supported) slimproto client."""
+        frame = struct.pack("!Hcb", offset, transition.encode(), param) + bitmap
+        await self._send_frame(b"grfe", frame)
+
+    async def _send_heartbeat(self) -> None:
+        """Send periodic heartbeat message to player."""
+        while self.connected:
+            self._last_heartbeat = heartbeat_id = self._last_heartbeat + 1
+            await self.send_strm(
+                b"t", autostart=b"0", flags=0, replay_gain=heartbeat_id
+            )
+            await asyncio.sleep(5)
 
     async def _send_frame(self, command: bytes, data: bytes) -> None:
         """Send command to Squeeze player."""
         if self._reader.at_eof() or self._writer.is_closing():
             self.logger.debug("Socket is disconnected.")
             self.disconnect()
             return
@@ -465,77 +623,154 @@
         )
         self.callback(EventType.PLAYER_DISCONNECTED, self)
         self.disconnect()
 
     async def send_strm(
         self,
         command=b"q",
-        formatbyte=b"?",
         autostart=b"0",
-        samplesize=b"?",
-        samplerate=b"?",
-        channels=b"?",
-        endian=b"?",
-        threshold=0,
+        codec_details=b"p1321",
+        threshold=255,
         spdif=b"0",
         trans_duration=0,
         trans_type=b"0",
-        flags=0x20,
+        flags=0x40,
         output_threshold=0,
         replay_gain=0,
         server_port=0,
-        server_ip=b"0",
+        server_ip=0,
         httpreq=b"",
     ) -> None:
         """Create stream request message based on given arguments."""
         data = struct.pack(
-            "!cccccccBcBcBBBLH",
+            "!cc5sBcBcBBBLHL",
             command,
             autostart,
-            formatbyte,
-            samplesize,
-            samplerate,
-            channels,
-            endian,
+            codec_details,
             threshold,
             spdif,
             trans_duration,
             trans_type,
             flags,
             output_threshold,
             0,
             replay_gain,
             server_port,
+            server_ip,
         )
-        await self._send_frame(b"strm", data + server_ip + httpreq)
+        await self._send_frame(b"strm", data + httpreq)
 
     async def _process_helo(self, data: bytes) -> None:
         """Process incoming HELO event from player (player connected)."""
         self.logger.debug("HELO received: %s", data)
         # player connected, sends helo info message
         (dev_id, _, mac) = struct.unpack("BB6s", data[:8])
         # pylint: disable = consider-using-f-string
         device_mac = ":".join("%02x" % x for x in mac)
         self._player_id = str(device_mac).lower()
         self._device_type = DEVICE_TYPE.get(dev_id, "unknown device")
         self._capabilities = parse_capabilities(data)
         self.logger.debug("Player connected: %s", self.player_id)
         # Set some startup settings for the player
-        await self._send_frame(b"vers", b"7.8")
+        await self._send_frame(b"vers", b"7.999.999")
+        await self.stop()
+        await self.set_brightness()
+        await self.set_visualisation()
         await self._send_frame(b"setd", struct.pack("B", 0))
         await self._send_frame(b"setd", struct.pack("B", 4))
         await self.stop()
         # restore last power and volume levels
         # NOTE: this can be improved by storing the previous volume/power levels
         # so they can be restored when the player (re)connects.
         await self.power(self._powered)
         await self.volume_set(self.volume_level)
         self._connected = True
+        await self.set_display()
+        self._heartbeat_task = asyncio.create_task(self._send_heartbeat())
         self.callback(EventType.PLAYER_CONNECTED, self)
 
+    def _process_butn(self, data: bytes) -> None:
+        """Handle 'butn' command from client."""
+        timestamp, button = struct.unpack("!LL", data)
+        # handle common buttons
+        if button == ButtonCode.POWER:
+            asyncio.create_task(self.toggle_power())
+            return
+        if button == ButtonCode.PAUSE:
+            asyncio.create_task(self.toggle_pause())
+            return
+        if button == ButtonCode.PLAY:
+            asyncio.create_task(self.play())
+            return
+        if button == ButtonCode.VOLUME_DOWN:
+            asyncio.create_task(self.volume_down())
+            return
+        if button == ButtonCode.VOLUME_UP:
+            asyncio.create_task(self.volume_up())
+            return
+        # forward all other
+        self.callback(
+            EventType.PLAYER_BTN_EVENT,
+            self,
+            {
+                "type": "butn",
+                "timestamp": timestamp,
+                "button": button,
+            },
+        )
+
+    def _process_knob(self, data: bytes) -> None:
+        """Handle 'knob' command from client."""
+        timestamp, position, sync = struct.unpack("!LLB", data)
+        self.callback(
+            EventType.PLAYER_BTN_EVENT,
+            self,
+            {
+                "type": "knob",
+                "timestamp": timestamp,
+                "position": position,
+                "sync": sync,
+            },
+        )
+
+    def _process_ir(self, data: bytes) -> None:
+        """Handle 'ir' command from client."""
+        # format for IR:
+        # [4]   time since startup in ticks (1KHz)
+        # [1]	code format
+        # [1]	number of bits
+        # [4]   the IR code, up to 32 bits
+        timestamp, code = struct.unpack("!LxxL", data)
+        # handle common buttons
+        if code == RemoteCode.POWER:
+            asyncio.create_task(self.toggle_power())
+            return
+        if code == RemoteCode.PAUSE:
+            asyncio.create_task(self.toggle_pause())
+            return
+        if code == RemoteCode.PLAY:
+            asyncio.create_task(self.play())
+            return
+        if code == RemoteCode.VOLUME_DOWN:
+            asyncio.create_task(self.volume_down())
+            return
+        if code == RemoteCode.VOLUME_UP:
+            asyncio.create_task(self.volume_up())
+            return
+        # forward all other
+        self.callback(
+            EventType.PLAYER_BTN_EVENT,
+            self,
+            {
+                "type": "ir",
+                "timestamp": timestamp,
+                "code": code,
+            },
+        )
+
     def _process_stat(self, data: bytes) -> None:
         """Redirect incoming STAT event from player to correct method."""
         event = data[:4].decode()
         event_data = data[4:]
         # pylint: disable = consider-using-f-string
         if event == b"\x00\x00\x00\x00":
             # Presumed informational stat message
@@ -544,19 +779,15 @@
         if event_handler is None:
             self.logger.debug("Unhandled event: %s - event_data: %s", event, event_data)
         else:
             asyncio.get_running_loop().call_soon(event_handler, data[4:])
 
     def _process_stat_aude(self, data: bytes) -> None:
         """Process incoming stat AUDe message (power level and mute)."""
-        (spdif_enable, dac_enable) = struct.unpack("2B", data[:2])
-        powered = spdif_enable or dac_enable
-        self._powered = powered
-        self._muted = not powered
-        self.callback(EventType.PLAYER_UPDATED, self)
+        # ignore this event (and use optimistic state instead), is is flaky across players
 
     def _process_stat_audg(self, data: bytes) -> None:
         """Process incoming stat AUDg message."""
         # srtm-s command received.
         # Some players may send this as aknowledge of volume change (audg command).
 
     def _process_stat_stmc(self, data: bytes) -> None:
@@ -629,33 +860,17 @@
             output_buffer_readyness,
             elapsed_seconds,
             voltage,
             elapsed_milliseconds,
             server_heartbeat,
         ) = struct.unpack("!BBBLLLLHLLLLHLL", data[:47])
 
-        # handle heartbeat response (used to measure roundtrip/latency and ping/pong)
-        if server_heartbeat == self._last_heartbeat[0]:
-            # consider latency as half of the roundtrip
-            latency = (time.time() - self._last_heartbeat[1]) / 2
-            self._packet_latency.append(latency)
-            # schedule heartbeat
-            # if playback busy we want high accuracy
-            # but otherwise every 5 seconds is good enough
-            if self.state == PlayerState.PLAYING:
-                heartbeat_delay = 0.1
-            elif self.powered:
-                heartbeat_delay = 1
-            else:
-                heartbeat_delay = HEARTBEAT_INTERVAL
-            asyncio.get_event_loop().call_later(heartbeat_delay, self._send_heartbeat)
-
+        self._jiffies = jiffies
         self._elapsed_milliseconds = elapsed_milliseconds
-        # consider latency when calculating the elapsed time
-        self._last_timestamp = time.time() - self.packet_latency
+        self._last_timestamp = time.time()
         self.callback(EventType.PLAYER_HEARTBEAT, self)
 
     def _process_stat_stmu(self, data: bytes) -> None:
         """Process incoming stat STMu message: Buffer underrun: Normal end of playback."""
         # pylint: disable=unused-argument
         self.logger.debug("STMu received - end of playback.")
         self._state = PlayerState.STOPPED
@@ -667,15 +882,16 @@
         self.callback(EventType.PLAYER_UPDATED, self)
 
     def _process_stat_stml(self, data: bytes) -> None:
         """Process incoming stat STMl message: Buffer threshold reached."""
         # pylint: disable=unused-argument
         self.logger.debug("STMl received - Buffer threshold reached.")
         # this is only used when autostart < 2 on strm-s commands
-        # send an event anyway for lib consumers to handle
+        # send an event for lib consumers to handle
+        self._state = PlayerState.BUFFER_READY
         self.callback(EventType.PLAYER_BUFFER_READY, self)
 
     def _process_stat_stmn(self, data: bytes) -> None:
         """Process incoming stat STMn message: player couldn't decode stream."""
         # pylint: disable=unused-argument
         self.logger.debug("STMn received - player couldn't decode stream.")
         self.callback(EventType.PLAYER_DECODER_ERROR, self)
@@ -693,238 +909,75 @@
                 self.logger.error("Server requires HTTPS.")
             else:
                 await self.play_url(location)
             return
 
         if "content-type" in headers:
             content_type = headers.get("content-type")
-            if "wav" in content_type:
-                # wave header may contain info about sample rate etc
-                # https://www.dialogic.com/webhelp/CSP1010/VXML1.1CI/WebHelp/standards_defaults%20-%20MIME%20Type%20Mapping.htm
-                if ";" in content_type:
-                    params = dict(parse_qsl(content_type.replace(";", "&")))
-                else:
-                    params = {}
-                sample_rate = int(params.get("rate", 44100))
-                sample_size = int(params.get("bitrate", 16))
-                channels = int(params.get("channels", 2))
-                codc_msg = (
-                    b"p"
-                    + PCM_SAMPLE_SIZE[sample_size]
-                    + PCM_SAMPLE_RATE[sample_rate]
-                    + str(channels).encode()
-                    + b"1"
-                )
-            elif content_type not in CODEC_MAPPING:
-                # use m as default/fallback
-                self.logger.debug(
-                    "Unable to parse mime type %s, using mp3 as default codec",
-                    content_type,
-                )
-                codc_msg = b"m????"
-            else:
-                # regular contenttype
-                codec = CODEC_MAPPING[content_type]
-                if codec not in self.supported_codecs:
-                    raise UnsupportedContentType(
-                        f"Player does not support content type: {content_type}"
-                    )
-                if content_type in ("audio/aac", "audio/aacp"):
-                    # https://wiki.slimdevices.com/index.php/SlimProto_TCP_protocol.html#AAC-specific_notes
-                    codc_msg = b"a2???"
-                else:
-                    codc_msg = FORMAT_BYTE[codec] + b"????"
+            codc_msg = self._parse_codc(content_type)
 
             # send the codc message to the player to inform about the codec that needs to be used
             self.logger.debug(
                 "send CODC for contenttype %s: %s", content_type, codc_msg
             )
             await self._send_frame(b"codc", codc_msg)
 
         # send continue (used when autoplay 1 or 3)
-        await self._send_frame(b"cont", b"1")
+        # await self._send_frame(b"cont", b"1")
 
     def _process_setd(self, data: bytes) -> None:
         """Process incoming SETD message: Get/set player firmware settings."""
         data_id = data[0]
         if data_id == 0:
             # received player name
             self._device_name = data[1:-1].decode()
             self.callback(EventType.PLAYER_NAME_RECEIVED, self)
             self.logger = logging.getLogger(__name__).getChild(self._device_name)
 
-
-class PySqueezeVolume:
-    """Represents a sound volume. This is an awful lot more complex than it sounds."""
-
-    minimum = 0
-    maximum = 100
-    step = 1
-
-    # this map is taken from Slim::Player::Squeezebox2 in the squeezecenter source
-    # i don't know how much magic it contains, or any way I can test it
-    old_map = [
-        0,
-        1,
-        1,
-        1,
-        2,
-        2,
-        2,
-        3,
-        3,
-        4,
-        5,
-        5,
-        6,
-        6,
-        7,
-        8,
-        9,
-        9,
-        10,
-        11,
-        12,
-        13,
-        14,
-        15,
-        16,
-        16,
-        17,
-        18,
-        19,
-        20,
-        22,
-        23,
-        24,
-        25,
-        26,
-        27,
-        28,
-        29,
-        30,
-        32,
-        33,
-        34,
-        35,
-        37,
-        38,
-        39,
-        40,
-        42,
-        43,
-        44,
-        46,
-        47,
-        48,
-        50,
-        51,
-        53,
-        54,
-        56,
-        57,
-        59,
-        60,
-        61,
-        63,
-        65,
-        66,
-        68,
-        69,
-        71,
-        72,
-        74,
-        75,
-        77,
-        79,
-        80,
-        82,
-        84,
-        85,
-        87,
-        89,
-        90,
-        92,
-        94,
-        96,
-        97,
-        99,
-        101,
-        103,
-        104,
-        106,
-        108,
-        110,
-        112,
-        113,
-        115,
-        117,
-        119,
-        121,
-        123,
-        125,
-        127,
-        128,
-    ]
-
-    # new gain parameters, from the same place
-    total_volume_range = -50  # dB
-    step_point = (
-        -1
-    )  # Number of steps, up from the bottom, where a 2nd volume ramp kicks in.
-    step_fraction = (
-        1  # fraction of totalVolumeRange where alternate volume ramp kicks in.
-    )
-
-    def __init__(self):
-        """Initialize class."""
-        self.volume = 50
-
-    def increment(self):
-        """Increment the volume."""
-        self.volume += self.step
-        if self.volume > self.maximum:
-            self.volume = self.maximum
-
-    def decrement(self):
-        """Decrement the volume."""
-        self.volume -= self.step
-        if self.volume < self.minimum:
-            self.volume = self.minimum
-
-    def old_gain(self):
-        """Return the "Old" gain value as required by the squeezebox."""
-        return self.old_map[self.volume]
-
-    def decibels(self):
-        """Return the "new" gain value."""
-        # pylint: disable=invalid-name
-
-        step_db = self.total_volume_range * self.step_fraction
-        max_volume_db = 0  # different on the boom?
-
-        # Equation for a line:
-        # y = mx+b
-        # y1 = mx1+b, y2 = mx2+b.
-        # y2-y1 = m(x2 - x1)
-        # y2 = m(x2 - x1) + y1
-        slope_high = max_volume_db - step_db / (100.0 - self.step_point)
-        slope_low = step_db - self.total_volume_range / (self.step_point - 0.0)
-        x2 = self.volume
-        if x2 > self.step_point:
-            m = slope_high
-            x1 = 100
-            y1 = max_volume_db
+    def _parse_codc(self, content_type: str) -> bytes:
+        """Parse CODEC details from mime/content type string."""
+        if "wav" in content_type or "pcm" in content_type:
+            # wave header may contain info about sample rate etc
+            # https://www.dialogic.com/webhelp/CSP1010/VXML1.1CI/WebHelp/standards_defaults%20-%20MIME%20Type%20Mapping.htm
+            if ";" in content_type:
+                params = dict(parse_qsl(content_type.replace(";", "&")))
+            else:
+                params = {}
+            sample_rate = int(params.get("rate", 44100))
+            sample_size = int(params.get("bitrate", 16))
+            channels = int(params.get("channels", 2))
+            codc_msg = (
+                b"p"
+                + PCM_SAMPLE_SIZE[sample_size]
+                + PCM_SAMPLE_RATE[sample_rate]
+                + str(channels).encode()
+                + b"1"  # endianness
+            )
+            codc_msg = struct.pack(
+                "ccccc",
+                b"p",
+                PCM_SAMPLE_SIZE[sample_size],
+                PCM_SAMPLE_RATE[sample_rate],
+                str(channels).encode(),
+                b"1",
+            )
+        elif content_type not in CODEC_MAPPING:
+            # use m as default/fallback
+            self.logger.debug(
+                "Unable to parse mime type %s, using mp3 as default codec",
+                content_type,
+            )
+            codc_msg = b"m????"
         else:
-            m = slope_low
-            x1 = 0
-            y1 = self.total_volume_range
-        return m * (x2 - x1) + y1
-
-    def new_gain(self):
-        """Return new gainvalue of the volume control."""
-        decibel = self.decibels()
-        floatmult = 10 ** (decibel / 20.0)
-        # avoid rounding errors somehow
-        if -30 <= decibel <= 0:
-            return int(floatmult * (1 << 8) + 0.5) * (1 << 8)
-        return int((floatmult * (1 << 16)) + 0.5)
+            # regular contenttype
+            codec = CODEC_MAPPING[content_type]
+            if codec not in self.supported_codecs:
+                self.logger.warning(
+                    "Player did report support for content_type %s, playback might fail",
+                    content_type,
+                )
+            if content_type in ("audio/aac", "audio/aacp"):
+                # https://wiki.slimdevices.com/index.php/SlimProto_TCP_protocol.html#AAC-specific_notes
+                codc_msg = b"a2???"
+            else:
+                codc_msg = FORMAT_BYTE[codec] + b"????"
+        return codc_msg
```

### Comparing `aioslimproto-2.2.2/aioslimproto/const.py` & `aioslimproto-2.3.0/aioslimproto/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,30 +3,32 @@
 
 from dataclasses import dataclass
 from enum import Enum
 from typing import Any, Dict, Optional
 
 
 class EventType(Enum):
-    """Enum with possible slim proto server events."""
+    """Enum with possible slim proto client events."""
 
     PLAYER_UPDATED = "player_updated"
     PLAYER_HEARTBEAT = "player_heartbeat"
     PLAYER_CONNECTED = "player_connected"
     PLAYER_DISCONNECTED = "player_disconnected"
     PLAYER_NAME_RECEIVED = "player_name_received"
-    PLAYER_DECODER_READY = "decoder_ready"
-    PLAYER_DECODER_ERROR = "decoder_error"
-    PLAYER_BUFFER_READY = "buffer_ready"
+    PLAYER_DECODER_READY = "player_decoder_ready"
+    PLAYER_DECODER_ERROR = "player_decoder_error"
+    PLAYER_BUFFER_READY = "player_buffer_ready"
     PLAYER_CLI_EVENT = "player_cli_event"
+    PLAYER_BTN_EVENT = "player_btn_event"
 
 
 @dataclass
 class SlimEvent:
     """Representation of an Event emitted by/on behalf of a player."""
 
     type: EventType
     player_id: str
     data: Optional[Dict[str, Any]] = None
 
 
 SLIMPROTO_PORT = 3483
+FALLBACK_CODECS = ["pcm", "mp3"]
```

### Comparing `aioslimproto-2.2.2/aioslimproto/discovery.py` & `aioslimproto-2.3.0/aioslimproto/discovery.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,148 +1,108 @@
-"""Logic for discovering slimproto clients on the local network."""
+"""Logic for slimproto clients to discover our (emulated) server on the local network."""
 from __future__ import annotations
 
 import asyncio
 import logging
 import socket
 import struct
 from collections import OrderedDict
-from typing import Optional
-
-from .util import get_hostname, get_ip
 
 LOGGER = logging.getLogger(__name__)
 
 # pylint:disable=consider-using-f-string
 
 
 async def start_discovery(
-    control_port: int, cli_port: Optional[int], cli_port_json: Optional[int]
+    ip_address: str,
+    control_port: int,
+    cli_port: int | None,
+    cli_port_json: int | None,
+    name: str = "Slimproto",
+    uuid: str = "slimproto",
 ) -> asyncio.BaseTransport:
     """Start discovery for players."""
     loop = asyncio.get_running_loop()
     transport, _ = await loop.create_datagram_endpoint(
-        lambda: DiscoveryProtocol(control_port, cli_port, cli_port_json),
+        lambda: DiscoveryProtocol(
+            ip_address, control_port, cli_port, cli_port_json, name, uuid
+        ),
         local_addr=("0.0.0.0", control_port),
     )
     return transport
 
 
-class Datagram:
-    """Description of a discovery datagram."""
-
-    @classmethod
-    def decode(cls, data):
-        """Decode a datagram message."""
-        data = data.decode(errors="replace")
-        if data[0] == "e":
-            return TLVDiscoveryRequestDatagram(data)
-        if data[0] == "E":
-            return TLVDiscoveryResponseDatagram(data)
-        if data[0] == "d":
-            return ClientDiscoveryDatagram(data)
-        if data[0] == "h":
-            pass  # Hello!
-        if data[0] == "i":
-            pass  # IR
-        if data[0] == "2":
-            pass  # i2c?
-        if data[0] == "a":
-            pass  # ack!
-
-
-class ClientDiscoveryDatagram(Datagram):
+class ClientDiscoveryDatagram:
     """Description of a client discovery datagram."""
 
     device = None
     firmware = None
     client = None
 
     def __init__(self, data):
         """Initialize class."""
-        msg = struct.unpack("!cxBB8x6B", data.encode())
+        msg = struct.unpack("!cxBB8x6B", data)
         self.device = msg[1]
         self.firmware = hex(msg[2])
-        self.client = ":".join(["%02x" % (x,) for x in msg[3:]])
+        self.client = ":".join([f"{x:02x}" for x in msg[3:]])
 
     def __repr__(self):
         """Print the class contents."""
-        return "<%s device=%r firmware=%r client=%r>" % (
+        return "<{} device={!r} firmware={!r} client={!r}>".format(
             self.__class__.__name__,
             self.device,
             self.firmware,
             self.client,
         )
 
 
-class DiscoveryResponseDatagram(Datagram):
-    """Description of a discovery response datagram."""
-
-    def __init__(self, hostname, port):
-        """Initialize class."""
-        # pylint: disable=unused-argument
-        hostname = hostname[:16].encode("UTF-8")
-        hostname += (16 - len(hostname)) * "\x00"
-        self.packet = struct.pack("!c16s", "D", hostname).decode()
-
-
-class TLVDiscoveryRequestDatagram(Datagram):
+class TLVDiscoveryRequestDatagram:
     """Description of a discovery request datagram."""
 
-    def __init__(self, data):
+    def __init__(self, data: str):
         """Initialize class."""
         requestdata = OrderedDict()
-        idx = 1
+        idx = 0
         length = len(data) - 5
         while idx <= length:
-            typ, _len = struct.unpack_from("4sB", data.encode(), idx)
+            key, _len = struct.unpack_from("4sB", data.encode(), idx)
             if _len:
                 val = data[idx + 5 : idx + 5 + _len]
                 idx += 5 + _len
             else:
                 val = None
                 idx += 5
-            typ = typ.decode()
-            requestdata[typ] = val
+            key = key.decode()
+            requestdata[key] = val
         self.data = requestdata
 
     def __repr__(self):
         """Pretty print class."""
-        return "<%s data=%r>" % (self.__class__.__name__, self.data.items())
-
-
-class TLVDiscoveryResponseDatagram(Datagram):
-    """Description of a TLV discovery response datagram."""
-
-    def __init__(self, responsedata):
-        """Initialize class."""
-        parts = ["E"]  # new discovery format
-        for typ, value in responsedata.items():
-            if value is None:
-                value = ""
-            elif len(value) > 255:
-                # Response too long, truncating to 255 bytes
-                value = value[:255]
-            parts.extend((typ, chr(len(value)), value))
-        self.packet = "".join(parts)
+        return f"<{self.__class__.__name__} data={self.data.items()!r}>"
 
 
 class DiscoveryProtocol:
     """Description of a discovery protocol."""
 
     def __init__(
         self,
+        ip_address: str,
         control_port: int,
-        cli_port: Optional[int],
-        cli_port_json: Optional[int],
+        cli_port: int | None,
+        cli_port_json: int | None,
+        name: str,
+        uuid: str,
     ):
         """Initialze class."""
+        self.ip_address = ip_address
         self.control_port = control_port
         self.cli_port = cli_port
         self.cli_port_json = cli_port_json
+        self.name = name
+        self.uuid = uuid
         self.transport = None
 
     def connection_made(self, transport):
         """Call on connection."""
         self.transport = transport
         # Allow receiving multicast broadcasts
         sock = self.transport.get_extra_info("socket")
@@ -157,68 +117,84 @@
 
     @classmethod
     def connection_lost(cls, *args, **kwargs):
         """Call on Connection lost."""
         # pylint: disable=unused-argument
         LOGGER.debug("Connection lost to discovery")
 
-    def build_tlv_response(self, requestdata):
+    def build_tlv_response(
+        self, requestdata: OrderedDict[str, str]
+    ) -> OrderedDict[str, str]:
         """Build TLV Response message."""
         responsedata = OrderedDict()
-        for typ, value in requestdata.items():
-            if typ == "NAME":
-                # send full host name - no truncation
-                value = get_hostname()
-            elif typ == "IPAD":
-                value = get_ip()
-                # :todo: IPv6
-                if value == "0.0.0.0":
-                    # do not send back an ip address
-                    typ = None
-            elif typ == "JSON" and self.cli_port_json is not None:
+        for key in requestdata:
+            if key == "NAME":
+                responsedata[key] = self.name
+            elif key == "IPAD":
+                responsedata[key] = self.ip_address
+            elif key == "JSON" and self.cli_port_json is not None:
                 # send port as a string
-                value = str(self.cli_port_json)
-            elif typ == "CLIP" and self.cli_port is not None:
+                responsedata[key] = str(self.cli_port_json)
+            elif key == "CLIP" and self.cli_port is not None:
                 # send port as a string
-                value = str(self.cli_port)
-            elif typ == "VERS":
+                responsedata[key] = str(self.cli_port)
+            elif key == "VERS":
                 # send server version
-                value = "7.9"
-            elif typ == "UUID":
+                responsedata[key] = "7.999.999"
+            elif key == "UUID":
                 # send server uuid
-                value = "aioslimproto"
-            elif typ == "JVID":
-                # send server JVID
-                value = "aioslimproto"
-            else:
-                LOGGER.debug("Unexpected information request: %r", typ)
-                typ = None
-            if typ:
-                responsedata[typ] = value
+                responsedata[key] = self.uuid
         return responsedata
 
-    def datagram_received(self, data, addr):
-        """Datagram received callback."""
+    def datagram_received(self, data: bytes, addr: tuple[str, int]) -> None:
+        """Handle Datagram received callback."""
         # pylint: disable=broad-except
         try:
-            dgram = Datagram.decode(data)
-            if isinstance(dgram, ClientDiscoveryDatagram):
+            # tlv discovery request
+            if data.startswith(b"e"):
+                # Discovery request and responses contain TLVs of the format:
+                # T (4 bytes), L (1 byte unsigned), V (0-255 bytes)
+                # To escape from previous discovery format,
+                # request are prepended by 'e', responses by 'E'
+                # strip leading char of the datagram message
+                decoded_data = data.decode("utf-8")[1:]
+                dgram = TLVDiscoveryRequestDatagram(decoded_data)
+                requestdata = self.build_tlv_response(dgram.data)
+                self.send_tlv_discovery_response(requestdata, addr)
+            # udp/legacy discovery request
+            if data.startswith(b"d"):
+                # Discovery request: note that SliMP3 sends deviceid and revision in the discovery
+                # request, but the revision is wrong (v 2.2 sends revision 1.1). Oops.
+                # also, it does not send the MAC address until the [h]ello packet.
+                # Squeezebox sends all fields correctly.
+                dgram = ClientDiscoveryDatagram(data)
                 self.send_discovery_response(addr)
-            elif isinstance(dgram, TLVDiscoveryRequestDatagram):
-                resonsedata = self.build_tlv_response(dgram.data)
-                self.send_tlv_discovery_response(resonsedata, addr)
+            # NOTE: ignore all other such as slimp3 - that is simply too old
         except Exception:
             LOGGER.exception(
                 "Error occured while trying to parse a datagram from %s - data: %s",
                 addr,
                 data,
             )
 
-    def send_discovery_response(self, addr):
+    def send_discovery_response(self, addr: tuple[str, int]) -> None:
         """Send discovery response message."""
-        dgram = DiscoveryResponseDatagram(get_hostname(), self.control_port)
-        self.transport.sendto(dgram.packet.encode(), addr)
-
-    def send_tlv_discovery_response(self, resonsedata, addr):
+        # prefer ip over hostname because its truncated to 16 chars
+        hostname = self.ip_address[:16].encode("iso-8859-1")
+        hostname += (16 - len(hostname)) * b"\x00"
+        dgram = struct.pack("!c16s", b"D", hostname).decode()
+        self.transport.sendto(dgram.encode(), addr)
+
+    def send_tlv_discovery_response(
+        self, requestdata: OrderedDict[str, str], addr: tuple[str, int]
+    ) -> None:
         """Send TLV discovery response message."""
-        dgram = TLVDiscoveryResponseDatagram(resonsedata)
-        self.transport.sendto(dgram.packet.encode(), addr)
+        parts = ["E"]  # new discovery format
+        for key, value in requestdata.items():
+            if value is None:
+                value = ""  # noqa: PLW2901
+            elif len(value) > 255:
+                # Response too long, truncating to 255 bytes
+                value = value[:255]  # noqa: PLW2901
+            parts.extend((key, chr(len(value)), value))
+        dgram = "".join(parts)
+        self.transport.sendto(dgram.encode(), addr)
```

### Comparing `aioslimproto-2.2.2/aioslimproto/server.py` & `aioslimproto-2.3.0/aioslimproto/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,35 +6,43 @@
 from types import TracebackType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union
 
 from .cli import SlimProtoCLI
 from .client import SlimClient
 from .const import SLIMPROTO_PORT, EventType, SlimEvent
 from .discovery import start_discovery
+from .util import get_hostname, get_ip
 
 EventCallBackType = Callable[[SlimEvent], None]
 EventSubscriptionType = Tuple[EventCallBackType, Tuple[EventType], Tuple[str]]
 
 
 class SlimServer:
     """Server holding the SLIMproto players."""
 
     def __init__(
         self,
         cli_port: Optional[int] = None,
         cli_port_json: Optional[int] = 0,
+        ip_address: str | None = None,
+        name: str | None = None,
     ) -> None:
         """
         Initialize SlimServer instance.
 
-        cli_port: Optionally start a simple Telnet CLI server on this port for compatability
+        Params:
+        - cli_port: Optionally start a simple Telnet CLI server on this port for compatability
         with players relying on the server providing this feature. None to disable, 0 for autoselect.
-        cli_port_json: Same as cli port but it's newer JSON RPC equivalent.
+        - cli_port_json: Same as cli port but it's newer JSON RPC equivalent.
+        - ip_address: IP to broadcast to clients to discover this server, None for autoselect.
+        - name: Name to broadcast to clients to discover this server, None for autoselect.
         """
         self.logger = logging.getLogger(__name__)
+        self.ip_address = ip_address or get_ip()
+        self.name = name or get_hostname()
         self.cli = SlimProtoCLI(self, cli_port, cli_port_json)
         self._subscribers: List[EventSubscriptionType] = []
         self._socket_servers: List[Union[asyncio.Server, asyncio.BaseTransport]] = []
         self._players: Dict[str, SlimClient] = {}
 
     @property
     def players(self) -> List[SlimClient]:
@@ -52,15 +60,19 @@
         self._socket_servers = [
             # start slimproto server
             await asyncio.start_server(self._create_client, "0.0.0.0", SLIMPROTO_PORT),
             # setup cli
             *await self.cli.start(),
             # setup discovery
             await start_discovery(
-                SLIMPROTO_PORT, self.cli.cli_port, self.cli.cli_port_json
+                self.ip_address,
+                SLIMPROTO_PORT,
+                self.cli.cli_port,
+                self.cli.cli_port_json,
+                self.name,
             ),
         ]
 
     async def stop(self):
         """Stop running the server."""
         for client in list(self._players.values()):
             client.disconnect()
```

### Comparing `aioslimproto-2.2.2/aioslimproto/util.py` & `aioslimproto-2.3.0/aioslimproto/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 
 import asyncio
 import logging
 import socket
 from typing import Any, Dict
 from urllib.parse import parse_qsl
 
+from .const import FALLBACK_CODECS
+
 
 def get_ip():
     """Get primary IP-address for this host."""
     # pylint: disable=broad-except,no-member
     sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         # doesn't even have to be reachable
@@ -66,15 +68,15 @@
         info = helo_data[36:].decode()
         params = dict(parse_qsl(info.replace(",", "&")))
         # try to parse codecs which are hidden in the connection string
         params["SupportedCodecs"] = [
             codec
             for codec in ("alc", "aac", "ogg", "ogf", "flc", "aif", "pcm", "mp3")
             if codec in info
-        ]
+        ] or FALLBACK_CODECS
     except Exception as exc:  # pylint: disable=broad-except
         # I have no idea if this message is the same for all device types
         # so a big try..except around it
 
         logging.getLogger(__name__).exception(
             "Error while parsing device info", exc_info=exc
         )
```

### Comparing `aioslimproto-2.2.2/aioslimproto.egg-info/PKG-INFO` & `aioslimproto-2.3.0/aioslimproto.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.2.2
+Version: 2.3.0
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.2.2/setup.cfg` & `aioslimproto-2.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.2/setup.py` & `aioslimproto-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README_FILE = PROJECT_DIR / "README.md"
 REQUIREMENTS_FILE = PROJECT_DIR / "requirements.txt"
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
 PROJECT_REQ_PYTHON_VERSION = "3.9"
 
 setup(
     name="aioslimproto",
-    version="2.2.2",
+    version="2.3.0",
     license="Apache License 2.0",
     url="https://github.com/music-assistant/aioslimproto",
     author="Marcel van der Veldt",
     author_email="marcelveldt@users.noreply.github.com",
     description="Python module to talk to Logitech Squeezebox players directly (without Logitech server).",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
```

