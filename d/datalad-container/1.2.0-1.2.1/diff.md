# Comparing `tmp/datalad_container-1.2.0.tar.gz` & `tmp/datalad_container-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datalad_container-1.2.0.tar", last modified: Thu May 25 19:30:05 2023, max compression
+gzip compressed data, was "datalad_container-1.2.1.tar", last modified: Fri Jun  9 11:28:12 2023, max compression
```

## Comparing `datalad_container-1.2.0.tar` & `datalad_container-1.2.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-25 19:29:30.000000 datalad_container-1.2.0/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-25 19:29:30.000000 datalad_container-1.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 19:29:30.000000 datalad_container-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-25 19:30:05.447893 datalad_container-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-25 19:29:30.000000 datalad_container-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/_datalad_buildsupport/
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-25 19:29:30.000000 datalad_container-1.2.0/_datalad_buildsupport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-05-25 19:29:30.000000 datalad_container-1.2.0/_datalad_buildsupport/formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-05-25 19:29:30.000000 datalad_container-1.2.0/_datalad_buildsupport/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container/adapters/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/adapters/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/containers_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/extractors/_load_singularity_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/extractors/metalad_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/find_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/datalad_container/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/fixtures/singularity_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_find.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)    11672 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/test_schemes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-25 19:29:30.000000 datalad_container-1.2.0/datalad_container/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 19:29:56.000000 datalad_container-1.2.0/datalad_container/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.443894 datalad_container-1.2.0/datalad_container.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 19:30:05.000000 datalad_container-1.2.0/datalad_container.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/examples/basic_demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/_static/datalad_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.439893 datalad_container-1.2.0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/acknowledgements.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/source/metadata-extraction.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 19:30:05.447893 datalad_container-1.2.0/docs/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-05-25 19:29:30.000000 datalad_container-1.2.0/docs/utils/pygments_ansi_color.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-25 19:29:30.000000 datalad_container-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-25 19:30:05.447893 datalad_container-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-05-25 19:29:30.000000 datalad_container-1.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    68607 2023-05-25 19:29:30.000000 datalad_container-1.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.125489 datalad_container-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 11:27:28.000000 datalad_container-1.2.1/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-06-09 11:27:28.000000 datalad_container-1.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 11:27:28.000000 datalad_container-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-09 11:28:12.125489 datalad_container-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-06-09 11:27:28.000000 datalad_container-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.113489 datalad_container-1.2.1/_datalad_buildsupport/
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-06-09 11:27:28.000000 datalad_container-1.2.1/_datalad_buildsupport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10720 2023-06-09 11:27:28.000000 datalad_container-1.2.1/_datalad_buildsupport/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9720 2023-06-09 11:27:28.000000 datalad_container-1.2.1/_datalad_buildsupport/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.125489 datalad_container-1.2.1/datalad_container/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 11:28:12.125489 datalad_container-1.2.1/datalad_container/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.117489 datalad_container-1.2.1/datalad_container/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/adapters/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.117489 datalad_container-1.2.1/datalad_container/adapters/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/adapters/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/adapters/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15451 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/containers_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/containers_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/containers_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6628 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/containers_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.117489 datalad_container-1.2.1/datalad_container/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/extractors/_load_singularity_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2799 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/extractors/metalad_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/find_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/datalad_container/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/datalad_container/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/fixtures/singularity_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11569 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/test_find.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13102 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/test_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-09 11:27:28.000000 datalad_container-1.2.1/datalad_container/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 11:27:59.000000 datalad_container-1.2.1/datalad_container/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.117489 datalad_container-1.2.1/datalad_container.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-06-09 11:28:12.000000 datalad_container-1.2.1/datalad_container.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-09 11:28:12.000000 datalad_container-1.2.1/datalad_container.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 11:28:12.000000 datalad_container-1.2.1/datalad_container.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-09 11:28:12.000000 datalad_container-1.2.1/datalad_container.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 11:28:12.000000 datalad_container-1.2.1/datalad_container.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-09 11:28:12.000000 datalad_container-1.2.1/datalad_container.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/examples/basic_demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/_static/datalad_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.109489 datalad_container-1.2.1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/acknowledgements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6977 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/source/metadata-extraction.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 11:28:12.121489 datalad_container-1.2.1/docs/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6164 2023-06-09 11:27:28.000000 datalad_container-1.2.1/docs/utils/pygments_ansi_color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 11:27:28.000000 datalad_container-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-09 11:28:12.125489 datalad_container-1.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      358 2023-06-09 11:27:28.000000 datalad_container-1.2.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68607 2023-06-09 11:27:28.000000 datalad_container-1.2.1/versioneer.py
```

### Comparing `datalad_container-1.2.0/COPYING` & `datalad_container-1.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/PKG-INFO` & `datalad_container-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad_container
-Version: 1.2.0
+Version: 1.2.1
 Summary: DataLad extension package for working with containerized environments
 Home-page: https://github.com/datalad/datalad-container
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `datalad_container-1.2.0/README.md` & `datalad_container-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/_datalad_buildsupport/__init__.py` & `datalad_container-1.2.1/_datalad_buildsupport/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/_datalad_buildsupport/formatters.py` & `datalad_container-1.2.1/_datalad_buildsupport/formatters.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/_datalad_buildsupport/setup.py` & `datalad_container-1.2.1/_datalad_buildsupport/setup.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/__init__.py` & `datalad_container-1.2.1/datalad_container/__init__.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/adapters/docker.py` & `datalad_container-1.2.1/datalad_container/adapters/docker.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/adapters/tests/test_docker.py` & `datalad_container-1.2.1/datalad_container/adapters/tests/test_docker.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/containers_add.py` & `datalad_container-1.2.1/datalad_container/containers_add.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/containers_list.py` & `datalad_container-1.2.1/datalad_container/containers_list.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/containers_remove.py` & `datalad_container-1.2.1/datalad_container/containers_remove.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/containers_run.py` & `datalad_container-1.2.1/datalad_container/containers_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 
     _docs_ = dict(
         name_envvar=CONTAINER_NAME_ENVVAR
     )
 
     _params_ = _run_params
 
+    # Analogous to 'run' command - stop on first error
+    on_failure = 'stop'
+
     @staticmethod
     @datasetmethod(name='containers_run')
     @eval_results
     def __call__(cmd, container_name=None, dataset=None,
                  inputs=None, outputs=None, message=None, expand=None,
                  explicit=False, sidecar=None):
         from unittest.mock import patch  # delayed, since takes long (~600ms for yoh)
```

