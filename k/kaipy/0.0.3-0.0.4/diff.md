# Comparing `tmp/kaipy-0.0.3.tar.gz` & `tmp/kaipy-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaipy-0.0.3.tar", last modified: Fri Jun  9 13:43:23 2023, max compression
+gzip compressed data, was "kaipy-0.0.4.tar", last modified: Fri Jun  9 15:30:54 2023, max compression
```

## Comparing `kaipy-0.0.3.tar` & `kaipy-0.0.4.tar`

### file list

```diff
@@ -1,104 +1,106 @@
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.800114 kaipy-0.0.3/
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 13:43:23.799385 kaipy-0.0.3/PKG-INFO
--rw-r--r--   0 winteel1   (503) staff       (20)      466 2023-06-09 13:13:22.000000 kaipy-0.0.3/README.md
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.725434 kaipy-0.0.3/kaipy/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/__init__.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.732744 kaipy-0.0.3/kaipy/chimp/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2297 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/chimph5p.py
--rw-r--r--   0 winteel1   (503) staff       (20)      922 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/chimpviz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1804 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/chimp/kCyl.py
--rw-r--r--   0 winteel1   (503) staff       (20)    13945 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/embiggenUtils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.743767 kaipy-0.0.3/kaipy/gamera/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    15993 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/block_gampp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3222 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/deltabViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)    19760 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/gamGrids.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7728 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/gampp.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10953 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/magsphere.py
--rw-r--r--   0 winteel1   (503) staff       (20)    14494 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/magsphereRescale.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7031 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/msphViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4119 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/rcmpp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3519 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamera/remixpp.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.746330 kaipy-0.0.3/kaipy/gamhelio/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    12994 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/helioViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)    14894 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/heliosphere.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.755741 kaipy-0.0.3/kaipy/gamhelio/lib/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2575 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/ace.py
--rw-r--r--   0 winteel1   (503) staff       (20)      758 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/cspice.py
--rw-r--r--   0 winteel1   (503) staff       (20)    12020 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/lfmhlib.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5369 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/mas.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1322 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/msgr.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4803 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/poisson.py
--rw-r--r--   0 winteel1   (503) staff       (20)      833 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/util.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3457 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/wsa.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     1064 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/lib/wsa2h5.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.757366 kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2475 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/params.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.759393 kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/
--rw-r--r--   0 winteel1   (503) staff       (20)       21 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1607 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/params.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2304 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kJobs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4817 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaiH5.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5485 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaiTools.py
--rw-r--r--   0 winteel1   (503) staff       (20)    11995 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaiViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2405 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaijson.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5401 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kaixdmf.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1302 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/kdefs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2709 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/lfm2kaiju.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.762688 kaipy-0.0.3/kaipy/paraview/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/paraview/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1207 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/paraview/pvGam.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2649 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/paraview/pvutils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.767413 kaipy-0.0.3/kaipy/rcm/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/__init__.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.775646 kaipy-0.0.3/kaipy/rcm/lambdautils/
--rw-r--r--   0 winteel1   (503) staff       (20)     1707 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/AlamData.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2469 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/AlamParams.py
--rw-r--r--   0 winteel1   (503) staff       (20)     6869 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/DistTypes.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2135 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/fileIO.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1932 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/genAlam.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4036 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils/plotter.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.783849 kaipy-0.0.3/kaipy/rcm/lambdautils_old/
--rw-r--r--   0 winteel1   (503) staff       (20)     4504 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/AlamData.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5507 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/alamTester.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5780 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpRangeEval.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10132 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpetadp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     6896 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/genAlam.py
--rw-r--r--   0 winteel1   (503) staff       (20)      309 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/helperdefs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     9050 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/lambdautils_old/plotter.py
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/rcminit.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3653 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/rcmutils.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3493 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/rcmxdmf.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.786341 kaipy-0.0.3/kaipy/rcm/wmutils/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/wmutils/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3191 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/wmutils/genWM.py
--rw-r--r--   0 winteel1   (503) staff       (20)      521 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/rcm/wmutils/wmData.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.787942 kaipy-0.0.3/kaipy/remix/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/remix/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    29846 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/remix/remix.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.797448 kaipy-0.0.3/kaipy/solarWind/
--rw-r--r--   0 winteel1   (503) staff       (20)    39655 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/CUSTOM.py
--rw-r--r--   0 winteel1   (503) staff       (20)    24499 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/OMNI.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7272 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/SolarWind.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1950 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/TimeSeries.py
--rw-r--r--   0 winteel1   (503) staff       (20)    43184 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/WIND.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     9375 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/jdutil.py
--rw-r--r--   0 winteel1   (503) staff       (20)     8166 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/ols.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10440 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/solarWind/swBCplots.py
--rw-r--r--   0 winteel1   (503) staff       (20)    32846 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/supermage.py
--rw-r--r--   0 winteel1   (503) staff       (20)    21838 2023-06-09 13:13:23.000000 kaipy-0.0.3/kaipy/transform.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 13:43:23.729351 kaipy-0.0.3/kaipy.egg-info/
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/PKG-INFO
--rw-r--r--   0 winteel1   (503) staff       (20)     2314 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/SOURCES.txt
--rw-r--r--   0 winteel1   (503) staff       (20)        1 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/dependency_links.txt
--rw-r--r--   0 winteel1   (503) staff       (20)      285 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/requires.txt
--rw-r--r--   0 winteel1   (503) staff       (20)        6 2023-06-09 13:43:23.000000 kaipy-0.0.3/kaipy.egg-info/top_level.txt
--rw-r--r--   0 winteel1   (503) staff       (20)       38 2023-06-09 13:43:23.800391 kaipy-0.0.3/setup.cfg
--rw-r--r--   0 winteel1   (503) staff       (20)     1289 2023-06-09 13:43:20.000000 kaipy-0.0.3/setup.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.933716 kaipy-0.0.4/
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:30:54.932873 kaipy-0.0.4/PKG-INFO
+-rw-r--r--   0 winteel1   (503) staff       (20)      466 2023-06-09 15:27:03.000000 kaipy-0.0.4/README.md
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.846899 kaipy-0.0.4/kaipy/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    23712 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/cdaweb_utils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.856578 kaipy-0.0.4/kaipy/chimp/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2297 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/chimph5p.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      922 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/chimpviz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1804 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/kCyl.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    13945 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/embiggenUtils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.868155 kaipy-0.0.4/kaipy/gamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    15993 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/block_gampp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3222 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/deltabViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    19760 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/gamGrids.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     8111 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/gamera/gampp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10963 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/gamera/magsphere.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    14527 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/gamera/magsphereRescale.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7031 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/msphViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4119 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/rcmpp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3519 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/remixpp.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.873663 kaipy-0.0.4/kaipy/gamhelio/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    12994 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/helioViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    14894 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/heliosphere.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.885682 kaipy-0.0.4/kaipy/gamhelio/lib/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2575 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/ace.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      758 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/cspice.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    12020 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/lfmhlib.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5369 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/mas.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1322 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/msgr.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4803 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/poisson.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      833 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/util.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     3457 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/wsa.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     1064 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/wsa2h5.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.887948 kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2475 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/params.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.890143 kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)       21 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1607 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/params.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2304 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/kJobs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5899 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kaiH5.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5485 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/kaiTools.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    21531 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kaiViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2405 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/kaijson.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5950 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kaixdmf.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1428 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kdefs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2709 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/lfm2kaiju.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.893279 kaipy-0.0.4/kaipy/paraview/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/paraview/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1207 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/paraview/pvGam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2649 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/paraview/pvutils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.897517 kaipy-0.0.4/kaipy/rcm/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/__init__.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.906294 kaipy-0.0.4/kaipy/rcm/lambdautils/
+-rw-r--r--   0 winteel1   (503) staff       (20)     1707 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/AlamData.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2469 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/AlamParams.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     6869 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/DistTypes.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2135 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/fileIO.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1932 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/genAlam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4036 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/plotter.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.914867 kaipy-0.0.4/kaipy/rcm/lambdautils_old/
+-rw-r--r--   0 winteel1   (503) staff       (20)     4504 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/AlamData.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5507 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/alamTester.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5780 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpRangeEval.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10132 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpetadp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     6896 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/genAlam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      309 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/helperdefs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     9050 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/plotter.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/rcminit.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3653 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/rcmutils.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3493 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/rcmxdmf.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.918480 kaipy-0.0.4/kaipy/rcm/wmutils/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/wmutils/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4095 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/rcm/wmutils/genWM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      694 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/rcm/wmutils/wmData.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.921327 kaipy-0.0.4/kaipy/remix/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/remix/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    29846 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/remix/remix.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.931586 kaipy-0.0.4/kaipy/solarWind/
+-rw-r--r--   0 winteel1   (503) staff       (20)    39786 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/solarWind/CUSTOM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    24794 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/solarWind/OMNI.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7272 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/SolarWind.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1950 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/TimeSeries.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    43184 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/WIND.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     9375 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/jdutil.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     8166 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/ols.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10900 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/solarWind/swBCplots.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    25735 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/supermag_api.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    32873 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/supermage.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2409 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/transform.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.852445 kaipy-0.0.4/kaipy.egg-info/
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/PKG-INFO
+-rw-r--r--   0 winteel1   (503) staff       (20)     2358 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/SOURCES.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)        1 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/dependency_links.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)      285 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/requires.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)        6 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/top_level.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)       38 2023-06-09 15:30:54.934134 kaipy-0.0.4/setup.cfg
+-rw-r--r--   0 winteel1   (503) staff       (20)     1289 2023-06-09 15:29:25.000000 kaipy-0.0.4/setup.py
```

### Comparing `kaipy-0.0.3/PKG-INFO` & `kaipy-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaipy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Postprocessing code for models in the kaiju software system
 Home-page: https://bitbucket.org/aplkaiju/kaiju/src/master/
 Author: Center for Geospace Storms
 Author-email: eric.winter@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kaipy-0.0.3/kaipy/chimp/chimph5p.py` & `kaipy-0.0.4/kaipy/chimp/chimph5p.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/chimp/chimpviz.py` & `kaipy-0.0.4/kaipy/chimp/chimpviz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/chimp/kCyl.py` & `kaipy-0.0.4/kaipy/chimp/kCyl.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/embiggenUtils.py` & `kaipy-0.0.4/kaipy/embiggenUtils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamera/block_gampp.py` & `kaipy-0.0.4/kaipy/gamera/block_gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamera/deltabViz.py` & `kaipy-0.0.4/kaipy/gamera/deltabViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamera/gamGrids.py` & `kaipy-0.0.4/kaipy/gamera/gamGrids.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamera/gampp.py` & `kaipy-0.0.4/kaipy/gamera/gampp.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 #Gamera post-processing routines
 #Get data from serial/MPI gamera output
 import glob
 import numpy as np
 from kaipy.kaiTools import MJD2UT
