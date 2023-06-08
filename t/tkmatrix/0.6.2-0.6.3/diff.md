# Comparing `tmp/tkmatrix-0.6.2.tar.gz` & `tmp/tkmatrix-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.6.2.tar", last modified: Thu May 18 17:17:21 2023, max compression
+gzip compressed data, was "tkmatrix-0.6.3.tar", last modified: Thu Jun  8 22:19:12 2023, max compression
```

## Comparing `tkmatrix-0.6.2.tar` & `tkmatrix-0.6.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.887184 tkmatrix-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 17:17:21.887184 tkmatrix-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41014 2023-05-18 17:17:11.000000 tkmatrix-0.6.2/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 17:17:21.883184 tkmatrix-0.6.2/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 17:17:21.000000 tkmatrix-0.6.2/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41582 2023-06-08 22:18:55.000000 tkmatrix-0.6.3/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 22:19:12.356270 tkmatrix-0.6.3/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-08 22:19:12.000000 tkmatrix-0.6.3/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 22:19:11.000000 tkmatrix-0.6.3/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.6.2/LICENSE` & `tkmatrix-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.2/PKG-INFO` & `tkmatrix-0.6.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,77 +1,53 @@
-Metadata-Version: 2.1
-Name: tkmatrix
-Version: 0.6.2
-Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
-Home-page: https://github.com/PlanetHunters/tkmatrix
-Author: M. Dévora-Pajares & F.J. Pozuelos
-Author-email: mdevorapajares@protonmail.com
-License: UNKNOWN
-Description: <p align="center">
-          <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
-        </p>
-        
-        # MATRIX ToolKit
-        ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
-        
-        ## Citation
-        We are planning to write a scientific paper based on the usage of MATRIX. In the meantime, we encourage the users to cite the Software DOI in their research:
-        ```
-        @MISC{2022zndo...6570831D,
-               author = {{D{\'e}vora-Pajares}, Mart{\'\i}n and {Pozuelos}, Francisco J.},
-                title = "{MATRIX: Multi-phAse Transits Recovery from Injected eXoplanets}",
-             keywords = {exoplanets, transits, injection \& recovery, python},
-         howpublished = {Zenodo},
-                 year = 2022,
-                month = may,
-                  eid = {10.5281/zenodo.6570831},
-                  doi = {10.5281/zenodo.6570831},
-              version = {0.3.17},
-            publisher = {Zenodo},
-               adsurl = {https://ui.adsabs.harvard.edu/abs/2022zndo...6570831D},
-              adsnote = {Provided by the SAO/NASA Astrophysics Data System}
-        }
-        ```
-        
-        ## Main Developers
-        [M. Dévora Pajares](https://github.com/martindevora)
-        
-        [F.J. Pozuelos](https://github.com/franpoz)
-        
-        
-        ## Additional contributors
-        [L. Cerdeño Mota](https://github.com/LuisCerdenoMota) 
-        
-        ## Installation
-        Supported Python versions: 3.8, 3.9. Install with:
-        
-        ```
-        python3.8 -m pip install numpy==1.22.4
-        python3.8 -m pip install -r requirements.txt
-        ```
-        
-        You can find the requirements.txt file [here](https://github.com/PlanetHunters/tkmatrix/blob/master/requirements.txt). 
-        
-        ## Tests
-        We use [tox](https://tox.readthedocs.io) to test MATRIX under all the supported Python versions. Usage:
-        
-        `tox`
-        
-        ## Examples
-        Under the [examples](https://github.com/PlanetHunters/tkmatrix/tree/master/examples) directory.
-        
-        ## Execution
-        Just execute the command below this text. Take into accont that the `user-properties.yaml` file needs to include several mandatory options. Please refer to the example file under the examples directory.
-        
-        `python3.8 -m tkmatrix --properties user-properties.yaml`
-        
-        ## By-products
-        * a_tls_report.csv: A file containing a csv formatted output given the orbital period, the radius and the epoch besides the outputs with found status, SNR and SDE of the results.
-        * a_tls_report.png: A file with an automatically generated plot from the csv report. You are free to build your own plot from the report if you feel like the one provided by MATRIX is not good enough for your purposes.
-        * Injected curves (csv files): In case you want to study the injected curves generated for the recovery, you can set a flag to the tool so that it keeps the files after it finishes. If you don't provide that flag, the files will be removed at the end of the execution.
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+<p align="center">
+  <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
+</p>
+
+# MATRIX ToolKit
+ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
+
+MATRIX is an injection-recovery software prepared to create grids of scenarios with a set of periods, radii and epochs
+of synthetic transiting exoplanet signals in a provided light curve. The typical injection-recovery execution has
+consisted in the usage of 2 dimensional scenarios, where only one epoch (random or hardcoded) was used for each period
+and radius. Even though this is a fair approach when the computational power is very limited, this reduces the accuracy
+of the experiment as the recoverability might vary depending on the transit epoch and hence, the places where the
+transits would appear in the curve. E.g: A transit would be clearly recovered falling in a quite region of the curve
+but not easy to recover when it happened close to a flare or a curve gap. A multi-phase analysis can now be done with
+MATRIX easily by only setting a few parameters in a configuration file and running one line of code.
+
+Just execute the command below this text. Take into accont that the `user-properties.yaml` file needs to include 
+several mandatory options. Please refer to the example files under the 
+[example](https://github.com/PlanetHunters/tkmatrix/tree/master/examples/TOI-2257/matrix_properties.yaml) directory.
+
+`python3.8 -m tkmatrix --properties user-properties.yaml`
+
+For the complete set of properties available for use please look at the root 
+[properties.yaml](https://github.com/PlanetHunters/tkmatrix/tree/master/tkmatrix/properties.yaml)
+
+
+## By-products
+* a_tls_report.csv: A file containing a csv formatted output given the orbital period, the radius and the epoch besides the outputs with found status, SNR and SDE of the results.
+* a_tls_report.png: A file with an automatically generated plot from the csv report. You are free to build your own plot from the report if you feel like the one provided by MATRIX is not good enough for your purposes.
+* Injected curves (csv files): In case you want to study the injected curves generated for the recovery, you can set a flag to the tool so that it keeps the files after it finishes. If you don't provide that flag, the files will be removed at the end of the execution.
+
+
+## Citation
+We are planning to write a scientific paper based on the usage of MATRIX. In the meantime, we encourage the users to cite the Software DOI in their research:
+```
+@MISC{2022zndo...6570831D,
+       author = {{D{\'e}vora-Pajares}, Mart{\'\i}n and {Pozuelos}, Francisco J.},
+        title = "{MATRIX: Multi-phAse Transits Recovery from Injected eXoplanets}",
+     keywords = {exoplanets, transits, injection \& recovery, python},
+ howpublished = {Zenodo},
+         year = 2022,
+        month = may,
+          eid = {10.5281/zenodo.6570831},
+          doi = {10.5281/zenodo.6570831},
+      version = {0.3.17},
+    publisher = {Zenodo},
+       adsurl = {https://ui.adsabs.harvard.edu/abs/2022zndo...6570831D},
+      adsnote = {Provided by the SAO/NASA Astrophysics Data System}
+}
+```
+
+## Documentation
+For more information please visit [https://tkmatrix.readthedocs.io/](https://tkmatrix.readthedocs.io/).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tkmatrix-0.6.2/setup.py` & `tkmatrix-0.6.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.6.2"
+version = "0.6.3"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
@@ -22,15 +22,15 @@
     python_requires='>=3.8',
     install_requires=['argparse==1.4.0',
                         'beautifulsoup4==4.9.3',
                         'configparser==5.0.1',
                         "corner==2.1.0",
                         "cython==0.29.21",
                         "ellc==1.8.5",
-                        "lcbuilder==0.12.2",
+                        "lcbuilder==0.12.5",
                         "matplotlib==3.5.2",
                         "mock==4.0.3",
                         'numba>=0.53.0rc1',
                         'pyparsing==2.4.7', # Matplotlib dependency
                         "seaborn==0.11.1",
                         'setuptools>=41.0.0',
                         "scipy==1.8.0",
```

### Comparing `tkmatrix-0.6.2/tkmatrix/__main__.py` & `tkmatrix-0.6.3/tkmatrix/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,11 +154,12 @@
                            period_grid_geom=matrix_user_properties["PERIOD_GRID_GEOM"],
                            radius_grid_geom=matrix_user_properties["RADIUS_GRID_GEOM"],
                            inject_dir=inject_dir)
     ir.recovery(inject_dir, matrix_user_properties["SNR_THRESHOLD"],
                 matrix_user_properties["DETREND_METHOD"],
                 matrix_user_properties["DETREND_WS"], matrix_user_properties["FIT_METHOD"],
                 matrix_user_properties["RUN_LIMIT"],
-                custom_search, matrix_user_properties["MAX_PERIOD_SEARCH"], matrix_user_properties["OVERSAMPLING"])
+                custom_search, matrix_user_properties["MAX_PERIOD_SEARCH"], matrix_user_properties["OVERSAMPLING"],
+                matrix_user_properties["SIGNAL_SELECTION_MODE"])
     ir.plot_results(target, inject_dir, period_grid, radius_grid, period_grid_geom=matrix_user_properties["PERIOD_GRID_GEOM"],
                     radius_grid_geom=matrix_user_properties["RADIUS_GRID_GEOM"])
     print("Execution time: " + str(datetime.datetime.now() - start_time))
```

### Comparing `tkmatrix-0.6.2/tkmatrix/inject_rv_model.py` & `tkmatrix-0.6.3/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.2/tkmatrix/rv.py` & `tkmatrix-0.6.3/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.2/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.6.3/tkmatrix/tests/test_tkmatrix.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.2/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.6.3/tkmatrix/tkmatrix_class.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,15 +93,15 @@
                                                        self.auto_detrend_ratio, self.auto_detrend_period,
                                                        self.prepare_algorithm, False,
                                                        self.oscillation_min_snr, self.oscillation_amplitude_threshold,
                                                        self.oscillation_ws_percent, self.oscillation_min_period,
                                                        self.oscillation_max_period)
         if inject_dir is None:
             inject_dir = self.build_inject_dir()
-        self.lc_build = self.lcbuilder.build(self.object_info, inject_dir, self.cache_dir)
+        self.lc_build = self.lcbuilder.build(self.object_info, inject_dir, self.cache_dir, self.cores)
         if self.star_info is None:
             self.star_info = self.lc_build.star_info
         self.ab = self.star_info.ld_coefficients
         if self.ab is None:
             raise ValueError("Limb Darkening parameters were not found. Please provide them in the STAR properties.")
         self.mass = self.star_info.mass
         self.massmin = self.star_info.mass_min
@@ -133,15 +133,15 @@
                                                        self.oscillation_ws_percent, self.oscillation_min_period,
                                                        self.oscillation_max_period)
 
         if self.object_info.reduce_simple_oscillations and \
                 self.object_info.oscillation_max_period < self.object_info.oscillation_min_period:
             logging.info("Stellar oscillation period has been set to empty. Defaulting to 1/3 the minimum search period")
             self.object_info.oscillation_max_period = self.MIN_SEARCH_PERIOD / 3
-        self.lc_build = self.lcbuilder.build(self.object_info, inject_dir, self.cache_dir)
+        self.lc_build = self.lcbuilder.build(self.object_info, inject_dir, self.cache_dir, self.cores)
 
     def build_inject_dir(self):
         inject_dir = self.dir + "/" + self.object_info.mission_id().replace(" ", "") + "_ir/"
         index = 0
         while os.path.exists(inject_dir) or os.path.isdir(inject_dir):
             inject_dir = self.dir + "/" + self.object_info.mission_id().replace(" ", "") + "_ir_" + str(index) + "/"
             index = index + 1
@@ -381,15 +381,15 @@
                 except Exception as e:
                     traceback.print_exc()
                     print("File not valid: " + file)
         self.remove_non_results_files(inject_dir)
 
     def recovery(self, inject_dir, snr_threshold=5, detrend_method=DETREND_BIWEIGHT, detrend_ws=0,
                  transit_template='tls', run_limit=5, custom_search_algorithm=None, max_period_search=25,
-                 oversampling=3):
+                 oversampling=3, signal_selection_mode='period-epoch'):
         """
         Given the injection dir, it will iterate over all the csvs matching light curves and try the recovery of their
         transit parameters (period and epoch).
 
         :param inject_dir: the directory to search for light curves
         :param snr_threshold: the SNR value to break the search for each curve
         :param detrend_ws: the window size to detrend the curves
@@ -432,15 +432,15 @@
                         found, snr, sde, run, duration_found, period_found, epoch_found = \
                             self.__search(self.lc_build.lc.time.value, self.lc_build.lc.flux.value, self.radius, self.radiusmin,
                                           self.radiusmax, self.mass, self.massmin,
                                           self.massmax, self.ab, epoch, period, self.MIN_SEARCH_PERIOD,
                                           max_period_search, snr_threshold,
                                           transit_template, detrend_method, detrend_ws,
                                           self.lc_build.transits_min_count, run_limit, custom_search_algorithm,
-                                          oversampling)
+                                          oversampling, signal_selection_mode)
                     new_report = {"period": period, "radius": r_planet, "epoch": epoch, "found": found, "snr": snr,
                                   "sde": sde, "run": run, "duration_found": duration_found,
                                   "period_found": period_found, "epoch_found": epoch_found}
                     reports_df = reports_df.append(new_report, ignore_index=True)
                     print("P=" + str(period) + ", R=" + str(r_planet) + ", T0=" + str(epoch) + ", FOUND WAS " + str(
                         found) +
                           " WITH SNR " + str(snr) + " AND SDE " + str(sde))
@@ -614,30 +614,31 @@
         if yticks is not None:
             plt.xticks(yticks)
         plt.savefig(output_dir + '/inj-rec-diff.png', bbox_inches='tight', dpi=200)
         plt.close()
 
     def __search(self, time, flux, rstar, rstar_min, rstar_max, mass, mstar_min, mstar_max, ab, epoch,
                  period, min_period, max_period, min_snr, transit_template, detrend_method, ws, transits_min_count,
-                 run_limit, custom_search_algorithm, oversampling):
+                 run_limit, custom_search_algorithm, oversampling, signal_selection_mode):
         tls_period_grid, oversampling = LcbuilderHelper.calculate_period_grid(time, min_period, max_period,
                                                                               oversampling, self.star_info,
                                                                               transits_min_count)
         if custom_search_algorithm is not None:
             return custom_search_algorithm.search(time, flux, rstar, rstar_min, rstar_max, mass, mstar_min, mstar_max,
                                                 ab, epoch, period, min_period, max_period, min_snr, self.cores,
                                                 transit_template, detrend_method, ws, transits_min_count, run_limit)
         else:
             return self.__tls_search(time, flux, rstar, rstar_min, rstar_max, mass, mstar_min, mstar_max, ab, epoch,
                                      period, min_period, max_period, min_snr, self.cores, transit_template,
-                                     detrend_method, ws, transits_min_count, run_limit, tls_period_grid)
+                                     detrend_method, ws, transits_min_count, run_limit, tls_period_grid,
+                                     signal_selection_mode)
 
     def __tls_search(self, time, flux, rstar, rstar_min, rstar_max, mass, mstar_min, mstar_max, ab, epoch,
                      period, min_period, max_period, min_snr, cores, transit_template, detrend_method, ws,
-                     transits_min_count, run_limit, tls_period_grid):
+                     transits_min_count, run_limit, tls_period_grid, signal_selection_mode):
         snr = 1e12
         found_signal = False
         time, flux = cleaned_array(time, flux)
         run = 0
         if ws > 0:
             if detrend_method == self.DETREND_BIWEIGHT:
                 flux = wotan.flatten(time, flux, window_length=ws, return_trend=False, method=detrend_method,
@@ -666,15 +667,21 @@
             snr = results.snr
             if results.snr >= min_snr:
                 intransit_result = transit_mask(time, results.period, 2 * results.duration, results.T0)
                 time = time[~intransit_result]
                 flux = flux[~intransit_result]
                 time, flux = cleaned_array(time, flux)
                 if results.transit_times is not None and len(results.transit_times) > 0:
-                    found_signal = HarmonicSelector.is_harmonic(results.transit_times[0], epoch, results.period, period)
+                    if signal_selection_mode == 'period-epoch':
+                        found_signal = HarmonicSelector.is_harmonic(results.transit_times[0], epoch, results.period, period)
+                    else:
+                        found_signal = HarmonicSelector.multiple_of(results.period, period) != 0
+                    # plt.plot(foldedleastsquares.fold(time, results.period, results.transit_times[0], flux))
+                    # plt.xlim([0.4, 0.6])
+                    # plt.show()
                     if found_signal:
                         break
             run = run + 1
         return found_signal, results.snr, results.SDE, run, results.duration, results.period, results.T0
 
     @staticmethod
     def num_of_zeros(n):
```

### Comparing `tkmatrix-0.6.2/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.6.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,47 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.2
+Version: 0.6.3
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
         </p>
         
         # MATRIX ToolKit
         ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
         
+        MATRIX is an injection-recovery software prepared to create grids of scenarios with a set of periods, radii and epochs
+        of synthetic transiting exoplanet signals in a provided light curve. The typical injection-recovery execution has
+        consisted in the usage of 2 dimensional scenarios, where only one epoch (random or hardcoded) was used for each period
+        and radius. Even though this is a fair approach when the computational power is very limited, this reduces the accuracy
+        of the experiment as the recoverability might vary depending on the transit epoch and hence, the places where the
+        transits would appear in the curve. E.g: A transit would be clearly recovered falling in a quite region of the curve
+        but not easy to recover when it happened close to a flare or a curve gap. A multi-phase analysis can now be done with
+        MATRIX easily by only setting a few parameters in a configuration file and running one line of code.
+        
+        Just execute the command below this text. Take into accont that the `user-properties.yaml` file needs to include 
+        several mandatory options. Please refer to the example files under the 
+        [example](https://github.com/PlanetHunters/tkmatrix/tree/master/examples/TOI-2257/matrix_properties.yaml) directory.
+        
+        `python3.8 -m tkmatrix --properties user-properties.yaml`
+        
+        For the complete set of properties available for use please look at the root 
+        [properties.yaml](https://github.com/PlanetHunters/tkmatrix/tree/master/tkmatrix/properties.yaml)
+        
+        
+        ## By-products
+        * a_tls_report.csv: A file containing a csv formatted output given the orbital period, the radius and the epoch besides the outputs with found status, SNR and SDE of the results.
+        * a_tls_report.png: A file with an automatically generated plot from the csv report. You are free to build your own plot from the report if you feel like the one provided by MATRIX is not good enough for your purposes.
+        * Injected curves (csv files): In case you want to study the injected curves generated for the recovery, you can set a flag to the tool so that it keeps the files after it finishes. If you don't provide that flag, the files will be removed at the end of the execution.
+        
+        
         ## Citation
         We are planning to write a scientific paper based on the usage of MATRIX. In the meantime, we encourage the users to cite the Software DOI in their research:
         ```
         @MISC{2022zndo...6570831D,
                author = {{D{\'e}vora-Pajares}, Mart{\'\i}n and {Pozuelos}, Francisco J.},
                 title = "{MATRIX: Multi-phAse Transits Recovery from Injected eXoplanets}",
              keywords = {exoplanets, transits, injection \& recovery, python},
@@ -28,50 +53,16 @@
               version = {0.3.17},
             publisher = {Zenodo},
                adsurl = {https://ui.adsabs.harvard.edu/abs/2022zndo...6570831D},
               adsnote = {Provided by the SAO/NASA Astrophysics Data System}
         }
         ```
         
-        ## Main Developers
-        [M. Dévora Pajares](https://github.com/martindevora)
-        
-        [F.J. Pozuelos](https://github.com/franpoz)
-        
-        
-        ## Additional contributors
-        [L. Cerdeño Mota](https://github.com/LuisCerdenoMota) 
-        
-        ## Installation
-        Supported Python versions: 3.8, 3.9. Install with:
-        
-        ```
-        python3.8 -m pip install numpy==1.22.4
-        python3.8 -m pip install -r requirements.txt
-        ```
-        
-        You can find the requirements.txt file [here](https://github.com/PlanetHunters/tkmatrix/blob/master/requirements.txt). 
-        
-        ## Tests
-        We use [tox](https://tox.readthedocs.io) to test MATRIX under all the supported Python versions. Usage:
-        
-        `tox`
-        
-        ## Examples
-        Under the [examples](https://github.com/PlanetHunters/tkmatrix/tree/master/examples) directory.
-        
-        ## Execution
-        Just execute the command below this text. Take into accont that the `user-properties.yaml` file needs to include several mandatory options. Please refer to the example file under the examples directory.
-        
-        `python3.8 -m tkmatrix --properties user-properties.yaml`
-        
-        ## By-products
-        * a_tls_report.csv: A file containing a csv formatted output given the orbital period, the radius and the epoch besides the outputs with found status, SNR and SDE of the results.
-        * a_tls_report.png: A file with an automatically generated plot from the csv report. You are free to build your own plot from the report if you feel like the one provided by MATRIX is not good enough for your purposes.
-        * Injected curves (csv files): In case you want to study the injected curves generated for the recovery, you can set a flag to the tool so that it keeps the files after it finishes. If you don't provide that flag, the files will be removed at the end of the execution.
+        ## Documentation
+        For more information please visit [https://tkmatrix.readthedocs.io/](https://tkmatrix.readthedocs.io/). 
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

