# Comparing `tmp/openbci-stream-1.0b1.post3.tar.gz` & `tmp/openbci-stream-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/openbci-stream-1.0b1.post3.tar", last modified: Mon Nov  2 23:14:07 2020, max compression
+gzip compressed data, was "openbci-stream-1.1.0.tar", last modified: Thu Jun  8 22:17:08 2023, max compression
```

## Comparing `openbci-stream-1.0b1.post3.tar` & `openbci-stream-1.1.0.tar`

### file list

```diff
@@ -1,38 +1,48 @@
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.278197 openbci-stream-1.0b1.post3/
--rw-r--r--   0 yeison    (1000) users      (985)      253 2020-10-25 17:00:20.000000 openbci-stream-1.0b1.post3/MANIFEST.in
--rw-r--r--   0 yeison    (1000) users      (985)     4981 2020-11-02 23:14:07.278197 openbci-stream-1.0b1.post3/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (985)     3423 2020-11-02 21:13:00.000000 openbci-stream-1.0b1.post3/README.md
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.274864 openbci-stream-1.0b1.post3/cmd/
--rw-r--r--   0 yeison    (1000) users      (985)       80 2020-10-19 21:11:47.000000 openbci-stream-1.0b1.post3/cmd/openbci_cli
--rw-r--r--   0 yeison    (1000) users      (985)     1201 2020-10-26 00:43:06.000000 openbci-stream-1.0b1.post3/cmd/stream_access_point.sh
--rw-r--r--   0 yeison    (1000) users      (985)     1271 2020-10-26 14:58:39.000000 openbci-stream-1.0b1.post3/cmd/stream_configure_kafka.sh
--rw-r--r--   0 yeison    (1000) users      (985)      397 2020-10-25 23:39:03.000000 openbci-stream-1.0b1.post3/cmd/stream_eeg
--rw-r--r--   0 yeison    (1000) users      (985)      366 2020-10-25 23:39:24.000000 openbci-stream-1.0b1.post3/cmd/stream_rpyc
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.274864 openbci-stream-1.0b1.post3/openbci_stream/
--rw-r--r--   0 yeison    (1000) users      (985)      348 2020-10-27 21:24:23.000000 openbci-stream-1.0b1.post3/openbci_stream/__init__.py
--rw-r--r--   0 yeison    (1000) users      (985)        8 2020-11-02 23:13:50.000000 openbci-stream-1.0b1.post3/openbci_stream/_version.txt
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.278197 openbci-stream-1.0b1.post3/openbci_stream/acquisition/
--rw-r--r--   0 yeison    (1000) users      (985)      138 2020-10-17 16:18:09.000000 openbci-stream-1.0b1.post3/openbci_stream/acquisition/__init__.py
--rw-r--r--   0 yeison    (1000) users      (985)     3121 2020-11-01 02:18:41.000000 openbci-stream-1.0b1.post3/openbci_stream/acquisition/binary_stream.py
--rw-r--r--   0 yeison    (1000) users      (985)     3986 2020-10-30 22:52:20.000000 openbci-stream-1.0b1.post3/openbci_stream/acquisition/consumer.py
--rw-r--r--   0 yeison    (1000) users      (985)    26572 2020-11-02 19:50:41.000000 openbci-stream-1.0b1.post3/openbci_stream/acquisition/cyton.py
--rw-r--r--   0 yeison    (1000) users      (985)    27283 2020-11-02 21:36:43.000000 openbci-stream-1.0b1.post3/openbci_stream/acquisition/cyton_base.py
--rw-r--r--   0 yeison    (1000) users      (985)     3212 2020-11-01 01:47:05.000000 openbci-stream-1.0b1.post3/openbci_stream/acquisition/tcp_server.py
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.278197 openbci-stream-1.0b1.post3/openbci_stream/daemons/
--rw-r--r--   0 yeison    (1000) users      (985)        0 2020-10-19 20:52:21.000000 openbci-stream-1.0b1.post3/openbci_stream/daemons/__init__.py
--rw-r--r--   0 yeison    (1000) users      (985)    14007 2020-11-02 21:20:35.000000 openbci-stream-1.0b1.post3/openbci_stream/daemons/stream_eeg.py
--rw-r--r--   0 yeison    (1000) users      (985)     1450 2020-10-29 16:54:32.000000 openbci-stream-1.0b1.post3/openbci_stream/daemons/stream_rpyc.py
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.278197 openbci-stream-1.0b1.post3/openbci_stream/utils/
--rw-r--r--   0 yeison    (1000) users      (985)      152 2020-10-29 14:55:50.000000 openbci-stream-1.0b1.post3/openbci_stream/utils/__init__.py
--rw-r--r--   0 yeison    (1000) users      (985)    21749 2020-10-30 22:06:54.000000 openbci-stream-1.0b1.post3/openbci_stream/utils/hdf5.py
--rw-r--r--   0 yeison    (1000) users      (985)     8584 2020-11-02 19:50:51.000000 openbci-stream-1.0b1.post3/openbci_stream/utils/openbci_cli.py
--rw-r--r--   0 yeison    (1000) users      (985)     1639 2020-10-29 14:17:28.000000 openbci-stream-1.0b1.post3/openbci_stream/utils/pid_admin.py
--rw-r--r--   0 yeison    (1000) users      (985)     1331 2020-11-01 03:08:25.000000 openbci-stream-1.0b1.post3/openbci_stream/utils/scan_wifi_modules.py
-drwxr-xr-x   0 yeison    (1000) users      (985)        0 2020-11-02 23:14:07.274864 openbci-stream-1.0b1.post3/openbci_stream.egg-info/
--rw-r--r--   0 yeison    (1000) users      (985)     4981 2020-11-02 23:14:06.000000 openbci-stream-1.0b1.post3/openbci_stream.egg-info/PKG-INFO
--rw-r--r--   0 yeison    (1000) users      (985)      902 2020-11-02 23:14:07.000000 openbci-stream-1.0b1.post3/openbci_stream.egg-info/SOURCES.txt
--rw-r--r--   0 yeison    (1000) users      (985)        1 2020-11-02 23:14:06.000000 openbci-stream-1.0b1.post3/openbci_stream.egg-info/dependency_links.txt
--rw-r--r--   0 yeison    (1000) users      (985)      175 2020-11-02 23:14:06.000000 openbci-stream-1.0b1.post3/openbci_stream.egg-info/requires.txt
--rw-r--r--   0 yeison    (1000) users      (985)       15 2020-11-02 23:14:06.000000 openbci-stream-1.0b1.post3/openbci_stream.egg-info/top_level.txt
--rw-r--r--   0 yeison    (1000) users      (985)       38 2020-11-02 23:14:07.278197 openbci-stream-1.0b1.post3/setup.cfg
--rw-r--r--   0 yeison    (1000) users      (985)     2741 2020-11-02 23:13:46.000000 openbci-stream-1.0b1.post3/setup.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/
+-rw-r--r--   0 yeison    (1000) users      (984)     1315 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/LICENSE
+-rw-r--r--   0 yeison    (1000) users      (984)      269 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/MANIFEST.in
+-rw-r--r--   0 yeison    (1000) users      (984)     7435 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)     6117 2022-03-20 15:39:33.000000 openbci-stream-1.1.0/README.md
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.312326 openbci-stream-1.1.0/cmd/
+-rw-r--r--   0 yeison    (1000) users      (984)       80 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/cmd/openbci_cli
+-rw-r--r--   0 yeison    (1000) users      (984)     1217 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/cmd/stream_access_point.sh
+-rw-r--r--   0 yeison    (1000) users      (984)      976 2021-09-22 21:11:42.000000 openbci-stream-1.1.0/cmd/stream_bin2eeg
+-rw-r--r--   0 yeison    (1000) users      (984)     5632 2021-10-24 02:24:06.000000 openbci-stream-1.1.0/cmd/stream_configure_kafka.sh
+-rw-r--r--   0 yeison    (1000) users      (984)     1199 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/cmd/stream_configure_ntpd.sh
+-rw-r--r--   0 yeison    (1000) users      (984)      415 2021-09-22 21:00:52.000000 openbci-stream-1.1.0/cmd/stream_eeg
+-rw-r--r--   0 yeison    (1000) users      (984)       89 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/cmd/stream_fake_binary
+-rw-r--r--   0 yeison    (1000) users      (984)      268 2021-09-21 16:20:17.000000 openbci-stream-1.1.0/cmd/stream_install_kafka.sh
+-rw-r--r--   0 yeison    (1000) users      (984)      402 2022-06-05 18:27:36.000000 openbci-stream-1.1.0/cmd/stream_rpyc
+-rw-r--r--   0 yeison    (1000) users      (984)      562 2021-10-24 02:18:48.000000 openbci-stream-1.1.0/cmd/stream_tlwr.sh
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.312326 openbci-stream-1.1.0/openbci_stream/
+-rw-r--r--   0 yeison    (1000) users      (984)      419 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)        6 2023-06-08 22:17:00.000000 openbci-stream-1.1.0/openbci_stream/_version.txt
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/openbci_stream/acquisition/
+-rw-r--r--   0 yeison    (1000) users      (984)      162 2021-10-20 20:57:37.000000 openbci-stream-1.1.0/openbci_stream/acquisition/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3362 2021-10-24 18:45:32.000000 openbci-stream-1.1.0/openbci_stream/acquisition/binary_stream.py
+-rw-r--r--   0 yeison    (1000) users      (984)     4734 2021-09-21 16:20:38.000000 openbci-stream-1.1.0/openbci_stream/acquisition/consumer.py
+-rw-r--r--   0 yeison    (1000) users      (984)    38136 2022-07-27 23:38:20.000000 openbci-stream-1.1.0/openbci_stream/acquisition/cyton.py
+-rw-r--r--   0 yeison    (1000) users      (984)    28536 2022-03-22 04:31:44.000000 openbci-stream-1.1.0/openbci_stream/acquisition/cyton_base.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3422 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/acquisition/tcp_server.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/openbci_stream/daemons/
+-rw-r--r--   0 yeison    (1000) users      (984)        0 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/daemons/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)    17606 2022-04-19 01:10:56.000000 openbci-stream-1.1.0/openbci_stream/daemons/stream_bin2eeg.py
+-rw-r--r--   0 yeison    (1000) users      (984)     7694 2022-04-18 22:49:41.000000 openbci-stream-1.1.0/openbci_stream/daemons/stream_eeg.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1747 2021-10-24 18:39:56.000000 openbci-stream-1.1.0/openbci_stream/daemons/stream_fake_binary.py
+-rw-r--r--   0 yeison    (1000) users      (984)     3929 2021-10-20 21:01:22.000000 openbci-stream-1.1.0/openbci_stream/daemons/stream_rpyc.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/openbci_stream/utils/
+-rw-r--r--   0 yeison    (1000) users      (984)      152 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/utils/__init__.py
+-rw-r--r--   0 yeison    (1000) users      (984)    11630 2022-03-06 01:47:11.000000 openbci-stream-1.1.0/openbci_stream/utils/filters.py
+-rw-r--r--   0 yeison    (1000) users      (984)    40580 2023-04-14 16:28:18.000000 openbci-stream-1.1.0/openbci_stream/utils/hdf5.py
+-rw-r--r--   0 yeison    (1000) users      (984)     8932 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/utils/openbci_cli.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1639 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/utils/pid_admin.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1331 2021-05-25 23:59:35.000000 openbci-stream-1.1.0/openbci_stream/utils/scan_wifi_modules.py
+-rw-r--r--   0 yeison    (1000) users      (984)     1707 2022-03-06 01:38:59.000000 openbci-stream-1.1.0/openbci_stream/utils/viz.py
+drwxr-xr-x   0 yeison    (1000) users      (984)        0 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/openbci_stream.egg-info/
+-rw-r--r--   0 yeison    (1000) users      (984)     7435 2023-06-08 22:17:08.000000 openbci-stream-1.1.0/openbci_stream.egg-info/PKG-INFO
+-rw-r--r--   0 yeison    (1000) users      (984)     1174 2023-06-08 22:17:08.000000 openbci-stream-1.1.0/openbci_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 yeison    (1000) users      (984)        1 2023-06-08 22:17:08.000000 openbci-stream-1.1.0/openbci_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 yeison    (1000) users      (984)      114 2023-06-08 22:17:08.000000 openbci-stream-1.1.0/openbci_stream.egg-info/requires.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       15 2023-06-08 22:17:08.000000 openbci-stream-1.1.0/openbci_stream.egg-info/top_level.txt
+-rw-r--r--   0 yeison    (1000) users      (984)       38 2023-06-08 22:17:08.315659 openbci-stream-1.1.0/setup.cfg
+-rw-r--r--   0 yeison    (1000) users      (984)     2672 2023-06-08 22:15:26.000000 openbci-stream-1.1.0/setup.py
```

### Comparing `openbci-stream-1.0b1.post3/cmd/stream_access_point.sh` & `openbci-stream-1.1.0/cmd/stream_access_point.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/bash
 
