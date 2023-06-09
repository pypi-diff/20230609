# Comparing `tmp/etos_lib-3.1.0.tar.gz` & `tmp/etos_lib-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_lib-3.1.0.tar", last modified: Thu Jun  8 05:46:27 2023, max compression
+gzip compressed data, was "etos_lib-3.2.0.tar", last modified: Fri Jun  9 06:01:50 2023, max compression
```

## Comparing `etos_lib-3.1.0.tar` & `etos_lib-3.2.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.840068 etos_lib-3.1.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-06-08 05:45:47.000000 etos_lib-3.1.0/.coveragerc
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/.github/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/.github/workflows/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-06-08 05:45:47.000000 etos_lib-3.1.0/.github/workflows/main.yml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      542 2023-06-08 05:45:47.000000 etos_lib-3.1.0/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-06-08 05:45:47.000000 etos_lib-3.1.0/AUTHORS.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-06-08 05:45:47.000000 etos_lib-3.1.0/CODEOWNERS
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-06-08 05:45:47.000000 etos_lib-3.1.0/LICENSE.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-08 05:46:27.840068 etos_lib-3.1.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-06-08 05:45:47.000000 etos_lib-3.1.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-06-08 05:45:47.000000 etos_lib-3.1.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1413 2023-06-08 05:46:27.840068 etos_lib-3.1.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-06-08 05:45:47.000000 etos_lib-3.1.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4915 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/etos.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/graphql/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/graphql/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/graphql/query_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/kubernetes/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/kubernetes/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3103 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/kubernetes/base.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3288 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/kubernetes/jobs.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4814 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/config.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/database.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5164 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/debug.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/events.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/exceptions.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/feature_flags.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/http.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/monitor.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/utils.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.840068 etos_lib-3.1.0/src/etos_lib/logging/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/default_config.yaml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/filter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/formatter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1967 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/log_publisher.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     6829 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/logger.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2331 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/rabbitmq_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1316 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/top_level.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-06-08 05:45:47.000000 etos_lib-3.1.0/test-requirements.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.840068 etos_lib-3.1.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-06-08 05:45:47.000000 etos_lib-3.1.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-06-08 05:45:47.000000 etos_lib-3.1.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-06-08 05:45:47.000000 etos_lib-3.1.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.972139 etos_lib-3.2.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-06-08 05:45:47.000000 etos_lib-3.2.0/.coveragerc
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/.github/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/.github/workflows/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-06-08 05:45:47.000000 etos_lib-3.2.0/.github/workflows/main.yml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      542 2023-06-08 05:45:47.000000 etos_lib-3.2.0/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-06-08 05:45:47.000000 etos_lib-3.2.0/AUTHORS.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-06-08 05:45:47.000000 etos_lib-3.2.0/CODEOWNERS
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-06-08 05:45:47.000000 etos_lib-3.2.0/LICENSE.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-09 06:01:50.972139 etos_lib-3.2.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-06-08 05:45:47.000000 etos_lib-3.2.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-06-08 05:45:47.000000 etos_lib-3.2.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-06-08 05:45:47.000000 etos_lib-3.2.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1413 2023-06-09 06:01:50.972139 etos_lib-3.2.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-06-08 05:45:47.000000 etos_lib-3.2.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/src/etos_lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4915 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/etos.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/src/etos_lib/graphql/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/graphql/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/graphql/query_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/src/etos_lib/kubernetes/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/kubernetes/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3103 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/kubernetes/base.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3288 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/kubernetes/jobs.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.972139 etos_lib-3.2.0/src/etos_lib/lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4814 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/config.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/database.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5179 2023-06-09 06:01:45.000000 etos_lib-3.2.0/src/etos_lib/lib/debug.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/events.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/exceptions.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/feature_flags.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/http.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/monitor.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/lib/utils.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.972139 etos_lib-3.2.0/src/etos_lib/logging/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/default_config.yaml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/filter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/formatter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1967 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/log_publisher.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     6829 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/logger.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2331 2023-06-08 05:45:47.000000 etos_lib-3.2.0/src/etos_lib/logging/rabbitmq_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.968139 etos_lib-3.2.0/src/etos_lib.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-09 06:01:50.000000 etos_lib-3.2.0/src/etos_lib.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1316 2023-06-09 06:01:50.000000 etos_lib-3.2.0/src/etos_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-09 06:01:50.000000 etos_lib-3.2.0/src/etos_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-08 05:46:27.000000 etos_lib-3.2.0/src/etos_lib.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-06-09 06:01:50.000000 etos_lib-3.2.0/src/etos_lib.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-09 06:01:50.000000 etos_lib-3.2.0/src/etos_lib.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-06-08 05:45:47.000000 etos_lib-3.2.0/test-requirements.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-09 06:01:50.972139 etos_lib-3.2.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-06-08 05:45:47.000000 etos_lib-3.2.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-06-08 05:45:47.000000 etos_lib-3.2.0/tests/conftest.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-06-08 05:45:47.000000 etos_lib-3.2.0/tox.ini
```

### Comparing `etos_lib-3.1.0/.coveragerc` & `etos_lib-3.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/.github/workflows/main.yml` & `etos_lib-3.2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/.gitignore` & `etos_lib-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/LICENSE.txt` & `etos_lib-3.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/PKG-INFO` & `etos_lib-3.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_lib
-Version: 3.1.0
+Version: 3.2.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-3.1.0/README.rst` & `etos_lib-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/docs/Makefile` & `etos_lib-3.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/docs/conf.py` & `etos_lib-3.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/setup.cfg` & `etos_lib-3.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/setup.py` & `etos_lib-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/__init__.py` & `etos_lib-3.2.0/src/etos_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/etos.py` & `etos_lib-3.2.0/src/etos_lib/etos.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/graphql/__init__.py` & `etos_lib-3.2.0/src/etos_lib/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/graphql/query_handler.py` & `etos_lib-3.2.0/src/etos_lib/graphql/query_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/kubernetes/__init__.py` & `etos_lib-3.2.0/src/etos_lib/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/kubernetes/base.py` & `etos_lib-3.2.0/src/etos_lib/kubernetes/base.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/kubernetes/jobs.py` & `etos_lib-3.2.0/src/etos_lib/kubernetes/jobs.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/__init__.py` & `etos_lib-3.2.0/src/etos_lib/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/config.py` & `etos_lib-3.2.0/src/etos_lib/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/database.py` & `etos_lib-3.2.0/src/etos_lib/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/debug.py` & `etos_lib-3.2.0/src/etos_lib/lib/debug.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,16 +50,16 @@
     @property
     def disable_sending_events(self):
         """Disable sending eiffel events."""
         return bool(os.getenv("ETOS_DISABLE_SENDING_EVENTS", None))
 
     @property
     def enable_sending_logs(self):
