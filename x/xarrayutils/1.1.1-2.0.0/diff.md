# Comparing `tmp/xarrayutils-1.1.1.tar.gz` & `tmp/xarrayutils-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xarrayutils-1.1.1.tar", last modified: Wed Mar 16 02:27:55 2022, max compression
+gzip compressed data, was "xarrayutils-2.0.0.tar", last modified: Fri Jun  9 18:26:22 2023, max compression
```

## Comparing `xarrayutils-1.1.1.tar` & `xarrayutils-2.0.0.tar`

### file list

```diff
@@ -1,71 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.631491 xarrayutils-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.623491 xarrayutils-1.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      156 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)      305 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.623491 xarrayutils-1.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      474 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.github/workflows/linting.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     4232 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.github/workflows/pythonpublish.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       70 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-03-16 02:27:55.631491 xarrayutils-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.623491 xarrayutils-1.1.1/ci/
--rw-r--r--   0 runner    (1001) docker     (121)      446 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/ci/environment-upstream-dev.yml
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      230 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.627491 xarrayutils-1.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      634 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      338 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3072 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1461 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/contributor_guide.rst
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2344 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)   689757 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   851989 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/utils.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)   246650 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/vertical_coords.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1409 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/docs/whats-new.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.627491 xarrayutils-1.1.1/notebooks/
--rw-r--r--   0 runner    (1001) docker     (121)     9173 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/notebooks/Untitled.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    27015 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/notebooks/regression.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-03-16 02:27:55.631491 xarrayutils-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68751 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/versioneer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.631491 xarrayutils-1.1.1/xarrayutils/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-03-16 02:27:55.631491 xarrayutils-1.1.1/xarrayutils/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    10018 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/build_grids.py
--rw-r--r--   0 runner    (1001) docker     (121)     4362 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/climate_indicies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9242 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     2036 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     2649 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    22060 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.631491 xarrayutils-1.1.1/xarrayutils/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5794 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/datasets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_build_grids.py
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_file_handling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1404 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_filtering.py
--rw-r--r--   0 runner    (1001) docker     (121)     3878 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)    20566 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16586 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_vertical_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     1797 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_vertical_remapping.py
--rw-r--r--   0 runner    (1001) docker     (121)    11619 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_xgcm_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      749 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/test/test_xmitgcm_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/utilities.py
--rw-r--r--   0 runner    (1001) docker     (121)    27958 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    19077 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/vertical_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)     5699 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/vertical_remapping.py
--rw-r--r--   0 runner    (1001) docker     (121)     8614 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)     9268 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/xgcm_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4024 2022-03-16 02:27:43.000000 xarrayutils-1.1.1/xarrayutils/xmitgcm_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-16 02:27:55.627491 xarrayutils-1.1.1/xarrayutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2077 2022-03-16 02:27:55.000000 xarrayutils-1.1.1/xarrayutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1564 2022-03-16 02:27:55.000000 xarrayutils-1.1.1/xarrayutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-16 02:27:55.000000 xarrayutils-1.1.1/xarrayutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-03-16 02:27:55.000000 xarrayutils-1.1.1/xarrayutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-16 02:27:55.000000 xarrayutils-1.1.1/xarrayutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.337704 xarrayutils-2.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.337704 xarrayutils-2.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.github/workflows/pythonpublish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.341704 xarrayutils-2.0.0/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/ci/environment-upstream-dev.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.345704 xarrayutils-2.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/contributor_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   689757 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   851989 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/utils.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   246650 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/vertical_coords.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/docs/whats-new.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.345704 xarrayutils-2.0.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9173 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/notebooks/Untitled.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    27015 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/notebooks/regression.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68751 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10018 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/build_grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/climate_indicies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_build_grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20499 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_xgcm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/test/test_xmitgcm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27953 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/xgcm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-06-09 18:26:11.000000 xarrayutils-2.0.0/xarrayutils/xmitgcm_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 18:26:22.349704 xarrayutils-2.0.0/xarrayutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 18:26:22.000000 xarrayutils-2.0.0/xarrayutils.egg-info/top_level.txt
```

### Comparing `xarrayutils-1.1.1/.github/workflows/pythonpublish.yaml` & `xarrayutils-2.0.0/.github/workflows/pythonpublish.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,21 @@
       - published #this will be triggered by any kind of release. Pre releases are uploaded to testpypi and real releases to pypi
 
 jobs:
   build-artifacts:
     runs-on: ubuntu-latest
     if: github.repository == 'jbusecke/xarrayutils'
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         name: Install Python
         with:
-          python-version: 3.8
+          python-version: 3.9
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           python -m pip install setuptools setuptools-scm[toml] wheel twine
       - name: Check python version
         run: |
           python --version
@@ -37,61 +37,61 @@
           pwd
           if [ -f dist/xarrayutils-0.0.0.tar.gz ]; then
             echo "❌ INVALID VERSION NUMBER"
             exit 1
           else
             echo "✅ Looks good"
           fi
-      - uses: actions/upload-artifact@v2
+      - uses: actions/upload-artifact@v3
         with:
           name: releases
           path: dist
 
   test-built-dist:
     needs: build-artifacts
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v4
         name: Install Python
         with:
-          python-version: 3.8
-      - uses: actions/download-artifact@v2
+          python-version: 3.9
+      - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: List contents of built dist
         run: |
           ls -ltrh
           ls -ltrh dist
   upload-to-testpypi:
     needs: test-built-dist
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to TestPyPI
-        uses: pypa/gh-action-pypi-publish@v1.5.0
+        uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
           user: __token__
           repository_url: https://test.pypi.org/legacy/
           password: ${{ secrets.TESTPYPI_TOKEN }}
           verbose: true
   upload-to-pypi:
     needs: upload-to-testpypi
     if: "!github.event.release.prerelease"
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/download-artifact@v2
+      - uses: actions/download-artifact@v3
         with:
           name: releases
           path: dist
       - name: Publish package to PyPI
-        uses: pypa/gh-action-pypi-publish@v1.5.0
+        uses: pypa/gh-action-pypi-publish@v1.6.4
         with:
           user: __token__
           password: ${{ secrets.PYPI_TOKEN }}
           verbose: true
   check-version-testpypi:
       needs: upload-to-testpypi
       runs-on: ubuntu-latest
```

### Comparing `xarrayutils-1.1.1/.gitignore` & `xarrayutils-2.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/LICENSE` & `xarrayutils-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/PKG-INFO` & `xarrayutils-2.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: xarrayutils
-Version: 1.1.1
+Version: 2.0.0
 Summary: A collection of various tools for data analysis built on top of xarray and xgcm
 Home-page: https://github.com/jbusecke/xarrayutils
 Author: xarrayutils Developers
 Author-email: julius@ldeo.columbia.edu
 License: MIT
