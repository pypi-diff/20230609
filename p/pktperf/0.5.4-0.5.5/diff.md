# Comparing `tmp/pktperf-0.5.4.tar.gz` & `tmp/pktperf-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pktperf-0.5.4.tar", last modified: Mon Jun  5 14:32:18 2023, max compression
+gzip compressed data, was "pktperf-0.5.5.tar", last modified: Fri Jun  9 15:16:41 2023, max compression
```

## Comparing `pktperf-0.5.4.tar` & `pktperf-0.5.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:18.981997 pktperf-0.5.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:18.977997 pktperf-0.5.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:18.977997 pktperf-0.5.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-05 14:32:08.000000 pktperf-0.5.4/.github/workflows/pylint.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-05 14:32:08.000000 pktperf-0.5.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-05 14:32:08.000000 pktperf-0.5.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-05 14:32:08.000000 pktperf-0.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-05 14:32:08.000000 pktperf-0.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-05 14:32:18.981997 pktperf-0.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-05 14:32:08.000000 pktperf-0.5.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 14:32:08.000000 pktperf-0.5.4/example.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:18.981997 pktperf-0.5.4/pktperf/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/ethtoolsar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:18.981997 pktperf-0.5.4/pktperf/module/
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/module/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/module/common.mk
--rw-r--r--   0 runner    (1001) docker     (123)   143867 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/module/pktgen_5.4.c
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/pktgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/pktperf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-05 14:32:08.000000 pktperf-0.5.4/pktperf/pktsar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 14:32:18.981997 pktperf-0.5.4/pktperf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-05 14:32:18.000000 pktperf-0.5.4/pktperf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-05 14:32:18.000000 pktperf-0.5.4/pktperf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 14:32:18.000000 pktperf-0.5.4/pktperf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 14:32:18.000000 pktperf-0.5.4/pktperf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-05 14:32:18.000000 pktperf-0.5.4/pktperf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-05 14:32:18.000000 pktperf-0.5.4/pktperf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-05 14:32:08.000000 pktperf-0.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 14:32:18.981997 pktperf-0.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-05 14:32:08.000000 pktperf-0.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.189414 pktperf-0.5.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-06-09 15:16:30.000000 pktperf-0.5.5/.github/workflows/pylint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-09 15:16:30.000000 pktperf-0.5.5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-09 15:16:30.000000 pktperf-0.5.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-09 15:16:30.000000 pktperf-0.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-09 15:16:30.000000 pktperf-0.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-09 15:16:41.193414 pktperf-0.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-09 15:16:30.000000 pktperf-0.5.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-09 15:16:30.000000 pktperf-0.5.5/example.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/pktperf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12944 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/ethtoolsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/pktperf/module/
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/module/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/module/common.mk
+-rw-r--r--   0 runner    (1001) docker     (123)   144669 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/module/pktgen_5.4.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26196 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/pktgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/pktperf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-09 15:16:30.000000 pktperf-0.5.5/pktperf/pktsar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 15:16:41.193414 pktperf-0.5.5/pktperf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 15:16:41.000000 pktperf-0.5.5/pktperf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-09 15:16:30.000000 pktperf-0.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 15:16:41.193414 pktperf-0.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-09 15:16:30.000000 pktperf-0.5.5/setup.py
```

### Comparing `pktperf-0.5.4/.github/workflows/pylint.yml` & `pktperf-0.5.5/.github/workflows/pylint.yml`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.4/.github/workflows/python-publish.yml` & `pktperf-0.5.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.4/LICENSE` & `pktperf-0.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.4/PKG-INFO` & `pktperf-0.5.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pktperf
-Version: 0.5.4
+Version: 0.5.5
 Summary: pktgen scripts tool
 Author-email: junka <wan.junjie@foxmail.com>
 Project-URL: Homepage, https://github.com/junka/pktperf
 Project-URL: Bug Tracker, https://github.com/junka/pktperf/issues
 Platform: manylinux2014_x86_64
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -66,18 +66,18 @@
 packets sent.
 
 ```
 
 
 micro burst test case:
 
-```microburst duration_wait,duration_send```
+```microburst duration_poll,duration_idle```
 
 ```
-microbust 200,100
+microburst 200,100
 
 pktgen will be sending 200ms and then keep 100ms idle, loop follow the pattern
 ```
 
 
 During pktgen running, all stats will be display with 1 sec interval
 ```
```

### Comparing `pktperf-0.5.4/README.md` & `pktperf-0.5.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,18 +50,18 @@
 packets sent.
 
 ```
 
 
 micro burst test case:
 
-```microburst duration_wait,duration_send```
+```microburst duration_poll,duration_idle```
 
 ```
-microbust 200,100
+microburst 200,100
 
 pktgen will be sending 200ms and then keep 100ms idle, loop follow the pattern
 ```
 
 
 During pktgen running, all stats will be display with 1 sec interval
 ```
```

### Comparing `pktperf-0.5.4/pktperf/ethtoolsar.py` & `pktperf-0.5.5/pktperf/ethtoolsar.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,55 +6,73 @@
 import re
 import time
 import datetime
 import signal
 from decimal import Decimal
 from os.path import exists
 from os import listdir
-import copy
 import argparse
 import netifaces
 
 
 stop = False
 
 
 def check_output(args, stderr=None):
-    '''Run a command and capture its output'''
-    p = subprocess.Popen(args, stdout=subprocess.PIPE, shell=False,
-                            stderr=stderr)
+    """Run a command and capture its output"""
+    p = subprocess.Popen(args, stdout=subprocess.PIPE, shell=False, stderr=stderr)
     out, err = p.communicate()
     return p.returncode, out, err
 
-def print_format_header(tm):
-    print("% s% 20s% 16s% 16s% 16s% 16s% 16s % 16s" %
-          (tm, "IFACE", "rxpck/s", "txpck/s", "rxkB/s", "txkB/s", "txdrop/s", "rxdrop/s"))
 
-def print_format_string(tm, port_name, diff_rxpkts, diff_txpkts,
-                        diff_rxbytes, diff_txbytes, diff_txdrops, diff_rxdrops):
+def print_format_header(tm):
+    print(
+        "% s% 20s% 16s% 16s% 16s% 16s% 16s % 16s"
+        % (
+            tm,
+            "IFACE",
+            "rxpck/s",
+            "txpck/s",
+            "rxkB/s",
+            "txkB/s",
+            "txdrop/s",
+            "rxdrop/s",
+        )
+    )
+
+
+def print_format_string(
+    tm,
+    port_name,
+    diff_rxpkts,
+    diff_txpkts,
+    diff_rxbytes,
+    diff_txbytes,
+    diff_txdrops,
+    diff_rxdrops,
+):
     rxpps = Decimal(diff_rxpkts).quantize(Decimal("0.00"))
     txpps = Decimal(diff_txpkts).quantize(Decimal("0.00"))
-    rxbps = Decimal(diff_rxbytes /
-                    (1024)).quantize(Decimal("0.00"))
-    txbps = Decimal(diff_txbytes /
-                    (1024)).quantize(Decimal("0.00"))
-    txdrop = Decimal(diff_txdrops /
-                    (1024)).quantize(Decimal("0.00"))
-    rxdrop = Decimal(diff_rxdrops /
-                    (1024)).quantize(Decimal("0.00"))
-    print("%s% 20s% 16s% 16s% 16s% 16s% 16s % 16s" %
-          (tm, port_name, rxpps, txpps, rxbps, txbps, txdrop, rxdrop))
+    rxbps = Decimal(diff_rxbytes / (1024)).quantize(Decimal("0.00"))
+    txbps = Decimal(diff_txbytes / (1024)).quantize(Decimal("0.00"))
+    txdrop = Decimal(diff_txdrops / (1024)).quantize(Decimal("0.00"))
+    rxdrop = Decimal(diff_rxdrops / (1024)).quantize(Decimal("0.00"))
+    print(
+        "%s% 20s% 16s% 16s% 16s% 16s% 16s % 16s"
+        % (tm, port_name, rxpps, txpps, rxbps, txbps, txdrop, rxdrop)
+    )
 
 
 class PhyStats:
     """
     Implements ethtool -s DEV commands
 
     @ \todo dynamic port add
     """
