# Comparing `tmp/solver4mpi-3.4.tar.gz` & `tmp/solver4mpi-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.4.tar", last modified: Fri Jun  9 01:04:48 2023, max compression
+gzip compressed data, was "solver4mpi-3.4.1.tar", last modified: Fri Jun  9 01:58:23 2023, max compression
```

## Comparing `solver4mpi-3.4.tar` & `solver4mpi-3.4.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:04:48.036228 solver4mpi-3.4/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 01:04:48.035867 solver4mpi-3.4/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 01:04:48.036348 solver4mpi-3.4/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      738 2023-06-09 01:04:31.000000 solver4mpi-3.4/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:04:48.030440 solver4mpi-3.4/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6313 2023-06-09 01:03:35.000000 solver4mpi-3.4/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2603 2023-06-09 00:32:04.000000 solver4mpi-3.4/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:04:48.035406 solver4mpi-3.4/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      229 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 01:04:47.000000 solver4mpi-3.4/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:58:23.216517 solver4mpi-3.4.1/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 01:58:23.216372 solver4mpi-3.4.1/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.4.1/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 01:58:23.216564 solver4mpi-3.4.1/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-09 01:57:44.000000 solver4mpi-3.4.1/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:58:23.213380 solver4mpi-3.4.1/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.4.1/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6294 2023-06-09 01:57:29.000000 solver4mpi-3.4.1/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.4.1/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2641 2023-06-09 01:52:46.000000 solver4mpi-3.4.1/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 01:58:23.216203 solver4mpi-3.4.1/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 01:58:23.000000 solver4mpi-3.4.1/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 01:58:23.000000 solver4mpi-3.4.1/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 01:58:23.000000 solver4mpi-3.4.1/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 01:58:23.000000 solver4mpi-3.4.1/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 01:58:23.000000 solver4mpi-3.4.1/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.4/setup.py` & `solver4mpi-3.4.1/setup.py`

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
-    version='3.4',
+    version='3.4.1',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.4/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.4.1/solver4mpi/minimizer_multiprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,17 @@
         index_per_process_per_cpu = np.array_split(index_per_process, chunk_size)
 
         return index_per_process_per_cpu
 
 
     def run(self, x):
         res = np.zeros(x.shape[0])
+        
         index_per_process_per_cpu = self._split_params_with_cpu(x, self.ncpu)
-        #print(index_per_process_per_cpu)
+        #stop
         _loop = len(index_per_process_per_cpu)
 
         for i in range(_loop):
             print(self.rank, x[index_per_process_per_cpu[i]])
             res[index_per_process_per_cpu[i]] = self.perform(x[index_per_process_per_cpu[i]])
 
         return self.comm.allreduce(res, op=MPI.SUM)
```

### Comparing `solver4mpi-3.4/solver4mpi/test.py` & `solver4mpi-3.4.1/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.4/solver4mpi/test_mpi.py` & `solver4mpi-3.4.1/solver4mpi/test_mpi.py`

 * *Files 15% similar despite different names*

```diff
@@ -49,26 +49,28 @@
 def chi2(x, ipix, mref, m_nu, allnus):
 
     #map_beta[ipix] = x
     m_nu_fake = _scale_components_1pix(x, ipix, mref, allnus)
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
-index_beta = np.arange(50, 60, 1)
+index_beta = np.array([4,12,13,20,21,27,28,29,35,36,43, 44, 67, 78, 80, 90])#np.arange(50, 60, 1)
 
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
 cpu = 2
 wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1))
-index_per_process_per_cpu = wrap._split_params_with_cpu(index_beta, cpu)
 #print(index_per_process_per_cpu)
 start = time.time()
 a = wrap.run(index_beta)
+
 end = time.time()
 if rank == 0:
-    print(np.mean(a - beta[50:60]))
+    print(a)
+    print(beta[index_beta])
+    print(np.mean(a - beta[index_beta]))
     print(f'Execution time : {end - start} s')
 
 
 
 
 '''
 if rank == 0:
```