### Comparing `datalad_container-1.2.0/datalad_container/extractors/_load_singularity_versions.py` & `datalad_container-1.2.1/datalad_container/extractors/_load_singularity_versions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 """
 Importing this file extends datalad.support.external_version:
 
 Adds:
     - external_versions["cmd:apptainer"]
     - external_versions["cmd:singularity"]
 """
-import subprocess
 
 from datalad.cmd import (
-    StdOutCapture,
+    StdOutErrCapture,
     WitlessRunner,
 )
 from datalad.support.external_versions import external_versions
 
 
 def __get_apptainer_version():
-    version = WitlessRunner().run("apptainer --version", protocol=StdOutCapture)['stdout'].strip()
+    version = WitlessRunner().run("apptainer --version", protocol=StdOutErrCapture)['stdout'].strip()
     return version.split("apptainer version ")[1]
 
 
 def __get_singularity_version():
-    return WitlessRunner().run("singularity version", protocol=StdOutCapture)['stdout'].strip()
+    return WitlessRunner().run("singularity version", protocol=StdOutErrCapture)['stdout'].strip()
 
 
 # Load external_versions and patch with "cmd:singularity" and "cmd:apptainer"
 external_versions.add("cmd:apptainer", func=__get_apptainer_version)
 external_versions.add("cmd:singularity", func=__get_singularity_version)
```

### Comparing `datalad_container-1.2.0/datalad_container/extractors/metalad_container.py` & `datalad_container-1.2.1/datalad_container/extractors/metalad_container.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/find_container.py` & `datalad_container-1.2.1/datalad_container/find_container.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/tests/fixtures/singularity_image.py` & `datalad_container-1.2.1/datalad_container/tests/fixtures/singularity_image.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/tests/test_add.py` & `datalad_container-1.2.1/datalad_container/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/tests/test_containers.py` & `datalad_container-1.2.1/datalad_container/tests/test_containers.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/tests/test_find.py` & `datalad_container-1.2.1/datalad_container/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/tests/test_run.py` & `datalad_container-1.2.1/datalad_container/tests/test_run.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,34 +10,37 @@
     create,
 )
 from datalad.local.rerun import get_run_info
 from datalad.cmd import (
     StdOutCapture,
     WitlessRunner,
 )
+from datalad.support.exceptions import IncompleteResultsError
 from datalad.support.network import get_local_file_url
 from datalad.tests.utils_pytest import (
     assert_false,
     assert_in,
     assert_not_in_results,
     assert_raises,
+    assert_repo_status,
     assert_result_count,
     ok_,
     ok_clean_git,
     ok_file_has_content,
     skip_if_no_network,
     with_tempfile,
     with_tree,
 )
 from datalad.utils import (
     Path,
     chpwd,
     on_windows,
 )
 
+import pytest
 from datalad_container.tests.utils import add_pyscript_image
 
 testimg_url = 'shub://datalad/datalad-container:testhelper'
 
 
 @with_tree(tree={"dummy0.img": "doesn't matter 0",
                  "dummy1.img": "doesn't matter 1"})
@@ -152,14 +155,48 @@
         res, 1, action='get', status='ok',
         path=op.join(super_ds.path, 'sub', 'righthere'), type='file')
     assert_no_change(res, super_ds.path)
 
 
 @with_tempfile
 @with_tree(tree={'some_container.img': "doesn't matter"})
+def test_non0_exit(path=None, local_file=None):
+    ds = Dataset(path).create()
+
+    # plug in a proper singularity image
+    ds.containers_add(
+        'mycontainer',
+        url=get_local_file_url(op.join(local_file, 'some_container.img')),
+        image='righthere',
+        call_fmt="sh -c '{cmd}'"
+    )
+    ds.save()  # record the effect in super-dataset
+    ok_clean_git(path)
+
+    # now we can run stuff in the container
+    # and because there is just one, we don't even have to name the container
+    ds.containers_run(['touch okfile'])
+    assert_repo_status(path)
+
+    # Test that regular 'run' behaves as expected -- it does not proceed to save upon error
+    with pytest.raises(IncompleteResultsError):
+        ds.run(['sh', '-c', 'touch nokfile && exit 1'])
+    assert_repo_status(path, untracked=['nokfile'])
+    (ds.pathobj / "nokfile").unlink()  # remove for the next test
+    assert_repo_status(path)
+
+    # Now test with containers-run which should behave similarly -- not save in case of error
+    with pytest.raises(IncompleteResultsError):
+        ds.containers_run(['touch nokfile && exit 1'])
+    # check - must have created the file but not saved anything since failed to run!
+    assert_repo_status(path, untracked=['nokfile'])
+
+
+@with_tempfile
+@with_tree(tree={'some_container.img': "doesn't matter"})
 def test_custom_call_fmt(path=None, local_file=None):
     ds = Dataset(path).create()
     subds = ds.create('sub')
 
     # plug in a proper singularity image
     subds.containers_add(
         'mycontainer',
```

### Comparing `datalad_container-1.2.0/datalad_container/tests/test_schemes.py` & `datalad_container-1.2.1/datalad_container/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container/tests/utils.py` & `datalad_container-1.2.1/datalad_container/tests/utils.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/datalad_container.egg-info/PKG-INFO` & `datalad_container-1.2.1/datalad_container.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datalad-container
-Version: 1.2.0
+Version: 1.2.1
 Summary: DataLad extension package for working with containerized environments
 Home-page: https://github.com/datalad/datalad-container
 Author: The DataLad Team and Contributors
 Author-email: team@datalad.org
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `datalad_container-1.2.0/datalad_container.egg-info/SOURCES.txt` & `datalad_container-1.2.1/datalad_container.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/Makefile` & `datalad_container-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/examples/basic_demo.sh` & `datalad_container-1.2.1/docs/examples/basic_demo.sh`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/source/_static/datalad_logo.png` & `datalad_container-1.2.1/docs/source/_static/datalad_logo.png`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/source/acknowledgements.rst` & `datalad_container-1.2.1/docs/source/acknowledgements.rst`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/source/changelog.rst` & `datalad_container-1.2.1/docs/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/source/conf.py` & `datalad_container-1.2.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/source/index.rst` & `datalad_container-1.2.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/source/metadata-extraction.rst` & `datalad_container-1.2.1/docs/source/metadata-extraction.rst`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/docs/utils/pygments_ansi_color.py` & `datalad_container-1.2.1/docs/utils/pygments_ansi_color.py`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/setup.cfg` & `datalad_container-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `datalad_container-1.2.0/versioneer.py` & `datalad_container-1.2.1/versioneer.py`

 * *Files identical despite different names*

