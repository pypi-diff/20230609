# Comparing `tmp/pygem-0.2.2.tar.gz` & `tmp/pygem-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygem-0.2.2.tar", last modified: Wed Jun  7 17:21:02 2023, max compression
+gzip compressed data, was "pygem-0.2.3.tar", last modified: Fri Jun  9 17:04:16 2023, max compression
```

## Comparing `pygem-0.2.2.tar` & `pygem-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.137871 pygem-0.2.2/
--rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2020-11-22 15:57:18.000000 pygem-0.2.2/.gitignore
--rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2020-11-22 15:57:18.000000 pygem-0.2.2/LICENSE
--rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 17:21:02.137554 pygem-0.2.2/PKG-INFO
--rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 04:01:43.000000 pygem-0.2.2/README.md
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.132023 pygem-0.2.2/pygem/
--rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-07 17:13:35.000000 pygem-0.2.2/pygem/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    28650 2023-06-07 17:03:36.000000 pygem-0.2.2/pygem/class_climate.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    35877 2023-06-07 17:03:36.000000 pygem-0.2.2/pygem/gcmbiasadj.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 03:54:10.000000 pygem-0.2.2/pygem/glacierdynamics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 04:01:43.000000 pygem-0.2.2/pygem/massbalance.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 03:54:10.000000 pygem-0.2.2/pygem/oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.133600 pygem-0.2.2/pygem/preprocess/
--rwxr-xr-x   0 drounce    (501) staff       (20)     9171 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/preprocess/ecmwf_data.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    22140 2023-06-07 05:08:29.000000 pygem-0.2.2/pygem/pygem_input.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    23592 2023-06-07 17:03:36.000000 pygem-0.2.2/pygem/pygem_modelsetup.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.134157 pygem-0.2.2/pygem/scraps/
--rwxr-xr-x   0 drounce    (501) staff       (20)      529 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/scraps/dummy_task_module.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/scraps/run.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.135697 pygem-0.2.2/pygem/shop/
--rwxr-xr-x   0 drounce    (501) staff       (20)     6736 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/shop/calving.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    21905 2021-02-01 14:09:24.000000 pygem-0.2.2/pygem/shop/climate.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2021-02-01 14:09:24.000000 pygem-0.2.2/pygem/shop/debris.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2021-09-23 17:13:56.000000 pygem-0.2.2/pygem/shop/icethickness.py
--rwxr-xr-x   0 drounce    (501) staff       (20)    12429 2022-08-11 04:33:58.000000 pygem-0.2.2/pygem/shop/mbdata.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.136664 pygem-0.2.2/pygem/tests/
--rwxr-xr-x   0 drounce    (501) staff       (20)        0 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/tests/__init__.py
--rwxr-xr-x   0 drounce    (501) staff       (20)      149 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/tests/test_basics.py
--rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2020-11-22 15:57:18.000000 pygem-0.2.2/pygem/tests/test_oggm_compat.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.137152 pygem-0.2.2/pygem/utils/
--rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2021-01-10 16:41:45.000000 pygem-0.2.2/pygem/utils/_funcs.py
--rw-r--r--   0 drounce    (501) staff       (20)     2651 2022-06-13 02:59:07.000000 pygem-0.2.2/pygem/utils/_funcs_selectglaciers.py
-drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-07 17:21:02.133151 pygem-0.2.2/pygem.egg-info/
--rw-r--r--   0 drounce    (501) staff       (20)     2386 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/PKG-INFO
--rw-r--r--   0 drounce    (501) staff       (20)      674 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/SOURCES.txt
--rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/dependency_links.txt
--rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-07 17:21:02.000000 pygem-0.2.2/pygem.egg-info/top_level.txt
--rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-07 17:13:35.000000 pygem-0.2.2/pyproject.toml
--rw-r--r--   0 drounce    (501) staff       (20)       38 2023-06-07 17:21:02.137981 pygem-0.2.2/setup.cfg
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.190827 pygem-0.2.3/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1361 2020-11-22 15:57:18.000000 pygem-0.2.3/.gitignore
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1069 2020-11-22 15:57:18.000000 pygem-0.2.3/LICENSE
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.172400 pygem-0.2.3/LICENSES/
+-rw-r--r--   0 drounce    (501) staff       (20)     1522 2023-06-07 04:01:43.000000 pygem-0.2.3/LICENSES/OGGM_LICENSE.txt
+-rw-r--r--   0 drounce    (501) staff       (20)     2442 2023-06-09 17:04:16.191062 pygem-0.2.3/PKG-INFO
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1931 2023-06-07 04:01:43.000000 pygem-0.2.3/README.md
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.179348 pygem-0.2.3/pygem/
+-rwxr-xr-x   0 drounce    (501) staff       (20)       83 2023-06-09 15:31:45.000000 pygem-0.2.3/pygem/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    28650 2023-06-07 17:03:36.000000 pygem-0.2.3/pygem/class_climate.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    14035 2023-06-09 15:31:45.000000 pygem-0.2.3/pygem/gcmbiasadj.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    48958 2023-06-07 03:54:10.000000 pygem-0.2.3/pygem/glacierdynamics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    60883 2023-06-07 04:01:43.000000 pygem-0.2.3/pygem/massbalance.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12724 2023-06-07 03:54:10.000000 pygem-0.2.3/pygem/oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.183407 pygem-0.2.3/pygem/preprocess/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     9171 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/preprocess/ecmwf_data.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    22140 2023-06-07 05:08:29.000000 pygem-0.2.3/pygem/pygem_input.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    23592 2023-06-07 17:03:36.000000 pygem-0.2.3/pygem/pygem_modelsetup.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.184254 pygem-0.2.3/pygem/scraps/
+-rwxr-xr-x   0 drounce    (501) staff       (20)      529 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/scraps/dummy_task_module.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1000 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/scraps/run.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.187096 pygem-0.2.3/pygem/shop/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     6736 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/shop/calving.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    21905 2021-02-01 14:09:24.000000 pygem-0.2.3/pygem/shop/climate.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     7783 2021-02-01 14:09:24.000000 pygem-0.2.3/pygem/shop/debris.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     5063 2021-09-23 17:13:56.000000 pygem-0.2.3/pygem/shop/icethickness.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)    12429 2022-08-11 04:33:58.000000 pygem-0.2.3/pygem/shop/mbdata.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.189317 pygem-0.2.3/pygem/tests/
+-rwxr-xr-x   0 drounce    (501) staff       (20)        0 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/tests/__init__.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)      149 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/tests/test_basics.py
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2594 2020-11-22 15:57:18.000000 pygem-0.2.3/pygem/tests/test_oggm_compat.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.190513 pygem-0.2.3/pygem/utils/
+-rwxr-xr-x   0 drounce    (501) staff       (20)     2304 2021-01-10 16:41:45.000000 pygem-0.2.3/pygem/utils/_funcs.py
+-rw-r--r--   0 drounce    (501) staff       (20)     2651 2022-06-13 02:59:07.000000 pygem-0.2.3/pygem/utils/_funcs_selectglaciers.py
+drwxr-xr-x   0 drounce    (501) staff       (20)        0 2023-06-09 17:04:16.182968 pygem-0.2.3/pygem.egg-info/
+-rw-r--r--   0 drounce    (501) staff       (20)     2442 2023-06-09 17:04:15.000000 pygem-0.2.3/pygem.egg-info/PKG-INFO
+-rw-r--r--   0 drounce    (501) staff       (20)      747 2023-06-09 17:04:16.000000 pygem-0.2.3/pygem.egg-info/SOURCES.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        1 2023-06-09 17:04:15.000000 pygem-0.2.3/pygem.egg-info/dependency_links.txt
+-rw-r--r--   0 drounce    (501) staff       (20)       72 2023-06-09 17:04:15.000000 pygem-0.2.3/pygem.egg-info/requires.txt
+-rw-r--r--   0 drounce    (501) staff       (20)        6 2023-06-09 17:04:15.000000 pygem-0.2.3/pygem.egg-info/top_level.txt
+-rw-r--r--   0 drounce    (501) staff       (20)      610 2023-06-09 17:03:00.000000 pygem-0.2.3/pyproject.toml
+-rwxr-xr-x   0 drounce    (501) staff       (20)     1026 2023-06-09 17:04:16.192620 pygem-0.2.3/setup.cfg
+-rwxr-xr-x   0 drounce    (501) staff       (20)      539 2023-06-09 17:01:16.000000 pygem-0.2.3/setup.py
```

### Comparing `pygem-0.2.2/.gitignore` & `pygem-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/LICENSE` & `pygem-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/PKG-INFO` & `pygem-0.2.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
+Home-page: https://github.com/drounce/PyGEM
+Author: David Rounce
 Author-email: David Rounce <drounce@cmu.edu>
