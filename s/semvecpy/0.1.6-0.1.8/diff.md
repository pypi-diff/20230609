# Comparing `tmp/semvecpy-0.1.6.tar.gz` & `tmp/semvecpy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/semvecpy-0.1.6.tar", last modified: Thu Sep  5 21:12:35 2019, max compression
+gzip compressed data, was "dist/semvecpy-0.1.8.tar", last modified: Mon Sep  9 17:43:14 2019, max compression
```

## Comparing `semvecpy-0.1.6.tar` & `semvecpy-0.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-05 21:12:35.000000 semvecpy-0.1.6/
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     1523 2019-06-18 01:38:09.000000 semvecpy-0.1.6/LICENSE.txt
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      127 2019-08-14 14:30:43.000000 semvecpy-0.1.6/MANIFEST.in
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     3929 2019-09-05 21:12:35.000000 semvecpy-0.1.6/PKG-INFO
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     2958 2019-08-14 15:30:14.000000 semvecpy-0.1.6/README.md
-drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy/
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)       48 2019-08-21 06:51:34.000000 semvecpy-0.1.6/semvecpy/__init__.py
-drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy/permutations/
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      116 2019-08-21 06:51:34.000000 semvecpy-0.1.6/semvecpy/permutations/__init__.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      252 2019-08-14 13:18:28.000000 semvecpy-0.1.6/semvecpy/permutations/constants.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     5194 2019-09-05 21:11:00.000000 semvecpy-0.1.6/semvecpy/permutations/dense_permutations.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     2202 2019-08-30 06:52:40.000000 semvecpy-0.1.6/semvecpy/permutations/sparse_permutations.py
-drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy/vectors/
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      138 2019-08-21 06:51:34.000000 semvecpy-0.1.6/semvecpy/vectors/__init__.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)    10062 2019-09-04 19:06:14.000000 semvecpy-0.1.6/semvecpy/vectors/binary_vectors.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     3819 2019-09-04 19:06:14.000000 semvecpy-0.1.6/semvecpy/vectors/graded_vectors.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)    11521 2019-08-21 06:51:34.000000 semvecpy-0.1.6/semvecpy/vectors/semvec_utils.py
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     2578 2019-09-04 19:06:14.000000 semvecpy-0.1.6/semvecpy/vectors/vector_utils.py
-drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy.egg-info/
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     3929 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy.egg-info/PKG-INFO
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      545 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy.egg-info/SOURCES.txt
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)        1 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy.egg-info/dependency_links.txt
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)       15 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy.egg-info/requires.txt
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)        9 2019-09-05 21:12:35.000000 semvecpy-0.1.6/semvecpy.egg-info/top_level.txt
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)       38 2019-09-05 21:12:35.000000 semvecpy-0.1.6/setup.cfg
--rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      740 2019-09-05 21:12:06.000000 semvecpy-0.1.6/setup.py
+drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-09 17:43:14.000000 semvecpy-0.1.8/
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     1523 2019-06-18 01:38:09.000000 semvecpy-0.1.8/LICENSE.txt
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      127 2019-08-14 14:30:43.000000 semvecpy-0.1.8/MANIFEST.in
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     4359 2019-09-09 17:43:14.000000 semvecpy-0.1.8/PKG-INFO
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     3331 2019-09-09 17:41:19.000000 semvecpy-0.1.8/README.md
+drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy/
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)       48 2019-08-21 06:51:34.000000 semvecpy-0.1.8/semvecpy/__init__.py
+drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy/permutations/
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      116 2019-08-21 06:51:34.000000 semvecpy-0.1.8/semvecpy/permutations/__init__.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      252 2019-08-14 13:18:28.000000 semvecpy-0.1.8/semvecpy/permutations/constants.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     5194 2019-09-05 21:11:00.000000 semvecpy-0.1.8/semvecpy/permutations/dense_permutations.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     2202 2019-08-30 06:52:40.000000 semvecpy-0.1.8/semvecpy/permutations/sparse_permutations.py
+drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy/vectors/
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      138 2019-08-21 06:51:34.000000 semvecpy-0.1.8/semvecpy/vectors/__init__.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)    10062 2019-09-04 19:06:14.000000 semvecpy-0.1.8/semvecpy/vectors/binary_vectors.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     3819 2019-09-04 19:06:14.000000 semvecpy-0.1.8/semvecpy/vectors/graded_vectors.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)    11521 2019-08-21 06:51:34.000000 semvecpy-0.1.8/semvecpy/vectors/semvec_utils.py
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     2578 2019-09-04 19:06:14.000000 semvecpy-0.1.8/semvecpy/vectors/vector_utils.py
+drwxr-xr-x   0 dominic.widdows   (503) dominic.widdows   (502)        0 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy.egg-info/
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)     4359 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy.egg-info/PKG-INFO
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      545 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy.egg-info/SOURCES.txt
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)        1 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy.egg-info/dependency_links.txt
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)       15 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy.egg-info/requires.txt
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)        9 2019-09-09 17:43:14.000000 semvecpy-0.1.8/semvecpy.egg-info/top_level.txt
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)       38 2019-09-09 17:43:14.000000 semvecpy-0.1.8/setup.cfg
+-rw-r--r--   0 dominic.widdows   (503) dominic.widdows   (502)      741 2019-09-09 17:42:52.000000 semvecpy-0.1.8/setup.py
```

### Comparing `semvecpy-0.1.6/LICENSE.txt` & `semvecpy-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/PKG-INFO` & `semvecpy-0.1.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: semvecpy
-Version: 0.1.6
+Version: 0.1.8
 Summary: Semantic Vectors work in Python
