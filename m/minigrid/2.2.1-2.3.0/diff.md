# Comparing `tmp/minigrid-2.2.1.tar.gz` & `tmp/minigrid-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minigrid-2.2.1.tar", last modified: Mon Mar 27 23:38:35 2023, max compression
+gzip compressed data, was "minigrid-2.3.0.tar", last modified: Fri Jun  9 12:13:38 2023, max compression
```

## Comparing `minigrid-2.2.1.tar` & `minigrid-2.3.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.399314 minigrid-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-03-27 23:38:26.000000 minigrid-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-03-27 23:38:35.399314 minigrid-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-03-27 23:38:26.000000 minigrid-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.383314 minigrid-2.2.1/minigrid/
--rw-r--r--   0 runner    (1001) docker     (123)    28823 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3430 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/benchmark.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.387314 minigrid-2.2.1/minigrid/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9463 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8724 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/mission.py
--rw-r--r--   0 runner    (1001) docker     (123)    13059 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/roomgrid.py
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/core/world_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.395314 minigrid-2.2.1/minigrid/envs/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.395314 minigrid-2.2.1/minigrid/envs/babyai/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.399314 minigrid-2.2.1/minigrid/envs/babyai/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/core/levelgen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/core/roomgrid_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/core/verifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    23748 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/goto.py
--rw-r--r--   0 runner    (1001) docker     (123)    12188 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/open.py
--rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/other.py
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/pickup.py
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/putnext.py
--rw-r--r--   0 runner    (1001) docker     (123)    14856 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/synth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13690 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/babyai/unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/blockedunlockpickup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/crossing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/distshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3356 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/doorkey.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/dynamicobstacles.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/fourrooms.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/gotodoor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/gotoobject.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/keycorridor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4051 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/lavagap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/lockedroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/multiroom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/obstructedmaze.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/obstructedmaze_v1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/putnear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/redbluedoors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/unlock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/envs/unlockpickup.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3756 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/manual_control.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23789 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/minigrid_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.399314 minigrid-2.2.1/minigrid/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/utils/rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)    24772 2023-03-27 23:38:26.000000 minigrid-2.2.1/minigrid/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.387314 minigrid-2.2.1/minigrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-03-27 23:38:35.000000 minigrid-2.2.1/minigrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-03-27 23:38:35.000000 minigrid-2.2.1/minigrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 23:38:35.000000 minigrid-2.2.1/minigrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-27 23:38:35.000000 minigrid-2.2.1/minigrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-27 23:38:35.000000 minigrid-2.2.1/minigrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-27 23:38:35.000000 minigrid-2.2.1/minigrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-03-27 23:38:26.000000 minigrid-2.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 23:38:35.399314 minigrid-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-03-27 23:38:26.000000 minigrid-2.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 23:38:35.399314 minigrid-2.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10344 2023-03-27 23:38:26.000000 minigrid-2.2.1/tests/test_envs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-03-27 23:38:26.000000 minigrid-2.2.1/tests/test_obstructed_maze.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-03-27 23:38:26.000000 minigrid-2.2.1/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-03-27 23:38:26.000000 minigrid-2.2.1/tests/test_wrappers.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.070874 minigrid-2.3.0/
+-rw-r--r--   0 marktowers   (501) staff       (20)     2507 2023-02-14 13:49:06.000000 minigrid-2.3.0/LICENSE
+-rw-r--r--   0 marktowers   (501) staff       (20)     5813 2023-06-09 12:13:38.070607 minigrid-2.3.0/PKG-INFO
+-rw-r--r--   0 marktowers   (501) staff       (20)     4710 2023-06-09 10:02:36.000000 minigrid-2.3.0/README.md
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.046684 minigrid-2.3.0/minigrid/
+-rw-r--r--   0 marktowers   (501) staff       (20)    28823 2023-06-09 12:13:00.000000 minigrid-2.3.0/minigrid/__init__.py
+-rwxr-xr-x   0 marktowers   (501) staff       (20)     3430 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/benchmark.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.052598 minigrid-2.3.0/minigrid/core/
+-rw-r--r--   0 marktowers   (501) staff       (20)        0 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/core/__init__.py
+-rw-r--r--   0 marktowers   (501) staff       (20)      367 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/core/actions.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     1241 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/core/constants.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     9463 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/core/grid.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     8724 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/core/mission.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    13059 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/core/roomgrid.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     8423 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/core/world_object.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.062405 minigrid-2.3.0/minigrid/envs/
+-rw-r--r--   0 marktowers   (501) staff       (20)     1169 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/__init__.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.065897 minigrid-2.3.0/minigrid/envs/babyai/
+-rw-r--r--   0 marktowers   (501) staff       (20)      986 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/babyai/__init__.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.067432 minigrid-2.3.0/minigrid/envs/babyai/core/
+-rw-r--r--   0 marktowers   (501) staff       (20)        0 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/babyai/core/__init__.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     6440 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/babyai/core/levelgen.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     9601 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/babyai/core/roomgrid_level.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    16579 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/babyai/core/verifier.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    23748 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/goto.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    12188 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/open.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    11983 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/other.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    10540 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/pickup.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5858 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/putnext.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    14856 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/synth.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    13690 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/babyai/unlock.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3641 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/blockedunlockpickup.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     6256 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/crossing.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3606 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/distshift.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3356 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/doorkey.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5302 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/dynamicobstacles.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3475 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/empty.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5395 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/fetch.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3904 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/fourrooms.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     4819 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/gotodoor.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5161 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/gotoobject.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     4305 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/keycorridor.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     4051 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/lavagap.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5788 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/lockedroom.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     5487 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/memory.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     9182 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/multiroom.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     8750 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/envs/obstructedmaze.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3249 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/envs/obstructedmaze_v1.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     2891 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/envs/playground.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     6374 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/putnear.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     4149 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/redbluedoors.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     2728 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/unlock.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3188 2023-03-14 12:40:32.000000 minigrid-2.3.0/minigrid/envs/unlockpickup.py
+-rwxr-xr-x   0 marktowers   (501) staff       (20)     3756 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/manual_control.py
+-rwxr-xr-x   0 marktowers   (501) staff       (20)    23789 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/minigrid_env.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.068139 minigrid-2.3.0/minigrid/utils/
+-rw-r--r--   0 marktowers   (501) staff       (20)        0 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/utils/__init__.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     3049 2023-02-14 13:49:07.000000 minigrid-2.3.0/minigrid/utils/rendering.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    25300 2023-06-09 10:02:36.000000 minigrid-2.3.0/minigrid/wrappers.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.049411 minigrid-2.3.0/minigrid.egg-info/
+-rw-r--r--   0 marktowers   (501) staff       (20)     5813 2023-06-09 12:13:38.000000 minigrid-2.3.0/minigrid.egg-info/PKG-INFO
+-rw-r--r--   0 marktowers   (501) staff       (20)     1723 2023-06-09 12:13:38.000000 minigrid-2.3.0/minigrid.egg-info/SOURCES.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)        1 2023-06-09 12:13:38.000000 minigrid-2.3.0/minigrid.egg-info/dependency_links.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)       69 2023-06-09 12:13:38.000000 minigrid-2.3.0/minigrid.egg-info/entry_points.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)      107 2023-06-09 12:13:38.000000 minigrid-2.3.0/minigrid.egg-info/requires.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)        9 2023-06-09 12:13:38.000000 minigrid-2.3.0/minigrid.egg-info/top_level.txt
+-rw-r--r--   0 marktowers   (501) staff       (20)     2789 2023-06-09 12:11:20.000000 minigrid-2.3.0/pyproject.toml
+-rw-r--r--   0 marktowers   (501) staff       (20)       38 2023-06-09 12:13:38.070964 minigrid-2.3.0/setup.cfg
+-rw-r--r--   0 marktowers   (501) staff       (20)      976 2023-02-14 13:49:07.000000 minigrid-2.3.0/setup.py
+drwxr-xr-x   0 marktowers   (501) staff       (20)        0 2023-06-09 12:13:38.070167 minigrid-2.3.0/tests/
+-rw-r--r--   0 marktowers   (501) staff       (20)    10344 2023-02-14 13:49:07.000000 minigrid-2.3.0/tests/test_envs.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     2252 2023-06-09 10:02:36.000000 minigrid-2.3.0/tests/test_obstructed_maze.py
+-rw-r--r--   0 marktowers   (501) staff       (20)     1621 2023-06-09 10:02:36.000000 minigrid-2.3.0/tests/test_scripts.py
+-rw-r--r--   0 marktowers   (501) staff       (20)    10541 2023-06-09 10:02:36.000000 minigrid-2.3.0/tests/test_wrappers.py
```

### Comparing `minigrid-2.2.1/LICENSE` & `minigrid-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/PKG-INFO` & `minigrid-2.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minigrid
-Version: 2.2.1
+Version: 2.3.0
 Summary: Minimalistic gridworld reinforcement learning environments.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://minigrid.farama.org/
 Project-URL: Documentation, https://minigrid.farama.org/
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Minigrid/issues
@@ -12,17 +12,18 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Minigrid/master/minigrid-text.png" width="500px"/>
 </p>