+License: MIT
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ## Python Glacier Evolution Model (PyGEM)
 
 Overview: Python Glacier Evolution Model (PyGEM) is an open-source glacier evolution model coded in Python that models the transient evolution of glaciers. Each glacier is modeled independently using a monthly timestep. PyGEM has a modular framework that allows different schemes to be used for model calibration or model physics (e.g., climatic mass balance, glacier dynamics).  In the newest version under development, PyGEM is working to become compatible with the Open Global Glacier Model (OGGM; https://oggm.org/).
 
 Manual: Details concerning the model physics, installation, and running the model may be found here: https://github.com/drounce/PyGEM/wiki
```

### Comparing `pygem-0.2.2/README.md` & `pygem-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/class_climate.py` & `pygem-0.2.3/pygem/class_climate.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/glacierdynamics.py` & `pygem-0.2.3/pygem/glacierdynamics.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/massbalance.py` & `pygem-0.2.3/pygem/massbalance.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/oggm_compat.py` & `pygem-0.2.3/pygem/oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/preprocess/ecmwf_data.py` & `pygem-0.2.3/pygem/preprocess/ecmwf_data.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/pygem_input.py` & `pygem-0.2.3/pygem/pygem_input.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/pygem_modelsetup.py` & `pygem-0.2.3/pygem/pygem_modelsetup.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/scraps/dummy_task_module.py` & `pygem-0.2.3/pygem/scraps/dummy_task_module.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/scraps/run.py` & `pygem-0.2.3/pygem/scraps/run.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/shop/calving.py` & `pygem-0.2.3/pygem/shop/calving.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/shop/climate.py` & `pygem-0.2.3/pygem/shop/climate.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/shop/debris.py` & `pygem-0.2.3/pygem/shop/debris.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/shop/icethickness.py` & `pygem-0.2.3/pygem/shop/icethickness.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/shop/mbdata.py` & `pygem-0.2.3/pygem/shop/mbdata.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/tests/test_oggm_compat.py` & `pygem-0.2.3/pygem/tests/test_oggm_compat.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/utils/_funcs.py` & `pygem-0.2.3/pygem/utils/_funcs.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem/utils/_funcs_selectglaciers.py` & `pygem-0.2.3/pygem/utils/_funcs_selectglaciers.py`

 * *Files identical despite different names*

### Comparing `pygem-0.2.2/pygem.egg-info/PKG-INFO` & `pygem-0.2.3/pygem.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: pygem
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python Glacier Evolution Model for large-scale glacier modeling
+Home-page: https://github.com/drounce/PyGEM
+Author: David Rounce
 Author-email: David Rounce <drounce@cmu.edu>
+License: MIT
 Project-URL: Homepage, https://github.com/drounce/PyGEM
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 ## Python Glacier Evolution Model (PyGEM)
 
 Overview: Python Glacier Evolution Model (PyGEM) is an open-source glacier evolution model coded in Python that models the transient evolution of glaciers. Each glacier is modeled independently using a monthly timestep. PyGEM has a modular framework that allows different schemes to be used for model calibration or model physics (e.g., climatic mass balance, glacier dynamics).  In the newest version under development, PyGEM is working to become compatible with the Open Global Glacier Model (OGGM; https://oggm.org/).
 
 Manual: Details concerning the model physics, installation, and running the model may be found here: https://github.com/drounce/PyGEM/wiki
```

### Comparing `pygem-0.2.2/pyproject.toml` & `pygem-0.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     "wheel",
 ]
 
 [tool.setuptools_scm]
 
 [project]
 name = "pygem"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="David Rounce", email="drounce@cmu.edu" },
 ]
 description = "Python Glacier Evolution Model for large-scale glacier modeling"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

