# Comparing `tmp/niceplots-2.3.0-py3-none-any.whl.zip` & `tmp/niceplots-2.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 16859 bytes, number of entries: 11
--rw-r--r--  2.0 unx       66 b- defN 23-May-09 17:32 niceplots/__init__.py
--rw-r--r--  2.0 unx     3452 b- defN 23-May-09 17:32 niceplots/parula.py
--rw-r--r--  2.0 unx    34658 b- defN 23-May-09 17:32 niceplots/utils.py
--rw-r--r--  2.0 unx     1146 b- defN 23-May-09 17:32 niceplots/styles/doumont-dark.mplstyle
--rw-r--r--  2.0 unx     1112 b- defN 23-May-09 17:32 niceplots/styles/doumont-light.mplstyle
--rw-r--r--  2.0 unx      909 b- defN 23-May-09 17:32 niceplots/styles/james-dark.mplstyle
--rw-r--r--  2.0 unx      904 b- defN 23-May-09 17:32 niceplots/styles/james-light.mplstyle
--rw-r--r--  2.0 unx     4485 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      910 b- defN 23-May-09 17:32 niceplots-2.3.0.dist-info/RECORD
-11 files, 47744 bytes uncompressed, 15313 bytes compressed:  67.9%
+Zip file size: 17416 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       66 b- defN 23-Jun-09 15:52 niceplots/__init__.py
+-rw-r--r--  2.0 unx     3452 b- defN 23-Jun-09 15:52 niceplots/parula.py
+-rw-r--r--  2.0 unx    37149 b- defN 23-Jun-09 15:52 niceplots/utils.py
+-rw-r--r--  2.0 unx     1146 b- defN 23-Jun-09 15:52 niceplots/styles/doumont-dark.mplstyle
+-rw-r--r--  2.0 unx     1112 b- defN 23-Jun-09 15:52 niceplots/styles/doumont-light.mplstyle
+-rw-r--r--  2.0 unx      909 b- defN 23-Jun-09 15:52 niceplots/styles/james-dark.mplstyle
+-rw-r--r--  2.0 unx      904 b- defN 23-Jun-09 15:52 niceplots/styles/james-light.mplstyle
+-rw-r--r--  2.0 unx     4491 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      910 b- defN 23-Jun-09 15:52 niceplots-2.4.0.dist-info/RECORD
+11 files, 50241 bytes uncompressed, 15870 bytes compressed:  68.4%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: niceplots/styles/james-dark.mplstyle
 Comment: 
 
 Filename: niceplots/styles/james-light.mplstyle
 Comment: 
 
-Filename: niceplots-2.3.0.dist-info/METADATA
+Filename: niceplots-2.4.0.dist-info/METADATA
 Comment: 
 
-Filename: niceplots-2.3.0.dist-info/WHEEL
+Filename: niceplots-2.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: niceplots-2.3.0.dist-info/top_level.txt
+Filename: niceplots-2.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: niceplots-2.3.0.dist-info/RECORD
+Filename: niceplots-2.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## niceplots/__init__.py

```diff
@@ -1,4 +1,4 @@
-__version__ = "2.3.0"
+__version__ = "2.4.0"
 
 from .utils import *
 from .parula import *
```

## niceplots/utils.py

