# Comparing `tmp/bomf-0.5.8.tar.gz` & `tmp/bomf-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bomf-0.5.8.tar", last modified: Wed Jun  7 22:50:47 2023, max compression
+gzip compressed data, was "bomf-0.5.9.tar", last modified: Fri Jun  9 13:21:33 2023, max compression
```

## Comparing `bomf-0.5.8.tar` & `bomf-0.5.9.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.244782 bomf-0.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.236782 bomf-0.5.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/packaging_test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/pythonlint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-07 22:50:37.000000 bomf-0.5.8/.github/workflows/unittests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-07 22:50:37.000000 bomf-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-07 22:50:37.000000 bomf-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-07 22:50:37.000000 bomf-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-07 22:50:47.244782 bomf-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-07 22:50:37.000000 bomf-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-07 22:50:37.000000 bomf-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-07 22:50:37.000000 bomf-0.5.8/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-07 22:50:37.000000 bomf-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-07 22:50:47.244782 bomf-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 22:50:37.000000 bomf-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.236782 bomf-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/filter/
--rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/filter/sourcedataproviderfilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/loader/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/loader/entityloader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/mapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/model/
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf/validation/
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.244782 bomf-0.5.8/src/bomf/validation/core/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/core/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/path_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/query_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-07 22:50:37.000000 bomf-0.5.8/src/bomf/validation/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.240782 bomf-0.5.8/src/bomf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-07 22:50:47.000000 bomf-0.5.8/src/bomf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-07 22:50:47.000000 bomf-0.5.8/src/bomf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:50:47.000000 bomf-0.5.8/src/bomf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:50:47.000000 bomf-0.5.8/src/bomf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-07 22:50:47.000000 bomf-0.5.8/src/bomf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 22:50:47.000000 bomf-0.5.8/src/bomf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-07 22:50:37.000000 bomf-0.5.8/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:50:47.244782 bomf-0.5.8/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/example_source_data.json
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_bo4e_data_set.py
--rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_entity_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_list_conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_source_data_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-07 22:50:37.000000 bomf-0.5.8/unittests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/packaging_test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/pythonlint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 13:21:25.000000 bomf-0.5.9/.github/workflows/unittests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-09 13:21:25.000000 bomf-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-09 13:21:25.000000 bomf-0.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-09 13:21:25.000000 bomf-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-09 13:21:33.478128 bomf-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-09 13:21:25.000000 bomf-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-09 13:21:25.000000 bomf-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 13:21:25.000000 bomf-0.5.9/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-09 13:21:25.000000 bomf-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-09 13:21:33.482128 bomf-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-09 13:21:25.000000 bomf-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.474128 bomf-0.5.9/src/bomf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)     6292 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/filter/sourcedataproviderfilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/loader/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7835 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/loader/entityloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/mapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     4928 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf/validation/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7672 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17577 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/core/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/path_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10855 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/query_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-09 13:21:25.000000 bomf-0.5.9/src/bomf/validation/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/src/bomf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 13:21:33.000000 bomf-0.5.9/src/bomf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-09 13:21:25.000000 bomf-0.5.9/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:21:33.478128 bomf-0.5.9/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/example_source_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_bo4e_data_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5290 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_entity_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_list_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_source_data_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-06-09 13:21:25.000000 bomf-0.5.9/unittests/test_validation.py
```

### Comparing `bomf-0.5.8/.github/dependabot.yml` & `bomf-0.5.9/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/black.yml` & `bomf-0.5.9/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/codeql-analysis.yml` & `bomf-0.5.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/coverage.yml` & `bomf-0.5.9/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/packaging_test.yml` & `bomf-0.5.9/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/python-publish.yml` & `bomf-0.5.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/pythonlint.yml` & `bomf-0.5.9/.github/workflows/pythonlint.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.github/workflows/unittests.yml` & `bomf-0.5.9/.github/workflows/unittests.yml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.gitignore` & `bomf-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/.pre-commit-config.yaml` & `bomf-0.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/LICENSE` & `bomf-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/PKG-INFO` & `bomf-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.8
+Version: 0.5.9
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.8/README.md` & `bomf-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/pyproject.toml` & `bomf-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/requirements.txt` & `bomf-0.5.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/setup.cfg` & `bomf-0.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/__init__.py` & `bomf-0.5.9/src/bomf/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/filter/__init__.py` & `bomf-0.5.9/src/bomf/filter/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/filter/sourcedataproviderfilter.py` & `bomf-0.5.9/src/bomf/filter/sourcedataproviderfilter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/loader/entityloader.py` & `bomf-0.5.9/src/bomf/loader/entityloader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/mapper/__init__.py` & `bomf-0.5.9/src/bomf/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/model/__init__.py` & `bomf-0.5.9/src/bomf/model/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/provider/__init__.py` & `bomf-0.5.9/src/bomf/provider/__init__.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/core/analysis.py` & `bomf-0.5.9/src/bomf/validation/core/analysis.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/core/errors.py` & `bomf-0.5.9/src/bomf/validation/core/errors.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/core/execution.py` & `bomf-0.5.9/src/bomf/validation/core/execution.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/core/types.py` & `bomf-0.5.9/src/bomf/validation/core/types.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/core/utils.py` & `bomf-0.5.9/src/bomf/validation/core/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/core/validator.py` & `bomf-0.5.9/src/bomf/validation/core/validator.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/path_map.py` & `bomf-0.5.9/src/bomf/validation/path_map.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf/validation/query_map.py` & `bomf-0.5.9/src/bomf/validation/query_map.py`

 * *Files 3% similar despite different names*

```diff
@@ -151,28 +151,34 @@
     def provide(self, data_set: DataSetT) -> Generator[Parameters[DataSetT] | Exception, None, None]:
         """
         Provides the parameter map to the ValidationManager. For each parameter in the defined parameter mapping the
         query will be evaluated against the data set. Generally, these queries can return more than one value (for
         each parameter). The validator will be executed against all possible combinations of all parameter values.
         If a parameter list could not be filled correctly an error will be yielded instead.
         """
