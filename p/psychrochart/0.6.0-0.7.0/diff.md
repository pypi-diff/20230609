# Comparing `tmp/psychrochart-0.6.0.tar.gz` & `tmp/psychrochart-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychrochart-0.6.0.tar", max compression
+gzip compressed data, was "psychrochart-0.7.0.tar", max compression
```

## Comparing `psychrochart-0.6.0.tar` & `psychrochart-0.7.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0     7288 2023-06-07 17:46:43.829993 psychrochart-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-06-07 17:46:43.829993 psychrochart-0.6.0/LICENSE
--rw-r--r--   0        0        0     7077 2023-06-07 17:46:43.829993 psychrochart-0.6.0/README.md
--rw-r--r--   0        0        0      711 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/__init__.py
--rw-r--r--   0        0        0      336 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/__main__.py
--rw-r--r--   0        0        0    12177 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart.py
--rw-r--r--   0        0        0     2157 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/ashrae_chart_style.json
--rw-r--r--   0        0        0     2380 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
--rw-r--r--   0        0        0     3080 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/default_chart_config.json
--rw-r--r--   0        0        0      585 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/default_comfort_zones.json
--rw-r--r--   0        0        0     2436 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/interior_chart_style.json
--rw-r--r--   0        0        0     2490 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chart_styles/minimal_chart_style.json
--rw-r--r--   0        0        0    17119 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/chartdata.py
--rw-r--r--   0        0        0        0 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/__init__.py
--rw-r--r--   0        0        0     4427 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/annots.py
--rw-r--r--   0        0        0     1246 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/base.py
--rw-r--r--   0        0        0     6715 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/config.py
--rw-r--r--   0        0        0     9238 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/curves.py
--rw-r--r--   0        0        0     5852 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/parsers.py
--rw-r--r--   0        0        0     1909 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/styles.py
--rw-r--r--   0        0        0     1744 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/models/validators.py
--rw-r--r--   0        0        0     7361 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/plot_logic.py
--rw-r--r--   0        0        0     9076 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/process_logic.py
--rw-r--r--   0        0        0     3977 2023-06-07 17:46:43.841993 psychrochart-0.6.0/psychrochart/util.py
--rw-r--r--   0        0        0     2195 2023-06-07 17:46:43.841993 psychrochart-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     8366 1970-01-01 00:00:00.000000 psychrochart-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     7837 2023-06-09 12:36:51.287968 psychrochart-0.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-06-09 12:36:51.287968 psychrochart-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7077 2023-06-09 12:36:51.287968 psychrochart-0.7.0/README.md
+-rw-r--r--   0        0        0      711 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/__init__.py
+-rw-r--r--   0        0        0      336 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/__main__.py
+-rw-r--r--   0        0        0    12221 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart.py
+-rw-r--r--   0        0        0      178 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_entities.py
+-rw-r--r--   0        0        0     2157 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/ashrae_chart_style.json
+-rw-r--r--   0        0        0     2380 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/ashrae_ip_chart_style.json
+-rw-r--r--   0        0        0     3080 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/default_chart_config.json
+-rw-r--r--   0        0        0      585 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/default_comfort_zones.json
+-rw-r--r--   0        0        0     2436 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/interior_chart_style.json
+-rw-r--r--   0        0        0     2490 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chart_styles/minimal_chart_style.json
+-rw-r--r--   0        0        0    17122 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/chartdata.py
+-rw-r--r--   0        0        0        0 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/__init__.py
+-rw-r--r--   0        0        0     4427 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/annots.py
+-rw-r--r--   0        0        0     1246 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/base.py
+-rw-r--r--   0        0        0     6715 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/config.py
+-rw-r--r--   0        0        0     3584 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/curves.py
+-rw-r--r--   0        0        0     5852 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/parsers.py
+-rw-r--r--   0        0        0     1909 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/styles.py
+-rw-r--r--   0        0        0     1924 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/models/validators.py
+-rw-r--r--   0        0        0    13156 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/plot_logic.py
+-rw-r--r--   0        0        0     9048 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/process_logic.py
+-rw-r--r--   0        0        0     3977 2023-06-09 12:36:51.299968 psychrochart-0.7.0/psychrochart/util.py
+-rw-r--r--   0        0        0     2222 2023-06-09 12:36:51.299968 psychrochart-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     8406 1970-01-01 00:00:00.000000 psychrochart-0.7.0/PKG-INFO
```

### Comparing `psychrochart-0.6.0/CHANGELOG.md` & `psychrochart-0.7.0/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.0] - ♻️ Testing suite refactor + model changes - 2023-06-09
+
+Maintenance-only update, without new features.
+
+##### Changes
+
+- 💥 Remove plotting methods from `PsychroCurve`/`PsychroCurves` for a more functional approach, using methods in `plot_logic.py`
+- 💥 Add `PsychroCurve.internal_value` field, to identify the trigger value for each curve (constant H/V/RH...), and evolve validation of data arrays
+- ✅ tests: Increase test coverage and optimize tests for faster run (~2x)
+- 📦️ env: Add slugify to deps and bump version
+
 ## [0.6.0] - ✨ Chart config auto-refresh + bugfixes - 2023-06-07
 
 Before, chart customize was done by creating a new `Psychrochart` object based on some modified chart configuration,
 so creating custom plots, or even changing chart limits, was _challenging_ 😓
 
 **Now**, when `chart.config` changes, any call to `chart.save()`, `chart.make_svg()`, or `chart.plot()`
 will regenerate the chart data (limits, enabled curves, styling, etc.) before plotting, with only the visible curves inside limits,
