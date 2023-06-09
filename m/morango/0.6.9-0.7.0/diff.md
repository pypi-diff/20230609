# Comparing `tmp/morango-0.6.9.tar.gz` & `tmp/morango-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/morango-0.6.9.tar", last modified: Thu Feb 24 21:25:11 2022, max compression
+gzip compressed data, was "dist/morango-0.7.0.tar", last modified: Fri Jun  9 14:33:59 2023, max compression
```

## Comparing `morango-0.6.9.tar` & `morango-0.7.0.tar`

### file list

```diff
@@ -1,101 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/
--rw-r--r--   0 runner    (1001) docker     (116)     4532 2022-02-24 21:25:03.000000 morango-0.6.9/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)     2616 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)     2355 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      134 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        8 2022-02-24 21:25:11.000000 morango-0.6.9/morango.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      268 2022-02-24 21:25:03.000000 morango-0.6.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1530 2022-02-24 21:25:03.000000 morango-0.6.9/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)     1374 2022-02-24 21:25:03.000000 morango-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      757 2022-02-24 21:25:11.000000 morango-0.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1074 2022-02-24 21:25:03.000000 morango-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     2355 2022-02-24 21:25:11.000000 morango-0.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      276 2022-02-24 21:25:03.000000 morango-0.6.9/AUTHORS.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/
--rw-r--r--   0 runner    (1001) docker     (116)     3735 2022-02-24 21:25:03.000000 morango-0.6.9/morango/proquint.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/management/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/management/commands/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3044 2022-02-24 21:25:03.000000 morango-0.6.9/morango/management/commands/cleanupsyncs.py
--rw-r--r--   0 runner    (1001) docker     (116)      546 2022-02-24 21:25:03.000000 morango-0.6.9/morango/apps.py
--rw-r--r--   0 runner    (1001) docker     (116)     3127 2022-02-24 21:25:03.000000 morango-0.6.9/morango/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)      141 2022-02-24 21:25:03.000000 morango-0.6.9/morango/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)     3676 2022-02-24 21:25:03.000000 morango-0.6.9/morango/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      190 2022-02-24 21:25:03.000000 morango-0.6.9/morango/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1423 2022-02-24 21:25:03.000000 morango-0.6.9/morango/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/api/
--rw-r--r--   0 runner    (1001) docker     (116)      273 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/fields.py
--rw-r--r--   0 runner    (1001) docker     (116)     1037 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (116)     3550 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/permissions.py
--rw-r--r--   0 runner    (1001) docker     (116)      557 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/parsers.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5293 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (116)    20330 2022-02-24 21:25:03.000000 morango-0.6.9/morango/api/viewsets.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/models/
--rw-r--r--   0 runner    (1001) docker     (116)      163 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/models/fields/
--rw-r--r--   0 runner    (1001) docker     (116)     4283 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/fields/uuids.py
--rw-r--r--   0 runner    (1001) docker     (116)      225 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13984 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/fields/crypto.py
--rw-r--r--   0 runner    (1001) docker     (116)    35929 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/core.py
--rw-r--r--   0 runner    (1001) docker     (116)     6644 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1983 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      478 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/signals.py
--rw-r--r--   0 runner    (1001) docker     (116)     1024 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/morango_mptt.py
--rw-r--r--   0 runner    (1001) docker     (116)    15279 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/certificates.py
--rw-r--r--   0 runner    (1001) docker     (116)      869 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/query.py
--rw-r--r--   0 runner    (1001) docker     (116)     7130 2022-02-24 21:25:03.000000 morango-0.6.9/morango/models/fsic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/constants/
--rw-r--r--   0 runner    (1001) docker     (116)     1871 2022-02-24 21:25:03.000000 morango-0.6.9/morango/constants/settings.py
--rw-r--r--   0 runner    (1001) docker     (116)      510 2022-02-24 21:25:03.000000 morango-0.6.9/morango/constants/transfer_statuses.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      453 2022-02-24 21:25:03.000000 morango-0.6.9/morango/constants/api_urls.py
--rw-r--r--   0 runner    (1001) docker     (116)     1379 2022-02-24 21:25:03.000000 morango-0.6.9/morango/constants/transfer_stages.py
--rw-r--r--   0 runner    (1001) docker     (116)      166 2022-02-24 21:25:03.000000 morango-0.6.9/morango/constants/capabilities.py
--rw-r--r--   0 runner    (1001) docker     (116)     1170 2022-02-24 21:25:03.000000 morango-0.6.9/morango/errors.py
--rw-r--r--   0 runner    (1001) docker     (116)    10897 2022-02-24 21:25:03.000000 morango-0.6.9/morango/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/sync/
--rw-r--r--   0 runner    (1001) docker     (116)     3293 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/session.py
--rw-r--r--   0 runner    (1001) docker     (116)    10992 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/context.py
--rw-r--r--   0 runner    (1001) docker     (116)    57757 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/operations.py
--rw-r--r--   0 runner    (1001) docker     (116)     8099 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/sync/backends/
--rw-r--r--   0 runner    (1001) docker     (116)    12360 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/backends/postgres.py
--rw-r--r--   0 runner    (1001) docker     (116)     9952 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/backends/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (116)     1774 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/backends/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     7804 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    25906 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/syncsession.py
--rw-r--r--   0 runner    (1001) docker     (116)    10633 2022-02-24 21:25:03.000000 morango-0.6.9/morango/sync/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/morango/migrations/
--rw-r--r--   0 runner    (1001) docker     (116)     1541 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0019_auto_20220113_1807.py
--rw-r--r--   0 runner    (1001) docker     (116)      841 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0010_auto_20171206_1615.py
--rw-r--r--   0 runner    (1001) docker     (116)      476 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0006_instanceidmodel_system_id.py
--rw-r--r--   0 runner    (1001) docker     (116)    11933 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (116)     8190 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0007_auto_20171018_1615.py
--rw-r--r--   0 runner    (1001) docker     (116)      505 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0013_auto_20190627_1513.py
--rw-r--r--   0 runner    (1001) docker     (116)      481 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0014_syncsession_extra_fields.py
--rw-r--r--   0 runner    (1001) docker     (116)      682 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0003_auto_20170519_0543.py
--rw-r--r--   0 runner    (1001) docker     (116)     2304 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0002_auto_20170511_0400.py
--rw-r--r--   0 runner    (1001) docker     (116)      987 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0012_auto_20180927_1658.py
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      461 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0016_store_deserialization_error.py
--rw-r--r--   0 runner    (1001) docker     (116)      558 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0004_auto_20170520_2112.py
--rw-r--r--   0 runner    (1001) docker     (116)      695 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0005_auto_20170629_2139.py
--rw-r--r--   0 runner    (1001) docker     (116)      561 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0017_store_last_transfer_session_id.py
--rw-r--r--   0 runner    (1001) docker     (116)      967 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0011_sharedkey.py
--rw-r--r--   0 runner    (1001) docker     (116)     1619 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0018_auto_20210714_2216.py
--rw-r--r--   0 runner    (1001) docker     (116)      400 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0009_auto_20171205_0252.py
--rw-r--r--   0 runner    (1001) docker     (116)      687 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0015_auto_20200508_2104.py
--rw-r--r--   0 runner    (1001) docker     (116)     2126 2022-02-24 21:25:03.000000 morango-0.6.9/morango/migrations/0008_auto_20171114_2217.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-24 21:25:11.000000 morango-0.6.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (116)       37 2022-02-24 21:25:03.000000 morango-0.6.9/requirements/accelerated.txt
--rw-r--r--   0 runner    (1001) docker     (116)       45 2022-02-24 21:25:03.000000 morango-0.6.9/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      175 2022-02-24 21:25:03.000000 morango-0.6.9/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (116)      295 2022-02-24 21:25:03.000000 morango-0.6.9/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (116)       34 2022-02-24 21:25:03.000000 morango-0.6.9/requirements/postgres.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-09 14:33:44.000000 morango-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      276 2023-06-09 14:33:44.000000 morango-0.7.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (122)     5662 2023-06-09 14:33:44.000000 morango-0.7.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-09 14:33:44.000000 morango-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-09 14:33:59.000000 morango-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      757 2023-06-09 14:33:59.000000 morango-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-06-09 14:33:44.000000 morango-0.7.0/requirements/postgres.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-06-09 14:33:44.000000 morango-0.7.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-06-09 14:33:44.000000 morango-0.7.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-06-09 14:33:44.000000 morango-0.7.0/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       37 2023-06-09 14:33:44.000000 morango-0.7.0/requirements/accelerated.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2785 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      134 2023-06-09 14:33:59.000000 morango-0.7.0/morango.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1702 2023-06-09 14:33:44.000000 morango-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/management/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)     3044 2023-06-09 14:33:44.000000 morango-0.7.0/morango/management/commands/cleanupsyncs.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/api/
+-rw-r--r--   0 runner    (1001) docker     (122)    20769 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/viewsets.py
+-rw-r--r--   0 runner    (1001) docker     (122)      273 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5444 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3550 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      557 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-06-09 14:33:44.000000 morango-0.7.0/morango/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      546 2023-06-09 14:33:44.000000 morango-0.7.0/morango/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)      166 2023-06-09 14:33:44.000000 morango-0.7.0/morango/constants/capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (122)      510 2023-06-09 14:33:44.000000 morango-0.7.0/morango/constants/transfer_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-06-09 14:33:44.000000 morango-0.7.0/morango/constants/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1379 2023-06-09 14:33:44.000000 morango-0.7.0/morango/constants/transfer_stages.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-09 14:33:44.000000 morango-0.7.0/morango/constants/api_urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/sync/
+-rw-r--r--   0 runner    (1001) docker     (122)    69494 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/operations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3293 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/session.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25198 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/syncsession.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8792 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/sync/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)    10867 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5198 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/backends/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12850 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/backends/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19850 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/backends/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11575 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/controller.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17815 2023-06-09 14:33:44.000000 morango-0.7.0/morango/sync/context.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10999 2023-06-09 14:33:44.000000 morango-0.7.0/morango/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3676 2023-06-09 14:33:44.000000 morango-0.7.0/morango/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/manager.py
+-rw-r--r--   0 runner    (1001) docker     (122)      478 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/models/fields/
+-rw-r--r--   0 runner    (1001) docker     (122)    13984 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/fields/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4283 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/fields/uuids.py
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1024 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/morango_mptt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7130 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/fsic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6644 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15331 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38771 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1983 2023-06-09 14:33:44.000000 morango-0.7.0/morango/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:59.000000 morango-0.7.0/morango/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      481 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0014_syncsession_extra_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)      461 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0016_store_deserialization_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0009_auto_20171205_0252.py
+-rw-r--r--   0 runner    (1001) docker     (122)      687 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0015_auto_20200508_2104.py
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0017_store_last_transfer_session_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      558 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0004_auto_20170520_2112.py
+-rw-r--r--   0 runner    (1001) docker     (122)      841 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0010_auto_20171206_1615.py
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0003_auto_20170519_0543.py
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0011_sharedkey.py
+-rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0005_auto_20170629_2139.py
+-rw-r--r--   0 runner    (1001) docker     (122)      987 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0012_auto_20180927_1658.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11933 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2250 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0021_store_partition_index_create.py
+-rw-r--r--   0 runner    (1001) docker     (122)      505 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0013_auto_20190627_1513.py
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0023_add_instance_id_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0008_auto_20171114_2217.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1247 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0020_postgres_fix_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0022_rename_instance_fields.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1619 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0018_auto_20210714_2216.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0002_auto_20170511_0400.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8190 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0007_auto_20171018_1615.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1541 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0019_auto_20220113_1807.py
+-rw-r--r--   0 runner    (1001) docker     (122)      476 2023-06-09 14:33:44.000000 morango-0.7.0/morango/migrations/0006_instanceidmodel_system_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-09 14:33:44.000000 morango-0.7.0/morango/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-06-09 14:33:44.000000 morango-0.7.0/morango/errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-06-09 14:33:44.000000 morango-0.7.0/morango/proquint.py
+-rw-r--r--   0 runner    (1001) docker     (122)      141 2023-06-09 14:33:44.000000 morango-0.7.0/morango/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1374 2023-06-09 14:33:44.000000 morango-0.7.0/README.md
```

### Comparing `morango-0.6.9/CHANGELOG.md` & `morango-0.7.0/CHANGELOG.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,36 @@
 # Release Notes
 
 List of the most important changes for each release.
 
+## 0.6.16
+- Added dedicated `client_instance_id` and `server_instance_id` fields to `SyncSession`
+- Renamed `client_instance` and `server_instance` fields on `SyncSession` to `client_instance_json` and `server_instance_json` respectively
+
+## 0.6.15
+- Fixes issue causing overflow error during lengthy syncs
+
+## 0.6.14
+- Fixes issue that caused discrepancies between the client's and server's sync state
+- Fixes issue with transaction isolation persisting longer than intended
+
+## 0.6.13
+- Capture and retry transaction isolation errors that occur when conflicting concurrent updates are made during the transaction
+
+## 0.6.12
+- Replace serializable transaction isolation using a separate DB connection for Postgres with advisory locking.
+
+## 0.6.11
+- Added deferred processing of foreign keys to allow bulk processing and to improve performance.
+- Eliminated extraneous SQL queries for the transfer session when querying for buffers.
+- Added database index to Store's partition field to improve querying performance.
+
+## 0.6.10
+- Fixes Django migration issue introduced in 0.6.7 allowing nullable fields with PostgreSQL backends
+
 ## 0.6.9
 - Fixes un-ordered selection of buffers during sync which can allow duplicates to be synced with PostgreSQL backends
 - Moves updating of database counters to occur in the same DB transaction as updates to the Store
 - Adds setting to disable reduction of FSICs when calculating them for a set of partitions
 
 ## 0.6.8
 - Fixes subset syncing issues by introducing new FSIC v2 format
```

### Comparing `morango-0.6.9/morango.egg-info/SOURCES.txt` & `morango-0.7.0/morango.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,16 @@
 setup.cfg
 setup.py
 morango/__init__.py
 morango/apps.py
 morango/errors.py
 morango/proquint.py
 morango/registry.py
-morango/settings.py
 morango/urls.py
 morango/utils.py
-morango/wsgi.py
 morango.egg-info/PKG-INFO
 morango.egg-info/SOURCES.txt
 morango.egg-info/dependency_links.txt
 morango.egg-info/not-zip-safe
 morango.egg-info/requires.txt
 morango.egg-info/top_level.txt
 morango/api/__init__.py
@@ -51,14 +49,18 @@
 morango/migrations/0013_auto_20190627_1513.py
 morango/migrations/0014_syncsession_extra_fields.py
 morango/migrations/0015_auto_20200508_2104.py
 morango/migrations/0016_store_deserialization_error.py
 morango/migrations/0017_store_last_transfer_session_id.py
 morango/migrations/0018_auto_20210714_2216.py
 morango/migrations/0019_auto_20220113_1807.py
+morango/migrations/0020_postgres_fix_nullable.py
+morango/migrations/0021_store_partition_index_create.py
+morango/migrations/0022_rename_instance_fields.py
+morango/migrations/0023_add_instance_id_fields.py
 morango/migrations/__init__.py
 morango/models/__init__.py
 morango/models/certificates.py
 morango/models/core.py
 morango/models/fsic_utils.py
 morango/models/manager.py
 morango/models/morango_mptt.py
```

### Comparing `morango-0.6.9/morango.egg-info/PKG-INFO` & `morango-0.7.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morango
-Version: 0.6.9
+Version: 0.7.0
 Summary: Pure Python sqlite-based Django DB replication engine.
 Home-page: https://github.com/learningequality/morango
 Author: Learning Equality
 Author-email: dev@learningequality.org
 License: MIT
 Description: # Morango
         
