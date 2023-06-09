# Comparing `tmp/pydraughts-0.6.2.tar.gz` & `tmp/pydraughts-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydraughts-0.6.2.tar", last modified: Wed Jun  7 12:47:53 2023, max compression
+gzip compressed data, was "pydraughts-0.6.3.tar", last modified: Fri Jun  9 18:44:40 2023, max compression
```

## Comparing `pydraughts-0.6.2.tar` & `pydraughts-0.6.3.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.712388 pydraughts-0.6.2/
--rw-rw-rw-   0        0        0     1078 2023-06-07 12:45:22.000000 pydraughts-0.6.2/LICENSE
--rw-rw-rw-   0        0        0       46 2023-06-07 12:42:58.000000 pydraughts-0.6.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5393 2023-06-07 12:47:53.713387 pydraughts-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4147 2023-06-07 12:42:58.000000 pydraughts-0.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.461323 pydraughts-0.6.2/draughts/
--rw-rw-rw-   0        0        0    12623 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/PDN.py
--rw-rw-rw-   0        0        0      238 2023-06-07 12:45:00.000000 pydraughts-0.6.2/draughts/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.532343 pydraughts-0.6.2/draughts/ballot_files/
--rw-rw-rw-   0        0        0   350063 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/11_english.json
--rw-rw-rw-   0        0        0   191861 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/11_italian.json
--rw-rw-rw-   0        0        0    17530 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/150russian_and_brazilian.json
--rw-rw-rw-   0        0        0     5225 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/2move_english.json
--rw-rw-rw-   0        0        0    21036 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/3move_english.json
--rw-rw-rw-   0        0        0   104689 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/4move_english.json
--rw-rw-rw-   0        0        0   388564 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/5move_english.json
--rw-rw-rw-   0        0        0    95519 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/brazilian.json
--rw-rw-rw-   0        0        0    96764 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballot_files/russian.json
--rw-rw-rw-   0        0        0     2185 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/ballots.py
--rw-rw-rw-   0        0        0    11930 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/convert.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.585355 pydraughts-0.6.2/draughts/core/
--rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/__init__.py
--rw-rw-rw-   0        0        0     7019 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/board.py
--rw-rw-rw-   0        0        0     2635 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/board_initializer.py
--rw-rw-rw-   0        0        0     3406 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/board_searcher.py
--rw-rw-rw-   0        0        0    35852 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/game.py
--rw-rw-rw-   0        0        0    19525 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/move.py
--rw-rw-rw-   0        0        0    28954 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/piece.py
--rw-rw-rw-   0        0        0    17684 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/core/variant.py
--rw-rw-rw-   0        0        0     1218 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engine.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.618363 pydraughts-0.6.2/draughts/engines/
--rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/__init__.py
--rw-rw-rw-   0        0        0     6447 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.648370 pydraughts-0.6.2/draughts/engines/checkerboard_extra/
--rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/__init__.py
--rw-rw-rw-   0        0        0     5506 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_64.py
--rw-rw-rw-   0        0        0     1133 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_client.py
--rw-rw-rw-   0        0        0     5091 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_server.py
--rw-rw-rw-   0        0        0     4405 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/checkerboard_extra/get_checker_board.py
--rw-rw-rw-   0        0        0     7267 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.665373 pydraughts-0.6.2/draughts/engines/dxp_communication/
--rw-rw-rw-   0        0        0        0 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp_communication/__init__.py
--rw-rw-rw-   0        0        0     8959 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_classes.py
--rw-rw-rw-   0        0        0    14219 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_run.py
--rw-rw-rw-   0        0        0    10797 2023-06-07 12:42:58.000000 pydraughts-0.6.2/draughts/engines/hub.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.681378 pydraughts-0.6.2/other_licenses/
--rw-rw-rw-   0        0        0     1111 2023-06-07 12:42:58.000000 pydraughts-0.6.2/other_licenses/ImparaAI checkers LICENSE
--rw-rw-rw-   0        0        0     1075 2023-06-07 12:42:58.000000 pydraughts-0.6.2/other_licenses/akalverboer DXC100_draughts_client LICENSE
--rw-rw-rw-   0        0        0     1073 2023-06-07 12:42:58.000000 pydraughts-0.6.2/other_licenses/fishnet LICENSE.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 12:47:53.707385 pydraughts-0.6.2/pydraughts.egg-info/
--rw-rw-rw-   0        0        0     5393 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1538 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 12:47:53.000000 pydraughts-0.6.2/pydraughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-07 12:42:58.000000 pydraughts-0.6.2/pyproject.toml
--rw-rw-rw-   0        0        0     1217 2023-06-07 12:47:53.716388 pydraughts-0.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.689990 pydraughts-0.6.3/
+-rw-rw-rw-   0        0        0     1078 2023-06-09 18:40:53.000000 pydraughts-0.6.3/LICENSE
+-rw-rw-rw-   0        0        0       46 2023-06-09 18:40:53.000000 pydraughts-0.6.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     5389 2023-06-09 18:44:40.689990 pydraughts-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4147 2023-06-09 18:40:53.000000 pydraughts-0.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.193872 pydraughts-0.6.3/draughts/
+-rw-rw-rw-   0        0        0    12623 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/PDN.py
+-rw-rw-rw-   0        0        0      238 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.386915 pydraughts-0.6.3/draughts/ballot_files/
+-rw-rw-rw-   0        0        0   350063 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/11_english.json
+-rw-rw-rw-   0        0        0   191861 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/11_italian.json
+-rw-rw-rw-   0        0        0    17530 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/150russian_and_brazilian.json
+-rw-rw-rw-   0        0        0     5225 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/2move_english.json
+-rw-rw-rw-   0        0        0    21036 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/3move_english.json
+-rw-rw-rw-   0        0        0   104689 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/4move_english.json
+-rw-rw-rw-   0        0        0   388564 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/5move_english.json
+-rw-rw-rw-   0        0        0    95519 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/brazilian.json
+-rw-rw-rw-   0        0        0    96764 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballot_files/russian.json
+-rw-rw-rw-   0        0        0     2185 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/ballots.py
+-rw-rw-rw-   0        0        0    11930 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/convert.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.458933 pydraughts-0.6.3/draughts/core/
+-rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/__init__.py
+-rw-rw-rw-   0        0        0     7019 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/board.py
+-rw-rw-rw-   0        0        0     2635 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/board_initializer.py
+-rw-rw-rw-   0        0        0     3406 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/board_searcher.py
+-rw-rw-rw-   0        0        0    35852 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/game.py
+-rw-rw-rw-   0        0        0    19525 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/move.py
+-rw-rw-rw-   0        0        0    28954 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/piece.py
+-rw-rw-rw-   0        0        0    17684 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/core/variant.py
+-rw-rw-rw-   0        0        0     1218 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engine.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.490941 pydraughts-0.6.3/draughts/engines/
+-rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/__init__.py
+-rw-rw-rw-   0        0        0     6447 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.582963 pydraughts-0.6.3/draughts/engines/checkerboard_extra/
+-rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/__init__.py
+-rw-rw-rw-   0        0        0     5506 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_64.py
+-rw-rw-rw-   0        0        0     1133 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_client.py
+-rw-rw-rw-   0        0        0     5091 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_server.py
+-rw-rw-rw-   0        0        0     4405 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/checkerboard_extra/get_checker_board.py
+-rw-rw-rw-   0        0        0     7062 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.616973 pydraughts-0.6.3/draughts/engines/dxp_communication/
+-rw-rw-rw-   0        0        0        0 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/__init__.py
+-rw-rw-rw-   0        0        0     8989 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_classes.py
+-rw-rw-rw-   0        0        0     8796 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_communication.py
+-rw-rw-rw-   0        0        0    14219 2023-06-07 12:42:58.000000 pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_run.py
+-rw-rw-rw-   0        0        0    10797 2023-06-09 18:40:53.000000 pydraughts-0.6.3/draughts/engines/hub.py
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.658983 pydraughts-0.6.3/other_licenses/
+-rw-rw-rw-   0        0        0     1111 2023-06-09 18:40:53.000000 pydraughts-0.6.3/other_licenses/ImparaAI checkers LICENSE
+-rw-rw-rw-   0        0        0     1075 2023-06-09 18:40:53.000000 pydraughts-0.6.3/other_licenses/akalverboer DXC100_draughts_client LICENSE
+-rw-rw-rw-   0        0        0     1073 2023-06-09 18:40:53.000000 pydraughts-0.6.3/other_licenses/fishnet LICENSE.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 18:44:40.685988 pydraughts-0.6.3/pydraughts.egg-info/
+-rw-rw-rw-   0        0        0     5389 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1594 2023-06-09 18:44:40.000000 pydraughts-0.6.3/pydraughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-09 18:44:39.000000 pydraughts-0.6.3/pydraughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-09 18:40:53.000000 pydraughts-0.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0     1213 2023-06-09 18:44:40.695992 pydraughts-0.6.3/setup.cfg
```

### Comparing `pydraughts-0.6.2/LICENSE` & `pydraughts-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/PKG-INFO` & `pydraughts-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydraughts
-Version: 0.6.2
+Version: 0.6.3
 Summary: A draughts library for Python with move generation, PDN reading and writing, engine communication and balloted openings
 Home-page: https://github.com/AttackingOrDefending/pydraughts
