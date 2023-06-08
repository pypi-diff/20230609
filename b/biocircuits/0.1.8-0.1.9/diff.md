# Comparing `tmp/biocircuits-0.1.8.tar.gz` & `tmp/biocircuits-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocircuits-0.1.8.tar", last modified: Tue Apr 19 20:47:18 2022, max compression
+gzip compressed data, was "biocircuits-0.1.9.tar", last modified: Sat Apr  1 04:08:41 2023, max compression
```

## Comparing `biocircuits-0.1.8.tar` & `biocircuits-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2022-04-19 20:47:18.644120 biocircuits-0.1.8/
--rw-r--r--   0 bois       (501) staff       (20)     2699 2019-03-29 05:51:59.000000 biocircuits-0.1.8/LICENSE.md
--rw-r--r--   0 bois       (501) staff       (20)       42 2019-03-29 05:51:59.000000 biocircuits-0.1.8/MANIFEST.in
--rw-r--r--   0 bois       (501) staff       (20)      834 2022-04-19 20:47:18.644242 biocircuits-0.1.8/PKG-INFO
--rw-r--r--   0 bois       (501) staff       (20)      314 2022-04-01 16:35:29.000000 biocircuits-0.1.8/README.md
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2022-04-19 20:47:18.637535 biocircuits-0.1.8/biocircuits/
--rw-r--r--   0 bois       (501) staff       (20)      362 2022-04-19 20:46:30.000000 biocircuits-0.1.8/biocircuits/__init__.py
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2022-04-19 20:47:18.643063 biocircuits-0.1.8/biocircuits/apps/
--rw-r--r--   0 bois       (501) staff       (20)       46 2021-04-06 17:02:35.000000 biocircuits-0.1.8/biocircuits/apps/__init__.py
--rw-r--r--   0 bois       (501) staff       (20)    10249 2022-04-04 17:57:44.000000 biocircuits-0.1.8/biocircuits/apps/ffl.py
--rw-r--r--   0 bois       (501) staff       (20)      109 2022-04-04 17:57:53.000000 biocircuits-0.1.8/biocircuits/apps/ffl_app.py
--rw-r--r--   0 bois       (501) staff       (20)    32299 2021-04-06 22:02:17.000000 biocircuits-0.1.8/biocircuits/apps/promiscuous.py
--rw-r--r--   0 bois       (501) staff       (20)     4518 2021-04-02 06:26:33.000000 biocircuits-0.1.8/biocircuits/dynsys.py
--rw-r--r--   0 bois       (501) staff       (20)    15329 2021-05-12 19:16:08.000000 biocircuits-0.1.8/biocircuits/gillespie.py
--rw-r--r--   0 bois       (501) staff       (20)    40691 2022-04-19 20:45:49.000000 biocircuits-0.1.8/biocircuits/jsfunctions.py
--rw-r--r--   0 bois       (501) staff       (20)    32874 2022-04-19 20:45:35.000000 biocircuits-0.1.8/biocircuits/jsplots.py
--rw-r--r--   0 bois       (501) staff       (20)     7949 2021-03-27 23:10:55.000000 biocircuits-0.1.8/biocircuits/rd.py
--rw-r--r--   0 bois       (501) staff       (20)     7008 2021-04-28 15:55:03.000000 biocircuits-0.1.8/biocircuits/reg.py
--rw-r--r--   0 bois       (501) staff       (20)     1375 2020-04-23 19:09:54.000000 biocircuits-0.1.8/biocircuits/utils.py
--rw-r--r--   0 bois       (501) staff       (20)    47100 2022-02-12 06:50:34.000000 biocircuits-0.1.8/biocircuits/viz.py
-drwxr-xr-x   0 bois       (501) staff       (20)        0 2022-04-19 20:47:18.640938 biocircuits-0.1.8/biocircuits.egg-info/
--rw-r--r--   0 bois       (501) staff       (20)      834 2022-04-19 20:47:18.000000 biocircuits-0.1.8/biocircuits.egg-info/PKG-INFO
--rw-r--r--   0 bois       (501) staff       (20)      553 2022-04-19 20:47:18.000000 biocircuits-0.1.8/biocircuits.egg-info/SOURCES.txt
--rw-r--r--   0 bois       (501) staff       (20)        1 2022-04-19 20:47:18.000000 biocircuits-0.1.8/biocircuits.egg-info/dependency_links.txt
--rw-r--r--   0 bois       (501) staff       (20)       74 2022-04-19 20:47:18.000000 biocircuits-0.1.8/biocircuits.egg-info/requires.txt
--rw-r--r--   0 bois       (501) staff       (20)       12 2022-04-19 20:47:18.000000 biocircuits-0.1.8/biocircuits.egg-info/top_level.txt
--rw-r--r--   0 bois       (501) staff       (20)       73 2021-04-23 16:58:50.000000 biocircuits-0.1.8/requirements.txt
--rw-r--r--   0 bois       (501) staff       (20)      108 2022-04-19 20:47:18.644714 biocircuits-0.1.8/setup.cfg
--rw-r--r--   0 bois       (501) staff       (20)     1364 2022-04-19 20:46:18.000000 biocircuits-0.1.8/setup.py
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2023-04-01 04:08:41.967606 biocircuits-0.1.9/
+-rwxr--r--   0 bois       (501) staff       (20)     2699 2019-03-29 05:51:59.000000 biocircuits-0.1.9/LICENSE.md
+-rwxr--r--   0 bois       (501) staff       (20)       42 2019-03-29 05:51:59.000000 biocircuits-0.1.9/MANIFEST.in
+-rw-r--r--   0 bois       (501) staff       (20)      815 2023-04-01 04:08:41.967720 biocircuits-0.1.9/PKG-INFO
+-rwxr--r--   0 bois       (501) staff       (20)      314 2022-04-01 16:35:29.000000 biocircuits-0.1.9/README.md
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2023-04-01 04:08:41.962148 biocircuits-0.1.9/biocircuits/
+-rwxr--r--   0 bois       (501) staff       (20)      362 2023-04-01 04:07:00.000000 biocircuits-0.1.9/biocircuits/__init__.py
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2023-04-01 04:08:41.967166 biocircuits-0.1.9/biocircuits/apps/
+-rwxr--r--   0 bois       (501) staff       (20)       46 2021-04-06 17:01:56.000000 biocircuits-0.1.9/biocircuits/apps/__init__.py
+-rwxr--r--   0 bois       (501) staff       (20)    10249 2022-04-04 17:57:44.000000 biocircuits-0.1.9/biocircuits/apps/ffl.py
+-rwxr--r--   0 bois       (501) staff       (20)      109 2022-04-04 17:57:53.000000 biocircuits-0.1.9/biocircuits/apps/ffl_app.py
+-rwxr--r--   0 bois       (501) staff       (20)    32299 2021-04-06 22:02:17.000000 biocircuits-0.1.9/biocircuits/apps/promiscuous.py
+-rwxr--r--   0 bois       (501) staff       (20)      121 2022-06-29 13:49:34.000000 biocircuits-0.1.9/biocircuits/apps/promiscuous_app.py
+-rwxr--r--   0 bois       (501) staff       (20)     4518 2021-04-02 06:26:29.000000 biocircuits-0.1.9/biocircuits/dynsys.py
+-rwxr--r--   0 bois       (501) staff       (20)    16498 2022-08-11 08:21:30.000000 biocircuits-0.1.9/biocircuits/gillespie.py
+-rwxr--r--   0 bois       (501) staff       (20)    41333 2022-04-29 08:23:01.000000 biocircuits-0.1.9/biocircuits/jsfunctions.py
+-rwxr--r--   0 bois       (501) staff       (20)    34708 2022-04-29 08:23:25.000000 biocircuits-0.1.9/biocircuits/jsplots.py
+-rwxr--r--   0 bois       (501) staff       (20)     7949 2021-03-27 23:10:55.000000 biocircuits-0.1.9/biocircuits/rd.py
+-rwxr--r--   0 bois       (501) staff       (20)     7008 2021-04-28 15:55:03.000000 biocircuits-0.1.9/biocircuits/reg.py
+-rwxr--r--   0 bois       (501) staff       (20)     6615 2022-07-16 23:26:55.000000 biocircuits-0.1.9/biocircuits/test.py
+-rwxr--r--   0 bois       (501) staff       (20)      469 2022-07-13 14:27:03.000000 biocircuits-0.1.9/biocircuits/test2.py
+-rwxr--r--   0 bois       (501) staff       (20)     1375 2020-04-23 19:09:54.000000 biocircuits-0.1.9/biocircuits/utils.py
+-rwxr--r--   0 bois       (501) staff       (20)    48709 2022-07-16 23:27:17.000000 biocircuits-0.1.9/biocircuits/viz.py
+drwxr-xr-x   0 bois       (501) staff       (20)        0 2023-04-01 04:08:41.964506 biocircuits-0.1.9/biocircuits.egg-info/
+-rwxr--r--   0 bois       (501) staff       (20)      815 2023-04-01 04:08:41.000000 biocircuits-0.1.9/biocircuits.egg-info/PKG-INFO
+-rwxr--r--   0 bois       (501) staff       (20)      630 2023-04-01 04:08:41.000000 biocircuits-0.1.9/biocircuits.egg-info/SOURCES.txt
+-rwxr--r--   0 bois       (501) staff       (20)        1 2023-04-01 04:08:41.000000 biocircuits-0.1.9/biocircuits.egg-info/dependency_links.txt
+-rwxr--r--   0 bois       (501) staff       (20)       74 2023-04-01 04:08:41.000000 biocircuits-0.1.9/biocircuits.egg-info/requires.txt
+-rwxr--r--   0 bois       (501) staff       (20)       12 2023-04-01 04:08:41.000000 biocircuits-0.1.9/biocircuits.egg-info/top_level.txt
+-rwxr--r--   0 bois       (501) staff       (20)       73 2021-04-23 16:58:50.000000 biocircuits-0.1.9/requirements.txt
+-rwxr--r--   0 bois       (501) staff       (20)      108 2023-04-01 04:08:41.968160 biocircuits-0.1.9/setup.cfg
+-rwxr--r--   0 bois       (501) staff       (20)     1364 2023-04-01 04:06:32.000000 biocircuits-0.1.9/setup.py
```

### Comparing `biocircuits-0.1.8/LICENSE.md` & `biocircuits-0.1.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/PKG-INFO` & `biocircuits-0.1.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: biocircuits
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities to accompany *Biological Circuit Design* by Michael Elowitz and Justin Bois.
 Home-page: https://github.com/justinbois/biocircuits
