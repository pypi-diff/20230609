# Comparing `tmp/pyFBS-0.2.9.tar.gz` & `tmp/pyFBS-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFBS-0.2.9.tar", last modified: Mon Sep 19 07:30:11 2022, max compression
+gzip compressed data, was "pyFBS-0.3.0.tar", last modified: Fri Jun  9 11:38:24 2023, max compression
```

## Comparing `pyFBS-0.2.9.tar` & `pyFBS-0.3.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2022-09-19 07:30:11.807479 pyFBS-0.2.9/
--rw-rw-rw-   0        0        0      396 2022-09-19 07:23:58.000000 pyFBS-0.2.9/AUTHORS.rst
--rw-rw-rw-   0        0        0     8409 2022-09-19 07:23:58.000000 pyFBS-0.2.9/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1101 2022-09-19 07:23:58.000000 pyFBS-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      265 2022-09-19 07:23:58.000000 pyFBS-0.2.9/MANIFEST.in
--rw-rw-rw-   0        0        0     2786 2022-09-19 07:30:11.805416 pyFBS-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0     2035 2022-09-19 07:23:58.000000 pyFBS-0.2.9/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-19 07:30:11.770466 pyFBS-0.2.9/data/
--rw-rw-rw-   0        0        0    15168 2022-09-19 07:23:58.000000 pyFBS-0.2.9/data/logo-small.png
--rw-rw-rw-   0        0        0    42036 2022-09-19 07:23:58.000000 pyFBS-0.2.9/data/logo_new.png
-drwxrwxrwx   0        0        0        0 2022-09-19 07:30:11.663650 pyFBS-0.2.9/pyFBS/
--rw-rw-rw-   0        0        0    12319 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/IO.py
--rw-rw-rw-   0        0        0    33376 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/MCK.py
--rw-rw-rw-   0        0        0    13879 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/OSI.py
--rw-rw-rw-   0        0        0    22066 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/SEMM.py
--rw-rw-rw-   0        0        0     7632 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/SVT.py
--rw-rw-rw-   0        0        0    18601 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/VPT.py
--rw-rw-rw-   0        0        0      199 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/__init__.py
--rw-rw-rw-   0        0        0    34741 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/app_stability.py
--rw-rw-rw-   0        0        0    51328 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/display.py
--rw-rw-rw-   0        0        0    12977 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/modal_id.py
--rw-rw-rw-   0        0        0    46545 2022-09-19 07:24:01.000000 pyFBS-0.2.9/pyFBS/utility.py
-drwxrwxrwx   0        0        0        0 2022-09-19 07:30:11.742860 pyFBS-0.2.9/pyFBS.egg-info/
--rw-rw-rw-   0        0        0     2786 2022-09-19 07:30:10.000000 pyFBS-0.2.9/pyFBS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      685 2022-09-19 07:30:11.000000 pyFBS-0.2.9/pyFBS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-19 07:30:10.000000 pyFBS-0.2.9/pyFBS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2022-09-19 07:30:10.000000 pyFBS-0.2.9/pyFBS.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      139 2022-09-19 07:30:10.000000 pyFBS-0.2.9/pyFBS.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-09-19 07:30:10.000000 pyFBS-0.2.9/pyFBS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      309 2022-09-19 07:24:01.000000 pyFBS-0.2.9/requirements.txt
--rw-rw-rw-   0        0        0      139 2022-09-19 07:24:01.000000 pyFBS-0.2.9/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2022-09-19 07:30:11.807479 pyFBS-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     2238 2022-09-19 07:25:07.000000 pyFBS-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2022-09-19 07:30:11.800943 pyFBS-0.2.9/tests/
--rw-rw-rw-   0        0        0       36 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/__init__.py
--rw-rw-rw-   0        0        0     4334 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/build_examples.py
--rw-rw-rw-   0        0        0     2320 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/conftest.py
--rw-rw-rw-   0        0        0      686 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/test_IO.py
--rw-rw-rw-   0        0        0     1549 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/test_MCK.py
--rw-rw-rw-   0        0        0     1115 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/test_SVT.py
--rw-rw-rw-   0        0        0      956 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/test_VPT.py
--rw-rw-rw-   0        0        0     2661 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/test_display.py
--rw-rw-rw-   0        0        0      748 2022-09-19 07:24:01.000000 pyFBS-0.2.9/tests/test_modal_id.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:38:24.299283 pyFBS-0.3.0/
+-rw-rw-rw-   0        0        0      396 2023-06-09 11:36:13.000000 pyFBS-0.3.0/AUTHORS.rst
+-rw-rw-rw-   0        0        0     8409 2023-06-09 11:36:13.000000 pyFBS-0.3.0/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1101 2023-06-09 11:36:13.000000 pyFBS-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      265 2023-06-09 11:36:13.000000 pyFBS-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2786 2023-06-09 11:38:24.298280 pyFBS-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2035 2023-06-09 11:36:13.000000 pyFBS-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-09 11:38:24.137101 pyFBS-0.3.0/data/
+-rw-rw-rw-   0        0        0    15168 2023-06-09 11:36:13.000000 pyFBS-0.3.0/data/logo-small.png
+-rw-rw-rw-   0        0        0    42036 2023-06-09 11:36:13.000000 pyFBS-0.3.0/data/logo_new.png
+drwxrwxrwx   0        0        0        0 2023-06-09 11:38:24.047355 pyFBS-0.3.0/pyFBS/
+-rw-rw-rw-   0        0        0    12319 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/IO.py
+-rw-rw-rw-   0        0        0    33594 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/MCK.py
+-rw-rw-rw-   0        0        0    13879 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/OSI.py
+-rw-rw-rw-   0        0        0    22066 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/SEMM.py
+-rw-rw-rw-   0        0        0     7632 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/SVT.py
+-rw-rw-rw-   0        0        0    18601 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/VPT.py
+-rw-rw-rw-   0        0        0      199 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/__init__.py
+-rw-rw-rw-   0        0        0    35062 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/app_stability.py
+-rw-rw-rw-   0        0        0    51438 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/display.py
+-rw-rw-rw-   0        0        0    37294 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/modal_id.py
+-rw-rw-rw-   0        0        0    46545 2023-06-09 11:36:16.000000 pyFBS-0.3.0/pyFBS/utility.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:38:24.109821 pyFBS-0.3.0/pyFBS.egg-info/
+-rw-rw-rw-   0        0        0     2786 2023-06-09 11:38:22.000000 pyFBS-0.3.0/pyFBS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      685 2023-06-09 11:38:23.000000 pyFBS-0.3.0/pyFBS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:38:22.000000 pyFBS-0.3.0/pyFBS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-09 11:38:22.000000 pyFBS-0.3.0/pyFBS.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      140 2023-06-09 11:38:23.000000 pyFBS-0.3.0/pyFBS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-09 11:38:23.000000 pyFBS-0.3.0/pyFBS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      294 2023-06-09 11:36:16.000000 pyFBS-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0      146 2023-06-09 11:36:16.000000 pyFBS-0.3.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2023-06-09 11:38:24.299746 pyFBS-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2238 2023-06-09 11:36:16.000000 pyFBS-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 11:38:24.297048 pyFBS-0.3.0/tests/
+-rw-rw-rw-   0        0        0       36 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     4334 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/build_examples.py
+-rw-rw-rw-   0        0        0     2320 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/conftest.py
+-rw-rw-rw-   0        0        0      686 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/test_IO.py
+-rw-rw-rw-   0        0        0     1549 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/test_MCK.py
+-rw-rw-rw-   0        0        0     1115 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/test_SVT.py
+-rw-rw-rw-   0        0        0      956 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/test_VPT.py
+-rw-rw-rw-   0        0        0     2661 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/test_display.py
+-rw-rw-rw-   0        0        0      748 2023-06-09 11:36:16.000000 pyFBS-0.3.0/tests/test_modal_id.py
```

### Comparing `pyFBS-0.2.9/CONTRIBUTING.rst` & `pyFBS-0.3.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/LICENSE` & `pyFBS-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/PKG-INFO` & `pyFBS-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFBS
-Version: 0.2.9
+Version: 0.3.0
 Summary: pyFBS: A Python package for Frequency Based Substructuring and Transfer Path Analysis
 Home-page: https://pyfbs.readthedocs.io/en/latest/intro.html
 Author: Tomaž Bregar, Ahmed El Mahmoudi, Miha Kodrič, Domen Ocepek, Francesco Trainotti, Miha Pogačar, Mert Göldeli
 Author-email: info.pyfbs@gmail.com
 License: MIT license
 Keywords: pyFBS
 Platform: UNKNOWN