-Author: AttackingOrDefending
+Author: Ioannis Pantidis
 Project-URL: Bug Tracker, https://github.com/AttackingOrDefending/pydraughts/issues
 Keywords: checkers,draughts,game,fen,pdn
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydraughts-0.6.2/README.md` & `pydraughts-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/PDN.py` & `pydraughts-0.6.3/draughts/PDN.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/11_english.json` & `pydraughts-0.6.3/draughts/ballot_files/11_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/11_italian.json` & `pydraughts-0.6.3/draughts/ballot_files/11_italian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/150russian_and_brazilian.json` & `pydraughts-0.6.3/draughts/ballot_files/150russian_and_brazilian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/2move_english.json` & `pydraughts-0.6.3/draughts/ballot_files/2move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/3move_english.json` & `pydraughts-0.6.3/draughts/ballot_files/3move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/4move_english.json` & `pydraughts-0.6.3/draughts/ballot_files/4move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/5move_english.json` & `pydraughts-0.6.3/draughts/ballot_files/5move_english.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/brazilian.json` & `pydraughts-0.6.3/draughts/ballot_files/brazilian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballot_files/russian.json` & `pydraughts-0.6.3/draughts/ballot_files/russian.json`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/ballots.py` & `pydraughts-0.6.3/draughts/ballots.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/convert.py` & `pydraughts-0.6.3/draughts/convert.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/board.py` & `pydraughts-0.6.3/draughts/core/board.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/board_initializer.py` & `pydraughts-0.6.3/draughts/core/board_initializer.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/board_searcher.py` & `pydraughts-0.6.3/draughts/core/board_searcher.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/game.py` & `pydraughts-0.6.3/draughts/core/game.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/move.py` & `pydraughts-0.6.3/draughts/core/move.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/piece.py` & `pydraughts-0.6.3/draughts/core/piece.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/core/variant.py` & `pydraughts-0.6.3/draughts/core/variant.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engine.py` & `pydraughts-0.6.3/draughts/engine.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/checkerboard.py` & `pydraughts-0.6.3/draughts/engines/checkerboard.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_64.py` & `pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_64.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_client.py` & `pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_client.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/checkerboard_extra/engine_server.py` & `pydraughts-0.6.3/draughts/engines/checkerboard_extra/engine_server.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/checkerboard_extra/get_checker_board.py` & `pydraughts-0.6.3/draughts/engines/checkerboard_extra/get_checker_board.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/dxp.py` & `pydraughts-0.6.3/draughts/engines/dxp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,37 @@
-import draughts.engines.dxp_communication.dxp_run as dxp
+import draughts.engines.dxp_communication.dxp_communication as dxp_communication
 import draughts
 import draughts.engine
 import subprocess
 import os
 import signal
 import threading
 import time
 import logging
-from importlib import reload
 from typing import Optional, Dict, Union, List, Any
 
 logger = logging.getLogger("pydraughts")
 
 
 class DXPEngine:
     def __init__(self, command: Union[List[str], str, None] = None, options: Optional[Dict[str, Union[str, int, bool]]] = None, initial_time: int = 0, cwd: Optional[str] = None, ENGINE: int = 5) -> None:
-        global dxp
-        dxp = reload(dxp)
         if options is None:
             options = {}
         self.initial_time = initial_time
         self.max_moves = 0
         self.ip = '127.0.0.1'
         self.port = '27531'
         self.command = command
         self.engine_opened = True  # Whether the engine is already open or pydraughts should open it
         self.wait_to_open_time = 10
         self.ENGINE = ENGINE
         self.info: Dict[str, Any] = {}
         self.id: Dict[str, str] = {}
-        self.console = dxp.tConsoleHandler
-        self.receiver = dxp.tReceiveHandler
+        self.sender = dxp_communication.Sender()
+        self.receiver = self.sender.receiver
         self.game_started = False
         self.exit = False
 
         self.configure(options)
 
         if not self.engine_opened:
             cwd = cwd or os.getcwd()
@@ -122,27 +119,27 @@
     def _connect(self) -> None:
         """Connect to the engine."""
         if not self.engine_opened:
             wait_time = self.start_time / 1e9 + self.wait_to_open_time - time.perf_counter_ns() / 1e9
             logger.debug(f'wait time before connecting: {wait_time}')
             if wait_time > 0:
                 time.sleep(wait_time)
-        self.console.run_command(f'connect {self.ip} {self.port}')
+        self.sender.connect(self.ip, int(self.port))
 
-    def _start(self, board: draughts.Board, time: int) -> None:
+    def _start(self, board: draughts.Board, game_time: int) -> None:
         """Start the game."""
         self._connect()
         color = 'B' if board.turn == draughts.WHITE else 'W'
-        time = str(round(time // 60))
+        game_time = int(round(game_time // 60))
         moves = self.max_moves
-        self.console.run_command(f'setup {board.initial_fen} {board.variant}')
-        self.console.run_command(f'gamereq {color} {time} {moves}')
+        self.sender.setup(board.initial_fen, board.variant)
+        self.sender.gamereq(color, game_time, moves)
         accepted = self._recv_accept()
         logger.debug(f'Aceepted: {accepted}')
-        self.id["name"] = dxp.current.engineName
+        self.id["name"] = self.sender.current.engineName
 
     def _recv(self) -> None:
         """Receive a line from the engine, if the engine is opened by pydraughts."""
         # The engine doesn't work otherwise.
         while True:
             try:
                 line = self.p.stdout.readline()
@@ -156,37 +153,34 @@
                     break
                 else:
                     raise err
 
     def _recv_accept(self) -> bool:
         """Get if the game was accepted."""
         while True:
-            if dxp.accepted is not None:
-                return dxp.accepted
+            if self.receiver.accepted is not None:
+                return self.receiver.accepted
 
     def _recv_move(self) -> Optional[List[List[int]]]:
         """Receive the engine move."""
         while True:
-            if not dxp.tReceiveHandler.isListening:
+            if not self.receiver.listening:
                 break
-            if dxp.last_move_changed:
-                logger.debug(f'new last move: {dxp.last_move.board_move}')
-                return dxp.last_move
+            if self.receiver.last_move_changed:
+                logger.debug(f'new last move: {self.receiver.last_move.board_move}')
+                return self.receiver.last_move
 
     def play(self, board: draughts.Board) -> Any:
         """Engine search."""
         if not self.game_started:
             self._start(board, self.initial_time)
             self.game_started = True
         if board.move_stack:
-            move = board.move_stack[-1].li_one_move
-            move = [move[i:i+2] for i in range(0, len(move), 2)]
-            move = '-'.join(move)
-            self.console.run_command(f'sm {move}')
+            self.sender.send_move(board.move_stack[-1])
         best_move = self._recv_move()
         return draughts.engine.PlayResult(best_move, None, {})
 
     def quit(self) -> None:
         """Quit the engine."""
-        self.console.run_command('gameend 0')
-        self.console.run_command("disconn")
+        self.sender.gameend()
+        self.sender.disconnect()
         self.quit_time = time.perf_counter_ns()
```