+import itertools
+import kaipy.kdefs as kdefs
 
 #Object to use to pull data from HDF5 structure (serial or mpi)
 
 #Initialize,
 #gIn = gampp.GameraPipe(fdir,ftag)
 #Set grid from data
 #gIn.GetGrid()
@@ -162,92 +164,103 @@
 			print("Variables (Root/Step) = (%d,%d)"%(self.Nv0,self.Nv))
 			print("\tRoot: %s"%(self.v0IDs))
 			print("\tStep: %s"%(self.vIDs))
 
 		self.SetUnits(f0)
 		if (doVerbose):
 			print("Units Type = %s"%(self.UnitsID))
-			print("Pulling grid ...")
+			#print("Pulling grid ...")
 		self.GetGrid(doVerbose)
 		self.f0 = f0
 
 	def SetUnits(self,f0):
 		import h5py
 		with h5py.File(f0,'r') as hf:
 			uID = hf.attrs.get("UnitsID","CODE")
 		if (not isinstance(uID,str)):
 			self.UnitsID = uID.decode('utf-8')
 
 	def GetGrid(self,doVerbose):
 		import kaipy.kaiH5 as kh5
+		from alive_progress import alive_bar
 		if (self.is2D):
 			self.X = np.zeros((self.Ni+1,self.Nj+1))
 			self.Y = np.zeros((self.Ni+1,self.Nj+1))
 		else:
 			self.X = np.zeros((self.Ni+1,self.Nj+1,self.Nk+1))
 			self.Y = np.zeros((self.Ni+1,self.Nj+1,self.Nk+1))
 			self.Z = np.zeros((self.Ni+1,self.Nj+1,self.Nk+1))
 		if (doVerbose):
-			print("Del = (%d,%d,%d)"%(self.dNi,self.dNj,self.dNk))
-		for i in range(self.Ri):
-			for j in range(self.Rj):
-				for k in range(self.Rk):
-					iS = i*self.dNi
-					jS = j*self.dNj
-					kS = k*self.dNk
-					iE = iS+self.dNi
-					jE = jS+self.dNj
-					kE = kS+self.dNk
-					#print("Bounds = (%d,%d,%d,%d,%d,%d)"%(iS,iE,jS,jE,kS,kE))
-					if (self.isMPI):
-						fIn = self.fdir + "/" + kh5.genName(self.ftag,i,j,k,self.Ri,self.Rj,self.Rk)
-					else:
-						fIn = self.fdir + "/" + self.ftag + ".h5"
-					if (self.is2D):
-						self.X[iS:iE+1,jS:jE+1] = kh5.PullVar(fIn,"X")
-						self.Y[iS:iE+1,jS:jE+1] = kh5.PullVar(fIn,"Y")
-					else:
-						self.X[iS:iE+1,jS:jE+1,kS:kE+1] = kh5.PullVar(fIn,"X")
-						self.Y[iS:iE+1,jS:jE+1,kS:kE+1] = kh5.PullVar(fIn,"Y")
-						self.Z[iS:iE+1,jS:jE+1,kS:kE+1] = kh5.PullVar(fIn,"Z")
+			#print("Del = (%d,%d,%d)"%(self.dNi,self.dNj,self.dNk))
+			titStr = "%s/Grid"%(self.ftag)
+		else:
+			titStr = None
+		NrX = max(self.Nr,1)
+		with alive_bar(NrX,title=titStr,length=kdefs.barLen) as bar:
+			for (i,j,k) in itertools.product(range(self.Ri),range(self.Rj),range(self.Rk)):
+				iS = i *self.dNi
+				jS = j *self.dNj
+				kS = k *self.dNk
+				iE = iS+self.dNi
+				jE = jS+self.dNj
+				kE = kS+self.dNk
+				#print("Bounds = (%d,%d,%d,%d,%d,%d)"%(iS,iE,jS,jE,kS,kE))
+				if (self.isMPI):
+					fIn = self.fdir + "/" + kh5.genName(self.ftag,i,j,k,self.Ri,self.Rj,self.Rk)
+				else:
+					fIn = self.fdir + "/" + self.ftag + ".h5"
+				if (self.is2D):
+					self.X[iS:iE+1,jS:jE+1] = kh5.PullVar(fIn,"X")
+					self.Y[iS:iE+1,jS:jE+1] = kh5.PullVar(fIn,"Y")
+				else:
+					self.X[iS:iE+1,jS:jE+1,kS:kE+1] = kh5.PullVar(fIn,"X")
+					self.Y[iS:iE+1,jS:jE+1,kS:kE+1] = kh5.PullVar(fIn,"Y")
+					self.Z[iS:iE+1,jS:jE+1,kS:kE+1] = kh5.PullVar(fIn,"Z")
+				bar()
 	#Get 3D variable "vID" from Step# sID
 	def GetVar(self,vID,sID=None,vScl=None,doVerb=True):
 		import kaipy.kaiH5 as kh5
-
+		from alive_progress import alive_bar
 		if (doVerb):
 			if (sID is None):
-				print("Reading %s/%s"%(self.ftag,vID))
+				titStr = "%s/%s"%(self.ftag,vID)
+				
 			else:
-				print("Reading %s/Step#%d/%s"%(self.ftag,sID,vID))
+				titStr = "%s/Step#%d/%s"%(self.ftag,sID,vID)
+		else:
+			titStr = ''
 
 		if (self.is2D):
 			V = np.zeros((self.Ni,self.Nj))
 		else:
 			V = np.zeros((self.Ni,self.Nj,self.Nk))
 
-		for i in range(self.Ri):
-			for j in range(self.Rj):
-				for k in range(self.Rk):
-					iS = i*self.dNi
-					jS = j*self.dNj
-					kS = k*self.dNk
-					iE = iS+self.dNi
-					jE = jS+self.dNj
-					kE = kS+self.dNk
-					#print("Bounds = (%d,%d,%d,%d,%d,%d)"%(iS,iE,jS,jE,kS,kE))
-					if (self.isMPI):
-						fIn = self.fdir + "/" + kh5.genName(self.ftag,i,j,k,self.Ri,self.Rj,self.Rk)
-					else:
-						fIn = self.fdir + "/" + self.ftag + ".h5"
-
-					if (self.is2D):
-						V[iS:iE,jS:jE] = kh5.PullVar(fIn,vID,sID)
-
-					else:
-						V[iS:iE,jS:jE,kS:kE] = kh5.PullVar(fIn,vID,sID)
+		NrX = max(self.Nr,1)
+		
+		with alive_bar(NrX,title=titStr.ljust(kdefs.barLab),length=kdefs.barLen) as bar:
+			for (i,j,k) in itertools.product(range(self.Ri),range(self.Rj),range(self.Rk)):
+
+				iS = i*self.dNi
+				jS = j*self.dNj
+				kS = k*self.dNk
+				iE = iS+self.dNi
+				jE = jS+self.dNj
+				kE = kS+self.dNk
+				#print("Bounds = (%d,%d,%d,%d,%d,%d)"%(iS,iE,jS,jE,kS,kE))
+				if (self.isMPI):
+					fIn = self.fdir + "/" + kh5.genName(self.ftag,i,j,k,self.Ri,self.Rj,self.Rk)
+				else:
+					fIn = self.fdir + "/" + self.ftag + ".h5"
+
+				if (self.is2D):
+					V[iS:iE,jS:jE] = kh5.PullVar(fIn,vID,sID)
+
+				else:
+					V[iS:iE,jS:jE,kS:kE] = kh5.PullVar(fIn,vID,sID)
+				bar()
 		if (vScl is not None):
 			V = vScl*V
 		return V
 
 	#Get variable slice of constant i,j,k
 	#Directions = idir/jdir/kdir strings
 	#Indexing = (1,Nijk)
