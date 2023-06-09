# Comparing `tmp/tkmatrix-0.6.3.tar.gz` & `tmp/tkmatrix-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.6.3.tar", last modified: Thu Jun  8 22:19:12 2023, max compression
+gzip compressed data, was "tkmatrix-0.6.4.tar", last modified: Fri Jun  9 08:07:04 2023, max compression
```

## Comparing `tkmatrix-0.6.3.tar` & `tkmatrix-0.6.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41582 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 22:19:12.000000 tkmatrix-0.6.3/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 08:06:51.000000 tkmatrix-0.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 08:06:51.000000 tkmatrix-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-09 08:06:51.000000 tkmatrix-0.6.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.714742 tkmatrix-0.6.4/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41602 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.6.3/LICENSE` & `tkmatrix-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/PKG-INFO` & `tkmatrix-0.6.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.3
+Version: 0.6.4
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.6.3/README.md` & `tkmatrix-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/setup.py` & `tkmatrix-0.6.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.6.3"
+version = "0.6.4"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
```

### Comparing `tkmatrix-0.6.3/tkmatrix/__main__.py` & `tkmatrix-0.6.4/tkmatrix/__main__.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/tkmatrix/inject_model.py` & `tkmatrix-0.6.4/tkmatrix/inject_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/tkmatrix/inject_rv_model.py` & `tkmatrix-0.6.4/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/tkmatrix/properties.yaml` & `tkmatrix-0.6.4/tkmatrix/properties.yaml`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/tkmatrix/rv.py` & `tkmatrix-0.6.4/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.6.4/tkmatrix/tests/test_tkmatrix.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.3/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.6.4/tkmatrix/tkmatrix_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -281,15 +281,15 @@
         time = self.lc_build.lc.time.value
         flux_err = self.lc_build.lc.flux_err.value
         inject_models = []
         for period in period_grid:
             for t0 in np.linspace(time[0], time[0] + period, phases + 2)[1:-1]:
                 for rplanet in radius_grid:
                     rplanet = np.around(rplanet, decimals=2) * u.R_earth
-                    inject_models.append(InjectModel(inject_dir, time, flux0, flux_err, self.rstar, self.mstar, t0,
+                    inject_models.append(InjectModel(inject_dir, time, np.array(flux0), np.array(flux_err), self.rstar, self.mstar, t0,
                                                      period, rplanet, self.exposure_time, self.ab))
         with Pool(processes=self.cores) as pool:
             pool.map(InjectModel.make_model, inject_models)
         return inject_dir, period_grid, radius_grid
 
     def recovery_rv_periods(self, filename, max_period_search, rv_masks=None, oversampling=1,
                             cores=os.cpu_count() - 1):
```

### Comparing `tkmatrix-0.6.3/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.6.4/tkmatrix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.3
+Version: 0.6.4
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