### Comparing `pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_classes.py` & `pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 logger = logging.getLogger("pydraughts")
 
 DXP_WHITE = 0
 DXP_BLACK = 1
 
 
 class GameStatus:
-    def __init__(self, fen: str = 'startpos', myColor: int = DXP_WHITE, started: bool = False, variant: str = 'standard') -> None:
+    def __init__(self, fen: str = 'startpos', my_color: int = DXP_WHITE, started: bool = False, variant: str = 'standard') -> None:
         self.fen = fen
-        self.myColor = myColor
+        self.my_color = my_color
         self.started = started
         self.variant = variant
         self.pos = draughts.Board(fen=fen, variant=variant)
         self.color = self.get_color()
         self.engineName = ''
         self.result = None
 
@@ -79,15 +79,15 @@
                 raise Exception("receive exception: socket connection broken")
             msg += chunk.decode()
             if msg.find("\0") > -1:
                 break
             if len(msg) > 128:
                 break  # too long, no null char
 
-        logger.debug("final msg: " + msg)
+        logger.debug(f"socket receive: {msg}")
         msg = msg.replace("\0", "")  # remove all null chars
 
         # Use strip to remove all whitespace at the start and end.
         # Including spaces, tabs, newlines and carriage returns.
         msg = msg.strip()
         return msg
 
