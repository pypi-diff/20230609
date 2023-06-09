# Comparing `tmp/gecco-tool-0.9.7.tar.gz` & `tmp/gecco-tool-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gecco-tool-0.9.7.tar", last modified: Fri May 26 12:00:09 2023, max compression
+gzip compressed data, was "gecco-tool-0.9.8.tar", last modified: Fri Jun  9 11:15:13 2023, max compression
```

## Comparing `gecco-tool-0.9.7.tar` & `gecco-tool-0.9.8.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    31905 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.400465 gecco-tool-0.9.7/gecco/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.400465 gecco-tool-0.9.7/gecco/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.404465 gecco-tool-0.9.7/gecco/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/annotate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)    15490 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/cli/commands/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.408465 gecco-tool-0.9.7/gecco/crf/
--rw-r--r--   0 runner    (1001) docker     (123)    16301 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/cv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/features.py
--rw-r--r--   0 runner    (1001) docker     (123)   517283 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/model.pkl
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/model.pkl.md5
--rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/crf/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.408465 gecco-tool-0.9.7/gecco/hmmer/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/hmmer/Pfam.ini
--rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/hmmer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.408465 gecco-tool-0.9.7/gecco/interpro/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/interpro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123) 20566339 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/interpro/interpro.json
--rw-r--r--   0 runner    (1001) docker     (123)    31338 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/orf.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/refine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.428465 gecco-tool-0.9.7/gecco/types/
--rw-r--r--   0 runner    (1001) docker     (123)     5385 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   143388 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/compositions.npz
--rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/domains.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    38175 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/gecco/types/types.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/gecco_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/gecco_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 12:00:09.000000 gecco-tool-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3465 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 12:00:09.432466 gecco-tool-0.9.7/static/
--rw-r--r--   0 runner    (1001) docker     (123)    23632 2023-05-26 11:59:14.000000 gecco-tool-0.9.7/static/gecco.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.301250 gecco-tool-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    31905 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-06-09 11:15:13.301250 gecco-tool-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.277250 gecco-tool-0.9.8/gecco/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.277250 gecco-tool-0.9.8/gecco/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.277250 gecco-tool-0.9.8/gecco/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8473 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22720 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9045 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/annotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13208 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9675 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14172 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15480 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/cli/commands/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.277250 gecco-tool-0.9.8/gecco/crf/
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/crf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/crf/cv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4288 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/crf/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)   517283 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/crf/model.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/crf/model.pkl.md5
+-rw-r--r--   0 runner    (1001) docker     (123)     6843 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/crf/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.277250 gecco-tool-0.9.8/gecco/hmmer/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/hmmer/Pfam.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/hmmer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.277250 gecco-tool-0.9.8/gecco/interpro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/interpro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123) 20566339 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/interpro/interpro.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31465 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/orf.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/refine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.301250 gecco-tool-0.9.8/gecco/types/
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143388 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/types/compositions.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    22128 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/types/domains.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    38175 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/gecco/types/types.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.301250 gecco-tool-0.9.8/gecco_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/gecco_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-09 11:15:13.000000 gecco-tool-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-06-09 11:15:13.301250 gecco-tool-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    16470 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:15:13.301250 gecco-tool-0.9.8/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    23632 2023-06-09 11:14:14.000000 gecco-tool-0.9.8/static/gecco.png
```

### Comparing `gecco-tool-0.9.7/CITATION.cff` & `gecco-tool-0.9.8/CITATION.cff`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/LICENSE` & `gecco-tool-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/PKG-INFO` & `gecco-tool-0.9.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecco-tool
-Version: 0.9.7
+Version: 0.9.8
 Summary: Gene cluster prediction with Conditional random fields.
 Home-page: https://gecco.embl.de
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Repository, https://github.com/zellerlab/GECCO
 Project-URL: Bug Tracker, https://github.com/zellerlab/GECCO/issues
@@ -129,19 +129,30 @@
   domains in the input sequences, in tabular format.
 - `{genome}.clusters.tsv`: If any were found, a *clusters* file, containing
   the coordinates of the predicted clusters along their putative biosynthetic
   type, in tabular format.
 - `{genome}_cluster_{N}.gbk`: If any were found, a GenBank file per cluster,
   containing the cluster sequence annotated with its member proteins and domains.
 
+GECCO can also convert results to other formats that may be more convenient
+depending on the downstream usage. GECCO can convert results into:
+
+- GFF3 format so they can be loaded into a genomic viewer 
+  (`gecco convert clusters --format gff`).
+- GenBank files with antiSMASH-style features so they can be loaded into 
+  [BiG-SLiCE](https://github.com/medema-group/bigslice) for further analysis
+  (`gecco convert gbk --format bigslice`).
+- FASTA files with the sequences of all the predicted BGCs (`gecco convert gbk --format fna`)
+  or with the sequences of all their proteins (`gecco convert gbk --format faa`).
+
 To get a more visual way of exploring of the predictions, you
 can open the GenBank files in a genome editing software like [UGENE](http://ugene.net/).
 You can otherwise load the results into an AntiSMASH report: check the
 [Integrations](https://gecco.embl.de/integrations.html#antismash) page of the
-documentation for a step-by-step guide.
+documentation for a step-by-step guide. 
 
 
 ## 🔖 Reference
 
 GECCO can be cited using the following preprint:
 
 > **Accurate de novo identification of biosynthetic gene clusters with GECCO**.
```

