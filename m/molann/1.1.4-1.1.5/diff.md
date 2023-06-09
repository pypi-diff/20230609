# Comparing `tmp/molann-1.1.4.tar.gz` & `tmp/molann-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molann-1.1.4.tar", last modified: Mon May 16 15:03:59 2022, max compression
+gzip compressed data, was "molann-1.1.5.tar", last modified: Fri Jun  9 12:10:46 2023, max compression
```

## Comparing `molann-1.1.4.tar` & `molann-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2022-05-16 15:03:59.709456 molann-1.1.4/
--rw-rw-r--   0 wei       (1000) wei       (1000)     1066 2022-05-10 07:32:41.000000 molann-1.1.4/LICENSE
--rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-05-10 07:32:41.000000 molann-1.1.4/MANIFEST.in
--rw-rw-r--   0 wei       (1000) wei       (1000)     2560 2022-05-16 15:03:59.709456 molann-1.1.4/PKG-INFO
--rwxrwxr-x   0 wei       (1000) wei       (1000)     2018 2022-05-10 07:32:41.000000 molann-1.1.4/README.rst
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2022-05-16 15:03:59.709456 molann-1.1.4/molann/
--rw-rw-r--   0 wei       (1000) wei       (1000)        1 2022-05-10 07:32:41.000000 molann-1.1.4/molann/__init__.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    22569 2022-05-16 12:53:56.000000 molann-1.1.4/molann/ann.py
--rw-rw-r--   0 wei       (1000) wei       (1000)    10185 2022-05-10 07:32:41.000000 molann-1.1.4/molann/feature.py
-drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2022-05-16 15:03:59.709456 molann-1.1.4/molann.egg-info/
--rw-rw-r--   0 wei       (1000) wei       (1000)     2560 2022-05-16 15:03:59.000000 molann-1.1.4/molann.egg-info/PKG-INFO
--rw-rw-r--   0 wei       (1000) wei       (1000)      264 2022-05-16 15:03:59.000000 molann-1.1.4/molann.egg-info/SOURCES.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        1 2022-05-16 15:03:59.000000 molann-1.1.4/molann.egg-info/dependency_links.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)       60 2022-05-16 15:03:59.000000 molann-1.1.4/molann.egg-info/requires.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)        7 2022-05-16 15:03:59.000000 molann-1.1.4/molann.egg-info/top_level.txt
--rw-rw-r--   0 wei       (1000) wei       (1000)      152 2022-05-10 07:32:41.000000 molann-1.1.4/pyproject.toml
--rw-rw-r--   0 wei       (1000) wei       (1000)      664 2022-05-16 15:03:59.709456 molann-1.1.4/setup.cfg
--rw-rw-r--   0 wei       (1000) wei       (1000)       93 2022-05-10 07:32:41.000000 molann-1.1.4/setup.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-09 12:10:46.655228 molann-1.1.5/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     1066 2022-05-10 07:32:41.000000 molann-1.1.5/LICENSE
+-rw-rw-r--   0 wei       (1000) wei       (1000)       15 2022-05-10 07:32:41.000000 molann-1.1.5/MANIFEST.in
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2523 2023-06-09 12:10:46.655228 molann-1.1.5/PKG-INFO
+-rwxrwxr-x   0 wei       (1000) wei       (1000)     2018 2022-05-10 07:32:41.000000 molann-1.1.5/README.rst
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-09 12:10:46.655228 molann-1.1.5/molann/
+-rw-rw-r--   0 wei       (1000) wei       (1000)        1 2022-05-10 07:32:41.000000 molann-1.1.5/molann/__init__.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    22514 2023-06-09 12:02:09.000000 molann-1.1.5/molann/ann.py
+-rw-rw-r--   0 wei       (1000) wei       (1000)    10185 2022-05-10 07:32:41.000000 molann-1.1.5/molann/feature.py
+drwxrwxr-x   0 wei       (1000) wei       (1000)        0 2023-06-09 12:10:46.655228 molann-1.1.5/molann.egg-info/
+-rw-rw-r--   0 wei       (1000) wei       (1000)     2523 2023-06-09 12:10:46.000000 molann-1.1.5/molann.egg-info/PKG-INFO
+-rw-rw-r--   0 wei       (1000) wei       (1000)      264 2023-06-09 12:10:46.000000 molann-1.1.5/molann.egg-info/SOURCES.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        1 2023-06-09 12:10:46.000000 molann-1.1.5/molann.egg-info/dependency_links.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)       60 2023-06-09 12:10:46.000000 molann-1.1.5/molann.egg-info/requires.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)        7 2023-06-09 12:10:46.000000 molann-1.1.5/molann.egg-info/top_level.txt
+-rw-rw-r--   0 wei       (1000) wei       (1000)      152 2022-05-10 07:32:41.000000 molann-1.1.5/pyproject.toml
+-rw-rw-r--   0 wei       (1000) wei       (1000)      664 2023-06-09 12:10:46.659227 molann-1.1.5/setup.cfg
+-rw-rw-r--   0 wei       (1000) wei       (1000)       93 2022-05-10 07:32:41.000000 molann-1.1.5/setup.py
```

### Comparing `molann-1.1.4/LICENSE` & `molann-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `molann-1.1.4/PKG-INFO` & `molann-1.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: molann
-Version: 1.1.4
+Version: 1.1.5
 Summary: "PyTorch Artificial Neural Networks (ANNs) for Molecular Systems",
 Home-page: https://github.com/zwpku/molann
 Author: Wei Zhang
 Author-email: wzhangpku@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/zwpku/molann/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -77,9 +75,7 @@
 Please refer to `MolANN docs`_.
 
 
 .. _`Installation`:
   https://molann.readthedocs.io/en/latest/installation.html
 .. _`MolANN docs`:
   https://molann.readthedocs.io/en/latest
-
-
```

