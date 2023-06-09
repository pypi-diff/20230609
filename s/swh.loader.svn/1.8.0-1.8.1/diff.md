# Comparing `tmp/swh.loader.svn-1.8.0.tar.gz` & `tmp/swh.loader.svn-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.svn-1.8.0.tar", last modified: Tue Jun  6 12:50:23 2023, max compression
+gzip compressed data, was "dist/swh.loader.svn-1.8.1.tar", last modified: Fri Jun  9 12:26:29 2023, max compression
```

## Comparing `swh.loader.svn-1.8.0.tar` & `swh.loader.svn-1.8.1.tar`

### file list

```diff
@@ -1,96 +1,97 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2023 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1095 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      552 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/bin/init-svn-repository.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      761 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/bin/swh-svn
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      391 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     6651 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/docs/swh-loader-svn.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/install/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      644 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/install/install-pysvn.sh
--rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/install/install-subvertpy.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/resources/svn.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     5522 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/setup.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/svn-lib-client-analysis.org
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/svn/
--rw-r--r--   0 jenkins    (115) docker     (999)      491 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2427 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2334 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)      667 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/exception.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9055 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.cpp
--rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.pyi
--rw-r--r--   0 jenkins    (115) docker     (999)    33376 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)    33988 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/replay.py
--rw-r--r--   0 jenkins    (115) docker     (999)    25221 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/svn_repo.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1521 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/svn_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1785 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2690 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)   360057 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/httthttt.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   389343 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
--rw-r--r--   0 jenkins    (115) docker     (999)   419840 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   430080 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   911360 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    28495 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   133120 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    35440 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    30908 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    28193 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)   406052 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4548 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    62193 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_externals.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2371 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_fast_crawler.py
--rw-r--r--   0 jenkins    (115) docker     (999)    17874 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.org
--rw-r--r--   0 jenkins    (115) docker     (999)    79798 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4415 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_repo.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12997 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_retry.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1475 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    21336 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3734 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/tests/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16004 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/swh/loader/svn/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2023 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2471 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       51 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      250 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 12:50:23.000000 swh.loader.svn-1.8.0/swh.loader.svn.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-06-06 12:50:21.000000 swh.loader.svn-1.8.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      160 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2020 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1092 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      552 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/bin/init-svn-repository.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      761 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/bin/swh-svn
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      391 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     6651 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/docs/swh-loader-svn.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/install/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      644 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/install/install-pysvn.sh
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      109 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/install/install-subvertpy.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      347 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      248 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       96 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/resources/svn.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     5579 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/setup.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5873 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/svn-lib-client-analysis.org
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh/loader/svn/
+-rw-r--r--   0 jenkins    (115) docker     (999)      672 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2427 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2328 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      667 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/exception.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9055 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/fast_crawler.cpp
+-rw-r--r--   0 jenkins    (115) docker     (999)      515 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/fast_crawler.pyi
+-rw-r--r--   0 jenkins    (115) docker     (999)    33376 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)    33988 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/replay.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    25221 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/svn_repo.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1521 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/svn_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1773 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2690 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)   360057 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/httthttt.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   389343 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
+-rw-r--r--   0 jenkins    (115) docker     (999)   419840 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   430080 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   911360 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    28495 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   133120 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    35440 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    30908 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   163840 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    28193 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)   406052 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     3985 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4533 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    62193 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_externals.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2371 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_fast_crawler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    17874 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_loader.org
+-rw-r--r--   0 jenkins    (115) docker     (999)    79798 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4415 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_svn_repo.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12997 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_svn_retry.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_task.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1469 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_task_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      459 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    21336 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3734 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/tests/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16004 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/swh/loader/svn/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2020 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2506 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      102 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      250 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-09 12:26:29.000000 swh.loader.svn-1.8.1/swh.loader.svn.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1531 2023-06-09 12:26:27.000000 swh.loader.svn-1.8.1/tox.ini
```

### Comparing `swh.loader.svn-1.8.0/.pre-commit-config.yaml` & `swh.loader.svn-1.8.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/CODE_OF_CONDUCT.md` & `swh.loader.svn-1.8.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/LICENSE` & `swh.loader.svn-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/PKG-INFO` & `swh.loader.svn-1.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 1.8.0
+Version: 1.8.1
 Summary: Software Heritage Loader SVN
 Home-page: https://forge.softwareheritage.org/diffusion/DLDSVN
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-svn
@@ -33,15 +33,15 @@
 
 - `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
 - `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
-- `swh.loader.svn.directory.SvnDirectoryLoader` which ingests an svn tree at a specific
+- `swh.loader.svn.directory.SvnExportLoader` which ingests an svn tree at a specific
   revision.
 
 ## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
```

### Comparing `swh.loader.svn-1.8.0/README.md` & `swh.loader.svn-1.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 - `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
 - `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
-- `swh.loader.svn.directory.SvnDirectoryLoader` which ingests an svn tree at a specific
+- `swh.loader.svn.directory.SvnExportLoader` which ingests an svn tree at a specific
   revision.
 
 ## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
