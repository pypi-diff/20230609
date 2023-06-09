# Comparing `tmp/copasi_basico-0.8.tar.gz` & `tmp/copasi_basico-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copasi_basico-0.8.tar", last modified: Thu Nov 25 10:49:41 2021, max compression
+gzip compressed data, was "copasi_basico-0.9.tar", last modified: Wed Jan 12 15:06:03 2022, max compression
```

## Comparing `copasi_basico-0.8.tar` & `copasi_basico-0.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 10:49:41.860370 copasi_basico-0.8/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-25 10:49:32.000000 copasi_basico-0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-11-25 10:49:41.860370 copasi_basico-0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2427 2021-11-25 10:49:32.000000 copasi_basico-0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 10:49:41.864370 copasi_basico-0.8/basico/
--rw-r--r--   0 runner    (1001) docker     (121)      628 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      495 2021-11-25 10:49:41.864370 copasi_basico-0.8/basico/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     3645 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/array_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     5484 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/biomodels.py
--rw-r--r--   0 runner    (1001) docker     (121)    20638 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/compartment_array_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 10:49:41.860370 copasi_basico-0.8/basico/data/
--rw-r--r--   0 runner    (1001) docker     (121)    48767 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/BIOM10-fit.cps
--rw-r--r--   0 runner    (1001) docker     (121)    67388 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/LM-test1.cps
--rw-r--r--   0 runner    (1001) docker     (121)      171 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/MAPKdata.txt
--rw-r--r--   0 runner    (1001) docker     (121)   187123 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/PK_fit2.cps
--rw-r--r--   0 runner    (1001) docker     (121)   491444 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/array_1d.cps
--rw-r--r--   0 runner    (1001) docker     (121)    58827 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/brusselator.cps
--rw-r--r--   0 runner    (1001) docker     (121)     3859 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/data_2.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3431 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/data_3.txt
--rw-r--r--   0 runner    (1001) docker     (121)    33572 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/linear_base.cps
--rw-r--r--   0 runner    (1001) docker     (121)    13950 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/mmspect3.txt
--rw-r--r--   0 runner    (1001) docker     (121)    41736 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/data/turing_base.cps
--rw-r--r--   0 runner    (1001) docker     (121)     4380 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/jws_online.py
--rw-r--r--   0 runner    (1001) docker     (121)   136605 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/model_info.py
--rw-r--r--   0 runner    (1001) docker     (121)    16516 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/model_io.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 10:49:41.860370 copasi_basico-0.8/basico/petab/
--rw-r--r--   0 runner    (1001) docker     (121)      256 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/petab/core.py
--rw-r--r--   0 runner    (1001) docker     (121)    10710 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/petab/select.py
--rw-r--r--   0 runner    (1001) docker     (121)    13022 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/task_optimization.py
--rw-r--r--   0 runner    (1001) docker     (121)    40321 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/task_parameterestimation.py
--rw-r--r--   0 runner    (1001) docker     (121)    16807 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/task_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     3138 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/task_steadystate.py
--rw-r--r--   0 runner    (1001) docker     (121)    15369 2021-11-25 10:49:32.000000 copasi_basico-0.8/basico/task_timecourse.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-25 10:49:41.860370 copasi_basico-0.8/copasi_basico.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2021-11-25 10:49:41.000000 copasi_basico-0.8/copasi_basico.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      899 2021-11-25 10:49:41.000000 copasi_basico-0.8/copasi_basico.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-25 10:49:41.000000 copasi_basico-0.8/copasi_basico.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-11-25 10:49:41.000000 copasi_basico-0.8/copasi_basico.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-25 10:49:41.000000 copasi_basico-0.8/copasi_basico.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-11-25 10:49:41.864370 copasi_basico-0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2572 2021-11-25 10:49:32.000000 copasi_basico-0.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2021-11-25 10:49:32.000000 copasi_basico-0.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:06:03.539662 copasi_basico-0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-01-12 15:05:45.000000 copasi_basico-0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-01-12 15:06:03.539662 copasi_basico-0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2427 2022-01-12 15:05:45.000000 copasi_basico-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:06:03.539662 copasi_basico-0.9/basico/
+-rw-r--r--   0 runner    (1001) docker     (121)      628 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      495 2022-01-12 15:06:03.539662 copasi_basico-0.9/basico/_version.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3645 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/array_tools.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/biomodels.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20638 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/compartment_array_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:06:03.539662 copasi_basico-0.9/basico/data/
+-rw-r--r--   0 runner    (1001) docker     (121)    48767 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/BIOM10-fit.cps
+-rw-r--r--   0 runner    (1001) docker     (121)    67388 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/LM-test1.cps
+-rw-r--r--   0 runner    (1001) docker     (121)      171 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/MAPKdata.txt
+-rw-r--r--   0 runner    (1001) docker     (121)   187123 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/PK_fit2.cps
+-rw-r--r--   0 runner    (1001) docker     (121)   491444 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/array_1d.cps
+-rw-r--r--   0 runner    (1001) docker     (121)    58827 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/brusselator.cps
+-rw-r--r--   0 runner    (1001) docker     (121)     3859 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/data_2.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3431 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/data_3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    33572 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/linear_base.cps
+-rw-r--r--   0 runner    (1001) docker     (121)    13950 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/mmspect3.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    41736 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/data/turing_base.cps
+-rw-r--r--   0 runner    (1001) docker     (121)     4380 2022-01-12 15:05:45.000000 copasi_basico-0.9/basico/jws_online.py
+-rw-r--r--   0 runner    (1001) docker     (121)   136605 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/model_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16516 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/model_io.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:06:03.539662 copasi_basico-0.9/basico/petab/
+-rw-r--r--   0 runner    (1001) docker     (121)      256 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10621 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/petab/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10710 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/petab/select.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13022 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/task_optimization.py
+-rw-r--r--   0 runner    (1001) docker     (121)    40644 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/task_parameterestimation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16807 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/task_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3138 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/task_steadystate.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15369 2022-01-12 15:05:46.000000 copasi_basico-0.9/basico/task_timecourse.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-12 15:06:03.539662 copasi_basico-0.9/copasi_basico.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-01-12 15:06:03.000000 copasi_basico-0.9/copasi_basico.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      899 2022-01-12 15:06:03.000000 copasi_basico-0.9/copasi_basico.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-12 15:06:03.000000 copasi_basico-0.9/copasi_basico.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-01-12 15:06:03.000000 copasi_basico-0.9/copasi_basico.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-12 15:06:03.000000 copasi_basico-0.9/copasi_basico.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-01-12 15:06:03.539662 copasi_basico-0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2572 2022-01-12 15:05:46.000000 copasi_basico-0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-01-12 15:05:46.000000 copasi_basico-0.9/versioneer.py
```

### Comparing `copasi_basico-0.8/PKG-INFO` & `copasi_basico-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copasi_basico
-Version: 0.8
+Version: 0.9
 Summary: Simplified COPASI interface for python
 Home-page: https://github.com/copasi/basico
 Author: COPASI Team
 Author-email: developers@copasi.org
 License: Artistic-2.0
 Project-URL: Github, https://github.com/copasi/basico
 Project-URL: Issues, https://github.com/copasi/basico/issues
