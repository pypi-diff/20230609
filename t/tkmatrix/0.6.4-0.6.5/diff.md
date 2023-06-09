# Comparing `tmp/tkmatrix-0.6.4.tar.gz` & `tmp/tkmatrix-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkmatrix-0.6.4.tar", last modified: Fri Jun  9 08:07:04 2023, max compression
+gzip compressed data, was "tkmatrix-0.6.5.tar", last modified: Fri Jun  9 12:59:57 2023, max compression
```

## Comparing `tkmatrix-0.6.4.tar` & `tkmatrix-0.6.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 08:06:51.000000 tkmatrix-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 08:06:51.000000 tkmatrix-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-09 08:06:51.000000 tkmatrix-0.6.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.714742 tkmatrix-0.6.4/tkmatrix/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/tkmatrix/custom_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/custom_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/inject_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/inject_rv_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/properties.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/rv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/tkmatrix/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9135 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/tests/test_tkmatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    41602 2023-06-09 08:06:52.000000 tkmatrix-0.6.4/tkmatrix/tkmatrix_class.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:07:04.718742 tkmatrix-0.6.4/tkmatrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 08:07:04.000000 tkmatrix-0.6.4/tkmatrix.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:59:57.459162 tkmatrix-0.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 12:59:57.459162 tkmatrix-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 12:59:57.459162 tkmatrix-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:59:57.455162 tkmatrix-0.6.5/tkmatrix/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:59:57.455162 tkmatrix-0.6.5/tkmatrix/custom_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/custom_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/inject_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/inject_rv_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/properties.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    17253 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/rv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:59:57.455162 tkmatrix-0.6.5/tkmatrix/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/tests/test_tkmatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43774 2023-06-09 12:59:43.000000 tkmatrix-0.6.5/tkmatrix/tkmatrix_class.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 12:59:57.455162 tkmatrix-0.6.5/tkmatrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 12:59:57.000000 tkmatrix-0.6.5/tkmatrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-09 12:59:57.000000 tkmatrix-0.6.5/tkmatrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 12:59:57.000000 tkmatrix-0.6.5/tkmatrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-09 12:59:57.000000 tkmatrix-0.6.5/tkmatrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 12:59:57.000000 tkmatrix-0.6.5/tkmatrix.egg-info/top_level.txt
```

### Comparing `tkmatrix-0.6.4/LICENSE` & `tkmatrix-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/PKG-INFO` & `tkmatrix-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.4
+Version: 0.6.5
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

