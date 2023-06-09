# Comparing `tmp/invenio-rdm-migrator-1.0.0a8.tar.gz` & `tmp/invenio-rdm-migrator-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a8.tar", last modified: Thu May  4 13:04:10 2023, max compression
+gzip compressed data, was "dist/invenio-rdm-migrator-1.0.0a9.tar", last modified: Tue May  9 13:25:51 2023, max compression
```

## Comparing `invenio-rdm-migrator-1.0.0a8.tar` & `invenio-rdm-migrator-1.0.0a9.tar`

### file list

```diff
@@ -1,113 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/extract/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/extract/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8335 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/postgresql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6035 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/drafts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/parents.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/load.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/records/
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    19218 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/records/test_records_table_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:04:10.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/
--rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_table_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-05-04 13:04:03.000000 invenio-rdm-migrator-1.0.0a8/tests/streams/test_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7465 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/extract/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8166 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/postgresql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/drafts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/parents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4098 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13302 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 13:25:50.000000 invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1410 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/records/test_records_table_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 13:25:51.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_table_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-05-09 13:25:43.000000 invenio-rdm-migrator-1.0.0a9/tests/streams/test_cache.py
```

### Comparing `invenio-rdm-migrator-1.0.0a8/.editorconfig` & `invenio-rdm-migrator-1.0.0a9/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/.github/workflows/pypi-publish.yml` & `invenio-rdm-migrator-1.0.0a9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/.github/workflows/tests.yml` & `invenio-rdm-migrator-1.0.0a9/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/CONTRIBUTING.rst` & `invenio-rdm-migrator-1.0.0a9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/LICENSE` & `invenio-rdm-migrator-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/MANIFEST.in` & `invenio-rdm-migrator-1.0.0a9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/PKG-INFO` & `invenio-rdm-migrator-1.0.0a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a8/README.rst` & `invenio-rdm-migrator-1.0.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/docs/Makefile` & `invenio-rdm-migrator-1.0.0a9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/docs/conf.py` & `invenio-rdm-migrator-1.0.0a9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/docs/index.rst` & `invenio-rdm-migrator-1.0.0a9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/docs/make.bat` & `invenio-rdm-migrator-1.0.0a9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/base.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/base.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/ids.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/ids.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/models.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/load/postgresql.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/load/postgresql.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,25 +16,18 @@
 from datetime import datetime
 from pathlib import Path
 from uuid import UUID
 
 import psycopg
 from invenio_records.dictutils import dict_set  # TODO: can we do without?
 
+from ..utils import ts
 from .base import Load
 
 
-def _ts(iso=True, fmt=None):
-    """Current timestamp string."""
-    dt = datetime.now()
-    if fmt:
-        return dt.strftime(fmt)
-    return dt.isoformat() if iso else dt.timestamp()
-
-
 def as_csv_row(dc):
     """Serialize a dataclass instance as a CSV-writable row."""
     row = []
     for f in fields(dc):
         val = getattr(dc, f.name)
         if val:
             if issubclass(f.type, (dict,)):
@@ -49,15 +42,15 @@
 
 class PostgreSQLCopyLoad(Load):
     """PostgreSQL COPY load."""
 
     def __init__(self, db_uri, table_generators, tmp_dir):
         """Constructor."""
         self.db_uri = db_uri
-        self.tmp_dir = Path(tmp_dir) / f"tables-{_ts(fmt='%Y-%m-%dT%H%M%S')}"
+        self.tmp_dir = Path(tmp_dir) / f"tables-{ts(fmt='%Y-%m-%dT%H%M%S')}"
         self.table_generators = table_generators
 
     def _cleanup(self, db=False):
         """Cleanup csv files and DB after load."""
         for table in self.table_generators:
             table.cleanup(db=db)
 
@@ -97,15 +90,15 @@
                 name = table._table_name
                 cols = ", ".join([f.name for f in fields(table)])
                 fpath = self.tmp_dir / f"{name}.csv"
                 if fpath.exists():
                     # total file size for progress logging
                     file_size = fpath.stat().st_size
 
-                    print(f"[{_ts()}] COPY FROM {fpath}")  # TODO: logging
+                    print(f"[{ts()}] COPY FROM {fpath}")  # TODO: logging
                     with contextlib.ExitStack() as stack:
                         cur = stack.enter_context(conn.cursor())
                         copy = stack.enter_context(
                             cur.copy(f"COPY {name} ({cols}) FROM STDIN (FORMAT csv)")
                         )
                         fp = stack.enter_context(open(fpath, "r"))
 
