# Comparing `tmp/vessim-0.0.1.tar.gz` & `tmp/vessim-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vessim-0.0.1.tar", last modified: Thu Mar  9 09:15:33 2023, max compression
+gzip compressed data, was "vessim-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `vessim-0.0.1.tar` & `vessim-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,47 @@
-drwxr-xr-x   0 philippwiesner   (501) staff       (20)        0 2023-03-09 09:15:33.679243 vessim-0.0.1/
--rw-r--r--   0 philippwiesner   (501) staff       (20)       86 2023-03-09 09:14:34.000000 vessim-0.0.1/.gitignore
--rw-r--r--   0 philippwiesner   (501) staff       (20)      276 2023-03-09 09:15:33.679028 vessim-0.0.1/PKG-INFO
--rw-r--r--   0 philippwiesner   (501) staff       (20)       10 2023-03-09 09:11:25.000000 vessim-0.0.1/README.md
--rw-r--r--   0 philippwiesner   (501) staff       (20)   304046 2023-03-09 09:15:03.000000 vessim-0.0.1/activity_diagram.drawio
-drwxr-xr-x   0 philippwiesner   (501) staff       (20)        0 2023-03-09 09:15:33.662382 vessim-0.0.1/data/
--rw-r--r--   0 philippwiesner   (501) staff       (20)    58362 2023-03-01 19:03:11.000000 vessim-0.0.1/data/custom.json
--rw-rw-r--   0 philippwiesner   (501) staff       (20) 15020336 2022-12-14 11:46:40.000000 vessim-0.0.1/data/pv_10kw.csv
--rw-r--r--   0 philippwiesner   (501) staff       (20)     2235 2023-03-09 08:45:12.000000 vessim-0.0.1/main.py
--rw-r--r--   0 philippwiesner   (501) staff       (20)     1319 2023-03-03 09:45:36.000000 vessim-0.0.1/pp_scenario.py
--rw-r--r--   0 philippwiesner   (501) staff       (20)      214 2023-03-09 08:35:44.000000 vessim-0.0.1/requirements.txt
--rw-r--r--   0 philippwiesner   (501) staff       (20)       38 2023-03-09 09:15:33.679312 vessim-0.0.1/setup.cfg
--rw-r--r--   0 philippwiesner   (501) staff       (20)     1135 2023-03-09 09:11:06.000000 vessim-0.0.1/setup.py
-drwxr-xr-x   0 philippwiesner   (501) staff       (20)        0 2023-03-09 09:15:33.677657 vessim-0.0.1/simulator/
--rw-r--r--   0 philippwiesner   (501) staff       (20)     1561 2023-03-03 23:46:05.000000 vessim-0.0.1/simulator/collector.py
--rw-r--r--   0 philippwiesner   (501) staff       (20)     2339 2023-03-09 08:38:17.000000 vessim-0.0.1/simulator/computing_system.py
--rw-r--r--   0 philippwiesner   (501) staff       (20)     2299 2023-03-09 08:42:22.000000 vessim-0.0.1/simulator/power_meter.py
-drwxr-xr-x   0 philippwiesner   (501) staff       (20)        0 2023-03-09 09:15:33.678753 vessim-0.0.1/vessim.egg-info/
--rw-r--r--   0 philippwiesner   (501) staff       (20)      276 2023-03-09 09:15:33.000000 vessim-0.0.1/vessim.egg-info/PKG-INFO
--rw-r--r--   0 philippwiesner   (501) staff       (20)      325 2023-03-09 09:15:33.000000 vessim-0.0.1/vessim.egg-info/SOURCES.txt
--rw-r--r--   0 philippwiesner   (501) staff       (20)        1 2023-03-09 09:15:33.000000 vessim-0.0.1/vessim.egg-info/dependency_links.txt
--rw-r--r--   0 philippwiesner   (501) staff       (20)        1 2023-03-09 09:15:33.000000 vessim-0.0.1/vessim.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1085 2023-06-04 18:37:57.805833 vessim-0.0.2/.github/workflows/vessim-ci.yml
+-rw-r--r--   0        0        0     1142 2023-06-09 11:35:36.040425 vessim-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1089 2023-06-09 10:55:14.692611 vessim-0.0.2/LICENSE
+-rw-r--r--   0        0        0      289 2023-06-09 11:36:26.384790 vessim-0.0.2/README.md
+-rw-r--r--   0        0        0     4696 2023-06-05 11:14:10.461302 vessim-0.0.2/carbon-aware_control_unit/carbon_aware_control_unit.py
+-rw-r--r--   0        0        0      931 2023-05-23 12:28:30.339243 vessim-0.0.2/carbon-aware_control_unit/main.py
+-rw-r--r--   0        0        0   427933 2023-05-23 13:29:52.934217 vessim-0.0.2/evaluation.ipynb
+-rw-r--r--   0        0        0     2097 2023-06-05 11:17:48.679082 vessim-0.0.2/example_node/README.md
+-rw-r--r--   0        0        0     2037 2023-06-08 11:05:26.203311 vessim-0.0.2/example_node/node_api_server.py
+-rw-r--r--   0        0        0      173 2023-06-05 11:14:10.462401 vessim-0.0.2/example_node/rpi/config/config.txt
+-rw-r--r--   0        0        0      159 2023-06-05 11:14:10.462724 vessim-0.0.2/example_node/rpi/config/rc.local
+-rw-r--r--   0        0        0     1405 2023-06-05 11:14:10.463000 vessim-0.0.2/example_node/rpi/init.sh
+-rw-r--r--   0        0        0     2127 2023-06-05 11:14:10.463312 vessim-0.0.2/example_node/rpi/lib/pi_controller.py
+-rw-r--r--   0        0        0       47 2023-06-05 11:14:10.463651 vessim-0.0.2/example_node/rpi/requirements.txt
+-rw-r--r--   0        0        0     1415 2023-06-08 11:05:26.203642 vessim-0.0.2/example_node/rpi/rpi_api_server.py
+-rw-r--r--   0        0        0      638 2023-06-05 11:14:10.464204 vessim-0.0.2/example_node/virtual_node/linear_power_model.py
+-rw-r--r--   0        0        0       23 2023-06-05 11:17:48.679232 vessim-0.0.2/example_node/virtual_node/requirements.txt
+-rw-r--r--   0        0        0     3671 2023-06-08 11:05:26.203868 vessim-0.0.2/example_node/virtual_node/v_node_api_server.py
+-rw-r--r--   0        0        0     1379 2023-06-09 11:06:42.915265 vessim-0.0.2/experimental/pp_scenario.py
+-rw-r--r--   0        0        0     2375 2023-06-08 11:04:22.045307 vessim-0.0.2/lib/http_client.py
+-rw-r--r--   0        0        0     3783 2023-06-09 08:28:46.374666 vessim-0.0.2/main.py
+-rw-r--r--   0        0        0     3533 2023-06-09 08:28:51.975101 vessim-0.0.2/main_new.py
+-rw-r--r--   0        0        0     2956 2023-06-09 11:38:59.333992 vessim-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      415 2023-06-09 11:36:08.170605 vessim-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     1811 2023-06-09 08:20:55.357876 vessim-0.0.2/simulator/computing_system.py
+-rw-r--r--   0        0        0     1753 2023-06-09 08:20:55.358152 vessim-0.0.2/simulator/power_meter.py
+-rw-r--r--   0        0        0     4522 2023-06-08 11:04:22.046853 vessim-0.0.2/simulator/redis_docker.py
+-rw-r--r--   0        0        0     1224 2023-06-08 11:04:22.047006 vessim-0.0.2/simulator/solar_controller.py
+-rw-r--r--   0        0        0     9403 2023-06-09 11:36:26.385012 vessim-0.0.2/simulator/virtual_energy_system.py
+-rw-r--r--   0        0        0     1438 2023-06-09 08:30:30.957245 vessim-0.0.2/tests/test_carbon_api.py
+-rw-r--r--   0        0        0     1910 2023-06-08 11:05:26.204334 vessim-0.0.2/tests/test_storage.py
+-rw-r--r--   0        0        0      897 2023-05-23 12:28:30.349242 vessim-0.0.2/tf_gcp_node/.gitignore
+-rw-r--r--   0        0        0     2253 2023-05-23 12:28:30.349446 vessim-0.0.2/tf_gcp_node/README.md
+-rw-r--r--   0        0        0     3194 2023-06-08 11:05:26.204615 vessim-0.0.2/tf_gcp_node/main.tf
+-rw-r--r--   0        0        0      249 2023-05-23 12:28:30.349833 vessim-0.0.2/tf_gcp_node/outputs.tf
+-rwxr-xr-x   0        0        0      262 2023-05-23 12:28:30.350118 vessim-0.0.2/tf_gcp_node/ssh_scripts/tfreceive
+-rwxr-xr-x   0        0        0      248 2023-05-23 12:28:30.350465 vessim-0.0.2/tf_gcp_node/ssh_scripts/tfsend
+-rwxr-xr-x   0        0        0      225 2023-05-23 12:28:30.350732 vessim-0.0.2/tf_gcp_node/ssh_scripts/tfssh
+-rw-r--r--   0        0        0      667 2023-05-23 12:28:30.351270 vessim-0.0.2/tf_gcp_node/variables.tf
+-rw-r--r--   0        0        0       83 2023-06-09 11:34:03.886216 vessim-0.0.2/vessim/__init__.py
+-rw-r--r--   0        0        0      416 2023-06-08 15:37:09.254824 vessim-0.0.2/vessim/_util.py
+-rw-r--r--   0        0        0     3661 2023-06-09 08:28:23.139799 vessim-0.0.2/vessim/carbon_api.py
+-rw-r--r--   0        0        0     4166 2023-06-09 08:24:59.930007 vessim-0.0.2/vessim/core.py
+-rw-r--r--   0        0        0     1500 2023-06-08 11:05:23.749112 vessim-0.0.2/vessim/microgrid.py
+-rw-r--r--   0        0        0     1977 2023-06-08 22:58:27.902499 vessim-0.0.2/vessim/monitor.py
+-rw-r--r--   0        0        0     4028 2023-06-08 14:26:16.529827 vessim-0.0.2/vessim/storage.py
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 vessim-0.0.2/PKG-INFO
```

### Comparing `vessim-0.0.1/pp_scenario.py` & `vessim-0.0.2/experimental/pp_scenario.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,33 +7,49 @@
 
 # create buses
 b1 = pp.create_bus(net, vn_kv=0.4, name="bus1")
 b2 = pp.create_bus(net, vn_kv=0.4, name="bus2")
 b3 = pp.create_bus(net, vn_kv=0.4, name="bus3")
 
 # create bus elements