+
     def __init__(self, name):
         self._name = name
         self._rx_pkts = 0
         self._tx_pkts = 0
         self._rx_pkts_phy = 0
         self._tx_pkts_phy = 0
         self._rx_bytes = 0
@@ -104,15 +122,15 @@
         self._interval = interval
 
     def _init_stats(self):
         ret, stats_info, err = check_output(["ethtool", "-S", self._name])
         if ret != 0:
             return
         if err is not None:
-            drv = re.search(r'no stats available', err.decode())
+            drv = re.search(r"no stats available", err.decode())
             if drv is not None:
                 return
         self._type = 1
         self.update_stats()
         self._init_rx_pkts = self._rx_pkts
         self._init_tx_pkts = self._tx_pkts
         self._init_rx_pkts_phy = self._rx_pkts_phy
@@ -136,33 +154,33 @@
         self._delta_rx_discard_phy = 0
         self._delta_tx_discard_phy = 0
         self._delta_tx_errors_phy = 0
         self._delta_rx_oob = 0
         self._delta_rx_oversize = 0
 
     def update_stats(self):
-        '''
+        """
         https://enterprise-support.nvidia.com/s/article/understanding-mlx5-ethtool-counters
 
-        '''
+        """
         self._times += 1
         _, statsresult, err = check_output(["ethtool", "-S", self._name])
         stats_info = statsresult.decode()
-        rxdrop = re.search(r'rx_discards_phy: (\d+)', stats_info)
-        txdrop = re.search(r'tx_discards_phy: (\d+)', stats_info)
-        rxpkts = re.search(r'rx_packets: (\d+)', stats_info)
-        rxpkts_phy = re.search(r'rx_packets_phy: (\d+)', stats_info)
-        txpkts = re.search(r'tx_packets: (\d+)', stats_info)
-        txpkts_phy = re.search(r'tx_packets_phy: (\d+)', stats_info)
-        rxbytes = re.search(r'rx_bytes: (\d+)', stats_info)
-        rxbytes_phy = re.search(r'rx_bytes_phy: (\d+)', stats_info)
-        txbytes = re.search(r'tx_bytes: (\d+)', stats_info)
-        txbytes_phy = re.search(r'tx_bytes_phy: (\d+)', stats_info)
-        rxoob = re.search(r'rx_out_of_buffer: (\d+)', stats_info)
-        rxoversize = re.search(r'rx_oversize_pkts_phy: (\d+)', stats_info)
+        rxdrop = re.search(r"rx_discards_phy: (\d+)", stats_info)
+        txdrop = re.search(r"tx_discards_phy: (\d+)", stats_info)
+        rxpkts = re.search(r"rx_packets: (\d+)", stats_info)
+        rxpkts_phy = re.search(r"rx_packets_phy: (\d+)", stats_info)
+        txpkts = re.search(r"tx_packets: (\d+)", stats_info)
+        txpkts_phy = re.search(r"tx_packets_phy: (\d+)", stats_info)
+        rxbytes = re.search(r"rx_bytes: (\d+)", stats_info)
+        rxbytes_phy = re.search(r"rx_bytes_phy: (\d+)", stats_info)
+        txbytes = re.search(r"tx_bytes: (\d+)", stats_info)
+        txbytes_phy = re.search(r"tx_bytes_phy: (\d+)", stats_info)
+        rxoob = re.search(r"rx_out_of_buffer: (\d+)", stats_info)
+        rxoversize = re.search(r"rx_oversize_pkts_phy: (\d+)", stats_info)
         if rxdrop is not None:
             self._delta_rx_discard_phy = int(rxdrop.group(1)) - self._rx_discard_phy
             self._rx_discard_phy = int(rxdrop.group(1))
         if txdrop is not None:
             self._delta_tx_discard_phy = int(txdrop.group(1)) - self._tx_discard_phy
             self._tx_discard_phy = int(txdrop.group(1))
         if rxpkts is not None:
@@ -194,55 +212,93 @@
             self._rx_oob = int(rxoob.group(1))
         if rxoversize is not None:
             self._delta_rx_oversize = int(rxoversize.group(1)) - self._rx_oversize
             self._rx_oversize = int(rxoversize.group(1))
 
     def print_calc_stats(self, ts):
         port_name = self._name
-        diff_rxpkts = (self._delta_rx_pkts_phy ) / (self._interval)
-        diff_txpkts = (self._delta_tx_pkts_phy ) / (self._interval)
+        diff_rxpkts = (self._delta_rx_pkts_phy) / (self._interval)
+        diff_txpkts = (self._delta_tx_pkts_phy) / (self._interval)
         diff_rxbytes = (self._delta_rx_bytes_phy) / (self._interval)
-        diff_txbytes = (self._delta_tx_bytes_phy ) / (self._interval)
-        diff_txdrops = (self._delta_tx_discard_phy + self._delta_tx_errors_phy)
-        diff_rxdrops = (self._delta_rx_discard_phy + self._delta_rx_oob) / (self._interval)
-        print_format_string(ts, port_name, diff_rxpkts, diff_txpkts, diff_rxbytes,
-                            diff_txbytes, diff_txdrops, diff_rxdrops)
+        diff_txbytes = (self._delta_tx_bytes_phy) / (self._interval)
+        diff_txdrops = self._delta_tx_discard_phy + self._delta_tx_errors_phy
+        diff_rxdrops = (self._delta_rx_discard_phy + self._delta_rx_oob) / (
+            self._interval
+        )
+        print_format_string(
+            ts,
+            port_name,
+            diff_rxpkts,
+            diff_txpkts,
+            diff_rxbytes,
+            diff_txbytes,
+            diff_txdrops,
+            diff_rxdrops,
+        )
 
     def print_average_stats(self):
         port_name = self._name
-        diff_rxpkts = (self._rx_pkts_phy - self._init_rx_pkts_phy) / (self._interval * (self._times - 1))
-        diff_txpkts = (self._tx_pkts_phy - self._init_tx_pkts_phy) / (self._interval * (self._times - 1))
-        diff_rxbytes = (self._rx_bytes_phy - self._init_rx_bytes_phy) / (self._interval * (self._times - 1))
-        diff_txbytes = (self._tx_bytes_phy- self._init_tx_bytes_phy ) / (self._interval * (self._times - 1))
-        diff_txdrops = (self._tx_discard_phy + self._tx_errors_phy - self._init_tx_discard_phy - self._init_tx_errors_phy) / (self._interval * (self._times - 1))
-        diff_rxdrops = (self._rx_discard_phy + self._rx_oob + self._rx_oversize - self._init_rx_discard_phy - self._init_rx_oob - self._init_rx_oversize) / (self._interval * (self._times - 1))
-        print_format_string("Average:", port_name, diff_rxpkts, diff_txpkts, diff_rxbytes,
-                            diff_txbytes, diff_txdrops, diff_rxdrops)
+        diff_rxpkts = (self._rx_pkts_phy - self._init_rx_pkts_phy) / (
+            self._interval * (self._times - 1)
+        )
+        diff_txpkts = (self._tx_pkts_phy - self._init_tx_pkts_phy) / (
+            self._interval * (self._times - 1)
+        )
+        diff_rxbytes = (self._rx_bytes_phy - self._init_rx_bytes_phy) / (
+            self._interval * (self._times - 1)
+        )
+        diff_txbytes = (self._tx_bytes_phy - self._init_tx_bytes_phy) / (
+            self._interval * (self._times - 1)
+        )
+        diff_txdrops = (
+            self._tx_discard_phy
+            + self._tx_errors_phy
+            - self._init_tx_discard_phy
+            - self._init_tx_errors_phy
+        ) / (self._interval * (self._times - 1))
+        diff_rxdrops = (
+            self._rx_discard_phy
+            + self._rx_oob
+            + self._rx_oversize
+            - self._init_rx_discard_phy
+            - self._init_rx_oob
+            - self._init_rx_oversize
+        ) / (self._interval * (self._times - 1))
+        print_format_string(
+            "Average:",
+            port_name,
+            diff_rxpkts,
+            diff_txpkts,
+            diff_rxbytes,
+            diff_txbytes,
+            diff_txdrops,
+            diff_rxdrops,
+        )
 
 
 class Bond:
     """
     read slaves for a bond from /proc/sys/class/net/xxx/bonding/slaves
     @ \todo dynamic port add
     """
+
     def __init__(self, name):
         self._times = 1
         self._name = name
         self._phys = []
         self._initphys = []
         slavespath = "/sys/class/net/%s/bonding/slaves" % name
         if exists(slavespath):
             try:
-                f = open(slavespath, "r")
-            except:
+                with open(slavespath, "r", encoding="utf-8") as f:
+                    self.slaves = f.read().split()
+            except IOError:
                 sys.exit("Error: unable to read slaves for %s", name)
         else:
             sys.exit("Error: unable to find slaves file for %s", name)
-        self.slaves = f.read().split()
-        f.close()
         print("%s has slaves %s" % (name, self.slaves))
         for i in self.slaves:
             phy = PhyStats(i)
             if phy._type == 0:
                 sys.exit("Error: slaves are not phy ports")
             self._phys.append(phy)
 
@@ -259,21 +315,22 @@
         for m in self._phys:
             m.print_calc_stats(ts)
 
     def print_average_stats(self):
         for m in self._phys:
             m.print_average_stats()
 
+
 def signal_handler():
     global stop
     stop = True
 
 
 def bonding_list(names) -> (list, list):
-    boding_path = '/proc/net/bonding'
+    boding_path = "/proc/net/bonding"
     bonds = []
     unbondphys = []
     if exists(boding_path):
         bondnames = listdir(boding_path)
         for i in bondnames:
             if names is None or i in names:
                 bonds.append(Bond(i))
@@ -290,15 +347,15 @@
                 unbondphys.append(p)
     return bonds, unbondphys
 
 
 def main():
     global stop
     parser = argparse.ArgumentParser(description="")
-    parser.add_argument("--name", "-n", type=str, action='append')
+    parser.add_argument("--name", "-n", type=str, action="append")
     parser.add_argument("--interval", "-i", type=float, default=1)
     args = parser.parse_args()
     if args.name is not None and len(args.name) > 1:
         for n in args.name:
             if n not in netifaces.interfaces():
                 print("%s is not a valid interface name" % n)
                 exit()
@@ -321,9 +378,10 @@
         for i in alldev:
             i.update_stats()
             i.print_calc_stats(ts)
         print("")
     for i in alldev:
         i.print_average_stats()
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `pktperf-0.5.4/pktperf/module/Makefile` & `pktperf-0.5.5/pktperf/module/Makefile`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.4/pktperf/module/common.mk` & `pktperf-0.5.5/pktperf/module/common.mk`

 * *Files identical despite different names*

### Comparing `pktperf-0.5.4/pktperf/module/pktgen_5.4.c` & `pktperf-0.5.5/pktperf/module/pktgen_5.4.c`

 * *Files 1% similar despite different names*

```diff
@@ -153,14 +153,15 @@
 #include <linux/kthread.h>
 #include <linux/prefetch.h>
 #include <linux/mmzone.h>
 #include <net/net_namespace.h>
 #include <net/checksum.h>
 #include <net/ipv6.h>
 #include <net/udp.h>
+#include <net/tcp.h>
 #include <net/ip6_checksum.h>
 #include <net/addrconf.h>
 #ifdef CONFIG_XFRM
 #include <net/xfrm.h>
 #endif
 #include <net/netns/generic.h>
 #include <asm/byteorder.h>
@@ -535,14 +536,27 @@
 struct pktgen_net {
     struct net        *net;
     struct proc_dir_entry    *proc_dir;
     struct list_head    pktgen_threads;
     bool            pktgen_exiting;
 };
 
+struct tcp_state {
+    __u64 retransmits;
+    __u32 flow_state;
+    __u32 seq;     /* our last sent seqno */
+    __u32 ack_seq; /* last seqno that got acked */
+    __u32 rcv_seq; /* receiver's seqno (our ACK seq) */
+
+    __u32 highest_seq;
+    __u16 window;
+    __u8 wscale;
+};
+
+
 struct pktgen_thread {
     struct mutex if_lock;        /* for list of devices */
     struct list_head if_list;    /* All device here */
     struct list_head th_list;
     struct task_struct *tsk;
     char result[512];
 
@@ -551,14 +565,15 @@
 
     u32 control;
     int cpu;
 
     wait_queue_head_t queue;
     struct completion start_done;
     struct pktgen_net *net;
+    struct tcp_state tcp_state;
 };
 
 #define REMOVE 1
 #define FIND   0
 
 static const char version[] =
     "Packet Generator for packet performance testing. "
@@ -3430,14 +3445,30 @@
         udph->source = htons(pkt_dev->cur_udp_src);
         udph->dest = htons(pkt_dev->cur_udp_dst);
     }    
     udph->len = htons(datalen + 8);    /* DATA + udphdr */
     udph->check = 0;
 }
 
+static void fill_tcp_syn(struct sk_buff *skb, struct tcphdr *tcph,
+                         struct pktgen_dev *pkt_dev, int datalen)
+{
+    tcph->source = htons(pkt_dev->cur_udp_src);
+    tcph->dest = htons(pkt_dev->cur_udp_dst);
+    // tcph->len = htons(datalen + 8); /* DATA + udphdr */
+    tcph->check = 0;
+    tcph->seq = 0;
+    tcph->ack_seq = 0;
+    tcph->window = htons(0x100);
+    tcph->urg_ptr = 0;
+    tcph->syn = 1;
+    tcph->doff = 5;
+    tcph->res1 = 0;
+}
+
 static void fill_ipv6_layer(struct ipv6hdr *iph, struct pktgen_dev *pkt_dev,
                      int datalen, bool tun)
 {
 
     *(__be32 *) iph = htonl(0x60000000);    /* Version + flow */
 
     if (pkt_dev->traffic_class) {
```

### Comparing `pktperf-0.5.4/pktperf/pktgen.py` & `pktperf-0.5.5/pktperf/pktgen.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,46 @@
 """
 classes provide functions for pktgen operation
 """
 import sys
 import re
 import os
 import math
+import platform
 import ipaddress
 import subprocess
 import configparser
 from .pktsar import PktSar
 
 
 def open_write_error(filename, flag, mode="r+"):
     """open and write a flag to file"""
     try:
-        with open(filename, mode, encoding='utf-8') as fp_dev:
+        with open(filename, mode, encoding="utf-8") as fp_dev:
             fp_dev.write("%s\n" % flag)
-    except IOError:
+    except IOError as exc:
         print("Error: Cannot open %s" % (filename))
-        raise Exception("Error writing flag %s", flag)
-        sys.exit(1)
+        raise IOError("Error writing flag %s" % flag) from exc
 
 
 def modinfo_check() -> str:
-    """ check module version """
-    p = subprocess.run(['modinfo', 'pktgen'], stdout=subprocess.PIPE, check=True)
+    """check module version"""
+    n = platform.uname()
+    depfile = "/lib/modules/%s/modules.dep" % n.release
+    try:
+        with open(depfile, "r", encoding="utf-8") as fp_dep:
+            fp_dep.readlines()
+    except IOError as exc:
+        print("Fail to open modules.dep, maybe you are not root privellge")
+        raise IOError("Error open modules.dep") from exc
+    p = subprocess.run(["modinfo", "pktgen"], stdout=subprocess.PIPE, check=True)
     if p.returncode != 0:
         return ""
-    ret = p.stdout.decode('utf-8')
-    ver = re.search(r'version:[\t\ ]+([\d\.]+)', ret)
+    ret = p.stdout.decode("utf-8")
+    ver = re.search(r"version:[\t\ ]+([\d\.]+)", ret)
     if ver is not None:
         return ver.group(1)
     return ""
 
 
 class Pktgen:
     """Pktgen class