### Comparing `tkmatrix-0.6.4/README.md` & `tkmatrix-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/setup.py` & `tkmatrix-0.6.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = "0.6.4"
+version = "0.6.5"
 setuptools.setup(
     name="tkmatrix",
     version=version,
     author="M. Dévora-Pajares & F.J. Pozuelos",
     author_email="mdevorapajares@protonmail.com",
     description="ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets",
     long_description=long_description,
```

### Comparing `tkmatrix-0.6.4/tkmatrix/__main__.py` & `tkmatrix-0.6.5/tkmatrix/__main__.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/tkmatrix/inject_model.py` & `tkmatrix-0.6.5/tkmatrix/inject_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/tkmatrix/inject_rv_model.py` & `tkmatrix-0.6.5/tkmatrix/inject_rv_model.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/tkmatrix/properties.yaml` & `tkmatrix-0.6.5/tkmatrix/properties.yaml`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/tkmatrix/rv.py` & `tkmatrix-0.6.5/tkmatrix/rv.py`

 * *Files identical despite different names*

### Comparing `tkmatrix-0.6.4/tkmatrix/tests/test_tkmatrix.py` & `tkmatrix-0.6.5/tkmatrix/tests/test_tkmatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,28 +31,28 @@
             self.assertAlmostEqual(0.5, matrix.mstar_max.value, 2)
             self.assertAlmostEqual(0.18, matrix.rstar.value, 2)
             self.assertAlmostEqual(0.076, matrix.rstar_min.value, 3)
             self.assertAlmostEqual(0.284, matrix.rstar_max.value, 3)
             self.assertEquals(".", matrix.dir)
             matrix.recovery(inject_dir, 5, detrend_ws=0, oversampling=0.1)
             matrix.plot_results(target, inject_dir)
-            self.assertEquals(8, len(os.listdir(inject_dir)))
+            self.assertEquals(9, len(os.listdir(inject_dir)))
         finally:
             if inject_dir is not None:
                 shutil.rmtree(inject_dir, ignore_errors=True)
 
     def test_inject_one_preserve(self):
         target = "TIC 220513363"
         matrix = MATRIX(target, [1], lcbuilder.constants.SPOC_AUTHOR, ".", True, exposure_time=120)
         inject_dir = None
         try:
             inject_dir, period_grid, radius_grid = matrix.inject(1, 5, 5, 1, 3, 3, 1)
             matrix.recovery(inject_dir, 5, detrend_ws=0, oversampling=0.1)
             matrix.plot_results(target, inject_dir)
-            self.assertEquals(9, len(os.listdir(inject_dir)))
+            self.assertEquals(10, len(os.listdir(inject_dir)))
         finally:
             if inject_dir is not None:
                 shutil.rmtree(inject_dir, ignore_errors=True)
 
     def test_inject_four(self):
         target = "TIC 220513363"
         matrix = MATRIX(target, [1], lcbuilder.constants.SPOC_AUTHOR, ".", exposure_time=120)
```

### Comparing `tkmatrix-0.6.4/tkmatrix/tkmatrix_class.py` & `tkmatrix-0.6.5/tkmatrix/tkmatrix_class.py`

 * *Files 3% similar despite different names*

```diff
@@ -406,50 +406,63 @@
         assert detrend_method == self.DETREND_GP or detrend_method == self.DETREND_BIWEIGHT
         if transit_template == 'tls':
             transit_template = 'default'
         elif transit_template == 'bls':
             transit_template = 'box'
         reports_df = pd.DataFrame(columns=['period', 'radius', 'epoch', 'duration_found', 'period_found', 'epoch_found',
                                            'found', 'snr', 'sde', 'run'])
+        run_reports_df = pd.DataFrame(columns=['period', 'radius', 'epoch', 'duration_found', 'period_found', 'epoch_found',
+                                           'found', 'snr', 'sde', 'run'])
         for file in sorted(os.listdir(inject_dir)):
             file_name_matches = re.search("P([0-9]+\\.*[0-9]*)+_R([0-9]+\\.*[0-9]*)_([0-9]+\\.*[0-9]*)\\.csv", file)
             if file_name_matches is not None:
                 try:
                     period = float(file_name_matches[1])
                     r_planet = float(file_name_matches[2])
                     epoch = float(file_name_matches[3])
                     df = pd.read_csv(inject_dir + file, float_precision='round_trip', sep=',',
                                      usecols=['#time', 'flux', 'flux_err'])
                     if len(df) == 0:
-                        found = True
-                        snr = 20
-                        sde = self.SDE_ROCHE
-                        run = 1
-                        duration_found = 20
-                        epoch_found = 0
-                        period_found = 0
+                        founds = [True]
+                        snrs = [20]
+                        sdes = [self.SDE_ROCHE]
+                        runs = [1]
+                        durations_found = [20]
+                        epochs_found = [0]
+                        periods_found = [0]
                     else:
                         self.retrieve_object_data_for_recovery(inject_dir + "/", inject_dir + file)
-                        found, snr, sde, run, duration_found, period_found, epoch_found = \
-                            self.__search(self.lc_build.lc.time.value, self.lc_build.lc.flux.value, self.radius, self.radiusmin,
-                                          self.radiusmax, self.mass, self.massmin,
+                        founds, snrs, sdes, runs, durations_found, periods_found, epochs_found = \
+                            self.__search(self.lc_build.lc.time.value, self.lc_build.lc.flux.value, self.radius,
+                                          self.radiusmin, self.radiusmax, self.mass, self.massmin,
                                           self.massmax, self.ab, epoch, period, self.MIN_SEARCH_PERIOD,
                                           max_period_search, snr_threshold,
                                           transit_template, detrend_method, detrend_ws,
                                           self.lc_build.transits_min_count, run_limit, custom_search_algorithm,
                                           oversampling, signal_selection_mode)
-                    new_report = {"period": period, "radius": r_planet, "epoch": epoch, "found": found, "snr": snr,
-                                  "sde": sde, "run": run, "duration_found": duration_found,
-                                  "period_found": period_found, "epoch_found": epoch_found}
+                    new_report = {"period": period, "radius": r_planet, "epoch": epoch,
+                                  "found": founds[-1], "snr": ','.join([str(i) for i in snrs]),
+                                  "sde": ','.join([str(i) for i in sdes]), "run": ','.join([str(i) for i in runs]),
+                                  "duration_found": ','.join([str(i) for i in durations_found]),
+                                  "period_found": ','.join([str(i) for i in periods_found]),
+                                  "epoch_found": ','.join([str(i) for i in epochs_found])}
                     reports_df = reports_df.append(new_report, ignore_index=True)
+                    for i in np.arange(0, len(founds)):
+                        run_reports_df = run_reports_df.append(
+                            {"period": period, "radius": r_planet, "epoch": epoch, "found": founds[i], "snr": snrs[i],
+                                  "sde": sdes[i], "run": runs[i], "duration_found": durations_found[i],
+                                  "period_found": periods_found[i], "epoch_found": epochs_found[i]}, ignore_index=True)
                     print("P=" + str(period) + ", R=" + str(r_planet) + ", T0=" + str(epoch) + ", FOUND WAS " + str(
-                        found) +
-                          " WITH SNR " + str(snr) + " AND SDE " + str(sde))
+                        founds[-1]) +
+                          " WITH SNRs " + str(snrs) + " AND SDEs " + str(sdes))
                     reports_df = reports_df.sort_values(['period', 'radius', 'epoch'], ascending=[True, True, True])
