# Comparing `tmp/solver4mpi-3.4.2.tar.gz` & `tmp/solver4mpi-3.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.4.2.tar", last modified: Fri Jun  9 08:22:07 2023, max compression
+gzip compressed data, was "solver4mpi-3.4.3.tar", last modified: Fri Jun  9 08:53:43 2023, max compression
```

## Comparing `solver4mpi-3.4.2.tar` & `solver4mpi-3.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:22:07.521099 solver4mpi-3.4.2/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:22:07.520965 solver4mpi-3.4.2/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.2/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 08:22:07.521143 solver4mpi-3.4.2/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-09 08:21:29.000000 solver4mpi-3.4.2/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:22:07.518435 solver4mpi-3.4.2/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.2/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6370 2023-06-09 08:20:40.000000 solver4mpi-3.4.2/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.2/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2651 2023-06-09 08:17:59.000000 solver4mpi-3.4.2/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:22:07.520799 solver4mpi-3.4.2/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:22:07.000000 solver4mpi-3.4.2/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 08:22:07.000000 solver4mpi-3.4.2/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 08:22:07.000000 solver4mpi-3.4.2/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 08:22:07.000000 solver4mpi-3.4.2/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 08:22:07.000000 solver4mpi-3.4.2/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:53:43.838206 solver4mpi-3.4.3/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:53:43.838055 solver4mpi-3.4.3/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.3/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 08:53:43.838257 solver4mpi-3.4.3/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      756 2023-06-09 08:53:10.000000 solver4mpi-3.4.3/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:53:43.834690 solver4mpi-3.4.3/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.3/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6498 2023-06-09 08:51:06.000000 solver4mpi-3.4.3/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.3/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2756 2023-06-09 08:47:41.000000 solver4mpi-3.4.3/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 08:53:43.837862 solver4mpi-3.4.3/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       37 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 08:53:43.000000 solver4mpi-3.4.3/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.4.2/setup.py` & `solver4mpi-3.4.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     name='solver4mpi',
     url='https://github.com/mathias77515/optimized_minimizer',
     author='Mathias Regnier',
     author_email='mathias.p.regnier@gmail.com',
     # Needed to actually package something
     packages=find_packages(),
     # Needed for dependencies
-    install_requires=['scipy', 'pyoperators', 'numpy'],
+    install_requires=['scipy', 'pyoperators', 'numpy', 'multiprocess'],
     # *strongly* suggested for sharing
-    version='3.4.2',
+    version='3.4.3',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.4.2/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.4.3/solver4mpi/minimizer_multiprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
         ### Minimizer
         self.chi2 = chi2
         self.x0 = x0
         self.method = method
         self.tol = tol
         self.options = options
+        self.verbose = verbose
 
     def _split_params(self, index):
 
         '''
         
         Distribute the parameters across all available processes
 
@@ -45,18 +46,19 @@
         return r.x
 
 
     def __call__(self, index):
 
         res = np.zeros(index.shape)
         x_per_process = self._split_params(index)
-        #print(self.rank, x_per_process)
+        if self.verbose:
+            print(self.rank, x_per_process)
 
         for ii, i in enumerate(x_per_process):
-            res[i] = self._apply_minimize(args=(i))
+            res[i] = self._apply_minimize(args=(index[i]))
         
         return self.comm.allreduce(res, op=MPI.SUM)
 
 class DistributeMPI(WrapperMPI):
 
     def __init__(self, comm, ncpu, chi2, x0, method='L-BFGS-B', tol=1e-10, options={}, verbose=False):
 
@@ -80,18 +82,20 @@
         res = np.zeros(x.shape[0])
         
         index_per_process_per_cpu = self._split_params_with_cpu(x, self.ncpu)
         #stop
         _loop = len(index_per_process_per_cpu)
 
         for i in range(_loop):
-            print(self.rank, index_per_process_per_cpu[i], x[index_per_process_per_cpu[i]])
+            if self.verbose:
+                print(self.rank, index_per_process_per_cpu[i], x[index_per_process_per_cpu[i]])
             res[index_per_process_per_cpu[i]] = self.perform(x[index_per_process_per_cpu[i]])
         self.comm.Barrier()
-        print(res)
+        if self.verbose:
+            print(res)
         return self.comm.allreduce(res, op=MPI.SUM)
 
 
     def perform(self, x):
         with ThreadPoolExecutor(max_workers=self.ncpu) as executor:
             futures = [executor.submit(self._apply_minimize, i) for i in x]
             results = [future.result() for future in futures]
```

### Comparing `solver4mpi-3.4.2/solver4mpi/test.py` & `solver4mpi-3.4.3/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.4.2/solver4mpi/test_mpi.py` & `solver4mpi-3.4.3/solver4mpi/test_mpi.py`

 * *Files 7% similar despite different names*

```diff
@@ -53,18 +53,19 @@
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
 index_beta = np.array([4,12,13,20,21,27,28,29,35,36,43])#np.arange(50, 60, 1)
 
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
 cpu = 2
-wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1), method='L-BFGS-B', tol=1e-10)
+wrap = WrapperMPI(comm, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10, options={}, verbose=False)
+#wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1)*1.5, method='TNC', tol=1e-10)
 #print(index_per_process_per_cpu)
 start = time.time()
-a = wrap.run(index_beta)
+a = wrap(index_beta)
 
 end = time.time()
 if rank == 0:
     print(a)
     print(beta[index_beta])
     print(np.mean(a - beta[index_beta]))
     print(f'Execution time : {end - start} s')
```

