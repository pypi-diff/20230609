# Comparing `tmp/pyproj-3.5.0rc0.tar.gz` & `tmp/pyproj-3.6.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproj-3.5.0rc0.tar", last modified: Sat Mar 25 02:01:32 2023, max compression
+gzip compressed data, was "pyproj-3.6.0rc0.tar", last modified: Fri Jun  9 01:25:20 2023, max compression
```

## Comparing `pyproj-3.5.0rc0.tar` & `pyproj-3.6.0rc0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.773213 pyproj-3.5.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/LICENSE_proj
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-03-25 02:01:32.773213 pyproj-3.5.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    27206 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.761212 pyproj-3.5.0rc0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9642 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/advanced_examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.761212 pyproj-3.5.0rc0/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/aoi.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.761212 pyproj-3.5.0rc0/docs/api/crs/
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/crs/coordinate_operation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/crs/coordinate_system.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/crs/crs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/crs/datum.rst
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/crs/enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/crs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/database.rst
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/datadir.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/geod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/global_context.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/list.rst
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/network.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/proj.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/show_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/sync.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/api/transformer.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/build_crs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/build_crs_cf.rst
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/crs_compatibility.rst
--rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/gotchas.rst
--rw-r--r--   0 runner    (1001) docker     (123)    25958 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.761212 pyproj-3.5.0rc0/docs/media/
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/media/icon.png
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/media/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/media/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/media/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/optimize_transformations.rst
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/past_versions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/docs/transformation_grids.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.765212 pyproj-3.5.0rc0/pyproj/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_compat.pxd
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_compat.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_compat.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_crs.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_crs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    91216 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_crs.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_datadir.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_datadir.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_datadir.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_geod.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_geod.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    20948 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_geod.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_network.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_network.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_sync.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_sync.pyx
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_transformer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_transformer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    39775 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/_transformer.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/base.pxi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.769213 pyproj-3.5.0rc0/pyproj/crs/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27038 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/_cf1x8.py
--rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/coordinate_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    63344 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/crs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/crs/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/database.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/database.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    44041 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/geod.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/list.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/list.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/proj.pxi
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/proj.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    44644 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproj/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.769213 pyproj-3.5.0rc0/pyproj.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    28776 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-25 02:01:32.000000 pyproj-3.5.0rc0/pyproj.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-25 02:01:32.773213 pyproj-3.5.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.769213 pyproj-3.5.0rc0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 02:01:32.773213 pyproj-3.5.0rc0/test/crs/
--rw-r--r--   0 runner    (1001) docker     (123)    53509 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs.py
--rw-r--r--   0 runner    (1001) docker     (123)    69167 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs_cf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs_coordinate_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs_coordinate_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/crs/test_crs_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/sample.out
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_aoi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_awips221.py
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_datadir.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_datum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_datum_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_doctest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_exception_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    26926 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_geod.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)    21257 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_proj.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_show_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    57638 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-03-25 02:00:32.000000 pyproj-3.5.0rc0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.867084 pyproj-3.6.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/LICENSE_proj
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    30157 2023-06-09 01:25:20.863084 pyproj-3.6.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28684 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.839084 pyproj-3.6.0rc0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/advanced_examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.839084 pyproj-3.6.0rc0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/aoi.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.843084 pyproj-3.6.0rc0/docs/api/crs/
+-rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/coordinate_operation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/coordinate_system.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/crs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/datum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/crs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/database.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/datadir.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/enums.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/geod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/global_context.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/list.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/network.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/proj.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/show_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/sync.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/api/transformer.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/build_crs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5741 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/build_crs_cf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2031 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7514 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/crs_compatibility.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    15702 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/gotchas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.843084 pyproj-3.6.0rc0/docs/media/
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    15779 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15435 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/media/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/optimize_transformations.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/past_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/docs/transformation_grids.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.855084 pyproj-3.6.0rc0/pyproj/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_compat.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_compat.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_crs.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7969 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_crs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    92777 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_crs.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_datadir.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_datadir.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_datadir.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_geod.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_geod.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    20903 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_geod.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_network.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_network.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_sync.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_sync.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_transformer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_transformer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    39998 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/_transformer.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/base.pxi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.859084 pyproj-3.6.0rc0/pyproj/crs/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27038 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/_cf1x8.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57878 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/coordinate_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10092 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64099 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/crs/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/database.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14931 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/database.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44078 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/geod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/list.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/list.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21319 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/proj.pxi
+-rw-r--r--   0 runner    (1001) docker     (123)    11254 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44983 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproj/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.855084 pyproj-3.6.0rc0/pyproj.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    30157 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-09 01:25:20.000000 pyproj-3.6.0rc0/pyproj.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 01:25:20.867084 pyproj-3.6.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7863 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.863084 pyproj-3.6.0rc0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 01:25:20.863084 pyproj-3.6.0rc0/test/crs/
+-rw-r--r--   0 runner    (1001) docker     (123)    55605 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69167 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_cf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23962 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_coordinate_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_coordinate_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12251 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/crs/test_crs_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/sample.out
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_aoi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_awips221.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_datadir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_datum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_datum_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_doctest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_exception_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27348 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_geod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21233 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_proj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_show_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56570 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-09 01:24:29.000000 pyproj-3.6.0rc0/test/test_utils.py
```

### Comparing `pyproj-3.5.0rc0/LICENSE` & `pyproj-3.6.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/LICENSE_proj` & `pyproj-3.6.0rc0/LICENSE_proj`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/Makefile` & `pyproj-3.6.0rc0/Makefile`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/PKG-INFO` & `pyproj-3.6.0rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 Metadata-Version: 2.1
 Name: pyproj
-Version: 3.5.0rc0
+Version: 3.6.0rc0
 Summary: Python interface to PROJ (cartographic projections and coordinate transformations library)
 Home-page: https://github.com/pyproj4/pyproj
-Download-URL: http://python.org/pypi/pyproj
-Author: Jeff Whitaker
-Author-email: jeffrey.s.whitaker@noaa.gov
+Author-email: Jeff Whitaker <jeffrey.s.whitaker@noaa.gov>
+Maintainer: pyproj contributors
 License: MIT
-Project-URL: Documentation, https://pyproj4.github.io/pyproj/
-Project-URL: Release Notes, https://pyproj4.github.io/pyproj/stable/history.html
-Project-URL: Bug Tracker, https://github.com/pyproj4/pyproj/issues
-Project-URL: Source Code, https://github.com/pyproj4/pyproj
+Project-URL: homepage, https://pyproj4.github.io/pyproj/
+Project-URL: documentation, https://pyproj4.github.io/pyproj/
+Project-URL: repository, https://github.com/pyproj4/pyproj
+Project-URL: changelog, https://pyproj4.github.io/pyproj/stable/history.html
 Keywords: GIS,map,geospatial,coordinate-systems,coordinate-transformation,cartographic-projection,geodesic
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_proj
 
 ![Pyproj logo](docs/media/logo.png)
 
 # pyproj
 
 Python interface to [PROJ](http://proj.org) (cartographic projections and coordinate transformations library).
 
 <p align="center">
 <a href="https://gitter.im/pyproj4-pyproj/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge"><img alt="Join the chat at https://gitter.im/pyproj4-pyproj/community" src="https://badges.gitter.im/pyproj4-pyproj/community.svg"></a>
-<a href="#contributors"><img alt="All Contributors" src="https://img.shields.io/badge/all_contributors-57-orange.svg?style=flat-square"></a>
+<a href="#contributors"><img alt="All Contributors" src="https://img.shields.io/badge/all_contributors-60-orange.svg?style=flat-square"></a>
 <a href="https://ci.appveyor.com/project/snowman2/pyproj"><img alt="Appveyor Build Status" src="https://ci.appveyor.com/api/projects/status/v2ypts9j76doa9ey/branch/main?svg=true"></a>
 <a href="https://github.com/pyproj4/pyproj/actions?query=workflow%3ATests"><img alt="GitHub Actions Build Status" src="https://github.com/pyproj4/pyproj/workflows/Tests/badge.svg"></a>
 <a href="https://codecov.io/gh/pyproj4/pyproj"><img alt="Codecov Status" src="https://codecov.io/gh/pyproj4/pyproj/branch/main/graph/badge.svg"></a>
 <a href="https://badge.fury.io/py/pyproj"><img alt="PyPI" src="https://badge.fury.io/py/pyproj.svg"></a>
 <a href="https://pepy.tech/project/pyproj"><img alt="Downloads" src="https://pepy.tech/badge/pyproj"></a>
 <a href="https://anaconda.org/conda-forge/pyproj"><img alt="Anaconda-Server Badge" src="https://anaconda.org/conda-forge/pyproj/badges/version.svg"></a>
 <a href="https://github.com/python/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -144,14 +141,17 @@
     <td align="center"><a href="https://github.com/DWesl"><img src="https://avatars.githubusercontent.com/u/22566757?v=4?s=100" width="100px;" alt=""/><br /><sub><b>DWesl</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=DWesl" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/molinav"><img src="https://avatars.githubusercontent.com/u/9979942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Víctor Molina García</b></sub></a><br /><a href="#platform-molinav" title="Packaging/porting to new platform">📦</a></td>
     <td align="center"><a href="https://github.com/skogler"><img src="https://avatars.githubusercontent.com/u/1032405?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Samuel Kogler</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/issues?q=author%3Askogler" title="Bug reports">🐛</a> <a href="https://github.com/pyproj4/pyproj/commits?author=skogler" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/shadchin"><img src="https://avatars.githubusercontent.com/u/61256?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexander Shadchin</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/issues?q=author%3Ashadchin" title="Bug reports">🐛</a> <a href="https://github.com/pyproj4/pyproj/commits?author=shadchin" title="Code">💻</a></td>
   </tr>
   <tr>
     <td align="center"><a href="https://github.com/greglucas"><img src="https://avatars.githubusercontent.com/u/12417828?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Greg Lucas</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=greglucas" title="Code">💻</a> <a href="#ideas-greglucas" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/dmahr1"><img src="https://avatars.githubusercontent.com/u/8354515?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dan Mahr</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://github.com/rhugonnet"><img src="https://avatars.githubusercontent.com/u/28896516?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Romain Hugonnet</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://javier.jimenezshaw.com/"><img src="https://avatars.githubusercontent.com/u/15678366?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Javier Jimenez Shaw</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Tests">⚠️</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: pyproj Version: 3.5.0rc0 Summary: Python interface
+Metadata-Version: 2.1 Name: pyproj Version: 3.6.0rc0 Summary: Python interface
 to PROJ (cartographic projections and coordinate transformations library) Home-
-page: https://github.com/pyproj4/pyproj Download-URL: http://python.org/pypi/
-pyproj Author: Jeff Whitaker Author-email: jeffrey.s.whitaker@noaa.gov License:
-MIT Project-URL: Documentation, https://pyproj4.github.io/pyproj/ Project-URL:
-Release Notes, https://pyproj4.github.io/pyproj/stable/history.html Project-
-URL: Bug Tracker, https://github.com/pyproj4/pyproj/issues Project-URL: Source
-Code, https://github.com/pyproj4/pyproj Keywords:
-GIS,map,geospatial,coordinate-systems,coordinate-transformation,cartographic-
-projection,geodesic Platform: any Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: GIS Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE License-File: LICENSE_proj ![Pyproj logo]
-(docs/media/logo.png) # pyproj Python interface to [PROJ](http://proj.org)
-(cartographic projections and coordinate transformations library).
+page: https://github.com/pyproj4/pyproj Author-email: Jeff Whitaker
+s.whitaker@noaa.gov> Maintainer: pyproj contributors License: MIT Project-URL:
+homepage, https://pyproj4.github.io/pyproj/ Project-URL: documentation, https:/
+/pyproj4.github.io/pyproj/ Project-URL: repository, https://github.com/pyproj4/
+pyproj Project-URL: changelog, https://pyproj4.github.io/pyproj/stable/
+history.html Keywords: GIS,map,geospatial,coordinate-systems,coordinate-
+transformation,cartographic-projection,geodesic Classifier: Development Status
+:: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: GIS Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Software Development
+:: Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python:
+>=3.9 Description-Content-Type: text/markdown License-File: LICENSE License-
+File: LICENSE_proj ![Pyproj logo](docs/media/logo.png) # pyproj Python
+interface to [PROJ](http://proj.org) (cartographic projections and coordinate
+transformations library).
       [Join_the_chat_at_https://gitter.im/pyproj4-pyproj/community] [All
  Contributors] [Appveyor_Build_Status] [GitHub_Actions_Build_Status] [Codecov
  Status] [PyPI] [Downloads] [Anaconda-Server_Badge] [Code_style:_black] [pre-
                                  commit] [DOI]
 ## Documentation - Stable: http://pyproj4.github.io/pyproj/stable/ - Latest:
 https://pyproj4.github.io/pyproj/latest/ ## Bugs/Questions - Report bugs/
 feature requests: https://github.com/pyproj4/pyproj/issues - Ask questions:
@@ -62,13 +61,13 @@
 
                                                                 ð                                                                                      ð                                                                        ð»                                                        ð ð»                       ð ð» â ï¸                 ð» ð              ð» ð â ï¸
 
                                                        Kyle_Penner                                                                             paulcochrane                                                                              Antonio_Ettorre                                                           DWesl                             VÃ­ctor_Molina_GarcÃ­a                    Samuel_Kogler                     Alexander_Shadchin
 
                                                      ð» ð ð                                                            ð» ð â ï¸ ð                                                            ð¦                                                              ð»                                  ð¦                               ð ð»                    ð ð»
 
-                                                          Greg_Lucas
+                                                          Greg_Lucas                                                                                Dan_Mahr                                                                      Romain_Hugonnet                                                   Javier_Jimenez_Shaw
 
-                                                           ð» ð¤
+                                                           ð» ð¤                                                                    ð» ð â ï¸                                                   ð» ð â ï¸                                       ð» ð â ï¸
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `pyproj-3.5.0rc0/README.md` & `pyproj-3.6.0rc0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # pyproj
 
 Python interface to [PROJ](http://proj.org) (cartographic projections and coordinate transformations library).
 
 <p align="center">
 <a href="https://gitter.im/pyproj4-pyproj/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge"><img alt="Join the chat at https://gitter.im/pyproj4-pyproj/community" src="https://badges.gitter.im/pyproj4-pyproj/community.svg"></a>
-<a href="#contributors"><img alt="All Contributors" src="https://img.shields.io/badge/all_contributors-57-orange.svg?style=flat-square"></a>
+<a href="#contributors"><img alt="All Contributors" src="https://img.shields.io/badge/all_contributors-60-orange.svg?style=flat-square"></a>
 <a href="https://ci.appveyor.com/project/snowman2/pyproj"><img alt="Appveyor Build Status" src="https://ci.appveyor.com/api/projects/status/v2ypts9j76doa9ey/branch/main?svg=true"></a>
 <a href="https://github.com/pyproj4/pyproj/actions?query=workflow%3ATests"><img alt="GitHub Actions Build Status" src="https://github.com/pyproj4/pyproj/workflows/Tests/badge.svg"></a>
 <a href="https://codecov.io/gh/pyproj4/pyproj"><img alt="Codecov Status" src="https://codecov.io/gh/pyproj4/pyproj/branch/main/graph/badge.svg"></a>
 <a href="https://badge.fury.io/py/pyproj"><img alt="PyPI" src="https://badge.fury.io/py/pyproj.svg"></a>
 <a href="https://pepy.tech/project/pyproj"><img alt="Downloads" src="https://pepy.tech/badge/pyproj"></a>
 <a href="https://anaconda.org/conda-forge/pyproj"><img alt="Anaconda-Server Badge" src="https://anaconda.org/conda-forge/pyproj/badges/version.svg"></a>
 <a href="https://github.com/python/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -109,14 +109,17 @@
     <td align="center"><a href="https://github.com/DWesl"><img src="https://avatars.githubusercontent.com/u/22566757?v=4?s=100" width="100px;" alt=""/><br /><sub><b>DWesl</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=DWesl" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/molinav"><img src="https://avatars.githubusercontent.com/u/9979942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Víctor Molina García</b></sub></a><br /><a href="#platform-molinav" title="Packaging/porting to new platform">📦</a></td>
     <td align="center"><a href="https://github.com/skogler"><img src="https://avatars.githubusercontent.com/u/1032405?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Samuel Kogler</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/issues?q=author%3Askogler" title="Bug reports">🐛</a> <a href="https://github.com/pyproj4/pyproj/commits?author=skogler" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/shadchin"><img src="https://avatars.githubusercontent.com/u/61256?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexander Shadchin</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/issues?q=author%3Ashadchin" title="Bug reports">🐛</a> <a href="https://github.com/pyproj4/pyproj/commits?author=shadchin" title="Code">💻</a></td>
   </tr>
   <tr>
     <td align="center"><a href="https://github.com/greglucas"><img src="https://avatars.githubusercontent.com/u/12417828?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Greg Lucas</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=greglucas" title="Code">💻</a> <a href="#ideas-greglucas" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/dmahr1"><img src="https://avatars.githubusercontent.com/u/8354515?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dan Mahr</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://github.com/rhugonnet"><img src="https://avatars.githubusercontent.com/u/28896516?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Romain Hugonnet</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://javier.jimenezshaw.com/"><img src="https://avatars.githubusercontent.com/u/15678366?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Javier Jimenez Shaw</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Tests">⚠️</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -41,13 +41,13 @@
 
                                                                 ð                                                                                      ð                                                                        ð»                                                        ð ð»                       ð ð» â ï¸                 ð» ð              ð» ð â ï¸
 
                                                        Kyle_Penner                                                                             paulcochrane                                                                              Antonio_Ettorre                                                           DWesl                             VÃ­ctor_Molina_GarcÃ­a                    Samuel_Kogler                     Alexander_Shadchin
 
                                                      ð» ð ð                                                            ð» ð â ï¸ ð                                                            ð¦                                                              ð»                                  ð¦                               ð ð»                    ð ð»
 
-                                                          Greg_Lucas
+                                                          Greg_Lucas                                                                                Dan_Mahr                                                                      Romain_Hugonnet                                                   Javier_Jimenez_Shaw
 
-                                                           ð» ð¤
+                                                           ð» ð¤                                                                    ð» ð â ï¸                                                   ð» ð â ï¸                                       ð» ð â ï¸
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `pyproj-3.5.0rc0/docs/Makefile` & `pyproj-3.6.0rc0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/advanced_examples.rst` & `pyproj-3.6.0rc0/docs/advanced_examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -151,14 +151,36 @@
     ...     CRS("EPSG:4326").to_3d(),
     ...     CRS("EPSG:2056").to_3d(),
     ...     always_xy=True,
     ...)
     >>> transformer_3d.transform(8.37909, 47.01987, 1000)
     (2671499.8913080636, 1208075.1135782297, 951.4265527743846)
 
