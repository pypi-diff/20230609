# Comparing `tmp/beanie_batteries_queue-0.1.0.tar.gz` & `tmp/beanie_batteries_queue-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beanie_batteries_queue-0.1.0.tar", max compression
+gzip compressed data, was "beanie_batteries_queue-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `beanie_batteries_queue-0.1.0.tar` & `beanie_batteries_queue-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,14 @@
--rw-r--r--   0        0        0      145 2023-05-25 20:54:40.364811 beanie_batteries_queue-0.1.0/README.md
--rw-r--r--   0        0        0       88 2023-05-25 20:58:36.779702 beanie_batteries_queue-0.1.0/beanie_batteries_queue/__init__.py
--rw-r--r--   0        0        0     1944 2023-05-25 20:57:53.467906 beanie_batteries_queue-0.1.0/beanie_batteries_queue/queue.py
--rw-r--r--   0        0        0     1656 2023-05-25 20:37:20.565342 beanie_batteries_queue-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      742 1970-01-01 00:00:00.000000 beanie_batteries_queue-0.1.0/setup.py
--rw-r--r--   0        0        0      631 1970-01-01 00:00:00.000000 beanie_batteries_queue-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      373 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.github/workflows/github-actions-publish-project.yml
+-rw-r--r--   0        0        0      816 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.github/workflows/github-actions-tests.yml
+-rw-r--r--   0        0        0     2623 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.gitignore
+-rw-r--r--   0        0        0      475 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11343 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/LICENSE
+-rw-r--r--   0        0        0      145 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/README.md
+-rw-r--r--   0        0        0      180 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/beanie_batteries_queue/__init__.py
+-rw-r--r--   0        0        0     5189 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/beanie_batteries_queue/queue.py
+-rw-r--r--   0        0        0     2375 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     1291 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0     1186 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/tasks.py
+-rw-r--r--   0        0        0     7542 2023-06-09 19:45:53.159658 beanie_batteries_queue-0.2.0/tests/test_tasks.py
+-rw-r--r--   0        0        0     1080 1970-01-01 00:00:00.000000 beanie_batteries_queue-0.2.0/PKG-INFO
```