@@ -81,15 +89,15 @@
         ver = modinfo_check()
         if ver == "":
             print("pktgen is not enabled in kernel")
             sys.exit()
         mod = "/proc/net/pktgen"
         is_exists = os.path.exists(mod)
         if is_exists is False:
-            print("No pktgen module\nPlease do \'modprobe pktgen\'")
+            print("No pktgen module\nPlease do 'modprobe pktgen'")
             sys.exit(0)
         self.pgdev = args.interface
         self.pkt_size = int(args.size)
         self.dst_mac = args.mac
         self.dst_ip_min, self.dst_ip_max = self.__init_ip_input(args.dst)
         self.src_ip_min, self.src_ip_max = self.__init_ip_input(args.src)
         self.dst_port_min, self.dst_port_max = self.__init_port_range(args.portrange)
@@ -105,15 +113,17 @@
         if args.burst is not None:
             self.burst = int(args.burst)
         if args.threads is not None:
             self.threads = int(args.threads)
         self.stats = []
         if args.firstthread is not None:
             self.first_thread = int(args.firstthread)
-        self.thread_list = list(range(self.first_thread, self.first_thread + self.threads))
+        self.thread_list = list(
+            range(self.first_thread, self.first_thread + self.threads)
+        )
         if args.delay is not None:
             self.tx_delay = int(args.delay)
         if args.flows is not None:
             self.flows = int(args.flows)
         if args.flowpkts is not None:
             self.flow_len = int(args.flowpkts)
         self.__init_irq(args.queuemap)