@@ -152,44 +152,44 @@
 
     def msg_chat(self, msg: str) -> str:
         """Generate a CHAT message."""
         # Generate CHAT message. Example: CWhat do you think about move 35?
         msg = "C" + msg
         return msg
 
-    def msg_gamereq(self, myColor: int, gameTime: int, numMoves: int, pos: Optional[draughts.Board] = None, colorToMove: Optional[int] = None) -> str:
+    def msg_gamereq(self, my_color: int, game_time: int, num_moves: int, pos: Optional[draughts.Board] = None, color_to_move: Optional[int] = None) -> str:
         """Generate a GAMEREQ message."""
         # Generate GAMEREQ message. Example: R01Tornado voor Windows 4.0        W060065A
         gamereq = []
         gamereq.append("R")  # header
         gamereq.append("01")  # version
 
         gamereq.append("DXP Client".ljust(32)[:32])  # iName: fixed length padding spaces
-        gamereq.append('Z' if myColor == DXP_WHITE else 'W')  # fColor: color of follower (server)
-        gamereq.append(str(gameTime).zfill(3))  # gameTime: time limit of game (ex: 090)
-        gamereq.append(str(numMoves).zfill(3))  # numMoves: number of moves of time limit (ex: 050)
-        if pos is None or colorToMove is None:
+        gamereq.append('Z' if my_color == DXP_WHITE else 'W')  # fColor: color of follower (server)
+        gamereq.append(str(game_time).zfill(3))  # game_time: time limit of game (ex: 090)
+        gamereq.append(str(num_moves).zfill(3))  # num_moves: number of moves of time limit (ex: 050)
+        if pos is None or color_to_move is None:
             gamereq.append("A")  # posInd == A: use starting position
         else:
-            gamereq.append("B")  # posInd == B: use parameters pos and colorToMove
-            gamereq.append("W" if colorToMove == DXP_WHITE else "Z")  # mColor
+            gamereq.append("B")  # posInd == B: use parameters pos and color_to_move
+            gamereq.append("W" if color_to_move == DXP_WHITE else "Z")  # mColor
             gamereq.append(pos._game.get_dxp_fen())  # board
 
         msg = ""
         for item in gamereq:
             msg = msg + item
         return msg
 
-    def msg_move(self, steps: List[int], captures: List[int], timeSpend: int) -> str:
+    def msg_move(self, steps: List[int], captures: List[int], time_spent: int) -> str:
         """Generate a MOVE message."""
         # Generate MOVE message. Example: M001205250422122320
         # Parm rmove is a "two-color" move
         move = []
         move.append("M")  # header
-        move.append(str(timeSpend % 10000).zfill(4))  # mTime: 0000 .. 9999
+        move.append(str(time_spent % 10000).zfill(4))  # mTime: 0000 .. 9999
         move.append(str(steps[0] % 100).zfill(2))  # mFrom
         move.append(str(steps[-1] % 100).zfill(2))  # mTo
         move.append(str(len(captures) % 100).zfill(2))  # mNumCaptured: number of takes (captures)
         for k in captures:
             move.append(str(k % 100).zfill(2))  # mCaptures
 
         msg = ""
@@ -205,21 +205,21 @@
         gameend.append(str(reason)[0])  # reason:  0 > unknown  1 > I lose  2 > draw  3 > I win
         gameend.append("1")  # stop code: 0 > next game preferred  1: > no next game
         msg = ""
         for item in gameend:
             msg = msg + item
         return msg
 
-    def msg_backreq(self, moveId: int, colorToMove: int) -> str:
+    def msg_backreq(self, moveId: int, color_to_move: int) -> str:
         """Generate a BACKREQ message."""
         # Generate BACKREQ message. Example: B005Z
         backreq = []
         backreq.append("B")
         backreq.append(str(moveId % 1000).zfill(3))  # moveId
-        backreq.append("W" if colorToMove == DXP_WHITE else "Z")  # mColor
+        backreq.append("W" if color_to_move == DXP_WHITE else "Z")  # mColor
         msg = ""
         for item in backreq:
             msg = msg + item
         return msg
 
     def msg_backacc(self, accCode: str) -> str:
         """Generate the response to a BACKREQ request."""
```

### Comparing `pydraughts-0.6.2/draughts/engines/dxp_communication/dxp_run.py` & `pydraughts-0.6.3/draughts/engines/dxp_communication/dxp_run.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/draughts/engines/hub.py` & `pydraughts-0.6.3/draughts/engines/hub.py`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/other_licenses/ImparaAI checkers LICENSE` & `pydraughts-0.6.3/other_licenses/ImparaAI checkers LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/other_licenses/akalverboer DXC100_draughts_client LICENSE` & `pydraughts-0.6.3/other_licenses/akalverboer DXC100_draughts_client LICENSE`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/other_licenses/fishnet LICENSE.txt` & `pydraughts-0.6.3/other_licenses/fishnet LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pydraughts-0.6.2/pydraughts.egg-info/PKG-INFO` & `pydraughts-0.6.3/pydraughts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pydraughts
-Version: 0.6.2
+Version: 0.6.3
 Summary: A draughts library for Python with move generation, PDN reading and writing, engine communication and balloted openings
 Home-page: https://github.com/AttackingOrDefending/pydraughts
