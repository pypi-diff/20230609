# Comparing `tmp/SeanFunctions-0.5.2.tar.gz` & `tmp/SeanFunctions-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SeanFunctions-0.5.2.tar", last modified: Fri May 12 21:32:21 2023, max compression
+gzip compressed data, was "SeanFunctions-0.5.3.tar", last modified: Fri Jun  9 17:32:11 2023, max compression
```

## Comparing `SeanFunctions-0.5.2.tar` & `SeanFunctions-0.5.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-12 21:32:21.244303 SeanFunctions-0.5.2/
--rw-rw-rw-   0        0        0      274 2022-12-23 21:21:19.000000 SeanFunctions-0.5.2/.gitignore
--rw-rw-rw-   0        0        0     1087 2022-12-10 20:47:50.000000 SeanFunctions-0.5.2/LICENSE
--rw-rw-rw-   0        0        0       36 2022-12-23 17:02:46.000000 SeanFunctions-0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0      686 2023-05-12 21:32:21.243807 SeanFunctions-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0      144 2022-12-10 20:41:39.000000 SeanFunctions-0.5.2/README.md
--rw-rw-rw-   0        0        0     1165 2023-05-12 20:31:09.000000 SeanFunctions-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-12 21:32:21.244799 SeanFunctions-0.5.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-12 21:32:21.203407 SeanFunctions-0.5.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-12 21:32:21.225885 SeanFunctions-0.5.2/src/SeanFunctions/
-drwxrwxrwx   0        0        0        0 2023-05-12 21:32:21.242815 SeanFunctions-0.5.2/src/SeanFunctions/Data/
--rw-rw-rw-   0        0        0    19820 2022-12-23 19:43:28.000000 SeanFunctions-0.5.2/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
--rw-rw-rw-   0        0        0    14993 2022-12-23 20:13:17.000000 SeanFunctions-0.5.2/src/SeanFunctions/Data/NeutronScatteringLengths.csv
--rw-rw-rw-   0        0        0    15625 2022-12-23 21:07:44.000000 SeanFunctions-0.5.2/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
--rw-rw-rw-   0        0        0       39 2022-12-23 17:31:09.000000 SeanFunctions-0.5.2/src/SeanFunctions/__init__.py
--rw-rw-rw-   0        0        0     4906 2023-04-18 20:46:49.000000 SeanFunctions-0.5.2/src/SeanFunctions/fitting.py
--rw-rw-rw-   0        0        0     9718 2023-04-12 20:00:53.000000 SeanFunctions-0.5.2/src/SeanFunctions/math.py
--rw-rw-rw-   0        0        0    15691 2023-05-12 21:32:05.000000 SeanFunctions-0.5.2/src/SeanFunctions/scattering.py
--rw-rw-rw-   0        0        0      220 2023-05-12 21:32:20.000000 SeanFunctions-0.5.2/src/SeanFunctions/version.py
-drwxrwxrwx   0        0        0        0 2023-05-12 21:32:21.238309 SeanFunctions-0.5.2/src/SeanFunctions.egg-info/
--rw-rw-rw-   0        0        0      686 2023-05-12 21:32:21.000000 SeanFunctions-0.5.2/src/SeanFunctions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2023-05-12 21:32:21.000000 SeanFunctions-0.5.2/src/SeanFunctions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-12 21:32:21.000000 SeanFunctions-0.5.2/src/SeanFunctions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-12 21:32:21.000000 SeanFunctions-0.5.2/src/SeanFunctions.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.091444 SeanFunctions-0.5.3/
+-rw-rw-rw-   0        0        0      274 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/.gitignore
+-rw-rw-rw-   0        0        0     1087 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      678 2023-06-09 17:32:11.090451 SeanFunctions-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/README.md
+-rw-rw-rw-   0        0        0     1157 2023-06-09 17:31:09.000000 SeanFunctions-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 17:32:11.091940 SeanFunctions-0.5.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.052593 SeanFunctions-0.5.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.069045 SeanFunctions-0.5.3/src/SeanFunctions/
+drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.089456 SeanFunctions-0.5.3/src/SeanFunctions/Data/
+-rw-rw-rw-   0        0        0    19820 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv
+-rw-rw-rw-   0        0        0    14993 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv
+-rw-rw-rw-   0        0        0    15625 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv
+-rw-rw-rw-   0        0        0       39 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/__init__.py
+-rw-rw-rw-   0        0        0     4906 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/fitting.py
+-rw-rw-rw-   0        0        0     9718 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/math.py
+-rw-rw-rw-   0        0        0    15741 2023-06-09 17:27:31.000000 SeanFunctions-0.5.3/src/SeanFunctions/scattering.py
+-rw-rw-rw-   0        0        0      220 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions/version.py
+drwxrwxrwx   0        0        0        0 2023-06-09 17:32:11.084967 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/
+-rw-rw-rw-   0        0        0      678 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2023-06-09 17:32:11.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-09 17:32:10.000000 SeanFunctions-0.5.3/src/SeanFunctions.egg-info/top_level.txt
```

### Comparing `SeanFunctions-0.5.2/LICENSE` & `SeanFunctions-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.2/pyproject.toml` & `SeanFunctions-0.5.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [project]
 name = "SeanFunctions"
