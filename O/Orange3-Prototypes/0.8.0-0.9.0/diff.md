# Comparing `tmp/Orange3-Prototypes-0.8.0.tar.gz` & `tmp/Orange3-Prototypes-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Orange3-Prototypes-0.8.0.tar", last modified: Sun Jan  7 19:27:38 2018, max compression
+gzip compressed data, was "dist/Orange3-Prototypes-0.9.0.tar", last modified: Thu Jan 25 18:52:08 2018, max compression
```

## Comparing `Orange3-Prototypes-0.8.0.tar` & `Orange3-Prototypes-0.9.0.tar`

### file list

```diff
@@ -1,99 +1,144 @@
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/
--rw-r--r--   0 jk        (1000) jk        (1000)     1106 2017-03-14 13:00:42.000000 Orange3-Prototypes-0.8.0/README.md
--rw-r--r--   0 jk        (1000) jk        (1000)      372 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)      182 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/MANIFEST.in
--rw-r--r--   0 jk        (1000) jk        (1000)     1892 2018-01-07 19:26:51.000000 Orange3-Prototypes-0.8.0/setup.py
--rw-r--r--   0 jk        (1000) jk        (1000)       38 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/setup.cfg
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/
--rw-r--r--   0 jk        (1000) jk        (1000)     1934 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/pandas_util.py
--rw-r--r--   0 jk        (1000) jk        (1000)     8215 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/significance.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/
--rw-r--r--   0 jk        (1000) jk        (1000)     5577 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owdbscan.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/
--rw-r--r--   0 jk        (1000) jk        (1000)     2165 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ToShoppingList.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     2504 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Category-Prototypes.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1544 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ImageLandscape.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1497 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Contingency.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     4316 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/IPythonConnector.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1126 2017-11-03 15:08:19.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/FeatureStatistics.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1435 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Correlations.svg
--rw-r--r--   0 jk        (1000) jk        (1000)    35223 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/1ka.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     3035 2017-03-14 12:54:37.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/CreateClass.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1659 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ModelMap.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     8381 2016-02-26 16:23:04.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/LinePlot.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1032 2017-09-18 10:59:07.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Stacking.svg
--rw-r--r--   0 jk        (1000) jk        (1000)    44313 2017-01-19 17:36:03.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Clock.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     3334 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/GoogleSheets.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1018 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Lookalike.svg
--rw-r--r--   0 jk        (1000) jk        (1000)    15459 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/WebcamCapture.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     3121 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Unique.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1181 2015-09-07 10:10:37.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Hub.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     5417 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ParallelCoordinates.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1349 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/LinearProjection.svg
--rw-r--r--   0 jk        (1000) jk        (1000)    30820 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/SignificantGroups.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1032 2017-09-18 10:59:07.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/NeighbourJoining.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1913 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/DBSCAN.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     1654 2016-06-27 12:03:31.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Neighbours.svg
--rw-r--r--   0 jk        (1000) jk        (1000)      808 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Face.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     2270 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/DataSets.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     8813 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/PolynomialRegression.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     3159 2017-03-14 12:54:37.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Scattermap.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     2128 2016-06-27 12:03:31.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Silhouette.svg
--rw-r--r--   0 jk        (1000) jk        (1000)     8651 2017-01-19 18:59:40.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owclock.py
--rw-r--r--   0 jk        (1000) jk        (1000)     6347 2017-11-09 16:06:31.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owwebcamcapture.py
--rw-r--r--   0 jk        (1000) jk        (1000)    45657 2017-11-27 22:32:19.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owscattermap.py
--rw-r--r--   0 jk        (1000) jk        (1000)     1973 2016-02-26 16:23:03.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owhub.py
--rw-r--r--   0 jk        (1000) jk        (1000)    61575 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owlookalike.py
--rw-r--r--   0 jk        (1000) jk        (1000)     4501 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owface.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/
--rw-r--r--   0 jk        (1000) jk        (1000)      403 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/style.css
--rw-r--r--   0 jk        (1000) jk        (1000)      440 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/html.html
--rw-r--r--   0 jk        (1000) jk        (1000)     1536 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/script.js
--rw-r--r--   0 jk        (1000) jk        (1000)  2246607 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.min.js
--rw-r--r--   0 jk        (1000) jk        (1000)  2497777 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.upstream.js
--rw-r--r--   0 jk        (1000) jk        (1000)    13445 2018-01-07 18:48:43.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/histogram.py
--rw-r--r--   0 jk        (1000) jk        (1000)     7445 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/plotly_widget.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/
--rw-r--r--   0 jk        (1000) jk        (1000)      869 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/style.css
--rw-r--r--   0 jk        (1000) jk        (1000)     2200 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/script.js
--rw-r--r--   0 jk        (1000) jk        (1000)     1900 2017-11-03 15:08:19.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owstack.py
--rw-r--r--   0 jk        (1000) jk        (1000)     5641 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owreshape.py
--rw-r--r--   0 jk        (1000) jk        (1000)    12999 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/ow1ka.py
--rw-r--r--   0 jk        (1000) jk        (1000)      333 2016-02-26 16:23:03.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/__init__.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/data/
--rw-r--r--   0 jk        (1000) jk        (1000)   930127 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/data/haarcascade_frontalface_default.xml
--rw-r--r--   0 jk        (1000) jk        (1000)     4243 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owunique.py
--rw-r--r--   0 jk        (1000) jk        (1000)     5542 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owgooglesheets.py
--rw-r--r--   0 jk        (1000) jk        (1000)     4837 2017-09-18 10:59:07.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owneighbours.py
--rw-r--r--   0 jk        (1000) jk        (1000)    14634 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owparallelcoordinates.py
--rw-r--r--   0 jk        (1000) jk        (1000)     3474 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owcontingency.py
--rw-r--r--   0 jk        (1000) jk        (1000)     9145 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owlineplot.py
--rw-r--r--   0 jk        (1000) jk        (1000)    12245 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owsignificantgroups.py
--rw-r--r--   0 jk        (1000) jk        (1000)     4691 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owipythonconnector.py
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/
--rw-r--r--   0 jk        (1000) jk        (1000)     4639 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owneighbours.py
--rw-r--r--   0 jk        (1000) jk        (1000)     9928 2018-01-07 18:48:43.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owfeaturestatistics.py
--rw-r--r--   0 jk        (1000) jk        (1000)     1848 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owlookalike.py
--rw-r--r--   0 jk        (1000) jk        (1000)     4453 2017-03-14 13:00:23.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owcorrelations.py
--rw-r--r--   0 jk        (1000) jk        (1000)     2371 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owlda.py
--rw-r--r--   0 jk        (1000) jk        (1000)     6860 2017-03-14 13:00:23.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owcorrelations.py
--rw-r--r--   0 jk        (1000) jk        (1000)    24158 2018-01-07 18:48:43.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owfeaturestatistics.py
--rw-r--r--   0 jk        (1000) jk        (1000)     1622 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/ipython_connector.py
--rw-r--r--   0 jk        (1000) jk        (1000)        0 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/__init__.py
--rw-r--r--   0 jk        (1000) jk        (1000)     4167 2017-11-03 15:08:19.000000 Orange3-Prototypes-0.8.0/orangecontrib/prototypes/stack.py
--rw-r--r--   0 jk        (1000) jk        (1000)      164 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.8.0/orangecontrib/__init__.py
--rw-r--r--   0 jk        (1000) jk        (1000)      210 2016-06-27 12:03:31.000000 Orange3-Prototypes-0.8.0/.gitignore
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/
--rw-r--r--   0 jk        (1000) jk        (1000)      372 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/PKG-INFO
--rw-r--r--   0 jk        (1000) jk        (1000)      119 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/entry_points.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/dependency_links.txt
--rw-r--r--   0 jk        (1000) jk        (1000)        1 2015-08-28 10:51:37.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/not-zip-safe
--rw-r--r--   0 jk        (1000) jk        (1000)     4191 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/SOURCES.txt
--rw-r--r--   0 jk        (1000) jk        (1000)       14 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/namespace_packages.txt
--rw-r--r--   0 jk        (1000) jk        (1000)      151 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/requires.txt
--rw-r--r--   0 jk        (1000) jk        (1000)       14 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/Orange3_Prototypes.egg-info/top_level.txt
-drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-07 19:27:38.000000 Orange3-Prototypes-0.8.0/.github/
--rw-r--r--   0 jk        (1000) jk        (1000)      382 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.8.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 jk        (1000) jk        (1000)      217 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:08.000000 Orange3-Prototypes-0.9.0/
+-rw-r--r--   0 jk        (1000) jk        (1000)     1106 2017-03-14 13:00:42.000000 Orange3-Prototypes-0.9.0/README.md
+-rw-r--r--   0 jk        (1000) jk        (1000)      372 2018-01-25 18:52:08.000000 Orange3-Prototypes-0.9.0/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)      182 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/MANIFEST.in
+-rw-r--r--   0 jk        (1000) jk        (1000)     2024 2018-01-25 18:52:01.000000 Orange3-Prototypes-0.9.0/setup.py
+-rw-r--r--   0 jk        (1000) jk        (1000)       38 2018-01-25 18:52:08.000000 Orange3-Prototypes-0.9.0/setup.cfg
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/
+-rw-r--r--   0 jk        (1000) jk        (1000)     1934 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/pandas_util.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     8215 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/significance.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/
+-rw-r--r--   0 jk        (1000) jk        (1000)     5577 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owdbscan.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/
+-rw-r--r--   0 jk        (1000) jk        (1000)     2165 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ToShoppingList.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     2504 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Category-Prototypes.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1544 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ImageLandscape.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1497 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Contingency.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     4316 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/IPythonConnector.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1126 2017-11-03 15:08:19.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/FeatureStatistics.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1435 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Correlations.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)    35223 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/1ka.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     3035 2017-03-14 12:54:37.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/CreateClass.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1654 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Neighbors.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1659 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ModelMap.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     8381 2016-02-26 16:23:04.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/LinePlot.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1032 2017-09-18 10:59:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Stacking.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)    44313 2017-01-19 17:36:03.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Clock.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     3334 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/GoogleSheets.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1018 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Lookalike.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)    15459 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/WebcamCapture.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     3121 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Unique.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1181 2015-09-07 10:10:37.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Hub.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     5417 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ParallelCoordinates.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1349 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/LinearProjection.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)    30820 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/SignificantGroups.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1032 2017-09-18 10:59:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/NeighbourJoining.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1913 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/DBSCAN.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     1098 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Grep.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)      808 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Face.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     2270 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/DataSets.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     8813 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/PolynomialRegression.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     3159 2017-03-14 12:54:37.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Scattermap.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     2128 2016-06-27 12:03:31.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Silhouette.svg
+-rw-r--r--   0 jk        (1000) jk        (1000)     8651 2017-01-19 18:59:40.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owclock.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     6347 2017-11-09 16:06:31.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owwebcamcapture.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    45657 2017-11-27 22:32:19.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owscattermap.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     1973 2016-02-26 16:23:03.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owhub.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    61575 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owlookalike.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     2965 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owselectsubset.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     4501 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owface.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:08.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/
+-rw-r--r--   0 jk        (1000) jk        (1000)      403 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/style.css
+-rw-r--r--   0 jk        (1000) jk        (1000)      440 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/html.html
+-rw-r--r--   0 jk        (1000) jk        (1000)     1536 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/script.js
+-rw-r--r--   0 jk        (1000) jk        (1000)  2246607 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.min.js
+-rw-r--r--   0 jk        (1000) jk        (1000)  2497777 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.upstream.js
+-rw-r--r--   0 jk        (1000) jk        (1000)    13445 2018-01-07 18:48:43.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/histogram.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     7445 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/plotly_widget.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/
+-rw-r--r--   0 jk        (1000) jk        (1000)      869 2018-01-09 16:46:23.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/style.css
+-rw-r--r--   0 jk        (1000) jk        (1000)     2200 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/script.js
+-rw-r--r--   0 jk        (1000) jk        (1000)     1900 2017-11-03 15:08:19.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owstack.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     5641 2017-07-11 11:43:00.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owreshape.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    12999 2018-01-09 16:43:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/ow1ka.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      881 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/__init__.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/data/
+-rw-r--r--   0 jk        (1000) jk        (1000)   930127 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/data/haarcascade_frontalface_default.xml
+-rw-r--r--   0 jk        (1000) jk        (1000)     4243 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owunique.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     5542 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owgooglesheets.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    14634 2018-01-05 19:52:47.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owparallelcoordinates.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     3474 2017-01-18 15:49:49.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owcontingency.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     9145 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owlineplot.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    12245 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owsignificantgroups.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     4691 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owipythonconnector.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     4908 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owneighbors.py
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/
+-rw-r--r--   0 jk        (1000) jk        (1000)    16712 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owgrep.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     9928 2018-01-07 18:48:43.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owfeaturestatistics.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     1056 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owselectsubset.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     1848 2016-11-29 13:49:46.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owlookalike.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      128 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owgrep_file.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)     4453 2017-03-14 13:00:23.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owcorrelations.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     4635 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owneighbors.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     2371 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owlda.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     7045 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owcorrelations.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    24158 2018-01-07 18:48:43.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owfeaturestatistics.py
+-rw-r--r--   0 jk        (1000) jk        (1000)    13644 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owgrep.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     1622 2017-12-12 20:20:44.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/ipython_connector.py
+-rw-r--r--   0 jk        (1000) jk        (1000)        0 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/__init__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)     4167 2017-11-03 15:08:19.000000 Orange3-Prototypes-0.9.0/orangecontrib/prototypes/stack.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      164 2015-09-04 14:22:48.000000 Orange3-Prototypes-0.9.0/orangecontrib/__init__.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      210 2016-06-27 12:03:31.000000 Orange3-Prototypes-0.9.0/.gitignore
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/doc/
+-rw-r--r--   0 jk        (1000) jk        (1000)      822 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/make.bat
+-rw-r--r--   0 jk        (1000) jk        (1000)      382 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/index.rst
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/doc/widgets/
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/
+-rw-r--r--   0 jk        (1000) jk        (1000)     5453 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/correlations.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     4926 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/google-sheets.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     5156 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/en-klik.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     4667 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/neighbors.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     5912 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/stacking.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     4554 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/contingency.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     4569 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/feature-statistics.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     4705 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/i-python.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     5660 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/icons/parallel-coordinates.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     1763 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/stacking.rst
+-rw-r--r--   0 jk        (1000) jk        (1000)     1929 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/enklik-anketa.rst
+-rw-r--r--   0 jk        (1000) jk        (1000)     1740 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/correlations.rst
+-rw-r--r--   0 jk        (1000) jk        (1000)     2208 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/neighbors.rst
+-rw-r--r--   0 jk        (1000) jk        (1000)     2150 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/parallel-coordinates.rst
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/
+-rw-r--r--   0 jk        (1000) jk        (1000)   169572 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Parallel-Coordinates-stamped.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   230871 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/EnKlik-Anketa-Example.png
+-rw-r--r--   0 jk        (1000) jk        (1000)    68354 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Correlations-links.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     7891 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Stacking-stamped.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   416694 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Neighbors-Example2.png
+-rw-r--r--   0 jk        (1000) jk        (1000)    75776 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Correlations-stamped.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   463644 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Parallel-Coordinates-Example.png
+-rw-r--r--   0 jk        (1000) jk        (1000)    18449 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Neighbors-stamped.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   183712 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Parallel-Coordinates-selection.png
+-rw-r--r--   0 jk        (1000) jk        (1000)    43156 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/EnKlik-Anketa-stamped.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   181014 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Contingency-Example.png
+-rw-r--r--   0 jk        (1000) jk        (1000)    38092 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Contingency-Table-stamped.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   166188 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Neighbors-Example1.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   149088 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Stacking-Example.png
+-rw-r--r--   0 jk        (1000) jk        (1000)   488121 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/Correlations-Example.png
+-rw-r--r--   0 jk        (1000) jk        (1000)    12353 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/images/public-link.png
+-rw-r--r--   0 jk        (1000) jk        (1000)     1170 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/widgets/contingency-table.rst
+-rw-r--r--   0 jk        (1000) jk        (1000)     4950 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/conf.py
+-rw-r--r--   0 jk        (1000) jk        (1000)      615 2018-01-25 18:51:32.000000 Orange3-Prototypes-0.9.0/doc/Makefile
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/
+-rw-r--r--   0 jk        (1000) jk        (1000)      372 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/PKG-INFO
+-rw-r--r--   0 jk        (1000) jk        (1000)      204 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/entry_points.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        1 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/dependency_links.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)        1 2015-08-28 10:51:37.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/not-zip-safe
+-rw-r--r--   0 jk        (1000) jk        (1000)     5762 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/SOURCES.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)       14 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/namespace_packages.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)      151 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/requires.txt
+-rw-r--r--   0 jk        (1000) jk        (1000)       14 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/Orange3_Prototypes.egg-info/top_level.txt
+drwxr-xr-x   0 jk        (1000) jk        (1000)        0 2018-01-25 18:52:07.000000 Orange3-Prototypes-0.9.0/.github/
+-rw-r--r--   0 jk        (1000) jk        (1000)      382 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.9.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 jk        (1000) jk        (1000)      217 2017-10-16 20:47:20.000000 Orange3-Prototypes-0.9.0/.github/PULL_REQUEST_TEMPLATE.md
```

### Comparing `Orange3-Prototypes-0.8.0/README.md` & `Orange3-Prototypes-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/setup.py` & `Orange3-Prototypes-0.9.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
-VERSION = '0.8.0'
+VERSION = '0.9.0'
 
 ENTRY_POINTS = {
     'orange3.addon': (
         'prototypes = orangecontrib.prototypes',
     ),
     # Entry point used to specify packages containing widgets.
     'orange.widgets': (
         # Syntax: category name = path.to.package.containing.widgets
         # Widget category specification can be seen in
         #    orangecontrib/datafusion/widgets/__init__.py
         'Prototypes = orangecontrib.prototypes.widgets',
     ),
+    # Register widget help
+    "orange.canvas.help": (
+    'html-index = orangecontrib.prototypes.widgets:WIDGET_HELP_PATH',
+    ),
 }
 
 if __name__ == '__main__':
     setup(
         name="Orange3-Prototypes",
         description="Prototype Orange widgets — only for the brave.",
         version=VERSION,
```

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/pandas_util.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/pandas_util.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/significance.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/significance.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owdbscan.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owdbscan.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ToShoppingList.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ToShoppingList.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Category-Prototypes.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Category-Prototypes.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ImageLandscape.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ImageLandscape.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Contingency.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Contingency.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/IPythonConnector.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/IPythonConnector.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/FeatureStatistics.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/FeatureStatistics.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Correlations.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Correlations.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/1ka.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/1ka.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/CreateClass.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/CreateClass.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ModelMap.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ModelMap.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/LinePlot.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/LinePlot.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Stacking.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Stacking.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Clock.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Clock.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/GoogleSheets.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/GoogleSheets.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Lookalike.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Lookalike.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/WebcamCapture.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/WebcamCapture.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Unique.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Unique.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Hub.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Hub.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/ParallelCoordinates.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/ParallelCoordinates.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/LinearProjection.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/LinearProjection.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/SignificantGroups.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/SignificantGroups.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/NeighbourJoining.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/NeighbourJoining.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/DBSCAN.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/DBSCAN.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Neighbours.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Neighbors.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Face.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Face.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/DataSets.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/DataSets.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/PolynomialRegression.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/PolynomialRegression.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Scattermap.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Scattermap.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/icons/Silhouette.svg` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/icons/Silhouette.svg`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owclock.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owclock.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owwebcamcapture.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owwebcamcapture.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owscattermap.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owscattermap.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owhub.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owhub.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owlookalike.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owlookalike.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owface.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owface.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/script.js` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/script.js`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.min.js` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.min.js`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.upstream.js` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/_plotly/plotly.upstream.js`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/histogram.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/utils/plotly_widget.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/utils/plotly_widget.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/style.css` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/style.css`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/script.js` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/_owparallelcoordinates/script.js`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owstack.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owstack.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owreshape.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owreshape.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/ow1ka.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/ow1ka.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/data/haarcascade_frontalface_default.xml` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/data/haarcascade_frontalface_default.xml`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owunique.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owunique.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owgooglesheets.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owgooglesheets.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owneighbours.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owneighbors.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,20 @@
     ("Jaccard", distance.Jaccard),
     ("Spearman", distance.SpearmanR),
     ("Absolute Spearman", distance.SpearmanRAbsolute),
     ("Pearson", distance.PearsonR),
     ("Absolute Pearson", distance.PearsonRAbsolute),
 ]
 
-class OWNeighbours(OWWidget):
-    name = "Neighbours"
-    description = "Compute nearest neighbours in data according to reference."
-    icon = "icons/Neighbours.svg"
+class OWNeighbors(OWWidget):
+    name = "Neighbors"
+    description = "Compute nearest neighbors in data according to reference."
+    icon = "icons/Neighbors.svg"
+
+    replaces = ["orangecontrib.prototypes.widgets.owneighbours.OWNeighbours"]
 
     inputs = [("Data", Table, "set_data"), ("Reference", Table, "set_ref")]
     outputs = [("Neighbors", Table)]
 
     n_neighbors = Setting(10)
     distance_index = Setting(0)
     exclude_reference = Setting(True)
@@ -103,28 +105,28 @@
         sorted_indices = list(np.argsort(dist.flatten()))[::-1]
         indices = []
         while len(sorted_indices) > 0 and len(indices) < self.n_neighbors:
             index = int(sorted_indices.pop() / len(self.reference))
             if (self.data[index] not in self.reference or
                     not self.exclude_reference) and index not in indices:
                 indices.append(index)
-        neighbours = data[indices]
-        neighbours.attributes = self.data.attributes
-        self.send("Neighbors", neighbours)
+        neighbors = data[indices]
+        neighbors.attributes = self.data.attributes
+        self.send("Neighbors", neighbors)
 
     @staticmethod
     def _add_similarity(data, dist):
         dist = np.min(dist, axis=1)[:, None]
         metas = data.domain.metas + (ContinuousVariable("similarity"),)
         domain = Domain(data.domain.attributes, data.domain.class_vars, metas)
         data_metas = np.hstack((data.metas, 100 * (1 - dist / np.max(dist))))
         return Table(domain, data.X, data.Y, data_metas)
 
 
 if __name__ == "__main__":
     a = QApplication([])
-    ow = OWNeighbours()
+    ow = OWNeighbors()
     ow.show()
     ow.set_data(Table("iris"))
     ow.set_ref(Table("iris")[:10])
     ow.raise_()
     a.exec_()
```

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owparallelcoordinates.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owparallelcoordinates.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owcontingency.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owcontingency.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owlineplot.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owlineplot.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owsignificantgroups.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owsignificantgroups.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owipythonconnector.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owipythonconnector.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owneighbours.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owneighbors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Test methods with long descriptive names can omit docstrings
 # pylint: disable=missing-docstring
 import numpy as np
 
 from Orange.data import Table
-from orangecontrib.prototypes.widgets.owneighbours import OWNeighbours
+from orangecontrib.prototypes.widgets.owneighbors import OWNeighbors
 from Orange.widgets.tests.base import WidgetTest, ParameterMapping
 
 
-class TestOWNeighbours(WidgetTest):
+class TestOWNeighbors(WidgetTest):
     def setUp(self):
-        self.widget = self.create_widget(OWNeighbours,
+        self.widget = self.create_widget(OWNeighbors,
                                          stored_settings={"auto_apply": False})
         self.iris = Table("iris")
 
     def test_input_data(self):
         """Check widget's data with data on the input"""
         self.assertEqual(self.widget.data, None)
         self.send_signal("Data", self.iris)
```

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owfeaturestatistics.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owfeaturestatistics.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owlookalike.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owlookalike.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/tests/test_owcorrelations.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/tests/test_owcorrelations.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owlda.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owlda.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owcorrelations.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owcorrelations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from enum import IntEnum
 from operator import attrgetter
 
 import numpy as np
+from Orange.widgets.utils.signals import Input, Output
 from scipy.stats import spearmanr
 
-from AnyQt.QtCore import Qt, QItemSelectionModel, QItemSelection
+from AnyQt.QtCore import Qt, QItemSelectionModel, QItemSelection, QSize
 from AnyQt.QtGui import QStandardItem
 from AnyQt.QtWidgets import QHeaderView
 
 from Orange.data import Table, Domain, ContinuousVariable, StringVariable
 from Orange.preprocess import SklImpute
 from Orange.widgets import gui
 from Orange.widgets.settings import Setting, ContextSetting, \
@@ -57,17 +58,21 @@
 
 class OWCorrelations(OWWidget):
     name = "Correlations"
     description = "Compute all pairwise attribute correlations."
     icon = "icons/Correlations.svg"
     priority = 2000
 
-    inputs = [("Data", Table, "set_data")]
-    outputs = [("Data", Table), ("Features", AttributeList),
-               ("Correlations", Table)]
+    class Inputs:
+        data = Input("Data", Table)
+
+    class Outputs:
+        data = Output("Data", Table)
+        features = Output("Features", AttributeList)
+        correlations = Output("Correlations", Table)
 
     want_control_area = False
 
     settingsHandler = DomainContextHandler()
     selection = ContextSetting(())
     correlation_type = Setting(0)
 
@@ -91,15 +96,17 @@
 
         gui.separator(box)
         box.layout().addWidget(self.vizrank.filter)
         box.layout().addWidget(self.vizrank.rank_table)
 
         button_box = gui.hBox(self.mainArea)
         button_box.layout().addWidget(self.vizrank.button)
-        button_box.layout().addWidget(self.report_button)
+
+    def sizeHint(self):
+        return QSize(350, 400)
 
     def _correlation_combo_changed(self):
         self.apply()
 
     def _vizrank_selection_changed(self, *args):
         self.selection = args
         self.commit()
@@ -111,14 +118,15 @@
             if model.data(model.index(i, 0)) == self.selection[0].name and \
                     model.data(model.index(i, 1)) == self.selection[1].name:
                 selection.select(model.index(i, 0), model.index(i, 2))
                 self.vizrank.rank_table.selectionModel().select(
                     selection, QItemSelectionModel.ClearAndSelect)
                 break
 
+    @Inputs.data
     def set_data(self, data):
         self.closeContext()
         self.clear_messages()
         self.data = data
         self.cont_data = None
         self.selection = ()
         if data is not None:
@@ -144,35 +152,35 @@
             header.setStretchLastSection(True)
             header.setSectionResizeMode(QHeaderView.ResizeToContents)
         else:
             self.commit()
 
     def commit(self):
         if self.data is None or self.cont_data is None:
-            self.send("Data", self.data)
-            self.send("Features", None)
-            self.send("Correlations", None)
+            self.Outputs.data.send(self.data)
+            self.Outputs.features.send(None)
+            self.Outputs.correlations.send(None)
             return
 
         metas = [StringVariable("Feature 1"), StringVariable("Feature 2")]
         domain = Domain([ContinuousVariable("Correlation")], metas=metas)
         model = self.vizrank.rank_model
         x = np.array([[float(model.data(model.index(row, 2)))] for row
                       in range(model.rowCount())])
         m = np.array([[model.data(model.index(row, 0)),
                        model.data(model.index(row, 1))] for row
                       in range(model.rowCount())], dtype=object)
         corr_table = Table(domain, x, metas=m)
         corr_table.name = "Correlations"
 
-        self.send("Data", self.data)
+        self.Outputs.data.send(self.data)
         # data has been imputed; send original attributes
-        self.send("Features", AttributeList([attr.compute_value.variable for
-                                             attr in self.selection]))
-        self.send("Correlations", corr_table)
+        self.Outputs.features.send(AttributeList([attr.compute_value.variable
+                                                  for attr in self.selection]))
+        self.Outputs.correlations.send(corr_table)
 
     def send_report(self):
         self.report_table(CorrelationType.items()[self.correlation_type],
                           self.vizrank.rank_table)
 
 
 if __name__ == "__main__":
```

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/widgets/owfeaturestatistics.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/widgets/owfeaturestatistics.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/ipython_connector.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/ipython_connector.py`

 * *Files identical despite different names*

### Comparing `Orange3-Prototypes-0.8.0/orangecontrib/prototypes/stack.py` & `Orange3-Prototypes-0.9.0/orangecontrib/prototypes/stack.py`

 * *Files identical despite different names*

