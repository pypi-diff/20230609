# Comparing `tmp/phoenixtools-0.0.4.tar.gz` & `tmp/phoenixtools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phoenixtools-0.0.4.tar", last modified: Tue Jun  6 23:54:25 2023, max compression
+gzip compressed data, was "phoenixtools-0.0.5.tar", last modified: Fri Jun  9 13:33:54 2023, max compression
```

## Comparing `phoenixtools-0.0.4.tar` & `phoenixtools-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:54:25.693080 phoenixtools-0.0.4/
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-06 23:54:25.693080 phoenixtools-0.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:54:25.693080 phoenixtools-0.0.4/phoenixtools/
--rw-r--r--   0 runner    (1000) runner    (1000)       28 2023-06-06 23:37:43.000000 phoenixtools-0.0.4/phoenixtools/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)      200 2023-06-06 23:52:31.000000 phoenixtools-0.0.4/phoenixtools/iptools.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-06 23:54:25.693080 phoenixtools-0.0.4/phoenixtools.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-06 23:54:25.000000 phoenixtools-0.0.4/phoenixtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-06-06 23:54:25.000000 phoenixtools-0.0.4/phoenixtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-06 23:54:25.000000 phoenixtools-0.0.4/phoenixtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-06-06 23:54:25.000000 phoenixtools-0.0.4/phoenixtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-06 23:54:25.693080 phoenixtools-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1000) runner    (1000)      964 2023-06-06 23:53:59.000000 phoenixtools-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-09 13:33:54.038460 phoenixtools-0.0.5/
+-rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-09 13:33:54.038460 phoenixtools-0.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-09 13:33:54.030460 phoenixtools-0.0.5/phoenixtools/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1094 2023-06-09 13:28:24.000000 phoenixtools-0.0.5/phoenixtools/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)      200 2023-06-06 23:52:31.000000 phoenixtools-0.0.5/phoenixtools/iptools.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2023-06-09 13:33:54.038460 phoenixtools-0.0.5/phoenixtools.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)      453 2023-06-09 13:33:53.000000 phoenixtools-0.0.5/phoenixtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      201 2023-06-09 13:33:53.000000 phoenixtools-0.0.5/phoenixtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2023-06-09 13:33:53.000000 phoenixtools-0.0.5/phoenixtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       13 2023-06-09 13:33:53.000000 phoenixtools-0.0.5/phoenixtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2023-06-09 13:33:54.038460 phoenixtools-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1000) runner    (1000)      964 2023-06-09 13:33:28.000000 phoenixtools-0.0.5/setup.py
```

### Comparing `phoenixtools-0.0.4/setup.py` & `phoenixtools-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4' 
+VERSION = '0.0.5' 
 DESCRIPTION = 'Easy hacking tools'
 LONG_DESCRIPTION = 'Easy hacking tools used for educational purposes'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="phoenixtools",
```