```

### Comparing `pyFBS-0.2.9/README.rst` & `pyFBS-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/data/logo-small.png` & `pyFBS-0.3.0/data/logo-small.png`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/data/logo_new.png` & `pyFBS-0.3.0/data/logo_new.png`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS/IO.py` & `pyFBS-0.3.0/pyFBS/IO.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS/MCK.py` & `pyFBS-0.3.0/pyFBS/MCK.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     :type recalculate: bool
     :param scale: distance scaling factor
     :type scale: float
     :param read_rst: if ``True`` reads the eigenvalue solution directly from .rst file
     :type read_rst: bool
     """
 
-    def __init__(self, rst_file=None, full_file=None, manual_mass_matrix=None, manual_stifenss_matrix=None, no_modes=100, allow_pickle=True, recalculate=False, scale=1000, read_rst=False):
+    def __init__(self, rst_file=None, full_file=None, manual_mass_matrix=None, manual_stifenss_matrix=None, no_modes=100, allow_pickle=True, recalculate=False, scale=1, read_rst=False):
         
         if rst_file and full_file: # check if rest and full files are defined, that mass and stifenss matrices will be importd from there
 
             rst = pymapdl_reader.read_binary(rst_file)
 
             # new version of pyansys
             self.nodes = rst.mesh.nodes*scale  # only translational dofs
@@ -50,31 +50,30 @@
                 self.no_modes = len(self.nodes)
             else:
                 self.no_modes = no_modes
 
             self._all = False
 
             full = pymapdl_reader.read_binary(full_file)
-            self.dof_ref, self.K, self.M = full.load_km(sort=True)  # dof_ref: 0-x 1-y 2-z
+            self.dof_ref, K_triu, M_triu = full.load_km(sort=True)  # dof_ref: 0-x 1-y 2-z
+            self.M = M_triu + sp.sparse.triu(M_triu, 1).T
+            self.K = K_triu + sp.sparse.triu(K_triu, 1).T
+            self._K = self.K + diags(np.random.random(self.K.shape[0]) / 1e20, shape=self.K.shape) # avoid error
+
             if self.dof_ref[0, 0] != 1:
                 self.dof_ref[:, 0] = self.dof_ref[:, 0] - (self.dof_ref[0, 0] - 1)
 
             if np.max(self.dof_ref[:, 1]) == 5:
                 self.rotation_included = True
             elif np.max(self.dof_ref[:, 1]) == 2:
                 self.rotation_included = False
 
             # an option to read directly the .rst file
             if read_rst == False:
                 #print("evaluating M and K matrices")
-                self._K = self.K + diags(np.random.random(self.K.shape[0]) / 1e20, shape=self.K.shape) # avoid error
-
-                self.M += sp.sparse.triu(self.M, 1).T
-                self._K += sp.sparse.triu(self._K, 1).T
-
                 p_file = '{}.pkl'.format(full_file)
                 # check if there is a .pkl file
                 same = False
                 if allow_pickle and path.exists(p_file):
                 
                     same = self.piclke_check(p_file, no_modes)
                     if same:
@@ -86,14 +85,20 @@
                 if same == False or recalculate == True:
                     self.eig_freq, self.eig_val, self.eig_vec = self.eig_solve(self.M, self._K, no_modes)
 
                     if allow_pickle:
                         pickle.dump([self.M, self.K, self.eig_freq, self.eig_val, self.eig_vec, no_modes],open(p_file, "wb"))
             else: # read from pyansys - from rst file
                 # print("Reading RST file")
+
+                self.M += sp.sparse.triu(self.M, 1).T
+                self.K += sp.sparse.triu(self.K, 1).T
+
+                self._K = self.K + diags(np.random.random(self.K.shape[0]) / 1e20, shape=self.K.shape) # avoid error
+
                 self.eig_freq, self.eig_val, self.eig_vec, self.eig_vec_strain = self.get_values_from_rst(rst)
                 if len(self.eig_freq)>=self.no_modes: # truncation of results in .rst file to match the desired number of modes in ``no_modes`` parameter
                     self.eig_freq = self.eig_freq[:self.no_modes]
                     self.eig_val = self.eig_val[:self.no_modes]
                     self.eig_vec = self.eig_vec[:, :self.no_modes]
                     try:
                         self.eig_vec_strain = self.eig_vec_strain[:, :self.no_modes]
@@ -207,15 +212,15 @@
         :type stiff_mat: scipy.sparse
         :param no_modes: number of considered modes
         :type no_modes: int
         :return:
         :rtype: (array(float), array(float), array(float))
         """
         try:
