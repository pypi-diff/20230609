# Comparing `tmp/vstt-0.29.0.tar.gz` & `tmp/vstt-0.30.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstt-0.29.0.tar", last modified: Wed Jun  7 12:11:58 2023, max compression
+gzip compressed data, was "vstt-0.30.0.tar", last modified: Fri Jun  9 13:19:24 2023, max compression
```

## Comparing `vstt-0.29.0.tar` & `vstt-0.30.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.959209 vstt-0.29.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-07 12:11:42.000000 vstt-0.29.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-07 12:11:58.959209 vstt-0.29.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-07 12:11:42.000000 vstt-0.29.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-07 12:11:42.000000 vstt-0.29.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 12:11:58.963209 vstt-0.29.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.951209 vstt-0.29.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.955209 vstt-0.29.0/src/vstt/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)    15227 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12942 2023-06-07 12:11:42.000000 vstt-0.29.0/src/vstt/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.955209 vstt-0.29.0/src/vstt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 12:11:58.000000 vstt-0.29.0/src/vstt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 12:11:58.959209 vstt-0.29.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_display.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_display_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_joystick_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_meta_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_results_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_trials_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-07 12:11:42.000000 vstt-0.29.0/tests/test_vstt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-09 13:19:15.000000 vstt-0.30.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 13:19:24.887920 vstt-0.30.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-09 13:19:15.000000 vstt-0.30.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-09 13:19:15.000000 vstt-0.30.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:19:24.887920 vstt-0.30.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.883920 vstt-0.30.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/src/vstt/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14458 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16330 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-09 13:19:15.000000 vstt-0.30.0/src/vstt/vtypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/src/vstt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 13:19:24.000000 vstt-0.30.0/src/vstt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:19:24.887920 vstt-0.30.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_display_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9067 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_joystick_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_meta_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_results_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10212 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9666 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_trials_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12342 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 13:19:15.000000 vstt-0.30.0/tests/test_vstt.py
```

### Comparing `vstt-0.29.0/LICENSE` & `vstt-0.30.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/PKG-INFO` & `vstt-0.30.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.29.0
+Version: 0.30.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.29.0/README.md` & `vstt-0.30.0/README.md`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/pyproject.toml` & `vstt-0.30.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/__main__.py` & `vstt-0.30.0/src/vstt/__main__.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/common.py` & `vstt-0.30.0/src/vstt/common.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import copy
 import logging
 from typing import Any
 from typing import Mapping
 from typing import Type
 from typing import TypeVar
 
-from vstt.types import DisplayOptions
-from vstt.types import Metadata
-from vstt.types import Trial
+from vstt.vtypes import DisplayOptions
+from vstt.vtypes import Metadata
+from vstt.vtypes import Trial
 
 VsttTypedDict = TypeVar(
     "VsttTypedDict",
     Trial,
     Metadata,
     DisplayOptions,
 )
```

### Comparing `vstt-0.29.0/src/vstt/display.py` & `vstt-0.30.0/src/vstt/display.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Dict
 
 import vstt
 
 
-def default_display_options() -> vstt.types.DisplayOptions:
+def default_display_options() -> vstt.vtypes.DisplayOptions:
     return {
         "to_target_paths": True,
         "to_center_paths": False,
         "targets": True,
         "central_target": True,
         "to_target_reaction_time": True,
         "to_center_reaction_time": False,
@@ -41,11 +41,11 @@
         "to_center_distance": "Statistic: movement distance to center",
         "to_target_rmse": "Statistic: RMSE movement to target",
         "to_center_rmse": "Statistic: RMSE movement to center",
         "averages": "Also show statistics averaged over all targets",
     }
 
 
-def import_display_options(display_options_dict: dict) -> vstt.types.DisplayOptions:
+def import_display_options(display_options_dict: dict) -> vstt.vtypes.DisplayOptions:
     return vstt.common.import_typed_dict(
         display_options_dict, default_display_options()
     )
```

### Comparing `vstt-0.29.0/src/vstt/display_widget.py` & `vstt-0.30.0/src/vstt/display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/experiment.py` & `vstt-0.30.0/src/vstt/experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 import pandas as pd
 from psychopy.data import TrialHandlerExt
 from psychopy.misc import fromFile
 from vstt.display import default_display_options
 from vstt.display import import_display_options
 from vstt.meta import default_metadata
 from vstt.meta import import_metadata
