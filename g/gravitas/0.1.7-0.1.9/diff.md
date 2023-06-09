# Comparing `tmp/gravitas-0.1.7.tar.gz` & `tmp/gravitas-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gravitas-0.1.7.tar", last modified: Thu Jun  1 16:33:24 2023, max compression
+gzip compressed data, was "gravitas-0.1.9.tar", last modified: Thu Jun  8 20:31:22 2023, max compression
```

## Comparing `gravitas-0.1.7.tar` & `gravitas-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:33:24.499450 gravitas-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 16:33:24.499450 gravitas-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-01 16:33:14.000000 gravitas-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:33:24.495449 gravitas-0.1.7/gravitas/
--rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/EGM96.c
--rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/GRGM360.c
--rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/MRO120F.c
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11267 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/gravlib.c
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 16:33:14.000000 gravitas-0.1.7/gravitas/libgrav.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:33:24.495449 gravitas-0.1.7/gravitas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 16:33:24.000000 gravitas-0.1.7/gravitas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-01 16:33:14.000000 gravitas-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:33:24.499450 gravitas-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-01 16:33:14.000000 gravitas-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:31:22.942773 gravitas-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 20:31:22.942773 gravitas-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-08 20:31:10.000000 gravitas-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:31:22.938773 gravitas-0.1.9/gravitas/
+-rw-r--r--   0 runner    (1001) docker     (123)  2750335 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/EGM96.c
+-rw-r--r--   0 runner    (1001) docker     (123)  2750581 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/GRGM360.c
+-rw-r--r--   0 runner    (1001) docker     (123)   300782 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/MRO120F.c
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/gravlib.c
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-08 20:31:10.000000 gravitas-0.1.9/gravitas/libgrav.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:31:22.942773 gravitas-0.1.9/gravitas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 20:31:22.000000 gravitas-0.1.9/gravitas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-06-08 20:31:22.000000 gravitas-0.1.9/gravitas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:31:22.000000 gravitas-0.1.9/gravitas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:31:22.000000 gravitas-0.1.9/gravitas.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 20:31:22.000000 gravitas-0.1.9/gravitas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 20:31:22.000000 gravitas-0.1.9/gravitas.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-08 20:31:10.000000 gravitas-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 20:31:22.942773 gravitas-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-08 20:31:10.000000 gravitas-0.1.9/setup.py
```

### Comparing `gravitas-0.1.7/PKG-INFO` & `gravitas-0.1.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.7
+Version: 0.1.9
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gravitas-0.1.7/README.md` & `gravitas-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/gravitas/EGM96.c` & `gravitas-0.1.9/gravitas/EGM96.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/gravitas/GRGM360.c` & `gravitas-0.1.9/gravitas/GRGM360.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/gravitas/MRO120F.c` & `gravitas-0.1.9/gravitas/MRO120F.c`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/gravitas/gravlib.c` & `gravitas-0.1.9/gravitas/gravlib.c`

 * *Files 4% similar despite different names*