-pacman -S hostapd dnsmasq
+pacman -S --needed hostapd dnsmasq dhcpcd
 systemctl enable hostapd dnsmasq dhcpcd
 systemctl start hostapd dnsmasq dhcpcd
 
 SSID=OpenBCI-Stream
 PASSPHRASE=raspberrypi
 
 function secure_file {
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/acquisition/binary_stream.py` & `openbci-stream-1.1.0/openbci_stream/acquisition/binary_stream.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,62 +2,64 @@
 =============
 Binary stream
 =============
 
 This module must be run in the same machine that OpenBCI hardware was attached.
 """
 
-from kafka import KafkaProducer
 import pickle
 import logging
-
+from datetime import datetime
 from typing import Dict, Any
 
+from kafka import KafkaProducer
+
 
 ########################################################################
 class BinaryStream:
     """Kafka producer for equal size packages streaming.
 
-    The dictionary streamed contain two objects: `contex` and `data`.
+    The dictionary streamed contain two objects: `data` and `context`.
+
+    **data:** Bytes with binary raw data.
 
     **context:** A dictionary with the following keys:
 
     * **created:**  The `timestamp` for the exact moment when binary data was read.
     * **daisy:** `True` if Daisy board is attached, otherwise `False`.
     * **boardmode:** Can be `default`, `digital`, ''analog', 'debug' or `marker`.
     * **montage:** A list means consecutive channels e.g. `['Fp1', 'Fp2', 'F3', 'Fz', 'F4']` and a dictionary means specific channels  `{1: 'Fp1', 2: 'Fp2', 3: 'F3', 4: 'Fz', 5: 'F4'}`.
     * **connection:** Can be `serial` or `wifi`.
     * **gain:** Array with gains.
 
-    **data:** Bytes with binary raw data.
-
     e.g
 
-    >>> contex = {'created': 1604196938.727064,
-                  'daisy': False,
-                  'boardmode': 'default',
-                  'montage': ['Fp1', 'Fp2', 'F3', 'Fz', 'F4'],
-                  'connection': 'wifi',
-                  'gain': [24, 24, 24, 24, 24, 24, 24, 24]
-                  }
+    >>> context = {'created': 1604196938.727064,
+                   'daisy': False,
+                   'boardmode': 'default',
+                   'montage': ['Fp1', 'Fp2', 'F3', 'Fz', 'F4'],
+                   'connection': 'wifi',
+                   'gain': [24, 24, 24, 24, 24, 24, 24, 24]
+                   }
     """
 
-    TOPIC = 'binary'
     accumulated = b''
 
     # ----------------------------------------------------------------------
-    def __init__(self, streaming_package_size: int) -> None:
+    def __init__(self, streaming_package_size: int, board_id: str = '') -> None:
         """
         Parameters
         ----------
         streaming_package_size
             The package size for streaming packages.
         """
 
-        logging.info(f'Creating {self.TOPIC} Produser')
+        self.topic = f'binary{board_id}'
+
+        logging.info(f'Creating {self.topic} Produser')
         self.streaming_package_size = streaming_package_size
         self.producer = KafkaProducer(bootstrap_servers=['localhost:9092'],
                                       compression_type='gzip',
                                       value_serializer=pickle.dumps,
                                       )
 
     # ----------------------------------------------------------------------
@@ -68,25 +70,26 @@
         all 16 channels, so the size of the packages is also doubled.
 
         Parameters
         ----------
         data
             Dictionary with context and raw binary data.
         """
+        self.accumulated += data['data']
 
         if data['context']['connection'] == 'wifi' and data['context']['daisy']:
             f = 2
         else:
             f = 1
+        size = self.streaming_package_size * 33 * f
 
-        if len(self.accumulated) > (self.streaming_package_size * 33 * f):
-            data['data'] = self.accumulated
-            self.producer.send(self.TOPIC, data)
-            self.accumulated = b''
+        if len(self.accumulated) >= size:
+            data['data'] = self.accumulated[:size]
+            data['context']['timestamp.binary'] = datetime.now().timestamp()
+            self.producer.send(self.topic, data)
+            self.accumulated = self.accumulated[size:]
 
     # ----------------------------------------------------------------------
     def close(self) -> None:
         """Terminate the produser."""
-        logging.info(f'Clossing {self.TOPIC} Produser')
+        logging.info(f'Clossing {self.topic} Produser')
         self.producer.close(timeout=0.3)
-
-
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/acquisition/consumer.py` & `openbci-stream-1.1.0/openbci_stream/acquisition/consumer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 OpenBCI Consumer
 ================
 """
 
 import pickle
 import logging
 from .cyton import Cyton
-from typing import Tuple, Optional, Union, Literal
+from typing import Tuple, Optional, Union, Literal, List
 
 from kafka import KafkaConsumer
 
 # Custom type var
 MODE = Literal['serial', 'wifi', None]
 DAISY = Literal['auto', True, False]
 
@@ -46,50 +46,70 @@
 
     Parameters
     ----------
     mode
         If specified, will try to start streaming with this connection mode.
     endpoint
         Serial port for RFduino or IP address for WiFi module.
-    host
-        IP address for the server that has the OpenBCI board attached, by
-        default its assume that is the same machine where is it executing, this
-        is the `localhost`.
     daisy
         Daisy board can be detected on runtime or declare it specifically.
     montage
         A list means consecutive channels e.g. `['Fp1', 'Fp2', 'F3', 'Fz',
         'F4']` and a dictionary means specific channels `{1: 'Fp1', 2: 'Fp2',
         3: 'F3', 4: 'Fz', 5: 'F4'}`.
     streaming_package_size
         The streamer will try to send packages of this size, this is NOT the
         sampling rate for data acquisition.
+    host
+        IP address for the server that has the OpenBCI board attached, by
+        default its assume that is the same machine where is it executing, this
+        is the `localhost`.
+    topics
+        List of topics to listen.
+    auto_start
+        If `mode` and `endpoint` are passed, then start the stream automatically.
     """
 
     # ----------------------------------------------------------------------
     def __init__(self, mode: MODE = None, endpoint: Optional[str] = None,
                  daisy: DAISY = 'auto',
                  montage: Optional[Union[list, dict]] = None,
-                 streaming_package_size: Optional[int] = None,
-                 host: Optional[str] = 'localhost') -> None:
+                 streaming_package_size: Optional[int] = 250,
+                 host: Optional[str] = 'localhost',
+                 topics: Optional[List[str]] = [
+                     'eeg', 'aux', 'marker', 'annotation'],
+                 auto_start: Optional[bool] = True,
+                 *args,
+                 **kwargs,
+                 ) -> None:
         """"""
 
         self.bootstrap_servers = [f'{host}:9092']