```

### Comparing `psychrochart-0.6.0/LICENSE` & `psychrochart-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/README.md` & `psychrochart-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/__init__.py` & `psychrochart-0.7.0/psychrochart/__init__.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chart.py` & `psychrochart-0.7.0/psychrochart/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """A library to make psychrometric charts and overlay information in them."""
 import gc
 from io import StringIO
 from pathlib import Path
-from typing import Any, Iterable, Mapping, Type
+from typing import Any, Iterable, Type
 
 from matplotlib import figure
 from matplotlib.artist import Artist
 from matplotlib.axes import Axes
 from matplotlib.backend_bases import FigureCanvasBase
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 from matplotlib.backends.backend_svg import FigureCanvasSVG
@@ -23,17 +23,19 @@
     ConvexGroupTuple,
     load_extra_annots,
     load_points_dbt_rh,
     obj_loader,
 )
 from psychrochart.models.styles import CurveStyle
 from psychrochart.plot_logic import (
+    add_label_to_curve,
     apply_axis_styling,
     plot_annots_dbt_rh,
     plot_chart,
+    plot_curve,
 )
 from psychrochart.process_logic import (
     append_zones_to_chart,
     generate_psychrochart,
     update_psychrochart_data,
 )
 from psychrochart.util import mod_color
@@ -259,18 +261,20 @@
             CurveStyle, style, default_obj=self.config.constant_dry_temp
         )
         curve = make_constant_dry_bulb_v_line(
             self.config.w_min,
             temp,
             self.pressure,
             style=style_curve,
+            type_curve="constant-dbt",
             reverse=reverse,
         )
