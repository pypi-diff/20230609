# Comparing `tmp/dvc-data-1.0.2.tar.gz` & `tmp/dvc-data-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-data-1.0.2.tar", last modified: Fri Jun  9 13:05:28 2023, max compression
+gzip compressed data, was "dvc-data-1.0.3.tar", last modified: Fri Jun  9 14:26:46 2023, max compression
```

## Comparing `dvc-data-1.0.2.tar` & `dvc-data-1.0.3.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.685489 dvc-data-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.673488 dvc-data-1.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.677488 dvc-data-1.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.github/workflows/benchmark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-09 13:05:06.000000 dvc-data-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-09 13:05:06.000000 dvc-data-1.0.2/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-09 13:05:06.000000 dvc-data-1.0.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 13:05:06.000000 dvc-data-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 13:05:28.685489 dvc-data-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-09 13:05:06.000000 dvc-data-1.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-09 13:05:06.000000 dvc-data-1.0.2/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-09 13:05:06.000000 dvc-data-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-09 13:05:28.685489 dvc-data-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.673488 dvc-data-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.677488 dvc-data-1.0.2/src/dvc_data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.681488 dvc-data-1.0.2/src/dvc_data/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/_ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/_progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.681488 dvc-data-1.0.2/src/dvc_data/hashfile/db/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/db/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/db/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/db/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/hash_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/hashfile/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.681488 dvc-data-1.0.2/src/dvc_data/index/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/index/view.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-09 13:05:06.000000 dvc-data-1.0.2/src/dvc_data/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.677488 dvc-data-1.0.2/src/dvc_data.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 13:05:28.000000 dvc-data-1.0.2/src/dvc_data.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.681488 dvc-data-1.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.681488 dvc-data-1.0.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/benchmarks/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.681488 dvc-data-1.0.2/tests/hashfile/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_db_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_hash_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_istextfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/hashfile/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:28.685489 dvc-data-1.0.2/tests/index/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/index/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/index/test_checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/index/test_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/index/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 13:05:06.000000 dvc-data-1.0.2/tests/test_dvc_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.182593 dvc-data-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.174594 dvc-data-1.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.174594 dvc-data-1.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.github/workflows/benchmark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-09 14:26:23.000000 dvc-data-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-09 14:26:23.000000 dvc-data-1.0.3/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-09 14:26:23.000000 dvc-data-1.0.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-09 14:26:23.000000 dvc-data-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 14:26:46.182593 dvc-data-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-09 14:26:23.000000 dvc-data-1.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-09 14:26:23.000000 dvc-data-1.0.3/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-09 14:26:23.000000 dvc-data-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-09 14:26:46.182593 dvc-data-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.170594 dvc-data-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.174594 dvc-data-1.0.3/src/dvc_data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.178593 dvc-data-1.0.3/src/dvc_data/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.178593 dvc-data-1.0.3/src/dvc_data/hashfile/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/db/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/db/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/db/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/hash_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5734 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11116 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/hashfile/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.178593 dvc-data-1.0.3/src/dvc_data/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18259 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5105 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/index/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1422 2023-06-09 14:26:23.000000 dvc-data-1.0.3/src/dvc_data/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.174594 dvc-data-1.0.3/src/dvc_data.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3887 2023-06-09 14:26:46.000000 dvc-data-1.0.3/src/dvc_data.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-06-09 14:26:46.000000 dvc-data-1.0.3/src/dvc_data.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:26:46.000000 dvc-data-1.0.3/src/dvc_data.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-09 14:26:46.000000 dvc-data-1.0.3/src/dvc_data.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:26:45.000000 dvc-data-1.0.3/src/dvc_data.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 14:26:46.000000 dvc-data-1.0.3/src/dvc_data.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-09 14:26:46.000000 dvc-data-1.0.3/src/dvc_data.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.178593 dvc-data-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.178593 dvc-data-1.0.3/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/benchmarks/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.182593 dvc-data-1.0.3/tests/hashfile/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_db_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2474 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_hash_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_istextfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/hashfile/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:46.182593 dvc-data-1.0.3/tests/index/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/index/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/index/test_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/index/test_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13499 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/index/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 14:26:23.000000 dvc-data-1.0.3/tests/test_dvc_data.py
```

### Comparing `dvc-data-1.0.2/.cruft.json` & `dvc-data-1.0.3/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/.github/dependabot.yml` & `dvc-data-1.0.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/.github/workflows/benchmark.yml` & `dvc-data-1.0.3/.github/workflows/benchmark.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/.github/workflows/release.yml` & `dvc-data-1.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/.github/workflows/tests.yml` & `dvc-data-1.0.3/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/.gitignore` & `dvc-data-1.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/.pre-commit-config.yaml` & `dvc-data-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/CODE_OF_CONDUCT.rst` & `dvc-data-1.0.3/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/CONTRIBUTING.rst` & `dvc-data-1.0.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/LICENSE` & `dvc-data-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/PKG-INFO` & `dvc-data-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.0.2
+Version: 1.0.3
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.0.2/README.rst` & `dvc-data-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/noxfile.py` & `dvc-data-1.0.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/pyproject.toml` & `dvc-data-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/setup.cfg` & `dvc-data-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/cli.py` & `dvc-data-1.0.3/src/dvc_data/cli.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/fs.py` & `dvc-data-1.0.3/src/dvc_data/fs.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/__init__.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/_progress.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/_progress.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/build.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/cache.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/checkout.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/db/__init__.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/db/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/db/index.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/db/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/db/local.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/db/local.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/db/reference.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/db/reference.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/diff.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/gc.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/gc.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/hash.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/hash_info.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/hash_info.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/istextfile.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/meta.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/meta.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/state.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/state.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/status.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/status.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/transfer.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/transfer.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/tree.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/hashfile/utils.py` & `dvc-data-1.0.3/src/dvc_data/hashfile/utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/__init__.py` & `dvc-data-1.0.3/src/dvc_data/index/__init__.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/add.py` & `dvc-data-1.0.3/src/dvc_data/index/add.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/build.py` & `dvc-data-1.0.3/src/dvc_data/index/build.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/checkout.py` & `dvc-data-1.0.3/src/dvc_data/index/checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/diff.py` & `dvc-data-1.0.3/src/dvc_data/index/diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/fetch.py` & `dvc-data-1.0.3/src/dvc_data/index/fetch.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/index.py` & `dvc-data-1.0.3/src/dvc_data/index/index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/save.py` & `dvc-data-1.0.3/src/dvc_data/index/save.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,23 @@
 
 def _save_dir_entry(
     index: "BaseDataIndex",
     key: "DataIndexKey",
     odb: Optional["HashFileDB"] = None,
 ) -> None:
     from ..hashfile.db import add_update_tree