-            eigen_val, eigen_vec = sp.sparse.linalg.eigsh(stiff_mat, k=no_modes, M=mass_mat, which='LM', sigma=-1)
+            eigen_val, eigen_vec = sp.sparse.linalg.eigsh(stiff_mat, k=no_modes, M=mass_mat, sigma=0)
         except np.linalg.LinAlgError:
             # sometimes eigenvalue problems can not be solved using sparse configuration, especially for small analytical systems
             eigen_val, eigen_vec = sp.linalg.eig(stiff_mat, mass_mat)
 
         eigen_val.sort()
         eigen_freq = np.sqrt(np.abs(np.real(eigen_val)))  #/(2*np.pi)
         return (eigen_freq, eigen_val, eigen_vec)
```

### Comparing `pyFBS-0.2.9/pyFBS/OSI.py` & `pyFBS-0.3.0/pyFBS/OSI.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS/SEMM.py` & `pyFBS-0.3.0/pyFBS/SEMM.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS/SVT.py` & `pyFBS-0.3.0/pyFBS/SVT.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS/VPT.py` & `pyFBS-0.3.0/pyFBS/VPT.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS/app_stability.py` & `pyFBS-0.3.0/pyFBS/app_stability.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,19 +74,19 @@
         wid.setLayout(hbox)
 
         # Data definition
         self.selected_poles = []
         self.selected_ind = [] # indices of selected poles with respect to the order of the imputed poles 
         self.get_modal_data()
 