@@ -132,88 +142,114 @@
         self.inner_dmac = args.innerdmac
         self.inner_smac = args.innersmac
         self.inner_dmac_count = 0
         self.inner_smac_count = 0
         self.microburst = args.microburst
         self.imixweight = args.imix
         self.__read_config_file(args.file)
+        if self.pgdev is None:
+            raise Exception("No interface specified")
+        if self.dst_ip_min == "":
+            raise Exception("No dst ip specified")
 
     def __read_config_file(self, file):
         cfg = configparser.ConfigParser()
         if file is not None:
-            with open(file, 'r') as f:
-                config_string = '[dummy]\n' + f.read()
+            with open(file, "r", encoding="utf-8") as f:
+                config_string = "[dummy]\n" + f.read()
                 cfg.read_string(config_string)
         else:
             return
-        if cfg.has_option('dummy', 'interface'):
-            self.pgdev = cfg.get('dummy', 'interface')
-        if cfg.has_option('dummy', 'pkt_size'):
-            self.pkt_size = cfg.getint('dummy', 'pkt_size')
-        if cfg.has_option('dummy', 'pkt_num'):
-            self.num = cfg.get_int('dummy', 'pkt_num')
-        if cfg.has_option('dummy', 'threads'):
-            self.thread_list = sum(((list(range(*[int(b) + c for c, b in enumerate(a.split('-'))]))
-                if '-' in a else [int(a)]) for a in cfg.get('dummy', 'threads').split(',')), [])
+        if cfg.has_option("dummy", "interface"):
+            self.pgdev = cfg.get("dummy", "interface")
+        if cfg.has_option("dummy", "pkt_size"):
+            self.pkt_size = cfg.getint("dummy", "pkt_size")
+        if cfg.has_option("dummy", "pkt_num"):
+            self.num = cfg.getint("dummy", "pkt_num")
+        if cfg.has_option("dummy", "threads"):
+            self.thread_list = sum(
+                (
+                    (
+                        list(range(*[int(b) + c for c, b in enumerate(a.split("-"))]))
+                        if "-" in a
+                        else [int(a)]
+                    )
+                    for a in cfg.get("dummy", "threads").split(",")
+                ),
+                [],
+            )
             self.first_thread = self.thread_list[0]
             self.threads = len(self.thread_list)