-        self.topics = ['eeg', 'marker']
+        self.topics = topics
+        self.auto_start = auto_start
 
         if mode:
-            self.openbci = Cyton(mode, endpoint, host,
-                                 daisy, False, montage, streaming_package_size)
+
+            self.openbci = Cyton(mode=mode,
+                                 endpoint=endpoint, host=host,
+                                 daisy=daisy,
+                                 capture_stream=False,
+                                 montage=montage,
+                                 streaming_package_size=streaming_package_size,
+                                 *args,
+                                 **kwargs,
+                                 )
 
     # ----------------------------------------------------------------------
     def __enter__(self) -> Tuple[KafkaConsumer, Optional[Cyton]]:
         """Start stream and create consumer."""
 
-        if hasattr(self, 'openbci'):
+        if hasattr(self, 'openbci') and self.auto_start:
             self.openbci.start_stream()
+
         self.consumer = KafkaConsumer(bootstrap_servers=self.bootstrap_servers,
                                       value_deserializer=pickle.loads,
                                       auto_offset_reset='latest',
                                       )
         self.consumer.subscribe(self.topics)
 
         if hasattr(self, 'openbci'):
@@ -107,7 +127,8 @@
 
         if exc_type:
             logging.warning(exc_type)
         if exc_val:
             logging.warning(exc_val)
         if exc_tb:
             logging.warning(exc_tb)
+
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/acquisition/cyton_base.py` & `openbci-stream-1.1.0/openbci_stream/acquisition/cyton_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 DAISY = Literal['auto', True, False]
 QUEUE = TypeVar('Queue')
 
 
 ########################################################################
 class CytonConstants:
-    """Default constants defined in the `Cyton SDK <https://docs.openbci.com/docs/02Cyton/CytonSDK>`_"""
+    """Default constants defined in the `Cyton SDK <https://docs.openbci.com/Cyton/CytonSDK/>`_"""
 
     VREF = 4.5
 
     BIN_HEADER = 0xa0
 
     VERSION = b'V'
     START_STREAM = b'b'
@@ -165,16 +165,16 @@
 
 ########################################################################
 class CytonBase(CytonConstants, metaclass=ABCMeta):
     """
     The Cyton data format and SDK define all interactions and capabilities of
     the board, the full instructions can be found in the official documentation.
 
-      * https://docs.openbci.com/Hardware/03-Cyton_Data_Format
-      * https://docs.openbci.com/OpenBCI%20Software/04-OpenBCI_Cyton_SDK
+      * https://docs.openbci.com/Cyton/CytonDataFormat/
+      * https://docs.openbci.com/Cyton/CytonSDK/
 
     daisy
         Daisy board can be detected on runtime or declare it specifically.
     montage
         A list means consecutive channels e.g. `['Fp1', 'Fp2', 'F3', 'Fz',
         'F4']` and a dictionary means specific channels `{1: 'Fp1', 2: 'Fp2',
         3: 'F3', 4: 'Fz', 5: 'F4'}`.
@@ -184,25 +184,32 @@
     capture_stream
         Indicates if the data from the stream will be captured in asynchronous
         mode.
     """
 
     # ----------------------------------------------------------------------
     def __init__(self, daisy: DAISY, montage: Optional[Union[list, dict]],
-                 streaming_package_size: int, capture_stream: bool) -> None:
+                 streaming_package_size: int, capture_stream: bool, board_id: str = '', parallel_boards: int = 1) -> None:
         """"""
-        # Default sample rate for serial and wifi mode
+        # Default values
         self.sample_rate = 250
+        self.boardmode = 'default'
+        self.closed = False
+        self.board_id = board_id
+        self.parallel_boards = parallel_boards
 
         # Daisy before Montage
         if daisy in [True, False]:
             self.daisy = daisy
         elif daisy == 'auto':
             self.daisy = self.daisy_attached()
 
+        # Gain
+        self._gain = None
+
         # Montage
         self.montage = montage
 
         # Data Structure with special queue that can live across process
         self._data_eeg = Manager().Queue()
         self._data_aux = Manager().Queue()
         self._data_markers = Manager().Queue()
@@ -210,29 +217,14 @@
 
         self.reset_input_buffer()
         self._auto_capture_stream = capture_stream
         self.streaming_package_size = streaming_package_size
 
     # ----------------------------------------------------------------------
     @property
-    def boardmode(self) -> str:
-        """Stop stream and ask for the current boardmode."""
-
-        self.command(self.STOP_STREAM)
-        response = self.command(self.BOARD_MODE_GET)
-
-        for mode in [b'analog', b'digital', b'debug', b'default', b'marker']:
-            if mode in response:
-                return mode.decode()
-
-        logging.warning(
-            'Stream must be stoped for read the current boardmode')
-
-    # ----------------------------------------------------------------------
-    @property
     def montage(self) -> Union[List, Dict]:
         """The current montage configured on initialization."""
         return self._montage
 
     # ----------------------------------------------------------------------
     @montage.setter
     def montage(self, montage: Union[List, Dict, None]) -> None:
@@ -249,23 +241,24 @@
             Object for generate the montage parameter.
         """
 
         if isinstance(montage, (bytes)):
             montage = pickle.loads(montage)
 
         if isinstance(montage, (list, tuple, range)):
-            self._montage = {i: ch for i, ch in enumerate(montage)}
+            self._montage = {i + 1: ch for i, ch in enumerate(montage)}
         elif isinstance(montage, (dict)):
-            self._montage = {i: ch for i, ch in enumerate(montage.values())}
+            self._montage = {i + 1: ch for i,
+                             ch in enumerate(montage.values())}
         else:
             # Default
             if self.daisy:
-                self._montage = {i: f'ch{i+1}' for i in range(16)}
+                self._montage = {i + 1: f'ch{i+1}' for i in range(16)}
             elif not self.daisy:
-                self._montage = {i: f'ch{i+1}' for i in range(8)}
+                self._montage = {i + 1: f'ch{i+1}' for i in range(8)}
 
     # ----------------------------------------------------------------------
     def deactivate_channel(self, channels: List[int]) -> None:
         """Deactivate the channels specified.
 
         Parameters
         ----------
