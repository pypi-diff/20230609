# Comparing `tmp/invenio-assets-2.0.0.tar.gz` & `tmp/invenio-assets-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/invenio-assets-2.0.0.tar", last modified: Mon Oct 24 11:51:38 2022, max compression
+gzip compressed data, was "dist/invenio-assets-3.0.0.tar", last modified: Fri Jun  9 07:23:32 2023, max compression
```

## Comparing `invenio-assets-2.0.0.tar` & `invenio-assets-3.0.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      955 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2914 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      930 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7441 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10290 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1128 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6997 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2783 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/upgrade.rst
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets/
--rw-r--r--   0 runner    (1001) docker     (121)     2939 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets/assets/
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/assets/.babelrc
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/assets/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (121)      847 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/assets/.eslintrc.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets/assets/build/
--rw-r--r--   0 runner    (1001) docker     (121)     6895 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/assets/build/webpack.config.js
--rw-r--r--   0 runner    (1001) docker     (121)     2264 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/assets/package.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets/assets/patches/
--rw-r--r--   0 runner    (1001) docker     (121)      560 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/assets/patches/watchpack+1.7.4.patch
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/collect.py
--rw-r--r--   0 runner    (1001) docker     (121)     2177 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/proxies.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/invenio_assets/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5567 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/invenio_assets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      311 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      477 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 11:51:38.000000 invenio-assets-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     2087 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/tests/test_invenio_assets.py
--rw-r--r--   0 runner    (1001) docker     (121)     1340 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/tests/test_invenio_assets_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3583 2022-10-24 11:51:34.000000 invenio-assets-2.0.0/tests/test_webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      504 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3027 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3720 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      522 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      930 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5728 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1161 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7441 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10302 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1128 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      907 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6997 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2783 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/upgrade.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      263 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets/
+-rw-r--r--   0 runner    (1001) docker     (122)     2939 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets/assets/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/assets/.babelrc
+-rw-r--r--   0 runner    (1001) docker     (122)       11 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/assets/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (122)      847 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/assets/.eslintrc.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets/assets/build/
+-rw-r--r--   0 runner    (1001) docker     (122)     7479 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/assets/build/webpack.config.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2358 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/assets/package.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets/assets/patches/
+-rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/assets/patches/semantic-ui-less+2.5.0.patch
+-rw-r--r--   0 runner    (1001) docker     (122)      617 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)      572 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/collect.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)      453 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4048 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/invenio_assets/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5728 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1268 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      122 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/invenio_assets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      311 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      477 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:23:32.000000 invenio-assets-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2087 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/tests/test_invenio_assets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1340 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/tests/test_invenio_assets_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-06-09 07:23:26.000000 invenio-assets-3.0.0/tests/test_webpack.py
```

### Comparing `invenio-assets-2.0.0/.editorconfig` & `invenio-assets-3.0.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/.github/workflows/pypi-publish.yml` & `invenio-assets-3.0.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/.github/workflows/tests.yml` & `invenio-assets-3.0.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/CHANGES.rst` & `invenio-assets-3.0.0/CHANGES.rst`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version 3.0.0 (released 2023-06-08)
+
+* upgrade to webpack 5
+* upgrade js dependencies
+* upgrade webpack plugins
+
 Version 2.0.0 (released 2022-10-24)
 
 * upgrade dependencies to node 18 compliance
 
 Version 1.3.1 (released 2022-09-01)
 
 * Upgrade eslint dependencies
```

### Comparing `invenio-assets-2.0.0/CONTRIBUTING.rst` & `invenio-assets-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/INSTALL.rst` & `invenio-assets-3.0.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/LICENSE` & `invenio-assets-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/MANIFEST.in` & `invenio-assets-3.0.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/PKG-INFO` & `invenio-assets-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-assets
-Version: 2.0.0
+Version: 3.0.0
 Summary: "Media assets management for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-assets
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-06-08)
+        
+        * upgrade to webpack 5
+        * upgrade js dependencies
+        * upgrade webpack plugins
+        
         Version 2.0.0 (released 2022-10-24)
         
         * upgrade dependencies to node 18 compliance
         
         Version 1.3.1 (released 2022-09-01)
         
         * Upgrade eslint dependencies
