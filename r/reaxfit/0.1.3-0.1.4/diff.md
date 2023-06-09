# Comparing `tmp/reaxfit-0.1.3.tar.gz` & `tmp/reaxfit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reaxfit-0.1.3.tar", last modified: Wed Apr 12 05:04:43 2023, max compression
+gzip compressed data, was "reaxfit-0.1.4.tar", last modified: Fri Jun  9 08:33:45 2023, max compression
```

## Comparing `reaxfit-0.1.3.tar` & `reaxfit-0.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/.github/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.1.3/.github/release.yml
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/.github/workflows/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.1.3/.github/workflows/tagpr.yml
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.1.3/.gitignore
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.1.3/.tagpr
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.1.3/LICENSE
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      796 2023-04-12 05:04:43.049054 reaxfit-0.1.3/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      543 2023-04-12 04:40:21.000000 reaxfit-0.1.3/README.md
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/example/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/example/CoCO/
--rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/0.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/1.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/2.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/3.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/4.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/5.xyz
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/6.xyz
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.1.3/example/CoCO/batch.sh
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.1.3/example/CoCO/chk.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.1.3/example/CoCO/config.json
--rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/data0
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-04-12 04:40:21.000000 reaxfit-0.1.3/example/CoCO/ffield.reax
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.1.3/example/CoCO/ffield.temp
--rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/refE
--rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.1.3/example/CoCO/refF
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.1.3/example/CoCO/run.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.1.3/example/README.md
--rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-04-12 04:40:21.000000 reaxfit-0.1.3/reaxfit_sample.ipynb
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-04-12 05:04:43.049054 reaxfit-0.1.3/setup.cfg
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-04-12 04:40:21.000000 reaxfit-0.1.3/setup.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.045054 reaxfit-0.1.3/src/
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/src/reaxfit/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.1.3/src/reaxfit/__init__.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.1.3/src/reaxfit/_version.py
--rw-rw-r--   0 ykane     (1000) ykane     (1000)     5952 2023-03-03 02:20:33.000000 reaxfit-0.1.3/src/reaxfit/reaxfit.py
-drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-04-12 05:04:43.049054 reaxfit-0.1.3/src/reaxfit.egg-info/
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      796 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/PKG-INFO
--rw-rw-r--   0 ykane     (1000) ykane     (1000)      667 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/SOURCES.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/dependency_links.txt
--rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-04-12 05:04:42.000000 reaxfit-0.1.3/src/reaxfit.egg-info/top_level.txt
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.765588 reaxfit-0.1.4/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/.github/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       48 2023-03-03 06:38:54.000000 reaxfit-0.1.4/.github/release.yml
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/.github/workflows/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      251 2023-03-03 06:38:54.000000 reaxfit-0.1.4/.github/workflows/tagpr.yml
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      111 2023-04-12 04:40:21.000000 reaxfit-0.1.4/.gitignore
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1794 2023-03-03 06:38:54.000000 reaxfit-0.1.4/.tagpr
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     1067 2023-03-01 01:38:22.000000 reaxfit-0.1.4/LICENSE
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-09 08:33:45.765588 reaxfit-0.1.4/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      732 2023-06-09 06:14:50.000000 reaxfit-0.1.4/README.md
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/example/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/example/CoCO/
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     1892 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/0.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2151 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/1.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/2.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/3.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/4.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2039 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/5.xyz
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2095 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/6.xyz
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      189 2023-02-28 13:43:09.000000 reaxfit-0.1.4/example/CoCO/batch.sh
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      374 2023-02-28 13:52:46.000000 reaxfit-0.1.4/example/CoCO/chk.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      260 2023-03-03 02:56:27.000000 reaxfit-0.1.4/example/CoCO/config.json
+-rw-r--r--   0 ykane     (1000) ykane     (1000)     2310 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/data0
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22606 2023-06-09 06:14:50.000000 reaxfit-0.1.4/example/CoCO/ffield.reax
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    22677 2023-03-02 14:08:20.000000 reaxfit-0.1.4/example/CoCO/ffield.temp
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       58 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/refE
+-rw-r--r--   0 ykane     (1000) ykane     (1000)       56 2023-02-22 04:48:36.000000 reaxfit-0.1.4/example/CoCO/refF
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      127 2023-02-28 13:40:22.000000 reaxfit-0.1.4/example/CoCO/run.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      235 2023-03-01 02:14:34.000000 reaxfit-0.1.4/example/README.md
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)    61858 2023-06-09 06:14:50.000000 reaxfit-0.1.4/reaxfit_sample.ipynb
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       38 2023-06-09 08:33:45.765588 reaxfit-0.1.4/setup.cfg
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      723 2023-06-09 06:14:50.000000 reaxfit-0.1.4/setup.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.757588 reaxfit-0.1.4/src/
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.761588 reaxfit-0.1.4/src/reaxfit/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)       30 2023-02-22 05:23:36.000000 reaxfit-0.1.4/src/reaxfit/__init__.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      160 2023-03-03 07:37:02.000000 reaxfit-0.1.4/src/reaxfit/_version.py
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)     8849 2023-06-09 08:31:23.000000 reaxfit-0.1.4/src/reaxfit/reaxfit.py
+drwxrwxr-x   0 ykane     (1000) ykane     (1000)        0 2023-06-09 08:33:45.765588 reaxfit-0.1.4/src/reaxfit.egg-info/
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      965 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/PKG-INFO
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)      667 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/SOURCES.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        1 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/dependency_links.txt
+-rw-rw-r--   0 ykane     (1000) ykane     (1000)        8 2023-06-09 08:33:45.000000 reaxfit-0.1.4/src/reaxfit.egg-info/top_level.txt
```

### Comparing `reaxfit-0.1.3/.tagpr` & `reaxfit-0.1.4/.tagpr`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/LICENSE` & `reaxfit-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/PKG-INFO` & `reaxfit-0.1.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.1.3
+Version: 0.1.4
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ReaxFit
 Parameter-fitting module for lammps-reaxff with differential_evolution of scipy.
 ## Requirements
 - lammps (library)
@@ -18,16 +17,15 @@
 ## Install
 - use anaconda
 ```sh
 conda install -c conda-forge lammps
 conda install scipy numpy
 pip3 install reaxfit
 ```
+For Windows, lammps from conda forge is not available. You can alternatively download the lammps binary with the python library from [lammps.org](https://packages.lammps.org/windows.html).
 - [option] install jupyterlab and ase
 It will be convenient to use reaxff with jupyterlab and ase.
 ```sh
 conda install -c conda-forge jupyterlab ase
 ```
 ## Useage 
 - See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/main/reaxfit_sample.ipynb)
-
-
```

