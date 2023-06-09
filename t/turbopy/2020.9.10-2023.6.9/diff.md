# Comparing `tmp/turbopy-2020.9.10.tar.gz` & `tmp/turbopy-2023.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/turbopy-2020.9.10.tar", last modified: Thu Sep 10 16:52:38 2020, max compression
+gzip compressed data, was "turbopy-2023.6.9.tar", last modified: Fri Jun  9 19:03:33 2023, max compression
```

## Comparing `turbopy-2020.9.10.tar` & `turbopy-2023.6.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/
--rw-r--r--   0 asrich     (501) staff       (20)     7048 2020-02-21 00:01:50.000000 turbopy-2020.9.10/LICENSE
--rw-r--r--   0 asrich     (501) staff       (20)       26 2020-08-12 19:07:54.000000 turbopy-2020.9.10/MANIFEST.in
--rw-r--r--   0 asrich     (501) staff       (20)     4483 2020-09-10 16:52:38.000000 turbopy-2020.9.10/PKG-INFO
--rw-r--r--   0 asrich     (501) staff       (20)     3303 2020-08-25 13:21:08.000000 turbopy-2020.9.10/README.md
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/docs/
--rw-r--r--   0 asrich     (501) staff       (20)     2997 2020-09-10 16:50:11.000000 turbopy-2020.9.10/docs/conf.py
--rw-r--r--   0 asrich     (501) staff       (20)       38 2020-09-10 16:52:38.000000 turbopy-2020.9.10/setup.cfg
--rw-r--r--   0 asrich     (501) staff       (20)     3671 2020-08-12 20:18:36.000000 turbopy-2020.9.10/setup.py
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/tests/
--rw-r--r--   0 asrich     (501) staff       (20)      128 2020-07-30 20:42:00.000000 turbopy-2020.9.10/tests/conftest.py
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/tests/fixtures/
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/tests/fixtures/block_on_spring/
--rw-r--r--   0 asrich     (501) staff       (20)     5581 2020-09-02 14:09:47.000000 turbopy-2020.9.10/tests/fixtures/block_on_spring/block_on_spring.py
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/tests/fixtures/particle_in_field/
--rw-r--r--   0 asrich     (501) staff       (20)     5054 2020-09-02 14:09:47.000000 turbopy-2020.9.10/tests/fixtures/particle_in_field/particle_in_field.py
--rw-r--r--   0 asrich     (501) staff       (20)     2469 2020-09-02 14:09:47.000000 turbopy-2020.9.10/tests/test_bos.py
--rw-r--r--   0 asrich     (501) staff       (20)    11817 2020-08-25 12:03:09.000000 turbopy-2020.9.10/tests/test_computetools.py
--rw-r--r--   0 asrich     (501) staff       (20)    14315 2020-09-09 20:45:55.000000 turbopy-2020.9.10/tests/test_core.py
--rw-r--r--   0 asrich     (501) staff       (20)     3917 2020-09-04 19:22:36.000000 turbopy-2020.9.10/tests/test_diagnostics.py
--rw-r--r--   0 asrich     (501) staff       (20)      761 2020-09-02 14:09:47.000000 turbopy-2020.9.10/tests/test_pif.py
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/turbopy/
--rw-r--r--   0 asrich     (501) staff       (20)      189 2020-07-27 19:40:12.000000 turbopy-2020.9.10/turbopy/__init__.py
--rw-r--r--   0 asrich     (501) staff       (20)      115 2020-09-10 16:49:56.000000 turbopy-2020.9.10/turbopy/__version__.py
--rw-r--r--   0 asrich     (501) staff       (20)    15822 2020-08-25 12:03:09.000000 turbopy-2020.9.10/turbopy/computetools.py
--rw-r--r--   0 asrich     (501) staff       (20)      693 2020-07-20 17:20:39.000000 turbopy-2020.9.10/turbopy/constructors.py
--rw-r--r--   0 asrich     (501) staff       (20)    33560 2020-09-09 20:45:55.000000 turbopy-2020.9.10/turbopy/core.py
--rw-r--r--   0 asrich     (501) staff       (20)    12405 2020-09-04 19:22:36.000000 turbopy-2020.9.10/turbopy/diagnostics.py
-drwxr-xr-x   0 asrich     (501) staff       (20)        0 2020-09-10 16:52:38.000000 turbopy-2020.9.10/turbopy.egg-info/
--rw-r--r--   0 asrich     (501) staff       (20)     4483 2020-09-10 16:52:37.000000 turbopy-2020.9.10/turbopy.egg-info/PKG-INFO
--rw-r--r--   0 asrich     (501) staff       (20)      565 2020-09-10 16:52:37.000000 turbopy-2020.9.10/turbopy.egg-info/SOURCES.txt
--rw-r--r--   0 asrich     (501) staff       (20)        1 2020-09-10 16:52:37.000000 turbopy-2020.9.10/turbopy.egg-info/dependency_links.txt
--rw-r--r--   0 asrich     (501) staff       (20)       25 2020-09-10 16:52:37.000000 turbopy-2020.9.10/turbopy.egg-info/requires.txt
--rw-r--r--   0 asrich     (501) staff       (20)       19 2020-09-10 16:52:37.000000 turbopy-2020.9.10/turbopy.egg-info/top_level.txt
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.442278 turbopy-2023.6.9/
+-rw-r--r--   0 ndisner    (502) staff       (20)     7048 2023-06-09 18:59:00.000000 turbopy-2023.6.9/LICENSE
+-rw-r--r--   0 ndisner    (502) staff       (20)       26 2023-06-09 18:59:00.000000 turbopy-2023.6.9/MANIFEST.in
+-rw-r--r--   0 ndisner    (502) staff       (20)     7846 2023-06-09 19:03:33.441559 turbopy-2023.6.9/PKG-INFO
+-rw-r--r--   0 ndisner    (502) staff       (20)     7092 2023-06-09 18:59:00.000000 turbopy-2023.6.9/README.md
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.426467 turbopy-2023.6.9/docs/
+-rw-r--r--   0 ndisner    (502) staff       (20)     3046 2023-06-09 18:59:00.000000 turbopy-2023.6.9/docs/conf.py
+-rw-r--r--   0 ndisner    (502) staff       (20)       38 2023-06-09 19:03:33.442477 turbopy-2023.6.9/setup.cfg
+-rw-r--r--   0 ndisner    (502) staff       (20)     3656 2023-06-09 18:59:00.000000 turbopy-2023.6.9/setup.py
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.431188 turbopy-2023.6.9/tests/
+-rw-r--r--   0 ndisner    (502) staff       (20)      128 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/conftest.py
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.422691 turbopy-2023.6.9/tests/fixtures/
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.431906 turbopy-2023.6.9/tests/fixtures/block_on_spring/
+-rw-r--r--   0 ndisner    (502) staff       (20)     4984 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/fixtures/block_on_spring/block_on_spring.py
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.432951 turbopy-2023.6.9/tests/fixtures/particle_in_field/
+-rw-r--r--   0 ndisner    (502) staff       (20)     3754 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/fixtures/particle_in_field/particle_in_field.py
+-rw-r--r--   0 ndisner    (502) staff       (20)     2469 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/test_bos.py
+-rw-r--r--   0 ndisner    (502) staff       (20)    11829 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/test_computetools.py
+-rw-r--r--   0 ndisner    (502) staff       (20)    19604 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/test_core.py
+-rw-r--r--   0 ndisner    (502) staff       (20)     6874 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/test_diagnostics.py
+-rw-r--r--   0 ndisner    (502) staff       (20)      784 2023-06-09 18:59:00.000000 turbopy-2023.6.9/tests/test_pif.py
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.437115 turbopy-2023.6.9/turbopy/
+-rw-r--r--   0 ndisner    (502) staff       (20)      189 2023-06-09 18:59:00.000000 turbopy-2023.6.9/turbopy/__init__.py
+-rw-r--r--   0 ndisner    (502) staff       (20)      115 2023-06-09 18:59:00.000000 turbopy-2023.6.9/turbopy/__version__.py
+-rw-r--r--   0 ndisner    (502) staff       (20)    15822 2023-06-09 18:59:00.000000 turbopy-2023.6.9/turbopy/computetools.py
+-rw-r--r--   0 ndisner    (502) staff       (20)      693 2023-06-09 18:59:00.000000 turbopy-2023.6.9/turbopy/constructors.py
+-rw-r--r--   0 ndisner    (502) staff       (20)    38390 2023-06-09 18:59:00.000000 turbopy-2023.6.9/turbopy/core.py
+-rw-r--r--   0 ndisner    (502) staff       (20)    23838 2023-06-09 18:59:00.000000 turbopy-2023.6.9/turbopy/diagnostics.py
+drwxr-xr-x   0 ndisner    (502) staff       (20)        0 2023-06-09 19:03:33.440537 turbopy-2023.6.9/turbopy.egg-info/
+-rw-r--r--   0 ndisner    (502) staff       (20)     7846 2023-06-09 19:03:33.000000 turbopy-2023.6.9/turbopy.egg-info/PKG-INFO
+-rw-r--r--   0 ndisner    (502) staff       (20)      565 2023-06-09 19:03:33.000000 turbopy-2023.6.9/turbopy.egg-info/SOURCES.txt
+-rw-r--r--   0 ndisner    (502) staff       (20)        1 2023-06-09 19:03:33.000000 turbopy-2023.6.9/turbopy.egg-info/dependency_links.txt
+-rw-r--r--   0 ndisner    (502) staff       (20)       25 2023-06-09 19:03:33.000000 turbopy-2023.6.9/turbopy.egg-info/requires.txt
+-rw-r--r--   0 ndisner    (502) staff       (20)       24 2023-06-09 19:03:33.000000 turbopy-2023.6.9/turbopy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `turbopy-2020.9.10/LICENSE` & `turbopy-2023.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `turbopy-2020.9.10/docs/conf.py` & `turbopy-2023.6.9/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,28 +6,29 @@
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 
+import sphinx_rtd_theme
 import os
 import sys
 sys.path.insert(0, os.path.abspath('..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'turboPy'
 # copyright = '2020, Steve Richardson'
 html_show_copyright = False
 author = 'Steve Richardson'
 
 # The full version, including alpha/beta/rc tags
-release = 'v2020.09.10'
+release = 'v2023.06.09'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
@@ -64,16 +65,17 @@
 master_doc = 'index'
 
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
-html_static_path = ['_static']
+# html_theme = 'alabaster'
+html_theme = "sphinx_rtd_theme"
+html_static_path = []
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 # html_static_path = ['_static']
 
 html_theme_options = {
```

### Comparing `turbopy-2020.9.10/setup.py` & `turbopy-2023.6.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 
 # Package meta-data.
 NAME = 'turbopy'
 DESCRIPTION = ('A lightweight computational physics framework, which '
                'implements a "Simulation, PhysicsModule, ComputeTool" '
                'class hierarchy.')
 URL = 'https://github.com/NRL-Plasma-Physics-Division/turbopy'
-EMAIL = 'steve.richardson@nrl.navy.mil'
-AUTHOR = 'Steve Richardson'
-REQUIRES_PYTHON = '>=3.7.0'
+EMAIL = 'ndisner10@gmail.com'
+AUTHOR = 'Nancy Isner'
+REQUIRES_PYTHON = '>=3.9.0'
 VERSION = None
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy', 'scipy', 'qtoml', 'xarray'
 ]
 
@@ -111,15 +111,15 @@
     include_package_data=True,
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
```

### Comparing `turbopy-2020.9.10/tests/fixtures/block_on_spring/block_on_spring.py` & `turbopy-2023.6.9/tests/fixtures/block_on_spring/block_on_spring.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,61 +11,45 @@
         super().__init__(owner, input_data)
         self.position = np.zeros((1, 3))
         self.momentum = np.zeros((1, 3))
         self.mass = input_data.get('mass', 1)
         self.spring_constant = input_data.get('spring_constant', 1)
         self.push = owner.find_tool_by_name(input_data["pusher"]).push
 
+        self._resources_to_share = {"Block:position": self.position,
+                                    "Block:momentum": self.momentum}
+
     def initialize(self):
         self.position[:] = np.array(self._input_data["x0"])
 
-    def exchange_resources(self):
-        self.publish_resource({"Block:position": self.position})
-        self.publish_resource({"Block:momentum": self.momentum})
-
     def update(self):
         self.push(self.position, self.momentum,
                   self.mass, self.spring_constant)
 
 
 class BlockDiagnostic(Diagnostic):
     def __init__(self, owner: Simulation, input_data: dict):
         super().__init__(owner, input_data)
         self.data = None
         self.component = input_data.get("component", 1)
-        self.output_function = None
-        self.csv = None
+        self.outputter = None
 
-    def inspect_resource(self, resource):
-        if "Block:" + self.component in resource:
-            self.data = resource["Block:" + self.component]
+        self._needed_resources = {"Block:" + self.component: "data"}
 
     def diagnose(self):
-        self.output_function(self.data[0, :])
+        self.outputter.diagnose(self.data[0, :])
 
     def initialize(self):
-        # setup output method
-        functions = {"stdout": self.print_diagnose,
-                     "csv": self.csv_diagnose,
-                     }
-        self.output_function = functions[self._input_data["output_type"]]
-        if self._input_data["output_type"] == "csv":
-            diagnostic_size = (self._owner.clock.num_steps + 1, 3)
-            self.csv = CSVOutputUtility(self._input_data["filename"], diagnostic_size)
+        diagnostic_size = (self._owner.clock.num_steps + 1, 3)
+        self.outputter = CSVOutputUtility(self._input_data["filename"],
+                                          diagnostic_size)
 
     def finalize(self):
         self.diagnose()
-        if self._input_data["output_type"] == "csv":
-            self.csv.finalize()
-
-    def print_diagnose(self, data):
-        print(data)
-
-    def csv_diagnose(self, data):
-        self.csv.append(data)
+        self.outputter.finalize()
 
 
 class ForwardEuler(ComputeTool):
     """Implementation of the forward Euler algorithm
 
     y_{n+1} = y_n + h * f(t_n, y_n)
     """
@@ -131,15 +115,14 @@
 ComputeTool.register("Leapfrog", Leapfrog)
 
 
 @pytest.fixture
 def bos_run():
     # Note: grid isn't used, but "gridless" sims aren't an option yet
     problem_config = {
-        "Grid": {"N": 2, "x_min": 0, "x_max": 1},
         "Clock": {"start_time": 0,
                   "end_time": 10,
                   "num_steps": 10},
         "PhysicsModules": {
             "BlockOnSpring": {
                 "mass": 1,
                 "spring_constant": 1,
@@ -147,15 +130,15 @@
                 "x0": [0, 1, 0],
                 "p0": [0, 0, 0]
             }
         },
         "Tools": {
             "Leapfrog": {},
             "BlockForwardEuler": {},
-            "BackwardEuler":{}
+            "BackwardEuler": {}
         },
         "Diagnostics": {
             # default values come first
             "directory": "block_on_spring/output_leapfrog/",
             "output_type": "csv",
             "clock": {"filename": "time.csv"},
             "BlockDiagnostic": [
```

### Comparing `turbopy-2020.9.10/tests/test_bos.py` & `turbopy-2023.6.9/tests/test_bos.py`

 * *Files identical despite different names*

### Comparing `turbopy-2020.9.10/tests/test_computetools.py` & `turbopy-2023.6.9/tests/test_computetools.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,16 +22,16 @@
     owner = Simulation(input_data)
     owner.prepare_simulation()
     push_example = BorisPush(owner, input_data)
     charge = 1.6022e-19
     mass = 1.6726e-27
     E = np.zeros(3)
     B = np.zeros(3)
-    x_i = np.array([[0, 0, 0.0]], dtype=np.float)
-    v_i = np.array([[0, 0, 3.0e2]], dtype=np.float)
+    x_i = np.array([[0, 0, 0.0]], dtype=np.float64)
+    v_i = np.array([[0, 0, 3.0e2]], dtype=np.float64)
     p_i = mass * v_i
     clock = input_data["Clock"]
     N = 10
     x_final = v_i * N * clock["dt"]
     for i in range(N):
         push_example.push(x_i, p_i, charge, mass, E, B)
     assert np.allclose(x_i, x_final)
@@ -46,18 +46,18 @@
         "PhysicsModules": {}}
     owner = Simulation(input_data)
     owner.prepare_simulation()
     push_example = BorisPush(owner, input_data)
     charge = 1.6022e-19
     mass = 1.6726e-27
     N = 10
-    x_i = np.array([[0, 0, 0.0]], dtype=np.float)
-    p_i = np.array([[0, 0, 0.0]], dtype=np.float)
-    E = np.array([[10, 0, 0]], dtype=np.float)
-    B = np.array([[0, 0, 10]], dtype=np.float)
+    x_i = np.array([[0, 0, 0.0]], dtype=np.float64)
+    p_i = np.array([[0, 0, 0.0]], dtype=np.float64)
+    E = np.array([[10, 0, 0]], dtype=np.float64)
+    B = np.array([[0, 0, 10]], dtype=np.float64)
     for i in range(N):
         push_example.push(x_i, p_i, charge, mass, E, B)
     x_final = np.array([[2.20028479e-09, -1.04482737e-08, 0]])
     assert np.allclose(x_i, x_final)
     p_final = np.array([[0.47183691, -1.88168585,  0]]) * mass
     assert np.allclose(p_i / mass, p_final / mass)
```

### Comparing `turbopy-2020.9.10/tests/test_core.py` & `turbopy-2023.6.9/tests/test_core.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 """Tests for turbopy/core.py"""
 import pytest
-from turbopy.core import *
+import warnings
+from pathlib import Path
+import numpy as np
+from turbopy.core import (
+    ComputeTool,
+    PhysicsModule,
+    Diagnostic,
+    Simulation,
+    Grid,
+    SimulationClock)
 
 
 class ExampleTool(ComputeTool):
     """Example ComputeTool subclass for tests"""
 
 
 class ExampleModule(PhysicsModule):
     """Example PhysicsModule subclass for tests"""
     def update(self):
         pass
-    
+
     def inspect_resource(self, resource: dict):
         for attribute in resource:
             self.__setattr__(attribute, resource[attribute])
 
 
 class ExampleDiagnostic(Diagnostic):
     """Example Diagnostic subclass for tests"""
@@ -37,15 +46,15 @@
                      "end_time": 10,
                      "num_steps": 100},
            "Tools": {"ExampleTool": [
                         {"custom_name": "example"},
                         {"custom_name": "example2"}]},
            "PhysicsModules": {"ExampleModule": {}},
            "Diagnostics": {
-               #default values come first
+               # default values come first
                "directory": f"{tmp_path}/default_output",
                "clock": {},
                "ExampleDiagnostic": [
                    {},
                    {}
                    ]
                }
@@ -85,14 +94,174 @@
     """Test read_grid_from_input method in Simulation class"""
     simple_sim.read_grid_from_input()
     assert simple_sim.grid.num_points == 2
     assert simple_sim.grid.r_min == 0
     assert simple_sim.grid.r_max == 1
 
 
+# Test the old sharing API
+class ReceivingModule(PhysicsModule):
+    """Example PhysicsModule subclass for tests"""
+    def __init__(self, owner: Simulation, input_data: dict):
+        super().__init__(owner, input_data)
+        self.data = None
+
+    def inspect_resource(self, resource: dict):
+        if 'shared' in resource:
+            self.data = resource['shared']
+
+    def initialize(self):
+        # if resources are shared correctly, then this list will be accessible
+        print(f'The first data item is {self.data[0]}')
+
+    def update(self):
+        pass
+
+
+class SharingModule(PhysicsModule):
+    """Example PhysicsModule subclass for tests"""
+    def __init__(self, owner: Simulation, input_data: dict):
+        super().__init__(owner, input_data)
+        self.data = ['test']
+
+    def exchange_resources(self):
+        self.publish_resource({'shared': self.data})
+
+    def update(self):
+        pass
+
+
+PhysicsModule.register("Receiving", ReceivingModule)
+PhysicsModule.register("Sharing", SharingModule)
+
+
+@pytest.fixture(name='share_sim')
+def shared_simulation_fixture():
+    """Pytest fixture for basic simulation class"""
+    dic = {"Grid": {"N": 2, "r_min": 0, "r_max": 1},
+           "Clock": {"start_time": 0,
+                     "end_time": 10,
+                     "num_steps": 1},
+           "PhysicsModules": {
+               "Receiving": {},
+               "Sharing": {}
+           },
+           }
+    return Simulation(dic)
+
+
+def test_that_simulation_is_created(share_sim):
+    assert share_sim.physics_modules == []
+
+
+def test_that_v1_sharing_is_deprecated(share_sim):
+    with pytest.deprecated_call():
+        share_sim.prepare_simulation()
+
+
+def test_that_shared_resource_is_available_in_initialize(share_sim):
+    share_sim.prepare_simulation()
+    assert len(share_sim.physics_modules) == 2
+    assert len(share_sim.physics_modules[0].data) == 1
+    assert (id(share_sim.physics_modules[0].data)
+            == id(share_sim.physics_modules[1].data))
+
+
+# Test the new sharing API
+class ReceivingModuleV2(PhysicsModule):
+    """Example PhysicsModule subclass for tests"""
+    def __init__(self, owner: Simulation, input_data: dict):
+        super().__init__(owner, input_data)
+        self.data = None
+        self._needed_resources = {'shared': 'data'}
+
+    def initialize(self):
+        # if resources are shared correctly, then this list will be accessible
+        print(f'The first data item is {self.data[0]}')
+
+    def update(self):
+        pass
+
+
+class SharingModuleV2(PhysicsModule):
+    """Example PhysicsModule subclass for tests"""
+    def __init__(self, owner: Simulation, input_data: dict):
+        super().__init__(owner, input_data)
+        self.data = ['test']
+        self._resources_to_share = {'shared': self.data}
+
+    def update(self):
+        pass
+
+
+PhysicsModule.register("ReceivingV2", ReceivingModuleV2)
+PhysicsModule.register("SharingV2", SharingModuleV2)
+
+
+# Still need to add tests for the Diagnostics with the new API
+
+
+@pytest.fixture(name='share_sim_V2')
+def shared_simulation_V2_fixture():
+    """Pytest fixture for basic simulation class"""
+    dic = {"Grid": {"N": 2, "r_min": 0, "r_max": 1},
+           "Clock": {"start_time": 0,
+                     "end_time": 10,
+                     "num_steps": 1},
+           "PhysicsModules": {
+               "ReceivingV2": {},
+               "SharingV2": {}
+           },
+           }
+    return Simulation(dic)
+
+
+def test_that_V2_shared_resource_is_available_in_initialize(share_sim_V2):
+    share_sim_V2.prepare_simulation()
+    assert len(share_sim_V2.physics_modules) == 2
+    assert len(share_sim_V2.physics_modules[0].data) == 1
+    assert (id(share_sim_V2.physics_modules[0].data)
+            == id(share_sim_V2.physics_modules[1].data))
+
+
+def test_gridless_simulation(tmp_path):
+    """Test a gridless simulation"""
+    dic = {"Clock": {"start_time": 0,
+                     "end_time": 10,
+                     "num_steps": 100},
+           "Tools": {"ExampleTool": [
+               {"custom_name": "example"},
+               {"custom_name": "example2"}]},
+           "PhysicsModules": {"ExampleModule": {}},
+           "Diagnostics": {
+               # default values come first
+               "directory": f"{tmp_path}/default_output",
+               "clock": {},
+               "ExampleDiagnostic": [
+                   {},
+                   {}
+               ]
+           }
+           }
+    with warnings.catch_warnings(record=True) as w:
+        sim = Simulation(dic)
+        sim.run()
+        assert sim.clock is not None
+        assert sim.grid is None
+        assert len(w) == 1
+        assert str(w[-1].message) == "No Grid Found."
+
+
+def test_subclass(simple_sim):
+    """Test if subclasses are contained in Simulation"""
+    assert issubclass(ExampleModule, PhysicsModule)
+    assert issubclass(ExampleDiagnostic, Diagnostic)
+    assert issubclass(ExampleTool, ComputeTool)
+
+
 def test_read_clock_from_input_should_set_clock_attr_when_called(simple_sim):
     """Test read_clock_from_input method in Simulation class"""
     simple_sim.read_clock_from_input()
     assert simple_sim.clock._owner == simple_sim
     assert simple_sim.clock.start_time == 0
     assert simple_sim.clock.time == 0
     assert simple_sim.clock.end_time == 10
@@ -144,15 +313,15 @@
     assert simple_sim.clock.time == 0.1
     simple_sim.clock.turn_back()
     assert simple_sim.clock.this_step == 0
     assert simple_sim.clock.time == 0
 
 
 def test_read_modules_from_input_should_set_modules_attr_when_called(simple_sim):
-    """Test read_modules_from_input method in Simulation calss"""
+    """Test read_modules_from_input method in Simulation class"""
     simple_sim.read_modules_from_input()
     assert simple_sim.physics_modules[0]._owner == simple_sim
     assert simple_sim.physics_modules[0]._input_data == {"name": "ExampleModule"}
 
 
 def test_find_tool_by_name_should_identify_one_tool(simple_sim):
     simple_sim.read_tools_from_input()
@@ -175,15 +344,15 @@
 
 
 def test_default_diagnostic_filename_increments_for_multiple_diagnostics(simple_sim, tmp_path):
     """Test read_diagnostic_from_input method in Simulation class"""
     simple_sim.read_diagnostics_from_input()
     assert simple_sim.diagnostics[0]._input_data["directory"] == str(Path(f"{tmp_path}/default_output"))
     assert simple_sim.diagnostics[0]._input_data["filename"] == str(Path(f"{tmp_path}/default_output")
-                                                                   / Path("clock0.out"))
+                                                                    / Path("clock0.out"))
     input_data = simple_sim.diagnostics[2]._input_data
     assert input_data["directory"] == str(Path(f"{tmp_path}/default_output"))
     assert input_data["filename"] == str(Path(f"{tmp_path}/default_output")
                                          / Path("ExampleDiagnostic1.out"))
 
 
 # Grid class test methods
@@ -242,14 +411,20 @@
 def test_create_interpolator(simple_grid):
     """Test create_interpolator method in Grid class"""
     field = simple_grid.generate_linear()
     r_val = 0.05
     interp = simple_grid.create_interpolator(r_val)
     linear_value = r_val / (simple_grid.r_max - simple_grid.r_min)
     assert np.allclose(interp(field), linear_value)
+    r_val = -0.1
+    with pytest.raises(AssertionError):
+        interp = simple_grid.create_interpolator(r_val)
+    r_val = 0.2
+    with pytest.raises(AssertionError):
+        interp = simple_grid.create_interpolator(r_val)
 
 
 def test_set_cartesian_volumes():
     """Test that cell volumes are set properly."""
     grid_conf2 = {"r_min": 0,
                   "r_max": 1,
                   "dr": 0.1,
```

### Comparing `turbopy-2020.9.10/tests/test_pif.py` & `turbopy-2023.6.9/tests/test_pif.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Integration test based on particle_in_field turbopy app
 
 This integration test simply runs the particle_in_field app and compares the 
 output files to "good" output.
 """
 import numpy as np
-import shutil
 
 
 def test_pif(pif_sim, tmp_path):
     pif_sim.input_data["Diagnostics"]["directory"] = f"{tmp_path}"
+    print(f"Temp path = {tmp_path}")
     pif_sim.run()
     for filename in ['e_0.5', 'grid', 'particle_p', 'particle_x', 'time']:
         ref_data = np.genfromtxt('tests/fixtures/particle_in_field/output/'
                                  f'{filename}.csv',
                                  delimiter=',')
         tmp_data = np.genfromtxt(f'{tmp_path}/{filename}.csv',
                                  delimiter=',')
```

### Comparing `turbopy-2020.9.10/turbopy/computetools.py` & `turbopy-2023.6.9/turbopy/computetools.py`

 * *Files identical despite different names*

### Comparing `turbopy-2020.9.10/turbopy/constructors.py` & `turbopy-2023.6.9/turbopy/constructors.py`

 * *Files identical despite different names*

### Comparing `turbopy-2020.9.10/turbopy/core.py` & `turbopy-2023.6.9/turbopy/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 """
 Core base classes of the turboPy framework
 
 Notes
 -----
-A preprint of the paper describing this code is available on
-the arxiv [1]_.
+The published paper for Turbopy: A lightweight python framework for \
+ computational physics can be found in the link below [1]_.
+
 
 References
 ----------
-.. [1] A. S. Richardson et al., "TurboPy: A Lightweight Python Framework
-       for Computational Physics." Preprint available online:
-       https://arxiv.org/abs/2002.08842
+.. [1] 1 A.S. Richardson, D.F. Gordon, S.B. Swanekamp, I.M. Rittersdorf, \
+P.E. Adamson, O.S. Grannis, G.T. Morgan, A. Ostenfeld, K.L. Phlips, C.G. Sun, \
+G. Tang, and D.J. Watkins, Comput. Phys. Commun. 258, 107607 (2021). \
+https://doi.org/10.1016/j.cpc.2020.107607
 
 """
 from pathlib import Path
 from abc import ABC, abstractmethod
 import numpy as np
+import warnings
 
 
 class Simulation:
     """Main turboPy simulation class
 
     This Class "owns" all the physics modules, compute tools, and
     diagnostics. It also coordinates them. The main simulation loop is
@@ -31,15 +34,15 @@
         This dictionary contains all parameters needed to set up a
         turboPy simulation. Each key describes a section, and the value
         is another dictionary with the needed parameters for that
         section.
 
         Expected keys are:
 
-        ``"Grid"``
+        ``"Grid"``, optional
             Dictionary containing parameters needed to define the grid.
             Currently only 1D grids are defined in turboPy.
 
             The expected parameters are:
 
             - ``"N"`` | {``"dr"`` | ``"dx"``} :
                 The number of grid points (`int`) | the grid spacing
@@ -89,18 +92,18 @@
 
             If the key is not found in the registry, then the key/value
             pair is interpreted as a default parameter value, and is
             added to dictionary of parameters for all of the
             :class:`Diagnostic` constructors.
 
             If the directory and filename keys are not specified,
-            default values are created in the 
+            default values are created in the
             :meth:`read_diagnostics_from_input` method.
-            The default name for the directory is "default_output" and 
-            the default filename is the name of the Diagnostic subclass 
+            The default name for the directory is "default_output" and
+            the default filename is the name of the Diagnostic subclass
             followed by a number.
 
         ``"Tools"`` : `dict` [`str`, `dict`], optional
             Dictionary of :class:`ComputeTool` items needed for the
             simulation.
 
             Each key in the dictionary should map to a
@@ -127,14 +130,20 @@
 
         self.grid = None
         self.clock = None
         self.units = None
 
         self.input_data = input_data
 
+        self.all_shared_resources = {}
+
+        # set default values for optional
+        self.input_data.setdefault('Tools', {})
+        self.input_data.setdefault('Diagnostics', {})
+
     def run(self):
         """
         Runs the simulation
 
         This initializes the simulation, runs the main loop, and then
         finalizes the simulation.
         """
@@ -165,17 +174,21 @@
         self.clock.advance()
 
     def prepare_simulation(self):
         """
         Prepares the simulation by reading the input and initializing
         physics modules and diagnostics.
         """
-        print("Reading Grid...")
-        self.read_grid_from_input()
-        
+        if 'Grid' in self.input_data:
+            print("Reading Grid...")
+            self.read_grid_from_input()
+        else:
+            warnings.warn('No Grid Found.')
+            print("Initializing Gridless Simulation...")
+
         print("Initializing Simulation Clock...")
         self.read_clock_from_input()
 
         print("Reading Tools...")
         self.read_tools_from_input()
 
         print("Reading PhysicsModules...")
@@ -188,18 +201,22 @@
         for t in self.compute_tools:
             t.initialize()
 
         print("Initializing PhysicsModules...")
         for m in self.physics_modules:
             m.exchange_resources()
         for m in self.physics_modules:
+            m.inspect_resources()
+        for m in self.physics_modules:
             m.initialize()
 
         print("Initializing Diagnostics...")
         for d in self.diagnostics:
+            d.inspect_resources()
+        for d in self.diagnostics:
             d.initialize()
 
     def finalize_simulation(self):
         """
         Close out the simulation
 
         Runs the :class:`Diagnostic.finalize()` method for each
@@ -214,96 +231,109 @@
 
     def read_clock_from_input(self):
         """Construct the clock based on input parameters"""
         self.clock = SimulationClock(self, self.input_data["Clock"])
 
     def read_tools_from_input(self):
         """Construct :class:`ComputeTools` based on input"""
-        if "Tools" in self.input_data:
-            for tool_name, params in self.input_data["Tools"].items():
-                tool_class = ComputeTool.lookup(tool_name)
-                if not isinstance(params, list):
-                    params = [params]
-                for tool in params:
-                    tool["type"] = tool_name
-                    self.compute_tools.append(tool_class(owner=self, 
-                                                         input_data=tool)) 
-    
+        for tool_name, params in self.input_data["Tools"].items():
+            tool_class = ComputeTool.lookup(tool_name)
+            if not isinstance(params, list):
+                params = [params]
+            for tool in params:
+                tool["type"] = tool_name
+                self.compute_tools.append(tool_class(owner=self,
+                                                     input_data=tool))
+
     def read_modules_from_input(self):
         """Construct :class:`PhysicsModule` instances based on input"""
         for physics_module_name, physics_module_data in \
                 self.input_data["PhysicsModules"].items():
+            print(f"Loading physics module: {physics_module_name}...")
             physics_module_class = PhysicsModule.lookup(physics_module_name)
             physics_module_data["name"] = physics_module_name
             self.physics_modules.append(physics_module_class(
                 owner=self, input_data=physics_module_data))
         self.sort_modules()
 
     def read_diagnostics_from_input(self):
         """Construct :class:`Diagnostic` instances based on input"""
-        if "Diagnostics" in self.input_data:
-            # This dictionary has two types of keys:
-            #    keys that are valid diagnostic types
-            #    other keys, which should be passed along
-            #    as "default" parameters
-            diags = {k: v for k, v in
-                     self.input_data["Diagnostics"].items()
-                     if Diagnostic.is_valid_name(k)}
-            params = {k: v for k, v in
-                      self.input_data["Diagnostics"].items()
-                      if not Diagnostic.is_valid_name(k)}
-
-            if "directory" not in params:
-                params["directory"] = str(Path("default_output"))
-
-            for diag_type, d in diags.items():
-                diagnostic_class = Diagnostic.lookup(diag_type)
-                if not type(d) is list:
-                    d = [d]
-                file_num = 0
-                for di in d:
-                    # Values in di supersede values in params because
-                    # of the order in which these are combined
-                    di = {**params, **di, "type": diag_type}
-                    if "filename" not in di:
-                        # Set a default output filename
-                        file_end = di.get("output_type", "out")
-                        di["filename"] = (f"{diag_type}{file_num}"
+        diagnostics, default_params = self.parse_diagnostic_input_dictionary()
+
+        diagnostics = make_values_into_lists(diagnostics)
+        default_params.setdefault('directory', 'default_output')
+
+        for diag_type, list_of_diagnostics in diagnostics.items():
+            diagnostic_class = Diagnostic.lookup(diag_type)
+
+            file_num = 0
+            for params in list_of_diagnostics:
+                params['type'] = diag_type
+                params = self.combine_dictionaries(default_params, params)
+                if "filename" not in params:
+                    # Set a default output filename
+                    file_end = params.get("output_type", "out")
+                    params["filename"] = (f"{diag_type}{file_num}"
                                           f".{file_end}")
-                        file_num += 1
-                    di["filename"] = str(Path(di["directory"])
-                                         / Path(di["filename"]))
-                    self.diagnostics.append(
-                        diagnostic_class(owner=self, input_data=di))
+                    file_num += 1
+                params["filename"] = str(Path(params["directory"])
+                                         / Path(params["filename"]))
+                self.diagnostics.append(
+                    diagnostic_class(owner=self, input_data=params))
+
+    def combine_dictionaries(self, defaults, custom):
+        # Values in "custom" dictionary supersede "defaults" because of
+        # the order in which they are combined here
+        return {**defaults, **custom}
+
+    def parse_diagnostic_input_dictionary(self):
+        # The input_data["Diagnostics"] dictionary has two types of keys:
+        #    1) keys that are valid diagnostic types
+        #    2) other keys, which should be passed along
+        #    as "default" parameters
+        diagnostics = {k: v for k, v in
+                       self.input_data["Diagnostics"].items()
+                       if Diagnostic.is_valid_name(k)}
+        default_params = {k: v for k, v in
+                          self.input_data["Diagnostics"].items()
+                          if not Diagnostic.is_valid_name(k)}
+        return diagnostics, default_params
 
     def sort_modules(self):
         """Sort :class:`Simulation.physics_modules` by some logic
 
         Unused stub for future implementation"""
         pass
 
     def find_tool_by_name(self, tool_name: str, custom_name: str = None):
         """Returns the :class:`ComputeTool` associated with the
         given name"""
-        tools = [t for t in self.compute_tools if t.name == tool_name 
+        tools = [t for t in self.compute_tools if t.name == tool_name
                  and t.custom_name == custom_name]
         if len(tools) == 1:
             return tools[0]
         return None
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.input_data})"
 
+    def gather_shared_resources(self, shared):
+        for k, v in shared.items():
+            if k in self.all_shared_resources:
+                warnings.warn(f'Shared resource {k} has been overwritten')
+            self.all_shared_resources[k] = v
+
 
 class DynamicFactory(ABC):
     """Abstract class which provides dynamic factory functionality
 
     This base class provides a dynamic factory pattern functionality to
     classes that derive from this.
     """
+
     @property
     @abstractmethod
     def _factory_type_name(self):
         """Override this in derived classes with a string that
         describes type of the derived factory"""
         pass
 
@@ -371,14 +401,25 @@
     _input_data : `dict`
        Dictionary that contains user defined parameters about this
        object such as its name.
     _registry : `dict`
         Registered derived ComputeTool classes.
     _factory_type_name : `str`
         Type of PhysicsModule child class.
+    _needed_resources: `dict`
+        Dictionary that lists shared resources that this module
+        needs. Format is `{shared_key: variable_name}`, where
+        `shared_key` is a string with the name of needed resource,
+        and `variable_name` is a string to use when saving this
+        variable. For example: {"Fields:E": "E"} will make `self.E`.
+    _resources_to_share: `dict`
+        Dictionary that lists shared resources that this module
+        is sharing to others. Format is `{shared_key: variable}`, where
+        `shared_key` is a string with the name of resource to share,
+        and `variable` is the data to be shared.
 
     Notes
     -----
     This class is based on Module class in TurboWAVE.
     Because python mutable/immutable is different than C++ pointers, the
     implementation here is different. Here, a "resource" is a
     dictionary, and can have more than one thing being shared. Note that
@@ -390,55 +431,91 @@
     _registry = {}
 
     def __init__(self, owner: Simulation, input_data: dict):
         self._owner = owner
         self._module_type = None
         self._input_data = input_data
 
+        # By default, share "public" attributes
+        shared = {f'{self.__class__.__name__}_{attribute}': value
+                  for attribute, value
+                  in self.__dict__.items()
+                  if not attribute.startswith('_')}
+        self._resources_to_share = shared
+
+        # Items should have key "shared_name", and value is the variable
+        # name for the "pointer".
+        # For example: {"Fields:E": "E"} will make self.E
+        self._needed_resources = {}
+
     def publish_resource(self, resource: dict):
-        """
-        Method which implements the details of sharing resources
+        """**Deprecated**
+
+        *This method is only here for backwards compatability. New
+        code should use the ``_resources_to_share`` dictionary.*
 
+        Method which implements the details of sharing resources
         Parameters
         ----------
         resource : `dict`
             resource dictionary to be shared
         """
+        warnings.warn("The resource-sharing API has changed. "
+                      "Add to `self._resources_to_share` instead of "
+                      "calling `publish_resource`.",
+                      DeprecationWarning)
+        for k in resource.keys():
+            print(f"Module {self.__class__.__name__} is sharing {k}")
         for physics_module in self._owner.physics_modules:
             physics_module.inspect_resource(resource)
         for diagnostic in self._owner.diagnostics:
             diagnostic.inspect_resource(resource)
 
     def inspect_resource(self, resource: dict):
-        """Method for accepting resources shared by other PhysicsModules
+        """**Deprecated**
+
+        *This method is only here for backwards compatability. New
+        code should use the ``_needed_resources`` dictionary.*
+
+        Method for accepting resources shared by other PhysicsModules
         If your subclass needs the data described by the key, now's
         their chance to save a pointer to the data.
-
         Parameters
         ----------
         resource : `dict`
             resource dictionary to be shared
         """
         pass
 
+    def inspect_resources(self):
+        for shared_name, var_name in self._needed_resources.items():
+            if shared_name not in self._owner.all_shared_resources:
+                warnings.warn(f"Module {self.__class__.__name__} can't find "
+                              f"needed resource {shared_name}")
+            else:
+                self.__dict__[var_name] = self._owner.all_shared_resources[
+                                              shared_name
+                                          ]
+
     def exchange_resources(self):
         """Main method for sharing resources with other
         :class:`PhysicsModule` objects.
 
         This is the function where you call :meth:`publish_resource`,
         to tell other physics modules about data you want to share.
 
         By default, any "public" attributes (those with names that do
         not start with an underscore) will be shared with the key
         `<class_name>_<attribute_name>`.
         """
-        shared = {f'{self.__class__}_{attribute}': value for attribute, value
-                  in self.__dict__.items()
-                  if not attribute.startswith('_')}
-        self.publish_resource(shared)
+
+        for k in self._resources_to_share.keys():
+            print(f"Module {self.__class__.__name__} is sharing {k}")
+
+        self._owner.gather_shared_resources(self._resources_to_share)
 
     def update(self):
         """Do the main work of the :class:`PhysicsModule`
 
         This is called at every time step in the main loop.
         """
         raise NotImplementedError
@@ -488,15 +565,15 @@
     _input_data : `dict`
         Dictionary that contains user defined parameters about this
         object such as its name.
     name : `str`
         Type of ComputeTool.
     custom_name: `str`
         Name given to individual instance of tool, optional.
-        Used when multiple tools of the same type exist in one 
+        Used when multiple tools of the same type exist in one
         :class:`Simulation`.
     """
 
     _factory_type_name = "Compute Tool"
     _registry = {}
 
     def __init__(self, owner: Simulation, input_data: dict):
@@ -542,15 +619,15 @@
     Attributes
     ----------
     _owner : :class:`Simulation`
         Simulation class that SimulationClock belongs to.
     _input_data : `dict`
         Dictionary of parameters needed to define the simulation
         clock.
-    
+
     start_time : `float`
         Clock start time.
     time : `float`
         Current time on clock.
     end_time : `float`
         Clock end time.
     this_step : `int`
@@ -573,37 +650,37 @@
         self.print_time = False
         if "print_time" in input_data:
             self.print_time = input_data["print_time"]
 
         if "num_steps" in input_data:
             self.num_steps = input_data["num_steps"]
             self.dt = (
-                (input_data["end_time"] - input_data["start_time"])
-                / input_data["num_steps"])
+                    (input_data["end_time"] - input_data["start_time"])
+                    / input_data["num_steps"])
         elif "dt" in input_data:
             self.dt = input_data["dt"]
             self.num_steps = (self.end_time - self.start_time) / self.dt
             if not np.isclose(self.num_steps, np.rint(self.num_steps)):
                 raise RuntimeError("Simulation interval is not an "
                                    "integer multiple of timestep dt")
-            self.num_steps = np.int(np.rint(self.num_steps))
+            self.num_steps = np.int64(np.rint(self.num_steps))
 
     def advance(self):
         """Increment the time"""
         self.this_step += 1
         self.time = self.start_time + self.dt * self.this_step
         if self.print_time:
-            print(f"t = {self.time}")
-    
+            print(f"t = {self.time:0.4e}")
+
     def turn_back(self, num_steps=1):
         """Set the time back `num_steps` time steps"""
         self.this_step = self.this_step - num_steps
         self.time = self.start_time + self.dt * self.this_step
         if self.print_time:
-            print(f"t = {self.time}")        
+            print(f"t = {self.time}")
 
     def is_running(self):
         """Check if time is less than end time"""
         return self.this_step < self.num_steps
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._input_data})"
@@ -647,14 +724,15 @@
         Value of the coordinate in the middle of each Grid cell.
     cell_widths : :class:`numpy.ndarray`
         Width of each cell in the Grid.
     r_inv : `float`
         Inverse of coordinate values at each Grid point,
         1/:class:`Grid.r`.
     """
+
     def __init__(self, input_data: dict):
         self._input_data = input_data
         self.r_min = None
         self.r_max = None
         self.num_points = None
         self.dr = None
         self.coordinate_system = "cartesian"
@@ -693,15 +771,15 @@
         else:
             self.set_value_from_keys("dr", {"dr", "dx"})
             self.num_points = 1 + (self.r_max - self.r_min) / self.dr
             if not self.num_points % 1 == 0:
                 raise (RuntimeError("Invalid grid spacing: "
                                     "configuration does not imply "
                                     "integer number of grid points"))
-            self.num_points = np.int(self.num_points)
+            self.num_points = np.int64(self.num_points)
 
         # set the coordinate system
         if "coordinate_system" in self._input_data:
             self.coordinate_system = self._input_data["coordinate_system"]
         self.coordinate_system = self.coordinate_system.lower().strip()
 
     def set_value_from_keys(self, var_name, options):
@@ -794,15 +872,15 @@
         assert (r0 >= self.r_min), "Requested point is not in the grid"
         assert (r0 <= self.r_max), "Requested point is not in the grid"
         i, = np.where((r0 - self.dr < self.r) & (self.r < r0 + self.dr))
         assert (len(i) in [1, 2]), ("Error finding requested point"
                                     "in the grid")
         if len(i) == 1:
             return lambda y: y[i]
-        if len(i) == 2:
+        else:
             # linearly interpolate
             def interpval(yvec):
                 """A function which takes a grid quantity ``y`` and
                 returns the interpolated value of ``y`` at the
                 point ``r0``.
 
                 Parameters
