# Comparing `tmp/hosgdSims-0.3.0.tar.gz` & `tmp/hosgdSims-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hosgdSims-0.3.0.tar", last modified: Tue Jun  6 05:08:27 2023, max compression
+gzip compressed data, was "hosgdSims-0.5.0.tar", last modified: Fri Jun  9 05:47:52 2023, max compression
```

## Comparing `hosgdSims-0.3.0.tar` & `hosgdSims-0.5.0.tar`

### file list

```diff
@@ -1,27 +1,33 @@
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/
--rw-r--r--   0 jaru      (1000) users      (100)       35 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/AUTHORS
--rw-r--r--   0 jaru      (1000) users      (100)       11 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/MANIFEST.in
--rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/PKG-INFO
--rw-r--r--   0 jaru      (1000) users      (100)      477 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/README.md
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/hosgdSims/
--rw-r--r--   0 jaru      (1000) users      (100)     2227 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDdefs.py
--rw-r--r--   0 jaru      (1000) users      (100)      283 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDegAF.py
--rw-r--r--   0 jaru      (1000) users      (100)     9091 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabAF.py
--rw-r--r--   0 jaru      (1000) users      (100)     6400 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabAGD.py
--rw-r--r--   0 jaru      (1000) users      (100)     9502 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabGD.py
--rw-r--r--   0 jaru      (1000) users      (100)    14694 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabHL.py
--rw-r--r--   0 jaru      (1000) users      (100)     8058 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabSGD.py
--rw-r--r--   0 jaru      (1000) users      (100)     7151 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/hosgdSims/HoSGDlabSGDVariants.py
--rw-r--r--   0 jaru      (1000) users      (100)      150 2023-06-06 05:01:25.000000 hosgdSims-0.3.0/hosgdSims/__init__.py
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/hosgdSims/__pycache__/
--rw-r--r--   0 jaru      (1000) users      (100)     7961 2023-06-06 04:49:29.000000 hosgdSims-0.3.0/hosgdSims/__pycache__/HoSGDlabGD.cpython-39.pyc
--rw-r--r--   0 jaru      (1000) users      (100)      346 2023-06-06 04:49:29.000000 hosgdSims-0.3.0/hosgdSims/__pycache__/__init__.cpython-39.pyc
-drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/hosgdSims.egg-info/
--rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/PKG-INFO
--rw-r--r--   0 jaru      (1000) users      (100)      536 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/SOURCES.txt
--rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/dependency_links.txt
--rw-r--r--   0 jaru      (1000) users      (100)       45 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/requires.txt
--rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-06 05:08:27.000000 hosgdSims-0.3.0/hosgdSims.egg-info/top_level.txt
--rw-r--r--   0 jaru      (1000) users      (100)       23 2023-06-05 10:39:10.000000 hosgdSims-0.3.0/requirements.txt
--rw-r--r--   0 jaru      (1000) users      (100)       38 2023-06-06 05:08:27.714021 hosgdSims-0.3.0/setup.cfg
--rw-r--r--   0 jaru      (1000) users      (100)      913 2023-06-06 05:01:11.000000 hosgdSims-0.3.0/setup.py
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-09 05:47:52.569061 hosgdSims-0.5.0/
+-rw-------   0 jaru      (1000) users      (100)       62 2023-06-09 05:39:36.000000 hosgdSims-0.5.0/.setup.py.kate-swp
+-rw-r--r--   0 jaru      (1000) users      (100)       35 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/AUTHORS
+-rw-r--r--   0 jaru      (1000) users      (100)       11 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/MANIFEST.in
+-rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-09 05:47:52.569061 hosgdSims-0.5.0/PKG-INFO
+-rw-r--r--   0 jaru      (1000) users      (100)      477 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/README.md
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-09 05:47:52.569061 hosgdSims-0.5.0/hosgdSims/
+-rw-r--r--   0 jaru      (1000) users      (100)     2227 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDdefs.py
+-rw-r--r--   0 jaru      (1000) users      (100)      283 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDegAF.py
+-rw-r--r--   0 jaru      (1000) users      (100)     9091 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabAF.py
+-rw-r--r--   0 jaru      (1000) users      (100)     6400 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabAGD.py
+-rw-r--r--   0 jaru      (1000) users      (100)     9502 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabGD.py
+-rw-r--r--   0 jaru      (1000) users      (100)    14201 2023-06-07 14:26:53.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabHL.py
+-rw-r--r--   0 jaru      (1000) users      (100)     5560 2023-06-09 04:49:19.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabOwnTF.py
+-rw-r--r--   0 jaru      (1000) users      (100)     2069 2023-06-08 15:08:34.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabOwnTF_tex.py
+-rw-r--r--   0 jaru      (1000) users      (100)     8058 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabSGD.py
+-rw-r--r--   0 jaru      (1000) users      (100)     7151 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabSGDVariants.py
+-rw-r--r--   0 jaru      (1000) users      (100)     5670 2023-06-09 04:59:37.000000 hosgdSims-0.5.0/hosgdSims/HoSGDlabTF.py
+-rw-r--r--   0 jaru      (1000) users      (100)      150 2023-06-09 05:38:21.000000 hosgdSims-0.5.0/hosgdSims/__init__.py
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-09 05:47:52.569061 hosgdSims-0.5.0/hosgdSims/__pycache__/
+-rw-r--r--   0 jaru      (1000) users      (100)     7961 2023-06-06 04:49:29.000000 hosgdSims-0.5.0/hosgdSims/__pycache__/HoSGDlabGD.cpython-39.pyc
+-rw-r--r--   0 jaru      (1000) users      (100)     4214 2023-06-08 21:13:12.000000 hosgdSims-0.5.0/hosgdSims/__pycache__/HoSGDlabOwnTF.cpython-39.pyc
+-rw-r--r--   0 jaru      (1000) users      (100)     4492 2023-06-08 20:56:27.000000 hosgdSims-0.5.0/hosgdSims/__pycache__/HoSGDlabTF.cpython-39.pyc
+-rw-r--r--   0 jaru      (1000) users      (100)      346 2023-06-06 04:49:29.000000 hosgdSims-0.5.0/hosgdSims/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jaru      (1000) users      (100)        0 2023-06-09 05:47:52.569061 hosgdSims-0.5.0/hosgdSims.egg-info/
+-rw-r--r--   0 jaru      (1000) users      (100)      924 2023-06-09 05:47:52.000000 hosgdSims-0.5.0/hosgdSims.egg-info/PKG-INFO
+-rw-r--r--   0 jaru      (1000) users      (100)      736 2023-06-09 05:47:52.000000 hosgdSims-0.5.0/hosgdSims.egg-info/SOURCES.txt
+-rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-09 05:47:52.000000 hosgdSims-0.5.0/hosgdSims.egg-info/dependency_links.txt
+-rw-r--r--   0 jaru      (1000) users      (100)       45 2023-06-09 05:47:52.000000 hosgdSims-0.5.0/hosgdSims.egg-info/requires.txt
+-rw-r--r--   0 jaru      (1000) users      (100)        1 2023-06-09 05:47:52.000000 hosgdSims-0.5.0/hosgdSims.egg-info/top_level.txt
+-rw-r--r--   0 jaru      (1000) users      (100)       23 2023-06-05 10:39:10.000000 hosgdSims-0.5.0/requirements.txt
+-rw-r--r--   0 jaru      (1000) users      (100)       38 2023-06-09 05:47:52.569061 hosgdSims-0.5.0/setup.cfg
+-rw-r--r--   0 jaru      (1000) users      (100)      913 2023-06-09 05:38:38.000000 hosgdSims-0.5.0/setup.py
```

### Comparing `hosgdSims-0.3.0/PKG-INFO` & `hosgdSims-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosgdSims
-Version: 0.3.0
+Version: 0.5.0
 Summary: Hands on SGD
 Home-page: https://gitlab.com/prodrig/hosgdsims
 Author: Paul Rodriguez
 Author-email: prodrig@pucp.edu.pe
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDdefs.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDdefs.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDlabAF.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDlabAF.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDlabAGD.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDlabAGD.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDlabGD.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDlabGD.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDlabHL.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDlabHL.py`

 * *Files 4% similar despite different names*

```diff
@@ -364,15 +364,14 @@
 def hosgdSGDHLSover(OptProb, sgdVariant, nEpoch, blkSize):
 
     W = []
 
     OptProb.setShapes()
     for l in range(len(OptProb.HL)):
         W.append( OptProb.HL[l].randSol( OptProb.zShape[l] ) )
