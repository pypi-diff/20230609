# Comparing `tmp/kaipy-0.0.7.tar.gz` & `tmp/kaipy-0.0.8.tar.gz`

## Comparing `kaipy-0.0.7.tar` & `kaipy-0.0.8.tar`

### file list

```diff
@@ -1,156 +1,156 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/__init__.py
--rw-r--r--   0        0        0    23712 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cdaweb_utils.py
--rw-r--r--   0        0        0    13945 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/embiggenUtils.py
--rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kJobs.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaiH5.py
--rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaiTools.py
--rw-r--r--   0        0        0    21531 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaiViz.py
--rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaijson.py
--rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kaixdmf.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/kdefs.py
--rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/lfm2kaiju.py
--rw-r--r--   0        0        0    25735 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/supermag_api.py
--rw-r--r--   0        0        0    32873 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/supermage.py
--rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/transform.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/__init__.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/chimph5p.py
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/chimpviz.py
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/chimp/kCyl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/__init__.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/cmDDiv.txt
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/cmMLT.txt
--rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/cmaps/kaimaps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/__init__.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/block_gampp.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/deltabViz.py
--rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/gamGrids.py
--rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/gampp.py
--rw-r--r--   0        0        0  1050390 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/lfmG.X.txt
--rw-r--r--   0        0        0  1027758 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/lfmG.Y.txt
--rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/magsphere.py
--rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/magsphereRescale.py
--rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/msphViz.py
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/rcmpp.py
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamera/remixpp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/__init__.py
--rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/helioViz.py
--rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/heliosphere.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startup.config
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startupOH.config
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startupTD.config
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/__init__.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/ace.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/cspice.py
--rw-r--r--   0        0        0    12020 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/lfmhlib.py
--rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/mas.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/msgr.py
--rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/poisson.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/util.py
--rwxr-xr-x   0        0        0     3457 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa.py
--rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa2h5.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2TDgamera/__init__.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2TDgamera/params.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2gamera/__init__.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/gamhelio/wsa2gamera/params.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/paraview/__init__.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/paraview/pvGam.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/paraview/pvutils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/__init__.py
--rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/dktable
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/enchan.dat
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcminit.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcmlas1
--rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcmutils.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/rcmxdmf.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamData.py
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamParams.py
--rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/DistTypes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/__init__.py
--rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/fileIO.py
--rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/genAlam.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/notes.txt
--rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils/plotter.py
--rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/AlamData.py
--rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/README
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/__init__.py
--rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/alamTester.py
--rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpRangeEval.py
--rw-r--r--   0        0        0    10132 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpetadp.py
--rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/genAlam.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/helperdefs.py
--rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/plotter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/__init__.py
--rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/genWM.py
--rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/tauTDS.txt
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/rcm/wmutils/wmData.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/remix/__init__.py
--rw-r--r--   0        0        0    29846 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/remix/remix.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/README.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/__init__.py
--rw-r--r--   0        0        0    45814 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/scRCM.py
--rw-r--r--   0        0        0    12324 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/sc_cdasws_strs.json
--rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/sc_helio.json
--rw-r--r--   0        0        0    75390 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/scutils.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/satcomp/test_cdas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/__init__.py
--rwxr-xr-x   0        0        0     8005 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/block_genmpiXDMF.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/calcdb.xml.template
--rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/dbCat.py
--rwxr-xr-x   0        0        0     8951 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggen.py
--rwxr-xr-x   0        0        0     1762 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenMIX.py
--rwxr-xr-x   0        0        0     2854 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenRCM.py
--rwxr-xr-x   0        0        0     1766 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenVOLT.py
--rwxr-xr-x   0        0        0     8833 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/genXDMF.py
--rwxr-xr-x   0        0        0     5094 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/genXLine.py
--rwxr-xr-x   0        0        0     4938 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/genmpiXDMF.py
--rwxr-xr-x   0        0        0     1509 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/numSteps.py
--rwxr-xr-x   0        0        0     3108 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/printResTimes.py
--rwxr-xr-x   0        0        0     9195 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/run_supermag_comparison.py
--rwxr-xr-x   0        0        0     3597 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/slimFL.py
--rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5.py
--rwxr-xr-x   0        0        0     4723 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5_classic.py
--rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/postproc/ut2mjd.py
--rwxr-xr-x   0        0        0     6161 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/INIGenerator.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/Readme.md
--rwxr-xr-x   0        0        0    11972 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/XMLGenerator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/__init__.py
--rwxr-xr-x   0        0        0    22405 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/cda2wind.py
--rwxr-xr-x   0        0        0      775 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/correctOMPenvironment.sh
--rwxr-xr-x   0        0        0     3525 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/genLFM.py
--rwxr-xr-x   0        0        0     5090 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/genRCM.py
--rwxr-xr-x   0        0        0    19183 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2TDgamera.py
--rwxr-xr-x   0        0        0     5532 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2gamera.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/__init__.py
--rwxr-xr-x   0        0        0     4115 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/dbVid.py
--rwxr-xr-x   0        0        0     8368 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/dbpic.py
--rwxr-xr-x   0        0        0     3111 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/dstpic.py
--rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/gamsphVid.py
--rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/heliopic.py
--rwxr-xr-x   0        0        0     8558 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/mixpic.py
--rwxr-xr-x   0        0        0    11563 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/msphpic.py
--rwxr-xr-x   0        0        0     6747 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmDataProbe.py
--rwxr-xr-x   0        0        0     5304 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py
--rwxr-xr-x   0        0        0     5259 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmSpecFlux.py
--rwxr-xr-x   0        0        0    15311 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmpic.py
--rwxr-xr-x   0        0        0     3945 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/remixTimeSeries.py
--rwxr-xr-x   0        0        0     2302 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/swpic.py
--rwxr-xr-x   0        0        0     2809 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/scripts/quicklook/vizTrj.py
--rw-r--r--   0        0        0    39786 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/CUSTOM.py
--rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/OMNI.py
--rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/SolarWind.py
--rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/TimeSeries.py
--rw-r--r--   0        0        0    43184 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/WIND.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/__init__.py
--rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/jdutil.py
--rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/ols.py
--rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/solarWind/swBCplots.py
--rw-r--r--   0        0        0   331079 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/Kaiju-ExamplePlot.ipynb
--rw-r--r--   0        0        0    20865 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/Kaiju-IdealSW.ipynb
--rw-r--r--   0        0        0    30198 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/Kaiju-PlotSW.ipynb
--rw-r--r--   0        0        0    35158 2020-02-02 00:00:00.000000 kaipy-0.0.7/src/kaipy/tutorial/RBSP-Spectra.ipynb
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 kaipy-0.0.7/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kaipy-0.0.7/LICENSE
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 kaipy-0.0.7/README.md
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 kaipy-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 kaipy-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/__init__.py
+-rw-r--r--   0        0        0    23712 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/cdaweb_utils.py
+-rw-r--r--   0        0        0    13945 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/embiggenUtils.py
+-rw-r--r--   0        0        0     2304 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kJobs.py
+-rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kaiH5.py
+-rw-r--r--   0        0        0     5485 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kaiTools.py
+-rw-r--r--   0        0        0    21531 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kaiViz.py
+-rw-r--r--   0        0        0     2405 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kaijson.py
+-rw-r--r--   0        0        0     5950 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kaixdmf.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/kdefs.py
+-rw-r--r--   0        0        0     2709 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/lfm2kaiju.py
+-rw-r--r--   0        0        0    25735 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/supermag_api.py
+-rw-r--r--   0        0        0    32873 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/supermage.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/transform.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/chimp/__init__.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/chimp/chimph5p.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/chimp/chimpviz.py
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/chimp/kCyl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/cmaps/__init__.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/cmaps/cmDDiv.txt
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/cmaps/cmMLT.txt
+-rw-r--r--   0        0        0      413 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/cmaps/kaimaps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/__init__.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/block_gampp.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/deltabViz.py
+-rw-r--r--   0        0        0    19760 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/gamGrids.py
+-rw-r--r--   0        0        0     8111 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/gampp.py
+-rw-r--r--   0        0        0  1050390 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/lfmG.X.txt
+-rw-r--r--   0        0        0  1027758 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/lfmG.Y.txt
+-rw-r--r--   0        0        0    10963 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/magsphere.py
+-rw-r--r--   0        0        0    14527 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/magsphereRescale.py
+-rw-r--r--   0        0        0     7031 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/msphViz.py
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/rcmpp.py
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamera/remixpp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/__init__.py
+-rw-r--r--   0        0        0    12994 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/helioViz.py
+-rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/heliosphere.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/ConfigScripts/startup.config
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/ConfigScripts/startupOH.config
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/ConfigScripts/startupTD.config
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/ace.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/cspice.py
+-rw-r--r--   0        0        0    12020 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/lfmhlib.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/mas.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/msgr.py
+-rw-r--r--   0        0        0     4803 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/poisson.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/util.py
+-rwxr-xr-x   0        0        0     3457 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/wsa.py
+-rwxr-xr-x   0        0        0     1064 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/lib/wsa2h5.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/wsa2TDgamera/__init__.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/wsa2TDgamera/params.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/wsa2gamera/__init__.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/gamhelio/wsa2gamera/params.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/paraview/__init__.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/paraview/pvGam.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/paraview/pvutils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/__init__.py
+-rw-r--r--   0        0        0     9477 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/dktable
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/enchan.dat
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/rcminit.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/rcmlas1
+-rw-r--r--   0        0        0     3653 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/rcmutils.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/rcmxdmf.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/AlamData.py
+-rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/AlamParams.py
+-rw-r--r--   0        0        0     6869 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/DistTypes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/__init__.py
+-rw-r--r--   0        0        0     2135 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/fileIO.py
+-rw-r--r--   0        0        0     1932 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/genAlam.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/notes.txt
+-rw-r--r--   0        0        0     4036 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils/plotter.py
+-rw-r--r--   0        0        0     4504 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/AlamData.py
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/README
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/__init__.py
+-rw-r--r--   0        0        0     5507 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/alamTester.py
+-rw-r--r--   0        0        0     5780 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/dpRangeEval.py
+-rw-r--r--   0        0        0    10132 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/dpetadp.py
+-rw-r--r--   0        0        0     6896 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/genAlam.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/helperdefs.py
+-rw-r--r--   0        0        0     9050 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/plotter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/wmutils/__init__.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/wmutils/genWM.py
+-rw-r--r--   0        0        0     8175 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/wmutils/tauTDS.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/rcm/wmutils/wmData.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/remix/__init__.py
+-rw-r--r--   0        0        0    29846 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/remix/remix.py
+-rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/README.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/__init__.py
+-rw-r--r--   0        0        0    45814 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/scRCM.py
+-rw-r--r--   0        0        0    12324 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/sc_cdasws_strs.json
+-rw-r--r--   0        0        0     3453 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/sc_helio.json
+-rw-r--r--   0        0        0    75390 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/scutils.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/satcomp/test_cdas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/__init__.py
+-rwxr-xr-x   0        0        0     8005 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/block_genmpiXDMF.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/calcdb.xml.template
+-rwxr-xr-x   0        0        0     2937 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/dbCat.py
+-rwxr-xr-x   0        0        0     8951 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/embiggen.py
+-rwxr-xr-x   0        0        0     1762 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/embiggenMIX.py
+-rwxr-xr-x   0        0        0     2854 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/embiggenRCM.py
+-rwxr-xr-x   0        0        0     1766 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/embiggenVOLT.py
+-rwxr-xr-x   0        0        0     8833 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/genXDMF.py
+-rwxr-xr-x   0        0        0     5094 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/genXLine.py
+-rwxr-xr-x   0        0        0     4938 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/genmpiXDMF.py
+-rwxr-xr-x   0        0        0     1509 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/numSteps.py
+-rwxr-xr-x   0        0        0     3108 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/printResTimes.py
+-rwxr-xr-x   0        0        0     9195 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/run_supermag_comparison.py
+-rwxr-xr-x   0        0        0     3597 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/slimFL.py
+-rwxr-xr-x   0        0        0     4945 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/slimh5.py
+-rwxr-xr-x   0        0        0     4723 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/slimh5_classic.py
+-rwxr-xr-x   0        0        0      787 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/postproc/ut2mjd.py
+-rwxr-xr-x   0        0        0     6161 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/INIGenerator.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/Readme.md
+-rwxr-xr-x   0        0        0    11972 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/XMLGenerator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/__init__.py
+-rwxr-xr-x   0        0        0    22405 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/cda2wind.py
+-rwxr-xr-x   0        0        0      775 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/correctOMPenvironment.sh
+-rwxr-xr-x   0        0        0     3525 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/genLFM.py
+-rwxr-xr-x   0        0        0     5090 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/genRCM.py
+-rwxr-xr-x   0        0        0    19183 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/wsa2TDgamera.py
+-rwxr-xr-x   0        0        0     5532 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/preproc/wsa2gamera.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/__init__.py
+-rwxr-xr-x   0        0        0     4115 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/dbVid.py
+-rwxr-xr-x   0        0        0     8368 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/dbpic.py
+-rwxr-xr-x   0        0        0     3111 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/dstpic.py
+-rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/gamsphVid.py
+-rwxr-xr-x   0        0        0    11214 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/heliopic.py
+-rwxr-xr-x   0        0        0     8558 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/mixpic.py
+-rwxr-xr-x   0        0        0    11563 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/msphpic.py
+-rwxr-xr-x   0        0        0     6747 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmDataProbe.py
+-rwxr-xr-x   0        0        0     5304 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py
+-rwxr-xr-x   0        0        0     5259 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmSpecFlux.py
+-rwxr-xr-x   0        0        0    15311 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmpic.py
+-rwxr-xr-x   0        0        0     3945 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/remixTimeSeries.py
+-rwxr-xr-x   0        0        0     2302 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/swpic.py
+-rwxr-xr-x   0        0        0     2809 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/scripts/quicklook/vizTrj.py
+-rw-r--r--   0        0        0    39786 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/CUSTOM.py
+-rw-r--r--   0        0        0    24794 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/OMNI.py
+-rw-r--r--   0        0        0     7272 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/SolarWind.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/TimeSeries.py
+-rw-r--r--   0        0        0    43184 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/WIND.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/__init__.py
+-rw-r--r--   0        0        0     9375 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/jdutil.py
+-rw-r--r--   0        0        0     8166 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/ols.py
+-rw-r--r--   0        0        0    10900 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/solarWind/swBCplots.py
+-rw-r--r--   0        0        0   331079 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/tutorial/Kaiju-ExamplePlot.ipynb
+-rw-r--r--   0        0        0    20865 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/tutorial/Kaiju-IdealSW.ipynb
+-rw-r--r--   0        0        0    30198 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/tutorial/Kaiju-PlotSW.ipynb
+-rw-r--r--   0        0        0    35158 2020-02-02 00:00:00.000000 kaipy-0.0.8/src/kaipy/tutorial/RBSP-Spectra.ipynb
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 kaipy-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 kaipy-0.0.8/LICENSE
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 kaipy-0.0.8/README.md
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 kaipy-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 kaipy-0.0.8/PKG-INFO
```

