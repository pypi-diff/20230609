# Comparing `tmp/swh.loader.mercurial-3.3.0.tar.gz` & `tmp/swh.loader.mercurial-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.loader.mercurial-3.3.0.tar", last modified: Tue Jun  6 12:48:47 2023, max compression
+gzip compressed data, was "dist/swh.loader.mercurial-3.4.0.tar", last modified: Fri Jun  9 13:51:55 2023, max compression
```

## Comparing `swh.loader.mercurial-3.3.0.tar` & `swh.loader.mercurial-3.4.0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      114 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       22 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      166 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1799 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      860 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      578 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      548 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)      195 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      148 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/
--rw-r--r--   0 jenkins    (115) docker     (999)      510 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1981 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/archive_extract.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2806 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5143 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/hgutil.py
--rw-r--r--   0 jenkins    (115) docker     (999)    16613 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/identify.py
--rw-r--r--   0 jenkins    (115) docker     (999)    29492 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     1473 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tasks.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)  2757941 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/anomad-d.tgz
--rwxr-xr-x   0 jenkins    (115) docker     (999)     7621 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/build.py
--rw-r--r--   0 jenkins    (115) docker     (999)      897 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.json
--rw-r--r--   0 jenkins    (115) docker     (999)     1392 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    51200 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      411 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/hello.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3070 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/hello.tgz
--rwxr-xr-x   0 jenkins    (115) docker     (999)      465 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/missing-filelog.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    40960 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/missing-filelog.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.json
--rw-r--r--   0 jenkins    (115) docker     (999)      448 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.sh
--rw-r--r--   0 jenkins    (115) docker     (999)    40960 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     5209 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.json
--rw-r--r--   0 jenkins    (115) docker     (999)    13309 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)      633 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.json
--rw-r--r--   0 jenkins    (115) docker     (999)     3206 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.tgz
--rw-r--r--   0 jenkins    (115) docker     (999)     2353 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/loader_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_converters.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6238 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3016 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_identify.py
--rw-r--r--   0 jenkins    (115) docker     (999)    26197 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_loader.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1746 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1440 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_tasks_directory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1462 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/swh/loader/mercurial/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1799 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     2158 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      135 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      300 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-06 12:48:47.000000 swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1549 2023-06-06 12:48:45.000000 swh.loader.mercurial-3.3.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      114 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      117 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       22 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      166 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1798 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      859 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      578 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      394 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      548 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)      195 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       90 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      148 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      333 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2527 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh/loader/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/
+-rw-r--r--   0 jenkins    (115) docker     (999)      745 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1981 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/archive_extract.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1040 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2805 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5143 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/hgutil.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    16613 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/identify.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    29492 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     1468 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tasks.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)  2757941 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/anomad-d.tgz
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     7621 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/build.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      897 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/example.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     1392 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/example.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    51200 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/example.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      411 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/hello.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3070 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/hello.tgz
+-rwxr-xr-x   0 jenkins    (115) docker     (999)      465 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/missing-filelog.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    40960 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/missing-filelog.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      456 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/multiple-heads.json
+-rw-r--r--   0 jenkins    (115) docker     (999)      448 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/multiple-heads.sh
+-rw-r--r--   0 jenkins    (115) docker     (999)    40960 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/multiple-heads.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     5209 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/the-sandbox.json
+-rw-r--r--   0 jenkins    (115) docker     (999)    13309 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/the-sandbox.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)      633 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/transplant.json
+-rw-r--r--   0 jenkins    (115) docker     (999)     3206 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/transplant.tgz
+-rw-r--r--   0 jenkins    (115) docker     (999)     2353 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/loader_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2155 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_converters.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6234 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3016 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_identify.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    26197 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_loader.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1970 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1438 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_tasks_directory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1462 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/swh/loader/mercurial/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1798 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     2158 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      202 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      300 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-09 13:51:55.000000 swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1549 2023-06-09 13:51:53.000000 swh.loader.mercurial-3.4.0/tox.ini
```

### Comparing `swh.loader.mercurial-3.3.0/.pre-commit-config.yaml` & `swh.loader.mercurial-3.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/CODE_OF_CONDUCT.md` & `swh.loader.mercurial-3.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/LICENSE` & `swh.loader.mercurial-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/PKG-INFO` & `swh.loader.mercurial-3.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.mercurial
-Version: 3.3.0
+Version: 3.4.0
 Summary: Software Heritage Mercurial Loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDHG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-mercurial
@@ -30,15 +30,15 @@
 The main entry points are:
 - :class:`swh.loader.mercurial.loader.HgLoader` which reads and loads a local
   repository into an SWH archive.
 
 - :class:`swh.loader.mercurial.loader.HgArchiveLoader` which reads and loads
   a local repository wrapped within a tarball
 