```

### Comparing `kaipy-0.0.3/kaipy/gamera/magsphere.py` & `kaipy-0.0.4/kaipy/gamera/magsphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,16 +133,16 @@
 		rmOuts = glob.glob(rmOStr)
 		Nrm = len(rmOuts)
 		if (Nrm>0):
 			mixtag = Stubs[0]+".mix"
 			self.hasRemix = True
 			print("Found ReMIX data, reading ...")
 			self.mixPipe = GameraPipe(self.fdir,mixtag,doVerbose=False)
-			self.nCPCP = kh5.getTs(rmOStr,sIds=None,aID="nCPCP")
-			self.sCPCP = kh5.getTs(rmOStr,sIds=None,aID="sCPCP")
+			self.nCPCP = kh5.getTs(rmOStr,sIds=self.sids,aID="nCPCP")
+			self.sCPCP = kh5.getTs(rmOStr,sIds=self.sids,aID="sCPCP")
 	#Get magnetic moment from file
 	def GetM0(self):
 		import h5py
 		with h5py.File(self.f0,'r') as hf:
 			M0 = hf.attrs.get("MagM0",self.MagM)
 		#Store value
 		self.MagM = M0
```

### Comparing `kaipy-0.0.3/kaipy/gamera/magsphereRescale.py` & `kaipy-0.0.4/kaipy/gamera/magsphereRescale.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,16 +14,15 @@
 KDIR = 2
 
 #Push restart data to an MPI tiling
 #fInA is a restart file to pull attributes from
 # add oG and oM for one step older for reproducible restart.
 # These variables are used by mhd predictor/corrector.
 def PushRestartMPI(outid,nRes,Ri,Rj,Rk,X,Y,Z,G,M,oG,oM,fInA,G0=None):
-	if (G0 is not None):
-		doGas0 = True
+	doGas0 = (G0 is not None)  # Make sure doGas0 is either True or False
 
 	print("Reading attributes from %s"%(fInA))
 	iH5 = h5py.File(fInA,'r')
 
 	Ns,Nv,Nk,Nj,Ni = G.shape
 	#Create output files
 	Nkp = Nk//Rk
```

### Comparing `kaipy-0.0.3/kaipy/gamera/msphViz.py` & `kaipy-0.0.4/kaipy/gamera/msphViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamera/rcmpp.py` & `kaipy-0.0.4/kaipy/gamera/rcmpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamera/remixpp.py` & `kaipy-0.0.4/kaipy/gamera/remixpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/helioViz.py` & `kaipy-0.0.4/kaipy/gamhelio/helioViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/heliosphere.py` & `kaipy-0.0.4/kaipy/gamhelio/heliosphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/ace.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/ace.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/cspice.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/cspice.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/lfmhlib.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/lfmhlib.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/mas.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/mas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/msgr.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/msgr.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/poisson.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/poisson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/util.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/util.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/wsa.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/wsa.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/lib/wsa2h5.py` & `kaipy-0.0.4/kaipy/gamhelio/lib/wsa2h5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/wsa2TDgamera/params.py` & `kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/gamhelio/wsa2gamera/params.py` & `kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/kJobs.py` & `kaipy-0.0.4/kaipy/kJobs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/kaiH5.py` & `kaipy-0.0.4/kaipy/kaiH5.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import h5py
 import numpy as np
-import sys
+import os, sys, subprocess
+import kaipy.kdefs as kdefs
 
 #Generate MPI-style name
 def genName(bStr,i,j,k,Ri,Rj,Rk,nRes=None):
 	n = k + j*Rk + i*Rj*Rk
 	if (nRes is None):
 		fID = bStr + "_%04d_%04d_%04d_%04d_%04d_%04d.gam.h5"%(Ri,Rj,Rk,i,j,k)
 	else:
@@ -31,14 +32,37 @@
 #Check directory exists and make it if not
 def CheckDirOrMake(fdir):
 	import os
 	isDir = os.path.isdir(fdir)
 	if (not isDir):
 		print("Creating %s"%(fdir))
 		os.makedirs(fdir)
+
+# Stamp file with git hash (using this script's location)
+def StampHash(fname):
+	with h5py.File(fname, 'a') as f5:
+		cwd = os.path.dirname(os.path.realpath(__file__))
+		try:
+			gh = subprocess.check_output(['git', '-C', cwd, 'rev-parse', 'HEAD']).decode('ascii').strip()
+		except:
+			print("ERROR: Couldn't grab git hash")
+			gh = "XXXXX"
+		f5.attrs['GITHASH'] = gh
+
+# Stamp file with git branch (using this script's location)
+def StampBranch(fname):
+	with h5py.File(fname, 'a') as f5:
+		cwd = os.path.dirname(os.path.realpath(__file__))
+		try:
+			gb = subprocess.check_output(['git', '-C', cwd, 'rev-parse', '--abbrev-ref', 'HEAD']).decode('ascii').strip()
+		except:
+			print("ERROR: Couldn't grab git branch")
+			gb = "XXXXX"
+		f5.attrs['GITBRANCH'] = gb
+
 #Get git hash from file if it exists
 def GetHash(fname):
 	CheckOrDie(fname)
 	with h5py.File(fname,'r') as hf:
 		rStr = hf.attrs.get("GITHASH","NONE")
 	try:
 		hStr = rStr.decode('utf-8')
@@ -66,21 +90,24 @@
 		if aID in hf[gID].attrs:
 			t = hf[gID].attrs[aID]
 		else:
 			t = aDef
 	return t
 	
 def cntSteps(fname,doTryRecover=True,s0=0):
+	from alive_progress import alive_it
 
 	try:
 		CheckOrDie(fname)
 		with h5py.File(fname,'r') as hf:
-			Steps = [grp for grp in hf.keys() if "Step#" in grp]
+			Steps = [grp for grp in alive_it(hf.keys(),title="#-Steps".ljust(kdefs.barLab),length=kdefs.barLen) if "Step#" in grp]
 		sIds = np.array([str.split(s,"#")[-1] for s in Steps],dtype=np.int)
+		sIds.sort()
 		nSteps = len(Steps)
+		
 		return nSteps,sIds
 	except (ValueError, IndexError) as e:
 		print("!!Warning: h5 file contains unreadable steps")
 
 	if not doTryRecover:
 		print("  Can try again with 'cntSteps(fname,doTryRecover=True)'")
 		raise ValueError("Unreadable steps")
@@ -99,14 +126,15 @@
 					print("Read step " + str(s))
 				except ValueError:
 					badCounts += 1
 					print("Bad count on step " + str(s))
 				s+=1
 			nSteps = len(sIds)
 			sIds = np.array(sIds)
+			sIds.sort()
 		return nSteps,sIds
 
 #More general version of cntSteps, useful for Step#X/Line#Y
 def cntX(fname,gID=None,StrX="/Step#"):
 	with h5py.File(fname,'r') as hf:
 		if (gID is not None):
 			grps = hf[gID].values()
@@ -114,28 +142,32 @@
 			grps = hf.values()
 		grpNames = [str(grp.name) for grp in grps]
 		#Steps = [stp if "/Step#" in stp for stp in grpNames]
 		Steps = [stp for stp in grpNames if StrX in stp]
 		nSteps = len(Steps)
 
 		sIds = np.array([str.split(s,"#")[-1] for s in Steps],dtype=np.int)
+		sIds.sort()
 		return nSteps,sIds
 
 def getTs(fname,sIds=None,aID="time",aDef=0.0):
+	from alive_progress import alive_bar
+	
 	if (sIds is None):
 		nSteps,sIds = cntSteps(fname)
 	Nt = len(sIds)
 	T = np.zeros(Nt)
-	i0 = sIds.min()
-	i1 = sIds.max()
 	CheckOrDie(fname)
-	with h5py.File(fname,'r') as hf:
-		for n in range(i0,i1+1):
+	titStr = "Time series: %s"%(aID)
+
+	with h5py.File(fname,'r') as hf, alive_bar(Nt,title=titStr.ljust(kdefs.barLab),length=kdefs.barLen) as bar:
+		for idx, n in enumerate(sIds):
 			gId = "/Step#%d"%(n)
-			T[n-i0] = hf[gId].attrs.get(aID,aDef)
+			T[idx] = hf[gId].attrs.get(aID,aDef)
+			bar()
 	return T
 
 #Get shape/dimension of grid
 def getDims(fname,vID="X",doFlip=True):
 	CheckOrDie(fname)
 	with h5py.File(fname,'r') as hf:
 		Dims = hf["/"][vID].shape