-        self.freq_trace = self.modal_id.freq#np.load("freq.npy")
+        self.freq_cmif = self.modal_id.freq#np.load("freq.npy")
         self.FRF_matrix = self.modal_id.FRF #np.load("Y.npy")
         self.poles = self.modal_id.stab_plot#np.load("for_plot.npy") # poles import
 
-        self.FRF_trace = np.trace(self.FRF_matrix, axis1=1, axis2=2)
+        self.FRF_cmif = np.linalg.svd(self.FRF_matrix)[1]
 
         #Model order / frequency / damping / pole type
         # Pole type:
         #   -   0 ... stable frequency, stable damping
         #   -   1 ... stable frequency, unstable samping
         #   -   2 ... unstable frequency, unstable damping
 
@@ -200,22 +200,22 @@
 
         editTableWidget = QWidget()
         editTableWidget.setLayout(editTableLayout)
 
         # FRF display option
         displyFRFoptionsLayout = QVBoxLayout()
         displyFRFsuboptionsLayout = QHBoxLayout()
-        self.display_trace = QCheckBox("Display trace")
-        self.display_trace.setChecked(True)
-        self.display_trace.stateChanged.connect(self.plot_trace)
+        self.display_cmif = QCheckBox("Display CMIF")
+        self.display_cmif.setChecked(True)
+        self.display_cmif.stateChanged.connect(self.plot_cmif)
 
         self.Btn_clear_FRF_display = QPushButton("Clear desplayed FRFs")
         self.Btn_clear_FRF_display.clicked.connect(self.clear_displayed_FRF)
 
