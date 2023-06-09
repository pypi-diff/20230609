# Comparing `tmp/scientific_plots-1.4.8.tar.gz` & `tmp/scientific_plots-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientific_plots-1.4.8.tar", last modified: Mon Apr  3 13:48:11 2023, max compression
+gzip compressed data, was "scientific_plots-1.4.9.tar", last modified: Tue Apr  4 10:52:24 2023, max compression
```

## Comparing `scientific_plots-1.4.8.tar` & `scientific_plots-1.4.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.076795 scientific_plots-1.4.8/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-04-03 13:48:11.076795 scientific_plots-1.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1356 2023-04-03 13:24:41.000000 scientific_plots-1.4.8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1924 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/readme.md
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-03 13:48:11.076795 scientific_plots-1.4.8/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.068795 scientific_plots-1.4.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.068795 scientific_plots-1.4.8/src/cycler-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/cycler-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.068795 scientific_plots-1.4.8/src/hurst-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/hurst-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.068795 scientific_plots-1.4.8/src/matplotlib-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1526 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/animation.pyi
--rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/cm.pyi
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/colors.pyi
--rw-rw-rw-   0 root         (0) root         (0)      773 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/figure.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.072795 scientific_plots-1.4.8/src/matplotlib-stubs/pyplot/
--rw-rw-rw-   0 root         (0) root         (0)     5865 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/pyplot/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/pyplot/style.pyi
--rw-rw-rw-   0 root         (0) root         (0)      148 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/matplotlib-stubs/ticker.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.072795 scientific_plots-1.4.8/src/numba-stubs/
--rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/numba-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.072795 scientific_plots-1.4.8/src/python_translator-stubs/
--rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/python_translator-stubs/__init__.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.072795 scientific_plots-1.4.8/src/scientific_plots/
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-03 13:24:41.000000 scientific_plots-1.4.8/src/scientific_plots/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scientific_plots/data_analysis.py
--rw-rw-rw-   0 root         (0) root         (0)    18014 2023-04-03 13:24:41.000000 scientific_plots-1.4.8/src/scientific_plots/default_plots.py
--rw-rw-rw-   0 root         (0) root         (0)    15183 2023-04-03 08:09:55.000000 scientific_plots-1.4.8/src/scientific_plots/plot_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-03 13:47:45.000000 scientific_plots-1.4.8/src/scientific_plots/py.typed
--rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scientific_plots/two_d_plot.py
--rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scientific_plots/types_.py
--rw-rw-rw-   0 root         (0) root         (0)     9647 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scientific_plots/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.072795 scientific_plots-1.4.8/src/scientific_plots.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2407 2023-04-03 13:48:11.000000 scientific_plots-1.4.8/src/scientific_plots.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1289 2023-04-03 13:48:11.000000 scientific_plots-1.4.8/src/scientific_plots.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-03 13:48:11.000000 scientific_plots-1.4.8/src/scientific_plots.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      139 2023-04-03 13:48:11.000000 scientific_plots-1.4.8/src/scientific_plots.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-04-03 13:48:11.000000 scientific_plots-1.4.8/src/scientific_plots.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.076795 scientific_plots-1.4.8/src/scipy-stubs/
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/fft.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/integrate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/interpolate.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/optimize.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.076795 scientific_plots-1.4.8/src/scipy-stubs/signal/
--rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/signal/__init__.pyi
--rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/signal/windows.pyi
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/special.pyi
--rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/src/scipy-stubs/stats.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-03 13:48:11.076795 scientific_plots-1.4.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/tests/test_plot_manual.py
--rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/tests/test_plots.py
--rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.4.8/tests/test_utilties.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1356 2023-04-03 13:24:41.000000 scientific_plots-1.4.9/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1925 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/cycler-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      713 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/cycler-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/hurst-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/hurst-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/matplotlib-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1526 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/animation.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      318 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/cm.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/colors.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      773 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/figure.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/
+-rw-rw-rw-   0 root         (0) root         (0)     5979 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      298 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/style.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/matplotlib-stubs/ticker.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/numba-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/numba-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.806645 scientific_plots-1.4.9/src/python_translator-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/python_translator-stubs/__init__.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scientific_plots/
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/scientific_plots/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1298 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scientific_plots/data_analysis.py
+-rw-rw-rw-   0 root         (0) root         (0)    18014 2023-04-03 13:24:41.000000 scientific_plots-1.4.9/src/scientific_plots/default_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    15134 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/scientific_plots/plot_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-04 10:51:59.000000 scientific_plots-1.4.9/src/scientific_plots/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)     5485 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scientific_plots/two_d_plot.py
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scientific_plots/types_.py
+-rw-rw-rw-   0 root         (0) root         (0)     9674 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/src/scientific_plots/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scientific_plots.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      139 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-04-04 10:52:24.000000 scientific_plots-1.4.9/src/scientific_plots.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scipy-stubs/
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/fft.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/integrate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/interpolate.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/optimize.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.810645 scientific_plots-1.4.9/src/scipy-stubs/signal/
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/signal/__init__.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      271 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/signal/windows.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/special.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      301 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/src/scipy-stubs/stats.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-04 10:52:24.814645 scientific_plots-1.4.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1765 2023-04-04 10:41:15.000000 scientific_plots-1.4.9/tests/test_plot_manual.py
+-rw-rw-rw-   0 root         (0) root         (0)     3093 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/tests/test_plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      710 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      807 2023-04-02 22:54:17.000000 scientific_plots-1.4.9/tests/test_utilties.py
```

### Comparing `scientific_plots-1.4.8/PKG-INFO` & `scientific_plots-1.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific_plots
-Version: 1.4.8
+Version: 1.4.9
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 Keywords: Plotting,science,library,utilities,styling
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -50,15 +50,15 @@
 for new plots.
 
 Alternatively, this package provides default plot settings in the submodule
 *default_plots*. The provided function apply a default design, which should
 look good in most situations.
 
 ```
-from scientifc_plots.default_plots import plot
+from scientific_plots.default_plots import plot
 
 plot(x, y, "x_label", "y_label", "subfolder/filename.pdf")
 ```
 
 ## Types
 Additional Vector like types for numpy-arrays are provided in
 `scientifc_plots.types_`.  These types can be used for static type checking