### Comparing `kaipy-0.0.7/src/kaipy/cdaweb_utils.py` & `kaipy-0.0.8/src/kaipy/cdaweb_utils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/embiggenUtils.py` & `kaipy-0.0.8/src/kaipy/embiggenUtils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kJobs.py` & `kaipy-0.0.8/src/kaipy/kJobs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kaiH5.py` & `kaipy-0.0.8/src/kaipy/kaiH5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kaiTools.py` & `kaipy-0.0.8/src/kaipy/kaiTools.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kaiViz.py` & `kaipy-0.0.8/src/kaipy/kaiViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kaijson.py` & `kaipy-0.0.8/src/kaipy/kaijson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kaixdmf.py` & `kaipy-0.0.8/src/kaipy/kaixdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/kdefs.py` & `kaipy-0.0.8/src/kaipy/kdefs.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/lfm2kaiju.py` & `kaipy-0.0.8/src/kaipy/lfm2kaiju.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/supermag_api.py` & `kaipy-0.0.8/src/kaipy/supermag_api.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/supermage.py` & `kaipy-0.0.8/src/kaipy/supermage.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/transform.py` & `kaipy-0.0.8/src/kaipy/transform.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/chimp/chimph5p.py` & `kaipy-0.0.8/src/kaipy/chimp/chimph5p.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/chimp/chimpviz.py` & `kaipy-0.0.8/src/kaipy/chimp/chimpviz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/chimp/kCyl.py` & `kaipy-0.0.8/src/kaipy/chimp/kCyl.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/cmaps/cmDDiv.txt` & `kaipy-0.0.8/src/kaipy/cmaps/cmDDiv.txt`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/cmaps/cmMLT.txt` & `kaipy-0.0.8/src/kaipy/cmaps/cmMLT.txt`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/block_gampp.py` & `kaipy-0.0.8/src/kaipy/gamera/block_gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/deltabViz.py` & `kaipy-0.0.8/src/kaipy/gamera/deltabViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/gamGrids.py` & `kaipy-0.0.8/src/kaipy/gamera/gamGrids.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/gampp.py` & `kaipy-0.0.8/src/kaipy/gamera/gampp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/lfmG.X.txt` & `kaipy-0.0.8/src/kaipy/gamera/lfmG.X.txt`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/lfmG.Y.txt` & `kaipy-0.0.8/src/kaipy/gamera/lfmG.Y.txt`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/magsphere.py` & `kaipy-0.0.8/src/kaipy/gamera/magsphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/magsphereRescale.py` & `kaipy-0.0.8/src/kaipy/gamera/magsphereRescale.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/msphViz.py` & `kaipy-0.0.8/src/kaipy/gamera/msphViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/rcmpp.py` & `kaipy-0.0.8/src/kaipy/gamera/rcmpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamera/remixpp.py` & `kaipy-0.0.8/src/kaipy/gamera/remixpp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/helioViz.py` & `kaipy-0.0.8/src/kaipy/gamhelio/helioViz.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/heliosphere.py` & `kaipy-0.0.8/src/kaipy/gamhelio/heliosphere.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startup.config` & `kaipy-0.0.8/src/kaipy/gamhelio/ConfigScripts/startup.config`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startupOH.config` & `kaipy-0.0.8/src/kaipy/gamhelio/ConfigScripts/startupOH.config`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/ConfigScripts/startupTD.config` & `kaipy-0.0.8/src/kaipy/gamhelio/ConfigScripts/startupTD.config`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/ace.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/ace.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/cspice.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/cspice.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/lfmhlib.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/lfmhlib.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/mas.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/mas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/msgr.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/msgr.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/poisson.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/poisson.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/util.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/util.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/wsa.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/lib/wsa2h5.py` & `kaipy-0.0.8/src/kaipy/gamhelio/lib/wsa2h5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/wsa2TDgamera/params.py` & `kaipy-0.0.8/src/kaipy/gamhelio/wsa2TDgamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/gamhelio/wsa2gamera/params.py` & `kaipy-0.0.8/src/kaipy/gamhelio/wsa2gamera/params.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/paraview/pvGam.py` & `kaipy-0.0.8/src/kaipy/paraview/pvGam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/paraview/pvutils.py` & `kaipy-0.0.8/src/kaipy/paraview/pvutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/dktable` & `kaipy-0.0.8/src/kaipy/rcm/dktable`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/enchan.dat` & `kaipy-0.0.8/src/kaipy/rcm/enchan.dat`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/rcminit.py` & `kaipy-0.0.8/src/kaipy/rcm/rcminit.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/rcmlas1` & `kaipy-0.0.8/src/kaipy/rcm/rcmlas1`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/rcmutils.py` & `kaipy-0.0.8/src/kaipy/rcm/rcmutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/rcmxdmf.py` & `kaipy-0.0.8/src/kaipy/rcm/rcmxdmf.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamData.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils/AlamParams.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils/AlamParams.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils/DistTypes.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils/DistTypes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils/fileIO.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils/fileIO.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils/genAlam.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils/plotter.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/AlamData.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/AlamData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/README` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/README`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/alamTester.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/alamTester.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpRangeEval.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/dpRangeEval.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/dpetadp.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/dpetadp.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/genAlam.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/genAlam.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/lambdautils_old/plotter.py` & `kaipy-0.0.8/src/kaipy/rcm/lambdautils_old/plotter.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/wmutils/genWM.py` & `kaipy-0.0.8/src/kaipy/rcm/wmutils/genWM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/wmutils/tauTDS.txt` & `kaipy-0.0.8/src/kaipy/rcm/wmutils/tauTDS.txt`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/rcm/wmutils/wmData.py` & `kaipy-0.0.8/src/kaipy/rcm/wmutils/wmData.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/remix/remix.py` & `kaipy-0.0.8/src/kaipy/remix/remix.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/satcomp/README.txt` & `kaipy-0.0.8/src/kaipy/satcomp/README.txt`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/satcomp/scRCM.py` & `kaipy-0.0.8/src/kaipy/satcomp/scRCM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/satcomp/sc_cdasws_strs.json` & `kaipy-0.0.8/src/kaipy/satcomp/sc_cdasws_strs.json`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/satcomp/sc_helio.json` & `kaipy-0.0.8/src/kaipy/satcomp/sc_helio.json`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/satcomp/scutils.py` & `kaipy-0.0.8/src/kaipy/satcomp/scutils.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/satcomp/test_cdas.py` & `kaipy-0.0.8/src/kaipy/satcomp/test_cdas.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/block_genmpiXDMF.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/block_genmpiXDMF.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/dbCat.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/dbCat.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggen.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/embiggen.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenMIX.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/embiggenMIX.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenRCM.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/embiggenRCM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/embiggenVOLT.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/embiggenVOLT.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/genXDMF.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/genXDMF.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/genXLine.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/genXLine.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/genmpiXDMF.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/genmpiXDMF.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/numSteps.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/numSteps.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/printResTimes.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/printResTimes.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/run_supermag_comparison.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/run_supermag_comparison.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/slimFL.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/slimFL.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/slimh5.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/slimh5_classic.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/slimh5_classic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/postproc/ut2mjd.py` & `kaipy-0.0.8/src/kaipy/scripts/postproc/ut2mjd.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/INIGenerator.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/INIGenerator.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/XMLGenerator.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/XMLGenerator.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/cda2wind.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/cda2wind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/correctOMPenvironment.sh` & `kaipy-0.0.8/src/kaipy/scripts/preproc/correctOMPenvironment.sh`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/genLFM.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/genLFM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/genRCM.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/genRCM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2TDgamera.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/wsa2TDgamera.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/preproc/wsa2gamera.py` & `kaipy-0.0.8/src/kaipy/scripts/preproc/wsa2gamera.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/dbVid.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/dbVid.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/dbpic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/dbpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/dstpic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/dstpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/gamsphVid.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/gamsphVid.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/heliopic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/heliopic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/mixpic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/mixpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/msphpic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/msphpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmDataProbe.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmDataProbe.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmPrecipSpecFlux.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmSpecFlux.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmSpecFlux.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/rcmpic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/rcmpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/remixTimeSeries.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/remixTimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/swpic.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/swpic.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/scripts/quicklook/vizTrj.py` & `kaipy-0.0.8/src/kaipy/scripts/quicklook/vizTrj.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/CUSTOM.py` & `kaipy-0.0.8/src/kaipy/solarWind/CUSTOM.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/OMNI.py` & `kaipy-0.0.8/src/kaipy/solarWind/OMNI.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/SolarWind.py` & `kaipy-0.0.8/src/kaipy/solarWind/SolarWind.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/TimeSeries.py` & `kaipy-0.0.8/src/kaipy/solarWind/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/WIND.py` & `kaipy-0.0.8/src/kaipy/solarWind/WIND.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/jdutil.py` & `kaipy-0.0.8/src/kaipy/solarWind/jdutil.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/ols.py` & `kaipy-0.0.8/src/kaipy/solarWind/ols.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/solarWind/swBCplots.py` & `kaipy-0.0.8/src/kaipy/solarWind/swBCplots.py`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/tutorial/Kaiju-ExamplePlot.ipynb` & `kaipy-0.0.8/src/kaipy/tutorial/Kaiju-ExamplePlot.ipynb`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/tutorial/Kaiju-IdealSW.ipynb` & `kaipy-0.0.8/src/kaipy/tutorial/Kaiju-IdealSW.ipynb`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/tutorial/Kaiju-PlotSW.ipynb` & `kaipy-0.0.8/src/kaipy/tutorial/Kaiju-PlotSW.ipynb`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/src/kaipy/tutorial/RBSP-Spectra.ipynb` & `kaipy-0.0.8/src/kaipy/tutorial/RBSP-Spectra.ipynb`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/.gitignore` & `kaipy-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `kaipy-0.0.7/LICENSE` & `kaipy-0.0.8/LICENSE`

 * *Files identical despite different names*

