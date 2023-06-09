# Comparing `tmp/solver4mpi-3.4.5.tar.gz` & `tmp/solver4mpi-3.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.4.5.tar", last modified: Fri Jun  9 09:03:39 2023, max compression
+gzip compressed data, was "solver4mpi-3.4.6.tar", last modified: Fri Jun  9 09:12:50 2023, max compression
```

## Comparing `solver4mpi-3.4.5.tar` & `solver4mpi-3.4.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:03:39.114740 solver4mpi-3.4.5/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 09:03:39.114433 solver4mpi-3.4.5/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.5/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 09:03:39.114839 solver4mpi-3.4.5/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 09:03:17.000000 solver4mpi-3.4.5/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:03:39.109157 solver4mpi-3.4.5/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.5/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6704 2023-06-09 09:01:32.000000 solver4mpi-3.4.5/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.5/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2755 2023-06-09 08:59:45.000000 solver4mpi-3.4.5/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:03:39.114035 solver4mpi-3.4.5/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 09:03:39.000000 solver4mpi-3.4.5/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:12:50.156721 solver4mpi-3.4.6/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 09:12:50.156576 solver4mpi-3.4.6/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.6/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 09:12:50.156770 solver4mpi-3.4.6/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 09:12:29.000000 solver4mpi-3.4.6/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:12:50.153546 solver4mpi-3.4.6/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.6/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     7692 2023-06-09 09:12:14.000000 solver4mpi-3.4.6/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.6/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2760 2023-06-09 09:09:54.000000 solver4mpi-3.4.6/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:12:50.156392 solver4mpi-3.4.6/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 09:12:50.000000 solver4mpi-3.4.6/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 09:12:50.000000 solver4mpi-3.4.6/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 09:12:50.000000 solver4mpi-3.4.6/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 09:12:50.000000 solver4mpi-3.4.6/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 09:12:50.000000 solver4mpi-3.4.6/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.4.5/setup.py` & `solver4mpi-3.4.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
     install_requires=['scipy', 'pyoperators', 'numpy', 'multiprocess'],
     # *strongly* suggested for sharing
-    version='3.4.5',
+    version='3.4.6',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.4.5/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.4.6/solver4mpi/minimizer_multiprocess.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import numpy as np
 from pyoperators import *
 from scipy.optimize import minimize
 import os
 import multiprocess as mp
 import time
 from concurrent.futures import ThreadPoolExecutor
-
+from queue import Queue
+from threading import Lock
 
 class WrapperMPI:
 
     def __init__(self, comm, chi2, x0, method='TNC', tol=1e-10, options={}, verbose=False):
 
         ### MPI distribution
         self.comm = comm
@@ -96,20 +97,46 @@
                 print(self.rank, index_per_process_per_cpu[i], x[index_per_process_per_cpu[i]])
             res[index_per_process_per_cpu[i]] = self.perform(x[index_per_process_per_cpu[i]])
         self.comm.Barrier()
         if self.verbose:
             print(res)
         return self.comm.allreduce(res, op=MPI.SUM)
 
+    def perform(self, x):
+        results = Queue()  # File d'attente pour stocker les résultats
+        lock = Lock()  # Verrou pour synchroniser l'accès à la file d'attente
+
+        def minimize_wrapper(index, args):
+            result = self._apply_minimize(args)
+            with lock:
+                results.put((index, result))  # Ajouter l'index avec le résultat
+
+        with ThreadPoolExecutor(max_workers=self.ncpu) as executor:
+            futures = [executor.submit(minimize_wrapper, index, i) for index, i in enumerate(x)]
+
+        # Attendre la fin de toutes les tâches
+        for future in futures:
+            future.result()
+
+        # Réorganiser les résultats dans l'ordre approprié
+        final_results = [None] * len(x)
+        while not results.empty():
+            index, result = results.get()
+            final_results[index] = result
+
+        return np.concatenate(final_results)
 
+    '''
     def perform(self, x):
         with ThreadPoolExecutor(max_workers=self.ncpu) as executor:
             futures = [executor.submit(self._apply_minimize, i) for i in x]
             results = [future.result() for future in futures]
         return np.concatenate(results)
+    '''
+    
 
 class WrapperCPU:
 
     def __init__(self, chi2, x0, nproc=None, method='TNC', tol=1e-3, options={}, verbose=False):
 
         ### Do some prints
         self.verbose = verbose
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `solver4mpi-3.4.5/solver4mpi/test.py` & `solver4mpi-3.4.6/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.4.5/solver4mpi/test_mpi.py` & `solver4mpi-3.4.6/solver4mpi/test_mpi.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import matplotlib.pyplot as plt
 from minimizer_multiprocess import *
 import sys
 import time
 import pickle
 from functools import partial
 import os
+
 os.environ['OMP_NUM_THREADS'] = '10'
 
 sys.path.append('/Users/mregnier/Desktop/Libs/qubic/qubic/scripts/MapMaking')
 
 import component_model as c
 import mixing_matrix as mm
 
@@ -53,19 +54,19 @@
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
 index_beta = np.array([4,12,13,20,21,27,28,29,35,36,43])#np.arange(50, 60, 1)
 
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
 cpu = 2
-wrap = WrapperMPI(comm, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10, options={}, verbose=True)
-#wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10)
+#wrap = WrapperMPI(comm, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10, options={}, verbose=True)
+wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10)
 #print(index_per_process_per_cpu)
 start = time.time()
-a = wrap(index_beta)
+a = wrap.run(index_beta)
 
 end = time.time()
 if rank == 0:
     print(a)
     print(beta[index_beta])
     print(np.mean(a - beta[index_beta]))
     print(f'Execution time : {end - start} s')
```