@@ -41,11 +41,14 @@
 Keywords: database,syncing,morango
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `morango-0.6.9/setup.py` & `morango-0.7.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 from __future__ import print_function
 from __future__ import unicode_literals
 
 import io
-from setuptools import find_packages, setup
+
+from setuptools import find_packages
+from setuptools import setup
 
 import morango
 
 readme = io.open("README.md", mode="r", encoding="utf-8").read()
 
 setup(
     name='morango',
@@ -39,12 +41,15 @@
     keywords=['database', 'syncing', 'morango'],
     classifiers=[
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Development Status :: 4 - Beta',
         'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 )
```

### Comparing `morango-0.6.9/README.md` & `morango-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/setup.cfg` & `morango-0.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/LICENSE` & `morango-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/PKG-INFO` & `morango-0.7.0/morango.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morango
-Version: 0.6.9
+Version: 0.7.0
 Summary: Pure Python sqlite-based Django DB replication engine.
 Home-page: https://github.com/learningequality/morango
 Author: Learning Equality
 Author-email: dev@learningequality.org
 License: MIT
 Description: # Morango
         
@@ -41,11 +41,14 @@
 Keywords: database,syncing,morango
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `morango-0.6.9/morango/proquint.py` & `morango-0.7.0/morango/proquint.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/management/commands/cleanupsyncs.py` & `morango-0.7.0/morango/management/commands/cleanupsyncs.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/apps.py` & `morango-0.7.0/morango/apps.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/utils.py` & `morango-0.7.0/morango/utils.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/api/urls.py` & `morango-0.7.0/morango/api/urls.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/api/permissions.py` & `morango-0.7.0/morango/api/permissions.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/api/parsers.py` & `morango-0.7.0/morango/api/parsers.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/api/serializers.py` & `morango-0.7.0/morango/api/serializers.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     class Meta:
         model = Nonce
         fields = ("id", "timestamp", "ip")
         read_only_fields = fields
 
 
 class SyncSessionSerializer(serializers.ModelSerializer):
+    client_instance = serializers.CharField(source='client_instance_json')
+    server_instance = serializers.CharField(source='server_instance_json')
+
     class Meta:
         model = SyncSession
         fields = (
             "id",
             "start_timestamp",
             "last_activity_timestamp",
             "active",
```

### Comparing `morango-0.6.9/morango/api/viewsets.py` & `morango-0.7.0/morango/api/viewsets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
+import logging
 import platform
 import uuid
-import logging
 
 from django.core.exceptions import ValidationError
 from django.utils import timezone
 from ipware.ip import get_ip
 from rest_framework import mixins
 from rest_framework import pagination
 from rest_framework import response
@@ -26,16 +26,16 @@
 from morango.models.core import Certificate
 from morango.models.core import InstanceIDModel
 from morango.models.core import SyncSession
 from morango.models.core import TransferSession
 from morango.models.fields.crypto import SharedKey
 from morango.sync.context import LocalSessionContext
 from morango.sync.controller import SessionController
-from morango.utils import CAPABILITIES
 from morango.utils import _assert
+from morango.utils import CAPABILITIES
 from morango.utils import parse_capabilities_from_server_request
 
 
 if GZIP_BUFFER_POST in CAPABILITIES:
     from .parsers import GzipParser
 
     parsers = (GzipParser, JSONParser)
@@ -232,15 +232,15 @@
     viewsets.mixins.RetrieveModelMixin,
     viewsets.GenericViewSet,
 ):
     serializer_class = serializers.SyncSessionSerializer
 
     def create(self, request):
 
-        instance_id, _ = InstanceIDModel.get_or_create_current_instance()
+        server_instance, _ = InstanceIDModel.get_or_create_current_instance()
 
         # verify and save the certificate chain to our cert store
         try:
             Certificate.save_certificate_chain(
                 request.data.get("certificate_chain"),
                 expected_last_id=request.data.get("client_certificate_id"),
             )
@@ -283,41 +283,49 @@
         try:
             certificates.Nonce.use_nonce(request.data["nonce"])
         except errors.MorangoNonceError:
             return response.Response(
                 "Nonce is not valid", status=status.HTTP_403_FORBIDDEN
             )
 
