# Comparing `tmp/solver4mpi-3.4.4.tar.gz` & `tmp/solver4mpi-3.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.4.4.tar", last modified: Fri Jun  9 08:57:28 2023, max compression
+gzip compressed data, was "solver4mpi-3.4.5.tar", last modified: Fri Jun  9 09:03:39 2023, max compression
```

## Comparing `solver4mpi-3.4.4.tar` & `solver4mpi-3.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:57:28.087205 solver4mpi-3.4.4/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:57:28.087069 solver4mpi-3.4.4/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.4/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 08:57:28.087250 solver4mpi-3.4.4/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 08:56:42.000000 solver4mpi-3.4.4/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:57:28.084413 solver4mpi-3.4.4/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.4/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6607 2023-06-09 08:57:13.000000 solver4mpi-3.4.4/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.4/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2756 2023-06-09 08:47:41.000000 solver4mpi-3.4.4/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:57:28.086905 solver4mpi-3.4.4/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 08:57:28.000000 solver4mpi-3.4.4/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:03:39.114740 solver4mpi-3.4.5/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 09:03:39.114433 solver4mpi-3.4.5/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.5/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 09:03:39.114839 solver4mpi-3.4.5/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 09:03:17.000000 solver4mpi-3.4.5/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:03:39.109157 solver4mpi-3.4.5/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.5/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6704 2023-06-09 09:01:32.000000 solver4mpi-3.4.5/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.5/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2755 2023-06-09 08:59:45.000000 solver4mpi-3.4.5/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 09:03:39.114035 solver4mpi-3.4.5/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 09:03:39.000000 solver4mpi-3.4.5/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 09:03:38.000000 solver4mpi-3.4.5/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.4.4/setup.py` & `solver4mpi-3.4.5/setup.py`

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
-    version='3.4.4',
+    version='3.4.5',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.4.4/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.4.5/solver4mpi/minimizer_multiprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,23 +50,27 @@
 
         res = np.zeros(index.shape)
         x_per_process = self._split_params(index)
         if self.verbose:
             print(self.rank, x_per_process)
 
         for ii, i in enumerate(x_per_process):
-            if self.verbose:
-                print(f'Minimizing parameter {index[i]} with rank {self.rank}')
+            
+            start = time.time()
             res[i] = self._apply_minimize(args=(index[i]))
+            end = time.time()
+
+            if self.verbose:
+                print(f'Minimized parameter {index[i]} with rank {self.rank} in {end - start:.6f} s')
         
         return self.comm.allreduce(res, op=MPI.SUM)
 
 class DistributeMPI(WrapperMPI):
 
-    def __init__(self, comm, ncpu, chi2, x0, method='L-BFGS-B', tol=1e-10, options={}, verbose=False):
+    def __init__(self, comm, ncpu, chi2, x0, method='L-BFGS-B', tol=1e-10, options={}, verbose=True):
 
         self.ncpu = ncpu
         WrapperMPI.__init__(self, comm, chi2, x0, method=method, tol=tol, options=options, verbose=verbose)
 
     def _split_params_with_cpu(self, index, cpu):
 
         index_per_process = self._split_params(index)
```

### Comparing `solver4mpi-3.4.4/solver4mpi/test.py` & `solver4mpi-3.4.5/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.4.4/solver4mpi/test_mpi.py` & `solver4mpi-3.4.5/solver4mpi/test_mpi.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
 index_beta = np.array([4,12,13,20,21,27,28,29,35,36,43])#np.arange(50, 60, 1)
 
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
 cpu = 2
-wrap = WrapperMPI(comm, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10, options={}, verbose=False)
+wrap = WrapperMPI(comm, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10, options={}, verbose=True)
 #wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10)
 #print(index_per_process_per_cpu)
 start = time.time()
 a = wrap(index_beta)
 
 end = time.time()
 if rank == 0:
```

