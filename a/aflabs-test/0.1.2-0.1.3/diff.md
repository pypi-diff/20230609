# Comparing `tmp/aflabs_test-0.1.2.tar.gz` & `tmp/aflabs_test-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aflabs_test-0.1.2.tar", max compression
+gzip compressed data, was "aflabs_test-0.1.3.tar", max compression
```

## Comparing `aflabs_test-0.1.2.tar` & `aflabs_test-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0       19 2023-06-09 13:49:57.239553 aflabs_test-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759473 aflabs_test-0.1.2/aflabs_test/README.rst
--rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.2/aflabs_test/afuser/__init__.py
--rw-r--r--   0        0        0      163 2023-06-09 10:40:21.758253 aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      543 2023-06-09 10:40:21.758253 aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     1118 2023-06-09 10:38:22.121578 aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/boot_django.cpython-311.pyc
--rw-r--r--   0        0        0     1222 2023-06-09 12:15:06.193490 aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0       63 2023-06-09 10:05:52.241773 aflabs_test-0.1.2/aflabs_test/afuser/admin.py
--rw-r--r--   0        0        0      153 2023-06-09 10:05:52.241773 aflabs_test-0.1.2/aflabs_test/afuser/apps.py
--rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.2/aflabs_test/afuser/migrations/__init__.py
--rw-r--r--   0        0        0      459 2023-06-09 12:14:32.665525 aflabs_test-0.1.2/aflabs_test/afuser/models.py
--rw-r--r--   0        0        0       60 2023-06-09 10:05:52.241773 aflabs_test-0.1.2/aflabs_test/afuser/tests.py
--rw-r--r--   0        0        0       63 2023-06-09 10:05:52.241773 aflabs_test-0.1.2/aflabs_test/afuser/views.py
--rw-r--r--   0        0        0      960 2023-06-09 13:45:25.769982 aflabs_test-0.1.2/aflabs_test/setup.cfg
--rw-r--r--   0        0        0       37 2023-06-09 12:41:04.915840 aflabs_test-0.1.2/aflabs_test/setup.py
--rw-r--r--   0        0        0      367 2023-06-09 13:49:04.375933 aflabs_test-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 aflabs_test-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-06-09 13:52:28.974653 aflabs_test-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 13:43:29.759473 aflabs_test-0.1.3/aflabs_test/README.rst
+-rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.3/aflabs_test/afuser/__init__.py
+-rw-r--r--   0        0        0      163 2023-06-09 10:40:21.758253 aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      543 2023-06-09 10:40:21.758253 aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     1118 2023-06-09 10:38:22.121578 aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/boot_django.cpython-311.pyc
+-rw-r--r--   0        0        0     1222 2023-06-09 12:15:06.193490 aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0       89 2023-06-09 13:58:13.809349 aflabs_test-0.1.3/aflabs_test/afuser/admin.py
+-rw-r--r--   0        0        0      153 2023-06-09 10:05:52.241773 aflabs_test-0.1.3/aflabs_test/afuser/apps.py
+-rw-r--r--   0        0        0      164 2023-06-09 13:57:48.693419 aflabs_test-0.1.3/aflabs_test/afuser/forms.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:05:52.241773 aflabs_test-0.1.3/aflabs_test/afuser/migrations/__init__.py
+-rw-r--r--   0        0        0      559 2023-06-09 13:56:29.481660 aflabs_test-0.1.3/aflabs_test/afuser/models.py
+-rw-r--r--   0        0        0       60 2023-06-09 10:05:52.241773 aflabs_test-0.1.3/aflabs_test/afuser/tests.py
+-rw-r--r--   0        0        0      488 2023-06-09 13:57:59.917387 aflabs_test-0.1.3/aflabs_test/afuser/urls.py
+-rw-r--r--   0        0        0     1890 2023-06-09 13:57:24.597489 aflabs_test-0.1.3/aflabs_test/afuser/views.py
+-rw-r--r--   0        0        0      960 2023-06-09 13:45:25.769982 aflabs_test-0.1.3/aflabs_test/setup.cfg
+-rw-r--r--   0        0        0       37 2023-06-09 12:41:04.915840 aflabs_test-0.1.3/aflabs_test/setup.py
+-rw-r--r--   0        0        0      367 2023-06-09 14:00:50.248981 aflabs_test-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 aflabs_test-0.1.3/PKG-INFO
```

### Comparing `aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/apps.cpython-311.pyc` & `aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/apps.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/boot_django.cpython-311.pyc` & `aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/boot_django.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aflabs_test-0.1.2/aflabs_test/afuser/__pycache__/models.cpython-311.pyc` & `aflabs_test-0.1.3/aflabs_test/afuser/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `aflabs_test-0.1.2/aflabs_test/setup.cfg` & `aflabs_test-0.1.3/aflabs_test/setup.cfg`

 * *Files identical despite different names*