-        displyFRFsuboptionsLayout.addWidget(self.display_trace)
+        displyFRFsuboptionsLayout.addWidget(self.display_cmif)
         displyFRFsuboptionsLayout.addWidget(self.Btn_clear_FRF_display)
         displyFRFsuboptionsWidget = QWidget()
         displyFRFsuboptionsWidget.setLayout(displyFRFsuboptionsLayout)
 
         displyFRFoptionsLayout.addWidget(QLabel("Plot FRF:"))
         displyFRFoptionsLayout.addWidget(displyFRFsuboptionsWidget)
 
@@ -396,15 +396,15 @@
         self.ax.yaxis.set_label_position("left")
         self.ax.yaxis.tick_left()
         self.axlog.yaxis.set_label_position("right")
         self.axlog.yaxis.tick_right()
         self.axlog.set_xlabel('Frequency [Hz]')
 
         # plot data
-        self.plot_trace()
+        self.plot_cmif()
         self.plot_FRF = self.axlog.semilogy([], [])
         self.data_3 = self.ax.scatter(self.x_data_3, self.y_data_3, s=int(self.point_size/2), color=self.colors[0], marker='o', 
                                         picker=1, pickradius=self.pick_radius_size, 
                                         label='Unstable', alpha=0.8)
         self.data_2 = self.ax.scatter(self.x_data_2, self.y_data_2, s=self.point_size, color=self.colors[1], marker='o', 
                                         picker=1, pickradius=self.pick_radius_size,
                                         label='Stable freq.', alpha=0.8)
@@ -449,18 +449,18 @@
         self.get_plot_limits()
         self.showMaximized()
         
     def autoscale_log_axis(self):
         self.axlog.autoscale(axis='y')
         self.fig.canvas.draw() # redraw graph
         
-    def plot_trace(self):
+    def plot_cmif(self):
         self.axlog.clear()
-        if self.display_trace.isChecked():
-            self.trace_plot = self.axlog.semilogy(self.freq_trace, np.abs(self.FRF_trace), c='k')
+        if self.display_cmif.isChecked():
+            self.cmif_plot = self.axlog.semilogy(self.freq_cmif, np.abs(self.FRF_cmif), c='k')
         
         self.axlog.set_ylabel("Amplitude")
         self.axlog.set_xlabel('Frequency [Hz]')
         self.axlog.yaxis.set_label_position("right")
         self.axlog.yaxis.tick_right()
         self.axlog.set_yscale('log')
         try:
@@ -603,18 +603,18 @@
                     self.statusBar.showMessage(f"The poles were deleted.")
                     self.statusBar.showMessage("Pole was deleted.")
         else:
             self.click_time_old = np.copy(self.click_time)
 
     def update_FRFS(self):
         self.get_plot_limits()
-        self.plot_trace()
+        self.plot_cmif()
         if len(np.array(self.selected_FRF).shape) == 2:
             FRF = np.abs(np.array(self.FRF_matrix[:, [np.array(self.selected_FRF)[:, 0]], [np.array(self.selected_FRF)[:, 1]]]))