@@ -295,15 +288,15 @@
     def command(self, c: Union[str, bytes]) -> str:
         """Send a command to device.
 
         Before send the commmand the input buffer is cleared, and after that
         waits 300 ms for a response. Is possible to send a raw bytes, a
         `CytonConstants` attribute or the constant name e.g.
 
-        >>> comand(b'~4')
+        >>> command(b'~4')
         >>> command(CytonConstants.SAMPLE_RATE_1KSPS)
         >>> command('SAMPLE_RATE_1KSPS')
 
         Parameters
         ----------
         c
             Command to send.
@@ -313,17 +306,22 @@
         str
             If the command generate a response this will be returned.
         """
 
         if hasattr(self, c.decode()):
             c = getattr(self, c.decode())
 
+        # asume that default is 250, then, new values are getted from commands
         if c in list(self.SAMPLE_RATE_VALUE.keys()):
             self.sample_rate = int(self.SAMPLE_RATE_VALUE[c])
 
+        # asume that default is `default`, then, new values are getted from commands
+        if c in list(self.BOARD_MODE_VALUE.keys()):
+            self.boardmode = self.BOARD_MODE_VALUE[c]
+
         self.reset_input_buffer()
         self.write(c)
         time.sleep(0.3)
         response = self.read(2**11)
         logging.info(f'Writing: {c}')
         if response and len(response) > 100:
             logging.info(f'Response: {response[:100]}...')
@@ -394,18 +392,28 @@
         """
 
         self.reset_input_buffer()
 
         start = b'x'
         end = b'X'
         chain = b''
-        for ch in channels:
+
+        if isinstance(srb2, (bytes, str)):
+            srb2 = [srb2] * len(channels)
+
+        for ch, srb2_ in zip(channels, srb2):
             ch = chr(self.CHANNEL_SETTING[ch - 1]).encode()
-            chain += b''.join([start, ch, power_down, gain, input_type, bias,
-                               srb2, srb1, end])
+
+            c = b''.join([start, ch, power_down, gain, input_type, bias, srb2_,
+                          srb1, end])
+            if len(chain + c) > 31:  # Over WiFi there is a limit of 31 chars
+                self.command(chain)
+                chain = c
+            else:
+                chain += c
 
         self.command(chain)
 
     # ----------------------------------------------------------------------
     def leadoff_impedance(self, channels: List[int],
                           pchan: Optional[bytes] = CytonConstants.TEST_SIGNAL_NOT_APPLIED,
                           nchan: Optional[bytes] = CytonConstants.TEST_SIGNAL_APPLIED) -> None:
@@ -417,43 +425,47 @@
             1-based indexing channels list that will share the configuration
             specified.
         pchan
             `TEST_SIGNAL_NOT_APPLIED` (default), `TEST_SIGNAL_APPLIED`.
         nchan
             `TEST_SIGNAL_APPLIED` (default), `TEST_SIGNAL_NOT_APPLIED`.
 
-
         Returns
         -------
-
         On success:
 
           * If streaming, no confirmation of success. Note: WiFi Shields will always get a response, even if streaming.
           * If not streaming, returns Success: Lead off set for 4$$$, where 4 is the channel that was requested to be set.
 
         On failure:
 
           * If not streaming, NOTE: WiFi shield always sends the following responses without $$$
 
               * Not enough characters received, Failure: too few chars$$$ (example user sends z102000Z)
               * 5th character is not the upper case ‘Z’, Failure: 5th char not Z$$$ (example user sends z1020000X)
               * Too many characters or some other issue, Failure: Err: too many chars$$$
           * If not all commands are not received within 1 second, Timeout processing multi byte message - please send all commands at once as of v2$$$
-
         """
 
         start = b'z'
         end = b'Z'
 
         self.reset_input_buffer()
         chain = b''
         for ch in channels:
             ch = chr(self.CHANNEL_SETTING[ch - 1]).encode()
-            chain += b''.join([start, ch, pchan, nchan, end])
-        self.command(chain)
+
+            c = b''.join([start, ch, pchan, nchan, end])
+            if len(chain + c) > 31:  # Over WiFi there is a limit of 31 chars
+                self.command(chain)
+                chain = c
+            else:
+                chain += c
+
+        return self.command(chain)
 
     # ----------------------------------------------------------------------
     def send_marker(self, marker: Union[str, bytes, int], burst: int = 4) -> None:
         """Send marker to device.
 
         The marker sended will be added to the `AUX` bytes in the next data
         input.
@@ -500,53 +512,69 @@
         response = self.command(self.USE_16CH_ONLY)
         if not response:
             return self.daisy_attached()
 
         daisy = not (('no daisy to attach' in response.decode(errors='ignore')) or
                      ('8' in response.decode(errors='ignore')))
 
-        return daisy
+        if daisy:
+            logging.info('Daisy detected.')
+        else:
+            logging.info('Daisy not detected.')
 
     # ----------------------------------------------------------------------
     def capture_stream(self) -> None:
         """Create a process for connecting to the stream and capture data from it."""
 
-        # For prevent circular import
+        # To prevent circular imports
         from .consumer import OpenBCIConsumer
 
         self.reset_buffers()
 
         def bulk_buffer():
             """"""
             with OpenBCIConsumer() as stream:
                 for message in stream:
                     if message.topic == 'eeg':
 
-                        eeg, aux = message.value['data']
-
+                        eeg = message.value['data']
                         self._data_eeg.put(eeg)
-                        self._data_aux.put(aux)
 
-                        timestamp = np.zeros(message.value['context']['samples'])
-                        timestamp[-1] = message.value['context']['created']
+                        timestamp = np.zeros(
+                            message.value['context']['samples'])
+                        timestamp[-1] = message.value['context']['timestamp.binary']
                         self._data_timestamp.put(timestamp)
 
+                    elif message.topic == 'aux':
+
+                        aux = message.value['data']
+                        self._data_aux.put(aux)
+
+                        # timestamp = np.zeros(message.value['context']['samples'])
+                        # timestamp[-1] = message.value['context']['timestamp.binary']
+                        # self._data_timestamp.put(timestamp)
+
                     elif message.topic == 'marker':
 
-                        timestamp = message.value['timestamp']
+                        # timestamp = message.value['timestamp']
+                        timestamp = message.timestamp / 1000
                         marker = message.value['marker']
                         self._data_markers.put((timestamp, marker))
 
         self.persistent_process = Process(target=bulk_buffer)
         self.persistent_process.start()
 
     # ----------------------------------------------------------------------
     def start_stream(self) -> None:
         """Create the binary stream channel."""
-        self.binary_stream = BinaryStream(self.streaming_package_size)
+        # self.binary_stream = BinaryStream(
+            # self.streaming_package_size, self.board_id)
+        if not hasattr(set, 'binary_stream'):
+            self.binary_stream = BinaryStream(
+                self.streaming_package_size, self.board_id)
 
         self.reset_buffers()
         self.reset_input_buffer()
 
         if self._auto_capture_stream:
             self.capture_stream()
 
@@ -557,14 +585,15 @@
             self.persistent_process.terminate()
             self.persistent_process.join()
 
     # ----------------------------------------------------------------------
     @abstractmethod
     def close(self):
         """Stops data stream."""
+        self.closed = True
 
     # ----------------------------------------------------------------------
     @abstractmethod
     def write(self):
         """Write bytes."""
 
     # ----------------------------------------------------------------------
@@ -633,15 +662,16 @@
     def timestamp_time_series(self) -> np.ndarray:
         """Return timestamps acquired.
 
         Since there is only one timestamp for package, the others values are
         interpolated.
         """
 
-        timestamp = [self._data_timestamp.get() for _ in range(self._data_timestamp.qsize())]
+        timestamp = [self._data_timestamp.get()
+                     for _ in range(self._data_timestamp.qsize())]
         timestamp = np.concatenate(timestamp, axis=0)
         length = self.eeg_time_series.shape[1]
         sample_rate = self.sample_rate
 
         timestamp = interpolate_datetime(timestamp, length)
 
         return timestamp
@@ -758,20 +788,23 @@
             writer.add_header(header)
 
             eeg = self.eeg_time_series
             time = self.timestamp_time_series
             aux = self.aux_time_series
 
             writer.add_eeg(eeg, time)
-            writer.add_aux(aux)
+            writer.add_aux(aux, time)
             writer.add_markers(self.markers)
 
-            logging.info(f'Writed a vector of shape ({eeg.shape}) for EEG data')
-            logging.info(f'Writed a vector of shape ({time.shape}) for time data')
-            logging.info(f'Writed a vector of shape ({aux.shape}) for aux data')
+            logging.info(
+                f'Writed a vector of shape ({eeg.shape}) for EEG data')
+            logging.info(
+                f'Writed a vector of shape ({time.shape}) for time data')
+            logging.info(
+                f'Writed a vector of shape ({aux.shape}) for aux data')
 
             if bool(self.markers):
                 logging.info(f'Writed {self.markers.keys()} markers')
 
     # ----------------------------------------------------------------------
     def __getattribute__(self, attr: str) -> Any:
         """Some attributes must be acceded from RPyC."""
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/acquisition/tcp_server.py` & `openbci-stream-1.1.0/openbci_stream/acquisition/tcp_server.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,30 +22,30 @@
     Parameters
     ----------
     host
         IP address of the machine that WiFi module will connect.
     binary_stream
         Function that return a kafka producer, this producer could not exist in
         the very moment of creation of this class instance.
-    context
-        Information from the acquisition side useful for deserializing and that
-        will be packaged back in the stream.
+    kafka_context
+        Funtion that return the information from the acquisition side useful for
+        deserializing and will be packaged back in the stream.
     """
 
     # ----------------------------------------------------------------------
