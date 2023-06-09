# Comparing `tmp/kaipy-0.0.6.tar.gz` & `tmp/kaipy-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaipy-0.0.6.tar", last modified: Fri Jun  9 18:01:14 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `kaipy-0.0.6.tar` & `kaipy-0.0.7.tar`

### file list

```diff
@@ -1,159 +1,156 @@
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.158508 kaipy-0.0.6/
--rw-r--r--   0 winteel1   (503) staff       (20)      754 2023-06-09 18:01:14.158697 kaipy-0.0.6/PKG-INFO
--rw-r--r--   0 winteel1   (503) staff       (20)      466 2023-06-09 15:27:03.000000 kaipy-0.0.6/README.md
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.067922 kaipy-0.0.6/kaipy/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    23712 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/cdaweb_utils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.073868 kaipy-0.0.6/kaipy/chimp/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/chimp/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2297 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/chimp/chimph5p.py
--rw-r--r--   0 winteel1   (503) staff       (20)      922 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/chimp/chimpviz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1804 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/chimp/kCyl.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.075347 kaipy-0.0.6/kaipy/cmaps/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:14:54.000000 kaipy-0.0.6/kaipy/cmaps/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)      413 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/cmaps/kaimaps.py
--rw-r--r--   0 winteel1   (503) staff       (20)    13945 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/embiggenUtils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.083090 kaipy-0.0.6/kaipy/gamera/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    15993 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/block_gampp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3222 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/deltabViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)    19760 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/gamGrids.py
--rw-r--r--   0 winteel1   (503) staff       (20)     8111 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/gamera/gampp.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10963 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/gamera/magsphere.py
--rw-r--r--   0 winteel1   (503) staff       (20)    14527 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/gamera/magsphereRescale.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7031 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/msphViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4119 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/rcmpp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3519 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamera/remixpp.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.085381 kaipy-0.0.6/kaipy/gamhelio/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    12994 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/helioViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)    14894 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/heliosphere.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.093187 kaipy-0.0.6/kaipy/gamhelio/lib/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2575 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/ace.py
--rw-r--r--   0 winteel1   (503) staff       (20)      758 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/cspice.py
--rw-r--r--   0 winteel1   (503) staff       (20)    12020 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/lfmhlib.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5369 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/mas.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1322 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/msgr.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4803 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/poisson.py
--rw-r--r--   0 winteel1   (503) staff       (20)      833 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/util.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3457 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/wsa.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     1064 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/lib/wsa2h5.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.094651 kaipy-0.0.6/kaipy/gamhelio/wsa2TDgamera/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/wsa2TDgamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2475 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/wsa2TDgamera/params.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.096227 kaipy-0.0.6/kaipy/gamhelio/wsa2gamera/
--rw-r--r--   0 winteel1   (503) staff       (20)       21 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/wsa2gamera/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1607 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/gamhelio/wsa2gamera/params.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2304 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/kJobs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5899 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/kaiH5.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5485 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/kaiTools.py
--rw-r--r--   0 winteel1   (503) staff       (20)    21531 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/kaiViz.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2405 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/kaijson.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5950 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/kaixdmf.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1428 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/kdefs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2709 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/lfm2kaiju.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.098905 kaipy-0.0.6/kaipy/paraview/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/paraview/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1207 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/paraview/pvGam.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2649 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/paraview/pvutils.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.102372 kaipy-0.0.6/kaipy/rcm/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/__init__.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.107734 kaipy-0.0.6/kaipy/rcm/lambdautils/
--rw-r--r--   0 winteel1   (503) staff       (20)     1707 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/AlamData.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2469 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/AlamParams.py
--rw-r--r--   0 winteel1   (503) staff       (20)     6869 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/DistTypes.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2135 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/fileIO.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1932 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/genAlam.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4036 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils/plotter.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.112275 kaipy-0.0.6/kaipy/rcm/lambdautils_old/
--rw-r--r--   0 winteel1   (503) staff       (20)     4504 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/AlamData.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5507 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/alamTester.py
--rw-r--r--   0 winteel1   (503) staff       (20)     5780 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/dpRangeEval.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10132 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/dpetadp.py
--rw-r--r--   0 winteel1   (503) staff       (20)     6896 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/genAlam.py
--rw-r--r--   0 winteel1   (503) staff       (20)      309 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/helperdefs.py
--rw-r--r--   0 winteel1   (503) staff       (20)     9050 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/lambdautils_old/plotter.py
--rw-r--r--   0 winteel1   (503) staff       (20)      926 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/rcminit.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3653 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/rcmutils.py
--rw-r--r--   0 winteel1   (503) staff       (20)     3493 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/rcmxdmf.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.114088 kaipy-0.0.6/kaipy/rcm/wmutils/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/rcm/wmutils/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     4095 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/rcm/wmutils/genWM.py
--rw-r--r--   0 winteel1   (503) staff       (20)      694 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/rcm/wmutils/wmData.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.115290 kaipy-0.0.6/kaipy/remix/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/remix/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    29846 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/remix/remix.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.118328 kaipy-0.0.6/kaipy/satcomp/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:15:52.000000 kaipy-0.0.6/kaipy/satcomp/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)    45814 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/satcomp/scRCM.py
--rw-r--r--   0 winteel1   (503) staff       (20)    75390 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/satcomp/scutils.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1756 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/satcomp/test_cdas.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.118860 kaipy-0.0.6/kaipy/scripts/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:10:50.000000 kaipy-0.0.6/kaipy/scripts/__init__.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.132020 kaipy-0.0.6/kaipy/scripts/postproc/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:59:39.000000 kaipy-0.0.6/kaipy/scripts/postproc/__init__.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     8005 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/block_genmpiXDMF.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     2937 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/dbCat.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     8951 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/embiggen.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     1762 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/embiggenMIX.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     2854 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/embiggenRCM.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     1766 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/embiggenVOLT.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     8833 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/genXDMF.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     5094 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/genXLine.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     4938 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/genmpiXDMF.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     1509 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/numSteps.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3108 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/printResTimes.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     9195 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/run_supermag_comparison.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3597 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/slimFL.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     4945 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/slimh5.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     4723 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/slimh5_classic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)      787 2023-06-09 17:59:00.000000 kaipy-0.0.6/kaipy/scripts/postproc/ut2mjd.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.139162 kaipy-0.0.6/kaipy/scripts/preproc/
--rwxr-xr-x   0 winteel1   (503) staff       (20)     6161 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/INIGenerator.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)    11972 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/XMLGenerator.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:58:03.000000 kaipy-0.0.6/kaipy/scripts/preproc/__init__.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)    22405 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/cda2wind.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3525 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/genLFM.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     5090 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/genRCM.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)    19183 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/wsa2TDgamera.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     5532 2023-06-09 17:57:53.000000 kaipy-0.0.6/kaipy/scripts/preproc/wsa2gamera.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.152375 kaipy-0.0.6/kaipy/scripts/quicklook/
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 17:17:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/__init__.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     4115 2023-06-09 17:40:57.000000 kaipy-0.0.6/kaipy/scripts/quicklook/dbVid.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     8368 2023-06-09 17:40:57.000000 kaipy-0.0.6/kaipy/scripts/quicklook/dbpic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3111 2023-06-09 17:40:57.000000 kaipy-0.0.6/kaipy/scripts/quicklook/dstpic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     6002 2023-06-09 17:40:57.000000 kaipy-0.0.6/kaipy/scripts/quicklook/gamsphVid.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)    11214 2023-06-09 17:40:57.000000 kaipy-0.0.6/kaipy/scripts/quicklook/heliopic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     8558 2023-06-09 17:40:57.000000 kaipy-0.0.6/kaipy/scripts/quicklook/mixpic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)    11563 2023-06-09 17:36:54.000000 kaipy-0.0.6/kaipy/scripts/quicklook/msphpic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     6747 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/rcmDataProbe.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     5304 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     5259 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/rcmSpecFlux.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)    15311 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/rcmpic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     3945 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/remixTimeSeries.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     2302 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/swpic.py
--rwxr-xr-x   0 winteel1   (503) staff       (20)     2809 2023-06-09 17:41:09.000000 kaipy-0.0.6/kaipy/scripts/quicklook/vizTrj.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.157957 kaipy-0.0.6/kaipy/solarWind/
--rw-r--r--   0 winteel1   (503) staff       (20)    39786 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/solarWind/CUSTOM.py
--rw-r--r--   0 winteel1   (503) staff       (20)    24794 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/solarWind/OMNI.py
--rw-r--r--   0 winteel1   (503) staff       (20)     7272 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/solarWind/SolarWind.py
--rw-r--r--   0 winteel1   (503) staff       (20)     1950 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/solarWind/TimeSeries.py
--rw-r--r--   0 winteel1   (503) staff       (20)    43184 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/solarWind/WIND.py
--rw-r--r--   0 winteel1   (503) staff       (20)        0 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/solarWind/__init__.py
--rw-r--r--   0 winteel1   (503) staff       (20)     9375 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/solarWind/jdutil.py
--rw-r--r--   0 winteel1   (503) staff       (20)     8166 2023-06-09 15:27:03.000000 kaipy-0.0.6/kaipy/solarWind/ols.py
--rw-r--r--   0 winteel1   (503) staff       (20)    10900 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/solarWind/swBCplots.py
--rw-r--r--   0 winteel1   (503) staff       (20)    25735 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/supermag_api.py
--rw-r--r--   0 winteel1   (503) staff       (20)    32873 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/supermage.py
--rw-r--r--   0 winteel1   (503) staff       (20)     2409 2023-06-09 15:27:20.000000 kaipy-0.0.6/kaipy/transform.py
-drwxr-xr-x   0 winteel1   (503) staff       (20)        0 2023-06-09 18:01:14.070870 kaipy-0.0.6/kaipy.egg-info/
--rw-r--r--   0 winteel1   (503) staff       (20)      754 2023-06-09 18:01:14.000000 kaipy-0.0.6/kaipy.egg-info/PKG-INFO
--rw-r--r--   0 winteel1   (503) staff       (20)     4007 2023-06-09 18:01:14.000000 kaipy-0.0.6/kaipy.egg-info/SOURCES.txt
--rw-r--r--   0 winteel1   (503) staff       (20)        1 2023-06-09 18:01:14.000000 kaipy-0.0.6/kaipy.egg-info/dependency_links.txt
--rw-r--r--   0 winteel1   (503) staff       (20)      331 2023-06-09 18:01:14.000000 kaipy-0.0.6/kaipy.egg-info/requires.txt
--rw-r--r--   0 winteel1   (503) staff       (20)        6 2023-06-09 18:01:14.000000 kaipy-0.0.6/kaipy.egg-info/top_level.txt
--rw-r--r--   0 winteel1   (503) staff       (20)      944 2023-06-09 17:52:49.000000 kaipy-0.0.6/pyproject.toml
--rw-r--r--   0 winteel1   (503) staff       (20)      153 2023-06-09 18:01:14.159298 kaipy-0.0.6/setup.cfg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/__init__.py
+-rw-r--r--   0        0        0    23712 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cdaweb_utils.py
+-rw-r--r--   0        0        0    13945 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/embiggenUtils.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kJobs.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaiH5.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaiTools.py
+-rw-r--r--   0        0        0    21531 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaiViz.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaijson.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaixdmf.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kdefs.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/lfm2kaiju.py
+-rw-r--r--   0        0        0    25735 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/supermag_api.py
+-rw-r--r--   0        0        0    32873 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/supermage.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/chimph5p.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/chimpviz.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/kCyl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/cmDDiv.txt
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/cmMLT.txt
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/kaimaps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/__init__.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/block_gampp.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/deltabViz.py
+-rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/gamGrids.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/gampp.py
+-rw-r--r--   0        0        0  1050390 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/lfmG.X.txt
+-rw-r--r--   0        0        0  1027758 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/lfmG.Y.txt
+-rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/magsphere.py
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/magsphereRescale.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/msphViz.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/rcmpp.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/remixpp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/__init__.py
+-rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/helioViz.py
+-rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/heliosphere.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startup.config
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startupOH.config
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startupTD.config
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/ace.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/cspice.py
+-rw-r--r--   0        0        0    12020 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/lfmhlib.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/mas.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/msgr.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/poisson.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/util.py
+-rwxr-xr-x   0        0        0     3457 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa.py
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa2h5.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2TDgamera/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2TDgamera/params.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2gamera/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2gamera/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/paraview/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/paraview/pvGam.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/paraview/pvutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/__init__.py
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/dktable
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/enchan.dat
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcminit.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcmlas1
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcmutils.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcmxdmf.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamData.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamParams.py
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/DistTypes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/__init__.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/fileIO.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/genAlam.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/notes.txt
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/plotter.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/AlamData.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/README
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/__init__.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/alamTester.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpRangeEval.py
+-rw-r--r--   0        0        0    10132 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpetadp.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/genAlam.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/helperdefs.py
+-rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/plotter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/__init__.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/genWM.py
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/tauTDS.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/wmData.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/remix/__init__.py
+-rw-r--r--   0        0        0    29846 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/remix/remix.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/README.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/__init__.py
+-rw-r--r--   0        0        0    45814 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/scRCM.py
+-rw-r--r--   0        0        0    12324 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/sc_cdasws_strs.json
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/sc_helio.json
+-rw-r--r--   0        0        0    75390 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/scutils.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/test_cdas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/__init__.py
+-rwxr-xr-x   0        0        0     8005 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/block_genmpiXDMF.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/calcdb.xml.template
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/dbCat.py
+-rwxr-xr-x   0        0        0     8951 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggen.py
+-rwxr-xr-x   0        0        0     1762 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenMIX.py
+-rwxr-xr-x   0        0        0     2854 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenRCM.py
+-rwxr-xr-x   0        0        0     1766 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenVOLT.py
+-rwxr-xr-x   0        0        0     8833 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/genXDMF.py
+-rwxr-xr-x   0        0        0     5094 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/genXLine.py
+-rwxr-xr-x   0        0        0     4938 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/genmpiXDMF.py
+-rwxr-xr-x   0        0        0     1509 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/numSteps.py
+-rwxr-xr-x   0        0        0     3108 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/printResTimes.py
+-rwxr-xr-x   0        0        0     9195 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/run_supermag_comparison.py
+-rwxr-xr-x   0        0        0     3597 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/slimFL.py
+-rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5.py
+-rwxr-xr-x   0        0        0     4723 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5_classic.py
+-rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/ut2mjd.py
+-rwxr-xr-x   0        0        0     6161 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/INIGenerator.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/Readme.md
+-rwxr-xr-x   0        0        0    11972 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/XMLGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/__init__.py
+-rwxr-xr-x   0        0        0    22405 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/cda2wind.py
+-rwxr-xr-x   0        0        0      775 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/correctOMPenvironment.sh
+-rwxr-xr-x   0        0        0     3525 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/genLFM.py
+-rwxr-xr-x   0        0        0     5090 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/genRCM.py
+-rwxr-xr-x   0        0        0    19183 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2TDgamera.py
+-rwxr-xr-x   0        0        0     5532 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2gamera.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/__init__.py
+-rwxr-xr-x   0        0        0     4115 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/dbVid.py
+-rwxr-xr-x   0        0        0     8368 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/dbpic.py
+-rwxr-xr-x   0        0        0     3111 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/dstpic.py
+-rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/gamsphVid.py
+-rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/heliopic.py
+-rwxr-xr-x   0        0        0     8558 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/mixpic.py
+-rwxr-xr-x   0        0        0    11563 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/msphpic.py
+-rwxr-xr-x   0        0        0     6747 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmDataProbe.py
+-rwxr-xr-x   0        0        0     5304 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py
+-rwxr-xr-x   0        0        0     5259 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmSpecFlux.py
+-rwxr-xr-x   0        0        0    15311 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmpic.py
+-rwxr-xr-x   0        0        0     3945 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/remixTimeSeries.py
+-rwxr-xr-x   0        0        0     2302 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/swpic.py
+-rwxr-xr-x   0        0        0     2809 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/vizTrj.py
+-rw-r--r--   0        0        0    39786 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/CUSTOM.py
+-rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/OMNI.py
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/SolarWind.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/TimeSeries.py
+-rw-r--r--   0        0        0    43184 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/WIND.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/__init__.py
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/jdutil.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/ols.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/swBCplots.py
+-rw-r--r--   0        0        0   331079 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/Kaiju-ExamplePlot.ipynb
+-rw-r--r--   0        0        0    20865 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/Kaiju-IdealSW.ipynb
+-rw-r--r--   0        0        0    30198 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/Kaiju-PlotSW.ipynb
+-rw-r--r--   0        0        0    35158 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/RBSP-Spectra.ipynb
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 kaipy-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kaipy-0.0.7/LICENSE
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 kaipy-0.0.7/README.md
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 kaipy-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kaipy-0.0.7/PKG-INFO
```

