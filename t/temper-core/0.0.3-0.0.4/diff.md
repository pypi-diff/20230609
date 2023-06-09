# Comparing `tmp/temper_core-0.0.3.tar.gz` & `tmp/temper_core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_core-0.0.3.tar", max compression
+gzip compressed data, was "temper_core-0.0.4.tar", max compression
```

## Comparing `temper_core-0.0.3.tar` & `temper_core-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      415 2022-12-19 18:05:07.926438 temper_core-0.0.3/pyproject.toml
--rw-r--r--   0        0        0    19766 2022-12-19 18:05:07.928440 temper_core-0.0.3/temper_core/__init__.py
--rw-r--r--   0        0        0     1189 2022-12-19 18:05:07.929439 temper_core-0.0.3/temper_core/regex.py
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 temper_core-0.0.3/setup.py
--rw-r--r--   0        0        0      595 1970-01-01 00:00:00.000000 temper_core-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      428 2023-06-09 16:40:49.254815 temper_core-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0    25341 2023-06-09 16:40:49.256811 temper_core-0.0.4/temper_core/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 16:40:49.255812 temper_core-0.0.4/temper_core/py.typed
+-rw-r--r--   0        0        0     1544 2023-06-09 16:40:49.257810 temper_core-0.0.4/temper_core/regex.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 temper_core-0.0.4/PKG-INFO
```