-    def __init__(self, host, binary_stream: Callable, kafka_context: Dict[str, Any] = {}) -> None:
+    def __init__(self, host, binary_stream: Callable, kafka_context: Callable) -> None:
         """"""
         asyncore.dispatcher.__init__(self)
         self.create_socket(socket.AF_INET, socket.SOCK_STREAM)
 
         self.set_reuse_addr()
         self.bind((host, 0))
         self.listen(1)
         # self.data = data_queue
-        self.kafka_context = kafka_context
+        self.kafka_context_ = kafka_context
 
         self.binary_stream = binary_stream
         self._gain = None
 
     # ----------------------------------------------------------------------
     def handle_accept(self) -> None:
         """Redirect the client connection."""
@@ -59,33 +59,41 @@
 
     # ----------------------------------------------------------------------
     def set_gain(self, gain) -> None:
         """"""
         self._gain = gain
 
     # ----------------------------------------------------------------------
+    @property
+    def kafka_context(self):
+        """"""
+        return self.kafka_context_()
+
+    # ----------------------------------------------------------------------
     def _handle_read(self) -> None:
         """Write the input streaming into the binary stream.
 
         There is a maximum of 3000 bytes that can read at once, so it is set to
         2970, a 33 multiple. But this not means that read this amount of data
-        on all events, the module WiFi will send on their consideration.
+        on all events, the module WiFi will send with their own consideration.
         """
 
-        self.kafka_context.update({'created': datetime.now().timestamp()})
+        kafka_context = self.kafka_context
+
+        # kafka_context.update({'created': datetime.now().timestamp()})
 
         if self._gain:
-            self.kafka_context.update({'gain': self._gain})
+            kafka_context.update({'gain': self._gain})
         else:
-            if self.kafka_context['daisy']:
-                self.kafka_context.update({'gain': [24] * 16})
+            if kafka_context['daisy']:
+                kafka_context.update({'gain': [24] * 16})
             else:
-                self.kafka_context.update({'gain': [24] * 8})
+                kafka_context.update({'gain': [24] * 8})
 