-Home-page: https://github.com/semanticvector/semvecpy
+Home-page: https://github.com/semanticvectors/semvecpy
 Author: Semantic Vectors Authors
 Author-email: semanticvectors@googlegroups.com
 License: UNKNOWN
 Description: # semvecpy 
         
         Semvecpy is a repository for Semantic Vectors work in Python (version 3 and above).
         
         It is a research project. It includes some well-tested production-grade work, but it's up to
         users to be aware of which parts this is.
         
         ## For External Users
         
         ### Installation
         
-        Clone the repository, or install using `pip install git+https://github.com/semanticvectors/semvecpy`.
-        TODO: It would be nice to make this just `pip install semvecpy`. See https://packaging.python.org/tutorials/packaging-projects/.
+        For the most recent released version, see run `pip install semvecpy`, which installs the most recent
+        deployed package from https://pypi.org/project/semvecpy/
+        
+        For development versions, `git clone` the repository, or install using `pip install git+https://github.com/semanticvectors/semvecpy`.
         
         ### Imports and Usage
         
         Import paths are designed to start with `semvecpy` in the hope that this will avoid name clashes from common terms such
         as `vectors`. So after installation, the following should work:
         
         ```
@@ -63,14 +65,19 @@
         
         To make things work together, code may be refactored. It's nice to discuss this with original 
         authors, but for small changes, developers with suitable permissions are encouraged to just
         go ahead. It follows that some changes may be unexpected to some authors. If 
         it's a bother just sync your repository wherever you left off, feel free to fork, and we can 
         discuss how to merge things back together later. Basically DON'T WORRY.
         
+        ### Release and Version Numbers
+        
+        Small "micro" updates are encouraged, typically using the `major.minor.micro` pattern as in https://www.python.org/dev/peps/pep-0440/#final-releases.
+        
+        We're using odd micro numbers for development versions (merged into github), and even numbers for released versions (in PyPi.)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `semvecpy-0.1.6/README.md` & `semvecpy-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 It is a research project. It includes some well-tested production-grade work, but it's up to
 users to be aware of which parts this is.
 
 ## For External Users
 
 ### Installation
 
-Clone the repository, or install using `pip install git+https://github.com/semanticvectors/semvecpy`.
-TODO: It would be nice to make this just `pip install semvecpy`. See https://packaging.python.org/tutorials/packaging-projects/.
+For the most recent released version, see run `pip install semvecpy`, which installs the most recent
+deployed package from https://pypi.org/project/semvecpy/
+
+For development versions, `git clone` the repository, or install using `pip install git+https://github.com/semanticvectors/semvecpy`.
 
 ### Imports and Usage
 
 Import paths are designed to start with `semvecpy` in the hope that this will avoid name clashes from common terms such
 as `vectors`. So after installation, the following should work:
 
 ```
@@ -55,7 +57,12 @@
 
 To make things work together, code may be refactored. It's nice to discuss this with original 
 authors, but for small changes, developers with suitable permissions are encouraged to just
 go ahead. It follows that some changes may be unexpected to some authors. If 
 it's a bother just sync your repository wherever you left off, feel free to fork, and we can 
 discuss how to merge things back together later. Basically DON'T WORRY.
 
+### Release and Version Numbers
+
+Small "micro" updates are encouraged, typically using the `major.minor.micro` pattern as in https://www.python.org/dev/peps/pep-0440/#final-releases.
+
+We're using odd micro numbers for development versions (merged into github), and even numbers for released versions (in PyPi.)
```