@@ -32,15 +33,15 @@
 
 <p align="center">
   <img src="figures/door-key-curriculum.gif" width=200 alt="Figure Door Key Curriculum">
 </p>
 
 The Minigrid library contains a collection of discrete grid-world environments to conduct research on Reinforcement Learning. The environments follow the [Gymnasium]() standard API and they are designed to be lightweight, fast, and easily customizable. 
 
-The documentation website is at [minigrid.farama.org](https://minigrid.farama.org/), and we have a public discord server (which we also use to coordinate development work) that you can join here: [https://discord.gg/B8ZJ92hu](https://discord.gg/B8ZJ92hu)
+The documentation website is at [minigrid.farama.org](https://minigrid.farama.org/), and we have a public discord server (which we also use to coordinate development work) that you can join here: [https://discord.gg/bnJ6kubTg6](https://discord.gg/bnJ6kubTg6)
 
 Note that the library was previously known as gym-minigrid and it has been referenced in several publications. If your publication uses the Minigrid library and you wish for it to be included in the [list of publications](https://minigrid.farama.org/content/publications/), please create an issue in the [GitHub repository](https://github.com/Farama-Foundation/Minigrid/issues/new/choose).
 
 
 # Installation
 
 To install the Minigrid library use `pip install minigrid`.
```

### Comparing `minigrid-2.2.1/README.md` & `minigrid-2.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 <p align="center">
   <img src="figures/door-key-curriculum.gif" width=200 alt="Figure Door Key Curriculum">
 </p>
 
 The Minigrid library contains a collection of discrete grid-world environments to conduct research on Reinforcement Learning. The environments follow the [Gymnasium]() standard API and they are designed to be lightweight, fast, and easily customizable. 
 
-The documentation website is at [minigrid.farama.org](https://minigrid.farama.org/), and we have a public discord server (which we also use to coordinate development work) that you can join here: [https://discord.gg/B8ZJ92hu](https://discord.gg/B8ZJ92hu)
+The documentation website is at [minigrid.farama.org](https://minigrid.farama.org/), and we have a public discord server (which we also use to coordinate development work) that you can join here: [https://discord.gg/bnJ6kubTg6](https://discord.gg/bnJ6kubTg6)
 
 Note that the library was previously known as gym-minigrid and it has been referenced in several publications. If your publication uses the Minigrid library and you wish for it to be included in the [list of publications](https://minigrid.farama.org/content/publications/), please create an issue in the [GitHub repository](https://github.com/Farama-Foundation/Minigrid/issues/new/choose).
 
 
 # Installation
 
 To install the Minigrid library use `pip install minigrid`.
```

### Comparing `minigrid-2.2.1/minigrid/__init__.py` & `minigrid-2.3.0/minigrid/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from gymnasium.envs.registration import register
 
 from minigrid import minigrid_env, wrappers
 from minigrid.core import roomgrid
 from minigrid.core.world_object import Wall
 
-__version__ = "2.2.1"
+__version__ = "2.3.0"
 
 
 try:
     import sys
 
     from farama_notifications import notifications
```

### Comparing `minigrid-2.2.1/minigrid/benchmark.py` & `minigrid-2.3.0/minigrid/benchmark.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/core/constants.py` & `minigrid-2.3.0/minigrid/core/constants.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/core/grid.py` & `minigrid-2.3.0/minigrid/core/grid.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         from copy import deepcopy
 
         return deepcopy(self)
 
     def set(self, i: int, j: int, v: WorldObj | None):
         assert (
             0 <= i < self.width
-        ), f"column index {j} outside of grid of width {self.width}"
+        ), f"column index {i} outside of grid of width {self.width}"
         assert (
             0 <= j < self.height
         ), f"row index {j} outside of grid of height {self.height}"
         self.grid[j * self.width + i] = v
 
     def get(self, i: int, j: int) -> WorldObj | None:
         assert 0 <= i < self.width
```

### Comparing `minigrid-2.2.1/minigrid/core/mission.py` & `minigrid-2.3.0/minigrid/core/mission.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/core/roomgrid.py` & `minigrid-2.3.0/minigrid/core/roomgrid.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/core/world_object.py` & `minigrid-2.3.0/minigrid/core/world_object.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/__init__.py` & `minigrid-2.3.0/minigrid/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/__init__.py` & `minigrid-2.3.0/minigrid/envs/babyai/__init__.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/core/levelgen.py` & `minigrid-2.3.0/minigrid/envs/babyai/core/levelgen.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/core/roomgrid_level.py` & `minigrid-2.3.0/minigrid/envs/babyai/core/roomgrid_level.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/core/verifier.py` & `minigrid-2.3.0/minigrid/envs/babyai/core/verifier.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/goto.py` & `minigrid-2.3.0/minigrid/envs/babyai/goto.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/open.py` & `minigrid-2.3.0/minigrid/envs/babyai/open.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/other.py` & `minigrid-2.3.0/minigrid/envs/babyai/other.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/pickup.py` & `minigrid-2.3.0/minigrid/envs/babyai/pickup.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/putnext.py` & `minigrid-2.3.0/minigrid/envs/babyai/putnext.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/synth.py` & `minigrid-2.3.0/minigrid/envs/babyai/synth.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/babyai/unlock.py` & `minigrid-2.3.0/minigrid/envs/babyai/unlock.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/blockedunlockpickup.py` & `minigrid-2.3.0/minigrid/envs/blockedunlockpickup.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/crossing.py` & `minigrid-2.3.0/minigrid/envs/crossing.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/distshift.py` & `minigrid-2.3.0/minigrid/envs/distshift.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/doorkey.py` & `minigrid-2.3.0/minigrid/envs/doorkey.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/dynamicobstacles.py` & `minigrid-2.3.0/minigrid/envs/dynamicobstacles.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/empty.py` & `minigrid-2.3.0/minigrid/envs/empty.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/fetch.py` & `minigrid-2.3.0/minigrid/envs/fetch.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/fourrooms.py` & `minigrid-2.3.0/minigrid/envs/fourrooms.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/gotodoor.py` & `minigrid-2.3.0/minigrid/envs/gotodoor.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/gotoobject.py` & `minigrid-2.3.0/minigrid/envs/gotoobject.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/keycorridor.py` & `minigrid-2.3.0/minigrid/envs/keycorridor.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/lavagap.py` & `minigrid-2.3.0/minigrid/envs/lavagap.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/lockedroom.py` & `minigrid-2.3.0/minigrid/envs/lockedroom.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/memory.py` & `minigrid-2.3.0/minigrid/envs/memory.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/multiroom.py` & `minigrid-2.3.0/minigrid/envs/multiroom.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/obstructedmaze.py` & `minigrid-2.3.0/minigrid/envs/obstructedmaze.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/obstructedmaze_v1.py` & `minigrid-2.3.0/minigrid/envs/obstructedmaze_v1.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/playground.py` & `minigrid-2.3.0/minigrid/envs/playground.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/putnear.py` & `minigrid-2.3.0/minigrid/envs/putnear.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/redbluedoors.py` & `minigrid-2.3.0/minigrid/envs/redbluedoors.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/unlock.py` & `minigrid-2.3.0/minigrid/envs/unlock.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/envs/unlockpickup.py` & `minigrid-2.3.0/minigrid/envs/unlockpickup.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/manual_control.py` & `minigrid-2.3.0/minigrid/manual_control.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/minigrid_env.py` & `minigrid-2.3.0/minigrid/minigrid_env.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/utils/rendering.py` & `minigrid-2.3.0/minigrid/utils/rendering.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/minigrid/wrappers.py` & `minigrid-2.3.0/minigrid/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import operator
 from functools import reduce
 from typing import Any
 
 import gymnasium as gym
 import numpy as np
 from gymnasium import logger, spaces
-from gymnasium.core import ObservationWrapper, ObsType, Wrapper
+from gymnasium.core import ActionWrapper, ObservationWrapper, ObsType, Wrapper
 
 from minigrid.core.constants import COLOR_TO_IDX, OBJECT_TO_IDX, STATE_TO_IDX
 from minigrid.core.world_object import Goal
 
 
 class ReseedWrapper(Wrapper):
     """
@@ -448,23 +448,17 @@
 
         if word_dict is None:
             word_dict = self.get_minigrid_words()
 
         self.max_words_in_mission = max_words_in_mission
         self.word_dict = word_dict
 
-        image_observation_space = spaces.Box(
-            low=0,
-            high=255,
-            shape=(self.agent_view_size, self.agent_view_size, 3),
-            dtype="uint8",
-        )
         self.observation_space = spaces.Dict(
             {
-                "image": image_observation_space,
+                "image": env.observation_space["image"],
                 "direction": spaces.Discrete(4),
                 "mission": spaces.MultiDiscrete(
                     [len(self.word_dict.keys())] * max_words_in_mission
                 ),
             }
         )
 
@@ -766,7 +760,31 @@
 
         grid = np.concatenate([grid, _objects])
         grid = np.transpose(grid, (1, 2, 0))
         grid[agent_pos[0], agent_pos[1], 2] = OBJECT_TO_IDX["agent"]
         obs["image"] = grid
 
         return obs
+
+
+class StochasticActionWrapper(ActionWrapper):
+    """
+    Add stochasticity to the actions
+
+    If a random action is provided, it is returned with probability `1 - prob`.
+    Else, a random action is sampled from the action space.
+    """
+
+    def __init__(self, env=None, prob=0.9, random_action=None):
+        super().__init__(env)
+        self.prob = prob
+        self.random_action = random_action
+
+    def action(self, action):
+        """ """
+        if np.random.uniform() < self.prob:
+            return action
+        else:
+            if self.random_action is None:
+                return self.np_random.integers(0, high=6)
+            else:
+                return self.random_action
```

### Comparing `minigrid-2.2.1/minigrid.egg-info/PKG-INFO` & `minigrid-2.3.0/minigrid.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minigrid
-Version: 2.2.1
+Version: 2.3.0
 Summary: Minimalistic gridworld reinforcement learning environments.
 Author-email: Farama Foundation <contact@farama.org>
 License: MIT License
 Project-URL: Homepage, https://farama.org
 Project-URL: Repository, https://minigrid.farama.org/
 Project-URL: Documentation, https://minigrid.farama.org/
 Project-URL: Bug Report, https://github.com/Farama-Foundation/Minigrid/issues
@@ -12,17 +12,18 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: <3.11,>=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE
 
 <p align="center">
     <img src="https://raw.githubusercontent.com/Farama-Foundation/Minigrid/master/minigrid-text.png" width="500px"/>
 </p>
@@ -32,15 +33,15 @@
 
 <p align="center">
   <img src="figures/door-key-curriculum.gif" width=200 alt="Figure Door Key Curriculum">
 </p>
 
 The Minigrid library contains a collection of discrete grid-world environments to conduct research on Reinforcement Learning. The environments follow the [Gymnasium]() standard API and they are designed to be lightweight, fast, and easily customizable. 
 
-The documentation website is at [minigrid.farama.org](https://minigrid.farama.org/), and we have a public discord server (which we also use to coordinate development work) that you can join here: [https://discord.gg/B8ZJ92hu](https://discord.gg/B8ZJ92hu)
+The documentation website is at [minigrid.farama.org](https://minigrid.farama.org/), and we have a public discord server (which we also use to coordinate development work) that you can join here: [https://discord.gg/bnJ6kubTg6](https://discord.gg/bnJ6kubTg6)
 
 Note that the library was previously known as gym-minigrid and it has been referenced in several publications. If your publication uses the Minigrid library and you wish for it to be included in the [list of publications](https://minigrid.farama.org/content/publications/), please create an issue in the [GitHub repository](https://github.com/Farama-Foundation/Minigrid/issues/new/choose).
 
 
 # Installation
 
 To install the Minigrid library use `pip install minigrid`.
```

### Comparing `minigrid-2.2.1/minigrid.egg-info/SOURCES.txt` & `minigrid-2.3.0/minigrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/pyproject.toml` & `minigrid-2.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -4,33 +4,34 @@
 requires = ["setuptools >= 61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minigrid"
 description = "Minimalistic gridworld reinforcement learning environments."
 readme = "README.md"
-requires-python = ">= 3.7, < 3.11"
+requires-python = ">= 3.7"
 authors = [{ name = "Farama Foundation", email = "contact@farama.org" }]
 license = { text = "MIT License" }
 keywords = ["Memory, Environment, Agent, RL, Gymnasium"]
 classifiers = [
     "Development Status :: 4 - Beta",  # change to `5 - Production/Stable` when ready
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     'Intended Audience :: Science/Research',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
 ]
 dependencies = [
     "numpy>=1.18.0",
-    "gymnasium>=0.26",
-    "pygame>=2.2.0",
+    "gymnasium>=0.28.1",
+    "pygame>=2.4.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 testing = [
     "pytest>=7.0.1",
     "pytest-mock>=3.10.0",
```

### Comparing `minigrid-2.2.1/setup.py` & `minigrid-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/tests/test_envs.py` & `minigrid-2.3.0/tests/test_envs.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/tests/test_obstructed_maze.py` & `minigrid-2.3.0/tests/test_obstructed_maze.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/tests/test_scripts.py` & `minigrid-2.3.0/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `minigrid-2.2.1/tests/test_wrappers.py` & `minigrid-2.3.0/tests/test_wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     FullyObsWrapper,
     ImgObsWrapper,
     OneHotPartialObsWrapper,
     PositionBonus,
     ReseedWrapper,
     RGBImgObsWrapper,
     RGBImgPartialObsWrapper,
+    StochasticActionWrapper,
     SymbolicObsWrapper,
     ViewSizeWrapper,
 )
 from tests.utils import all_testing_env_specs, assert_equals, minigrid_testing_env_specs
 
 SEEDS = [100, 243, 500]
 NUM_STEPS = 100
@@ -323,7 +324,35 @@
         == np.array([agent_pos[0], agent_pos[1], OBJECT_TO_IDX["agent"]])
     )
     assert np.alltrue(
         obs["image"][goal_pos[0], goal_pos[1], :]
         == np.array([goal_pos[0], goal_pos[1], OBJECT_TO_IDX["goal"]])
     )
     env.close()
+
+
+@pytest.mark.parametrize("env_id", ["MiniGrid-Empty-16x16-v0"])
+def test_stochastic_action_wrapper(env_id):
+    env = gym.make(env_id)
+    env = StochasticActionWrapper(env, prob=0.2)
+    _, _ = env.reset()
+    for _ in range(20):
+        _, _, _, _, _ = env.step(0)
+    env.close()
+
+    env = gym.make(env_id)
+    env = StochasticActionWrapper(env, prob=0.2, random_action=1)
+    _, _ = env.reset()
+    for _ in range(20):
+        _, _, _, _, _ = env.step(0)
+    env.close()
+
+
+def test_dict_observation_space_doesnt_clash_with_one_hot():
+    env = gym.make("MiniGrid-Empty-5x5-v0")
+    env = OneHotPartialObsWrapper(env)
+    env = DictObservationSpaceWrapper(env)
+    env.reset()
+    obs, _, _, _, _ = env.step(0)
+    assert obs["image"].shape == (7, 7, 20)
+    assert env.observation_space["image"].shape == (7, 7, 20)
+    env.close()
```