+    from .index import StorageKeyError
 
     entry = index[key]
-    cache = odb or index.storage_map.get_cache_odb(entry)
+
+    try:
+        cache = odb or index.storage_map.get_cache_odb(entry)
+    except StorageKeyError:
+        return
+
     assert cache
     meta, tree = build_tree(index, key)
     tree = add_update_tree(cache, tree)
     entry.meta = meta
     entry.hash_info = tree.hash_info
     assert tree.hash_info.name and tree.hash_info.value
     setattr(entry.meta, tree.hash_info.name, tree.hash_info.value)
```

### Comparing `dvc-data-1.0.2/src/dvc_data/index/serialize.py` & `dvc-data-1.0.3/src/dvc_data/index/serialize.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/index/view.py` & `dvc-data-1.0.3/src/dvc_data/index/view.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data/repo.py` & `dvc-data-1.0.3/src/dvc_data/repo.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data.egg-info/PKG-INFO` & `dvc-data-1.0.3/src/dvc_data.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-data
-Version: 1.0.2
+Version: 1.0.3
 Summary: dvc data
 Home-page: https://github.com/iterative/dvc-data
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `dvc-data-1.0.2/src/dvc_data.egg-info/SOURCES.txt` & `dvc-data-1.0.3/src/dvc_data.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/src/dvc_data.egg-info/requires.txt` & `dvc-data-1.0.3/src/dvc_data.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/benchmarks/test_checkout.py` & `dvc-data-1.0.3/tests/benchmarks/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_cache.py` & `dvc-data-1.0.3/tests/hashfile/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_db_index.py` & `dvc-data-1.0.3/tests/hashfile/test_db_index.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_diff.py` & `dvc-data-1.0.3/tests/hashfile/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_hash.py` & `dvc-data-1.0.3/tests/hashfile/test_hash.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_hash_stream.py` & `dvc-data-1.0.3/tests/hashfile/test_hash_stream.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_istextfile.py` & `dvc-data-1.0.3/tests/hashfile/test_istextfile.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_tree.py` & `dvc-data-1.0.3/tests/hashfile/test_tree.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/hashfile/test_utils.py` & `dvc-data-1.0.3/tests/hashfile/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/index/conftest.py` & `dvc-data-1.0.3/tests/index/conftest.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/index/test_checkout.py` & `dvc-data-1.0.3/tests/index/test_checkout.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/index/test_diff.py` & `dvc-data-1.0.3/tests/index/test_diff.py`

 * *Files identical despite different names*

### Comparing `dvc-data-1.0.2/tests/index/test_index.py` & `dvc-data-1.0.3/tests/index/test_index.py`

 * *Files identical despite different names*