-            self.plot_FRF = self.axlog.semilogy(self.freq_trace, np.abs(FRF).reshape(FRF.shape[0], int(FRF.shape[1]*FRF.shape[2])), alpha=self.FRF_transparency)
+            self.plot_FRF = self.axlog.semilogy(self.freq_cmif, np.abs(FRF).reshape(FRF.shape[0], int(FRF.shape[1]*FRF.shape[2])), alpha=self.FRF_transparency)
             self.fig.canvas.draw() # redraw graph
 
     def update_plot(self):
         if self.show_selected_poles.isChecked():
             try:
                 self.get_data_from_table()
                 self.selected_poles_plot.set_offsets(np.array([self.x_y_poles[:, 0], self.x_y_poles[:, 1]]).T)
@@ -770,17 +770,25 @@
                 ])
         self.x_y_poles = np.array(x_y_poles)
         self.all_selected_poles = np.asarray(all_selected_poles)
 
     def get_modal_data(self):
         selected_poles_id = []
         selected_mpf_id = []
+        nat_freq = []
+        damp_ratio = []
 
         for index_ in self.selected_ind:
             pole_, mpf_ = self.modal_id.pL_from_index(index_)
             selected_poles_id.append(pole_)
             selected_mpf_id.append(mpf_)
+
+            nat_freq_, damp_ratio_, _, __ = self.modal_id.transform_poles(pole_, mpf_.T, 1)
+
+            nat_freq.append(nat_freq_[0])
+            damp_ratio.append(damp_ratio_[0])
             
         self.modal_id.selected_poles = np.asarray(selected_poles_id)
         self.modal_id.selected_mpf = np.asarray(selected_mpf_id).T
-
+        self.modal_id.nat_freq = np.asarray(nat_freq)
+        self.modal_id.damp_ratio = np.asarray(damp_ratio)
```

### Comparing `pyFBS-0.2.9/pyFBS/display.py` & `pyFBS-0.3.0/pyFBS/display.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import numpy as np
 import pyvista as pv
 from pyvistaqt import BackgroundPlotter
 import pandas as pd
 from time import time,sleep
 from PyQt5.QtWidgets import QAction
 from PyQt5 import  QtGui
 import imageio
@@ -377,17 +378,17 @@
         :type direction: list
         :param size: Size of the impact
         :type size: float, optional
         :param color: Color of the impact
         :type color: str, optional
         """
         arrow = pv.Arrow(start=(0.0, 0.0, 0.0), direction=direction)
-        arrow.translate(-1*np.asarray(direction))
+        arrow.translate(-1*np.asarray(direction), inplace=True)
         arrow.points *= size
-        arrow.translate(np.asarray(position))
+        arrow.translate(np.asarray(position), inplace=True)
         imp_actor = self.plot.add_mesh(arrow, color=color,reset_camera = False, **kwargs)
 
         return arrow,imp_actor
 
 
     def add_channel(self, position, direction, size = 10, color = BLUE,**kwargs):
         """
@@ -436,15 +437,15 @@
 
         r = R.from_euler('xyz', [orientation[0], orientation[1], orientation[2]], degrees=True)
         rot = r.as_matrix()
 
         for item in accelerometer:
             item.points = (rot@item.points.T).T
 
-            item.translate(_new)
+            item.translate(_new, inplace=True)
 
         return accelerometer
 
     def add_accelerometer(self, acc):
         """
         Add an accelerometer to the 3D display.
 
@@ -688,15 +689,15 @@
         df = pd.DataFrame(columns=columns_chann)
 
         for i, _acc in enumerate(self.all_accs_dynamic):
             pos, euler_dir = _acc.get_pos_orient(euler_angles=True)
             data_chn = np.asarray([["Sensor " + str(1 + i), None, None, None, pos[0],pos[1],pos[2],euler_dir[0],euler_dir[1],euler_dir[2] ]])
 
             df_row = pd.DataFrame(data=data_chn, columns=columns_chann)
-            df = df.append(df_row, ignore_index=True)
+            df = pd.concat([df, df_row], ignore_index=True)
 
         return df
 
     def get_vp_data(self):
         """
         Returns positional information on interactive virtual points in the 3D display.
 