```

### Comparing `scientific_plots-1.4.8/pyproject.toml` & `scientific_plots-1.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/readme.md` & `scientific_plots-1.4.9/readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 for new plots.
 
 Alternatively, this package provides default plot settings in the submodule
 *default_plots*. The provided function apply a default design, which should
 look good in most situations.
 
 ```
-from scientifc_plots.default_plots import plot
+from scientific_plots.default_plots import plot
 
 plot(x, y, "x_label", "y_label", "subfolder/filename.pdf")
 ```
 
 ## Types
 Additional Vector like types for numpy-arrays are provided in
 `scientifc_plots.types_`.  These types can be used for static type checking
```

### Comparing `scientific_plots-1.4.8/src/cycler-stubs/__init__.pyi` & `scientific_plots-1.4.9/src/cycler-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/matplotlib-stubs/__init__.pyi` & `scientific_plots-1.4.9/src/matplotlib-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/matplotlib-stubs/colors.pyi` & `scientific_plots-1.4.9/src/matplotlib-stubs/colors.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/matplotlib-stubs/figure.pyi` & `scientific_plots-1.4.9/src/matplotlib-stubs/figure.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/matplotlib-stubs/pyplot/__init__.pyi` & `scientific_plots-1.4.9/src/matplotlib-stubs/pyplot/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,18 @@
     def get_xlabel(self) -> str: ...
 
     def set_frame_on(self, value: bool) -> str: ...
 
     def tick_params(self, axis: str = "x",
                     colors: str = "") -> None: ...
 
+    def ticklabel_format(
+        self,
+        useLocale: bool = False, useMathText: bool = False) -> None: ...
+
 
 def figure(figsize: Optional[Tuple[float, float]] = None) -> Figure: ...
 
 
 def close(fig: Union[Figure, str, None] = None) -> None: ...
```

### Comparing `scientific_plots-1.4.8/src/numba-stubs/__init__.pyi` & `scientific_plots-1.4.9/src/numba-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scientific_plots/data_analysis.py` & `scientific_plots-1.4.9/src/scientific_plots/data_analysis.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scientific_plots/default_plots.py` & `scientific_plots-1.4.9/src/scientific_plots/default_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scientific_plots/plot_settings.py` & `scientific_plots-1.4.9/src/scientific_plots/plot_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 from textwrap import dedent
 
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 from matplotlib.pyplot import Axes
 from matplotlib import colors
 from matplotlib import cm
-from matplotlib import ticker
 from cycler import cycler
 import numpy as np
 
 from .utilities import translate
 from .types_ import Vector
 
 mpl.use("Agg")
@@ -121,20 +120,21 @@
 
 def _germanify(ax: Axes, reverse: bool = False) -> None:
     """
     translate a figure from english to german.
     The direction can be reversed, if reverse it set to True
     Use the decorator instead
     """
+
     for axi in ax.figure.axes:
-        # axi.ticklabel_format(useMathText=False)
-        axi.yaxis.set_major_formatter(
-            ticker.StrMethodFormatter("{x:g}".replace(".", ",")))
-        axi.xaxis.set_major_formatter(
-            ticker.StrMethodFormatter("{x:g}".replace(".", ",")))
+        try:
+            axi.ticklabel_format(
+                useLocale=True)
+        except AttributeError:
+            pass
         items = [
             axi.xaxis.label,
             axi.yaxis.label,
             *axi.get_xticklabels(),
             *axi.get_yticklabels(),
         ]
         if axi.get_legend():