### Comparing `kaipy-0.0.6/kaipy/cdaweb_utils.py` & `kaipy-0.0.7/src/kaipy/cdaweb_utils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/chimp/chimph5p.py` & `kaipy-0.0.7/src/kaipy/chimp/chimph5p.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/chimp/chimpviz.py` & `kaipy-0.0.7/src/kaipy/chimp/chimpviz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/chimp/kCyl.py` & `kaipy-0.0.7/src/kaipy/chimp/kCyl.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/embiggenUtils.py` & `kaipy-0.0.7/src/kaipy/embiggenUtils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/block_gampp.py` & `kaipy-0.0.7/src/kaipy/gamera/block_gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/deltabViz.py` & `kaipy-0.0.7/src/kaipy/gamera/deltabViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/gamGrids.py` & `kaipy-0.0.7/src/kaipy/gamera/gamGrids.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/gampp.py` & `kaipy-0.0.7/src/kaipy/gamera/gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/magsphere.py` & `kaipy-0.0.7/src/kaipy/gamera/magsphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/magsphereRescale.py` & `kaipy-0.0.7/src/kaipy/gamera/magsphereRescale.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/msphViz.py` & `kaipy-0.0.7/src/kaipy/gamera/msphViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/rcmpp.py` & `kaipy-0.0.7/src/kaipy/gamera/rcmpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamera/remixpp.py` & `kaipy-0.0.7/src/kaipy/gamera/remixpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/helioViz.py` & `kaipy-0.0.7/src/kaipy/gamhelio/helioViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/heliosphere.py` & `kaipy-0.0.7/src/kaipy/gamhelio/heliosphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/ace.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/ace.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/cspice.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/cspice.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/lfmhlib.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/lfmhlib.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/mas.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/mas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/msgr.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/msgr.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/poisson.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/poisson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/util.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/util.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/wsa.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/lib/wsa2h5.py` & `kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa2h5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/wsa2TDgamera/params.py` & `kaipy-0.0.7/src/kaipy/gamhelio/wsa2TDgamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/gamhelio/wsa2gamera/params.py` & `kaipy-0.0.7/src/kaipy/gamhelio/wsa2gamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kJobs.py` & `kaipy-0.0.7/src/kaipy/kJobs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kaiH5.py` & `kaipy-0.0.7/src/kaipy/kaiH5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kaiTools.py` & `kaipy-0.0.7/src/kaipy/kaiTools.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kaiViz.py` & `kaipy-0.0.7/src/kaipy/kaiViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kaijson.py` & `kaipy-0.0.7/src/kaipy/kaijson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kaixdmf.py` & `kaipy-0.0.7/src/kaipy/kaixdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/kdefs.py` & `kaipy-0.0.7/src/kaipy/kdefs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/lfm2kaiju.py` & `kaipy-0.0.7/src/kaipy/lfm2kaiju.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/paraview/pvGam.py` & `kaipy-0.0.7/src/kaipy/paraview/pvGam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/paraview/pvutils.py` & `kaipy-0.0.7/src/kaipy/paraview/pvutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils/AlamData.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils/AlamParams.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamParams.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils/DistTypes.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils/DistTypes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils/fileIO.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils/fileIO.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils/genAlam.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils/plotter.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils_old/AlamData.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils_old/alamTester.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/alamTester.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils_old/dpRangeEval.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpRangeEval.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils_old/dpetadp.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpetadp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils_old/genAlam.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/lambdautils_old/plotter.py` & `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/rcminit.py` & `kaipy-0.0.7/src/kaipy/rcm/rcminit.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/rcmutils.py` & `kaipy-0.0.7/src/kaipy/rcm/rcmutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/rcmxdmf.py` & `kaipy-0.0.7/src/kaipy/rcm/rcmxdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/wmutils/genWM.py` & `kaipy-0.0.7/src/kaipy/rcm/wmutils/genWM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/rcm/wmutils/wmData.py` & `kaipy-0.0.7/src/kaipy/rcm/wmutils/wmData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/remix/remix.py` & `kaipy-0.0.7/src/kaipy/remix/remix.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/satcomp/scRCM.py` & `kaipy-0.0.7/src/kaipy/satcomp/scRCM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/satcomp/scutils.py` & `kaipy-0.0.7/src/kaipy/satcomp/scutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/satcomp/test_cdas.py` & `kaipy-0.0.7/src/kaipy/satcomp/test_cdas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/block_genmpiXDMF.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/block_genmpiXDMF.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/dbCat.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/dbCat.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/embiggen.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggen.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/embiggenMIX.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenMIX.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/embiggenRCM.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenRCM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/embiggenVOLT.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenVOLT.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/genXDMF.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/genXDMF.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/genXLine.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/genXLine.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/genmpiXDMF.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/genmpiXDMF.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/numSteps.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/numSteps.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/printResTimes.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/printResTimes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/run_supermag_comparison.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/run_supermag_comparison.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/slimFL.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/slimFL.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/slimh5.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/slimh5_classic.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5_classic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/postproc/ut2mjd.py` & `kaipy-0.0.7/src/kaipy/scripts/postproc/ut2mjd.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/INIGenerator.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/INIGenerator.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/XMLGenerator.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/XMLGenerator.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/cda2wind.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/cda2wind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/genLFM.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/genLFM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/genRCM.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/genRCM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/wsa2TDgamera.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2TDgamera.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/preproc/wsa2gamera.py` & `kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2gamera.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/dbVid.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/dbVid.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/dbpic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/dbpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/dstpic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/dstpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/gamsphVid.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/gamsphVid.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/heliopic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/heliopic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/mixpic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/mixpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/msphpic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/msphpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/rcmDataProbe.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmDataProbe.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/rcmSpecFlux.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmSpecFlux.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/rcmpic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/remixTimeSeries.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/remixTimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/swpic.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/swpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/scripts/quicklook/vizTrj.py` & `kaipy-0.0.7/src/kaipy/scripts/quicklook/vizTrj.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/CUSTOM.py` & `kaipy-0.0.7/src/kaipy/solarWind/CUSTOM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/OMNI.py` & `kaipy-0.0.7/src/kaipy/solarWind/OMNI.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/SolarWind.py` & `kaipy-0.0.7/src/kaipy/solarWind/SolarWind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/TimeSeries.py` & `kaipy-0.0.7/src/kaipy/solarWind/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/WIND.py` & `kaipy-0.0.7/src/kaipy/solarWind/WIND.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/jdutil.py` & `kaipy-0.0.7/src/kaipy/solarWind/jdutil.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/ols.py` & `kaipy-0.0.7/src/kaipy/solarWind/ols.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/solarWind/swBCplots.py` & `kaipy-0.0.7/src/kaipy/solarWind/swBCplots.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/supermag_api.py` & `kaipy-0.0.7/src/kaipy/supermag_api.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/supermage.py` & `kaipy-0.0.7/src/kaipy/supermage.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.6/kaipy/transform.py` & `kaipy-0.0.7/src/kaipy/transform.py`

 * *Files identical despite different names*