-- :class:`swh.loader.mercurial.directory.HgDirectoryLoader` which ingests the hg tree at
+- :class:`swh.loader.mercurial.directory.HgCheckoutLoader` which ingests the hg tree at
   a specific changeset or tag.
 
 # CLI run
 
 ## Configuration file
 
 /tmp/mercurial.yml:
```

### Comparing `swh.loader.mercurial-3.3.0/README.md` & `swh.loader.mercurial-3.4.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 The main entry points are:
 - :class:`swh.loader.mercurial.loader.HgLoader` which reads and loads a local
   repository into an SWH archive.
 
 - :class:`swh.loader.mercurial.loader.HgArchiveLoader` which reads and loads
   a local repository wrapped within a tarball
 
-- :class:`swh.loader.mercurial.directory.HgDirectoryLoader` which ingests the hg tree at
+- :class:`swh.loader.mercurial.directory.HgCheckoutLoader` which ingests the hg tree at
   a specific changeset or tag.
 
 # CLI run
 
 ## Configuration file
 
 /tmp/mercurial.yml:
```

### Comparing `swh.loader.mercurial-3.3.0/conftest.py` & `swh.loader.mercurial-3.4.0/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/mypy.ini` & `swh.loader.mercurial-3.4.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/setup.py` & `swh.loader.mercurial-3.4.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     setup_requires=["setuptools-scm"],
     use_scm_version=True,
     extras_require={"testing": parse_requirements("test")},
     include_package_data=True,
     entry_points="""
         [swh.workers]
         loader.mercurial=swh.loader.mercurial:register
+        loader.mercurial-checkout=swh.loader.mercurial:register_checkout
         [console_scripts]
         swh-hg-identify=swh.loader.mercurial.identify:main
     """,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/archive_extract.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/archive_extract.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/converters.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/directory.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/directory.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     with raise_not_found_repository():
         clone(repo_url, str(local_clone_dir), rev=hg_changeset)
 
     return local_clone_dir
 
 
-class HgDirectoryLoader(BaseDirectoryLoader):
+class HgCheckoutLoader(BaseDirectoryLoader):
     """Hg directory loader in charge of ingesting a mercurial tree at a specific
     changeset, tag or branch into the swh archive.
 
     The output snapshot is of the form:
 
     .. code::
```

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/hgutil.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/hgutil.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/identify.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/identify.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/loader.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tasks.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from celery import shared_task
 
 from swh.loader.core.utils import parse_visit_date
-from swh.loader.mercurial.directory import HgDirectoryLoader
+from swh.loader.mercurial.directory import HgCheckoutLoader
 
 from .loader import HgArchiveLoader, HgLoader
 
 
 def _process_kwargs(kwargs):
     if "visit_date" in kwargs:
         kwargs["visit_date"] = parse_visit_date(kwargs["visit_date"])
@@ -36,15 +36,15 @@
 
     Args: see :func:`HgArchiveLoader` constructor.
     """
     loader = HgArchiveLoader.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
 
 
-@shared_task(name=__name__ + ".LoadMercurialDirectory")
-def load_hg_directory(**kwargs):
+@shared_task(name=f"{__name__}.LoadMercurialCheckout")
+def load_hg_checkout(**kwargs):
     """Import a mercurial tree into swh.
 
-    Args: see :func:`HgDirectoryLoader` constructor.
+    Args: see :func:`HgCheckoutLoader` constructor.
     """
-    loader = HgDirectoryLoader.from_configfile(**_process_kwargs(kwargs))
+    loader = HgCheckoutLoader.from_configfile(**_process_kwargs(kwargs))
     return loader.load()