-Author: AttackingOrDefending
+Author: Ioannis Pantidis
 Project-URL: Bug Tracker, https://github.com/AttackingOrDefending/pydraughts/issues
 Keywords: checkers,draughts,game,fen,pdn
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pydraughts-0.6.2/pydraughts.egg-info/SOURCES.txt` & `pydraughts-0.6.3/pydraughts.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 draughts/engines/checkerboard_extra/__init__.py
 draughts/engines/checkerboard_extra/engine_64.py
 draughts/engines/checkerboard_extra/engine_client.py
 draughts/engines/checkerboard_extra/engine_server.py
 draughts/engines/checkerboard_extra/get_checker_board.py
 draughts/engines/dxp_communication/__init__.py
 draughts/engines/dxp_communication/dxp_classes.py
+draughts/engines/dxp_communication/dxp_communication.py
 draughts/engines/dxp_communication/dxp_run.py
 other_licenses/ImparaAI checkers LICENSE
 other_licenses/akalverboer DXC100_draughts_client LICENSE
 other_licenses/fishnet LICENSE.txt
 pydraughts.egg-info/PKG-INFO
 pydraughts.egg-info/SOURCES.txt
 pydraughts.egg-info/dependency_links.txt
```

### Comparing `pydraughts-0.6.2/setup.cfg` & `pydraughts-0.6.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 7964 7261 7567 6874 730d 0a76   = pydraughts..v
 00000020: 6572 7369 6f6e 203d 2061 7474 723a 2064  ersion = attr: d
 00000030: 7261 7567 6874 732e 5f5f 7665 7273 696f  raughts.__versio
