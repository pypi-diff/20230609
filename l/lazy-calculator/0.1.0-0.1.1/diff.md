# Comparing `tmp/lazy_calculator-0.1.0.tar.gz` & `tmp/lazy_calculator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_calculator-0.1.0.tar", max compression
+gzip compressed data, was "lazy_calculator-0.1.1.tar", max compression
```

## Comparing `lazy_calculator-0.1.0.tar` & `lazy_calculator-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-06-09 15:23:49.150279 lazy_calculator-0.1.0/LICENSE
--rw-r--r--   0        0        0       17 2023-06-09 15:21:55.902938 lazy_calculator-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-06-09 15:17:45.040357 lazy_calculator-0.1.0/lazy_calculator/__init__.py
--rw-r--r--   0        0        0      384 2023-06-09 15:48:31.093831 lazy_calculator-0.1.0/lazy_calculator/factorial.py
--rw-r--r--   0        0        0      420 2023-06-09 15:46:27.657912 lazy_calculator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      507 1970-01-01 00:00:00.000000 lazy_calculator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-09 15:23:49.150279 lazy_calculator-0.1.1/LICENSE
+-rw-r--r--   0        0        0       18 2023-06-09 15:53:10.167861 lazy_calculator-0.1.1/README.md
+-rw-r--r--   0        0        0       74 2023-06-09 16:03:28.709786 lazy_calculator-0.1.1/lazy_calculator/__init__.py
+-rw-r--r--   0        0        0      384 2023-06-09 15:48:31.093831 lazy_calculator-0.1.1/lazy_calculator/factorial.py
+-rw-r--r--   0        0        0      420 2023-06-09 16:04:02.734532 lazy_calculator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      508 1970-01-01 00:00:00.000000 lazy_calculator-0.1.1/PKG-INFO
```

### Comparing `lazy_calculator-0.1.0/LICENSE` & `lazy_calculator-0.1.1/LICENSE`

 * *Files identical despite different names*