@@ -120,19 +113,19 @@
                         for idx, block in enumerate(_data_blocks(block_size)):
                             if idx % 100:
                                 cur_bytes = idx * block_size
                                 percentage = (cur_bytes / file_size) * 100
                                 progress = (
                                     f"{cur_bytes}/{file_size} ({percentage:.2f}%)"
                                 )
-                                print(f"[{_ts()}] {name}: {progress}")
+                                print(f"[{ts()}] {name}: {progress}")
                             copy.write(block)
                 else:
                     # FIXME: log a WARNING/ERROR
-                    print(f"[{_ts()}] {name}: no data to load")
+                    print(f"[{ts()}] {name}: no data to load")
                 conn.commit()
 
     def _post_load(self):
         """Post load processing."""
         tables = set()
         for tg in self.table_generators:
             tables = tables.join(set(tg.tables))
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/cache.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/cache.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,35 +6,51 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Cache module."""
 
 import json
 from abc import ABC, abstractmethod
 
+from ..utils import ts
+
 
 class Cache(ABC):
     """Cache interface."""
 
     def __init__(self, filepath=None, validate=False):
         """Constructor."""
         self._data = {}
 
-        if filepath:  # load cache from file
+        if filepath and filepath.exists():  # load cache from file
+            start = ts(iso=False)
+            print(f"Loading cache from {filepath} {ts()}")
             with open(filepath, "r") as file:
                 self._data = json.loads(file.read())
 
+            print(f"Finished loading cache {ts()}")
             if validate:
+                print(f"Validating cache {ts()}")
                 for _, entry in self._data.items():
                     self._validate(entry)
+                print(f"Finished validating cache {ts()}")
+            end = ts(iso=False)
+            print(f"Cache loading took {end-start} seconds.")
 
     def dump(self, filepath):
         """Dump cache data into a json file."""
+        print(f"Dumping cache to {filepath} {ts()}")
+        start = ts(iso=False)
+
         with open(filepath, "w") as outfile:
             outfile.write(json.dumps(self._data))
 
+        end = ts(iso=False)
+        print(f"Finished dumping cache {ts()}")
+        print(f"Cache dumping took {end-start} seconds.")
+
     def get(self, key):
         """Get data from the cache."""
         key = str(key)  # in case they are numbers
         return self._data.get(key, {})
 
     def all(self):
         """Get all the data from the cache."""
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/__init__.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/load.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/models.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/table_generator.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/communities/transform.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/communities/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/__init__.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/load.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/models.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/table_generator.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/files/transform.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/files/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/load.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/models.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/drafts.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/drafts.py`

 * *Files 16% similar despite different names*

```diff
@@ -108,26 +108,16 @@
                 pid_value=draft["json"]["id"],
                 status=record_pid["status"],
                 object_type=record_pid["obj_type"],
                 object_uuid=draft["id"],
                 created=now,
                 updated=now,
             )
-            # DOI
-            if "doi" in draft["json"]["pids"]:
-                yield PersistentIdentifier(
-                    id=pid_pk(),
-                    pid_type="doi",
-                    pid_value=draft["json"]["pids"]["doi"]["identifier"],
-                    status="N",
-                    object_type="rec",
-                    object_uuid=draft["id"],
-                    created=now,
-                    updated=now,
-                )
+        # we don't emit doi Persistentidentifier for drafts as either they have already
+        # one from records or have an external doi that is registered on publish
 
     # FIXME: deduplicate with records.py
     def _resolve_references(self, data, **kwargs):
         """Resolve references e.g communities slug names."""
 
         def _resolve_communities(communities):
             default_slug = communities.get("default")
@@ -142,15 +132,39 @@
             _ids = []
             for slug in communities_slugs:
                 _id = self.communities_cache.get(slug)
                 if _id:
                     _ids.append(_id)
             communities["ids"] = _ids
 
+        def _resolve_pids(draft):
+            """Enforce record pids to draft."""
+            if not draft:
+                return
+
+            # some legacy records have different pid value in deposit than record
+            # however _deposit.pid.value would contain the correct one
+            # if it is not legacy we get it from the current field (json.id)
+            recid = draft["json"]["id"]
+            forked_published = self.records_cache.get(recid)
+            if forked_published:
+                pids = draft["json"]["pids"]
+                has_draft_external_doi = (
+                    pids.get("doi", {}).get("provider") == "external"
+                )
+                if has_draft_external_doi:
+                    # then keep the draft external value as it might be there for
+                    # updating the existing value. Update the draft only with `oai`
+                    pids["oai"] = forked_published["pids"]["oai"]
+                else:
+                    # enfore published record pids to draft
+                    pids = forked_published["pids"]
+
         # resolve parent communities slug
         parent = data["parent"]
         communities = parent["json"].get("communities")
         if communities:
             _resolve_communities(communities)
+        _resolve_pids(data.get("draft"))
 
     # FIXME: deduplicate with records.py
     # assumis records post load alters pidstore_pid_id_seq and pidstore_recid_recid_seq
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/parents.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/parents.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/records.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 """Invenio RDM migration record table load module."""
 
 from datetime import datetime
 from uuid import UUID
 
 from ....load.ids import generate_recid, generate_uuid, pid_pk
 from ....load.models import PersistentIdentifier
-from ....load.postgresql import TableGenerator, _ts
+from ....load.postgresql import TableGenerator
+from ....utils import ts
 from ...communities.models import RDMParentCommunityMetadata
 from ..models import RDMParentMetadata, RDMRecordFile, RDMRecordMetadata
 from .parents import generate_parent_rows
 
 
 def _is_valid_uuid(value):
     try:
@@ -103,15 +104,15 @@
                         community_id=parent_def_id,
                         record_id=parent_comm_id,
                         request_id=None,
                     )
                 else:
                     record_id = record["json"]["id"]
                     print(
-                        f"[{_ts()}] Record parent community not migrated. Record id[{record_id}]. parent community [{parent_comm_id}] parent default community [{parent_def_id}]"
+                        f"[{ts()}] Record parent community not migrated. Record id[{record_id}]. parent community [{parent_comm_id}] parent default community [{parent_def_id}]"
                     )
         else:
             self.parents_cache.update(
                 parent["json"]["id"],
                 {
                     "latest_index": record["index"],
                     "latest_id": record["id"],
@@ -123,14 +124,15 @@
         self.records_cache.add(
             record["json"]["id"],  # recid
             {
                 "index": record["index"],
                 "id": record["id"],  # uuid
                 "parent_id": parent_id,  # parent uuid
                 "fork_version_id": record["version_id"],
+                "pids": record["json"]["pids"],
             },
         )
 
         yield RDMRecordMetadata(
             id=record["id"],
             json=record["json"],
             created=record["created"],
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/table_generators/versions.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/table_generators/versions.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/records/transform.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/records/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,18 +51,23 @@
             "record": self._record(entry),
             "draft": self._draft(entry),
             "parent": self._parent(entry),
             "record_files": self._record_files(entry),
             "draft_files": self._draft_files(entry),
         }
 
-    def run(self, entries):
+    def run(self, entries, logger=None):
         """Transform and yield one element at a time."""
         for entry in entries:
-            yield self._transform(entry)
+            try:
+                yield self._transform(entry)
+            except Exception:
+                if logger:
+                    logger.error(entry, exc_info=1)
+                continue
 
 
 class RDMRecordEntry(Entry):
     """Transform a single record entry."""
 
     @abstractmethod
     def _id(self, entry):
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/load.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/models.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/table_generator.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/requests/transform.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/requests/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/streams.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/streams.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,27 +44,28 @@
         self.transform_cls = transform_cls or NoTransform
         self.load_cls = load_cls
 
 
 class Stream:
     """ETL stream."""
 
-    def __init__(self, name, extract, transform, load):
+    def __init__(self, name, extract, transform, load, logger=None):
         """Constructor."""
         self.name = name
         self.extract = extract
         self.transform = transform
         self.load = load
+        self.logger = logger
 
     def run(self, cleanup=False):
         """Run ETL stream."""
         start_time = datetime.now()
         print(f"Stream started {start_time.isoformat()}")
 
         extract_gen = self.extract.run()
-        transform_gen = self.transform.run(extract_gen)
+        transform_gen = self.transform.run(extract_gen, self.logger)
         self.load.run(transform_gen, cleanup=cleanup)
 
         end_time = datetime.now()
         print(f"Stream ended {end_time.isoformat()}")
 
         print(f"Execution time: {end_time - start_time}")
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/load.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/models.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/models.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/table_generator.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/streams/users/transform.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/streams/users/transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator/transform/base.py` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator/transform/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,18 +14,23 @@
     """Base class for data transformation."""
 
     @abstractmethod
     def _transform(self, entry):
         """Transform entry."""
         pass
 
-    def run(self, entries):
+    def run(self, entries, logger=None):
         """Transform and yield one element at a time."""
         for entry in entries:
-            yield self._transform(entry)
+            try:
+                yield self._transform(entry)
+            except Exception:
+                if logger:
+                    logger.error(entry, exc_info=1)
+                continue
 
 
 class Entry(ABC):
     """Base entry class."""
 
     @abstractmethod
     def transform(self, entry):
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/PKG-INFO` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-rdm-migrator
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: InvenioRDM module for data migration.
 Home-page: https://github.com/inveniosoftware/invenio-rdm-migrator
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             Copyright (C) 2022 CERN.
```

### Comparing `invenio-rdm-migrator-1.0.0a8/invenio_rdm_migrator.egg-info/SOURCES.txt` & `invenio-rdm-migrator-1.0.0a9/invenio_rdm_migrator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 docs/index.rst
 docs/installation.rst
 docs/license.rst
 docs/make.bat
 docs/requirements.txt
 docs/usage.rst
 invenio_rdm_migrator/__init__.py
+invenio_rdm_migrator/utils.py
 invenio_rdm_migrator.egg-info/PKG-INFO
 invenio_rdm_migrator.egg-info/SOURCES.txt
 invenio_rdm_migrator.egg-info/dependency_links.txt
 invenio_rdm_migrator.egg-info/not-zip-safe
 invenio_rdm_migrator.egg-info/requires.txt
 invenio_rdm_migrator.egg-info/top_level.txt
 invenio_rdm_migrator/extract/__init__.py
```

### Comparing `invenio-rdm-migrator-1.0.0a8/run-tests.sh` & `invenio-rdm-migrator-1.0.0a9/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/setup.cfg` & `invenio-rdm-migrator-1.0.0a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/conftest.py` & `invenio-rdm-migrator-1.0.0a9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/conftest.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_load.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_table_generator.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/communities/test_communities_transform.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/communities/test_communities_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/files/conftest.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/files/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_load.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_table_generator.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/files/test_files_transform.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/files/test_files_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/records/conftest.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/records/conftest.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,17 +101,16 @@
             "updated": "2023-01-31 12:00:00.00000",
             "version_id": 1,
             "index": 1,
             "json": {
                 "id": "12345678",
                 "pids": {
                     "doi": {
-                        "client": "datacite",
-                        "provider": "datacite",
-                        "identifier": "10.5281/zenodo.12345678",
+                        "provider": "external",
+                        "identifier": "10.1234/foo",
                     },
                 },
             },
             "expires_at": "2024-01-01 12:00:00.00000",
             "fork_version_id": None,
         },
         "record_files": {},
```

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/records/test_records_table_generator.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/records/test_records_table_generator.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Records/Drafts table generator tests."""
 
 from copy import deepcopy
 from unittest.mock import patch
 