+Download-URL: https://github.com/justinbois/biocircuits/tarball/0.1.9
 Author: Justin Bois
 Author-email: bois@caltech.edu
 License: BSD
-Download-URL: https://github.com/justinbois/biocircuits/tarball/0.1.8
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.md
 
 # biocircuits
 
@@ -24,8 +23,7 @@
 
     pip install biocircuits
 
 
 ## Documentation
 
 You can access the docs from the [Biological Circuit Design website](https://biocircuits.github.io/package_docs/index.html).
-
```

### Comparing `biocircuits-0.1.8/biocircuits/apps/ffl.py` & `biocircuits-0.1.9/biocircuits/apps/ffl.py`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/biocircuits/apps/promiscuous.py` & `biocircuits-0.1.9/biocircuits/apps/promiscuous.py`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/biocircuits/dynsys.py` & `biocircuits-0.1.9/biocircuits/dynsys.py`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/biocircuits/gillespie.py` & `biocircuits-0.1.9/biocircuits/gillespie.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,14 +45,18 @@
     """
     # Update propensities
     propensity_func(propensities, population, t, *args)
 
     # Sum of propensities
     props_sum = _sum(propensities)
 
+    # Bail if the sum of propensities is zero (no moves to make)
+    if props_sum == 0.0:
+        return -1, -1.0
+
     # Compute time
     time = _draw_time(props_sum)
 
     # Draw reaction given propensities
     rxn = _sample_discrete(propensities, props_sum)
 
     return rxn, time
@@ -81,35 +85,38 @@
     pop_out[0, :] = population
     propensities = np.zeros(update.shape[0])
     while j < len(time_points):
         while t < time_points[j_time]:
             # draw the event and time step
             event, dt = draw_fun(propensity_func, propensities, population, t, args)
 
-            # Update the population
-            _copy_population(population_previous, population)
-            population += update[event, :]
+            if event == -1:
+                # Skip to the end of the simulation with the same population
+                t = time_points[-1]
+            else:
+                # Update the population
+                _copy_population(population_previous, population)
+                population += update[event, :]
 
-            # Increment time
-            t += dt
+                # Increment time
+                t += dt
 
         # Update the index (Have to be careful about types for Numba)
         j = np.searchsorted((time_points > t).astype(np.int64), 1)
 
         # Update the population
         for k in np.arange(j_time, min(j, len(time_points))):
             pop_out[k, :] = population_previous
 
         # Increment index
         j_time = j
 
     return pop_out, None
 
 
-@numba.njit
 def _gillespie_trajectory_report_time_points(
     propensity_func, update, population_0, time_points, draw_fun, args=()
 ):
     # Number of iterations before concatenating arrays
     n_iter = 1000
 
     # Initialize arrays for storing trajectories
@@ -125,20 +132,28 @@
     j = 0
     while t < time_points[-1]:
         i = 0
         while i < n_iter and t < time_points[-1]:
             # draw the event and time step
             event, dt = draw_fun(propensity_func, propensities, population, t, args)
 
+            if event == -1:
+                # Skip to the end of the simulation with the same population
+                t = time_points[-1]
+            else:
+                # New population
+                population += update[event, :]
+
+                # Increment time
+                t += dt
+
             # Update the population
-            population += update[event, :]
             pop[i, :] = population
 
-            # Increment time
-            t += dt
+            # Updated time
             tp[i] = t
 
             # Increment indexes
             i += 1
             j += 1
 
         # Add this subtrajectory to output
@@ -222,14 +237,18 @@
             """
             # Compute propensities
             propensity_func(propensities, population, t, *args)
 
             # Sum of propensities
             props_sum = np.sum(propensities)
 
+            # Bail if the sum of propensities is zero
+            if props_sum == 0.0:
+                return -1, -1.0
+
             # Compute time
             time = np.random.exponential(1 / props_sum)
 
             # Draw reaction given propensities
             rxn = _sample_discrete(propensities, props_sum)
 
             return rxn, time
@@ -254,20 +273,28 @@
                 j = 0
                 while t < time_points[-1]:
                     i = 0
                     while i < n_iter and t < time_points[-1]:
                         # draw the event and time step
                         event, dt = _draw(propensities, population, t)
 
+                        if event == -1:
+                            # Skip to the end of the simulation with the same population
+                            t = time_points[-1]
+                        else:
+                            # New population
+                            population += update[event, :]
+
+                            # Increment time
+                            t += dt
+
                         # Update the population
-                        population += update[event, :]
                         pop[i, :] = population
 
-                        # Increment time
-                        t += dt
+                        # Updated time
                         tp[i] = t
 
                         # Increment indexes
                         i += 1
                         j += 1
 
                     # Add this subtrajectory to output
@@ -295,20 +322,24 @@
                 pop_out[0, :] = population
                 propensities = np.zeros(update.shape[0])
                 while j < len(time_points):
                     while t < time_points[j_time]:
                         # draw the event and time step
                         event, dt = _draw(propensities, population, t)
 
-                        # Update the population
-                        _copy_population(population_previous, population)
-                        population += update[event, :]
+                        if event == -1:
+                            # Skip to the end of the simulation with the same population
+                            t = time_points[-1]
+                        else:
+                            # Update the population
+                            _copy_population(population_previous, population)
+                            population += update[event, :]
 
-                        # Increment time
-                        t += dt
+                            # Increment time
+                            t += dt
 
                     # Update the index (Be careful about types for Numba)
                     j = np.searchsorted((time_points > t).astype(np.int64), 1)
 
                     # Update the population
                     for k in np.arange(j_time, min(j, len(time_points))):
                         pop_out[k, :] = population_previous
@@ -317,15 +348,15 @@
                     j_time = j
 
                 return pop_out, None
 
     else:
         if return_time_points:
 
-            def traj():
+            def _traj():
                 return _gillespie_trajectory_report_time_points(
                     propensity_func,
                     update,
                     population_0,
                     time_points,
                     _gillespie_draw,
                     args=args,
@@ -367,15 +398,15 @@
     for i in iterator:
         pop_out[i], t_out[i] = _traj()
 
     return pop_out, t_out
 
 
 def _gillespie_multi_fn(args):
-    """Convenient function for multithreading."""
+    """Convenience function for multithreading."""
     return _gillespie_ssa(*args)
 
 
 def gillespie_ssa(
     propensity_func,
     update,
     population_0,
```

### Comparing `biocircuits-0.1.8/biocircuits/jsfunctions.py` & `biocircuits-0.1.9/biocircuits/jsfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1613,14 +1613,42 @@
 	cds.data['x2'] = xSolve[4];
 	cds.data['x3'] = xSolve[5];
 
 	cds.change.emit();
 }
 
 """,
+    "simple_binding_sensitivity": """
+function sensitivity(a0, b0, Kd) {
+	let b = a0 - b0 - Kd;
+	let discrim = b * b + 4 * a0 * Kd;
+	let sqrtDiscrim = Math.sqrt(discrim);
+
+	return a0 * (1 - b / sqrtDiscrim) / (sqrtDiscrim - b);
+}
+
+
+function callback() {
+    let b0 = Math.pow(10, b0Slider.value);
+    let KdVals = [0.001, 0.01, 0.1, 1.0, 10.0];        
+    let a0 = cds.data['a0'];
+    
+    for (let i = 0; i < KdVals.length; i++) {
+    	let ind = 's' + i.toString();
+    	for (let j = 0; j < a0.length; j++) {
+    		cds.data[ind][j] = sensitivity(a0[j], b0, KdVals[i]);
+    	}
+    }
+
+    span.location = b0;
+
+    cds.change.emit();
+}
+
+""",
     "toggle_nullclines": """
 function f(x, beta, n) {return beta / (1.0 + Math.pow(x, n));}
 
 
 function ff(x, betax, nx, betay, ny) {
     return betax / (1.0 + Math.pow(f(x, betay, ny), nx));
 }