```

### Comparing `kaipy-0.0.3/kaipy/kaiTools.py` & `kaipy-0.0.4/kaipy/kaiTools.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/kaiViz.py` & `kaipy-0.0.4/kaipy/solarWind/swBCplots.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,402 +1,295 @@
-#Various scripts to support visualization of Kaiju data
-
-from kaipy.kdefs import *
-import h5py
+"""
+Generate plots of 1d time series data stored as pyLTR.TimeSeries
+objects.  See examples/TimeSeriesPlots.py for usage.
+"""
+from kaipy.solarWind.TimeSeries import TimeSeries
+import datetime
+from matplotlib import dates
 import numpy as np
-import matplotlib as mpl
 import matplotlib.pyplot as plt
-from matplotlib.colors import LogNorm
-from matplotlib.colors import Normalize
-
+import matplotlib.gridspec as gridspec
+import kaipy.kaiViz as kv
+import datetime
 
-#Create 2D equatorial grid (Ni,Nj*2+1) from lfm/egg-style
-def genEQGrid(fIn):
-    with h5py.File(fIn,'r') as hf:
-        Nk,Nj,Ni = hf.get("X")[()].shape
-        X3 = hf.get("X")[()].T
-        Y3 = hf.get("Y")[()].T
-        Z3 = hf.get("Z")[()].T
-    print("Ni,Nj,Nk = %d,%d,%d"%(Ni,Nj,Nk))
-    #Create grid
-    Nr = Ni-1
-    Np = 2*(Nj-1)
-    xx = np.zeros((Nr+1,Np+1))
-    yy = np.zeros((Nr+1,Np+1))
-
-    for i in range(Nr+1):
-        for j in range(Nj):
-            xx[i,j] = X3[i,j,0]
-            yy[i,j] = Y3[i,j,0]
-        for j in range(Nj,Np+1):
-            jp = Np-j
-            xx[i,j] =  X3[i,jp,0]
-            yy[i,j] = -Y3[i,jp,0]
-    return xx,yy
-def getEQVar(fIn,StpN=0,vID="D"):
-    gID = "Step#%d"%(StpN)
-    with h5py.File(fIn,'r') as hf:
-        V = hf.get(gID).get(vID)[()].T
-        Ni,Nj,Nk = V.shape #Cell-centered (not node)
-    Nr = Ni
-    Np = 2*(Nj)
-    kp = (Nk)/2
-    vv = np.zeros((Nr,Np))
-    for i in range(Nr):
-        for j in range(Np):
-            if (j>=Nj):
-                jp = Np-j-1
-                vv[i,j] = V[i,jp,kp]
-            else:
-                jp = j
-                vv[i,j] = V[i,jp,0]
-    return vv
-
-#Calculate equatorial Bz-D
-def getEQBzD(xx,yy,MagM=-EarthM0g):
-    Nip,Njp = xx.shape
-    Ni = Nip-1
-    Nj = Njp-1
-
-    BzD = np.zeros((Ni,Nj))
-    xxc = np.zeros((Ni,Nj))
-    yyc = np.zeros((Ni,Nj))
-
-    for i in range(Ni):
-        for j in range(Nj):
-            xc = 0.25*(xx[i,j]+xx[i+1,j]+xx[i,j+1]+xx[i+1,j+1])
-            yc = 0.25*(yy[i,j]+yy[i+1,j]+yy[i,j+1]+yy[i+1,j+1])
-            xxc[i,j] = xc
-            yyc[i,j] = yc
-            r = np.sqrt(xc**2.0+yc**2.0)
-            rm5 = r**(-5.0)
-            BzD[i,j] = -r*r*MagM*rm5
-    return xxc,yyc,BzD
-
-#---------------------------------
-#Matplotlib helpers
-
-#Set axis bounds w/ aspect ratio
-def SetAx(xyBds=[-1,1,-1,1],ax=None,Adj='box'):
-    if ax is None:
-        ax = plt.gca()
-    ax.set_xlim(xyBds[0],xyBds[1])
-    ax.set_ylim(xyBds[2],xyBds[3])
-    ax.set_aspect('equal',adjustable=Adj)
-
-#Set axis labels and locations
-def SetAxLabs(Ax,xLab,yLab,doBot=True,doLeft=True,fs="medium"):
-    Ax.set_xlabel(xLab,fontsize=fs)
-    Ax.set_ylabel(yLab,fontsize=fs)
-    if (not doBot):
-        Ax.xaxis.tick_top()
-        Ax.xaxis.set_label_position('top')
-    if (not doLeft):
-        Ax.yaxis.tick_right()
-        Ax.yaxis.set_label_position('right')
-
-    #Kill labels if not string is None
-    if (xLab is None):
-        Ax.xaxis.label.set_visible(False)
-        Ax.xaxis.set_visible(False)
-        plt.setp(Ax.get_xticklabels(),visible=False)
-
-    if (yLab is None):
-        Ax.yaxis.label.set_visible(False)
-        Ax.yaxis.set_visible(False)
-        plt.setp(Ax.get_yticklabels(),visible=False)
-
-#Set X axis to labels to well formatted date time
-def SetAxDate(Ax,fmt='%H:%M \n%Y-%m-%d'):
-    Ax.xaxis_date()
-    Ax.xaxis.set_major_formatter(mpl.dates.DateFormatter(fmt))
-
-#Adds 2D earth w/ dawn/dusk
-def addEarth2D(Re=1, angle=-90, ax=None):
-    from matplotlib.patches import Wedge
-
-    if ax is None:
-        ax = plt.gca()
-    colors=('w','k')
-    center = 0
-    theta1, theta2 = angle, angle + 180
-
-    w1 = Wedge(center, Re,-90,90,   fc=colors[0],ec='k')
-    w2 = Wedge(center, Re, 90, -90, fc=colors[1],ec='k')
-    for wedge in [w1, w2]:
-        ax.add_artist(wedge)
-    return [w1, w2]
-#Add inner cutout
-def DrawCut(Rin=2.5,ax=None):
-    from matplotlib.patches import Wedge
-    if ax is None:
-        ax = plt.gca()
-    w1 = Wedge(0,Rin,0,360,fc=None,ec='k')
-    ax.add_artist(w1)
-    return w1
-
-#Take cell-centered polar values and add extra phi layer
-#Useful for contour plots through +X
-def reWrap(V):
-    Ni,Nj = V.shape
-    Vp = np.zeros((Ni,Nj+1))
-    Vp[:,0:Nj] = V
-    Vp[:,-1] = V[:,0]
-    return Vp
-
-#Image files
-#Wrapper to save (and trim) figure
-def savePic(fOut,dpiQ=300,doTrim=True,bLenX=20,bLenY=None,doClose=False,doEps=False):
-    #Start by saving
-    import matplotlib.pyplot as plt
-    if (doEps):
-        plt.savefig(fOut,dpi=dpiQ,format='eps')
+def BasicPlot(VarDict,Xname,Yname,Xlabel=True,color='b'):
+    """
+    Mostly a wrapper for plt.plot(...)
+    """
+    x=VarDict[Xname]
+    y=VarDict[Yname]
+        
+    # y may be a time series of tuples/lists of variables to plot 
+    # simultaneously (e.g., vector components) using different colors
+    if (np.array(y['data'][0]).size > 1 and 
+        np.array(y['data'][0]).size == len(color) and
+        all([ylen == np.array(y['data'][0]).size for ylen in map(len,y['data'])]) ):
+        for i in range(np.array(y['data'][0]).size):
+            plt.plot(x['data'], [yts[i] for yts in y['data']], color=color[i])
     else:
-        plt.savefig(fOut,dpi=dpiQ)
-        if (doTrim):
-            trimFig(fOut,bLenX,bLenY)
-    if (doClose):
-        plt.close('all')
-
-#Use imagemagick to trim whitespace off figure
-#doEven: Guarantee even number of pixels in X/Y
-def trimFig(fName,bLenX=20,bLenY=None,doEven=True):
-    import os
-    if (bLenY is None):
-        bLenY = bLenX
-
-    ComS = 'convert -trim -border %dx%d -bordercolor "#FFFFFF" '%(bLenX,bLenY) + fName + ' ' + fName
-    os.system(ComS)
-
-    if (doEven):
-        Nx,Ny = picSz(fName)
-        #print(Nx,Ny)
-        while ( (Nx % 2) != 0 ):
-            #print("Shaving X")
-            ShaveX(fName)
-            Nx,Ny = picSz(fName)
-            #print('\t%d,%d'%(Nx,Ny))
-
-        while ( (Ny % 2) != 0 ):
-            #print("Shaving Y")
-            ShaveY(fName)
-            Nx,Ny = picSz(fName)
-            #print('\t%d,%d'%(Nx,Ny))
-
-        Nx,Ny = picSz(fName)
-        if ( ((Nx % 2) != 0) or ((Ny % 2) != 0) ):
-            print("Parity failure on pic sizing")
-            print(Nx,Ny)
-
-def picSz(fName):
-    from PIL import Image
-    with Image.open(fName) as img:
-        Nx,Ny = img.size
-    return Nx,Ny
-
-def ShaveX(fName):
-    import os
-    ComS = 'convert -crop -1+0 +repage ' + fName + ' ' + fName
-    os.system(ComS)
-def ShaveY(fName):
-    import os
-    ComS = 'convert -crop +0-1 +repage ' + fName + ' ' + fName
-    os.system(ComS)
-
-#---------------------------------
-#Create colorbar with specified midpoint (grabbed from stack overflow)
-class MidpointNormalize(Normalize):
-    def __init__(self, vmin=None, vmax=None, midpoint=None, clip=False):
-        self.midpoint = midpoint
-        Normalize.__init__(self, vmin, vmax, clip)
-
-    def __call__(self, value, clip=None):
-        # I'm ignoring masked values and all kinds of edge cases to make a
-        # simple example...
-        x, y = [self.vmin, self.midpoint, self.vmax], [0, 0.5, 1]
-        return np.ma.masked_array(np.interp(value, x, y))
-
-#Create norm object for MPL
-def genNorm(vMin,vMax=None,doLog=False,doSymLog=False,midP=None,linP=1.0):
-    from matplotlib.colors import LogNorm
-    from matplotlib.colors import Normalize
-    from matplotlib.colors import SymLogNorm
-    if (vMax is None):
-        vMin = -np.abs(vMin)
-        vMax = np.abs(vMin)
-    if (midP is None):
-        doMid = False
+        plt.plot(x['data'],y['data'],color=color)
+            
+    # Xname may point to a list of datetime.datetime objects, in which case
+    # pyplot must be told to plot these as datetimes
+    if all([type(ts) == datetime.datetime for ts in x['data']]):
+        dfmt = dates.DateFormatter('%m/%d/%y-%H:%M')
+        plt.gca().xaxis.set_major_formatter(dfmt)
+    elif any([type(ts) == datetime.datetime for ts in x['data']]):
+        raise Exception('Cannot mix datetime time-axis elements with other types')
+    
+    
+    if Xlabel:
+        #locs,labels=plt.xticks()
+        xStr = x['name']
+        if len(x['units']) > 0:
+            xStr += ' ['+x['units']+']'
+        plt.xlabel(xStr)
+    else: 
+        plt.xlabel(' ')
+        #locs,labels=plt.xticks()
+        #plt.xticks(locs,(' '))
+    
+    # y['name'] may not be a scalar
+    if (np.array(y['name']).size) > 1:
+        plt.ylabel('['+y['units']+']',fontsize='small')
     else:
-        doMid = True
+        plt.ylabel(y['name']+' ['+y['units']+']',fontsize='small')
+  
+def SummaryPlot(VarDict,Xname):
+    """
+    Plot every variable in VarDict.
 
-    if (doMid):
-        vN = MidpointNormalize(vmin=vMin,vmax=vMax,midpoint=midP)
-    elif (doLog):
-        vN = LogNorm(vmin=vMin,vmax=vMax)
-    elif (doSymLog):
-        vN = SymLogNorm(linthresh=linP,vmin=vMin,vmax=vMax,base=10)
-    else:
-        vN = Normalize(vmin=vMin,vmax=vMax)
+    This is a simple wrapper around the more generic MultiPlotN.  This
+    code may have problems with varDicts that store non-time series
+    data.  You've beeen warned.
+    """
+    #Loop over elements in Dict to make sure they all have data 
+    plotVariables=[]
+    for var in VarDict.keys():
+        if isinstance(VarDict[var], dict):
+            if 'data' in VarDict[var]:
+                plotVariables.append(var)
 
-    return vN
+    MultiPlotN([VarDict], Xname, plotVariables)
 
-#Create colorbar object into specified axis
-def genCB(AxCB,vN,cbT="Title",cM="viridis",doVert=False,cbSz="medium",Ntk=None):
-    from matplotlib import ticker
 
-    if (doVert):
-        cbOr = "vertical"
-    else:
-        cbOr = "horizontal"
-    cmData = plt.get_cmap(cM)
-    cb = mpl.colorbar.ColorbarBase(AxCB,cmap=cmData,norm=vN,orientation=cbOr)
-    if (Ntk is not None):
-        cb.locator = ticker.MaxNLocator(nbins=Ntk)
-        cb.update_ticks()
-
-    cb.set_label(cbT,fontsize=cbSz)
-    cb.ax.tick_params(labelsize=cbSz)
-    return cb
-
-def labelStr(data, key, vecComp):
-    vecLabel=[ 'x', 'y', 'z' ]
-    if (vecComp < 3) and (vecComp > -1):
-        label=(data['GAMERA_'+key].attrs['AXISLABEL']+
-        vecLabel[vecComp]+' ['+
-        data['GAMERA_'+key].attrs['UNITS'].decode()+']')
-    else:
-        label=(data['GAMERA_'+key].attrs['AXISLABEL']+
-        ' ['+data['GAMERA_'+key].attrs['UNITS'].decode()+']')
-    return label
-
-
-def itemPlot(Ax,data,key,plotNum,numPlots,vecComp=-1):
-    #print(key,vecComp)
-    if -1 == vecComp:
-        if key == "Br":
-            # Plot a horizontal line at Br=0. This indicates passage of the
-            # heliospheric current sheet.
-            Ax.axhline([0], linestyle="--", color="black")
-        # <HACK>
-        if key == "Density":
-            # Reduce the density vertical scale.
-            Ax.set_ylim(0, 50)  # cm**-3
-        # </HACK>
-        maskedData = np.ma.masked_where(data['GAMERA_inDom'][:]==0.0,
-            data[key][:])
-        Ax.plot(data['Epoch_bin'],maskedData)
-        maskedGamera = np.ma.masked_where(data['GAMERA_inDom'][:]==0.0,
-            data['GAMERA_'+key][:])
-        Ax.plot(data['Epoch_bin'],maskedGamera)
-    else:
-        maskedData = np.ma.masked_where(data['GAMERA_inDom'][:]==0.0,
-            data[key][:,vecComp])
-        Ax.plot(data['Epoch_bin'],maskedData)
-        maskedGamera = np.ma.masked_where(data['GAMERA_inDom'][:]==0.0,
-            data['GAMERA_'+key][:,vecComp])
-        Ax.plot(data['Epoch_bin'],maskedGamera)
-    if (plotNum % 2) == 0:
-        left = True
-    else:
-        left = False
-    label = labelStr(data, key,vecComp)
-    if plotNum == (numPlots-1):
-        SetAxLabs(Ax,'UT',label,doLeft=left)
-        SetAxDate(Ax)
-    else:
-        SetAxLabs(Ax,None,label,doLeft=left)
-    return
+def MultiPlot(VarDict,Xname,Items,color='b'):
+    """
+    Plot variables stored in TimeSeries object 'varDict'.
 
-def helioCompPlot(plotname, scId, data):
-    """Create comparison plots for heliospheric results.
+    This is a simple wrapper around the more generic MultiPlotN.
+    """
+    MultiPlotN([VarDict], Xname, Items, [color],[])
+    
+def MultiPlot2(VarDict,VarDict2,Xname,Items,color1='b',color2='r'):
+    """
+    Plot items (stored in TimeSeries objects VarDict and VarDict2)
+    against one another.  One sub plot for each item.
 