```diff
@@ -1,17 +1,36 @@
-import matplotlib.pyplot as plt
-import numpy as np
-from scipy.interpolate import make_interp_spline, Akima1DInterpolator
+"""
+==============================================================================
+NicePlots: A collection of stylesheets and helper functions for matplotlib
+==============================================================================
+"""
+
+# ==============================================================================
+# Standard Python modules
+# ==============================================================================
+import warnings
+import os
+import copy
+from collections.abc import Iterable
 from collections import OrderedDict
-from .parula import parula_map
+
+# ==============================================================================
+# External Python modules
+# ==============================================================================
 from matplotlib import patheffects
 from matplotlib.collections import LineCollection
 import matplotlib.colors as mcolor
-import warnings
-import os
+import matplotlib.pyplot as plt
+import numpy as np
+from scipy.interpolate import make_interp_spline, Akima1DInterpolator
+
+# ==============================================================================
+# Extension modules
+# ==============================================================================
+from .parula import parula_map
 
 
 def get_style(styleName="doumont-light"):
     """
     Get the stylesheet to pass to matplotlib's style setting functions. This function
     works both with niceplots styles and matplotlib's built-in styles. Usage examples::
 
@@ -369,15 +388,20 @@
         ax.spines["top"].set_visible(False)
         ax.spines["left"].set_visible(False)
         ax.spines["right"].set_visible(False)
         ax.spines["bottom"].set_visible(False)
         ax.set_ylabel(l, rotation="horizontal", ha="right", va="center")
         string = "{number:.{digits}f}".format(number=t, digits=nd)
         ax.annotate(
-            string, xy=(1, 1), xytext=(6, 0), xycoords=ax.get_yaxis_transform(), textcoords="offset points", va="center"
+            string,
+            xy=(1, 1),
+            xytext=(6, 0),
+            xycoords=ax.get_yaxis_transform(),
+            textcoords="offset points",
+            va="center",
         )
 
         # Create the top bar line
         if j == 0:
             ax.text(0, 1.02, header[0], ha="right", fontweight="bold", fontsize="large")
             ax.text(t_max, 1.02, header[1], ha="left", fontweight="bold", fontsize="large")
 
@@ -568,15 +592,18 @@
         cmap = parula_map
 
     if colors is None:
         colors = get_colors_list()
     nColor = len(colors)
 
     # --- Create grid of points for evaluating functions ---
-    X, Y = np.meshgrid(np.linspace(xRange[0], xRange[1], nPoints), np.linspace(yRange[0], yRange[1], nPoints))
+    X, Y = np.meshgrid(
+        np.linspace(xRange[0], xRange[1], nPoints),
+        np.linspace(yRange[0], yRange[1], nPoints),
+    )
 
     # --- Evaluate objective and constraint functions ---
     Fobj = obj(X, Y)
     g = []
     for ineq in cons["ineqCon"]:
         g.append(ineq(X, Y))
     h = []
@@ -594,17 +621,27 @@
     )
 
     # --- Plot constraint boundaries ---
     colorIndex = 0
     for conValue in g:
         contour = ax.contour(X, Y, conValue, levels=[0.0], colors=colors[colorIndex % nColor])
         if conStyle.lower() == "hashed":
-            plt.setp(contour.collections, path_effects=[patheffects.withTickedStroke(angle=60, length=2)])
+            plt.setp(
+                contour.collections,
+                path_effects=[patheffects.withTickedStroke(angle=60, length=2)],
+            )
         elif conStyle.lower() == "shaded":
-            ax.contourf(X, Y, conValue, levels=[0.0, np.inf], colors=colors[colorIndex % nColor], alpha=0.4)
+            ax.contourf(
+                X,
+                Y,
+                conValue,
+                levels=[0.0, np.inf],
+                colors=colors[colorIndex % nColor],
+                alpha=0.4,
+            )
 
         colorIndex += 1
 
     for conValue in h:
         ax.contour(X, Y, conValue, levels=[0.0], colors=colors[colorIndex % nColor])
 
     # --- Plot optimal point if provided ---
@@ -627,15 +664,25 @@
     if returnFig:
         return fig, ax
     else:
         return
 
 
 def plot_colored_line(
-    x, y, c, cmap=None, fig=None, ax=None, addColorBar=False, cRange=None, cBarLabel=None, norm=None, **kwargs
+    x,
+    y,
+    c,
+    cmap=None,
+    fig=None,
+    ax=None,
+    addColorBar=False,
+    cRange=None,
+    cBarLabel=None,
+    norm=None,
+    **kwargs,
 ):
     """Plot an XY line whose color is determined by some other variable C
 
     Parameters
     ----------
     x : iterable of length n
         x data
@@ -957,12 +1004,48 @@
     x_interp = np.linspace(np.min(x), np.max(x), num_interp_pts)
     ax.plot(x_interp, spline(x_interp), **plot_kwargs)
 
     if return_fig:
         return fig, ax
 
 
+def save_figs(fig, name, formats, format_kwargs=None, **kwargs):
+    """Save a figure in multiple formats
+
+    Parameters
+    ----------
+    fig : Matplotlib figure
+        The figure to save
+    name : str
+        Output path for the files, e.g "path/to/file/file_name", no file extension required
+    formats : str, list[str]
+        file formats to save the figure in, e.g. "png", "pdf", "svg"
+    format_kwargs : dict, optional
+        A dictionary of dictionaries, where the keys are the file formats and the values are any keyword arguments that
+        should only be applied to that format. These kwargs will be added to ones passed to all formats, by default None
+    kwargs :
+        Any keyword arguments to pass to `plt.savefig()` for all formats
+    """
+
+    # --- Strip any extension from the name ---
+    fileName = os.path.splitext(name)[0]
+
+    # --- Convert the file format to a list if only one given ---
+    if not isinstance(formats, Iterable):
+        formats = [formats]
+
+    # --- Save the figures ---
+    for ext in formats:
+        if ext[0] == ".":
+            ext = ext[1:]
+        # Add any format-specific kwargs
+        ext_kwargs = copy.deepcopy(kwargs)
+        if format_kwargs is not None and ext in format_kwargs:
+            ext_kwargs.update(format_kwargs[ext])
+        fig.savefig(fileName + "." + ext, **ext_kwargs)
+
+
 def All():
     """Runs commonly called functions provided in this module."""
     adjust_spines()
     draggable_legend()
     plt.gcf().canvas.mpl_connect("close_event", handle_close)
```

