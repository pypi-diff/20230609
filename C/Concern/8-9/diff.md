# Comparing `tmp/Concern-8.tar.gz` & `tmp/Concern-9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Concern-8.tar", last modified: Sun Oct  6 19:33:48 2019, max compression
+gzip compressed data, was "dist/Concern-9.tar", last modified: Mon Oct  7 20:55:34 2019, max compression
```

## Comparing `Concern-8.tar` & `Concern-9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-10-06 19:33:48.000000 Concern-8/
-drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-10-06 19:33:48.000000 Concern-8/concernlib/
--rw-r--r--   0 arc       (1000) arc       (1000)     1361 2019-10-06 00:03:33.000000 Concern-8/concernlib/pym2149.py
--rw-r--r--   0 arc       (1000) arc       (1000)      657 2019-10-06 00:03:33.000000 Concern-8/concernlib/vimrc.aridt
--rw-r--r--   0 arc       (1000) arc       (1000)     1810 2019-10-06 00:03:33.000000 Concern-8/concernlib/Concern.arid
--rw-r--r--   0 arc       (1000) arc       (1000)     3239 2019-10-06 00:03:33.000000 Concern-8/concernlib/test_getblock.py
--rw-r--r--   0 arc       (1000) arc       (1000)     1732 2019-10-06 00:03:33.000000 Concern-8/concernlib/sendblock.py.aridt
--rw-r--r--   0 arc       (1000) arc       (1000)      788 2019-10-06 00:03:33.000000 Concern-8/concernlib/initlogging.py
--rw-r--r--   0 arc       (1000) arc       (1000)     2436 2019-10-06 00:03:33.000000 Concern-8/concernlib/getblock.py
--rw-r--r--   0 arc       (1000) arc       (1000)      689 2019-10-06 00:03:33.000000 Concern-8/concernlib/__init__.py
--rw-r--r--   0 arc       (1000) arc       (1000)      722 2019-10-06 00:03:33.000000 Concern-8/concernlib/foxdot.py
--rw-r--r--   0 arc       (1000) arc       (1000)      249 2019-10-06 00:03:33.000000 Concern-8/concernlib/screenrc.aridt
--rwxr-xr-x   0 arc       (1000) arc       (1000)     3903 2019-10-06 00:03:33.000000 Concern-8/Concern
--rw-r--r--   0 arc       (1000) arc       (1000)       67 2019-10-06 19:33:48.000000 Concern-8/setup.cfg
--rw-r--r--   0 arc       (1000) arc       (1000)      404 2019-10-06 19:33:47.000000 Concern-8/setup.py
--rw-r--r--   0 arc       (1000) arc       (1000)     1732 2019-10-06 10:13:55.000000 Concern-8/README.md
--rw-r--r--   0 arc       (1000) arc       (1000)      205 2019-10-06 19:33:48.000000 Concern-8/PKG-INFO
-drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-10-06 19:33:48.000000 Concern-8/Concern.egg-info/
--rw-r--r--   0 arc       (1000) arc       (1000)        1 2019-10-06 19:33:47.000000 Concern-8/Concern.egg-info/dependency_links.txt
--rw-r--r--   0 arc       (1000) arc       (1000)       31 2019-10-06 19:33:47.000000 Concern-8/Concern.egg-info/requires.txt
--rw-r--r--   0 arc       (1000) arc       (1000)       11 2019-10-06 19:33:47.000000 Concern-8/Concern.egg-info/top_level.txt
--rw-r--r--   0 arc       (1000) arc       (1000)      205 2019-10-06 19:33:47.000000 Concern-8/Concern.egg-info/PKG-INFO
--rw-r--r--   0 arc       (1000) arc       (1000)      436 2019-10-06 19:33:48.000000 Concern-8/Concern.egg-info/SOURCES.txt
+drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-10-07 20:55:34.000000 Concern-9/
+drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-10-07 20:55:34.000000 Concern-9/concernlib/
+-rw-r--r--   0 arc       (1000) arc       (1000)     1361 2019-10-06 00:03:33.000000 Concern-9/concernlib/pym2149.py
+-rw-r--r--   0 arc       (1000) arc       (1000)      689 2019-10-06 22:37:30.000000 Concern-9/concernlib/vimrc.aridt
+-rw-r--r--   0 arc       (1000) arc       (1000)     1810 2019-10-06 00:03:33.000000 Concern-9/concernlib/Concern.arid
+-rw-r--r--   0 arc       (1000) arc       (1000)     3239 2019-10-06 00:03:33.000000 Concern-9/concernlib/test_getblock.py
+-rw-r--r--   0 arc       (1000) arc       (1000)     1732 2019-10-06 22:50:31.000000 Concern-9/concernlib/sendblock.py.aridt
+-rw-r--r--   0 arc       (1000) arc       (1000)      788 2019-10-06 00:03:33.000000 Concern-9/concernlib/initlogging.py
+-rw-r--r--   0 arc       (1000) arc       (1000)     2436 2019-10-06 00:03:33.000000 Concern-9/concernlib/getblock.py
+-rw-r--r--   0 arc       (1000) arc       (1000)      689 2019-10-06 00:03:33.000000 Concern-9/concernlib/__init__.py
+-rw-r--r--   0 arc       (1000) arc       (1000)      722 2019-10-06 00:03:33.000000 Concern-9/concernlib/foxdot.py
+-rw-r--r--   0 arc       (1000) arc       (1000)      249 2019-10-06 00:03:33.000000 Concern-9/concernlib/screenrc.aridt
+-rwxr-xr-x   0 arc       (1000) arc       (1000)     3903 2019-10-06 00:03:33.000000 Concern-9/Concern
+-rw-r--r--   0 arc       (1000) arc       (1000)       67 2019-10-07 20:55:34.000000 Concern-9/setup.cfg
+-rw-r--r--   0 arc       (1000) arc       (1000)      683 2019-10-07 20:55:33.000000 Concern-9/setup.py
+-rw-r--r--   0 arc       (1000) arc       (1000)     1732 2019-10-06 10:13:55.000000 Concern-9/README.md
+-rw-r--r--   0 arc       (1000) arc       (1000)     2380 2019-10-07 20:55:34.000000 Concern-9/PKG-INFO
+drwxr-xr-x   0 arc       (1000) arc       (1000)        0 2019-10-07 20:55:34.000000 Concern-9/Concern.egg-info/
+-rw-r--r--   0 arc       (1000) arc       (1000)        1 2019-10-07 20:55:33.000000 Concern-9/Concern.egg-info/dependency_links.txt
+-rw-r--r--   0 arc       (1000) arc       (1000)       31 2019-10-07 20:55:33.000000 Concern-9/Concern.egg-info/requires.txt
+-rw-r--r--   0 arc       (1000) arc       (1000)       11 2019-10-07 20:55:33.000000 Concern-9/Concern.egg-info/top_level.txt
+-rw-r--r--   0 arc       (1000) arc       (1000)     2380 2019-10-07 20:55:33.000000 Concern-9/Concern.egg-info/PKG-INFO
+-rw-r--r--   0 arc       (1000) arc       (1000)      436 2019-10-07 20:55:33.000000 Concern-9/Concern.egg-info/SOURCES.txt
```

### Comparing `Concern-8/concernlib/pym2149.py` & `Concern-9/concernlib/pym2149.py`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/Concern.arid` & `Concern-9/concernlib/Concern.arid`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/test_getblock.py` & `Concern-9/concernlib/test_getblock.py`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/sendblock.py.aridt` & `Concern-9/concernlib/sendblock.py.aridt`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/initlogging.py` & `Concern-9/concernlib/initlogging.py`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/getblock.py` & `Concern-9/concernlib/getblock.py`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/__init__.py` & `Concern-9/concernlib/__init__.py`

 * *Files identical despite different names*

### Comparing `Concern-8/concernlib/foxdot.py` & `Concern-9/concernlib/foxdot.py`

 * *Files identical despite different names*

### Comparing `Concern-8/Concern` & `Concern-9/Concern`

 * *Files identical despite different names*

### Comparing `Concern-8/README.md` & `Concern-9/README.md`

 * *Files identical despite different names*

