# Comparing `tmp/devpi-builder-5.1.0.tar.gz` & `tmp/devpi-builder-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devpi-builder-5.1.0.tar", last modified: Fri Nov  5 10:42:01 2021, max compression
+gzip compressed data, was "devpi-builder-6.0.0.tar", last modified: Fri Jun  9 10:31:32 2023, max compression
```

## Comparing `devpi-builder-5.1.0.tar` & `devpi-builder-6.0.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      568 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.332624 devpi-builder-5.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.336624 devpi-builder-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      133 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/.pyup.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4541 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1528 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)       41 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9491 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4014 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.336624 devpi-builder-5.1.0/devpi_builder/
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/devpi_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7005 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/devpi_builder/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2233 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/devpi_builder/requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/devpi_builder/wheeler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.336624 devpi-builder-5.1.0/devpi_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9491 2021-11-05 10:42:01.000000 devpi-builder-5.1.0/devpi_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2021-11-05 10:42:01.000000 devpi-builder-5.1.0/devpi_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-05 10:42:01.000000 devpi-builder-5.1.0/devpi_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-11-05 10:42:01.000000 devpi-builder-5.1.0/devpi_builder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-05 10:42:01.000000 devpi-builder-5.1.0/devpi_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-11-05 10:42:01.000000 devpi-builder-5.1.0/devpi_builder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/requirements.in
--rw-r--r--   0 runner    (1001) docker     (121)     3800 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2021-11-05 10:42:01.344624 devpi-builder-5.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.336624 devpi-builder-5.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/non-ascii_package/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/non-ascii_package/dist/
--rw-r--r--   0 runner    (1001) docker     (121)      762 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/non-ascii_package/dist/non-ascii-package-0.1.dev1.tar.gz
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/non-ascii_package/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      331 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/non-ascii_package/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/non-pure_package/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/non-pure_package/dist/
--rw-r--r--   0 runner    (1001) docker     (121)     1698 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/non-pure_package/dist/test_package-0.1.dev1-cp27-none-linux_x86_64.whl
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/non-pure_package/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/non-pure_package/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/pure_package/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/pure_package/dist/
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/pure_package/dist/test_package-0.1.dev1-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (121)       20 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/pure_package/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      218 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/pure_package/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-05 10:42:01.340624 devpi-builder-5.1.0/tests/fixture/pure_package/test_package/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/pure_package/test_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       61 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_blacklist.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_comments.txt
--rw-r--r--   0 runner    (1001) docker     (121)       58 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_continue_on_failed.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_different_styles.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_inexact_version.txt
--rw-r--r--   0 runner    (1001) docker     (121)       82 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_junit.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_multiple_versions.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_multiple_versions_on_line.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_no_version.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_non-ascii.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_pure_and_non-pure.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_simple.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/fixture/sample_test_package.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9790 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2024 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/test_requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     2237 2021-11-05 10:41:40.000000 devpi-builder-5.1.0/tests/test_wheeler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.061699 devpi-builder-6.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.065699 devpi-builder-6.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/core-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.065699 devpi-builder-6.0.0/devpi_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/devpi_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/devpi_builder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/devpi_builder/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/devpi_builder/wheeler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.069699 devpi-builder-6.0.0/devpi_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10031 2023-06-09 10:31:32.000000 devpi-builder-6.0.0/devpi_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-09 10:31:32.000000 devpi-builder-6.0.0/devpi_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:31:32.000000 devpi-builder-6.0.0/devpi_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-09 10:31:32.000000 devpi-builder-6.0.0/devpi_builder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-09 10:31:32.000000 devpi-builder-6.0.0/devpi_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-09 10:31:32.000000 devpi-builder-6.0.0/devpi_builder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.069699 devpi-builder-6.0.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/non-ascii_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/non-ascii_package/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/non-ascii_package/dist/non-ascii-package-0.1.dev1.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/non-ascii_package/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/non-ascii_package/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/non-pure_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/non-pure_package/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/non-pure_package/dist/test_package-0.1.dev1-cp27-none-linux_x86_64.whl
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/non-pure_package/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/non-pure_package/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/pure_package/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/pure_package/dist/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/pure_package/dist/test_package-0.1.dev1-py2.py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/pure_package/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/pure_package/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:31:32.073699 devpi-builder-6.0.0/tests/fixture/pure_package/test_package/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/pure_package/test_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_blacklist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_comments.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_continue_on_failed.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_different_styles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_inexact_version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_junit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_multiple_versions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_multiple_versions_on_line.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_no_version.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_non-ascii.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_pure_and_non-pure.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_simple.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/fixture/sample_test_package.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9790 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/test_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-06-09 10:31:19.000000 devpi-builder-6.0.0/tests/test_wheeler.py
```

### Comparing `devpi-builder-5.1.0/.coveragerc` & `devpi-builder-6.0.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/.github/workflows/publish.yml` & `devpi-builder-6.0.0/.github/workflows/publish.yml`

 * *Files 22% similar despite different names*

```diff
@@ -4,17 +4,17 @@
   release:
     types: [published]
 
 jobs:
   publish:
     runs-on: ubuntu-latest
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install build
     - name: Build package
