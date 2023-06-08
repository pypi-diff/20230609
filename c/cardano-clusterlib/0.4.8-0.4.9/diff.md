# Comparing `tmp/cardano-clusterlib-0.4.8.tar.gz` & `tmp/cardano-clusterlib-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.8.tar", last modified: Mon May  8 12:51:50 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.4.9.tar", last modified: Fri May 12 06:59:22 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.8.tar` & `cardano-clusterlib-0.4.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.174079 cardano-clusterlib-0.4.8/.github/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.176079 cardano-clusterlib-0.4.8/.github/workflows/
--rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.8/.github/workflows/repo_lint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.8/.gitignore
--rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.8/.markdownlint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-05-06 20:29:59.000000 cardano-clusterlib-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.8/.pylintrc
--rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.8/.readthedocs.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.8/CODE-OF-CONDUCT.md
--rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.8/LICENSE
--rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.8/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.8/README.md
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/cardano_clusterlib/
--rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/__init__.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/address_group.py
--rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)    15500 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/consts.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/coverage.py
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/exceptions.py
--rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/governance_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/key_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/node_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/py.typed
--rw-r--r--   0 martink   (1000) martink   (1000)    18252 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6849 2023-04-17 13:43:55.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/structs.py
--rw-r--r--   0 martink   (1000) martink   (1000)    63362 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/txtools.py
--rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/types.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/docs/
--rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.8/docs/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.8/docs/requirements.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/docs/source/
--rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.8/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.8/docs/source/conf.py
--rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.8/docs/source/index.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.8/docs/source/modules.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.8/docs/source/readme.rst
--rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.8/mypy.ini
--rw-r--r--   0 martink   (1000) martink   (1000)      610 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.8/pyproject.toml
--rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.8/requirements-dev.txt
--rw-r--r--   0 martink   (1000) martink   (1000)      776 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/setup.cfg
--rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.8/setup.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/upgrading/
--rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.8/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.564756 cardano-clusterlib-0.4.9/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.557756 cardano-clusterlib-0.4.9/.github/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.559756 cardano-clusterlib-0.4.9/.github/workflows/
+-rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.9/.github/workflows/repo_lint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.9/.gitignore
+-rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.9/.markdownlint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-05-06 20:29:59.000000 cardano-clusterlib-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.9/.pylintrc
+-rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.9/.readthedocs.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.9/CODE-OF-CONDUCT.md
+-rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.9/LICENSE
+-rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.9/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-12 06:59:22.564756 cardano-clusterlib-0.4.9/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.9/README.md
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.561756 cardano-clusterlib-0.4.9/cardano_clusterlib/
+-rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/__init__.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/address_group.py
+-rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    15619 2023-05-12 06:58:23.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/consts.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/coverage.py
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/key_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/node_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/py.typed
+-rw-r--r--   0 martink   (1000) martink   (1000)    18252 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6849 2023-04-17 13:43:55.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/structs.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    63362 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/txtools.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.9/cardano_clusterlib/types.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.562756 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-05-12 06:59:22.000000 cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.562756 cardano-clusterlib-0.4.9/docs/
+-rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.9/docs/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.9/docs/requirements.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.563756 cardano-clusterlib-0.4.9/docs/source/
+-rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.9/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.9/docs/source/conf.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.9/docs/source/index.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.9/docs/source/modules.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.9/docs/source/readme.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.9/mypy.ini
+-rw-r--r--   0 martink   (1000) martink   (1000)      610 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.9/pyproject.toml
+-rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.9/requirements-dev.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)      776 2023-05-12 06:59:22.564756 cardano-clusterlib-0.4.9/setup.cfg
+-rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.9/setup.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-12 06:59:22.563756 cardano-clusterlib-0.4.9/upgrading/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.9/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.8/.gitignore` & `cardano-clusterlib-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/.markdownlint.yaml` & `cardano-clusterlib-0.4.9/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/.pre-commit-config.yaml` & `cardano-clusterlib-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/.pylintrc` & `cardano-clusterlib-0.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.4.9/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/LICENSE` & `cardano-clusterlib-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/Makefile` & `cardano-clusterlib-0.4.9/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/PKG-INFO` & `cardano-clusterlib-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cardano-clusterlib-0.4.8/README.md` & `cardano-clusterlib-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/clusterlib_klass.py`

 * *Files 1% similar despite different names*

```diff
@@ -182,19 +182,20 @@
     @property
     def g_governance(self) -> governance_group.GovernanceGroup:
         """Governance group."""
         if not self._governance_group:
             self._governance_group = governance_group.GovernanceGroup(clusterlib_obj=self)
         return self._governance_group
 
-    def cli(self, cli_args: List[str]) -> structs.CLIOut:
+    def cli(self, cli_args: List[str], timeout: Optional[float] = None) -> structs.CLIOut:
         """Run the `cardano-cli` command.
 
         Args:
             cli_args: A list of arguments for cardano-cli.
+            timeout: A timeout for the command, in seconds (optional).
 
         Returns:
             structs.CLIOut: A tuple containing command stdout and stderr.
         """
         cli_args_strs_all = [str(arg) for arg in cli_args]
         cli_args_strs_all.insert(0, "cardano-cli")
         cli_args_strs = [arg for arg in cli_args_strs_all if arg != consts.SUBCOMMAND_MARK]
@@ -210,15 +211,15 @@
         # or
         # MuxError (MuxIOException writev: resource vanished (Broken pipe)) "(sendAll errored)"
         for __ in range(3):
             retcode = None
             with subprocess.Popen(
                 cli_args_strs, stdout=subprocess.PIPE, stderr=subprocess.PIPE
             ) as p:
-                stdout, stderr = p.communicate()
+                stdout, stderr = p.communicate(timeout=timeout)
                 retcode = p.returncode
 
             if retcode == 0:
                 break
 
             stderr_dec = stderr.decode()
             err_msg = (
```

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/query_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/structs.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/transaction_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/txtools.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib/types.py` & `cardano-clusterlib-0.4.9/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.8
+Version: 0.4.9
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.4.9/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/docs/Makefile` & `cardano-clusterlib-0.4.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.4.9/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/docs/source/conf.py` & `cardano-clusterlib-0.4.9/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/pyproject.toml` & `cardano-clusterlib-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/setup.cfg` & `cardano-clusterlib-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.8/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.4.9/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