```

### Comparing `copasi_basico-0.8/README.md` & `copasi_basico-0.9/README.md`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/__init__.py` & `copasi_basico-0.9/basico/__init__.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/array_tools.py` & `copasi_basico-0.9/basico/array_tools.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/biomodels.py` & `copasi_basico-0.9/basico/biomodels.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/compartment_array_tools.py` & `copasi_basico-0.9/basico/compartment_array_tools.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/BIOM10-fit.cps` & `copasi_basico-0.9/basico/data/BIOM10-fit.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/LM-test1.cps` & `copasi_basico-0.9/basico/data/LM-test1.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/PK_fit2.cps` & `copasi_basico-0.9/basico/data/PK_fit2.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/array_1d.cps` & `copasi_basico-0.9/basico/data/array_1d.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/brusselator.cps` & `copasi_basico-0.9/basico/data/brusselator.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/data_2.txt` & `copasi_basico-0.9/basico/data/data_2.txt`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/data_3.txt` & `copasi_basico-0.9/basico/data/data_3.txt`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/linear_base.cps` & `copasi_basico-0.9/basico/data/linear_base.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/mmspect3.txt` & `copasi_basico-0.9/basico/data/mmspect3.txt`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/data/turing_base.cps` & `copasi_basico-0.9/basico/data/turing_base.cps`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/jws_online.py` & `copasi_basico-0.9/basico/jws_online.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/model_info.py` & `copasi_basico-0.9/basico/model_info.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/model_io.py` & `copasi_basico-0.9/basico/model_io.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/petab/core.py` & `copasi_basico-0.9/basico/petab/core.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/petab/select.py` & `copasi_basico-0.9/basico/petab/select.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/task_optimization.py` & `copasi_basico-0.9/basico/task_optimization.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/task_parameterestimation.py` & `copasi_basico-0.9/basico/task_parameterestimation.py`

 * *Files 1% similar despite different names*

```diff
@@ -729,14 +729,20 @@
         if current.lower() == 'time':
             role = COPASI.CExperiment.time
         else:
             obj = model.findObjectByDisplayName(current)
             if obj is None:
                 logging.warning("Can't find model element for {0}".format(current))
             else:
+                assert(isinstance(obj, COPASI.CDataObject))
+                if obj.getObjectType() != 'Reference':
+                    try:
+                        obj = obj.getValueReference()
+                    except AttributeError:
+                        logging.warning("Cannot map the element {0}".format(current))
                 role = _get_role_for_reference(obj.getObjectName())
                 obj_map.setObjectCN(i, obj.getCN())
         obj_map.setRole(i, role)
 
     exp.calculateWeights()
     exp_set.compile(model.getModel().getMathContainer())
```

### Comparing `copasi_basico-0.8/basico/task_scan.py` & `copasi_basico-0.9/basico/task_scan.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/task_steadystate.py` & `copasi_basico-0.9/basico/task_steadystate.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/basico/task_timecourse.py` & `copasi_basico-0.9/basico/task_timecourse.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/copasi_basico.egg-info/PKG-INFO` & `copasi_basico-0.9/copasi_basico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copasi-basico
-Version: 0.8
+Version: 0.9
 Summary: Simplified COPASI interface for python
 Home-page: https://github.com/copasi/basico
 Author: COPASI Team
 Author-email: developers@copasi.org
 License: Artistic-2.0
 Project-URL: Github, https://github.com/copasi/basico
 Project-URL: Issues, https://github.com/copasi/basico/issues
```

### Comparing `copasi_basico-0.8/copasi_basico.egg-info/SOURCES.txt` & `copasi_basico-0.9/copasi_basico.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/setup.py` & `copasi_basico-0.9/setup.py`

 * *Files identical despite different names*

### Comparing `copasi_basico-0.8/versioneer.py` & `copasi_basico-0.9/versioneer.py`

 * *Files identical despite different names*

