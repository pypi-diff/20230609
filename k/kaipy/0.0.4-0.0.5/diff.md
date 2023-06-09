# Comparing `tmp/kaipy-0.0.4.tar.gz` & `tmp/kaipy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaipy-0.0.4.tar", last modified: Fri Jun  9 15:30:54 2023, max compression
+gzip compressed data, was "kaipy-0.0.5.tar", last modified: Fri Jun  9 17:53:44 2023, max compression
```

## Comparing `kaipy-0.0.4.tar` & `kaipy-0.0.5.tar`

### file list

```diff
@@ -1,106 +1,132 @@
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.933716 kaipy-0.0.4/
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:30:54.932873 kaipy-0.0.4/PKG-INFO
--rw-r--r--   0 winteel1   (503) staff       (20)      466 2023-06-09 15:27:03.000000 kaipy-0.0.4/README.md
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.846899 kaipy-0.0.4/kaipy/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    23712 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/cdaweb_utils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.856578 kaipy-0.0.4/kaipy/chimp/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2297 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/chimph5p.py
--rw-r--r--   0 winteel1   (503) staff       (20)      922 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/chimpviz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1804 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/chimp/kCyl.py
--rw-r--r--   0 winteel1   (503) staff       (20)    13945 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/embiggenUtils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.868155 kaipy-0.0.4/kaipy/gamera/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    15993 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/block_gampp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3222 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/deltabViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)    19760 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/gamGrids.py
--rw-r--r--   0 winteel1   (503) staff       (20)     8111 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/gamera/gampp.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10963 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/gamera/magsphere.py
--rw-r--r--   0 winteel1   (503) staff       (20)    14527 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/gamera/magsphereRescale.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7031 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/msphViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4119 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/rcmpp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3519 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamera/remixpp.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.873663 kaipy-0.0.4/kaipy/gamhelio/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    12994 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/helioViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)    14894 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/heliosphere.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.885682 kaipy-0.0.4/kaipy/gamhelio/lib/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2575 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/ace.py
--rw-r--r--   0 winteel1   (503) staff       (20)      758 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/cspice.py
--rw-r--r--   0 winteel1   (503) staff       (20)    12020 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/lfmhlib.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5369 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/mas.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1322 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/msgr.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4803 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/poisson.py
--rw-r--r--   0 winteel1   (503) staff       (20)      833 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/util.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3457 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/wsa.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     1064 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/lib/wsa2h5.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.887948 kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2475 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/params.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.890143 kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/
--rw-r--r--   0 winteel1   (503) staff       (20)       21 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1607 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/params.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2304 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/kJobs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5899 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kaiH5.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5485 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/kaiTools.py
--rw-r--r--   0 winteel1   (503) staff       (20)    21531 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kaiViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2405 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/kaijson.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5950 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kaixdmf.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1428 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/kdefs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2709 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/lfm2kaiju.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.893279 kaipy-0.0.4/kaipy/paraview/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/paraview/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1207 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/paraview/pvGam.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2649 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/paraview/pvutils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.897517 kaipy-0.0.4/kaipy/rcm/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/__init__.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.906294 kaipy-0.0.4/kaipy/rcm/lambdautils/
--rw-r--r--   0 winteel1   (503) staff       (20)     1707 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/AlamData.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2469 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/AlamParams.py
--rw-r--r--   0 winteel1   (503) staff       (20)     6869 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/DistTypes.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2135 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/fileIO.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1932 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/genAlam.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4036 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils/plotter.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.914867 kaipy-0.0.4/kaipy/rcm/lambdautils_old/
--rw-r--r--   0 winteel1   (503) staff       (20)     4504 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/AlamData.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5507 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/alamTester.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5780 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpRangeEval.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10132 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpetadp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     6896 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/genAlam.py
--rw-r--r--   0 winteel1   (503) staff       (20)      309 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/helperdefs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     9050 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/lambdautils_old/plotter.py
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/rcminit.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3653 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/rcmutils.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3493 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/rcmxdmf.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.918480 kaipy-0.0.4/kaipy/rcm/wmutils/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/rcm/wmutils/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4095 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/rcm/wmutils/genWM.py
--rw-r--r--   0 winteel1   (503) staff       (20)      694 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/rcm/wmutils/wmData.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.921327 kaipy-0.0.4/kaipy/remix/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/remix/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    29846 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/remix/remix.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.931586 kaipy-0.0.4/kaipy/solarWind/
--rw-r--r--   0 winteel1   (503) staff       (20)    39786 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/solarWind/CUSTOM.py
--rw-r--r--   0 winteel1   (503) staff       (20)    24794 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/solarWind/OMNI.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7272 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/SolarWind.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1950 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/TimeSeries.py
--rw-r--r--   0 winteel1   (503) staff       (20)    43184 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/WIND.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     9375 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/jdutil.py
--rw-r--r--   0 winteel1   (503) staff       (20)     8166 2023-06-09 15:27:03.000000 kaipy-0.0.4/kaipy/solarWind/ols.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10900 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/solarWind/swBCplots.py
--rw-r--r--   0 winteel1   (503) staff       (20)    25735 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/supermag_api.py
--rw-r--r--   0 winteel1   (503) staff       (20)    32873 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/supermage.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2409 2023-06-09 15:27:20.000000 kaipy-0.0.4/kaipy/transform.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 15:30:54.852445 kaipy-0.0.4/kaipy.egg-info/
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/PKG-INFO
--rw-r--r--   0 winteel1   (503) staff       (20)     2358 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/SOURCES.txt
--rw-r--r--   0 winteel1   (503) staff       (20)        1 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/dependency_links.txt
--rw-r--r--   0 winteel1   (503) staff       (20)      285 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/requires.txt
--rw-r--r--   0 winteel1   (503) staff       (20)        6 2023-06-09 15:30:54.000000 kaipy-0.0.4/kaipy.egg-info/top_level.txt
--rw-r--r--   0 winteel1   (503) staff       (20)       38 2023-06-09 15:30:54.934134 kaipy-0.0.4/setup.cfg
--rw-r--r--   0 winteel1   (503) staff       (20)     1289 2023-06-09 15:29:25.000000 kaipy-0.0.4/setup.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.955208 kaipy-0.0.5/
+-rw-r--r--   0 winteel1   (503) staff       (20)      754 2023-06-09 17:53:44.955461 kaipy-0.0.5/PKG-INFO
+-rw-r--r--   0 winteel1   (503) staff       (20)      466 2023-06-09 15:27:03.000000 kaipy-0.0.5/README.md
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.880137 kaipy-0.0.5/kaipy/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    23712 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/cdaweb_utils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.887264 kaipy-0.0.5/kaipy/chimp/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/chimp/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2297 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/chimp/chimph5p.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      922 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/chimp/chimpviz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1804 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/chimp/kCyl.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.888929 kaipy-0.0.5/kaipy/cmaps/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:14:54.000000 kaipy-0.0.5/kaipy/cmaps/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      413 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/cmaps/kaimaps.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    13945 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/embiggenUtils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.897725 kaipy-0.0.5/kaipy/gamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    15993 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/block_gampp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3222 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/deltabViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    19760 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/gamGrids.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     8111 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/gamera/gampp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10963 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/gamera/magsphere.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    14527 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/gamera/magsphereRescale.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7031 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/msphViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4119 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/rcmpp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3519 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamera/remixpp.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.899981 kaipy-0.0.5/kaipy/gamhelio/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    12994 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/helioViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    14894 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/heliosphere.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.908327 kaipy-0.0.5/kaipy/gamhelio/lib/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2575 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/ace.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      758 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/cspice.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    12020 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/lfmhlib.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5369 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/mas.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1322 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/msgr.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4803 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/poisson.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      833 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/util.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     3457 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/wsa.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     1064 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/lib/wsa2h5.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.909859 kaipy-0.0.5/kaipy/gamhelio/wsa2TDgamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/wsa2TDgamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2475 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/wsa2TDgamera/params.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.911672 kaipy-0.0.5/kaipy/gamhelio/wsa2gamera/
+-rw-r--r--   0 winteel1   (503) staff       (20)       21 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/wsa2gamera/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1607 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/gamhelio/wsa2gamera/params.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2304 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/kJobs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5899 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/kaiH5.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5485 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/kaiTools.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    21531 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/kaiViz.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2405 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/kaijson.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5950 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/kaixdmf.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1428 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/kdefs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2709 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/lfm2kaiju.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.913963 kaipy-0.0.5/kaipy/paraview/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/paraview/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1207 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/paraview/pvGam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2649 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/paraview/pvutils.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.916844 kaipy-0.0.5/kaipy/rcm/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/__init__.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.922383 kaipy-0.0.5/kaipy/rcm/lambdautils/
+-rw-r--r--   0 winteel1   (503) staff       (20)     1707 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/AlamData.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2469 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/AlamParams.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     6869 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/DistTypes.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2135 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/fileIO.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1932 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/genAlam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4036 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils/plotter.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.928650 kaipy-0.0.5/kaipy/rcm/lambdautils_old/
+-rw-r--r--   0 winteel1   (503) staff       (20)     4504 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/AlamData.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5507 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/alamTester.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     5780 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/dpRangeEval.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10132 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/dpetadp.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     6896 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/genAlam.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      309 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/helperdefs.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     9050 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/lambdautils_old/plotter.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/rcminit.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3653 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/rcmutils.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     3493 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/rcmxdmf.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.930838 kaipy-0.0.5/kaipy/rcm/wmutils/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/rcm/wmutils/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     4095 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/rcm/wmutils/genWM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)      694 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/rcm/wmutils/wmData.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.932253 kaipy-0.0.5/kaipy/remix/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/remix/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    29846 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/remix/remix.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.935405 kaipy-0.0.5/kaipy/satcomp/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:15:52.000000 kaipy-0.0.5/kaipy/satcomp/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    45814 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/satcomp/scRCM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    75390 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/satcomp/scutils.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1756 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/satcomp/test_cdas.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.936159 kaipy-0.0.5/kaipy/scripts/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:10:50.000000 kaipy-0.0.5/kaipy/scripts/__init__.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.947597 kaipy-0.0.5/kaipy/scripts/quicklook/
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:17:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/__init__.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     4115 2023-06-09 17:40:57.000000 kaipy-0.0.5/kaipy/scripts/quicklook/dbVid.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     8368 2023-06-09 17:40:57.000000 kaipy-0.0.5/kaipy/scripts/quicklook/dbpic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     3111 2023-06-09 17:40:57.000000 kaipy-0.0.5/kaipy/scripts/quicklook/dstpic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     6002 2023-06-09 17:40:57.000000 kaipy-0.0.5/kaipy/scripts/quicklook/gamsphVid.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)    11214 2023-06-09 17:40:57.000000 kaipy-0.0.5/kaipy/scripts/quicklook/heliopic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     8558 2023-06-09 17:40:57.000000 kaipy-0.0.5/kaipy/scripts/quicklook/mixpic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)    11563 2023-06-09 17:36:54.000000 kaipy-0.0.5/kaipy/scripts/quicklook/msphpic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     6747 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/rcmDataProbe.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     5304 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     5259 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/rcmSpecFlux.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)    15311 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/rcmpic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     3945 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/remixTimeSeries.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     2302 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/swpic.py
+-rwxr-xr-x   0 winteel1   (503) staff       (20)     2809 2023-06-09 17:41:09.000000 kaipy-0.0.5/kaipy/scripts/quicklook/vizTrj.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.954589 kaipy-0.0.5/kaipy/solarWind/
+-rw-r--r--   0 winteel1   (503) staff       (20)    39786 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/solarWind/CUSTOM.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    24794 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/solarWind/OMNI.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     7272 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/solarWind/SolarWind.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     1950 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/solarWind/TimeSeries.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    43184 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/solarWind/WIND.py
+-rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/solarWind/__init__.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     9375 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/solarWind/jdutil.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     8166 2023-06-09 15:27:03.000000 kaipy-0.0.5/kaipy/solarWind/ols.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    10900 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/solarWind/swBCplots.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    25735 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/supermag_api.py
+-rw-r--r--   0 winteel1   (503) staff       (20)    32873 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/supermage.py
+-rw-r--r--   0 winteel1   (503) staff       (20)     2409 2023-06-09 15:27:20.000000 kaipy-0.0.5/kaipy/transform.py
+drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 17:53:44.884258 kaipy-0.0.5/kaipy.egg-info/
+-rw-r--r--   0 winteel1   (503) staff       (20)      754 2023-06-09 17:53:44.000000 kaipy-0.0.5/kaipy.egg-info/PKG-INFO
+-rw-r--r--   0 winteel1   (503) staff       (20)     3094 2023-06-09 17:53:44.000000 kaipy-0.0.5/kaipy.egg-info/SOURCES.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)        1 2023-06-09 17:53:44.000000 kaipy-0.0.5/kaipy.egg-info/dependency_links.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)      331 2023-06-09 17:53:44.000000 kaipy-0.0.5/kaipy.egg-info/requires.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)        6 2023-06-09 17:53:44.000000 kaipy-0.0.5/kaipy.egg-info/top_level.txt
+-rw-r--r--   0 winteel1   (503) staff       (20)      944 2023-06-09 17:52:49.000000 kaipy-0.0.5/pyproject.toml
+-rw-r--r--   0 winteel1   (503) staff       (20)      153 2023-06-09 17:53:44.956509 kaipy-0.0.5/setup.cfg
```

### Comparing `kaipy-0.0.4/kaipy/cdaweb_utils.py` & `kaipy-0.0.5/kaipy/cdaweb_utils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/chimp/chimph5p.py` & `kaipy-0.0.5/kaipy/chimp/chimph5p.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/chimp/chimpviz.py` & `kaipy-0.0.5/kaipy/chimp/chimpviz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/chimp/kCyl.py` & `kaipy-0.0.5/kaipy/chimp/kCyl.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/embiggenUtils.py` & `kaipy-0.0.5/kaipy/embiggenUtils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/block_gampp.py` & `kaipy-0.0.5/kaipy/gamera/block_gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/deltabViz.py` & `kaipy-0.0.5/kaipy/gamera/deltabViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/gamGrids.py` & `kaipy-0.0.5/kaipy/gamera/gamGrids.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/gampp.py` & `kaipy-0.0.5/kaipy/gamera/gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/magsphere.py` & `kaipy-0.0.5/kaipy/gamera/magsphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/magsphereRescale.py` & `kaipy-0.0.5/kaipy/gamera/magsphereRescale.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/msphViz.py` & `kaipy-0.0.5/kaipy/gamera/msphViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/rcmpp.py` & `kaipy-0.0.5/kaipy/gamera/rcmpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamera/remixpp.py` & `kaipy-0.0.5/kaipy/gamera/remixpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/helioViz.py` & `kaipy-0.0.5/kaipy/gamhelio/helioViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/heliosphere.py` & `kaipy-0.0.5/kaipy/gamhelio/heliosphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/ace.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/ace.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/cspice.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/cspice.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/lfmhlib.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/lfmhlib.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/mas.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/mas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/msgr.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/msgr.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/poisson.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/poisson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/util.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/util.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/wsa.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/wsa.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/lib/wsa2h5.py` & `kaipy-0.0.5/kaipy/gamhelio/lib/wsa2h5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/wsa2TDgamera/params.py` & `kaipy-0.0.5/kaipy/gamhelio/wsa2TDgamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/gamhelio/wsa2gamera/params.py` & `kaipy-0.0.5/kaipy/gamhelio/wsa2gamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kJobs.py` & `kaipy-0.0.5/kaipy/kJobs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kaiH5.py` & `kaipy-0.0.5/kaipy/kaiH5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kaiTools.py` & `kaipy-0.0.5/kaipy/kaiTools.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kaiViz.py` & `kaipy-0.0.5/kaipy/kaiViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kaijson.py` & `kaipy-0.0.5/kaipy/kaijson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kaixdmf.py` & `kaipy-0.0.5/kaipy/kaixdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/kdefs.py` & `kaipy-0.0.5/kaipy/kdefs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/lfm2kaiju.py` & `kaipy-0.0.5/kaipy/lfm2kaiju.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/paraview/pvGam.py` & `kaipy-0.0.5/kaipy/paraview/pvGam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/paraview/pvutils.py` & `kaipy-0.0.5/kaipy/paraview/pvutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils/AlamData.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils/AlamParams.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils/AlamParams.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils/DistTypes.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils/DistTypes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils/fileIO.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils/fileIO.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils/genAlam.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils/plotter.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils_old/AlamData.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils_old/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils_old/alamTester.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils_old/alamTester.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpRangeEval.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils_old/dpRangeEval.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils_old/dpetadp.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils_old/dpetadp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils_old/genAlam.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils_old/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/lambdautils_old/plotter.py` & `kaipy-0.0.5/kaipy/rcm/lambdautils_old/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/rcminit.py` & `kaipy-0.0.5/kaipy/rcm/rcminit.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/rcmutils.py` & `kaipy-0.0.5/kaipy/rcm/rcmutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/rcmxdmf.py` & `kaipy-0.0.5/kaipy/rcm/rcmxdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/wmutils/genWM.py` & `kaipy-0.0.5/kaipy/rcm/wmutils/genWM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/rcm/wmutils/wmData.py` & `kaipy-0.0.5/kaipy/rcm/wmutils/wmData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/remix/remix.py` & `kaipy-0.0.5/kaipy/remix/remix.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/CUSTOM.py` & `kaipy-0.0.5/kaipy/solarWind/CUSTOM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/OMNI.py` & `kaipy-0.0.5/kaipy/solarWind/OMNI.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/SolarWind.py` & `kaipy-0.0.5/kaipy/solarWind/SolarWind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/TimeSeries.py` & `kaipy-0.0.5/kaipy/solarWind/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/WIND.py` & `kaipy-0.0.5/kaipy/solarWind/WIND.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/jdutil.py` & `kaipy-0.0.5/kaipy/solarWind/jdutil.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/ols.py` & `kaipy-0.0.5/kaipy/solarWind/ols.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/solarWind/swBCplots.py` & `kaipy-0.0.5/kaipy/solarWind/swBCplots.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/supermag_api.py` & `kaipy-0.0.5/kaipy/supermag_api.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/supermage.py` & `kaipy-0.0.5/kaipy/supermage.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.4/kaipy/transform.py` & `kaipy-0.0.5/kaipy/transform.py`

 * *Files identical despite different names*

