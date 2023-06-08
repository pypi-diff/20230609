# Comparing `tmp/metaphor-sqllineage-2.0.8.tar.gz` & `tmp/metaphor-sqllineage-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaphor-sqllineage-2.0.8.tar", last modified: Tue Mar 14 21:29:52 2023, max compression
+gzip compressed data, was "metaphor-sqllineage-2.0.9.tar", last modified: Thu Mar 16 16:52:38 2023, max compression
```

## Comparing `metaphor-sqllineage-2.0.8.tar` & `metaphor-sqllineage-2.0.9.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.303275 metaphor-sqllineage-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-14 21:29:52.303275 metaphor-sqllineage-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.283274 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-14 21:29:52.000000 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-14 21:29:52.000000 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 21:29:52.000000 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-14 21:29:52.000000 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-14 21:29:52.000000 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-14 21:29:52.000000 metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 21:29:52.303275 metaphor-sqllineage-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.283274 metaphor-sqllineage-2.0.8/sqllineage/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.283274 metaphor-sqllineage-2.0.8/sqllineage/core/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.287274 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/cte.py
--rw-r--r--   0 runner    (1001) docker     (123)     8513 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/holders.py
--rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.283274 metaphor-sqllineage-2.0.8/sqllineage/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.295275 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query02.sql
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query03.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query04.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query05.sql
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query06.sql
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query07.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query08.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query09.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query10.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query11.sql
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query12.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query13.sql
--rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query14.sql
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query15.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query16.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query17.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query18.sql
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query19.sql
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query20.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query21.sql
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query22.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query23.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query24.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query25.sql
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query26.sql
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query27.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query28.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query29.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query30.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query31.sql
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query32.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query33.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query34.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query35.sql
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query36.sql
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query37.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query38.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query39.sql
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query40.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query41.sql
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query42.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query43.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query44.sql
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query45.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query46.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query47.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query48.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query49.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query50.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query51.sql
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query52.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query53.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query54.sql
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query55.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query56.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query57.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query58.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query59.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query60.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query61.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query62.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query63.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query64.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query65.sql
--rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query66.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query67.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query68.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query69.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query70.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query71.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query72.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query73.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query74.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query75.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query76.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query77.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query78.sql
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query79.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query80.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query81.sql
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query82.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query83.sql
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query84.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query85.sql
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query86.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query87.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query88.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query89.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query90.sql
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query91.sql
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query92.sql
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query93.sql
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query94.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query95.sql
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query96.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query97.sql
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query98.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query99.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.295275 metaphor-sqllineage-2.0.8/sqllineage/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/utils/schemaFetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineage/utils/sqlparse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/config-overrides.js
--rw-r--r--   0 runner    (1001) docker     (123)  1249041 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/public/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/public/logo192.png
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/public/logo512.png
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/App.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/api/client.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/src/app/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/app/store.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.283274 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/Directory.js
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/DirectoryTreeItem.js
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/directorySlice.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/
--rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/DAG.js
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/DAGDesc.js
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/Editor.js
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/editorSlice.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 21:29:52.299275 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/widget/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/widget/LoadError.js
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/features/widget/Loading.js
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-14 21:29:42.000000 metaphor-sqllineage-2.0.8/sqllineagejs/src/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.657485 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-03-16 16:52:38.000000 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-03-16 16:52:38.000000 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:52:38.000000 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-16 16:52:38.000000 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-16 16:52:38.000000 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-16 16:52:38.000000 metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.657485 metaphor-sqllineage-2.0.9/sqllineage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.657485 metaphor-sqllineage-2.0.9/sqllineage/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.657485 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/cte.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12083 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17222 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.657485 metaphor-sqllineage-2.0.9/sqllineage/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.669485 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query02.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query03.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6696 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query04.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query05.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query06.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query07.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query08.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query09.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query10.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query11.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query12.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query13.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     9021 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query14.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query15.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query16.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query17.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query18.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query19.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query20.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query21.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query22.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4349 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query23.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query24.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query25.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query26.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query27.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query28.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query29.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query30.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query31.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query32.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query33.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query34.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query35.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query36.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query37.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query38.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query39.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query40.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query41.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query42.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query43.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query44.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query45.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query46.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query47.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query48.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query49.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query50.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query51.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query52.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query53.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query54.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query55.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query56.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query57.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2780 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query58.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query59.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query60.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query61.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query62.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query63.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query64.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query65.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    13205 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query66.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query67.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query68.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query69.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query70.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query71.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query72.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query73.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query74.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query75.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query76.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query77.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query78.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query79.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query80.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query81.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query82.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query83.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query84.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query85.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query86.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query87.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query88.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query89.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query90.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query91.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query92.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query93.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query94.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query95.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query96.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query97.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query98.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query99.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7284 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.669485 metaphor-sqllineage-2.0.9/sqllineage/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/utils/schemaFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineage/utils/sqlparse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.669485 metaphor-sqllineage-2.0.9/sqllineagejs/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/config-overrides.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1249041 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.669485 metaphor-sqllineage-2.0.9/sqllineagejs/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/sqllineagejs/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/App.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/sqllineagejs/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/api/client.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/sqllineagejs/src/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/app/store.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.657485 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/Directory.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/DirectoryTreeItem.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/directorySlice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/
+-rw-r--r--   0 runner    (1001) docker     (123)    12152 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/DAG.js
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/DAGDesc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/Editor.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/editorSlice.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:52:38.673485 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/widget/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/widget/LoadError.js
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/features/widget/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-03-16 16:52:29.000000 metaphor-sqllineage-2.0.9/sqllineagejs/src/index.js
```

### Comparing `metaphor-sqllineage-2.0.8/LICENSE` & `metaphor-sqllineage-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/PKG-INFO` & `metaphor-sqllineage-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-sqllineage
-Version: 2.0.8
+Version: 2.0.9
 Summary: SQL Lineage Analysis Tool powered by Python
 Home-page: https://github.com/reata/sqllineage
 Author: Reata
 Author-email: reddevil.hjw@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metaphor-sqllineage-2.0.8/README.md` & `metaphor-sqllineage-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/PKG-INFO` & `metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaphor-sqllineage