-        if cfg.has_option('dummy', 'bps_limit'):
-            self.bps_rate = cfg.get('dummy', 'bps_limit')
-        if cfg.has_option('dummy', 'pps_limit'):
-            self.pps_rate = cfg.get('dummy', 'pps_limit')
-        if cfg.has_option('dummy', 'burst'):
-            self.burst = cfg.getint('dummy', 'burst')
-        if cfg.has_option('dummy', 'imix_weight'):
-            self.clone = cfg.getint('dummy', 'clone')
-        if cfg.has_option('dummy', 'dst_ip'):
-            self.dst_ip_min, self.dst_ip_max = self.__init_ip_input(cfg.get('dummy', 'dst_ip'))
-        if cfg.has_option('dummy', 'src_ip'):
-            self.src_ip_min, self.src_ip_max = self.__init_ip_input(cfg.get('dummy', 'src_ip'))
-        if cfg.has_option('dummy', 'dstmac'):
-            self.dst_mac = cfg.get('dummy', 'dstmac')
-        if cfg.has_option('dummy', 'vlan'):
-            self.vlan = cfg.get('dummy', 'vlan')
-        if cfg.has_option('dummy', 'svlan'):
-            self.svlan = cfg.get('dummy', 'svlan')
-        if cfg.has_option('dummy', 'udp_src_port'):
-            self.src_port_min, self.src_port_max = self.__init_port_range(cfg.get('dummy', 'udp_src_port'))
-        if cfg.has_option('dummy', 'udp_dst_port'):
-            self.dst_port_min, self.dst_port_max = self.__init_port_range(cfg.get('dummy', 'udp_dst_port'))
-        if cfg.has_option('dummy', 'tos'):
-            self.tos = cfg['tos']
-        if cfg.has_option('dummy', 'tun_vni'):
-            self.tun_vni = cfg.get('dummy', 'tun_vni')
-        if cfg.has_option('dummy', 'tun_udp_port'):
-            self.tun_udpport = cfg.get('dummy', 'tun_udp_port')
-        if cfg.has_option('dummy', 'tun_src_ip'):
-            self.tun_src_min, self.tun_src_max = self.__init_ip_input(cfg.get('dummy', 'tun_src_ip'))
-        if cfg.has_option('dummy', 'tun_dst_ip'):
-            self.tun_dst_min, self.tun_dst_max = self.__init_ip_input(cfg.get('dummy', 'tun_dst_ip'))
-        if cfg.has_option('dummy', 'inner_dstmac'):
-            self.inner_dmac = cfg.get('dummy', 'inner_dstmac')
-        if cfg.has_option('dummy', 'inner_srcmac'):
-            self.inner_smac = cfg.get('dummy', 'inner_srcmac')
-        if cfg.has_option('dummy', 'inner_dmac_num'):
-            self.inner_dmac_count = cfg.getint('dummy', 'inner_dmac_num')
-        if cfg.has_option('dummy', 'inner_smac_num'):
-            self.inner_smac_count = cfg.getint('dummy', 'inner_smac_num')
-        if cfg.has_option('dummy', 'micro_burst'):
-            self.microburst = cfg.get('dummy', 'micro_burst')
-        if cfg.has_option('dummy', 'imix_weight'):
-            self.imixweight = cfg.get('dummy', 'imix_weight')
+        if cfg.has_option("dummy", "bps_limit"):
+            self.bps_rate = cfg.get("dummy", "bps_limit")
+        if cfg.has_option("dummy", "pps_limit"):
+            self.pps_rate = cfg.get("dummy", "pps_limit")
+        if cfg.has_option("dummy", "burst"):
+            self.burst = cfg.getint("dummy", "burst")
+        if cfg.has_option("dummy", "imix_weight"):
+            self.clone = cfg.getint("dummy", "clone")
+        if cfg.has_option("dummy", "dst_ip"):
+            self.dst_ip_min, self.dst_ip_max = self.__init_ip_input(
+                cfg.get("dummy", "dst_ip")
+            )
+        if cfg.has_option("dummy", "src_ip"):
+            self.src_ip_min, self.src_ip_max = self.__init_ip_input(
+                cfg.get("dummy", "src_ip")
+            )
+        if cfg.has_option("dummy", "dstmac"):
+            self.dst_mac = cfg.get("dummy", "dstmac")
+        if cfg.has_option("dummy", "vlan"):
+            self.vlan = cfg.get("dummy", "vlan")
+        if cfg.has_option("dummy", "svlan"):
+            self.svlan = cfg.get("dummy", "svlan")
+        if cfg.has_option("dummy", "udp_src_port"):
+            self.src_port_min, self.src_port_max = self.__init_port_range(
+                cfg.get("dummy", "udp_src_port")
+            )
+        if cfg.has_option("dummy", "udp_dst_port"):
+            self.dst_port_min, self.dst_port_max = self.__init_port_range(
+                cfg.get("dummy", "udp_dst_port")
+            )
+        if cfg.has_option("dummy", "tos"):
+            self.tos = cfg["tos"]
+        if cfg.has_option("dummy", "tun_vni"):
+            self.tun_vni = cfg.get("dummy", "tun_vni")
+        if cfg.has_option("dummy", "tun_udp_port"):
+            self.tun_udpport = cfg.get("dummy", "tun_udp_port")
+        if cfg.has_option("dummy", "tun_src_ip"):
+            self.tun_src_min, self.tun_src_max = self.__init_ip_input(
+                cfg.get("dummy", "tun_src_ip")
+            )
+        if cfg.has_option("dummy", "tun_dst_ip"):
+            self.tun_dst_min, self.tun_dst_max = self.__init_ip_input(
+                cfg.get("dummy", "tun_dst_ip")
+            )
+        if cfg.has_option("dummy", "inner_dstmac"):
+            self.inner_dmac = cfg.get("dummy", "inner_dstmac")
+        if cfg.has_option("dummy", "inner_srcmac"):
+            self.inner_smac = cfg.get("dummy", "inner_srcmac")
+        if cfg.has_option("dummy", "inner_dmac_num"):
+            self.inner_dmac_count = cfg.getint("dummy", "inner_dmac_num")
+        if cfg.has_option("dummy", "inner_smac_num"):
+            self.inner_smac_count = cfg.getint("dummy", "inner_smac_num")
+        if cfg.has_option("dummy", "micro_burst"):
+            self.microburst = cfg.get("dummy", "micro_burst")
+            self.burst = 0
+        if cfg.has_option("dummy", "imix_weight"):
+            self.imixweight = cfg.get("dummy", "imix_weight")
 
     def __init_ip_input(self, ipstr):
-        """ Init pktgen module ip dst """
+        """Init pktgen module ip dst"""
         if ipstr is None:
             return "", ""
         net = None
         try:
             net = ipaddress.ip_network(ipstr, strict=False)
         except (ValueError, TypeError):
-            ip_list = ipstr.split('-')
+            ip_list = ipstr.split("-")
             try:
                 ip_min = ipaddress.ip_address(ip_list[0])
             except (ValueError, TypeError):
                 print("invalid ip address format")
                 sys.exit()
             if len(ip_list) == 2:
                 try:
@@ -230,15 +266,15 @@
         return ip_min, ip_max
 
     def __init_port_range(self, portrange):
         """init port range for pktgen"""
         port_max = 65535
         port_min = 65535
         if portrange is not None:
-            ports = portrange.split('-')
+            ports = portrange.split("-")
             if len(ports) == 2:
                 port_max = int(ports[1])
             elif len(ports) == 1:
                 port_max = int(ports[0])
             port_min = int(ports[0])
         return port_min, port_max
 
@@ -258,69 +294,82 @@
         """pg_ctrl control "pgctrl" (/proc/net/pktgen/pgctrl)"""
         pgctrl = "/proc/net/pktgen/pgctrl"
         if cmd not in ["start", "stop", "reset"]:
             print("pgctrl do not support cmd %s" % cmd)
             sys.exit(1)
         open_write_error(pgctrl, cmd)
 
+    @staticmethod
+    def pg_version() -> str:
+        pgctrl = "/proc/net/pktgen/pgctrl"
+        try:
+            with open(pgctrl, "r", encoding="utf-8") as f_ctl:
+                cont = f_ctl.read()
+                m = re.search(r"Version: (\d.\d+)", cont)
+        except IOError:
+            return ""
+        if m is not None:
+            return m.group(1)
+        return ""
+
     def pg_set(self, dev, flag) -> None:
         """pg_set control setup of individual devices"""
         if dev.find(self.pgdev) < 0:
             print("device not match")
             sys.exit(1)
         pgdev = "/proc/net/pktgen/%s" % dev
         open_write_error(pgdev, flag)
 
     def __pg_get_devpath(self, index) -> str:
-        """ get dev path for thread index"""
+        """get dev path for thread index"""
         if self.queue is True:
             dev = "%s@%d" % (self.pgdev, self.cpu_list[index])
         else:
             dev = "%s@%d" % (self.pgdev, index)
         devpath = "/proc/net/pktgen/%s" % dev
         return devpath
 
     @staticmethod
     def pg_thread(thread, cmd) -> None:
-        """pg_thread() control the kernel threads and binding to devices """
+        """pg_thread() control the kernel threads and binding to devices"""
         pgthread = "/proc/net/pktgen/kpktgend_%d" % thread
         if cmd != "rem_device_all" and cmd.find("add_device") != 0:
             print("pg_thread do not support cmd %s" % cmd)
             sys.exit(1)
         open_write_error(pgthread, cmd, "w")
 
     @staticmethod
     def os_check() -> bool:
-        """ check if os is linux """
+        """check if os is linux"""
         return os.name == "posix"
 
     def __config_irq_affinity(self, irq, thread):
-        """ config irq affinity """
+        """config irq affinity"""
         irq_path = "/proc/irq/%d/smp_affinity_list" % irq
         open_write_error(irq_path, thread)
         if self.debug is True:
             print("irq %d is set affinity to %d" % (irq, thread))
 
     def __config_tos(self, dev) -> None:
-        """config tos """
+        """config tos"""
         if self.tos is not None and self.tos != 0:
             if self.ipv6 is True:
                 self.pg_set(dev, "traffic_class %0x" % self.tos)
             else:
                 self.pg_set(dev, "tos %0x" % self.tos)
 
     def __config_vlan(self, dev) -> None:
-        """config vlan related parameter """
+        """config vlan related parameter"""
         if self.vlan is not None and 0 <= int(self.vlan) < 4096:
             self.pg_set(dev, "vlan_id %d" % int(self.vlan))
         if self.svlan is not None and 0 <= int(self.svlan) < 4096:
             self.pg_set(dev, "svlan_id %d" % int(self.svlan))
 
     def __config_udp_portrange(self, dev) -> None:
-        """config udp port range """
+        """config udp port range"""
         if self.dst_port_max is not None:
             # Single destination port or random port range
             self.pg_set(dev, "flag UDPDST_RND")
             self.pg_set(dev, "udp_dst_min %d" % (self.dst_port_min))
             self.pg_set(dev, "udp_dst_max %d" % (self.dst_port_max))
 
         if self.csum is True:
@@ -348,23 +397,28 @@
             self.pg_set(dev, "src_max6 %s" % (self.src_ip_max))
         else:
             self.pg_set(dev, "src_min %s" % (self.src_ip_min))
             self.pg_set(dev, "src_max %s" % (self.src_ip_max))
 
     def __config_imix(self, dev) -> None:
         if self.imixweight is not None:
-            self.pg_set(dev, "imix_weights %s" % self.imixweight.replace(",", " ").replace(":", ","))
+            weight = self.imixweight.replace(",", " ").replace(":", ",")
+            self.pg_set(dev, "imix_weights %s" % weight)
 
-    def __config_microburst(self, dev) -> None:
+    def __config_burst_mode(self, dev) -> None:
         if self.microburst is not None:
             self.pg_set(dev, "micro_burst %s" % self.microburst)
+            self.burst = 0
+        # hw burst
+        if self.burst is not None and self.burst > 0:
+            self.pg_set(dev, "burst %d" % self.burst)
 
     def __config_tun_meta(self, dev) -> None:
         if self.tun_vni is not None:
-            vni = self.tun_vni.split('-')
+            vni = self.tun_vni.split("-")
             if len(vni) == 2:
                 vni_max = vni[1]
             elif len(vni) == 1:
                 vni_max = vni[0]
             vni_min = vni[0]
             self.pg_set(dev, "tun_meta_min %06x" % int(vni_min))
             self.pg_set(dev, "tun_meta_max %06x" % int(vni_max))
@@ -442,175 +496,185 @@
             self.__config_tun_meta(dev)
             self.pg_set(dev, "dst_mac %s" % (self.dst_mac))
             self.__config_ip_dst(dev)
             self.__config_ip_src(dev)
             self.__config_udp_portrange(dev)
             self.__config_vlan(dev)
 
-            # hw burst
-            if self.burst is not None and self.burst > 0:
-                self.pg_set(dev, "burst %d" % self.burst)
-
             self.__config_ratelimit(dev)
 
             self.__config_imix(dev)
-            self.__config_microburst(dev)
+            self.__config_burst_mode(dev)
 
     def reset(self) -> None:
-        """ reset pktgen"""
+        """reset pktgen"""
         if self.append is False:
             self.pg_ctrl("reset")
 
     def start(self) -> None:
         """start pktgen"""
         if self.append is False:
             self.pg_ctrl("start")
 
     def stop(self) -> None:
         """stop pktgen"""
         self.pg_ctrl("stop")
 
     @staticmethod
     def result_last(core_id, fp_dev, print_cb):
-        """print last result """
+        """print last result"""
         tpkts = 0
         tpps = 0
         tbps = 0
         tbps = 0
         stats_content = fp_dev.read()
         result_field = re.compile(
-            r'Result: (\w+): \d+\([\w\+]+\) \w+, (\d+) \(\d+byte,\d+frags\)')
+            r"Result: (\w+): \d+\([\w\+]+\) \w+, (\d+) \(\d+byte,\d+frags\)"
+        )
         throughput_field = re.compile(
-            r'  (\d+)pps \d+Mb\/sec \((\d+)bps\) errors: (\d+)')
-        unresult_field = re.compile(r'Result: (\w+)')
+            r"  (\d+)pps \d+Mb\/sec \((\d+)bps\) errors: (\d+)"
+        )
+        unresult_field = re.compile(r"Result: (\w+)")
         res = result_field.search(stats_content)
         pkt = throughput_field.search(stats_content)
         if res is not None and pkt is not None:
             tpkts = int(res.group(2))
             tpps = int(pkt.group(1))
             tbps = int(pkt.group(2))
             tbps = int(pkt.group(3))
-            print_cb("Core%3d send %18d pkts: %18d pps %18d bps %6d errors" %
-                     (core_id, int(res.group(2)), int(
-                         pkt.group(1)), int(pkt.group(2)), int(pkt.group(3))))
+            print_cb(
+                "Core%3d send %18d pkts: %18d pps %18d bps %6d errors"
+                % (
+                    core_id,
+                    int(res.group(2)),
+                    int(pkt.group(1)),
+                    int(pkt.group(2)),
+                    int(pkt.group(3)),
+                )
+            )
         else:
             other = unresult_field.search(stats_content)
             if other is not None:
                 print_cb("Core%3d %s" % (core_id, other.group(1)))
         return tpkts, tpps, tbps, tbps
 
     def result_transient(self, need_init, core_id, fp_dev, print_cb):
-        """print result during """
+        """print result during"""
         stats_content = fp_dev.read()
-        sofar_field = re.compile(r'pkts-sofar: (\d+)  errors: (\d+)')
-        time_field = re.compile(r'started: (\d+)us  stopped: (\d+)us')
+        sofar_field = re.compile(r"pkts-sofar: (\d+)  errors: (\d+)")
+        time_field = re.compile(r"started: (\d+)us  stopped: (\d+)us")
         sofar = sofar_field.search(stats_content)
         tim = time_field.search(stats_content)
         if need_init is True:
             pkt_sar = PktSar(int(tim.group(1)), self.pkt_size)
             self.stats.append(pkt_sar)
         else:
             pkt_sar = self.stats[core_id - self.first_thread]
         if sofar is not None:
             pkt_sar.update(int(sofar.group(1)), int(tim.group(2)))
             pps, bps = pkt_sar.get_stats()
             print_cb(
-                "Core%3d send %18d pkts: %18f pps %18f bps %6d errors" %
-                (core_id, int(sofar.group(1)), pps, bps, int(sofar.group(2))))
+                "Core%3d send %18d pkts: %18f pps %18f bps %6d errors"
+                % (core_id, int(sofar.group(1)), pps, bps, int(sofar.group(2)))
+            )
             return int(sofar.group(1)), pps, bps, int(sofar.group(2))
         return 0, 0, 0, 0
 
     def result(self, last, print_cb) -> int:
-        """ Print results """
+        """Print results"""
         if last is True:
             print("%d cores enabled" % self.threads)
         need_init = False
         total_pkts = 0
         total_pps = 0
         total_bps = 0
         total_err = 0
         if len(self.stats) == 0:
             need_init = True
         for i in self.thread_list:
             with open(self.__pg_get_devpath(i), "r") as fp_dev:
                 if last is False:
                     sg_pkts, sg_pps, sg_bps, sg_err = self.result_transient(
-                        need_init, i, fp_dev, print_cb)
+                        need_init, i, fp_dev, print_cb
+                    )
                 else:
                     sg_pkts, sg_pps, sg_bps, sg_err = self.result_last(
-                        i, fp_dev, print_cb)
+                        i, fp_dev, print_cb
+                    )
                 total_pkts += sg_pkts
                 total_pps += sg_pps
                 total_bps += sg_bps
                 total_err += sg_err