### Comparing `semvecpy-0.1.6/semvecpy/permutations/dense_permutations.py` & `semvecpy-0.1.8/semvecpy/permutations/dense_permutations.py`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/semvecpy/permutations/sparse_permutations.py` & `semvecpy-0.1.8/semvecpy/permutations/sparse_permutations.py`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/semvecpy/vectors/binary_vectors.py` & `semvecpy-0.1.8/semvecpy/vectors/binary_vectors.py`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/semvecpy/vectors/graded_vectors.py` & `semvecpy-0.1.8/semvecpy/vectors/graded_vectors.py`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/semvecpy/vectors/semvec_utils.py` & `semvecpy-0.1.8/semvecpy/vectors/semvec_utils.py`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/semvecpy/vectors/vector_utils.py` & `semvecpy-0.1.8/semvecpy/vectors/vector_utils.py`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/semvecpy.egg-info/PKG-INFO` & `semvecpy-0.1.8/semvecpy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: semvecpy
-Version: 0.1.6
+Version: 0.1.8
 Summary: Semantic Vectors work in Python
-Home-page: https://github.com/semanticvector/semvecpy
+Home-page: https://github.com/semanticvectors/semvecpy
 Author: Semantic Vectors Authors
 Author-email: semanticvectors@googlegroups.com
 License: UNKNOWN
 Description: # semvecpy 
         
         Semvecpy is a repository for Semantic Vectors work in Python (version 3 and above).
         
         It is a research project. It includes some well-tested production-grade work, but it's up to
         users to be aware of which parts this is.
         
         ## For External Users
         
         ### Installation
         
-        Clone the repository, or install using `pip install git+https://github.com/semanticvectors/semvecpy`.
-        TODO: It would be nice to make this just `pip install semvecpy`. See https://packaging.python.org/tutorials/packaging-projects/.
+        For the most recent released version, see run `pip install semvecpy`, which installs the most recent
+        deployed package from https://pypi.org/project/semvecpy/
+        
+        For development versions, `git clone` the repository, or install using `pip install git+https://github.com/semanticvectors/semvecpy`.
         
         ### Imports and Usage
         
         Import paths are designed to start with `semvecpy` in the hope that this will avoid name clashes from common terms such
         as `vectors`. So after installation, the following should work:
         
         ```
@@ -63,14 +65,19 @@
         
         To make things work together, code may be refactored. It's nice to discuss this with original 
         authors, but for small changes, developers with suitable permissions are encouraged to just
         go ahead. It follows that some changes may be unexpected to some authors. If 
         it's a bother just sync your repository wherever you left off, feel free to fork, and we can 
         discuss how to merge things back together later. Basically DON'T WORRY.
         
+        ### Release and Version Numbers
+        
+        Small "micro" updates are encouraged, typically using the `major.minor.micro` pattern as in https://www.python.org/dev/peps/pep-0440/#final-releases.
+        
+        We're using odd micro numbers for development versions (merged into github), and even numbers for released versions (in PyPi.)
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `semvecpy-0.1.6/semvecpy.egg-info/SOURCES.txt` & `semvecpy-0.1.8/semvecpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semvecpy-0.1.6/setup.py` & `semvecpy-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="semvecpy",
-    version="0.1.6",
+    version="0.1.8",
     author="Semantic Vectors Authors",
     author_email="semanticvectors@googlegroups.com",
     description="Semantic Vectors work in Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/semanticvector/semvecpy",
+    url="https://github.com/semanticvectors/semvecpy",
     packages=setuptools.find_packages(),
     python_requires=">=3",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
```

