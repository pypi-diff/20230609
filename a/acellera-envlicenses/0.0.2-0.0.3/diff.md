# Comparing `tmp/acellera-envlicenses-0.0.2.tar.gz` & `tmp/acellera-envlicenses-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acellera-envlicenses-0.0.2.tar", last modified: Thu Jun  8 14:15:23 2023, max compression
+gzip compressed data, was "acellera-envlicenses-0.0.3.tar", last modified: Fri Jun  9 13:16:50 2023, max compression
```

## Comparing `acellera-envlicenses-0.0.2.tar` & `acellera-envlicenses-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 14:15:23.000000 acellera-envlicenses-0.0.2/acellera_envlicenses.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/envlicenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/envlicenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/envlicenses/permissive.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:15:23.432448 acellera-envlicenses-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-08 14:15:11.000000 acellera-envlicenses-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:16:50.043290 acellera-envlicenses-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 13:16:50.043290 acellera-envlicenses-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 13:16:38.000000 acellera-envlicenses-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:16:50.043290 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-09 13:16:49.000000 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-09 13:16:50.000000 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:16:49.000000 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 13:16:49.000000 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 13:16:49.000000 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 13:16:49.000000 acellera-envlicenses-0.0.3/acellera_envlicenses.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 13:16:50.043290 acellera-envlicenses-0.0.3/envlicenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-09 13:16:38.000000 acellera-envlicenses-0.0.3/envlicenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-09 13:16:38.000000 acellera-envlicenses-0.0.3/envlicenses/permissive.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 13:16:50.043290 acellera-envlicenses-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-09 13:16:38.000000 acellera-envlicenses-0.0.3/setup.py
```

### Comparing `acellera-envlicenses-0.0.2/envlicenses/__init__.py` & `acellera-envlicenses-0.0.3/envlicenses/__init__.py`

 * *Files identical despite different names*

### Comparing `acellera-envlicenses-0.0.2/envlicenses/permissive.txt` & `acellera-envlicenses-0.0.3/envlicenses/permissive.txt`

 * *Files 8% similar despite different names*

```diff
@@ -66,8 +66,12 @@
 Public-Domain AND BSD-3-clause
 bzip2
 HPND
 LicenseRef-PSF-2.0 and CC0-1.0
 JasPer-2.0
 zlib-acknowledgement
 PostgreSQL
-BSD-2-Clause AND BSD-3-Clause
+BSD-2-Clause AND BSD-3-Clause
+CC-PDDC OR BSD-3-Clause
+CC-PDDC
+BSD-4-Clause
+CC-BY-4.0
```

### Comparing `acellera-envlicenses-0.0.2/setup.py` & `acellera-envlicenses-0.0.3/setup.py`

 * *Files identical despite different names*

