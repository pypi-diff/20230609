# Comparing `tmp/pypinterest-0.0.1.tar.gz` & `tmp/pypinterest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypinterest-0.0.1.tar", last modified: Sun Jun  4 07:31:04 2023, max compression
+gzip compressed data, was "pypinterest-0.0.2.tar", last modified: Fri Jun  9 03:49:18 2023, max compression
```

## Comparing `pypinterest-0.0.1.tar` & `pypinterest-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 07:31:04.305586 pypinterest-0.0.1/
--rw-rw-rw-   0        0        0    11553 2023-06-04 07:18:01.000000 pypinterest-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      283 2023-06-04 07:31:04.305586 pypinterest-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-04 07:24:30.000000 pypinterest-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 07:31:04.305586 pypinterest-0.0.1/pypinterest.egg-info/
--rw-rw-rw-   0        0        0      283 2023-06-04 07:31:04.000000 pypinterest-0.0.1/pypinterest.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-06-04 07:31:04.000000 pypinterest-0.0.1/pypinterest.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 07:31:04.000000 pypinterest-0.0.1/pypinterest.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      101 2023-06-04 07:31:04.000000 pypinterest-0.0.1/pypinterest.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 07:31:04.000000 pypinterest-0.0.1/pypinterest.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 07:31:04.305586 pypinterest-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1819 2023-06-04 07:25:38.000000 pypinterest-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 03:49:18.621223 pypinterest-0.0.2/
+-rw-rw-rw-   0        0        0    11553 2023-06-04 07:18:01.000000 pypinterest-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      283 2023-06-09 03:49:18.621223 pypinterest-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-04 07:24:30.000000 pypinterest-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-09 03:49:18.612769 pypinterest-0.0.2/pypinterest.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      101 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 03:49:18.000000 pypinterest-0.0.2/pypinterest.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 03:49:18.621223 pypinterest-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2023-06-04 07:25:38.000000 pypinterest-0.0.2/setup.py
```

### Comparing `pypinterest-0.0.1/LICENSE` & `pypinterest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pypinterest-0.0.1/setup.py` & `pypinterest-0.0.2/setup.py`

 * *Files identical despite different names*

