# Comparing `tmp/simpledft-2.2.tar.gz` & `tmp/simpledft-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simpledft-2.2.tar", last modified: Wed Feb 22 10:58:37 2023, max compression
+gzip compressed data, was "simpledft-2.5.tar", last modified: Fri Jun  9 10:25:07 2023, max compression
```

## Comparing `simpledft-2.2.tar` & `simpledft-2.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-02-22 10:58:37.627742 simpledft-2.2/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2023-02-22 10:02:25.000000 simpledft-2.2/LICENSE
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3348 2023-02-22 10:58:37.627742 simpledft-2.2/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2230 2023-02-22 10:02:55.000000 simpledft-2.2/README.md
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-02-22 10:02:25.000000 simpledft-2.2/pyproject.toml
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-02-22 10:58:37.627742 simpledft-2.2/setup.cfg
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1452 2023-02-22 10:43:54.000000 simpledft-2.2/setup.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-02-22 10:58:37.627742 simpledft-2.2/simpledft/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       94 2023-02-22 10:43:47.000000 simpledft-2.2/simpledft/__init__.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2227 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/atoms.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1680 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/dft.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2799 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/energies.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1072 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/minimizer.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2838 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/operators.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      299 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/potentials.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      859 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/scf.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      662 2023-02-22 10:02:25.000000 simpledft-2.2/simpledft/utils.py
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1423 2023-02-22 10:53:50.000000 simpledft-2.2/simpledft/xc.py
-drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-02-22 10:58:37.627742 simpledft-2.2/simpledft.egg-info/
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3348 2023-02-22 10:58:37.000000 simpledft-2.2/simpledft.egg-info/PKG-INFO
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      439 2023-02-22 10:58:37.000000 simpledft-2.2/simpledft.egg-info/SOURCES.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-02-22 10:58:37.000000 simpledft-2.2/simpledft.egg-info/dependency_links.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-02-22 10:27:33.000000 simpledft-2.2/simpledft.egg-info/not-zip-safe
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       12 2023-02-22 10:58:37.000000 simpledft-2.2/simpledft.egg-info/requires.txt
--rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       10 2023-02-22 10:58:37.000000 simpledft-2.2/simpledft.egg-info/top_level.txt
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-06-09 10:25:07.493145 simpledft-2.5/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)    10173 2023-06-09 08:41:34.000000 simpledft-2.5/LICENSE
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3484 2023-06-09 10:25:07.489145 simpledft-2.5/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2230 2023-06-09 08:41:34.000000 simpledft-2.5/README.md
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       86 2023-06-09 08:41:34.000000 simpledft-2.5/pyproject.toml
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       38 2023-06-09 10:25:07.493145 simpledft-2.5/setup.cfg
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1579 2023-06-09 10:19:49.000000 simpledft-2.5/setup.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-06-09 10:25:07.489145 simpledft-2.5/simpledft/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       94 2023-06-09 10:11:41.000000 simpledft-2.5/simpledft/__init__.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2223 2023-06-09 09:04:36.000000 simpledft-2.5/simpledft/atoms.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1672 2023-06-09 09:06:03.000000 simpledft-2.5/simpledft/dft.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2779 2023-06-09 09:09:32.000000 simpledft-2.5/simpledft/energies.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1058 2023-06-09 09:52:56.000000 simpledft-2.5/simpledft/minimizer.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     2838 2023-06-09 09:28:48.000000 simpledft-2.5/simpledft/operators.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      299 2023-06-09 08:41:34.000000 simpledft-2.5/simpledft/potentials.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      859 2023-06-09 09:00:03.000000 simpledft-2.5/simpledft/scf.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      536 2023-06-09 08:41:34.000000 simpledft-2.5/simpledft/utils.py
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     1369 2023-06-09 09:45:02.000000 simpledft-2.5/simpledft/xc.py
+drwxrwxr-x   0 wangenau  (1000) wangenau  (1000)        0 2023-06-09 10:25:07.489145 simpledft-2.5/simpledft.egg-info/
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)     3484 2023-06-09 10:25:07.000000 simpledft-2.5/simpledft.egg-info/PKG-INFO
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)      439 2023-06-09 10:25:07.000000 simpledft-2.5/simpledft.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-06-09 10:25:07.000000 simpledft-2.5/simpledft.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)        1 2023-06-09 08:42:26.000000 simpledft-2.5/simpledft.egg-info/not-zip-safe
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       12 2023-06-09 10:25:07.000000 simpledft-2.5/simpledft.egg-info/requires.txt
+-rw-rw-r--   0 wangenau  (1000) wangenau  (1000)       10 2023-06-09 10:25:07.000000 simpledft-2.5/simpledft.egg-info/top_level.txt
```

### Comparing `simpledft-2.2/LICENSE` & `simpledft-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `simpledft-2.2/PKG-INFO` & `simpledft-2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: simpledft
-Version: 2.2
+Version: 2.5
 Summary: A simple density functional theory code.
 Home-page: https://gitlab.com/wangenau/simpledft
 Author: Wanja Timm Schulze
 Author-email: wangenau@protonmail.com
 License: APACHE2.0
 Project-URL: Bug Tracker, https://gitlab.com/wangenau/simpledft/-/issues
-Keywords: ESP
+Project-URL: Documentation, https://wangenau.gitlab.io/simpledft_pages
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Education
```