-        if curve.plot_curve(self.axes) and label is not None:
-            curve.add_label(self.axes, label, **label_params)
+
+        if plot_curve(curve, self.axes) and label is not None:
+            add_label_to_curve(curve, self.axes, label, **label_params)
 
     def plot_legend(
         self,
         loc: str = "upper left",
         markerscale: float = 0.9,
         frameon: bool = True,
         fancybox: bool = True,
@@ -322,15 +326,15 @@
             self._legend.remove()
             self._legend = None
 
     def save(
         self,
         path_dest: Any,
         canvas_cls: Type[FigureCanvasBase] | None = None,
-        **params: Mapping[str, Any],
+        **params,
     ) -> None:
         """Write the chart to disk."""
         # ensure destination path if folder does not exist
         if (
             isinstance(path_dest, (str, Path))
             and not Path(path_dest).parent.exists()
         ):
@@ -338,15 +342,15 @@
         if self._axes is None or self.config.has_changed:
             self.plot()
         assert self._fig is not None
         canvas_use = _select_fig_canvas(path_dest, canvas_cls)
         canvas_use(self._fig).print_figure(path_dest, **params)
         gc.collect()
 
-    def make_svg(self, **params: Mapping[str, Any]) -> str:
+    def make_svg(self, **params) -> str:
         """Generate chart as SVG and return as text."""
         svg_io = StringIO()
         self.save(svg_io, canvas_cls=FigureCanvasSVG, **params)
         svg_io.seek(0)
         return svg_io.read()
 
     def close_fig(self) -> None:
```

### Comparing `psychrochart-0.6.0/psychrochart/chart_styles/ashrae_chart_style.json` & `psychrochart-0.7.0/psychrochart/chart_styles/ashrae_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chart_styles/ashrae_ip_chart_style.json` & `psychrochart-0.7.0/psychrochart/chart_styles/ashrae_ip_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chart_styles/default_chart_config.json` & `psychrochart-0.7.0/psychrochart/chart_styles/default_chart_config.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chart_styles/default_comfort_zones.json` & `psychrochart-0.7.0/psychrochart/chart_styles/default_comfort_zones.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chart_styles/interior_chart_style.json` & `psychrochart-0.7.0/psychrochart/chart_styles/interior_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chart_styles/minimal_chart_style.json` & `psychrochart-0.7.0/psychrochart/chart_styles/minimal_chart_style.json`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/chartdata.py` & `psychrochart-0.7.0/psychrochart/chartdata.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,17 +15,18 @@
     GetTDryBulbFromMoistAirVolumeAndHumRatio,
     GetTWetBulbFromHumRatio,
     GetVapPresFromHumRatio,
     isIP,
 )
 from scipy.interpolate import interp1d
 
+from psychrochart.chart_entities import random_internal_value
 from psychrochart.models.annots import ChartZone
 from psychrochart.models.curves import PsychroCurve, PsychroCurves
-from psychrochart.models.styles import CurveStyle, ZoneStyle
+from psychrochart.models.styles import CurveStyle
 from psychrochart.util import solve_curves_with_iteration
 
 f_vec_hum_ratio_from_vap_press = np.vectorize(GetHumRatioFromVapPres)
 f_vec_moist_air_enthalpy = np.vectorize(GetMoistAirEnthalpy)
 f_vec_moist_air_volume = np.vectorize(GetMoistAirVolume)
 f_vec_dew_point_from_vap_press = np.vectorize(GetTDewPointFromVapPres)
 f_vec_dry_temp_from_enthalpy = np.vectorize(GetTDryBulbFromEnthalpyAndHumRatio)
@@ -130,14 +131,15 @@
             PsychroCurve(
                 x_data=temps_ct_rh,
                 y_data=curve_ct_rh,
                 style=style,
                 type_curve="constant_rh_data",
                 label_loc=label_loc,
                 label=f"RH {rh:g} %" if rh in rh_label_values else None,
+                internal_value=float(rh),
             )
             for rh, curve_ct_rh in zip(rh_values, curves_ct_rh)
         ],
         family_label=family_label,
     )
 
 
@@ -158,14 +160,15 @@
     else:
         path_y = [w_humidity_ratio_min, w_max]
     return PsychroCurve(
         x_data=np.array([temp, temp]),
         y_data=np.array(path_y),
         style=style,
         type_curve=type_curve,
+        internal_value=temp,
     )
 
 
 def make_constant_dry_bulb_v_lines(
     w_humidity_ratio_min: float,
     pressure: float,
     temps_vl: np.ndarray,
@@ -177,14 +180,15 @@
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=np.array([temp, temp]),
                 y_data=np.array([w_humidity_ratio_min, w_max]),
                 style=style,
                 type_curve="constant_dry_temp_data",
+                internal_value=temp,
             )
             for temp, w_max in zip(temps_vl, w_max_vec)
         ],
         family_label=family_label,
     )
 
 
@@ -203,14 +207,15 @@
     return PsychroCurves(
         curves=[
             PsychroCurve(
                 x_data=np.array([t_dp, dbt_max]),
                 y_data=np.array([w, w]),
                 style=style,
                 type_curve="constant_humidity_data",
+                internal_value=w,
             )
             for w, t_dp in zip(ws_hl, dew_points)
         ],
         family_label=family_label,
     )
 
 
@@ -227,14 +232,15 @@
         temps_sat_line, 100, pressure
     )
     sat_c = PsychroCurve(
         x_data=temps_sat_line,
         y_data=w_sat,
         style=style,
         type_curve="saturation",
+        internal_value=100.0,
     )
     return PsychroCurves(curves=[sat_c])
 
 
 def make_constant_enthalpy_lines(
     w_humidity_ratio_min: float,
     pressure: float,
@@ -304,14 +310,15 @@
                 type_curve="constant_h_data",
                 label_loc=label_loc,
                 label=(
                     _make_enthalpy_label(h)
                     if round(h, 3) in h_label_values
                     else None
                 ),
+                internal_value=round(h, 3),
             )
             for t_sat, w_sat, t_max, h in zip(
                 t_sat_points, w_in_sat, temps_max_constant_h, h_objective
             )
         ],
         family_label=family_label,
     )
@@ -382,14 +389,15 @@
                 type_curve="constant_v_data",
                 label_loc=label_loc,
                 label=(
                     _make_vol_label(vol)
                     if round(vol, 3) in v_label_values
                     else None
                 ),
+                internal_value=round(vol, 3),
             )
             for t_sat, w_sat, t_max, vol in zip(
                 t_sat_points, w_in_sat, temps_max_constant_v, v_objective
             )
         ],
         family_label=family_label,
     )
@@ -470,75 +478,59 @@
         c = PsychroCurve(
             x_data=np.array([wbt, dbt_objective]),
             y_data=np.array([w_left, w_right]),
             style=style,
             type_curve="constant_wbt_data",
             label_loc=label_loc,
             label=(_make_temp_label(wbt) if wbt in wbt_label_values else None),
+            internal_value=wbt,
         )
         curves.append(c)
 
     return PsychroCurves(curves=curves, family_label=family_label)
 
 
-def _make_zone_dbt_rh(
-    t_min: float,
-    t_max: float,
-    increment: float,
-    rh_min: float,
-    rh_max: float,
-    pressure: float,
-    style: ZoneStyle,
-    label: str | None = None,
+def make_zone_curve(
+    zone_conf: ChartZone, increment: float, pressure: float
 ) -> PsychroCurve:
-    """Generate points for zone between constant dry bulb temps and RH."""
-    temps = np.arange(t_min, t_max + increment, increment)
+    """Generate plot-points for zone."""
+    # todo better id for overlay zones if no label
+    zone_value = random_internal_value() if zone_conf.label is None else None
+    if zone_conf.zone_type == "xy-points":
+        # expect points in plot coordinates!
+        return PsychroCurve(
+            x_data=np.array(zone_conf.points_x),
+            y_data=np.array(zone_conf.points_y),
+            style=zone_conf.style,
+            type_curve="xy-points",
+            label=zone_conf.label,
+            internal_value=zone_value,
+        )
+
+    assert zone_conf.zone_type == "dbt-rh"
+    # points for zone between constant dry bulb temps and RH
+    t_min = zone_conf.points_x[0]
+    t_max = zone_conf.points_x[-1]
+    rh_min = zone_conf.points_y[0]
+    rh_max = zone_conf.points_y[-1]
     assert rh_min >= 0.0 and rh_max <= 100.0
+    assert t_min < t_max
+
+    temps = np.arange(t_min, t_max + increment, increment)
     curve_rh_up = gen_points_in_constant_relative_humidity(
         temps, rh_max, pressure
     )
     curve_rh_down = gen_points_in_constant_relative_humidity(
         temps, rh_min, pressure
     )
     abs_humid: list[float] = (
         list(curve_rh_up) + list(curve_rh_down)[::-1] + [curve_rh_up[0]]
     )
     temps_zone: list[float] = list(temps) + list(temps)[::-1] + [temps[0]]
     return PsychroCurve(
         x_data=np.array(temps_zone),
         y_data=np.array(abs_humid),
-        style=style,
-        type_curve="constant_rh_data",
-        label=label,
+        style=zone_conf.style,
+        type_curve="dbt-rh",
+        label=zone_conf.label,
+        internal_value=zone_value,
     )
-
-
-def make_zone_curve(
-    zone_conf: ChartZone, increment: float, pressure: float
-) -> PsychroCurve:
-    """Generate points for zone between constant dry bulb temps and RH."""
-    # TODO make conversion rh -> w and new zone_type: "dbt-rh-points"
-    assert isinstance(zone_conf.style, ZoneStyle)
-    if zone_conf.zone_type == "dbt-rh":
-        t_min = zone_conf.points_x[0]
-        t_max = zone_conf.points_x[-1]
-        rh_min = zone_conf.points_y[0]
-        rh_max = zone_conf.points_y[-1]
-        return _make_zone_dbt_rh(
-            t_min,
-            t_max,
-            increment,
-            rh_min,
-            rh_max,
-            pressure,
-            zone_conf.style,
-            label=zone_conf.label,
-        )
-    else:
-        # zone_type: 'xy-points'
-        return PsychroCurve(
-            x_data=np.array(zone_conf.points_x),
-            y_data=np.array(zone_conf.points_y),
-            style=zone_conf.style,
-            type_curve="custom path",
-            label=zone_conf.label,
-        )
```

### Comparing `psychrochart-0.6.0/psychrochart/models/annots.py` & `psychrochart-0.7.0/psychrochart/models/annots.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/models/base.py` & `psychrochart-0.7.0/psychrochart/models/base.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/models/config.py` & `psychrochart-0.7.0/psychrochart/models/config.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/models/parsers.py` & `psychrochart-0.7.0/psychrochart/models/parsers.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/models/styles.py` & `psychrochart-0.7.0/psychrochart/models/styles.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/psychrochart/models/validators.py` & `psychrochart-0.7.0/psychrochart/models/validators.py`

 * *Files 15% similar despite different names*

```diff
@@ -45,8 +45,11 @@
 
 def parse_curve_arrays(values):
     """Pydantic validator to convert values into np.arrays."""
     if "x_data" in values and not isinstance(values["x_data"], np.ndarray):
         values["x_data"] = np.array(values["x_data"])
     if "y_data" in values and not isinstance(values["y_data"], np.ndarray):
         values["y_data"] = np.array(values["y_data"])
+    shape = values["x_data"].shape[0], values["y_data"].shape[0]
+    if shape[0] == 0 or shape[1] == 0 or shape[0] != shape[1]:
+        raise ValueError(f"Invalid shape: {shape}")
     return values
```

### Comparing `psychrochart-0.6.0/psychrochart/process_logic.py` & `psychrochart-0.7.0/psychrochart/process_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,26 +52,23 @@
 
 def append_zones_to_chart(
     config: ChartConfig,
     chart: PsychroChartModel,
     zones: ChartZones | dict[str, Any] | str | None = None,
 ) -> None:
     """Append zones as patches to the psychrometric chart data-container."""
-    chart.zones.append(
-        PsychroCurves(
+    zones_use = obj_loader(ChartZones, zones, default_obj=DEFAULT_ZONES).zones
+    if zones_use:
+        curves = PsychroCurves(
             curves=[
-                make_zone_curve(
-                    zone_conf, config.limits.step_temp, chart.pressure
-                )
-                for zone_conf in obj_loader(
-                    ChartZones, zones, default_obj=DEFAULT_ZONES
-                ).zones
+                make_zone_curve(zone, config.limits.step_temp, chart.pressure)
+                for zone in zones_use
             ]
         )
-    )
+        chart.zones.append(curves)
 
 
 def _generate_chart_curves(
     config: ChartConfig, chart: PsychroChartModel, pressure: float
 ):
     # check chart limits are not fully above the saturation curve!
     assert (chart.saturation.curves[0].y_data > config.w_min).any()
```

### Comparing `psychrochart-0.6.0/psychrochart/util.py` & `psychrochart-0.7.0/psychrochart/util.py`

 * *Files identical despite different names*

### Comparing `psychrochart-0.6.0/pyproject.toml` & `psychrochart-0.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 log_level = "INFO"
 log_cli = true
 log_format = "%(asctime)s %(levelname)s: (%(filename)s:%(lineno)s): %(message)s"
 log_date_format = "%Y-%m-%d %H:%M:%S"
 
 [tool.poetry]
 name = "psychrochart"
-version = "0.6.0"
+version = "0.7.0"
 description = "A python 3 library to make psychrometric charts and overlay information on them"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 packages = [
     { include = "psychrochart" }
 ]
 license = "MIT"
 readme = "README.md"
@@ -70,14 +70,15 @@
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 matplotlib = ">=3.7"
 scipy = ">=1.10"
 psychrolib = ">=2.5"
 pydantic = ">=1.8"
+python-slugify = ">=8.0.1"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.10.0"
 pytest = "*"
 pytest-cov = "*"
 
 [build-system]
```

### Comparing `psychrochart-0.6.0/PKG-INFO` & `psychrochart-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychrochart
-Version: 0.6.0
+Version: 0.7.0
 Summary: A python 3 library to make psychrometric charts and overlay information on them
 Home-page: https://github.com/azogue/psychrochart
 License: MIT
 Keywords: psychrometrics,moist,humid air,climate control,matplotlib
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.10,<3.12
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: matplotlib (>=3.7)
 Requires-Dist: psychrolib (>=2.5)
 Requires-Dist: pydantic (>=1.8)
+Requires-Dist: python-slugify (>=8.0.1)
 Requires-Dist: scipy (>=1.10)
 Project-URL: Repository, https://github.com/azogue/psychrochart
 Description-Content-Type: text/markdown
 
 [![pre-commit.ci Status][pre-commit-ci-image]][pre-commit-ci-url]
 [![Build Status][build-image]][build-url]
 [![PyPI Version][pypi-image]][pypi-url]
```