-        """Disable sending eiffel events."""
-        return bool(os.getenv("ETOS_ENABLE_SENDING_LOGS", None))
+        """Enable sending ETOS log events."""
+        return os.getenv("ETOS_ENABLE_SENDING_LOGS", "true").lower() == "true"
 
     @property
     def disable_receiving_events(self):
         """Disable receiving eiffel events."""
         return bool(os.getenv("ETOS_DISABLE_RECEIVING_EVENTS", None))
 
     @property
```

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/events.py` & `etos_lib-3.2.0/src/etos_lib/lib/events.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/exceptions.py` & `etos_lib-3.2.0/src/etos_lib/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/feature_flags.py` & `etos_lib-3.2.0/src/etos_lib/lib/feature_flags.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/http.py` & `etos_lib-3.2.0/src/etos_lib/lib/http.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/monitor.py` & `etos_lib-3.2.0/src/etos_lib/lib/monitor.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/lib/utils.py` & `etos_lib-3.2.0/src/etos_lib/lib/utils.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/logging/__init__.py` & `etos_lib-3.2.0/src/etos_lib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/logging/filter.py` & `etos_lib-3.2.0/src/etos_lib/logging/filter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/logging/formatter.py` & `etos_lib-3.2.0/src/etos_lib/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/logging/log_publisher.py` & `etos_lib-3.2.0/src/etos_lib/logging/log_publisher.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/logging/logger.py` & `etos_lib-3.2.0/src/etos_lib/logging/logger.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib/logging/rabbitmq_handler.py` & `etos_lib-3.2.0/src/etos_lib/logging/rabbitmq_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/src/etos_lib.egg-info/PKG-INFO` & `etos_lib-3.2.0/src/etos_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos-lib
-Version: 3.1.0
+Version: 3.2.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-3.1.0/src/etos_lib.egg-info/SOURCES.txt` & `etos_lib-3.2.0/src/etos_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-3.1.0/tests/__init__.py` & `etos_lib-3.2.0/tests/__init__.py`

 * *Files identical despite different names*