@@ -157,27 +157,29 @@
     the translation in the other direction. If reverse is set to false, no
     reversal of the translation will be applied.
     """
     old_locale = locale.getlocale(locale.LC_NUMERIC)
     try:
         try:
             locale.setlocale(locale.LC_ALL, "de_DE")
+            locale.setlocale(locale.LC_NUMERIC, "de_DE")
         except locale.Error:
             # locale not available
             pass
         plt.rcParams["axes.formatter.use_locale"] = True
         _germanify(ax)
         yield
     except Exception as e:
         print("Translation of the plot has failed")
         print(e)
         raise
     finally:
         try:
             locale.setlocale(locale.LC_ALL, old_locale)
+            locale.setlocale(locale.LC_ALL, old_locale)
         except locale.Error:
             pass
         plt.rcParams["axes.formatter.use_locale"] = False
         if reverse:
             _germanify(ax, reverse=True)
```

### Comparing `scientific_plots-1.4.8/src/scientific_plots/two_d_plot.py` & `scientific_plots-1.4.9/src/scientific_plots/two_d_plot.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scientific_plots/types_.py` & `scientific_plots-1.4.9/src/scientific_plots/types_.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scientific_plots/utilities.py` & `scientific_plots-1.4.9/src/scientific_plots/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,14 +274,15 @@
         "simulation": "Simulation",
         "Simulation": "Simulation",
         "analytical": "analytisch",
         "Analytical": "Analytisch",
         "signal": "Signal",
         "off": "zu",
         "on": "auf",
+        "valve": "Ventil",
         "relative pressure": "Relativdruck",
         "absolute pressure": "Absolutdruck",
         "relative": "relativ",
         "absolute": "absolut"
     })
     if not reverse:
         for key, value in _dict.items():
```

### Comparing `scientific_plots-1.4.8/src/scientific_plots.egg-info/PKG-INFO` & `scientific_plots-1.4.9/src/scientific_plots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientific-plots
-Version: 1.4.8
+Version: 1.4.9
 Summary: Useful methods for plots used in science
 Author-email: Felix Fischer <f.fischer@ifas.rwth-aachen.de>
 Keywords: Plotting,science,library,utilities,styling
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
@@ -50,15 +50,15 @@
 for new plots.
 
 Alternatively, this package provides default plot settings in the submodule
 *default_plots*. The provided function apply a default design, which should
 look good in most situations.
 
 ```
-from scientifc_plots.default_plots import plot
+from scientific_plots.default_plots import plot
 
 plot(x, y, "x_label", "y_label", "subfolder/filename.pdf")
 ```
 
 ## Types
 Additional Vector like types for numpy-arrays are provided in
 `scientifc_plots.types_`.  These types can be used for static type checking
```

### Comparing `scientific_plots-1.4.8/src/scientific_plots.egg-info/SOURCES.txt` & `scientific_plots-1.4.9/src/scientific_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scipy-stubs/fft.pyi` & `scientific_plots-1.4.9/src/scipy-stubs/fft.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scipy-stubs/integrate.pyi` & `scientific_plots-1.4.9/src/scipy-stubs/integrate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scipy-stubs/interpolate.pyi` & `scientific_plots-1.4.9/src/scipy-stubs/interpolate.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scipy-stubs/optimize.pyi` & `scientific_plots-1.4.9/src/scipy-stubs/optimize.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/src/scipy-stubs/signal/__init__.pyi` & `scientific_plots-1.4.9/src/scipy-stubs/signal/__init__.pyi`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/tests/test_plot_manual.py` & `scientific_plots-1.4.9/tests/test_plot_manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,13 +48,13 @@
         filename, color=(3, 4, 5))
     assert filename.exists()
 
 
 @mark.use_style
 def test_skip_color() -> None:
     """Test the skipping of a color in the cycle."""
-    x_test: Vector = linspace(1., 100., 100)
+    x_test: Vector = linspace(1., 2., 100)
     y_test1: Vector = x_test**2
     filename = LOCATION3
     filename.parent.mkdir(exist_ok=True)
     plot(x_test, y_test1, "x", "y", filename, cycler=1)
     assert filename.exists()
```

### Comparing `scientific_plots-1.4.8/tests/test_plots.py` & `scientific_plots-1.4.9/tests/test_plots.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/tests/test_types.py` & `scientific_plots-1.4.9/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `scientific_plots-1.4.8/tests/test_utilties.py` & `scientific_plots-1.4.9/tests/test_utilties.py`

 * *Files identical despite different names*

