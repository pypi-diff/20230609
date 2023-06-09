# Comparing `tmp/swh.loader.git-2.4.0.tar.gz` & `tmp/swh.loader.git-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.git-2.4.0.tar", last modified: Tue Jun  6 12:46:27 2023, max compression
+gzip compressed data, was "dist/swh.loader.git-2.5.0.tar", last modified: Fri Jun  9 15:25:27 2023, max compression
```

## Comparing `swh.loader.git-2.4.0.tar` & `swh.loader.git-2.5.0.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2954 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2027 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/bin/
--rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/bin/dir-git-repo-meta.sh
--rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/_templates/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/docs/attic/
--rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/attic/api-backend-protocol.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/attic/git-loading-design.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       35 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/requirements.txt
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/resources/
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/local-loader-git.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/remote-loader-git.ini
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/resources/test/
--rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/test/back.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/test/db-manager.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/resources/updater.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2387 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/
--rw-r--r--   0 jenkins    (115) docker     (999)      653 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/base.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9923 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8043 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/dumb.py
--rw-r--r--   0 jenkins    (115) docker     (999)    15273 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    27520 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     1904 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1331 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/git-repos/
--rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle
--rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/data/testrepo.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5875 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_from_disk.py
--rw-r--r--   0 jenkins    (115) docker     (999)    39895 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2390 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1261 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2799 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5449 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/swh/loader/git/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2954 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1576 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      103 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      256 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 12:46:27.000000 swh.loader.git-2.4.0/swh.loader.git.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-06-06 12:46:24.000000 swh.loader.git-2.4.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      290 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2953 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2026 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/bin/
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      605 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/bin/dir-git-repo-meta.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)      567 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/_templates/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/docs/attic/
+-rw-r--r--   0 jenkins    (115) docker     (999)     6851 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/attic/api-backend-protocol.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     5476 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/attic/git-loading-design.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      360 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      399 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      241 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      109 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      115 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       33 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/requirements.txt
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/resources/
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/resources/local-loader-git.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/resources/remote-loader-git.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/resources/test/
+-rw-r--r--   0 jenkins    (115) docker     (999)      502 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/resources/test/back.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      125 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/resources/test/db-manager.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      307 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/resources/updater.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2448 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh/loader/git/
+-rw-r--r--   0 jenkins    (115) docker     (999)      842 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4603 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/base.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9923 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2730 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8043 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/dumb.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    15273 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    27520 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     1900 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh/loader/git/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)      251 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1331 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh/loader/git/tests/data/
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh/loader/git/tests/data/git-repos/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5433 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle
+-rw-r--r--   0 jenkins    (115) docker     (999)    10630 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/data/testrepo.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)    33966 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5871 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    20607 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_from_disk.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    39895 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2602 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1259 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_tasks_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2799 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5449 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/swh/loader/git/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2953 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1576 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      158 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      254 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-09 15:25:27.000000 swh.loader.git-2.5.0/swh.loader.git.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-06-09 15:25:26.000000 swh.loader.git-2.5.0/tox.ini
```

### Comparing `swh.loader.git-2.4.0/.pre-commit-config.yaml` & `swh.loader.git-2.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/CODE_OF_CONDUCT.md` & `swh.loader.git-2.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/LICENSE` & `swh.loader.git-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/PKG-INFO` & `swh.loader.git-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.4.0
+Version: 2.5.0
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
@@ -35,15 +35,15 @@
 
 - :class:`swh.loader.git.from_disk.GitLoaderFromDisk` which ingests only local git clone
   repository.
 
 - :class:`swh.loader.git.loader.GitLoaderFromArchive` which ingests a git repository
   wrapped in an archive.
 
