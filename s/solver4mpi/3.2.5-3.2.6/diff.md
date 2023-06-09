# Comparing `tmp/solver4mpi-3.2.5.tar.gz` & `tmp/solver4mpi-3.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solver4mpi-3.2.5.tar", last modified: Thu Jun  8 23:44:13 2023, max compression
+gzip compressed data, was "solver4mpi-3.2.6.tar", last modified: Fri Jun  9 00:20:58 2023, max compression
```

## Comparing `solver4mpi-3.2.5.tar` & `solver4mpi-3.2.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 23:44:13.369991 solver4mpi-3.2.5/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 23:44:13.369799 solver4mpi-3.2.5/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2.5/README.md
--rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-08 23:44:13.370053 solver4mpi-3.2.5/setup.cfg
--rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-08 23:43:29.000000 solver4mpi-3.2.5/setup.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 23:44:13.365493 solver4mpi-3.2.5/solver4mpi/
--rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2.5/solver4mpi/__init__.py
--rw-r--r--   0 mregnier   (501) staff       (20)     6310 2023-06-08 23:40:26.000000 solver4mpi-3.2.5/solver4mpi/minimizer_multiprocess.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.2.5/solver4mpi/test.py
--rw-r--r--   0 mregnier   (501) staff       (20)     2602 2023-06-08 23:42:50.000000 solver4mpi-3.2.5/solver4mpi/test_mpi.py
-drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-08 23:44:13.369550 solver4mpi-3.2.5/solver4mpi.egg-info/
--rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-08 23:44:13.000000 solver4mpi-3.2.5/solver4mpi.egg-info/PKG-INFO
--rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-08 23:44:13.000000 solver4mpi-3.2.5/solver4mpi.egg-info/SOURCES.txt
--rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-08 23:44:13.000000 solver4mpi-3.2.5/solver4mpi.egg-info/dependency_links.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-08 23:44:13.000000 solver4mpi-3.2.5/solver4mpi.egg-info/requires.txt
--rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-08 23:44:13.000000 solver4mpi-3.2.5/solver4mpi.egg-info/top_level.txt
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:20:58.399767 solver4mpi-3.2.6/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 00:20:58.399626 solver4mpi-3.2.6/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)       21 2023-06-08 10:41:05.000000 solver4mpi-3.2.6/README.md
+-rw-r--r--   0 mregnier   (501) staff       (20)       38 2023-06-09 00:20:58.399817 solver4mpi-3.2.6/setup.cfg
+-rw-r--r--   0 mregnier   (501) staff       (20)      740 2023-06-09 00:20:21.000000 solver4mpi-3.2.6/setup.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:20:58.395720 solver4mpi-3.2.6/solver4mpi/
+-rw-r--r--   0 mregnier   (501) staff       (20)       47 2023-06-08 10:41:05.000000 solver4mpi-3.2.6/solver4mpi/__init__.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     6360 2023-06-09 00:20:04.000000 solver4mpi-3.2.6/solver4mpi/minimizer_multiprocess.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2199 2023-06-08 15:58:25.000000 solver4mpi-3.2.6/solver4mpi/test.py
+-rw-r--r--   0 mregnier   (501) staff       (20)     2603 2023-06-09 00:19:45.000000 solver4mpi-3.2.6/solver4mpi/test_mpi.py
+drwxr-xr-x   0 mregnier   (501) staff       (20)        0 2023-06-09 00:20:58.399433 solver4mpi-3.2.6/solver4mpi.egg-info/
+-rw-r--r--   0 mregnier   (501) staff       (20)      231 2023-06-09 00:20:58.000000 solver4mpi-3.2.6/solver4mpi.egg-info/PKG-INFO
+-rw-r--r--   0 mregnier   (501) staff       (20)      289 2023-06-09 00:20:58.000000 solver4mpi-3.2.6/solver4mpi.egg-info/SOURCES.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)        1 2023-06-09 00:20:58.000000 solver4mpi-3.2.6/solver4mpi.egg-info/dependency_links.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       24 2023-06-09 00:20:58.000000 solver4mpi-3.2.6/solver4mpi.egg-info/requires.txt
+-rw-r--r--   0 mregnier   (501) staff       (20)       11 2023-06-09 00:20:58.000000 solver4mpi-3.2.6/solver4mpi.egg-info/top_level.txt
```

### Comparing `solver4mpi-3.2.5/setup.py` & `solver4mpi-3.2.6/setup.py`

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
-    version='3.2.5',
+    version='3.2.6',
     # The license can be anything you like
     license='',
     description='Optimized minimizer for MPI in python.',
     # We will also need a readme eventually (there will be a warning)
     # long_description=open('README.txt').read(),
 )
```

### Comparing `solver4mpi-3.2.5/solver4mpi/minimizer_multiprocess.py` & `solver4mpi-3.2.6/solver4mpi/minimizer_multiprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,20 +74,21 @@
         index_per_process_per_cpu = np.array_split(index_per_process, chunk_size)
 
         return index_per_process_per_cpu
 
 
     def run(self, x):
         res = np.zeros(x.shape[0])
-        index_per_process_per_cpu = self._split_params_with_cpu(x, self.ncpu)
+        index_per_process_per_cpu_i = self._split_params_with_cpu(x, self.ncpu)
+        index_per_process_per_cpu = x[self._split_params_with_cpu(x, self.ncpu)]
         _loop = len(index_per_process_per_cpu)
 
         for i in range(_loop):
-            print(self.rank, len(index_per_process_per_cpu[i]), index_per_process_per_cpu[i])
-            res[index_per_process_per_cpu[i]] = self.perform(np.array(index_per_process_per_cpu[i]))
+            print(self.rank, index_per_process_per_cpu[i])
+            res[index_per_process_per_cpu_i[i]] = self.perform(np.array(index_per_process_per_cpu[i]))
 
         return self.comm.allreduce(res, op=MPI.SUM)
 
 
     def perform(self, x):
         with ThreadPoolExecutor(max_workers=self.ncpu) as executor:
             futures = [executor.submit(self._apply_minimize, i) for i in x]
```

### Comparing `solver4mpi-3.2.5/solver4mpi/test.py` & `solver4mpi-3.2.6/solver4mpi/test.py`

 * *Files identical despite different names*

### Comparing `solver4mpi-3.2.5/solver4mpi/test_mpi.py` & `solver4mpi-3.2.6/solver4mpi/test_mpi.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,26 +49,26 @@
 def chi2(x, ipix, mref, m_nu, allnus):
 
     #map_beta[ipix] = x
     m_nu_fake = _scale_components_1pix(x, ipix, mref, allnus)
     
     return np.sum((m_nu_fake - m_nu[:, ipix, :])**2)
 
-index_beta = np.arange(0, 100, 1)
+index_beta = np.arange(50, 60, 1)
 
 chi2_partial = partial(chi2, mref=mref, m_nu=m_nu, allnus=allnus)
 cpu = 5
 wrap = DistributeMPI(comm, cpu, chi2_partial, x0=np.ones(1))
 index_per_process_per_cpu = wrap._split_params_with_cpu(index_beta, cpu)
 #print(index_per_process_per_cpu)
 start = time.time()
 a = wrap.run(index_beta)
 end = time.time()
 if rank == 0:
-    print(np.mean(a - beta[:100]))
+    print(np.mean(a - beta[50:60]))
     print(f'Execution time : {end - start} s')
 
 
 
 
 '''
 if rank == 0:
```