```

### Comparing `devpi-builder-5.1.0/.github/workflows/tests.yml` & `devpi-builder-6.0.0/.github/workflows/tests.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,19 +7,19 @@
     branches: [ master ]
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: [3.6, 3.7, 3.8, 3.9]
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install -r requirements.txt
         python -m pip install --no-deps -e .
@@ -45,7 +45,21 @@
     steps:
     - name: Finished
       run: |
         python -m pip install coveralls
         coveralls --service=github --finish
       env:
         GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+  check_packaging:
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v3
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v4
+      with:
+        python-version: '3.x'
+    - name: Verify packaging
+      run: |
+        python -m pip install build twine
+        python -m build
+        twine check dist/*
+
```

### Comparing `devpi-builder-5.1.0/CHANGELOG.rst` & `devpi-builder-6.0.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 =========
 Changelog
 =========
 
 This lists the most important changes for each release.
 
 
+Version 6.0.0 — 2023-06-09
+==========================
+
+Added
+-----
+
+* Python 3.10 and 3.11 are now supported.
+
+Changed
+-------
+
+* Improved performance of checking for already built packages.
+
+Removed
+-------
+
+* Dropped support for running tests via `setup.py test`.
+  The mechanism is considered deprecated by upstream and removing it allows us to drop a dependency.
+* Python 3.6 is no longer supported. It likely still works but we will no longer run CI against it.
+
+
 Version 5.1.0 — 2021-11-05
 ==========================
 
 Added
 -----
 
 * Provide compatibility with pip 21.3 and above which drops the `--build-directory` option.
```

### Comparing `devpi-builder-5.1.0/COPYING` & `devpi-builder-6.0.0/COPYING`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/PKG-INFO` & `devpi-builder-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: devpi-builder
-Version: 5.1.0
+Version: 6.0.0
 Summary: Devpi-builder takes a requirements.txt and incrementally fills a devpi index with wheels of the listed python packages.
 Home-page: https://github.com/blue-yonder/devpi-builder
 Author: Matthias Bach
 Author-email: matthias.bach@blue-yonder.com
 License: new BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: COPYING
 
 =========================
 Brandon the Devpi Builder
 =========================
 
 .. image:: https://coveralls.io/repos/blue-yonder/devpi-builder/badge.svg?branch=master
@@ -124,14 +125,35 @@
 =========
 Changelog
 =========
 
 This lists the most important changes for each release.
 
 
+Version 6.0.0 — 2023-06-09
+==========================
+
+Added
+-----
+
+* Python 3.10 and 3.11 are now supported.
+
+Changed
+-------
+
+* Improved performance of checking for already built packages.
+
+Removed
+-------
+
+* Dropped support for running tests via `setup.py test`.
+  The mechanism is considered deprecated by upstream and removing it allows us to drop a dependency.
+* Python 3.6 is no longer supported. It likely still works but we will no longer run CI against it.
+
+
 Version 5.1.0 — 2021-11-05
 ==========================
 
 Added
 -----
 
 * Provide compatibility with pip 21.3 and above which drops the `--build-directory` option.
@@ -335,9 +357,7 @@
 -----
 
 - Build a list of packages and upload them to a Devpi index
 
 
 .. _devpi-plumber: https://github.com/blue-yonder/devpi-plumber
 .. _Keep-a-CHANGELOG: http://keepachangelog.com
-
-
```

### Comparing `devpi-builder-5.1.0/README.rst` & `devpi-builder-6.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/devpi_builder/cli.py` & `devpi-builder-6.0.0/devpi_builder/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import codecs
 import getpass
 import locale
 import logging
 import os
 
 from junit_xml import TestSuite, TestCase
-from devpi_plumber.client import DevpiClient
+from devpi_plumber.client import DevpiClient, DevpiClientError
 
 from devpi_builder import requirements, wheeler
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 
@@ -52,24 +52,55 @@
         log_entry.add_failure_info(str(exception))
         self._results.append(log_entry)
 
     def _log_success(self, package, version):
         log_entry = self._new_log_entry(package, version)
         self._results.append(log_entry)
 
+    def _list_distribution_links(self, client, package, version):
+        """
+        For looking up an exact version, `devpi getjson <package>/<version>` is much faster
+        than calling `devpi list <package>==<version>`. This is because `list` needs
+        to pull the entire list from the api (very slow when there are many version) before
+        filtering by spec on the client-side, whereas `getjson` quickly pulls the
+        specific version.
+        """
+        package_url = "{}/{}".format(package, version)
+
+        try:
+            data = client.get_json(package_url)
+        except DevpiClientError as error:
+            if '404 Not Found' in str(error):
+                return []
+            raise error
+
+        result = data['result']
+        links = result.get('+links') or []
+
+        if '+shadowing' in result:
+            # Add any upstream links that are being shadowed
+            for shadow_result in result['+shadowing']:
+                shadowing_links = shadow_result.get('+links') or []
+                links.extend(shadowing_links)
+
+        return [link['href'] for link in links]
+
     def _should_package_be_build(self, package, version):
-        spec = "{}=={}".format(package, version)
 
         if self._blacklist and requirements.matched_by_list(package, version, self._blacklist):
             self._log_skip('Skipping %s %s as it is matched by the blacklist.', package, version)
             return False
-        elif wheeler.has_compatible_wheel(self._devpi_client.list(spec)):
+        elif wheeler.has_compatible_wheel(
+                self._list_distribution_links(self._devpi_client, package, version)
+        ):
             self._log_skip('Skipping %s %s as is already available on the index.', package, version)
             return False
-        elif self._pure_index_client and wheeler.has_compatible_wheel(self._pure_index_client.list(spec)):
+        elif self._pure_index_client and wheeler.has_compatible_wheel(
+                self._list_distribution_links(self._pure_index_client, package, version)
+        ):
             self._log_skip('Skipping %s %s as is already available on the pure index.', package, version)
             return False
         return True
 
     def _upload_package(self, package, version, wheel_file):
         if self._pure_index_client and wheeler.is_pure(wheel_file):
             logger.debug('Uploading %s %s to pure index %s', package, version, self._pure_index_client.url)
```

### Comparing `devpi-builder-5.1.0/devpi_builder/requirements.py` & `devpi-builder-6.0.0/devpi_builder/requirements.py`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/devpi_builder/wheeler.py` & `devpi-builder-6.0.0/devpi_builder/wheeler.py`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/devpi_builder.egg-info/PKG-INFO` & `devpi-builder-6.0.0/devpi_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: devpi-builder
-Version: 5.1.0
+Version: 6.0.0
 Summary: Devpi-builder takes a requirements.txt and incrementally fills a devpi index with wheels of the listed python packages.
 Home-page: https://github.com/blue-yonder/devpi-builder
 Author: Matthias Bach
 Author-email: matthias.bach@blue-yonder.com
 License: new BSD
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
 License-File: COPYING
 
 =========================
 Brandon the Devpi Builder
 =========================
 
 .. image:: https://coveralls.io/repos/blue-yonder/devpi-builder/badge.svg?branch=master
@@ -124,14 +125,35 @@
 =========
 Changelog
 =========
 
 This lists the most important changes for each release.
 
 
+Version 6.0.0 — 2023-06-09
+==========================
+
+Added
+-----
+
+* Python 3.10 and 3.11 are now supported.
+
+Changed
+-------
+
+* Improved performance of checking for already built packages.
+
+Removed
+-------
+
+* Dropped support for running tests via `setup.py test`.
+  The mechanism is considered deprecated by upstream and removing it allows us to drop a dependency.
+* Python 3.6 is no longer supported. It likely still works but we will no longer run CI against it.
+
+
 Version 5.1.0 — 2021-11-05
 ==========================
 
 Added
 -----
 
 * Provide compatibility with pip 21.3 and above which drops the `--build-directory` option.
@@ -335,9 +357,7 @@
 -----
 
 - Build a list of packages and upload them to a Devpi index
 
 
 .. _devpi-plumber: https://github.com/blue-yonder/devpi-plumber
 .. _Keep-a-CHANGELOG: http://keepachangelog.com
-
-
```

### Comparing `devpi-builder-5.1.0/devpi_builder.egg-info/SOURCES.txt` & `devpi-builder-6.0.0/devpi_builder.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .coveragerc
 .gitignore
 .pyup.yml
 CHANGELOG.rst
 COPYING
 MANIFEST.in
 README.rst
+core-requirements.txt
 requirements.in
 requirements.txt
 setup.cfg
 setup.py
 .github/workflows/publish.yml
 .github/workflows/tests.yml
 devpi_builder/__init__.py
```

### Comparing `devpi-builder-5.1.0/requirements.txt` & `devpi-builder-6.0.0/requirements.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,198 +1,219 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.7
+# by the following command:
 #
 #    pip-compile --no-emit-index-url
 #
-apipkg==1.5
-    # via execnet
-appdirs==1.4.4
+aiohttp==3.8.3
+    # via devpi-server
+aiosignal==1.2.0
+    # via aiohttp
+argon2-cffi==21.3.0
     # via
     #   devpi-server
-    #   virtualenv
-argon2-cffi==20.1.0
-    # via passlib
-attrs==20.3.0
+    #   passlib
+argon2-cffi-bindings==21.2.0
+    # via argon2-cffi
+async-timeout==4.0.2
+    # via aiohttp
+attrs==21.4.0
     # via
+    #   aiohttp
     #   devpi-server
     #   pytest
     #   wheel-inspect
-bleach==4.1.0
+bleach==5.0.1
     # via readme-renderer
-build==0.3.1.post1
+build==0.8.0
     # via check-manifest
-certifi==2020.12.5
-    # via requests
-cffi==1.14.5
-    # via argon2-cffi
-chardet==4.0.0
+certifi==2022.12.7
     # via requests
-check-manifest==0.46
+cffi==1.15.0
+    # via argon2-cffi-bindings
+charset-normalizer==2.0.12
+    # via
+    #   aiohttp
+    #   requests
+check-manifest==0.48
     # via devpi-client
-coverage==5.5
+coverage[toml]==6.4.1
     # via pytest-cov
-devpi-client==5.2.2
+defusedxml==0.7.1
+    # via devpi-server
+devpi-client==5.2.3
     # via devpi-plumber
 devpi-common==3.6.0
     # via
     #   devpi-client
     #   devpi-server
-devpi-plumber[test]==0.5.1
+devpi-plumber[test]==0.6.0
     # via
+    #   -r core-requirements.txt
     #   -r requirements.in
-    #   sanitized-package
-devpi-server==5.5.1
+devpi-server==6.5.1
     # via devpi-plumber
-distlib==0.3.1
+distlib==0.3.4
     # via virtualenv
-docutils==0.16
+docutils==0.19
     # via readme-renderer
 entry-points-txt==0.1.0
     # via wheel-inspect
-execnet==1.8.0
-    # via devpi-server
-filelock==3.0.12
+filelock==3.7.1
     # via
     #   tox
     #   virtualenv
+frozenlist==1.3.3
+    # via
+    #   aiohttp
+    #   aiosignal
 headerparser==0.4.0
     # via wheel-inspect
-hupper==1.10.2
+hupper==1.10.3
     # via pyramid
-idna==2.10
-    # via requests
+idna==3.3
+    # via
+    #   requests
+    #   yarl
 iniconfig==1.1.1
     # via pytest
-itsdangerous==1.1.0
+itsdangerous==2.1.2
     # via devpi-server
 junit-xml==1.9
-    # via sanitized-package
+    # via -r core-requirements.txt
 lazy==1.4
-    # via devpi-common
+    # via
+    #   devpi-common
+    #   devpi-server
 mock==4.0.3
     # via -r requirements.in
-packaging==20.9
+multidict==6.0.2
+    # via
+    #   aiohttp
+    #   yarl
+packaging==21.3
     # via
-    #   bleach
     #   build
     #   pytest
+    #   setuptools-scm
     #   tox
     #   wheel-inspect
 passlib[argon2]==1.7.4
     # via devpi-server
 pastedeploy==2.1.1
     # via plaster-pastedeploy
-pep517==0.10.0
+pep517==0.12.0
     # via build
-pkginfo==1.7.0
+pkginfo==1.8.2
     # via devpi-client
-plaster-pastedeploy==0.7
-    # via pyramid
 plaster==1.0
     # via
     #   plaster-pastedeploy
     #   pyramid
-pluggy==0.13.1
+plaster-pastedeploy==0.7
+    # via pyramid
+platformdirs==2.5.2
+    # via
+    #   devpi-server
+    #   virtualenv
+pluggy==1.0.0
     # via
     #   devpi-client
     #   devpi-server
     #   pytest
     #   tox
-py==1.10.0
+py==1.11.0
     # via
     #   devpi-client
     #   devpi-common
     #   devpi-server
     #   pytest
     #   tox
-pycparser==2.20
+pycparser==2.21
     # via cffi
-pygments==2.8.1
+pygments==2.13.0
     # via readme-renderer
-pyparsing==2.4.7
+pyparsing==3.0.9
     # via packaging
-pyramid==1.10.8
+pyramid==2.0
     # via devpi-server
-pytest-cov==2.11.1
-    # via -r requirements.in
-pytest-mock==3.5.1
-    # via -r requirements.in
-pytest-runner==5.3.0
-    # via -r requirements.in
-pytest==6.2.2
+pytest==7.1.2
     # via
     #   -r requirements.in
     #   pytest-cov
     #   pytest-mock
-python-dateutil==2.8.1
+pytest-cov==3.0.0
+    # via -r requirements.in
+pytest-mock==3.10.0
+    # via -r requirements.in
+python-dateutil==2.8.2
     # via strictyaml
-readme-renderer==24.0
+readme-renderer==37.3
     # via wheel-inspect
-repoze.lru==0.7
+repoze-lru==0.7
     # via devpi-server
-requests==2.25.1
-    # via devpi-common
-ruamel.yaml.clib==0.2.2
-    # via ruamel.yaml
-ruamel.yaml==0.17.0
-    # via strictyaml
-setuptools-scm==6.0.1
+requests==2.31.0
+    # via
+    #   devpi-common
+    #   devpi-plumber
+ruamel-yaml==0.17.21
+    # via devpi-server
+setuptools-scm==6.4.2
     # via -r requirements.in
-six==1.15.0
+six==1.16.0
     # via
-    #   argon2-cffi
     #   bleach
-    #   devpi-plumber
     #   headerparser
     #   junit-xml
     #   python-dateutil
-    #   readme-renderer
     #   tox
     #   virtualenv
-strictyaml==1.3.2
+strictyaml==1.6.1
     # via devpi-server
 toml==0.10.2
+    # via tox
+tomli==2.0.1
     # via
-    #   build
     #   check-manifest
     #   pep517
     #   pytest
-    #   tox
-tox==3.23.0
+    #   setuptools-scm
+tox==3.25.0
     # via devpi-client
 translationstring==1.4
     # via pyramid
-twitter.common.contextutil==0.3.11
+twitter-common-contextutil==0.3.11
     # via devpi-plumber
-twitter.common.dirutil==0.3.11
-    # via twitter.common.contextutil
-twitter.common.lang==0.3.11
-    # via twitter.common.dirutil
-urllib3==1.26.5
+twitter-common-dirutil==0.3.11
+    # via twitter-common-contextutil
+twitter-common-lang==0.3.11
+    # via twitter-common-dirutil
+urllib3==1.26.9
     # via requests
 venusian==3.0.0
     # via pyramid
-virtualenv==20.4.3
+virtualenv==20.14.1
     # via tox
-waitress==2.0.0
+waitress==2.1.2
     # via devpi-server
 webencodings==0.5.1
     # via bleach
 webob==1.8.7
     # via pyramid
-wheel-filename==1.3.0
+wheel==0.38.4
+    # via -r core-requirements.txt
+wheel-filename==1.4.1
     # via
-    #   sanitized-package
+    #   -r core-requirements.txt
     #   wheel-inspect
-wheel-inspect==1.7.0
-    # via sanitized-package
-wheel==0.36.2
-    # via sanitized-package
-zope.deprecation==4.4.0
+wheel-inspect==1.7.1
+    # via -r core-requirements.txt
+yarl==1.8.2
+    # via aiohttp
+zope-deprecation==4.4.0
     # via pyramid
-zope.interface==5.3.0
+zope-interface==5.4.0
     # via pyramid
 
 # The following packages are considered to be unsafe in a requirements file:
 # pip
 # setuptools
```

### Comparing `devpi-builder-5.1.0/tests/fixture/non-ascii_package/dist/non-ascii-package-0.1.dev1.tar.gz` & `devpi-builder-6.0.0/tests/fixture/non-ascii_package/dist/non-ascii-package-0.1.dev1.tar.gz`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/tests/fixture/non-pure_package/dist/test_package-0.1.dev1-cp27-none-linux_x86_64.whl` & `devpi-builder-6.0.0/tests/fixture/non-pure_package/dist/test_package-0.1.dev1-cp27-none-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/tests/fixture/pure_package/dist/test_package-0.1.dev1-py2.py3-none-any.whl` & `devpi-builder-6.0.0/tests/fixture/pure_package/dist/test_package-0.1.dev1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/tests/test_cli.py` & `devpi-builder-6.0.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/tests/test_requirements.py` & `devpi-builder-6.0.0/tests/test_requirements.py`

 * *Files identical despite different names*

### Comparing `devpi-builder-5.1.0/tests/test_wheeler.py` & `devpi-builder-6.0.0/tests/test_wheeler.py`

 * *Files identical despite different names*