-        data = {'context': self.kafka_context,
+        data = {'context': kafka_context,
                 'data': self.handler.recv(33 * 90),
                 }
 
         self.binary_stream().stream(data)
 
     # ----------------------------------------------------------------------
     def _handle_error(self) -> None:
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/daemons/stream_eeg.py` & `openbci-stream-1.1.0/openbci_stream/daemons/stream_bin2eeg.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,103 +10,125 @@
 For examples and descriptions refers to documentation:
 `Data storage handler <../A1-raw_cleaning.ipynb>`_
 """
 
 import sys
 import pickle
 import struct
+from functools import cached_property
 import numpy as np
-from queue import Queue
-from threading import Thread
 from datetime import datetime
-import rawutil
+
+# import rawutil
+import logging
 
 from kafka import KafkaConsumer, KafkaProducer
-from typing import TypeVar, List, Dict, Tuple, Any
+from typing import TypeVar, Dict, Tuple, Any
+
+# from openbci_stream.utils import autokill_process
+# autokill_process(name='binary_2_eeg')
+
+DEBUG = '--debug' in sys.argv
 
-from openbci_stream.utils import autokill_process
-autokill_process(name='binary_2_eeg')
+if DEBUG:
+    logging.getLogger().setLevel(logging.DEBUG)
+    # logging.getLogger('kafka').setLevel(logging.WARNING)
 
-DEBUG = ('--debug' in sys.argv)
 
 KafkaStream = TypeVar('kafka-stream')
 
 
 ########################################################################
 class BinaryToEEG:
     """Kafka transformer with parallel implementation for processing binary raw
     data into EEG microvolts. This script requires the Kafka daemon running and
     enables an `auto-kill process <openbci_stream.utils.pid_admin.rst#module-openbci_stream.utils.pid_admin>`_
     """
 
-    BIN_HEADER = 0xa0
+    BIN_HEADER = 0xA0
+    LAST_AUX_SHAPE = 0
 
     # ----------------------------------------------------------------------
-    def __init__(self):
+    def __init__(self, board_id: str = ''):
         """"""
+        self.board_id = board_id
 
-        self.consumer_binary = KafkaConsumer(bootstrap_servers=['localhost:9092'],
-                                             value_deserializer=pickle.loads,
-                                             auto_offset_reset='latest',
-                                             )
-        self.consumer_binary.subscribe(['binary'])
-
-        self.producer_eeg = KafkaProducer(bootstrap_servers=['localhost:9092'],
-                                          compression_type='gzip',
-                                          value_serializer=pickle.dumps,
-                                          )
-
-        self.buffer = Queue(maxsize=33)
-
-        self._last_marker = 0
-        self.counter = 0
+        self.consumer_binary = KafkaConsumer(
+            bootstrap_servers=['localhost:9092'],
+            value_deserializer=pickle.loads,
+            auto_offset_reset='latest',
+        )
+        self.consumer_binary.subscribe([f'binary{self.board_id}'])
+
+        self.producer_eeg = KafkaProducer(
+            bootstrap_servers=['localhost:9092'],
+            compression_type='gzip',
+            value_serializer=pickle.dumps,
+        )
 
         self.remnant = b''
-        self.offset = [0] * 8
-        self._last_aux_shape = 0
+        self.offset = None, None
 
     # ----------------------------------------------------------------------
-    @property
+    @cached_property
     def scale_factor_eeg(self) -> float:
         """Vector with the correct factors for scale eeg data samples."""
         gain = 24
         # vref = 4.5  # for V
         vref = 4500000  # for uV
 
-        return vref / (gain * ((2 ** 23) - 1))
+        return vref / (gain * ((2**23) - 1))
 
     # ----------------------------------------------------------------------
     def consume(self) -> None:
         """Infinite loop for read Kafka stream."""
         while True:
             for record in self.consumer_binary:
-                if DEBUG:
-                    print(f"processing {len(record.value['data'])}")
+                logging.debug(f"processing {len(record.value['data'])}")
                 self.process(record)
 
     # ----------------------------------------------------------------------
     def process(self, record: KafkaStream) -> None:
         """Prepare the binary package for a successful unpack and stream.
 
         Parameters
         ----------
         record
             Kafka stream with binary data.
         """
-
         buffer = record.value
         context = buffer['context']
+        context['timestamp.binary.consume'] = datetime.now().timestamp()
 
+        # Deserialize data
+        logging.debug(
+            f'Aligning data: renmant({len(self.remnant)}), buffer({len(buffer["data"])})'
+        )
         data, self.remnant = self.align_data(self.remnant + buffer['data'])
+        logging.debug('aligned')
         if not data.shape[0]:
+            logging.debug('No data after alignement')
+            self.remnant = b''  # reset deserialicig
             return
+        logging.debug(
+            f'Deserilizing data: data({data.shape}), context({context})'
+        )
+        eeg_data, aux, ids = self.deserialize(data, context)
+        logging.debug(
+            f'deserialized eeg_data({eeg_data.shape}), aux({aux.shape})'
+        )
+        logging.debug(f'IDs: {ids}')
 
-        # Thread for unpack data
-        self.b = Thread(target=self.deserialize, args=(data, context))
-        self.b.start()
+        # Stream
+        context['samples'] = eeg_data.shape[1]
+        context['timestamp.eeg'] = datetime.now().timestamp()
+        context['sample_ids'] = ids
+
+        logging.debug(f'Streaming')
+        self.stream([eeg_data, aux], context)
 
     # ----------------------------------------------------------------------
     def align_data(self, binary: bytes) -> Tuple[np.ndarray, bytes]:
         """Align data following the headers and footers.
 
         Parameters
         ----------
@@ -116,30 +138,40 @@
         Returns
         -------
         data_aligned
             Numpy array of shape (`33, LENGTH`) with headers and footer aligned.
         remnant
             This bytes could be used for complete next binary input.
         """
-
+        logging.debug('Binary to np.ndarray')
         data = np.array(list(binary))
 
         # Search for the the first index with a `BIN_HEADER`
-        start = [np.median(np.roll(data, -i, axis=0)[::33]) ==
-                 self.BIN_HEADER for i in range(33)].index(True)
+        logging.debug('Looking for BIN_HEADER')
+        start = [
+            np.median(np.roll(data, -i, axis=0)[::33]) == self.BIN_HEADER
+            for i in range(33)
+        ].index(True)
 
         if (start == 0) and (data.shape[0] % 33 == 0):
+            logging.debug('No alignment necesary')
             data_aligned = data
             remnant = b''
         else:
             # Fix the offset to complete 33 bytes divisible array
+            logging.debug('Alingnig...')
             end = (data.shape[0] - start) % 33
+            logging.debug(
+                f'Alingnig data({len(data)}) at data({start}:-{end})'
+            )
             data_aligned = data[start:-end]
+            logging.debug('Saving remnant')
             remnant = binary[-end:]
 
+        logging.debug('Reshaping')
         data_aligned = data_aligned.reshape(-1, 33)
 
         return data_aligned, remnant
 
     # ----------------------------------------------------------------------
     def deserialize(self, data: np.ndarray, context: Dict[str, Any]) -> None:
         """From signed 24-bits integer to signed 32-bits integer.
@@ -149,151 +181,202 @@
         data
             Numpy array of shape (`33, LENGTH`)
         context
             Information from the acquisition side useful for deserializing and
             that will be packaged back in the stream.
         """
 
-        # From in index
-        pair = not data[:, 1][0] % 2
-
         # EGG
         eeg_data = data[:, 2:26]
-        eeg_data = getattr(self, f'deserialize_eeg_{context["connection"]}')(
-            eeg_data, pair, context)
+        ids = data[:, 1]
+        eeg_data, ids = getattr(
+            self, f'deserialize_eeg_{context["connection"]}'
+        )(eeg_data, ids, context)
 
         # Auxiliar
-        # stop_byte = data[0][-1]
         stop_byte = int((np.median(data[:, -1])))
-
         aux = self.deserialize_aux(stop_byte, data[:, 26:32], context)
-        self._last_aux_shape = aux.shape
+        self.LAST_AUX_SHAPE = aux.shape
 
         # Stream
-        channels = list(context['montage'].keys())
-        self.stream([eeg_data.T[channels], aux.T], eeg_data.shape[0], context)
+        channels = np.array(list(context['montage'].keys())) - 1
+
+        return eeg_data.T[channels], aux.T, ids
+        # self.stream([eeg_data.T[channels], aux.T], eeg_data.shape[0], context)
 
     # ----------------------------------------------------------------------
-    def deserialize_eeg_wifi(self, eeg: np.ndarray, pair: bool, context: Dict[str, Any]) -> np.ndarray:
+    def deserialize_eeg_wifi(
+        self, eeg: np.ndarray, ids: np.ndarray, context: Dict[str, Any]
+    ) -> np.ndarray:
         """From signed 24-bits integer to signed 32-bits integer by channels.
 
         The `Cyton data format <https://docs.openbci.com/docs/02Cyton/CytonDataFormat>`_
         says that only can send packages of 33 bits, when a Daisy board is
         attached these same packages will be sent at double speed in favor to
         keep the desired sample rate for 16 channels.
 
         Parameters
         ----------
         eeg
             Numpy array in signed 24-bits integer (`8, LENGTH`)
-        pair
-            True if the first data is from a pair ID.
+        ids
+            List of IDs for eeg data.
         context
             Information from the acquisition side useful for deserializing and
             that will be packaged back in the stream.
 
         Returns
         -------
         eeg_data
             EEG data in microvolts, signed 32-bits integer, (`CHANNELS, LENGTH`),
             if there is a Daisy board `CHANNELS` is 16, otherwise is 8.
         """
 
-        eeg_data = np.array([[rawutil.unpack('>u', bytes(ch))[0]
-                              for ch in row.reshape(-1, 3).tolist()] for row in eeg])
+        # eeg_data = np.array([[rawutil.unpack('>u', bytes(ch))[0]
+        # for ch in row.reshape(-1, 3).tolist()] for row in eeg])
+        eeg_data = np.array(
+            [
+                struct.unpack(
+                    '>i', (b'\0' if chunk[0] < 128 else b'\xff') + chunk
+                )
+                for chunk in [
+                    bytes(ch.tolist()) for ch in eeg.reshape(-1, 3)
+                ]
+            ]
+        ).reshape(-1, 8)
         eeg_data = eeg_data * self.scale_factor_eeg
 
         if context['daisy']:
 
-            # If offset, the pair index condition must change
-            if np.array(self.offset).any():
-                eeg_data = np.concatenate([[self.offset], eeg_data], axis=0)
-                pair = not pair
+            # # If offset, the pair index condition must change
+            if np.array(self.offset[0]).any():
+                eeg_data = np.concatenate(
+                    [[self.offset[0]], eeg_data], axis=0
+                )
+                ids = np.concatenate([[self.offset[1]], ids], axis=0)
+                # pair = not pair
+
+            if ids[0] != ids[1]:
+                eeg_data = np.delete(eeg_data, 0, axis=0)
+                ids = np.delete(ids, 0, axis=0)
 
             # if not pair dataset, create an offeset
             if eeg_data.shape[0] % 2:
-                self.offset = eeg_data[-1]
+                self.offset = eeg_data[-1], ids[-1]
                 eeg_data = np.delete(eeg_data, -1, axis=0)
-
-            if pair:
-                board = eeg_data[::2]
-                daisy = eeg_data[1::2]
+                ids = np.delete(ids, -1, axis=0)
             else:
-                daisy = eeg_data[::2]
-                board = eeg_data[1::2]
+                self.offset = None, None
 
-            return np.concatenate([board, daisy], axis=1)
+            return eeg_data.reshape(-1, 16), ids
 
-        return eeg_data
+        return eeg_data, ids
 
     # ----------------------------------------------------------------------
-    def deserialize_eeg_serial(self, eeg: np.ndarray, pair: bool, context: Dict[str, Any]) -> np.ndarray:
+    def deserialize_eeg_serial(
+        self, eeg: np.ndarray, ids: np.ndarray, context: Dict[str, Any]
+    ) -> np.ndarray:
         """From signed 24-bits integer to signed 32-bits integer by channels.
 
         The `Cyton data format <https://docs.openbci.com/docs/02Cyton/CytonDataFormat>`_
         says that only can send packages of 33 bits, over serial (RFduino) this
         limit is absolute, when a Daisy board is attached these same amount of
         packages will be sent, in this case, the data must be distributed and
         interpolated in order to complete the sample rate.
 
         Parameters
         ----------
         eeg
             Numpy array in signed 24-bits integer (`8, LENGTH`)
-        pair
-            True if the first data is from a pair ID.
+        ids
+            List of IDs for eeg data.
         context
             Information from the acquisition side useful for deserializing and
             that will be packaged back in the stream.
 
         Returns
         -------
         eeg_data
             EEG data in microvolts, signed 32-bits integer, (`CHANNELS, LENGTH`),
             if there is a Daisy board `CHANNELS` is 16, otherwise is 8.
         """
 
-        eeg_data = np.array([[rawutil.unpack('>u', bytes(ch))[0]
-                              for ch in row.reshape(-1, 3).tolist()] for row in eeg])
+        # eeg_data = np.array([[rawutil.unpack('>u', bytes(ch))[0]
+        # for ch in row.reshape(-1, 3).tolist()] for row in eeg])
+        eeg_data = np.array(
+            [
+                struct.unpack(
+                    '>i', (b'\0' if chunk[0] < 128 else b'\xff') + chunk
+                )
+                for chunk in [
+                    bytes(ch.tolist()) for ch in eeg.reshape(-1, 3)
+                ]
+            ]
+        ).reshape(-1, 8)
         eeg_data = eeg_data * self.scale_factor_eeg
 
         if context['daisy']:
 
-            # If offset, the pair index condition must change
-            if np.array(self.offset).any():
-                eeg_data = np.concatenate([[self.offset], eeg_data], axis=0)
-                pair = not pair
+            even = not ids[0] % 2
 
-            # if not pair dataset, create an offeset
+            # If offset, the even index condition must change
+            if np.array(self.offset[0]).any():
+                eeg_data = np.concatenate(
+                    [[self.offset[0]], eeg_data], axis=0
+                )
+                ids = np.concatenate([[self.offset[1]], ids], axis=0)
+                even = not even
+
+            # if not even dataset, create an offset
             if eeg_data.shape[0] % 2:
-                self.offset = eeg_data[-1]
+                self.offset = eeg_data[-1], ids[-1]
                 eeg_data = np.delete(eeg_data, -1, axis=0)
+                ids = np.delete(ids, -1, axis=0)
 
-            if pair:
+            # Data can start with a even or odd id
+            if even:
                 board = eeg_data[::2]
                 daisy = eeg_data[1::2]
             else:
                 daisy = eeg_data[::2]
                 board = eeg_data[1::2]
 
-            board = np.array([np.interp(np.arange(0, p.shape[0], 0.5), np.arange(p.shape[0]), p) for p in board.T]).T
-            daisy = np.array([np.interp(np.arange(0, p.shape[0], 0.5), np.arange(p.shape[0]), p) for p in daisy.T]).T
+            board = np.array(
+                [
+                    np.interp(
+                        np.arange(0, p.shape[0], 0.5),
+                        np.arange(p.shape[0]),
+                        p,
+                    )
+                    for p in board.T
+                ]
+            ).T
+            daisy = np.array(
+                [
+                    np.interp(
+                        np.arange(0, p.shape[0], 0.5),
+                        np.arange(p.shape[0]),
+                        p,
+                    )
+                    for p in daisy.T
+                ]
+            ).T
 
             eeg = np.concatenate([np.stack(board), np.stack(daisy)], axis=1)
 
         else:
             eeg = eeg_data
 
-        if len(context['montage'].keys()) > eeg.shape[1]:
-            return eeg
-
-        return eeg[:, list(context['montage'].keys())]
+        return eeg, ids
 
     # ----------------------------------------------------------------------
-    def deserialize_aux(self, stop_byte: int, aux: int, context: Dict[str, Any]) -> np.ndarray:
+    @classmethod
+    def deserialize_aux(
+        cls, stop_byte: int, aux: int, context: Dict[str, Any]
+    ) -> np.ndarray:
         """Determine the content of `AUX` bytes and format it.
 
         Auxialiar data could contain different kind of information: accelometer,
         user defined, time stamped and digital or analog inputs.
         The context of `AUX` bytes are determined by the stop byte.
 
         If `stop_byte` is `0xc0` the `AUX` bytes contain `Standard with accel`,
@@ -322,87 +405,121 @@
         -------
         list
             Correct data formated.
 
         """
 
         # Standard with accel
-        if stop_byte == 0xc0:
-            return 0.002 * \
-                np.array([struct.unpack('>hhh', a.astype('i1').tobytes())
-                          for a in aux]) / 16
+        if stop_byte == 0xC0:
+            return (
+                0.002
+                * np.array(
+                    [
+                        struct.unpack('>hhh', a.astype('i1').tobytes())
+                        for a in aux
+                    ]
+                )
+                / 16
+            )
 
         # Standard with raw aux
-        elif stop_byte == 0xc1:
+        elif stop_byte == 0xC1:
 
             if context['boardmode'] == 'analog':
-                # A7, A6, A5
-                # D13, D12, D11
-                return aux[:, 1::2]
+                if context['connection'] == 'wifi':
+                    # A7, A6
+                    # D13, D12
+
+                    # 2.36 ms ± 89.7 µs
+                    # return np.array([[rawutil.unpack('>H', bytes(ch))[0] for ch in row.reshape(-1, 2).tolist()][:2] for row in aux])
+
+                    # 185 µs ± 3.27 µs
+                    return np.array(
+                        [
+                            struct.unpack('>hhh', a.astype('i1').tobytes())[
+                                :2
+                            ]
+                            for a in aux
+                        ]
+                    )
+
+                else:
+                    # A7, A6, A5
+                    # D13, D12, D11
+                    # return np.array([[rawutil.unpack('>H', bytes(ch))[0] for ch in row.reshape(-1, 2).tolist()] for row in aux])
+                    return np.array(
+                        [
+                            struct.unpack('>hhh', a.astype('i1').tobytes())
+                            for a in aux
+                        ]
+                    )
 
             elif context['boardmode'] == 'digital':
-                # D11, D12, D13, D17, D18
-                return np.delete(aux, 4, axis=1)
+                if context['connection'] == 'wifi':
+                    # D11, D12, D17
+                    return aux[:, [0, 1, 3]]
+                else:
+                    # D11, D12, D13, D17, D18
+                    return aux[:, :-1]
 
             elif context['boardmode'] == 'marker':
                 # Some time for some reason, marker not always send back from
                 # OpenBCI, so this module implement a strategy to send a burst of
                 # markers but read back only one.
                 a = aux[:, 1]
                 a[a > ord('Z')] = 0
                 a[a < ord('A')] = 0
                 return a
 
         # User defined
-        elif stop_byte == 0xc2:
+        elif stop_byte == 0xC2:
             pass
 
         # Time stamped set with accel
-        elif stop_byte == 0xc3:
+        elif stop_byte == 0xC3:
             pass
 
         # Time stamped with accel
-        elif stop_byte == 0xc4:
+        elif stop_byte == 0xC4:
             pass
 
         # Time stamped set with raw auxcalculate_sample_rate
-        elif stop_byte == 0xc5:
+        elif stop_byte == 0xC5:
             pass
 
         # Time stamped with raw aux
-        elif stop_byte == 0xc6:
+        elif stop_byte == 0xC6:
             pass
 
-        return np.zeros(self._last_aux_shape)
+        return np.zeros(cls.LAST_AUX_SHAPE)
 
     # ----------------------------------------------------------------------
-    def stream(self, data, samples, context):
+    def stream(self, data, context):
         """Kafka produser.
 
         Stream data to network.
 
         Parameters
         ----------
         data : list
             The EEG data format.
-        samples : int
-            The number of samples in this package.
 
         """
-        context.update({'samples': samples, })
-
-        data_ = {'context': context,
-                 'data': data,
-                 # 'binary_created': self.created,
-                 # 'created': datetime.now().timestamp(),
-                 # 'samples': samples,
-                 }
 
-        self.producer_eeg.send('eeg', data_)
+        data_ = {
+            'context': context.copy(),
+            'data': data.copy(),
+        }
+
+        self.producer_eeg.send(f'eeg{self.board_id}', data_)
+        # future = self.producer_eeg.send(f'eeg{self.board_id}', data_)
+        # try:
+        # future.get()
+        # except Exception as e:
+        # logging.error(e)
 
-        if DEBUG:
-            print(f"streamed {samples} samples")
+        logging.debug(f"streamed ({data[0].shape}, {data[1].shape}) samples")
 
 
 if __name__ == '__main__':
-    tranformer = BinaryToEEG()
+    tranformer = BinaryToEEG(0)
     tranformer.consume()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/utils/openbci_cli.py` & `openbci-stream-1.1.0/openbci_stream/utils/openbci_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -140,17 +140,16 @@
                                      daisy=args.daisy,
                                      capture_stream=False,
                                      montage=None,
                                      streaming_package_size=args.streaming_package_size
                                      )
 
         elif args.endpoint == 'wifi':
-            interface = CytonWiFi(args.ip,
+            interface = CytonWiFi(args.ip, host=args.host,
                                   daisy=args.daisy,
-                                  host=args.host,
                                   capture_stream=False,
                                   montage=None,
                                   streaming_package_size=args.streaming_package_size
                                   )
 
         if args.command:
             for command in args.command:
@@ -167,42 +166,54 @@
                 writer = HDF5Writer(args.output)
                 header = {'sample_rate': args.streaming_package_size,
                           'datetime': datetime.now().timestamp(),
                           # 'montage': 'standard_1020',
                           # 'ch_names': 'Fp1,Fp2,F7,Fz,F8,C3,Cz,C4,T5,P3,Pz,P4,T6,O1,Oz,O2'.split(','),
                           }
                 writer.add_header(header)
+                print(
+                    f"Writing data in {Fore.LIGHTYELLOW_EX}{args.output}{Fore.RESET}.")
 
-            print(f"Writing data in {Fore.LIGHTYELLOW_EX}{Fore.RESET}\n"
-                  f"{Fore.LIGHTYELLOW_EX}Ctrl+C{Fore.RESET} for stop it.\n")
-            for message in stream:
+            print(f"{Fore.LIGHTYELLOW_EX}Ctrl+C{Fore.RESET} for stop it.")
+            for i, message in enumerate(stream):
 
                 if message.topic == 'eeg':
 
                     eeg, aux = message.value['data']
                     created = datetime.fromtimestamp(
-                        message.value['binary_created'])
+                        message.value['context']['timestamp.binary'])
                     since = (datetime.now() - created).total_seconds()
-                    count = message.value['samples']
+
+                    count = message.value['context']['samples']
                     channels = eeg.shape[0]
 
                     print(f"{Fore.YELLOW}[EEG]{Fore.RESET} {Fore.LIGHTYELLOW_EX}{created}{Fore.RESET}\t"
-                          f"{Fore.LIGHTRED_EX if since>1 else Fore.RESET}{since:0.4f}s ago{Fore.RESET}\t"
-                          f"{count} samples, {channels} channels")
+                          f"{Fore.LIGHTRED_EX if since>1 else Fore.RESET}{since*1000:0.2f} ms ago{Fore.RESET}\t"
+                          f"({channels},{count}) eeg", end='')
+
+                    if aux.size:
+                        print(f"\t({aux.shape[0]},{aux.shape[1]}) aux")
+                    else:
+                        print('')
 
                     if args.output:
                         writer.add_eeg(eeg.T, created.timestamp())
 
-                if message.topic == 'marker':
+                if message.topic in ['marker', 'annotation']:
+
+                    if message.topic == 'marker':
+                        head = 'MKR'
+                    elif message.topic == 'annotation':
+                        head = 'ANN'
 
                     marker = message.value
                     created = datetime.fromtimestamp(message.timestamp / 1000)
                     since = (datetime.now() - created).total_seconds()
-                    print(f"{Fore.YELLOW}[MKR]{Fore.RESET} {Fore.LIGHTYELLOW_EX}{created}{Fore.RESET}\t"
-                          f"{Fore.LIGHTRED_EX if since>1 else Fore.RESET}{since*1000:0.4f} ms ago{Fore.RESET}\t"
+                    print(f"{Fore.YELLOW}[{head}]{Fore.RESET} {Fore.LIGHTYELLOW_EX}{created}{Fore.RESET}\t"
+                          f"{Fore.LIGHTRED_EX if since>1 else Fore.RESET}{since*1000:0.2f} ms ago{Fore.RESET}\t"
                           f"{Fore.LIGHTBLUE_EX}{marker}{Fore.RESET}")
 
                     if args.output:
                         writer.add_marker(marker, created.timestamp())
 
             if args.output:
                 writer.close()
@@ -213,13 +224,12 @@
                                      # compression_type='gzip',
                                      value_serializer=pickle.dumps,
                                      )
 
         while True:
             marker = input(f'{Fore.YELLOW}>>> {Fore.RESET}')
             if mkr := marker.strip():
-                producer_eeg.send(
-                    'marker', {'timestamp': datetime.now().timestamp(), 'marker': mkr})
+                producer_eeg.send('marker', {'marker': mkr})
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/utils/pid_admin.py` & `openbci-stream-1.1.0/openbci_stream/utils/pid_admin.py`

 * *Files identical despite different names*

### Comparing `openbci-stream-1.0b1.post3/openbci_stream/utils/scan_wifi_modules.py` & `openbci-stream-1.1.0/openbci_stream/utils/scan_wifi_modules.py`

 * *Files identical despite different names*

### Comparing `openbci-stream-1.0b1.post3/openbci_stream.egg-info/SOURCES.txt` & `openbci-stream-1.1.0/openbci_stream.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 cmd/openbci_cli
 cmd/stream_access_point.sh
+cmd/stream_bin2eeg
 cmd/stream_configure_kafka.sh
+cmd/stream_configure_ntpd.sh
 cmd/stream_eeg
+cmd/stream_fake_binary
+cmd/stream_install_kafka.sh
 cmd/stream_rpyc
+cmd/stream_tlwr.sh
 openbci_stream/__init__.py
 openbci_stream/_version.txt
 openbci_stream.egg-info/PKG-INFO
 openbci_stream.egg-info/SOURCES.txt
 openbci_stream.egg-info/dependency_links.txt
 openbci_stream.egg-info/requires.txt
 openbci_stream.egg-info/top_level.txt
 openbci_stream/acquisition/__init__.py
 openbci_stream/acquisition/binary_stream.py
 openbci_stream/acquisition/consumer.py
 openbci_stream/acquisition/cyton.py
 openbci_stream/acquisition/cyton_base.py
 openbci_stream/acquisition/tcp_server.py
 openbci_stream/daemons/__init__.py
+openbci_stream/daemons/stream_bin2eeg.py
 openbci_stream/daemons/stream_eeg.py
+openbci_stream/daemons/stream_fake_binary.py
 openbci_stream/daemons/stream_rpyc.py
 openbci_stream/utils/__init__.py
+openbci_stream/utils/filters.py
 openbci_stream/utils/hdf5.py
 openbci_stream/utils/openbci_cli.py
 openbci_stream/utils/pid_admin.py
-openbci_stream/utils/scan_wifi_modules.py
+openbci_stream/utils/scan_wifi_modules.py
+openbci_stream/utils/viz.py
```

### Comparing `openbci-stream-1.0b1.post3/setup.py` & `openbci-stream-1.1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,56 +17,50 @@
     author='Yeison Cardona',
     author_email='yencardonaal@unal.edu.co',
     maintainer='Yeison Cardona',
     maintainer_email='yencardonaal@unal.edu.co',
 
     download_url='https://github.com/UN-GCPDS/openbci_stream',
 
-    install_requires=['pyserial',
-                      'scipy',
+    install_requires=['ntplib',
+                      'tables',
                       'numpy',
-                      'psutil',
                       'mne',
                       'requests',
                       'colorama',
-                      'rawutil',
-                      'plumbum',
-                      'pyedflib',
-
-                      'crc32c',
-                      'kafka-python',
+                      'scipy',
+                      'kafka_python',
                       'rpyc',
-                      'tables',
+                      'netifaces',
+                      'python3-nmap',
+                      'pyserial',
                       'systemd_service',
                       ],
 
-    extras_require={
-        'utils': ['nmap',
-                  'systemd_service',
-                  'netifaces',
-                  'python-nmap',
-                  ],
-    },
-
     scripts=[
        "cmd/openbci_cli",
        "cmd/stream_rpyc",
        "cmd/stream_eeg",
+       "cmd/stream_bin2eeg",
+       "cmd/stream_fake_binary",
        "cmd/stream_configure_kafka.sh",
        "cmd/stream_access_point.sh",
+       "cmd/stream_configure_ntpd.sh",
+       "cmd/stream_install_kafka.sh",
+       "cmd/stream_tlwr.sh",
     ],
 
     include_package_data=True,
     license='BSD-2-Clause',
     description="High level Python module for EEG/EMG/ECG acquisition and distributed streaming for OpenBCI Cyton board.",
 
     long_description=README,
     long_description_content_type='text/markdown',
 
-    python_requires='>=3.8',
+    python_requires='>=3.7',
 
     classifiers=[
        'Development Status :: 4 - Beta',
        'Intended Audience :: Developers',
        'Intended Audience :: Education',
        'Intended Audience :: Healthcare Industry',
        'Intended Audience :: Science/Research',
```