-00000040: 6e5f 5f0d 0a61 7574 686f 7220 3d20 4174  n__..author = At
-00000050: 7461 636b 696e 674f 7244 6566 656e 6469  tackingOrDefendi
-00000060: 6e67 0d0a 6465 7363 7269 7074 696f 6e20  ng..description 
-00000070: 3d20 4120 6472 6175 6768 7473 206c 6962  = A draughts lib
-00000080: 7261 7279 2066 6f72 2050 7974 686f 6e20  rary for Python 
-00000090: 7769 7468 206d 6f76 6520 6765 6e65 7261  with move genera
-000000a0: 7469 6f6e 2c20 5044 4e20 7265 6164 696e  tion, PDN readin
-000000b0: 6720 616e 6420 7772 6974 696e 672c 2065  g and writing, e
-000000c0: 6e67 696e 6520 636f 6d6d 756e 6963 6174  ngine communicat
-000000d0: 696f 6e20 616e 6420 6261 6c6c 6f74 6564  ion and balloted
-000000e0: 206f 7065 6e69 6e67 730d 0a6c 6f6e 675f   openings..long_
-000000f0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-00000100: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-00000110: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-00000120: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000130: 6578 742f 6d61 726b 646f 776e 0d0a 6b65  ext/markdown..ke
-00000140: 7977 6f72 6473 203d 2063 6865 636b 6572  ywords = checker
-00000150: 732c 2064 7261 7567 6874 732c 2067 616d  s, draughts, gam
-00000160: 652c 2066 656e 2c20 7064 6e0d 0a75 726c  e, fen, pdn..url
-00000170: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-00000180: 622e 636f 6d2f 4174 7461 636b 696e 674f  b.com/AttackingO
-00000190: 7244 6566 656e 6469 6e67 2f70 7964 7261  rDefending/pydra
-000001a0: 7567 6874 730d 0a70 726f 6a65 6374 5f75  ughts..project_u
-000001b0: 726c 7320 3d20 0d0a 0942 7567 2054 7261  rls = ...Bug Tra
-000001c0: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-000001d0: 6974 6875 622e 636f 6d2f 4174 7461 636b  ithub.com/Attack
-000001e0: 696e 674f 7244 6566 656e 6469 6e67 2f70  ingOrDefending/p
-000001f0: 7964 7261 7567 6874 732f 6973 7375 6573  ydraughts/issues
-00000200: 0d0a 636c 6173 7369 6669 6572 7320 3d20  ..classifiers = 
-00000210: 0d0a 0949 6e74 656e 6465 6420 4175 6469  ...Intended Audi
-00000220: 656e 6365 203a 3a20 4465 7665 6c6f 7065  ence :: Develope
-00000230: 7273 0d0a 0949 6e74 656e 6465 6420 4175  rs...Intended Au
-00000240: 6469 656e 6365 203a 3a20 5363 6965 6e63  dience :: Scienc
-00000250: 652f 5265 7365 6172 6368 0d0a 0950 726f  e/Research...Pro
-00000260: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
-00000270: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
-00000280: 0d0a 094c 6963 656e 7365 203a 3a20 4f53  ...License :: OS
-00000290: 4920 4170 7072 6f76 6564 203a 3a20 4d49  I Approved :: MI
-000002a0: 5420 4c69 6365 6e73 650d 0a09 4f70 6572  T License...Oper
-000002b0: 6174 696e 6720 5379 7374 656d 203a 3a20  ating System :: 
-000002c0: 4f53 2049 6e64 6570 656e 6465 6e74 0d0a  OS Independent..
-000002d0: 0954 6f70 6963 203a 3a20 4761 6d65 732f  .Topic :: Games/
-000002e0: 456e 7465 7274 6169 6e6d 656e 7420 3a3a  Entertainment ::
-000002f0: 2042 6f61 7264 2047 616d 6573 0d0a 0954   Board Games...T
-00000300: 6f70 6963 203a 3a20 4761 6d65 732f 456e  opic :: Games/En
-00000310: 7465 7274 6169 6e6d 656e 7420 3a3a 2054  tertainment :: T
-00000320: 7572 6e20 4261 7365 6420 5374 7261 7465  urn Based Strate
-00000330: 6779 0d0a 0954 6f70 6963 203a 3a20 536f  gy...Topic :: So
-00000340: 6674 7761 7265 2044 6576 656c 6f70 6d65  ftware Developme
-00000350: 6e74 203a 3a20 4c69 6272 6172 6965 7320  nt :: Libraries 
-00000360: 3a3a 2050 7974 686f 6e20 4d6f 6475 6c65  :: Python Module
-00000370: 730d 0a6c 6963 656e 7365 5f66 696c 6573  s..license_files
-00000380: 203d 200d 0a09 4c49 4345 4e53 450d 0a09   = ...LICENSE...
-00000390: 6f74 6865 725f 6c69 6365 6e73 6573 2f2a  other_licenses/*
-000003a0: 0d0a 0d0a 5b6f 7074 696f 6e73 5d0d 0a69  ....[options]..i
-000003b0: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-000003c0: 6174 6120 3d20 5472 7565 0d0a 7061 636b  ata = True..pack
-000003d0: 6167 6573 203d 200d 0a09 6472 6175 6768  ages = ...draugh
-000003e0: 7473 0d0a 0964 7261 7567 6874 732e 636f  ts...draughts.co
-000003f0: 7265 0d0a 0964 7261 7567 6874 732e 656e  re...draughts.en
-00000400: 6769 6e65 730d 0a09 6472 6175 6768 7473  gines...draughts
-00000410: 2e65 6e67 696e 6573 2e64 7870 5f63 6f6d  .engines.dxp_com
-00000420: 6d75 6e69 6361 7469 6f6e 0d0a 0964 7261  munication...dra
-00000430: 7567 6874 732e 656e 6769 6e65 732e 6368  ughts.engines.ch
-00000440: 6563 6b65 7262 6f61 7264 5f65 7874 7261  eckerboard_extra
-00000450: 0d0a 7079 7468 6f6e 5f72 6571 7569 7265  ..python_require
-00000460: 7320 3d20 3e3d 332e 380d 0a69 6e73 7461  s = >=3.8..insta
-00000470: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
-00000480: 096d 736c 2d6c 6f61 646c 6962 3d3d 302e  .msl-loadlib==0.
-00000490: 392e 300d 0a0d 0a5b 6567 675f 696e 666f  9.0....[egg_info
-000004a0: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-000004b0: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-000004c0: 0a                                       .
+00000040: 6e5f 5f0d 0a61 7574 686f 7220 3d20 496f  n__..author = Io
+00000050: 616e 6e69 7320 5061 6e74 6964 6973 0d0a  annis Pantidis..
+00000060: 6465 7363 7269 7074 696f 6e20 3d20 4120  description = A 
+00000070: 6472 6175 6768 7473 206c 6962 7261 7279  draughts library
+00000080: 2066 6f72 2050 7974 686f 6e20 7769 7468   for Python with
+00000090: 206d 6f76 6520 6765 6e65 7261 7469 6f6e   move generation
+000000a0: 2c20 5044 4e20 7265 6164 696e 6720 616e  , PDN reading an
+000000b0: 6420 7772 6974 696e 672c 2065 6e67 696e  d writing, engin
+000000c0: 6520 636f 6d6d 756e 6963 6174 696f 6e20  e communication 
+000000d0: 616e 6420 6261 6c6c 6f74 6564 206f 7065  and balloted ope
+000000e0: 6e69 6e67 730d 0a6c 6f6e 675f 6465 7363  nings..long_desc
+000000f0: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
+00000100: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
+00000110: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+00000120: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
+00000130: 6d61 726b 646f 776e 0d0a 6b65 7977 6f72  markdown..keywor
+00000140: 6473 203d 2063 6865 636b 6572 732c 2064  ds = checkers, d
+00000150: 7261 7567 6874 732c 2067 616d 652c 2066  raughts, game, f
+00000160: 656e 2c20 7064 6e0d 0a75 726c 203d 2068  en, pdn..url = h
+00000170: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000180: 6d2f 4174 7461 636b 696e 674f 7244 6566  m/AttackingOrDef
+00000190: 656e 6469 6e67 2f70 7964 7261 7567 6874  ending/pydraught
+000001a0: 730d 0a70 726f 6a65 6374 5f75 726c 7320  s..project_urls 
+000001b0: 3d20 0d0a 0942 7567 2054 7261 636b 6572  = ...Bug Tracker
+000001c0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
+000001d0: 622e 636f 6d2f 4174 7461 636b 696e 674f  b.com/AttackingO
+000001e0: 7244 6566 656e 6469 6e67 2f70 7964 7261  rDefending/pydra
+000001f0: 7567 6874 732f 6973 7375 6573 0d0a 636c  ughts/issues..cl
+00000200: 6173 7369 6669 6572 7320 3d20 0d0a 0949  assifiers = ...I
+00000210: 6e74 656e 6465 6420 4175 6469 656e 6365  ntended Audience
+00000220: 203a 3a20 4465 7665 6c6f 7065 7273 0d0a   :: Developers..
+00000230: 0949 6e74 656e 6465 6420 4175 6469 656e  .Intended Audien
+00000240: 6365 203a 3a20 5363 6965 6e63 652f 5265  ce :: Science/Re
+00000250: 7365 6172 6368 0d0a 0950 726f 6772 616d  search...Program
+00000260: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000270: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+00000280: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000290: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000002a0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+000002b0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+000002c0: 6e64 6570 656e 6465 6e74 0d0a 0954 6f70  ndependent...Top
+000002d0: 6963 203a 3a20 4761 6d65 732f 456e 7465  ic :: Games/Ente
+000002e0: 7274 6169 6e6d 656e 7420 3a3a 2042 6f61  rtainment :: Boa
+000002f0: 7264 2047 616d 6573 0d0a 0954 6f70 6963  rd Games...Topic
+00000300: 203a 3a20 4761 6d65 732f 456e 7465 7274   :: Games/Entert
+00000310: 6169 6e6d 656e 7420 3a3a 2054 7572 6e20  ainment :: Turn 
+00000320: 4261 7365 6420 5374 7261 7465 6779 0d0a  Based Strategy..
+00000330: 0954 6f70 6963 203a 3a20 536f 6674 7761  .Topic :: Softwa
+00000340: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
+00000350: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
+00000360: 7974 686f 6e20 4d6f 6475 6c65 730d 0a6c  ython Modules..l
+00000370: 6963 656e 7365 5f66 696c 6573 203d 200d  icense_files = .
+00000380: 0a09 4c49 4345 4e53 450d 0a09 6f74 6865  ..LICENSE...othe
+00000390: 725f 6c69 6365 6e73 6573 2f2a 0d0a 0d0a  r_licenses/*....
+000003a0: 5b6f 7074 696f 6e73 5d0d 0a69 6e63 6c75  [options]..inclu
+000003b0: 6465 5f70 6163 6b61 6765 5f64 6174 6120  de_package_data 
+000003c0: 3d20 5472 7565 0d0a 7061 636b 6167 6573  = True..packages
+000003d0: 203d 200d 0a09 6472 6175 6768 7473 0d0a   = ...draughts..
+000003e0: 0964 7261 7567 6874 732e 636f 7265 0d0a  .draughts.core..
+000003f0: 0964 7261 7567 6874 732e 656e 6769 6e65  .draughts.engine
+00000400: 730d 0a09 6472 6175 6768 7473 2e65 6e67  s...draughts.eng
+00000410: 696e 6573 2e64 7870 5f63 6f6d 6d75 6e69  ines.dxp_communi
+00000420: 6361 7469 6f6e 0d0a 0964 7261 7567 6874  cation...draught
+00000430: 732e 656e 6769 6e65 732e 6368 6563 6b65  s.engines.checke
+00000440: 7262 6f61 7264 5f65 7874 7261 0d0a 7079  rboard_extra..py
+00000450: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000460: 3e3d 332e 380d 0a69 6e73 7461 6c6c 5f72  >=3.8..install_r
+00000470: 6571 7569 7265 7320 3d20 0d0a 096d 736c  equires = ...msl
+00000480: 2d6c 6f61 646c 6962 3d3d 302e 392e 300d  -loadlib==0.9.0.
+00000490: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
+000004a0: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
+000004b0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
```