@@ -1754,8 +1782,8 @@
 
     // Emit changes
     cds.change.emit();
     cdsStable.change.emit();
     cdsUnstable.change.emit();
 }
 """,
-}
+}
```

### Comparing `biocircuits-0.1.8/biocircuits/jsplots.py` & `biocircuits-0.1.9/biocircuits/jsplots.py`

 * *Files 2% similar despite different names*

```diff
@@ -714,18 +714,15 @@
     # Obtain solution for plot
     t, x = _solve_repressilator(beta_slider.value, n_slider.value, 40.0)
 
     # Build the plot
     colors = colorcet.b_glasbey_category10[:3]
 
     p_rep = bokeh.plotting.figure(
-        frame_width=550,
-        frame_height=200,
-        x_axis_label="t",
-        x_range=[0, 40.0],
+        frame_width=550, frame_height=200, x_axis_label="t", x_range=[0, 40.0],
     )
 
     cds = bokeh.models.ColumnDataSource(data=dict(t=t, x1=x[0], x2=x[1], x3=x[2]))
     labels = dict(x1="x₁", x2="x₂", x3="x₃")
     for color, x_val in zip(colors, labels):
         p_rep.line(
             source=cds,
@@ -749,22 +746,19 @@
     js_code = (
         jsfuns["reg"]
         + jsfuns["ode"]
         + jsfuns["circuits"]
         + jsfuns["utils"]
         + jsfuns["linalg"]
         + jsfuns["proteinRepressilator"]
-        + 'callback()'
+        + "callback()"
     )
     callback = bokeh.models.CustomJS(
         args=dict(
-            cds=cds,
-            xRange=p_rep.x_range,
-            betaSlider=beta_slider,
-            nSlider=n_slider,
+            cds=cds, xRange=p_rep.x_range, betaSlider=beta_slider, nSlider=n_slider,
         ),
         code=js_code,
     )
 
     beta_slider.js_on_change("value", callback)
     n_slider.js_on_change("value", callback)
     p_rep.x_range.js_on_change("end", callback)
@@ -790,35 +784,40 @@
     # Sliders
     beta_slider = bokeh.models.Slider(
         title="β",
         start=0,
         end=4,
         step=0.1,
         value=1,
-        format=bokeh.models.FuncTickFormatter(code="return Math.pow(10, tick).toFixed(2)"),
+        format=bokeh.models.FuncTickFormatter(
+            code="return Math.pow(10, tick).toFixed(2)"
+        ),
     )
     gamma_slider = bokeh.models.Slider(
         title="γ",
         start=-3,
         end=0,
         step=0.1,
         value=0,
-        format=bokeh.models.FuncTickFormatter(code="return Math.pow(10, tick).toFixed(3)"),
+        format=bokeh.models.FuncTickFormatter(
+            code="return Math.pow(10, tick).toFixed(3)"
+        ),
     )
     rho_slider = bokeh.models.Slider(
         title="ρ",
         start=-6,
         end=0,
         step=0.1,
         value=-3,
-        format=bokeh.models.FuncTickFormatter(code="return Math.pow(10, tick).toFixed(6)"),
+        format=bokeh.models.FuncTickFormatter(
+            code="return Math.pow(10, tick).toFixed(6)"
+        ),
     )
     n_slider = bokeh.models.Slider(title="n", start=1, end=5, step=0.1, value=3)
 
-
     def repressilator_rhs(mx, t, beta, gamma, rho, n):
         """
         Returns 6-array of (dm_1/dt, dm_2/dt, dm_3/dt, dx_1/dt, dx_2/dt, dx_3/dt)
         """
         m_1, m_2, m_3, x_1, x_2, x_3 = mx
         return np.array(
             [
@@ -827,15 +826,14 @@
                 beta * (rho + 1 / (1 + x_2 ** n)) - m_3,
                 gamma * (m_1 - x_1),
                 gamma * (m_2 - x_2),
                 gamma * (m_3 - x_3),
             ]
         )
 
-
     # Initial condiations
     x0 = np.array([0, 0, 0, 1, 1.1, 1.2])
 
     # Number of points to use in plots
     n_points = 1000
 
     # Solve for species concentrations
@@ -844,32 +842,24 @@
         gamma = 10 ** log_gamma
         rho = 10 ** log_rho
         t = np.linspace(0, t_max, n_points)
         x = scipy.integrate.odeint(repressilator_rhs, x0, t, args=(beta, gamma, rho, n))
         m1, m2, m3, x1, x2, x3 = x.transpose()
         return t, m1, m2, m3, x1, x2, x3
 
-
     t, m1, m2, m3, x1, x2, x3 = _solve_repressilator(
-        beta_slider.value,
-        gamma_slider.value,
-        rho_slider.value,
-        n_slider.value,
-        40.0,
+        beta_slider.value, gamma_slider.value, rho_slider.value, n_slider.value, 40.0,
     )
 
     cds = bokeh.models.ColumnDataSource(
         dict(t=t, m1=m1, m2=m2, m3=m3, x1=x1, x2=x2, x3=x3)
     )
 
     p = bokeh.plotting.figure(
-        frame_width=500,
-        frame_height=200,
-        x_axis_label="t",
-        x_range=[0, 40.0],
+        frame_width=500, frame_height=200, x_axis_label="t", x_range=[0, 40.0],
     )
 
     colors = bokeh.palettes.d3["Category20"][6]
     m1_line = p.line(source=cds, x="t", y="m1", line_width=2, color=colors[1])
     x1_line = p.line(source=cds, x="t", y="x1", line_width=2, color=colors[0])
     m2_line = p.line(source=cds, x="t", y="m2", line_width=2, color=colors[3])
     x2_line = p.line(source=cds, x="t", y="x2", line_width=2, color=colors[2])
@@ -881,40 +871,34 @@
         ("x₁", [x1_line]),
         ("m₂", [m2_line]),
         ("x₂", [x2_line]),
         ("m₃", [m3_line]),
         ("x₃", [x3_line]),
     ]
     legend = bokeh.models.Legend(items=legend_items)
-    legend.click_policy = 'hide'
+    legend.click_policy = "hide"
 
     p.add_layout(legend, "right")
 
     # Build the layout
     layout = bokeh.layouts.column(
-        bokeh.layouts.row(
-            beta_slider,
-            gamma_slider,
-            rho_slider,
-            n_slider,
-            width=575,
-        ),
+        bokeh.layouts.row(beta_slider, gamma_slider, rho_slider, n_slider, width=575,),
         bokeh.layouts.Spacer(height=10),
         p,
     )
 
     # Set up callbacks
     js_code = (
         jsfuns["reg"]
         + jsfuns["ode"]
         + jsfuns["circuits"]
         + jsfuns["utils"]
         + jsfuns["linalg"]
         + jsfuns["repressilator"]
-        + 'callback()'
+        + "callback()"
     )
     callback = bokeh.models.CustomJS(
         args=dict(
             cds=cds,
             xRange=p.x_range,
             betaSlider=beta_slider,
             rhoSlider=rho_slider,
@@ -929,14 +913,88 @@
     rho_slider.js_on_change("value", callback)
     n_slider.js_on_change("value", callback)
     p.x_range.js_on_change("end", callback)
 
     return layout
 
 
+def simple_binding_sensitivity():
+    """Make a simple plot of sensitivity for binding of A and B.
+    """
+
+    def sensitivity(a_tot, b_tot, Kd):
+        b = a_tot - b_tot - Kd
+        discrim = b ** 2 + 4 * a_tot * Kd
+
+        return a_tot * (1 - b / np.sqrt(discrim)) / (-b + np.sqrt(discrim))
+
+    a_tot = np.logspace(-2, 2, 1001)
+    b_tot = 1.0
+    Kd_vals = np.logspace(-3, 1, 5)
+
+    colors = bokeh.palettes.Blues9[3:8]
+
+    b0_slider = bokeh.models.Slider(
+        title="total B conc. (µM)",
+        start=-1,
+        end=1,
+        value=np.log10(b_tot),
+        step=0.01,
+        width=200,
+        format=bokeh.models.FuncTickFormatter(
+            code="return Math.pow(10, tick).toFixed(2)"
+        ),
+    )
+
+    p = bokeh.plotting.figure(
+        frame_width=400,
+        height=325,
+        x_axis_label="total A conc. (µM)",
+        y_axis_label="sensitivity",
+        x_axis_type="log",
+        y_axis_type="log",
+        x_range=[a_tot.min(), a_tot.max()],
+    )
+
+    cds = bokeh.models.ColumnDataSource(
+        {
+            **{"a0": a_tot},
+            **{f"s{i}": sensitivity(a_tot, b_tot, Kd) for i, Kd in enumerate(Kd_vals)},
+        }
+    )
+
+    for i, (color, Kd) in enumerate(zip(colors, Kd_vals)):
+        p.line(
+            source=cds,
+            x="a0",
+            y=f"s{i}",
+            line_width=2,
+            color=color,
+            legend_label=str(Kd) + " µM",
+        )
+
+    span = bokeh.models.Span(location=10 ** b0_slider.value, dimension="height")
+    p.add_layout(span)
+
+    p.legend.location = "bottom_right"
+    p.legend.title = "Kd"
+
+    # Set up callbacks
+    js_code = jsfuns["simple_binding_sensitivity"] + "callback()"
+    callback = bokeh.models.CustomJS(
+        args=dict(cds=cds, b0Slider=b0_slider, span=span), code=js_code,
+    )
+
+    b0_slider.js_on_change("value", callback)
+
+    return bokeh.layouts.column(
+        bokeh.layouts.row(bokeh.models.Spacer(width=153), b0_slider), p
+    )
+
+
 def turing_dispersion_relation():
     """Plot of dispersion relation for Turing patterns.
 
     Replaces Python code:
 
     def dispersion_relation(k_vals, d, mu):
         lam = np.empty_like(k_vals)