-pp.create_ext_grid(net, bus=b1, vm_pu=1.02, name="grid connection")  # TODO Why voltage 1.02 pu https://github.com/e2nIEE/pandapower/blob/develop/tutorials/minimal_example.ipynb
+pp.create_ext_grid(
+    net, bus=b1, vm_pu=1.02, name="grid connection"
+)  # TODO Why voltage 1.02 pu https://github.com/e2nIEE/pandapower/blob/develop/tutorials/minimal_example.ipynb
 pp.create_load(net, bus=b3, p_mw=0.1, q_mvar=0.05, name="load")
 
 # create branch elements
-pp.create_line(net, from_bus=b1, to_bus=b2, length_km=0.1, name="line1", std_type="NAYY 4x50 SE")
-pp.create_line(net, from_bus=b2, to_bus=b3, length_km=0.1, name="line2", std_type="NAYY 4x50 SE")
+pp.create_line(
+    net,
+    from_bus=b1,
+    to_bus=b2,
+    length_km=0.1,
+    name="line1",
+    std_type="NAYY 4x50 SE",
+)
+pp.create_line(
+    net,
+    from_bus=b2,
+    to_bus=b3,
+    length_km=0.1,
+    name="line2",
+    std_type="NAYY 4x50 SE",
+)
 
