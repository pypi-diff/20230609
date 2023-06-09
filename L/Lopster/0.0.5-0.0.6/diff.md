# Comparing `tmp/Lopster-0.0.5.tar.gz` & `tmp/Lopster-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Lopster-0.0.5.tar", last modified: Fri Jun  9 15:54:06 2023, max compression
+gzip compressed data, was "Lopster-0.0.6.tar", last modified: Fri Jun  9 15:58:31 2023, max compression
```

## Comparing `Lopster-0.0.5.tar` & `Lopster-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 15:54:06.600476 Lopster-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-06-09 15:54:06.569218 Lopster-0.0.5/Lopster/
--rw-rw-rw-   0        0        0     7201 2023-06-09 15:29:02.000000 Lopster-0.0.5/Lopster/Lopster.py
--rw-rw-rw-   0        0        0       73 2023-06-09 15:53:47.000000 Lopster-0.0.5/Lopster/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-09 15:54:06.600476 Lopster-0.0.5/Lopster.egg-info/
--rw-rw-rw-   0        0        0      235 2023-06-09 15:54:06.000000 Lopster-0.0.5/Lopster.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-06-09 15:54:06.000000 Lopster-0.0.5/Lopster.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 15:54:06.000000 Lopster-0.0.5/Lopster.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-09 15:54:06.000000 Lopster-0.0.5/Lopster.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-09 15:54:06.000000 Lopster-0.0.5/Lopster.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      235 2023-06-09 15:54:06.600476 Lopster-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-09 15:54:06.600476 Lopster-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      383 2023-06-09 15:54:01.000000 Lopster-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:58:31.823288 Lopster-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:58:31.792029 Lopster-0.0.6/Lopster/
+-rw-rw-rw-   0        0        0     7201 2023-06-09 15:29:02.000000 Lopster-0.0.6/Lopster/Lopster.py
+-rw-rw-rw-   0        0        0     7350 2023-06-09 15:58:27.000000 Lopster-0.0.6/Lopster/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:58:31.823288 Lopster-0.0.6/Lopster.egg-info/
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-09 15:58:31.000000 Lopster-0.0.6/Lopster.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-06-09 15:58:31.823288 Lopster-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:58:31.823288 Lopster-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      383 2023-06-09 15:58:27.000000 Lopster-0.0.6/setup.py
```

### Comparing `Lopster-0.0.5/Lopster/Lopster.py` & `Lopster-0.0.6/Lopster/Lopster.py`

 * *Files identical despite different names*

