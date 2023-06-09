# Comparing `tmp/solver4mpi-3.3.tar.gz` & `tmp/solver4mpi-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.3.tar", last modified: Fri Jun  9 00:56:41 2023, max compression
+gzip compressed data, was "solver4mpi-3.4.tar", last modified: Fri Jun  9 01:04:48 2023, max compression
```

## Comparing `solver4mpi-3.3.tar` & `solver4mpi-3.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:56:41.878036 solver4mpi-3.3/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 00:56:41.877736 solver4mpi-3.3/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.3/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 00:56:41.878141 solver4mpi-3.3/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-09 00:55:24.000000 solver4mpi-3.3/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:56:41.872405 solver4mpi-3.3/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.3/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6313 2023-06-09 00:54:10.000000 solver4mpi-3.3/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.3/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2603 2023-06-09 00:32:04.000000 solver4mpi-3.3/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:56:41.877317 solver4mpi-3.3/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:04:48.036228 solver4mpi-3.4/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 01:04:48.035867 solver4mpi-3.4/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 01:04:48.036348 solver4mpi-3.4/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-09 01:04:31.000000 solver4mpi-3.4/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:04:48.030440 solver4mpi-3.4/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6313 2023-06-09 01:03:35.000000 solver4mpi-3.4/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2603 2023-06-09 00:32:04.000000 solver4mpi-3.4/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:04:48.035406 solver4mpi-3.4/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.3/setup.py` & `solver4mpi-3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['scipy', 'pyoperators', 'numpy'],
     # *strongly* suggested for sharing
-    version='3.3',
+    version='3.4',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.3/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.4/solver4mpi/minimizer_multiprocess.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.3/solver4mpi/test.py` & `solver4mpi-3.4/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.3/solver4mpi/test_mpi.py` & `solver4mpi-3.4/solver4mpi/test_mpi.py`

 * *Files identical despite different names*

