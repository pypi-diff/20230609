# Comparing `tmp/daisytuner-likwid-0.0.1.tar.gz` & `tmp/daisytuner-likwid-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisytuner-likwid-0.0.1.tar", last modified: Fri Jun  9 06:14:01 2023, max compression
+gzip compressed data, was "daisytuner-likwid-0.0.2.tar", last modified: Fri Jun  9 06:31:08 2023, max compression
```

## Comparing `daisytuner-likwid-0.0.1.tar` & `daisytuner-likwid-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-09 06:14:01.854349 daisytuner-likwid-0.0.1/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    18047 2023-06-09 05:40:01.000000 daisytuner-likwid-0.0.1/LICENSE
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      349 2023-06-09 06:14:01.854349 daisytuner-likwid-0.0.1/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      118 2023-06-09 05:47:12.000000 daisytuner-likwid-0.0.1/README.md
--rw-rw-r--   0 lukas     (1000) lukas     (1000)    12212 2023-06-09 06:13:07.000000 daisytuner-likwid-0.0.1/daisy_likwid_helpers.c
-drwxrwxr-x   0 lukas     (1000) lukas     (1000)        0 2023-06-09 06:14:01.854349 daisytuner-likwid-0.0.1/daisytuner_likwid.egg-info/
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      349 2023-06-09 06:14:01.000000 daisytuner-likwid-0.0.1/daisytuner_likwid.egg-info/PKG-INFO
--rw-rw-r--   0 lukas     (1000) lukas     (1000)      213 2023-06-09 06:14:01.000000 daisytuner-likwid-0.0.1/daisytuner_likwid.egg-info/SOURCES.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)        1 2023-06-09 06:14:01.000000 daisytuner-likwid-0.0.1/daisytuner_likwid.egg-info/dependency_links.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       21 2023-06-09 06:14:01.000000 daisytuner-likwid-0.0.1/daisytuner_likwid.egg-info/top_level.txt
--rw-rw-r--   0 lukas     (1000) lukas     (1000)       38 2023-06-09 06:14:01.854349 daisytuner-likwid-0.0.1/setup.cfg
--rw-rw-r--   0 lukas     (1000) lukas     (1000)     4059 2023-06-09 06:13:21.000000 daisytuner-likwid-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:31:08.542022 daisytuner-likwid-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18047 2023-06-09 06:28:41.000000 daisytuner-likwid-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-09 06:31:08.542022 daisytuner-likwid-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-09 06:28:41.000000 daisytuner-likwid-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12212 2023-06-09 06:28:41.000000 daisytuner-likwid-0.0.2/daisy_likwid_helpers.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 06:31:08.542022 daisytuner-likwid-0.0.2/daisytuner_likwid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-06-09 06:31:08.000000 daisytuner-likwid-0.0.2/daisytuner_likwid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-09 06:31:08.000000 daisytuner-likwid-0.0.2/daisytuner_likwid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 06:31:08.000000 daisytuner-likwid-0.0.2/daisytuner_likwid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-09 06:31:08.000000 daisytuner-likwid-0.0.2/daisytuner_likwid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 06:31:08.542022 daisytuner-likwid-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-06-09 06:28:41.000000 daisytuner-likwid-0.0.2/setup.py
```

### Comparing `daisytuner-likwid-0.0.1/LICENSE` & `daisytuner-likwid-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `daisytuner-likwid-0.0.1/daisy_likwid_helpers.c` & `daisytuner-likwid-0.0.2/daisy_likwid_helpers.c`

 * *Files identical despite different names*

### Comparing `daisytuner-likwid-0.0.1/setup.py` & `daisytuner-likwid-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     libraries=[LIKWID_LIB],
     library_dirs=[LIKWID_LIBPATH],
     sources=["daisy_likwid_helpers.c"],
 )
 
 setup(
     name="daisytuner-likwid",
-    version="0.0.1",
+    version="0.0.2",
     author="Lukas Truemper",
     author_email="lukas.truemper@outlook.de",
     description="Likwid functions used by the daisytuner",
     long_description="Likwid functions used by the daisytuner",
     url="https://github.com/daisytuner/daisytuner-likwid",
     classifiers=[
         "Topic :: Utilities",
```