### Comparing `molann-1.1.4/README.rst` & `molann-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `molann-1.1.4/molann/ann.py` & `molann-1.1.5/molann/ann.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,18 +428,15 @@
 
     def get_feature_info(self):
         r"""display information of features 
 
         Returns:
             :external+pandas:class:`pandas.DataFrame`, information of features
         """
-        df = pd.DataFrame()
-        for f in self.feature_list:
-            df = df.append(f.get_feature_info(), ignore_index=True)
-        return df
+        return pd.concat([f.get_feature_info() for f in self.feature_list], ignore_index=True)
 
     def get_feature(self, idx):
         r"""
         Args: 
             idx (int): index of feature in feature list
         Returns:
              :class:`molann.feature.Feature`, the feature in the feature list
```

### Comparing `molann-1.1.4/molann/feature.py` & `molann-1.1.5/molann/feature.py`

 * *Files identical despite different names*

### Comparing `molann-1.1.4/molann.egg-info/PKG-INFO` & `molann-1.1.5/molann.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: molann
-Version: 1.1.4
+Version: 1.1.5
 Summary: "PyTorch Artificial Neural Networks (ANNs) for Molecular Systems",
 Home-page: https://github.com/zwpku/molann
 Author: Wei Zhang
 Author-email: wzhangpku@gmail.com
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/zwpku/molann/issues
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
@@ -77,9 +75,7 @@
 Please refer to `MolANN docs`_.
 
 
 .. _`Installation`:
   https://molann.readthedocs.io/en/latest/installation.html
 .. _`MolANN docs`:
   https://molann.readthedocs.io/en/latest
-
-
```

### Comparing `molann-1.1.4/setup.cfg` & `molann-1.1.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = molann
-version = 1.1.4
+version = 1.1.5
 author = Wei Zhang
 author_email = wzhangpku@gmail.com
 description = "PyTorch Artificial Neural Networks (ANNs) for Molecular Systems",
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/zwpku/molann
 project_urls =
```