```

### Comparing `biocircuits-0.1.8/biocircuits/rd.py` & `biocircuits-0.1.9/biocircuits/rd.py`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/biocircuits/reg.py` & `biocircuits-0.1.9/biocircuits/reg.py`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/biocircuits/utils.py` & `biocircuits-0.1.9/biocircuits/utils.py`

 * *Files identical despite different names*

### Comparing `biocircuits-0.1.8/biocircuits/viz.py` & `biocircuits-0.1.9/biocircuits/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,15 +263,15 @@
     Returns
     -------
     output : Bokeh application
         A Bokeh application with sliders, toggles, and a plot.
     """
     warnings.warn(
         DeprecationWarning,
-        "`interactive_xy_plot() is deprecated. Either custom build an interactive plot with base Bokeh or use Panel.",
+        "`interactive_xy_plot() is deprecated.",
     )
 
     def _plot_app(doc):
         # Build the initial plot and data source
         p, source = base_plot(callback, slider_params, toggle_params, extra_args)
 
         # Make sure axis ranges have no padding
@@ -1447,7 +1447,59 @@
         var text = div.text.concat(line);
         var lines = text.split("\\n")
         if ( lines.length > 35 ) { lines.shift(); }
         div.text = lines.join("\\n");
     """
         % (attributes, style),
     )
