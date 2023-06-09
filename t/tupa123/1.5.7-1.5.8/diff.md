# Comparing `tmp/tupa123-1.5.7.tar.gz` & `tmp/tupa123-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tupa123-1.5.7.tar", last modified: Tue Jun  6 20:06:17 2023, max compression
+gzip compressed data, was "tupa123-1.5.8.tar", last modified: Fri Jun  9 13:44:43 2023, max compression
```

## Comparing `tupa123-1.5.7.tar` & `tupa123-1.5.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.865681 tupa123-1.5.7/
--rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2352 2023-06-06 20:06:17.865681 tupa123-1.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.7/README.md
--rw-rw-rw-   0        0        0       42 2023-06-06 20:06:17.865681 tupa123-1.5.7/setup.cfg
--rw-rw-rw-   0        0        0      839 2023-06-06 20:05:09.000000 tupa123-1.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.765444 tupa123-1.5.7/tupa12/
--rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.7/tupa12/__init__.py
--rw-rw-rw-   0        0        0    54180 2023-06-05 16:54:03.000000 tupa123-1.5.7/tupa12/tupa12.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.843757 tupa123-1.5.7/tupa123/
--rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.7/tupa123/__init__.py
--rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.7/tupa123/machine1.txt
--rw-rw-rw-   0        0        0    94178 2023-06-06 19:56:11.000000 tupa123-1.5.7/tupa123/tupa123.py
-drwxrwxrwx   0        0        0        0 2023-06-06 20:06:17.865681 tupa123-1.5.7/tupa123.egg-info/
--rw-rw-rw-   0        0        0     2352 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-06 20:06:16.000000 tupa123-1.5.7/tupa123.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 13:44:43.298881 tupa123-1.5.8/
+-rw-rw-rw-   0        0        0     1101 2023-03-27 13:05:36.000000 tupa123-1.5.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2352 2023-06-09 13:44:43.283291 tupa123-1.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1876 2023-04-18 13:58:59.000000 tupa123-1.5.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-09 13:44:43.298881 tupa123-1.5.8/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-06-09 13:43:28.000000 tupa123-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:44:43.267665 tupa123-1.5.8/tupa12/
+-rw-rw-rw-   0        0        0       23 2023-05-30 20:43:01.000000 tupa123-1.5.8/tupa12/__init__.py
+-rw-rw-rw-   0        0        0    54797 2023-06-09 13:40:33.000000 tupa123-1.5.8/tupa12/tupa12.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:44:43.283291 tupa123-1.5.8/tupa123/
+-rw-rw-rw-   0        0        0       24 2023-05-30 20:42:30.000000 tupa123-1.5.8/tupa123/__init__.py
+-rw-rw-rw-   0        0        0   172319 2023-05-29 13:46:41.000000 tupa123-1.5.8/tupa123/machine1.txt
+-rw-rw-rw-   0        0        0    94790 2023-06-09 13:29:29.000000 tupa123-1.5.8/tupa123/tupa123.py
+drwxrwxrwx   0        0        0        0 2023-06-09 13:44:43.283291 tupa123-1.5.8/tupa123.egg-info/
+-rw-rw-rw-   0        0        0     2352 2023-06-09 13:44:43.000000 tupa123-1.5.8/tupa123.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-06-09 13:44:43.000000 tupa123-1.5.8/tupa123.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 13:44:43.000000 tupa123-1.5.8/tupa123.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-09 13:44:43.000000 tupa123-1.5.8/tupa123.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-09 13:44:43.000000 tupa123-1.5.8/tupa123.egg-info/top_level.txt
```

### Comparing `tupa123-1.5.7/LICENSE.txt` & `tupa123-1.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.7/PKG-INFO` & `tupa123-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.7
+Version: 1.5.8
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `tupa123-1.5.7/README.md` & `tupa123-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.7/setup.py` & `tupa123-1.5.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tupa123',
-    version='1.5.7',
+    version='1.5.8',
     license = 'MIT',
     license_files=('LICENSE.txt',),
     packages=['tupa123', 'tupa12'],
     package_data={'tupa123': ['machine1.txt'],},    
     install_requires=['numpy','matplotlib','pandas','opencv-python'],    
     author='Leandro Schemmer',
     author_email='leandro.schemmer@gmail.com',
```

