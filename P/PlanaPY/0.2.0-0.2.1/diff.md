# Comparing `tmp/PlanaPY-0.2.0.tar.gz` & `tmp/PlanaPY-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PlanaPY-0.2.0.tar", last modified: Tue Jun  6 06:29:30 2023, max compression
+gzip compressed data, was "PlanaPY-0.2.1.tar", last modified: Fri Jun  9 20:29:06 2023, max compression
```

## Comparing `PlanaPY-0.2.0.tar` & `PlanaPY-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.514716 PlanaPY-0.2.0/
--rw-rw-rw-   0        0        0     1078 2023-06-06 05:14:36.000000 PlanaPY-0.2.0/License.txt
--rw-rw-rw-   0        0        0      272 2023-06-06 06:29:30.512818 PlanaPY-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 06:29:30.515721 PlanaPY-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      482 2023-06-06 06:29:10.000000 PlanaPY-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.451276 PlanaPY-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.477744 PlanaPY-0.2.0/src/PlanaPY/
--rw-rw-rw-   0        0        0        0 2023-06-06 06:28:39.000000 PlanaPY-0.2.0/src/PlanaPY/__init__.py
--rw-rw-rw-   0        0        0    13468 2023-06-05 22:36:53.000000 PlanaPY-0.2.0/src/PlanaPY/anaplan_api.py
-drwxrwxrwx   0        0        0        0 2023-06-06 06:29:30.509733 PlanaPY-0.2.0/src/PlanaPY.egg-info/
--rw-rw-rw-   0        0        0      272 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-06 06:29:30.000000 PlanaPY-0.2.0/src/PlanaPY.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 20:29:06.858405 PlanaPY-0.2.1/
+-rw-rw-rw-   0        0        0      286 2023-06-09 20:29:06.857406 PlanaPY-0.2.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-09 20:29:06.856410 PlanaPY-0.2.1/PlanaPY.egg-info/
+-rw-rw-rw-   0        0        0      286 2023-06-09 20:29:06.000000 PlanaPY-0.2.1/PlanaPY.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      172 2023-06-09 20:29:06.000000 PlanaPY-0.2.1/PlanaPY.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:29:06.000000 PlanaPY-0.2.1/PlanaPY.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-09 20:29:06.000000 PlanaPY-0.2.1/PlanaPY.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 20:29:06.000000 PlanaPY-0.2.1/PlanaPY.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-06-06 05:35:28.000000 PlanaPY-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 20:29:06.859407 PlanaPY-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      485 2023-06-09 19:49:49.000000 PlanaPY-0.2.1/setup.py
```