+                    run_reports_df = run_reports_df.sort_values(['period', 'radius', 'epoch', 'run'],
+                                                            ascending=[True, True, True, True])
                     reports_df.to_csv(inject_dir + "a_tls_report.csv", index=False)
+                    run_reports_df.to_csv(inject_dir + "a_tls_report_per_run.csv", index=False)
                 except Exception as e:
                     traceback.print_exc()
                     print("File not valid: " + file)
         self.remove_non_results_files(inject_dir)
 
     def remove_non_results_files(self, inject_dir):
         """
@@ -642,14 +655,21 @@
         if ws > 0:
             if detrend_method == self.DETREND_BIWEIGHT:
                 flux = wotan.flatten(time, flux, window_length=ws, return_trend=False, method=detrend_method,
                                      break_tolerance=0.5)
             elif detrend_method == self.DETREND_GP:
                 flux = wotan.flatten(time, flux, method=self.DETREND_GP, kernel='matern', kernel_size=ws,
                                      return_trend=False, break_tolerance=0.5)
+        found_signals = []
+        snrs = []
+        sdes = []
+        runs = []
+        durations = []
+        periods = []
+        t0s = []
         while snr >= min_snr and not found_signal and (run_limit > 0 and run < run_limit):
             model = transitleastsquares(time, flux)
             # R_starx = rstar / u.R_sun
             results = model.power(u=ab,
                                   R_star=rstar,  # rstar/u.R_sun,
                                   R_star_min=rstar_min,  # rstar_min/u.R_sun,
                                   R_star_max=rstar_max,  # rstar_max/u.R_sun,
@@ -667,25 +687,40 @@
             snr = results.snr
             if results.snr >= min_snr:
                 intransit_result = transit_mask(time, results.period, 2 * results.duration, results.T0)
                 time = time[~intransit_result]
                 flux = flux[~intransit_result]
                 time, flux = cleaned_array(time, flux)
                 if results.transit_times is not None and len(results.transit_times) > 0:
+                    print(f"Selecting signal with mode {signal_selection_mode}")
                     if signal_selection_mode == 'period-epoch':
                         found_signal = HarmonicSelector.is_harmonic(results.transit_times[0], epoch, results.period, period)
                     else:
                         found_signal = HarmonicSelector.multiple_of(results.period, period) != 0
                     # plt.plot(foldedleastsquares.fold(time, results.period, results.transit_times[0], flux))
                     # plt.xlim([0.4, 0.6])
                     # plt.show()
                     if found_signal:
+                        found_signals = found_signals + [found_signal]
+                        snrs = snrs + [results.snr]
+                        sdes = sdes + [results.SDE]
+                        runs = runs + [run]
+                        durations = durations + [results.duration]
+                        periods = periods + [results.period]
+                        t0s = t0s + [results.T0]
                         break
+            found_signals = found_signals + [found_signal]
+            snrs = snrs + [results.snr]
+            sdes = sdes + [results.SDE]
+            runs = runs + [run]
+            durations = durations + [results.duration]
+            periods = periods + [results.period]
+            t0s = t0s + [results.T0]
             run = run + 1
-        return found_signal, results.snr, results.SDE, run, results.duration, results.period, results.T0
+        return found_signals, snrs, sdes, runs, durations, periods, t0s
 
     @staticmethod
     def num_of_zeros(n):
         """
         Counts the number of zeros in a decimal
 
         :param n: the number
```

### Comparing `tkmatrix-0.6.4/tkmatrix.egg-info/PKG-INFO` & `tkmatrix-0.6.5/tkmatrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkmatrix
-Version: 0.6.4
+Version: 0.6.5
 Summary: ToolKit for Multi-phAse Transits Recovery from Injected eXoplanets
 Home-page: https://github.com/PlanetHunters/tkmatrix
 Author: M. Dévora-Pajares & F.J. Pozuelos
 Author-email: mdevorapajares@protonmail.com
 License: UNKNOWN
 Description: <p align="center">
           <img width="400px" src="https://github.com/martindevora/tkmatrix/blob/master/images/matrix.jpg?raw=true">
```