-    Create comparison plots for heliospheric results and save the plots to a
-    file.
+    This is a simple wrapper around the more generic MultiPlotN.
+    """
+    MultiPlotN([VarDict, VarDict2],
+               Xname,
+               Items,
+               [color1, color2],
+               [])
 
-    Parameters
-    ----------
-    plotname : str
-        Path to file to hold plot image.
-    scId : str
-        ID string for spacecraft.
-    data : spacepy.datamodel.SpaceData
-        The current spacecraft and model data
-
-    Returns
-    -------
-    None
-    """
-    # Determine which data are available to plot.
-    numPlots = 0
-    keysToPlot = []
-    keys = data.keys()
-    if "Speed" in keys:
-        keysToPlot.append("Speed")
-    if "Br" in keys:
-        keysToPlot.append("Br")
-    if "Density" in keys:
-        keysToPlot.append("Density")
-    if "Temperature" in keys:
-        keysToPlot.append("Temperature")
-    numPlots = len(keysToPlot)
-
-    # Create the figure to hold the plots.
-    figsize = (10, 10)
-    fig = plt.figure(figsize=figsize)
-    gs = fig.add_gridspec(numPlots, 1)
-
-    # Plot each variabble in its own subplot.
-    plotNum = 0
-    for key in keysToPlot:
-        if plotNum == 0:
-            ax1 = fig.add_subplot(gs[plotNum, 0])
-            itemPlot(ax1, data, key, plotNum, numPlots)
-            plotNum += 1
+def MultiPlotN(varDicts, Xname, variables, colors = [], legendLabels=[]):
+    """
+    Creates one subplot for each variable.  Each subplot renders a plot
+    of that variable for each varDict passed.
+    
+    For example:
+      - one varDict and 5 variables will give 5 subplots with one line each
+      - 5 varDicts and one variable will give 1 subplot with 5 lines
+    
+    Parameters:
+      varDicts:  List of TimeSeries data dictionaries
+      Xname:  key of horizontal axes label (must be defined in all varDicts)
+      variables:  List of keys to plot for each varDict
+      colors:  color of each line to be drawn
+      legendLabels: Display a legend on the plot    
+    """
+    nSubplots = len(variables)
+
+    # Set default colors (all blue)
+    if not colors:
+        for d in varDicts:
+            colors.append('b')    
+  
+    # Need to declare these here for proper scope:
+    axes=None
+    ax=None
+  
+    for plotIndex, variable in enumerate(variables):
+        # Sharing the x-axes applies the same zoom to all subplots when
+        # user interacts with a single subplot.
+        if plotIndex == 0:
+            axes = plt.subplot(nSubplots, 1, plotIndex+1)
+            ax=axes
+        else:
+            ax =  plt.subplot(nSubplots, 1, plotIndex+1, sharex=axes)
+    
+        # Turn off x-axis to prevent pointillism problem with upper subplots.
+        #ax.xaxis.set_visible(False)
+        
+        # Alternate vertical axes
+        if plotIndex%2 == 0:
+            #ax.yaxis.tick_left()
+            ax.yaxis.set_ticks_position('left')
+            ax.yaxis.set_label_position('left')
         else:
-            ax = fig.add_subplot(gs[plotNum, 0], sharex=ax1)
-            itemPlot(ax, data, key, plotNum, numPlots)
-            plotNum += 1
-    ax1.legend([scId, "GAMERA"], loc="best")
-    ax1.set_title(plotname)
+            #ax.yaxis.tick_right()
+            ax.yaxis.set_ticks_position('right')
+            ax.yaxis.set_label_position('right')
+    
+        # Fill in subplot data
+        for (idx, data) in enumerate(varDicts):
+            if plotIndex < nSubplots-1:
+                BasicPlot(data, Xname, variable, Xlabel=False, color=colors[idx])
+                
+                # remove xticklabels from all but bottom subplot...it seems like
+                # someone was attempting something similar with ax.xaxis.set_visible(False)
+                # in the past, then commented this out; might be worth asking why -EJR 2/2014
+                plt.setp(ax.get_xticklabels(), visible=False)
+            else:
+                BasicPlot(data, Xname, variable, Xlabel=True, color=colors[idx])
+                
     plt.subplots_adjust(hspace=0)
+    #ax.xaxis.set_visible(True)
+    
+    plt.subplot(nSubplots, 1, 1)
+    if legendLabels:
+        plt.legend(legendLabels, loc='best')
+
+def swQuickPlot(UT,D,Temp,Vx,Vy,Vz,Bx,By,Bz,SYMH,interped,fname,
+                xBS=None,yBS=None,zBS=None,
+                t0fmt='%Y-%m-%d %H:%M:%S',
+                utfmt='%H:%M\n%Y-%m%d',
+                title="Solar Wind",
+                doTrim=True,doEps=False,returnAxs=False):
+    """
+    Plot solar wind n,T, dyn p, V, B and sym/h over time period specified by the user.
 
-    # Save the figure.
-    savePic(plotname)
-
-
-def trajPlot(plotname,scId,data):
-    Re = 6380.0
-    toRe = 1.0/Re
-    figsize = (15,5)
-    fig = plt.figure(figsize=figsize)
-    gs = fig.add_gridspec(1,3)
-    Ax1 = fig.add_subplot(gs[0,0])
-    Ax2 = fig.add_subplot(gs[0,1])
-    Ax3 = fig.add_subplot(gs[0,2])
-    Ax1.plot(data['Ephemeris'][:,0]*toRe,data['Ephemeris'][:,1]*toRe)
-    Ax2.plot(data['Ephemeris'][:,0]*toRe,data['Ephemeris'][:,2]*toRe)
-    Ax3.plot(data['Ephemeris'][:,1]*toRe,data['Ephemeris'][:,2]*toRe)
-    Ax1.set_title('XY SM')
-    Ax2.set_title('XZ SM')
-    Ax3.set_title('YZ SM')
-    titlestr = (scId + ' - ' + data['Epoch_bin'][0].strftime('%m/%d/%Y - %H:%M:%S') + ' to ' +  
-                data['Epoch_bin'][-1].strftime('%m/%d/%Y - %H:%M:%S'))
-    fig.suptitle(titlestr)
-    savePic(plotname)
-
-
-def get_aspect(ax):
-    """Get current aspect ratio of ax
-    """
-    from operator import sub
-    # Total figure size
-    figW, figH = ax.get_figure().get_size_inches()
-    # Axis size on figure
-    _, _, w, h = ax.get_position().bounds
-    # Ratio of display units
-    disp_ratio = (figH * h) / (figW * w)
-    # Ratio of data units
-    # Negative over negative because of the order of subtraction
-    data_ratio = sub(*ax.get_ylim()) / sub(*ax.get_xlim())
+    """
 
-    return disp_ratio #/ data_ratio
+    utall = []
+    for n in range(len(UT)):
+        utall.append(datetime.datetime.strptime(UT[n].decode('utf-8'),t0fmt))
+
+    # constants
+    gamma = 5/3.0
+    mp = 1.67e-27 #Proton mass [kg]w
+    
+    # calculating the solar wind dynamic pressure 
+    Vmag = np.sqrt(Vx**2+Vy**2+Vz**2)
+    Pram = mp*D*Vmag**2*1.0e15 # nPa
+
+    #Setup figure
+    fSz = (10,14)
+    if xBS is None:
+        Nr = 6
+    else:
+        Nr = 7
+    Nc = 1
+    clrs = ['#7570b3','#1b9e77','#d95f02','black'] # from colorbrewer2.org for colorblind safe
+
+    fig = plt.figure(figsize=fSz)
+
+    gs = gridspec.GridSpec(Nr,Nc,hspace=0.05,wspace=0.05)
+
+    ax11 = fig.add_subplot(gs[0,0])
+    ax12 = fig.add_subplot(gs[3,0])
+    ax21 = fig.add_subplot(gs[1,0])
+    ax22 = fig.add_subplot(gs[4,0])
+    ax31 = fig.add_subplot(gs[2,0])
+    if xBS is None:
+        ax32 = fig.add_subplot(gs[5,0])
+    else:
+        ax32 = fig.add_subplot(gs[6,0])
+        ax41 = fig.add_subplot(gs[5,0])
+    
+    smlabel = ['SM-X','SM-Y','SM-Z']
+    xvec = np.zeros((len(D),3))+1e9
+
+    fig.suptitle(title,y=0.92,fontsize=14)
+    Dlim=np.max(D)-np.min(D)
+    ax11.plot(utall,D,color=clrs[3])
+    for i in range(3):
+        ax11.plot(utall,xvec[:,i],linewidth=4,label=smlabel[i],color=clrs[i])
+    kv.SetAxLabs(ax11,"","n [cm^-3]",doBot=True,doLeft=True)
+    ax11.set_ylim(np.min(D)-0.05*Dlim,np.max(D)+0.05*Dlim)
+    ax11.tick_params(axis="x",direction="in")
+    ax11.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax11.get_xaxis_transform())
+    plt.setp(ax11.get_xticklabels(),visible=False)
+    ax11.legend(ncol=len(smlabel), bbox_to_anchor=(0.5,1),loc='lower center', fontsize='small')
+    
+    TScl = 1.0e-6
+    ax21.plot(utall,Temp*TScl,color=clrs[3])
+    kv.SetAxLabs(ax21,"","T [MK]",doBot=True,doLeft=False)
+    ax21.tick_params(axis="x",direction="in")
+    ax21.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax21.get_xaxis_transform())
+    plt.setp(ax21.get_xticklabels(),visible=False)
+    
+    ax31.plot(utall,Pram,color=clrs[3])
+    ax31.xaxis_date()
+    kv.SetAxLabs(ax31,"","Dynamic P [nPa]",doBot=True,doLeft=True)
+    ax31.tick_params(axis="x",direction="in")
+    ax31.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax31.get_xaxis_transform())
+    plt.setp(ax31.get_xticklabels(),visible=False)
+    
+    vScl = 1.0e-3
+    secax12 = ax12.twinx()
+    ax12.plot(utall,Vx*vScl,color=clrs[0],linewidth=0.95)
+    secax12.plot(utall,Vy*vScl,color=clrs[1],linewidth=0.95)
+    secax12.plot(utall,Vz*vScl,color=clrs[2],linewidth=0.95)
+    secax12.set_ylabel('Vy,z [km/s]')
+    kv.SetAxLabs(ax12,"","Vx [km/s]",doBot=True,doLeft=True)
+    ax12.tick_params(axis="x",direction="in")
+    ax12.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax12.get_xaxis_transform())
+    plt.setp(ax12.get_xticklabels(),visible=False)
+    
+    ax22.plot(utall,Bx,color=clrs[0],linewidth=0.95)
+    ax22.plot(utall,By,color=clrs[1],linewidth=0.95)
+    ax22.plot(utall,Bz,color=clrs[2],linewidth=0.95)
+    ax22.axhline(y=0.0, color='black', linestyle='--',alpha=0.6,linewidth=0.9)
+    kv.SetAxLabs(ax22,"","B [nT]",doBot=True,doLeft=False)
+    ax22.tick_params(axis="x",direction="in")
+    ax22.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax22.get_xaxis_transform())
+    plt.setp(ax22.get_xticklabels(),visible=False)
+    
+    if xBS is not None:
+        ax41.plot(utall,xBS,color=clrs[0],linewidth=0.95)
+        ax41.plot(utall,yBS,color=clrs[1],linewidth=0.95)
+        ax41.plot(utall,zBS,color=clrs[2],linewidth=0.95)
+        ax41.axhline(y=0.0, color='black', linestyle='--',alpha=0.6,linewidth=0.9)
+        kv.SetAxLabs(ax41,"","BowS [RE]",doBot=True,doLeft=False)
+        ax41.tick_params(axis="x",direction="in")
+        ax41.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax41.get_xaxis_transform())
+        plt.setp(ax41.get_xticklabels(),visible=False)
+
+    ax32.plot(utall,SYMH,color=clrs[3])
+    ax32.axhline(y=0.0, color='black', linestyle='--',alpha=0.6,linewidth=0.9)
+    ax32.fill_between(utall, 0, 1, where=interped, alpha=0.4, transform=ax32.get_xaxis_transform())
+    ax32.xaxis_date()
+    xfmt = dates.DateFormatter(utfmt)
+    ax32.xaxis.set_major_formatter(xfmt)
+    kv.SetAxLabs(ax32,"UT","SYM/H [nT]",doBot=True,doLeft=True)
+
+    # Give axes back to user if they want them
+    if returnAxs:
+        axDict = {}
+        axDict['D'] = ax11
+        axDict['Temp'] = ax21
+        axDict['dynP'] = ax31
+        axDict['V'] = ax12
+        axDict['B'] = ax22
+        axDict['symh'] = ax32
+        if xBS is not None:
+            axDict['BowS'] = ax41
+
+        return axDict
+    
+    # Otherwise, save the figure and leave
+    kv.savePic(fname,doEps=doEps,doTrim=doTrim)
+    plt.close('all')
```

### Comparing `kaipy-0.0.3/kaipy/kaijson.py` & `kaipy-0.0.4/kaipy/kaijson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/kaixdmf.py` & `kaipy-0.0.4/kaipy/kaixdmf.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,30 +71,46 @@
 					vLocs.append(vLoc)
 				else:
 					print("Excluding %s"%(vID))
 
 	return vIds,vLocs
 
 #Get variables in initial Step
