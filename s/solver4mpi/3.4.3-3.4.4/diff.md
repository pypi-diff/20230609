# Comparing `tmp/solver4mpi-3.4.3.tar.gz` & `tmp/solver4mpi-3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.4.3.tar", last modified: Fri Jun  9 08:53:43 2023, max compression
+gzip compressed data, was "solver4mpi-3.4.4.tar", last modified: Fri Jun  9 08:57:28 2023, max compression
```

## Comparing `solver4mpi-3.4.3.tar` & `solver4mpi-3.4.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:53:43.838206 solver4mpi-3.4.3/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:53:43.838055 solver4mpi-3.4.3/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.3/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 08:53:43.838257 solver4mpi-3.4.3/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 08:53:10.000000 solver4mpi-3.4.3/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:53:43.834690 solver4mpi-3.4.3/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.3/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6498 2023-06-09 08:51:06.000000 solver4mpi-3.4.3/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.3/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2756 2023-06-09 08:47:41.000000 solver4mpi-3.4.3/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:53:43.837862 solver4mpi-3.4.3/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:57:28.087205 solver4mpi-3.4.4/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:57:28.087069 solver4mpi-3.4.4/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.4/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 08:57:28.087250 solver4mpi-3.4.4/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 08:56:42.000000 solver4mpi-3.4.4/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:57:28.084413 solver4mpi-3.4.4/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.4/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6607 2023-06-09 08:57:13.000000 solver4mpi-3.4.4/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.4/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2756 2023-06-09 08:47:41.000000 solver4mpi-3.4.4/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:57:28.086905 solver4mpi-3.4.4/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.4.3/setup.py` & `solver4mpi-3.4.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['scipy', 'pyoperators', 'numpy', 'multiprocess'],
     # *strongly* suggested for sharing
-    version='3.4.3',
+    version='3.4.4',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.4.3/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.4.4/solver4mpi/minimizer_multiprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 
         res = np.zeros(index.shape)
         x_per_process = self._split_params(index)
         if self.verbose:
             print(self.rank, x_per_process)
 
         for ii, i in enumerate(x_per_process):
+            if self.verbose:
+                print(f'Minimizing parameter {index[i]} with rank {self.rank}')
             res[i] = self._apply_minimize(args=(index[i]))
         
         return self.comm.allreduce(res, op=MPI.SUM)
 
 class DistributeMPI(WrapperMPI):
 
     def __init__(self, comm, ncpu, chi2, x0, method='L-BFGS-B', tol=1e-10, options={}, verbose=False):
```

### Comparing `solver4mpi-3.4.3/solver4mpi/test.py` & `solver4mpi-3.4.4/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.4.3/solver4mpi/test_mpi.py` & `solver4mpi-3.4.4/solver4mpi/test_mpi.py`

 * *Files identical despite different names*