@@ -836,25 +914,25 @@
         else:
             raise ValueError(f'Coordinate system '
                              f'{self.coordinate_system} is undefined')
         self.set_interface_volumes()
 
     def set_cartesian_volumes(self):
         self.cell_volumes = self.cell_edges[1:] - self.cell_edges[:-1]
-        self.inverse_cell_volumes = 1./self.cell_volumes
+        self.inverse_cell_volumes = 1. / self.cell_volumes
 
     def set_cylindrical_volumes(self):
         scratch = self.cell_edges ** 2
         self.cell_volumes = np.pi * (scratch[1:] - scratch[:-1])
-        self.inverse_cell_volumes = 1./self.cell_volumes
+        self.inverse_cell_volumes = 1. / self.cell_volumes
 
     def set_spherical_volumes(self):
         scratch = self.cell_edges ** 3
-        self.cell_volumes = 4/3 * np.pi * (scratch[1:] - scratch[:-1])
-        self.inverse_cell_volumes = 1./self.cell_volumes
+        self.cell_volumes = 4 / 3 * np.pi * (scratch[1:] - scratch[:-1])
+        self.inverse_cell_volumes = 1. / self.cell_volumes
 
     def set_cartesian_areas(self):
         self.interface_areas = np.ones_like(self.cell_edges)
 
     def set_cylindrical_areas(self):
         self.interface_areas = 2.0 * np.pi * self.cell_edges
 