-def getVars(fname,s0,gDims):
+def getVars(fname,gId,gDims,recursive=False):
+
+	def getVarName(gId, k, recursive):
+		if recursive:
+			# Want to keep the group name, since all vars need to be at the same level in xdmf
+			spl = gId.split('/')
+			return '/'.join(spl[1:]) + '/' + str(k)
+		else:
+			return str(k)
+
 
 	with h5py.File(fname,'r') as hf:
-		gId = "/Step#%d"%(s0)
 		stp0 = hf[gId]
 		vIds = []
 		vLocs = []
 		for k in stp0.keys():
-			vID = str(k)
-			Nv = stp0[k].shape
-			vLoc = getLoc(gDims,Nv)
-			if (vLoc != "Other"):
-				vIds.append(vID)
-				vLocs.append(vLoc)
+			vID = getVarName(gId,k,recursive)
+			
+			# If its a group, recursively call this function to get to the vars and add them to the list
+			if type(stp0[k]) == h5py._hl.group.Group:
+				vIdR, vLR = getVars(fname, gId+'/'+k, gDims, recursive=True)
+				for vi, vl in zip(vIdR, vLR):
+					vIds.append(vi)
+					vLocs.append(vl)
 			else:
-				print("Excluding %s"%(vID))
+				Nv = stp0[k].shape
+				vLoc = getLoc(gDims,Nv)
+				if (vLoc != "Other"):
+					vIds.append(vID)
+					vLocs.append(vLoc)
+				else:
+					print("Excluding %s"%(vID))
 	return vIds,vLocs
 
 def AddVectors(Grid,fname,vIds,cDims,vDims,Nd,nStp):
 	#Velocity (2D)
 	if ( (Nd == 2) and ("Vx" in vIds) and ("Vy" in vIds) ):
 		vAtt = et.SubElement(Grid,"Attribute")
 		vAtt.set("Name","VecV")
```

### Comparing `kaipy-0.0.3/kaipy/kdefs.py` & `kaipy-0.0.4/kaipy/kdefs.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,7 +48,14 @@
 #------
 #Helio
 #------
 Rsolar = 6.956E5  #[km] Solar radius
 kbltz  = 1.38e-16 #Boltzmann constant [erg/K]
 mp     = 1.67e-24 #Proton mass in grams
 Tsolar = 25.38    #Siderial solar rotation period
+JD2MJD = 2400000.5 #Conversion from JD to MJD: MJD = JD - 2400000.5
+
+#------
+#Output defaults
+#------
+barLen = 30
+barLab = 30
```

### Comparing `kaipy-0.0.3/kaipy/lfm2kaiju.py` & `kaipy-0.0.4/kaipy/lfm2kaiju.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/paraview/pvGam.py` & `kaipy-0.0.4/kaipy/paraview/pvGam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/paraview/pvutils.py` & `kaipy-0.0.4/kaipy/paraview/pvutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils/AlamData.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils/AlamParams.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils/AlamParams.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils/DistTypes.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils/DistTypes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils/fileIO.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils/fileIO.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils/genAlam.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils/plotter.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils_old/AlamData.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils_old/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils_old/alamTester.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils_old/alamTester.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpRangeEval.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpRangeEval.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils_old/dpetadp.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpetadp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils_old/genAlam.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils_old/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/lambdautils_old/plotter.py` & `kaipy-0.0.4/kaipy/rcm/lambdautils_old/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/rcminit.py` & `kaipy-0.0.4/kaipy/rcm/rcminit.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/rcmutils.py` & `kaipy-0.0.4/kaipy/rcm/rcmutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/rcmxdmf.py` & `kaipy-0.0.4/kaipy/rcm/rcmxdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/rcm/wmutils/wmData.py` & `kaipy-0.0.4/kaipy/rcm/wmutils/wmData.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import h5py as h5
 import numpy as np
 
 class wmParams:
 
     #All energies in eV
-    def __init__(self, dim = 4, nKp = 7, nMLT = 25, nL = 41, nEk = 155):
+    def __init__(self, dim = 4, nKp = 7, nMLT = 25, nL = 41, nEk = 155, dimTDS = 1, nEkTDS = 109):
         self.dim        = dim
         self.nKp        = nKp
         self.nMLT       = nMLT
-        self.nL       = nL
+        self.nL         = nL
         self.nEk        = nEk
-
+        self.dimTDS     = dimTDS
+        self.nEkTDS     = nEkTDS
     def getAttrs(self):
         return {
                 'tauDim': self.dim,
                 'nKp': self.nKp,
                 'nMLT': self.nMLT,
                 'nL': self.nL,
                 'nEk': self.nEk,
+                'tauTDSDim': self.dimTDS,
+                'nEkTDS': self.nEkTDS
         }
```

### Comparing `kaipy-0.0.3/kaipy/remix/remix.py` & `kaipy-0.0.4/kaipy/remix/remix.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/solarWind/CUSTOM.py` & `kaipy-0.0.4/kaipy/solarWind/CUSTOM.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
         self.__read(filename,t0)
 
     def __read(self, filename,t0):
         """
         Read the solar wind file & store results in self.data TimeSeries object.
         """
-        (startDate, dates, data) = self.__readData(filename,t0)
-        (dataArray, hasBeenInterpolated) = self._removeBadData(data)
+        (startDate, dates, data, datanames) = self.__readData(filename,t0)
+        (dataArray, hasBeenInterpolated) = self._removeBadData(data,datanames)
         if self.filter:
             (dataArray, hasBeenInterpolated) = self._coarseFilter(dataArray, hasBeenInterpolated)
         self._storeDataDict(dates, dataArray, hasBeenInterpolated)
         self.__appendMetaData(startDate, filename)
         self._appendDerivedQuantities()
 
     def __readData(self, filename,t0):
@@ -99,15 +99,17 @@
             else:
               ic = int(i-timeshift)
               data = [nMin,bx[ic],by[ic],bz[ic],vx[ic],vy[ic],vz[ic],n[ic],cs[ic],0.,0.,0.,dst[int(i/60.)]]
 
             dates.append( currentTime )
             rows.append( data )
 