-        print('OptProb',l, W[l].shape)
 
     stats = np.zeros( [nEpoch, OptProb.Nstats] )
 
 
     nBlk = np.floor_divide(OptProb.X.shape[1],blkSize)
 
     if np.remainder(OptProb.X.shape[1],blkSize) > 0:
@@ -416,27 +415,14 @@
 
             # bw Pass
             g = OptProb.bwPass(W, y, l)
 
             # Update gradient
             W[l] = sgdVariant.update( W[l].copy(), g, e, l)
 
-            #if l == len(OptProb.HL)-1:
-                #g =  OptProb.HL[l].gradFun(W[l], OptProb.z[l], y)
-            #else:
-
-                #nabW = OptProb.HL[l].gradFun(W[l], OptProb.z[l], y)
-                #nabZ = OptProb.HL[l+1].gradFunZVar(W[l+1], OptProb.z[l+1], y)
-
-                #g = OptProb.HL[l].bwPass(nabW, nabZ, OptProb.z[l])
-
-
-            #if l <= len(OptProb.HL)-1:
-               #W[l] = bbSGD( W[l].copy(), g, alpha0, e, hyperFun)
-
 
       stats[e,:] = OptProb.computeStats(W, sgdVariant.alpha0, e, g)
       OptProb.printStats(e, nEpoch, stats)
 
 
     return W, stats