@@ -1088,15 +1089,15 @@
                                        [0, 0.5, 0],
                                        [0, 0, 0.5]]) * size
 
         self.points = (rot.T @ (self.points).T).T + size/2
 
         # Creates a bounding box
         self.box = pv.Box((-size, size, -size, size, -size, size))
-        self.box.translate([size, size, size])
+        self.box.translate([size, size, size], inplace=True)
         self.box.points /= 2
 
         self.fixed_theta = fixed_rotation
         # defines the objects
         objects.insert(0, self.box)
         self.objects = objects
 
@@ -1248,15 +1249,15 @@
         # move everything to a new location
         _new = point - self.box.center_of_mass()
 
         # snaps to the mesh and moves point widgets to the new location
         if snap:
             # translates
             for item in self.objects:
-                item.translate(_new)
+                item.translate(_new, inplace=True)
 
             self.p.sphere_widgets[self.N + 0].SetCenter(point)
             t_new = self.box.center_of_mass()
 
             for k in range(3):
                 self.local_widgets[k + 1, :] = rot @ self.local_widgets[k + 1, :]
                 self.p.sphere_widgets[self.N + k + 1].SetCenter(self.local_widgets[k + 1, :] + t_new)
@@ -1268,15 +1269,15 @@
             # rotate everything within accelerometer
             for item in self.objects:
                 item.points = (rot @ (item.points - t_new).T).T + t_new
             
 
         else:
             for item in self.objects:
-                item.translate(_new)
+                item.translate(_new, inplace=True)
             for i in range(4):
                 self.p.sphere_widgets[self.N + i].SetCenter(_new + np.asarray(self.p.sphere_widgets[self.N + i].GetCenter()))
 
     def callback(self, point, i):
         """
         A callback function for interaction with a sphere-widget.
```

### Comparing `pyFBS-0.2.9/pyFBS/utility.py` & `pyFBS-0.3.0/pyFBS/utility.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/pyFBS.egg-info/PKG-INFO` & `pyFBS-0.3.0/pyFBS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFBS
-Version: 0.2.9
+Version: 0.3.0
 Summary: pyFBS: A Python package for Frequency Based Substructuring and Transfer Path Analysis
 Home-page: https://pyfbs.readthedocs.io/en/latest/intro.html
 Author: Tomaž Bregar, Ahmed El Mahmoudi, Miha Kodrič, Domen Ocepek, Francesco Trainotti, Miha Pogačar, Mert Göldeli
 Author-email: info.pyfbs@gmail.com
 License: MIT license
 Keywords: pyFBS
 Platform: UNKNOWN
```

### Comparing `pyFBS-0.2.9/pyFBS.egg-info/SOURCES.txt` & `pyFBS-0.3.0/pyFBS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/setup.py` & `pyFBS-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,9 +66,9 @@
     include_package_data=True,
     package_data={'': extra_files},
     keywords='pyFBS',
     name='pyFBS',
     packages=["pyFBS"],
     test_suite='tests',
     url='https://pyfbs.readthedocs.io/en/latest/intro.html',
-    version='0.2.9',
+    version='0.3.0',
 )
```

### Comparing `pyFBS-0.2.9/tests/build_examples.py` & `pyFBS-0.3.0/tests/build_examples.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/conftest.py` & `pyFBS-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/test_IO.py` & `pyFBS-0.3.0/tests/test_IO.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/test_MCK.py` & `pyFBS-0.3.0/tests/test_MCK.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/test_SVT.py` & `pyFBS-0.3.0/tests/test_SVT.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/test_VPT.py` & `pyFBS-0.3.0/tests/test_VPT.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/test_display.py` & `pyFBS-0.3.0/tests/test_display.py`

 * *Files identical despite different names*

### Comparing `pyFBS-0.2.9/tests/test_modal_id.py` & `pyFBS-0.3.0/tests/test_modal_id.py`

 * *Files identical despite different names*

