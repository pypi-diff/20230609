# Comparing `tmp/callmebot-1.2.4.tar.gz` & `tmp/callmebot-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callmebot-1.2.4.tar", last modified: Fri Jun  9 07:40:45 2023, max compression
+gzip compressed data, was "callmebot-1.2.5.tar", last modified: Fri Jun  9 08:28:40 2023, max compression
```

## Comparing `callmebot-1.2.4.tar` & `callmebot-1.2.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:40:45.545081 callmebot-1.2.4/
--rw-r--r--   0 jpetit     (501) staff       (20)    11368 2023-02-26 09:44:51.000000 callmebot-1.2.4/LICENSE
--rw-r--r--   0 jpetit     (501) staff       (20)      122 2023-02-26 09:44:51.000000 callmebot-1.2.4/Makefile
--rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 07:40:45.544586 callmebot-1.2.4/PKG-INFO
--rw-r--r--   0 jpetit     (501) staff       (20)     1004 2023-02-26 10:42:04.000000 callmebot-1.2.4/README.md
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:40:45.535957 callmebot-1.2.4/callmebot/
--rw-r--r--   0 jpetit     (501) staff       (20)     1315 2023-02-26 09:57:08.000000 callmebot-1.2.4/callmebot/__init__.py
--rw-r--r--   0 jpetit     (501) staff       (20)      115 2023-06-09 07:27:10.000000 callmebot-1.2.4/callmebot/__init__.pyi
--rw-r--r--   0 jpetit     (501) staff       (20)     1312 2023-02-26 10:36:48.000000 callmebot-1.2.4/callmebot/cmd.py
--rw-r--r--   0 jpetit     (501) staff       (20)        0 2023-06-09 07:20:55.000000 callmebot-1.2.4/callmebot/py.typed
-drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 07:40:45.543739 callmebot-1.2.4/callmebot.egg-info/
--rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/PKG-INFO
--rw-r--r--   0 jpetit     (501) staff       (20)      358 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/SOURCES.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/dependency_links.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       49 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/entry_points.txt
--rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/not-zip-safe
--rw-r--r--   0 jpetit     (501) staff       (20)       30 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/requires.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-06-09 07:40:45.000000 callmebot-1.2.4/callmebot.egg-info/top_level.txt
--rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-06-09 07:40:45.545224 callmebot-1.2.4/setup.cfg
--rwxr-xr-x   0 jpetit     (501) staff       (20)      890 2023-06-09 07:40:43.000000 callmebot-1.2.4/setup.py
--rwxr-xr-x   0 jpetit     (501) staff       (20)      508 2023-06-09 07:38:01.000000 callmebot-1.2.4/upload.sh
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 08:28:40.463001 callmebot-1.2.5/
+-rw-r--r--   0 jpetit     (501) staff       (20)    11368 2023-02-26 09:44:51.000000 callmebot-1.2.5/LICENSE
+-rw-r--r--   0 jpetit     (501) staff       (20)      122 2023-02-26 09:44:51.000000 callmebot-1.2.5/Makefile
+-rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 08:28:40.462419 callmebot-1.2.5/PKG-INFO
+-rw-r--r--   0 jpetit     (501) staff       (20)     1004 2023-02-26 10:42:04.000000 callmebot-1.2.5/README.md
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 08:28:40.454687 callmebot-1.2.5/callmebot/
+-rw-r--r--   0 jpetit     (501) staff       (20)     1315 2023-02-26 09:57:08.000000 callmebot-1.2.5/callmebot/__init__.py
+-rw-r--r--   0 jpetit     (501) staff       (20)      217 2023-06-09 08:27:56.000000 callmebot-1.2.5/callmebot/__init__.pyi
+-rw-r--r--   0 jpetit     (501) staff       (20)     1312 2023-02-26 10:36:48.000000 callmebot-1.2.5/callmebot/cmd.py
+-rw-r--r--   0 jpetit     (501) staff       (20)        0 2023-06-09 07:20:55.000000 callmebot-1.2.5/callmebot/py.typed
+drwxr-xr-x   0 jpetit     (501) staff       (20)        0 2023-06-09 08:28:40.461608 callmebot-1.2.5/callmebot.egg-info/
+-rw-r--r--   0 jpetit     (501) staff       (20)      338 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/PKG-INFO
+-rw-r--r--   0 jpetit     (501) staff       (20)      358 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/SOURCES.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/dependency_links.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       49 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/entry_points.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)        1 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/not-zip-safe
+-rw-r--r--   0 jpetit     (501) staff       (20)       30 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/requires.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       10 2023-06-09 08:28:40.000000 callmebot-1.2.5/callmebot.egg-info/top_level.txt
+-rw-r--r--   0 jpetit     (501) staff       (20)       38 2023-06-09 08:28:40.463272 callmebot-1.2.5/setup.cfg
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      890 2023-06-09 08:28:37.000000 callmebot-1.2.5/setup.py
+-rwxr-xr-x   0 jpetit     (501) staff       (20)      508 2023-06-09 07:38:01.000000 callmebot-1.2.5/upload.sh
```

### Comparing `callmebot-1.2.4/LICENSE` & `callmebot-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `callmebot-1.2.4/README.md` & `callmebot-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `callmebot-1.2.4/callmebot/__init__.py` & `callmebot-1.2.5/callmebot/__init__.py`

 * *Files identical despite different names*

### Comparing `callmebot-1.2.4/callmebot/cmd.py` & `callmebot-1.2.5/callmebot/cmd.py`

 * *Files identical despite different names*

### Comparing `callmebot-1.2.4/setup.py` & `callmebot-1.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # coding=utf-8
 
 from setuptools import setup
 
-version = '1.2.4'
+version = '1.2.5'
 
 setup(
     name='callmebot',
     packages=['callmebot'],
     package_data={"callmebot": ["__init__.pyi", "py.typed"]},
     install_requires=[
         'requests',
```