-version = "0.5.2"
+version = "0.5.3"
 # dynamic = ["version"]
 authors = [
   { name="Sean Fayfar", email="sfayfar@gmail.com" },
 ]
 description = "Collection of useful python functions"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-Homepage = "https://github.mit.edu/sfayfar/SeanFunctions"
-"Bug Tracker" = "https://github.mit.edu/sfayfar/SeanFunctions/issues"
+Homepage = "https://github.com/sfayfar/SeanFunctions"
+"Bug Tracker" = "https://github.com/sfayfar/SeanFunctions/issues"
 
 
 [options]
 packages = "find:"
 python_requires = ">=3.7"
 setup_requires = "setuptools_scm"
 package_dir = "src"
```

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions/Data/AtomicFormFactorConstants.csv` & `SeanFunctions-0.5.3/src/SeanFunctions/Data/AtomicFormFactorConstants.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions/Data/NeutronScatteringLengths.csv` & `SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv` & `SeanFunctions-0.5.3/src/SeanFunctions/Data/NeutronScatteringLengths_Corrected.csv`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions/fitting.py` & `SeanFunctions-0.5.3/src/SeanFunctions/fitting.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions/math.py` & `SeanFunctions-0.5.3/src/SeanFunctions/math.py`

 * *Files identical despite different names*

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions/scattering.py` & `SeanFunctions-0.5.3/src/SeanFunctions/scattering.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                                         'Scatt xs':np.float64,
                                         'Abs xs':np.float64})
     return nsl_DF
 
 
 class weight_RDF_for_scattering:
     
-    def __init__(self,RDF_DataFrame,composition,cutoffR=None,isotopeDict=None,ionsDict=None,interpType='cubic',interpAmount=10):
+    def __init__(self,RDF_DataFrame,composition,cutoffR=None,isotopeDict=None,ionsDict=None,interpType='cubic',interpAmount=10,xrayRCut=100):
         '''
         Converts molecular dynamics partial RDFs into weighted g(r) and S(Q) for neutron and X-ray scattering.
         The input RDF must be a Pandas DataFrame with the column names as the atomic pairs such as "F-F" or "Na-Cl".
 
         Parameters
         ---------
         RDF_DataFrame : DataFrame
@@ -284,17 +284,17 @@
             totalSofQ += self.SofQXray[column]
         self.SofQXray['Total'] = totalSofQ
         
         # X-ray gofr
         self.gofrXray = pd.DataFrame()
         # self.gofrXray['r'] = RDF_DataFrame.iloc[:,0]
         totalgofr = 0
-        cutAt100InvAng = find_nearest(self.SofQXray['Q'],100)[0]
+        cutAt100InvAng = find_nearest(self.SofQXray['Q'],xrayRCut)[0]
         for column in RDF_DataFrame.keys()[1:]:
-            r, gofr = fourierbesseltransform(self.SofQXray['Q'].iloc[:cutAt100InvAng:10].to_numpy(),self.SofQXray[column].iloc[:cutAt100InvAng:10].to_numpy(),unpack=True)
+            r, gofr = fourierbesseltransform(self.SofQXray['Q'].iloc[:cutAt100InvAng:interpAmount].to_numpy(),self.SofQXray[column].iloc[:cutAt100InvAng:interpAmount].to_numpy(),unpack=True)
             self.gofrXray['r'] = r
             self.gofrXray[column] = gofr * 2 / np.pi
             totalgofr += gofr * 2 / np.pi
         self.gofrXray['Total'] = totalgofr
         
         
         
@@ -331,21 +331,21 @@
 
         for atoms in self.compositionTable.index:
             if neutron:
                 labelValue = atoms
                 if self.isotopeDict is not None:
                     if atoms in self.isotopeDict.keys():
                         labelValue + str(self.isotopeDict[atoms])
-                ax.plot(self.QArrInterp,np.full(len(self.QArrInterp),self.compositionTable.b[atoms]),'-',lw=1,label=labelValue,**kwargs)
+                ax.plot(self.QArrInterp,np.full(len(self.QArrInterp),self.compositionTable.b[atoms]),'-',lw=1,label=labelValue+' b',**kwargs)
             if xray:
                 labelValue = atoms
                 if self.ionsDict is not None:
                         if atoms in self.ionsDict.keys():
                             labelValue += str(self.ionsDict[atoms])
-                ax.plot(self.QArrInterp,self.compositionTable.aff[atoms],'-',lw=1,label=labelValue,**kwargs)
+                ax.plot(self.QArrInterp,self.compositionTable.aff[atoms],'-',lw=1,label=labelValue+' aff',**kwargs)
 
     def calc_num_density(self,density):
         '''
         Calculates the number density (in num per Ang^3) using the 
         chemical formula and input density.
 
         Inputs
```

### Comparing `SeanFunctions-0.5.2/src/SeanFunctions.egg-info/SOURCES.txt` & `SeanFunctions-0.5.3/src/SeanFunctions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