-import dictdiffer
 import pytest
 
 from invenio_rdm_migrator.load.models import PersistentIdentifier
 from invenio_rdm_migrator.streams.communities.models import RDMParentCommunityMetadata
 from invenio_rdm_migrator.streams.records.load import (
     RDMDraftTableGenerator,
     RDMRecordTableGenerator,
@@ -250,17 +249,16 @@
                     "pk": "10123",
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "N",
                 },
                 "pids": {
                     "doi": {
-                        "client": "datacite",
-                        "provider": "datacite",
-                        "identifier": "10.5281/zenodo.12345678",
+                        "provider": "external",
+                        "identifier": "10.1234/foo",
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
@@ -275,24 +273,14 @@
             pid_value="12345678",
             status="N",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823386",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
-        PersistentIdentifier(  # doi
-            id="10124",
-            pid_type="doi",
-            pid_value="10.5281/zenodo.12345678",
-            status="N",
-            object_type="rec",
-            object_uuid="2d6970ea-602d-4e8b-a918-063a59823386",
-            created="2023-04-01 12:00:00.00000",
-            updated="2023-04-01 12:00:00.00000",
-        ),
     ]
 
     assert rows == expected_rows
 
     assert len(cache["parents"].all()) == 2  # pre-existing and new
     assert len(cache["records"].all()) == 0
 
@@ -423,17 +411,16 @@
                     "pk": "10123",
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "R",
                 },
                 "pids": {
                     "doi": {
-                        "client": "datacite",
-                        "provider": "datacite",
-                        "identifier": "10.5281/zenodo.12345678",
+                        "provider": "external",
+                        "identifier": "10.1234/foo",
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
@@ -496,15 +483,15 @@
     v2["record"]["json"]["pid"]["pk"] = "10126"  # pk, not pid value
     v2["record"]["json"]["pids"]["oai"]["identifier"] = "oai:zenodo.org:12345679"
     v2["record"]["json"]["pids"]["doi"]["identifier"] = "10.5281/zenodo.12345679"
     d_v3 = transformed_draft_entry_pks
     d_v3["draft"]["id"] = "2d6970ea-602d-4e8b-a918-063a59823389"
     d_v3["draft"]["json"]["id"] = "12345680"
     d_v3["draft"]["json"]["pid"]["pk"] = "10128"  # pk, not pid value, same as v1
-    d_v3["draft"]["json"]["pids"]["doi"]["identifier"] = "10.5281/zenodo.12345680"
+    d_v3["draft"]["json"]["pids"]["doi"]["identifier"] = "10.1234/bar"
 
     rows = []
     for entry in [v1, v2, d_v3]:
         for tg in tgs:
             rows.extend(list(tg._generate_rows(entry)))
 
     expected_rows_d_v3 = [
@@ -516,17 +503,16 @@
                     "pk": "10128",
                     "obj_type": "rec",
                     "pid_type": "recid",
                     "status": "N",
                 },
                 "pids": {
                     "doi": {
-                        "client": "datacite",
-                        "provider": "datacite",
-                        "identifier": "10.5281/zenodo.12345680",
+                        "provider": "external",
+                        "identifier": "10.1234/bar",
                     },
                 },
             },
             created="2023-01-01 12:00:00.00000",
             updated="2023-01-31 12:00:00.00000",
             version_id=1,
             index=1,
@@ -541,26 +527,17 @@
             pid_value="12345680",
             status="N",
             object_type="rec",
             object_uuid="2d6970ea-602d-4e8b-a918-063a59823389",
             created="2023-04-01 12:00:00.00000",
             updated="2023-04-01 12:00:00.00000",
         ),