### Comparing `simpledft-2.2/README.md` & `simpledft-2.5/README.md`

 * *Files identical despite different names*

### Comparing `simpledft-2.2/setup.py` & `simpledft-2.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='simpledft',
-    version='2.2',
+    version='2.5',
     description='A simple density functional theory code.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Wanja Timm Schulze',
     author_email='wangenau@protonmail.com',
     url='https://gitlab.com/wangenau/simpledft',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Developers',
+        'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
+        'License :: OSI Approved',
         'License :: OSI Approved :: Apache Software License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Education',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Chemistry',
         'Topic :: Scientific/Engineering :: Physics',
         'Topic :: Software Development'
     ],
     license='APACHE2.0',
     install_requires=['numpy>=1.10'],
-    keywords=['ESP'],
     include_package_data=True,
     zip_safe=False,
     python_requires='>=3.5',
     project_urls={
-        'Bug Tracker': 'https://gitlab.com/wangenau/simpledft/-/issues'
+        'Bug Tracker': 'https://gitlab.com/wangenau/simpledft/-/issues',
+        'Documentation': 'https://wangenau.gitlab.io/simpledft_pages',
     }
 )
```

### Comparing `simpledft-2.2/simpledft/atoms.py` & `simpledft-2.5/simpledft/atoms.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
     def _get_index_matrices(self):
         '''Build index matrices M and N to build the real and reciprocal space samplings.
         Thesis: List 3.4
                 List 3.5
         '''
         ms = np.arange(np.prod(self.s))
-        m1 = ms % self.s[0]
-        m2 = np.floor(ms / self.s[0]) % self.s[1]
-        m3 = np.floor(ms / (self.s[0] * self.s[1])) % self.s[2]
+        m1 = np.floor(ms / (self.s[2] * self.s[1])) % self.s[0]
+        m2 = np.floor(ms / self.s[2]) % self.s[1]
+        m3 = ms % self.s[2]
         M = np.column_stack((m1, m2, m3))
 
         n1 = m1 - (m1 > self.s[0] / 2) * self.s[0]
         n2 = m2 - (m2 > self.s[1] / 2) * self.s[1]
         n3 = m3 - (m3 > self.s[2] / 2) * self.s[2]
         N = np.column_stack((n1, n2, n3))
         return M, N
