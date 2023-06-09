# Comparing `tmp/aflabs_test-0.1.0.tar.gz` & `tmp/aflabs_test-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aflabs_test-0.1.0.tar", max compression
+gzip compressed data, was "aflabs_test-0.1.1.tar", max compression
```

## Comparing `aflabs_test-0.1.0.tar` & `aflabs_test-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       35 2023-06-09 10:23:07.869221 aflabs_test-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.0/aflabs_test/__init__.py
--rw-r--r--   0        0        0       63 2023-06-09 10:05:52.241773 aflabs_test-0.1.0/aflabs_test/admin.py
--rw-r--r--   0        0        0      153 2023-06-09 10:05:52.241773 aflabs_test-0.1.0/aflabs_test/apps.py
--rw-r--r--   0        0        0      700 2023-06-09 10:15:47.044953 aflabs_test-0.1.0/aflabs_test/boot_django.py
--rw-r--r--   0        0        0      142 2023-06-09 10:20:32.301082 aflabs_test-0.1.0/aflabs_test/makemigrations.py
--rw-r--r--   0        0        0      136 2023-06-09 10:22:05.973161 aflabs_test-0.1.0/aflabs_test/migrate.py
--rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.0/aflabs_test/migrations/__init__.py
--rw-r--r--   0        0        0      426 2023-06-09 10:13:32.980975 aflabs_test-0.1.0/aflabs_test/models.py
--rw-r--r--   0        0        0       60 2023-06-09 10:05:52.241773 aflabs_test-0.1.0/aflabs_test/tests.py
--rw-r--r--   0        0        0       63 2023-06-09 10:05:52.241773 aflabs_test-0.1.0/aflabs_test/views.py
--rw-r--r--   0        0        0      367 2023-06-09 10:17:52.520985 aflabs_test-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aflabs_test-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       35 2023-06-09 10:23:07.869221 aflabs_test-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.1/aflabs_test/__init__.py
+-rw-r--r--   0        0        0       63 2023-06-09 10:05:52.241773 aflabs_test-0.1.1/aflabs_test/admin.py
+-rw-r--r--   0        0        0      153 2023-06-09 10:05:52.241773 aflabs_test-0.1.1/aflabs_test/apps.py
+-rw-r--r--   0        0        0      700 2023-06-09 10:15:47.044953 aflabs_test-0.1.1/aflabs_test/boot_django.py
+-rw-r--r--   0        0        0      199 2023-06-09 12:23:11.389493 aflabs_test-0.1.1/aflabs_test/makemigrations.py
+-rw-r--r--   0        0        0      151 2023-06-09 12:23:11.385492 aflabs_test-0.1.1/aflabs_test/migrate.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.1/aflabs_test/migrations/__init__.py
+-rw-r--r--   0        0        0      459 2023-06-09 12:14:32.665525 aflabs_test-0.1.1/aflabs_test/models.py
+-rw-r--r--   0        0        0       60 2023-06-09 10:05:52.241773 aflabs_test-0.1.1/aflabs_test/tests.py
+-rw-r--r--   0        0        0       63 2023-06-09 10:05:52.241773 aflabs_test-0.1.1/aflabs_test/views.py
+-rw-r--r--   0        0        0      367 2023-06-09 12:47:11.448672 aflabs_test-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aflabs_test-0.1.1/PKG-INFO
```

### Comparing `aflabs_test-0.1.0/aflabs_test/boot_django.py` & `aflabs_test-0.1.1/aflabs_test/boot_django.py`

 * *Files identical despite different names*

