# Comparing `tmp/testing_poetry-1.0.1.tar.gz` & `tmp/testing_poetry-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testing_poetry-1.0.1.tar", max compression
+gzip compressed data, was "testing_poetry-1.0.2.tar", max compression
```

## Comparing `testing_poetry-1.0.1.tar` & `testing_poetry-1.0.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0       21 2023-06-09 14:36:29.313015 testing_poetry-1.0.1/README.md
--rw-r--r--   0        0        0      407 2023-06-09 14:56:50.705678 testing_poetry-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      129 2023-06-09 14:53:00.531336 testing_poetry-1.0.1/testing_poetry/main.py
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 testing_poetry-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       21 2023-06-09 14:36:29.313015 testing_poetry-1.0.2/README.md
+-rw-r--r--   0        0        0      411 2023-06-09 14:58:49.588171 testing_poetry-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      129 2023-06-09 14:53:00.531336 testing_poetry-1.0.2/testing_poetry/main.py
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 testing_poetry-1.0.2/PKG-INFO
```