-from vstt.stat import append_stats_data_to_excel
-from vstt.stat import stats_dataframe
+from vstt.stats import append_stats_data_to_excel
+from vstt.stats import stats_dataframe
 from vstt.trial import default_trial
 from vstt.trial import import_and_validate_trial
 
 
 class Experiment:
     def __init__(self, filename: Optional[str] = None):
         self.filename = "default-experiment.psydat"
```

### Comparing `vstt-0.29.0/src/vstt/geom.py` & `vstt-0.30.0/src/vstt/geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/gui.py` & `vstt-0.30.0/src/vstt/gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/joystick_wrapper.py` & `vstt-0.30.0/src/vstt/joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/meta.py` & `vstt-0.30.0/src/vstt/meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Dict
 
 import vstt
 
 
-def default_metadata() -> vstt.types.Metadata:
+def default_metadata() -> vstt.vtypes.Metadata:
     return {
         "name": "Experiment",
         "subject": "Joe Smith",
         "date": "2022/01/01",
         "author": "Author",
         "display_title": "Welcome to the experiment",
         "display_text1": "When a target is presented the target circle will turn red.",
@@ -37,9 +37,9 @@
         "display_text4": "Main text line 4",
         "display_duration": "Display duration (seconds)",
         "show_delay_countdown": "Display a countdown",
         "enter_to_skip_delay": "Skip by pressing enter key",
     }
 
 
-def import_metadata(metadata_dict: dict) -> vstt.types.Metadata:
+def import_metadata(metadata_dict: dict) -> vstt.vtypes.Metadata:
     return vstt.common.import_typed_dict(metadata_dict, default_metadata())
```

### Comparing `vstt-0.29.0/src/vstt/meta_widget.py` & `vstt-0.30.0/src/vstt/meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/results_widget.py` & `vstt-0.30.0/src/vstt/results_widget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from __future__ import annotations
 
+from typing import List
 from typing import Optional
 
+import numpy as np
 from psychopy.visual.window import Window
 from PyQt5 import QtWidgets
 from vstt.experiment import Experiment
 from vstt.vis import display_results
 
 
 class ResultsWidget(QtWidgets.QWidget):
@@ -17,14 +19,15 @@
         self._experiment = Experiment()
 
         outer_layout = QtWidgets.QVBoxLayout()
         group_box = QtWidgets.QGroupBox("Results")
         outer_layout.addWidget(group_box)
         inner_layout = QtWidgets.QGridLayout()
         group_box.setLayout(inner_layout)
+        self._list_trial_row_to_trial_index: List[int] = []
         self._list_trials = QtWidgets.QListWidget()
         self._list_trials.currentRowChanged.connect(self._row_changed)
         self._list_trials.itemDoubleClicked.connect(self._btn_display_trial_clicked)
         inner_layout.addWidget(self._list_trials, 0, 0, 1, 2)
         self._btn_display_trial = QtWidgets.QPushButton("Display Trial")
         self._btn_display_trial.clicked.connect(self._btn_display_trial_clicked)
         inner_layout.addWidget(self._btn_display_trial, 1, 0)
@@ -58,15 +61,15 @@
             return
         display_results(
             60,
             True,
             False,
             self._experiment.trial_handler_with_results,
             self._experiment.display_options,
-            row,
+            self._list_trial_row_to_trial_index[row],
             all_trials_for_this_condition,
             win=self._win,
         )
 
     def _btn_display_trial_clicked(self) -> None:
         self._display_results(False)
 
@@ -76,18 +79,24 @@
     @property
     def experiment(self) -> Experiment:
         return self._experiment
 
     @experiment.setter
     def experiment(self, experiment: Experiment) -> None:
         self._list_trials.clear()
+        self._list_trial_row_to_trial_index.clear()
         self._experiment = experiment
-        if experiment.trial_handler_with_results is None:
+        trial_handler = experiment.trial_handler_with_results
+        if trial_handler is None:
             return
         # assume 1 repetition of experiment
         rep_index = 0