```

### Comparing `swh.loader.svn-1.8.0/bin/init-svn-repository.sh` & `swh.loader.svn-1.8.1/bin/init-svn-repository.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/bin/swh-svn` & `swh.loader.svn-1.8.1/bin/swh-svn`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/conftest.py` & `swh.loader.svn-1.8.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/docs/swh-loader-svn.txt` & `swh.loader.svn-1.8.1/docs/swh-loader-svn.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/install/install-pysvn.sh` & `swh.loader.svn-1.8.1/install/install-pysvn.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/resources/svn.ini` & `swh.loader.svn-1.8.1/resources/svn.ini`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/setup.py` & `swh.loader.svn-1.8.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,14 +135,15 @@
     setup_requires=["setuptools-scm"],
     use_scm_version=True,
     extras_require={"testing": parse_requirements("test")},
     include_package_data=True,
     entry_points="""
         [swh.workers]
         loader.svn=swh.loader.svn:register
+        loader.svn-export=swh.loader.svn:register_export
     """,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Development Status :: 5 - Production/Stable",
```

### Comparing `swh.loader.svn-1.8.0/svn-lib-client-analysis.org` & `swh.loader.svn-1.8.1/svn-lib-client-analysis.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/converters.py` & `swh.loader.svn-1.8.1/swh/loader/svn/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/directory.py` & `swh.loader.svn-1.8.1/swh/loader/svn/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 from typing import Iterator, Optional
 
 from swh.loader.core.loader import BaseDirectoryLoader
 from swh.loader.svn.svn_repo import SvnRepo, get_svn_repo
 from swh.model.model import Snapshot, SnapshotBranch, TargetType
 
 
-class SvnDirectoryLoader(BaseDirectoryLoader):
-    """Svn tree (directory) loader at a specific commit (revision) or tag (release) into
+class SvnExportLoader(BaseDirectoryLoader):
+    """Svn export (of a tree) loader at a specific svn revision or tag (release) into
     the swh archive.
 
     The output snapshot is of the form:
 
     .. code::
 
        id: <bytes>
```

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/exception.py` & `swh.loader.svn-1.8.1/swh/loader/svn/exception.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.cpp` & `swh.loader.svn-1.8.1/swh/loader/svn/fast_crawler.cpp`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/fast_crawler.pyi` & `swh.loader.svn-1.8.1/swh/loader/svn/fast_crawler.pyi`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/loader.py` & `swh.loader.svn-1.8.1/swh/loader/svn/loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/replay.py` & `swh.loader.svn-1.8.1/swh/loader/svn/replay.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/svn_repo.py` & `swh.loader.svn-1.8.1/swh/loader/svn/svn_repo.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/svn_retry.py` & `swh.loader.svn-1.8.1/swh/loader/svn/svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tasks.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 
 from celery import shared_task
 
 from swh.loader.core.utils import parse_visit_date
 
-from .directory import SvnDirectoryLoader
+from .directory import SvnExportLoader
 from .loader import SvnLoader, SvnLoaderFromDumpArchive, SvnLoaderFromRemoteDump
 
 
 def _process_kwargs(kwargs):
     if "visit_date" in kwargs:
         kwargs["visit_date"] = parse_visit_date(kwargs["visit_date"])
     return kwargs
@@ -43,12 +43,12 @@
     2. Load it through the svn loader.
     3. Clean up mounted svn repository archive.
     """
     loader = SvnLoaderFromRemoteDump.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
 
 
-@shared_task(name=f"{__name__}.LoadSvnDirectory")
-def load_svn_directory(**kwargs):
+@shared_task(name=f"{__name__}.LoadSvnExport")
+def load_svn_export(**kwargs):
     """Load svn tree into the swh archive."""
-    loader = SvnDirectoryLoader.from_configfile(**_process_kwargs(kwargs))
+    loader = SvnExportLoader.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
```

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/conftest.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/httthttt.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/httthttt.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-doc-linux-r12.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-add-remove-dir.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-tampered-rev6-log.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-edge-case-links-and-files.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-external-id.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-updates.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet-with-wrong-link-cases.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pkg-gourmet.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pkg-gourmet.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/data/pyang-repo-r343-eol-native-mixed-lf-crlf.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_converters.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_directory.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_directory.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import os
 
 from swh.loader.core.nar import Nar
-from swh.loader.svn.directory import SvnDirectoryLoader
+from swh.loader.svn.directory import SvnExportLoader
 from swh.loader.svn.svn_repo import get_svn_repo
 from swh.loader.tests import (
     assert_last_visit_matches,
     fetch_nar_extids_from_checksums,
     get_stats,
     prepare_repository_from_archive,
 )
@@ -32,15 +32,15 @@
     archive_path = os.path.join(datadir, f"{archive_name}.tgz")
     repo_url = prepare_repository_from_archive(
         archive_path, archive_name, tmp_path=tmp_path
     )
     svn_revision = 5
     checksums = {"sha256": compute_nar_hash_for_rev(repo_url, svn_revision)}
 