-        print_cb("Total   send %18d pkts: %18d pps %18d bps %6d errors" %
-                 (total_pkts, total_pps, total_bps, total_err))
+        print_cb(
+            "Total   send %18d pkts: %18d pps %18d bps %6d errors"
+            % (total_pkts, total_pps, total_bps, total_err)
+        )
         if last is False and self.num > 0 and total_pkts >= self.num:
             return 1
         return 0
 
     def __get_dev_numa(self) -> int:
-        """ __get_dev_numa returns the numa node of the device"""
+        """__get_dev_numa returns the numa node of the device"""
         numa_path = "/sys/class/net/%s/device/numa_node" % self.pgdev
         try:
             with open(numa_path, "r") as fp_numa:
-                node = fp_numa.read().rstrip('\n')
+                node = fp_numa.read().rstrip("\n")
         except IOError:
             print("Error: Cannot open %s" % (numa_path))
             return 0
-        if node == '-1':
+        if node == "-1":
             return 0
         return int(node)
 
     @staticmethod
     def __node_cpu_list(node) -> list:
-        """ __node_cpu_list returns the cpu list of the node """
+        """__node_cpu_list returns the cpu list of the node"""
         cpu_list = "/sys/devices/system/node/node%d/cpulist" % node
         try:
-            with open(cpu_list, 'r') as fp_cpu:
+            with open(cpu_list, "r") as fp_cpu:
                 cpu_range = fp_cpu.read()
         except IOError:
             print("Error: Cannot open %s" % (cpu_list))
             sys.exit(-1)
-        ranges = cpu_range.split(',')
+        ranges = cpu_range.split(",")
         ret = []
         for i in ranges:
-            cpu_start, cpu_end = i.split('-')
+            cpu_start, cpu_end = i.split("-")
             for j in range(int(cpu_start), int(cpu_end) + 1):
                 ret.append(j)
         return ret
 
     def __get_irqs(self):
-        """ read out irqs """
+        """read out irqs"""
         proc_intr = "/proc/interrupts"
         msi_irqs = "/sys/class/net/%s/device/msi_irqs" % self.pgdev
         try:
             with open(proc_intr, "r") as fp_proc:
                 intrs = fp_proc.read()
         except IOError:
             return []
         irqs = []
         devq_irq = re.compile(
-            r'(\d+):[ \d]+ [\w-]+ \d+-edge[ ]+%s-.*TxRx-\d+' % (self.pgdev))
+            r"(\d+):[ \d]+ [\w-]+ \d+-edge[ ]+%s-.*TxRx-\d+" % (self.pgdev)
+        )
         match = devq_irq.finditer(intrs)
         print(match)
         if len(devq_irq.findall(intrs)) > 0:
             for i in match:
                 irqs.append(int(i.group(1)))
             return irqs
-        dev_irq = re.compile(r'(\d+):[ \d]+ [\w-]+ \d+-edge[ ]+%s-\d+' %
-                             (self.pgdev))
+        dev_irq = re.compile(r"(\d+):[ \d]+ [\w-]+ \d+-edge[ ]+%s-\d+" % (self.pgdev))
         match = dev_irq.finditer(intrs)
         if len(dev_irq.findall(intrs)) > 0:
             for i in match:
                 irqs.append(int(i.group(1)))
             return irqs
         try:
             dirs = os.listdir(msi_irqs)
             for dev_q in dirs:
-                msi_irq = re.compile(r'%s:.*TxRx' % dev_q)
+                msi_irq = re.compile(r"%s:.*TxRx" % dev_q)
                 match = msi_irq.search(intrs)
                 if match is not None:
                     irqs.append(int(dev_q))
             return irqs
         except IOError:
             return []
```

### Comparing `pktperf-0.5.4/pktperf/pktperf.py` & `pktperf-0.5.5/pktperf/pktperf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,108 +1,151 @@
 #!/usr/bin/env python
 # -*- coding: UTF-8 -*-
 """ pktperf with cli options"""
-import sys
 import os
 import signal
 from threading import Thread, Event
 import time
 import argparse
 from .pktgen import Pktgen, modinfo_check
 
 