+
+Demote CRS to 2D
+----------------
+
+.. versionadded:: 3.6
+
+
+With the need for explicit 3D CRS since PROJ 6+, one might need to retrieve their 2D version,
+for example to create another 3D CRS compound between a 2D CRS and a vertical CRS.
+
+.. code-block:: python
+
+    >>> from pyproj import CRS, Transformer
+    >>> from pyproj.crs import CompoundCRS
+    >>> src_crs = CRS("EPSG:4979") # Any 3D CRS, here the 3D WGS 84
+    >>> vert_crs = CRS("EPSG:5773") # Any vertical CRS, here the EGM96 geoid
+    >>> dst_crs = CompoundCRS(src_crs.name + vert_crs.name, components=[src_crs.to_2d(), vert_crs])
+    >>> transformer_3d = Transformer.from_crs(src_crs, dst_crs, always_xy=True)
+    >>> transformer_3d.transform(8.37909, 47.01987, 1000)
+    (8.37909, 47.01987, 951.7851086745321)
+
+
 Projected CRS Bounds
 ----------------------
 
 .. versionadded:: 3.1
 
 The boundary of the CRS is given in geographic coordinates.
 This is the recommended method for calculating the projected bounds.
```

### Comparing `pyproj-3.5.0rc0/docs/api/crs/coordinate_operation.rst` & `pyproj-3.6.0rc0/docs/api/crs/coordinate_operation.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/crs/coordinate_system.rst` & `pyproj-3.6.0rc0/docs/api/crs/coordinate_system.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/crs/crs.rst` & `pyproj-3.6.0rc0/docs/api/crs/crs.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/crs/datum.rst` & `pyproj-3.6.0rc0/docs/api/crs/datum.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/crs/enums.rst` & `pyproj-3.6.0rc0/docs/api/crs/enums.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/database.rst` & `pyproj-3.6.0rc0/docs/api/database.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/global_context.rst` & `pyproj-3.6.0rc0/docs/api/global_context.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/list.rst` & `pyproj-3.6.0rc0/docs/api/list.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/api/transformer.rst` & `pyproj-3.6.0rc0/docs/api/transformer.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/build_crs.rst` & `pyproj-3.6.0rc0/docs/build_crs.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/build_crs_cf.rst` & `pyproj-3.6.0rc0/docs/build_crs_cf.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/conf.py` & `pyproj-3.6.0rc0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/crs_compatibility.rst` & `pyproj-3.6.0rc0/docs/crs_compatibility.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/examples.rst` & `pyproj-3.6.0rc0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/gotchas.rst` & `pyproj-3.6.0rc0/docs/gotchas.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/history.rst` & `pyproj-3.6.0rc0/docs/history.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 Change Log
 ==========
 