@@ -42,15 +42,15 @@
         Thesis: Eq. 3.3
                 List. 3.3
                 Eq. 3.5
                 List. 3.3
         '''
         self.Natoms = len(self.atom)
         self.Nstate = len(self.f)
-        self.X = np.asarray(self.X)
+        self.X = np.atleast_2d(self.X)
         self.Z = np.asarray(self.Z)
 
         R = self.a * np.eye(3)
         self.R = R
         self.Omega = np.abs(np.linalg.det(R))
         self.r = M @ np.linalg.inv(np.diag(self.s)) @ R.T
 
@@ -66,8 +66,8 @@
         G = 2 * np.pi * N @ np.linalg.inv(self.R)
         self.G = G
         G2 = np.linalg.norm(G, axis=1)**2
         self.G2 = G2
         active = np.nonzero(G2 <= 2 * self.ecut)
         self.active = active
         self.G2c = G2[active]
-        self.Sf = np.sum(np.exp(-1j * self.G @ self.X.conj().T), axis=1)
+        self.Sf = np.sum(np.exp(-1j * self.G @ self.X.T), axis=1)
```

### Comparing `simpledft-2.2/simpledft/dft.py` & `simpledft-2.5/simpledft/dft.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from .utils import diagprod, sqrtm
+from .utils import sqrtm
 
 
 def solve_poisson(atoms, op, n):
     '''Solve the Poisson equation.
     Thesis: Eq. 2.48
     '''
     return -4 * np.pi * op.Linv(op.O(op.J(n)))
@@ -32,28 +32,29 @@
     '''Calculate the energy gradient with respect to W.
     Thesis: Eq. 2.43
             List. 3.24
     '''
     F = np.diag(atoms.f)
     HW = H(atoms, op, W, Y, n, phi, vxc, Vreciproc)
     WHW = W.conj().T @ HW
-    U = W.conj().T @ op.O(W)
+    OW = op.O(W)
+    U = W.conj().T @ OW
     invU = np.linalg.inv(U)
     U12 = sqrtm(invU)
     Ht = U12 @ WHW @ U12
-    return (HW - (op.O(W) @ invU) @ WHW) @ (U12 @ F @ U12) + op.O(W) @ (U12 @ Q(Ht @ F - F @ Ht, U))
+    return (HW - (OW @ invU) @ WHW) @ (U12 @ F @ U12) + OW @ (U12 @ Q(Ht @ F - F @ Ht, U))
 
 
 def H(atoms, op, W, Y, n, phi, vxc, Vreciproc):
     '''Left-hand side of the eigenvalue equation.
     Thesis: Eq. 2.45 ff.
             List. 3.26
     '''
     Veff = Vreciproc + op.Jdag(op.O(op.J(vxc) + phi))
-    return -0.5 * op.L(W) + op.Idag(diagprod(Veff, op.I(W)))
+    return -0.5 * op.L(W) + op.Idag(Veff[:, None] * op.I(W))
 
 
 def Q(inp, U):
     '''Operator needed to calculate gradients with non-constant occupations.
     Thesis: Eq. 2.47
             List. 3.25
     '''
```

### Comparing `simpledft-2.2/simpledft/energies.py` & `simpledft-2.5/simpledft/energies.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 
 
 def get_Ekin(atoms, op, W):
     '''Calculate the kinetic energy.
     Thesis: Eq. 2.37
     '''
     F = np.diag(atoms.f)
-    T = -0.5 * np.trace(F @ (W.conj().T @ op.L(W)))
+    T = -0.5 * np.trace(F @ W.conj().T @ op.L(W))
     return np.real(T)
 
 
 def get_Ecoul(op, n, phi):
     '''Calculate the Coulomb energy.
     Thesis: Eq. 2.40 + Eq. 2.41 (as in Eq. 2.49)
     '''
-    Ecoul = 0.5 * n.conj().T @ op.Jdag(op.O(phi))
+    Ecoul = 0.5 * n @ op.Jdag(op.O(phi))
     return np.real(Ecoul)
 
 
 def get_Exc(op, n, exc):
     '''Calculate the exchange-correlation energy.
     Thesis: Eq. 2.39
     '''
-    Exc = n.conj().T @ op.Jdag(op.O(op.J(exc)))
+    Exc = n @ op.Jdag(op.O(op.J(exc)))
     return np.real(Exc)
 
 
 def get_Een(n, Vreciproc):
     '''Calculate the electron-ion interaction.
     Thesis: Eq. 2.38
     '''
@@ -70,15 +70,15 @@
     M = get_index_vectors(s)
     T = M @ atoms.R
 
     for ia in range(atoms.Natoms):
         for ja in range(atoms.Natoms):
             dX = atoms.X[ia] - atoms.X[ja]
             ZiZj = atoms.Z[ia] * atoms.Z[ja]
-            for t in T:
+            for _ in T:
                 rmag = np.sqrt(np.linalg.norm(dX - T)**2)
                 Eewald += 0.5 * ZiZj * math.erfc(rmag * nu) / rmag
             if ia != ja:
                 rmag = np.sqrt(np.linalg.norm(dX)**2)
                 Eewald += 0.5 * ZiZj * math.erfc(rmag * nu) / rmag
 
     g = 2 * np.pi * np.linalg.inv(atoms.R.T)
```

### Comparing `simpledft-2.2/simpledft/minimizer.py` & `simpledft-2.5/simpledft/minimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .dft import get_grad, get_n_total, orth, solve_poisson
 from .energies import get_E
-from .xc import lda_chachiyo_c, lda_slater_x
+from .xc import lda_c_chachiyo, lda_x
 
 
 def scf_step(scf):
     '''Perform one SCF step for a DFT calculation.'''
     scf.Y = orth(scf.atoms, scf.op, scf.W)
     scf.n = get_n_total(scf.atoms, scf.op, scf.Y)
     scf.phi = solve_poisson(scf.atoms, scf.op, scf.n)
-    x, c = lda_slater_x(scf.n), lda_chachiyo_c(scf.n)
+    x, c = lda_x(scf.n), lda_c_chachiyo(scf.n)
     scf.exc = x[0] + c[0]
     scf.vxc = x[1] + c[1]
     return get_E(scf)
 
 
 def sd(scf, Nit, etol=1e-6, beta=1e-5):
     '''Steepest descent minimization algorithm.
