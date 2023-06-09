# Comparing `tmp/toori-server-1.1.8.tar.gz` & `tmp/toori-server-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toori-server-1.1.8.tar", last modified: Fri Jun  9 02:30:11 2023, max compression
+gzip compressed data, was "dist/toori-server-1.1.9.tar", last modified: Fri Jun  9 13:31:02 2023, max compression
```

## Comparing `toori-server-1.1.8.tar` & `toori-server-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:30:11.000000 toori-server-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 02:30:11.000000 toori-server-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-09 02:29:55.000000 toori-server-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:30:11.000000 toori-server-1.1.8/iro/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 02:29:55.000000 toori-server-1.1.8/iro/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-09 02:29:55.000000 toori-server-1.1.8/iro/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-06-09 02:29:55.000000 toori-server-1.1.8/iro/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 02:29:55.000000 toori-server-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 02:30:11.000000 toori-server-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-09 02:29:55.000000 toori-server-1.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 02:30:11.000000 toori-server-1.1.8/toori_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:31:01.000000 toori-server-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 13:31:01.000000 toori-server-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-09 13:30:45.000000 toori-server-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:31:01.000000 toori-server-1.1.9/iro/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-09 13:30:45.000000 toori-server-1.1.9/iro/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-09 13:30:45.000000 toori-server-1.1.9/iro/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-09 13:30:45.000000 toori-server-1.1.9/iro/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 13:30:45.000000 toori-server-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:31:01.000000 toori-server-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-09 13:30:45.000000 toori-server-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-09 13:31:01.000000 toori-server-1.1.9/toori_server.egg-info/top_level.txt
```

### Comparing `toori-server-1.1.8/PKG-INFO` & `toori-server-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.8
+Version: 1.1.9
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
         [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
         [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
```

### Comparing `toori-server-1.1.8/README.md` & `toori-server-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `toori-server-1.1.8/iro/main.py` & `toori-server-1.1.9/iro/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import struct
 import socket
 from collections import deque
 import socketio
 from scapy.all import (
     AsyncSniffer,
+    get_if_list,
     get_if_addr,
     conf,
     IP,
     TCP,
     UDP,
 )
 import asyncio
@@ -191,23 +192,28 @@
 
             pkt.dport, sid = rnat_value
 
         await sio.emit("in", bytes(pkt), to=sid)
 
 
 def start(port, certs_dir=None):
+    target_ifaces = [conf.iface]
+    if "lo" in get_if_list():
+        target_ifaces.append("lo")
 
     AsyncSniffer(
-        filter=f"src host not {LOCAL_IP} and ip and dst port not {port} and dst port not 22",
+        # Only capture return traffic belonging to the client (likely not dst port 1-1024)
+        filter=f"ip && dst host {LOCAL_IP} && dst port not {port} && dst port not 22",
         store=False,
         prn=lambda pkt: handle_inbound_packet(pkt),
+        iface=target_ifaces,
     ).start()
 
     app.add_task(background_sender)
     app.run(
         "::",
         port=port,
         debug=False,
         access_log=False,
         single_process=True,
         ssl=certs_dir,
-    )
+    )
```

### Comparing `toori-server-1.1.8/setup.py` & `toori-server-1.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 import pathlib
 import subprocess
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `toori-server-1.1.8/toori_server.egg-info/PKG-INFO` & `toori-server-1.1.9/toori_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.8
+Version: 1.1.9
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
         [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
         [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
```