-        ordered_param_map = OrderedDict(self.param_map)
-        param_iterables = [
-            query.iterable(data_set, include_exceptions=param_name in self.validator.optional_param_names)
-            for param_name, query in ordered_param_map.items()
-        ]
+        param_iterables = {
+            param_name: query.iterable(data_set, include_exceptions=param_name in self.validator.optional_param_names)
+            for param_name, query in self.param_map.items()
+        }
         # I want to exclude exceptions from the iterables for required parameters because in those cases this function
         # will yield an exception, and we don't have to explore all the combinations with these exceptions.
         # I.e. if a tuple from the product below contains an exception, this should not be yielded because the
         # parameter is optional. Instead, it will just be filled with the default value and treated as "not provided".
-        for parameter_tuple in itertools.product(*param_iterables):
+        for parameters in self.param_sets(param_iterables):
             parameter_dict: dict[str, Parameter] = {}
-            for param_name, param_value in zip(ordered_param_map.keys(), parameter_tuple):
+            if isinstance(parameters, Exception):
+                yield parameters
+                continue
+            for param_name, param_value in parameters.items():
                 if isinstance(param_value, Exception):
-                    assert param_name in self.validator.optional_param_names, "Shouldn't fail"
+                    assert param_name in self.validator.optional_param_names, (
+                        "If the parameter is required but not supplied you should yield an exception "
+                        "in `paran_sets` directly. The dictionary of parameters should only contain exceptions if"
+                        "they are negligible aka the parameter is optional."
+                    )
                     parameter_dict[param_name] = Parameter(
                         mapped_validator=self,
                         name=param_name,
                         param_id="None",
                         value=self.validator.signature.parameters[param_name].default,
                         provided=False,
                     )
@@ -181,15 +187,26 @@
                         mapped_validator=self,
                         name=param_name,
                         param_id=param_value[1],
                         value=param_value[0],
                         provided=True,
                     )
             yield Parameters(self, **parameter_dict)
-        for param_name, iterable in zip(ordered_param_map.keys(), param_iterables):
+
+    def param_sets(self, param_iterables: dict[str, _QueryIterable]) -> Iterator[dict[str, Any] | Exception]:
+        """
+        Gets for each parameter an iterable of all possible values. This method defines how those iterables are
+        combined to parameter sets to call the validator with.
+        By standard this method returns the cartesian product of all iterables i.e. every possible combination.
+        You can override this method to change this behavior.
+        """
+        ordered_params = OrderedDict(param_iterables)
+        for param_tuple in itertools.product(*ordered_params.values()):
+            yield dict(zip(ordered_params.keys(), param_tuple))
+        for param_name, iterable in param_iterables.items():
             if param_name in self.validator.optional_param_names:
                 continue
             assert iterable.cur_exceptions is not None
             for exception in iterable.cur_exceptions:
                 yield exception
 
     def __eq__(self, other):
```

### Comparing `bomf-0.5.8/src/bomf/validation/utils.py` & `bomf-0.5.9/src/bomf/validation/utils.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/src/bomf.egg-info/PKG-INFO` & `bomf-0.5.9/src/bomf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bomf
-Version: 0.5.8
+Version: 0.5.9
 Summary: BO4E Migration Framework
 Home-page: https://github.com/Hochfrequenz/bo4e_migration_framework
 Author: Hochfrequenz Unternehmensberatung GmbH
 Author-email: info@hochfrequenz.de
 License: mit
 Project-URL: Documentation, https://github.com/Hochfrequenz/bo4e_migration_framework
 Project-URL: Code, https://github.com/Hochfrequenz/bo4e_migration_framework
```

### Comparing `bomf-0.5.8/src/bomf.egg-info/SOURCES.txt` & `bomf-0.5.9/src/bomf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/tox.ini` & `bomf-0.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_bo4e_data_set.py` & `bomf-0.5.9/unittests/test_bo4e_data_set.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_entity_loader.py` & `bomf-0.5.9/unittests/test_entity_loader.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_filter.py` & `bomf-0.5.9/unittests/test_filter.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_list_conversion.py` & `bomf-0.5.9/unittests/test_list_conversion.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_mapper.py` & `bomf-0.5.9/unittests/test_mapper.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_migration.py` & `bomf-0.5.9/unittests/test_migration.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_source_data_provider.py` & `bomf-0.5.9/unittests/test_source_data_provider.py`

 * *Files identical despite different names*

### Comparing `bomf-0.5.8/unittests/test_validation.py` & `bomf-0.5.9/unittests/test_validation.py`

 * *Files identical despite different names*