-- :class:`swh.loader.git.directory.GitDirectoryLoader` which ingests a git tree at a
+- :class:`swh.loader.git.directory.GitCheckoutLoader` which ingests a git tree at a
   specific commit, branch or tag.
 
 
 License
 -------
 
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `swh.loader.git-2.4.0/README.md` & `swh.loader.git-2.5.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 - :class:`swh.loader.git.from_disk.GitLoaderFromDisk` which ingests only local git clone
   repository.
 
 - :class:`swh.loader.git.loader.GitLoaderFromArchive` which ingests a git repository
   wrapped in an archive.
 
-- :class:`swh.loader.git.directory.GitDirectoryLoader` which ingests a git tree at a
+- :class:`swh.loader.git.directory.GitCheckoutLoader` which ingests a git tree at a
   specific commit, branch or tag.
 
 
 License
 -------
 
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `swh.loader.git-2.4.0/bin/dir-git-repo-meta.sh` & `swh.loader.git-2.5.0/bin/dir-git-repo-meta.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/conftest.py` & `swh.loader.git-2.5.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/docs/attic/api-backend-protocol.txt` & `swh.loader.git-2.5.0/docs/attic/api-backend-protocol.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/docs/attic/git-loading-design.txt` & `swh.loader.git-2.5.0/docs/attic/git-loading-design.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/setup.py` & `swh.loader.git-2.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
     use_scm_version=True,
     extras_require={"testing": parse_requirements("test")},
     include_package_data=True,
     entry_points="""
         [swh.workers]
         loader.git=swh.loader.git:register
         loader.git_disk=swh.loader.git:register_from_disk
+        loader.git-checkout=swh.loader.git:register_checkout
     """,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Development Status :: 5 - Production/Stable",
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/__init__.py` & `swh.loader.git-2.5.0/swh/loader/git/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,16 @@
 def register_from_disk() -> Dict[str, Any]:
     from swh.loader.git.from_disk import GitLoaderFromDisk
 
     return {
         "task_modules": [],
         "loader": GitLoaderFromDisk,
     }
+
+
+def register_checkout() -> Dict[str, Any]:
+    from swh.loader.git.directory import GitCheckoutLoader
+
+    return {
+        "task_modules": [],
+        "loader": GitCheckoutLoader,
+    }
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/base.py` & `swh.loader.git-2.5.0/swh/loader/git/base.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/converters.py` & `swh.loader.git-2.5.0/swh/loader/git/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/directory.py` & `swh.loader.git-2.5.0/swh/loader/git/directory.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     if commit_ref:
         checkout_branch(repo, git_ref)
 
     return repo
 
 
-class GitDirectoryLoader(BaseDirectoryLoader):
+class GitCheckoutLoader(BaseDirectoryLoader):
     """Git directory loader in charge of ingesting a git tree at a specific commit, tag
     or branch into the swh archive.
 
     The output snapshot is of the form:
 
     .. code::
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/dumb.py` & `swh.loader.git-2.5.0/swh/loader/git/dumb.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/from_disk.py` & `swh.loader.git-2.5.0/swh/loader/git/from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/loader.py` & `swh.loader.git-2.5.0/swh/loader/git/loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tasks.py` & `swh.loader.git-2.5.0/swh/loader/git/tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # See top-level LICENSE file for more information
 
 from typing import Any, Dict
 
 from celery import shared_task
 
 from swh.loader.core.utils import parse_visit_date
-from swh.loader.git.directory import GitDirectoryLoader
+from swh.loader.git.directory import GitCheckoutLoader
 from swh.loader.git.from_disk import GitLoaderFromArchive, GitLoaderFromDisk
 from swh.loader.git.loader import GitLoader
 
 
 def _process_kwargs(kwargs):
     if "visit_date" in kwargs:
         kwargs["visit_date"] = parse_visit_date(kwargs["visit_date"])
@@ -42,12 +42,12 @@
     3. Clean up the temporary folder
 
     """
     loader = GitLoaderFromArchive.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
 
 
-@shared_task(name=__name__ + ".LoadGitDirectory")
-def load_git_directory(**kwargs) -> Dict[str, Any]:
+@shared_task(name=__name__ + ".LoadGitCheckout")
+def load_git_checkout(**kwargs) -> Dict[str, Any]:
     """Load a git tree at a specific commit, tag or branch."""
