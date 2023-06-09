# Comparing `tmp/solver4mpi-3.2.8.tar.gz` & `tmp/solver4mpi-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.2.8.tar", last modified: Fri Jun  9 00:53:07 2023, max compression
+gzip compressed data, was "solver4mpi-3.3.tar", last modified: Fri Jun  9 00:56:41 2023, max compression
```

## Comparing `solver4mpi-3.2.8.tar` & `solver4mpi-3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:53:07.173197 solver4mpi-3.2.8/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 00:53:07.172841 solver4mpi-3.2.8/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2.8/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 00:53:07.173323 solver4mpi-3.2.8/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-09 00:52:24.000000 solver4mpi-3.2.8/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:53:07.166869 solver4mpi-3.2.8/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2.8/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6310 2023-06-09 00:51:00.000000 solver4mpi-3.2.8/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.2.8/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2603 2023-06-09 00:32:04.000000 solver4mpi-3.2.8/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:53:07.172336 solver4mpi-3.2.8/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 00:53:06.000000 solver4mpi-3.2.8/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 00:53:07.000000 solver4mpi-3.2.8/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 00:53:06.000000 solver4mpi-3.2.8/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 00:53:06.000000 solver4mpi-3.2.8/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 00:53:06.000000 solver4mpi-3.2.8/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:56:41.878036 solver4mpi-3.3/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 00:56:41.877736 solver4mpi-3.3/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.3/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 00:56:41.878141 solver4mpi-3.3/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-09 00:55:24.000000 solver4mpi-3.3/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:56:41.872405 solver4mpi-3.3/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.3/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6313 2023-06-09 00:54:10.000000 solver4mpi-3.3/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.3/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2603 2023-06-09 00:32:04.000000 solver4mpi-3.3/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:56:41.877317 solver4mpi-3.3/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 00:56:41.000000 solver4mpi-3.3/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.2.8/setup.py` & `solver4mpi-3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['scipy', 'pyoperators', 'numpy'],
     # *strongly* suggested for sharing
-    version='3.2.8',
+    version='3.3',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.2.8/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.3/solver4mpi/minimizer_multiprocess.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,15 @@
     def run(self, x):
         res = np.zeros(x.shape[0])
         index_per_process_per_cpu = self._split_params_with_cpu(x, self.ncpu)
         #print(index_per_process_per_cpu)
         _loop = len(index_per_process_per_cpu)
 
         for i in range(_loop):
-            print(self.rank, index_per_process_per_cpu[i])
+            print(self.rank, x[index_per_process_per_cpu[i]])
             res[index_per_process_per_cpu[i]] = self.perform(x[index_per_process_per_cpu[i]])
 
         return self.comm.allreduce(res, op=MPI.SUM)
 
 
     def perform(self, x):
         with ThreadPoolExecutor(max_workers=self.ncpu) as executor:
```

### Comparing `solver4mpi-3.2.8/solver4mpi/test.py` & `solver4mpi-3.3/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.2.8/solver4mpi/test_mpi.py` & `solver4mpi-3.3/solver4mpi/test_mpi.py`

 * *Files identical despite different names*