-        return (t0, dates, rows)
+        datanames = ['Time','Bx','By','Bz','Vx','Vy','Vz','n','Sound Speed','AE','AL','AU','Dst']
+
+        return (t0, dates, rows, datanames)
 
     def _storeDataDict(self, dates, dataArray, hasBeenInterpolated):
         """
         Populate self.data TimeSeries object via the 2d dataArray read from file.
         """
         #self.__gse2gsm(dates, dataArray)
```

### Comparing `kaipy-0.0.3/kaipy/solarWind/OMNI.py` & `kaipy-0.0.4/kaipy/solarWind/OMNI.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 
         self.__read(filename)
 
     def __read(self, filename):
         """
         Read the solar wind file & store results in self.data TimeSeries object.
         """
-        (startDate, dates, data) = self.__readData(filename)
-        (dataArray, hasBeenInterpolated) = self._removeBadData(data)
+        (startDate, dates, data, datanames) = self.__readData(filename)
+        (dataArray, hasBeenInterpolated) = self._removeBadData(data,datanames)
         if self.filter:
             (dataArray, hasBeenInterpolated) = self._coarseFilter(dataArray, hasBeenInterpolated)
         self._storeDataDict(dates, dataArray, hasBeenInterpolated)
         self.__appendMetaData(startDate, filename)
         self._appendDerivedQuantities()
 
         
@@ -78,15 +78,17 @@
             nMin = self._deltaMinutes(time[i],startTime)
 
             data = [nMin,bx[i],by[i],bz[i],vx[i],vy[i],vz[i],n[i],T[i],ae[i],al[i],au[i],symh[i],xBow[i],yBow[i],zBow[i]]
 
             dates.append( time[i] )
             rows.append( data )
 
-        return (startTime, dates, rows)
+        datanames = ['Time','Bx','By','Bz','Vx','Vy','Vz','n','Temperature','AE','AL','AU','SYMH','BowShockX','BowShockY','BowShockZ']
+
+        return (startTime, dates, rows, datanames)
 
     def __appendMetaData(self, date, filename):
         """
         Add standard metadata to the data dictionary.
         """
         metadata = {'Model': 'OMNI',
                     'Source': filename,
@@ -95,15 +97,15 @@
                     }
         
         self.data.append(key='meta',
                          name='Metadata for OMNI Solar Wind file',
                          units='n/a',
                          data=metadata)
 
-    def _removeBadData(self, data, hasBeenInterpolated = None):
+    def _removeBadData(self, data, datanames=['Time','Bx','By','Bz','Vx','Vy','Vz','n','Temp','AE','AL','AU','SYMH','BowShockX','BowShockY','BowShockZ'], hasBeenInterpolated = None):
         """
         Linearly interpolate over bad data (defined by self.bad_data
         list) for each variable in dataStrs.
         
         data: 2d list.  Each row is a list containing:
           [nMinutes, Bx, By, Bz, Vx, Vy, Vz, rho, temp, ae, al, au, symh]
 
@@ -126,15 +128,15 @@
             for curIndex,row in enumerate(data):
                 if row[varIdx] in numpy.float32(self.bad_data) or numpy.isnan(row[varIdx]) or numpy.ma.is_masked(row[varIdx]):
                     # This item has bad data.
                     hasBeenInterpolated[curIndex, varIdx-1] = True
                     if (lastValidIndex == -1) & (curIndex == len(data)-1):
                         # Data does not have at least one valid element!
                         # Setting all values to 0 so that file can still be made
-                        print("No good elements, setting all values to 0 for variable ID: ", varIdx)
+                        print("No good elements, setting all values to 0 for variable: ", datanames[varIdx])
                         data[curIndex][varIdx] = 0.
                         #raise Exception("First & Last datapoint(s) in OMNI "+
                         #                  "solar wind file are invalid.  Not sure "+
                         #                  "how to interpolate across bad data.")
                     elif (curIndex == len(data)-1):
                         # Clamp last bad data to previous known good data.
                         data[curIndex][varIdx] = data[lastValidIndex][varIdx]
```

### Comparing `kaipy-0.0.3/kaipy/solarWind/SolarWind.py` & `kaipy-0.0.4/kaipy/solarWind/SolarWind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/solarWind/TimeSeries.py` & `kaipy-0.0.4/kaipy/solarWind/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/solarWind/WIND.py` & `kaipy-0.0.4/kaipy/solarWind/WIND.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/solarWind/jdutil.py` & `kaipy-0.0.4/kaipy/solarWind/jdutil.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/solarWind/ols.py` & `kaipy-0.0.4/kaipy/solarWind/ols.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.3/kaipy/supermage.py` & `kaipy-0.0.4/kaipy/supermage.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import warnings
 import math
 import datetime
 import json
 
 #### NEED TO POINT TO SUPERMAG API SCRIPT
 #### /glade/p/hao/msphere/gamshare/supermag/supermag_api.py 
-import supermag_api as smapi
+import kaipy.supermag_api as smapi
 ####
 
 # this warning is very annoying
 warnings.filterwarnings("ignore", category=DeprecationWarning) 
 
 ###############################################################################
 ###############################################################################
@@ -279,27 +279,27 @@
     thetacc = np.rad2deg(np.array(f['Thetacc'])[0].ravel())
     lat = 90 - thetacc
     phicc   = np.rad2deg(np.array(f['Phicc'])[0].ravel())
     lon = np.copy(phicc)
     lon[lon>180] -= 360
 
 
-    data = f['Step#1']
+    first_step_name = "Step#%s" % sIds[0]
+    data = f[first_step_name]
     dBt, dBp = np.array(data['dBt'])[0], np.array(data['dBp'])[0]
     BH = np.sqrt(dBt**2 + dBp**2)
     maglat = np.array(data['smlat'])[0].flatten()
 
     # Create the arrays to populate with data
     masterdBn = np.zeros((nSteps, len(dBt.flatten())))
     masterdBt, masterdBp, masterdBr = np.copy(masterdBn), np.copy(masterdBn), np.copy(masterdBn)
     mastersmlon, masterMLT = np.copy(masterdBn), np.copy(masterdBn)
 
     # make big array of all of the data
-    for i in range(nSteps):
-        #print(i)
+    for i in sIds:
         data = f['Step#%01d' % i]
         dBt = np.array(data['dBt'])[0].flatten()
         dBp = np.array(data['dBp'])[0].flatten()
         dBr = np.array(data['dBr'])[0].flatten()
         dBn = np.array(data['dBn'])[0].flatten()        # change back for STPAT!
 
         masterdBt[i] = dBt*-1 # Bx (mag coords) points South, opposite of SM Z
@@ -694,15 +694,14 @@
     plt.plot(SMI['td'], SMI['smr12'], 'b')
     plt.plot(SMI['td'], SMI['smr18'], 'b')
 
     plt.xlim([SMinterp['td'][0], SMinterp['td'][-1]])
     plt.legend()
     plt.grid(True)
     plt.ylabel("SMR 6-hour bins", fontsize = 20)
-
     plt.show()
 
 #-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#-#
 
 def Z_Tensor_1D(resistivities, thicknesses, frequencies):
     """Calculate 1D Z-Tensor for given ground resistivity profile.
     Parameters
```

### Comparing `kaipy-0.0.3/kaipy.egg-info/PKG-INFO` & `kaipy-0.0.4/kaipy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kaipy
-Version: 0.0.3
+Version: 0.0.4
 Summary: Postprocessing code for models in the kaiju software system
 Home-page: https://bitbucket.org/aplkaiju/kaiju/src/master/
 Author: Center for Geospace Storms
 Author-email: eric.winter@jhuapl.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `kaipy-0.0.3/kaipy.egg-info/SOURCES.txt` & `kaipy-0.0.4/kaipy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 README.md
 setup.py
 kaipy/__init__.py
+kaipy/cdaweb_utils.py
 kaipy/embiggenUtils.py
 kaipy/kJobs.py
 kaipy/kaiH5.py
 kaipy/kaiTools.py
 kaipy/kaiViz.py
 kaipy/kaijson.py
 kaipy/kaixdmf.py
 kaipy/kdefs.py
 kaipy/lfm2kaiju.py
+kaipy/supermag_api.py
 kaipy/supermage.py
 kaipy/transform.py
 kaipy.egg-info/PKG-INFO
 kaipy.egg-info/SOURCES.txt
 kaipy.egg-info/dependency_links.txt
 kaipy.egg-info/requires.txt
 kaipy.egg-info/top_level.txt
```

### Comparing `kaipy-0.0.3/setup.py` & `kaipy-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="kaipy",
-    version="0.0.3",
+    version="0.0.4",
     author="Center for Geospace Storms",
     author_email="eric.winter@jhuapl.edu",
     description="Postprocessing code for models in the kaiju software system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bitbucket.org/aplkaiju/kaiju/src/master/",
     packages=setuptools.find_packages(),
```