-    loader = GitDirectoryLoader.from_configfile(**_process_kwargs(kwargs))
+    loader = GitCheckoutLoader.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/conftest.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle` & `swh.loader.git-2.5.0/swh/loader/git/tests/data/git-repos/example-submodule.bundle`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/data/testrepo.tgz` & `swh.loader.git-2.5.0/swh/loader/git/tests/data/testrepo.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_converters.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_directory.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_directory.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from pathlib import Path
 from typing import Tuple
 
 import pytest
 
 from swh.loader.core.nar import Nar
-from swh.loader.git.directory import GitDirectoryLoader, clone_repository
+from swh.loader.git.directory import GitCheckoutLoader, clone_repository
 from swh.loader.tests import (
     assert_last_visit_matches,
     fetch_nar_extids_from_checksums,
     get_stats,
     prepare_repository_from_archive,
 )
 
@@ -88,15 +88,15 @@
     _, repo_url = prepare_test_git_clone(
         archive_path, archive_name, tmp_path, reference
     )
 
     checksums = {
         "sha256": compute_nar_hash_for_ref(repo_url, reference, "sha256", tmp_path)
     }
-    loader = GitDirectoryLoader(
+    loader = GitCheckoutLoader(
         swh_storage,
         repo_url,
         ref=reference,
         checksum_layout="nar",
         checksums=checksums,
     )
 
@@ -130,15 +130,15 @@
     _, repo_url = prepare_test_git_clone(
         archive_path, archive_name, tmp_path, release_name
     )
 
     reference = "branch2-before-delete"
     truthy_checksums = compute_nar_hash_for_ref(repo_url, reference, "sha256", tmp_path)
     faulty_checksums = {"sha256": truthy_checksums.replace("5", "0")}
-    loader = GitDirectoryLoader(
+    loader = GitCheckoutLoader(
         swh_storage,
         repo_url,
         ref=reference,
         checksum_layout="nar",
         checksums=faulty_checksums,
     )
 
@@ -160,15 +160,15 @@
     # Ensure no extids got stored
     extids = fetch_nar_extids_from_checksums(loader.storage, faulty_checksums)
     assert len(extids) == 0
 
 
 def test_loader_git_directory_not_found(swh_storage, datadir, tmp_path):
     """Loading a git tree from an unknown origin should fail"""
-    loader = GitDirectoryLoader(
+    loader = GitCheckoutLoader(
         swh_storage,
         "file:///home/origin/does/not/exist",
         ref="not-important",
         checksum_layout="standard",
         checksums={},
     )
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_from_disk.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_from_disk.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_loader.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,26 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 import pytest
 
+from swh.loader.tests import assert_module_tasks_are_scheduler_ready
 from swh.scheduler.model import ListedOrigin
 
 from .conftest import NAMESPACE
 
 
+def test_tasks_loader_visit_type_match_task_name():
+    import swh.loader.git
+
+    assert_module_tasks_are_scheduler_ready([swh.loader.git])
+
+
 @pytest.fixture
 def git_listed_origin(git_lister):
     return ListedOrigin(
         lister_id=git_lister.id, url="https://git.example.org/repo", visit_type="git"
     )
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_tasks_directory.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_tasks_directory.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,12 +32,12 @@
     git_lister,
     git_listed_origin,
     extra_loader_arguments,
 ):
     git_listed_origin.extra_loader_arguments = extra_loader_arguments
 
     loading_task_creation_for_listed_origin_test(
-        loader_class_name=f"{NAMESPACE}.directory.GitDirectoryLoader",
-        task_function_name=f"{NAMESPACE}.tasks.LoadGitDirectory",
+        loader_class_name=f"{NAMESPACE}.directory.GitCheckoutLoader",
+        task_function_name=f"{NAMESPACE}.tasks.LoadGitCheckout",
         lister=git_lister,
         listed_origin=git_listed_origin,
     )
```

### Comparing `swh.loader.git-2.4.0/swh/loader/git/tests/test_utils.py` & `swh.loader.git-2.5.0/swh/loader/git/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh/loader/git/utils.py` & `swh.loader.git-2.5.0/swh/loader/git/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/swh.loader.git.egg-info/PKG-INFO` & `swh.loader.git-2.5.0/swh.loader.git.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.git
-Version: 2.4.0
+Version: 2.5.0
 Summary: Software Heritage git loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-git
@@ -35,15 +35,15 @@
 
 - :class:`swh.loader.git.from_disk.GitLoaderFromDisk` which ingests only local git clone
   repository.
 
 - :class:`swh.loader.git.loader.GitLoaderFromArchive` which ingests a git repository
   wrapped in an archive.
 
-- :class:`swh.loader.git.directory.GitDirectoryLoader` which ingests a git tree at a
+- :class:`swh.loader.git.directory.GitCheckoutLoader` which ingests a git tree at a
   specific commit, branch or tag.
 
 
 License
 -------
 
 This program is free software: you can redistribute it and/or modify it
```

### Comparing `swh.loader.git-2.4.0/swh.loader.git.egg-info/SOURCES.txt` & `swh.loader.git-2.5.0/swh.loader.git.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.git-2.4.0/tox.ini` & `swh.loader.git-2.5.0/tox.ini`

 * *Files identical despite different names*