-        for trial_index, condition_index in enumerate(
-            experiment.trial_handler_with_results.sequenceIndices
-        ):
-            self._list_trials.addItem(
-                f"Trial {trial_index} [Condition {condition_index[rep_index]}]"
-            )
+        for trial_index, condition_index in enumerate(trial_handler.sequenceIndices):
+            # trials that have no data have a default string instead of a numpy array
+            if (
+                type(trial_handler.data["target_indices"][(trial_index, rep_index)])
+                is np.ndarray
+            ):
+                self._list_trials.addItem(
+                    f"Trial {trial_index} [Condition {condition_index[rep_index]}]"
+                )
+                self._list_trial_row_to_trial_index.append(trial_index)
```

### Comparing `vstt-0.29.0/src/vstt/stat.py` & `vstt-0.30.0/src/vstt/stats.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/task.py` & `vstt-0.30.0/src/vstt/task.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from psychopy.visual.window import Window
 from vstt import joystick_wrapper
 from vstt import vis
 from vstt.experiment import Experiment
 from vstt.geom import JoystickPointUpdater
 from vstt.geom import PointRotator
 from vstt.geom import to_target_dists
-from vstt.stat import stats_dataframe
+from vstt.stats import stats_dataframe
 
 
 def _get_target_indices(outer_target_index: int, trial: Dict[str, Any]) -> List[int]:
     # always include outer target index
     indices = [outer_target_index]
     if trial["add_central_target"] and not trial["automove_cursor_to_center"]:
         # add central target index
@@ -156,73 +156,90 @@
             raise
 
     def _do_trials(self) -> None:
         self._do_splash_screen()
         condition_trial_indices: List[List[int]] = [
             [] for _ in self.trial_handler.trialList
         ]
+        current_condition_index = -1
+        current_condition_first_trial_index = 0
+        current_condition_clock = Clock()
+        current_condition_max_time = 0.0
         for trial in self.trial_handler:
-            self._do_trial(trial, condition_trial_indices)
+            if self.trial_handler.thisIndex != current_condition_index:
+                # starting a new set of conditions
+                current_condition_clock.reset()
+                current_condition_max_time = trial["condition_timeout"]
+                current_condition_index = self.trial_handler.thisIndex
+                current_condition_first_trial_index = self.trial_handler.thisTrialN
+            condition_trial_indices[self.trial_handler.thisIndex].append(
+                self.trial_handler.thisTrialN
+            )
+            if (
+                current_condition_max_time == 0.0
+                or current_condition_clock.getTime() < current_condition_max_time
+            ):
+                # only do the trial if there is still time left for this condition
+                self._do_trial(trial)
+            is_final_trial_of_block = (
+                len(condition_trial_indices[self.trial_handler.thisIndex])
+                == trial["weight"]
+            )
+            if is_final_trial_of_block and trial["post_block_delay"] > 0:
+                vis.display_results(
+                    trial["post_block_delay"],
+                    trial["enter_to_skip_delay"],
+                    trial["show_delay_countdown"],
+                    self.trial_handler if trial["post_block_display_results"] else None,
+                    self.experiment.display_options,
+                    current_condition_first_trial_index,
+                    True,
+                    self.win,
+                )
         if self.win.nDroppedFrames > 0:
             logging.warning(f"Dropped {self.win.nDroppedFrames} frames")
 
     def _do_splash_screen(self) -> None:
         vis.splash_screen(
             display_time_seconds=self.experiment.metadata["display_duration"],
             enter_to_skip_delay=self.experiment.metadata["enter_to_skip_delay"],
             show_delay_countdown=self.experiment.metadata["show_delay_countdown"],
             metadata=self.experiment.metadata,
             win=self.win,
         )
 
-    def _do_trial(
-        self, trial: Dict[str, Any], condition_trial_indices: List[List[int]]
-    ) -> None:
+    def _do_trial(self, trial: Dict[str, Any]) -> None:
         if trial["use_joystick"] and self.js is None:
             raise RuntimeError("Use joystick option is enabled, but no joystick found.")
-        tom = TrialManager(self.win, trial, self.rng)
-        condition_trial_indices[self.trial_handler.thisIndex].append(
-            self.trial_handler.thisTrialN
-        )
-        is_final_trial_of_block = (
-            len(condition_trial_indices[self.trial_handler.thisIndex])
-            == trial["weight"]
-        )
-        self.mouse.setPos(tom.cursor.pos)
+        tm = TrialManager(self.win, trial, self.rng)
+        self.mouse.setPos(tm.cursor.pos)
         self.win.recordFrameIntervals = True
-        tom.clock.reset()
-        for index in tom.data.target_indices:
-            self._do_target(trial, index, tom)
+        tm.clock.reset()
+        vis.update_target_colors(tm.targets, trial["show_inactive_targets"], None)
+        if trial["show_target_labels"]:
+            vis.update_target_label_colors(
+                tm.target_labels, trial["show_inactive_targets"], None
+            )
+        for index in tm.data.target_indices:
+            self._do_target(trial, index, tm)
         self.win.recordFrameIntervals = False