```

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDlabSGD.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDlabSGD.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims/HoSGDlabSGDVariants.py` & `hosgdSims-0.5.0/hosgdSims/HoSGDlabSGDVariants.py`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims/__pycache__/HoSGDlabGD.cpython-39.pyc` & `hosgdSims-0.5.0/hosgdSims/__pycache__/HoSGDlabGD.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `hosgdSims-0.3.0/hosgdSims.egg-info/PKG-INFO` & `hosgdSims-0.5.0/hosgdSims.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hosgdSims
-Version: 0.3.0
+Version: 0.5.0
 Summary: Hands on SGD
 Home-page: https://gitlab.com/prodrig/hosgdsims
 Author: Paul Rodriguez
 Author-email: prodrig@pucp.edu.pe
 License: GNU General Public License v3 or later (GPLv3+)
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hosgdSims-0.3.0/hosgdSims.egg-info/SOURCES.txt` & `hosgdSims-0.5.0/hosgdSims.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,27 @@
+.setup.py.kate-swp
 AUTHORS
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 hosgdSims/HoSGDdefs.py
 hosgdSims/HoSGDegAF.py
 hosgdSims/HoSGDlabAF.py
 hosgdSims/HoSGDlabAGD.py
 hosgdSims/HoSGDlabGD.py
 hosgdSims/HoSGDlabHL.py
+hosgdSims/HoSGDlabOwnTF.py
+hosgdSims/HoSGDlabOwnTF_tex.py
 hosgdSims/HoSGDlabSGD.py
 hosgdSims/HoSGDlabSGDVariants.py
+hosgdSims/HoSGDlabTF.py
 hosgdSims/__init__.py
 hosgdSims.egg-info/PKG-INFO
 hosgdSims.egg-info/SOURCES.txt
 hosgdSims.egg-info/dependency_links.txt
 hosgdSims.egg-info/requires.txt
 hosgdSims.egg-info/top_level.txt
 hosgdSims/__pycache__/HoSGDlabGD.cpython-39.pyc
+hosgdSims/__pycache__/HoSGDlabOwnTF.cpython-39.pyc
+hosgdSims/__pycache__/HoSGDlabTF.cpython-39.pyc
 hosgdSims/__pycache__/__init__.cpython-39.pyc
```

### Comparing `hosgdSims-0.3.0/setup.py` & `hosgdSims-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="hosgdSims",
-    version="0.3.0",
+    version="0.5.0",
     description="Hands on SGD",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/prodrig/hosgdsims",
     author="Paul Rodriguez",
     author_email="prodrig@pucp.edu.pe",
     license="GNU General Public License v3 or later (GPLv3+)",
```

