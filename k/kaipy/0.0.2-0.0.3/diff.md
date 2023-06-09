# Comparing `tmp/kaipy-0.0.2.tar.gz` & `tmp/kaipy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaipy-0.0.2.tar", last modified: Mon Nov 28 16:02:59 2022, max compression
+gzip compressed data, was "kaipy-0.0.3.tar", last modified: Fri Jun  9 13:43:23 2023, max compression
```

## Comparing `kaipy-0.0.2.tar` & `kaipy-0.0.3.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.915060 kaipy-0.0.2/
--rw-r--r--   0 winteel1   (502) staff       (20)      926 2022-11-28 16:02:59.914767 kaipy-0.0.2/PKG-INFO
--rw-r--r--   0 winteel1   (502) staff       (20)      466 2022-11-28 15:39:51.000000 kaipy-0.0.2/README.md
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.864836 kaipy-0.0.2/kaipy/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/__init__.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.870963 kaipy-0.0.2/kaipy/chimp/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/chimp/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2297 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/chimp/chimph5p.py
--rw-r--r--   0 winteel1   (502) staff       (20)      922 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/chimp/chimpviz.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1804 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/chimp/kCyl.py
--rw-r--r--   0 winteel1   (502) staff       (20)    13945 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/embiggenUtils.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.878084 kaipy-0.0.2/kaipy/gamera/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)    15993 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/block_gampp.py
--rw-r--r--   0 winteel1   (502) staff       (20)     3222 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/deltabViz.py
--rw-r--r--   0 winteel1   (502) staff       (20)    19760 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/gamGrids.py
--rw-r--r--   0 winteel1   (502) staff       (20)     7728 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/gampp.py
--rw-r--r--   0 winteel1   (502) staff       (20)    10953 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/magsphere.py
--rw-r--r--   0 winteel1   (502) staff       (20)    14494 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/magsphereRescale.py
--rw-r--r--   0 winteel1   (502) staff       (20)     7031 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/msphViz.py
--rw-r--r--   0 winteel1   (502) staff       (20)     4119 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/rcmpp.py
--rw-r--r--   0 winteel1   (502) staff       (20)     3519 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamera/remixpp.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.880288 kaipy-0.0.2/kaipy/gamhelio/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)    12994 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/helioViz.py
--rw-r--r--   0 winteel1   (502) staff       (20)    14894 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/heliosphere.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.887182 kaipy-0.0.2/kaipy/gamhelio/lib/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2575 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/ace.py
--rw-r--r--   0 winteel1   (502) staff       (20)      758 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/cspice.py
--rw-r--r--   0 winteel1   (502) staff       (20)    12020 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/lfmhlib.py
--rw-r--r--   0 winteel1   (502) staff       (20)     5369 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/mas.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1322 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/msgr.py
--rw-r--r--   0 winteel1   (502) staff       (20)     4803 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/poisson.py
--rw-r--r--   0 winteel1   (502) staff       (20)      833 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/util.py
--rwxr-xr-x   0 winteel1   (502) staff       (20)     3457 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/wsa.py
--rwxr-xr-x   0 winteel1   (502) staff       (20)     1064 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/lib/wsa2h5.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.888642 kaipy-0.0.2/kaipy/gamhelio/wsa2TDgamera/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/wsa2TDgamera/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2475 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/wsa2TDgamera/params.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.890128 kaipy-0.0.2/kaipy/gamhelio/wsa2gamera/
--rw-r--r--   0 winteel1   (502) staff       (20)       21 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/wsa2gamera/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1607 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/gamhelio/wsa2gamera/params.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2304 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kJobs.py
--rw-r--r--   0 winteel1   (502) staff       (20)     4817 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kaiH5.py
--rw-r--r--   0 winteel1   (502) staff       (20)     5485 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kaiTools.py
--rw-r--r--   0 winteel1   (502) staff       (20)    11995 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kaiViz.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2405 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kaijson.py
--rw-r--r--   0 winteel1   (502) staff       (20)     5401 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kaixdmf.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1302 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/kdefs.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2709 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/lfm2kaiju.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.891929 kaipy-0.0.2/kaipy/paraview/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/paraview/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1207 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/paraview/pvGam.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2649 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/paraview/pvutils.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.894412 kaipy-0.0.2/kaipy/rcm/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/__init__.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.899729 kaipy-0.0.2/kaipy/rcm/lambdautils/
--rw-r--r--   0 winteel1   (502) staff       (20)     1707 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/AlamData.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2469 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/AlamParams.py
--rw-r--r--   0 winteel1   (502) staff       (20)     6869 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/DistTypes.py
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     2135 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/fileIO.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1932 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/genAlam.py
--rw-r--r--   0 winteel1   (502) staff       (20)     4036 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils/plotter.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.904653 kaipy-0.0.2/kaipy/rcm/lambdautils_old/
--rw-r--r--   0 winteel1   (502) staff       (20)     4504 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/AlamData.py
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     5507 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/alamTester.py
--rw-r--r--   0 winteel1   (502) staff       (20)     5780 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/dpRangeEval.py
--rw-r--r--   0 winteel1   (502) staff       (20)    10132 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/dpetadp.py
--rw-r--r--   0 winteel1   (502) staff       (20)     6896 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/genAlam.py
--rw-r--r--   0 winteel1   (502) staff       (20)      309 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/helperdefs.py
--rw-r--r--   0 winteel1   (502) staff       (20)     9050 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/lambdautils_old/plotter.py
--rw-r--r--   0 winteel1   (502) staff       (20)      926 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/rcminit.py
--rw-r--r--   0 winteel1   (502) staff       (20)     3653 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/rcmutils.py
--rw-r--r--   0 winteel1   (502) staff       (20)     3493 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/rcmxdmf.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.906459 kaipy-0.0.2/kaipy/rcm/wmutils/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/wmutils/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     3191 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/wmutils/genWM.py
--rw-r--r--   0 winteel1   (502) staff       (20)      521 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/rcm/wmutils/wmData.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.907482 kaipy-0.0.2/kaipy/remix/
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/remix/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)    29846 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/remix/remix.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.914105 kaipy-0.0.2/kaipy/solarWind/
--rw-r--r--   0 winteel1   (502) staff       (20)    39655 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/CUSTOM.py
--rw-r--r--   0 winteel1   (502) staff       (20)    24499 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/OMNI.py
--rw-r--r--   0 winteel1   (502) staff       (20)     7272 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/SolarWind.py
--rw-r--r--   0 winteel1   (502) staff       (20)     1950 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/TimeSeries.py
--rw-r--r--   0 winteel1   (502) staff       (20)    43184 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/WIND.py
--rw-r--r--   0 winteel1   (502) staff       (20)        0 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/__init__.py
--rw-r--r--   0 winteel1   (502) staff       (20)     9375 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/jdutil.py
--rw-r--r--   0 winteel1   (502) staff       (20)     8166 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/ols.py
--rw-r--r--   0 winteel1   (502) staff       (20)    10440 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/solarWind/swBCplots.py
--rw-r--r--   0 winteel1   (502) staff       (20)    32846 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/supermage.py
--rw-r--r--   0 winteel1   (502) staff       (20)    21838 2022-11-28 15:39:51.000000 kaipy-0.0.2/kaipy/transform.py
-drwxr-xr-x   0 winteel1   (502) staff       (20)        0 2022-11-28 16:02:59.867903 kaipy-0.0.2/kaipy.egg-info/
--rw-r--r--   0 winteel1   (502) staff       (20)      926 2022-11-28 16:02:59.000000 kaipy-0.0.2/kaipy.egg-info/PKG-INFO
--rw-r--r--   0 winteel1   (502) staff       (20)     2286 2022-11-28 16:02:59.000000 kaipy-0.0.2/kaipy.egg-info/SOURCES.txt
--rw-r--r--   0 winteel1   (502) staff       (20)        1 2022-11-28 16:02:59.000000 kaipy-0.0.2/kaipy.egg-info/dependency_links.txt
--rw-r--r--   0 winteel1   (502) staff       (20)        6 2022-11-28 16:02:59.000000 kaipy-0.0.2/kaipy.egg-info/top_level.txt
--rw-r--r--   0 winteel1   (502) staff       (20)       38 2022-11-28 16:02:59.915178 kaipy-0.0.2/setup.cfg
--rw-r--r--   0 winteel1   (502) staff       (20)      777 2022-11-28 16:01:25.000000 kaipy-0.0.2/setup.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.800114 kaipy-0.0.3/
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 13:43:23.799385 kaipy-0.0.3/PKG-INFO
+-rw-r--r--   0 winteel1   (503) staff       (20)      466 2023-06-09 13:13:22.000000 kaipy-0.0.3/README.md
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.725434 kaipy-0.0.3/kaipy/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/__init__.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.732744 kaipy-0.0.3/kaipy/chimp/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2297 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/chimph5p.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      922 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/chimpviz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1804 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/kCyl.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    13945 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/embiggenUtils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.743767 kaipy-0.0.3/kaipy/gamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    15993 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/block_gampp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3222 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/deltabViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    19760 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/gamGrids.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7728 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/gampp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10953 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/magsphere.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    14494 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/magsphereRescale.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7031 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/msphViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4119 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/rcmpp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3519 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/remixpp.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.746330 kaipy-0.0.3/kaipy/gamhelio/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    12994 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/helioViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    14894 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/heliosphere.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.755741 kaipy-0.0.3/kaipy/gamhelio/lib/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2575 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/ace.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      758 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/cspice.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    12020 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/lfmhlib.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5369 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/mas.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1322 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/msgr.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4803 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/poisson.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      833 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/util.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     3457 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/wsa.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     1064 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/wsa2h5.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.757366 kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2475 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/params.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.759393 kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)       21 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1607 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/params.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2304 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kJobs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4817 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaiH5.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5485 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaiTools.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    11995 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaiViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2405 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaijson.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5401 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaixdmf.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1302 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kdefs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2709 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/lfm2kaiju.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.762688 kaipy-0.0.3/kaipy/paraview/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/paraview/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1207 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/paraview/pvGam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2649 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/paraview/pvutils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.767413 kaipy-0.0.3/kaipy/rcm/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/__init__.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.775646 kaipy-0.0.3/kaipy/rcm/lambdautils/
+-rw-r--r--   0 winteel1   (503) staff       (20)     1707 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/AlamData.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2469 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/AlamParams.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     6869 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/DistTypes.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2135 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/fileIO.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1932 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/genAlam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4036 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/plotter.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.783849 kaipy-0.0.3/kaipy/rcm/lambdautils_old/
+-rw-r--r--   0 winteel1   (503) staff       (20)     4504 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/AlamData.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5507 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/alamTester.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5780 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpRangeEval.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10132 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpetadp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     6896 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/genAlam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      309 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/helperdefs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     9050 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/plotter.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/rcminit.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3653 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/rcmutils.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3493 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/rcmxdmf.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.786341 kaipy-0.0.3/kaipy/rcm/wmutils/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/wmutils/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3191 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/wmutils/genWM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      521 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/wmutils/wmData.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.787942 kaipy-0.0.3/kaipy/remix/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/remix/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    29846 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/remix/remix.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.797448 kaipy-0.0.3/kaipy/solarWind/
+-rw-r--r--   0 winteel1   (503) staff       (20)    39655 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/CUSTOM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    24499 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/OMNI.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7272 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/SolarWind.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1950 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/TimeSeries.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    43184 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/WIND.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     9375 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/jdutil.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     8166 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/ols.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10440 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/swBCplots.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    32846 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/supermage.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    21838 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/transform.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.729351 kaipy-0.0.3/kaipy.egg-info/
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/PKG-INFO
+-rw-r--r--   0 winteel1   (503) staff       (20)     2314 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/SOURCES.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)        1 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/dependency_links.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)      285 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/requires.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)        6 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/top_level.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)       38 2023-06-09 13:43:23.800391 kaipy-0.0.3/setup.cfg
+-rw-r--r--   0 winteel1   (503) staff       (20)     1289 2023-06-09 13:43:20.000000 kaipy-0.0.3/setup.py
```

### Comparing `kaipy-0.0.2/PKG-INFO` & `kaipy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Postprocessing code for models in the kaiju software system
 Home-page: https://bitbucket.org/aplkaiju/kaiju/src/master/
 Author: Center for Geospace Storms
 Author-email: eric.winter@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kaipy-0.0.2/kaipy/chimp/chimph5p.py` & `kaipy-0.0.3/kaipy/chimp/chimph5p.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/chimp/chimpviz.py` & `kaipy-0.0.3/kaipy/chimp/chimpviz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/chimp/kCyl.py` & `kaipy-0.0.3/kaipy/chimp/kCyl.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/embiggenUtils.py` & `kaipy-0.0.3/kaipy/embiggenUtils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/block_gampp.py` & `kaipy-0.0.3/kaipy/gamera/block_gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/deltabViz.py` & `kaipy-0.0.3/kaipy/gamera/deltabViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/gamGrids.py` & `kaipy-0.0.3/kaipy/gamera/gamGrids.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/gampp.py` & `kaipy-0.0.3/kaipy/gamera/gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/magsphere.py` & `kaipy-0.0.3/kaipy/gamera/magsphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/magsphereRescale.py` & `kaipy-0.0.3/kaipy/gamera/magsphereRescale.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/msphViz.py` & `kaipy-0.0.3/kaipy/gamera/msphViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/rcmpp.py` & `kaipy-0.0.3/kaipy/gamera/rcmpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamera/remixpp.py` & `kaipy-0.0.3/kaipy/gamera/remixpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/helioViz.py` & `kaipy-0.0.3/kaipy/gamhelio/helioViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/heliosphere.py` & `kaipy-0.0.3/kaipy/gamhelio/heliosphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/ace.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/ace.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/cspice.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/cspice.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/lfmhlib.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/lfmhlib.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/mas.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/mas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/msgr.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/msgr.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/poisson.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/poisson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/util.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/util.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/wsa.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/wsa.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/lib/wsa2h5.py` & `kaipy-0.0.3/kaipy/gamhelio/lib/wsa2h5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/wsa2TDgamera/params.py` & `kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/gamhelio/wsa2gamera/params.py` & `kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kJobs.py` & `kaipy-0.0.3/kaipy/kJobs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kaiH5.py` & `kaipy-0.0.3/kaipy/kaiH5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kaiTools.py` & `kaipy-0.0.3/kaipy/kaiTools.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kaiViz.py` & `kaipy-0.0.3/kaipy/kaiViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kaijson.py` & `kaipy-0.0.3/kaipy/kaijson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kaixdmf.py` & `kaipy-0.0.3/kaipy/kaixdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/kdefs.py` & `kaipy-0.0.3/kaipy/kdefs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/lfm2kaiju.py` & `kaipy-0.0.3/kaipy/lfm2kaiju.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/paraview/pvGam.py` & `kaipy-0.0.3/kaipy/paraview/pvGam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/paraview/pvutils.py` & `kaipy-0.0.3/kaipy/paraview/pvutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils/AlamData.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils/AlamParams.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils/AlamParams.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils/DistTypes.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils/DistTypes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils/fileIO.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils/fileIO.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils/genAlam.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils/plotter.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils_old/AlamData.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils_old/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils_old/alamTester.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils_old/alamTester.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils_old/dpRangeEval.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpRangeEval.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils_old/dpetadp.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpetadp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils_old/genAlam.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils_old/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/lambdautils_old/plotter.py` & `kaipy-0.0.3/kaipy/rcm/lambdautils_old/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/rcminit.py` & `kaipy-0.0.3/kaipy/rcm/rcminit.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/rcmutils.py` & `kaipy-0.0.3/kaipy/rcm/rcmutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/rcmxdmf.py` & `kaipy-0.0.3/kaipy/rcm/rcmxdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/wmutils/genWM.py` & `kaipy-0.0.3/kaipy/rcm/wmutils/genWM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/rcm/wmutils/wmData.py` & `kaipy-0.0.3/kaipy/rcm/wmutils/wmData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/remix/remix.py` & `kaipy-0.0.3/kaipy/remix/remix.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/CUSTOM.py` & `kaipy-0.0.3/kaipy/solarWind/CUSTOM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/OMNI.py` & `kaipy-0.0.3/kaipy/solarWind/OMNI.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/SolarWind.py` & `kaipy-0.0.3/kaipy/solarWind/SolarWind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/TimeSeries.py` & `kaipy-0.0.3/kaipy/solarWind/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/WIND.py` & `kaipy-0.0.3/kaipy/solarWind/WIND.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/jdutil.py` & `kaipy-0.0.3/kaipy/solarWind/jdutil.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/ols.py` & `kaipy-0.0.3/kaipy/solarWind/ols.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/solarWind/swBCplots.py` & `kaipy-0.0.3/kaipy/solarWind/swBCplots.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/supermage.py` & `kaipy-0.0.3/kaipy/supermage.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy/transform.py` & `kaipy-0.0.3/kaipy/transform.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.2/kaipy.egg-info/PKG-INFO` & `kaipy-0.0.3/kaipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaipy
-Version: 0.0.2
+Version: 0.0.3
 Summary: Postprocessing code for models in the kaiju software system
 Home-page: https://bitbucket.org/aplkaiju/kaiju/src/master/
 Author: Center for Geospace Storms
 Author-email: eric.winter@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kaipy-0.0.2/kaipy.egg-info/SOURCES.txt` & `kaipy-0.0.3/kaipy.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 kaipy/kdefs.py
 kaipy/lfm2kaiju.py
 kaipy/supermage.py
 kaipy/transform.py
 kaipy.egg-info/PKG-INFO
 kaipy.egg-info/SOURCES.txt
 kaipy.egg-info/dependency_links.txt
+kaipy.egg-info/requires.txt
 kaipy.egg-info/top_level.txt
 kaipy/chimp/__init__.py
 kaipy/chimp/chimph5p.py
 kaipy/chimp/chimpviz.py
 kaipy/chimp/kCyl.py
 kaipy/gamera/__init__.py
 kaipy/gamera/block_gampp.py
```