### Comparing `reaxfit-0.1.3/README.md` & `reaxfit-0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ## Install
 - use anaconda
 ```sh
 conda install -c conda-forge lammps
 conda install scipy numpy
 pip3 install reaxfit
 ```
+For Windows, lammps from conda forge is not available. You can alternatively download the lammps binary with the python library from [lammps.org](https://packages.lammps.org/windows.html).
 - [option] install jupyterlab and ase
 It will be convenient to use reaxff with jupyterlab and ase.
 ```sh
 conda install -c conda-forge jupyterlab ase
 ```
 ## Useage 
 - See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/main/reaxfit_sample.ipynb)
```

### Comparing `reaxfit-0.1.3/example/CoCO/0.xyz` & `reaxfit-0.1.4/example/CoCO/0.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/1.xyz` & `reaxfit-0.1.4/example/CoCO/1.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/2.xyz` & `reaxfit-0.1.4/example/CoCO/2.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/3.xyz` & `reaxfit-0.1.4/example/CoCO/3.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/4.xyz` & `reaxfit-0.1.4/example/CoCO/4.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/5.xyz` & `reaxfit-0.1.4/example/CoCO/5.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/6.xyz` & `reaxfit-0.1.4/example/CoCO/6.xyz`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/data0` & `reaxfit-0.1.4/example/CoCO/data0`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/ffield.reax` & `reaxfit-0.1.4/example/CoCO/ffield.reax`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/example/CoCO/ffield.temp` & `reaxfit-0.1.4/example/CoCO/ffield.temp`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/reaxfit_sample.ipynb` & `reaxfit-0.1.4/reaxfit_sample.ipynb`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/setup.py` & `reaxfit-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `reaxfit-0.1.3/src/reaxfit/reaxfit.py` & `reaxfit-0.1.4/src/reaxfit/reaxfit.py`

 * *Files 25% similar despite different names*

```diff
@@ -14,29 +14,95 @@
             "refE_file":"refE", # reference energy
             "refF_file":"refF", # reference force norm
             "datafile":"data0", # data file with initial structure
             "initfile":"ffield.temp", # initial template file
             "midfile":"ffield.currentbest", # intermediate file
             "endfile":"ffield.end", # final file
             "bound":0.1, # define range of parameters 
+            "bound2":0.1, # define range of parameters 
             "stopfile":"STOP", # file for early stopping
             "seed":None, # file for early stopping
             "tol":0.01, # tolerance for convergence
             "workers":4, # file for early stopping
             "maxiter":1000, # maximum number of iteration
             "scrdir":"scr" # scratch directory
     }
     isconfig=os.path.isfile(cfile)
     if dump_config:
         if isconfig: os.rename(cfile,cfile+".bk")
         with open(cfile,"w") as f:
             json.dump(self.option,f,indent=1)
         sys.exit()
     return
