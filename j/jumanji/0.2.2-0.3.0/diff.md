# Comparing `tmp/jumanji-0.2.2.tar.gz` & `tmp/jumanji-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jumanji-0.2.2.tar", last modified: Fri Apr 14 16:56:59 2023, max compression
+gzip compressed data, was "jumanji-0.3.0.tar", last modified: Fri Jun  9 16:54:07 2023, max compression
```

## Comparing `jumanji-0.2.2.tar` & `jumanji-0.3.0.tar`

### file list

```diff
@@ -1,211 +1,295 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-14 16:56:47.000000 jumanji-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-14 16:56:47.000000 jumanji-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-14 16:56:59.213251 jumanji-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-04-14 16:56:47.000000 jumanji-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/commons/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/commons/maze_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_rendering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/commons/maze_utils/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/logic/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji/environments/logic/game_2048/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12383 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/game_2048/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.193250 jumanji-0.2.2/jumanji/environments/logic/minesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/done.py
--rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/minesweeper/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.193250 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.193250 jumanji-0.2.2/jumanji/environments/packing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/packing/bin_pack/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    31516 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/bin_pack/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/packing/job_shop/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/job_shop/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/packing/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/packing/knapsack/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.197250 jumanji-0.2.2/jumanji/environments/routing/cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cleaner/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    16078 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8083 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/connector/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/cvrp/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/maze/
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13670 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/maze/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.201250 jumanji-0.2.2/jumanji/environments/routing/snake/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19278 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/snake/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/snake/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/environments/routing/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11435 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/reward.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/environments/routing/tsp/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/specs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/env_not_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/testing/pytrees.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/agents/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/agents/a2c/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/a2c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/a2c/a2c_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.205250 jumanji-0.2.2/jumanji/training/agents/random/
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/agents/random/random_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7953 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/bin_pack/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/bin_pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/bin_pack/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/bin_pack/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/cleaner/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cleaner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cleaner/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cleaner/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/connector/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/connector/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/cvrp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cvrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cvrp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/cvrp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/game_2048/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/game_2048/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/game_2048/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/game_2048/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.209251 jumanji-0.2.2/jumanji/training/networks/job_shop/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/job_shop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/job_shop/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/job_shop/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/knapsack/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/knapsack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/knapsack/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/knapsack/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/masked_categorical_random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/maze/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/maze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/maze/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/maze/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/minesweeper/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/minesweeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/minesweeper/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/minesweeper/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/parametric_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/protocols.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/rubiks_cube/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/snake/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/snake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/snake/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/snake/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/transformer_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/jumanji/training/networks/tsp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/tsp/actor_critic.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/networks/tsp/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    13745 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/setup_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/training/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/tree_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/viewer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25676 2023-04-14 16:56:47.000000 jumanji-0.2.2/jumanji/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.189249 jumanji-0.2.2/jumanji.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15654 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-14 16:56:59.000000 jumanji-0.2.2/jumanji.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-14 16:56:47.000000 jumanji-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:56:59.213251 jumanji-0.2.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-14 16:56:47.000000 jumanji-0.2.2/requirements/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-14 16:56:47.000000 jumanji-0.2.2/requirements/requirements-train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-14 16:56:47.000000 jumanji-0.2.2/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-14 16:56:59.217251 jumanji-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-14 16:56:47.000000 jumanji-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.481079 jumanji-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-06-09 16:53:56.000000 jumanji-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 16:53:56.000000 jumanji-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-06-09 16:54:07.481079 jumanji-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-06-09 16:53:56.000000 jumanji-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.433078 jumanji-0.3.0/jumanji/
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/commons/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/commons/maze_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8106 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5594 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_rendering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/commons/maze_utils/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/logic/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji/environments/logic/game_2048/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12404 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8300 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/game_2048/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.441078 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/graph_coloring/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.441078 jumanji-0.3.0/jumanji/environments/logic/minesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/done.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11768 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/minesweeper/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.441078 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/logic/sudoku/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   810128 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/10000_mixed_puzzles.npy
+-rw-r--r--   0 runner    (1001) docker     (123)    81128 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/1000_very_easy_puzzles.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7095 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/logic/sudoku/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/packing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.445078 jumanji-0.3.0/jumanji/environments/packing/bin_pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30996 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31516 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10044 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/bin_pack/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.449079 jumanji-0.3.0/jumanji/environments/packing/job_shop/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24068 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7376 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/job_shop/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.449079 jumanji-0.3.0/jumanji/environments/packing/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1780 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/knapsack/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/packing/tetris/
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14175 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12469 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/packing/tetris/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15120 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cleaner/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14491 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22636 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/connector/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.453079 jumanji-0.3.0/jumanji/environments/routing/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14532 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8505 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/cvrp/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.457079 jumanji-0.3.0/jumanji/environments/routing/maze/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12892 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/maze/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.457079 jumanji-0.3.0/jumanji/environments/routing/mmst/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24530 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11708 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/mmst/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.457079 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17123 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7089 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9929 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9209 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/multi_cvrp/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.461079 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19997 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11126 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_shelf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/utils_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/robot_warehouse/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.461079 jumanji-0.3.0/jumanji/environments/routing/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14788 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7370 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/snake/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.461079 jumanji-0.3.0/jumanji/environments/routing/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/reward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/environments/routing/tsp/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4776 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21752 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/specs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/env_not_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/testing/pytrees.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/agents/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/agents/a2c/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/a2c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9577 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/a2c/a2c_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.465079 jumanji-0.3.0/jumanji/training/agents/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/agents/random/random_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5694 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/bin_pack/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/bin_pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9478 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/bin_pack/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/bin_pack/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/cleaner/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cleaner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cleaner/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cleaner/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/connector/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/connector/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.469079 jumanji-0.3.0/jumanji/training/networks/cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9701 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cvrp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/cvrp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/distribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/game_2048/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/game_2048/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/game_2048/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/game_2048/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/graph_coloring/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/graph_coloring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11309 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/graph_coloring/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/graph_coloring/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/job_shop/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/job_shop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/job_shop/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/job_shop/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/knapsack/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/knapsack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8666 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/knapsack/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/knapsack/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/masked_categorical_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/maze/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/maze/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/maze/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/maze/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/minesweeper/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/minesweeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4499 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/minesweeper/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/minesweeper/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.473079 jumanji-0.3.0/jumanji/training/networks/mmst/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/mmst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11209 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/mmst/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/mmst/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/multi_cvrp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7123 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/parametric_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/protocols.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/robot_warehouse/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/rubiks_cube/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/snake/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/snake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/snake/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/snake/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/sudoku/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/sudoku/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/sudoku/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/sudoku/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.477079 jumanji-0.3.0/jumanji/training/networks/tetris/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tetris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tetris/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tetris/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/transformer_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.481079 jumanji-0.3.0/jumanji/training/networks/tsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9602 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tsp/actor_critic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/networks/tsp/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18340 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/setup_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/training/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/tree_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/viewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25577 2023-06-09 16:53:56.000000 jumanji-0.3.0/jumanji/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.437078 jumanji-0.3.0/jumanji.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18237 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 16:54:07.000000 jumanji-0.3.0/jumanji.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-09 16:53:56.000000 jumanji-0.3.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 16:54:07.481079 jumanji-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-09 16:53:56.000000 jumanji-0.3.0/requirements/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-06-09 16:53:56.000000 jumanji-0.3.0/requirements/requirements-train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 16:53:56.000000 jumanji-0.3.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-09 16:54:07.481079 jumanji-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-06-09 16:53:56.000000 jumanji-0.3.0/setup.py
```

### Comparing `jumanji-0.2.2/LICENSE` & `jumanji-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/PKG-INFO` & `jumanji-0.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,72 +1,60 @@
-Metadata-Version: 2.1
-Name: jumanji
-Version: 0.2.2
-Summary: A suite of diverse and challenging RL environments in JAX
-Home-page: https://github.com/instadeepai/jumanji/
-Author: InstaDeep
-Author-email: hello@instadeep.com
-License: Apache 2.0
-Keywords: reinforcement-learning python jax
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: train
-License-File: LICENSE
-
 <p align="center">
     <a href="docs/img/jumanji_logo.png">
         <img src="docs/img/jumanji_logo.png" alt="Jumanji logo" width="50%"/>
     </a>
 </p>
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/)
 [![PyPI Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/jumanji)
 [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/workflows/tests_linters.yml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![MyPy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-F8D521)](https://huggingface.co/InstaDeepAI)
 
 [**Environments**](#environments-)
 | [**Installation**](#installation-)
 | [**Quickstart**](#quickstart-)
 | [**Training**](#training-%EF%B8%8F)
 | [**Citation**](#citing-jumanji-%EF%B8%8F)
 | [**Docs**](https://instadeepai.github.io/jumanji)
 ---
 
-
-<p float="left" align="center">
-  <img src="docs/env_anim/connector.gif" alt="Connector" width="30%" />
-  <img src="docs/env_anim/snake.gif" alt="Snake" width="30%" />
-  <img src="docs/env_anim/cleaner.gif" alt="Cleaner" width="30%" />
-  <img src="docs/env_anim/job_shop.gif" alt="JobShop" width="30%" />
-  <img src="docs/env_anim/bin_pack.gif" alt="BinPack" width="30%" />
-  <img src="docs/env_anim/cvrp.gif" alt="CVRP" width="30%" />
-  <img src="docs/env_anim/rubiks_cube.gif" alt="RubiksCube" width="30%" />
-  <img src="docs/env_anim/game_2048.gif" alt="Game2048" width="30%" />
-  <img src="docs/env_anim/minesweeper.gif" alt="Minesweeper" width="30%" />
-</p>
-
+<div class="collage">
+  <div class="row" align="center">
+    <img src="docs/env_anim/bin_pack.gif" alt="BinPack" width="16%">
+    <img src="docs/env_anim/cleaner.gif" alt="Cleaner" width="16%">
+    <img src="docs/env_anim/connector.gif" alt="Connector" width="16%">
+    <img src="docs/env_anim/cvrp.gif" alt="CVRP" width="16%">
+    <img src="docs/env_anim/game_2048.gif" alt="Game2048" width="16%">
+    <img src="docs/env_anim/graph_coloring.gif" alt="GraphColoring" width="16%">
+  </div>
+  <div class="row" align="center">
+    <img src="docs/env_anim/job_shop.gif" alt="JobShop" width="16%">
+    <img src="docs/env_anim/knapsack.gif" alt="Knapsack" width="16%">
+    <img src="docs/env_anim/maze.gif" alt="Maze" width="16%">
+    <img src="docs/env_anim/minesweeper.gif" alt="Minesweeper" width="16%">
+    <img src="docs/env_anim/mmst.gif" alt="MMST" width="16%">
+    <img src="docs/env_anim/multi_cvrp.gif" alt="MultiCVRP" width="16%">
+  </div>
+  <div class="row" align="center">
+    <img src="docs/env_anim/robot_warehouse.gif" alt="RobotWarehouse" width="16%">
+    <img src="docs/env_anim/rubiks_cube.gif" alt="RubiksCube" width="16%">
+    <img src="docs/env_anim/snake.gif" alt="Snake" width="16%">
+    <img src="docs/env_anim/sudoku.gif" alt="Sudoku" width="16%">
+    <img src="docs/env_anim/tetris.gif" alt="Tetris" width="16%">
+    <img src="docs/env_anim/tsp.gif" alt="Tetris" width="16%">
+  </div>
+</div>
 
 
 ## Welcome to the Jungle! 🌴
 
-Jumanji is a suite of diverse and challenging reinforcement learning (RL) environments written in
-JAX.
+Jumanji is a diverse suite of scalable reinforcement learning environments written in JAX.
 
 Jumanji is helping pioneer a new wave of hardware-accelerated research and development in the
 field of RL. Jumanji's high-speed environments enable faster iteration and large-scale
 experimentation while simultaneously reducing complexity. Originating in the Research Team at
 [InstaDeep](https://www.instadeep.com/), Jumanji is now developed jointly with the open-source
 community. To join us in these efforts, reach out, raise issues and read our
 [contribution guidelines](https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just
@@ -91,58 +79,65 @@
 [RLlib](https://docs.ray.io/en/latest/rllib/index.html), [OpenAI Gym](https://github.com/openai/gym)
 and [DeepMind-Env](https://github.com/deepmind/dm_env) through our `dm_env` and `gym` wrappers.
 - 🎓 **Examples**: guides to facilitate Jumanji's adoption and highlight the added value of
 JAX-based environments.
 - 🏎️ **Training:** example agents that can be used as inspiration for the agents one may implement
 in their research.
 
-
 ## Environments 🌍
 
 Jumanji provides a diverse range of environments ranging from simple games to NP-hard combinatorial
 problems.
 
 | Environment                              | Category | Registered Version(s)                                | Source                                                                                           | Description                                                            |
 |------------------------------------------|----------|------------------------------------------------------|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
-| 🔢 Game2048                              | Logic  | `Game2048-v0`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/)   | [doc](https://instadeepai.github.io/jumanji/environments/game_2048/)   |
+| 🔢 Game2048                              | Logic  | `Game2048-v1`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/)   | [doc](https://instadeepai.github.io/jumanji/environments/game_2048/)   |
+| 🎨 GraphColoring                              | Logic  | `GraphColoring-v0`                                   | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/graph_coloring/)   | [doc](https://instadeepai.github.io/jumanji/environments/graph_coloring/)   |
 | 💣 Minesweeper                           | Logic    | `Minesweeper-v0`                                     | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc](https://instadeepai.github.io/jumanji/environments/minesweeper/) |
 | 🎲 RubiksCube                            | Logic    | `RubiksCube-v0`<br/>`RubiksCube-partly-scrambled-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/rubiks_cube/) | [doc](https://instadeepai.github.io/jumanji/environments/rubiks_cube/) |
-| 📦 BinPack (3D BinPacking Problem)       | Packing  | `BinPack-v1`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/)  | [doc](https://instadeepai.github.io/jumanji/environments/bin_pack/)    |
+| ✏️ Sudoku                       | Logic    | `Sudoku-v0` <br/>`Sudoku-very-easy-v0`               | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/sudoku/) | [doc](https://instadeepai.github.io/jumanji/environments/sudoku/) |
+| 📦 BinPack (3D BinPacking Problem)       | Packing  | `BinPack-v2`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/)  | [doc](https://instadeepai.github.io/jumanji/environments/bin_pack/)    |
 | 🏭 JobShop (Job Shop Scheduling Problem) | Packing  | `JobShop-v0`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/)  | [doc](https://instadeepai.github.io/jumanji/environments/job_shop/)    |
 | 🎒 Knapsack                              | Packing  | `Knapsack-v1`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/knapsack/)  | [doc](https://instadeepai.github.io/jumanji/environments/knapsack/)    |
+| ▒ Tetris                              | Packing  | `Tetris-v0`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/tetris/)  | [doc](https://instadeepai.github.io/jumanji/environments/tetris/)    |
 | 🧹 Cleaner                               | Routing  | `Cleaner-v0`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cleaner/)   | [doc](https://instadeepai.github.io/jumanji/environments/cleaner/)     |
-| :link: Connector                         | Routing  | `Connector-v0`                                       | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/connector/) | [doc](https://instadeepai.github.io/jumanji/environments/connector/)   |
+| :link: Connector                         | Routing  | `Connector-v2`                                       | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/connector/) | [doc](https://instadeepai.github.io/jumanji/environments/connector/)   |
 | 🚚 CVRP (Capacitated Vehicle Routing Problem)  | Routing  | `CVRP-v1`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cvrp/)      | [doc](https://instadeepai.github.io/jumanji/environments/cvrp/)        |
+| 🚚 MultiCVRP (Multi-Agent Capacitated Vehicle Routing Problem)  | Routing  | `MultiCVRP-v0`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/multi_cvrp/)      | [doc](https://instadeepai.github.io/jumanji/environments/multi_cvrp/)        |
 | :mag: Maze   | Routing  | `Maze-v0`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/maze/)      | [doc](https://instadeepai.github.io/jumanji/environments/maze/)        |
+| :robot: RobotWarehouse  | Routing  | `RobotWarehouse-v0`                                  | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/robot_warehouse/)      | [doc](https://instadeepai.github.io/jumanji/environments/robot_warehouse/)        |
 | 🐍 Snake                                       | Routing  | `Snake-v1`                                           | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/snake/)     | [doc](https://instadeepai.github.io/jumanji/environments/snake/)       |
 | 📬 TSP (Travelling Salesman Problem)           | Routing  | `TSP-v1`                                             | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/tsp/)       | [doc](https://instadeepai.github.io/jumanji/environments/tsp/)         |
-
+| Multi Minimum Spanning Tree Problem | Routing  | `MMST-v0`                                | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/mmst)    | [doc](https://instadeepai.github.io/jumanji/environments/mmst/)    |
 
 ## Installation 🎬
 
 You can install the latest release of Jumanji from PyPI:
+
 ```bash
 pip install jumanji
 ```
+
 Alternatively, you can install the latest development version directly from GitHub:
+
 ```bash
 pip install git+https://github.com/instadeepai/jumanji.git
 ```
+
 Jumanji has been tested on Python 3.8 and 3.9.
 Note that because the installation of JAX differs depending on your hardware accelerator,
 we advise users to explicitly install the correct JAX version (see the
 [official installation guide](https://github.com/google/jax#installation)).
 
 **Rendering:** Matplotlib is used for rendering all the environments. To visualize the environments
 you will need a GUI backend. For example, on Linux, you can install Tk via:
 `apt-get install python3-tk`, or using conda: `conda install tk`. Check out
 [Matplotlib backends](https://matplotlib.org/stable/users/explain/backends.html) for a list of
 backends you can use.
 
-
 ## Quickstart ⚡
 
 RL practitioners will find Jumanji's interface familiar as it combines the widely adopted
 [OpenAI Gym](https://github.com/openai/gym) and
 [DeepMind Environment](https://github.com/deepmind/dm_env) interfaces. From OpenAI Gym, we adopted
 the idea of a `registry` and the `render` method, while our `TimeStep` structure is inspired by
 DeepMind Environment.
@@ -191,15 +186,14 @@
 We maintain a registry of standard environments with their configuration.
 For each environment, a version suffix is appended, e.g. `Snake-v1`.
 When changes are made to environments that might impact learning results,
 the version number is incremented by one to prevent potential confusion.
 For a full list of registered versions of each environment, check out
 [the documentation](https://instadeepai.github.io/jumanji/environments/tsp/).
 
-
 ## Training 🏎️
 
 To showcase how to train RL agents on Jumanji environments, we provide a random agent and a vanilla
 actor-critic (A2C) agent. These agents can be found in
 [jumanji/training/](https://github.com/instadeepai/jumanji/tree/main/jumanji/training/).
 
 Because the environment framework in Jumanji is so flexible, it allows pretty much any problem to
@@ -212,40 +206,38 @@
 > ⚠️ The example agents in `jumanji/training` are **only** meant to serve as inspiration for how one
 > can implement an agent. Jumanji is first and foremost a library of environments - as such, the
 > agents and networks will **not** be maintained to a production standard.
 
 For more information on how to use the example agents, see the
 [training guide](https://instadeepai.github.io/jumanji/guides/training/).
 
-
 ## Contributing 🤝
 
 Contributions are welcome! See our issue tracker for
 [good first issues](https://github.com/instadeepai/jumanji/labels/good%20first%20issue). Please read
 our [contributing guidelines](https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) for
 details on how to submit pull requests, our Contributor License Agreement, and community guidelines.
 
-
 ## Citing Jumanji ✏️
 
 If you use Jumanji in your work, please cite the library using:
+
 ```
 @software{jumanji2023github,
   author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
         and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
         Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
         and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
   title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
   url = {https://github.com/instadeepai/jumanji},
   version = {0.2.2},
   year = {2023},
 }
 ```
 
-
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
 
 - 🤖 [Qdax](https://github.com/adaptive-intelligent-robotics/QDax) is a library to accelerate
 Quality-Diversity and neuro-evolution algorithms through hardware accelerators and parallelization.
```

#### html2text {}

```diff
@@ -1,49 +1,39 @@
-Metadata-Version: 2.1 Name: jumanji Version: 0.2.2 Summary: A suite of diverse
-and challenging RL environments in JAX Home-page: https://github.com/
-instadeepai/jumanji/ Author: InstaDeep Author-email: hello@instadeep.com
-License: Apache 2.0 Keywords: reinforcement-learning python jax Classifier:
-Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
-Intended Audience :: Science/Research Classifier: Intended Audience ::
-Developers Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev Provides-Extra: train License-File: LICENSE
                                 [Jumanji_logo]
 [![Python Versions](https://img.shields.io/pypi/pyversions/
 jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/) [![PyPI
 Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/
 jumanji) [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/
 tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/
 workflows/tests_linters.yml) [![Code Style](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) [![MyPy](http://
 www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License]
 (https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://
-opensource.org/licenses/Apache-2.0) [**Environments**](#environments-) |
-[**Installation**](#installation-) | [**Quickstart**](#quickstart-) |
-[**Training**](#training-%EF%B8%8F) | [**Citation**](#citing-jumanji-%EF%B8%8F)
-| [**Docs**](https://instadeepai.github.io/jumanji) ---
-    [Connector] [Snake] [Cleaner] [JobShop] [BinPack] [CVRP] [RubiksCube]
-                           [Game2048] [Minesweeper]
-## Welcome to the Jungle! ð´ Jumanji is a suite of diverse and challenging
-reinforcement learning (RL) environments written in JAX. Jumanji is helping
-pioneer a new wave of hardware-accelerated research and development in the
-field of RL. Jumanji's high-speed environments enable faster iteration and
-large-scale experimentation while simultaneously reducing complexity.
-Originating in the Research Team at [InstaDeep](https://www.instadeep.com/),
-Jumanji is now developed jointly with the open-source community. To join us in
-these efforts, reach out, raise issues and read our [contribution guidelines]
-(https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just
-[star](https://github.com/instadeepai/jumanji) ð to stay up to date with the
-latest developments! ### Goals ð 1. Provide a simple, well-tested API for
-JAX-based environments. 2. Make research in RL more accessible. 3. Facilitate
-the research on RL for problems in the industry and help close the gap between
+opensource.org/licenses/Apache-2.0) [![Hugging Face](https://img.shields.io/
+badge/%F0%9F%A4%97-Hugging%20Face-F8D521)](https://huggingface.co/InstaDeepAI)
+[**Environments**](#environments-) | [**Installation**](#installation-) |
+[**Quickstart**](#quickstart-) | [**Training**](#training-%EF%B8%8F) |
+[**Citation**](#citing-jumanji-%EF%B8%8F) | [**Docs**](https://
+instadeepai.github.io/jumanji) ---
+       [BinPack] [Cleaner] [Connector] [CVRP] [Game2048] [GraphColoring]
+         [JobShop] [Knapsack] [Maze] [Minesweeper] [MMST] [MultiCVRP]
+       [RobotWarehouse] [RubiksCube] [Snake] [Sudoku] [Tetris] [Tetris]
+## Welcome to the Jungle! ð´ Jumanji is a diverse suite of scalable
+reinforcement learning environments written in JAX. Jumanji is helping pioneer
+a new wave of hardware-accelerated research and development in the field of RL.
+Jumanji's high-speed environments enable faster iteration and large-scale
+experimentation while simultaneously reducing complexity. Originating in the
+Research Team at [InstaDeep](https://www.instadeep.com/), Jumanji is now
+developed jointly with the open-source community. To join us in these efforts,
+reach out, raise issues and read our [contribution guidelines](https://
+github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just [star](https:
+//github.com/instadeepai/jumanji) ð to stay up to date with the latest
+developments! ### Goals ð 1. Provide a simple, well-tested API for JAX-based
+environments. 2. Make research in RL more accessible. 3. Facilitate the
+research on RL for problems in the industry and help close the gap between
 research and industrial applications. 4. Provide environments whose difficulty
 can be scaled to be arbitrarily hard. ### Overview ð¦ - ð¥ **Environment
 API**: core abstractions for JAX-based environments. - ð¹ï¸ **Environment
 Suite**: a collection of RL environments ranging from simple games to NP-hard
 combinatorial problems. - ð¬ **Wrappers**: easily connect to your favourite
 RL frameworks and libraries such as [Acme](https://github.com/deepmind/acme),
 [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3), [RLlib]
@@ -55,67 +45,86 @@
 inspiration for the agents one may implement in their research. ## Environments
 ð Jumanji provides a diverse range of environments ranging from simple games
 to NP-hard combinatorial problems. | Environment | Category | Registered
 Version(s) | Source | Description | |------------------------------------------
 |----------|------------------------------------------------------|------------
 -------------------------------------------------------------------------------
 -------|-----------------------------------------------------------------------
--| | ð¢ Game2048 | Logic | `Game2048-v0` | [code](https://github.com/
+-| | ð¢ Game2048 | Logic | `Game2048-v1` | [code](https://github.com/
 instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/game_2048/) | | ð£
-Minesweeper | Logic | `Minesweeper-v0` | [code](https://github.com/instadeepai/
-jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc](https://
-instadeepai.github.io/jumanji/environments/minesweeper/) | | ð² RubiksCube |
-Logic | `RubiksCube-v0`
+(https://instadeepai.github.io/jumanji/environments/game_2048/) | | ð¨
+GraphColoring | Logic | `GraphColoring-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/logic/graph_coloring/) |
+[doc](https://instadeepai.github.io/jumanji/environments/graph_coloring/) | |
+ð£ Minesweeper | Logic | `Minesweeper-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc]
+(https://instadeepai.github.io/jumanji/environments/minesweeper/) | | ð²
+RubiksCube | Logic | `RubiksCube-v0`
 `RubiksCube-partly-scrambled-v0` | [code](https://github.com/instadeepai/
 jumanji/tree/main/jumanji/environments/logic/rubiks_cube/) | [doc](https://
-instadeepai.github.io/jumanji/environments/rubiks_cube/) | | ð¦ BinPack (3D
-BinPacking Problem) | Packing | `BinPack-v1` | [code](https://github.com/
-instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/bin_pack/) | | ð­ JobShop
-(Job Shop Scheduling Problem) | Packing | `JobShop-v0` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/
-) | [doc](https://instadeepai.github.io/jumanji/environments/job_shop/) | |
-ð Knapsack | Packing | `Knapsack-v1` | [code](https://github.com/
-instadeepai/jumanji/tree/main/jumanji/environments/packing/knapsack/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/knapsack/) | | ð§¹ Cleaner
-| Routing | `Cleaner-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/cleaner/) | [doc](https://
-instadeepai.github.io/jumanji/environments/cleaner/) | | :link: Connector |
-Routing | `Connector-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/connector/) | [doc](https://
-instadeepai.github.io/jumanji/environments/connector/) | | ð CVRP
-(Capacitated Vehicle Routing Problem) | Routing | `CVRP-v1` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cvrp/) |
-[doc](https://instadeepai.github.io/jumanji/environments/cvrp/) | | :mag: Maze
-| Routing | `Maze-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/maze/) | [doc](https://instadeepai.github.io/
-jumanji/environments/maze/) | | ð Snake | Routing | `Snake-v1` | [code]
-(https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/
-snake/) | [doc](https://instadeepai.github.io/jumanji/environments/snake/) | |
-ð¬ TSP (Travelling Salesman Problem) | Routing | `TSP-v1` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/tsp/) |
-[doc](https://instadeepai.github.io/jumanji/environments/tsp/) | ##
-Installation ð¬ You can install the latest release of Jumanji from PyPI:
-```bash pip install jumanji ``` Alternatively, you can install the latest
-development version directly from GitHub: ```bash pip install git+https://
-github.com/instadeepai/jumanji.git ``` Jumanji has been tested on Python 3.8
-and 3.9. Note that because the installation of JAX differs depending on your
-hardware accelerator, we advise users to explicitly install the correct JAX
-version (see the [official installation guide](https://github.com/google/
-jax#installation)). **Rendering:** Matplotlib is used for rendering all the
-environments. To visualize the environments you will need a GUI backend. For
-example, on Linux, you can install Tk via: `apt-get install python3-tk`, or
-using conda: `conda install tk`. Check out [Matplotlib backends](https://
-matplotlib.org/stable/users/explain/backends.html) for a list of backends you
-can use. ## Quickstart â¡ RL practitioners will find Jumanji's interface
-familiar as it combines the widely adopted [OpenAI Gym](https://github.com/
-openai/gym) and [DeepMind Environment](https://github.com/deepmind/dm_env)
-interfaces. From OpenAI Gym, we adopted the idea of a `registry` and the
-`render` method, while our `TimeStep` structure is inspired by DeepMind
+instadeepai.github.io/jumanji/environments/rubiks_cube/) | | âï¸ Sudoku |
+Logic | `Sudoku-v0`
+`Sudoku-very-easy-v0` | [code](https://github.com/instadeepai/jumanji/tree/
+main/jumanji/environments/logic/sudoku/) | [doc](https://instadeepai.github.io/
+jumanji/environments/sudoku/) | | ð¦ BinPack (3D BinPacking Problem) |
+Packing | `BinPack-v2` | [code](https://github.com/instadeepai/jumanji/tree/
+main/jumanji/environments/packing/bin_pack/) | [doc](https://
+instadeepai.github.io/jumanji/environments/bin_pack/) | | ð­ JobShop (Job
+Shop Scheduling Problem) | Packing | `JobShop-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/) | [doc]
+(https://instadeepai.github.io/jumanji/environments/job_shop/) | | ð
+Knapsack | Packing | `Knapsack-v1` | [code](https://github.com/instadeepai/
+jumanji/tree/main/jumanji/environments/packing/knapsack/) | [doc](https://
+instadeepai.github.io/jumanji/environments/knapsack/) | | â Tetris | Packing
+| `Tetris-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/packing/tetris/) | [doc](https://instadeepai.github.io/
+jumanji/environments/tetris/) | | ð§¹ Cleaner | Routing | `Cleaner-v0` |
+[code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/
+routing/cleaner/) | [doc](https://instadeepai.github.io/jumanji/environments/
+cleaner/) | | :link: Connector | Routing | `Connector-v2` | [code](https://
+github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/
+connector/) | [doc](https://instadeepai.github.io/jumanji/environments/
+connector/) | | ð CVRP (Capacitated Vehicle Routing Problem) | Routing |
+`CVRP-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/
+environments/routing/cvrp/) | [doc](https://instadeepai.github.io/jumanji/
+environments/cvrp/) | | ð MultiCVRP (Multi-Agent Capacitated Vehicle Routing
+Problem) | Routing | `MultiCVRP-v0` | [code](https://github.com/instadeepai/
+jumanji/tree/main/jumanji/environments/routing/multi_cvrp/) | [doc](https://
+instadeepai.github.io/jumanji/environments/multi_cvrp/) | | :mag: Maze |
+Routing | `Maze-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/maze/) | [doc](https://instadeepai.github.io/
+jumanji/environments/maze/) | | :robot: RobotWarehouse | Routing |
+`RobotWarehouse-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/robot_warehouse/) | [doc](https://
+instadeepai.github.io/jumanji/environments/robot_warehouse/) | | ð Snake |
+Routing | `Snake-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/snake/) | [doc](https://instadeepai.github.io/
+jumanji/environments/snake/) | | ð¬ TSP (Travelling Salesman Problem) |
+Routing | `TSP-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/tsp/) | [doc](https://instadeepai.github.io/
+jumanji/environments/tsp/) | | Multi Minimum Spanning Tree Problem | Routing |
+`MMST-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/
+environments/routing/mmst) | [doc](https://instadeepai.github.io/jumanji/
+environments/mmst/) | ## Installation ð¬ You can install the latest release
+of Jumanji from PyPI: ```bash pip install jumanji ``` Alternatively, you can
+install the latest development version directly from GitHub: ```bash pip
+install git+https://github.com/instadeepai/jumanji.git ``` Jumanji has been
+tested on Python 3.8 and 3.9. Note that because the installation of JAX differs
+depending on your hardware accelerator, we advise users to explicitly install
+the correct JAX version (see the [official installation guide](https://
+github.com/google/jax#installation)). **Rendering:** Matplotlib is used for
+rendering all the environments. To visualize the environments you will need a
+GUI backend. For example, on Linux, you can install Tk via: `apt-get install
+python3-tk`, or using conda: `conda install tk`. Check out [Matplotlib
+backends](https://matplotlib.org/stable/users/explain/backends.html) for a list
+of backends you can use. ## Quickstart â¡ RL practitioners will find Jumanji's
+interface familiar as it combines the widely adopted [OpenAI Gym](https://
+github.com/openai/gym) and [DeepMind Environment](https://github.com/deepmind/
+dm_env) interfaces. From OpenAI Gym, we adopted the idea of a `registry` and
+the `render` method, while our `TimeStep` structure is inspired by DeepMind
 Environment. ### Basic Usage ð§âð» ```python import jax import jumanji #
 Instantiate a Jumanji environment using the registry env = jumanji.make('Snake-
 v1') # Reset your (jit-able) environment key = jax.random.PRNGKey(0) state,
 timestep = jax.jit(env.reset)(key) # (Optional) Render the env state env.render
 (state) # Interact with the (jit-able) environment action = env.action_spec
 ().generate_value() # Action selection (dummy value here) state, timestep =
 jax.jit(env.step)(state, action) # Take a step and observe the next state and
```

### Comparing `jumanji-0.2.2/README.md` & `jumanji-0.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,85 @@
+Metadata-Version: 2.1
+Name: jumanji
+Version: 0.3.0
+Summary: A diverse suite of scalable reinforcement learning environments in JAX
+Home-page: https://github.com/instadeepai/jumanji/
+Author: InstaDeep
+Author-email: c.bonnet@instadeep.com
+License: Apache 2.0
+Keywords: reinforcement-learning python jax
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+Provides-Extra: train
+License-File: LICENSE
+
 <p align="center">
     <a href="docs/img/jumanji_logo.png">
         <img src="docs/img/jumanji_logo.png" alt="Jumanji logo" width="50%"/>
     </a>
 </p>
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/)
 [![PyPI Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/jumanji)
 [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/workflows/tests_linters.yml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![MyPy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-F8D521)](https://huggingface.co/InstaDeepAI)
 
 [**Environments**](#environments-)
 | [**Installation**](#installation-)
 | [**Quickstart**](#quickstart-)
 | [**Training**](#training-%EF%B8%8F)
 | [**Citation**](#citing-jumanji-%EF%B8%8F)
 | [**Docs**](https://instadeepai.github.io/jumanji)
 ---
 
-
-<p float="left" align="center">
-  <img src="docs/env_anim/connector.gif" alt="Connector" width="30%" />
-  <img src="docs/env_anim/snake.gif" alt="Snake" width="30%" />
-  <img src="docs/env_anim/cleaner.gif" alt="Cleaner" width="30%" />
-  <img src="docs/env_anim/job_shop.gif" alt="JobShop" width="30%" />
-  <img src="docs/env_anim/bin_pack.gif" alt="BinPack" width="30%" />
-  <img src="docs/env_anim/cvrp.gif" alt="CVRP" width="30%" />
-  <img src="docs/env_anim/rubiks_cube.gif" alt="RubiksCube" width="30%" />
-  <img src="docs/env_anim/game_2048.gif" alt="Game2048" width="30%" />
-  <img src="docs/env_anim/minesweeper.gif" alt="Minesweeper" width="30%" />
-</p>
-
+<div class="collage">
+  <div class="row" align="center">
+    <img src="docs/env_anim/bin_pack.gif" alt="BinPack" width="16%">
+    <img src="docs/env_anim/cleaner.gif" alt="Cleaner" width="16%">
+    <img src="docs/env_anim/connector.gif" alt="Connector" width="16%">
+    <img src="docs/env_anim/cvrp.gif" alt="CVRP" width="16%">
+    <img src="docs/env_anim/game_2048.gif" alt="Game2048" width="16%">
+    <img src="docs/env_anim/graph_coloring.gif" alt="GraphColoring" width="16%">
+  </div>
+  <div class="row" align="center">
+    <img src="docs/env_anim/job_shop.gif" alt="JobShop" width="16%">
+    <img src="docs/env_anim/knapsack.gif" alt="Knapsack" width="16%">
+    <img src="docs/env_anim/maze.gif" alt="Maze" width="16%">
+    <img src="docs/env_anim/minesweeper.gif" alt="Minesweeper" width="16%">
+    <img src="docs/env_anim/mmst.gif" alt="MMST" width="16%">
+    <img src="docs/env_anim/multi_cvrp.gif" alt="MultiCVRP" width="16%">
+  </div>
+  <div class="row" align="center">
+    <img src="docs/env_anim/robot_warehouse.gif" alt="RobotWarehouse" width="16%">
+    <img src="docs/env_anim/rubiks_cube.gif" alt="RubiksCube" width="16%">
+    <img src="docs/env_anim/snake.gif" alt="Snake" width="16%">
+    <img src="docs/env_anim/sudoku.gif" alt="Sudoku" width="16%">
+    <img src="docs/env_anim/tetris.gif" alt="Tetris" width="16%">
+    <img src="docs/env_anim/tsp.gif" alt="Tetris" width="16%">
+  </div>
+</div>
 
 
 ## Welcome to the Jungle! 🌴
 
-Jumanji is a suite of diverse and challenging reinforcement learning (RL) environments written in
-JAX.
+Jumanji is a diverse suite of scalable reinforcement learning environments written in JAX.
 
 Jumanji is helping pioneer a new wave of hardware-accelerated research and development in the
 field of RL. Jumanji's high-speed environments enable faster iteration and large-scale
 experimentation while simultaneously reducing complexity. Originating in the Research Team at
 [InstaDeep](https://www.instadeep.com/), Jumanji is now developed jointly with the open-source
 community. To join us in these efforts, reach out, raise issues and read our
 [contribution guidelines](https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just
@@ -66,58 +104,65 @@
 [RLlib](https://docs.ray.io/en/latest/rllib/index.html), [OpenAI Gym](https://github.com/openai/gym)
 and [DeepMind-Env](https://github.com/deepmind/dm_env) through our `dm_env` and `gym` wrappers.
 - 🎓 **Examples**: guides to facilitate Jumanji's adoption and highlight the added value of
 JAX-based environments.
 - 🏎️ **Training:** example agents that can be used as inspiration for the agents one may implement
 in their research.
 
-
 ## Environments 🌍
 
 Jumanji provides a diverse range of environments ranging from simple games to NP-hard combinatorial
 problems.
 
 | Environment                              | Category | Registered Version(s)                                | Source                                                                                           | Description                                                            |
 |------------------------------------------|----------|------------------------------------------------------|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
-| 🔢 Game2048                              | Logic  | `Game2048-v0`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/)   | [doc](https://instadeepai.github.io/jumanji/environments/game_2048/)   |
+| 🔢 Game2048                              | Logic  | `Game2048-v1`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/)   | [doc](https://instadeepai.github.io/jumanji/environments/game_2048/)   |
+| 🎨 GraphColoring                              | Logic  | `GraphColoring-v0`                                   | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/graph_coloring/)   | [doc](https://instadeepai.github.io/jumanji/environments/graph_coloring/)   |
 | 💣 Minesweeper                           | Logic    | `Minesweeper-v0`                                     | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc](https://instadeepai.github.io/jumanji/environments/minesweeper/) |
 | 🎲 RubiksCube                            | Logic    | `RubiksCube-v0`<br/>`RubiksCube-partly-scrambled-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/rubiks_cube/) | [doc](https://instadeepai.github.io/jumanji/environments/rubiks_cube/) |
-| 📦 BinPack (3D BinPacking Problem)       | Packing  | `BinPack-v1`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/)  | [doc](https://instadeepai.github.io/jumanji/environments/bin_pack/)    |
+| ✏️ Sudoku                       | Logic    | `Sudoku-v0` <br/>`Sudoku-very-easy-v0`               | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/sudoku/) | [doc](https://instadeepai.github.io/jumanji/environments/sudoku/) |
+| 📦 BinPack (3D BinPacking Problem)       | Packing  | `BinPack-v2`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/)  | [doc](https://instadeepai.github.io/jumanji/environments/bin_pack/)    |
 | 🏭 JobShop (Job Shop Scheduling Problem) | Packing  | `JobShop-v0`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/)  | [doc](https://instadeepai.github.io/jumanji/environments/job_shop/)    |
 | 🎒 Knapsack                              | Packing  | `Knapsack-v1`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/knapsack/)  | [doc](https://instadeepai.github.io/jumanji/environments/knapsack/)    |
+| ▒ Tetris                              | Packing  | `Tetris-v0`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/tetris/)  | [doc](https://instadeepai.github.io/jumanji/environments/tetris/)    |
 | 🧹 Cleaner                               | Routing  | `Cleaner-v0`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cleaner/)   | [doc](https://instadeepai.github.io/jumanji/environments/cleaner/)     |
-| :link: Connector                         | Routing  | `Connector-v0`                                       | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/connector/) | [doc](https://instadeepai.github.io/jumanji/environments/connector/)   |
+| :link: Connector                         | Routing  | `Connector-v2`                                       | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/connector/) | [doc](https://instadeepai.github.io/jumanji/environments/connector/)   |
 | 🚚 CVRP (Capacitated Vehicle Routing Problem)  | Routing  | `CVRP-v1`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cvrp/)      | [doc](https://instadeepai.github.io/jumanji/environments/cvrp/)        |
+| 🚚 MultiCVRP (Multi-Agent Capacitated Vehicle Routing Problem)  | Routing  | `MultiCVRP-v0`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/multi_cvrp/)      | [doc](https://instadeepai.github.io/jumanji/environments/multi_cvrp/)        |
 | :mag: Maze   | Routing  | `Maze-v0`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/maze/)      | [doc](https://instadeepai.github.io/jumanji/environments/maze/)        |
+| :robot: RobotWarehouse  | Routing  | `RobotWarehouse-v0`                                  | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/robot_warehouse/)      | [doc](https://instadeepai.github.io/jumanji/environments/robot_warehouse/)        |
 | 🐍 Snake                                       | Routing  | `Snake-v1`                                           | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/snake/)     | [doc](https://instadeepai.github.io/jumanji/environments/snake/)       |
 | 📬 TSP (Travelling Salesman Problem)           | Routing  | `TSP-v1`                                             | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/tsp/)       | [doc](https://instadeepai.github.io/jumanji/environments/tsp/)         |
-
+| Multi Minimum Spanning Tree Problem | Routing  | `MMST-v0`                                | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/mmst)    | [doc](https://instadeepai.github.io/jumanji/environments/mmst/)    |
 
 ## Installation 🎬
 
 You can install the latest release of Jumanji from PyPI:
+
 ```bash
 pip install jumanji
 ```
+
 Alternatively, you can install the latest development version directly from GitHub:
+
 ```bash
 pip install git+https://github.com/instadeepai/jumanji.git
 ```
+
 Jumanji has been tested on Python 3.8 and 3.9.
 Note that because the installation of JAX differs depending on your hardware accelerator,
 we advise users to explicitly install the correct JAX version (see the
 [official installation guide](https://github.com/google/jax#installation)).
 
 **Rendering:** Matplotlib is used for rendering all the environments. To visualize the environments
 you will need a GUI backend. For example, on Linux, you can install Tk via:
 `apt-get install python3-tk`, or using conda: `conda install tk`. Check out
 [Matplotlib backends](https://matplotlib.org/stable/users/explain/backends.html) for a list of
 backends you can use.
 
-
 ## Quickstart ⚡
 
 RL practitioners will find Jumanji's interface familiar as it combines the widely adopted
 [OpenAI Gym](https://github.com/openai/gym) and
 [DeepMind Environment](https://github.com/deepmind/dm_env) interfaces. From OpenAI Gym, we adopted
 the idea of a `registry` and the `render` method, while our `TimeStep` structure is inspired by
 DeepMind Environment.
@@ -166,15 +211,14 @@
 We maintain a registry of standard environments with their configuration.
 For each environment, a version suffix is appended, e.g. `Snake-v1`.
 When changes are made to environments that might impact learning results,
 the version number is incremented by one to prevent potential confusion.
 For a full list of registered versions of each environment, check out
 [the documentation](https://instadeepai.github.io/jumanji/environments/tsp/).
 
-
 ## Training 🏎️
 
 To showcase how to train RL agents on Jumanji environments, we provide a random agent and a vanilla
 actor-critic (A2C) agent. These agents can be found in
 [jumanji/training/](https://github.com/instadeepai/jumanji/tree/main/jumanji/training/).
 
 Because the environment framework in Jumanji is so flexible, it allows pretty much any problem to
@@ -187,40 +231,38 @@
 > ⚠️ The example agents in `jumanji/training` are **only** meant to serve as inspiration for how one
 > can implement an agent. Jumanji is first and foremost a library of environments - as such, the
 > agents and networks will **not** be maintained to a production standard.
 
 For more information on how to use the example agents, see the
 [training guide](https://instadeepai.github.io/jumanji/guides/training/).
 
-
 ## Contributing 🤝
 
 Contributions are welcome! See our issue tracker for
 [good first issues](https://github.com/instadeepai/jumanji/labels/good%20first%20issue). Please read
 our [contributing guidelines](https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) for
 details on how to submit pull requests, our Contributor License Agreement, and community guidelines.
 
-
 ## Citing Jumanji ✏️
 
 If you use Jumanji in your work, please cite the library using:
+
 ```
 @software{jumanji2023github,
   author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
         and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
         Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
         and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
   title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
   url = {https://github.com/instadeepai/jumanji},
   version = {0.2.2},
   year = {2023},
 }
 ```
 
-
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
 
 - 🤖 [Qdax](https://github.com/adaptive-intelligent-robotics/QDax) is a library to accelerate
 Quality-Diversity and neuro-evolution algorithms through hardware accelerators and parallelization.
```

#### html2text {}

```diff
@@ -1,36 +1,52 @@
+Metadata-Version: 2.1 Name: jumanji Version: 0.3.0 Summary: A diverse suite of
+scalable reinforcement learning environments in JAX Home-page: https://
+github.com/instadeepai/jumanji/ Author: InstaDeep Author-email:
+c.bonnet@instadeep.com License: Apache 2.0 Keywords: reinforcement-learning
+python jax Classifier: Development Status :: 4 - Beta Classifier: Environment
+:: Console Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: License :: OSI Approved :: Apache Software
+License Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: train License-File: LICENSE
                                 [Jumanji_logo]
 [![Python Versions](https://img.shields.io/pypi/pyversions/
 jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/) [![PyPI
 Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/
 jumanji) [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/
 tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/
 workflows/tests_linters.yml) [![Code Style](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) [![MyPy](http://
 www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License]
 (https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://
-opensource.org/licenses/Apache-2.0) [**Environments**](#environments-) |
-[**Installation**](#installation-) | [**Quickstart**](#quickstart-) |
-[**Training**](#training-%EF%B8%8F) | [**Citation**](#citing-jumanji-%EF%B8%8F)
-| [**Docs**](https://instadeepai.github.io/jumanji) ---
-    [Connector] [Snake] [Cleaner] [JobShop] [BinPack] [CVRP] [RubiksCube]
-                           [Game2048] [Minesweeper]
-## Welcome to the Jungle! ð´ Jumanji is a suite of diverse and challenging
-reinforcement learning (RL) environments written in JAX. Jumanji is helping
-pioneer a new wave of hardware-accelerated research and development in the
-field of RL. Jumanji's high-speed environments enable faster iteration and
-large-scale experimentation while simultaneously reducing complexity.
-Originating in the Research Team at [InstaDeep](https://www.instadeep.com/),
-Jumanji is now developed jointly with the open-source community. To join us in
-these efforts, reach out, raise issues and read our [contribution guidelines]
-(https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just
-[star](https://github.com/instadeepai/jumanji) ð to stay up to date with the
-latest developments! ### Goals ð 1. Provide a simple, well-tested API for
-JAX-based environments. 2. Make research in RL more accessible. 3. Facilitate
-the research on RL for problems in the industry and help close the gap between
+opensource.org/licenses/Apache-2.0) [![Hugging Face](https://img.shields.io/
+badge/%F0%9F%A4%97-Hugging%20Face-F8D521)](https://huggingface.co/InstaDeepAI)
+[**Environments**](#environments-) | [**Installation**](#installation-) |
+[**Quickstart**](#quickstart-) | [**Training**](#training-%EF%B8%8F) |
+[**Citation**](#citing-jumanji-%EF%B8%8F) | [**Docs**](https://
+instadeepai.github.io/jumanji) ---
+       [BinPack] [Cleaner] [Connector] [CVRP] [Game2048] [GraphColoring]
+         [JobShop] [Knapsack] [Maze] [Minesweeper] [MMST] [MultiCVRP]
+       [RobotWarehouse] [RubiksCube] [Snake] [Sudoku] [Tetris] [Tetris]
+## Welcome to the Jungle! ð´ Jumanji is a diverse suite of scalable
+reinforcement learning environments written in JAX. Jumanji is helping pioneer
+a new wave of hardware-accelerated research and development in the field of RL.
+Jumanji's high-speed environments enable faster iteration and large-scale
+experimentation while simultaneously reducing complexity. Originating in the
+Research Team at [InstaDeep](https://www.instadeep.com/), Jumanji is now
+developed jointly with the open-source community. To join us in these efforts,
+reach out, raise issues and read our [contribution guidelines](https://
+github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just [star](https:
+//github.com/instadeepai/jumanji) ð to stay up to date with the latest
+developments! ### Goals ð 1. Provide a simple, well-tested API for JAX-based
+environments. 2. Make research in RL more accessible. 3. Facilitate the
+research on RL for problems in the industry and help close the gap between
 research and industrial applications. 4. Provide environments whose difficulty
 can be scaled to be arbitrarily hard. ### Overview ð¦ - ð¥ **Environment
 API**: core abstractions for JAX-based environments. - ð¹ï¸ **Environment
 Suite**: a collection of RL environments ranging from simple games to NP-hard
 combinatorial problems. - ð¬ **Wrappers**: easily connect to your favourite
 RL frameworks and libraries such as [Acme](https://github.com/deepmind/acme),
 [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3), [RLlib]
@@ -42,67 +58,86 @@
 inspiration for the agents one may implement in their research. ## Environments
 ð Jumanji provides a diverse range of environments ranging from simple games
 to NP-hard combinatorial problems. | Environment | Category | Registered
 Version(s) | Source | Description | |------------------------------------------
 |----------|------------------------------------------------------|------------
 -------------------------------------------------------------------------------
 -------|-----------------------------------------------------------------------
--| | ð¢ Game2048 | Logic | `Game2048-v0` | [code](https://github.com/
+-| | ð¢ Game2048 | Logic | `Game2048-v1` | [code](https://github.com/
 instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/game_2048/) | | ð£
-Minesweeper | Logic | `Minesweeper-v0` | [code](https://github.com/instadeepai/
-jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc](https://
-instadeepai.github.io/jumanji/environments/minesweeper/) | | ð² RubiksCube |
-Logic | `RubiksCube-v0`
+(https://instadeepai.github.io/jumanji/environments/game_2048/) | | ð¨
+GraphColoring | Logic | `GraphColoring-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/logic/graph_coloring/) |
+[doc](https://instadeepai.github.io/jumanji/environments/graph_coloring/) | |
+ð£ Minesweeper | Logic | `Minesweeper-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc]
+(https://instadeepai.github.io/jumanji/environments/minesweeper/) | | ð²
+RubiksCube | Logic | `RubiksCube-v0`
 `RubiksCube-partly-scrambled-v0` | [code](https://github.com/instadeepai/
 jumanji/tree/main/jumanji/environments/logic/rubiks_cube/) | [doc](https://
-instadeepai.github.io/jumanji/environments/rubiks_cube/) | | ð¦ BinPack (3D
-BinPacking Problem) | Packing | `BinPack-v1` | [code](https://github.com/
-instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/bin_pack/) | | ð­ JobShop
-(Job Shop Scheduling Problem) | Packing | `JobShop-v0` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/
-) | [doc](https://instadeepai.github.io/jumanji/environments/job_shop/) | |
-ð Knapsack | Packing | `Knapsack-v1` | [code](https://github.com/
-instadeepai/jumanji/tree/main/jumanji/environments/packing/knapsack/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/knapsack/) | | ð§¹ Cleaner
-| Routing | `Cleaner-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/cleaner/) | [doc](https://
-instadeepai.github.io/jumanji/environments/cleaner/) | | :link: Connector |
-Routing | `Connector-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/connector/) | [doc](https://
-instadeepai.github.io/jumanji/environments/connector/) | | ð CVRP
-(Capacitated Vehicle Routing Problem) | Routing | `CVRP-v1` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cvrp/) |
-[doc](https://instadeepai.github.io/jumanji/environments/cvrp/) | | :mag: Maze
-| Routing | `Maze-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/maze/) | [doc](https://instadeepai.github.io/
-jumanji/environments/maze/) | | ð Snake | Routing | `Snake-v1` | [code]
-(https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/
-snake/) | [doc](https://instadeepai.github.io/jumanji/environments/snake/) | |
-ð¬ TSP (Travelling Salesman Problem) | Routing | `TSP-v1` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/tsp/) |
-[doc](https://instadeepai.github.io/jumanji/environments/tsp/) | ##
-Installation ð¬ You can install the latest release of Jumanji from PyPI:
-```bash pip install jumanji ``` Alternatively, you can install the latest
-development version directly from GitHub: ```bash pip install git+https://
-github.com/instadeepai/jumanji.git ``` Jumanji has been tested on Python 3.8
-and 3.9. Note that because the installation of JAX differs depending on your
-hardware accelerator, we advise users to explicitly install the correct JAX
-version (see the [official installation guide](https://github.com/google/
-jax#installation)). **Rendering:** Matplotlib is used for rendering all the
-environments. To visualize the environments you will need a GUI backend. For
-example, on Linux, you can install Tk via: `apt-get install python3-tk`, or
-using conda: `conda install tk`. Check out [Matplotlib backends](https://
-matplotlib.org/stable/users/explain/backends.html) for a list of backends you
-can use. ## Quickstart â¡ RL practitioners will find Jumanji's interface
-familiar as it combines the widely adopted [OpenAI Gym](https://github.com/
-openai/gym) and [DeepMind Environment](https://github.com/deepmind/dm_env)
-interfaces. From OpenAI Gym, we adopted the idea of a `registry` and the
-`render` method, while our `TimeStep` structure is inspired by DeepMind
+instadeepai.github.io/jumanji/environments/rubiks_cube/) | | âï¸ Sudoku |
+Logic | `Sudoku-v0`
+`Sudoku-very-easy-v0` | [code](https://github.com/instadeepai/jumanji/tree/
+main/jumanji/environments/logic/sudoku/) | [doc](https://instadeepai.github.io/
+jumanji/environments/sudoku/) | | ð¦ BinPack (3D BinPacking Problem) |
+Packing | `BinPack-v2` | [code](https://github.com/instadeepai/jumanji/tree/
+main/jumanji/environments/packing/bin_pack/) | [doc](https://
+instadeepai.github.io/jumanji/environments/bin_pack/) | | ð­ JobShop (Job
+Shop Scheduling Problem) | Packing | `JobShop-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/) | [doc]
+(https://instadeepai.github.io/jumanji/environments/job_shop/) | | ð
+Knapsack | Packing | `Knapsack-v1` | [code](https://github.com/instadeepai/
+jumanji/tree/main/jumanji/environments/packing/knapsack/) | [doc](https://
+instadeepai.github.io/jumanji/environments/knapsack/) | | â Tetris | Packing
+| `Tetris-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/packing/tetris/) | [doc](https://instadeepai.github.io/
+jumanji/environments/tetris/) | | ð§¹ Cleaner | Routing | `Cleaner-v0` |
+[code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/
+routing/cleaner/) | [doc](https://instadeepai.github.io/jumanji/environments/
+cleaner/) | | :link: Connector | Routing | `Connector-v2` | [code](https://
+github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/
+connector/) | [doc](https://instadeepai.github.io/jumanji/environments/
+connector/) | | ð CVRP (Capacitated Vehicle Routing Problem) | Routing |
+`CVRP-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/
+environments/routing/cvrp/) | [doc](https://instadeepai.github.io/jumanji/
+environments/cvrp/) | | ð MultiCVRP (Multi-Agent Capacitated Vehicle Routing
+Problem) | Routing | `MultiCVRP-v0` | [code](https://github.com/instadeepai/
+jumanji/tree/main/jumanji/environments/routing/multi_cvrp/) | [doc](https://
+instadeepai.github.io/jumanji/environments/multi_cvrp/) | | :mag: Maze |
+Routing | `Maze-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/maze/) | [doc](https://instadeepai.github.io/
+jumanji/environments/maze/) | | :robot: RobotWarehouse | Routing |
+`RobotWarehouse-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/robot_warehouse/) | [doc](https://
+instadeepai.github.io/jumanji/environments/robot_warehouse/) | | ð Snake |
+Routing | `Snake-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/snake/) | [doc](https://instadeepai.github.io/
+jumanji/environments/snake/) | | ð¬ TSP (Travelling Salesman Problem) |
+Routing | `TSP-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/tsp/) | [doc](https://instadeepai.github.io/
+jumanji/environments/tsp/) | | Multi Minimum Spanning Tree Problem | Routing |
+`MMST-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/
+environments/routing/mmst) | [doc](https://instadeepai.github.io/jumanji/
+environments/mmst/) | ## Installation ð¬ You can install the latest release
+of Jumanji from PyPI: ```bash pip install jumanji ``` Alternatively, you can
+install the latest development version directly from GitHub: ```bash pip
+install git+https://github.com/instadeepai/jumanji.git ``` Jumanji has been
+tested on Python 3.8 and 3.9. Note that because the installation of JAX differs
+depending on your hardware accelerator, we advise users to explicitly install
+the correct JAX version (see the [official installation guide](https://
+github.com/google/jax#installation)). **Rendering:** Matplotlib is used for
+rendering all the environments. To visualize the environments you will need a
+GUI backend. For example, on Linux, you can install Tk via: `apt-get install
+python3-tk`, or using conda: `conda install tk`. Check out [Matplotlib
+backends](https://matplotlib.org/stable/users/explain/backends.html) for a list
+of backends you can use. ## Quickstart â¡ RL practitioners will find Jumanji's
+interface familiar as it combines the widely adopted [OpenAI Gym](https://
+github.com/openai/gym) and [DeepMind Environment](https://github.com/deepmind/
+dm_env) interfaces. From OpenAI Gym, we adopted the idea of a `registry` and
+the `render` method, while our `TimeStep` structure is inspired by DeepMind
 Environment. ### Basic Usage ð§âð» ```python import jax import jumanji #
 Instantiate a Jumanji environment using the registry env = jumanji.make('Snake-
 v1') # Reset your (jit-able) environment key = jax.random.PRNGKey(0) state,
 timestep = jax.jit(env.reset)(key) # (Optional) Render the env state env.render
 (state) # Interact with the (jit-able) environment action = env.action_spec
 ().generate_value() # Action selection (dummy value here) state, timestep =
 jax.jit(env.step)(state, action) # Take a step and observe the next state and
```

### Comparing `jumanji-0.2.2/jumanji/env.py` & `jumanji-0.3.0/jumanji/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/__init__.py` & `jumanji-0.3.0/jumanji/environments/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,25 +12,41 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import sys
 
 from jumanji.environments.logic import game_2048, minesweeper, rubiks_cube
 from jumanji.environments.logic.game_2048.env import Game2048
+from jumanji.environments.logic.graph_coloring.env import GraphColoring
 from jumanji.environments.logic.minesweeper import Minesweeper
 from jumanji.environments.logic.rubiks_cube import RubiksCube
-from jumanji.environments.packing import bin_pack, job_shop, knapsack
+from jumanji.environments.logic.sudoku import Sudoku
+from jumanji.environments.packing import bin_pack, job_shop, knapsack, tetris
 from jumanji.environments.packing.bin_pack.env import BinPack
 from jumanji.environments.packing.job_shop.env import JobShop
 from jumanji.environments.packing.knapsack.env import Knapsack
-from jumanji.environments.routing import cleaner, connector, cvrp, maze, snake, tsp
+from jumanji.environments.packing.tetris.env import Tetris
+from jumanji.environments.routing import (
+    cleaner,
+    connector,
+    cvrp,
+    maze,
+    mmst,
+    multi_cvrp,
+    robot_warehouse,
+    snake,
+    tsp,
+)
 from jumanji.environments.routing.cleaner.env import Cleaner
 from jumanji.environments.routing.connector.env import Connector
 from jumanji.environments.routing.cvrp.env import CVRP
 from jumanji.environments.routing.maze.env import Maze
+from jumanji.environments.routing.mmst.env import MMST
+from jumanji.environments.routing.multi_cvrp import MultiCVRP
+from jumanji.environments.routing.robot_warehouse.env import RobotWarehouse
 from jumanji.environments.routing.snake.env import Snake
 from jumanji.environments.routing.tsp.env import TSP
 
 
 def is_colab() -> bool:
     return "google.colab" in sys.modules
```

### Comparing `jumanji-0.2.2/jumanji/environments/commons/__init__.py` & `jumanji-0.3.0/jumanji/environments/commons/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/commons/maze_utils/__init__.py` & `jumanji-0.3.0/jumanji/environments/commons/maze_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_generation.py` & `jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_generation.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,16 +199,16 @@
     return ~empty_stack(state.chambers)
 
 
 def generate_maze(width: int, height: int, key: chex.PRNGKey) -> chex.Array:
     """Randomly generate a maze.
 
     Args:
-        width: the number of rows of the maze to create.
-        height: the number of columns of the maze to create.
+        width: the number of columns of the maze to create.
+        height: the number of rows of the maze to create.
         key: the Jax random number generation key.
 
     Returns:
         maze: the generated maze.
     """
     maze = create_empty_maze(width, height)
     chambers = create_chambers_stack(width, height)
```

### Comparing `jumanji-0.2.2/jumanji/environments/commons/maze_utils/maze_rendering.py` & `jumanji-0.3.0/jumanji/environments/commons/maze_utils/maze_rendering.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/commons/maze_utils/stack.py` & `jumanji-0.3.0/jumanji/environments/commons/maze_utils/stack.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/__init__.py` & `jumanji-0.3.0/jumanji/environments/logic/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/game_2048/__init__.py` & `jumanji-0.3.0/jumanji/environments/logic/game_2048/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/game_2048/env.py` & `jumanji-0.3.0/jumanji/environments/logic/game_2048/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,33 +183,30 @@
         # Take the action in the environment: Up, Right, Down, Left.
         updated_board, additional_reward = jax.lax.switch(
             action,
             [move_up, move_right, move_down, move_left],
             state.board,
         )
 
-        # Generate action mask to keep in the state for the next step and
-        # to provide to the agent in the observation.
-        action_mask = self._get_action_mask(board=updated_board)
-
-        # Check if the episode terminates (i.e. there are no legal actions).
-        done = ~jnp.any(action_mask)
-
         # Generate new key.
         random_cell_key, new_state_key = jax.random.split(state.key)
 
         # Update the state of the board by adding a new random cell.
         updated_board = jax.lax.cond(
-            done,
-            lambda board, key: board,
+            state.action_mask[action],
             self._add_random_cell,
+            lambda board, key: board,
             updated_board,
             random_cell_key,
         )
 
+        # Generate action mask to keep in the state for the next step and
+        # to provide to the agent in the observation.
+        action_mask = self._get_action_mask(board=updated_board)
+
         # Build the state.
         state = State(
             board=updated_board,
             action_mask=action_mask,
             step_count=state.step_count + 1,
             key=new_state_key,
             score=state.score + additional_reward.astype(float),
@@ -217,14 +214,17 @@
 
         # Generate the observation from the environment state.
         observation = Observation(
             board=updated_board,
             action_mask=action_mask,
         )
 
+        # Check if the episode terminates (i.e. there are no legal actions).
+        done = ~jnp.any(action_mask)
+
         # Return either a MID or a LAST timestep depending on done.
         highest_tile = 2 ** jnp.max(updated_board)
         extras = {"highest_tile": highest_tile}
         timestep = jax.lax.cond(
             done,
             lambda: termination(
                 reward=additional_reward,
```

### Comparing `jumanji-0.2.2/jumanji/environments/logic/game_2048/types.py` & `jumanji-0.3.0/jumanji/environments/logic/game_2048/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/game_2048/utils.py` & `jumanji-0.3.0/jumanji/environments/logic/game_2048/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/game_2048/viewer.py` & `jumanji-0.3.0/jumanji/environments/logic/game_2048/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/__init__.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/constants.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/done.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/done.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/env.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/generator.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/reward.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/types.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/utils.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/minesweeper/viewer.py` & `jumanji-0.3.0/jumanji/environments/logic/minesweeper/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/__init__.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/constants.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/env.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/generator.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/reward.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/types.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/utils.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/logic/rubiks_cube/viewer.py` & `jumanji-0.3.0/jumanji/environments/logic/rubiks_cube/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/__init__.py` & `jumanji-0.3.0/jumanji/environments/packing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/__init__.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/env.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,46 +111,50 @@
     env.render(state)
     ```
     """
 
     def __init__(
         self,
         generator: Optional[Generator] = None,
-        obs_num_ems: int = 70,
+        obs_num_ems: int = 40,
         reward_fn: Optional[RewardFn] = None,
         normalize_dimensions: bool = True,
         debug: bool = False,
         viewer: Optional[Viewer[State]] = None,
     ):
         """Instantiates a `BinPack` environment.
 
         Args:
             generator: `Generator` whose `__call__` instantiates an environment
                 instance. Implemented options are [`RandomGenerator`, `ToyGenerator`,
-                `CSVGenerator`]. Defaults to `RandomGenerator` that generates up to 30 items maximum
-                and that can handle 100 EMSs.
+                `CSVGenerator`]. Defaults to `RandomGenerator` that generates up to 20 items maximum
+                and that can handle 40 EMSs.
             obs_num_ems: number of EMSs (possible spaces in which to place an item) to show to the
                 agent. If `obs_num_ems` is smaller than `generator.max_num_ems`, the first
                 `obs_num_ems` largest EMSs (in terms of volume) will be returned in the observation.
                 The good number heavily depends on the number of items (given by the instance
-                generator). Default to 70 EMSs observable.
+                generator). Default to 40 EMSs observable.
             reward_fn: compute the reward based on the current state, the chosen action, the next
                 state, whether the transition is valid and if it is terminal. Implemented options
                 are [`DenseReward`, `SparseReward`]. In each case, the total return at the end of
                 an episode is the volume utilization of the container. Defaults to `DenseReward`.
             normalize_dimensions: if True, the observation is normalized (float) along each
                 dimension into a unit cubic container. If False, the observation is returned in
                 millimeters, i.e. integers (for both items and EMSs). Default to True.
             debug: if True, will add to timestep.extras an `invalid_ems_from_env` field that checks
                 if an invalid EMS was created by the environment, which should not happen. Computing
                 this metric slows down the environment. Default to False.
             viewer: `Viewer` used for rendering. Defaults to `BinPackViewer` with "human" render
                 mode.
         """
-        self.generator = generator or RandomGenerator(max_num_items=30, max_num_ems=100)
+        self.generator = generator or RandomGenerator(
+            max_num_items=20,
+            max_num_ems=40,
+            split_num_same_items=2,
+        )
         self.obs_num_ems = obs_num_ems
         self.reward_fn = reward_fn or DenseReward()
         self.normalize_dimensions = normalize_dimensions
         self._viewer = viewer or BinPackViewer("BinPack", render_mode="human")
         self.debug = debug
 
     def __repr__(self) -> str:
```

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/generator.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/reward.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/space.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/space.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/types.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/bin_pack/viewer.py` & `jumanji-0.3.0/jumanji/environments/packing/bin_pack/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/job_shop/__init__.py` & `jumanji-0.3.0/jumanji/environments/packing/job_shop/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/job_shop/env.py` & `jumanji-0.3.0/jumanji/environments/packing/job_shop/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/job_shop/generator.py` & `jumanji-0.3.0/jumanji/environments/packing/job_shop/generator.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/job_shop/types.py` & `jumanji-0.3.0/jumanji/environments/packing/job_shop/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/job_shop/viewer.py` & `jumanji-0.3.0/jumanji/environments/packing/job_shop/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/knapsack/__init__.py` & `jumanji-0.3.0/jumanji/environments/packing/knapsack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/knapsack/env.py` & `jumanji-0.3.0/jumanji/environments/packing/knapsack/env.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import jax
 import jax.numpy as jnp
 import matplotlib
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
+from jumanji.environments.packing.knapsack.generator import Generator, RandomGenerator
 from jumanji.environments.packing.knapsack.reward import DenseReward, RewardFn
 from jumanji.environments.packing.knapsack.types import Observation, State
 from jumanji.environments.packing.knapsack.viewer import KnapsackViewer
 from jumanji.types import TimeStep, restart, termination, transition
 from jumanji.viewer import Viewer
 
 
@@ -79,39 +80,43 @@
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        num_items: int = 50,
-        total_budget: float = 12.5,
+        generator: Optional[Generator] = None,
         reward_fn: Optional[RewardFn] = None,
         viewer: Optional[Viewer[State]] = None,
     ):
         """Instantiates a `Knapsack` environment.
 
         Args:
-            num_items: the number of items in the environment. Defaults to 50.
-            total_budget: the capacity of the knapsack. Defaults to 12.5.
+            generator: `Generator` whose `__call__` instantiates an environment instance.
+                The default option is 'RandomGenerator' which samples Knapsack instances
+                with 50 items and a total budget of 12.5.
             reward_fn: `RewardFn` whose `__call__` method computes the reward of an environment
                 transition. The function must compute the reward based on the current state,
                 the chosen action, the next state and whether the action is valid.
                 Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
             viewer: `Viewer` used for rendering. Defaults to `KnapsackViewer` with "human" render
                 mode.
         """
 
-        self.num_items = num_items
-        self.total_budget = total_budget
+        self.generator = generator or RandomGenerator(
+            num_items=50,
+            total_budget=12.5,
+        )
+        self.num_items = self.generator.num_items
+        self.total_budget = self.generator.total_budget
         self.reward_fn = reward_fn or DenseReward()
         self._viewer = viewer or KnapsackViewer(
             name="Knapsack",
             render_mode="human",
-            total_budget=total_budget,
+            total_budget=self.total_budget,
         )
 
     def __repr__(self) -> str:
         return (
             f"Knapsack environment with {self.num_items} items "
             f"and a total budget of {self.total_budget}."
         )
@@ -122,25 +127,15 @@
         Args:
             key: used to randomly generate the weights and values of the items.
 
         Returns:
             state: the new state of the environment.
             timestep: the first timestep returned by the environment.
         """
-        key, sample_key = jax.random.split(key)
-        weights, values = jax.random.uniform(
-            sample_key, (2, self.num_items), minval=0, maxval=1
-        )
-        state = State(
-            weights=weights,
-            values=values,
-            packed_items=jnp.zeros(self.num_items, dtype=bool),
-            remaining_budget=jnp.array(self.total_budget, float),
-            key=key,
-        )
+        state = self.generator(key)
         timestep = restart(observation=self._state_to_observation(state))
         return state, timestep
 
     def step(
         self, state: State, action: chex.Numeric
     ) -> Tuple[State, TimeStep[Observation]]:
         """Run one timestep of the environment's dynamics.
```

### Comparing `jumanji-0.2.2/jumanji/environments/packing/knapsack/reward.py` & `jumanji-0.3.0/jumanji/environments/packing/knapsack/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/knapsack/types.py` & `jumanji-0.3.0/jumanji/environments/packing/knapsack/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/packing/knapsack/viewer.py` & `jumanji-0.3.0/jumanji/environments/packing/knapsack/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cleaner/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cleaner/constants.py` & `jumanji-0.3.0/jumanji/environments/routing/cleaner/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cleaner/env.py` & `jumanji-0.3.0/jumanji/environments/routing/cleaner/env.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cleaner/generator.py` & `jumanji-0.3.0/jumanji/environments/routing/cleaner/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
             key: the Jax random number generation key.
 
         Returns:
             state: the generated state.
         """
         generator_key, state_key = jax.random.split(key)
         maze = maze_generation.generate_maze(
-            self.num_rows, self.num_cols, generator_key
+            self.num_cols, self.num_rows, generator_key
         )
 
         grid = self._adapt_values(maze)
 
         # Agents start in upper left corner
         agents_locations = jnp.zeros((self.num_agents, 2), jnp.int32)
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cleaner/types.py` & `jumanji-0.3.0/jumanji/environments/routing/cleaner/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cleaner/viewer.py` & `jumanji-0.3.0/jumanji/environments/routing/cleaner/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/constants.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/env.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/env.py`

 * *Files 14% similar despite different names*

```diff
@@ -25,71 +25,65 @@
 from jumanji.environments.routing.connector.constants import (
     AGENT_INITIAL_VALUE,
     NOOP,
     PATH,
 )
 from jumanji.environments.routing.connector.generator import (
     Generator,
-    UniformRandomGenerator,
+    RandomWalkGenerator,
 )
 from jumanji.environments.routing.connector.reward import DenseRewardFn, RewardFn
 from jumanji.environments.routing.connector.types import Agent, Observation, State
 from jumanji.environments.routing.connector.utils import (
     connected_or_blocked,
     get_agent_grid,
     get_correction_mask,
     is_valid_position,
     move_agent,
     move_position,
-    switch_perspective,
 )
 from jumanji.environments.routing.connector.viewer import ConnectorViewer
 from jumanji.types import TimeStep, restart, termination, transition
 from jumanji.viewer import Viewer
 
 
 class Connector(Environment[State]):
-    """The `Connector` environment is a multi-agent gridworld problem where each agent must connect a
-    start to a target. However, when moving through this gridworld the agent leaves an impassable
-    trail behind it. Therefore, agents must connect to their targets without overlapping the routes
-    taken by any other agent.
+    """The `Connector` environment is a gridworld problem where multiple pairs of points (sets)
+    must be connected without overlapping the paths taken by any other set. This is achieved
+    by allowing certain points to move to an adjacent cell at each step. However, each time a
+    point moves it leaves an impassable trail behind it. The goal is to connect all sets.
 
     - observation - `Observation`
         - action mask: jax array (bool) of shape (num_agents, 5).
         - step_count: jax array (int32) of shape ()
             the current episode step.
-        - grid: jax array (int32) of shape (num_agents, size, size)
-            - each 2d array (size, size) along axis 0 is the agent's local observation.
-            - agents have ids from 0 to (num_agents - 1)
+        - grid: jax array (int32) of shape (grid_size, grid_size)
             - with 2 agents you might have a grid like this:
               4 0 1
               5 0 1
               6 3 2
               which means agent 1 has moved from the top right of the grid down and is currently in
               the bottom right corner and is aiming to get to the middle bottom cell. Agent 2
               started in the top left and moved down once towards its target in the bottom left.
 
-              This would just be agent 0's view, the numbers would be flipped for agent 1's view.
-              So the full observation would be of shape (2, 3, 3).
-
     - action: jax array (int32) of shape (num_agents,):
         - can take the values [0,1,2,3,4] which correspond to [No Op, Up, Right, Down, Left].
         - each value in the array corresponds to an agent's action.
 
     - reward: jax array (float) of shape ():
-        - dense: each agent is given 1.0 if it connects on that step, otherwise 0.0. Additionally,
-            each agent that has not connected receives a penalty reward of -0.03.
+        - dense: reward is 1 for each successful connection on that step. Additionally,
+            each pair of points that have not connected receives a penalty reward of -0.03.
 
-    - episode termination: if an agent can't move, or the time limit is reached, or the agent
-        connects to its target, it is considered done. Once all agents are done, the episode
-        terminates. The timestep discounts are of shape (num_agents,).
+    - episode termination:
+        - all agents either can't move (no available actions) or have connected to their target.
+        - the time limit is reached.
 
     - state: State:
         - key: jax PRNG key used to randomly spawn agents and targets.
-        - grid: jax array (int32) of shape (size, size) which corresponds to agent 0's observation.
+        - grid: jax array (int32) of shape (grid_size, grid_size) giving the observation.
         - step_count: jax array (int32) of shape () number of steps elapsed in the current episode.
 
     ```python
     from jumanji.environments import Connector
     env = Connector()
     key = jax.random.key(0)
     state, timestep = jax.jit(env.reset)(key)
@@ -107,25 +101,23 @@
         time_limit: int = 50,
         viewer: Optional[Viewer[State]] = None,
     ) -> None:
         """Create the `Connector` environment.
 
         Args:
             generator: `Generator` whose `__call__` instantiates an environment instance.
-                Implemented options are [`UniformRandomGenerator`].
-                Defaults to `UniformRandomGenerator` with `grid_size=10` and `num_agents=5`.
+                Implemented options are [`UniformRandomGenerator`, `RandomWalkGenerator`].
+                Defaults to `RandomWalkGenerator` with `grid_size=10` and `num_agents=10`.
             reward_fn: class of type `RewardFn`, whose `__call__` is used as a reward function.
                 Implemented options are [`DenseRewardFn`]. Defaults to `DenseRewardFn`.
             time_limit: the number of steps allowed before an episode terminates. Defaults to 50.
             viewer: `Viewer` used for rendering. Defaults to `ConnectorViewer` with "human" render
                 mode.
         """
-        self._generator = generator or UniformRandomGenerator(
-            grid_size=10, num_agents=5
-        )
+        self._generator = generator or RandomWalkGenerator(grid_size=10, num_agents=10)
         self._reward_fn = reward_fn or DenseRewardFn()
         self.time_limit = time_limit
         self.num_agents = self._generator.num_agents
         self.grid_size = self._generator.grid_size
         self._agent_ids = jnp.arange(self.num_agents)
         self._viewer = viewer or ConnectorViewer(
             "Connector", self.num_agents, render_mode="human"
@@ -143,22 +135,20 @@
         """
         state = self._generator(key)
 
         action_mask = jax.vmap(self._get_action_mask, (0, None))(
             state.agents, state.grid
         )
         observation = Observation(
-            grid=self._obs_from_grid(state.grid),
+            grid=state.grid,
             action_mask=action_mask,
             step_count=state.step_count,
         )
         extras = self._get_extras(state)
-        timestep = restart(
-            observation=observation, extras=extras, shape=(self.num_agents,)
-        )
+        timestep = restart(observation=observation, extras=extras)
         return state, timestep
 
     def step(
         self, state: State, action: chex.Array
     ) -> Tuple[State, TimeStep[Observation]]:
         """Perform an environment step.
 
@@ -176,39 +166,34 @@
             timestep: `TimeStep` object corresponding the timestep returned by the environment.
         """
         agents, grid = self._step_agents(state, action)
         new_state = State(
             grid=grid, step_count=state.step_count + 1, agents=agents, key=state.key
         )
 
-        # Construct timestep: get observations, rewards, discounts
-        grids = self._obs_from_grid(grid)
+        # Construct timestep: get reward, legal actions and done
         reward = self._reward_fn(state, action, new_state)
         action_mask = jax.vmap(self._get_action_mask, (0, None))(agents, grid)
         observation = Observation(
-            grid=grids, action_mask=action_mask, step_count=new_state.step_count
+            grid=grid, action_mask=action_mask, step_count=new_state.step_count
         )
 
-        dones = jax.vmap(connected_or_blocked)(agents, action_mask)
-        discount = jnp.asarray(jnp.logical_not(dones), dtype=float)
+        done = jnp.all(jax.vmap(connected_or_blocked)(agents, action_mask))
         extras = self._get_extras(new_state)
         timestep = jax.lax.cond(
-            dones.all() | (new_state.step_count >= self.time_limit),
+            done | (new_state.step_count >= self.time_limit),
             lambda: termination(
                 reward=reward,
                 observation=observation,
                 extras=extras,
-                shape=self.num_agents,
             ),
             lambda: transition(
                 reward=reward,
                 observation=observation,
-                discount=discount,
                 extras=extras,
-                shape=self.num_agents,
             ),
         )
 
         return new_state, timestep
 
     def _step_agents(
         self, state: State, action: chex.Array
@@ -267,20 +252,14 @@
             agent,
             grid,
             new_pos,
         )
 
         return new_agent, new_grid
 
-    def _obs_from_grid(self, grid: chex.Array) -> chex.Array:
-        """Gets the observation vector for all agents."""
-        return jax.vmap(switch_perspective, (None, 0, None))(
-            grid, self._agent_ids, self.num_agents
-        )
-
     def _get_action_mask(self, agent: Agent, grid: chex.Array) -> chex.Array:
         """Gets an agent's action mask."""
         # Don't check action 0 because no-op is always valid
         actions = jnp.arange(1, 5)
 
         def is_valid_action(action: int) -> chex.Array:
             agent_pos = move_position(agent.position, action)
@@ -340,20 +319,20 @@
         self._viewer.close()
 
     def observation_spec(self) -> specs.Spec[Observation]:
         """Specifications of the observation of the `Connector` environment.
 
         Returns:
             Spec for the `Observation` whose fields are:
-            - grid: BoundedArray (int32) of shape (num_agents, grid_size, grid_size).
+            - grid: BoundedArray (int32) of shape (grid_size, grid_size).
             - action_mask: BoundedArray (bool) of shape (num_agents, 5).
             - step_count: BoundedArray (int32) of shape ().
         """
         grid = specs.BoundedArray(
-            shape=(self.num_agents, self.grid_size, self.grid_size),
+            shape=(self.grid_size, self.grid_size),
             dtype=jnp.int32,
             name="grid",
             minimum=0,
             maximum=self.num_agents * 3 + AGENT_INITIAL_VALUE,
         )
         action_mask = specs.BoundedArray(
             shape=(self.num_agents, 5),
@@ -376,38 +355,18 @@
             action_mask=action_mask,
             step_count=step_count,
         )
 
     def action_spec(self) -> specs.MultiDiscreteArray:
         """Returns the action spec for the Connector environment.
 
-        5 actions: [0,1,2,3,4] -> [No Op, Up, Right, Down, Left]. Since this is a multi-agent
-        environment, the environment expects an array of actions of shape (num_agents,).
+        5 actions: [0,1,2,3,4] -> [No Op, Up, Right, Down, Left]. Since this is an environment with
+        a multi-dimensional action space, it expects an array of actions of shape (num_agents,).
 
         Returns:
             observation_spec: `MultiDiscreteArray` of shape (num_agents,).
         """
         return specs.MultiDiscreteArray(
             num_values=jnp.array([5] * self.num_agents),
             dtype=jnp.int32,
             name="action",
         )
-
-    def reward_spec(self) -> specs.Array:
-        """
-        Returns:
-            reward_spec: a `specs.Array` spec of shape (num_agents,). One for each agent.
-        """
-        return specs.Array(shape=(self.num_agents,), dtype=float, name="reward")
-
-    def discount_spec(self) -> specs.BoundedArray:
-        """
-        Returns:
-            discount_spec: a `specs.Array` spec of shape (num_agents,). One for each agent
-        """
-        return specs.BoundedArray(
-            shape=(self.num_agents,),
-            dtype=float,
-            minimum=0.0,
-            maximum=1.0,
-            name="discount",
-        )
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/reward.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/reward.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,16 +39,16 @@
 
         Returns:
             The reward for the current step.
         """
 
 
 class DenseRewardFn(RewardFn):
-    """Rewards each agent with 1.0 if it connects on that step, otherwise 0.0. Each agent also
-    receives a penalty of -0.03 at every timestep if they have not connected yet.
+    """Returns: reward of 1.0 for each agent that connects on that step and adds a penalty of
+    -0.03, per agent, at every timestep where they have yet to connect.
     """
 
     def __init__(
         self,
         connected_reward: float = 1.0,
         timestep_reward: float = -0.03,
     ) -> None:
@@ -69,8 +69,8 @@
     ) -> chex.Array:
         connected_rewards = self.connected_reward * jnp.asarray(
             ~state.agents.connected & next_state.agents.connected, float
         )
         timestep_rewards = self.timestep_reward * jnp.asarray(
             ~state.agents.connected, float
         )
-        return connected_rewards + timestep_rewards
+        return jnp.sum(connected_rewards + timestep_rewards)
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/types.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import TYPE_CHECKING, NamedTuple
+from typing import TYPE_CHECKING, Any, NamedTuple
+
+import chex
+import jax.numpy as jnp
 
 if TYPE_CHECKING:  # https://github.com/python/mypy/issues/6239
     from dataclasses import dataclass
 else:
     from chex import dataclass
 
-import chex
-import jax.numpy as jnp
-
 
 @dataclass
 class Agent:
     """
     id: unique number representing only this agent.
     start: start position of this agent.
     target: goal position of this agent.
@@ -38,14 +38,23 @@
     position: chex.Array  # (2,)
 
     @property
     def connected(self) -> chex.Array:
         """returns: True if the agent has reached its target."""
         return jnp.all(self.position == self.target, axis=-1)
 
+    def __eq__(self: "Agent", agent_2: Any) -> chex.Array:
+        if not isinstance(agent_2, Agent):
+            return NotImplemented
+        same_ids = (agent_2.id == self.id).all()
+        same_starts = (agent_2.start == self.start).all()
+        same_targets = (agent_2.target == self.target).all()
+        same_position = (agent_2.position == self.position).all()
+        return same_ids & same_starts & same_targets & same_position
+
 
 @dataclass
 class State:
     """
     grid: grid representing the position of all agents.
     step_count: the index of the current step.
     agents: a stacked pytree of type Agent.
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/utils.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from typing import Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 
 from jumanji.environments.routing.connector.constants import (
-    AGENT_INITIAL_VALUE,
     EMPTY,
     PATH,
     POSITION,
     TARGET,
 )
 from jumanji.environments.routing.connector.types import Agent
 
@@ -145,46 +144,14 @@
     path = get_path(agent_id)
     agent_head = (grid == position) * position
     agent_target = (grid == target) * target
     agent_path = (grid == path) * path
     return agent_head + agent_target + agent_path
 
 
-def switch_perspective(grid: chex.Array, agent_id: int, num_agents: int) -> chex.Array:
-    """Encodes the observation with respect to the current agent defined by `agent_id`.
-
-    `agent_id`'s observations will always take the values 1,2,3 and ordering of observations
-    will be preserved (agent 0's observations always come before agent 1's).
-
-    For example, in a 3-agent game, if we wanted to switch to
-    agent 1's perspective, then:
-    agent 1s values will change from 4,5,6 -> 1,2,3
-    agent 2s values will change from 7,8,9 -> 4,5,6
-    agent 0s values will change from 1,2,3 -> 7,8,9
-
-    Agent 0 will be passed observations where it is represented by the values 1,2,3. Agent 1
-    will be passed observations where it is represented by the values 1,2,3. However in the
-    state agent 0 will always be 1,2,3 and agent 1 will always be 4,5,6.
-
-    Args:
-        grid: the environment state grid.
-        agent_id: the id of the agent whose observation is being requested.
-        num_agents: the number of agents on the grid.
-
-    Returns:
-        Array: the grid in the perspective of the given agent id.
-    """
-    new_grid = grid - AGENT_INITIAL_VALUE  # Center agent values around 0
-    new_grid -= 3 * agent_id  # Move the obs
-    new_grid %= 3 * num_agents  # Keep obs in bounds
-    new_grid += AGENT_INITIAL_VALUE  # 'Un-center' agent obs around 0
-    # Take agent values from rotated grid and empty values from old grid
-    return jnp.where((grid >= AGENT_INITIAL_VALUE), new_grid, grid)
-
-
 def get_correction_mask(
     old_grid: chex.Array, joined_grid: chex.Array, agent_id: chex.Numeric
 ) -> Tuple[chex.Array, chex.Array]:
     """Creates a correction grid for collided agents.
 
     This is used when vmapping each agents movements, in order to correct for collisions.
     Checks if the agent's position is on the new grid, if not, it has been overwritten when
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/connector/viewer.py` & `jumanji-0.3.0/jumanji/environments/routing/connector/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cvrp/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cvrp/constants.py` & `jumanji-0.3.0/jumanji/environments/routing/cvrp/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cvrp/env.py` & `jumanji-0.3.0/jumanji/environments/routing/cvrp/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import jax
 import jax.numpy as jnp
 import matplotlib
 
 from jumanji import specs
 from jumanji.env import Environment
 from jumanji.environments.routing.cvrp.constants import DEPOT_IDX
+from jumanji.environments.routing.cvrp.generator import Generator, UniformGenerator
 from jumanji.environments.routing.cvrp.reward import DenseReward, RewardFn
 from jumanji.environments.routing.cvrp.types import Observation, State
 from jumanji.environments.routing.cvrp.viewer import CVRPViewer
 from jumanji.types import TimeStep, restart, termination, transition
 from jumanji.viewer import Viewer
 
 
@@ -92,41 +93,45 @@
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        num_nodes: int = 20,
-        max_capacity: int = 30,
-        max_demand: int = 10,
+        generator: Optional[Generator] = None,
         reward_fn: Optional[RewardFn] = None,
         viewer: Optional[Viewer[State]] = None,
     ):
         """Instantiates a `CVRP` environment.
 
         Args:
-            num_nodes: number of city nodes in the environment. Defaults to 20.
-            max_capacity: maximum capacity of the vehicle. Defaults to 30.
-            max_demand: maximum demand of each node. Defaults to 10.
+            generator: `Generator` whose `__call__` instantiates an environment instance.
+                The default option is 'UniformGenerator' which randomly generates
+                CVRP instances with 20 cities sampled from a uniform distribution,
+                a maximum vehicle capacity of 30, and a maximum city demand of 10.
             reward_fn: `RewardFn` whose `__call__` method computes the reward of an environment
                 transition. The function must compute the reward based on the current state,
                 the chosen action, the next state and whether the action is valid.
                 Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
             viewer: `Viewer` used for rendering. Defaults to `CVRPViewer` with "human" render mode.
         """
 
-        if max_capacity < max_demand:
+        self.generator = generator or UniformGenerator(
+            num_nodes=20,
+            max_capacity=30,
+            max_demand=10,
+        )
+        self.num_nodes = self.generator.num_nodes
+        self.max_capacity = self.generator.max_capacity
+        self.max_demand = self.generator.max_demand
+        if self.max_capacity < self.max_demand:
             raise ValueError(
                 f"The demand associated with each node must be lower than the maximum capacity, "
-                f"hence the maximum capacity must be >= {max_demand}."
+                f"hence the maximum capacity must be >= {self.max_demand}."
             )
-        self.num_nodes = num_nodes
-        self.max_capacity = max_capacity
-        self.max_demand = max_demand
         self.reward_fn = reward_fn or DenseReward()
         self._viewer = viewer or CVRPViewer(
             name="CVRP",
             num_cities=self.num_nodes,
             render_mode="human",
         )
 
@@ -143,33 +148,15 @@
             key: used to randomly generate the coordinates.
 
         Returns:
              state: `State` object corresponding to the new state of the environment.
              timestep: `TimeStep` object corresponding to the first timestep returned by the
                 environment.
         """
-        key, coordinates_key, demands_key = jax.random.split(key, 3)
-        coordinates = jax.random.uniform(
-            coordinates_key, (self.num_nodes + 1, 2), minval=0, maxval=1
-        )
-        demands = jax.random.randint(
-            demands_key, (self.num_nodes + 1,), minval=1, maxval=self.max_demand
-        )
-        demands = demands.at[DEPOT_IDX].set(0)
-        visited_mask = jnp.zeros(self.num_nodes + 1, dtype=bool).at[DEPOT_IDX].set(True)
-        state = State(
-            coordinates=coordinates,
-            demands=demands,
-            position=jnp.array(DEPOT_IDX, jnp.int32),
-            capacity=jnp.array(self.max_capacity, jnp.int32),
-            visited_mask=visited_mask,
-            trajectory=jnp.full(2 * self.num_nodes, DEPOT_IDX, jnp.int32),
-            num_total_visits=jnp.array(1, jnp.int32),
-            key=key,
-        )
+        state = self.generator(key)
         timestep = restart(observation=self._state_to_observation(state))
         return state, timestep
 
     def step(
         self, state: State, action: chex.Numeric
     ) -> Tuple[State, TimeStep[Observation]]:
         """Run one timestep of the environment's dynamics.
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cvrp/reward.py` & `jumanji-0.3.0/jumanji/environments/routing/cvrp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cvrp/types.py` & `jumanji-0.3.0/jumanji/environments/routing/cvrp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/cvrp/viewer.py` & `jumanji-0.3.0/jumanji/environments/routing/cvrp/viewer.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,25 +57,29 @@
         if render_mode == "rgb_array":
             self._display = self._display_rgb_array
         elif render_mode == "human":
             self._display = self._display_human
         else:
             raise ValueError(f"Invalid render mode: {render_mode}")
 
-    def render(self, state: State) -> Optional[NDArray]:
+    def render(
+        self, state: State, save_path: Optional[str] = None
+    ) -> Optional[NDArray]:
         """Render the given state of the `CVRP` environment.
 
         Args:
             state: the environment state to render.
         """
         self._clear_display()
         fig, ax = self._get_fig_ax()
         ax.clear()
         self._prepare_figure(ax)
         self._add_tour(ax, state)
+        if save_path:
+            fig.savefig(save_path, bbox_inches="tight", pad_inches=0.2)
         return self._display(fig)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/maze/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/maze/constants.py` & `jumanji-0.3.0/jumanji/environments/routing/maze/constants.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/maze/env.py` & `jumanji-0.3.0/jumanji/environments/routing/maze/env.py`

 * *Files 9% similar despite different names*

```diff
@@ -175,42 +175,18 @@
 
         Returns:
             state: `State` object corresponding to the new state of the environment after a reset.
             timestep: `TimeStep` object corresponding the first timestep returned by the environment
                 after a reset.
         """
 
-        key, maze_key, agent_key = jax.random.split(key, 3)
+        state = self.generator(key)
 
-        walls = self.generator(maze_key)
-
-        # Randomise agent start and target positions.
-        start_and_target_indices = jax.random.choice(
-            agent_key,
-            jnp.arange(self.num_rows * self.num_cols),
-            (2,),
-            replace=False,
-            p=~walls.flatten(),
-        )
-        (agent_row, target_row), (agent_col, target_col) = jnp.divmod(
-            start_and_target_indices, self.num_cols
-        )
-
-        agent_position = Position(row=agent_row, col=agent_col)
-        target_position = Position(row=target_row, col=target_col)
-
-        # Build the state.
-        state = State(
-            agent_position=agent_position,
-            target_position=target_position,
-            walls=walls,
-            action_mask=self._compute_action_mask(walls, agent_position),
-            key=key,
-            step_count=jnp.array(0, jnp.int32),
-        )
+        # Create the action mask and update the state
+        state.action_mask = self._compute_action_mask(state.walls, state.agent_position)
 
         # Generate the observation from the environment state.
         observation = self._observation_from_state(state)
 
         # Return a restart timestep whose step type is FIRST.
         timestep = restart(observation)
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/maze/generator.py` & `jumanji-0.3.0/jumanji/environments/routing/maze/generator.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,17 +10,19 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import abc
 
 import chex
+import jax
 import jax.numpy as jnp
 
 from jumanji.environments.commons.maze_utils import maze_generation
+from jumanji.environments.routing.maze.types import Position, State
 
 
 class Generator(abc.ABC):
     def __init__(self, num_rows: int, num_cols: int):
         """Interface for maze generator.
 
         Args:
@@ -34,46 +36,85 @@
     def __call__(self, key: chex.PRNGKey) -> chex.Array:
         """Generate a problem instance.
 
         Args:
             key: random key.
 
         Returns:
-            A `Maze` representing a problem instance.
+            state: the generated state.
         """
 
 
 class ToyGenerator(Generator):
     """Generate a hardcoded 5x5 toy maze."""
 
     def __init__(self) -> None:
         super(ToyGenerator, self).__init__(num_rows=5, num_cols=5)
 
-    def __call__(self, key: chex.PRNGKey) -> chex.Array:
+    def __call__(self, key: chex.PRNGKey) -> State:
         walls = jnp.ones((self.num_rows, self.num_cols), bool)
         walls = walls.at[0, :].set((False, True, False, False, False))
         walls = walls.at[1, :].set((False, True, False, True, True))
         walls = walls.at[2, :].set((False, True, False, False, False))
         walls = walls.at[3, :].set((False, False, False, True, True))
         walls = walls.at[4, :].set((False, False, False, False, False))
-        return walls
+
+        agent_position = Position(row=0, col=0)
+        target_position = Position(row=0, col=4)
+
+        # Build the state.
+        return State(
+            agent_position=agent_position,
+            target_position=target_position,
+            walls=walls,
+            action_mask=None,
+            key=key,
+            step_count=jnp.array(0, jnp.int32),
+        )
 
 
 class RandomGenerator(Generator):
     def __init__(self, num_rows: int, num_cols: int) -> None:
         super(RandomGenerator, self).__init__(num_rows=num_rows, num_cols=num_cols)
 
-    def __call__(self, key: chex.PRNGKey) -> chex.Array:
+    def __call__(self, key: chex.PRNGKey) -> State:
         """Generate a random maze.
 
         This method relies on the `generate_maze` method from the `maze_generation` module to
         generate a maze.
 
         Args:
             key: the Jax random number generation key.
 
         Returns:
-            maze: A generated maze as an array of booleans.
+            state: the generated state.
         """
-        return maze_generation.generate_maze(self.num_cols, self.num_rows, key).astype(
-            bool
+        key, maze_key, agent_key = jax.random.split(key, 3)
+
+        walls = maze_generation.generate_maze(
+            self.num_cols, self.num_rows, maze_key
+        ).astype(bool)
+
+        # Randomise agent start and target positions.
+        start_and_target_indices = jax.random.choice(
+            agent_key,
+            jnp.arange(self.num_rows * self.num_cols),
+            (2,),
+            replace=False,
+            p=~walls.flatten(),
+        )
+        (agent_row, target_row), (agent_col, target_col) = jnp.divmod(
+            start_and_target_indices, self.num_cols
+        )
+
+        agent_position = Position(row=agent_row, col=agent_col)
+        target_position = Position(row=target_row, col=target_col)
+
+        # Build the state.
+        return State(
+            agent_position=agent_position,
+            target_position=target_position,
+            walls=walls,
+            action_mask=None,
+            key=key,
+            step_count=jnp.array(0, jnp.int32),
         )
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/maze/types.py` & `jumanji-0.3.0/jumanji/environments/routing/maze/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/maze/viewer.py` & `jumanji-0.3.0/jumanji/environments/routing/maze/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/snake/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/snake/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/snake/env.py` & `jumanji-0.3.0/jumanji/environments/routing/snake/env.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,31 +8,29 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Any, List, Optional, Sequence, Tuple
+from typing import Optional, Sequence, Tuple
 
 import chex
 import jax
 import jax.numpy as jnp
 import matplotlib
 import matplotlib.animation
 import matplotlib.artist
-import matplotlib.pyplot as plt
-from matplotlib.patches import Circle, Rectangle
 
-import jumanji
-import jumanji.environments
 from jumanji import specs
 from jumanji.env import Environment
 from jumanji.environments.routing.snake.types import Observation, Position, State
+from jumanji.environments.routing.snake.viewer import SnakeViewer
 from jumanji.types import TimeStep, restart, termination, transition
+from jumanji.viewer import Viewer
 
 
 class Snake(Environment[State]):
     """A JAX implementation of the 'Snake' game.
 
     - observation: `Observation`
         - grid: jax array (float) of shape (num_rows, num_cols, 5)
@@ -88,36 +86,38 @@
     env.render(state)
     action = env.action_spec().generate_value()
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
-    FIGURE_NAME = "Snake"
-    FIGURE_SIZE = (6.0, 6.0)
     MOVES = jnp.array([[-1, 0], [0, 1], [1, 0], [0, -1]], jnp.int32)
 
-    def __init__(self, num_rows: int = 12, num_cols: int = 12, time_limit: int = 4000):
+    def __init__(
+        self,
+        num_rows: int = 12,
+        num_cols: int = 12,
+        time_limit: int = 4000,
+        viewer: Optional[Viewer[State]] = None,
+    ):
         """Instantiates a `Snake` environment.
 
         Args:
             num_rows: number of rows of the 2D grid. Defaults to 12.
             num_cols: number of columns of the 2D grid. Defaults to 12.
             time_limit: time_limit of an episode, i.e. number of environment steps before
                 the episode ends. Defaults to 4000.
+            viewer: `Viewer` used for rendering. Defaults to `SnakeViewer`.
         """
         super().__init__()
         self.num_rows = num_rows
         self.num_cols = num_cols
         self.board_shape = (num_rows, num_cols)
         self.time_limit = time_limit
-
-        # You must store the created Animation in a variable that lives as long as the animation
-        # should run. Otherwise, the animation will get garbage-collected.
-        self._animation: Optional[matplotlib.animation.Animation] = None
+        self._viewer = viewer or SnakeViewer()
 
     def __repr__(self) -> str:
         return "\n".join(
             [
                 "Snake environment:",
                 f" - num_rows: {self.num_rows}",
                 f" - num_cols: {self.num_cols}",
@@ -376,28 +376,16 @@
         return next_head_position
 
     def render(self, state: State) -> None:
         """Render frames of the environment for a given state using matplotlib.
 
         Args:
             state: State object containing the current dynamics of the environment.
-
         """
-        self._clear_display()
-        fig, ax = self._get_fig_ax()
-        self._draw(ax, state)
-        self._update_display(fig)
-
-    def close(self) -> None:
-        """Perform any necessary cleanup.
-
-        Environments will automatically :meth:`close()` themselves when
-        garbage collected or when the program exits.
-        """
-        plt.close(self.FIGURE_NAME)
+        self._viewer.render(state)
 
     def animate(
         self,
         states: Sequence[State],
         interval: int = 200,
         save_path: Optional[str] = None,
     ) -> matplotlib.animation.FuncAnimation:
@@ -408,130 +396,16 @@
             interval: delay between frames in milliseconds, default to 200.
             save_path: the path where the animation file should be saved. If it is None, the plot
                 will not be saved.
 
         Returns:
             Animation object that can be saved as a GIF, MP4, or rendered with HTML.
         """
-        fig, ax = plt.subplots(num=f"{self.FIGURE_NAME}Anim", figsize=self.FIGURE_SIZE)
-        self._draw_board(ax)
-        plt.close(fig)
-
-        patches: List[matplotlib.patches.Patch] = []
-
-        def make_frame(state: State) -> Any:
-            while patches:
-                patches.pop().remove()
-            patches.extend(self._create_entities(state))
-            for patch in patches:
-                ax.add_patch(patch)
-
-        # Create the animation object.
-        matplotlib.rc("animation", html="jshtml")
-        self._animation = matplotlib.animation.FuncAnimation(
-            fig,
-            make_frame,
-            frames=states,
-            interval=interval,
-        )
-
-        # Save the animation as a gif.
-        if save_path:
-            self._animation.save(save_path)
-
-        return self._animation
-
-    def _get_fig_ax(self) -> Tuple[plt.Figure, plt.Axes]:
-        exists = plt.fignum_exists(self.FIGURE_NAME)
-        if exists:
-            fig = plt.figure(self.FIGURE_NAME)
-            ax = fig.get_axes()[0]
-        else:
-            fig = plt.figure(self.FIGURE_NAME, figsize=self.FIGURE_SIZE)
-            fig.set_tight_layout({"pad": False, "w_pad": 0.0, "h_pad": 0.0})
-            if not plt.isinteractive():
-                fig.show()
-            ax = fig.add_subplot()
-        return fig, ax
-
-    def _draw(self, ax: plt.Axes, state: State) -> None:
-        ax.clear()
-        self._draw_board(ax)
-        for patch in self._create_entities(state):
-            ax.add_patch(patch)
-
-    def _draw_board(self, ax: plt.Axes) -> None:
-        # Draw the square box that delimits the board.
-        ax.axis("off")
-        ax.plot([0, 0], [0, self.num_rows], "-k", lw=2)
-        ax.plot([0, self.num_cols], [self.num_rows, self.num_rows], "-k", lw=2)
-        ax.plot([self.num_cols, self.num_cols], [self.num_rows, 0], "-k", lw=2)
-        ax.plot([self.num_cols, 0], [0, 0], "-k", lw=2)
-
-    def _create_entities(self, state: State) -> List[matplotlib.patches.Patch]:
-        """Loop over the different cells and draws corresponding shapes in the ax object."""
-        patches = []
-        linewidth = (
-            min(
-                n * size
-                for n, size in zip((self.num_rows, self.num_cols), self.FIGURE_SIZE)
-            )
-            / 44.0
-        )
-        cmap = matplotlib.colors.LinearSegmentedColormap.from_list(
-            "", ["yellowgreen", "forestgreen"]
-        )
-        for row in range(self.num_rows):
-            for col in range(self.num_cols):
-                if state.body_state[row, col]:
-                    body_cell_patch = Rectangle(
-                        (col, self.num_rows - 1 - row),
-                        1,
-                        1,
-                        edgecolor=cmap(1),
-                        facecolor=cmap(state.body_state[row, col] / state.length),
-                        fill=True,
-                        lw=linewidth,
-                    )
-                    patches.append(body_cell_patch)
-        head_patch = Circle(
-            (
-                state.head_position[1] + 0.5,
-                self.num_rows - 1 - state.head_position[0] + 0.5,
-            ),
-            0.3,
-            edgecolor=cmap(0.5),
-            facecolor=cmap(0),
-            fill=True,
-            lw=linewidth,
-        )
-        patches.append(head_patch)
-        fruit_patch = Circle(
-            (
-                state.fruit_position[1] + 0.5,
-                self.num_rows - 1 - state.fruit_position[0] + 0.5,
-            ),
-            0.2,
-            edgecolor="brown",
-            facecolor="lightcoral",
-            fill=True,
-            lw=linewidth,
-        )
-        patches.append(fruit_patch)
-        return patches
-
-    def _update_display(self, fig: plt.Figure) -> None:
-        if plt.isinteractive():
-            # Required to update render when using Jupyter Notebook.
-            fig.canvas.draw()
-            if jumanji.environments.is_colab():
-                plt.show(self.FIGURE_NAME)
-        else:
-            # Required to update render when not using Jupyter Notebook.
-            fig.canvas.draw_idle()
-            fig.canvas.flush_events()
-
-    def _clear_display(self) -> None:
-        if jumanji.environments.is_colab():
-            import IPython.display
+        return self._viewer.animate(states, interval, save_path)
+
+    def close(self) -> None:
+        """Perform any necessary cleanup.
 
-            IPython.display.clear_output(True)
+        Environments will automatically :meth:`close()` themselves when
+        garbage collected or when the program exits.
+        """
+        self._viewer.close()
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/snake/types.py` & `jumanji-0.3.0/jumanji/environments/routing/snake/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/tsp/__init__.py` & `jumanji-0.3.0/jumanji/environments/routing/tsp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/tsp/env.py` & `jumanji-0.3.0/jumanji/environments/routing/tsp/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 import jax.numpy as jnp
 import matplotlib
 from chex import PRNGKey
 from numpy.typing import NDArray
 
 from jumanji import specs
 from jumanji.env import Environment
+from jumanji.environments.routing.tsp.generator import Generator, UniformGenerator
 from jumanji.environments.routing.tsp.reward import DenseReward, RewardFn
 from jumanji.environments.routing.tsp.types import Observation, State
 from jumanji.environments.routing.tsp.viewer import TSPViewer
 from jumanji.types import TimeStep, restart, termination, transition
 from jumanji.viewer import Viewer
 
 
@@ -86,30 +87,35 @@
     state, timestep = jax.jit(env.step)(state, action)
     env.render(state)
     ```
     """
 
     def __init__(
         self,
-        num_cities: int = 20,
+        generator: Optional[Generator] = None,
         reward_fn: Optional[RewardFn] = None,
         viewer: Optional[Viewer[State]] = None,
     ):
         """Instantiates a `TSP` environment.
 
         Args:
-            num_cities: number of cities to visit. Defaults to 20.
+            generator: `Generator` whose `__call__` instantiates an environment instance.
+                The default option is 'UniformGenerator' which randomly generates
+                TSP instances with 20 cities sampled from a uniform distribution.
             reward_fn: RewardFn whose `__call__` method computes the reward of an environment
                 transition. The function must compute the reward based on the current state,
                 the chosen action and the next state.
                 Implemented options are [`DenseReward`, `SparseReward`]. Defaults to `DenseReward`.
             viewer: `Viewer` used for rendering. Defaults to `TSPViewer` with "human" render mode.
         """
 
-        self.num_cities = num_cities
+        self.generator = generator or UniformGenerator(
+            num_cities=20,
+        )
+        self.num_cities = self.generator.num_cities
         self.reward_fn = reward_fn or DenseReward()
         self._viewer = viewer or TSPViewer(name="TSP", render_mode="human")
 
     def __repr__(self) -> str:
         return f"TSP environment with {self.num_cities} cities."
 
     def reset(self, key: PRNGKey) -> Tuple[State, TimeStep[Observation]]:
@@ -119,26 +125,15 @@
             key: used to randomly generate the coordinates.
 
         Returns:
             state: State object corresponding to the new state of the environment.
             timestep: TimeStep object corresponding to the first timestep returned
                 by the environment.
         """
-        key, sample_key = jax.random.split(key)
-        coordinates = jax.random.uniform(
-            sample_key, (self.num_cities, 2), minval=0, maxval=1
-        )
-        state = State(
-            coordinates=coordinates,
-            position=jnp.array(-1, jnp.int32),
-            visited_mask=jnp.zeros(self.num_cities, dtype=bool),
-            trajectory=jnp.full(self.num_cities, -1, jnp.int32),
-            num_visited=jnp.array(0, jnp.int32),
-            key=key,
-        )
+        state = self.generator(key)
         timestep = restart(observation=self._state_to_observation(state))
         return state, timestep
 
     def step(
         self, state: State, action: chex.Numeric
     ) -> Tuple[State, TimeStep[Observation]]:
         """Run one timestep of the environment's dynamics.
```

### Comparing `jumanji-0.2.2/jumanji/environments/routing/tsp/reward.py` & `jumanji-0.3.0/jumanji/environments/routing/tsp/reward.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/tsp/types.py` & `jumanji-0.3.0/jumanji/environments/routing/tsp/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/environments/routing/tsp/viewer.py` & `jumanji-0.3.0/jumanji/environments/routing/tsp/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/registration.py` & `jumanji-0.3.0/jumanji/registration.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/specs.py` & `jumanji-0.3.0/jumanji/specs.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/testing/__init__.py` & `jumanji-0.3.0/jumanji/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/testing/env_not_smoke.py` & `jumanji-0.3.0/jumanji/testing/env_not_smoke.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/testing/fakes.py` & `jumanji-0.3.0/jumanji/testing/fakes.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/testing/pytrees.py` & `jumanji-0.3.0/jumanji/testing/pytrees.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/__init__.py` & `jumanji-0.3.0/jumanji/training/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/agents/__init__.py` & `jumanji-0.3.0/jumanji/training/agents/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/agents/a2c/__init__.py` & `jumanji-0.3.0/jumanji/training/agents/a2c/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/agents/a2c/a2c_agent.py` & `jumanji-0.3.0/jumanji/training/agents/a2c/a2c_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/agents/base.py` & `jumanji-0.3.0/jumanji/training/agents/base.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/agents/random/__init__.py` & `jumanji-0.3.0/jumanji/training/agents/random/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/agents/random/random_agent.py` & `jumanji-0.3.0/jumanji/training/agents/random/random_agent.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/evaluator.py` & `jumanji-0.3.0/jumanji/training/evaluator.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,23 +35,24 @@
         eval_env: Environment,
         agent: Agent,
         total_batch_size: int,
         stochastic: bool,
     ):
         self.eval_env = eval_env
         self.agent = agent
-        num_devices = jax.local_device_count()
-        self.num_devices = num_devices
-        if total_batch_size % num_devices != 0:
+        self.num_local_devices = jax.local_device_count()
+        self.num_global_devices = jax.device_count()
+        self.num_workers = self.num_global_devices // self.num_local_devices
+        if total_batch_size % self.num_global_devices != 0:
             raise ValueError(
                 "Expected eval total_batch_size to be a multiple of num_devices, "
-                f"got {total_batch_size} and {num_devices}."
+                f"got {total_batch_size} and {self.num_global_devices}."
             )
         self.total_batch_size = total_batch_size
-        self.batch_size_per_device = total_batch_size // num_devices
+        self.batch_size_per_device = total_batch_size // self.num_global_devices
         self.generate_evaluations = jax.pmap(
             functools.partial(
                 self._generate_evaluations, eval_batch_size=self.batch_size_per_device
             ),
             axis_name="devices",
         )
         self.stochastic = stochastic
@@ -83,15 +84,15 @@
             acting_state, return_ = carry
             key, action_key = jax.random.split(acting_state.key)
             observation = jax.tree_util.tree_map(
                 lambda x: x[None], acting_state.timestep.observation
             )
             action = acting_policy(observation, action_key)
             state, timestep = self.eval_env.step(
-                acting_state.state, jnp.squeeze(action)
+                acting_state.state, jnp.squeeze(action, axis=0)
             )
             return_ += timestep.reward
             acting_state = ActingState(
                 state=state,
                 timestep=timestep,
                 key=key,
                 episode_count=jnp.array(0, jnp.int32),
@@ -147,13 +148,16 @@
 
         return eval_metrics
 
     def run_evaluation(
         self, params_state: Optional[ParamsState], eval_key: chex.PRNGKey
     ) -> Dict:
         """Run one batch of evaluations."""
-        eval_keys = jax.random.split(eval_key, self.num_devices)
+        eval_keys = jax.random.split(eval_key, self.num_global_devices).reshape(
+            self.num_workers, self.num_local_devices, -1
+        )
+        eval_keys_per_worker = eval_keys[jax.process_index()]
         eval_metrics: Dict = self.generate_evaluations(
             params_state,
-            eval_keys,
+            eval_keys_per_worker,
         )
         return eval_metrics
```

### Comparing `jumanji-0.2.2/jumanji/training/loggers.py` & `jumanji-0.3.0/jumanji/training/loggers.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,31 @@
         """Returns the local variables that are accessible in the context of the context manager.
         This function gets the locals 2 stacks above. Index 0 is this very function, 1 is the
         __init__/__exit__ level, 2 is the context manager level.
         """
         return {(k, id(v)): v for k, v in inspect.stack()[2].frame.f_locals.items()}
 
 
+class NoOpLogger(Logger):
+    """Does nothing. This logger is useful in the case of multi-node training where only the
+    master node should log.
+    """
+
+    def __init__(self) -> None:
+        super().__init__(save_checkpoint=False)
+
+    def write(
+        self,
+        data: Dict[str, Any],
+        label: Optional[str] = None,
+        env_steps: Optional[int] = None,
+    ) -> None:
+        pass
+
+
 class TerminalLogger(Logger):
     """Logs to terminal."""
 
     def __init__(
         self, name: Optional[str] = None, save_checkpoint: bool = False
     ) -> None:
         super().__init__(save_checkpoint=save_checkpoint)
```

### Comparing `jumanji-0.2.2/jumanji/training/networks/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -30,31 +30,58 @@
 from jumanji.training.networks.connector.random import make_random_policy_connector
 from jumanji.training.networks.cvrp.actor_critic import make_actor_critic_networks_cvrp
 from jumanji.training.networks.cvrp.random import make_random_policy_cvrp
 from jumanji.training.networks.game_2048.actor_critic import (
     make_actor_critic_networks_game_2048,
 )
 from jumanji.training.networks.game_2048.random import make_random_policy_game_2048
+from jumanji.training.networks.graph_coloring.actor_critic import (
+    make_actor_critic_networks_graph_coloring,
+)
+from jumanji.training.networks.graph_coloring.random import (
+    make_random_policy_graph_coloring,
+)
 from jumanji.training.networks.job_shop.actor_critic import (
     make_actor_critic_networks_job_shop,
 )
 from jumanji.training.networks.job_shop.random import make_random_policy_job_shop
 from jumanji.training.networks.knapsack.actor_critic import (
     make_actor_critic_networks_knapsack,
 )
 from jumanji.training.networks.knapsack.random import make_random_policy_knapsack
 from jumanji.training.networks.maze.actor_critic import make_actor_critic_networks_maze
 from jumanji.training.networks.maze.random import make_random_policy_maze
 from jumanji.training.networks.minesweeper.actor_critic import (
     make_actor_critic_networks_minesweeper,
 )
 from jumanji.training.networks.minesweeper.random import make_random_policy_minesweeper
+from jumanji.training.networks.mmst.actor_critic import make_actor_critic_networks_mmst
+from jumanji.training.networks.mmst.random import make_random_policy_mmst
+from jumanji.training.networks.multi_cvrp.actor_critic import (
+    make_actor_critic_networks_multicvrp,
+)
+from jumanji.training.networks.multi_cvrp.random import make_random_policy_multicvrp
+from jumanji.training.networks.robot_warehouse.actor_critic import (
+    make_actor_critic_networks_robot_warehouse,
+)
+from jumanji.training.networks.robot_warehouse.random import (
+    make_random_policy_robot_warehouse,
+)
 from jumanji.training.networks.rubiks_cube.actor_critic import (
     make_actor_critic_networks_rubiks_cube,
 )
 from jumanji.training.networks.rubiks_cube.random import make_random_policy_rubiks_cube
 from jumanji.training.networks.snake.actor_critic import (
     make_actor_critic_networks_snake,
 )
 from jumanji.training.networks.snake.random import make_random_policy_snake
+from jumanji.training.networks.sudoku.actor_critic import (
+    make_cnn_actor_critic_networks_sudoku,
+    make_equivariant_actor_critic_networks_sudoku,
+)
+from jumanji.training.networks.sudoku.random import make_random_policy_sudoku
+from jumanji.training.networks.tetris.actor_critic import (
+    make_actor_critic_networks_tetris,
+)
+from jumanji.training.networks.tetris.random import make_random_policy_tetris
 from jumanji.training.networks.tsp.actor_critic import make_actor_critic_networks_tsp
 from jumanji.training.networks.tsp.random import make_random_policy_tsp
```

### Comparing `jumanji-0.2.2/jumanji/training/networks/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/base.py` & `jumanji-0.3.0/jumanji/training/networks/base.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/bin_pack/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/bin_pack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/bin_pack/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/bin_pack/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/bin_pack/random.py` & `jumanji-0.3.0/jumanji/training/networks/bin_pack/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/cleaner/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/cleaner/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/cleaner/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/cleaner/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/cleaner/random.py` & `jumanji-0.3.0/jumanji/training/networks/cleaner/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/connector/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/connector/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/connector/actor_critic.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 import chex
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 from jumanji.environments.routing.connector import Connector, Observation
-from jumanji.environments.routing.connector.constants import (
-    AGENT_INITIAL_VALUE,
-    PATH,
-    POSITION,
-    TARGET,
+from jumanji.environments.routing.connector.constants import AGENT_INITIAL_VALUE
+from jumanji.environments.routing.connector.utils import (
+    get_path,
+    get_position,
+    get_target,
 )
 from jumanji.training.networks.actor_critic import (
     ActorCriticNetworks,
     FeedForwardNetwork,
 )
 from jumanji.training.networks.parametric_distribution import (
     MultiCategoricalParametricDistribution,
@@ -46,85 +46,94 @@
     conv_n_channels: int,
 ) -> ActorCriticNetworks:
     """Make actor-critic networks for the `Connector` environment."""
     num_values = np.asarray(connector.action_spec().num_values)
     parametric_action_distribution = MultiCategoricalParametricDistribution(
         num_values=num_values
     )
+    # num_values is of shape (num_agents,) and contains num_actions everywhere.
+    num_agents = num_values.shape[0]
+    num_actions = num_values[0]
     policy_network = make_actor_network_connector(
-        num_actions=num_values[0],
+        num_agents=num_agents,
+        num_actions=num_actions,
         transformer_num_blocks=transformer_num_blocks,
         transformer_num_heads=transformer_num_heads,
         transformer_key_size=transformer_key_size,
         transformer_mlp_units=transformer_mlp_units,
         conv_n_channels=conv_n_channels,
         env_time_limit=connector.time_limit,
     )
     value_network = make_critic_network_connector(
+        num_agents=num_agents,
         transformer_num_blocks=transformer_num_blocks,
         transformer_num_heads=transformer_num_heads,
         transformer_key_size=transformer_key_size,
         transformer_mlp_units=transformer_mlp_units,
         conv_n_channels=conv_n_channels,
         env_time_limit=connector.time_limit,
     )
     return ActorCriticNetworks(
         policy_network=policy_network,
         value_network=value_network,
         parametric_action_distribution=parametric_action_distribution,
     )
 
 
-def process_grid(grid: chex.Array) -> chex.Array:
-    def channels_for_one_agent(agent_grid: chex.Array) -> chex.Array:
+def process_grid(grid: chex.Array, num_agents: jnp.int32) -> chex.Array:
+    def channel_per_agent(agent_grid: chex.Array, agent_id: jnp.int32) -> chex.Array:
         """Concatenates two feature maps: the info of the agent and the info about all other agents
         in an indiscernible way (to keep permutation equivariance).
         """
+        agent_path = get_path(agent_id)
+        agent_target = get_target(agent_id)
+        agent_pos = get_position(agent_id)
         agent_grid = jnp.expand_dims(agent_grid, -1)
         agent_mask = (
-            (agent_grid == PATH) | (agent_grid == TARGET) | (agent_grid == POSITION)
-        )
-        agent_channel = jnp.where(
-            agent_mask,
-            agent_grid,
-            0,
-        )
+            (agent_grid == agent_path)
+            | (agent_grid == agent_target)
+            | (agent_grid == agent_pos)
+        )
+        # Only current agent's info as values: 1, 2 or 3
+        # [G, G, 1]
+        agent_channel = jnp.where(agent_mask, agent_grid - 3 * agent_id, 0)
+
+        # Collapse all other agent values into just 1, 2 or 3
         offset = AGENT_INITIAL_VALUE
         others_channel = offset + (agent_grid - offset) % 3
-        others_channel = jnp.where(
-            agent_mask | (agent_grid == 0),
-            0,
-            others_channel,
-        )
-        channels = jnp.concatenate(
-            [agent_channel, others_channel], axis=-1
-        )  # [G, G, 2]
+        # [G, G, 1]
+        others_channel = jnp.where(agent_mask | (agent_grid == 0), 0, others_channel)
+        # [G, G, 2]
+        channels = jnp.concatenate([agent_channel, others_channel], axis=-1)
         return channels
 
-    channels = jax.vmap(channels_for_one_agent)(grid)  # (N, G, G, 2)
+    # (N, G, G, 2)
+    channels = jax.vmap(channel_per_agent, (None, 0))(grid, jnp.arange(num_agents))
     return channels.astype(float)
 
 
 class ConnectorTorso(hk.Module):
     def __init__(
         self,
         transformer_num_blocks: int,
         transformer_num_heads: int,
         transformer_key_size: int,
         transformer_mlp_units: Sequence[int],
         conv_n_channels: int,
         env_time_limit: int,
+        num_agents: int,
         name: Optional[str] = None,
     ):
         super().__init__(name=name)
         self.transformer_num_blocks = transformer_num_blocks
         self.transformer_num_heads = transformer_num_heads
         self.transformer_key_size = transformer_key_size
         self.transformer_mlp_units = transformer_mlp_units
         self.model_size = transformer_num_heads * transformer_key_size
+        self.num_agents = num_agents
         self.cnn_block = hk.Sequential(
             [
                 hk.Conv2D(conv_n_channels, (3, 3), 1, padding="VALID"),
                 jax.nn.relu,
                 hk.Conv2D(conv_n_channels, (3, 3), 1, padding="VALID"),
                 jax.nn.relu,
                 hk.Conv2D(conv_n_channels, (3, 3), 1, padding="VALID"),
@@ -134,15 +143,16 @@
                 hk.Flatten(),
             ],
             name="cnn_block",
         )
         self.env_time_limit = env_time_limit
 
     def __call__(self, observation: Observation) -> chex.Array:
-        grid = jax.vmap(process_grid)(observation.grid)  # (B, N, G, G, 2)
+        # (B, N, G, G, 2)
+        grid = jax.vmap(process_grid, (0, None))(observation.grid, self.num_agents)
         embeddings = jax.vmap(self.cnn_block)(grid)  # (B, N, H)
         embeddings = self._augment_with_step_count(embeddings, observation.step_count)
 
         mlp_torso = hk.Sequential(
             [
                 hk.nets.MLP((*self.transformer_mlp_units, self.model_size)),
                 hk.LayerNorm(axis=-1, create_scale=True, create_offset=True),
@@ -175,21 +185,22 @@
         mask = jnp.expand_dims(mask, axis=-3)
         return mask
 
     def _augment_with_step_count(
         self, embeddings: chex.Array, step_count: chex.Array
     ) -> chex.Array:
         step_count = jnp.asarray(step_count / self.env_time_limit, float)
-        num_agents = embeddings.shape[-2]
+        num_agents = self.num_agents
         step_count = jnp.repeat(step_count[:, None], num_agents, axis=-1)[..., None]
         embeddings = jnp.concatenate([embeddings, step_count], axis=-1)
         return embeddings
 
 
 def make_actor_network_connector(
+    num_agents: int,
     num_actions: int,
     transformer_num_blocks: int,
     transformer_num_heads: int,
     transformer_key_size: int,
     transformer_mlp_units: Sequence[int],
     env_time_limit: int,
     conv_n_channels: int,
@@ -199,27 +210,29 @@
             transformer_num_blocks=transformer_num_blocks,
             transformer_num_heads=transformer_num_heads,
             transformer_key_size=transformer_key_size,
             transformer_mlp_units=transformer_mlp_units,
             conv_n_channels=conv_n_channels,
             env_time_limit=env_time_limit,
             name="policy_torso",
+            num_agents=num_agents,
         )
         embeddings = torso(observation)
         logits = hk.nets.MLP((*transformer_mlp_units, num_actions), name="policy_head")(
             embeddings
         )
         logits = jnp.where(observation.action_mask, logits, jnp.finfo(jnp.float32).min)
         return logits
 
     init, apply = hk.without_apply_rng(hk.transform(network_fn))
     return FeedForwardNetwork(init=init, apply=apply)
 
 
 def make_critic_network_connector(
+    num_agents: int,
     transformer_num_blocks: int,
     transformer_num_heads: int,
     transformer_key_size: int,
     transformer_mlp_units: Sequence[int],
     env_time_limit: int,
     conv_n_channels: int,
 ) -> FeedForwardNetwork:
@@ -228,14 +241,15 @@
             transformer_num_blocks=transformer_num_blocks,
             transformer_num_heads=transformer_num_heads,
             transformer_key_size=transformer_key_size,
             transformer_mlp_units=transformer_mlp_units,
             conv_n_channels=conv_n_channels,
             env_time_limit=env_time_limit,
             name="critic_torso",
+            num_agents=num_agents,
         )
         embeddings = torso(observation)
         # Sum embeddings over the sequence length (num_agents).
         agent_mask = jnp.any(observation.action_mask[..., 1:], axis=-1)
         embedding = jnp.sum(embeddings, axis=-2, where=agent_mask[..., None])
         value = hk.nets.MLP((*transformer_mlp_units, 1), name="critic_head")(embedding)
         return jnp.squeeze(value, axis=-1)
```

### Comparing `jumanji-0.2.2/jumanji/training/networks/connector/random.py` & `jumanji-0.3.0/jumanji/training/networks/connector/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/cvrp/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/cvrp/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/cvrp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/cvrp/random.py` & `jumanji-0.3.0/jumanji/training/networks/cvrp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/distribution.py` & `jumanji-0.3.0/jumanji/training/networks/distribution.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/game_2048/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/game_2048/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/game_2048/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/game_2048/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/game_2048/random.py` & `jumanji-0.3.0/jumanji/training/networks/game_2048/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/job_shop/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/graph_coloring/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/job_shop/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/job_shop/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/job_shop/random.py` & `jumanji-0.3.0/jumanji/training/networks/job_shop/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/knapsack/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/job_shop/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/knapsack/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/knapsack/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/knapsack/random.py` & `jumanji-0.3.0/jumanji/training/networks/knapsack/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/masked_categorical_random.py` & `jumanji-0.3.0/jumanji/training/networks/masked_categorical_random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/maze/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/knapsack/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/maze/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/maze/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/maze/random.py` & `jumanji-0.3.0/jumanji/training/networks/maze/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/minesweeper/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/maze/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/minesweeper/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/minesweeper/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/minesweeper/random.py` & `jumanji-0.3.0/jumanji/training/networks/minesweeper/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/parametric_distribution.py` & `jumanji-0.3.0/jumanji/training/networks/parametric_distribution.py`

 * *Files 12% similar despite different names*

```diff
@@ -45,16 +45,19 @@
             param_size: size of the parameters for the distribution
             postprocessor: bijector which is applied after sampling (in practice, it's
                 tanh or identity)
             event_ndims: rank of the distribution sample (i.e. action)
         """
         self._param_size = param_size
         self._postprocessor = postprocessor
+        if event_ndims not in [0, 1]:
+            raise ValueError(
+                f"Event ndims {event_ndims} is not supported, expected value in [0, 1]."
+            )
         self._event_ndims = event_ndims  # rank of events
-        assert event_ndims in [0, 1]
 
     @abc.abstractmethod
     def create_dist(self, parameters: chex.Array) -> Distribution:
         """Creates distribution from parameters."""
 
     @property
     def param_size(self) -> int:
@@ -87,36 +90,40 @@
     def log_prob(self, parameters: chex.Array, raw_actions: chex.Array) -> chex.Array:
         """Compute the log probability of actions."""
         dist = self.create_dist(parameters)
         log_probs = dist.log_prob(raw_actions)
         log_probs -= self._postprocessor.forward_log_det_jacobian(raw_actions)
         if self._event_ndims == 1:
             log_probs = jnp.sum(log_probs, axis=-1)  # sum over action dimension
-        else:
-            assert self._event_ndims == 0
         return log_probs
 
     def entropy(self, parameters: chex.Array, seed: chex.PRNGKey) -> chex.Array:
         """Return the entropy of the given distribution."""
         dist = self.create_dist(parameters)
         entropy = dist.entropy()
         entropy += self._postprocessor.forward_log_det_jacobian(dist.sample(seed=seed))
         if self._event_ndims == 1:
             entropy = jnp.sum(entropy, axis=-1)
-        else:
-            assert self._event_ndims == 0
         return entropy
 
     def kl_divergence(
         self, parameters: chex.Array, other_parameters: chex.Array
     ) -> chex.Array:
         """KL divergence is invariant with respect to transformation by the same bijector."""
+        if not isinstance(self._postprocessor, IdentityBijector):
+            raise ValueError(
+                f"The current post_processor used ({self._postprocessor}) is a non-identity"
+                "bijector which does not implement kl_divergence."
+            )
         dist = self.create_dist(parameters)
         other_dist = self.create_dist(other_parameters)
-        return dist.kl_divergence(other_dist)
+        kl_divergence = dist.kl_divergence(other_dist)
+        if self._event_ndims == 1:
+            kl_divergence = jnp.sum(kl_divergence, axis=-1)
+        return kl_divergence
 
 
 class CategoricalParametricDistribution(ParametricDistribution):
     """Categorical distribution for discrete action spaces."""
 
     def __init__(self, num_actions: int):
         """Initialize the distribution.
```

### Comparing `jumanji-0.2.2/jumanji/training/networks/postprocessor.py` & `jumanji-0.3.0/jumanji/training/networks/postprocessor.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/protocols.py` & `jumanji-0.3.0/jumanji/training/networks/protocols.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/rubiks_cube/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/minesweeper/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/rubiks_cube/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/rubiks_cube/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/rubiks_cube/random.py` & `jumanji-0.3.0/jumanji/training/networks/rubiks_cube/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/snake/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/mmst/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/snake/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/snake/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/snake/random.py` & `jumanji-0.3.0/jumanji/training/networks/snake/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/transformer_block.py` & `jumanji-0.3.0/jumanji/training/networks/transformer_block.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/tsp/__init__.py` & `jumanji-0.3.0/jumanji/training/networks/multi_cvrp/__init__.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/tsp/actor_critic.py` & `jumanji-0.3.0/jumanji/training/networks/tsp/actor_critic.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/networks/tsp/random.py` & `jumanji-0.3.0/jumanji/training/networks/tsp/random.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/timer.py` & `jumanji-0.3.0/jumanji/training/timer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/train.py` & `jumanji-0.3.0/jumanji/training/train.py`

 * *Files 9% similar despite different names*

```diff
@@ -79,34 +79,37 @@
             # Evaluation
             key, stochastic_eval_key, greedy_eval_key = jax.random.split(key, 3)
             # Stochastic evaluation
             with eval_timer:
                 metrics = stochastic_eval.run_evaluation(
                     training_state.params_state, stochastic_eval_key
                 )
+                jax.block_until_ready(metrics)
             logger.write(
                 data=utils.first_from_device(metrics),
                 label="eval_stochastic",
                 env_steps=env_steps,
             )
             if not isinstance(agent, RandomAgent):
                 # Greedy evaluation
                 with eval_timer:
                     metrics = greedy_eval.run_evaluation(
                         training_state.params_state, greedy_eval_key
                     )
+                    jax.block_until_ready(metrics)
                 logger.write(
                     data=utils.first_from_device(metrics),
                     label="eval_greedy",
                     env_steps=env_steps,
                 )
 
             # Training
             with train_timer:
                 training_state, metrics = epoch_fn(training_state)
+                jax.block_until_ready((training_state, metrics))
             logger.write(
                 data=utils.first_from_device(metrics),
                 label="train",
                 env_steps=env_steps,
             )
```

### Comparing `jumanji-0.2.2/jumanji/training/types.py` & `jumanji-0.3.0/jumanji/training/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/training/utils.py` & `jumanji-0.3.0/jumanji/training/utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/tree_utils.py` & `jumanji-0.3.0/jumanji/tree_utils.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/types.py` & `jumanji-0.3.0/jumanji/types.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/version.py` & `jumanji-0.3.0/jumanji/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.2.2"
+__version__ = "0.3.0"
```

### Comparing `jumanji-0.2.2/jumanji/viewer.py` & `jumanji-0.3.0/jumanji/viewer.py`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/jumanji/wrappers.py` & `jumanji-0.3.0/jumanji/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -350,15 +350,15 @@
         state_0 = tree_utils.tree_slice(state, 0)
         return super().render(state_0)
 
 
 class AutoResetWrapper(Wrapper):
     """Automatically resets environments that are done. Once the terminal state is reached,
     the state, observation, and step_type are reset. The observation and step_type of the
-    terminal TimeStep is reset to the reset observation and StepType.FIRST, respectively.
+    terminal TimeStep is reset to the reset observation and StepType.LAST, respectively.
     The reward, discount, and extras retrieved from the transition to the terminal state.
     WARNING: do not `jax.vmap` the wrapped environment (e.g. do not use with the `VmapWrapper`),
     which would lead to inefficient computation due to both the `step` and `reset` functions
     being processed each time `step` is called. Please use the `VmapAutoResetWrapper` instead.
     """
 
     def _auto_reset(
@@ -376,16 +376,15 @@
         # Make sure that the random key in the environment changes at each call to reset.
         # State is a type variable hence it does not have key type hinted, so we type ignore.
         key, _ = jax.random.split(state.key)  # type: ignore
         state, reset_timestep = self._env.reset(key)
 
         # Replace observation with reset observation.
         timestep = timestep.replace(  # type: ignore
-            observation=reset_timestep.observation,
-            step_type=reset_timestep.step_type,
+            observation=reset_timestep.observation
         )
 
         return state, timestep
 
     def step(
         self, state: State, action: chex.Array
     ) -> Tuple[State, TimeStep[Observation]]:
@@ -477,16 +476,15 @@
         # Make sure that the random key in the environment changes at each call to reset.
         # State is a type variable hence it does not have key type hinted, so we type ignore.
         key, _ = jax.random.split(state.key)
         state, reset_timestep = self._env.reset(key)
 
         # Replace observation with reset observation.
         timestep = timestep.replace(  # type: ignore
-            observation=reset_timestep.observation,
-            step_type=reset_timestep.step_type,
+            observation=reset_timestep.observation
         )
 
         return state, timestep
 
     def _maybe_reset(
         self, state: State, timestep: TimeStep
     ) -> Tuple[State, TimeStep[Observation]]:
```

### Comparing `jumanji-0.2.2/jumanji.egg-info/PKG-INFO` & `jumanji-0.3.0/jumanji.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: jumanji
-Version: 0.2.2
-Summary: A suite of diverse and challenging RL environments in JAX
+Version: 0.3.0
+Summary: A diverse suite of scalable reinforcement learning environments in JAX
 Home-page: https://github.com/instadeepai/jumanji/
 Author: InstaDeep
-Author-email: hello@instadeep.com
+Author-email: c.bonnet@instadeep.com
 License: Apache 2.0
 Keywords: reinforcement-learning python jax
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -31,42 +31,55 @@
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/)
 [![PyPI Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/jumanji)
 [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/workflows/tests_linters.yml)
 [![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![MyPy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![License](https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://opensource.org/licenses/Apache-2.0)
+[![Hugging Face](https://img.shields.io/badge/%F0%9F%A4%97-Hugging%20Face-F8D521)](https://huggingface.co/InstaDeepAI)
 
 [**Environments**](#environments-)
 | [**Installation**](#installation-)
 | [**Quickstart**](#quickstart-)
 | [**Training**](#training-%EF%B8%8F)
 | [**Citation**](#citing-jumanji-%EF%B8%8F)
 | [**Docs**](https://instadeepai.github.io/jumanji)
 ---
 
-
-<p float="left" align="center">
-  <img src="docs/env_anim/connector.gif" alt="Connector" width="30%" />
-  <img src="docs/env_anim/snake.gif" alt="Snake" width="30%" />
-  <img src="docs/env_anim/cleaner.gif" alt="Cleaner" width="30%" />
-  <img src="docs/env_anim/job_shop.gif" alt="JobShop" width="30%" />
-  <img src="docs/env_anim/bin_pack.gif" alt="BinPack" width="30%" />
-  <img src="docs/env_anim/cvrp.gif" alt="CVRP" width="30%" />
-  <img src="docs/env_anim/rubiks_cube.gif" alt="RubiksCube" width="30%" />
-  <img src="docs/env_anim/game_2048.gif" alt="Game2048" width="30%" />
-  <img src="docs/env_anim/minesweeper.gif" alt="Minesweeper" width="30%" />
-</p>
-
+<div class="collage">
+  <div class="row" align="center">
+    <img src="docs/env_anim/bin_pack.gif" alt="BinPack" width="16%">
+    <img src="docs/env_anim/cleaner.gif" alt="Cleaner" width="16%">
+    <img src="docs/env_anim/connector.gif" alt="Connector" width="16%">
+    <img src="docs/env_anim/cvrp.gif" alt="CVRP" width="16%">
+    <img src="docs/env_anim/game_2048.gif" alt="Game2048" width="16%">
+    <img src="docs/env_anim/graph_coloring.gif" alt="GraphColoring" width="16%">
+  </div>
+  <div class="row" align="center">
+    <img src="docs/env_anim/job_shop.gif" alt="JobShop" width="16%">
+    <img src="docs/env_anim/knapsack.gif" alt="Knapsack" width="16%">
+    <img src="docs/env_anim/maze.gif" alt="Maze" width="16%">
+    <img src="docs/env_anim/minesweeper.gif" alt="Minesweeper" width="16%">
+    <img src="docs/env_anim/mmst.gif" alt="MMST" width="16%">
+    <img src="docs/env_anim/multi_cvrp.gif" alt="MultiCVRP" width="16%">
+  </div>
+  <div class="row" align="center">
+    <img src="docs/env_anim/robot_warehouse.gif" alt="RobotWarehouse" width="16%">
+    <img src="docs/env_anim/rubiks_cube.gif" alt="RubiksCube" width="16%">
+    <img src="docs/env_anim/snake.gif" alt="Snake" width="16%">
+    <img src="docs/env_anim/sudoku.gif" alt="Sudoku" width="16%">
+    <img src="docs/env_anim/tetris.gif" alt="Tetris" width="16%">
+    <img src="docs/env_anim/tsp.gif" alt="Tetris" width="16%">
+  </div>
+</div>
 
 
 ## Welcome to the Jungle! 🌴
 
-Jumanji is a suite of diverse and challenging reinforcement learning (RL) environments written in
-JAX.
+Jumanji is a diverse suite of scalable reinforcement learning environments written in JAX.
 
 Jumanji is helping pioneer a new wave of hardware-accelerated research and development in the
 field of RL. Jumanji's high-speed environments enable faster iteration and large-scale
 experimentation while simultaneously reducing complexity. Originating in the Research Team at
 [InstaDeep](https://www.instadeep.com/), Jumanji is now developed jointly with the open-source
 community. To join us in these efforts, reach out, raise issues and read our
 [contribution guidelines](https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just
@@ -91,58 +104,65 @@
 [RLlib](https://docs.ray.io/en/latest/rllib/index.html), [OpenAI Gym](https://github.com/openai/gym)
 and [DeepMind-Env](https://github.com/deepmind/dm_env) through our `dm_env` and `gym` wrappers.
 - 🎓 **Examples**: guides to facilitate Jumanji's adoption and highlight the added value of
 JAX-based environments.
 - 🏎️ **Training:** example agents that can be used as inspiration for the agents one may implement
 in their research.
 
-
 ## Environments 🌍
 
 Jumanji provides a diverse range of environments ranging from simple games to NP-hard combinatorial
 problems.
 
 | Environment                              | Category | Registered Version(s)                                | Source                                                                                           | Description                                                            |
 |------------------------------------------|----------|------------------------------------------------------|--------------------------------------------------------------------------------------------------|------------------------------------------------------------------------|
-| 🔢 Game2048                              | Logic  | `Game2048-v0`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/)   | [doc](https://instadeepai.github.io/jumanji/environments/game_2048/)   |
+| 🔢 Game2048                              | Logic  | `Game2048-v1`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/)   | [doc](https://instadeepai.github.io/jumanji/environments/game_2048/)   |
+| 🎨 GraphColoring                              | Logic  | `GraphColoring-v0`                                   | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/graph_coloring/)   | [doc](https://instadeepai.github.io/jumanji/environments/graph_coloring/)   |
 | 💣 Minesweeper                           | Logic    | `Minesweeper-v0`                                     | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc](https://instadeepai.github.io/jumanji/environments/minesweeper/) |
 | 🎲 RubiksCube                            | Logic    | `RubiksCube-v0`<br/>`RubiksCube-partly-scrambled-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/rubiks_cube/) | [doc](https://instadeepai.github.io/jumanji/environments/rubiks_cube/) |
-| 📦 BinPack (3D BinPacking Problem)       | Packing  | `BinPack-v1`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/)  | [doc](https://instadeepai.github.io/jumanji/environments/bin_pack/)    |
+| ✏️ Sudoku                       | Logic    | `Sudoku-v0` <br/>`Sudoku-very-easy-v0`               | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/logic/sudoku/) | [doc](https://instadeepai.github.io/jumanji/environments/sudoku/) |
+| 📦 BinPack (3D BinPacking Problem)       | Packing  | `BinPack-v2`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/)  | [doc](https://instadeepai.github.io/jumanji/environments/bin_pack/)    |
 | 🏭 JobShop (Job Shop Scheduling Problem) | Packing  | `JobShop-v0`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/)  | [doc](https://instadeepai.github.io/jumanji/environments/job_shop/)    |
 | 🎒 Knapsack                              | Packing  | `Knapsack-v1`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/knapsack/)  | [doc](https://instadeepai.github.io/jumanji/environments/knapsack/)    |
+| ▒ Tetris                              | Packing  | `Tetris-v0`                                        | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/tetris/)  | [doc](https://instadeepai.github.io/jumanji/environments/tetris/)    |
 | 🧹 Cleaner                               | Routing  | `Cleaner-v0`                                         | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cleaner/)   | [doc](https://instadeepai.github.io/jumanji/environments/cleaner/)     |
-| :link: Connector                         | Routing  | `Connector-v0`                                       | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/connector/) | [doc](https://instadeepai.github.io/jumanji/environments/connector/)   |
+| :link: Connector                         | Routing  | `Connector-v2`                                       | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/connector/) | [doc](https://instadeepai.github.io/jumanji/environments/connector/)   |
 | 🚚 CVRP (Capacitated Vehicle Routing Problem)  | Routing  | `CVRP-v1`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cvrp/)      | [doc](https://instadeepai.github.io/jumanji/environments/cvrp/)        |
+| 🚚 MultiCVRP (Multi-Agent Capacitated Vehicle Routing Problem)  | Routing  | `MultiCVRP-v0`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/multi_cvrp/)      | [doc](https://instadeepai.github.io/jumanji/environments/multi_cvrp/)        |
 | :mag: Maze   | Routing  | `Maze-v0`                                            | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/maze/)      | [doc](https://instadeepai.github.io/jumanji/environments/maze/)        |
+| :robot: RobotWarehouse  | Routing  | `RobotWarehouse-v0`                                  | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/robot_warehouse/)      | [doc](https://instadeepai.github.io/jumanji/environments/robot_warehouse/)        |
 | 🐍 Snake                                       | Routing  | `Snake-v1`                                           | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/snake/)     | [doc](https://instadeepai.github.io/jumanji/environments/snake/)       |
 | 📬 TSP (Travelling Salesman Problem)           | Routing  | `TSP-v1`                                             | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/tsp/)       | [doc](https://instadeepai.github.io/jumanji/environments/tsp/)         |
-
+| Multi Minimum Spanning Tree Problem | Routing  | `MMST-v0`                                | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/mmst)    | [doc](https://instadeepai.github.io/jumanji/environments/mmst/)    |
 
 ## Installation 🎬
 
 You can install the latest release of Jumanji from PyPI:
+
 ```bash
 pip install jumanji
 ```
+
 Alternatively, you can install the latest development version directly from GitHub:
+
 ```bash
 pip install git+https://github.com/instadeepai/jumanji.git
 ```
+
 Jumanji has been tested on Python 3.8 and 3.9.
 Note that because the installation of JAX differs depending on your hardware accelerator,
 we advise users to explicitly install the correct JAX version (see the
 [official installation guide](https://github.com/google/jax#installation)).
 
 **Rendering:** Matplotlib is used for rendering all the environments. To visualize the environments
 you will need a GUI backend. For example, on Linux, you can install Tk via:
 `apt-get install python3-tk`, or using conda: `conda install tk`. Check out
 [Matplotlib backends](https://matplotlib.org/stable/users/explain/backends.html) for a list of
 backends you can use.
 
-
 ## Quickstart ⚡
 
 RL practitioners will find Jumanji's interface familiar as it combines the widely adopted
 [OpenAI Gym](https://github.com/openai/gym) and
 [DeepMind Environment](https://github.com/deepmind/dm_env) interfaces. From OpenAI Gym, we adopted
 the idea of a `registry` and the `render` method, while our `TimeStep` structure is inspired by
 DeepMind Environment.
@@ -191,15 +211,14 @@
 We maintain a registry of standard environments with their configuration.
 For each environment, a version suffix is appended, e.g. `Snake-v1`.
 When changes are made to environments that might impact learning results,
 the version number is incremented by one to prevent potential confusion.
 For a full list of registered versions of each environment, check out
 [the documentation](https://instadeepai.github.io/jumanji/environments/tsp/).
 
-
 ## Training 🏎️
 
 To showcase how to train RL agents on Jumanji environments, we provide a random agent and a vanilla
 actor-critic (A2C) agent. These agents can be found in
 [jumanji/training/](https://github.com/instadeepai/jumanji/tree/main/jumanji/training/).
 
 Because the environment framework in Jumanji is so flexible, it allows pretty much any problem to
@@ -212,40 +231,38 @@
 > ⚠️ The example agents in `jumanji/training` are **only** meant to serve as inspiration for how one
 > can implement an agent. Jumanji is first and foremost a library of environments - as such, the
 > agents and networks will **not** be maintained to a production standard.
 
 For more information on how to use the example agents, see the
 [training guide](https://instadeepai.github.io/jumanji/guides/training/).
 
-
 ## Contributing 🤝
 
 Contributions are welcome! See our issue tracker for
 [good first issues](https://github.com/instadeepai/jumanji/labels/good%20first%20issue). Please read
 our [contributing guidelines](https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) for
 details on how to submit pull requests, our Contributor License Agreement, and community guidelines.
 
-
 ## Citing Jumanji ✏️
 
 If you use Jumanji in your work, please cite the library using:
+
 ```
 @software{jumanji2023github,
   author = {Clément Bonnet and Daniel Luo and Donal Byrne and Sasha Abramowitz
         and Vincent Coyette and Paul Duckworth and Daniel Furelos-Blanco and
         Nathan Grinsztajn and Tristan Kalloniatis and Victor Le and Omayma Mahjoub
         and Laurence Midgley and Shikha Surana and Cemlyn Waters and Alexandre Laterre},
   title = {Jumanji: a Suite of Diverse and Challenging Reinforcement Learning Environments in JAX},
   url = {https://github.com/instadeepai/jumanji},
   version = {0.2.2},
   year = {2023},
 }
 ```
 
-
 ## See Also 🔎
 
 Other works have embraced the approach of writing RL environments in JAX.
 In particular, we suggest users check out the following sister repositories:
 
 - 🤖 [Qdax](https://github.com/adaptive-intelligent-robotics/QDax) is a library to accelerate
 Quality-Diversity and neuro-evolution algorithms through hardware accelerators and parallelization.
```

#### html2text {}

```diff
@@ -1,49 +1,52 @@
-Metadata-Version: 2.1 Name: jumanji Version: 0.2.2 Summary: A suite of diverse
-and challenging RL environments in JAX Home-page: https://github.com/
-instadeepai/jumanji/ Author: InstaDeep Author-email: hello@instadeep.com
-License: Apache 2.0 Keywords: reinforcement-learning python jax Classifier:
-Development Status :: 4 - Beta Classifier: Environment :: Console Classifier:
-Intended Audience :: Science/Research Classifier: Intended Audience ::
-Developers Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra:
-dev Provides-Extra: train License-File: LICENSE
+Metadata-Version: 2.1 Name: jumanji Version: 0.3.0 Summary: A diverse suite of
+scalable reinforcement learning environments in JAX Home-page: https://
+github.com/instadeepai/jumanji/ Author: InstaDeep Author-email:
+c.bonnet@instadeep.com License: Apache 2.0 Keywords: reinforcement-learning
+python jax Classifier: Development Status :: 4 - Beta Classifier: Environment
+:: Console Classifier: Intended Audience :: Science/Research Classifier:
+Intended Audience :: Developers Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Topic :: Scientific/Engineering ::
+Artificial Intelligence Classifier: Topic :: Software Development :: Libraries
+:: Python Modules Classifier: License :: OSI Approved :: Apache Software
+License Requires-Python: >=3.8 Description-Content-Type: text/markdown
+Provides-Extra: dev Provides-Extra: train License-File: LICENSE
                                 [Jumanji_logo]
 [![Python Versions](https://img.shields.io/pypi/pyversions/
 jumanji.svg?style=flat-square)](https://www.python.org/doc/versions/) [![PyPI
 Version](https://badge.fury.io/py/jumanji.svg)](https://badge.fury.io/py/
 jumanji) [![Tests](https://github.com/instadeepai/jumanji/actions/workflows/
 tests_linters.yml/badge.svg)](https://github.com/instadeepai/jumanji/actions/
 workflows/tests_linters.yml) [![Code Style](https://img.shields.io/badge/
 code%20style-black-000000.svg)](https://github.com/psf/black) [![MyPy](http://
 www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/) [![License]
 (https://img.shields.io/badge/License-Apache%202.0-orange.svg)](https://
-opensource.org/licenses/Apache-2.0) [**Environments**](#environments-) |
-[**Installation**](#installation-) | [**Quickstart**](#quickstart-) |
-[**Training**](#training-%EF%B8%8F) | [**Citation**](#citing-jumanji-%EF%B8%8F)
-| [**Docs**](https://instadeepai.github.io/jumanji) ---
-    [Connector] [Snake] [Cleaner] [JobShop] [BinPack] [CVRP] [RubiksCube]
-                           [Game2048] [Minesweeper]
-## Welcome to the Jungle! ð´ Jumanji is a suite of diverse and challenging
-reinforcement learning (RL) environments written in JAX. Jumanji is helping
-pioneer a new wave of hardware-accelerated research and development in the
-field of RL. Jumanji's high-speed environments enable faster iteration and
-large-scale experimentation while simultaneously reducing complexity.
-Originating in the Research Team at [InstaDeep](https://www.instadeep.com/),
-Jumanji is now developed jointly with the open-source community. To join us in
-these efforts, reach out, raise issues and read our [contribution guidelines]
-(https://github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just
-[star](https://github.com/instadeepai/jumanji) ð to stay up to date with the
-latest developments! ### Goals ð 1. Provide a simple, well-tested API for
-JAX-based environments. 2. Make research in RL more accessible. 3. Facilitate
-the research on RL for problems in the industry and help close the gap between
+opensource.org/licenses/Apache-2.0) [![Hugging Face](https://img.shields.io/
+badge/%F0%9F%A4%97-Hugging%20Face-F8D521)](https://huggingface.co/InstaDeepAI)
+[**Environments**](#environments-) | [**Installation**](#installation-) |
+[**Quickstart**](#quickstart-) | [**Training**](#training-%EF%B8%8F) |
+[**Citation**](#citing-jumanji-%EF%B8%8F) | [**Docs**](https://
+instadeepai.github.io/jumanji) ---
+       [BinPack] [Cleaner] [Connector] [CVRP] [Game2048] [GraphColoring]
+         [JobShop] [Knapsack] [Maze] [Minesweeper] [MMST] [MultiCVRP]
+       [RobotWarehouse] [RubiksCube] [Snake] [Sudoku] [Tetris] [Tetris]
+## Welcome to the Jungle! ð´ Jumanji is a diverse suite of scalable
+reinforcement learning environments written in JAX. Jumanji is helping pioneer
+a new wave of hardware-accelerated research and development in the field of RL.
+Jumanji's high-speed environments enable faster iteration and large-scale
+experimentation while simultaneously reducing complexity. Originating in the
+Research Team at [InstaDeep](https://www.instadeep.com/), Jumanji is now
+developed jointly with the open-source community. To join us in these efforts,
+reach out, raise issues and read our [contribution guidelines](https://
+github.com/instadeepai/jumanji/blob/main/CONTRIBUTING.md) or just [star](https:
+//github.com/instadeepai/jumanji) ð to stay up to date with the latest
+developments! ### Goals ð 1. Provide a simple, well-tested API for JAX-based
+environments. 2. Make research in RL more accessible. 3. Facilitate the
+research on RL for problems in the industry and help close the gap between
 research and industrial applications. 4. Provide environments whose difficulty
 can be scaled to be arbitrarily hard. ### Overview ð¦ - ð¥ **Environment
 API**: core abstractions for JAX-based environments. - ð¹ï¸ **Environment
 Suite**: a collection of RL environments ranging from simple games to NP-hard
 combinatorial problems. - ð¬ **Wrappers**: easily connect to your favourite
 RL frameworks and libraries such as [Acme](https://github.com/deepmind/acme),
 [Stable Baselines3](https://github.com/DLR-RM/stable-baselines3), [RLlib]
@@ -55,67 +58,86 @@
 inspiration for the agents one may implement in their research. ## Environments
 ð Jumanji provides a diverse range of environments ranging from simple games
 to NP-hard combinatorial problems. | Environment | Category | Registered
 Version(s) | Source | Description | |------------------------------------------
 |----------|------------------------------------------------------|------------
 -------------------------------------------------------------------------------
 -------|-----------------------------------------------------------------------
--| | ð¢ Game2048 | Logic | `Game2048-v0` | [code](https://github.com/
+-| | ð¢ Game2048 | Logic | `Game2048-v1` | [code](https://github.com/
 instadeepai/jumanji/tree/main/jumanji/environments/logic/game_2048/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/game_2048/) | | ð£
-Minesweeper | Logic | `Minesweeper-v0` | [code](https://github.com/instadeepai/
-jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc](https://
-instadeepai.github.io/jumanji/environments/minesweeper/) | | ð² RubiksCube |
-Logic | `RubiksCube-v0`
+(https://instadeepai.github.io/jumanji/environments/game_2048/) | | ð¨
+GraphColoring | Logic | `GraphColoring-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/logic/graph_coloring/) |
+[doc](https://instadeepai.github.io/jumanji/environments/graph_coloring/) | |
+ð£ Minesweeper | Logic | `Minesweeper-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/logic/minesweeper/) | [doc]
+(https://instadeepai.github.io/jumanji/environments/minesweeper/) | | ð²
+RubiksCube | Logic | `RubiksCube-v0`
 `RubiksCube-partly-scrambled-v0` | [code](https://github.com/instadeepai/
 jumanji/tree/main/jumanji/environments/logic/rubiks_cube/) | [doc](https://
-instadeepai.github.io/jumanji/environments/rubiks_cube/) | | ð¦ BinPack (3D
-BinPacking Problem) | Packing | `BinPack-v1` | [code](https://github.com/
-instadeepai/jumanji/tree/main/jumanji/environments/packing/bin_pack/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/bin_pack/) | | ð­ JobShop
-(Job Shop Scheduling Problem) | Packing | `JobShop-v0` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/
-) | [doc](https://instadeepai.github.io/jumanji/environments/job_shop/) | |
-ð Knapsack | Packing | `Knapsack-v1` | [code](https://github.com/
-instadeepai/jumanji/tree/main/jumanji/environments/packing/knapsack/) | [doc]
-(https://instadeepai.github.io/jumanji/environments/knapsack/) | | ð§¹ Cleaner
-| Routing | `Cleaner-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/cleaner/) | [doc](https://
-instadeepai.github.io/jumanji/environments/cleaner/) | | :link: Connector |
-Routing | `Connector-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/connector/) | [doc](https://
-instadeepai.github.io/jumanji/environments/connector/) | | ð CVRP
-(Capacitated Vehicle Routing Problem) | Routing | `CVRP-v1` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/cvrp/) |
-[doc](https://instadeepai.github.io/jumanji/environments/cvrp/) | | :mag: Maze
-| Routing | `Maze-v0` | [code](https://github.com/instadeepai/jumanji/tree/
-main/jumanji/environments/routing/maze/) | [doc](https://instadeepai.github.io/
-jumanji/environments/maze/) | | ð Snake | Routing | `Snake-v1` | [code]
-(https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/
-snake/) | [doc](https://instadeepai.github.io/jumanji/environments/snake/) | |
-ð¬ TSP (Travelling Salesman Problem) | Routing | `TSP-v1` | [code](https://
-github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/tsp/) |
-[doc](https://instadeepai.github.io/jumanji/environments/tsp/) | ##
-Installation ð¬ You can install the latest release of Jumanji from PyPI:
-```bash pip install jumanji ``` Alternatively, you can install the latest
-development version directly from GitHub: ```bash pip install git+https://
-github.com/instadeepai/jumanji.git ``` Jumanji has been tested on Python 3.8
-and 3.9. Note that because the installation of JAX differs depending on your
-hardware accelerator, we advise users to explicitly install the correct JAX
-version (see the [official installation guide](https://github.com/google/
-jax#installation)). **Rendering:** Matplotlib is used for rendering all the
-environments. To visualize the environments you will need a GUI backend. For
-example, on Linux, you can install Tk via: `apt-get install python3-tk`, or
-using conda: `conda install tk`. Check out [Matplotlib backends](https://
-matplotlib.org/stable/users/explain/backends.html) for a list of backends you
-can use. ## Quickstart â¡ RL practitioners will find Jumanji's interface
-familiar as it combines the widely adopted [OpenAI Gym](https://github.com/
-openai/gym) and [DeepMind Environment](https://github.com/deepmind/dm_env)
-interfaces. From OpenAI Gym, we adopted the idea of a `registry` and the
-`render` method, while our `TimeStep` structure is inspired by DeepMind
+instadeepai.github.io/jumanji/environments/rubiks_cube/) | | âï¸ Sudoku |
+Logic | `Sudoku-v0`
+`Sudoku-very-easy-v0` | [code](https://github.com/instadeepai/jumanji/tree/
+main/jumanji/environments/logic/sudoku/) | [doc](https://instadeepai.github.io/
+jumanji/environments/sudoku/) | | ð¦ BinPack (3D BinPacking Problem) |
+Packing | `BinPack-v2` | [code](https://github.com/instadeepai/jumanji/tree/
+main/jumanji/environments/packing/bin_pack/) | [doc](https://
+instadeepai.github.io/jumanji/environments/bin_pack/) | | ð­ JobShop (Job
+Shop Scheduling Problem) | Packing | `JobShop-v0` | [code](https://github.com/
+instadeepai/jumanji/tree/main/jumanji/environments/packing/job_shop/) | [doc]
+(https://instadeepai.github.io/jumanji/environments/job_shop/) | | ð
+Knapsack | Packing | `Knapsack-v1` | [code](https://github.com/instadeepai/
+jumanji/tree/main/jumanji/environments/packing/knapsack/) | [doc](https://
+instadeepai.github.io/jumanji/environments/knapsack/) | | â Tetris | Packing
+| `Tetris-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/packing/tetris/) | [doc](https://instadeepai.github.io/
+jumanji/environments/tetris/) | | ð§¹ Cleaner | Routing | `Cleaner-v0` |
+[code](https://github.com/instadeepai/jumanji/tree/main/jumanji/environments/
+routing/cleaner/) | [doc](https://instadeepai.github.io/jumanji/environments/
+cleaner/) | | :link: Connector | Routing | `Connector-v2` | [code](https://
+github.com/instadeepai/jumanji/tree/main/jumanji/environments/routing/
+connector/) | [doc](https://instadeepai.github.io/jumanji/environments/
+connector/) | | ð CVRP (Capacitated Vehicle Routing Problem) | Routing |
+`CVRP-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/
+environments/routing/cvrp/) | [doc](https://instadeepai.github.io/jumanji/
+environments/cvrp/) | | ð MultiCVRP (Multi-Agent Capacitated Vehicle Routing
+Problem) | Routing | `MultiCVRP-v0` | [code](https://github.com/instadeepai/
+jumanji/tree/main/jumanji/environments/routing/multi_cvrp/) | [doc](https://
+instadeepai.github.io/jumanji/environments/multi_cvrp/) | | :mag: Maze |
+Routing | `Maze-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/maze/) | [doc](https://instadeepai.github.io/
+jumanji/environments/maze/) | | :robot: RobotWarehouse | Routing |
+`RobotWarehouse-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/robot_warehouse/) | [doc](https://
+instadeepai.github.io/jumanji/environments/robot_warehouse/) | | ð Snake |
+Routing | `Snake-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/snake/) | [doc](https://instadeepai.github.io/
+jumanji/environments/snake/) | | ð¬ TSP (Travelling Salesman Problem) |
+Routing | `TSP-v1` | [code](https://github.com/instadeepai/jumanji/tree/main/
+jumanji/environments/routing/tsp/) | [doc](https://instadeepai.github.io/
+jumanji/environments/tsp/) | | Multi Minimum Spanning Tree Problem | Routing |
+`MMST-v0` | [code](https://github.com/instadeepai/jumanji/tree/main/jumanji/
+environments/routing/mmst) | [doc](https://instadeepai.github.io/jumanji/
+environments/mmst/) | ## Installation ð¬ You can install the latest release
+of Jumanji from PyPI: ```bash pip install jumanji ``` Alternatively, you can
+install the latest development version directly from GitHub: ```bash pip
+install git+https://github.com/instadeepai/jumanji.git ``` Jumanji has been
+tested on Python 3.8 and 3.9. Note that because the installation of JAX differs
+depending on your hardware accelerator, we advise users to explicitly install
+the correct JAX version (see the [official installation guide](https://
+github.com/google/jax#installation)). **Rendering:** Matplotlib is used for
+rendering all the environments. To visualize the environments you will need a
+GUI backend. For example, on Linux, you can install Tk via: `apt-get install
+python3-tk`, or using conda: `conda install tk`. Check out [Matplotlib
+backends](https://matplotlib.org/stable/users/explain/backends.html) for a list
+of backends you can use. ## Quickstart â¡ RL practitioners will find Jumanji's
+interface familiar as it combines the widely adopted [OpenAI Gym](https://
+github.com/openai/gym) and [DeepMind Environment](https://github.com/deepmind/
+dm_env) interfaces. From OpenAI Gym, we adopted the idea of a `registry` and
+the `render` method, while our `TimeStep` structure is inspired by DeepMind
 Environment. ### Basic Usage ð§âð» ```python import jax import jumanji #
 Instantiate a Jumanji environment using the registry env = jumanji.make('Snake-
 v1') # Reset your (jit-able) environment key = jax.random.PRNGKey(0) state,
 timestep = jax.jit(env.reset)(key) # (Optional) Render the env state env.render
 (state) # Interact with the (jit-able) environment action = env.action_spec
 ().generate_value() # Action selection (dummy value here) state, timestep =
 jax.jit(env.step)(state, action) # Take a step and observe the next state and
```

### Comparing `jumanji-0.2.2/pyproject.toml` & `jumanji-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/setup.cfg` & `jumanji-0.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `jumanji-0.2.2/setup.py` & `jumanji-0.3.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     return dict_["__version__"]
 
 
 setup(
     name="jumanji",
     version=_get_version(),
     author="InstaDeep",
-    author_email="hello@instadeep.com",
-    description="A suite of diverse and challenging RL environments in JAX",
+    author_email="c.bonnet@instadeep.com",
+    description="A diverse suite of scalable reinforcement learning environments in JAX",
     license="Apache 2.0",
     url="https://github.com/instadeepai/jumanji/",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     keywords="reinforcement-learning python jax",
     packages=setuptools.find_packages(),
     python_requires=">=3.8",
```