-    loader = SvnDirectoryLoader(
+    loader = SvnExportLoader(
         swh_storage,
         repo_url,
         ref=svn_revision,
         checksum_layout="nar",
         checksums=checksums,
     )
 
@@ -74,15 +74,15 @@
     }
 
     # Ensure the extids got stored as well
     extids = fetch_nar_extids_from_checksums(loader.storage, checksums)
     assert len(extids) == len(checksums)
 
     # Another run on the same svn directory should be uneventful
-    loader2 = SvnDirectoryLoader(
+    loader2 = SvnExportLoader(
         swh_storage,
         repo_url,
         ref=svn_revision,
         checksum_layout="nar",
         checksums=checksums,
     )
     actual_result2 = loader2.load()
@@ -95,15 +95,15 @@
     archive_path = os.path.join(datadir, f"{archive_name}.tgz")
     repo_url = prepare_repository_from_archive(
         archive_path, archive_name, tmp_path=tmp_path
     )
     faulty_checksums = {
         "sha256": "00000ed1855beadfa9c00f730242f5efe3e4612e76f0dcc45215c4a3234c7466"
     }
-    loader = SvnDirectoryLoader(
+    loader = SvnExportLoader(
         swh_storage,
         repo_url,
         ref=5,
         checksum_layout="nar",
         checksums=faulty_checksums,
     )
 
@@ -125,15 +125,15 @@
     # Ensure no extids got stored
     extids = fetch_nar_extids_from_checksums(loader.storage, faulty_checksums)
     assert len(extids) == 0
 
 
 def test_loader_svn_directory_not_found(swh_storage, datadir, tmp_path):
     """Loading a svn tree from an unknown origin should fail"""
-    loader = SvnDirectoryLoader(
+    loader = SvnExportLoader(
         swh_storage,
         "file:///home/origin/does/not/exist",
         ref=5,
         checksum_layout="standard",
         checksums={},
     )
```

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_externals.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_externals.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_fast_crawler.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_fast_crawler.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.org` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_loader.org`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_loader.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_repo.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_svn_repo.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_svn_retry.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_svn_retry.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_task_directory.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_task_directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,12 +40,12 @@
     svn_lister,
     svn_listed_svn_directory_origin,
     extra_loader_arguments,
 ):
     svn_listed_svn_directory_origin.extra_loader_arguments = extra_loader_arguments
 
     loading_task_creation_for_listed_origin_test(
-        loader_class_name=f"{NAMESPACE}.directory.SvnDirectoryLoader",
-        task_function_name=f"{NAMESPACE}.tasks.LoadSvnDirectory",
+        loader_class_name=f"{NAMESPACE}.directory.SvnExportLoader",
+        task_function_name=f"{NAMESPACE}.tasks.LoadSvnExport",
         lister=svn_lister,
         listed_origin=svn_listed_svn_directory_origin,
     )
```

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/test_utils.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/tests/utils.py` & `swh.loader.svn-1.8.1/swh/loader/svn/tests/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh/loader/svn/utils.py` & `swh.loader.svn-1.8.1/swh/loader/svn/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.svn-1.8.0/swh.loader.svn.egg-info/PKG-INFO` & `swh.loader.svn-1.8.1/swh.loader.svn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.svn
-Version: 1.8.0
+Version: 1.8.1
 Summary: Software Heritage Loader SVN
 Home-page: https://forge.softwareheritage.org/diffusion/DLDSVN
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-svn
@@ -33,15 +33,15 @@
 
 - `swh.loader.svn.loader.SvnLoaderFromDumpArchive` which mounts a repository out of a
   svn dump prior to ingest it.
 
 - `swh.loader.svn.loader.SvnLoaderFromRemoteDump` which mounts a repository with
   svnrdump prior to ingest its content.
 
-- `swh.loader.svn.directory.SvnDirectoryLoader` which ingests an svn tree at a specific
+- `swh.loader.svn.directory.SvnExportLoader` which ingests an svn tree at a specific
   revision.
 
 ## CLI run
 
 With the configuration:
 
 /tmp/loader_svn.yml:
```

### Comparing `swh.loader.svn-1.8.0/swh.loader.svn.egg-info/SOURCES.txt` & `swh.loader.svn-1.8.1/swh.loader.svn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 swh/loader/svn/tests/test_fast_crawler.py
 swh/loader/svn/tests/test_loader.org
 swh/loader/svn/tests/test_loader.py
 swh/loader/svn/tests/test_svn_repo.py
 swh/loader/svn/tests/test_svn_retry.py
 swh/loader/svn/tests/test_task.py
 swh/loader/svn/tests/test_task_directory.py
+swh/loader/svn/tests/test_tasks.py
 swh/loader/svn/tests/test_utils.py
 swh/loader/svn/tests/utils.py
 swh/loader/svn/tests/data/httthttt.tgz
 swh/loader/svn/tests/data/mediawiki-repo-r407-eol-native-crlf.tgz
 swh/loader/svn/tests/data/penguinsdbtools2018.dump.gz
 swh/loader/svn/tests/data/pkg-doc-linux-r10.tgz
 swh/loader/svn/tests/data/pkg-doc-linux-r11.tgz
```

### Comparing `swh.loader.svn-1.8.0/tox.ini` & `swh.loader.svn-1.8.1/tox.ini`

 * *Files identical despite different names*