```

### Comparing `invenio-assets-2.0.0/README.rst` & `invenio-assets-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/docs/Makefile` & `invenio-assets-3.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/docs/conf.py` & `invenio-assets-3.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 # texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
 intersphinx_mapping = {
-    "https://docs.python.org/": None,
+    "python": ("https://docs.python.org/", None),
     "flask": ("https://flask.palletsprojects.com/en/1.1.x/", None),
     "flask_collect": ("https://flask-collect.readthedocs.io/en/latest/", None),
     "flask_webpackext": ("https://flask-webpackext.readthedocs.io/en/latest/", None),
 }
 
 # Autodoc configuraton.
 autoclass_content = "both"
```

### Comparing `invenio-assets-2.0.0/docs/configuration.rst` & `invenio-assets-3.0.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/docs/index.rst` & `invenio-assets-3.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/docs/make.bat` & `invenio-assets-3.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/docs/upgrade.rst` & `invenio-assets-3.0.0/docs/upgrade.rst`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/invenio_assets/__init__.py` & `invenio-assets-3.0.0/invenio_assets/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,14 @@
 
     $ flask collect -v
 """
 
 from .ext import InvenioAssets
 from .proxies import current_assets
 
-__version__ = "2.0.0"
+__version__ = "3.0.0"
 
 __all__ = (
     "__version__",
     "InvenioAssets",
     "current_assets",
 )
```

### Comparing `invenio-assets-2.0.0/invenio_assets/assets/.eslintrc.js` & `invenio-assets-3.0.0/invenio_assets/assets/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/invenio_assets/assets/build/webpack.config.js` & `invenio-assets-3.0.0/invenio_assets/assets/build/webpack.config.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,29 +1,28 @@
 /*
  * This file is part of Invenio.
  * Copyright (C) 2017-2018 CERN.
- * Copyright (C) 2022 Graz University of Technology.
+ * Copyright (C) 2022-2023 Graz University of Technology.
+ * Copyright (C) 2023      TU Wien.
  *
  * Invenio is free software; you can redistribute it and/or modify it
  * under the terms of the MIT License; see LICENSE file for more details.
  */
 
-const fs = require("fs");
-const path = require("path");
+const BundleTracker = require("webpack-bundle-tracker");
 const {
     CleanWebpackPlugin
 } = require("clean-webpack-plugin");
-const config = require("./config");
-const BundleTracker = require("webpack-bundle-tracker");
+const CssMinimizerPlugin = require("css-minimizer-webpack-plugin");
+const ESLintPlugin = require("eslint-webpack-plugin");
 const MiniCssExtractPlugin = require("mini-css-extract-plugin");
-const OptimizeCSSAssetsPlugin = require("optimize-css-assets-webpack-plugin");
-const safePostCssParser = require("postcss-safe-parser");
 const TerserPlugin = require("terser-webpack-plugin");
+const config = require("./config");
+const path = require("path");
 const webpack = require("webpack");