-        PersistentIdentifier(  # doi
-            id="10128",
-            pid_type="doi",
-            pid_value="10.5281/zenodo.12345680",
-            status="N",
-            object_type="rec",
-            object_uuid="2d6970ea-602d-4e8b-a918-063a59823389",
-            created="2023-04-01 12:00:00.00000",
-            updated="2023-04-01 12:00:00.00000",
-        ),
     ]
 
-    assert len(rows) == 14
+    assert len(rows) == 13
+
     # v1 rows not asserted since they are checked at test_single_record_generate_rows
     # v2 rows not asserted since they are checked at test_record_versions_and_old_draft_generate_rows
-    assert rows[11:14] == expected_rows_d_v3
+    assert rows[11:13] == expected_rows_d_v3
 
     assert len(cache["parents"].all()) == 2  # pre-existing and new
     assert len(cache["records"].all()) == 2  # two added records
```

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/conftest.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/requests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_load.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_load.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_table_generator.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_table_generator.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/requests/test_requests_transform.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/requests/test_requests_transform.py`

 * *Files identical despite different names*

### Comparing `invenio-rdm-migrator-1.0.0a8/tests/streams/test_cache.py` & `invenio-rdm-migrator-1.0.0a9/tests/streams/test_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # Invenio-RDM-Migrator is free software; you can redistribute it and/or modify
 # it under the terms of the MIT License; see LICENSE file for more details.
 
 """Cache tests."""
 
 import json
+from pathlib import Path
 
 import pytest
 
 from invenio_rdm_migrator.streams.cache import Cache, ParentsCache, RecordsCache
 
 ###
 # Parent Cache
@@ -176,15 +177,15 @@
         """Validate data value is not 2."""
         assert not data["value"] == 2
 
 
 @pytest.fixture(scope="function")
 def data_file(tmp_dir):
     """Cache data filepath."""
-    filepath = f"{tmp_dir.name}/data.json"
+    filepath = Path(f"{tmp_dir.name}/data.json")
     with open(filepath, "w") as file:
         file.write(json.dumps({"one": {"value": 1}, "two": {"value": 2}}))
 
     return filepath
 
 
 def test_cache_from_source_data_no_validation(data_file):
```

