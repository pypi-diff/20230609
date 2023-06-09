# Comparing `tmp/nessclient-0.9.9.tar.gz` & `tmp/nessclient-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nessclient-0.9.9.tar", last modified: Mon Dec 31 00:34:45 2018, max compression
+gzip compressed data, was "nessclient-1.0.0.tar", last modified: Fri Jun  9 13:03:53 2023, max compression
```

## Comparing `nessclient-0.9.9.tar` & `nessclient-1.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-31 00:34:45.000000 nessclient-0.9.9/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-12-31 00:34:28.000000 nessclient-0.9.9/nessclient.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)       64 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     2469 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      673 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1690 2018-12-31 00:34:14.000000 nessclient-0.9.9/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5735 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient/cli/
--rw-rw-r--   0 travis    (2000) travis    (2000)      901 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/events.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-31 00:34:45.000000 nessclient-0.9.9/nessclient/cli/server/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3189 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/server/server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      190 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/server/zone.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      260 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/server/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5521 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/server/alarm_server.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2987 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/server/alarm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      499 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/__main__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      476 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/cli/send_command.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2640 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/connection.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5668 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/packet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11439 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/event.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5582 2018-12-31 00:34:14.000000 nessclient-0.9.9/nessclient/alarm.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1361 2018-12-31 00:34:14.000000 nessclient-0.9.9/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1071 2018-12-31 00:34:14.000000 nessclient-0.9.9/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)       79 2018-12-31 00:34:45.000000 nessclient-0.9.9/setup.cfg
--rwxrwxr-x   0 travis    (2000) travis    (2000)       44 2018-12-31 00:34:14.000000 nessclient-0.9.9/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2469 2018-12-31 00:34:45.000000 nessclient-0.9.9/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2018-12-31 00:34:29.000000 nessclient-0.9.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:03:53.871958 nessclient-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-09 13:03:20.000000 nessclient-1.0.0/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)       36 2023-06-09 13:03:20.000000 nessclient-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-09 13:03:53.871958 nessclient-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-09 13:03:20.000000 nessclient-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:03:53.871958 nessclient-1.0.0/nessclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7241 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/alarm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:03:53.871958 nessclient-1.0.0/nessclient/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/send_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:03:53.871958 nessclient-1.0.0/nessclient/cli/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/server/alarm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/server/alarm_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/cli/server/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15196 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-09 13:03:20.000000 nessclient-1.0.0/nessclient/packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:03:53.871958 nessclient-1.0.0/nessclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:03:34.000000 nessclient-1.0.0/nessclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 13:03:53.000000 nessclient-1.0.0/nessclient.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      143 2023-06-09 13:03:53.871958 nessclient-1.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1317 2023-06-09 13:03:20.000000 nessclient-1.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nessclient-0.9.9/nessclient.egg-info/PKG-INFO` & `nessclient-1.0.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,56 +1,42 @@
-Metadata-Version: 2.1
-Name: nessclient
-Version: 0.9.9
-Summary: Implementation/abstraction of the Ness D8x / D16x Serial Interface ASCII protocol
-Home-page: https://github.com/nickw444/nessclient
-Author: Nick Whyte
-Author-email: nick@nickwhyte.com
-License: UNKNOWN
-Description: # nessclient
-        
-        [![](https://travis-ci.org/nickw444/nessclient.svg?branch=master)](https://travis-ci.org/nickw444/nessclient)
-        [![](https://coveralls.io/repos/nickw444/nessclient/badge.svg)](https://coveralls.io/r/nickw444/nessclient)
-        [![](https://img.shields.io/pypi/v/nessclient.svg)](https://pypi.python.org/pypi/nessclient/)
-        [![](https://readthedocs.org/projects/nessclient/badge/?version=latest&style=flat)](https://nessclient.readthedocs.io/en/latest/)
-        
-        A python implementation/abstraction of the [Ness D8x / D16x Serial Interface ASCII protocol](http://www.nesscorporation.com/Software/Ness_D8-D16_ASCII_protocol.pdf)
-        
-        ## Installing nessclient
-        
-        `nessclient` is available directly from pip:
-        
-        ```sh
-        pip install nessclient
-        ```
-        
-        ## Documentation
-        
-        The full documentation can be found at [Read the Docs](https://nessclient.readthedocs.io/en/latest/)
-        
-        ## CLI
-        
-        This package includes a CLI which uses the library to interface with the Ness Serial Interface. You can read more in [the docs](https://nessclient.readthedocs.io/en/latest/cli.html)
-        
-        To use the CLI you must install it's dependencies by installing it with extras for `cli`: 
-        
-        ```
-        pip install nessclient[cli]
-        ness-cli --help
-        ``` 
-        
-        ## API Documentation
-        You can find the full API documentation [here](https://nessclient.readthedocs.io/en/latest/api.html)
-        
-        ## Examples
-        
-        Please see [Examples](https://nessclient.readthedocs.io/en/latest/examples.html) section in the docs for examples. These same examples can be found as source in the [examples/](examples) directory. 
-         
-        ## Developing
-        
-        Please see [Developing](https://nessclient.readthedocs.io/en/latest/developing.html) section in the docs for development environment setup information.
-        
-Platform: UNKNOWN
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown
-Provides-Extra: cli
+# nessclient
+
+[![](https://travis-ci.org/nickw444/nessclient.svg?branch=master)](https://travis-ci.org/nickw444/nessclient)
+[![codecov](https://codecov.io/gh/nickw444/nessclient/branch/master/graph/badge.svg)](https://codecov.io/gh/nickw444/nessclient)
+[![](https://img.shields.io/pypi/v/nessclient.svg)](https://pypi.python.org/pypi/nessclient/)
+[![](https://readthedocs.org/projects/nessclient/badge/?version=latest&style=flat)](https://nessclient.readthedocs.io/en/latest/)
+
+A python implementation/abstraction of the [Ness D8x / D16x Serial Interface ASCII protocol](http://www.nesscorporation.com/Software/Ness_D8-D16_ASCII_protocol_rev13.pdf)
+
+## Installing nessclient
+
+`nessclient` is available directly from pip:
+
+```sh
+pip install nessclient
+```
+
+## Documentation
+
+The full documentation can be found at [Read the Docs](https://nessclient.readthedocs.io/en/latest/)
+
+## CLI
+
+This package includes a CLI which uses the library to interface with the Ness Serial Interface. You can read more in [the docs](https://nessclient.readthedocs.io/en/latest/cli.html)
+
+To use the CLI you must install it's dependencies by installing it with extras for `cli`: 
+
+```
+pip install nessclient[cli]
+ness-cli --help
+``` 
+
+## API Documentation
+You can find the full API documentation [here](https://nessclient.readthedocs.io/en/latest/api.html)
+
+## Examples
+
+Please see [Examples](https://nessclient.readthedocs.io/en/latest/examples.html) section in the docs for examples. These same examples can be found as source in the [examples/](examples) directory. 
+ 
+## Developing
+
+Please see [Developing](https://nessclient.readthedocs.io/en/latest/developing.html) section in the docs for development environment setup information.
```

### Comparing `nessclient-0.9.9/nessclient.egg-info/SOURCES.txt` & `nessclient-1.0.0/nessclient.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.md
-VERSION
 setup.cfg
 setup.py
 nessclient/__init__.py
 nessclient/alarm.py
 nessclient/client.py
 nessclient/connection.py
 nessclient/event.py
@@ -13,14 +12,15 @@
 nessclient.egg-info/PKG-INFO
 nessclient.egg-info/SOURCES.txt
 nessclient.egg-info/dependency_links.txt
 nessclient.egg-info/entry_points.txt
 nessclient.egg-info/not-zip-safe
 nessclient.egg-info/requires.txt
 nessclient.egg-info/top_level.txt
+nessclient/cli/__init__.py
 nessclient/cli/__main__.py
 nessclient/cli/events.py
 nessclient/cli/send_command.py
 nessclient/cli/server/__init__.py
 nessclient/cli/server/alarm.py
 nessclient/cli/server/alarm_server.py
 nessclient/cli/server/server.py
```

### Comparing `nessclient-0.9.9/README.md` & `nessclient-1.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,28 @@
+Metadata-Version: 2.1
+Name: nessclient
+Version: 1.0.0
+Summary: Implementation/abstraction of the Ness D8x / D16x Serial Interface ASCII protocol
+Home-page: https://github.com/nickw444/nessclient
+Author: Nick Whyte
+Author-email: nick@nickwhyte.com
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+Provides-Extra: cli
+License-File: LICENSE
+
 # nessclient
 
 [![](https://travis-ci.org/nickw444/nessclient.svg?branch=master)](https://travis-ci.org/nickw444/nessclient)
-[![](https://coveralls.io/repos/nickw444/nessclient/badge.svg)](https://coveralls.io/r/nickw444/nessclient)
+[![codecov](https://codecov.io/gh/nickw444/nessclient/branch/master/graph/badge.svg)](https://codecov.io/gh/nickw444/nessclient)
 [![](https://img.shields.io/pypi/v/nessclient.svg)](https://pypi.python.org/pypi/nessclient/)
 [![](https://readthedocs.org/projects/nessclient/badge/?version=latest&style=flat)](https://nessclient.readthedocs.io/en/latest/)
 
-A python implementation/abstraction of the [Ness D8x / D16x Serial Interface ASCII protocol](http://www.nesscorporation.com/Software/Ness_D8-D16_ASCII_protocol.pdf)
+A python implementation/abstraction of the [Ness D8x / D16x Serial Interface ASCII protocol](http://www.nesscorporation.com/Software/Ness_D8-D16_ASCII_protocol_rev13.pdf)
 
 ## Installing nessclient
 
 `nessclient` is available directly from pip:
 
 ```sh
 pip install nessclient
```

### Comparing `nessclient-0.9.9/nessclient/client.py` & `nessclient-1.0.0/nessclient/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,87 +2,99 @@
 import datetime
 import logging
 from asyncio import sleep
 from typing import Optional, Callable
 
 from justbackoff import Backoff
 
-from .alarm import ArmingState, Alarm
+from .alarm import ArmingState, Alarm, ArmingMode
 from .connection import Connection, IP232Connection
 from .event import BaseEvent
 from .packet import CommandType, Packet
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class Client:
-    def __init__(self,
-                 connection: Optional[Connection] = None,
-                 host: Optional[str] = None,
-                 port: Optional[int] = None,
-                 loop: Optional[asyncio.AbstractEventLoop] = None,
-                 update_interval: int = 60):
+    """
+    :param update_interval: Frequency (in seconds) to trigger a full state
+        refresh
+    :param infer_arming_state: Infer the `DISARMED` arming state only via
+        system status events. This works around a bug with some panels
+        (`<v5.8`) which emit `update.status = []` when they are armed.
+    """
+
+    def __init__(
+        self,
+        connection: Optional[Connection] = None,
+        host: Optional[str] = None,
+        port: Optional[int] = None,
+        update_interval: int = 60,
+        infer_arming_state: bool = False,
+        alarm: Optional[Alarm] = None,
+    ):
         if connection is None:
             assert host is not None
             assert port is not None
-            assert loop is not None
-            connection = IP232Connection(host=host, port=port, loop=loop)
+            connection = IP232Connection(host=host, port=port)
 
-        self.alarm = Alarm()
+        if alarm is None:
+            alarm = Alarm(infer_arming_state=infer_arming_state)
+
+        self.alarm = alarm
         self._on_event_received: Optional[Callable[[BaseEvent], None]] = None
         self._connection = connection
         self._closed = False
         self._backoff = Backoff()
         self._connect_lock = asyncio.Lock()
         self._last_recv: Optional[datetime.datetime] = None
         self._update_interval = update_interval
 
     async def arm_away(self, code: Optional[str] = None) -> None:
-        command = 'A{}E'.format(code if code else '')
+        command = "A{}E".format(code if code else "")
         return await self.send_command(command)
 
     async def arm_home(self, code: Optional[str] = None) -> None:
-        command = 'H{}E'.format(code if code else '')
+        command = "H{}E".format(code if code else "")
         return await self.send_command(command)
 
     async def disarm(self, code: str) -> None:
-        command = '{}E'.format(code)
+        command = "{}E".format(code)
         return await self.send_command(command)
 
     async def panic(self, code: str) -> None:
-        command = '*{}#'.format(code)
+        command = "*{}#".format(code)
         return await self.send_command(command)
 
     async def aux(self, output_id: int, state: bool = True) -> None:
-        command = '{}{}{}'.format(
-            output_id, output_id,
-            '*' if state else '#')
+        command = "{}{}{}".format(output_id, output_id, "*" if state else "#")
         return await self.send_command(command)
 
     async def update(self) -> None:
         """Force update of alarm status and zones"""
+        _LOGGER.debug("Requesting state update from server (S00, S14)")
         await asyncio.gather(
             # List unsealed Zones
-            self.send_command('S00'),
+            self.send_command("S00"),
             # Arming status update
-            self.send_command('S14'),
+            self.send_command("S14"),
         )
 
     async def _connect(self) -> None:
         async with self._connect_lock:
             if self._should_reconnect():
-                _LOGGER.debug('Closing stale connection and reconnecting')
+                _LOGGER.debug("Closing stale connection and reconnecting")
                 await self._connection.close()
 
             while not self._connection.connected:
-                _LOGGER.debug('Attempting to connect')
+                _LOGGER.debug("Attempting to connect")
                 try:
                     await self._connection.connect()
                 except (ConnectionRefusedError, OSError) as e:
-                    _LOGGER.warning('Failed to connect: %s', e)
+                    _LOGGER.warning("Failed to connect: %s", e)
                     await sleep(self._backoff.duration())
 
                 self._last_recv = datetime.datetime.now()
 
             self._backoff.reset()
 
     async def send_command(self, command: str) -> None:
@@ -90,72 +102,84 @@
             address=0x00,
             seq=0x00,
             command=CommandType.USER_INTERFACE,
             data=command,
             timestamp=None,
         )
         await self._connect()
-        return await self._connection.write(packet.encode().encode('ascii'))
+        payload = packet.encode() + "\r\n"
+        _LOGGER.debug("Sending payload: %s", repr(payload))
+        return await self._connection.write(payload.encode("ascii"))
 
     async def _recv_loop(self) -> None:
         while not self._closed:
             await self._connect()
 
             while True:
                 data = await self._connection.read()
                 if data is None:
                     _LOGGER.debug("Received None data from connection.read()")
                     break
 
                 self._last_recv = datetime.datetime.now()
                 try:
-                    decoded_data = data.decode('utf-8').strip()
+                    decoded_data = data.decode("utf-8").strip()
                 except UnicodeDecodeError:
                     _LOGGER.warning("Failed to decode data", exc_info=True)
                     continue
 
                 _LOGGER.debug("Decoding data: '%s'", decoded_data)
                 if len(decoded_data) > 0:
-                    pkt = Packet.decode(decoded_data)
-                    event = BaseEvent.decode(pkt)
+                    try:
+                        pkt = Packet.decode(decoded_data)
+                        event = BaseEvent.decode(pkt)
+                    except Exception:
+                        _LOGGER.warning("Failed to decode packet", exc_info=True)
+                        continue
+
                     if self._on_event_received is not None:
                         self._on_event_received(event)
 
                     self.alarm.handle_event(event)
 
     def _should_reconnect(self) -> bool:
         now = datetime.datetime.now()
-        return self._last_recv is not None and self._last_recv < now - datetime.timedelta(
-            seconds=self._update_interval + 30)
+        return (
+            self._last_recv is not None
+            and self._last_recv
+            < now - datetime.timedelta(seconds=self._update_interval + 30)
+        )
 
     async def _update_loop(self) -> None:
         """Schedule a state update to keep the connection alive"""
         await asyncio.sleep(self._update_interval)
         while not self._closed:
-            _LOGGER.debug("Forcing a keepalive state update")
-            await self.send_command('S00')  # List unsealed Zones
+            await self.update()
             await asyncio.sleep(self._update_interval)
 
     async def keepalive(self) -> None:
         await asyncio.gather(
             self._recv_loop(),
             self._update_loop(),
         )
 
     async def close(self) -> None:
         self._closed = True
         await self._connection.close()
 
-    def on_state_change(self, f: Callable[[ArmingState], None]
-                        ) -> Callable[[ArmingState], None]:
-        self.alarm._on_state_change = f
+    def on_state_change(
+        self, f: Callable[[ArmingState, ArmingMode | None], None]
+    ) -> Callable[[ArmingState, ArmingMode | None], None]:
+        self.alarm.on_state_change(f)
         return f
 
-    def on_zone_change(self, f: Callable[[int, bool], None]
-                       ) -> Callable[[int, bool], None]:
-        self.alarm._on_zone_change = f
+    def on_zone_change(
+        self, f: Callable[[int, bool], None]
+    ) -> Callable[[int, bool], None]:
+        self.alarm.on_zone_change(f)
         return f
 
-    def on_event_received(self, f: Callable[[BaseEvent], None]
-                          ) -> Callable[[BaseEvent], None]:
+    def on_event_received(
+        self, f: Callable[[BaseEvent], None]
+    ) -> Callable[[BaseEvent], None]:
         self._on_event_received = f
         return f
```

### Comparing `nessclient-0.9.9/nessclient/cli/server/server.py` & `nessclient-1.0.0/nessclient/cli/server/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 import socket
 import threading
-from typing import List, Callable
+from typing import List, Callable, Any
 
 from .zone import Zone
 from ...event import BaseEvent, SystemStatusEvent
 from ...packet import Packet, CommandType
 
 _LOGGER = logging.getLogger(__name__)
 
@@ -13,69 +13,70 @@
 class Server:
     def __init__(self, handle_command: Callable[[str], None]):
         self._handle_command = handle_command
         self._handle_event_lock: threading.Lock = threading.Lock()
         self._clients_lock: threading.Lock = threading.Lock()
         self._clients: List[socket.socket] = []
 
-    def start(self, host, port):
+    def start(self, host: str, port: int) -> None:
         threading.Thread(target=self._loop, args=(host, port)).start()
 
-    def _loop(self, host, port):
+    def _loop(self, host: str, port: int) -> None:
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
             s.bind((host, port))
             s.listen(5)
 
             _LOGGER.info("Server listening on {}:{}".format(host, port))
             while True:
                 conn, addr = s.accept()
                 threading.Thread(
-                    target=self._on_client_connected, args=(conn, addr)).start()
+                    target=self._on_client_connected, args=(conn, addr)
+                ).start()
 
-    def write_event(self, event: BaseEvent):
+    def write_event(self, event: BaseEvent) -> None:
         pkt = event.encode()
         self._write_to_all_clients(pkt.encode())
 
-    def on_zone_state_change(self, zone_id: int, state: Zone.State):
+    def on_zone_state_change(self, zone_id: int, state: Zone.State) -> None:
         event = SystemStatusEvent(
             type=get_zone_state_event_type(state),
             zone=zone_id,
             area=0,
             timestamp=None,
-            address=0
+            address=0,
         )
         pkt = event.encode()
         self._write_to_all_clients(pkt.encode())
 
-    def _on_client_connected(self, conn: socket.socket, addr):
+    def _on_client_connected(self, conn: socket.socket, addr: Any) -> None:
         _LOGGER.info("Client connected from: %s", addr)
         with self._clients_lock:
             self._clients.append(conn)
 
         while True:
             data = conn.recv(1024)
-            if data is None or len(data) is 0:
+            if data is None or len(data) == 0:
                 _LOGGER.info("client %s disconnected", addr)
                 with self._clients_lock:
                     self._clients.remove(conn)
 
                 break
 
             self._handle_incoming_data(data)
 
-    def _write_to_all_clients(self, data: str):
+    def _write_to_all_clients(self, data: str) -> None:
         _LOGGER.debug("Writing message '%s' to all clients", data)
         with self._clients_lock:
             for conn in self._clients:
-                conn.send(data.encode('utf-8') + b'\r\n')
+                conn.send(data.encode("utf-8") + b"\r\n")
 
-    def _handle_incoming_data(self, data: bytes):
+    def _handle_incoming_data(self, data: bytes) -> None:
         _LOGGER.debug("Received incoming data: %s", data)
-        pkt = Packet.decode(data.strip().decode('utf-8'))
+        pkt = Packet.decode(data.strip().decode("utf-8"))
         _LOGGER.debug("Packet is: %s", pkt)
         # Handle Incoming Command:
         if pkt.command == CommandType.USER_INTERFACE and not pkt.is_user_interface_resp:
             _LOGGER.info("Handling User interface incoming: %s", pkt.data)
             with self._handle_event_lock:
                 self._handle_command(pkt.data)
         else:
```

### Comparing `nessclient-0.9.9/nessclient/cli/server/alarm_server.py` & `nessclient-1.0.0/nessclient/cli/server/alarm_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,164 +1,195 @@
 import logging
 import random
 import threading
 import time
-from typing import List
+from typing import List, Iterator
 
 from .alarm import Alarm
 from .server import Server, get_zone_state_event_type
 from .zone import Zone
 from ...event import SystemStatusEvent, ArmingUpdate, ZoneUpdate, StatusUpdate
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class AlarmServer():
+class AlarmServer:
     def __init__(self, host: str, port: int):
         self._alarm = Alarm.create(
             num_zones=8,
             alarm_state_changed=self._alarm_state_changed,
             zone_state_changed=self._zone_state_changed,
         )
         self._server = Server(handle_command=self._handle_command)
         self._host = host
         self._port = port
         self._simulation_running = False
 
-    def start(self):
+    def start(self) -> None:
         self._server.start(host=self._host, port=self._port)
         self._start_simulation()
 
         while True:
             command = input("Command: ")
             if command is None:
                 continue
 
             command = command.upper().strip()
             if command == "D":
                 self._alarm.disarm()
-            elif command == "A":
-                self._alarm.arm()
+            elif command == "A" or command == "AA":
+                self._alarm.arm(Alarm.ArmingMode.ARMED_AWAY)
+            elif command == "AH":
+                self._alarm.arm(Alarm.ArmingMode.ARMED_HOME)
+            elif command == "AD":
+                self._alarm.arm(Alarm.ArmingMode.ARMED_DAY)
+            elif command == "AN":
+                self._alarm.arm(Alarm.ArmingMode.ARMED_NIGHT)
+            elif command == "AV":
+                self._alarm.arm(Alarm.ArmingMode.ARMED_VACATION)
             elif command == "T":
                 self._alarm.trip()
 
             print(command)
 
-    def _alarm_state_changed(self, previous_state: Alarm.ArmingState,
-                             state: Alarm.ArmingState):
+    def _alarm_state_changed(
+        self,
+        previous_state: Alarm.ArmingState,
+        state: Alarm.ArmingState,
+        arming_mode: Alarm.ArmingMode | None,
+    ) -> None:
         if state != Alarm.ArmingState.DISARMED:
             self._stop_simulation()
 
-        for event_type in get_events_for_state_update(previous_state, state):
+        for event_type in get_events_for_state_update(
+            previous_state, state, arming_mode
+        ):
             event = SystemStatusEvent(
-                type=event_type,
-                zone=0x00,
-                area=0x00,
-                timestamp=None,
-                address=0
+                type=event_type, zone=0x00, area=0x00, timestamp=None, address=0
             )
             self._server.write_event(event)
 
-    def _zone_state_changed(self, zone_id: int, state: Zone.State):
+    def _zone_state_changed(self, zone_id: int, state: Zone.State) -> None:
         event = SystemStatusEvent(
             type=get_zone_state_event_type(state),
             zone=zone_id,
             area=0,
             timestamp=None,
-            address=0
+            address=0,
         )
         self._server.write_event(event)
 
-    def _handle_command(self, command: str):
+    def _handle_command(self, command: str) -> None:
         _LOGGER.info("Incoming User Command: {}".format(command))
-        if command == 'AE' or command == 'A1234E':
+        if command == "AE" or command == "A1234E":
             self._alarm.arm()
-        elif command == '1234E':
+        elif command == "1234E":
             self._alarm.disarm()
-        elif command == 'S00':
+        elif command == "S00":
             self._handle_zone_input_unsealed_status_update_request()
-        elif command == 'S14':
+        elif command == "S14":
             self._handle_arming_status_update_request()
 
-    def _handle_arming_status_update_request(self):
+    def _handle_arming_status_update_request(self) -> None:
         event = ArmingUpdate(
             status=get_arming_status(self._alarm.state),
             address=0x00,
             timestamp=None,
         )
         self._server.write_event(event)
 
-    def _handle_zone_input_unsealed_status_update_request(self):
+    def _handle_zone_input_unsealed_status_update_request(self) -> None:
         event = ZoneUpdate(
             request_id=StatusUpdate.RequestID.ZONE_INPUT_UNSEALED,
             included_zones=[
-                get_zone_for_id(z.id) for z in
-                self._alarm.zones if z.state == Zone.State.UNSEALED],
+                get_zone_for_id(z.id)
+                for z in self._alarm.zones
+                if z.state == Zone.State.UNSEALED
+            ],
             address=0x00,
             timestamp=None,
         )
         self._server.write_event(event)
 
-    def _simulate_zone_events(self):
+    def _simulate_zone_events(self) -> None:
         while self._simulation_running:
             zone: Zone = random.choice(self._alarm.zones)
             self._alarm.update_zone(zone.id, toggled_state(zone.state))
             _LOGGER.info("Toggled zone: %s", zone)
             time.sleep(random.randint(1, 5))
 
-    def _stop_simulation(self):
+    def _stop_simulation(self) -> None:
         self._simulation_running = False
 
-    def _start_simulation(self):
+    def _start_simulation(self) -> None:
         if not self._simulation_running:
             self._simulation_running = True
             threading.Thread(target=self._simulate_zone_events).start()
 
 
-def get_events_for_state_update(
-        previous_state: Alarm.ArmingState,
-        state: Alarm.ArmingState) -> List[SystemStatusEvent.EventType]:
+def mode_to_event(mode: Alarm.ArmingMode | None) -> SystemStatusEvent.EventType:
+    if mode == Alarm.ArmingMode.ARMED_AWAY:
+        return SystemStatusEvent.EventType.ARMED_AWAY
+    elif mode == Alarm.ArmingMode.ARMED_HOME:
+        return SystemStatusEvent.EventType.ARMED_HOME
+    elif mode == Alarm.ArmingMode.ARMED_DAY:
+        return SystemStatusEvent.EventType.ARMED_DAY
+    elif mode == Alarm.ArmingMode.ARMED_NIGHT:
+        return SystemStatusEvent.EventType.ARMED_NIGHT
+    elif mode == Alarm.ArmingMode.ARMED_VACATION:
+        return SystemStatusEvent.EventType.ARMED_VACATION
+    else:
+        raise AssertionError("Unknown alarm mode")
+
 
+def get_events_for_state_update(
+    previous_state: Alarm.ArmingState,
+    state: Alarm.ArmingState,
+    arming_mode: Alarm.ArmingMode | None,
+) -> Iterator[SystemStatusEvent.EventType]:
     if state == Alarm.ArmingState.DISARMED:
         yield SystemStatusEvent.EventType.DISARMED
     if state == Alarm.ArmingState.EXIT_DELAY:
-        yield SystemStatusEvent.EventType.ARMED_AWAY
+        yield mode_to_event(arming_mode)
         yield SystemStatusEvent.EventType.EXIT_DELAY_START
 
     if state == Alarm.ArmingState.TRIPPED:
         yield SystemStatusEvent.EventType.ALARM
 
     # When state transitions from EXIT_DELAY, trigger EXIT_DELAY_END.
-    if (previous_state == Alarm.ArmingState.EXIT_DELAY and state != previous_state or
-            state == Alarm.ArmingState.ARMED_AWAY):
+    if (
+        previous_state == Alarm.ArmingState.EXIT_DELAY
+        and state != previous_state
+        or state == Alarm.ArmingState.ARMED
+    ):
         yield SystemStatusEvent.EventType.EXIT_DELAY_END
 
     if state == Alarm.ArmingState.ENTRY_DELAY:
         yield SystemStatusEvent.EventType.ENTRY_DELAY_START
 
     # When state transitions from ENTRY_DELAY, trigger ENTRY_DELAY_END
     if previous_state == Alarm.ArmingState.ENTRY_DELAY and state != previous_state:
         yield SystemStatusEvent.EventType.ENTRY_DELAY_END
 
 
 def get_arming_status(state: Alarm.ArmingState) -> List[ArmingUpdate.ArmingStatus]:
-    if state == Alarm.ArmingState.ARMED_AWAY:
+    if state == Alarm.ArmingState.ARMED:
         return [
-            ArmingUpdate.ArmingStatus.MANUAL_EXCLUDE_MODE,
-            ArmingUpdate.ArmingStatus.DAY_ZONE_SELECT
+            ArmingUpdate.ArmingStatus.AREA_1_ARMED,
+            ArmingUpdate.ArmingStatus.AREA_1_FULLY_ARMED,
         ]
     elif state == Alarm.ArmingState.EXIT_DELAY:
-        return [ArmingUpdate.ArmingStatus.MANUAL_EXCLUDE_MODE]
+        return [ArmingUpdate.ArmingStatus.AREA_1_ARMED]
     else:
         return []
 
 
 def toggled_state(state: Zone.State) -> Zone.State:
     if state == Zone.State.SEALED:
         return Zone.State.UNSEALED
     else:
         return Zone.State.SEALED
 
 
 def get_zone_for_id(zone_id: int) -> ZoneUpdate.Zone:
-    key = 'ZONE_{}'.format(zone_id)
+    key = "ZONE_{}".format(zone_id)
     return ZoneUpdate.Zone[key]
```

### Comparing `nessclient-0.9.9/nessclient/cli/server/alarm.py` & `nessclient-1.0.0/nessclient/cli/server/alarm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,133 @@
 import logging
 import threading
 import time
 import uuid
-from dataclasses import dataclass
 from enum import Enum
 from typing import List, Callable, Optional
 
 from .zone import Zone
 
 _LOGGER = logging.getLogger(__name__)
 
 EXIT_DELAY = 10
 ENTRY_DELAY = 10
 
 
-@dataclass
 class Alarm:
     """
     Represents the complex alarm state machine
     """
 
     class ArmingState(Enum):
-        DISARMED = 'DISARMED'
-        EXIT_DELAY = 'EXIT_DELAY'
-        ARMED_AWAY = 'ARMED_AWAY'
-        ENTRY_DELAY = 'ENTRY_DELAY'
-        TRIPPED = 'TRIPPED'
-
-    state: ArmingState
-    zones: List[Zone]
-
-    _alarm_state_changed: Callable[[ArmingState, ArmingState], None]
-    _zone_state_changed: Callable[[int, Zone.State], None]
-
-    _pending_event: Optional[str] = None
+        DISARMED = "DISARMED"
+        EXIT_DELAY = "EXIT_DELAY"
+        ARMED = "ARMED"
+        ENTRY_DELAY = "ENTRY_DELAY"
+        TRIPPED = "TRIPPED"
+
+    class ArmingMode(Enum):
+        ARMED_AWAY = "ARMED_AWAY"
+        ARMED_HOME = "ARMED_HOME"
+        ARMED_DAY = "ARMED_DAY"
+        ARMED_NIGHT = "ARMED_NIGHT"
+        ARMED_VACATION = "ARMED_VACATION"
+
+    def __init__(
+        self,
+        state: ArmingState,
+        zones: List[Zone],
+        _alarm_state_changed: Callable[[ArmingState, ArmingState, ArmingMode], None],
+        _zone_state_changed: Callable[[int, Zone.State], None],
+    ):
+        self.state = state
+        self.zones = zones
+        self._arming_mode: Alarm.ArmingMode | None = None
+        self._alarm_state_changed = _alarm_state_changed
+        self._zone_state_changed = _zone_state_changed
+        self._pending_event: Optional[str] = None
 
     @staticmethod
-    def create(num_zones: int,
-               alarm_state_changed: Callable[[ArmingState, ArmingState], None],
-               zone_state_changed: Callable[[int, Zone.State], None]) -> 'Alarm':
+    def create(
+        num_zones: int,
+        alarm_state_changed: Callable[[ArmingState, ArmingState, ArmingMode], None],
+        zone_state_changed: Callable[[int, Zone.State], None],
+    ) -> "Alarm":
         return Alarm(
             state=Alarm.ArmingState.DISARMED,
             zones=Alarm._generate_zones(num_zones),
             _alarm_state_changed=alarm_state_changed,
             _zone_state_changed=zone_state_changed,
         )
 
     @staticmethod
     def _generate_zones(num_zones: int) -> List[Zone]:
         rv = []
         for i in range(num_zones):
             rv.append(Zone(id=i + 1, state=Zone.State.SEALED))
         return rv
 
-    def arm(self):
-        self._update_state(Alarm.ArmingState.EXIT_DELAY)
+    def arm(self, mode: ArmingMode = ArmingMode.ARMED_AWAY) -> None:
+        self._update_state(Alarm.ArmingState.EXIT_DELAY, mode)
         self._schedule(EXIT_DELAY, self._arm_complete)
 
-    def disarm(self):
+    def disarm(self) -> None:
         self._cancel_pending_update()
-        self._update_state(Alarm.ArmingState.DISARMED)
+        self._update_state(Alarm.ArmingState.DISARMED, None)
 
-    def trip(self):
+    def trip(self) -> None:
         self._update_state(Alarm.ArmingState.ENTRY_DELAY)
         self._schedule(ENTRY_DELAY, self._trip_complete)
 
-    def update_zone(self, zone_id: int, state: Zone.State):
+    def update_zone(self, zone_id: int, state: Zone.State) -> None:
         zone = next(z for z in self.zones if z.id == zone_id)
         zone.state = state
         if self._zone_state_changed is not None:
             self._zone_state_changed(zone_id, state)
 
-        if self.state == Alarm.ArmingState.ARMED_AWAY:
+        if self.state == Alarm.ArmingState.ARMED:
             self.trip()
 
-    def _arm_complete(self):
+    def _arm_complete(self) -> None:
         _LOGGER.debug("Arm completed")
-        self._update_state(Alarm.ArmingState.ARMED_AWAY)
+        self._update_state(Alarm.ArmingState.ARMED)
 
-    def _trip_complete(self):
+    def _trip_complete(self) -> None:
         _LOGGER.debug("Trip completed")
         self._update_state(Alarm.ArmingState.TRIPPED)
 
-    def _cancel_pending_update(self):
+    def _cancel_pending_update(self) -> None:
         if self._pending_event is not None:
             self._pending_event = None
 
-    def _schedule(self, delay, fn):
+    def _schedule(self, delay: int, fn: Callable[[], None]) -> None:
         self._cancel_pending_update()
         event = uuid.uuid4().hex
         self._pending_event = event
 
-        def _run():
+        def _run() -> None:
             time.sleep(delay)
             if event == self._pending_event:
                 fn()
 
         threading.Thread(target=_run).start()
 
-    def _update_state(self, state: ArmingState):
+    # Sentinel value
+    ArmingModeMissing = object()
+
+    def _update_state(
+        self,
+        state: ArmingState,
+        arming_mode: ArmingMode | object | None = ArmingModeMissing,
+    ) -> None:
         if self._alarm_state_changed is not None:
-            self._alarm_state_changed(self.state, state)
+            self._alarm_state_changed(
+                self.state,
+                state,
+                self._arming_mode
+                if arming_mode is Alarm.ArmingModeMissing
+                else arming_mode,  # type: ignore
+            )
 
         self.state = state
+        if arming_mode is not Alarm.ArmingModeMissing:
+            self._arming_mode = arming_mode  # type: ignore
```

### Comparing `nessclient-0.9.9/nessclient/connection.py` & `nessclient-1.0.0/nessclient/connection.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,64 +30,65 @@
     def connected(self) -> bool:
         raise NotImplementedError()
 
 
 class IP232Connection(Connection):
     """A connection via IP232 with a Ness D8X/D16X server"""
 
-    def __init__(self, host: str, port: int,
-                 loop: asyncio.AbstractEventLoop = asyncio.get_event_loop()):
+    def __init__(self, host: str, port: int):
         super().__init__()
 
+        self._write_lock = asyncio.Lock()
         self._host = host
         self._port = port
-        self._loop = loop
         self._reader: Optional[asyncio.StreamReader] = None
         self._writer: Optional[asyncio.StreamWriter] = None
 
     @property
     def connected(self) -> bool:
         return self._reader is not None and self._writer is not None
 
     async def connect(self) -> bool:
         self._reader, self._writer = await asyncio.open_connection(
             host=self._host,
             port=self._port,
-            loop=self._loop,
         )
         return True
 
     async def read(self) -> Optional[bytes]:
         assert self._reader is not None
 
         try:
-            data = await self._reader.readuntil(b'\n')
-        except (asyncio.IncompleteReadError, TimeoutError,
-                ConnectionResetError) as e:
+            data = await self._reader.readuntil(b"\n")
+        except (asyncio.IncompleteReadError, TimeoutError, ConnectionResetError) as e:
             _LOGGER.info(
-                "Got exception: %s. Most likely the other side has "
-                "disconnected!", e)
+                "Got exception: %s. Most likely the other side has " "disconnected!", e
+            )
             self._writer = None
             self._reader = None
             return None
 
         if data is None:
             _LOGGER.info("Empty response received")
             self._writer = None
             self._reader = None
             return None
 
         return data.strip()
 
     async def write(self, data: bytes) -> None:
-        assert self._writer is not None
-
-        self._writer.write(data)
-        await self._writer.drain()
+        _LOGGER.debug("Waiting for write_lock to write data: %s", data)
+        async with self._write_lock:
+            _LOGGER.debug("Obtained write_lock to write data: %s", data)
+            assert self._writer is not None
+
+            self._writer.write(data)
+            await self._writer.drain()
+            _LOGGER.debug("Data was written: %s", data)
 
     async def close(self) -> None:
         if self.connected and self._writer is not None:
             self._writer.close()
-            if hasattr(self._writer, 'wait_closed'):
-                await self._writer.wait_closed()  # type: ignore
+            if hasattr(self._writer, "wait_closed"):
+                await self._writer.wait_closed()
             self._writer = None
             self._reader = None
```

### Comparing `nessclient-0.9.9/nessclient/packet.py` & `nessclient-1.0.0/nessclient/packet.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import datetime
 import logging
 from dataclasses import dataclass
 from enum import Enum
-from typing import Optional, Iterable
+from typing import Optional
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class CommandType(Enum):
     SYSTEM_STATUS = 0x61
     USER_INTERFACE = 0x60
@@ -43,40 +43,40 @@
             return len(self.data)
         else:
             return int(len(self.data) / 2)
 
     @property
     def checksum(self) -> int:
         bytes = self.encode(with_checksum=False)
-        total = sum([ord(x) for x in bytes]) & 0xff
-        return 256 - total
+        total = sum([ord(x) for x in bytes]) & 0xFF
+        return (256 - total) % 256
 
     def encode(self, with_checksum: bool = True) -> str:
-        data = ''
-        data += '{:02x}'.format(self.start)
+        data = ""
+        data += "{:02x}".format(self.start)
 
         if self.address is not None:
             if is_user_interface_req(self.start):
-                data += '{:01x}'.format(self.address)
+                data += "{:01x}".format(self.address)
             else:
-                data += '{:02x}'.format(self.address)
+                data += "{:02x}".format(self.address)
 
-        data += '{:02x}'.format(self.length_field)
-        data += '{:02x}'.format(self.command.value)
+        data += "{:02x}".format(self.length_field)
+        data += "{:02x}".format(self.command.value)
         data += self.data
         if self.timestamp is not None:
-            data += self.timestamp.strftime('%y%m%d%H%M%S')
+            data += self.timestamp.strftime("%y%m%d%H%M%S")
 
         if with_checksum:
-            data += '{:02x}'.format(self.checksum).upper()
+            data += "{:02x}".format(self.checksum).upper()
 
         return data
 
     @classmethod
-    def decode(cls, _data: str) -> 'Packet':
+    def decode(cls, _data: str) -> "Packet":
         """
         Packets are ASCII encoded data. Packet layout is as follows:
 
         +---------------------------------------------------------------------------+
         | start | address | length | command | data | timestamp | checksum | finish |
         | hex   | hex     | hex    | hex     | str  | dec       | hex      | crlf   |
         | 1     | 1       | 1      | 1       | n    | 6         | 1        |        |
@@ -103,35 +103,36 @@
 
         data = DataIterator(_data)
         _LOGGER.debug("Decoding bytes: '%s'", _data)
 
         start = data.take_hex()
 
         address = None
-        if has_address(start):
+        if has_address(start, len(_data)):
             address = data.take_hex(half=is_user_interface_req(start))
 
         length = data.take_hex()
-        data_length = length & 0x7f
+        data_length = length & 0x7F
         seq = length >> 7
         command = CommandType(data.take_hex())
         msg_data = data.take_bytes(data_length, half=is_user_interface_req(start))
         timestamp = None
         if has_timestamp(start):
             timestamp = decode_timestamp(data.take_bytes(6))
 
         # TODO(NW): Figure out checksum validation
-        checksum = data.take_hex() # noqa
+        checksum = data.take_hex()  # noqa
 
         if not data.is_consumed():
-            raise ValueError('Unable to consume all data')
+            raise ValueError("Unable to consume all data")
 
         return Packet(
-            is_user_interface_resp=(is_user_interface_resp(start) and
-                                    command == CommandType.USER_INTERFACE),
+            is_user_interface_resp=(
+                is_user_interface_resp(start) and command == CommandType.USER_INTERFACE
+            ),
             address=address,
             seq=seq,
             command=command,
             data=msg_data,
             timestamp=timestamp,
         )
 
@@ -144,28 +145,34 @@
     def take_bytes(self, n: int, half: bool = False) -> str:
         multi = 2 if not half else 1
         position = self._position
         self._position += n * multi
         if self._position > len(self._data):
             raise ValueError("Unable to take more data than exists")
 
-        return self._data[position:self._position]
+        return self._data[position : self._position]
 
     def take_hex(self, half: bool = False) -> int:
         return int(self.take_bytes(1, half), 16)
 
     def take_dec(self, half: bool = False) -> int:
         return int(self.take_bytes(1, half), 10)
 
     def is_consumed(self) -> bool:
         return self._position >= len(self._data)
 
 
-def has_address(start: int) -> bool:
-    return bool(0x01 & start) or start == 0x82
+def has_address(start: int, data_length: int) -> bool:
+    """
+    Determine whether the packet has an "address" encoded into it.
+    There exists an undocumented bug/edge case in the spec - some packets
+    with 0x82 as _start_, still encode the address into the packet, and thus
+    throws off decoding. This edge case is handled explicitly.
+    """
+    return bool(0x01 & start) or (start == 0x82 and data_length == 16)
 
 
 def has_timestamp(start: int) -> bool:
     return bool(0x04 & start)
 
 
 def is_user_interface_req(start: int) -> bool:
@@ -173,21 +180,27 @@
 
 
 def is_user_interface_resp(start: int) -> bool:
     return start == 0x82
 
 
 def decode_timestamp(data: str) -> datetime.datetime:
-    return datetime.datetime.strptime(data, '%y%m%d%H%M%S')
-
-
-def split_string(x: str, n: int) -> Iterable[str]:
-    for i in range(0, len(x), n):
-        yield x[i:i + n]
-
-
-def is_data_valid(data: str) -> bool:
-    sum = 0
-    for byte in split_string(data, 2):
-        sum += int(byte, 16)
-
-    return sum & 0xff == 0
+    """
+    Decode timestamp using bespoke decoder.
+    Cannot use simple strptime since the ness panel contains a bug
+    that P199E zone and state updates emitted on the hour cause a minute
+    value of `60` to be sent, causing strptime to fail. This decoder handles
+    this edge case.
+    """
+    year = 2000 + int(data[0:2])
+    month = int(data[2:4])
+    day = int(data[4:6])
+    hour = int(data[6:8])
+    minute = int(data[8:10])
+    second = int(data[10:12])
+    if minute == 60:
+        minute = 0
+        hour += 1
+
+    return datetime.datetime(
+        year=year, month=month, day=day, hour=hour, minute=minute, second=second
+    )
```

### Comparing `nessclient-0.9.9/nessclient/alarm.py` & `nessclient-1.0.0/nessclient/alarm.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,78 +2,107 @@
 from enum import Enum
 from typing import Optional, Callable, List
 
 from .event import BaseEvent, ZoneUpdate, ArmingUpdate, SystemStatusEvent
 
 
 class ArmingState(Enum):
-    UNKNOWN = 'UNKNOWN'
-    DISARMED = 'DISARMED'
-    ARMING = 'ARMING'
-    EXIT_DELAY = 'EXIT_DELAY'
-    ARMED = 'ARMED'
-    ENTRY_DELAY = 'ENTRY_DELAY'
-    TRIGGERED = 'TRIGGERED'
+    UNKNOWN = "UNKNOWN"
+    DISARMED = "DISARMED"
+    ARMING = "ARMING"
+    EXIT_DELAY = "EXIT_DELAY"
+    ARMED = "ARMED"
+    ENTRY_DELAY = "ENTRY_DELAY"
+    TRIGGERED = "TRIGGERED"
+
+
+class ArmingMode(Enum):
+    ARMED_AWAY = "ARMED_AWAY"
+    ARMED_HOME = "ARMED_HOME"
+    ARMED_DAY = "ARMED_DAY"
+    ARMED_NIGHT = "ARMED_NIGHT"
+    ARMED_VACATION = "ARMED_VACATION"
+    ARMED_HIGHEST = "ARMED_HIGHEST"
 
 
 class Alarm:
     """
-    In-memory representation of the state of the alarm the client is connected to.
-
-    TODO(NW): Handle output state events to determine when alarm is on/off
+    In-memory representation of the state of the alarm the client is connected
+    to.
     """
-    ARM_EVENTS = [
-        SystemStatusEvent.EventType.ARMED_AWAY,
-        SystemStatusEvent.EventType.ARMED_HOME,
-        SystemStatusEvent.EventType.ARMED_DAY,
-        SystemStatusEvent.EventType.ARMED_NIGHT,
-        SystemStatusEvent.EventType.ARMED_VACATION,
-        SystemStatusEvent.EventType.ARMED_HIGHEST
-    ]
+
+    ARM_EVENTS_MAP = {
+        SystemStatusEvent.EventType.ARMED_AWAY: ArmingMode.ARMED_AWAY,
+        SystemStatusEvent.EventType.ARMED_HOME: ArmingMode.ARMED_HOME,
+        SystemStatusEvent.EventType.ARMED_DAY: ArmingMode.ARMED_DAY,
+        SystemStatusEvent.EventType.ARMED_NIGHT: ArmingMode.ARMED_NIGHT,
+        SystemStatusEvent.EventType.ARMED_VACATION: ArmingMode.ARMED_VACATION,
+        SystemStatusEvent.EventType.ARMED_HIGHEST: ArmingMode.ARMED_HIGHEST,
+    }
 
     @dataclass
     class Zone:
         triggered: Optional[bool]
 
-    def __init__(self) -> None:
+    def __init__(self, infer_arming_state: bool = False) -> None:
+        self._infer_arming_state = infer_arming_state
         self.arming_state: ArmingState = ArmingState.UNKNOWN
         self.zones: List[Alarm.Zone] = [Alarm.Zone(triggered=None) for _ in range(16)]
 
-        self._on_state_change: Optional[Callable[['ArmingState'], None]] = None
+        self._arming_mode: ArmingMode | None = None
+
+        self._on_state_change: Optional[
+            Callable[[ArmingState, ArmingMode | None], None]
+        ] = None
         self._on_zone_change: Optional[Callable[[int, bool], None]] = None
 
     def handle_event(self, event: BaseEvent) -> None:
         if isinstance(event, ArmingUpdate):
             self._handle_arming_update(event)
-        elif (isinstance(event, ZoneUpdate)
-              and event.request_id == ZoneUpdate.RequestID.ZONE_INPUT_UNSEALED):
+        elif (
+            isinstance(event, ZoneUpdate)
+            and event.request_id == ZoneUpdate.RequestID.ZONE_INPUT_UNSEALED
+        ):
             self._handle_zone_input_update(event)
         elif isinstance(event, SystemStatusEvent):
             self._handle_system_status_event(event)
 
     def _handle_arming_update(self, update: ArmingUpdate) -> None:
-        if update.status == [ArmingUpdate.ArmingStatus.MANUAL_EXCLUDE_MODE]:
+        if update.status == [ArmingUpdate.ArmingStatus.AREA_1_ARMED]:
             return self._update_arming_state(ArmingState.EXIT_DELAY)
-        if ArmingUpdate.ArmingStatus.MANUAL_EXCLUDE_MODE in update.status and \
-                ArmingUpdate.ArmingStatus.DAY_ZONE_SELECT:
-            # TODO(NW): This might not be the correct condition for an "armed"
-            #  system, in fact, the same states are shown throughout armed, and
-            #  entry delay. We should determine a better way to query the
-            #  current alarm state.
+        if (
+            ArmingUpdate.ArmingStatus.AREA_1_ARMED in update.status
+            and ArmingUpdate.ArmingStatus.AREA_1_FULLY_ARMED in update.status
+        ):
             return self._update_arming_state(ArmingState.ARMED)
-        elif self.arming_state == ArmingState.UNKNOWN:
-            # TODO(NW): Initially update to disarmed when the state is unknown.
-            #  In the future, it would be ideal to infer other states by making
-            #  calls to other status commands (i.e. zones in delay).
-            return self._update_arming_state(ArmingState.DISARMED)
+        else:
+            if self._infer_arming_state:
+                # State inference is enabled. Therefore the arming state can
+                # only be reverted to disarmed via a system status event.
+                # This works around a bug with some panels (<v5.8) which emit
+                # update.status = [] when they are armed.
+                # TODO(NW): It would be ideal to find a better way to
+                #  query this information on-demand, but for now this should
+                #  resolve the issue.
+                if self.arming_state == ArmingState.UNKNOWN:
+                    return self._update_arming_state(ArmingState.DISARMED)
+            else:
+                # State inference is disabled, therefore we can assume the
+                # panel is "disarmed" as it did not have any arming flags set
+                # in the arming update status as per the documentation.
+                # Note: This may not be correct and may not correctly represent
+                # other modes of arming other than ARMED_AWAY.
+                # TODO(NW): Perform some testing to determine how the client
+                #  handles other arming modes.
+                return self._update_arming_state(ArmingState.DISARMED)
 
     def _handle_zone_input_update(self, update: ZoneUpdate) -> None:
         for i, zone in enumerate(self.zones):
             zone_id = i + 1
-            name = 'ZONE_{}'.format(zone_id)
+            name = "ZONE_{}".format(zone_id)
             if ZoneUpdate.Zone[name] in update.included_zones:
                 self._update_zone(zone_id, True)
             else:
                 self._update_zone(zone_id, False)
 
     def _handle_system_status_event(self, event: SystemStatusEvent) -> None:
         """
@@ -88,36 +117,49 @@
         if event.type == SystemStatusEvent.EventType.UNSEALED:
             return self._update_zone(event.zone, True)
         elif event.type == SystemStatusEvent.EventType.SEALED:
             return self._update_zone(event.zone, False)
         elif event.type == SystemStatusEvent.EventType.ALARM:
             return self._update_arming_state(ArmingState.TRIGGERED)
         elif event.type == SystemStatusEvent.EventType.ALARM_RESTORE:
-            return self._update_arming_state(ArmingState.ARMED)
+            if self.arming_state != ArmingState.DISARMED:
+                return self._update_arming_state(ArmingState.ARMED)
         elif event.type == SystemStatusEvent.EventType.ENTRY_DELAY_START:
             return self._update_arming_state(ArmingState.ENTRY_DELAY)
         elif event.type == SystemStatusEvent.EventType.ENTRY_DELAY_END:
             pass
         elif event.type == SystemStatusEvent.EventType.EXIT_DELAY_START:
             return self._update_arming_state(ArmingState.EXIT_DELAY)
         elif event.type == SystemStatusEvent.EventType.EXIT_DELAY_END:
             # Exit delay finished - if we were in the process of arming update
             # state to armed
             if self.arming_state == ArmingState.EXIT_DELAY:
-                self._update_arming_state(ArmingState.ARMED)
-        elif event.type in Alarm.ARM_EVENTS:
+                return self._update_arming_state(ArmingState.ARMED)
+        elif event.type in Alarm.ARM_EVENTS_MAP.keys():
+            self._arming_mode = Alarm.ARM_EVENTS_MAP[event.type]
             return self._update_arming_state(ArmingState.ARMING)
         elif event.type == SystemStatusEvent.EventType.DISARMED:
+            self._arming_mode = None  # Restore arming mode on disarmed.
             return self._update_arming_state(ArmingState.DISARMED)
         elif event.type == SystemStatusEvent.EventType.ARMING_DELAYED:
             pass
 
-    def _update_arming_state(self, state: 'ArmingState') -> None:
-        if self._on_state_change is not None and self.arming_state != state:
+    def _update_arming_state(self, state: ArmingState) -> None:
+        if self.arming_state != state:
             self.arming_state = state
-            self._on_state_change(state)
+            if self._on_state_change is not None:
+                self._on_state_change(state, self._arming_mode)
 
     def _update_zone(self, zone_id: int, state: bool) -> None:
         zone = self.zones[zone_id - 1]
-        if self._on_zone_change is not None and zone.triggered != state:
+        if zone.triggered != state:
             zone.triggered = state
-            self._on_zone_change(zone_id, state)
+            if self._on_zone_change is not None:
+                self._on_zone_change(zone_id, state)
+
+    def on_state_change(
+        self, f: Callable[[ArmingState, ArmingMode | None], None]
+    ) -> None:
+        self._on_state_change = f
+
+    def on_zone_change(self, f: Callable[[int, bool], None]) -> None:
+        self._on_zone_change = f
```

### Comparing `nessclient-0.9.9/setup.py` & `nessclient-1.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 import os
+import sys
 
 from setuptools import setup
 
-
-def get_version():
-    version_path = os.path.join(
-        os.path.dirname(os.path.abspath(__file__)),
-        'VERSION')
-    v = open(version_path).read()
-    if type(v) == str:
-        return v.strip()
-    return v.decode('UTF-8').strip()
-
-
 readme_path = os.path.join(os.path.dirname(
     os.path.abspath(__file__)),
     'README.md',
 )
 long_description = open(readme_path).read()
 
 try:
     version = get_version()
 except Exception:
     version = '0.0.0-dev'
 
+needs_pytest = {'pytest', 'test', 'ptr'}.intersection(sys.argv)
+pytest_runner = ['pytest-runner'] if needs_pytest else []
+
 setup(
     name='nessclient',
-    version=version,
     packages=['nessclient', 'nessclient.cli', 'nessclient.cli.server'],
     author="Nick Whyte",
     author_email='nick@nickwhyte.com',
     description="Implementation/abstraction of the Ness D8x / D16x Serial "
                 "Interface ASCII protocol",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nickw444/nessclient',
     zip_safe=False,
     classifiers=[
         'Intended Audience :: Developers',
         'Programming Language :: Python',
     ],
-    test_suite="nessclient_tests",
     install_requires=[
         'justbackoff',
         'dataclasses;python_version<"3.7"'
     ],
     extras_require={
         'cli': ['click']
     },
     entry_points={
         'console_scripts': ['ness-cli=nessclient.cli.__main__:cli'],
-    }
+    },
+    test_suite='nessclient_tests',
+    setup_requires=[] + pytest_runner,
+    tests_require=['pytest', 'pytest-asyncio'],
 )
```

### Comparing `nessclient-0.9.9/LICENSE` & `nessclient-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nessclient-0.9.9/PKG-INFO` & `nessclient-1.0.0/nessclient.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,55 @@
 Metadata-Version: 2.1
 Name: nessclient
-Version: 0.9.9
+Version: 1.0.0
 Summary: Implementation/abstraction of the Ness D8x / D16x Serial Interface ASCII protocol
 Home-page: https://github.com/nickw444/nessclient
 Author: Nick Whyte
 Author-email: nick@nickwhyte.com
-License: UNKNOWN
-Description: # nessclient
-        
-        [![](https://travis-ci.org/nickw444/nessclient.svg?branch=master)](https://travis-ci.org/nickw444/nessclient)
-        [![](https://coveralls.io/repos/nickw444/nessclient/badge.svg)](https://coveralls.io/r/nickw444/nessclient)
-        [![](https://img.shields.io/pypi/v/nessclient.svg)](https://pypi.python.org/pypi/nessclient/)
-        [![](https://readthedocs.org/projects/nessclient/badge/?version=latest&style=flat)](https://nessclient.readthedocs.io/en/latest/)
-        
-        A python implementation/abstraction of the [Ness D8x / D16x Serial Interface ASCII protocol](http://www.nesscorporation.com/Software/Ness_D8-D16_ASCII_protocol.pdf)
-        
-        ## Installing nessclient
-        
-        `nessclient` is available directly from pip:
-        
-        ```sh
-        pip install nessclient
-        ```
-        
-        ## Documentation
-        
-        The full documentation can be found at [Read the Docs](https://nessclient.readthedocs.io/en/latest/)
-        
-        ## CLI
-        
-        This package includes a CLI which uses the library to interface with the Ness Serial Interface. You can read more in [the docs](https://nessclient.readthedocs.io/en/latest/cli.html)
-        
-        To use the CLI you must install it's dependencies by installing it with extras for `cli`: 
-        
-        ```
-        pip install nessclient[cli]
-        ness-cli --help
-        ``` 
-        
-        ## API Documentation
-        You can find the full API documentation [here](https://nessclient.readthedocs.io/en/latest/api.html)
-        
-        ## Examples
-        
-        Please see [Examples](https://nessclient.readthedocs.io/en/latest/examples.html) section in the docs for examples. These same examples can be found as source in the [examples/](examples) directory. 
-         
-        ## Developing
-        
-        Please see [Developing](https://nessclient.readthedocs.io/en/latest/developing.html) section in the docs for development environment setup information.
-        
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown
 Provides-Extra: cli
+License-File: LICENSE
+
+# nessclient
+
+[![](https://travis-ci.org/nickw444/nessclient.svg?branch=master)](https://travis-ci.org/nickw444/nessclient)
+[![codecov](https://codecov.io/gh/nickw444/nessclient/branch/master/graph/badge.svg)](https://codecov.io/gh/nickw444/nessclient)
+[![](https://img.shields.io/pypi/v/nessclient.svg)](https://pypi.python.org/pypi/nessclient/)
+[![](https://readthedocs.org/projects/nessclient/badge/?version=latest&style=flat)](https://nessclient.readthedocs.io/en/latest/)
+
+A python implementation/abstraction of the [Ness D8x / D16x Serial Interface ASCII protocol](http://www.nesscorporation.com/Software/Ness_D8-D16_ASCII_protocol_rev13.pdf)
+
+## Installing nessclient
+
+`nessclient` is available directly from pip:
+
+```sh
+pip install nessclient
+```
+
+## Documentation
+
+The full documentation can be found at [Read the Docs](https://nessclient.readthedocs.io/en/latest/)
+
+## CLI
+
+This package includes a CLI which uses the library to interface with the Ness Serial Interface. You can read more in [the docs](https://nessclient.readthedocs.io/en/latest/cli.html)
+
+To use the CLI you must install it's dependencies by installing it with extras for `cli`: 
+
+```
+pip install nessclient[cli]
+ness-cli --help
+``` 
+
+## API Documentation
+You can find the full API documentation [here](https://nessclient.readthedocs.io/en/latest/api.html)
+
+## Examples
+
+Please see [Examples](https://nessclient.readthedocs.io/en/latest/examples.html) section in the docs for examples. These same examples can be found as source in the [examples/](examples) directory. 
+ 
+## Developing
+
+Please see [Developing](https://nessclient.readthedocs.io/en/latest/developing.html) section in the docs for development environment setup information.
```