+
+
+def phase_portrait2(
+    du_dt,
+    dv_dt,
+    u_range,
+    v_range,
+    args_u=(),
+    args_v=(),
+    log=False,
+    p=None,
+    zoomable=False,
+    **kwargs,
+):
+    """
+    Plots the phase portrait for a 2D dynamical system in the u-v plane.
+
+    Parameters
+    ----------
+    du_dt : function
+        A function to compute the right hand side of du/dt. Must have
+        call signature `du_dt(u, v, *args_u)`. Note that there can be
+        no explicit time dependence.
+    dv_dt : function
+        A function to compute the right hand side of dv/dt. Must have
+        call signature `dv_dt(u, v, *args_v)`. Note that there can be
+        no explicit time dependence.
+    u_range : array_like, shape (2,)
+        Minimum and maximum values of u to consider.
+    v_range : array_like, shape (2,)
+        Minimum and maximum values of v to consider.
+    args_u : tuple, default ()
+        Tuple of extra arguments to be passed to `du_dt`.
+    args_v : tuple, default ()
+        Tuple of extra arguments to be passed to `dv_dt`.
+    log : bool, default False
+        If True, plot u and v on a logarithmic scale.
+    p : bokeh.plotting.Figure instance, default None
+        Figure to use for the phase portrait. If None, a new one is
+        created according to `streamplot()`.
+    zoomable : bool, default False
+        If True, generates a zoomable plot where the streamlines will be
+        redrawn to correspond for the level so zoom. This requires
+        Python to be running for the plot to render.
+    kwargs :
+        All other kwargs are passed to `streamplot`.
+
+    Returns
+    -------
+    output : bokeh.plotting.Figure instance populated with streamplot
+    """
+
```

### Comparing `biocircuits-0.1.8/biocircuits.egg-info/PKG-INFO` & `biocircuits-0.1.9/biocircuits.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: biocircuits
-Version: 0.1.8
+Version: 0.1.9
 Summary: Utilities to accompany *Biological Circuit Design* by Michael Elowitz and Justin Bois.
 Home-page: https://github.com/justinbois/biocircuits