-Description: [![Build Status](https://img.shields.io/github/workflow/status/jbusecke/xarrayutils/CI?logo=github)](https://github.com/jbusecke/xarrayutils/actions)
-        [![codecov](https://codecov.io/gh/jbusecke/xarrayutils/branch/master/graph/badge.svg)](https://codecov.io/gh/jbusecke/xarrayutils)
-        [![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
-        [![pypi](https://img.shields.io/pypi/v/xarrayutils.svg)](https://pypi.org/project/xarrayutils)
-        [![conda-forge](https://img.shields.io/conda/dn/conda-forge/xarrayutils?label=conda-forge)](https://anaconda.org/conda-forge/xarrayutils)
-        [![Documentation Status](https://readthedocs.org/projects/xarrayutils/badge/?version=latest)](https://xarrayutils.readthedocs.io/en/latest/?badge=latest)
-        
-        
-        # A collection of various tools for data analysis built on top of xarray and xgcm
-        
-        This package contains a variety of utility functions I have used in the past few years for data analysis.
-        
-        Please be aware that I am currently refactoring a lot of the code, which might cause breaking changes.
-        
-        For more information see the [documentation](https://xarrayutils.readthedocs.io/en/latest/)
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: complete
 Provides-Extra: docs
 Provides-Extra: dev
+License-File: LICENSE
+
+[![Build Status](https://img.shields.io/github/workflow/status/jbusecke/xarrayutils/CI?logo=github)](https://github.com/jbusecke/xarrayutils/actions)
+[![codecov](https://codecov.io/gh/jbusecke/xarrayutils/branch/master/graph/badge.svg)](https://codecov.io/gh/jbusecke/xarrayutils)
+[![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
+[![pypi](https://img.shields.io/pypi/v/xarrayutils.svg)](https://pypi.org/project/xarrayutils)
+[![conda-forge](https://img.shields.io/conda/dn/conda-forge/xarrayutils?label=conda-forge)](https://anaconda.org/conda-forge/xarrayutils)
+[![Documentation Status](https://readthedocs.org/projects/xarrayutils/badge/?version=latest)](https://xarrayutils.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6360900.svg)](https://doi.org/10.5281/zenodo.6360900)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/jbusecke/xarrayutils/master.svg)](https://results.pre-commit.ci/latest/github/jbusecke/xarrayutils/master)
+
+
+
+# A collection of various tools for data analysis built on top of xarray and xgcm
+
+This package contains a variety of utility functions I have used in the past few years for data analysis.
+
+Please be aware that I am currently refactoring a lot of the code, which might cause breaking changes.
+
+For more information see the [documentation](https://xarrayutils.readthedocs.io/en/latest/)
+
+
```

### Comparing `xarrayutils-1.1.1/README.md` & `xarrayutils-2.0.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 [![Build Status](https://img.shields.io/github/workflow/status/jbusecke/xarrayutils/CI?logo=github)](https://github.com/jbusecke/xarrayutils/actions)
 [![codecov](https://codecov.io/gh/jbusecke/xarrayutils/branch/master/graph/badge.svg)](https://codecov.io/gh/jbusecke/xarrayutils)
 [![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
 [![pypi](https://img.shields.io/pypi/v/xarrayutils.svg)](https://pypi.org/project/xarrayutils)
 [![conda-forge](https://img.shields.io/conda/dn/conda-forge/xarrayutils?label=conda-forge)](https://anaconda.org/conda-forge/xarrayutils)
 [![Documentation Status](https://readthedocs.org/projects/xarrayutils/badge/?version=latest)](https://xarrayutils.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6360900.svg)](https://doi.org/10.5281/zenodo.6360900)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/jbusecke/xarrayutils/master.svg)](https://results.pre-commit.ci/latest/github/jbusecke/xarrayutils/master)
+
 
 
 # A collection of various tools for data analysis built on top of xarray and xgcm
 
 This package contains a variety of utility functions I have used in the past few years for data analysis.
 
 Please be aware that I am currently refactoring a lot of the code, which might cause breaking changes.
```

### Comparing `xarrayutils-1.1.1/docs/Makefile` & `xarrayutils-2.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/docs/conf.py` & `xarrayutils-2.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/docs/contributor_guide.rst` & `xarrayutils-2.0.0/docs/contributor_guide.rst`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/docs/index.rst` & `xarrayutils-2.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/docs/plotting.ipynb` & `xarrayutils-2.0.0/docs/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/docs/utils.ipynb` & `xarrayutils-2.0.0/docs/utils.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/docs/vertical_coords.ipynb` & `xarrayutils-2.0.0/docs/vertical_coords.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/notebooks/Untitled.ipynb` & `xarrayutils-2.0.0/notebooks/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/notebooks/regression.ipynb` & `xarrayutils-2.0.0/notebooks/regression.ipynb`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/setup.py` & `xarrayutils-2.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,19 +37,19 @@
     license="MIT",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
     ],
     packages=find_packages(exclude=["docs", "tests", "tests.*", "docs.*"]),
     install_requires=install_requires,
     extras_require=extras_require,
-    python_requires=">=3.8",
+    python_requires=">=3.9",
     version=versioneer.get_version(),
     cmdclass=versioneer.get_cmdclass(),
     long_description=long_description,
     long_description_content_type="text/markdown",
 )
```

### Comparing `xarrayutils-1.1.1/versioneer.py` & `xarrayutils-2.0.0/versioneer.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/build_grids.py` & `xarrayutils-2.0.0/xarrayutils/build_grids.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/climate_indicies.py` & `xarrayutils-2.0.0/xarrayutils/climate_indicies.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/file_handling.py` & `xarrayutils-2.0.0/xarrayutils/file_handling.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/filtering.py` & `xarrayutils-2.0.0/xarrayutils/filtering.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/plotting.py` & `xarrayutils-2.0.0/xarrayutils/plotting.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/test/datasets.py` & `xarrayutils-2.0.0/xarrayutils/test/datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,18 +9,18 @@
         [1, 1, 1, 3, 3, 3, 5, 5],
         [1, np.nan, 1, 3, 3, 3, 5, 5],
         [1, 1, 1, 3, 3, 3, 5, 5],
         [2, 2, 2, 4, 4, 4, 6, 6],
         [2, 2, 2, 4, 4, 4, 6, 6],
         [2, 2, 2, 4, 4, 4, 6, 6],
     ],
-    dtype=np.float,
+    dtype=float,
 )
 
-ones_2d = np.ones([6, 8], dtype=np.float)
+ones_2d = np.ones([6, 8], dtype=float)
 
 ones_2d_nan = ones_2d.copy()
 ones_2d_nan[2, 2] = np.nan
 
 # # for the grid dataset in non ll coordinates
 # grid_i = np.arange(0,8)
 # grid_j = np.arange(0,6)
```

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_build_grids.py` & `xarrayutils-2.0.0/xarrayutils/test/test_build_grids.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_file_handling.py` & `xarrayutils-2.0.0/xarrayutils/test/test_file_handling.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     assert subfolder.exists()
 
     with pytest.warns(UserWarning):
         maybe_create_folder(subfolder)
 
 
 def test_total_nested_size(ds):
-
     # create a bunch of broadcasted copies of a dataset
     a = ds.copy(deep=True).expand_dims(new=2)
     b = ds.copy(deep=True).expand_dims(new=5)
     c = ds.copy(deep=True).expand_dims(new=4, new_new=10)
 
     # nest them into a dict
     nested_dict = {"experiment_a": a, "experiment_b": {"label_x": b, "label_y": c}}
```

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_filtering.py` & `xarrayutils-2.0.0/xarrayutils/test/test_filtering.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_plotting.py` & `xarrayutils-2.0.0/xarrayutils/test/test_plotting.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_utils.py` & `xarrayutils-2.0.0/xarrayutils/test/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,20 +148,22 @@
     assert np.isnan(_linregress_ufunc(x, y)).all()
     assert np.allclose(fit, _linregress_ufunc(x, y, nanmask=True))
     # test with all nansum
     y[:] = np.nan
     assert np.isnan(_linregress_ufunc(x, y, nanmask=True)).all()
 
 
-def _linregress_ufunc(a, b, nanmask=False):
+def _linregress_ufunc(a: np.ndarray, b: np.ndarray, nanmask: bool = False):
     """ufunc to wrap check output of `xr_linregress` against pure scipy results"""
     if nanmask:
         idxa = np.isnan(a)
         idxb = np.isnan(b)
+
         mask = np.logical_and(~idxa, ~idxb)
+
         if sum(~mask) < len(b):  # only applies the mask if not all nan
             a = a[mask]
             b = b[mask]
     slope, intercept, r_value, p_value, std_err = stats.linregress(a, b)
     return np.array([slope, intercept, r_value, p_value, std_err])
 
 
@@ -170,19 +172,16 @@
     [
         (None, "time"),
         ({"x": -1, "y": 1}, "time"),
         ({"x": 1, "y": 1}, "time"),
         ({"x": -1, "y": 1}, "x"),
     ],
 )
-# @pytest.mark.parametrize("variant", range(3))
 @pytest.mark.parametrize("variant", [0])
-# @pytest.mark.parametrize("dtype", [None, np.float])
 @pytest.mark.parametrize("dtype", [None])
-# @pytest.mark.parametrize("nans", [False, True])
 @pytest.mark.parametrize("nans", [True, "all"])
 @pytest.mark.parametrize(
     "ni, parameter", enumerate(["slope", "intercept", "r_value", "p_value", "std_err"])
 )
 def test_xr_linregress(chunks, dim, variant, dtype, nans, parameter, ni):
     a = xr.DataArray(np.random.rand(6, 8, 5), dims=["x", "time", "y"])
     b = xr.DataArray(np.random.rand(6, 5, 8), dims=["x", "y", "time"])
@@ -212,15 +211,17 @@
     reg = xr_linregress(a, b, dim=dim)
 
     dims = list(set(a.dims) - set([dim]))
     for ii in range(len(a[dims[0]])):
         for jj in range(len(a[dims[1]])):
             pos = dict({dims[0]: ii, dims[1]: jj})
 
-            expected = _linregress_ufunc(a.isel(**pos), b.isel(**pos), nanmask=True)
+            expected = _linregress_ufunc(
+                a.isel(**pos).load().data, b.isel(**pos).load().data, nanmask=True
+            )
             reg_sub = reg.isel(**pos)
 
             np.testing.assert_allclose(reg_sub[parameter].data, expected[ni])
 
 
 def test_linear_trend():
     # TODO implement a test for nans
@@ -591,15 +592,15 @@
 def test_aggregate_input_da(dataarray_2d_example):
     blocks = [("i", 3), ("j", 3)]
     with pytest.raises(RuntimeError):
         aggregate(dataarray_2d_example.compute(), blocks, func=np.nanmean)
 
 
 def test_aggregate_w_nanmean(dataarray_2d_ones, dataarray_2d_ones_nan):
-    expected_result = np.array([[1, 1], [1, 1]], dtype=np.float)
+    expected_result = np.array([[1, 1], [1, 1]], dtype=float)
     blocks = [("i", 3), ("j", 3)]
 
     data = dataarray_2d_ones_nan
     weights = dataarray_2d_ones
     a = aggregate_w_nanmean(data, weights, blocks)
     assert_allclose(a.data.compute(), expected_result)
```

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_xgcm_utils.py` & `xarrayutils-2.0.0/xarrayutils/test/test_xgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/test/test_xmitgcm_utils.py` & `xarrayutils-2.0.0/xarrayutils/test/test_xmitgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/utils.py` & `xarrayutils-2.0.0/xarrayutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 def linear_trend(obj, dim):
     """Convenience wrapper for 'xr_linregress'. Calculates the trend per
     given timestep. E.g. if the data is passed as yearly values, the
     trend is in units/yr.
     """
     x = xr.DataArray(
-        np.arange(len(obj[dim])).astype(np.float), dims=dim, coords={dim: obj[dim]}
+        np.arange(len(obj[dim])).astype(float), dims=dim, coords={dim: obj[dim]}
     )
     trend = xr_linregress(x, obj, dim=dim)
     return trend
 
 
 def _lin_trend_legacy(y):
     """ufunc to be used by linear_trend"""
@@ -197,15 +197,14 @@
     if not isinstance(da.data, Array):
         raise RuntimeError("data array data must be a dask array")
     # Check data type of blocks
     # TODO write test
     if not all(isinstance(n[0], str) for n in blocks) or not all(
         isinstance(n[1], int) for n in blocks
     ):
-
         print("blocks input", str(blocks))
         raise RuntimeError(
             "block dimension must be dtype(str), \
         e.g. ('lon',4)"
         )
 
     # Check if the given array has the dimension specified in blocks
@@ -588,15 +587,14 @@
 
         p = a.mean(dim=t_dim).copy()
         p[:] = np.nan
         p.name = "p value " + a.name + "/" + b.name
 
         for ii in range(len(a[a_x_dim])):
             for jj in range(len(a[a_y_dim])):
-
                 # Define the 'input' (position in a) correctly, accounting for
                 # the possibility that the
                 # lat/lon position can be defined in the coordinates
                 # or dimensions
                 # interp timeseries onto the data.time
                 in_a = a[{a_x_dim: ii, a_y_dim: jj}]
```

### Comparing `xarrayutils-1.1.1/xarrayutils/xgcm_utils.py` & `xarrayutils-2.0.0/xarrayutils/xgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils/xmitgcm_utils.py` & `xarrayutils-2.0.0/xarrayutils/xmitgcm_utils.py`

 * *Files identical despite different names*

### Comparing `xarrayutils-1.1.1/xarrayutils.egg-info/PKG-INFO` & `xarrayutils-2.0.0/xarrayutils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 Metadata-Version: 2.1
 Name: xarrayutils
-Version: 1.1.1
+Version: 2.0.0
 Summary: A collection of various tools for data analysis built on top of xarray and xgcm
 Home-page: https://github.com/jbusecke/xarrayutils
 Author: xarrayutils Developers
 Author-email: julius@ldeo.columbia.edu
 License: MIT
-Description: [![Build Status](https://img.shields.io/github/workflow/status/jbusecke/xarrayutils/CI?logo=github)](https://github.com/jbusecke/xarrayutils/actions)
-        [![codecov](https://codecov.io/gh/jbusecke/xarrayutils/branch/master/graph/badge.svg)](https://codecov.io/gh/jbusecke/xarrayutils)
-        [![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
-        [![pypi](https://img.shields.io/pypi/v/xarrayutils.svg)](https://pypi.org/project/xarrayutils)
-        [![conda-forge](https://img.shields.io/conda/dn/conda-forge/xarrayutils?label=conda-forge)](https://anaconda.org/conda-forge/xarrayutils)
-        [![Documentation Status](https://readthedocs.org/projects/xarrayutils/badge/?version=latest)](https://xarrayutils.readthedocs.io/en/latest/?badge=latest)
-        
-        
-        # A collection of various tools for data analysis built on top of xarray and xgcm
-        
-        This package contains a variety of utility functions I have used in the past few years for data analysis.
-        
-        Please be aware that I am currently refactoring a lot of the code, which might cause breaking changes.
-        
-        For more information see the [documentation](https://xarrayutils.readthedocs.io/en/latest/)
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: complete
 Provides-Extra: docs
 Provides-Extra: dev
+License-File: LICENSE
+
+[![Build Status](https://img.shields.io/github/workflow/status/jbusecke/xarrayutils/CI?logo=github)](https://github.com/jbusecke/xarrayutils/actions)
+[![codecov](https://codecov.io/gh/jbusecke/xarrayutils/branch/master/graph/badge.svg)](https://codecov.io/gh/jbusecke/xarrayutils)
+[![License:MIT](https://img.shields.io/badge/License-MIT-lightgray.svg?style=flt-square)](https://opensource.org/licenses/MIT)
+[![pypi](https://img.shields.io/pypi/v/xarrayutils.svg)](https://pypi.org/project/xarrayutils)
+[![conda-forge](https://img.shields.io/conda/dn/conda-forge/xarrayutils?label=conda-forge)](https://anaconda.org/conda-forge/xarrayutils)
+[![Documentation Status](https://readthedocs.org/projects/xarrayutils/badge/?version=latest)](https://xarrayutils.readthedocs.io/en/latest/?badge=latest)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.6360900.svg)](https://doi.org/10.5281/zenodo.6360900)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/jbusecke/xarrayutils/master.svg)](https://results.pre-commit.ci/latest/github/jbusecke/xarrayutils/master)
+
+
+
+# A collection of various tools for data analysis built on top of xarray and xgcm
+
+This package contains a variety of utility functions I have used in the past few years for data analysis.
+
+Please be aware that I am currently refactoring a lot of the code, which might cause breaking changes.
+
+For more information see the [documentation](https://xarrayutils.readthedocs.io/en/latest/)
+
+
```

