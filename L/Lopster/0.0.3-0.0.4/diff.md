# Comparing `tmp/Lopster-0.0.3.tar.gz` & `tmp/Lopster-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.0.3.tar", last modified: Fri Jun  9 15:45:29 2023, max compression
+gzip compressed data, was "Lopster-0.0.4.tar", last modified: Fri Jun  9 15:47:26 2023, max compression
```

## Comparing `Lopster-0.0.3.tar` & `Lopster-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:45:29.749031 Lopster-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-06-09 15:45:29.717784 Lopster-0.0.3/Lopster/
--rw-rw-rw-   0        0        0     7201 2023-06-09 15:29:02.000000 Lopster-0.0.3/Lopster/Lopster.py
--rw-rw-rw-   0        0        0       21 2023-06-09 15:29:47.000000 Lopster-0.0.3/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:45:29.749031 Lopster-0.0.3/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-09 15:45:29.000000 Lopster-0.0.3/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-09 15:45:29.000000 Lopster-0.0.3/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:45:29.000000 Lopster-0.0.3/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 15:45:29.000000 Lopster-0.0.3/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 15:45:29.000000 Lopster-0.0.3/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-09 15:45:29.749031 Lopster-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 15:45:29.749031 Lopster-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-06-09 15:45:28.000000 Lopster-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:47:26.260209 Lopster-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:47:26.228964 Lopster-0.0.4/Lopster/
+-rw-rw-rw-   0        0        0     7201 2023-06-09 15:29:02.000000 Lopster-0.0.4/Lopster/Lopster.py
+-rw-rw-rw-   0        0        0       21 2023-06-09 15:29:47.000000 Lopster-0.0.4/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:47:26.244586 Lopster-0.0.4/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:47:26.000000 Lopster-0.0.4/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-09 15:47:26.000000 Lopster-0.0.4/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:47:26.000000 Lopster-0.0.4/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 15:47:26.000000 Lopster-0.0.4/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 15:47:26.000000 Lopster-0.0.4/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:47:26.244586 Lopster-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:47:26.260209 Lopster-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-09 15:47:23.000000 Lopster-0.0.4/setup.py
```

### Comparing `Lopster-0.0.3/Lopster/Lopster.py` & `Lopster-0.0.4/Lopster/Lopster.py`

 * *Files identical despite different names*