+3.6.0
+------
+- DEP: Minimum supported Python version 3.9 (issue #1111)
+- WHL: Wheels contain PROJ 9.2.1 (pull #1291)
+- ENH: Added allow_superseded kwargs to :class:`pyproj.transformer.TransformerGroup` (pull #1269)
+- ENH: Added :meth:`CRS.to_2d` to demote 3D CRS to 2D (issue #1266)
+- ENH: Added parameter `output_axis_rule` to :meth:`CRS.to_wkt` (pull #1287)
+- BUG: fix Geod.npts NaN handling (issue #1282)
+
 3.5.0
 ------
 - DEP: Minimum PROJ version 9.0 (issue #1223)
 - WHL: PROJ 9.2 in wheels (pull #1243)
 - ENH: Add `return_back_azimuth: bool` to allow compatibility between the azimuth output of the following functions (issue #1163):
     `fwd` and `fwd_intermediate`, `inv` and `inv_intermediate`,
     Note: BREAKING CHANGE for the default value `return_back_azimuth=True` in the functions `fwd_intermediate` and `inv_intermediate`
     to mach the default value in `fwd` and `inv`
 - ENH: Added only_best kwarg to :meth:`.Transformer.from_crs` (issue #1228)
 - PERF: Optimize point transformations (pull #1204)
+- PERF: Optimize for single point in Geod fwd/inv functions (pull #1206)
 - REF: Raise error when :meth:`.CRS.to_wkt`, :meth:`.CRS.to_json`, or :meth:`.CRS.to_proj4` returns None (issue #1036)
 - CLN: Remove `AzumuthalEquidistantConversion` & :class:`LambertAzumuthalEqualAreaConversion`. :class:`AzimuthalEquidistantConversion` & :class:`LambertAzimuthalEqualAreaConversion` should be used instead (pull #1219)
 - BUG: Fix Derived Projected CRS support (issue #1182)
 - BUG: Add horizontal_datum_name for geographic CRS in :meth:`.CRS.to_cf` (issue #1251)
 - BUG: Add datum ensemble support to :class:`.GeographicCRS` (pull #1255)
 
 3.4.1
```

### Comparing `pyproj-3.5.0rc0/docs/index.rst` & `pyproj-3.6.0rc0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 Python interface to  `PROJ <https://proj.org/>`_ (cartographic projections and coordinate transformations library).
 
 GitHub Repository: https://github.com/pyproj4/pyproj
 
 .. note:: Minimum supported PROJ version is 9.0
 
-.. note:: Minimum supported Python version is 3.8
+.. note:: Minimum supported Python version is 3.9
 
 .. note:: Linux (manylinux2014) wheels require pip 19.3+
 
 .. note:: pyproj 3 wheels do not include transformation grids.
           For migration assistance see: :ref:`transformation_grids`
```

### Comparing `pyproj-3.5.0rc0/docs/installation.rst` & `pyproj-3.6.0rc0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/make.bat` & `pyproj-3.6.0rc0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/media/icon.png` & `pyproj-3.6.0rc0/docs/media/icon.png`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/media/icon.svg` & `pyproj-3.6.0rc0/docs/media/icon.svg`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/media/logo.png` & `pyproj-3.6.0rc0/docs/media/logo.png`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/media/logo.svg` & `pyproj-3.6.0rc0/docs/media/logo.svg`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/docs/past_versions.rst` & `pyproj-3.6.0rc0/docs/past_versions.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 Documentation Archive
 =====================
 
+- `3.5.0 <https://pyproj4.github.io/pyproj/3.5.0/>`_
 - `3.4.1 <https://pyproj4.github.io/pyproj/3.4.1/>`_
 - `3.3.1 <https://pyproj4.github.io/pyproj/3.3.1/>`_
 - `3.2.1 <https://pyproj4.github.io/pyproj/3.2.1/>`_
 - `3.1.0 <https://pyproj4.github.io/pyproj/3.1.0/>`_
 - `3.0.1 <https://pyproj4.github.io/pyproj/3.0.1/>`_
 - `2.6.1 <https://pyproj4.github.io/pyproj/v2.6.1rel/>`_
 - `2.5.0 <https://pyproj4.github.io/pyproj/v2.5.0rel/>`_
```

### Comparing `pyproj-3.5.0rc0/docs/transformation_grids.rst` & `pyproj-3.6.0rc0/docs/transformation_grids.rst`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/__init__.py` & `pyproj-3.6.0rc0/pyproj/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Python interface to PROJ (https://proj.org),
 cartographic projections and coordinate transformations library.
 
 Download: http://python.org/pypi/pyproj
 
-Requirements: Python 3.8+.
+Requirements: Python 3.9+.
 
 Contact:  Jeffrey Whitaker <jeffrey.s.whitaker@noaa.gov>
 
 Copyright (c) 2006-2018, Jeffrey Whitaker.
 Copyright (c) 2019-2023, Open source contributors.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
@@ -62,15 +62,15 @@
 from pyproj.transformer import (  # noqa: F401 pylint: disable=unused-import
     Transformer,
     itransform,
     proj_version_str,
     transform,
 )
 
-__version__ = "3.5.0rc0"
+__version__ = "3.6.0rc0"
 __all__ = [
     "Proj",
     "Geod",
     "CRS",
     "Transformer",
     "transform",
     "itransform",
```

### Comparing `pyproj-3.5.0rc0/pyproj/__main__.py` & `pyproj-3.6.0rc0/pyproj/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_compat.pyx` & `pyproj-3.6.0rc0/pyproj/_compat.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_crs.pxd` & `pyproj-3.6.0rc0/pyproj/_crs.pxd`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,37 @@
 include "proj.pxi"
 
 
 from pyproj.enums import WktVersion
 
+from cpython cimport bool
+
 
 cdef extern from "proj_experimental.h":
     PJ *proj_crs_promote_to_3D(PJ_CONTEXT *ctx,
                                const char* crs_3D_name,
                                const PJ* crs_2D)
 
+    PJ *proj_crs_demote_to_2D(PJ_CONTEXT *ctx,
+                              const char *crs_2D_name,
+                              const PJ *crs_3D)
 
 cdef tuple _get_concatenated_operations(PJ_CONTEXT*context, PJ*concatenated_operation)
 cdef _to_proj4(
     PJ_CONTEXT* context,
     PJ* projobj,
     object version,
     bint pretty,
 )
 cdef _to_wkt(
     PJ_CONTEXT* context,
     PJ* projobj,
     object version,
     bint pretty,
+    bool output_axis_rule=*,
 )
 
 cdef class Axis:
     cdef readonly str name
     cdef readonly str abbrev
     cdef readonly str direction
     cdef readonly double unit_conversion_factor
```

### Comparing `pyproj-3.5.0rc0/pyproj/_crs.pyi` & `pyproj-3.6.0rc0/pyproj/_crs.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Any, Iterable, List, NamedTuple, Optional, Tuple, Union
+from collections.abc import Iterable
+from typing import Any, NamedTuple, Optional, Union
 
 from pyproj.crs.enums import CoordinateOperationType
 from pyproj.enums import ProjVersion, WktVersion
 
 class Axis:
     name: str
     abbrev: str
@@ -19,26 +20,27 @@
     south: float
     east: float
     north: float
     name: str
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
     @property
-    def bounds(self) -> Tuple[float, float, float, float]: ...
+    def bounds(self) -> tuple[float, float, float, float]: ...
 
 class Base:
     name: str
     @property
     def remarks(self) -> str: ...
     @property
     def scope(self) -> str: ...
     def to_wkt(
         self,
         version: Union[WktVersion, str] = WktVersion.WKT2_2019,
         pretty: bool = False,
+        output_axis_rule: Optional[bool] = None,
     ) -> str: ...
     def to_json(self, pretty: bool = False, indentation: int = 2) -> str: ...
     def to_json_dict(self) -> dict: ...
     def __str__(self) -> str: ...
     def __repr__(self) -> str: ...
     def __eq__(self, other: Any) -> bool: ...
     def is_exact_same(self, other: Any) -> bool: ...
@@ -111,15 +113,15 @@
     def axis_list(self) -> Iterable[Axis]: ...
     @staticmethod
     def from_string(coordinate_system_string: str) -> "CoordinateSystem": ...
     @staticmethod
     def from_json_dict(coordinate_system_dict: dict) -> "CoordinateSystem": ...
     @staticmethod
     def from_json(coordinate_system_json_str: str) -> "CoordinateSystem": ...
-    def to_cf(self, rotated_pole: bool = False) -> List[dict]: ...
+    def to_cf(self, rotated_pole: bool = False) -> list[dict]: ...
 
 class Param:
     name: str
     auth_name: str
     code: str
     value: str
     unit_conversion_factor: float
@@ -154,15 +156,15 @@
     @property
     def grids(self) -> Iterable[Grid]: ...
     @property
     def area_of_use(self) -> Optional[AreaOfUse]: ...
     @property
     def towgs84(self) -> Iterable[float]: ...
     @property
-    def operations(self) -> Tuple["CoordinateOperation"]: ...
+    def operations(self) -> tuple["CoordinateOperation"]: ...
     def __init__(self) -> None: ...
     def __repr__(self) -> str: ...
     @staticmethod
     def from_authority(
         auth_name: str, code: Union[int, str]
     ) -> "CoordinateOperation": ...
     @staticmethod
@@ -195,15 +197,15 @@
     type_name: str
     def __init__(self, proj_string: str) -> None: ...
     @property
     def ellipsoid(self) -> Optional[Ellipsoid]: ...
     @property
     def area_of_use(self) -> Optional[AreaOfUse]: ...
     @property
-    def axis_info(self) -> List[Axis]: ...
+    def axis_info(self) -> list[Axis]: ...
     @property
     def prime_meridian(self) -> Optional[PrimeMeridian]: ...
     @property
     def datum(self) -> Optional[Datum]: ...
     @property
     def sub_crs_list(self) -> Iterable["_CRS"]: ...
     @property
@@ -221,16 +223,17 @@
     ) -> str: ...
     def to_epsg(self, min_confidence: int = 70) -> Optional[int]: ...
     def to_authority(
         self, auth_name: Optional[str] = None, min_confidence: int = 70
     ): ...
     def list_authority(
         self, auth_name: Optional[str] = None, min_confidence: int = 70
-    ) -> List[AuthorityMatchInfo]: ...
+    ) -> list[AuthorityMatchInfo]: ...
     def to_3d(self, name: Optional[str] = None) -> "_CRS": ...
+    def to_2d(self, name: Optional[str] = None) -> "_CRS": ...
     @property
     def is_geographic(self) -> bool: ...
     @property
     def is_projected(self) -> bool: ...
     @property
     def is_vertical(self) -> bool: ...
     @property
```

### Comparing `pyproj-3.5.0rc0/pyproj/_crs.pyx` & `pyproj-3.6.0rc0/pyproj/_crs.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -71,24 +71,26 @@
 
 
 cdef _to_wkt(
     PJ_CONTEXT* context,
     PJ* projobj,
     object version,
     bint pretty,
+    bool output_axis_rule=None,
 ):
     """
     Convert a PJ object to a wkt string.
 
     Parameters
     ----------
     context: PJ_CONTEXT*
     projobj: PJ*
     wkt_out_type: PJ_WKT_TYPE
     pretty: bool
+    output_axis_rule: bool or None
 
     Return
     ------
     str or None
     """
     # get the output WKT format
     supported_wkt_types = {
@@ -100,20 +102,26 @@
         WktVersion.WKT2_2019_SIMPLIFIED: PJ_WKT2_2019_SIMPLIFIED,
         WktVersion.WKT1_GDAL: PJ_WKT1_GDAL,
         WktVersion.WKT1_ESRI: PJ_WKT1_ESRI
     }
     cdef PJ_WKT_TYPE wkt_out_type
     wkt_out_type = supported_wkt_types[WktVersion.create(version)]
 
-    cdef const char* options_wkt[2]
+    cdef const char* options_wkt[3]
     cdef bytes multiline = b"MULTILINE=NO"
     if pretty:
         multiline = b"MULTILINE=YES"
+    cdef bytes output_axis = b"OUTPUT_AXIS=AUTO"
+    if output_axis_rule is False:
+        output_axis = b"OUTPUT_AXIS=NO"
+    elif output_axis_rule is True:
+        output_axis = b"OUTPUT_AXIS=YES"
     options_wkt[0] = multiline
-    options_wkt[1] = NULL
+    options_wkt[1] = output_axis
+    options_wkt[2] = NULL
     cdef const char* proj_string
     proj_string = proj_as_wkt(
         context,
         projobj,
         wkt_out_type,
         options_wkt,
     )
@@ -394,39 +402,43 @@
         Returns
         -------
         str:
             Scope of object.
         """
         return self._scope
 
-    def to_wkt(self, version=WktVersion.WKT2_2019, pretty=False):
+    def to_wkt(self, version=WktVersion.WKT2_2019, pretty=False, output_axis_rule=None):
         """
         Convert the projection to a WKT string.
 
         Version options:
           - WKT2_2015
           - WKT2_2015_SIMPLIFIED
           - WKT2_2019
           - WKT2_2019_SIMPLIFIED
           - WKT1_GDAL
           - WKT1_ESRI
 
+        .. versionadded:: 3.6.0 output_axis_rule
 
         Parameters
         ----------
         version: pyproj.enums.WktVersion, default=pyproj.enums.WktVersion.WKT2_2019
             The version of the WKT output.
         pretty: bool, default=False
             If True, it will set the output to be a multiline string.
+        output_axis_rule: bool, optional, default=None
+            If True, it will set the axis rule on any case. If false, never.
+            None for AUTO, that depends on the CRS and version.
 
         Returns
         -------
         str
         """
-        return _to_wkt(self.context, self.projobj, version, pretty=pretty)
+        return _to_wkt(self.context, self.projobj, version, pretty=pretty, output_axis_rule=output_axis_rule)
 
     def to_json(self, bint pretty=False, int indentation=2):
         """
         .. versionadded:: 2.4.0
 
         Convert the object to a JSON string.
 
@@ -702,15 +714,15 @@
         ----------
         rotated_pole: bool, default=False
             If True, the geographic coordinates are on a rotated pole grid.
             This corresponds to the rotated_latitude_longitude grid_mapping_name.
 
         Returns
         -------
-        List[dict]:
+        list[dict]:
             CF-1.8 version of the CoordinateSystem.
         """
         axis_list = self.to_json_dict()["axis"]
         cf_params = []
         def get_linear_unit(axis):
             try:
                 return f'{axis["unit"]["conversion_factor"]} metre'
@@ -2151,15 +2163,15 @@
         return CoordinateOperation.create(context, coordinate_operation_pj)
 
     @property
     def params(self):
         """
         Returns
         -------
-        List[Param]:
+        list[Param]:
             The coordinate operation parameters.
         """
         if self._params is not None:
             return self._params
         self._params = []
         cdef int num_params = 0
         num_params = proj_coordoperation_get_param_count(
@@ -2178,15 +2190,15 @@
         return self._params
 
     @property
     def grids(self):
         """
         Returns
         -------
-        List[Grid]:
+        list[Grid]:
             The coordinate operation grids.
         """
         if self._grids is not None:
             return self._grids
         self._grids = []
         cdef int num_grids = 0
         num_grids = proj_coordoperation_get_grid_used_count(
@@ -2239,15 +2251,15 @@
         return _to_proj4(self.context, self.projobj, version=version, pretty=pretty)
 
     @property
     def towgs84(self):
         """
         Returns
         -------
-        List[float]:
+        list[float]:
             A list of 3 or 7 towgs84 values if they exist.
 
         """
         if self._towgs84 is not None:
             return self._towgs84
         towgs84_dict = OrderedDict(
             (
@@ -2269,15 +2281,15 @@
     @property
     def operations(self):
         """
         .. versionadded:: 2.4.0
 
         Returns
         -------
-        Tuple[CoordinateOperation]:
+        tuple[CoordinateOperation]:
             The operations in a concatenated operation.
 
         """
         if self._operations is not None:
             return self._operations
         self._operations = _get_concatenated_operations(self.context, self.projobj)
         return self._operations
@@ -2407,15 +2419,15 @@
         """
         Retrieves all relevant axis information in the CRS.
         If it is a Bound CRS, it gets the axis list from the Source CRS.
         If it is a Compound CRS, it gets the axis list from the Sub CRS list.
 
         Returns
         -------
-        List[Axis]:
+        list[Axis]:
             The list of axis information.
         """
         axis_info_list = []
         if self.coordinate_system:
             axis_info_list.extend(self.coordinate_system.axis_list)
         elif self.is_bound and self.source_crs:
             axis_info_list.extend(self.source_crs.axis_info)
@@ -2639,15 +2651,15 @@
     @property
     def sub_crs_list(self):
         """
         If the CRS is a compound CRS, it will return a list of sub CRS objects.
 
         Returns
         -------
-        List[_CRS]
+        list[_CRS]
         """
         if self._sub_crs_list is not None:
             return self._sub_crs_list
         if not self.is_compound:
             self._sub_crs_list = []
             return self._sub_crs_list
 
@@ -2852,15 +2864,15 @@
             The name of the authority to filter by.
         min_confidence: int, default=70
             A value between 0-100 where 100 is the most confident.
             :ref:`min_confidence`
 
         Returns
         -------
-        List[AuthorityMatchInfo]:
+        list[AuthorityMatchInfo]:
             List of authority matches for the CRS.
         """
         # get list of possible matching projections
         cdef PJ_OBJ_LIST *proj_list = NULL
         cdef int *c_out_confidence_list = NULL
         cdef int num_proj_objects = -9999
         cdef bytes b_auth_name
@@ -2961,14 +2973,52 @@
                 version=WktVersion.WKT2_2019,
                 pretty=False,
             ))
         finally:
             proj_destroy(projobj)
         return crs_3d
 
+    def to_2d(self, str name=None):
+        """
+        .. versionadded:: 3.6.0
+
+        Convert the current CRS to the 2D version if it makes sense.
+
+        Parameters
+        ----------
+        name: str, optional
+            CRS name. If None, it will use the name of the original CRS.
+
+        Returns
+        -------
+        _CRS
+        """
+        cdef char* c_name = NULL
+        cdef bytes b_name
+        if name is not None:
+            b_name = cstrencode(name)
+            c_name = b_name
+
+        cdef PJ * projobj = proj_crs_demote_to_2D(
+            self.context, c_name, self.projobj
+        )
+        _clear_proj_error()
+        if projobj == NULL:
+            return self
+        try:
+            crs_2d = _CRS(_to_wkt(
+                self.context,
+                projobj,
+                version=WktVersion.WKT2_2019,
+                pretty=False,
+            ))
+        finally:
+            proj_destroy(projobj)
+        return crs_2d
+
     def _is_crs_property(
         self, str property_name, tuple property_types, int sub_crs_index=0
     ):
         """
         .. versionadded:: 2.2.0
 
         This method will check for a property on the CRS.
```

### Comparing `pyproj-3.5.0rc0/pyproj/_datadir.pyx` & `pyproj-3.6.0rc0/pyproj/_datadir.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_geod.pxd` & `pyproj-3.6.0rc0/pyproj/_geod.pxd`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_geod.pyi` & `pyproj-3.6.0rc0/pyproj/_geod.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, NamedTuple, Tuple, Type
+from typing import Any, NamedTuple
 
 geodesic_version_str: str
 
 class GeodIntermediateReturn(NamedTuple):
     npts: int
     del_s: float
     dist: float
@@ -16,15 +16,15 @@
     b: float
     f: float
     es: float
     sphere: bool
     def __init__(
         self, a: float, f: float, sphere: bool, b: float, es: float
     ) -> None: ...
-    def __reduce__(self) -> Tuple[Type["Geod"], str]: ...
+    def __reduce__(self) -> tuple[type["Geod"], str]: ...
     def __repr__(self) -> str: ...
     def _fwd(
         self,
         lons: Any,
         lats: Any,
         az: Any,
         dist: Any,
@@ -35,15 +35,15 @@
         self,
         lons: float,
         lats: float,
         az: float,
         dist: float,
         radians: bool = False,
         return_back_azimuth: bool = True,
-    ) -> Tuple[float, float, float]: ...
+    ) -> tuple[float, float, float]: ...
     def _inv(
         self,
         lons1: Any,
         lats1: Any,
         lons2: Any,
         lats2: Any,
         radians: bool = False,
@@ -53,31 +53,32 @@
         self,
         lons1: float,
         lats1: float,
         lons2: float,
         lats2: float,
         radians: bool = False,
         return_back_azimuth: bool = False,
-    ) -> Tuple[float, float, float]: ...
+    ) -> tuple[float, float, float]: ...
     def _inv_or_fwd_intermediate(
         self,
         lon1: float,
         lat1: float,
         lon2_or_azi1: float,
-        lat2_or_nan: float,
+        lat2: float,
         npts: int,
         del_s: float,
         radians: bool,
         initial_idx: int,
         terminus_idx: int,
         flags: int,
         out_lons: Any,
         out_lats: Any,
         out_azis: Any,
         return_back_azimuth: bool,
+        is_fwd: bool,
     ) -> GeodIntermediateReturn: ...
     def _line_length(self, lons: Any, lats: Any, radians: bool = False) -> float: ...
     def _polygon_area_perimeter(
         self, lons: Any, lats: Any, radians: bool = False
-    ) -> Tuple[float, float]: ...
+    ) -> tuple[float, float]: ...
 
 def reverse_azimuth(azi: Any, radians: bool = False) -> None: ...
```

### Comparing `pyproj-3.5.0rc0/pyproj/_geod.pyx` & `pyproj-3.6.0rc0/pyproj/_geod.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -361,25 +361,26 @@
     @cython.boundscheck(False)
     @cython.wraparound(False)
     def _inv_or_fwd_intermediate(
         self,
         double lon1,
         double lat1,
         double lon2_or_azi1,
-        double lat2_or_nan,
+        double lat2,
         int npts,
         double del_s,
         bint radians,
         int initial_idx,
         int terminus_idx,
         int flags,
         object out_lons,
         object out_lats,
         object out_azis,
         bint return_back_azimuth,
+        bint is_fwd,
     ) -> GeodIntermediateReturn:
         """
         .. versionadded:: 3.1.0
 
         given initial and terminus lat/lon, find npts intermediate points.
         using given lons, lats buffers
         """
@@ -393,36 +394,35 @@
             bint store_az = (
                 out_azis is not None or
                 (flags & GEOD_INTER_FLAG_AZIS_MASK) == GEOD_INTER_FLAG_AZIS_KEEP
             )
             PyBuffWriteManager lons_buff
             PyBuffWriteManager lats_buff
             PyBuffWriteManager azis_buff
-            bint is_fwd = isnan(lat2_or_nan)
 
         if not is_fwd and (del_s == 0) == (npts == 0):
             raise GeodError("inv_intermediate: "
                             "npts and del_s are mutually exclusive, "
                             "only one of them must be != 0.")
         with nogil:
             if radians:
                 lon1 *= _RAD2DG
                 lat1 *= _RAD2DG
                 lon2_or_azi1 *= _RAD2DG
                 if not is_fwd:
-                    lat2_or_nan *= _RAD2DG
+                    lat2 *= _RAD2DG
 
             if is_fwd:
                 # do fwd computation to set azimuths, distance.
                 geod_lineinit(&line, &self._geod_geodesic, lat1, lon1, lon2_or_azi1, 0u)
                 line.s13 = del_s * (npts + initial_idx + terminus_idx - 1)
             else:
                 # do inverse computation to set azimuths, distance.
                 geod_inverseline(&line, &self._geod_geodesic, lat1, lon1,
-                                 lat2_or_nan, lon2_or_azi1, 0u)
+                                 lat2, lon2_or_azi1, 0u)
 
                 if npts == 0:
                     # calc the number of required points by the distance increment
                     # s12 holds a temporary float value of npts (just reusing this var)
                     s12 = line.s13 / del_s - initial_idx - terminus_idx + 1
                     if (flags & GEOD_INTER_FLAG_NPTS_MASK) == \
                             GEOD_INTER_FLAG_NPTS_ROUND:
```

### Comparing `pyproj-3.5.0rc0/pyproj/_network.pyx` & `pyproj-3.6.0rc0/pyproj/_network.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_show_versions.py` & `pyproj-3.6.0rc0/pyproj/_show_versions.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_transformer.pxd` & `pyproj-3.6.0rc0/pyproj/_transformer.pxd`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/_transformer.pyi` & `pyproj-3.6.0rc0/pyproj/_transformer.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import numbers
 from array import array
-from typing import Any, List, NamedTuple, Optional, Tuple, Union
+from typing import Any, NamedTuple, Optional, Union
 
 from pyproj._crs import _CRS, AreaOfUse, Base, CoordinateOperation
 from pyproj.enums import ProjVersion, TransformDirection
 
 proj_version_str: str
-PROJ_VERSION: Tuple[int, int, int]
+PROJ_VERSION: tuple[int, int, int]
 
 class AreaOfInterest(NamedTuple):
     west_lon_degree: float
     south_lat_degree: float
     east_lon_degree: float
     north_lat_degree: float
 
@@ -26,25 +26,26 @@
     dx_dlam: float
     dx_dphi: float
     dy_dlam: float
     dy_dphi: float
 
 class _TransformerGroup:
     _transformers: Any
-    _unavailable_operations: List[CoordinateOperation]
+    _unavailable_operations: list[CoordinateOperation]
     _best_available: bool
     def __init__(
         self,
         crs_from: str,
         crs_to: str,
         always_xy: bool,
         area_of_interest: Optional[AreaOfInterest],
         authority: Optional[str],
         accuracy: Optional[float],
         allow_ballpark: bool,
+        allow_superseded: bool,
     ) -> None: ...
 
 class _Transformer(Base):
     input_geographic: bool
     output_geographic: bool
     is_pipeline: bool
     type_name: str
@@ -61,15 +62,15 @@
     @property
     def area_of_use(self) -> AreaOfUse: ...
     @property
     def source_crs(self) -> Optional[_CRS]: ...
     @property
     def target_crs(self) -> Optional[_CRS]: ...
     @property
-    def operations(self) -> Union[Tuple[CoordinateOperation], None]: ...
+    def operations(self) -> Union[tuple[CoordinateOperation], None]: ...
     def get_last_used_operation(self) -> _Transformer: ...
     @property
     def is_network_enabled(self) -> bool: ...
     def to_proj4(
         self,
         version: Union[ProjVersion, str] = ProjVersion.PROJ_5,
         pretty: bool = False,
@@ -124,11 +125,11 @@
         bottom: float,
         right: float,
         top: float,
         densify_pts: int = 21,
         radians: bool = False,
         errcheck: bool = False,
         direction: Union[TransformDirection, str] = TransformDirection.FORWARD,
-    ) -> Tuple[float, float, float, float]: ...
+    ) -> tuple[float, float, float, float]: ...
     def _get_factors(
         self, longitude: Any, latitude: Any, radians: bool, errcheck: bool
     ) -> Factors: ...
```

### Comparing `pyproj-3.5.0rc0/pyproj/_transformer.pyx` & `pyproj-3.6.0rc0/pyproj/_transformer.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -73,37 +73,37 @@
 
 These are the scaling and angular distortion factors.
 
 See PROJ :c:type:`PJ_FACTORS` documentation.
 
 Parameters
 ----------
-meridional_scale: List[float]
+meridional_scale: list[float]
      Meridional scale at coordinate.
-parallel_scale: List[float]
+parallel_scale: list[float]
     Parallel scale at coordinate.
-areal_scale: List[float]
+areal_scale: list[float]
     Areal scale factor at coordinate.
-angular_distortion: List[float]
+angular_distortion: list[float]
     Angular distortion at coordinate.
-meridian_parallel_angle: List[float]
+meridian_parallel_angle: list[float]
     Meridian/parallel angle at coordinate.
-meridian_convergence: List[float]
+meridian_convergence: list[float]
     Meridian convergence at coordinate. Sometimes also described as *grid declination*.
-tissot_semimajor: List[float]
+tissot_semimajor: list[float]
     Maximum scale factor.
-tissot_semiminor: List[float]
+tissot_semiminor: list[float]
     Minimum scale factor.
-dx_dlam: List[float]
+dx_dlam: list[float]
     Partial derivative of coordinate.
-dx_dphi: List[float]
+dx_dphi: list[float]
     Partial derivative of coordinate.
-dy_dlam: List[float]
+dy_dlam: list[float]
     Partial derivative of coordinate.
-dy_dphi: List[float]
+dy_dphi: list[float]
     Partial derivative of coordinate.
 """
 
 cdef PJ_DIRECTION get_pj_direction(object direction) except *:
     # optimized lookup to avoid creating a new instance every time
     # gh-1205
     if not isinstance(direction, TransformDirection):
@@ -137,14 +137,15 @@
         _CRS crs_from not None,
         _CRS crs_to not None,
         bint always_xy,
         area_of_interest,
         bint allow_ballpark,
         str authority,
         double accuracy,
+        bint allow_superseded,
     ):
         """
         From PROJ docs:
 
         The operations are sorted with the most relevant ones first: by
         descending area (intersection of the transformation area with the
         area of interest, or intersection of the transformation with the
@@ -198,14 +199,19 @@
                     accuracy,
                 )
             proj_operation_factory_context_set_allow_ballpark_transformations(
                 self.context,
                 operation_factory_context,
                 allow_ballpark,
             )
+            proj_operation_factory_context_set_discard_superseded(
+                self.context,
+                operation_factory_context,
+                not allow_superseded,
+            )
             proj_operation_factory_context_set_grid_availability_use(
                 self.context,
                 operation_factory_context,
                 PROJ_GRID_AVAILABILITY_IGNORED,
             )
             proj_operation_factory_context_set_spatial_criterion(
                 self.context,
@@ -448,15 +454,15 @@
     @property
     def operations(self):
         """
         .. versionadded:: 2.4.0
 
         Returns
         -------
-        Tuple[CoordinateOperation]:
+        tuple[CoordinateOperation]:
             The operations in a concatenated operation.
         """
         if self._operations is not None:
             return self._operations
         self._operations = _get_concatenated_operations(self.context, self.projobj)
         return self._operations
```

### Comparing `pyproj-3.5.0rc0/pyproj/aoi.py` & `pyproj-3.6.0rc0/pyproj/aoi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module contains the structures related to areas of interest.
 """
 from dataclasses import dataclass
-from typing import NamedTuple, Optional, Tuple, Union
+from typing import NamedTuple, Optional, Union
 
 from pyproj.utils import is_null
 
 
 @dataclass(frozen=True)
 class AreaOfInterest:
     """
@@ -52,21 +52,21 @@
     east: float
     #: North bound of area of use.
     north: float
     #: Name of area of use.
     name: Optional[str] = None
 
     @property
-    def bounds(self) -> Tuple[float, float, float, float]:
+    def bounds(self) -> tuple[float, float, float, float]:
         """
         The bounds of the area of use.
 
         Returns
         -------
-        Tuple[float, float, float, float]
+        tuple[float, float, float, float]
             west, south, east, and north bounds.
         """
         return self.west, self.south, self.east, self.north
 
     def __str__(self) -> str:
         return f"- name: {self.name}\n" f"- bounds: {self.bounds}"
```

### Comparing `pyproj-3.5.0rc0/pyproj/base.pxi` & `pyproj-3.6.0rc0/pyproj/base.pxi`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/crs/__init__.py` & `pyproj-3.6.0rc0/pyproj/crs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/crs/_cf1x8.py` & `pyproj-3.6.0rc0/pyproj/crs/_cf1x8.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/crs/coordinate_operation.py` & `pyproj-3.6.0rc0/pyproj/crs/coordinate_operation.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/crs/coordinate_system.py` & `pyproj-3.6.0rc0/pyproj/crs/coordinate_system.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/crs/crs.py` & `pyproj-3.6.0rc0/pyproj/crs/crs.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 to the coordinate reference system (CRS) information.
 """
 # pylint: disable=too-many-lines
 import json
 import re
 import threading
 import warnings
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Optional, Union
 
 from pyproj._crs import (
     _CRS,
     AreaOfUse,
     AuthorityMatchInfo,
     Axis,
     CoordinateOperation,
@@ -85,15 +85,15 @@
 
 
 def _prepare_from_proj_string(in_crs_string: str) -> str:
     in_crs_string = re.sub(r"[\s+]?=[\s+]?", "=", in_crs_string.lstrip())
     # make sure the projection starts with +proj or +init
     starting_params = ("+init", "+proj", "init", "proj")
     if not in_crs_string.startswith(starting_params):
-        kvpairs: List[str] = []
+        kvpairs: list[str] = []
         first_item_inserted = False
         for kvpair in in_crs_string.split():
             if not first_item_inserted and (kvpair.startswith(starting_params)):
                 kvpairs.insert(0, kvpair)
                 first_item_inserted = True
             else:
                 kvpairs.append(kvpair)
@@ -639,24 +639,24 @@
         Returns
         -------
         dict:
             CF-1.8 version of the projection.
 
         """
         # pylint: disable=too-many-branches,too-many-return-statements
-        cf_dict: Dict[str, Any] = {"crs_wkt": self.to_wkt(wkt_version)}
+        cf_dict: dict[str, Any] = {"crs_wkt": self.to_wkt(wkt_version)}
 
         # handle bound CRS
         if (
             self.is_bound
             and self.coordinate_operation
             and self.coordinate_operation.towgs84
             and self.source_crs
         ):
-            sub_cf: Dict[str, Any] = self.source_crs.to_cf(
+            sub_cf: dict[str, Any] = self.source_crs.to_cf(
                 wkt_version=wkt_version,
                 errcheck=errcheck,
             )
             sub_cf.pop("crs_wkt")
             cf_dict.update(sub_cf)
             cf_dict["towgs84"] = self.coordinate_operation.towgs84
             return cf_dict
@@ -869,26 +869,26 @@
         )
 
         # build compound CRS
         return CompoundCRS(
             name="undefined", components=[bound_crs or projected_crs, vertical_crs]
         )
 
-    def cs_to_cf(self) -> List[dict]:
+    def cs_to_cf(self) -> list[dict]:
         """
         .. versionadded:: 3.0.0
 
         This converts all coordinate systems (cs) in the CRS
         to a list of Climate and Forecast (CF) Version 1.8 dicts.
 
         :ref:`build_crs_cf`
 
         Returns
         -------
-        List[dict]:
+        list[dict]:
             CF-1.8 version of the coordinate systems.
         """
         cf_axis_list = []
 
         def rotated_pole(crs):
             try:
                 return (
@@ -1029,21 +1029,21 @@
         return (
             None
             if self._crs.target_crs is None
             else self.__class__(self._crs.target_crs)
         )
 
     @property
-    def sub_crs_list(self) -> List["CRS"]:
+    def sub_crs_list(self) -> list["CRS"]:
         """
         If the CRS is a compound CRS, it will return a list of sub CRS objects.
 
         Returns
         -------
-        List[CRS]
+        list[CRS]
         """
         return [self.__class__(sub_crs) for sub_crs in self._crs.sub_crs_list]
 
     @property
     def utm_zone(self) -> Optional[str]:
         """
         .. versionadded:: 2.6.0
@@ -1085,23 +1085,23 @@
         -------
         str:
             The name of the type of the CRS object.
         """
         return self._crs.type_name
 
     @property
-    def axis_info(self) -> List[Axis]:
+    def axis_info(self) -> list[Axis]:
         """
         Retrieves all relevant axis information in the CRS.
         If it is a Bound CRS, it gets the axis list from the Source CRS.
         If it is a Compound CRS, it gets the axis list from the Sub CRS list.
 
         Returns
         -------
-        List[Axis]:
+        list[Axis]:
             The list of axis information.
         """
         return self._crs.axis_info
 
     @property
     def area_of_use(self) -> Optional[AreaOfUse]:
         """
@@ -1193,40 +1193,47 @@
         """
         return self._crs.scope
 
     def to_wkt(
         self,
         version: Union[WktVersion, str] = WktVersion.WKT2_2019,
         pretty: bool = False,
+        output_axis_rule: Optional[bool] = None,
     ) -> str:
         """
         Convert the projection to a WKT string.
 
         Version options:
           - WKT2_2015
           - WKT2_2015_SIMPLIFIED
           - WKT2_2019
           - WKT2_2019_SIMPLIFIED
           - WKT1_GDAL
           - WKT1_ESRI
 
+        .. versionadded:: 3.6.0 output_axis_rule
 
         Parameters
         ----------
         version: pyproj.enums.WktVersion, optional
             The version of the WKT output.
             Default is :attr:`pyproj.enums.WktVersion.WKT2_2019`.
         pretty: bool, default=False
             If True, it will set the output to be a multiline string.
+        output_axis_rule: bool, optional, default=None
+            If True, it will set the axis rule on any case. If false, never.
+            None for AUTO, that depends on the CRS and version.
 
         Returns
         -------
         str
         """
-        wkt = self._crs.to_wkt(version=version, pretty=pretty)
+        wkt = self._crs.to_wkt(
+            version=version, pretty=pretty, output_axis_rule=output_axis_rule
+        )
         if wkt is None:
             raise CRSError(
                 f"CRS cannot be converted to a WKT string of a '{version}' version. "
                 "Select a different version of a WKT string or edit your CRS."
             )
         return wkt
 
@@ -1365,15 +1372,15 @@
         """
         return self._crs.to_authority(
             auth_name=auth_name, min_confidence=min_confidence
         )
 
     def list_authority(
         self, auth_name: Optional[str] = None, min_confidence: int = 70
-    ) -> List[AuthorityMatchInfo]:
+    ) -> list[AuthorityMatchInfo]:
         """
         .. versionadded:: 3.2.0
 
         Return the authority names and codes best matching the CRS.
 
         Example:
 
@@ -1400,15 +1407,15 @@
             The name of the authority to filter by.
         min_confidence: int, default=70
             A value between 0-100 where 100 is the most confident.
             :ref:`min_confidence`
 
         Returns
         -------
-        List[AuthorityMatchInfo]:
+        list[AuthorityMatchInfo]:
             List of authority matches for the CRS.
         """
         return self._crs.list_authority(
             auth_name=auth_name, min_confidence=min_confidence
         )
 
     def to_3d(self, name: Optional[str] = None) -> "CRS":
@@ -1429,14 +1436,31 @@
 
         Returns
         -------
         CRS
         """
         return self.__class__(self._crs.to_3d(name=name))
 
+    def to_2d(self, name: Optional[str] = None) -> "CRS":
+        """
+        .. versionadded:: 3.6.0
+
+        Convert the current CRS to the 2D version if it makes sense.
+
+        Parameters
+        ----------
+        name: str, optional
+            CRS name. Defaults to use the name of the original CRS.
+
+        Returns
+        -------
+        CRS
+        """
+        return self.__class__(self._crs.to_2d(name=name))
+
     @property
     def is_geographic(self) -> bool:
         """
         This checks if the CRS is geographic.
         It will check if it has a geographic CRS
         in the sub CRS if it is a compound CRS and will check if
         the source CRS is geographic if it is a bound CRS.
@@ -1538,30 +1562,30 @@
             True if CRS is a Derived CRS.
         """
         return self._crs.is_derived
 
     def __eq__(self, other: Any) -> bool:
         return self.equals(other)
 
-    def __getstate__(self) -> Dict[str, str]:
+    def __getstate__(self) -> dict[str, str]:
         return {"srs": self.srs}
 
-    def __setstate__(self, state: Dict[str, Any]):
+    def __setstate__(self, state: dict[str, Any]):
         self.__dict__.update(state)
         self._local = CRSLocal()
 
     def __hash__(self) -> int:
         return hash(self.to_wkt())
 
     def __str__(self) -> str:
         return self.srs
 
     def __repr__(self) -> str:
         # get axis information
-        axis_info_list: List[str] = []
+        axis_info_list: list[str] = []
         for axis in self.axis_info:
             axis_info_list.extend(["- ", str(axis), "\n"])
         axis_info_str = "".join(axis_info_list)
 
         # get coordinate system & sub CRS info
         source_crs_repr = ""
         sub_crs_repr = ""
@@ -1620,15 +1644,15 @@
 
     .. versionadded:: 3.2.0
 
     See: https://github.com/pyproj4/pyproj/issues/847
     """
 
     @property
-    def _expected_types(self) -> Tuple[str, ...]:
+    def _expected_types(self) -> tuple[str, ...]:
         """
         These are the type names of the CRS class
         that are expected when using the from_* methods.
         """
         raise NotImplementedError
 
     def _check_type(self):
@@ -1707,21 +1731,21 @@
         CRS:
             The hub CRS of a BoundCRS or the target CRS of a CoordinateOperation.
 
         """
         return None if self._crs.target_crs is None else CRS(self._crs.target_crs)
 
     @property
-    def sub_crs_list(self) -> List["CRS"]:
+    def sub_crs_list(self) -> list["CRS"]:
         """
         If the CRS is a compound CRS, it will return a list of sub CRS objects.
 
         Returns
         -------
-        List[CRS]
+        list[CRS]
         """
         return [CRS(sub_crs) for sub_crs in self._crs.sub_crs_list]
 
     def to_3d(self, name: Optional[str] = None) -> "CRS":
         """
         .. versionadded:: 3.1.0
 
@@ -1996,21 +2020,21 @@
     .. versionadded:: 2.5.0
 
     This class is for building a Compound CRS.
     """
 
     _expected_types = ("Compound CRS",)
 
-    def __init__(self, name: str, components: List[Any]) -> None:
+    def __init__(self, name: str, components: list[Any]) -> None:
         """
         Parameters
         ----------
         name: str
             The name of the Compound CRS.
-        components: List[Any], optional
+        components: list[Any], optional
             List of CRS to create a Compound Coordinate System.
             List of anything accepted by :meth:`pyproj.crs.CRS.from_user_input`
         """
         compound_crs_json = {
             "$schema": "https://proj.org/schemas/v0.2/projjson.schema.json",
             "type": "CompoundCRS",
             "name": name,
```

### Comparing `pyproj-3.5.0rc0/pyproj/crs/datum.py` & `pyproj-3.6.0rc0/pyproj/crs/datum.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 This module is for building datums to be used when
 building a CRS.
 """
-from typing import Any, Dict, Optional, Union
+from typing import Any, Optional, Union
 
 from pyproj._crs import Datum, Ellipsoid, PrimeMeridian
 
 
 class CustomDatum(Datum):
     """
     .. versionadded:: 2.5.0
@@ -71,15 +71,15 @@
         semi_minor_axis: float, optional
             The semi minor axis in meters.
             Required if missing inverse_flattening and radius.
         radius: float, optional
             The radius in meters. Can only be used alone.
             Cannot be mixed with other parameters.
         """
-        ellipsoid_json: Dict[str, Union[float, str]] = {
+        ellipsoid_json: dict[str, Union[float, str]] = {
             "$schema": "https://proj.org/schemas/v0.2/projjson.schema.json",
             "type": "Ellipsoid",
             "name": name,
         }
         if semi_major_axis is not None:
             ellipsoid_json["semi_major_axis"] = semi_major_axis
         if inverse_flattening is not None:
```

### Comparing `pyproj-3.5.0rc0/pyproj/crs/enums.py` & `pyproj-3.6.0rc0/pyproj/crs/enums.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/database.pyi` & `pyproj-3.6.0rc0/pyproj/database.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, NamedTuple, Optional, Union
+from typing import NamedTuple, Optional, Union
 
 from pyproj.aoi import AreaOfInterest, AreaOfUse
 from pyproj.enums import PJType
 
 class Unit(NamedTuple):
     auth_name: str
     code: str
@@ -12,35 +12,35 @@
     proj_short_name: Optional[str]
     deprecated: bool
 
 def get_units_map(
     auth_name: Optional[str] = None,
     category: Optional[str] = None,
     allow_deprecated: bool = False,
-) -> Dict[str, Unit]: ...
-def get_authorities() -> List[str]: ...
+) -> dict[str, Unit]: ...
+def get_authorities() -> list[str]: ...
 def get_codes(
     auth_name: str, pj_type: Union[PJType, str], allow_deprecated: bool = False
-) -> List[str]: ...
+) -> list[str]: ...
 
 class CRSInfo(NamedTuple):
     auth_name: str
     code: str
     name: str
     type: PJType
     deprecated: bool
     area_of_use: Optional[AreaOfUse]
     projection_method_name: Optional[str]
 
 def query_crs_info(
     auth_name: Optional[str] = None,
-    pj_types: Union[PJType, List[PJType], None] = None,
+    pj_types: Union[PJType, list[PJType], None] = None,
     area_of_interest: Optional[AreaOfInterest] = None,
     contains: bool = False,
     allow_deprecated: bool = False,
-) -> List[CRSInfo]: ...
+) -> list[CRSInfo]: ...
 def query_utm_crs_info(
     datum_name: Optional[str] = None,
     area_of_interest: Optional[AreaOfInterest] = None,
     contains: bool = False,
-) -> List[CRSInfo]: ...
+) -> list[CRSInfo]: ...
 def get_database_metadata(key: str) -> Optional[str]: ...
```

### Comparing `pyproj-3.5.0rc0/pyproj/database.pyx` & `pyproj-3.6.0rc0/pyproj/database.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     """
     .. versionadded:: 2.4.0
 
     See: :c:func:`proj_get_authorities_from_database`
 
     Returns
     -------
-    List[str]:
+    list[str]:
         Authorities in PROJ database.
     """
     cdef PJ_CONTEXT* context = pyproj_context_create()
     cdef PROJ_STRING_LIST proj_auth_list = proj_get_authorities_from_database(context)
     if proj_auth_list == NULL:
         pyproj_context_destroy(context)
         return []
@@ -98,15 +98,15 @@
     pj_type: pyproj.enums.PJType
         The type of object to get the authorities.
     allow_deprecated: bool, default=False
         Allow a deprecated code in the return.
 
     Returns
     -------
-    List[str]:
+    list[str]:
         Codes associated with authorities in PROJ database.
     """
     cdef PJ_CONTEXT* context = NULL
     cdef PJ_TYPE cpj_type = get_pj_type(pj_type)
     cdef PROJ_STRING_LIST proj_code_list = NULL
     try:
         context = pyproj_context_create()
@@ -181,30 +181,30 @@
 
     See: :c:func:`proj_get_crs_info_list_from_database`
 
     Parameters
     ----------
     auth_name: Optional[str], optional
         The name of the authority. Default is all authorities.
-    pj_types: Union[pyproj.enums.PJType, List[pyproj.enums.PJType], None], optional
+    pj_types: Union[pyproj.enums.PJType, list[pyproj.enums.PJType], None], optional
         The type(s) of CRS to get the information (i.e. the types with CRS in the name).
         If None is provided, it will use all of types (i.e. PJType.CRS).
     area_of_interest: Optional[AreaOfInterest], optional
         Filter returned CRS by the area of interest. Default method is intersection.
     contains: bool, default=False
         Only works if the area of interest is passed in.
         If True, then only CRS whose area of use entirely contains the specified
         bounding box will be returned. If False, then only CRS whose area of use
         intersects the specified bounding box will be returned.
     allow_deprecated: bool, default=False
         Allow a deprecated code in the return.
 
     Returns
     -------
-    List[CRSInfo]:
+    list[CRSInfo]:
         CRS information from the PROJ database.
     """
     cdef PJ_CONTEXT* context = NULL
     cdef PJ_TYPE *pj_type_list = NULL
     cdef PROJ_CRS_LIST_PARAMETERS *query_params = NULL
     cdef PROJ_CRS_INFO **crs_info_list = NULL
     cdef const char* c_auth_name = NULL
@@ -304,15 +304,15 @@
         Only works if the area of interest is passed in.
         If True, then only CRS whose area of use entirely contains the specified
         bounding box will be returned. If False, then only CRS whose area of use
         intersects the specified bounding box will be returned.
 
     Returns
     -------
-    List[CRSInfo]:
+    list[CRSInfo]:
         UTM CRS information from the PROJ database.
     """
     projected_crs = query_crs_info(
         auth_name="EPSG",
         pj_types=PJType.PROJECTED_CRS,
         area_of_interest=area_of_interest,
         contains=contains,
@@ -381,15 +381,15 @@
         Category of the unit: one of "linear", "linear_per_time", "angular",
         "angular_per_time", "scale", "scale_per_time" or "time". Default is all.
     allow_deprecated: bool, default=False
         Whether or not to allow deprecated units.
 
     Returns
     -------
-    Dict[str, Unit]
+    dict[str, Unit]
     """
     cdef const char* c_auth_name = NULL
     cdef const char* c_category = NULL
     cdef bytes b_auth_name
     cdef bytes b_category
     if auth_name is not None:
         b_auth_name = cstrencode(auth_name)
```

### Comparing `pyproj-3.5.0rc0/pyproj/datadir.py` & `pyproj-3.6.0rc0/pyproj/datadir.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/enums.py` & `pyproj-3.6.0rc0/pyproj/enums.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/exceptions.py` & `pyproj-3.6.0rc0/pyproj/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/geod.py` & `pyproj-3.6.0rc0/pyproj/geod.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,39 +15,39 @@
     "GeodIntermediateFlag",
     "GeodIntermediateReturn",
     "reverse_azimuth",
 ]
 
 import math
 import warnings
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Optional, Union
 
 from pyproj._geod import Geod as _Geod
 from pyproj._geod import GeodIntermediateReturn, geodesic_version_str
 from pyproj._geod import reverse_azimuth as _reverse_azimuth
 from pyproj.enums import GeodIntermediateFlag
 from pyproj.exceptions import GeodError
 from pyproj.list import get_ellps_map
 from pyproj.utils import DataType, _convertback, _copytobuffer
 
 pj_ellps = get_ellps_map()
 
 
-def _params_from_ellps_map(ellps: str) -> Tuple[float, float, float, float, bool]:
+def _params_from_ellps_map(ellps: str) -> tuple[float, float, float, float, bool]:
     """
     Build Geodesic parameters from PROJ ellips map
 
     Parameter
     ---------
     ellps: str
         The name of the ellipse in the map.
 
     Returns
     -------
-    Tuple[float, float, float, float, bool]
+    tuple[float, float, float, float, bool]
 
     """
     ellps_dict = pj_ellps[ellps]
     semi_major_axis: float = ellps_dict["a"]
     sphere = False
     if ellps_dict["description"] == "Normal Sphere":
         sphere = True
@@ -58,15 +58,15 @@
     elif "rf" in ellps_dict:
         flattening = 1.0 / ellps_dict["rf"]
         semi_minor_axis = semi_major_axis * (1.0 - flattening)
         eccentricity_squared = 1.0 - semi_minor_axis**2 / semi_major_axis**2
     return semi_major_axis, semi_minor_axis, flattening, eccentricity_squared, sphere
 
 
-def _params_from_kwargs(kwargs: Dict) -> Tuple[float, float, float, float]:
+def _params_from_kwargs(kwargs: dict) -> tuple[float, float, float, float]:
     """
     Build Geodesic parameters from input kwargs:
 
     - a: the semi-major axis (required).
 
     Need least one of these parameters.
 
@@ -79,15 +79,15 @@
     Parameter
     ---------
     kwargs: dict
         The input kwargs for an ellipse.
 
     Returns
     -------
-    Tuple[float, float, float, float]
+    tuple[float, float, float, float]
 
     """
     semi_major_axis = kwargs["a"]
     if "b" in kwargs:
         semi_minor_axis = kwargs["b"]
         eccentricity_squared = 1.0 - semi_minor_axis**2 / semi_major_axis**2
         flattening = (semi_major_axis - semi_minor_axis) / semi_major_axis
@@ -199,15 +199,15 @@
         >>> g2 = Geod('+ellps=clrk66') # use proj4 style initialization string
         >>> az12,az21,dist = g2.inv(boston_lon,boston_lat,portland_lon,portland_lat)
         >>> f"{az12:.3f} {az21:.3f} {dist:.3f}"
         '-66.531 75.654 4164192.708'
         """
         # if initparams is a proj-type init string,
         # convert to dict.
-        ellpsd: Dict[str, Union[str, float]] = {}
+        ellpsd: dict[str, Union[str, float]] = {}
         if initstring is not None:
             for kvpair in initstring.split():
                 # Actually only +a and +b are needed
                 # We can ignore safely any parameter that doesn't have a value
                 if kvpair.find("=") == -1:
                     continue
                 key, val = kvpair.split("=")
@@ -247,15 +247,15 @@
         lons: Any,
         lats: Any,
         az: Any,
         dist: Any,
         radians: bool = False,
         inplace: bool = False,
         return_back_azimuth: bool = True,
-    ) -> Tuple[Any, Any, Any]:
+    ) -> tuple[Any, Any, Any]:
         """
         Forward transformation
 
         Determine longitudes, latitudes and back azimuths of terminus
         points given longitudes and latitudes of initial points,
         plus forward azimuths and distances.
 
@@ -339,15 +339,15 @@
         lons1: Any,
         lats1: Any,
         lons2: Any,
         lats2: Any,
         radians: bool = False,
         inplace: bool = False,
         return_back_azimuth: bool = True,
-    ) -> Tuple[Any, Any, Any]:
+    ) -> tuple[Any, Any, Any]:
         """
 
         Inverse transformation
 
         Determine forward and back azimuths, plus distances
         between initial points and terminus points.
 
@@ -432,15 +432,15 @@
         lat1: float,
         lon2: float,
         lat2: float,
         npts: int,
         radians: bool = False,
         initial_idx: int = 1,
         terminus_idx: int = 1,
-    ) -> List:
+    ) -> list:
         """
         .. versionadded:: 3.1.0 initial_idx, terminus_idx
 
         Given a single initial point and terminus point, returns
         a list of longitude/latitude pairs describing npts equally
         spaced intermediate points along the geodesic between the
         initial and terminus points.
@@ -520,25 +520,26 @@
             between the initial and terminus points.
         """
 
         res = self._inv_or_fwd_intermediate(
             lon1=lon1,
             lat1=lat1,
             lon2_or_azi1=lon2,
-            lat2_or_nan=lat2,
+            lat2=lat2,
             npts=npts,
             del_s=0,
             radians=radians,
             initial_idx=initial_idx,
             terminus_idx=terminus_idx,
             flags=GeodIntermediateFlag.AZIS_DISCARD,
             out_lons=None,
             out_lats=None,
             out_azis=None,
             return_back_azimuth=False,
+            is_fwd=False,
         )
         return list(zip(res.lons, res.lats))
 
     def inv_intermediate(
         self,
         lon1: float,
         lat1: float,
@@ -684,25 +685,26 @@
                 "Otherwise, to restore old behaviour, set return_back_azimuth=False."
                 "This warning will be removed in future version."
             )
         return super()._inv_or_fwd_intermediate(
             lon1=lon1,
             lat1=lat1,
             lon2_or_azi1=lon2,
-            lat2_or_nan=lat2,
+            lat2=lat2,
             npts=npts,
             del_s=del_s,
             radians=radians,
             initial_idx=initial_idx,
             terminus_idx=terminus_idx,
             flags=int(flags),
             out_lons=out_lons,
             out_lats=out_lats,
             out_azis=out_azis,
             return_back_azimuth=return_back_azimuth,
+            is_fwd=False,
         )
 
     def fwd_intermediate(
         self,
         lon1: float,
         lat1: float,
         azi1: float,
@@ -831,25 +833,26 @@
                 "Otherwise, to restore old behaviour, set return_back_azimuth=False."
                 "This warning will be removed in future version."
             )
         return super()._inv_or_fwd_intermediate(
             lon1=lon1,
             lat1=lat1,
             lon2_or_azi1=azi1,
-            lat2_or_nan=math.nan,
+            lat2=math.nan,
             npts=npts,
             del_s=del_s,
             radians=radians,
             initial_idx=initial_idx,
             terminus_idx=terminus_idx,
             flags=int(flags),
             out_lons=out_lons,
             out_lats=out_lats,
             out_azis=out_azis,
             return_back_azimuth=return_back_azimuth,
+            is_fwd=True,
         )
 
     def line_length(self, lons: Any, lats: Any, radians: bool = False) -> float:
         """
         .. versionadded:: 2.3.0
 
         Calculate the total distance between points along a line (meters).
@@ -920,15 +923,15 @@
         iny = _copytobuffer(lats)[0]
         self._line_length(inx, iny, radians=radians)
         line_lengths = _convertback(x_data_type, inx)
         return line_lengths if x_data_type == DataType.FLOAT else line_lengths[:-1]
 
     def polygon_area_perimeter(
         self, lons: Any, lats: Any, radians: bool = False
-    ) -> Tuple[float, float]:
+    ) -> tuple[float, float]:
         """
         .. versionadded:: 2.3.0
 
         A simple interface for computing the area (meters^2) and perimeter (meters)
         of a geodesic polygon.
 
         Arbitrarily complex polygons are allowed. In the case self-intersecting
@@ -1016,15 +1019,15 @@
             for geom in geometry.geoms:
                 total_length += self.geometry_length(geom, radians=radians)
             return total_length
         raise GeodError("Invalid geometry provided.")
 
     def geometry_area_perimeter(
         self, geometry, radians: bool = False
-    ) -> Tuple[float, float]:
+    ) -> tuple[float, float]:
         """
         .. versionadded:: 2.3.0
 
         A simple interface for computing the area (meters^2) and perimeter (meters)
         of a geodesic polygon as a shapely geometry.
 
         Arbitrarily complex polygons are allowed.  In the case self-intersecting
```

### Comparing `pyproj-3.5.0rc0/pyproj/list.pyx` & `pyproj-3.6.0rc0/pyproj/list.pyx`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/network.py` & `pyproj-3.6.0rc0/pyproj/network.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/pyproj/proj.pxi` & `pyproj-3.6.0rc0/pyproj/proj.pxi`

 * *Files 1% similar despite different names*

```diff
@@ -474,14 +474,19 @@
         double north_lat_degree
     )
     void proj_operation_factory_context_set_allow_ballpark_transformations(
         PJ_CONTEXT *ctx,
         PJ_OPERATION_FACTORY_CONTEXT *factory_ctx,
         int allow
     )
+    void proj_operation_factory_context_set_discard_superseded(
+        PJ_CONTEXT *ctx,
+        PJ_OPERATION_FACTORY_CONTEXT *factory_ctx,
+        int discard
+    )
     void proj_operation_factory_context_set_desired_accuracy(
         PJ_CONTEXT *ctx,
         PJ_OPERATION_FACTORY_CONTEXT *factory_ctx,
         double accuracy
     )
     ctypedef enum PROJ_SPATIAL_CRITERION:
         PROJ_SPATIAL_CRITERION_STRICT_CONTAINMENT
```

### Comparing `pyproj-3.5.0rc0/pyproj/proj.py` & `pyproj-3.6.0rc0/pyproj/proj.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 Calling a Proj class instance with the arguments lon, lat will
 convert lon/lat (in degrees) to x/y native map projection
 coordinates (in meters).
 """
 import re
 import warnings
-from typing import Any, Optional, Tuple, Type
+from typing import Any, Optional
 
 from pyproj._compat import cstrencode
 from pyproj._transformer import Factors
 from pyproj.crs import CRS
 from pyproj.enums import TransformDirection
 from pyproj.list import get_proj_operations_map
 from pyproj.transformer import Transformer, TransformerFromPipeline
@@ -136,15 +136,15 @@
     def __call__(
         self,
         longitude: Any,
         latitude: Any,
         inverse: bool = False,
         errcheck: bool = False,
         radians: bool = False,
-    ) -> Tuple[Any, Any]:
+    ) -> tuple[Any, Any]:
         """
         Calling a Proj class instance with the arguments lon, lat will
         convert lon/lat (in degrees) to x/y native map projection
         coordinates (in meters).
 
         Inputs should be doubles (they will be cast to doubles if they
         are not, causing a slight performance hit).
@@ -181,15 +181,15 @@
             in pyproj 3.
         errcheck: bool, default=False
             If True, an exception is raised if the errors are found in the process.
             If False, ``inf`` is returned for errors.
 
         Returns
         -------
-        Tuple[Any, Any]:
+        tuple[Any, Any]:
             The transformed coordinates.
         """
         if inverse:
             direction = TransformDirection.INVERSE
         else:
             direction = TransformDirection.FORWARD
         return self.transform(
@@ -290,10 +290,10 @@
         return self.crs.geodetic_crs.to_proj4(4) if self.crs.geodetic_crs else None
 
     def to_latlong(self) -> "Proj":
         """return a new Proj instance which is the geographic (lat/lon)
         coordinate version of the current projection"""
         return Proj(self.crs.geodetic_crs)
 
-    def __reduce__(self) -> Tuple[Type["Proj"], Tuple[str]]:
+    def __reduce__(self) -> tuple[type["Proj"], tuple[str]]:
         """special method that allows pyproj.Proj instance to be pickled"""
         return self.__class__, (self.crs.srs,)
```

### Comparing `pyproj-3.5.0rc0/pyproj/sync.py` & `pyproj-3.6.0rc0/pyproj/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 """
 import hashlib
 import json
 import os
 from datetime import datetime
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Optional
 from urllib.request import urlretrieve
 
 from pyproj._sync import get_proj_endpoint
 from pyproj.aoi import BBox
 from pyproj.datadir import get_data_dir, get_user_data_dir
 
 
-def _bbox_from_coords(coords: List) -> Optional[BBox]:
+def _bbox_from_coords(coords: list) -> Optional[BBox]:
     """
     Get the bounding box from coordinates
     """
     try:
         xxx, yyy = zip(*coords)
         return BBox(west=min(xxx), south=min(yyy), east=max(xxx), north=max(yyy))
     except ValueError:
@@ -35,15 +35,15 @@
             coord_bbox.west = min(coord_bbox.west, bbox.west)
             coord_bbox.south = min(coord_bbox.south, bbox.south)
             coord_bbox.north = max(coord_bbox.north, bbox.north)
             coord_bbox.east = max(coord_bbox.east, bbox.east)
     return coord_bbox
 
 
-def _bbox_from_geom(geom: Dict[str, Any]) -> Optional[BBox]:
+def _bbox_from_geom(geom: dict[str, Any]) -> Optional[BBox]:
     """
     Get the bounding box from geojson geometry
     """
     if "coordinates" not in geom or "type" not in geom:
         return None
     coordinates = geom["coordinates"]
     if geom["type"] != "MultiPolygon":
@@ -72,15 +72,15 @@
             grid_bbox.south = min(grid_bbox.south, bbox.south)
             grid_bbox.north = max(grid_bbox.north, bbox.north)
             grid_bbox.east = max(grid_bbox.east, bbox.east)
     return grid_bbox
 
 
 def _filter_bbox(
-    feature: Dict[str, Any], bbox: BBox, spatial_test: str, include_world_coverage: bool
+    feature: dict[str, Any], bbox: BBox, spatial_test: str, include_world_coverage: bool
 ) -> bool:
     """
     Filter by the bounding box. Designed to use with 'filter'
     """
     geom = feature.get("geometry")
     if geom is not None:
         geom_bbox = _bbox_from_geom(geom)
@@ -98,15 +98,15 @@
             geom_bbox.west -= 360
             geom_bbox.east -= 360
         return getattr(bbox, spatial_test)(geom_bbox)
     return False
 
 
 def _filter_properties(
-    feature: Dict[str, Any],
+    feature: dict[str, Any],
     source_id: Optional[str] = None,
     area_of_use: Optional[str] = None,
     filename: Optional[str] = None,
 ) -> bool:
     """
     Filter by the properties. Designed to use with 'filter'
     """
@@ -136,15 +136,15 @@
         return False
     for data_dir in get_data_dir().split(os.pathsep):
         if Path(data_dir, grid_name).exists():
             return False
     return True
 
 
-def _filter_download_needed(feature: Dict[str, Any]) -> bool:
+def _filter_download_needed(feature: dict[str, Any]) -> bool:
     """
     Filter grids so only those that need to be downloaded are included.
     """
     properties = feature.get("properties")
     if not properties:
         return False
     filename = properties.get("name")
@@ -183,19 +183,19 @@
     finally:
         try:
             os.remove(tmp_path)
         except FileNotFoundError:
             pass
 
 
-def _load_grid_geojson(target_directory=None) -> Dict[str, Any]:
+def _load_grid_geojson(target_directory=None) -> dict[str, Any]:
     """
     Returns
     -------
-    Dict[str, Any]:
+    dict[str, Any]:
         The PROJ grid data list.
     """
     if target_directory is None:
         target_directory = get_user_data_dir(True)
     local_path = Path(target_directory, "files.geojson")
     if not local_path.exists() or (
         (datetime.utcnow() - datetime.fromtimestamp(local_path.stat().st_mtime)).days
@@ -214,15 +214,15 @@
     area_of_use: Optional[str] = None,
     filename: Optional[str] = None,
     bbox: Optional[BBox] = None,
     spatial_test: str = "intersects",
     include_world_coverage: bool = True,
     include_already_downloaded: bool = False,
     target_directory: Optional[str] = None,
-) -> Tuple:
+) -> tuple:
     """
     Get a list of transform grids that can be downloaded.
 
     Parameters
     ----------
     source_id: str, optional
     area_of_use: str, optional
@@ -236,15 +236,15 @@
         If True, it will list grids regardless of if they are downloaded.
     target_directory: Union[str, Path, None], optional
         The directory to download the geojson file to.
         Default is the user writable directory.
 
     Returns
     -------
-    List[Dict[str, Any]]:
+    list[dict[str, Any]]:
         A list of geojson data of containing information about features
         that can be downloaded.
     """
     features = _load_grid_geojson(target_directory=target_directory)["features"]
     if bbox is not None:
         if bbox.west > 180 and bbox.east > bbox.west:
             bbox.west -= 360
```

### Comparing `pyproj-3.5.0rc0/pyproj/transformer.py` & `pyproj-3.6.0rc0/pyproj/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,18 +8,19 @@
     "TransformerGroup",
     "AreaOfInterest",
 ]
 import threading
 import warnings
 from abc import ABC, abstractmethod
 from array import array
+from collections.abc import Iterable, Iterator
 from dataclasses import dataclass
 from itertools import chain, islice
 from pathlib import Path
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union, overload
+from typing import Any, Optional, Union, overload
 
 from pyproj import CRS
 from pyproj._compat import cstrencode
 from pyproj._crs import AreaOfUse, CoordinateOperation
 from pyproj._datadir import _clear_proj_error
 from pyproj._transformer import (  # noqa: F401 pylint: disable=unused-import
     AreaOfInterest,
@@ -157,19 +158,21 @@
         crs_from: Any,
         crs_to: Any,
         always_xy: bool = False,
         area_of_interest: Optional[AreaOfInterest] = None,
         authority: Optional[str] = None,
         accuracy: Optional[float] = None,
         allow_ballpark: bool = True,
+        allow_superseded: bool = False,
     ) -> None:
         """Get all possible transformations from a :obj:`pyproj.crs.CRS`
         or input used to create one.
 
         .. versionadded:: 3.4.0 authority, accuracy, allow_ballpark
+        .. versionadded:: 3.6.0 allow_superseded
 
         Parameters
         ----------
         crs_from: pyproj.crs.CRS or input used to create one
             Projection of input data.
         crs_to: pyproj.crs.CRS or input used to create one
             Projection of output data.
@@ -191,40 +194,45 @@
             namespace (e.g. EPSG).
         accuracy: float, optional
             The minimum desired accuracy (in metres) of the candidate
             coordinate operations.
         allow_ballpark: bool, default=True
             Set to False to disallow the use of Ballpark transformation
             in the candidate coordinate operations. Default is to allow.
+        allow_superseded: bool, default=False
+            Set to True to allow the use of superseded (but not deprecated)
+            transformations in the candidate coordinate operations. Default is
+            to disallow.
 
         """
         super().__init__(
             CRS.from_user_input(crs_from)._crs,
             CRS.from_user_input(crs_to)._crs,
             always_xy=always_xy,
             area_of_interest=area_of_interest,
             authority=authority,
             accuracy=-1 if accuracy is None else accuracy,
             allow_ballpark=allow_ballpark,
+            allow_superseded=allow_superseded,
         )
         for iii, transformer in enumerate(self._transformers):
             # pylint: disable=unsupported-assignment-operation
             self._transformers[iii] = Transformer(TransformerUnsafe(transformer))
 
     @property
-    def transformers(self) -> List["Transformer"]:
+    def transformers(self) -> list["Transformer"]:
         """
         list[:obj:`Transformer`]:
             List of available :obj:`Transformer`
             associated with the transformation.
         """
         return self._transformers
 
     @property
-    def unavailable_operations(self) -> List[CoordinateOperation]:
+    def unavailable_operations(self) -> list[CoordinateOperation]:
         """
         list[:obj:`pyproj.crs.CoordinateOperation`]:
             List of :obj:`pyproj.crs.CoordinateOperation` that are not
             available due to missing grids.
         """
         return self._unavailable_operations
 
@@ -325,18 +333,18 @@
                 "'from_crs' or 'from_pipeline'."
             )
 
         self._local = TransformerLocal()
         self._local.transformer = transformer_maker()
         self._transformer_maker = transformer_maker
 
-    def __getstate__(self) -> Dict[str, Any]:
+    def __getstate__(self) -> dict[str, Any]:
         return {"_transformer_maker": self._transformer_maker}
 
-    def __setstate__(self, state: Dict[str, Any]):
+    def __setstate__(self, state: dict[str, Any]):
         self.__dict__.update(state)
         self._local = TransformerLocal()
         self._local.transformer = self._transformer_maker()
 
     @property
     def _transformer(self):
         """
@@ -418,21 +426,21 @@
         -------
         str:
             Scope of object.
         """
         return self._transformer.scope
 
     @property
-    def operations(self) -> Optional[Tuple[CoordinateOperation]]:
+    def operations(self) -> Optional[tuple[CoordinateOperation]]:
         """
         .. versionadded:: 2.4.0
 
         Returns
         -------
-        Tuple[CoordinateOperation]:
+        tuple[CoordinateOperation]:
             The operations in a concatenated operation.
         """
         return self._transformer.operations
 
     def get_last_used_operation(self) -> "Transformer":
         """
         .. versionadded:: 3.4.0
@@ -671,42 +679,42 @@
         self,
         xx: Any,
         yy: Any,
         radians: bool = False,
         errcheck: bool = False,
         direction: Union[TransformDirection, str] = TransformDirection.FORWARD,
         inplace: bool = False,
-    ) -> Tuple[Any, Any]:
+    ) -> tuple[Any, Any]:
         ...
 
     @overload
     def transform(  # pylint: disable=invalid-name
         self,
         xx: Any,
         yy: Any,
         zz: Any,
         radians: bool = False,
         errcheck: bool = False,
         direction: Union[TransformDirection, str] = TransformDirection.FORWARD,
         inplace: bool = False,
-    ) -> Tuple[Any, Any, Any]:
+    ) -> tuple[Any, Any, Any]:
         ...
 
     @overload
     def transform(  # pylint: disable=invalid-name
         self,
         xx: Any,
         yy: Any,
         zz: Any,
         tt: Any,
         radians: bool = False,
         errcheck: bool = False,
         direction: Union[TransformDirection, str] = TransformDirection.FORWARD,
         inplace: bool = False,
-    ) -> Tuple[Any, Any, Any, Any]:
+    ) -> tuple[Any, Any, Any, Any]:
         ...
 
     def transform(  # pylint: disable=invalid-name
         self,
         xx,
         yy,
         zz=None,
@@ -840,15 +848,15 @@
             direction=direction,
             radians=radians,
             errcheck=errcheck,
         )
         # if inputs were lists, tuples or floats, convert back.
         outx = _convertback(x_data_type, inx)
         outy = _convertback(y_data_type, iny)
-        return_data: Tuple[Any, ...] = (outx, outy)
+        return_data: tuple[Any, ...] = (outx, outy)
         if inz is not None:
             return_data += (_convertback(z_data_type, inz),)
         if intime is not None:
             return_data += (_convertback(t_data_type, intime),)
         return return_data
 
     def itransform(
@@ -973,28 +981,27 @@
                 switch=switch,
                 direction=direction,
                 time_3rd=time_3rd,
                 radians=radians,
                 errcheck=errcheck,
             )
 
-            for point in zip(*([iter(buff)] * stride)):
-                yield point
+            yield from zip(*([iter(buff)] * stride))
 
     def transform_bounds(
         self,
         left: float,
         bottom: float,
         right: float,
         top: float,
         densify_pts: int = 21,
         radians: bool = False,
         errcheck: bool = False,
         direction: Union[TransformDirection, str] = TransformDirection.FORWARD,
-    ) -> Tuple[float, float, float, float]:
+    ) -> tuple[float, float, float, float]:
         """
         .. versionadded:: 3.1.0
 
         See: :c:func:`proj_trans_bounds`
 
         Transform boundary densifying the edges to account for nonlinear
         transformations along these edges and extracting the outermost bounds.
```

### Comparing `pyproj-3.5.0rc0/pyproj/utils.py` & `pyproj-3.6.0rc0/pyproj/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Utility functions used within pyproj
 """
 import json
 from array import array
 from enum import Enum, auto
-from typing import Any, Tuple
+from typing import Any
 
 
 def is_null(value: Any) -> bool:
     """
     Check if value is NaN or None
     """
     # pylint: disable=comparison-with-itself
@@ -59,37 +59,37 @@
 
     FLOAT = auto()
     LIST = auto()
     TUPLE = auto()
     ARRAY = auto()
 
 
-def _copytobuffer_return_scalar(xxx: Any) -> Tuple[array, DataType]:
+def _copytobuffer_return_scalar(xxx: Any) -> tuple[array, DataType]:
     """
     Prepares scalar for PROJ C-API:
     - Makes a copy because PROJ modifies buffer in place
     - Make sure dtype is double as that is what PROJ expects
     - Makes sure object supports Python Buffer API
 
     Parameters
     -----------
     xxx: float or 0-d numpy array
 
     Returns
     -------
-    Tuple[Any, DataType]
+    tuple[Any, DataType]
         The copy of the data prepared for the PROJ API & Python Buffer API.
     """
     try:
         return array("d", (float(xxx),)), DataType.FLOAT
     except Exception:
         raise TypeError("input must be a scalar") from None
 
 
-def _copytobuffer(xxx: Any, inplace: bool = False) -> Tuple[Any, DataType]:
+def _copytobuffer(xxx: Any, inplace: bool = False) -> tuple[Any, DataType]:
     """
     Prepares data for PROJ C-API:
     - Makes a copy because PROJ modifies buffer in place
     - Make sure dtype is double as that is what PROJ expects
     - Makes sure object supports Python Buffer API
 
     If the data is a numpy array, it ensures the data is in C order.
@@ -101,15 +101,15 @@
         pandas.Series, xaray.DataArray, or dask.array.Array.
     inplace: bool, default=False
         If True, will return the array without a copy if it
         meets the requirements of the Python Buffer API & PROJ C-API.
 
     Returns
     -------
-    Tuple[Any, DataType]
+    tuple[Any, DataType]
         The copy of the data prepared for the PROJ API & Python Buffer API.
     """
     # check for pandas.Series, xarray.DataArray or dask.array.Array
     # also handle numpy masked Arrays; note that pandas.Series also has a
     # "mask" attribute, hence checking for simply the "mask" attr in that
     # case isn't sufficient
     if (
```

### Comparing `pyproj-3.5.0rc0/pyproj.egg-info/PKG-INFO` & `pyproj-3.6.0rc0/pyproj.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,51 +1,48 @@
 Metadata-Version: 2.1
 Name: pyproj
-Version: 3.5.0rc0
+Version: 3.6.0rc0
 Summary: Python interface to PROJ (cartographic projections and coordinate transformations library)
 Home-page: https://github.com/pyproj4/pyproj
-Download-URL: http://python.org/pypi/pyproj
-Author: Jeff Whitaker
-Author-email: jeffrey.s.whitaker@noaa.gov
+Author-email: Jeff Whitaker <jeffrey.s.whitaker@noaa.gov>
+Maintainer: pyproj contributors
 License: MIT
-Project-URL: Documentation, https://pyproj4.github.io/pyproj/
-Project-URL: Release Notes, https://pyproj4.github.io/pyproj/stable/history.html
-Project-URL: Bug Tracker, https://github.com/pyproj4/pyproj/issues
-Project-URL: Source Code, https://github.com/pyproj4/pyproj
+Project-URL: homepage, https://pyproj4.github.io/pyproj/
+Project-URL: documentation, https://pyproj4.github.io/pyproj/
+Project-URL: repository, https://github.com/pyproj4/pyproj
+Project-URL: changelog, https://pyproj4.github.io/pyproj/stable/history.html
 Keywords: GIS,map,geospatial,coordinate-systems,coordinate-transformation,cartographic-projection,geodesic
-Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE_proj
 
 ![Pyproj logo](docs/media/logo.png)
 
 # pyproj
 
 Python interface to [PROJ](http://proj.org) (cartographic projections and coordinate transformations library).
 
 <p align="center">
 <a href="https://gitter.im/pyproj4-pyproj/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge"><img alt="Join the chat at https://gitter.im/pyproj4-pyproj/community" src="https://badges.gitter.im/pyproj4-pyproj/community.svg"></a>
-<a href="#contributors"><img alt="All Contributors" src="https://img.shields.io/badge/all_contributors-57-orange.svg?style=flat-square"></a>
+<a href="#contributors"><img alt="All Contributors" src="https://img.shields.io/badge/all_contributors-60-orange.svg?style=flat-square"></a>
 <a href="https://ci.appveyor.com/project/snowman2/pyproj"><img alt="Appveyor Build Status" src="https://ci.appveyor.com/api/projects/status/v2ypts9j76doa9ey/branch/main?svg=true"></a>
 <a href="https://github.com/pyproj4/pyproj/actions?query=workflow%3ATests"><img alt="GitHub Actions Build Status" src="https://github.com/pyproj4/pyproj/workflows/Tests/badge.svg"></a>
 <a href="https://codecov.io/gh/pyproj4/pyproj"><img alt="Codecov Status" src="https://codecov.io/gh/pyproj4/pyproj/branch/main/graph/badge.svg"></a>
 <a href="https://badge.fury.io/py/pyproj"><img alt="PyPI" src="https://badge.fury.io/py/pyproj.svg"></a>
 <a href="https://pepy.tech/project/pyproj"><img alt="Downloads" src="https://pepy.tech/badge/pyproj"></a>
 <a href="https://anaconda.org/conda-forge/pyproj"><img alt="Anaconda-Server Badge" src="https://anaconda.org/conda-forge/pyproj/badges/version.svg"></a>
 <a href="https://github.com/python/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
@@ -144,14 +141,17 @@
     <td align="center"><a href="https://github.com/DWesl"><img src="https://avatars.githubusercontent.com/u/22566757?v=4?s=100" width="100px;" alt=""/><br /><sub><b>DWesl</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=DWesl" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/molinav"><img src="https://avatars.githubusercontent.com/u/9979942?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Víctor Molina García</b></sub></a><br /><a href="#platform-molinav" title="Packaging/porting to new platform">📦</a></td>
     <td align="center"><a href="https://github.com/skogler"><img src="https://avatars.githubusercontent.com/u/1032405?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Samuel Kogler</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/issues?q=author%3Askogler" title="Bug reports">🐛</a> <a href="https://github.com/pyproj4/pyproj/commits?author=skogler" title="Code">💻</a></td>
     <td align="center"><a href="https://github.com/shadchin"><img src="https://avatars.githubusercontent.com/u/61256?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Alexander Shadchin</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/issues?q=author%3Ashadchin" title="Bug reports">🐛</a> <a href="https://github.com/pyproj4/pyproj/commits?author=shadchin" title="Code">💻</a></td>
   </tr>
   <tr>
     <td align="center"><a href="https://github.com/greglucas"><img src="https://avatars.githubusercontent.com/u/12417828?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Greg Lucas</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=greglucas" title="Code">💻</a> <a href="#ideas-greglucas" title="Ideas, Planning, & Feedback">🤔</a></td>
+    <td align="center"><a href="https://github.com/dmahr1"><img src="https://avatars.githubusercontent.com/u/8354515?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Dan Mahr</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=dmahr1" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://github.com/rhugonnet"><img src="https://avatars.githubusercontent.com/u/28896516?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Romain Hugonnet</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=rhugonnet" title="Tests">⚠️</a></td>
+    <td align="center"><a href="https://javier.jimenezshaw.com/"><img src="https://avatars.githubusercontent.com/u/15678366?v=4?s=100" width="100px;" alt=""/><br /><sub><b>Javier Jimenez Shaw</b></sub></a><br /><a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Code">💻</a> <a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Documentation">📖</a> <a href="https://github.com/pyproj4/pyproj/commits?author=jjimenezshaw" title="Tests">⚠️</a></td>
   </tr>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: pyproj Version: 3.5.0rc0 Summary: Python interface
+Metadata-Version: 2.1 Name: pyproj Version: 3.6.0rc0 Summary: Python interface
 to PROJ (cartographic projections and coordinate transformations library) Home-
-page: https://github.com/pyproj4/pyproj Download-URL: http://python.org/pypi/
-pyproj Author: Jeff Whitaker Author-email: jeffrey.s.whitaker@noaa.gov License:
-MIT Project-URL: Documentation, https://pyproj4.github.io/pyproj/ Project-URL:
-Release Notes, https://pyproj4.github.io/pyproj/stable/history.html Project-
-URL: Bug Tracker, https://github.com/pyproj4/pyproj/issues Project-URL: Source
-Code, https://github.com/pyproj4/pyproj Keywords:
-GIS,map,geospatial,coordinate-systems,coordinate-transformation,cartographic-
-projection,geodesic Platform: any Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering Classifier: Topic :: Scientific/
-Engineering :: GIS Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed Requires-Python: >=3.8 Description-Content-Type:
-text/markdown License-File: LICENSE License-File: LICENSE_proj ![Pyproj logo]
-(docs/media/logo.png) # pyproj Python interface to [PROJ](http://proj.org)
-(cartographic projections and coordinate transformations library).
+page: https://github.com/pyproj4/pyproj Author-email: Jeff Whitaker
+s.whitaker@noaa.gov> Maintainer: pyproj contributors License: MIT Project-URL:
+homepage, https://pyproj4.github.io/pyproj/ Project-URL: documentation, https:/
+/pyproj4.github.io/pyproj/ Project-URL: repository, https://github.com/pyproj4/
+pyproj Project-URL: changelog, https://pyproj4.github.io/pyproj/stable/
+history.html Keywords: GIS,map,geospatial,coordinate-systems,coordinate-
+transformation,cartographic-projection,geodesic Classifier: Development Status
+:: 4 - Beta Classifier: Intended Audience :: Science/Research Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
+Language :: Python :: 3 :: Only Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: GIS Classifier: Topic ::
+Scientific/Engineering :: Mathematics Classifier: Topic :: Software Development
+:: Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python:
+>=3.9 Description-Content-Type: text/markdown License-File: LICENSE License-
+File: LICENSE_proj ![Pyproj logo](docs/media/logo.png) # pyproj Python
+interface to [PROJ](http://proj.org) (cartographic projections and coordinate
+transformations library).
       [Join_the_chat_at_https://gitter.im/pyproj4-pyproj/community] [All
  Contributors] [Appveyor_Build_Status] [GitHub_Actions_Build_Status] [Codecov
  Status] [PyPI] [Downloads] [Anaconda-Server_Badge] [Code_style:_black] [pre-
                                  commit] [DOI]
 ## Documentation - Stable: http://pyproj4.github.io/pyproj/stable/ - Latest:
 https://pyproj4.github.io/pyproj/latest/ ## Bugs/Questions - Report bugs/
 feature requests: https://github.com/pyproj4/pyproj/issues - Ask questions:
@@ -62,13 +61,13 @@
 
                                                                 ð                                                                                      ð                                                                        ð»                                                        ð ð»                       ð ð» â ï¸                 ð» ð              ð» ð â ï¸
 
                                                        Kyle_Penner                                                                             paulcochrane                                                                              Antonio_Ettorre                                                           DWesl                             VÃ­ctor_Molina_GarcÃ­a                    Samuel_Kogler                     Alexander_Shadchin
 
                                                      ð» ð ð                                                            ð» ð â ï¸ ð                                                            ð¦                                                              ð»                                  ð¦                               ð ð»                    ð ð»
 
-                                                          Greg_Lucas
+                                                          Greg_Lucas                                                                                Dan_Mahr                                                                      Romain_Hugonnet                                                   Javier_Jimenez_Shaw
 
-                                                           ð» ð¤
+                                                           ð» ð¤                                                                    ð» ð â ï¸                                                   ð» ð â ï¸                                       ð» ð â ï¸
    This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `pyproj-3.5.0rc0/pyproj.egg-info/SOURCES.txt` & `pyproj-3.6.0rc0/pyproj.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 LICENSE_proj
 MANIFEST.in
 Makefile
 README.md
 pyproject.toml
 pytest.ini
-setup.cfg
 setup.py
 docs/Makefile
 docs/advanced_examples.rst
 docs/build_crs.rst
 docs/build_crs_cf.rst
 docs/cli.rst
 docs/conf.py
```

### Comparing `pyproj-3.5.0rc0/setup.py` & `pyproj-3.6.0rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import platform
 import re
 import shutil
 import subprocess
 import sys
 from pathlib import Path
-from typing import Dict, List, Optional
+from typing import Optional
 
 from pkg_resources import parse_version
 from setuptools import Extension, setup
 
 PROJ_MIN_VERSION = parse_version("9.0.0")
 CURRENT_FILE_PATH = Path(__file__).absolute().parent
 BASE_INTERNAL_PROJ_DIR = Path("proj_dir")
@@ -69,15 +69,15 @@
     elif proj_dir is not None and proj_dir.exists():
         print("PROJ_DIR is set, using existing PROJ installation..\n")
     else:
         raise SystemExit(f"ERROR: Invalid path for PROJ_DIR {proj_dir}")
     return proj_dir
 
 
-def get_proj_libdirs(proj_dir: Path) -> List[str]:
+def get_proj_libdirs(proj_dir: Path) -> list[str]:
     """
     This function finds the library directories
     """
     proj_libdir = os.environ.get("PROJ_LIBDIR")
     libdirs = []
     if proj_libdir is None:
         libdir_search_paths = (proj_dir / "lib", proj_dir / "lib64")
@@ -89,15 +89,15 @@
                 "ERROR: PROJ_LIBDIR dir not found. Please set PROJ_LIBDIR."
             )
     else:
         libdirs.append(proj_libdir)
     return libdirs
 
 
-def get_proj_incdirs(proj_dir: Path) -> List[str]:
+def get_proj_incdirs(proj_dir: Path) -> list[str]:
     """
     This function finds the include directories
     """
     proj_incdir = os.environ.get("PROJ_INCDIR")
     incdirs = []
     if proj_incdir is None:
         if (proj_dir / "include").exists():
@@ -126,15 +126,15 @@
     }
     if os.environ.get("PYPROJ_FULL_COVERAGE"):
         cythonize_options["compiler_directives"].update(linetrace=True)
         cythonize_options["annotate"] = True
     return cythonize_options
 
 
-def get_libraries(libdirs: List[str]) -> List[str]:
+def get_libraries(libdirs: list[str]) -> list[str]:
     """
     This function gets the libraries to cythonize with
     """
     libraries = ["proj"]
     if os.name == "nt":
         for libdir in libdirs:
             projlib = list(Path(libdir).glob("proj*.lib"))
@@ -202,15 +202,15 @@
             "CTE_PROJ_VERSION_PATCH": int(proj_version_patch),
             "CTE_PYTHON_IMPLEMENTATION": platform.python_implementation(),
         },
         **get_cythonize_options(),
     )
 
 
-def get_package_data() -> Dict[str, List[str]]:
+def get_package_data() -> dict[str, list[str]]:
     """
     This function retrieves the package data
     """
     # setup package data
     package_data = {"pyproj": ["*.pyi", "py.typed"]}
     if os.environ.get("PROJ_WHEEL") is not None and INTERNAL_PROJ_DIR.exists():
         package_data["pyproj"].append(
@@ -220,12 +220,14 @@
         os.environ.get("PROJ_WHEEL") is not None
         and (CURRENT_FILE_PATH / "pyproj" / ".lib").exists()
     ):
         package_data["pyproj"].append(os.path.join(".lib", "*"))
     return package_data
 
 
-# static items in setup.cfg
+# static items in pyproject.toml
 setup(
     ext_modules=get_extension_modules(),
     package_data=get_package_data(),
+    # temptorary hack to add in metadata
+    url="https://github.com/pyproj4/pyproj",
 )
```

### Comparing `pyproj-3.5.0rc0/test/conftest.py` & `pyproj-3.6.0rc0/test/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,18 +8,20 @@
 from packaging import version
 
 import pyproj
 from pyproj.datadir import get_data_dir, get_user_data_dir, set_data_dir
 
 _NETWORK_ENABLED = pyproj.network.is_network_enabled()
 PROJ_LOOSE_VERSION = version.parse(pyproj.__proj_version__)
+PROJ_911 = PROJ_LOOSE_VERSION == version.parse("9.1.1")
 PROJ_GTE_901 = PROJ_LOOSE_VERSION >= version.parse("9.0.1")
 PROJ_GTE_91 = PROJ_LOOSE_VERSION >= version.parse("9.1")
 PROJ_GTE_911 = PROJ_LOOSE_VERSION >= version.parse("9.1.1")
 PROJ_GTE_92 = PROJ_LOOSE_VERSION >= version.parse("9.2.0")
+PROJ_GTE_921 = PROJ_LOOSE_VERSION >= version.parse("9.2.1")
 
 
 def unset_data_dir():
     pyproj.datadir._USER_PROJ_DATA = None
     pyproj.datadir._VALIDATED_PROJ_DATA = None
```

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs.py` & `pyproj-3.6.0rc0/test/crs/test_crs.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 from pyproj.enums import ProjVersion, WktVersion
 from pyproj.exceptions import CRSError
 from pyproj.transformer import TransformerGroup
 from test.conftest import (
     PROJ_GTE_91,
     PROJ_GTE_901,
     PROJ_GTE_911,
+    PROJ_GTE_921,
     assert_can_pickle,
     grids_available,
 )
 
 
-class CustomCRS(object):
+class CustomCRS:
     def to_wkt(self):
         return CRS.from_epsg(4326).to_wkt()
 
 
 def test_from_proj4_json():
     json_str = '{"proj": "longlat", "ellps": "WGS84", "datum": "WGS84"}'
     proj = CRS.from_string(json_str)
@@ -227,14 +228,48 @@
 
 def test_to_wkt_pretty():
     crs = CRS.from_epsg(4326)
     assert "\n" in crs.to_wkt(pretty=True)
     assert "\n" not in crs.to_wkt()
 
 
+@pytest.mark.parametrize(
+    "version, expected",
+    [
+        ("WKT1_GDAL", False),
+        ("WKT1_ESRI", False),
+        ("WKT2_2019", True),
+    ],
+)
+def test_to_wkt_with_axis_rule_4326(version, expected):
+    crs = CRS.from_epsg(4326)
+    axis = "AXIS"
+    assert (axis in crs.to_wkt(version)) == expected
+    assert (axis in crs.to_wkt(version, output_axis_rule=None)) == expected
+    assert axis in crs.to_wkt(version, output_axis_rule=True)
+    assert axis not in crs.to_wkt(version, output_axis_rule=False)
+
+
+@pytest.mark.parametrize(
+    "version, expected",
+    [
+        ("WKT1_GDAL", True),
+        ("WKT1_ESRI", False),
+        ("WKT2_2019", True),
+    ],
+)
+def test_to_wkt_with_axis_rule_32630(version, expected):
+    crs = CRS.from_epsg(32630)
+    axis = "AXIS"
+    assert (axis in crs.to_wkt(version)) == expected
+    assert (axis in crs.to_wkt(version, output_axis_rule=None)) == expected
+    assert axis in crs.to_wkt(version, output_axis_rule=True)
+    assert axis not in crs.to_wkt(version, output_axis_rule=False)
+
+
 def test_repr():
     with pytest.warns(FutureWarning):
         assert repr(CRS({"init": "EPSG:4326"})) == (
             "<Geographic 2D CRS: +init=epsg:4326 +type=crs>\n"
             "Name: WGS 84\n"
             "Axis Info [ellipsoidal]:\n"
             "- lon[east]: Longitude (degree)\n"
@@ -369,14 +404,16 @@
     crs = CRS(
         "+proj=omerc +lat_0=-36.10360962430914 "
         "+lonc=147.06322917270154 +alpha=-54.786229796129035 "
         "+k=1 +x_0=0 +y_0=0 +gamma=0 +ellps=WGS84 "
         "+towgs84=0,0,0,0,0,0,0 +units=m +no_defs"
     )
     datum_name = "Unknown based on WGS84 ellipsoid"
+    if PROJ_GTE_921:
+        datum_name = "Unknown based on WGS 84 ellipsoid"
     if PROJ_GTE_901:
         datum_name = f"{datum_name} using towgs84=0,0,0,0,0,0,0"
     assert crs.datum.name == datum_name
 
 
 def test_epsg__not_found():
     assert CRS("+proj=longlat +datum=WGS84 +no_defs +towgs84=0,0,0").to_epsg(0) is None
@@ -1604,14 +1641,44 @@
 
 
 def test_to_3d__name():
     crs_3d = CRS("EPSG:2056").to_3d(name="TEST")
     assert crs_3d.name == "TEST"
 
 
+@pytest.mark.parametrize(
+    "crs_input",
+    [
+        CRS("EPSG:4979"),  # native 3D
+        CRS("EPSG:2056").to_3d(),  # a 2D CRS converted to 3D
+        CRS("EPSG:4326+5773"),  # a 3D CRS based on a compound
+    ],
+)
+def test_to_2d(crs_input):
+    assert len(crs_input.axis_info) == 3
+    horizon_axis_crs_3d = crs_input.axis_info[:-1]
+    crs_2d = crs_input.to_2d()
+    horizon_axis_crs_2d = crs_input.axis_info
+    assert len(crs_2d.axis_info) == 2
+    assert horizon_axis_crs_2d[0] == horizon_axis_crs_3d[0]
+    assert horizon_axis_crs_2d[1] == horizon_axis_crs_3d[1]
+    assert crs_2d.to_2d() == crs_2d
+    # For CompoundCRS, the 3D name is initialized different from 2D
+    if crs_input.name == "WGS 84 + EGM96 height":
+        assert crs_2d.name == "WGS 84"
+    # Otherwise, no change
+    else:
+        assert crs_2d.name == crs_input.name
+
+
+def test_to_2d__name():
+    crs_2d = CRS("EPSG:2056").to_3d().to_2d(name="TEST")
+    assert crs_2d.name == "TEST"
+
+
 def test_crs__pickle(tmp_path):
     assert_can_pickle(CRS("epsg:4326"), tmp_path)
 
 
 def test_is_derived():
     assert CRS(
         "+proj=ob_tran +o_proj=longlat +o_lat_p=0 +o_lon_p=0 +lon_0=0"
```

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs_cf.py` & `pyproj-3.6.0rc0/test/crs/test_crs_cf.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs_coordinate_operation.py` & `pyproj-3.6.0rc0/test/crs/test_crs_coordinate_operation.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs_coordinate_system.py` & `pyproj-3.6.0rc0/test/crs/test_crs_coordinate_system.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs_datum.py` & `pyproj-3.6.0rc0/test/crs/test_crs_datum.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs_json.py` & `pyproj-3.6.0rc0/test/crs/test_crs_json.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/crs/test_crs_maker.py` & `pyproj-3.6.0rc0/test/crs/test_crs_maker.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/sample.out` & `pyproj-3.6.0rc0/test/sample.out`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_aoi.py` & `pyproj-3.6.0rc0/test/test_aoi.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_awips221.py` & `pyproj-3.6.0rc0/test/test_awips221.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,37 +65,37 @@
     y = llcrnry + dy * numpy.indices((ny, nx), "f")[0, :, :]
     t1 = perf_counter()
     lons, lats = awips221(
         numpy.ravel(x).tolist(), numpy.ravel(y).tolist(), inverse=True
     )
     t2 = perf_counter()
     print("data in lists:")
-    print("compute lats/lons for all points on AWIPS 221 grid (%sx%s)" % (nx, ny))
+    print("compute lats/lons for all points on AWIPS 221 grid ({}x{})".format(nx, ny))
     print("max/min lons")
     print(min(lons), max(lons))
     print("max/min lats")
     print(min(lats), max(lats))
     print("took", t2 - t1, "secs")
     xa = array.array("f", numpy.ravel(x).tolist())
     ya = array.array("f", numpy.ravel(y).tolist())
     t1 = perf_counter()
     lons, lats = awips221(xa, ya, inverse=True)
     t2 = perf_counter()
     print("data in python arrays:")
-    print("compute lats/lons for all points on AWIPS 221 grid (%sx%s)" % (nx, ny))
+    print("compute lats/lons for all points on AWIPS 221 grid ({}x{})".format(nx, ny))
     print("max/min lons")
     print(min(lons), max(lons))
     print("max/min lats")
     print(min(lats), max(lats))
     print("took", t2 - t1, "secs")
     t1 = perf_counter()
     lons, lats = awips221(x, y, inverse=True)
     t2 = perf_counter()
     print("data in a numpy array:")
-    print("compute lats/lons for all points on AWIPS 221 grid (%sx%s)" % (nx, ny))
+    print("compute lats/lons for all points on AWIPS 221 grid ({}x{})".format(nx, ny))
     print("max/min lons")
     print(
         numpy.minimum.reduce(numpy.ravel(lons)), numpy.maximum.reduce(numpy.ravel(lons))
     )
     print("max/min lats")
     print(
         numpy.minimum.reduce(numpy.ravel(lats)), numpy.maximum.reduce(numpy.ravel(lats))
```

### Comparing `pyproj-3.5.0rc0/test/test_cli.py` & `pyproj-3.6.0rc0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_database.py` & `pyproj-3.6.0rc0/test/test_database.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_datadir.py` & `pyproj-3.6.0rc0/test/test_datadir.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_datum.py` & `pyproj-3.6.0rc0/test/test_datum.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_datum_shift.py` & `pyproj-3.6.0rc0/test/test_datum_shift.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_doctest_wrapper.py` & `pyproj-3.6.0rc0/test/test_doctest_wrapper.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_geod.py` & `pyproj-3.6.0rc0/test/test_geod.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 import pickle
 from contextlib import nullcontext
 from itertools import permutations
 
 import numpy
 import pytest
-from numpy.testing import assert_almost_equal
+from numpy.testing import assert_almost_equal, assert_array_equal
 
 from pyproj import Geod
 from pyproj.geod import GeodIntermediateFlag, reverse_azimuth
 
 try:
     from shapely.geometry import (
         LinearRing,
@@ -440,14 +440,29 @@
         expected_lonlats.insert(0, (_BOSTON_LON, _BOSTON_LAT))
     if include_terminus:
         expected_lonlats.append((_PORTLAND_LON, _PORTLAND_LAT))
     assert_almost_equal(lonlats, expected_lonlats, decimal=3)
 
 
 @pytest.mark.parametrize(
+    "input_data",
+    [
+        [1.0, 2.0, 3.0, math.nan],
+        [1.0, 2.0, math.nan, 4.0],
+        [1.0, math.nan, 3.0, 4.0],
+        [math.nan, 2.0, 3.0, 4.0],
+        [math.nan, math.nan, math.nan, math.nan],
+    ],
+)
+def test_geodesic_npts__nan(input_data):
+    geod = Geod(ellps="WGS84")
+    assert_array_equal(geod.npts(*input_data, npts=1), [(math.nan, math.nan)])
+
+
+@pytest.mark.parametrize(
     "ellipsoid,expected_azi12,expected_az21,expected_dist",
     [("clrk66", -66.531, 75.654, 4164192.708), ("WGS84", -66.530, 75.654, 4164074.239)],
 )
 def test_geodesic_inv__pickle(
     ellipsoid, expected_azi12, expected_az21, expected_dist, tmp_path, scalar_and_array
 ):
     geod = Geod(ellps=ellipsoid)
```

### Comparing `pyproj-3.5.0rc0/test/test_list.py` & `pyproj-3.6.0rc0/test/test_list.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_network.py` & `pyproj-3.6.0rc0/test/test_network.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_pickle.py` & `pyproj-3.6.0rc0/test/test_pickle.py`

 * *Files 3% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         with open(os.path.join(tmpdir, "test.pickle"), "wb") as pfh:
             pickle.dump(awips221_pre_pickle, pfh, -1)
         with open(os.path.join(tmpdir, "test.pickle"), "rb") as prh:
             awips221 = pickle.load(prh)
     t1 = perf_counter()
     lons, lats = awips221(x, y, inverse=True)
     t2 = perf_counter()
-    print("compute lats/lons for all points on AWIPS 221 grid (%sx%s)" % (nx, ny))
+    print("compute lats/lons for all points on AWIPS 221 grid ({}x{})".format(nx, ny))
     print("max/min lons in radians")
     print(
         numpy.minimum.reduce(numpy.ravel(lons)), numpy.maximum.reduce(numpy.ravel(lons))
     )
     print("max/min lats in radians")
     print(
         numpy.minimum.reduce(numpy.ravel(lats)), numpy.maximum.reduce(numpy.ravel(lats))
```

### Comparing `pyproj-3.5.0rc0/test/test_proj.py` & `pyproj-3.6.0rc0/test/test_proj.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import concurrent.futures
 import math
 import os
 import sys
 import unittest
 from unittest.mock import patch
```

### Comparing `pyproj-3.5.0rc0/test/test_show_versions.py` & `pyproj-3.6.0rc0/test/test_show_versions.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_sync.py` & `pyproj-3.6.0rc0/test/test_sync.py`

 * *Files identical despite different names*

### Comparing `pyproj-3.5.0rc0/test/test_transform.py` & `pyproj-3.6.0rc0/test/test_transform.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy
 import pytest
 from numpy.testing import assert_allclose, assert_almost_equal
 
 from pyproj import Proj, __proj_version__, transform
-from test.conftest import PROJ_GTE_92, grids_available
+from test.conftest import PROJ_911, PROJ_GTE_92, PROJ_GTE_911, grids_available
 
 
 def test_transform():
     # convert awips221 grid to awips218 coordinate system
     # (grids defined at http://www.nco.ncep.noaa.gov/pmb/docs/on388/tableb.html)
     nx = 614
     ny = 428
@@ -48,14 +48,15 @@
     print("(should be close to zero)")
     assert_allclose(numpy.minimum.reduce(numpy.ravel(x3 - x1)), 0, atol=1e-4)
     assert_allclose(numpy.maximum.reduce(numpy.ravel(x3 - x1)), 0, atol=1e-4)
     assert_allclose(numpy.minimum.reduce(numpy.ravel(y3 - y1)), 0, atol=1e-4)
     assert_allclose(numpy.maximum.reduce(numpy.ravel(y3 - y1)), 0, atol=1e-4)
 
 
+@pytest.mark.xfail(PROJ_911, reason="Patch applied in conda-forge changes behavior")
 def test_transform_single_point_nad83_to_nad27():
     # projection 1: UTM zone 15, grs80 ellipse, NAD83 datum
     # (defined by epsg code 26915)
     p1 = Proj("epsg:26915", preserve_units=False)
     # projection 2: UTM zone 15, clrk66 ellipse, NAD27 datum
     p2 = Proj("epsg:26715", preserve_units=False)
     # find x,y of Jefferson City, MO.
@@ -63,38 +64,44 @@
     # transform this point to projection 2 coordinates.
     x2, y2 = transform(p1, p2, x1, y1)
     assert_almost_equal(
         (x1, y1),
         (569704.566, 4269024.671),
         decimal=3,
     )
-    expected_xy2 = (569722.342, 4268814.028)
-    if PROJ_GTE_92:
-        expected_xy2 = (569720.46, 4268813.88)
-        if grids_available(
-            "ca_nrc_ntv2_0.tif", "us_noaa_nadcon5_nad27_nad83_1986_conus.tif"
+    expected_xy2 = (569722, 4268814)
+    if PROJ_GTE_911:
+        expected_xy2 = (569720, 4268813)
+        if (
+            PROJ_GTE_92
+            and grids_available(
+                "us_noaa_nadcon5_nad27_nad83_1986_conus.tif", check_network=False
+            )
+        ) or grids_available():
+            expected_xy2 = (569722, 4268814)
+        elif grids_available(
+            "ca_nrc_ntv2_0.tif", "ca_nrc_ntv1_can.tif", check_network=False
         ):
-            expected_xy2 = (569722.394, 4268814.27)
-        elif grids_available("ca_nrc_ntv2_0.tif", "ca_nrc_ntv1_can.tif"):
-            expected_xy2 = (569706.333, 4268817.68)
-        elif grids_available("us_noaa_conus.tif"):
-            expected_xy2 = (569722.342, 4268814.028)
+            expected_xy2 = (569706, 4268817)
+        elif grids_available("us_noaa_conus.tif", check_network=False):
+            expected_xy2 = (569722, 4268814)
 
     assert_almost_equal(
         (x2, y2),
         expected_xy2,
-        decimal=3,
+        decimal=0,
     )
     assert_almost_equal(
-        p2(x2, y2, inverse=True),
+        p2(x2, y2, inverse=True, errcheck=True),
         (-92.200, 38.567),
         decimal=3,
     )
 
 
+@pytest.mark.xfail(PROJ_911, reason="Patch applied in conda-forge changes behavior")
 def test_transform_tuple_nad83_to_nad27():
     # projection 1: UTM zone 15, grs80 ellipse, NAD83 datum
     # (defined by epsg code 26915)
     p1 = Proj("epsg:26915", preserve_units=False)
     # projection 2: UTM zone 15, clrk66 ellipse, NAD27 datum
     p2 = Proj("epsg:26715", preserve_units=False)
     # process 3 points at a time in a tuple
@@ -108,40 +115,47 @@
         decimal=3,
     )
     assert_almost_equal(
         y1,
         (4298200.739, 4353698.725, 4292319.005),
         decimal=3,
     )
-    expected_x2 = (567721.149, 351747.558, 728569.133)
-    expected_y2 = (4297989.112, 4353489.645, 4292106.305)
-    if PROJ_GTE_92:
-        expected_x2 = (567719.249, 351748.119, 728568.053)
-        expected_y2 = (4297989.776, 4353487.434, 4292108.075)
-        if grids_available("us_noaa_nadcon5_nad27_nad83_1986_conus.tif"):
-            expected_x2 = (567721.401, 351747.526, 728569.212)
-            expected_y2 = (4297989.733, 4353489.752, 4292106.351)
-        elif grids_available("ca_nrc_ntv2_0.tif", "ca_nrc_ntv1_can.tif"):
-            expected_x2 = (567705.072, 351727.113, 728558.917)
-            expected_y2 = (4297993.157, 4353490.111, 4292111.678)
-        elif grids_available("us_noaa_conus.tif"):
-            expected_x2 = (567721.149, 351747.558, 728569.133)
-            expected_y2 = (4297989.112, 4353489.645, 4292106.305)
+    expected_x2 = (567721, 351747, 728569)
+    expected_y2 = (4297989, 4353489, 4292106)
+    if PROJ_GTE_911:
+        expected_x2 = (567719, 351748, 728568)
+        expected_y2 = (4297989, 4353487, 4292108)
+        if (
+            PROJ_GTE_92
+            and grids_available(
+                "us_noaa_nadcon5_nad27_nad83_1986_conus.tif", check_network=False
+            )
+        ) or grids_available():
+            expected_x2 = (567721, 351747, 728569)
+            expected_y2 = (4297989, 4353489, 4292106)
+        elif grids_available(
+            "ca_nrc_ntv2_0.tif", "ca_nrc_ntv1_can.tif", check_network=False
+        ):
+            expected_x2 = (567705, 351727, 728558)
+            expected_y2 = (4297993, 4353490, 4292111)
+        elif grids_available("us_noaa_conus.tif", check_network=False):
+            expected_x2 = (567721, 351747, 728569.133)
+            expected_y2 = (4297989, 4353489, 4292106)
 
     assert_almost_equal(
         x2,
         expected_x2,
-        decimal=3,
+        decimal=0,
     )
     assert_almost_equal(
         y2,
         expected_y2,
-        decimal=3,
+        decimal=0,
     )
-    lons2, lats2 = p2(x2, y2, inverse=True)
+    lons2, lats2 = p2(x2, y2, inverse=True, errcheck=True)
     assert_almost_equal(
         lons2,
         (-92.220, -94.720, -90.370),
         decimal=3,
     )
     assert_almost_equal(
         lats2,
```

### Comparing `pyproj-3.5.0rc0/test/test_transformer.py` & `pyproj-3.6.0rc0/test/test_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -517,53 +517,22 @@
     )
 
 
 def test_str():
     assert str(Transformer.from_crs(4326, 3857)).startswith("proj=pipeline")
 
 
-@pytest.mark.parametrize(
-    "from_crs, to_crs, expected_repr",
-    [
-        (
-            7789,
-            8401,
-            (
-                "<Transformation Transformer: helmert>\n"
-                "Description: ITRF2014 to ETRF2014 (2)\n"
-                "Area of Use:\n"
-                "- name: Europe - onshore and offshore: Albania; Andorra; Austria; "
-                "Belgium; Bosnia and Herzegovina; Bulgaria; Croatia; Cyprus; Czechia; "
-                "Denmark; Estonia; Faroe Islands; Finland; France; Germany; Gibraltar; "
-                "Greece; Hungary; Ireland; Italy; Kosovo; Latvia; Liechtenstein; "
-                "Lithuania; Luxembourg; Malta; Moldova; Monaco; Montenegro; "
-                "Netherlands; North Macedonia; "
-                "Norway including Svalbard and Jan Mayen; "
-                "Poland; Portugal; Romania; San Marino; Serbia; Slovakia; Slovenia; "
-                "Spain; Sweden; Switzerland; "
-                "United Kingdom (UK) including Channel Islands and Isle of Man; "
-                "Vatican City State.\n"
-                "- bounds: (-16.1, 32.88, 40.18, 84.73)"
-            ),
-        ),
-        (
-            4326,
-            3857,
-            (
-                "<Conversion Transformer: pipeline>\n"
-                "Description: Popular Visualisation Pseudo-Mercator\n"
-                "Area of Use:\n"
-                "- name: World.\n"
-                "- bounds: (-180.0, -90.0, 180.0, 90.0)"
-            ),
-        ),
-    ],
-)
-def test_repr(from_crs, to_crs, expected_repr):
-    assert repr(Transformer.from_crs(from_crs, to_crs)) == expected_repr
+def test_repr():
+    assert repr(Transformer.from_crs(4326, 3857)) == (
+        "<Conversion Transformer: pipeline>\n"
+        "Description: Popular Visualisation Pseudo-Mercator\n"
+        "Area of Use:\n"
+        "- name: World.\n"
+        "- bounds: (-180.0, -90.0, 180.0, 90.0)"
+    )
 
 
 @pytest.mark.grid
 def test_repr__conditional():
     trans_repr = repr(Transformer.from_crs("EPSG:4326+3855", "EPSG:4979"))
     if grids_available("us_nga_egm08_25.tif"):
         assert trans_repr == (
@@ -1647,14 +1616,20 @@
     group = TransformerGroup(
         "EPSG:4326", "EPSG:4258", authority="PROJ", allow_ballpark=False
     )
     assert not group.transformers
     assert not group.unavailable_operations
 
 
+def test_transformer_group_allow_superseded_filter():
+    default_group = TransformerGroup(4203, 4326)
+    superseded_group = TransformerGroup(4203, 4326, allow_superseded=True)
+    assert len(superseded_group.transformers) > len(default_group.transformers)
+
+
 def test_transformer_group_authority_filter():
     group = TransformerGroup("EPSG:4326", "EPSG:4258", authority="PROJ")
     assert len(group.transformers) == 1
     assert not group.unavailable_operations
     assert (
         group.transformers[0].description
         == "Ballpark geographic offset from WGS 84 to ETRS89"
```

### Comparing `pyproj-3.5.0rc0/test/test_utils.py` & `pyproj-3.6.0rc0/test/test_utils.py`

 * *Files identical despite different names*