### Comparing `gecco-tool-0.9.7/README.md` & `gecco-tool-0.9.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -93,19 +93,30 @@
   domains in the input sequences, in tabular format.
 - `{genome}.clusters.tsv`: If any were found, a *clusters* file, containing
   the coordinates of the predicted clusters along their putative biosynthetic
   type, in tabular format.
 - `{genome}_cluster_{N}.gbk`: If any were found, a GenBank file per cluster,
   containing the cluster sequence annotated with its member proteins and domains.
 
+GECCO can also convert results to other formats that may be more convenient
+depending on the downstream usage. GECCO can convert results into:
+
+- GFF3 format so they can be loaded into a genomic viewer 
+  (`gecco convert clusters --format gff`).
+- GenBank files with antiSMASH-style features so they can be loaded into 
+  [BiG-SLiCE](https://github.com/medema-group/bigslice) for further analysis
+  (`gecco convert gbk --format bigslice`).
+- FASTA files with the sequences of all the predicted BGCs (`gecco convert gbk --format fna`)
+  or with the sequences of all their proteins (`gecco convert gbk --format faa`).
+
 To get a more visual way of exploring of the predictions, you
 can open the GenBank files in a genome editing software like [UGENE](http://ugene.net/).
 You can otherwise load the results into an AntiSMASH report: check the
 [Integrations](https://gecco.embl.de/integrations.html#antismash) page of the
-documentation for a step-by-step guide.
+documentation for a step-by-step guide. 
 
 
 ## 🔖 Reference
 
 GECCO can be cited using the following preprint:
 
 > **Accurate de novo identification of biosynthetic gene clusters with GECCO**.
```

### Comparing `gecco-tool-0.9.7/gecco/_base.py` & `gecco-tool-0.9.8/gecco/_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,14 +24,19 @@
     TextIO,
     Union,
     Sequence,
 )
 
 import polars
 
+try:
+    _POLARS_VERSION = tuple(map(int, polars.__version__.split('.')))
+except ValueError:
+    _POLARS_VERSION = (0, 0, 0)
+
 if typing.TYPE_CHECKING:
     _SELF = typing.TypeVar("_SELF")
     _TABLE = typing.TypeVar("_TABLE", bound="Table")
 
 
 class Dumpable(metaclass=abc.ABCMeta):
     """A metaclass for objects that can be dumped to a file.
@@ -111,19 +116,19 @@
 
     @classmethod
     def load(
         cls: typing.Type["_TABLE"], 
         fh: Union[BinaryIO, str, os.PathLike], 
     ) -> "_TABLE":
         columns = cls._get_columns()
-        data = polars.read_csv(
-            fh,
-            sep="\t",
-            dtypes={ column.name: column.dtype for column in columns }
-        )
+        dtypes = { column.name: column.dtype for column in columns }
+        if _POLARS_VERSION < (0, 16, 14):
+            data = polars.read_csv(fh, sep="\t", dtypes=dtypes)
+        else:
+            data = polars.read_csv(fh, separator="\t", dtypes=dtypes)
         for column_name in data.columns:
             if data[column_name].dtype in (polars.Float32, polars.Float64):
                 data = data.with_columns(polars.col(column_name).fill_null(math.nan))
         return cls(data)
 
     def dump(self, fh: Union[BinaryIO, str, os.PathLike]) -> None:
         # remove columns that contain only default values
@@ -137,10 +142,12 @@
             elif self.data[column.name].eq(column.default).all():
                 columns.remove(column)
         # write the table as a TSV file
         view = self.data[[column.name for column in columns]]
         for column_name in view.columns:
             if view[column_name].dtype in (polars.Float32, polars.Float64):
                 view = view.with_columns(polars.col(column_name).fill_nan(None))
-        view.write_csv(fh, sep="\t")
-
+        if _POLARS_VERSION < (0, 16, 14):
+            view.write_csv(fh, sep="\t")
+        else:
+            view.write_csv(fh, separator="\t")
```

### Comparing `gecco-tool-0.9.7/gecco/_meta.py` & `gecco-tool-0.9.8/gecco/_meta.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/_utils.py` & `gecco-tool-0.9.8/gecco/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/_base.py` & `gecco-tool-0.9.8/gecco/cli/commands/_base.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/_main.py` & `gecco-tool-0.9.8/gecco/cli/commands/_main.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/_mixins.py` & `gecco-tool-0.9.8/gecco/cli/commands/_mixins.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/annotate.py` & `gecco-tool-0.9.8/gecco/cli/commands/annotate.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/convert.py` & `gecco-tool-0.9.8/gecco/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/cv.py` & `gecco-tool-0.9.8/gecco/cli/commands/cv.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/help.py` & `gecco-tool-0.9.8/gecco/cli/commands/help.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/predict.py` & `gecco-tool-0.9.8/gecco/cli/commands/predict.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/run.py` & `gecco-tool-0.9.8/gecco/cli/commands/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from ... import __version__
 from ._base import Command, CommandExit, InvalidArgument
 from .annotate import Annotate
 from ._mixins import SequenceLoaderMixin, OutputWriterMixin, PredictorMixin
 from .._utils import patch_showwarnings
 
 try:
-    import importlib.resources as importlib_resources
+    from importlib.resources import files
 except ImportError:
-    import importlib_resources  # type: ignore
+    from importlib_resources import files # type: ignore
 
 if typing.TYPE_CHECKING:
     from ...types import TypeClassifier
     from ...model import Cluster, Gene
 
 
 class Run(Annotate, SequenceLoaderMixin, OutputWriterMixin, PredictorMixin):  # noqa: D101
@@ -179,15 +179,15 @@
 
     # ---
 
     def _load_model_domains(self) -> typing.Set[str]:
         try:
             if self.model is None:
                 self.info("Loading", "feature list from internal model", level=2)
-                domains_file = importlib_resources.open_text("gecco.types", "domains.tsv")
+                domains_file = files("gecco.types").joinpath("domains.tsv").open()
             else:
                 self.info("Loading", "feature list from", repr(self.model), level=2)
                 domains_file = open(os.path.join(self.model, "domains.tsv"))
             with domains_file as f:
                 domains = set(filter(None, map(str.strip, f)))
         except FileNotFoundError as err:
             if self.model is not None:
```

### Comparing `gecco-tool-0.9.7/gecco/cli/commands/train.py` & `gecco-tool-0.9.8/gecco/cli/commands/train.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/crf/__init__.py` & `gecco-tool-0.9.8/gecco/crf/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 from .._meta import sliding_window
 from ..model import Gene
 from . import features
 from .cv import LeaveOneGroupOut
 from .select import fisher_significance
 
 try:
-    import importlib.resources as importlib_resources
+    from importlib.resources import files
 except ImportError:
-    import importlib_resources  # type: ignore
+    from importlib_resources import files  # type: ignore
 
 __all__ = ["ClusterCRF"]
 
 
 class ClusterCRF(object):
     """A wrapper for `sklearn_crfsuite.CRF` to work with the GECCO data model.
     """
@@ -79,16 +79,16 @@
 
         """
         # get the path to the pickled model and read its signature file
         if model_path is not None:
             pkl_file: ContextManager[BinaryIO] = open(os.path.join(model_path, cls._FILENAME), "rb")
             md5_file: ContextManager[TextIO] = open(os.path.join(model_path, f"{cls._FILENAME}.md5"))
         else:
-            pkl_file = importlib_resources.open_binary(__name__, "model.pkl")
-            md5_file = importlib_resources.open_text(__name__, f"{cls._FILENAME}.md5")
+            pkl_file = files(__name__).joinpath(cls._FILENAME).open("rb")
+            md5_file = files(__name__).joinpath(f"{cls._FILENAME}.md5").open()
         with md5_file as sig:
             signature = sig.read().strip()
 
         # check the file content matches its MD5 hashsum
         hasher = hashlib.md5()
         with pkl_file as bin:
             read = functools.partial(bin.read, io.DEFAULT_BUFFER_SIZE)
```

### Comparing `gecco-tool-0.9.7/gecco/crf/cv.py` & `gecco-tool-0.9.8/gecco/crf/cv.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/crf/features.py` & `gecco-tool-0.9.8/gecco/crf/features.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/crf/model.pkl` & `gecco-tool-0.9.8/gecco/crf/model.pkl`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/crf/select.py` & `gecco-tool-0.9.8/gecco/crf/select.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/hmmer/__init__.py` & `gecco-tool-0.9.8/gecco/hmmer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 from pyhmmer.hmmer import hmmsearch
 
 from .._meta import requires, UniversalContainer
 from ..model import Gene, Domain
 from ..interpro import InterPro
 
 try:
-    import importlib.resources as importlib_resources
+    from importlib.resources import files, as_file
 except ImportError:
-    import importlib_resources  # type: ignore
+    from importlib_resources import files, as_file  # type: ignore
 
 __all__ = ["DomainAnnotator", "HMM", "PyHMMER", "embedded_hmms"]
 
 
 class HMM(typing.NamedTuple):
     """A Hidden Markov Model library to use with `~gecco.hmmer.HMMER`.
     """
@@ -197,26 +197,23 @@
         # return the updated list of genes that was given in argument
         return gene_index
 
 
 def embedded_hmms() -> Iterator[HMM]:
     """Iterate over the embedded HMMs that are shipped with GECCO.
     """
-    for filename in importlib_resources.contents(__name__):
+    for filename in files(__name__).glob("*.ini"):
 
-        if not filename.endswith(".ini"):
-            continue
-
-        ini_ctx = importlib_resources.path(__name__, filename)
+        ini_ctx = as_file(filename)
         ini_path = ini_ctx.__enter__()
         atexit.register(ini_ctx.__exit__, None, None, None)
 
         cfg = configparser.ConfigParser()
         cfg.read(ini_path)
         args: Dict[str, Any] = dict(cfg.items("hmm"))
         size = int(args.pop("size", 0))
 
-        hmm_ctx = importlib_resources.path(__name__, filename.replace(".ini", ".h3m"))
+        hmm_ctx = as_file(filename.with_suffix(".h3m"))
         hmm_path = hmm_ctx.__enter__()
         atexit.register(hmm_ctx.__exit__, None, None, None)
 
         yield HMM(path=os.fspath(hmm_path), size=size, **args)
```

### Comparing `gecco-tool-0.9.7/gecco/interpro/__init__.py` & `gecco-tool-0.9.8/gecco/interpro/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 import gzip
 import json
 from dataclasses import dataclass, field, fields
 from typing import Dict, List, Optional
 
 try:
-    import importlib.resources as importlib_resources
+    from importlib.resources import files
 except ImportError:
-    import importlib_resources  # type: ignore
+    from importlib_resources import files  # type: ignore
 
 
 __all__ = ["InterProEntry", "InterPro", "GeneOntologyTerm"]
 
 
 
 
@@ -61,15 +61,15 @@
 
     def __init__(self, entries: List[InterProEntry]):
         self.entries = entries
         self.by_accession = { member:entry for entry in entries for member in entry.members }
 
     @classmethod
     def load(cls) -> "InterPro":
-        with importlib_resources.open_binary(__name__, "interpro.json") as f:
+        with files(__name__).joinpath("interpro.json").open() as f:
             data = json.load(f)
             entries = []
             for raw_entry in data:
                 # get terms corresponding to domain
                 go_terms = [
                     GOTerm(**t) for t in raw_entry.pop("go_terms")
                 ]
```

### Comparing `gecco-tool-0.9.7/gecco/interpro/interpro.json` & `gecco-tool-0.9.8/gecco/interpro/interpro.json`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/model.py` & `gecco-tool-0.9.8/gecco/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import polars
 from Bio.Seq import Seq
 from Bio.SeqFeature import SeqFeature, FeatureLocation, CompoundLocation, Reference
 from Bio.SeqRecord import SeqRecord
 
 from . import __version__
 from .interpro import GOTerm
-from ._base import Dumpable, Table
+from ._base import Dumpable, Table, _POLARS_VERSION
 from ._meta import patch_locale
 
 if typing.TYPE_CHECKING:
     from numpy.typing import NDArray
 
 
 __all__ = [
@@ -725,15 +725,15 @@
     @classmethod
     def from_clusters(cls, clusters: Iterable[Cluster]) -> "ClusterTable":
         """Create a new cluster table from an iterable of clusters.
         """
         data = collections.defaultdict(list)
         for cluster in clusters:
             data["sequence_id"].append(cluster.source.id)
-            data["bgc_id"].append(cluster.id)
+            data["cluster_id"].append(cluster.id)
             data["start"].append(cluster.start)
             data["end"].append(cluster.end)
             if cluster.average_probability is not None:
                 data["average_p"].append(cluster.average_probability)
             if cluster.maximum_probability is not None:
                 data["max_p"].append(cluster.maximum_probability)
             if cluster.type is not None:
@@ -754,16 +754,18 @@
 
     def dump(self, fh: Union[BinaryIO, str, os.PathLike]) -> None:
         # patch `Table.dump` so that all columns are always written
         data = self.data
         for column_name in data.columns:
             if data[column_name].dtype in (polars.Float64, polars.Float64):
                 data = data.with_columns(polars.col(column_name).fill_nan(None))
-        data.write_csv(fh, sep="\t")
-
+        if _POLARS_VERSION < (0, 16, 14):
+            data.write_csv(fh, sep="\t")
+        else:
+            data.write_csv(fh, separator="\t")
 
 class GeneTable(Table):
     """A table storing gene coordinates and optional cluster probabilities.
     """
 
     @classmethod
     def _get_columns(cls) -> List["Table.Column"]:
```

### Comparing `gecco-tool-0.9.7/gecco/orf.py` & `gecco-tool-0.9.8/gecco/orf.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/refine.py` & `gecco-tool-0.9.8/gecco/refine.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/types/__init__.py` & `gecco-tool-0.9.8/gecco/types/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,17 +25,17 @@
 import scipy.sparse
 import sklearn.ensemble
 import sklearn.preprocessing
 
 from ..model import ClusterType, Cluster
 
 try:
-    import importlib.resources as importlib_resources
+    from importlib.resources import files
 except ImportError:
-    import importlib_resources  # type: ignore
+    from importlib_resources import files  # type: ignore
 
 if typing.TYPE_CHECKING:
     from numpy.typing import NDArray
 
 
 __all__ = ["TypeBinarizer", "TypeClassifier"]
 
@@ -83,17 +83,17 @@
         """
 
         if model_path is not None:
             doms_file: ContextManager[TextIO] = open(os.path.join(model_path, "domains.tsv"))
             typs_file: ContextManager[TextIO] = open(os.path.join(model_path, "types.tsv"))
             comp_file: ContextManager[BinaryIO] = open(os.path.join(model_path, "compositions.npz"), "rb")
         else:
-            doms_file = importlib_resources.open_text(__name__, "domains.tsv")
-            typs_file = importlib_resources.open_text(__name__, "types.tsv")
-            comp_file = importlib_resources.open_binary(__name__, "compositions.npz")
+            doms_file = files(__name__).joinpath("domains.tsv").open()
+            typs_file = files(__name__).joinpath("types.tsv").open()
+            comp_file = files(__name__).joinpath("compositions.npz").open("rb")
 
         with comp_file as comp_src:
             compositions = scipy.sparse.load_npz(comp_src)
         with doms_file as doms_src:
             domains = [ line.strip() for line in doms_src ]
         with typs_file as typs_src:
             types = []
```

### Comparing `gecco-tool-0.9.7/gecco/types/compositions.npz` & `gecco-tool-0.9.8/gecco/types/compositions.npz`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/types/domains.tsv` & `gecco-tool-0.9.8/gecco/types/domains.tsv`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco/types/types.tsv` & `gecco-tool-0.9.8/gecco/types/types.tsv`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/gecco_tool.egg-info/PKG-INFO` & `gecco-tool-0.9.8/gecco_tool.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gecco-tool
-Version: 0.9.7
+Version: 0.9.8
 Summary: Gene cluster prediction with Conditional random fields.
 Home-page: https://gecco.embl.de
 Author: Martin Larralde
 Author-email: martin.larralde@embl.de
 License: GPLv3
 Project-URL: Repository, https://github.com/zellerlab/GECCO
 Project-URL: Bug Tracker, https://github.com/zellerlab/GECCO/issues
@@ -129,19 +129,30 @@
   domains in the input sequences, in tabular format.
 - `{genome}.clusters.tsv`: If any were found, a *clusters* file, containing
   the coordinates of the predicted clusters along their putative biosynthetic
   type, in tabular format.
 - `{genome}_cluster_{N}.gbk`: If any were found, a GenBank file per cluster,
   containing the cluster sequence annotated with its member proteins and domains.
 
+GECCO can also convert results to other formats that may be more convenient
+depending on the downstream usage. GECCO can convert results into:
+
+- GFF3 format so they can be loaded into a genomic viewer 
+  (`gecco convert clusters --format gff`).
+- GenBank files with antiSMASH-style features so they can be loaded into 
+  [BiG-SLiCE](https://github.com/medema-group/bigslice) for further analysis
+  (`gecco convert gbk --format bigslice`).
+- FASTA files with the sequences of all the predicted BGCs (`gecco convert gbk --format fna`)
+  or with the sequences of all their proteins (`gecco convert gbk --format faa`).
+
 To get a more visual way of exploring of the predictions, you
 can open the GenBank files in a genome editing software like [UGENE](http://ugene.net/).
 You can otherwise load the results into an AntiSMASH report: check the
 [Integrations](https://gecco.embl.de/integrations.html#antismash) page of the
-documentation for a step-by-step guide.
+documentation for a step-by-step guide. 
 
 
 ## 🔖 Reference
 
 GECCO can be cited using the following preprint:
 
 > **Accurate de novo identification of biosynthetic gene clusters with GECCO**.
```

### Comparing `gecco-tool-0.9.7/gecco_tool.egg-info/SOURCES.txt` & `gecco-tool-0.9.8/gecco_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/setup.cfg` & `gecco-tool-0.9.8/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 	pyhmmer ~=0.8.0
 	wheel >=0.30
 	pronto ~=2.2
 install_requires = 
 	biopython ~=1.73
 	docopt ~=0.6.2
 	importlib-metadata >=4.0      ; python_version < '3.10'
+	importlib-resources >=1.0     ; python_version < '3.9'
 	numpy ~=1.16
 	polars ~=0.16.1
 	psutil ~=5.8
 	pyhmmer ~=0.8.0
 	pyrodigal ~=2.1
 	rich >=12.4.0
 	scikit-learn ~=1.0
```

### Comparing `gecco-tool-0.9.7/setup.py` & `gecco-tool-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `gecco-tool-0.9.7/static/gecco.png` & `gecco-tool-0.9.8/static/gecco.png`

 * *Files identical despite different names*