```

### Comparing `simpledft-2.2/simpledft/operators.py` & `simpledft-2.5/simpledft/operators.py`

 * *Files identical despite different names*

### Comparing `simpledft-2.2/simpledft/scf.py` & `simpledft-2.5/simpledft/scf.py`

 * *Files identical despite different names*

### Comparing `simpledft-2.2/simpledft/xc.py` & `simpledft-2.5/simpledft/xc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import numpy as np
 
 
-def lda_slater_x(n):
+def lda_x(n):
     '''Slater exchange functional (spin-paired).
     Thesis: Eq. 2.11
     '''
     f = -3 / 4 * (3 / (2 * np.pi))**(2 / 3)
-
     rs = (3 / (4 * np.pi * n))**(1 / 3)
 
     ex = f / rs
     vx = 4 / 3 * ex
     return ex, vx
 
 
-def lda_chachiyo_c(n):
+def lda_c_chachiyo(n):
     '''Chachiyo parametrization of the correlation functional (spin-paired).'''
     a = -0.01554535  # (np.log(2) - 1) / (2 * np.pi**2)
     b = 20.4562557
 
     rs = (3 / (4 * np.pi * n))**(1 / 3)
 
     ec = a * np.log(1 + b / rs + b / rs**2)
     vc = ec + a * b * (2 + rs) / (3 * (b + b * rs + rs**2))
     return ec, vc
 
 
-def lda_vwn_c(n):
+def lda_c_vwn(n):
     '''Vosko-Wilk-Nusair parametrization of the correlation functional (spin-paired).
     Not used, only for reference as it was used in the master thesis.
     Thesis: Eq. 2.12 ff.
     '''
-    a = 0.0310907
+    A = 0.0310907
     b = 3.72744
     c = 12.9352
     x0 = -0.10498
 
     rs = (3 / (4 * np.pi * n))**(1 / 3)
 
-    q = np.sqrt(4 * c - b * b)
-    f1 = 2 * b / q
-    f2 = b * x0 / (x0 * x0 + b * x0 + c)
-    f3 = 2 * (2 * x0 + b) / q
-    rs12 = np.sqrt(rs)
-    fx = rs + b * rs12 + c
-    qx = np.arctan(q / (2 * rs12 + b))
-
-    ec = a * (np.log(rs / fx) + f1 * qx - f2 * (np.log((rs12 - x0)**2 / fx) + f3 * qx))
-    tx = 2 * rs12 + b
-    tt = tx * tx + q * q
-    vc = ec - rs12 * a / 6 * (2 / rs12 - tx / fx - 4 * b / tt - f2 * (2 / (rs12 - x0) - tx / fx - 4 * (2 * x0 + b) / tt))  # noqa: E501
+    x = np.sqrt(rs)
+    X = rs + b * x + c
+    Q = np.sqrt(4 * c - b**2)
+    fx0 = b * x0 / (x0**2 + b * x0 + c)
+    f3 = 2 * (2 * x0 + b) / Q
+    tx = 2 * x + b
+    tanx = np.arctan(Q / tx)
+
+    ec = A * (np.log(rs / X) + 2 * b / Q * tanx - fx0 * (np.log((x - x0)**2 / X) + f3 * tanx))
+
+    tt = tx**2 + Q**2
+    vc = ec - x * A / 6 * (2 / x - tx / X - 4 * b / tt - fx0 * (2 / (x - x0) - tx / X - 4 * (2 * x0 + b) / tt))  # noqa: E501
     return ec, vc
```

### Comparing `simpledft-2.2/simpledft.egg-info/PKG-INFO` & `simpledft-2.5/simpledft.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: simpledft
-Version: 2.2
+Version: 2.5
 Summary: A simple density functional theory code.
 Home-page: https://gitlab.com/wangenau/simpledft
 Author: Wanja Timm Schulze
 Author-email: wangenau@protonmail.com
 License: APACHE2.0
 Project-URL: Bug Tracker, https://gitlab.com/wangenau/simpledft/-/issues
-Keywords: ESP
+Project-URL: Documentation, https://wangenau.gitlab.io/simpledft_pages
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Education
```