```diff
@@ -112,14 +112,15 @@
 
 
 int nm2i(int n, int m) {
     return n * (n+1) / 2 + m;
 }
 
 void read_cnm_snm(int nmax, int model_index, double cnm[], double snm[]) {
+    printf("Starting coefficients read!\n");
     int num = ncoef_EGM96;
     const int* n = (int*) malloc(ncoef_EGM96 * sizeof(int));
     const int* m = (int*) malloc(ncoef_EGM96 * sizeof(int));
     const double* c = (double*) malloc(ncoef_EGM96 * sizeof(double));
     const double* s = (double*) malloc(ncoef_EGM96 * sizeof(double));
 
     if(model_index == EGM96) {
@@ -148,37 +149,34 @@
     }
     
     int i;
     for(i = 0; i < num; i++) {
         int ind = nm2i(*(n+i), *(m+i));
         cnm[ind] = *(c+i);
         snm[ind] = *(s+i);
-        // printf("n=%d, m=%d, c=%.2e, s=%.2e, cnm=%.2e, snm=%.2e\n", *(n+i), *(m+i), *(c+i), *(s+i), cnm[ind], snm[ind]);
+        printf("n=%d, m=%d, c=%.2e, s=%.2e, cnm=%.2e, snm=%.2e\n", *(n+i), *(m+i), *(c+i), *(s+i), cnm[ind], snm[ind]);
         if(*(m+i) == nmax) {
             break;
         }
     }
 
     snm[0] = 0.0;
     cnm[0] = 1.0;
-    // free((void*) n); //ansi-c but also not working
-    // free((void*) m);
-    // free((void*) c);
-    // free((void*) s);
+    printf("Finished coefficients read!\n");
     return;
 }
 
 Vector3 pinesnorm(Vector3 rf, double cnm[],
                double snm[], int nmax, double mu, double req) {
+    printf("Starting pinesnorm!\n");   
     // Based on pinesnorm() from: https://core.ac.uk/download/pdf/76424485.pdf
     double rmag = Vector3Norm(rf);
     Vector3 stu = Vector3Hat(rf);
     int anm_sz = nm2i(nmax+3, nmax+3);
     double *anm = malloc(anm_sz * sizeof(double)); //ansi-c
-    // double anm[anm_sz];
     anm[0] = sqrt(2.0);
 
     int m;
     for(m = 0; m <= nmax+2; m++) {
         if(m != 0) { // DIAGONAL RECURSION
             anm[nm2i(m,m)] = sqrt(1.0+1.0/(2.0*m))*anm[nm2i(m-1,m-1)];
         }
@@ -231,18 +229,18 @@
             double enm = cnm[nm2i(n,m)]*rm[m] + snm[nm2i(n,m)]*im[m];
             double fnm = snm[nm2i(n,m)]*rm[m] - cnm[nm2i(n,m)]*im[m];
             double alpha  = sqrt(sm*(n-m)*(n+m+1));
             g1t += anm[nm2i(n,m)]*m*enm;
             g2t += anm[nm2i(n,m)]*m*fnm;
             g3t += alpha*anmp1*dnm;
             g4t += ((n+m+1)*anm[nm2i(n,m)]+alpha*stu.z*anmp1)*dnm;
-            // printf("ANM: %d %d %.2e %.2e\n", n, m, anm[nm2i(n,m)], anmp1);
-            // printf("DEF: %d %d %.2e %.2e %.2e\n", n, m, dnm, enm, fnm);
-            // printf("G1-4t: %d %d %.2e %.2e %.2e %.2e\n", n, m, g1t, g2t, g3t, g4t);
-            // printf("CS: %d %d %.2e %.2e\n", n, m, cnm[nm2i(n,m)], snm[nm2i(n,m)]);
+            printf("ANM: %d %d %.2e %.2e\n", n, m, anm[nm2i(n,m)], anmp1);
+            printf("DEF: %d %d %.2e %.2e %.2e\n", n, m, dnm, enm, fnm);
+            printf("G1-4t: %d %d %.2e %.2e %.2e %.2e\n", n, m, g1t, g2t, g3t, g4t);
+            printf("CS: %d %d %.2e %.2e\n", n, m, cnm[nm2i(n,m)], snm[nm2i(n,m)]);
             if(m == 0) sm = 1.0;
         }
         rho *= rhop;
         g1 += rho*g1t; 
         g2 += rho*g2t; 
         g3 += rho*g3t; 
         g4 += rho*g4t;
```

### Comparing `gravitas-0.1.7/gravitas/lib.py` & `gravitas-0.1.9/gravitas/lib.py`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/gravitas/libgrav.h` & `gravitas-0.1.9/gravitas/libgrav.h`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/gravitas.egg-info/PKG-INFO` & `gravitas-0.1.9/gravitas.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gravitas
-Version: 0.1.7
+Version: 0.1.9
 Author: Liam Robinson
 Author-email: robin502@purdue.edu
 License: GPL-2
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `gravitas-0.1.7/pyproject.toml` & `gravitas-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gravitas-0.1.7/setup.py` & `gravitas-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 class CustomBuildExt(build_ext):
     def build_extensions(self):
         super().build_extensions()
 
 # _LIB_DIR
 setup(
     name='gravitas',
-    version='0.1.7',
+    version='0.1.9',
     packages=find_packages(),
     license='GPL-2',
     long_description="""High-fidelity gravity fields for satellite propagation""",
     long_description_content_type='text/markdown',
     author="Liam Robinson",
     author_email="robin502@purdue.edu",
     install_requires=['numpy'],
```