-
         if trial["automove_cursor_to_center"]:
-            tom.data.to_center_success = [True] * trial["num_targets"]
-        add_trial_data_to_trial_handler(tom.data, self.trial_handler)
+            tm.data.to_center_success = [True] * trial["num_targets"]
+        add_trial_data_to_trial_handler(tm.data, self.trial_handler)
         if trial["post_trial_delay"] > 0:
             vis.display_results(
                 trial["post_trial_delay"],
                 trial["enter_to_skip_delay"],
                 trial["show_delay_countdown"],
                 self.trial_handler if trial["post_trial_display_results"] else None,
                 self.experiment.display_options,
                 self.trial_handler.thisTrialN,
                 False,
                 self.win,
             )
-        if is_final_trial_of_block and trial["post_block_delay"] > 0:
-            vis.display_results(
-                trial["post_block_delay"],
-                trial["enter_to_skip_delay"],
-                trial["show_delay_countdown"],
-                self.trial_handler if trial["post_block_display_results"] else None,
-                self.experiment.display_options,
-                self.trial_handler.thisTrialN,
-                True,
-                self.win,
-            )
 
     def _do_target(self, trial: Dict[str, Any], index: int, tm: TrialManager) -> None:
         minimum_window_for_flip = 1.0 / 60.0
         mouse_pos = tm.cursor.pos
         stop_waiting_time = 0.0
         stop_target_time = 0.0
         if trial["fixed_target_intervals"]:
@@ -239,22 +256,22 @@
                     mouse_pos = np.array([0.0, 0.0])
                     self.mouse.setPos(mouse_pos)
                     tm.cursor.setPos(mouse_pos)
                 tm.cursor_path_add_vertex(mouse_pos, clear_existing=True)
                 if not trial["fixed_target_intervals"]:
                     stop_waiting_time = t0 + trial["inter_target_duration"]
                 if stop_waiting_time > t0:
-                    # no target displayed
-                    vis.update_target_colors(
-                        tm.targets, trial["show_inactive_targets"], None
-                    )
-                    if trial["show_target_labels"]:
-                        vis.update_target_label_colors(
-                            tm.target_labels, trial["show_inactive_targets"], None
+                    if trial["hide_target_when_reached"]:
+                        vis.update_target_colors(
+                            tm.targets, trial["show_inactive_targets"], None
                         )
+                        if trial["show_target_labels"]:
+                            vis.update_target_label_colors(
+                                tm.target_labels, trial["show_inactive_targets"], None
+                            )
                     # ensure we get at least a single flip
                     should_continue_waiting = True
                     while should_continue_waiting:
                         if trial["freeze_cursor_between_targets"]:
                             self.mouse.setPos(mouse_pos)
                         vis.draw_and_flip(self.win, tm.drawables, self.kb)
                         if not trial["freeze_cursor_between_targets"]:
```

### Comparing `vstt-0.29.0/src/vstt/trial.py` & `vstt-0.30.0/src/vstt/trial.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 from typing import List
 from typing import Mapping
 from typing import Optional
 
 import numpy as np
 from psychopy.gui import DlgFromDict
 from vstt.common import import_typed_dict
-from vstt.types import Trial
+from vstt.vtypes import Trial
 
 
 def describe_trial(trial: Trial) -> str:
     repeats = f"{trial['weight']} repeat{'s' if trial['weight'] > 1 else ''}"
     targets = f"target{'s' if trial['num_targets'] > 1 else ''}"
+    if trial["condition_timeout"] > 0.0:
+        repeats = f"up to {repeats}"
+        targets = f"{targets} in {trial['condition_timeout']}s"
     return f"{repeats} of {trial['num_targets']} {trial['target_order']} {targets}"
 
 
 def describe_trials(trials: List[Trial]) -> str:
     return "\n".join(["  - " + describe_trial(trial) for trial in trials])
 
 
 def default_trial() -> Trial:
     return {
         "weight": 1,
+        "condition_timeout": 0.0,
         "num_targets": 8,
         "target_order": "clockwise",
         "target_indices": "0 1 2 3 4 5 6 7",
         "add_central_target": True,
         "show_target_labels": False,
+        "hide_target_when_reached": True,
         "target_labels": "0 1 2 3 4 5 6 7",
         "fixed_target_intervals": False,
         "target_duration": 5.0,
         "central_target_duration": 5.0,
         "inter_target_duration": 1.0,
         "target_distance": 0.4,
         "target_size": 0.04,
@@ -58,19 +63,21 @@
         "enter_to_skip_delay": True,
     }
 
 
 def trial_labels() -> Dict:
     return {
         "weight": "Repetitions",
+        "condition_timeout": "Maximum time, 0=unlimited (secs)",
         "num_targets": "Number of targets",
         "target_order": "Target order",
         "target_indices": "Target indices",
         "add_central_target": "Add a central target",
         "show_target_labels": "Display target labels",
+        "hide_target_when_reached": "Hide target when reached",
         "target_labels": "Target labels",
         "fixed_target_intervals": "Fixed target display intervals",
         "target_duration": "Target display duration (secs)",
         "central_target_duration": "Central target display duration (secs)",
         "inter_target_duration": "Delay between targets (secs)",
         "target_distance": "Distance to targets (screen height fraction)",
         "target_size": "Target size (screen height fraction)",
@@ -115,14 +122,15 @@
     return import_and_validate_trial(trial)
 
 
 def import_and_validate_trial(trial_or_dict: Mapping[str, Any]) -> Trial:
     trial = import_typed_dict(trial_or_dict, default_trial())
     # make any negative time durations zero
     for duration in [
+        "condition_timeout",
         "target_duration",
         "central_target_duration",
         "inter_target_duration",
         "post_trial_delay",
         "post_block_delay",
     ]:
         if trial[duration] < 0.0:  # type: ignore
```

### Comparing `vstt-0.29.0/src/vstt/trials_widget.py` & `vstt-0.30.0/src/vstt/trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/src/vstt/types.py` & `vstt-0.30.0/src/vstt/vtypes.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
 
 class Trial(TypedDict):
     weight: int
+    condition_timeout: float
     num_targets: int
     target_order: Union[str, List]
     target_indices: str
     add_central_target: bool
     show_target_labels: bool
+    hide_target_when_reached: bool
     target_labels: str
     fixed_target_intervals: bool
     target_duration: float
     central_target_duration: float
     inter_target_duration: float
     target_distance: float
     target_size: float
```

### Comparing `vstt-0.29.0/src/vstt/update.py` & `vstt-0.30.0/src/vstt/update.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ver = version.parse(version_str)
     logging.info(f"  -> {ver}")
     return ver
 
 
 def check_for_new_version() -> Tuple[bool, str]:
     try:
-        current_version = version.parse(vstt.__version__)
+        current_version = version.Version(vstt.__version__)
         logging.info(f"Current version: {current_version}")
         latest_version = _get_latest_pypi_version()
         logging.info(f"Latest version: {latest_version}")
         if latest_version > current_version:
             return (
                 True,
                 f"Latest version of VSTT: {latest_version}.\nYou currently have version {current_version}.\nWould you like to upgrade now?",
```

### Comparing `vstt-0.29.0/src/vstt/vis.py` & `vstt-0.30.0/src/vstt/vis.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 from psychopy.visual.basevisual import BaseVisualStim
 from psychopy.visual.circle import Circle
 from psychopy.visual.elementarray import ElementArrayStim
 from psychopy.visual.shape import ShapeStim
 from psychopy.visual.textbox2 import TextBox2
 from psychopy.visual.window import Window
 from vstt.geom import points_on_circle
-from vstt.stat import list_dest_stat_label_units
-from vstt.stat import stats_dataframe
-from vstt.types import DisplayOptions
-from vstt.types import Metadata
+from vstt.stats import list_dest_stat_label_units
+from vstt.stats import stats_dataframe
+from vstt.vtypes import DisplayOptions
+from vstt.vtypes import Metadata
 
 colorNames.pop("none")
 colors = list(colorNames.values())
 
 
 def make_cursor(window: Window, cursor_size: float) -> ShapeStim:
     return ShapeStim(
```

### Comparing `vstt-0.29.0/src/vstt.egg-info/PKG-INFO` & `vstt-0.30.0/src/vstt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstt
-Version: 0.29.0
+Version: 0.30.0
 Summary: Visuomotor Serial Targeting Task (VSTT)
 Author-email: Liam Keegan <ssc@iwr.uni-heidelberg.de>
 License: MIT
 Project-URL: Github, https://github.com/ssciwr/vstt
 Project-URL: Issues, https://github.com/ssciwr/vstt/issues
 Project-URL: Documentation, https://vstt.readthedocs.io/
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `vstt-0.29.0/src/vstt.egg-info/SOURCES.txt` & `vstt-0.30.0/src/vstt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 src/vstt/experiment.py
 src/vstt/geom.py
 src/vstt/gui.py
 src/vstt/joystick_wrapper.py
 src/vstt/meta.py
 src/vstt/meta_widget.py
 src/vstt/results_widget.py
-src/vstt/stat.py
+src/vstt/stats.py
 src/vstt/task.py
 src/vstt/trial.py
 src/vstt/trials_widget.py
-src/vstt/types.py
 src/vstt/update.py
 src/vstt/vis.py
+src/vstt/vtypes.py
 src/vstt.egg-info/PKG-INFO
 src/vstt.egg-info/SOURCES.txt
 src/vstt.egg-info/dependency_links.txt
 src/vstt.egg-info/entry_points.txt
 src/vstt.egg-info/requires.txt
 src/vstt.egg-info/top_level.txt
 tests/test_common.py
@@ -33,14 +33,14 @@
 tests/test_experiment.py
 tests/test_geom.py
 tests/test_gui.py
 tests/test_joystick_wrapper.py
 tests/test_meta.py
 tests/test_meta_widget.py
 tests/test_results_widget.py
-tests/test_stat.py
+tests/test_stats.py
 tests/test_task.py
 tests/test_trial.py
 tests/test_trials_widget.py
 tests/test_update.py
 tests/test_vis.py
 tests/test_vstt.py
```

### Comparing `vstt-0.29.0/tests/test_display.py` & `vstt-0.30.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_display_widget.py` & `vstt-0.30.0/tests/test_display_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_experiment.py` & `vstt-0.30.0/tests/test_experiment.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_geom.py` & `vstt-0.30.0/tests/test_geom.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_gui.py` & `vstt-0.30.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_joystick_wrapper.py` & `vstt-0.30.0/tests/test_joystick_wrapper.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_meta.py` & `vstt-0.30.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_meta_widget.py` & `vstt-0.30.0/tests/test_meta_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_results_widget.py` & `vstt-0.30.0/tests/test_results_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_stat.py` & `vstt-0.30.0/tests/test_stats.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import numpy as np
 import vstt
 from vstt.experiment import Experiment
 
 
 def test_data_df(experiment_with_results: Experiment) -> None:
     # results from 3 reps of 8-target trial, 1 rep of 4-target trial with automove back to center
-    df = vstt.stat._data_df(experiment_with_results.trial_handler_with_results)
-    assert len(df.columns) == len(vstt.stat._get_trial_data_columns())
+    df = vstt.stats._data_df(experiment_with_results.trial_handler_with_results)
+    assert len(df.columns) == len(vstt.stats._get_trial_data_columns())
     for index, row in df.iterrows():
         assert row["to_target_mouse_positions"].shape[1] == 2
         assert (
             row["to_center_mouse_positions"].shape[0] == 0
             or row["to_center_mouse_positions"].shape[1] == 2
         )
         assert (
@@ -33,39 +33,39 @@
         assert np.allclose(
             df.loc[df.condition_index == i]["i_target"].unique(),
             list(range(targets[i])),
         )
 
 
 def test_stats_df(experiment_with_results: Experiment) -> None:
-    df = vstt.stat.stats_dataframe(experiment_with_results.trial_handler_with_results)
+    df = vstt.stats.stats_dataframe(experiment_with_results.trial_handler_with_results)
     assert np.alltrue(np.isnan(df.loc[df.condition_index == 1]["to_center_time"]))
-    for destination, stat_label_units in vstt.stat.list_dest_stat_label_units():
+    for destination, stat_label_units in vstt.stats.list_dest_stat_label_units():
         for stat, label, unit in stat_label_units:
             assert stat in df.columns
 
 
 def test_distance() -> None:
-    assert np.allclose(vstt.stat._distance(np.array([[0, 0]])), [0])
-    assert np.allclose(vstt.stat._distance(np.array([[3, 4]])), [0])
-    assert np.allclose(vstt.stat._distance(np.array([[0, 0], [1, 1]])), [np.sqrt(2)])
-    assert np.allclose(vstt.stat._distance(np.array([[1, 1], [0, 0]])), [np.sqrt(2)])
+    assert np.allclose(vstt.stats._distance(np.array([[0, 0]])), [0])
+    assert np.allclose(vstt.stats._distance(np.array([[3, 4]])), [0])
+    assert np.allclose(vstt.stats._distance(np.array([[0, 0], [1, 1]])), [np.sqrt(2)])
+    assert np.allclose(vstt.stats._distance(np.array([[1, 1], [0, 0]])), [np.sqrt(2)])
     assert np.allclose(
-        vstt.stat._distance(np.array([[0, 0], [1, 1], [0, 0]])), [2.0 * np.sqrt(2)]
+        vstt.stats._distance(np.array([[0, 0], [1, 1], [0, 0]])), [2.0 * np.sqrt(2)]
     )
     assert np.allclose(
-        vstt.stat._distance(np.array([[0, 0], [1, 1], [0, 0], [-1, -1]])),
+        vstt.stats._distance(np.array([[0, 0], [1, 1], [0, 0], [-1, -1]])),
         [3.0 * np.sqrt(2)],
     )
     assert np.allclose(
-        vstt.stat._distance(np.array([[0, 0], [1, 1], [0, 0], [-1, -1], [1, 1]])),
+        vstt.stats._distance(np.array([[0, 0], [1, 1], [0, 0], [-1, -1], [1, 1]])),
         [5.0 * np.sqrt(2)],
     )
     assert np.allclose(
-        vstt.stat._distance(np.array([[0, 0], [np.sqrt(2), np.sqrt(2)], [0, 0]])), [4]
+        vstt.stats._distance(np.array([[0, 0], [np.sqrt(2), np.sqrt(2)], [0, 0]])), [4]
     )
 
 
 def test_reaction_movement_time() -> None:
     for times in [
         [0.0, 0.1],
         [-1.0, -0.5],
@@ -75,40 +75,40 @@
     ]:
         n = len(times)
         for n_zeros in range(1, n):
             for n_before_visible in range(1, n):
                 positions = [[-1e-13, 1e-14]] * n_zeros + [[1, 1]] * (n - n_zeros)
                 reaction_time = times[n_zeros] - times[n_before_visible]
                 assert np.allclose(
-                    vstt.stat._reaction_time(
+                    vstt.stats._reaction_time(
                         np.array(times), np.array(positions), n_before_visible
                     ),
                     [reaction_time],
                 )
 
 
 def test_rmse() -> None:
     target = np.array([1, 1])
     # all points lie on the straight line between start and end point
-    assert np.allclose(vstt.stat._rmse(np.array([(0, 0), (1, 1)]), target), [0])
-    assert np.allclose(vstt.stat._rmse(np.array([(0, 0), (0.2, 0.2)]), target), [0])
+    assert np.allclose(vstt.stats._rmse(np.array([(0, 0), (1, 1)]), target), [0])
+    assert np.allclose(vstt.stats._rmse(np.array([(0, 0), (0.2, 0.2)]), target), [0])
     assert np.allclose(
-        vstt.stat._rmse(
+        vstt.stats._rmse(
             np.array([(0, 0), (0.25, 0.25), (0.5, 0.5), (0.75, 0.75)]), target
         ),
         [0],
     )
     # points which are all 1/sqrt(2) perpendicular distance from line
     assert np.allclose(
-        vstt.stat._rmse(np.array([(0, 0), (0, 1)]), target), [1.0 / np.sqrt(2.0)]
+        vstt.stats._rmse(np.array([(0, 0), (0, 1)]), target), [1.0 / np.sqrt(2.0)]
     )
     assert np.allclose(
-        vstt.stat._rmse(np.array([(0, 0), (1, 0)]), target), [1.0 / np.sqrt(2.0)]
+        vstt.stats._rmse(np.array([(0, 0), (1, 0)]), target), [1.0 / np.sqrt(2.0)]
     )
     assert np.allclose(
-        vstt.stat._rmse(np.array([(0, 0), (0, 1), (1, 0)]), target),
+        vstt.stats._rmse(np.array([(0, 0), (0, 1), (1, 0)]), target),
         [1.0 / np.sqrt(2.0)],
     )
     assert np.allclose(
-        vstt.stat._rmse(np.array([(0, 0), (0, 1), (1, 0), (0, 1), (1, 0)]), target),
+        vstt.stats._rmse(np.array([(0, 0), (0, 1), (1, 0), (0, 1), (1, 0)]), target),
         [1.0 / np.sqrt(2.0)],
     )
```

### Comparing `vstt-0.29.0/tests/test_task.py` & `vstt-0.30.0/tests/test_task.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import threading
+from copy import deepcopy
 from time import sleep
 from typing import Dict
 from typing import List
 from typing import Tuple
 
 import gui_test_utils as gtu
 import numpy as np
@@ -211,7 +212,44 @@
             abs(to_target_timestamps[0] - (count + 2) * target_duration)
             < allowed_error_on_timestamp
         )
         assert (
             abs(to_target_timestamps[-1] - (count + 3) * target_duration)
             < allowed_error_on_timestamp
         )
+
+
+def test_task_condition_timeout_no_user_input(window: Window) -> None:
+    # 4 seconds condition timeout where each trial has 1 target which is displayed for up to 2.1 seconds
+    # trial runs as long as it starts within the timeout -> should get 2 trials
+    experiment = Experiment()
+    experiment.metadata["display_duration"] = 0.0
+    trial1 = vstt.trial.default_trial()
+    trial1["weight"] = 100
+    trial1["condition_timeout"] = 4.0
+    trial1["num_targets"] = 1
+    trial1["target_duration"] = 2.1
+    trial1["inter_target_duration"] = 0.0
+    trial1["add_central_target"] = False
+    trial1["automove_cursor_to_center"] = False
+    trial1["freeze_cursor_between_targets"] = False
+    trial1["post_block_delay"] = 0.0
+    trial1["play_sound"] = False
+    # then a second copy but with 3 targets, each for 0.4 seconds, and a 1-second condition timeout -> single trial
+    trial2 = deepcopy(trial1)
+    trial2["condition_timeout"] = 1.0
+    trial2["num_targets"] = 3
+    trial2["target_duration"] = 0.4
+    experiment.trial_list = [trial1, trial2]
+    assert experiment.trial_handler_with_results is None
+    task = vstt.task.MotorTask(experiment, window)
+    # run task without moving mouse, which will stay in center for entire experiment
+    assert task.run() is True
+    # task ran successfully, updated experiment with results
+    assert experiment.has_unsaved_changes is True
+    assert experiment.trial_handler_with_results is not None
+    # we should get exactly 3 trials (as long as first flip on first trial has <4sec delay!)
+    assert len(experiment.stats.i_trial.unique()) == 3
+    # first two trials have 1 target, last trial has 3 targets -> 5 targets total
+    assert len(experiment.stats.to_target_success) == 5
+    # all targets should have been missed
+    assert np.all(~experiment.stats.to_target_success)
```

### Comparing `vstt-0.29.0/tests/test_trial.py` & `vstt-0.30.0/tests/test_trial.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,19 +43,21 @@
     assert trial.keys() == labels.keys()
 
 
 def test_import_trial() -> None:
     default_trial = vstt.trial.default_trial()
     trial_dict = {
         "weight": 2,
+        "condition_timeout": 0,
         "num_targets": 6,
         "target_order": "clockwise",
         "target_indices": "0 1 2 3 4 5",
         "add_central_target": True,
         "show_target_labels": False,
+        "hide_target_when_reached": True,
         "target_labels": "0 1 2 3 4 5",
         "fixed_target_intervals": False,
         "target_duration": 3,
         "central_target_duration": 3,
         "inter_target_duration": 0,
         "target_distance": 0.3,
         "target_size": 0.03,
@@ -74,14 +76,17 @@
         "post_trial_delay": 0.2,
         "post_trial_display_results": True,
         "post_block_delay": 2.0,
         "post_block_display_results": False,
         "show_delay_countdown": False,
         "enter_to_skip_delay": True,
     }
+    # start with a dict containing valid values for all keys
+    for key in default_trial:
+        assert key in trial_dict
     # all valid keys are imported
     trial = vstt.trial.import_and_validate_trial(trial_dict)
     for key in trial:
         assert trial[key] == trial_dict[key]  # type: ignore
     # if any keys are missing, default values are used instead
     missing_keys = [
         "weight",
```

### Comparing `vstt-0.29.0/tests/test_trials_widget.py` & `vstt-0.30.0/tests/test_trials_widget.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_update.py` & `vstt-0.30.0/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `vstt-0.29.0/tests/test_vis.py` & `vstt-0.30.0/tests/test_vis.py`

 * *Files identical despite different names*