-with pd.option_context('display.expand_frame_repr', False):
+with pd.option_context("display.expand_frame_repr", False):
     print("\nBus")
     print(net.bus)
     print("\nLine")
     print(net.line)
     print("\nLoad")
     print(net.load)
 
 print("\n---------------\nSOLVE\n---------------")
 pp.runpp(net)
 
-with pd.option_context('display.expand_frame_repr', False):
+with pd.option_context("display.expand_frame_repr", False):
     print("\nResult: Ext Grid")
     print(net.res_ext_grid)
     print("\nResult: Bus")
     print(net.res_bus)
     print("\nResult: Line")
     print(net.res_line)
     print("\nResult: Load")
```

### Comparing `vessim-0.0.1/simulator/collector.py` & `vessim-0.0.2/vessim/monitor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,59 +1,69 @@
-"""
-A simple data collector that prints all data when the simulation finishes.
+from collections import defaultdict
+from datetime import datetime, timedelta
+from typing import Dict, Callable, Any
 
-"""
-import collections
+import pandas as pd
+import csv
 from loguru import logger
 
 import mosaik_api
 
+from vessim._util import Clock
 
 META = {
-    'type': 'event-based',
-    'models': {
-        'Monitor': {
-            'public': True,
-            'any_inputs': True,
-            'params': [],
-            'attrs': [],
+    "type": "event-based",
+    "models": {
+        "Monitor": {
+            "public": True,
+            "any_inputs": True,
+            "params": ["fn", "sim_start"],
+            "attrs": [],
         },
     },
 }
 
 
-class Collector(mosaik_api.Simulator):
+class Monitor(mosaik_api.Simulator):
+    """Simple data collector for printing data at the end of simulation.
+
+    Attributes:
+        eid: Identifier of Simulator Instance
+        data: Dictionary for holding the necessary simulation data
+    """
+
     def __init__(self):
         super().__init__(META)
         self.eid = None
-        self.data = collections.defaultdict(lambda: collections.defaultdict(dict))
+        self.data = defaultdict(dict)
+        self.fn = None
+        self._clock = None
 
     def init(self, sid, time_resolution):
         return self.meta
 
-    def create(self, num, model):
+    def create(self, num, model, fn: Callable[[], Dict[str, Any]], sim_start: datetime):
+        self.fn = fn
+        self._clock = Clock(sim_start)
         if num > 1 or self.eid is not None:
-            raise RuntimeError('Can only create one instance of Monitor.')
+            raise RuntimeError("Can only create one instance of Monitor.")
 
-        self.eid = 'Monitor'
-        return [{'eid': self.eid, 'type': model}]
+        self.eid = "Monitor"
+        return [{"eid": self.eid, "type": model}]
 
     def step(self, time, inputs, max_advance):
+        dt = self._clock.to_datetime(time)
         data = inputs.get(self.eid, {})
-        logger.info(f"# {str(time):>5} ----------")
+        logger.info(f"# --- {str(dt):>5} ---")
         for attr, values in data.items():
             for src, value in values.items():
-                logger.info(f"{src}[{attr}] = {value}")
-                self.data[src][attr][time] = value
+                logger.info(f"{attr}: {value}")
+                self.data[attr][dt] = value
+        if self.fn is not None:
+            for attr, value in self.fn().items():
+                logger.info(f"{attr}: {value}")
+                self.data[attr][dt] = value
         return None
 
     def finalize(self):
-        return
-        print('Collected data:')
-        for sim, sim_data in sorted(self.data.items()):
-            print('- %s:' % sim)
-            for attr, values in sorted(sim_data.items()):
-                print('  - %s: %s' % (attr, values))
-
-
-if __name__ == '__main__':
-    mosaik_api.start_simulation(Collector())
+        """Collected data is printed to file at simulation end."""
+        pd.DataFrame(self.data).to_csv("data.csv")
```