```

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/conftest.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/anomad-d.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/anomad-d.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/build.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/build.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.json` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/example.json`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.sh` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/example.sh`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/example.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/example.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/hello.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/hello.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/missing-filelog.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/missing-filelog.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/multiple-heads.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/multiple-heads.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.json` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/the-sandbox.json`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/the-sandbox.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/the-sandbox.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.json` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/transplant.json`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/data/transplant.tgz` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/data/transplant.tgz`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/loader_checker.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/loader_checker.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_converters.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_directory.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_directory.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import os
 from pathlib import Path
 
 import pytest
 
 from swh.loader.core.nar import Nar
 from swh.loader.exception import NotFound
-from swh.loader.mercurial.directory import HgDirectoryLoader, clone_repository
+from swh.loader.mercurial.directory import HgCheckoutLoader, clone_repository
 from swh.loader.mercurial.hgutil import repository
 from swh.loader.tests import (
     assert_last_visit_matches,
     fetch_nar_extids_from_checksums,
     get_stats,
     prepare_repository_from_archive,
 )
@@ -91,15 +91,15 @@
     repo_url = prepare_repository_from_archive(
         archive_path, archive_name, tmp_path=tmp_path
     )
 
     hash_algo = "sha256"
     nar_ref = compute_nar_hash_for_ref(repo_url, reference, hash_algo, tmp_path)
     checksums = {hash_algo: nar_ref}
-    loader = HgDirectoryLoader(
+    loader = HgCheckoutLoader(
         swh_storage,
         repo_url,
         ref=reference,
         checksum_layout="nar",
         checksums=checksums,
     )
 
@@ -137,15 +137,15 @@
     repo_url = prepare_repository_from_archive(
         archive_path, archive_name, tmp_path=tmp_path
     )
 
     reference = "default"
     truthy_checksums = compute_nar_hash_for_ref(repo_url, reference, "sha256", tmp_path)
     faulty_checksums = {"sha256": truthy_checksums.replace("5", "0")}
-    loader = HgDirectoryLoader(
+    loader = HgCheckoutLoader(
         swh_storage,
         repo_url,
         ref=reference,
         checksum_layout="nar",
         checksums=faulty_checksums,
     )
 
@@ -175,15 +175,15 @@
     extids = fetch_nar_extids_from_checksums(loader.storage, faulty_checksums)
     assert extids == []
 
 
 def test_hg_directory_loader_not_found(swh_storage, datadir, tmp_path):
     """Loading a hg tree from an unknown origin should result in a not-found visit"""
     repo_url = "file:///origin/does/not/exist"
-    loader = HgDirectoryLoader(
+    loader = HgCheckoutLoader(
         swh_storage,
         repo_url,
         ref="not-important",
         checksum_layout="standard",
         checksums={},
     )
```

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_identify.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_identify.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_loader.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_loader.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_tasks.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_tasks.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 # Copyright (C) 2018-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import pytest
 
+from swh.loader.tests import assert_module_tasks_are_scheduler_ready
 from swh.scheduler.model import ListedOrigin
 
 from .conftest import NAMESPACE
 
 
+def test_tasks_loader_visit_type_match_task_name():
+    import swh.loader.mercurial
+
+    assert_module_tasks_are_scheduler_ready([swh.loader.mercurial])
+
+
 @pytest.fixture
 def hg_listed_origin(hg_lister):
     return ListedOrigin(
         lister_id=hg_lister.id, url="https://hg.example.org/repo", visit_type="hg"
     )
```

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/tests/test_tasks_directory.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/tests/test_tasks_directory.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,12 +40,12 @@
     hg_lister,
     hg_listed_origin,
     extra_loader_arguments,
 ):
     hg_listed_origin.extra_loader_arguments = extra_loader_arguments
 
     loading_task_creation_for_listed_origin_test(
-        loader_class_name=f"{NAMESPACE}.directory.HgDirectoryLoader",
-        task_function_name=f"{NAMESPACE}.tasks.LoadMercurialDirectory",
+        loader_class_name=f"{NAMESPACE}.directory.HgCheckoutLoader",
+        task_function_name=f"{NAMESPACE}.tasks.LoadMercurialCheckout",
         lister=hg_lister,
         listed_origin=hg_listed_origin,
     )
```

### Comparing `swh.loader.mercurial-3.3.0/swh/loader/mercurial/utils.py` & `swh.loader.mercurial-3.4.0/swh/loader/mercurial/utils.py`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/PKG-INFO` & `swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.loader.mercurial
-Version: 3.3.0
+Version: 3.4.0
 Summary: Software Heritage Mercurial Loader
 Home-page: https://forge.softwareheritage.org/diffusion/DLDHG/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-loader-mercurial
@@ -30,15 +30,15 @@
 The main entry points are:
 - :class:`swh.loader.mercurial.loader.HgLoader` which reads and loads a local
   repository into an SWH archive.
 
 - :class:`swh.loader.mercurial.loader.HgArchiveLoader` which reads and loads
   a local repository wrapped within a tarball
 
-- :class:`swh.loader.mercurial.directory.HgDirectoryLoader` which ingests the hg tree at
+- :class:`swh.loader.mercurial.directory.HgCheckoutLoader` which ingests the hg tree at
   a specific changeset or tag.
 
 # CLI run
 
 ## Configuration file
 
 /tmp/mercurial.yml:
```

### Comparing `swh.loader.mercurial-3.3.0/swh.loader.mercurial.egg-info/SOURCES.txt` & `swh.loader.mercurial-3.4.0/swh.loader.mercurial.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.loader.mercurial-3.3.0/tox.ini` & `swh.loader.mercurial-3.4.0/tox.ini`

 * *Files identical despite different names*