@@ -867,16 +945,16 @@
 
         self.interface_volumes[0] = self.cell_volumes[0]
         self.interface_volumes[1:-1] = 0.5 * (self.cell_volumes[1:]
                                               + self.cell_volumes[0:-1])
         self.interface_volumes[-1] = self.cell_volumes[-1]
 
         self.inverse_interface_volumes[0] = self.inverse_cell_volumes[0]
-        self.inverse_interface_volumes[1:-1] = 0.5 * (self.inverse_cell_volumes[1:]
-                                                      + self.inverse_cell_volumes[0:-1])
+        self.inverse_interface_volumes[1:-1] = 0.5 * \
+            (self.inverse_cell_volumes[1:] + self.inverse_cell_volumes[0:-1])
         self.inverse_interface_volumes[-1] = self.inverse_cell_volumes[-1]
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._input_data})"
 
 
 class Diagnostic(DynamicFactory):
@@ -897,37 +975,61 @@
     _registry: `dict`
         Registered derived Diagnostic classes
     _owner: Simulation
         The Simulation object that contains this object
     _input_data: `dict`
         Dictionary that contains user defined parameters about this
         object such as its name.
+    _needed_resources: `dict`
+        Dictionary that lists shared resources that this module
+        needs. Format is `{shared_key: variable_name}`, where
+        `shared_key` is a string with the name of needed resource,
+        and `variable_name` is a string to use when saving this
+        variable. For example: {"Fields:E": "E"} will make `self.E`.
     """
 
     _factory_type_name = "Diagnostic"
     _registry = {}
 
     def __init__(self, owner: Simulation, input_data: dict):
         self._owner = owner
         self._input_data = input_data
 
+        # Items should have key "shared_name", and value is the variable
+        # name for the "pointer"
+        # For example: {"Fields:E": "E"} will make self.E
+        self._needed_resources = {}
+
     def inspect_resource(self, resource: dict):
-        """Save references to data from other PhysicsModules
+        """**Deprecated**
 
+        *This method is only here for backwards compatability. New
+        code should use the ``_needed_resources`` dictionary.*
+
+        Save references to data from other PhysicsModules
         If your subclass needs the data described by the key, now's
         their chance to save a reference to the data
-
         Parameters
         ----------
         resource: `dict`
             A dictionary containing references to data shared by other
             PhysicsModules.
         """
         pass
 
+    def inspect_resources(self):
+        for shared_name, var_name in self._needed_resources.items():
+            if shared_name not in self._owner.all_shared_resources:
+                warnings.warn(f"Diagnostic {self.__class__.__name__} can't "
+                              f"find needed resource {shared_name}")
+            else:
+                self.__dict__[var_name] = self._owner.all_shared_resources[
+                                              shared_name
+                                          ]
+
     def diagnose(self):
         """Perform diagnostic step
 
         This gets called on every step of the main simulation loop.
 
         Raises
         ------
@@ -955,7 +1057,18 @@
         This gets called once after the main simulation loop is
         complete.
         """
         pass
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self._input_data})"
+
+
+def wrap_item_in_list(item):
+    if type(item) is list:
+        return item
+    else:
+        return [item]
+
+
+def make_values_into_lists(dictionary):
+    return {k: wrap_item_in_list(v) for k, v in dictionary.items()}
```

### Comparing `turbopy-2020.9.10/turbopy.egg-info/SOURCES.txt` & `turbopy-2023.6.9/turbopy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