+        client_instance_json = request.data.get("instance")
+        client_instance_id = None
+        if client_instance_json:
+            client_instance = json.loads(client_instance_json)
+            client_instance_id = client_instance.get("id")
+
         # build the data to be used for creation the syncsession
         data = {
             "id": request.data.get("id"),
             "start_timestamp": timezone.now(),
             "last_activity_timestamp": timezone.now(),
             "active": True,
             "is_server": True,
             "client_certificate": client_cert,
             "server_certificate": server_cert,
             "profile": server_cert.profile,
             "connection_kind": "network",
             "connection_path": request.data.get("connection_path"),
             "client_ip": get_ip(request) or "",
             "server_ip": request.data.get("server_ip") or "",
-            "client_instance": request.data.get("instance"),
-            "server_instance": json.dumps(
-                serializers.InstanceIDSerializer(instance_id).data
+            "client_instance_id": client_instance_id,
+            "client_instance_json": client_instance_json,
+            "server_instance_id": server_instance.id,
+            "server_instance_json": json.dumps(
+                serializers.InstanceIDSerializer(server_instance).data
             ),
         }
 
         syncsession = SyncSession(**data)
         syncsession.full_clean()
         syncsession.save()
 
         resp_data = {
             "signature": server_cert.sign(message),
-            "server_instance": data["server_instance"],
+            "server_instance": data["server_instance_json"],
         }
 
         return response.Response(resp_data, status=status.HTTP_201_CREATED)
 
     def perform_destroy(self, syncsession):
         syncsession.active = False
         syncsession.save()
@@ -364,16 +372,16 @@
             if not requested_filter.is_subset_of(client_scope.read_filter):
                 scope_error_msg = "Client certificate scope does not permit pulling for the requested filter."
             if not requested_filter.is_subset_of(server_scope.write_filter):
                 scope_error_msg = "Server certificate scope does not permit responding to pulls for the requested filter."
         if scope_error_msg:
             return response.Response(scope_error_msg, status=status.HTTP_403_FORBIDDEN)
 
-        context = LocalSessionContext(
-            request=request,
+        context = LocalSessionContext.from_request(
+            request,
             sync_session=syncsession,
             sync_filter=requested_filter,
             is_push=is_a_push,
         )
 
         # If both client and ourselves allow async, we just return accepted status, and the client
         # should PATCH the transfer_session to the appropriate stage. If not async, we wait until
@@ -412,31 +420,31 @@
                 "Only PATCH updates allowed", status=status.HTTP_405_METHOD_NOT_ALLOWED
             )
 
         update_stage = request.data.pop("transfer_stage", None)
         if update_stage is not None:
             # if client is trying to update `transfer_stage`, then we use the controller to proceed
             # to the stage, but wait for completion if both do not support async
-            context = LocalSessionContext(
-                request=request,
+            context = LocalSessionContext.from_request(
+                request,
                 transfer_session=self.get_object(),
             )
             # special case for transferring, not to wait since it's a chunked process
             if self.async_allowed() or update_stage == transfer_stages.TRANSFERRING:
                 session_controller.proceed_to(update_stage, context=context)
             else:
                 session_controller.proceed_to_and_wait_for(
                     update_stage, context=context, max_interval=2
                 )
 
         return super(TransferSessionViewSet, self).update(request, *args, **kwargs)
 
     def perform_destroy(self, transfer_session):
-        context = LocalSessionContext(
-            request=self.request,
+        context = LocalSessionContext.from_request(
+            self.request,
             transfer_session=transfer_session,
         )
         if self.async_allowed():
             session_controller.proceed_to(transfer_stages.CLEANUP, context=context)
         else:
             result = session_controller.proceed_to_and_wait_for(
                 transfer_stages.CLEANUP, context=context, max_interval=2
@@ -478,16 +486,16 @@
             )
         if len(set(rec["transfer_session"] for rec in data)) > 1:
             return response.Response(
                 "All pushed records must be associated with the same TransferSession.",
                 status=status.HTTP_403_FORBIDDEN,
             )
 
-        context = LocalSessionContext(
-            request=request, transfer_session=transfer_session
+        context = LocalSessionContext.from_request(
+            request, transfer_session=transfer_session
         )
         result = session_controller.proceed_to(
             transfer_stages.TRANSFERRING, context=context
         )
 
         if result == transfer_statuses.ERRORED:
             if context.error:
@@ -505,21 +513,23 @@
 
 
 class MorangoInfoViewSet(viewsets.ViewSet):
     def retrieve(self, request, pk=None):
         (id_model, _) = InstanceIDModel.get_or_create_current_instance()
         # include custom instance info as well
         m_info = id_model.instance_info.copy()
-        m_info.update({
-            "instance_hash": id_model.get_proquint(),
-            "instance_id": id_model.id,
-            "system_os": platform.system(),
-            "version": morango.__version__,
-            "capabilities": CAPABILITIES,
-        })
+        m_info.update(
+            {
+                "instance_hash": id_model.get_proquint(),
+                "instance_id": id_model.id,
+                "system_os": platform.system(),
+                "version": morango.__version__,
+                "capabilities": CAPABILITIES,
+            }
+        )
         return response.Response(m_info)
 
 
 class PublicKeyViewSet(viewsets.ReadOnlyModelViewSet):
     permission_classes = (permissions.CertificatePushPermissions,)
     serializer_class = serializers.SharedKeySerializer
```

### Comparing `morango-0.6.9/morango/models/fields/uuids.py` & `morango-0.7.0/morango/models/fields/uuids.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/models/fields/crypto.py` & `morango-0.7.0/morango/models/fields/crypto.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/models/core.py` & `morango-0.7.0/morango/models/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import unicode_literals
 
 import functools
 import json
 import logging
 import uuid
+from collections import defaultdict
+from collections import namedtuple
+from functools import reduce
 
 from django.core import exceptions
 from django.db import connection
 from django.db import models
 from django.db import router
 from django.db import transaction
 from django.db.models import F
@@ -20,32 +23,30 @@
 from django.db.models.expressions import CombinedExpression
 from django.db.models.fields.related import ForeignKey
 from django.db.models.functions import Cast
 from django.utils import six
 from django.utils import timezone
 from django.utils.functional import cached_property
 
-from functools import reduce
-
 from morango import proquint
+from morango.constants import transfer_stages
+from morango.constants import transfer_statuses
 from morango.errors import InvalidMorangoSourceId
-from morango.registry import syncable_models
 from morango.models.certificates import Certificate
 from morango.models.certificates import Filter
 from morango.models.fields.uuids import sha2_uuid
 from morango.models.fields.uuids import UUIDField
 from morango.models.fields.uuids import UUIDModelMixin
 from morango.models.fsic_utils import remove_redundant_instance_counters
 from morango.models.manager import SyncableModelManager
 from morango.models.morango_mptt import MorangoMPTTModel
 from morango.models.utils import get_0_4_system_parameters
-from morango.models.utils import get_0_5_system_id
 from morango.models.utils import get_0_5_mac_address
-from morango.constants import transfer_stages
-from morango.constants import transfer_statuses
+from morango.models.utils import get_0_5_system_id
+from morango.registry import syncable_models
 from morango.utils import _assert
 from morango.utils import SETTINGS
 
 logger = logging.getLogger(__name__)
 
 
 class DatabaseIDManager(models.Manager):
@@ -117,15 +118,15 @@
 
     id = UUIDField(max_length=32, primary_key=True, editable=False)
 
     platform = models.TextField()
     hostname = models.TextField()
     sysversion = models.TextField()
     node_id = models.CharField(max_length=20, blank=True)
-    database = models.ForeignKey(DatabaseIDModel)
+    database = models.ForeignKey(DatabaseIDModel, on_delete=models.CASCADE)
     counter = models.IntegerField(default=0)
     current = models.BooleanField(default=True)
     db_path = models.CharField(max_length=1000)
     system_id = models.CharField(max_length=100, blank=True)
 
     @property
     def instance_info(self):
@@ -214,18 +215,18 @@
     active = models.BooleanField(default=True)
 
     # track whether this device is acting as the server for the sync session
     is_server = models.BooleanField(default=False)
 
     # track the certificates being used by each side for this session
     client_certificate = models.ForeignKey(
-        Certificate, blank=True, null=True, related_name="syncsessions_client"
+        Certificate, blank=True, null=True, related_name="syncsessions_client", on_delete=models.CASCADE
     )
     server_certificate = models.ForeignKey(
-        Certificate, blank=True, null=True, related_name="syncsessions_server"
+        Certificate, blank=True, null=True, related_name="syncsessions_server", on_delete=models.CASCADE
     )
 
     # track the morango profile this sync session is happening for
     profile = models.CharField(max_length=40)
 
     # information about the connection over which this sync session is happening
     connection_kind = models.CharField(
@@ -235,31 +236,34 @@
         max_length=1000
     )  # file path if kind=disk, and base URL of server if kind=network
 
     # for network connections, keep track of the IPs on either end
     client_ip = models.CharField(max_length=100, blank=True)
     server_ip = models.CharField(max_length=100, blank=True)
 
-    # serialized copies of the client and server instance model fields, for debugging/tracking purposes
-    client_instance = models.TextField(default="{}")
-    server_instance = models.TextField(default="{}")
+    # track the instance IDs for convenient querying, as well as serialized copies of
+    # the client and server instance model fields for debugging/tracking purposes
+    client_instance_id = models.UUIDField(null=True, blank=True)
+    client_instance_json = models.TextField(default="{}")
+    server_instance_id = models.UUIDField(null=True, blank=True)
+    server_instance_json = models.TextField(default="{}")
 
     # used to store other data we may need to know about this sync session
     extra_fields = models.TextField(default="{}")
 
     # system process ID for ensuring same sync session does not run in parallel
     process_id = models.IntegerField(blank=True, null=True)
 
     @cached_property
     def client_instance_data(self):
-        return json.loads(self.client_instance)
+        return json.loads(self.client_instance_json)
 
     @cached_property
     def server_instance_data(self):
-        return json.loads(self.server_instance)
+        return json.loads(self.server_instance_json)
 
 
 class TransferSession(models.Model):
     """
     ``TransferSession`` holds metadata that is related to a specific transfer (push/pull) session
     between 2 morango instances.
     """
@@ -275,15 +279,15 @@
     )  # track how many records have already been transferred
     records_total = models.IntegerField(
         blank=True, null=True
     )  # total number of records to be synced across in this transfer
     bytes_sent = models.BigIntegerField(default=0, null=True, blank=True)
     bytes_received = models.BigIntegerField(default=0, null=True, blank=True)
 
-    sync_session = models.ForeignKey(SyncSession)
+    sync_session = models.ForeignKey(SyncSession, on_delete=models.CASCADE)
 
     # track when the transfer session started and the last time there was activity on it
     start_timestamp = models.DateTimeField(default=timezone.now)
     last_activity_timestamp = models.DateTimeField(blank=True)
 
     # we keep track of FSICs for both client and server
     client_fsic = models.TextField(blank=True, default="{}")
@@ -442,94 +446,103 @@
 
     last_transfer_session_id = UUIDField(
         blank=True, null=True, default=None, db_index=True
     )
 
     objects = StoreManager()
 
-    def _deserialize_store_model(self, fk_cache):  # noqa: C901
+    class Meta:
+        indexes = [
+            models.Index(fields=["partition"], name="idx_morango_store_partition"),
+        ]
+
+    def _deserialize_store_model(self, fk_cache, defer_fks=False):  # noqa: C901
         """
         When deserializing a store model, we look at the deleted flags to know if we should delete the app model.
         Upon loading the app model in memory we validate the app models fields, if any errors occurs we follow
         foreign key relationships to see if the related model has been deleted to propagate that deletion to the target app model.
         We return:
-        None => if the model was deleted successfully
-        model => if the model validates successfully
+            None => if the model was deleted successfully
+            model => if the model validates successfully
         """
+        deferred_fks = {}
         klass_model = syncable_models.get_model(self.profile, self.model_name)
         # if store model marked as deleted, attempt to delete in app layer
         if self.deleted:
             # if hard deleted, propagate to related models
             if self.hard_deleted:
                 try:
                     klass_model.objects.get(id=self.id).delete(hard_delete=True)
                 except klass_model.DoesNotExist:
                     pass
             else:
                 klass_model.objects.filter(id=self.id).delete()
-            return None
+            return None, deferred_fks
         else:
             # load model into memory
             app_model = klass_model.deserialize(json.loads(self.serialized))
             app_model._morango_source_id = self.source_id
             app_model._morango_partition = self.partition
             app_model._morango_dirty_bit = False
 
             try:
-
                 # validate and return the model
-                app_model.cached_clean_fields(fk_cache)
-                return app_model
+                if defer_fks:
+                    deferred_fks = app_model.deferred_clean_fields()
+                else:
+                    app_model.cached_clean_fields(fk_cache)
+                return app_model, deferred_fks
 
             except (exceptions.ValidationError, exceptions.ObjectDoesNotExist) as e:
 
                 logger.warning(
                     "Error deserializing instance of {model} with id {id}: {error}".format(
                         model=klass_model.__name__, id=app_model.id, error=e
                     )
                 )
 
-                # check FKs in store to see if any of those models were deleted or hard_deleted to propagate to this model
-                fk_ids = [
-                    getattr(app_model, field.attname)
-                    for field in app_model._meta.fields
-                    if isinstance(field, ForeignKey)
-                ]
-                for fk_id in fk_ids:
-                    try:
-                        st_model = Store.objects.get(id=fk_id)
-                        if st_model.deleted:
-                            # if hard deleted, propagate to store model
-                            if st_model.hard_deleted:
-                                app_model._update_hard_deleted_models()
-                            app_model._update_deleted_models()
-                            return None
-                    except Store.DoesNotExist:
-                        pass
+                if not defer_fks and isinstance(e, exceptions.ObjectDoesNotExist):
+                    # check FKs in store to see if any of those models were deleted or hard_deleted to propagate to this model
+                    fk_ids = [
+                        getattr(app_model, field.attname)
+                        for field in app_model._meta.fields
+                        if isinstance(field, ForeignKey)
+                    ]
+                    for fk_id in fk_ids:
+                        try:
+                            st_model = Store.objects.get(id=fk_id)
+                            if st_model.deleted:
+                                # if hard deleted, propagate to store model
+                                if st_model.hard_deleted:
+                                    app_model._update_hard_deleted_models()
+                                app_model._update_deleted_models()
+                                return None, {}
+                        except Store.DoesNotExist:
+                            pass
 
                 # if we got here, it means the validation error wasn't handled by propagating deletion, so re-raise it
                 raise e
 
 
 class Buffer(AbstractStore):
     """
     ``Buffer`` is where records from the internal store are queued up temporarily, before being
     sent to another morango instance, or stored while being received from another instance, before
     dequeuing into the local store.
     """
 
-    transfer_session = models.ForeignKey(TransferSession)
+    transfer_session = models.ForeignKey(TransferSession, on_delete=models.CASCADE)
     model_uuid = UUIDField()
 
     class Meta:
         unique_together = ("transfer_session", "model_uuid")
 
     def rmcb_list(self):
         return RecordMaxCounterBuffer.objects.filter(
-            model_uuid=self.model_uuid, transfer_session=self.transfer_session
+            model_uuid=self.model_uuid, transfer_session_id=self.transfer_session_id
         )
 
 
 class AbstractCounter(models.Model):
     """
     Abstract class which shares fields across multiple counter models.
     """
@@ -747,30 +760,35 @@
 class RecordMaxCounter(AbstractCounter):
     """
     ``RecordMaxCounter`` keeps track of the maximum counter each serialized record has been saved at,
     for each instance that has modified it. This is used to determine fast-forwards and merge conflicts
     during the sync process.
     """
 
-    store_model = models.ForeignKey(Store)
+    store_model = models.ForeignKey(Store, on_delete=models.CASCADE)
 
     class Meta:
         unique_together = ("store_model", "instance_id")
 
 
 class RecordMaxCounterBuffer(AbstractCounter):
     """
     ``RecordMaxCounterBuffer`` is where combinations of instance ID and counters (from ``RecordMaxCounter``) are stored temporarily,
     until they are sent or received by another morango instance.
     """
 
-    transfer_session = models.ForeignKey(TransferSession)
+    transfer_session = models.ForeignKey(TransferSession, on_delete=models.CASCADE)
     model_uuid = UUIDField(db_index=True)
 
 
+ForeignKeyReference = namedtuple(
+    "ForeignKeyReference", ["from_field", "from_pk", "to_pk"]
+)
+
+
 class SyncableModel(UUIDModelMixin):
     """
     ``SyncableModel`` is the base model class for syncing. Other models inherit from this class if they want to make
     their data syncable across devices.
     """
 
     # constant value to insert into partition strings in place of current model's ID, as needed (to avoid circularity)
@@ -831,35 +849,80 @@
                         model, MorangoMPTTModel
                     ):
                         for obj in instances:
                             obj._update_hard_deleted_models()
             return collector.delete()
 
     def cached_clean_fields(self, fk_lookup_cache):
+        """
+        Immediately validates all fields, but uses a cache for foreign key (FK) lookups to reduce
+        repeated queries for many records with the same FK
+
+        :param fk_lookup_cache: A dictionary to use as a cache to prevent querying the database if a
+            FK exists in the cache, having already been validated
+        """
         excluded_fields = []
         fk_fields = [
             field for field in self._meta.fields if isinstance(field, models.ForeignKey)
         ]
+
         for f in fk_fields:
             raw_value = getattr(self, f.attname)
-            key = "morango_{id}_{db_table}_foreignkey".format(
+            key = "{id}_{db_table}".format(
                 db_table=f.related_model._meta.db_table, id=raw_value
             )
             try:
                 fk_lookup_cache[key]
                 excluded_fields.append(f.name)
             except KeyError:
                 try:
                     f.validate(raw_value, self)
                 except exceptions.ValidationError:
                     pass
                 else:
                     fk_lookup_cache[key] = 1
                     excluded_fields.append(f.name)
+
+        self.clean_fields(exclude=excluded_fields)
+
+        # after cleaning, we can confidently set ourselves in the fk_lookup_cache
+        self_key = "{id}_{db_table}".format(
+            db_table=self._meta.db_table,
+            id=self.id,
+        )
+        fk_lookup_cache[self_key] = 1
+
+    def deferred_clean_fields(self):
+        """
+        Calls `.clean_fields()` but excludes all foreign key fields and instead returns them as a
+        dictionary for deferred batch processing
+
+        :return: A dictionary containing lists of `ForeignKeyReference`s keyed by the name of the
+            model being referenced by the FK
+        """
+        excluded_fields = []
+        deferred_fks = defaultdict(list)
+        for field in self._meta.fields:
+            if not isinstance(field, models.ForeignKey):
+                continue
+            # by not excluding the field if it's null, the default validation logic will apply
+            # and should raise a ValidationError if the FK field is not nullable
+            if getattr(self, field.attname) is None:
+                continue
+            excluded_fields.append(field.name)
+            deferred_fks[field.related_model._meta.verbose_name].append(
+                ForeignKeyReference(
+                    from_field=field.attname,
+                    from_pk=self.pk,
+                    to_pk=getattr(self, field.attname),
+                )
+            )
+
         self.clean_fields(exclude=excluded_fields)
+        return deferred_fks
 
     def serialize(self):
         """All concrete fields of the ``SyncableModel`` subclass, except for those specifically blacklisted, are returned in a dict."""
         # NOTE: code adapted from https://github.com/django/django/blob/master/django/forms/models.py#L75
         opts = self._meta
 
         data = {}
```

### Comparing `morango-0.6.9/morango/models/utils.py` & `morango-0.7.0/morango/models/utils.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/models/__init__.py` & `morango-0.7.0/morango/models/__init__.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/models/morango_mptt.py` & `morango-0.7.0/morango/models/morango_mptt.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/models/certificates.py` & `morango-0.7.0/morango/models/certificates.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,21 +31,21 @@
 
 
 @python_2_unicode_compatible
 class Certificate(mptt.models.MPTTModel, UUIDModelMixin):
 
     uuid_input_fields = ("public_key", "profile", "salt")
 
-    parent = models.ForeignKey("Certificate", blank=True, null=True)
+    parent = models.ForeignKey("Certificate", blank=True, null=True, on_delete=models.CASCADE)
 
     # the Morango profile with which this certificate is associated
     profile = models.CharField(max_length=20)
 
     # scope of this certificate, and version of the scope, along with associated params
-    scope_definition = models.ForeignKey("ScopeDefinition")
+    scope_definition = models.ForeignKey("ScopeDefinition", on_delete=models.CASCADE)
     scope_version = models.IntegerField()
     scope_params = (
         models.TextField()
     )  # JSON dict of values to insert into scope definitions
 
     # track the certificate's public key so we can verify any certificates it signs
     public_key = PublicKeyField()
```

### Comparing `morango-0.6.9/morango/models/query.py` & `morango-0.7.0/morango/models/query.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/models/fsic_utils.py` & `morango-0.7.0/morango/models/fsic_utils.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/constants/settings.py` & `morango-0.7.0/morango/constants/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,17 @@
     "morango.sync.operations:ProducerQueueOperation",
     "morango.sync.operations:ReceiverQueueOperation",
     "morango.sync.operations:LegacyNetworkQueueOperation",
     "morango.sync.operations:NetworkQueueOperation",
 )
 MORANGO_TRANSFERRING_OPERATIONS = (
     "morango.sync.operations:PullProducerOperation",
+    "morango.sync.operations:PushProducerOperation",
     "morango.sync.operations:PushReceiverOperation",
+    "morango.sync.operations:PullReceiverOperation",
     "morango.sync.operations:NetworkPushTransferOperation",
     "morango.sync.operations:NetworkPullTransferOperation",
 )
 MORANGO_DEQUEUE_OPERATIONS = (
     "morango.sync.operations:ProducerDequeueOperation",
     "morango.sync.operations:ReceiverDequeueOperation",
     "morango.sync.operations:LegacyNetworkDequeueOperation",
@@ -39,7 +41,8 @@
     "morango.sync.operations:LegacyNetworkDeserializeOperation",
     "morango.sync.operations:NetworkDeserializeOperation",
 )
 MORANGO_CLEANUP_OPERATIONS = (
     "morango.sync.operations:CleanupOperation",
     "morango.sync.operations:NetworkCleanupOperation",
 )
+MORANGO_TEST_POSTGRESQL = False
```

### Comparing `morango-0.6.9/morango/constants/transfer_stages.py` & `morango-0.7.0/morango/constants/transfer_stages.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/errors.py` & `morango-0.7.0/morango/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,7 +72,11 @@
 
 class MorangoInvalidFSICPartition(MorangoError):
     pass
 
 
 class MorangoSkipOperation(MorangoError):
     pass
+
+
+class MorangoDatabaseError(MorangoError):
+    pass
```

### Comparing `morango-0.6.9/morango/registry.py` & `morango-0.7.0/morango/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 `SyncableModelRegistry` holds all syncable models for a project, on a per profile basis.
 This class is registered at app load time for morango in `apps.py`.
 """
-import sys
 import inspect
+import sys
 from collections import OrderedDict
 
 from django.db.models.fields.related import ForeignKey
 from django.utils import six
 
 from morango.constants import transfer_stages
 from morango.errors import InvalidMorangoModelConfiguration
@@ -15,15 +15,15 @@
 from morango.errors import UnsupportedFieldType
 from morango.utils import do_import
 from morango.utils import SETTINGS
 
 
 def _get_foreign_key_classes(m):
     return set(
-        [field.rel.to for field in m._meta.fields if isinstance(field, ForeignKey)]
+        [field.related_model for field in m._meta.fields if isinstance(field, ForeignKey)]
     )
 
 
 def _multiple_self_ref_fk_check(class_model):
     """
     We check whether a class has more than 1 FK reference to itself.
     """
@@ -192,14 +192,15 @@
 
 
 class SessionMiddlewareOperations(list):
     """
     Iterable list class that holds and initializes a list of transfer operations as configured
     through Morango settings, and associate the group with a transfer stage by `related_stage`
     """
+
     __slots__ = ("related_stage",)
 
     def __init__(self, related_stage):
         super(SessionMiddlewareOperations, self).__init__()
         self.related_stage = related_stage
 
     def populate(self, callable_imports):
@@ -226,15 +227,17 @@
         for operation in self:
             result = operation(context)
             # operation tells us it has "handled" the context by returning result that is not False
             if result is not False:
                 return result
         else:
             raise NotImplementedError(
-                "Operation for {} stage has no middleware".format(self.related_stage)
+                "Operation for {} stage has no applicable middleware for context '{}'".format(
+                    self.related_stage, context.__class__.__name__
+                )
             )
 
 
 STAGE_TO_SETTINGS = {
     transfer_stages.INITIALIZING: "MORANGO_INITIALIZE_OPERATIONS",
     transfer_stages.SERIALIZING: "MORANGO_SERIALIZE_OPERATIONS",
     transfer_stages.QUEUING: "MORANGO_QUEUE_OPERATIONS",
```

### Comparing `morango-0.6.9/morango/sync/session.py` & `morango-0.7.0/morango/sync/session.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/sync/context.py` & `morango-0.7.0/morango/sync/backends/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,319 +1,212 @@
-from morango.constants import transfer_stages
-from morango.constants import transfer_statuses
-from morango.errors import MorangoContextUpdateError
-from morango.models.certificates import Filter
-from morango.models.core import SyncSession
-from morango.models.core import TransferSession
-from morango.utils import parse_capabilities_from_server_request
-from morango.utils import CAPABILITIES
-
-
-class SessionContext(object):
-    """
-    Class that holds the context of a transfer, for executing transfer ops through the middleware
-    """
-
-    __slots__ = (
-        "sync_session",
-        "transfer_session",
-        "filter",
-        "is_push",
-        "capabilities",
-        "error",
-    )
-
-    def __init__(
-        self,
-        sync_session=None,
-        transfer_session=None,
-        sync_filter=None,
-        is_push=None,
-        capabilities=None,
-    ):
-        """
-        :param sync_session: The sync session instance
-        :type sync_session: SyncSession|None
-        :param transfer_session: The current transfer session that will be operated against
-        :type transfer_session: TransferSession|None
-        :param sync_filter The sync filter to use for the TransferSession
-        :type sync_filter Filter|None
-        :param is_push: A boolean indicating whether or not the transfer is a push or pull
-        :type is_push: bool
-        :param capabilities: Capabilities set that is combined (intersected) with our own capabilities
-        :type capabilities: set|None
-        """
-        self.sync_session = sync_session
-        self.transfer_session = transfer_session
-        self.filter = sync_filter
-        self.is_push = is_push
-        self.capabilities = set(capabilities or []) & CAPABILITIES
-        self.error = None
-
-        if self.transfer_session:
-            self.sync_session = transfer_session.sync_session or self.sync_session
-            self.is_push = transfer_session.push or self.is_push
-            if transfer_session.filter:
-                self.filter = transfer_session.get_filter()
-
-    def update(
-        self,
-        transfer_session=None,
-        sync_filter=None,
-        is_push=None,
-        stage=None,
-        stage_status=None,
-        capabilities=None,
-        error=None,
-    ):
-        """
-        Updates the context
-        :type transfer_session: TransferSession|None
-        :type sync_filter Filter|None
-        :type is_push: bool
-        :type stage: str|None
-        :type stage_status: str|None
-        :type capabilities: str[]|None
-        :type error: BaseException|None
-        """
-        if transfer_session and self.transfer_session:
-            raise MorangoContextUpdateError("Transfer session already exists")
-        elif (
-            transfer_session
-            and self.sync_session
-            and transfer_session.sync_session_id != self.sync_session.id
-        ):
-            raise MorangoContextUpdateError("Sync session mismatch")
-
-        if sync_filter and self.filter:
-            raise MorangoContextUpdateError("Filter already exists")
-
-        if is_push is not None and self.is_push is not None:
-            raise MorangoContextUpdateError("Push/pull method already exists")
-
-        self.transfer_session = transfer_session or self.transfer_session
-        self.filter = sync_filter or self.filter
-        self.is_push = is_push if is_push is not None else self.is_push
-        self.capabilities = set(capabilities or self.capabilities) & CAPABILITIES
-        self.update_state(stage=stage, stage_status=stage_status)
-        self.error = error or self.error
-
-        # if transfer session was passed in, that takes precedence
-        if transfer_session:
-            self.sync_session = transfer_session.sync_session
-            self.is_push = transfer_session.push
-            if transfer_session.filter:
-                self.filter = transfer_session.get_filter()
+from contextlib import contextmanager
 
-    @property
-    def is_pull(self):
-        """
-        :rtype: bool
-        """
-        return not self.is_push
+from morango.models.core import Buffer
+from morango.models.core import RecordMaxCounter
+from morango.models.core import RecordMaxCounterBuffer
+from morango.models.core import Store
 
-    @property
-    def stage(self):
-        """
-        The stage of the transfer context
-        :return: A transfer_stages.* constant
-        :rtype: str
-        """
-        raise NotImplementedError("Context `stage` getter is missing")
 
-    @property
-    def stage_status(self):
-        """
-        The status of the transfer context's stage
-        :return: A transfer_statuses.* constant
-        :rtype: str
-        """
-        raise NotImplementedError("Context `stage_status` getter is missing")
+class BaseSQLWrapper(object):
+    create_temporary_table_template = "CREATE TEMP TABLE {name} ({fields})"
 
-    def update_state(self, stage=None, stage_status=None):
-        """
-        Updates the stage state
-        :type stage: transfer_stages.*|None
-        :type stage_status: transfer_statuses.*|None
-        """
-        raise NotImplementedError("Context `update_state` method is missing")
+    def __init__(self, connection):
+        self.connection = connection
 
-    def __getstate__(self):
-        """Return dict of simplified data for serialization"""
-        return dict(
-            sync_session_id=self.sync_session.id if self.sync_session else None,
-            transfer_session_id=(
-                self.transfer_session.id if self.transfer_session else None
-            ),
-            filter=str(self.filter),
-            is_push=self.is_push,
-            stage=self.stage,
-            stage_status=self.stage_status,
-            capabilities=self.capabilities,
-            error=self.error,
+    def _is_transaction_isolation_error(self, error):
+        """
+        Determine if an error is related to transaction isolation
+        :param error: An exception
+        :return: A bool whether the error is a transaction isolation error
+        """
+        return False
+
+    @contextmanager
+    def _set_transaction_repeatable_read(self):
+        """Set the current transaction isolation level"""
+        yield
+
+    def _create_placeholder_list(self, fields, db_values):
+        # number of rows to update
+        num_of_rows = len(db_values) // len(fields)
+        # create '%s' placeholders for a single row
+        placeholder_tuple = tuple(["%s" for _ in range(len(fields))])
+        # create list of the '%s' tuple placeholders based on number of rows to update
+        return [str(placeholder_tuple) for _ in range(num_of_rows)]
+
+    def _bulk_full_record_upsert(self, cursor, table_name, fields, db_values):
+        raise NotImplementedError("Subclass must implement this method.")
+
+    def _bulk_insert(self, cursor, table_name, fields, db_values):
+        placeholder_str = ", ".join(
+            self._create_placeholder_list(fields, db_values)
+        ).replace("'", "")
+        fields_str = str(tuple(str(f.attname) for f in fields)).replace("'", "")
+        insert = """
+            INSERT INTO {table_name} {fields}
+            VALUES {placeholder_str}
+        """.format(
+            table_name=table_name, fields=fields_str, placeholder_str=placeholder_str
         )
+        cursor.execute(insert, db_values)
 
-    def __setstate__(self, state):
-        """Re-apply dict state after serialization"""
-        sync_session_id = state.get("sync_session_id", None)
-        if sync_session_id is not None:
-            self.sync_session = SyncSession.objects.get(pk=sync_session_id)
-
-        transfer_session_id = state.get("transfer_session_id", None)
-        if transfer_session_id is not None:
-            self.transfer_session = TransferSession.objects.get(pk=transfer_session_id)
-            if self.sync_session is None:
-                self.sync_session = self.transfer_session.sync_session
-
-        sync_filter = state.get("filter", None)
-        if sync_filter is not None:
-            self.filter = Filter(sync_filter)
-
-        self.is_push = state.get("is_push", None)
-        self.capabilities = state.get("capabilities", None)
-
-        stage = state.get("stage", None)
-        stage_status = state.get("stage_status", None)
-        self.update_state(stage=stage, stage_status=stage_status)
-        self.error = state.get("error", None)
-
-
-class LocalSessionContext(SessionContext):
-    """
-    Class that holds the context for operating on a transfer locally
-    """
-
-    __slots__ = (
-        "request",
-        "is_server",
-    )
+    def _bulk_update(self, cursor, table_name, fields, db_values):
+        raise NotImplementedError("Subclass must implement this method.")
 
-    def __init__(self, request=None, **kwargs):
-        """
-        :param request: If acting as the server, it should pass in the request, but the request
-            is not serialized into context. See `is_server` prop for determining if request was
-            passed in.
-        :type request: django.http.request.HttpRequest
-        """
-        capabilities = kwargs.pop("capabilities", [])
-        if request is not None:
-            capabilities = parse_capabilities_from_server_request(request)
-
-        super(LocalSessionContext, self).__init__(capabilities=capabilities, **kwargs)
-        self.request = request
-        self.is_server = request is not None
+    def _dequeuing_delete_rmcb_records(self, cursor, transfersession_id):
+        # delete all RMCBs which are a reverse FF (store version newer than buffer version)
+        delete_rmcb_records = """DELETE FROM {rmcb}
+                                 WHERE model_uuid IN
+                                 (SELECT rmcb.model_uuid FROM {store} as store, {buffer} as buffer, {rmc} as rmc, {rmcb} as rmcb
+                                 /*Scope to a single record*/
+                                 WHERE store.id = buffer.model_uuid
+                                 AND  store.id = rmc.store_model_id
+                                 AND  store.id = rmcb.model_uuid
+                                 /*Checks whether LSB of buffer or less is in RMC of store*/
+                                 AND buffer.last_saved_instance = rmc.instance_id
+                                 AND buffer.last_saved_counter <= rmc.counter
+                                 AND rmcb.transfer_session_id = '{transfer_session_id}'
+                                 AND buffer.transfer_session_id = '{transfer_session_id}')
+                                  """.format(
+            buffer=Buffer._meta.db_table,
+            store=Store._meta.db_table,
+            rmc=RecordMaxCounter._meta.db_table,
+            rmcb=RecordMaxCounterBuffer._meta.db_table,
+            transfer_session_id=transfersession_id,
+        )
 
-    @property
-    def _has_transfer_session(self):
-        """
-        :rtype: bool
-        """
-        return getattr(self, "transfer_session", None) is not None
+        cursor.execute(delete_rmcb_records)
 
-    @property
-    def stage(self):
-        """
-        :return: A transfer_stage.* constant
-        """
-        stage = transfer_stages.INITIALIZING
-        if self._has_transfer_session:
-            stage = self.transfer_session.transfer_stage or stage
-        return stage
+    def _dequeuing_delete_buffered_records(self, cursor, transfersession_id):
+        # delete all buffer records which are a reverse FF (store version newer than buffer version)
+        delete_buffered_records = """DELETE FROM {buffer}
+                                     WHERE model_uuid in
+                                     (SELECT buffer.model_uuid FROM {store} as store, {buffer} as buffer, {rmc} as rmc
+                                     /*Scope to a single record*/
+                                     WHERE store.id = buffer.model_uuid
+                                     AND rmc.store_model_id = buffer.model_uuid
+                                     /*Checks whether LSB of buffer or less is in RMC of store*/
+                                     AND buffer.last_saved_instance = rmc.instance_id
+                                     AND buffer.last_saved_counter <= rmc.counter
+                                     AND buffer.transfer_session_id = '{transfer_session_id}')
+                                  """.format(
+            buffer=Buffer._meta.db_table,
+            store=Store._meta.db_table,
+            rmc=RecordMaxCounter._meta.db_table,
+            transfer_session_id=transfersession_id,
+        )
+        cursor.execute(delete_buffered_records)
 
-    @property
-    def stage_status(self):
-        """
-        :return: A transfer_statuses.* constant
-        """
-        stage_status = transfer_statuses.PENDING
-        if self._has_transfer_session:
-            stage_status = self.transfer_session.transfer_stage_status or stage_status
-        return stage_status
+    def _dequeuing_merge_conflict_rmcb(self, cursor, transfersession_id):
+        raise NotImplementedError("Subclass must implement this method.")
 
-    @property
-    def is_receiver(self):
-        """
-        Whether or not the context indicates that the current local instance is receiving data,
-        which means either:
-            - A server context and a push transfer, or
-            - A client context and a pull transfer
-        :return: bool
-        """
-        return self.is_push == self.is_server
+    def _dequeuing_merge_conflict_buffer(self, cursor, current_id, transfersession_id):
+        raise NotImplementedError("Subclass must implement this method.")
 
-    @property
-    def is_producer(self):
-        """
-        The opposite of `is_receiver`, meaning either:
-            - A server context and a pull transfer, or
-            - A client context and a push transfer
-        :return: bool
-        """
-        return not self.is_receiver
+    def _dequeuing_update_rmcs_last_saved_by(
+        self, cursor, current_id, transfersession_id
+    ):
+        raise NotImplementedError("Subclass must implement this method.")
 
-    def update_state(self, stage=None, stage_status=None):
-        """
-        Passes through updating state to `TransferSession`, refreshing it from the DB in case it
-        has changed during operation
+    def _dequeuing_delete_mc_buffer(self, cursor, transfersession_id):
+        # delete records with merge conflicts from buffer
+        delete_mc_buffer = """DELETE FROM {buffer}
+                                    WHERE EXISTS
+                                    (SELECT 1 FROM {store} AS store, {buffer} AS buffer
+                                    /*Scope to a single record.*/
+                                    WHERE store.id = {buffer}.model_uuid
+                                    AND {buffer}.transfer_session_id = '{transfer_session_id}'
+                                    /*Exclude fast-forwards*/
+                                    AND NOT EXISTS (SELECT 1 FROM {rmcb} AS rmcb WHERE store.id = rmcb.model_uuid
+                                                                                  AND store.last_saved_instance = rmcb.instance_id
+                                                                                  AND store.last_saved_counter <= rmcb.counter
+                                                                                  AND rmcb.transfer_session_id = '{transfer_session_id}'))
+                               """.format(
+            buffer=Buffer._meta.db_table,
+            store=Store._meta.db_table,
+            rmcb=RecordMaxCounterBuffer._meta.db_table,
+            transfer_session_id=transfersession_id,
+        )
+        cursor.execute(delete_mc_buffer)
 
-        :param stage: Target stage for update
-        :param stage_status: Target status for update
-        """
-        if self._has_transfer_session:
-            self.transfer_session.refresh_from_db()
-            self.transfer_session.update_state(stage=stage, stage_status=stage_status)
-
-    def __getstate__(self):
-        """Return dict of simplified data for serialization"""
-        state = super(LocalSessionContext, self).__getstate__()
-        state.update(is_server=self.is_server)
-        return state
-
-    def __setstate__(self, state):
-        """Re-apply dict state after serialization"""
-        self.is_server = state.pop("is_server", False)
-        super(LocalSessionContext, self).__setstate__(state)
-
-
-class NetworkSessionContext(SessionContext):
-    """
-    Class that holds the context for operating on a transfer remotely through network connection
-    """
+    def _dequeuing_delete_mc_rmcb(self, cursor, transfersession_id):
+        # delete rmcb records with merge conflicts
+        delete_mc_rmc = """DELETE FROM {rmcb}
+                                    WHERE EXISTS
+                                    (SELECT 1 FROM {store} AS store, {rmc} AS rmc
+                                    /*Scope to a single record.*/
+                                    WHERE store.id = {rmcb}.model_uuid
+                                    AND store.id = rmc.store_model_id
+                                    /*Where buffer rmc is greater than store rmc*/
+                                    AND {rmcb}.instance_id = rmc.instance_id
+                                    AND {rmcb}.transfer_session_id = '{transfer_session_id}'
+                                    /*Exclude fast fast-forwards*/
+                                    AND NOT EXISTS (SELECT 1 FROM {rmcb} AS rmcb2 WHERE store.id = rmcb2.model_uuid
+                                                                                  AND store.last_saved_instance = rmcb2.instance_id
+                                                                                  AND store.last_saved_counter <= rmcb2.counter
+                                                                                  AND rmcb2.transfer_session_id = '{transfer_session_id}'))
+                               """.format(
+            store=Store._meta.db_table,
+            rmc=RecordMaxCounter._meta.db_table,
+            rmcb=RecordMaxCounterBuffer._meta.db_table,
+            transfer_session_id=transfersession_id,
+        )
+        cursor.execute(delete_mc_rmc)
 
-    __slots__ = ("connection", "_stage", "_stage_status")
+    def _dequeuing_insert_remaining_buffer(self, cursor, transfersession_id):
+        raise NotImplementedError("Subclass must implement this method.")
 
-    def __init__(self, connection, **kwargs):
-        """
-        :param connection: The sync client connection that allows operations to execute API calls
-            against the remote Morango server instance
-        :type connection: NetworkSyncConnection
-        """
-        self.connection = connection
-        super(NetworkSessionContext, self).__init__(
-            capabilities=self.connection.server_info.get("capabilities", []), **kwargs
+    def _dequeuing_insert_remaining_rmcb(self, cursor, transfersession_id):
+        raise NotImplementedError("Subclass must implement this method.")
+
+    def _dequeuing_delete_remaining_rmcb(self, cursor, transfersession_id):
+        # delete the remaining rmcb for this transfer session
+        delete_remaining_rmcb = """
+                                DELETE FROM {rmcb}
+                                WHERE {rmcb}.transfer_session_id = '{transfer_session_id}'
+                                """.format(
+            rmcb=RecordMaxCounterBuffer._meta.db_table,
+            transfer_session_id=transfersession_id,
         )
 
-        # since this is network context, keep local reference to state vars
-        self._stage = transfer_stages.INITIALIZING
-        self._stage_status = transfer_statuses.PENDING
+        cursor.execute(delete_remaining_rmcb)
 
-    @property
-    def stage(self):
+    def _dequeuing_delete_remaining_buffer(self, cursor, transfersession_id):
+        # delete the remaining buffer for this transfer session
+        delete_remaining_buffer = """
+                                  DELETE FROM {buffer}
+                                  WHERE {buffer}.transfer_session_id = '{transfer_session_id}'
+                                  """.format(
+            buffer=Buffer._meta.db_table, transfer_session_id=transfersession_id
+        )
+        cursor.execute(delete_remaining_buffer)
+
+    def _create_temporary_table(self, cursor, name, field_sqls, fields_params):
         """
-        :return: A transfer_stage.* constant
+        :param cursor: The database connection cursor
+        :param name: The str name of the temp table
+        :param field_sqls: A list of SQL strings representing the fields
+        :param fields_params: A list of SQL parameters if necessary for the fields SQL
         """
-        return self._stage
+        sql = self.create_temporary_table_template.format(
+            name=name, fields=", ".join(field_sqls)
+        )
+        cursor.execute(sql, fields_params)
 
-    @property
-    def stage_status(self):
+    def _lock_all_partitions(self, shared=False):
         """
-        :return: A transfer_statuses.* constant
+        Execute a lock within the database for all partitions, if the backend supports it. The lock
+        should block until acquired
+
+        :param shared: Whether or not the lock is exclusive or shared
         """
-        return self._stage_status
+        pass
 
-    def update_state(self, stage=None, stage_status=None):
+    def _lock_partition(self, partition, shared=False):
         """
-        :param stage: Target stage for update
-        :param stage_status: Target status for update
+        Execute a lock within the database for a specific partition, if the database supports it.
+        The lock should block until acquired
+
+        :param partition: The partition prefix string to lock
+        :param shared: Whether or not the lock is exclusive or shared
         """
-        self._stage = stage or self._stage
-        self._stage_status = stage_status or self._stage_status
+        pass
```

### Comparing `morango-0.6.9/morango/sync/operations.py` & `morango-0.7.0/morango/sync/operations.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,73 +1,66 @@
 import functools
 import itertools
 import json
 import logging
 import uuid
+from collections import defaultdict
+from contextlib import contextmanager
 
 from django.core import exceptions
 from django.core.serializers.json import DjangoJSONEncoder
 from django.db import connection
-from django.db import connections
-from django.db import router
 from django.db import transaction
+from django.db.models import CharField
 from django.db.models import Q
 from django.db.models import signals
+from django.db.utils import OperationalError
 from django.utils import timezone
 from rest_framework.exceptions import ValidationError
 
 from morango.api.serializers import BufferSerializer
-from morango.constants.capabilities import ASYNC_OPERATIONS
-from morango.constants.capabilities import FSIC_V2_FORMAT
 from morango.constants import transfer_stages
 from morango.constants import transfer_statuses
-from morango.errors import MorangoResumeSyncError
-from morango.errors import MorangoLimitExceeded
+from morango.constants.capabilities import ASYNC_OPERATIONS
+from morango.constants.capabilities import FSIC_V2_FORMAT
+from morango.errors import MorangoDatabaseError
 from morango.errors import MorangoInvalidFSICPartition
+from morango.errors import MorangoLimitExceeded
+from morango.errors import MorangoResumeSyncError
 from morango.errors import MorangoSkipOperation
 from morango.models.certificates import Filter
 from morango.models.core import Buffer
 from morango.models.core import DatabaseMaxCounter
 from morango.models.core import DeletedModels
 from morango.models.core import HardDeletedModels
 from morango.models.core import InstanceIDModel
 from morango.models.core import RecordMaxCounter
 from morango.models.core import RecordMaxCounterBuffer
 from morango.models.core import Store
 from morango.models.core import TransferSession
-from morango.models.fsic_utils import (
-    calculate_directional_fsic_diff,
-    calculate_directional_fsic_diff_v2,
-    chunk_fsic_v2,
-    expand_fsic_for_use,
-)
+from morango.models.core import UUIDField
+from morango.models.fsic_utils import calculate_directional_fsic_diff
+from morango.models.fsic_utils import calculate_directional_fsic_diff_v2
+from morango.models.fsic_utils import chunk_fsic_v2
+from morango.models.fsic_utils import expand_fsic_for_use
 from morango.registry import syncable_models
 from morango.sync.backends.utils import load_backend
+from morango.sync.backends.utils import TemporaryTable
 from morango.sync.context import LocalSessionContext
 from morango.sync.context import NetworkSessionContext
+from morango.sync.utils import lock_partitions
 from morango.sync.utils import mute_signals
 from morango.sync.utils import validate_and_create_buffer_data
 from morango.utils import _assert
 from morango.utils import SETTINGS
 
 
 logger = logging.getLogger(__name__)
 
-DBBackend = load_backend(connection).SQLWrapper()
-
-# if postgres, get serializable db connection
-db_name = router.db_for_write(Store)
-USING_DB = db_name
-if "postgresql" in transaction.get_connection(USING_DB).vendor:
-    USING_DB = db_name + "-serializable"
-    _assert(
-        USING_DB in connections,
-        "Please add a `default-serializable` database connection in your django settings file, \
-            which copies all the configuration settings of the `default` db connection",
-    )
+DBBackend = load_backend(connection)
 
 SQL_UNION_MAX = 500
 
 
 class OperationLogger(object):
     def __init__(self, start_msg, end_msg):
         self.start_msg = start_msg
@@ -95,29 +88,55 @@
     for f in model._meta.concrete_fields:
         if f.related_model:
             if issubclass(model, f.related_model):
                 return f.attname
     return None
 
 
+@contextmanager
+def _begin_transaction(sync_filter, isolated=False, shared_lock=False):
+    """
+    Starts a transaction, sets the transaction isolation level to repeatable read, and locks
+    affected partitions
+
+    :param sync_filter: The filter for filtering applicable records of the sync
+    :type sync_filter: morango.models.certificates.Filter|None
+    :param isolated: Whether to alter the transaction isolation to repeatable-read
+    :type isolated: bool
+    :param shared_lock: Whether the advisory lock should be exclusive or shared
+    :type shared_lock: bool
+    """
+    if isolated:
+        # when isolation is requested, we modify the transaction isolation of the connection for the
+        # duration of the transaction
+        with DBBackend._set_transaction_repeatable_read():
+            with transaction.atomic(savepoint=False):
+                lock_partitions(DBBackend, sync_filter=sync_filter, shared=shared_lock)
+                yield
+    else:
+        with transaction.atomic():
+            lock_partitions(DBBackend, sync_filter=sync_filter, shared=shared_lock)
+            yield
+
+
 def _serialize_into_store(profile, filter=None):
     """
     Takes data from app layer and serializes the models into the store.
 
     ALGORITHM: On a per syncable model basis, we iterate through each class model and we go through 2 possible cases:
 
     1. If there is a store record pertaining to that app model, we update the serialized store record with
     the latest changes from the model's fields. We also update the counter's based on this device's current Instance ID.
     2. If there is no store record for this app model, we proceed to create an in memory store model and append to a list to be
     bulk created on a per class model basis.
     """
     # ensure that we write and retrieve the counter in one go for consistency
     current_id = InstanceIDModel.get_current_instance_and_increment_counter()
 
-    with transaction.atomic(using=USING_DB):
+    with _begin_transaction(filter, isolated=True):
         # create Q objects for filtering by prefixes
         prefix_condition = None
         if filter:
             prefix_condition = functools.reduce(
                 lambda x, y: x | y,
                 [Q(_morango_partition__startswith=prefix) for prefix in filter],
             )
@@ -258,32 +277,184 @@
                 DatabaseMaxCounter.objects.update_or_create(
                     instance_id=current_id.id,
                     partition=f,
                     defaults={"counter": current_id.counter},
                 )
 
 
+def _validate_missing_store_foreign_keys(from_model_name, to_model_name, temp_table):
+    """
+    Performs validation on a bulk set of foreign keys (FKs), given a temp table with two columns,
+    `from_pk` and `to_pk`, the primary key (PK) pair to validate. Any store record matching
+    `from_pk`, while missing a store record matching `to_pk`, will be updated with a deserialization
+    error and its PK returned within a list.
+
+    :param from_model_name: A str name of the model which has the FK, for logging purposes
+    :param to_model_name: A str name of the model referenced by the FK, for logging purposes
+    :param temp_table: A temp table object for querying against in the DB
+    :type temp_table: morango.sync.backends.utils.TemporaryTable
+    :return: A list of store PKs that have broken FKs
+    """
+    invalid_pks = []
+    select_sql = """
+        SELECT t.from_field, t.from_pk, t.to_pk
+        FROM {temp_table} t
+        WHERE NOT EXISTS (
+            SELECT 1
+            FROM {store} s
+            WHERE s.{pk_field} = t.to_pk
+        )
+    """.format(
+        temp_table=temp_table.sql_name,
+        store=Store._meta.db_table,
+        pk_field=Store._meta.pk.column,
+    )
+
+    store_deserialization_error = next(
+        f for f in Store._meta.fields if f.name == "deserialization_error"
+    )
+    store_update_fields = [Store._meta.pk, store_deserialization_error]
+
+    from_pk_field = temp_table.get_field("from_pk")
+    to_pk_field = temp_table.get_field("to_pk")
+    update_values = []
+    with connection.cursor() as c:
+        c.execute(select_sql)
+        for from_field, from_pk, to_pk in c.fetchall():
+            err = dict(
+                {
+                    from_field: "{to_model_name} instance with id '{to_pk}' does not exist".format(
+                        to_model_name=to_model_name,
+                        to_pk=to_pk_field.to_python(to_pk),
+                    )
+                }
+            )
+            logger.warning(
+                "Error deserializing instance of {from_model} with id {from_pk}: {err}".format(
+                    from_model=from_model_name,
+                    from_pk=from_pk,
+                    err=str(err),
+                )
+            )
+            update_values.extend([from_pk, str(err)])
+            invalid_pks.append(from_pk_field.to_python(from_pk))
+        if update_values:
+            # update Store with errors
+            DBBackend._bulk_update(
+                c, Store._meta.db_table, store_update_fields, update_values
+            )
+    return invalid_pks
+
+
+def _handle_deleted_store_foreign_keys(temp_table):
+    """
+    Handles store records with foreign key (FK) references to other deleted store records to prevent
+    their deserialization and update the `DeletedModels` and `HardDeletedModels` tracking, given a
+    temp table with two columns, `from_pk` and `to_pk`, the primary key (PK) pair
+    :param temp_table: A temp table object for querying against in the DB
+    :type temp_table: morango.sync.backends.utils.TemporaryTable
+    :return: A list of store PKs that have FKs to deleted records
+    """
+    select_sql = """
+        SELECT t.from_pk, s.profile, s.deleted, s.hard_deleted
+        FROM {temp_table} t
+            INNER JOIN {store} s ON s.{pk_field} = t.to_pk
+        WHERE s.deleted OR s.hard_deleted
+    """.format(
+        temp_table=temp_table.sql_name,
+        store=Store._meta.db_table,
+        pk_field=Store._meta.pk.column,
+    )
+
+    from_pk_field = temp_table.get_field("from_pk")
+    deleted_pks = []
+    deleted_values = []
+    hard_deleted_values = []
+    with connection.cursor() as c:
+        c.execute(select_sql)
+        # find all the store PKs which have FKs to deleted store PKs
+        for from_pk, profile, deleted, hard_deleted in c.fetchall():
+            if deleted or hard_deleted:
+                deleted_values.extend([from_pk, profile])
+            if hard_deleted:
+                hard_deleted_values.extend([from_pk, profile])
+            deleted_pks.append(from_pk_field.to_python(from_pk))
+        # update deleted tracking models
+        if deleted_values:
+            DBBackend._bulk_full_record_upsert(
+                c,
+                DeletedModels._meta.db_table,
+                DeletedModels._meta.fields,
+                deleted_values,
+            )
+        if hard_deleted_values:
+            DBBackend._bulk_full_record_upsert(
+                c,
+                HardDeletedModels._meta.db_table,
+                HardDeletedModels._meta.fields,
+                hard_deleted_values,
+            )
+    return deleted_pks
+
+
+def _validate_store_foreign_keys(from_model_name, fk_references):
+    """
+    Validates the foreign key (FK) references of a model whose name is `from_model_name`, through
+    bulk processing using a temporary table within the database for holding the FK references
+
+    :param from_model_name: A str name of the model which has the FKs, for logging purposes
+    :param fk_references: A dictionary of lists containing `morango.models.core.ForeignKeyReference`
+        keyed by the
+    :return: A tuple of two lists containing store PKs with broken FKs and FKs to deleted records
+    """
+    exclude_pks = []
+    deleted_pks = []
+
+    for to_model_name, to_fk_references in fk_references.items():
+        with TemporaryTable(
+            connection,
+            "fks",
+            from_field=CharField(max_length=255),
+            from_pk=UUIDField(),
+            to_pk=UUIDField(),
+        ) as temp_table:
+            # insert all the FK references into a temp table in the database
+            temp_table.bulk_insert([fks._asdict() for fks in to_fk_references])
+            # now pass the temp table to validate against broken FKs
+            exclude_pks.extend(
+                _validate_missing_store_foreign_keys(
+                    from_model_name, to_model_name, temp_table
+                )
+            )
+            # find any FKs referencing deleted records
+            deleted_pks.extend(_handle_deleted_store_foreign_keys(temp_table))
+
+    return exclude_pks, deleted_pks
+
+
 def _deserialize_from_store(profile, skip_erroring=False, filter=None):
     """
     Takes data from the store and integrates into the application.
 
     ALGORITHM: On a per syncable model basis, we iterate through each class model and we go through 2 possible cases:
 
     1. For class models that have a self referential foreign key, we iterate down the dependency tree deserializing model by model.
     2. On a per app model basis, we append the field values to a single list, and do a single bulk insert/replace query.
 
     If a model fails to deserialize/validate, we exclude it from being marked as clean in the store.
     """
 
     fk_cache = {}
-    with transaction.atomic(using=USING_DB):
-        excluded_list = []
+    excluded_list = []
+    deleted_list = []
+
+    with _begin_transaction(filter, isolated=True):
         # iterate through classes which are in foreign key dependency order
         for model in syncable_models.get_models(profile):
-
+            deferred_fks = defaultdict(list)
             store_models = Store.objects.filter(profile=profile)
 
             model_condition = Q(model_name=model.morango_model_name)
             for klass in model.morango_model_dependencies:
                 model_condition |= Q(model_name=klass.morango_model_name)
 
             store_models = store_models.filter(model_condition)
@@ -309,27 +480,30 @@
                     .filter(Q(_self_ref_fk__in=clean_parents) | Q(_self_ref_fk=""))
                 )
 
                 # keep iterating until size of dirty_children is 0
                 while len(dirty_children) > 0:
                     for store_model in dirty_children:
                         try:
-                            app_model = store_model._deserialize_store_model(fk_cache)
+                            app_model, _ = store_model._deserialize_store_model(
+                                fk_cache
+                            )
                             if app_model:
                                 with mute_signals(signals.pre_save, signals.post_save):
                                     app_model.save(update_dirty_bit_to=False)
                             # we update a store model after we have deserialized it to be able to mark it as a clean parent
                             store_model.dirty_bit = False
                             store_model.deserialization_error = ""
                             store_model.save(
                                 update_fields=["dirty_bit", "deserialization_error"]
                             )
                         except (
                             exceptions.ValidationError,
                             exceptions.ObjectDoesNotExist,
+                            ValueError,
                         ) as e:
                             excluded_list.append(store_model.id)
                             # if the app model did not validate, we leave the store dirty bit set, but mark the error
                             store_model.deserialization_error = str(e)
                             store_model.save(update_fields=["deserialization_error"])
 
                     # update lists with new clean parents and dirty children
@@ -351,354 +525,397 @@
                 store_models.filter(dirty_bit=True).exclude(
                     _self_ref_fk__in=all_parents
                 ).exclude(id__in=excluded_list).update(
                     deserialization_error="Parent does not exist in Store; could not deserialize."
                 )
 
             else:
-                # array for holding db values from the fields of each model for this class
-                db_values = []
+                # collect all initially valid app models
+                app_models = []
                 fields = model._meta.fields
                 for store_model in store_models.filter(dirty_bit=True):
                     try:
-                        app_model = store_model._deserialize_store_model(fk_cache)
-                        # if the model was not deleted add its field values to the list
+                        (
+                            app_model,
+                            model_deferred_fks,
+                        ) = store_model._deserialize_store_model(
+                            fk_cache, defer_fks=True
+                        )
                         if app_model:
-                            for f in fields:
-                                value = getattr(app_model, f.attname)
-                                db_value = f.get_db_prep_value(value, connection)
-                                db_values.append(db_value)
+                            app_models.append(app_model)
+                        for fk_model, fk_refs in model_deferred_fks.items():
+                            # validate that the FK references aren't to anything already in the
+                            # excluded list, which should only contain models which failed to
+                            # deserialize for reasons other than broken FKs at this point
+                            for fk_ref in fk_refs:
+                                if fk_ref.to_pk in excluded_list:
+                                    raise exceptions.ValidationError(
+                                        "{} with id {} failed to deserialize".format(
+                                            fk_model, fk_ref.to_pk
+                                        )
+                                    )
+                            deferred_fks[fk_model].extend(fk_refs)
                     except (
                         exceptions.ValidationError,
                         exceptions.ObjectDoesNotExist,
+                        ValueError,
                     ) as e:
                         # if the app model did not validate, we leave the store dirty bit set
                         excluded_list.append(store_model.id)
                         store_model.deserialization_error = str(e)
                         store_model.save(update_fields=["deserialization_error"])
 
+                # validate app model FKs
+                model_excluded_pks, model_deleted_pks = _validate_store_foreign_keys(
+                    model.__name__, deferred_fks
+                )
+                excluded_list.extend(model_excluded_pks)
+                deleted_list.extend(model_deleted_pks)
+
+                # array for holding db values from the fields of each model for this class
+                db_values = []
+                for app_model in app_models:
+                    if (
+                        app_model.pk not in excluded_list
+                        and app_model.pk not in deleted_list
+                    ):
+                        # handle any errors that might come from `get_db_prep_value`
+                        try:
+                            new_db_values = []
+                            for f in fields:
+                                value = getattr(app_model, f.attname)
+                                db_value = f.get_db_prep_value(value, connection)
+                                new_db_values.append(db_value)
+                            db_values += new_db_values
+                        except ValueError as e:
+                            excluded_list.append(app_model.pk)
+                            store_model = store_models.get(pk=app_model.pk)
+                            store_model.deserialization_error = str(e)
+                            store_model.save(update_fields=["deserialization_error"])
+
                 if db_values:
-                    # number of rows to update
-                    num_of_rows = len(db_values) // len(fields)
-                    # create '%s' placeholders for a single row
-                    placeholder_tuple = tuple(["%s" for _ in range(len(fields))])
-                    # create list of the '%s' tuple placeholders based on number of rows to update
-                    placeholder_list = [
-                        str(placeholder_tuple) for _ in range(num_of_rows)
-                    ]
                     with connection.cursor() as cursor:
-                        DBBackend._bulk_insert_into_app_models(
+                        DBBackend._bulk_full_record_upsert(
                             cursor,
                             model._meta.db_table,
                             fields,
                             db_values,
-                            placeholder_list,
                         )
 
                 # clear dirty bit for all store records for this model/profile except for rows that did not validate
                 store_models.exclude(id__in=excluded_list).filter(
                     dirty_bit=True
                 ).update(dirty_bit=False)
 
 
-@transaction.atomic(using=USING_DB)
 def _queue_into_buffer_v1(transfersession):
     """
     Takes a chunk of data from the store to be put into the buffer to be sent to another morango instance. This is the legacy
     code to handle backwards compatibility with older versions of Morango, with the v1 version of the FSIC data structure.
 
     ALGORITHM: We do Filter Specific Instance Counter arithmetic to get our newest data compared to the server's older data.
     We use raw sql queries to place data in the buffer and the record max counter buffer, which matches the conditions of the FSIC,
     as well as the partition for the data we are syncing.
     """
     filter_prefixes = Filter(transfersession.filter)
-    server_fsic = json.loads(transfersession.server_fsic)
-    client_fsic = json.loads(transfersession.client_fsic)
+    with _begin_transaction(filter_prefixes, shared_lock=True):
+        server_fsic = json.loads(transfersession.server_fsic)
+        client_fsic = json.loads(transfersession.client_fsic)
 
-    if transfersession.push:
-        fsics = calculate_directional_fsic_diff(client_fsic, server_fsic)
-    else:
-        fsics = calculate_directional_fsic_diff(server_fsic, client_fsic)
+        if transfersession.push:
+            fsics = calculate_directional_fsic_diff(client_fsic, server_fsic)
+        else:
+            fsics = calculate_directional_fsic_diff(server_fsic, client_fsic)
 
-    # if fsics are identical or receiving end has newer data, then there is nothing to queue
-    if not fsics:
-        return
-
-    profile_condition = ["profile = '{}'".format(transfersession.sync_session.profile)]
-    partition_conditions = []
-    # create condition for filtering by partitions
-    for prefix in filter_prefixes:
-        partition_conditions += ["partition LIKE '{}%'".format(prefix)]
-    if filter_prefixes:
-        partition_conditions = [_join_with_logical_operator(partition_conditions, "OR")]
-
-    chunk_size = 200
-    fsics = list(fsics.items())
-    fsics_len = len(fsics)
-    fsics_limit = chunk_size * SQL_UNION_MAX
-
-    if fsics_len >= fsics_limit:
-        raise MorangoLimitExceeded(
-            "Limit of {limit} instance counters exceeded with {actual}".format(
-                limit=fsics_limit, actual=fsics_len
-            )
-        )
+        # if fsics are identical or receiving end has newer data, then there is nothing to queue
+        if not fsics:
+            return
 
-    # chunk fsics creating multiple SQL selects which will be unioned before insert
-    i = 0
-    chunk = fsics[:chunk_size]
-    select_buffers = []
-
-    while chunk:
-        # create condition for all push FSICs where instance_ids are equal, but internal counters are higher than
-        # FSICs counters
-        last_saved_by_conditions = [
-            "(last_saved_instance = '{0}' AND last_saved_counter > {1})".format(
-                instance, counter
-            )
-            for instance, counter in chunk
+        profile_condition = [
+            "profile = '{}'".format(transfersession.sync_session.profile)
         ]
-        if last_saved_by_conditions:
-            last_saved_by_conditions = [
-                _join_with_logical_operator(last_saved_by_conditions, "OR")
+        partition_conditions = []
+        # create condition for filtering by partitions
+        for prefix in filter_prefixes:
+            partition_conditions += ["partition LIKE '{}%'".format(prefix)]
+        if filter_prefixes:
+            partition_conditions = [
+                _join_with_logical_operator(partition_conditions, "OR")
             ]
 
-        # combine conditions and filter by profile
-        where_condition = _join_with_logical_operator(
-            profile_condition + last_saved_by_conditions + partition_conditions, "AND"
-        )
+        chunk_size = 200
+        fsics = list(fsics.items())
+        fsics_len = len(fsics)
+        fsics_limit = chunk_size * SQL_UNION_MAX
+
+        if fsics_len >= fsics_limit:
+            raise MorangoLimitExceeded(
+                "Limit of {limit} instance counters exceeded with {actual}".format(
+                    limit=fsics_limit, actual=fsics_len
+                )
+            )
 
-        # execute raw sql to take all records that match condition, to be put into buffer for transfer
-        select_buffers.append(
-            """SELECT
-                   id, serialized, deleted, last_saved_instance, last_saved_counter, hard_deleted, model_name, profile,
-                   partition, source_id, conflicting_serialized_data,
-                   CAST ('{transfer_session_id}' AS {transfer_session_id_type}), _self_ref_fk
-               FROM {store} WHERE {condition}
-            """.format(
-                transfer_session_id=transfersession.id,
-                transfer_session_id_type=TransferSession._meta.pk.rel_db_type(
-                    connection
-                ),
-                condition=where_condition,
-                store=Store._meta.db_table,
+        # chunk fsics creating multiple SQL selects which will be unioned before insert
+        i = 0
+        chunk = fsics[:chunk_size]
+        select_buffers = []
+
+        while chunk:
+            # create condition for all push FSICs where instance_ids are equal, but internal counters are higher than
+            # FSICs counters
+            last_saved_by_conditions = [
+                "(last_saved_instance = '{0}' AND last_saved_counter > {1})".format(
+                    instance, counter
+                )
+                for instance, counter in chunk
+            ]
+            if last_saved_by_conditions:
+                last_saved_by_conditions = [
+                    _join_with_logical_operator(last_saved_by_conditions, "OR")
+                ]
+
+            # combine conditions and filter by profile
+            where_condition = _join_with_logical_operator(
+                profile_condition + last_saved_by_conditions + partition_conditions,
+                "AND",
             )
-        )
-        i += chunk_size
-        chunk = fsics[i : i + chunk_size]
 
-    # take all record max counters that are foreign keyed onto store models, which were queued into the buffer
-    select_rmc_buffer_query = """SELECT instance_id, counter, CAST ('{transfer_session_id}' AS {transfer_session_id_type}), store_model_id
-            FROM {record_max_counter} AS rmc
-            INNER JOIN {outgoing_buffer} AS buffer ON rmc.store_model_id = buffer.model_uuid
-            WHERE buffer.transfer_session_id = '{transfer_session_id}'
-        """.format(
-        transfer_session_id=transfersession.id,
-        transfer_session_id_type=TransferSession._meta.pk.rel_db_type(connection),
-        record_max_counter=RecordMaxCounter._meta.db_table,
-        outgoing_buffer=Buffer._meta.db_table,
-    )
+            # execute raw sql to take all records that match condition, to be put into buffer for transfer
+            select_buffers.append(
+                """SELECT
+                       id, serialized, deleted, last_saved_instance, last_saved_counter, hard_deleted, model_name, profile,
+                       partition, source_id, conflicting_serialized_data,
+                       CAST ('{transfer_session_id}' AS {transfer_session_id_type}), _self_ref_fk
+                   FROM {store} WHERE {condition}
+                """.format(
+                    transfer_session_id=transfersession.id,
+                    transfer_session_id_type=TransferSession._meta.pk.rel_db_type(
+                        connection
+                    ),
+                    condition=where_condition,
+                    store=Store._meta.db_table,
+                )
+            )
+            i += chunk_size
+            chunk = fsics[i : i + chunk_size]
 
-    with connection.cursor() as cursor:
-        cursor.execute(
-            """INSERT INTO {outgoing_buffer}
-               (model_uuid, serialized, deleted, last_saved_instance, last_saved_counter,
-               hard_deleted, model_name, profile, partition, source_id, conflicting_serialized_data,
-               transfer_session_id, _self_ref_fk)
-               {select}
+        # take all record max counters that are foreign keyed onto store models, which were queued into the buffer
+        select_rmc_buffer_query = """SELECT instance_id, counter, CAST ('{transfer_session_id}' AS {transfer_session_id_type}), store_model_id
+                FROM {record_max_counter} AS rmc
+                INNER JOIN {outgoing_buffer} AS buffer ON rmc.store_model_id = buffer.model_uuid
+                WHERE buffer.transfer_session_id = '{transfer_session_id}'
             """.format(
-                outgoing_buffer=Buffer._meta.db_table,
-                select=" UNION ".join(select_buffers),
-            )
+            transfer_session_id=transfersession.id,
+            transfer_session_id_type=TransferSession._meta.pk.rel_db_type(connection),
+            record_max_counter=RecordMaxCounter._meta.db_table,
+            outgoing_buffer=Buffer._meta.db_table,
         )
-        cursor.execute(
-            """INSERT INTO {outgoing_rmcb}
-               (instance_id, counter, transfer_session_id, model_uuid)
-               {select}
-            """.format(
-                outgoing_rmcb=RecordMaxCounterBuffer._meta.db_table,
-                select=select_rmc_buffer_query,
+
+        with connection.cursor() as cursor:
+            cursor.execute(
+                """INSERT INTO {outgoing_buffer}
+                   (model_uuid, serialized, deleted, last_saved_instance, last_saved_counter,
+                   hard_deleted, model_name, profile, partition, source_id, conflicting_serialized_data,
+                   transfer_session_id, _self_ref_fk)
+                   {select}
+                """.format(
+                    outgoing_buffer=Buffer._meta.db_table,
+                    select=" UNION ".join(select_buffers),
+                )
+            )
+            cursor.execute(
+                """INSERT INTO {outgoing_rmcb}
+                   (instance_id, counter, transfer_session_id, model_uuid)
+                   {select}
+                """.format(
+                    outgoing_rmcb=RecordMaxCounterBuffer._meta.db_table,
+                    select=select_rmc_buffer_query,
+                )
             )
-        )
 
 
-@transaction.atomic(using=USING_DB)
 def _queue_into_buffer_v2(transfersession, chunk_size=200):
     """
     Takes a chunk of data from the store to be put into the buffer to be sent to another morango instance.
 
     This version uses the new v2 FSIC format that is split out by partition, divided into sub partitions (the ones under the filter)
     and super partitions (prefixes of the sub partitions).
 
     ALGORITHM: We do Filter Specific Instance Counter arithmetic to get our newest data compared to the server's older data.
     We use raw sql queries to place data in the buffer and the record max counter buffer, which matches the conditions of the FSIC.
     """
     sync_filter = Filter(transfersession.filter)
-    server_fsic = json.loads(transfersession.server_fsic)
-    client_fsic = json.loads(transfersession.client_fsic)
+    with _begin_transaction(sync_filter, shared_lock=True):
+        server_fsic = json.loads(transfersession.server_fsic)
+        client_fsic = json.loads(transfersession.client_fsic)
+
+        assert "sub" in server_fsic
+        assert "super" in server_fsic
+        assert "sub" in client_fsic
+        assert "super" in client_fsic
+
+        # ensure that the partitions in the FSICs are under the current filter, before using them
+        for partition in itertools.chain(
+            server_fsic["sub"].keys(), client_fsic["sub"].keys()
+        ):
+            if partition not in sync_filter:
+                raise MorangoInvalidFSICPartition(
+                    "Partition '{}' is not in filter".format(partition)
+                )
 
-    assert "sub" in server_fsic
-    assert "super" in server_fsic
-    assert "sub" in client_fsic
-    assert "super" in client_fsic
-
-    # ensure that the partitions in the FSICs are under the current filter, before using them
-    for partition in itertools.chain(
-        server_fsic["sub"].keys(), client_fsic["sub"].keys()
-    ):
-        if partition not in sync_filter:
-            raise MorangoInvalidFSICPartition(
-                "Partition '{}' is not in filter".format(partition)
-            )
+        server_fsic = expand_fsic_for_use(server_fsic, sync_filter)
+        client_fsic = expand_fsic_for_use(client_fsic, sync_filter)
 
-    server_fsic = expand_fsic_for_use(server_fsic, sync_filter)
-    client_fsic = expand_fsic_for_use(client_fsic, sync_filter)
+        if transfersession.push:
+            fsics = calculate_directional_fsic_diff_v2(client_fsic, server_fsic)
+        else:
+            fsics = calculate_directional_fsic_diff_v2(server_fsic, client_fsic)
 
-    if transfersession.push:
-        fsics = calculate_directional_fsic_diff_v2(client_fsic, server_fsic)
-    else:
-        fsics = calculate_directional_fsic_diff_v2(server_fsic, client_fsic)
+        # if fsics are identical or receiving end has newer data, then there is nothing to queue
+        if not fsics:
+            return
 
-    # if fsics are identical or receiving end has newer data, then there is nothing to queue
-    if not fsics:
-        return
-
-    profile_condition = ["profile = '{}'".format(transfersession.sync_session.profile)]
-
-    fsics_len = sum(len(fsics[part]) for part in fsics) + len(fsics)
-    # subtract one because when partitions overflow chunks they add up to an extra item per chunk
-    fsics_limit = chunk_size * (SQL_UNION_MAX - 1)
-
-    if fsics_len >= fsics_limit:
-        raise MorangoLimitExceeded(
-            "Limit of {limit} instances + partitions exceeded with {actual}".format(
-                limit=fsics_limit, actual=fsics_len
+        profile_condition = [
+            "profile = '{}'".format(transfersession.sync_session.profile)
+        ]
+
+        fsics_len = sum(len(fsics[part]) for part in fsics) + len(fsics)
+        # subtract one because when partitions overflow chunks they add up to an extra item per chunk
+        fsics_limit = chunk_size * (SQL_UNION_MAX - 1)
+
+        if fsics_len >= fsics_limit:
+            raise MorangoLimitExceeded(
+                "Limit of {limit} instances + partitions exceeded with {actual}".format(
+                    limit=fsics_limit, actual=fsics_len
+                )
             )
-        )
 
-    # if needed, split the fsics into chunks
-    if fsics_len > chunk_size:
-        chunked_fsics = chunk_fsic_v2(fsics, chunk_size)
-    else:
-        chunked_fsics = [fsics]
+        # if needed, split the fsics into chunks
+        if fsics_len > chunk_size:
+            chunked_fsics = chunk_fsic_v2(fsics, chunk_size)
+        else:
+            chunked_fsics = [fsics]
 
-    select_buffers = []
+        select_buffers = []
 
-    for fsic_chunk in chunked_fsics:
+        for fsic_chunk in chunked_fsics:
 
-        # create condition for filtering by partitions
-        partition_conditions = []
-        for part, insts in fsic_chunk.items():
-            if not insts:
-                continue
-
-            partition_conditions.append(
-                "partition LIKE '{}%' AND (".format(part)
-                + _join_with_logical_operator(
-                    [
-                        "(last_saved_instance = '{}' AND last_saved_counter > {})".format(
-                            inst, counter
-                        )
-                        for inst, counter in insts.items()
-                    ],
-                    "OR",
+            # create condition for filtering by partitions
+            partition_conditions = []
+            for part, insts in fsic_chunk.items():
+                if not insts:
+                    continue
+
+                partition_conditions.append(
+                    "partition LIKE '{}%' AND (".format(part)
+                    + _join_with_logical_operator(
+                        [
+                            "(last_saved_instance = '{}' AND last_saved_counter > {})".format(
+                                inst, counter
+                            )
+                            for inst, counter in insts.items()
+                        ],
+                        "OR",
+                    )
+                    + ")"
                 )
-                + ")"
-            )
-
-        partition_conditions = [_join_with_logical_operator(partition_conditions, "OR")]
 
-        # combine conditions and filter by profile
-        where_condition = _join_with_logical_operator(
-            profile_condition + partition_conditions, "AND"
-        )
+            partition_conditions = [
+                _join_with_logical_operator(partition_conditions, "OR")
+            ]
 
-        # execute raw sql to take all records that match condition, to be put into buffer for transfer
-        select_buffers.append(
-            """SELECT
-                    id, serialized, deleted, last_saved_instance, last_saved_counter, hard_deleted, model_name, profile,
-                    partition, source_id, conflicting_serialized_data,
-                    CAST ('{transfer_session_id}' AS {transfer_session_id_type}), _self_ref_fk
-                FROM {store} WHERE {condition}
-            """.format(
-                transfer_session_id=transfersession.id,
-                transfer_session_id_type=TransferSession._meta.pk.rel_db_type(
-                    connection
-                ),
-                condition=where_condition,
-                store=Store._meta.db_table,
+            # combine conditions and filter by profile
+            where_condition = _join_with_logical_operator(
+                profile_condition + partition_conditions, "AND"
             )
-        )
 
-    # take all record max counters that are foreign keyed onto store models, which were queued into the buffer
-    select_rmc_buffer_query = """SELECT instance_id, counter, CAST ('{transfer_session_id}' AS {transfer_session_id_type}), store_model_id
-            FROM {record_max_counter} AS rmc
-            INNER JOIN {outgoing_buffer} AS buffer ON rmc.store_model_id = buffer.model_uuid
-            WHERE buffer.transfer_session_id = '{transfer_session_id}'
-        """.format(
-        transfer_session_id=transfersession.id,
-        transfer_session_id_type=TransferSession._meta.pk.rel_db_type(connection),
-        record_max_counter=RecordMaxCounter._meta.db_table,
-        outgoing_buffer=Buffer._meta.db_table,
-    )
+            # execute raw sql to take all records that match condition, to be put into buffer for transfer
+            select_buffers.append(
+                """SELECT
+                        id, serialized, deleted, last_saved_instance, last_saved_counter, hard_deleted, model_name, profile,
+                        partition, source_id, conflicting_serialized_data,
+                        CAST ('{transfer_session_id}' AS {transfer_session_id_type}), _self_ref_fk
+                    FROM {store} WHERE {condition}
+                """.format(
+                    transfer_session_id=transfersession.id,
+                    transfer_session_id_type=TransferSession._meta.pk.rel_db_type(
+                        connection
+                    ),
+                    condition=where_condition,
+                    store=Store._meta.db_table,
+                )
+            )
 
-    with connection.cursor() as cursor:
-        cursor.execute(
-            """INSERT INTO {outgoing_buffer}
-               (model_uuid, serialized, deleted, last_saved_instance, last_saved_counter,
-               hard_deleted, model_name, profile, partition, source_id, conflicting_serialized_data,
-               transfer_session_id, _self_ref_fk)
-               {select}
+        # take all record max counters that are foreign keyed onto store models, which were queued into the buffer
+        select_rmc_buffer_query = """SELECT instance_id, counter, CAST ('{transfer_session_id}' AS {transfer_session_id_type}), store_model_id
+                FROM {record_max_counter} AS rmc
+                INNER JOIN {outgoing_buffer} AS buffer ON rmc.store_model_id = buffer.model_uuid
+                WHERE buffer.transfer_session_id = '{transfer_session_id}'
             """.format(
-                outgoing_buffer=Buffer._meta.db_table,
-                select=" UNION ".join(select_buffers),
-            )
+            transfer_session_id=transfersession.id,
+            transfer_session_id_type=TransferSession._meta.pk.rel_db_type(connection),
+            record_max_counter=RecordMaxCounter._meta.db_table,
+            outgoing_buffer=Buffer._meta.db_table,
         )
-        cursor.execute(
-            """INSERT INTO {outgoing_rmcb}
-               (instance_id, counter, transfer_session_id, model_uuid)
-               {select}
-            """.format(
-                outgoing_rmcb=RecordMaxCounterBuffer._meta.db_table,
-                select=select_rmc_buffer_query,
+
+        with connection.cursor() as cursor:
+            cursor.execute(
+                """INSERT INTO {outgoing_buffer}
+                   (model_uuid, serialized, deleted, last_saved_instance, last_saved_counter,
+                   hard_deleted, model_name, profile, partition, source_id, conflicting_serialized_data,
+                   transfer_session_id, _self_ref_fk)
+                   {select}
+                """.format(
+                    outgoing_buffer=Buffer._meta.db_table,
+                    select=" UNION ".join(select_buffers),
+                )
+            )
+            cursor.execute(
+                """INSERT INTO {outgoing_rmcb}
+                   (instance_id, counter, transfer_session_id, model_uuid)
+                   {select}
+                """.format(
+                    outgoing_rmcb=RecordMaxCounterBuffer._meta.db_table,
+                    select=select_rmc_buffer_query,
+                )
             )
-        )
 
 
-@transaction.atomic(using=USING_DB)
 def _dequeue_into_store(transfer_session, fsic, v2_format=False):
     """
     Takes data from the buffers and merges into the store and record max counters.
 
     ALGORITHM: Incrementally insert and delete on a case by case basis to ensure subsequent cases
     are not affected by previous cases.
     """
-    with connection.cursor() as cursor:
-        DBBackend._dequeuing_delete_rmcb_records(cursor, transfer_session.id)
-        DBBackend._dequeuing_delete_buffered_records(cursor, transfer_session.id)
-        current_id = InstanceIDModel.get_current_instance_and_increment_counter()
-        DBBackend._dequeuing_merge_conflict_buffer(
-            cursor, current_id, transfer_session.id
-        )
-        DBBackend._dequeuing_merge_conflict_rmcb(cursor, transfer_session.id)
-        DBBackend._dequeuing_update_rmcs_last_saved_by(
-            cursor, current_id, transfer_session.id
+
+    with _begin_transaction(Filter(transfer_session.filter)):
+        with connection.cursor() as cursor:
+            DBBackend._dequeuing_delete_rmcb_records(cursor, transfer_session.id)
+            DBBackend._dequeuing_delete_buffered_records(cursor, transfer_session.id)
+            current_id = InstanceIDModel.get_current_instance_and_increment_counter()
+            DBBackend._dequeuing_merge_conflict_buffer(
+                cursor, current_id, transfer_session.id
+            )
+            DBBackend._dequeuing_merge_conflict_rmcb(cursor, transfer_session.id)
+            DBBackend._dequeuing_update_rmcs_last_saved_by(
+                cursor, current_id, transfer_session.id
+            )
+            DBBackend._dequeuing_delete_mc_rmcb(cursor, transfer_session.id)
+            DBBackend._dequeuing_delete_mc_buffer(cursor, transfer_session.id)
+            DBBackend._dequeuing_insert_remaining_buffer(cursor, transfer_session.id)
+            DBBackend._dequeuing_insert_remaining_rmcb(cursor, transfer_session.id)
+            DBBackend._dequeuing_delete_remaining_rmcb(cursor, transfer_session.id)
+            DBBackend._dequeuing_delete_remaining_buffer(cursor, transfer_session.id)
+
+        DatabaseMaxCounter.update_fsics(
+            json.loads(fsic),
+            transfer_session.get_filter(),
+            v2_format=v2_format,
         )
-        DBBackend._dequeuing_delete_mc_rmcb(cursor, transfer_session.id)
-        DBBackend._dequeuing_delete_mc_buffer(cursor, transfer_session.id)
-        DBBackend._dequeuing_insert_remaining_buffer(cursor, transfer_session.id)
-        DBBackend._dequeuing_insert_remaining_rmcb(cursor, transfer_session.id)
-        DBBackend._dequeuing_delete_remaining_rmcb(cursor, transfer_session.id)
-        DBBackend._dequeuing_delete_remaining_buffer(cursor, transfer_session.id)
-
-    DatabaseMaxCounter.update_fsics(
-        json.loads(fsic),
-        transfer_session.get_filter(),
-        v2_format=v2_format,
-    )
 
 
 class BaseOperation(object):
     """
     Base Operation class which defines operation specific behavior that occurs during a sync
     """
 
@@ -825,15 +1042,22 @@
         """
         :type context: LocalSessionContext
         """
         self._assert(context.sync_session is not None)
         self._assert(context.filter is not None)
 
         if context.is_producer and SETTINGS.MORANGO_SERIALIZE_BEFORE_QUEUING:
-            _serialize_into_store(context.sync_session.profile, filter=context.filter)
+            try:
+                _serialize_into_store(context.sync_session.profile, filter=context.filter)
+            except OperationalError as e:
+                # if we run into a transaction isolation error, we return a pending status to force
+                # retrying through the controller flow
+                if DBBackend._is_transaction_isolation_error(e):
+                    return transfer_statuses.PENDING
+                raise e
 
         fsic = json.dumps(
             DatabaseMaxCounter.calculate_filter_specific_instance_counters(
                 context.filter,
                 is_producer=context.is_producer,
                 v2_format=FSIC_V2_FORMAT in context.capabilities,
             )
@@ -910,14 +1134,46 @@
         )
 
         if records_transferred == context.transfer_session.records_total:
             return transfer_statuses.COMPLETED
         return transfer_statuses.PENDING
 
 
+class PullReceiverOperation(LocalOperation):
+    """
+    Operation that ensures we don't run into unhandled stages when the sync is a pull,
+    and the local instance is receiving the pulled data
+    """
+
+    def handle(self, context):
+        """
+        :type context: LocalSessionContext
+        """
+        self._assert(context.is_pull)
+        self._assert(context.is_receiver)
+        self._assert(context.request is None)
+        return transfer_statuses.COMPLETED
+
+
+class PushProducerOperation(LocalOperation):
+    """
+    Operation that ensures we don't run into unhandled stages when the sync is a push,
+    but we're the local instance is the one pushing data
+    """
+
+    def handle(self, context):
+        """
+        :type context: LocalSessionContext
+        """
+        self._assert(context.is_push)
+        self._assert(context.is_producer)
+        self._assert(context.request is None)
+        return transfer_statuses.COMPLETED
+
+
 class PushReceiverOperation(LocalOperation):
     """
     Operation that handles the result of a push, as the server, using a local context / session
     """
 
     def handle(self, context):
         """
@@ -1013,17 +1269,24 @@
         self._assert(context.sync_session is not None)
         self._assert(context.transfer_session is not None)
         self._assert(context.filter is not None)
         self._assert(context.is_receiver)
 
         records_transferred = context.transfer_session.records_transferred or 0
         if SETTINGS.MORANGO_DESERIALIZE_AFTER_DEQUEUING and records_transferred > 0:
-            # we first serialize to avoid deserialization merge conflicts
-            _serialize_into_store(context.sync_session.profile, filter=context.filter)
-            _deserialize_from_store(context.sync_session.profile, filter=context.filter)
+            try:
+                # we first serialize to avoid deserialization merge conflicts
+                _serialize_into_store(context.sync_session.profile, filter=context.filter)
+                _deserialize_from_store(context.sync_session.profile, filter=context.filter)
+            except OperationalError as e:
+                # if we run into a transaction isolation error, we return a pending status to force
+                # retrying through the controller flow
+                if DBBackend._is_transaction_isolation_error(e):
+                    return transfer_statuses.PENDING
+                raise e
 
         return transfer_statuses.COMPLETED
 
 
 class CleanupOperation(LocalOperation):
     """
     Marks the local transfer session as inactive, and deletes queued buffer data if applicable
```

### Comparing `morango-0.6.9/morango/sync/utils.py` & `morango-0.7.0/morango/sync/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -226,7 +226,25 @@
         return self
 
     def __exit__(self, *args, **kwargs):
         """
         Fires the `completed` signal.
         """
         self.completed.fire()
+
+
+def lock_partitions(backend, sync_filter=None, shared=False):
+    """
+    Lock all partitions for a filter, and really lock everything if the filter is null
+
+    :type backend: morango.sync.backends.base.BaseSQLWrapper
+    :type sync_filter: morango.models.certificates.Filter|None
+    :type shared: bool
+    """
+    if sync_filter is None:
+        backend._lock_all_partitions(shared=shared)
+    else:
+        # parse the first 32 chars to obtain the primary partitions in the filter
+        partitions = set(f[:32] for f in sync_filter)
+        # for every unique partition, acquire a lock
+        for partition in partitions:
+            backend._lock_partition(partition, shared=shared)
```

### Comparing `morango-0.6.9/morango/sync/syncsession.py` & `morango-0.7.0/morango/sync/syncsession.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """
 The main module to be used for initiating the synchronization of data between morango instances.
 """
-import os
 import json
 import logging
+import os
 import socket
 import uuid
 from io import BytesIO
 
 from django.utils import timezone
 from django.utils.six import iteritems
 from django.utils.six import raise_from
+from django.utils.six.moves.urllib.parse import urljoin
+from django.utils.six.moves.urllib.parse import urlparse
 from requests.adapters import HTTPAdapter
 from requests.exceptions import HTTPError
 from requests.packages.urllib3.util.retry import Retry
-from django.utils.six.moves.urllib.parse import urljoin
-from django.utils.six.moves.urllib.parse import urlparse
 
 from .session import SessionWrapper
 from morango.api.serializers import CertificateSerializer
 from morango.api.serializers import InstanceIDSerializer
 from morango.constants import api_urls
 from morango.constants import transfer_stages
 from morango.constants import transfer_statuses
@@ -29,17 +29,18 @@
 from morango.errors import MorangoError
 from morango.errors import MorangoResumeSyncError
 from morango.errors import MorangoServerDoesNotAllowNewCertPush
 from morango.models.certificates import Certificate
 from morango.models.certificates import Key
 from morango.models.core import InstanceIDModel
 from morango.models.core import SyncSession
-from morango.sync.controller import SessionController
+from morango.sync.context import CompositeSessionContext
 from morango.sync.context import LocalSessionContext
 from morango.sync.context import NetworkSessionContext
+from morango.sync.controller import SessionController
 from morango.sync.utils import SyncSignal
 from morango.sync.utils import SyncSignalGroup
 from morango.utils import CAPABILITIES
 from morango.utils import pid_exists
 
 if GZIP_BUFFER_POST in CAPABILITIES:
     from gzip import GzipFile
@@ -220,34 +221,44 @@
         # Sync Session creation request
         session_resp = self._create_sync_session(data)
 
         # check that the nonce/id were properly signed by the server cert
         if not server_cert.verify(message, session_resp.json().get("signature")):
             raise CertificateSignatureInvalid()
 
+        client_instance = InstanceIDModel.get_or_create_current_instance()[0]
+
+        server_instance_json = session_resp.json().get("server_instance") or "{}"
+        server_instance_id = None
+        if server_instance_json:
+            server_instance = json.loads(server_instance_json)
+            server_instance_id = server_instance.get("id")
+
         # build the data to be used for creating our own syncsession
         data = {
             "id": data["id"],
             "start_timestamp": timezone.now(),
             "last_activity_timestamp": timezone.now(),
             "active": True,
             "is_server": False,
             "client_certificate": client_cert,
             "server_certificate": server_cert,
             "profile": client_cert.profile,
             "connection_kind": "network",
             "connection_path": self.base_url,
             "client_ip": data["client_ip"],
             "server_ip": data["server_ip"],
-            "client_instance": json.dumps(
+            "client_instance_id": client_instance.id,
+            "client_instance_json": json.dumps(
                 InstanceIDSerializer(
-                    InstanceIDModel.get_or_create_current_instance()[0]
+                    client_instance
                 ).data
             ),
-            "server_instance": session_resp.json().get("server_instance") or "{}",
+            "server_instance_id": server_instance_id,
+            "server_instance_json": session_resp.json().get("server_instance") or "{}",
             "process_id": os.getpid(),
         }
         sync_session = SyncSession.objects.create(**data)
         return SyncSessionClient(self, sync_session)
 
     def resume_sync_session(self, sync_session_id, chunk_size=None):
         """
@@ -571,141 +582,114 @@
     Base class for handling common operations for initiating syncing and other related operations.
     """
 
     __slots__ = (
         "sync_connection",
         "sync_session",
         "controller",
-        "current_transfer_session",
         "signals",
-        "local_context",
-        "remote_context",
+        "context",
     )
 
     def __init__(self, sync_connection, sync_session, controller):
         """
         :param sync_connection: NetworkSyncConnection
         :param sync_session: SyncSession
         :param controller: SessionController
         """
         self.sync_connection = sync_connection
         self.sync_session = sync_session
         self.controller = controller
-        self.current_transfer_session = None
         self.signals = SyncClientSignals()
 
-        # TODO: come up with strategy to use only one context here
-        self.remote_context = NetworkSessionContext(
-            sync_connection, sync_session=sync_session
-        )
-        self.local_context = LocalSessionContext(
-            sync_session=sync_session, capabilities=self.remote_context.capabilities
-        )
-
-    def proceed_to_and_wait_for(self, stage):
-        contexts = (self.local_context, self.remote_context)
-        for context in contexts:
-            max_interval = 1 if context is self.local_context else 5
-            result = self.controller.proceed_to_and_wait_for(
-                stage, context=context, max_interval=max_interval
-            )
-            if result == transfer_statuses.ERRORED:
-                raise_from(
-                    MorangoError("Stage `{}` failed".format(stage)),
-                    context.error,
-                )
+        capabilities = sync_connection.server_info.get("capabilities", [])
+        self.context = CompositeSessionContext(
+            [LocalSessionContext(), NetworkSessionContext(sync_connection)],
+            sync_session=sync_session,
+            capabilities=capabilities,
+        )
+        self.controller.context = self.context
+
+    @property
+    def current_transfer_session(self):
+        return self.context.transfer_session
+
+    def proceed_to_and_wait_for(self, stage, error_msg=None, callback=None):
+        """
+        Raises an exception if an ERROR result is received from calling `proceed_to_and_wait_for`
+        :param stage: The stage to proceed to
+        :param error_msg: An error message str to use as the exception message if it errors
+        :param callback: A callback to pass along to the controller
+        """
+        result = self.controller.proceed_to_and_wait_for(stage, callback=callback)
+        if result == transfer_statuses.ERRORED:
+            raise_from(
+                MorangoError(
+                    error_msg or "Stage `{}` failed".format(self.context.stage)
+                ),
+                self.context.error,
+            )
 
     def initialize(self, sync_filter):
         """
         :param sync_filter: Filter
         """
         # set filter on controller
-        self.local_context.update(sync_filter=sync_filter)
-        self.remote_context.update(sync_filter=sync_filter)
+        self.context.update(sync_filter=sync_filter)
 
-        # initialize the transfer session locally
-        status = self.controller.proceed_to_and_wait_for(
-            transfer_stages.INITIALIZING, context=self.local_context, max_interval=1
+        # initialize the transfer session
+        self.proceed_to_and_wait_for(
+            transfer_stages.INITIALIZING,
+            error_msg="Failed to initialize transfer session",
         )
-        if status == transfer_statuses.ERRORED:
-            raise_from(
-                MorangoError("Failed to initialize transfer session"),
-                self.local_context.error,
-            )
-
-        # copy the transfer session to local state and update remote controller context
-        self.current_transfer_session = self.local_context.transfer_session
-        self.remote_context.update(transfer_session=self.current_transfer_session)
 
         self.signals.session.started.fire(
             transfer_session=self.current_transfer_session
         )
 
         # backwards compatibility for the queuing signal as it included both serialization
         # and queuing originally
         with self.signals.queuing.send(transfer_session=self.current_transfer_session):
-            # proceeding to serialization on remote will trigger initialization as well
-            self.proceed_to_and_wait_for(transfer_stages.SERIALIZING)
+            # proceeding to queuing on remote will trigger initialization and serialization as well
             self.proceed_to_and_wait_for(transfer_stages.QUEUING)
 
     def run(self):
+        """
+        Execute the transferring portion of the sync
+        """
         with self.signals.transferring.send(
             transfer_session=self.current_transfer_session
         ) as status:
-            self._transfer(callback=status.in_progress.fire)
+            self.proceed_to_and_wait_for(
+                transfer_stages.TRANSFERRING, callback=status.in_progress.fire
+            )
 
     def finalize(self):
-        # if not initialized, we don't need to finalize
-        if not self.current_transfer_session:
-            return
-
         with self.signals.dequeuing.send(
             transfer_session=self.current_transfer_session
         ):
             self.proceed_to_and_wait_for(transfer_stages.DESERIALIZING)
 
         self.proceed_to_and_wait_for(transfer_stages.CLEANUP)
         self.signals.session.completed.fire(
             transfer_session=self.current_transfer_session
         )
-        self.current_transfer_session = None
-
-    def _transfer(self, callback=None):
-        result = transfer_statuses.PENDING
-
-        while result not in transfer_statuses.FINISHED_STATES:
-            result = self.controller.proceed_to(
-                transfer_stages.TRANSFERRING, context=self.remote_context
-            )
-            self.local_context.update(
-                stage=transfer_stages.TRANSFERRING, stage_status=result
-            )
-            if callback is not None:
-                callback()
-
-        if result == transfer_statuses.ERRORED:
-            raise_from(
-                MorangoError("Failure occurred during transfer"),
-                self.remote_context.error,
-            )
 
 
 class PushClient(TransferClient):
     """
     Sync client for pushing to a server
     """
 
     def __init__(self, *args, **kwargs):
         super(PushClient, self).__init__(*args, **kwargs)
-        self.local_context.update(is_push=True)
-        self.remote_context.update(is_push=True)
+        self.context.update(is_push=True)
 
 
 class PullClient(TransferClient):
     """
     Sync class to pull from server
     """
 
     def __init__(self, *args, **kwargs):
         super(PullClient, self).__init__(*args, **kwargs)
-        self.local_context.update(is_push=False)
-        self.remote_context.update(is_push=False)
+        self.context.update(is_push=False)
```

### Comparing `morango-0.6.9/morango/sync/controller.py` & `morango-0.7.0/morango/sync/controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
+import math
 from time import sleep
 
 from morango.constants import transfer_stages
 from morango.constants import transfer_statuses
 from morango.registry import session_middleware
-
 from morango.sync.operations import _deserialize_from_store
 from morango.sync.operations import _serialize_into_store
 from morango.sync.operations import OperationLogger
 from morango.sync.utils import SyncSignalGroup
 from morango.utils import _assert
 
 
@@ -126,18 +126,18 @@
         status, that status is returned indicating that the method call has not reached
         `target_stage`. Therefore middleware can perform operations asynchronously and this can be
         repeatedly called to move forward through the transfer stages and their operations
 
         When invoking the middleware, if the status result is:
             PENDING: The controller will continue to invoke the middleware again when this method
                 is called repeatedly, until the status result changes
-            STARTED: The controller will not invoke any middleware until the the status changes,
+            STARTED: The controller will not invoke any middleware until the status changes,
                 and assumes the "started" operation will update the state itself
             COMPLETED: The controller will proceed to invoke the middleware for the next stage
-            ERRORED: The controller will not invoke any middleware until the the status changes,
+            ERRORED: The controller will not invoke any middleware until the status changes,
                 which would require codified resolution of the error outside of the controller
 
         :param target_stage: transfer_stage.* - The transfer stage to proceed to
         :type target_stage: str
         :param context: Override controller context, or provide it if missing
         :type context: morango.sync.context.SessionContext|None
         :return: transfer_status.* - The status of proceeding to that stage
@@ -183,36 +183,49 @@
                 if result != transfer_statuses.COMPLETED:
                     break
 
         # since the middleware must handle our request, or throw an unimplemented error, this
         # should always be a non-False status
         return result
 
-    def proceed_to_and_wait_for(self, target_stage, context=None, max_interval=5):
+    def proceed_to_and_wait_for(
+        self, target_stage, context=None, max_interval=None, callback=None
+    ):
         """
         Same as `proceed_to` but waits for a finished status to be returned by sleeping between
         calls to `proceed_to` if status is not complete
 
         :param target_stage: transfer_stage.* - The transfer stage to proceed to
         :type target_stage: str
         :param context: Override controller context, or provide it if missing
         :type context: morango.sync.context.SessionContext|None
         :param max_interval: The max time, in seconds, between repeat calls to `.proceed_to`
+        :param callback: A callable to invoke after every attempt
         :return: transfer_status.* - The status of proceeding to that stage,
             which should be `ERRORED` or `COMPLETE`
         :rtype: str
         """
         result = transfer_statuses.PENDING
         tries = 0
+        context = context or self.context
+        max_interval = max_interval or context.max_backoff_interval
+        # solve for the number of tries at which our sleep time will always be max_interval
+        max_interval_tries = math.ceil(math.log(max_interval / 0.3 + 1) / math.log(2))
+
         while result not in transfer_statuses.FINISHED_STATES:
             if tries > 0:
                 # exponential backoff up to max_interval
-                sleep(min(0.3 * (2 ** tries - 1), max_interval))
+                if tries >= max_interval_tries:
+                    sleep(max_interval)
+                else:
+                    sleep(0.3 * (2 ** tries - 1))
             result = self.proceed_to(target_stage, context=context)
             tries += 1
+            if callable(callback):
+                callback()
         return result
 
     def _invoke_middleware(self, context, middleware):
         """
         Invokes middleware, with logging if enabled, and handles updating the transfer session state
 
         :param context: The context to invoke the middleware with
@@ -220,36 +233,42 @@
         :type middleware: morango.registry.SessionMiddlewareOperations
         :return: transfer_status.* - The result of invoking the middleware
         :rtype: str
         """
         stage = middleware.related_stage
         signal = getattr(self.signals, stage)
         at_stage = context.stage == stage
+        prepared_context = None
 
         try:
             context.update(stage=stage, stage_status=transfer_statuses.PENDING)
 
+            # we'll use the prepared context for passing to the middleware and any signal handlers
+            prepared_context = context.prepare()
+
             # only fire "started" when we first try to invoke the stage
             # NOTE: this means that signals.started is not equivalent to transfer_stage.STARTED
             if not at_stage:
-                signal.started.fire(context=context)
+                signal.started.fire(context=prepared_context)
 
-            result = middleware(context)
+            # invoke the middleware with the prepared context
+            result = middleware(prepared_context)
 
             # don't update stage result if context's stage was updated during operation
             if context.stage == stage:
                 context.update(stage_status=result)
 
             # fire signals based off middleware invocation result; the progress signal if incomplete
             if result == transfer_statuses.COMPLETED:
-                signal.completed.fire(context=context)
+                signal.completed.fire(context=prepared_context)
             else:
-                signal.in_progress.fire(context=context)
+                signal.in_progress.fire(context=prepared_context)
 
-            return result
+            # context should take precedence over result, and was likely updated
+            return context.stage_status
         except Exception as e:
             # always log the error itself
             logger.error(e)
             context.update(stage_status=transfer_statuses.ERRORED, error=e)
             # fire completed signal, after context update. handlers can use context to detect error
-            signal.completed.fire(context=context)
+            signal.completed.fire(context=prepared_context or context)
             return transfer_statuses.ERRORED
```

### Comparing `morango-0.6.9/morango/migrations/0019_auto_20220113_1807.py` & `morango-0.7.0/morango/migrations/0019_auto_20220113_1807.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0010_auto_20171206_1615.py` & `morango-0.7.0/morango/migrations/0010_auto_20171206_1615.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0001_initial.py` & `morango-0.7.0/morango/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0007_auto_20171018_1615.py` & `morango-0.7.0/morango/migrations/0007_auto_20171018_1615.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0003_auto_20170519_0543.py` & `morango-0.7.0/morango/migrations/0003_auto_20170519_0543.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0002_auto_20170511_0400.py` & `morango-0.7.0/morango/migrations/0002_auto_20170511_0400.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0012_auto_20180927_1658.py` & `morango-0.7.0/morango/migrations/0012_auto_20180927_1658.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0004_auto_20170520_2112.py` & `morango-0.7.0/morango/migrations/0004_auto_20170520_2112.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0005_auto_20170629_2139.py` & `morango-0.7.0/morango/migrations/0005_auto_20170629_2139.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0017_store_last_transfer_session_id.py` & `morango-0.7.0/morango/migrations/0017_store_last_transfer_session_id.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0011_sharedkey.py` & `morango-0.7.0/morango/migrations/0011_sharedkey.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0018_auto_20210714_2216.py` & `morango-0.7.0/morango/migrations/0018_auto_20210714_2216.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0015_auto_20200508_2104.py` & `morango-0.7.0/morango/migrations/0015_auto_20200508_2104.py`

 * *Files identical despite different names*

### Comparing `morango-0.6.9/morango/migrations/0008_auto_20171114_2217.py` & `morango-0.7.0/morango/migrations/0008_auto_20171114_2217.py`

 * *Files identical despite different names*

