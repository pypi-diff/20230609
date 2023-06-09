# Comparing `tmp/callmebot-1.1.2.tar.gz` & `tmp/callmebot-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callmebot-1.1.2.tar", last modified: Fri Jun  9 07:21:30 2023, max compression
+gzip compressed data, was "callmebot-1.1.3.tar", last modified: Fri Jun  9 07:24:16 2023, max compression
```

## Comparing `callmebot-1.1.2.tar` & `callmebot-1.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:21:30.368908 callmebot-1.1.2/
--rw-r--r--   0 jpetit     (501) staff       (20)    11368 2023-02-26 09:44:51.000000 callmebot-1.1.2/LICENSE
--rw-r--r--   0 jpetit     (501) staff       (20)      122 2023-02-26 09:44:51.000000 callmebot-1.1.2/Makefile
--rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 07:21:30.368575 callmebot-1.1.2/PKG-INFO
--rw-r--r--   0 jpetit     (501) staff       (20)     1004 2023-02-26 10:42:04.000000 callmebot-1.1.2/README.md
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:21:30.362196 callmebot-1.1.2/callmebot/
--rw-r--r--   0 jpetit     (501) staff       (20)     1315 2023-02-26 09:57:08.000000 callmebot-1.1.2/callmebot/__init__.py
--rw-r--r--   0 jpetit     (501) staff       (20)     1312 2023-02-26 10:36:48.000000 callmebot-1.1.2/callmebot/cmd.py
--rw-r--r--   0 jpetit     (501) staff       (20)        0 2023-06-09 07:20:55.000000 callmebot-1.1.2/callmebot/py.typed
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:21:30.368104 callmebot-1.1.2/callmebot.egg-info/
--rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 07:21:30.000000 callmebot-1.1.2/callmebot.egg-info/PKG-INFO
--rw-r--r--   0 jpetit     (501) staff       (20)      335 2023-06-09 07:21:30.000000 callmebot-1.1.2/callmebot.egg-info/SOURCES.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-06-09 07:21:30.000000 callmebot-1.1.2/callmebot.egg-info/dependency_links.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       49 2023-06-09 07:21:30.000000 callmebot-1.1.2/callmebot.egg-info/entry_points.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-02-26 10:37:24.000000 callmebot-1.1.2/callmebot.egg-info/not-zip-safe
--rw-r--r--   0 jpetit     (501) staff       (20)       30 2023-06-09 07:21:30.000000 callmebot-1.1.2/callmebot.egg-info/requires.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-06-09 07:21:30.000000 callmebot-1.1.2/callmebot.egg-info/top_level.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-06-09 07:21:30.369028 callmebot-1.1.2/setup.cfg
--rwxr-xr-x   0 jpetit     (501) staff       (20)      828 2023-06-09 07:21:27.000000 callmebot-1.1.2/setup.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)      415 2023-02-26 10:21:24.000000 callmebot-1.1.2/upload.sh
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:24:16.550159 callmebot-1.1.3/
+-rw-r--r--   0 jpetit     (501) staff       (20)    11368 2023-02-26 09:44:51.000000 callmebot-1.1.3/LICENSE
+-rw-r--r--   0 jpetit     (501) staff       (20)      122 2023-02-26 09:44:51.000000 callmebot-1.1.3/Makefile
+-rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 07:24:16.549612 callmebot-1.1.3/PKG-INFO
+-rw-r--r--   0 jpetit     (501) staff       (20)     1004 2023-02-26 10:42:04.000000 callmebot-1.1.3/README.md
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:24:16.540835 callmebot-1.1.3/callmebot/
+-rw-r--r--   0 jpetit     (501) staff       (20)     1315 2023-02-26 09:57:08.000000 callmebot-1.1.3/callmebot/__init__.py
+-rw-r--r--   0 jpetit     (501) staff       (20)     1312 2023-02-26 10:36:48.000000 callmebot-1.1.3/callmebot/cmd.py
+-rw-r--r--   0 jpetit     (501) staff       (20)        0 2023-06-09 07:20:55.000000 callmebot-1.1.3/callmebot/py.typed
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:24:16.548840 callmebot-1.1.3/callmebot.egg-info/
+-rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 07:24:16.000000 callmebot-1.1.3/callmebot.egg-info/PKG-INFO
+-rw-r--r--   0 jpetit     (501) staff       (20)      335 2023-06-09 07:24:16.000000 callmebot-1.1.3/callmebot.egg-info/SOURCES.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-06-09 07:24:16.000000 callmebot-1.1.3/callmebot.egg-info/dependency_links.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       49 2023-06-09 07:24:16.000000 callmebot-1.1.3/callmebot.egg-info/entry_points.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-02-26 10:37:24.000000 callmebot-1.1.3/callmebot.egg-info/not-zip-safe
+-rw-r--r--   0 jpetit     (501) staff       (20)       30 2023-06-09 07:24:16.000000 callmebot-1.1.3/callmebot.egg-info/requires.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-06-09 07:24:16.000000 callmebot-1.1.3/callmebot.egg-info/top_level.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-06-09 07:24:16.550294 callmebot-1.1.3/setup.cfg
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      828 2023-06-09 07:24:13.000000 callmebot-1.1.3/setup.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      415 2023-02-26 10:21:24.000000 callmebot-1.1.3/upload.sh
```

### Comparing `callmebot-1.1.2/LICENSE` & `callmebot-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `callmebot-1.1.2/README.md` & `callmebot-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `callmebot-1.1.2/callmebot/__init__.py` & `callmebot-1.1.3/callmebot/__init__.py`

 * *Files identical despite different names*

### Comparing `callmebot-1.1.2/callmebot/cmd.py` & `callmebot-1.1.3/callmebot/cmd.py`

 * *Files identical despite different names*

### Comparing `callmebot-1.1.2/setup.py` & `callmebot-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # coding=utf-8
 
 from setuptools import setup
 
-version = '1.1.2'
+version = '1.1.3'
 
 setup(
     name='callmebot',
     packages=['callmebot'],
     install_requires=[
         'requests',
         'typer',
```