## Comparing `niceplots-2.3.0.dist-info/METADATA` & `niceplots-2.4.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: niceplots
-Version: 2.3.0
+Version: 2.4.0
 Summary: Plotting utilities for matplotlib in python
 Home-page: https://github.com/mdolab/niceplots
 Author: 
 Author-email: 
 License: Apache License, Version 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Requires-Dist: numpy (>=1.16)
 Requires-Dist: matplotlib (>=2.2)
 Requires-Dist: scipy (>=1.7)
 
 # NicePlots
-## A collection of small tweaks to improve Python / plotting
+## A collection of nice styles and helper functions for matplotlib
 
 ![Build Status](https://github.com/mdolab/niceplots/workflows/niceplots/badge.svg)
 [![Documentation Status](https://readthedocs.com/projects/mdolab-niceplots/badge/?version=latest)](https://mdolab-niceplots.readthedocs-hosted.com/en/latest)
 [![PyPI](https://img.shields.io/pypi/v/niceplots)](https://pypi.org/project/niceplots/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/niceplots)](https://pypi.org/project/niceplots/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
```

## Comparing `niceplots-2.3.0.dist-info/RECORD` & `niceplots-2.4.0.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-niceplots/__init__.py,sha256=zeXTZYXNljlzdfbh3JWQyNaQSH4oU1bTw7-do_O-qlI,66
+niceplots/__init__.py,sha256=Dg11PWdNO-v99L9OX7PyMQyd5gUefeQlS7Mzit4UbVo,66
 niceplots/parula.py,sha256=by5EIIIjnxZalrrgXHkcT5PeIiT7rv6bn-W3rg3VaOU,3452
-niceplots/utils.py,sha256=6XQD_iKncARcyTJrHz0aIDXXMHEbRXV5ceEfO7_1hx0,34658
+niceplots/utils.py,sha256=I2GykuvCLeamqrWbx9VXRdrAIqPCaSlLni1mDQjc5hw,37149
 niceplots/styles/doumont-dark.mplstyle,sha256=8S0wCuAk7YYTWmY4wZ5mgDoyYAsS6yx5Uv5oNdNXIKc,1146
 niceplots/styles/doumont-light.mplstyle,sha256=cxNC2Au1VLDVizB7pQXcAZZbCCrVVLab_fNsChmsURE,1112
 niceplots/styles/james-dark.mplstyle,sha256=xoIEscAkdxItnivxgBLQ1RZ2-t9lTDsctebEdNlcIlk,909
 niceplots/styles/james-light.mplstyle,sha256=OYy_nIw0GDbKhJmN2LX8zzqeW6IfO7pHv_1i-0eeddI,904
-niceplots-2.3.0.dist-info/METADATA,sha256=agUvpbsl8dOYFEB9M3sib9tl7tdjSX1Pypw1Nwsf3cU,4485
-niceplots-2.3.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-niceplots-2.3.0.dist-info/top_level.txt,sha256=AXPTUh13A4r5iKtvXz0ZzOPnkrYIDczBiw3z9IyS4uI,10
-niceplots-2.3.0.dist-info/RECORD,,
+niceplots-2.4.0.dist-info/METADATA,sha256=_AAuZAEroLumLG67yHLUMN-4cb7FJMWTCQQf-poL1Bg,4491
+niceplots-2.4.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+niceplots-2.4.0.dist-info/top_level.txt,sha256=AXPTUh13A4r5iKtvXz0ZzOPnkrYIDczBiw3z9IyS4uI,10
+niceplots-2.4.0.dist-info/RECORD,,
```

