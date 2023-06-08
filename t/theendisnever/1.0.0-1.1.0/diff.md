# Comparing `tmp/theendisnever-1.0.0.tar.gz` & `tmp/theendisnever-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "theendisnever-1.1.0.tar", last modified: Thu Jun  8 22:27:52 2023, max compression
```

## Comparing `theendisnever-1.0.0.tar` & `theendisnever-1.1.0.tar`

### file list

```diff
@@ -1,10 +1,15 @@
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 theendisnever-1.0.0/dev.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 theendisnever-1.0.0/environment.yml
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 theendisnever-1.0.0/prod.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 theendisnever-1.0.0/src/theendisnever/__init__.py
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 theendisnever-1.0.0/src/theendisnever/theend.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 theendisnever-1.0.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 theendisnever-1.0.0/LICENSE
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 theendisnever-1.0.0/README.md
--rw-r--r--   0        0        0      610 2020-02-02 00:00:00.000000 theendisnever-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 theendisnever-1.0.0/PKG-INFO
+drwxrwxr-x   0 andrewhinh  (1000) andrewhinh  (1000)        0 2023-06-08 22:27:52.469648 theendisnever-1.1.0/
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)     1068 2023-06-07 22:53:32.000000 theendisnever-1.1.0/LICENSE
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)     2696 2023-06-08 22:27:52.469648 theendisnever-1.1.0/PKG-INFO
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)     2146 2023-06-08 22:16:32.000000 theendisnever-1.1.0/README.md
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)      672 2023-06-08 22:26:55.000000 theendisnever-1.1.0/pyproject.toml
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)       38 2023-06-08 22:27:52.469648 theendisnever-1.1.0/setup.cfg
+drwxrwxr-x   0 andrewhinh  (1000) andrewhinh  (1000)        0 2023-06-08 22:27:52.469648 theendisnever-1.1.0/src/
+drwxrwxr-x   0 andrewhinh  (1000) andrewhinh  (1000)        0 2023-06-08 22:27:52.469648 theendisnever-1.1.0/src/theendisnever/
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)        0 2023-06-08 14:26:06.000000 theendisnever-1.1.0/src/theendisnever/__init__.py
+-rw-r--r--   0 andrewhinh  (1000) andrewhinh  (1000)     2800 2023-06-08 17:49:38.000000 theendisnever-1.1.0/src/theendisnever/theend.py
+drwxrwxr-x   0 andrewhinh  (1000) andrewhinh  (1000)        0 2023-06-08 22:27:52.469648 theendisnever-1.1.0/src/theendisnever.egg-info/
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)     2696 2023-06-08 22:27:52.000000 theendisnever-1.1.0/src/theendisnever.egg-info/PKG-INFO
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)      254 2023-06-08 22:27:52.000000 theendisnever-1.1.0/src/theendisnever.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)        1 2023-06-08 22:27:52.000000 theendisnever-1.1.0/src/theendisnever.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrewhinh  (1000) andrewhinh  (1000)       14 2023-06-08 22:27:52.000000 theendisnever-1.1.0/src/theendisnever.egg-info/top_level.txt
```

### Comparing `theendisnever-1.0.0/src/theendisnever/theend.py` & `theendisnever-1.1.0/src/theendisnever/theend.py`

 * *Files identical despite different names*

### Comparing `theendisnever-1.0.0/LICENSE` & `theendisnever-1.1.0/LICENSE`

 * *Files identical despite different names*