-
+  def changes(self,para,file_name,atm1,atm2,numbers):
+    with open(file_name) as f:
+        text=f.read().splitlines()
+    general =text[1].split()
+    generals = int(general[0]) + 1
+    atom=text[generals+1].split()
+    atoms = int(atom[0])*4 +1 +3
+    x = generals +atoms
+    j=1 
+    atm=[]
+    atm_dict={}
+    while j <= int(atom[0]):
+        y = text[generals+1+j*4].split()
+        atm.append(y[0])
+        atm_dict[y[0]]=j
+        j+=1
+    bonds=text[x+1].split()
+    bond_max =int(bonds[0])*2+2+x
+    #print(x)
+    i=x+1
+    while i <= bond_max:
+        regax=re.compile(f"^\s*{atm_dict[atm1]}\s+{atm_dict[atm2]}\s|^\s*{atm_dict[atm2]}\s+{atm_dict[atm1]}\s")
+        fire=regax.findall(text[i])
+        if len(fire) != 0:
+            #print(i)
+            #print(text[i])
+            #print(text[i+1])
+            d = text[i].split()
+            if numbers <= 8:
+                if d[numbers+1].startswith("{") or d[numbers+1].startswith("["):
+                    pass
+                elif para=="{":
+                    d[numbers+1]="{"+d[numbers+1]
+                    print(text[i])
+                    print(d[numbers+1])
+                else:
+                    d[numbers+1]="["+d[numbers+1]
+                    print(text[i])
+                    print(d[numbers+1])
+                result =" ".join(d)
+                gyou = i
+            else:
+                i+=1
+                gyou = i
+                d = text[i].split()
+                if d[numbers-9].startswith("{") or d[numbers-9].startswith("["):
+                    pass
+                elif para=="{":
+                    d[numbers-9]="{"+d[numbers-9]
+                    print(text[i])
+                    print(d[numbers-9])
+                    i-=1
+                else:
+                    d[numbers-9]="["+d[numbers-9]
+                    print(text[i])
+                    print(d[numbers-9])
+                    i-=1
+                    
+                result=" ".join(d)
+        i+=1
+    with open(file_name) as f:
+        l = f.readlines()
+    del l[gyou]
+    l.insert(gyou,f"{result}\n")
+    with open(file_name,mode="w")as f:
+        f.writelines(l)
   def config(self,**kwargs):
     global dump_best
     if hasattr(kwargs,"cfile"): self.cfile=kwargs["cfile"]
     opt=self.option
     isconfig=os.path.isfile(self.cfile)
     if isconfig:
         print(f"read {self.cfile}")
@@ -63,23 +129,49 @@
     with open(self.refF_file) as f:
       refF=f.read().split()
     refE=np.array(refE,dtype=float)
     refF=np.array(refF,dtype=float)
     # read template and x0
     with open(self.initfile) as f:
       _template=f.read()
-    regex=re.compile(r"{([\d.-]+)}?")
+    regex=re.compile("[\{\[][\d.-]+")
     x0=regex.findall(_template)
+    isBound1=[]
+    x1 = 0
+    for x1 in range(len(x0)):
+        if x0[x1].startswith("{"):
+            isBound1.append("True")
+            x0[x1]=x0[x1].strip("{")
+        else:
+            isBound1.append("False")
+            x0[x1]=x0[x1].strip("[")
+        x1+=1
+    #print(x0)
     self.x0=[float(x) for x in x0]
+    #print(x1)
+    self.template = _template
+    # change {S
     # define bounds
-    bounds=[]
     for x in self.x0:
-      delta = abs(float(self.bound)*x)
-      t = (x-delta,x+delta)
-      bounds.append(t)
+        if x==0:
+            print("error:0 cannot be used as a parameter.")
+            sys.exit(1)
+        else:
+            pass
+    bounds=[]
+    for i,x in enumerate(self.x0):
+        if isBound1[i] =="True":
+            delta = abs(float(self.bound)*x)
+            t = (x-delta,x+delta)
+            bounds.append(t)
+        else:
+            sigma = abs(float(self.bound2)*x)
+            k=(x-sigma,x+sigma)
+            bounds.append(k)
+    #print(bounds)
     self.bounds=bounds
     template=regex.sub("{}",_template)
     self.template=template
     # get elements from templates
     eles=re.findall(r"\n *(:?[A-Z][a-z]?)",template)
     self.elements=" ".join(eles)
     self.refE=refE
```

### Comparing `reaxfit-0.1.3/src/reaxfit.egg-info/PKG-INFO` & `reaxfit-0.1.4/src/reaxfit.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: reaxfit
-Version: 0.1.3
+Version: 0.1.4
 Summary: parameter fitting for ReaxFF
 Home-page: https://github.com/ykanematsu/reaxfit
 Author: ykanematsu
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ReaxFit
 Parameter-fitting module for lammps-reaxff with differential_evolution of scipy.
 ## Requirements
 - lammps (library)
@@ -18,16 +17,15 @@
 ## Install
 - use anaconda
 ```sh
 conda install -c conda-forge lammps
 conda install scipy numpy
 pip3 install reaxfit
 ```
+For Windows, lammps from conda forge is not available. You can alternatively download the lammps binary with the python library from [lammps.org](https://packages.lammps.org/windows.html).
 - [option] install jupyterlab and ase
 It will be convenient to use reaxff with jupyterlab and ase.
 ```sh
 conda install -c conda-forge jupyterlab ase
 ```
 ## Useage 
 - See [A sample on colab](https://colab.research.google.com/github/ykanematsu/reaxfit/blob/main/reaxfit_sample.ipynb)
-
-
```

### Comparing `reaxfit-0.1.3/src/reaxfit.egg-info/SOURCES.txt` & `reaxfit-0.1.4/src/reaxfit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