### Comparing `tupa123-1.5.7/tupa12/tupa12.py` & `tupa123-1.5.8/tupa12/tupa12.py`

 * *Files 1% similar despite different names*

```diff
@@ -458,15 +458,20 @@
 ###############################################################
         
 
     #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
     def Fit_ADAM(self, matX, matY, matX2=[0], matY2=[0]):
         
         tinicio = time.time()
-        
+     
+        if np.ndim(matY) == 1: #ajusta caso for um vetor p/ matriz de 1 coluna
+            matY = np.reshape(matY, (-1, 1))
+            if (len(matY2)>1):
+                matY2 = np.reshape(matY2, (-1, 1))
+
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
 
         #bias
@@ -770,15 +775,20 @@
 
 
 
     #machine learning stochastic case by case------------------------------------------------------
     def Fit_STOC(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
-        
+
+        if np.ndim(matY) == 1: #ajusta caso for um vetor p/ matriz de 1 coluna
+            matY = np.reshape(matY, (-1, 1))
+            if (len(matY2)>1):
+                matY2 = np.reshape(matY2, (-1, 1))
+
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
 
         #bias
@@ -1022,15 +1032,20 @@
 
 
 
     #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
     def Fit_STOC_ADAM(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
-        
+
+        if np.ndim(matY) == 1: #ajusta caso for um vetor p/ matriz de 1 coluna
+            matY = np.reshape(matY, (-1, 1))
+            if (len(matY2)>1):
+                matY2 = np.reshape(matY2, (-1, 1))
+
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
 
         #bias
```

### Comparing `tupa123-1.5.7/tupa123/machine1.txt` & `tupa123-1.5.8/tupa123/machine1.txt`

 * *Files identical despite different names*

### Comparing `tupa123-1.5.7/tupa123/tupa123.py` & `tupa123-1.5.8/tupa123/tupa123.py`

 * *Files 0% similar despite different names*

```diff
@@ -1237,15 +1237,20 @@
 ###############################################################
         
 
     #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
     def Fit_ADAM(self, matX, matY, matX2=[0], matY2=[0]):
         
         tinicio = time.time()
-        
+
+        if np.ndim(matY) == 1: #ajusta caso for um vetor p/ matriz de 1 coluna
+            matY = np.reshape(matY, (-1, 1))
+            if (len(matY2)>1):
+                matY2 = np.reshape(matY2, (-1, 1))
+
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
         P34 = np.zeros((self.nn3c,self.nn4c))
 
@@ -1599,15 +1604,20 @@
 
 
 
     #machine learning stochastic case by case------------------------------------------------------
     def Fit_STOC(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
-        
+
+        if np.ndim(matY) == 1: #ajusta caso for um vetor p/ matriz de 1 coluna
+            matY = np.reshape(matY, (-1, 1))
+            if (len(matY2)>1):
+                matY2 = np.reshape(matY2, (-1, 1))
+
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
         P34 = np.zeros((self.nn3c,self.nn4c))
 
@@ -1885,15 +1895,20 @@
 
 
 
     #machine learning,  single batch with ADAM accelerator-----------------------------------------------------
     def Fit_STOC_ADAM(self, matX, matY, matX2=[0], matY2=[0]):
 
         tinicio = time.time()
-        
+
+        if np.ndim(matY) == 1: #ajusta caso for um vetor p/ matriz de 1 coluna
+            matY = np.reshape(matY, (-1, 1))
+            if (len(matY2)>1):
+                matY2 = np.reshape(matY2, (-1, 1))
+
         #Criação ou leitura da matriz dos pesos--------
 
         #pesos
         P12 = np.zeros((self.nn1c,self.nn2c))
         P23 = np.zeros((self.nn2c,self.nn3c))
         P34 = np.zeros((self.nn3c,self.nn4c))
```

### Comparing `tupa123-1.5.7/tupa123.egg-info/PKG-INFO` & `tupa123-1.5.8/tupa123.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tupa123
-Version: 1.5.7
+Version: 1.5.8
 Summary: fully connected neural network with four layers
 Author: Leandro Schemmer
 Author-email: leandro.schemmer@gmail.com
 License: MIT
 Keywords: artificial-intelligence neural-networks four-layers regression regression-analysis classification-algorithms tupa123 deep-learning machine-learning data-science artificial-neural-network open-source
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

