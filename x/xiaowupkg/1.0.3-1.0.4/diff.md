# Comparing `tmp/xiaowupkg-1.0.3.tar.gz` & `tmp/xiaowupkg-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xiaowupkg-1.0.3.tar", last modified: Thu Jun  1 09:59:48 2023, max compression
+gzip compressed data, was "xiaowupkg-1.0.4.tar", last modified: Fri Jun  9 08:08:03 2023, max compression
```

## Comparing `xiaowupkg-1.0.3.tar` & `xiaowupkg-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:59:48.230164 xiaowupkg-1.0.3/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 09:59:48.210163 xiaowupkg-1.0.3/PKG-INFO
--rwxrw-rw-   0 root         (0) root         (0)      105 2023-06-01 09:52:58.000000 xiaowupkg-1.0.3/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 09:59:48.230164 xiaowupkg-1.0.3/setup.cfg
--rwxrw-rw-   0 root         (0) root         (0)      342 2023-06-01 09:58:48.000000 xiaowupkg-1.0.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:59:48.034163 xiaowupkg-1.0.3/xiaowupkg/
--rwxrw-rw-   0 root         (0) root         (0)      193 2023-06-01 09:50:19.000000 xiaowupkg-1.0.3/xiaowupkg/__init__.py
--rwxrw-rw-   0 root         (0) root         (0)      697 2023-06-01 06:46:27.000000 xiaowupkg-1.0.3/xiaowupkg/filefunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 09:59:48.178164 xiaowupkg-1.0.3/xiaowupkg.egg-info/
--rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 09:59:47.000000 xiaowupkg-1.0.3/xiaowupkg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      226 2023-06-01 09:59:47.000000 xiaowupkg-1.0.3/xiaowupkg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 09:59:47.000000 xiaowupkg-1.0.3/xiaowupkg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 09:59:47.000000 xiaowupkg-1.0.3/xiaowupkg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-01 09:59:47.000000 xiaowupkg-1.0.3/xiaowupkg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 08:08:03.417691 xiaowupkg-1.0.4/
+-rw-rw-rw-   0        0        0      158 2023-06-09 08:08:03.395745 xiaowupkg-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      105 2023-06-01 09:52:58.000000 xiaowupkg-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 08:08:03.418686 xiaowupkg-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      350 2023-06-09 08:07:14.000000 xiaowupkg-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:08:03.380786 xiaowupkg-1.0.4/xiaowupkg/
+-rw-rw-rw-   0        0        0      193 2023-06-01 09:50:19.000000 xiaowupkg-1.0.4/xiaowupkg/__init__.py
+-rw-rw-rw-   0        0        0      697 2023-06-01 06:46:27.000000 xiaowupkg-1.0.4/xiaowupkg/filefunc.py
+drwxrwxrwx   0        0        0        0 2023-06-09 08:08:03.395745 xiaowupkg-1.0.4/xiaowupkg.egg-info/
+-rw-rw-rw-   0        0        0      158 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      194 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-09 08:08:03.000000 xiaowupkg-1.0.4/xiaowupkg.egg-info/top_level.txt
```

### Comparing `xiaowupkg-1.0.3/xiaowupkg/filefunc.py` & `xiaowupkg-1.0.4/xiaowupkg/filefunc.py`

 * *Files identical despite different names*