-Version: 2.0.8
+Version: 2.0.9
 Summary: SQL Lineage Analysis Tool powered by Python
 Home-page: https://github.com/reata/sqllineage
 Author: Reata
 Author-email: reddevil.hjw@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `metaphor-sqllineage-2.0.8/metaphor_sqllineage.egg-info/SOURCES.txt` & `metaphor-sqllineage-2.0.9/metaphor_sqllineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/setup.py` & `metaphor-sqllineage-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/__init__.py` & `metaphor-sqllineage-2.0.9/sqllineage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # when imported by setup.py for constant variables, dependency is not ready yet
         pass
 
 
 _monkey_patch()
 
 NAME = "metaphor-sqllineage"
-VERSION = "2.0.8"
+VERSION = "2.0.9"
 DEFAULT_LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {"default": {"format": "%(levelname)s: %(message)s"}},
     "handlers": {
         "console": {
             "level": "WARNING",
```

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/cli.py` & `metaphor-sqllineage-2.0.9/sqllineage/cli.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/analyzer.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/handlers/base.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/handlers/base.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/handlers/cte.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/handlers/cte.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/handlers/source.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/handlers/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,17 +43,19 @@
     def _indicate(self, token: Token) -> bool:
         if token.normalized in ("UNION", "UNION ALL"):
             self.union_barriers.append((len(self.columns), len(self.tables)))
 
         if any(re.match(regex, token.normalized) for regex in self.SOURCE_TABLE_TOKENS):
             self.column_flag = False
             return True
-        elif bool(token.normalized == "SELECT"):
+        elif token.normalized == "SELECT":
             self.column_flag = True
             return True
+        elif token.normalized == "DISTINCT" and self.column_flag:
+            return True
         else:
             return False
 
     def _handle(self, token: Token, holder: SubQueryLineageHolder) -> None:
         if self.column_flag:
             self._handle_column(token)
         else:
```

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/handlers/swap_partition.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/handlers/target.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/handlers/target.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/holders.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/holders.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/core/models.py` & `metaphor-sqllineage-2.0.9/sqllineage/core/models.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query01.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query01.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query02.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query02.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query04.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query04.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query05.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query05.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query06.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query06.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query07.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query07.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query08.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query08.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query09.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query09.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query10.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query10.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query11.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query11.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query12.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query12.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query13.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query13.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query14.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query14.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query15.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query15.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query16.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query16.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query17.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query17.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query18.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query18.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query19.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query19.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query20.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query20.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query21.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query21.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query23.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query23.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query24.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query24.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query25.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query25.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query26.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query26.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query27.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query27.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query28.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query28.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query29.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query29.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query30.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query30.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query31.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query31.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query32.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query32.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query33.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query33.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query34.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query34.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query35.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query35.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query36.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query36.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query37.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query37.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query38.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query38.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query39.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query39.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query40.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query40.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query41.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query41.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query42.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query42.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query43.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query43.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query44.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query44.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query45.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query45.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query46.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query46.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query47.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query47.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query48.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query48.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query49.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query49.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query50.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query50.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query51.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query51.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query52.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query52.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query53.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query53.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query54.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query54.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query56.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query56.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query57.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query57.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query58.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query58.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query59.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query59.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query60.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query60.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query61.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query61.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query62.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query62.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query63.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query63.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query64.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query64.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query65.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query65.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query66.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query66.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query67.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query67.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query68.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query68.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query69.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query69.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query70.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query70.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query71.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query71.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query72.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query72.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query73.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query73.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query74.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query74.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query75.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query75.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query76.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query76.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query77.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query77.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query78.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query78.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query79.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query79.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query80.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query80.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query81.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query81.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query82.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query82.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query83.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query83.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query84.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query84.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query85.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query85.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query86.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query86.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query87.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query87.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query88.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query88.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query89.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query89.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query90.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query90.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query91.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query91.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query92.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query92.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query93.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query93.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query94.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query94.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query95.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query95.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query97.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query97.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query98.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query98.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/data/tpcds/query99.sql` & `metaphor-sqllineage-2.0.9/sqllineage/data/tpcds/query99.sql`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/drawing.py` & `metaphor-sqllineage-2.0.9/sqllineage/drawing.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/io.py` & `metaphor-sqllineage-2.0.9/sqllineage/io.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/runner.py` & `metaphor-sqllineage-2.0.9/sqllineage/runner.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/utils/helpers.py` & `metaphor-sqllineage-2.0.9/sqllineage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/utils/schemaFetcher.py` & `metaphor-sqllineage-2.0.9/sqllineage/utils/schemaFetcher.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineage/utils/sqlparse.py` & `metaphor-sqllineage-2.0.9/sqllineage/utils/sqlparse.py`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/package-lock.json` & `metaphor-sqllineage-2.0.9/sqllineagejs/package-lock.json`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/package.json` & `metaphor-sqllineage-2.0.9/sqllineagejs/package.json`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/public/favicon.ico` & `metaphor-sqllineage-2.0.9/sqllineagejs/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/public/index.html` & `metaphor-sqllineage-2.0.9/sqllineagejs/public/index.html`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/public/logo192.png` & `metaphor-sqllineage-2.0.9/sqllineagejs/public/logo192.png`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/public/logo512.png` & `metaphor-sqllineage-2.0.9/sqllineagejs/public/logo512.png`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/App.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/App.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/api/client.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/api/client.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/Directory.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/Directory.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/DirectoryTreeItem.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/DirectoryTreeItem.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/directory/directorySlice.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/directory/directorySlice.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/DAG.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/DAG.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/DAGDesc.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/DAGDesc.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/Editor.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/Editor.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/editor/editorSlice.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/editor/editorSlice.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/widget/LoadError.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/widget/LoadError.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/features/widget/Loading.js` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/features/widget/Loading.js`

 * *Files identical despite different names*

### Comparing `metaphor-sqllineage-2.0.8/sqllineagejs/src/index.css` & `metaphor-sqllineage-2.0.9/sqllineagejs/src/index.css`

 * *Files identical despite different names*