-const ESLintPlugin = require("eslint-webpack-plugin");
 
 // Load aliases from config and resolve their full path
 let aliases = {};
 if (config.aliases) {
     aliases = Object.fromEntries(
         Object.entries(config.aliases).map(([alias, alias_path]) => [
             alias,
@@ -32,32 +31,48 @@
     );
 }
 
 var webpackConfig = {
     mode: process.env.NODE_ENV,
     entry: config.entry,
     context: config.build.context,
+    stats: {
+        warnings: true,
+        errors: true,
+        errorsCount: true,
+        errorStack: true,
+        errorDetails: true,
+        children: true,
+    },
     resolve: {
         extensions: ["*", ".js", ".jsx"],
         symlinks: false,
         alias: aliases,
+        fallback: {
+            zlib: require.resolve("browserify-zlib"),
+            stream: require.resolve("stream-browserify"),
+            https: require.resolve("https-browserify"),
+            http: require.resolve("stream-http"),
+            url: false,
+            assert: false,
+        },
     },
     output: {
         path: config.build.assetsPath,
         filename: "js/[name].[chunkhash].js",
         chunkFilename: "js/[id].[chunkhash].js",
         publicPath: config.build.assetsURL,
     },
     optimization: {
         minimizer: [
             new TerserPlugin({
                 terserOptions: {
                     parse: {
-                        // we want terser to parse ecma 8 code. However, we don't want it
-                        // to apply any minfication steps that turns valid ecma 5 code
+                        // We want terser to parse ecma 8 code. However, we don't want it
+                        // to apply any minification steps that turns valid ecma 5 code
                         // into invalid ecma 5 code. This is why the 'compress' and 'output'
                         // sections only apply transformations that are ecma 5 safe
                         // https://github.com/facebook/create-react-app/pull/4234
                         ecma: 8,
                     },
                     compress: {
                         ecma: 5,
@@ -80,25 +95,16 @@
                         ecma: 5,
                         comments: false,
                         // Turned on because emoji and regex is not minified properly using default
                         // https://github.com/facebook/create-react-app/issues/2488
                         ascii_only: true,
                     },
                 },
-                // Use multi-process parallel running to improve the build speed
-                // Default number of concurrent runs: os.cpus().length - 1
-                parallel: true,
-                cache: true,
-            }),
-            new OptimizeCSSAssetsPlugin({
-                cssProcessorOptions: {
-                    parser: safePostCssParser,
-                    map: false,
-                },
             }),
+            new CssMinimizerPlugin(),
         ],
         splitChunks: {
             chunks: "all",
         },
         // Extract webpack runtime and module manifest to its own file in order to
         // prevent vendor hash from being updated whenever app bundle is updated.
         runtimeChunk: {
@@ -132,43 +138,60 @@
                 use: [MiniCssExtractPlugin.loader, "css-loader", "sass-loader"],
             }, {
                 test: /\.(less)$/,
                 use: [MiniCssExtractPlugin.loader, "css-loader", "less-loader"],
             },
             // Inline images smaller than 10k
             {
-                test: /\.(png|cur|jpe?g|gif|svg)(\?.*)?$/,
-                use: [{
-                    loader: require.resolve("url-loader"),
-                    options: {
-                        limit: 10000,
-                        name: "img/[name].[hash:7].[ext]",
+                test: /\.(png|jpe?g|gif|svg)(\?.*)?$/,
+                type: "asset/inline",
+                parser: {
+                    dataUrlCondition: {
+                        maxSize: 10 * 1024, // 10kb
                     },
-                }, ],
+                },
+            },
+            // no mimetype for ".cur" in mimetype database, specify it with `generator`
+            {
+                test: /\.(cur)(\?.*)?$/,
+                type: "asset/inline",
+                generator: {
+                    dataUrl: {
+                        encoding: "base64",
+                        mimetype: "image/x-icon",
+                    },
+                },
+                parser: {
+                    dataUrlCondition: {
+                        maxSize: 10 * 1024, // 10kb
+                    },
+                },
             },
             // Inline webfonts smaller than 10k
             {
                 test: /\.(woff2?|eot|ttf|otf)(\?.*)?$/,
-                use: [{
-                    loader: require.resolve("file-loader"),
-                    options: {
-                        limit: 10000,
-                        name: "fonts/[name].[hash:7].[ext]",
+                type: "asset/resource",
+                generator: {
+                    filename: "fonts/[name].[contenthash:7].[ext]",
+                },
+                parser: {
+                    dataUrlCondition: {
+                        maxSize: 10 * 1024, // 10kb
                     },
-                }, ],
+                },
             },
         ],
     },
     devtool: process.env.NODE_ENV === "production" ? "source-map" : "inline-source-map",
     plugins: [
         new ESLintPlugin({
             emitWarning: true,
             quiet: true,
             formatter: require("eslint-friendly-formatter"),
-            eslintPath: require.resolve("eslint")
+            eslintPath: require.resolve("eslint"),
         }),
         // Pragmas
         new webpack.DefinePlugin({
             "process.env": process.env.NODE_ENV,
         }),
         new MiniCssExtractPlugin({
             // Options similar to the same options in webpackOptions.output
@@ -177,14 +200,15 @@
             chunkFilename: "css/[name].[contenthash].css",
         }),
         // Removes the dist folder before each run.
         new CleanWebpackPlugin({
             dry: false,
             verbose: false,
             dangerouslyAllowCleanPatternsOutsideProject: true,
+            cleanStaleWebpackAssets: process.env.NODE_ENV === "production", // keep stale assets in dev because of OS issues
         }),
         // Automatically inject jquery
         new webpack.ProvidePlugin({
             jQuery: "jquery",
             $: "jquery",
             jquery: "jquery",
             "window.jQuery": "jquery",
@@ -195,19 +219,25 @@
             filename: path.join(config.build.assetsPath, "manifest.json"),
             publicPath: config.build.assetsURL,
         }),
     ],
     performance: {
         hints: false
     },
+    snapshot: {
+        managedPaths: [],
+    },
+    watchOptions: {
+        followSymlinks: true,
+    },
 };
 
 if (process.env.npm_config_report) {
-    var BundleAnalyzerPlugin = require("webpack-bundle-analyzer")
-        .BundleAnalyzerPlugin;
+    var BundleAnalyzerPlugin =
+        require("webpack-bundle-analyzer").BundleAnalyzerPlugin;
     webpackConfig.plugins.push(new BundleAnalyzerPlugin());
 }
 
 if (process.env.NODE_ENV === "development") {
     const LiveReloadPlugin = require("webpack-livereload-plugin");
     webpackConfig.plugins.push(new LiveReloadPlugin());
 }
```

### Comparing `invenio-assets-2.0.0/invenio_assets/cli.py` & `invenio-assets-3.0.0/invenio_assets/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/invenio_assets/collect.py` & `invenio-assets-3.0.0/invenio_assets/collect.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/invenio_assets/ext.py` & `invenio-assets-3.0.0/invenio_assets/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/invenio_assets/webpack.py` & `invenio-assets-3.0.0/invenio_assets/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/invenio_assets.egg-info/PKG-INFO` & `invenio-assets-3.0.0/invenio_assets.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-assets
-Version: 2.0.0
+Version: 3.0.0
 Summary: "Media assets management for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-assets
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -45,14 +45,20 @@
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
+        Version 3.0.0 (released 2023-06-08)
+        
+        * upgrade to webpack 5
+        * upgrade js dependencies
+        * upgrade webpack plugins
+        
         Version 2.0.0 (released 2022-10-24)
         
         * upgrade dependencies to node 18 compliance
         
         Version 1.3.1 (released 2022-09-01)
         
         * Upgrade eslint dependencies
```

### Comparing `invenio-assets-2.0.0/invenio_assets.egg-info/SOURCES.txt` & `invenio-assets-3.0.0/invenio_assets.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,12 +43,12 @@
 invenio_assets.egg-info/requires.txt
 invenio_assets.egg-info/top_level.txt
 invenio_assets/assets/.babelrc
 invenio_assets/assets/.eslintignore
 invenio_assets/assets/.eslintrc.js
 invenio_assets/assets/package.json
 invenio_assets/assets/build/webpack.config.js
-invenio_assets/assets/patches/watchpack+1.7.4.patch
+invenio_assets/assets/patches/semantic-ui-less+2.5.0.patch
 tests/conftest.py
 tests/test_invenio_assets.py
 tests/test_invenio_assets_cli.py
 tests/test_webpack.py
```

### Comparing `invenio-assets-2.0.0/setup.cfg` & `invenio-assets-3.0.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/tests/conftest.py` & `invenio-assets-3.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/tests/test_invenio_assets.py` & `invenio-assets-3.0.0/tests/test_invenio_assets.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/tests/test_invenio_assets_cli.py` & `invenio-assets-3.0.0/tests/test_invenio_assets_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-assets-2.0.0/tests/test_webpack.py` & `invenio-assets-3.0.0/tests/test_webpack.py`

 * *Files identical despite different names*

