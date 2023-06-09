# Comparing `tmp/toori-server-1.1.7.tar.gz` & `tmp/toori-server-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toori-server-1.1.7.tar", last modified: Thu Jun  8 09:13:51 2023, max compression
+gzip compressed data, was "dist/toori-server-1.1.8.tar", last modified: Fri Jun  9 02:30:11 2023, max compression
```

## Comparing `toori-server-1.1.7.tar` & `toori-server-1.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:13:51.000000 toori-server-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 09:13:51.000000 toori-server-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-08 09:13:38.000000 toori-server-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:13:51.000000 toori-server-1.1.7/iro/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 09:13:38.000000 toori-server-1.1.7/iro/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 09:13:38.000000 toori-server-1.1.7/iro/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-06-08 09:13:38.000000 toori-server-1.1.7/iro/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 09:13:38.000000 toori-server-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:13:51.000000 toori-server-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 09:13:38.000000 toori-server-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 09:13:51.000000 toori-server-1.1.7/toori_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:30:11.000000 toori-server-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 02:30:11.000000 toori-server-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-09 02:29:55.000000 toori-server-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:30:11.000000 toori-server-1.1.8/iro/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 02:29:55.000000 toori-server-1.1.8/iro/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-09 02:29:55.000000 toori-server-1.1.8/iro/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-09 02:29:55.000000 toori-server-1.1.8/iro/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 02:29:55.000000 toori-server-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 02:30:11.000000 toori-server-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-09 02:29:55.000000 toori-server-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/top_level.txt
```

### Comparing `toori-server-1.1.7/PKG-INFO` & `toori-server-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.7
+Version: 1.1.8
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
         [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
         [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
```

### Comparing `toori-server-1.1.7/README.md` & `toori-server-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `toori-server-1.1.7/iro/main.py` & `toori-server-1.1.8/iro/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,34 +9,19 @@
     IP,
     TCP,
     UDP,
 )
 import asyncio
 from sanic import Sanic
 
-import urllib.request
-import netifaces as ni
-
 from engineio.payload import Payload
 
 Payload.max_decode_packets = 2500000
 
-PUBLIC_IP = urllib.request.urlopen('https://checkip.amazonaws.com').read().decode('utf8').strip()
 LOCAL_IP = get_if_addr(conf.iface)
-SSH_IP = LOCAL_IP
-
-if PUBLIC_IP == LOCAL_IP:
-    default_interface = ni.gateways()["default"][ni.AF_INET][1]
-    addrs = {d['addr'] for d in ni.ifaddresses(default_interface)[ni.AF_INET]}
-    addrs.remove(PUBLIC_IP)
-
-    if addrs:
-        # Obtain alternative local address that can be used for ssh
-        SSH_IP = addrs.pop()
-
 conf.layers.filter([IP, TCP, UDP])
 
 app = Sanic("Iro")
 app.config["CORS_SUPPORTS_CREDENTIALS"] = True
 
 sio = socketio.AsyncServer(async_mode="sanic", cors_allowed_origins=[])
 sio.attach(app)
@@ -85,17 +70,14 @@
         pkt.src = virtual_ip_map.get((pkt.src, sid))
         pkt.dst, target_sid = vtarget
         await sio.emit("in", bytes(pkt), to=target_sid)
         return
 
     if pkt.haslayer(TCP) or pkt.haslayer(UDP):
 
-        if pkt.dst == PUBLIC_IP:
-            pkt.dst = SSH_IP
-
         # Check if existing mapping exists
         # For O(1) lookup for existing connections instead of using the loop below
         fake_sport = forward_nat.get((pkt.sport, sid, pkt.dst, pkt.dport))
 
         if fake_sport is None:
             decrement = False
             # New first-time connection
```

### Comparing `toori-server-1.1.7/setup.py` & `toori-server-1.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 import pathlib
 import subprocess
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `toori-server-1.1.7/toori_server.egg-info/PKG-INFO` & `toori-server-1.1.8/toori_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.7
+Version: 1.1.8
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
         [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
         [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
```