-parser = argparse.ArgumentParser(description="pktgen python scripts %s" %  modinfo_check(),
-                                epilog='\n')
-parser.add_argument('-i', '--interface', help="output interface/device",
-                    required=False)
-parser.add_argument('-s', '--size', help="packet size",
-                    default=60, required=False)
-parser.add_argument('-d', '--dst',
-                    help="destination IP address. CIDR is"
-                    " also allowed", required=False)
-parser.add_argument('--src',
-                    help="source IP address. CIDR is also allowed",
-                    required=False)
-parser.add_argument('-m', '--mac', help="destination MAC-addr",
-                    default="90:e2:ba:ff:ff:ff", required=False)
-parser.add_argument('-p', '--portrange', help="destination PORT range is"
-                    " also allowed", required=False)
-parser.add_argument('-k', '--txcsum', help="enable UDP tx checksum",
-                    required=False, action="store_true")
-parser.add_argument('-t', '--threads', help="threads to start",
-                    default=1, required=False)
-parser.add_argument('-f', '--firstthread', help="index of first thread",
-                    default=0, required=False)
-parser.add_argument('-c', '--clone', help="SKB clones before alloc new SKB",
-                    default=0, required=False)
-parser.add_argument('-n', '--num', help="num messages to send per thread,"
-                    " 0 means indefinitely",
-                    default=100000, required=False)
-parser.add_argument('-b', '--burst', help="HW level bursting of SKBs",
-                    default=0, required=False)
-parser.add_argument('-v', '--verbose', help="verbose", action="store_true")
-parser.add_argument('--debug', help="debug", action="store_true")
-parser.add_argument('--flows', help="Limit number of flows",
-                    default=0, required=False)
-parser.add_argument('--flowpkts', help="packets number a flow will send",
-                    required=False)
-parser.add_argument('-w', '--delay', help="Tx Delay value (ns)",
-                    default=0, required=False)
-parser.add_argument('--append', help="Script will not reset generator's"
-                    "state, but will append its config",
-                    required=False, action="store_true")
-parser.add_argument('-q', '--queuemap', help="queue mapping with irq affinity",
-                    required=False, action="store_true")
-parser.add_argument('--tos', help="tos for IPv4 or traffic class for IPv6 traffic",
-                    default=0, required=False)
-parser.add_argument('-r', '--bps', help="bps rate limit per thread", required=False)
-parser.add_argument('-y', '--pps', help="pps rate limit per thread", required=False)
-parser.add_argument('--frags', help="frags number in skb_shared_info",
-                    required=False)
-parser.add_argument('--vlan', help="vlan id 0-4095", required=False)
-parser.add_argument('--svlan', help="svlan id 0-4095", required=False)
-parser.add_argument('--file', help="config file for all pktgen parameters, will"
-                    " override all parameters specified from cmdline", required=False)
-
-if modinfo_check() == '3.0':
-    parser.add_argument('--vni', help="vxlan vni", required=False)
-    parser.add_argument('--tundport', help="vxlan udp port", required=False, default=4789)
-    parser.add_argument('--tundst', help="tunnel outer ip dst", required=False)
-    parser.add_argument('--tunsrc', help="tunnerl outer ip src", required=False)
-    parser.add_argument('--innerdmac', help="inner dst mac", required=False)
-    parser.add_argument('--innersmac', help="inner src mac", required=False)
-    parser.add_argument('--microburst', help="enable micro burst model", required=False)
-    parser.add_argument('--timeout', help="set timeout for pktgen runs", default=0, type=int)
-    parser.add_argument('--imix', help="set imix test weight parameter list", required=False)
+parser = argparse.ArgumentParser(
+    description="pktgen python scripts %s" % modinfo_check(), epilog="\n"
+)
+parser.add_argument("-i", "--interface", help="output interface/device", required=False)
+parser.add_argument("-s", "--size", help="packet size", default=60, required=False)
+parser.add_argument(
+    "-d",
+    "--dst",
+    help="destination IP address. CIDR is" " also allowed",
+    required=False,
+)
+parser.add_argument(
+    "--src", help="source IP address. CIDR is also allowed", required=False
+)
+parser.add_argument(
+    "-m",
+    "--mac",
+    help="destination MAC-addr",
+    default="90:e2:ba:ff:ff:ff",
+    required=False,
+)
+parser.add_argument(
+    "-p",
+    "--portrange",
+    help="destination PORT range is" " also allowed",
+    required=False,
+)
+parser.add_argument(
+    "-k", "--txcsum", help="enable UDP tx checksum", required=False, action="store_true"
+)
+parser.add_argument(
+    "-t", "--threads", help="threads to start", default=1, required=False
+)
+parser.add_argument(
+    "-f", "--firstthread", help="index of first thread", default=0, required=False
+)
+parser.add_argument(
+    "-c", "--clone", help="SKB clones before alloc new SKB", default=0, required=False
+)
+parser.add_argument(
+    "-n",
+    "--num",
+    help="num messages to send per thread," " 0 means indefinitely",
+    default=100000,
+    required=False,
+)
+parser.add_argument(
+    "-b", "--burst", help="HW level bursting of SKBs", default=0, required=False
+)
+parser.add_argument("-v", "--verbose", help="verbose", action="store_true")
+parser.add_argument("--debug", help="debug", action="store_true")
+parser.add_argument("--flows", help="Limit number of flows", default=0, required=False)
+parser.add_argument(
+    "--flowpkts", help="packets number a flow will send", required=False
+)
+parser.add_argument(
+    "-w", "--delay", help="Tx Delay value (ns)", default=0, required=False
+)
+parser.add_argument(
+    "--append",
+    help="Script will not reset generator's" "state, but will append its config",
+    required=False,
+    action="store_true",
+)
+parser.add_argument(
+    "-q",
+    "--queuemap",
+    help="queue mapping with irq affinity",
+    required=False,
+    action="store_true",
+)
+parser.add_argument(
+    "--tos",
+    help="tos for IPv4 or traffic class for IPv6 traffic",
+    default=0,
+    required=False,
+)
+parser.add_argument("-r", "--bps", help="bps rate limit per thread", required=False)
+parser.add_argument("-y", "--pps", help="pps rate limit per thread", required=False)
+parser.add_argument("--frags", help="frags number in skb_shared_info", required=False)
+parser.add_argument("--vlan", help="vlan id 0-4095", required=False)
+parser.add_argument("--svlan", help="svlan id 0-4095", required=False)
+parser.add_argument(
+    "--file",
+    help="config file for all pktgen parameters, will"
+    " override all parameters specified from cmdline",
+    required=False,
+)
+
+if modinfo_check() == "3.0":
+    parser.add_argument("--vni", help="vxlan vni", required=False)
+    parser.add_argument(
+        "--tundport", help="vxlan udp port", required=False, default=4789
+    )
+    parser.add_argument("--tundst", help="tunnel outer ip dst", required=False)
+    parser.add_argument("--tunsrc", help="tunnerl outer ip src", required=False)
+    parser.add_argument("--innerdmac", help="inner dst mac", required=False)
+    parser.add_argument("--innersmac", help="inner src mac", required=False)
+    parser.add_argument("--microburst", help="enable micro burst model", required=False)
+    parser.add_argument(
+        "--timeout", help="set timeout for pktgen runs", default=0, type=int
+    )
+    parser.add_argument(
+        "--imix", help="set imix test weight parameter list", required=False
+    )
 
 
 def ui_func(pktgen, event):
-    """ ui_func prints out statistics """
+    """ui_func prints out statistics"""
     while not event.is_set():
         print("")
         ret = pktgen.result(False, print)
         if ret == 1:
             os.kill(os.getpid(), signal.SIGINT)
         time.sleep(1)
     return 0
 
 
 def main():
-    """ main function entry """
+    """main function entry"""
     args = parser.parse_args()
     pktgen = Pktgen(args)
 
     event = Event()
-    tui = Thread(target=ui_func,
-                 name="ui",
-                 args=(
-                     pktgen,
-                     event,
-                 ),
-                 daemon=False)
+    tui = Thread(
+        target=ui_func,
+        name="ui",
+        args=(
+            pktgen,
+            event,
+        ),
+        daemon=False,
+    )
 
     def sig_exit(_sig, _frame):
         event.set()
         tui.join()
         pktgen.stop()
         pktgen.result(True, print)
```

### Comparing `pktperf-0.5.4/pktperf/pktsar.py` & `pktperf-0.5.5/pktperf/pktsar.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,33 +8,33 @@
 class PktSar:
     """pkt sar stats class
 
     calculate the pps and bps from the text
     """
 
     def __init__(self, start_time: int, pkt_size: int) -> None:
-        """ init sar stats """
+        """init sar stats"""
         self.start = start_time
         self._pkts = 0
         self._pkt_size = pkt_size
         self._bytes = 0
         self.last_update = start_time
         self.pps = 0.0
         self.bps = 0.0
 
     def update(self, pkts_so_far, timestamp):
-        """ update stats """
+        """update stats"""
         diff_pkts = pkts_so_far - self._pkts
         self._pkts = pkts_so_far
         diff_time = (timestamp - self.last_update) / 1000000
         if diff_time != 0:
             self.last_update = timestamp
             if timestamp == self.start:
                 self.pps = 0.0
                 self.bps = 0.0
             else:
                 self.pps = diff_pkts / diff_time
                 self.bps = self.pps * (self._pkt_size + 4)
 
     def get_stats(self):
-        """ get stats """
+        """get stats"""
         return self.pps, self.bps
```

### Comparing `pktperf-0.5.4/pktperf.egg-info/PKG-INFO` & `pktperf-0.5.5/pktperf.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pktperf
-Version: 0.5.4
+Version: 0.5.5
 Summary: pktgen scripts tool
 Author-email: junka <wan.junjie@foxmail.com>
 Project-URL: Homepage, https://github.com/junka/pktperf
 Project-URL: Bug Tracker, https://github.com/junka/pktperf/issues
 Platform: manylinux2014_x86_64
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
@@ -66,18 +66,18 @@
 packets sent.
 
 ```
 
 
 micro burst test case:
 
-```microburst duration_wait,duration_send```
+```microburst duration_poll,duration_idle```
 
 ```
-microbust 200,100
+microburst 200,100
 
 pktgen will be sending 200ms and then keep 100ms idle, loop follow the pattern
 ```
 
 
 During pktgen running, all stats will be display with 1 sec interval
 ```
```

### Comparing `pktperf-0.5.4/pyproject.toml` & `pktperf-0.5.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pktperf"
-version = "0.5.4"
+version = "0.5.5"
 authors = [
   { name="junka", email="wan.junjie@foxmail.com" },
 ]
 description = "pktgen scripts tool"
 readme = "README.md"
 requires-python = ">=3.5"
 classifiers = [
```