+Download-URL: https://github.com/justinbois/biocircuits/tarball/0.1.9
 Author: Justin Bois
 Author-email: bois@caltech.edu
 License: BSD
-Download-URL: https://github.com/justinbois/biocircuits/tarball/0.1.8
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE.md
 
 # biocircuits
 
@@ -24,8 +23,7 @@
 
     pip install biocircuits
 
 
 ## Documentation
 
 You can access the docs from the [Biological Circuit Design website](https://biocircuits.github.io/package_docs/index.html).
-
```

### Comparing `biocircuits-0.1.8/biocircuits.egg-info/SOURCES.txt` & `biocircuits-0.1.9/biocircuits.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,18 +7,21 @@
 biocircuits/__init__.py
 biocircuits/dynsys.py
 biocircuits/gillespie.py
 biocircuits/jsfunctions.py
 biocircuits/jsplots.py
 biocircuits/rd.py
 biocircuits/reg.py
+biocircuits/test.py
+biocircuits/test2.py
 biocircuits/utils.py
 biocircuits/viz.py
 biocircuits.egg-info/PKG-INFO
 biocircuits.egg-info/SOURCES.txt
 biocircuits.egg-info/dependency_links.txt
 biocircuits.egg-info/requires.txt
 biocircuits.egg-info/top_level.txt
 biocircuits/apps/__init__.py
 biocircuits/apps/ffl.py
 biocircuits/apps/ffl_app.py
-biocircuits/apps/promiscuous.py
+biocircuits/apps/promiscuous.py
+biocircuits/apps/promiscuous_app.py
```

### Comparing `biocircuits-0.1.8/setup.py` & `biocircuits-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
```

