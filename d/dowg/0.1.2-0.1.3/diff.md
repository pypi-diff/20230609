# Comparing `tmp/dowg-0.1.2.tar.gz` & `tmp/dowg-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowg-0.1.2.tar", last modified: Thu Jun  8 16:19:58 2023, max compression
+gzip compressed data, was "dowg-0.1.3.tar", last modified: Thu Jun  8 16:26:52 2023, max compression
```

## Comparing `dowg-0.1.2.tar` & `dowg-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.261800 dowg-0.1.2/
--rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-08 16:19:58.260800 dowg-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.1.2/README.md
--rw-rw-rw-   0        0        0      552 2023-06-08 16:19:35.000000 dowg-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 16:19:58.261800 dowg-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.243799 dowg-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.250798 dowg-0.1.2/src/dowg/
--rw-rw-rw-   0        0        0     2037 2023-06-08 16:09:08.000000 dowg-0.1.2/src/dowg/CoordinateDoWG.py
--rw-rw-rw-   0        0        0     1914 2023-06-08 16:09:01.000000 dowg-0.1.2/src/dowg/ScalarDoWG.py
--rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.1.2/src/dowg/__init__.py
--rw-rw-rw-   0        0        0      844 2023-06-08 15:06:06.000000 dowg-0.1.2/src/dowg/clip.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.259800 dowg-0.1.2/src/dowg.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 16:26:52.997257 dowg-0.1.3/
+-rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-08 16:26:52.997257 dowg-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.1.3/README.md
+-rw-rw-rw-   0        0        0      552 2023-06-08 16:26:25.000000 dowg-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:26:52.998257 dowg-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 16:26:52.974258 dowg-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 16:26:52.986257 dowg-0.1.3/src/dowg/
+-rw-rw-rw-   0        0        0     2035 2023-06-08 16:26:29.000000 dowg-0.1.3/src/dowg/CoordinateDoWG.py
+-rw-rw-rw-   0        0        0     1912 2023-06-08 16:26:27.000000 dowg-0.1.3/src/dowg/ScalarDoWG.py
+-rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.1.3/src/dowg/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-06-08 15:06:06.000000 dowg-0.1.3/src/dowg/clip.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:26:52.996257 dowg-0.1.3/src/dowg.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-08 16:26:52.000000 dowg-0.1.3/src/dowg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-08 16:26:52.000000 dowg-0.1.3/src/dowg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:26:52.000000 dowg-0.1.3/src/dowg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-08 16:26:52.000000 dowg-0.1.3/src/dowg.egg-info/top_level.txt
```

### Comparing `dowg-0.1.2/LICENSE` & `dowg-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dowg-0.1.2/PKG-INFO` & `dowg-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.1.2
+Version: 0.1.3
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dowg-0.1.2/pyproject.toml` & `dowg-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dowg"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Patrick Shanahan", email="patrick.e.shanahan@gmail.com" },
 ]
 description = "DoWG parameter-free adaptive optimizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dowg-0.1.2/src/dowg/CoordinateDoWG.py` & `dowg-0.1.3/src/dowg/CoordinateDoWG.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             params (iterable): iterable of parameters to optimize or dicts defining
                 parameter groups
             eps (float, optional): term added to the denominator to improve
                 numerical stability (default: 1e-8)
         """
 
     def __init__(self, params, epsilon=1e-8, clip=0.5, *args, **kwargs):
-        defaults = dict(r_epsilon=epsilon, lr=1, clip=clip)
+        defaults = dict(epsilon=epsilon, lr=1, clip=clip)
         super(CoordinateDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (callable, optional): A closure that reevaluates the model
```

### Comparing `dowg-0.1.2/src/dowg/ScalarDoWG.py` & `dowg-0.1.3/src/dowg/ScalarDoWG.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import torch
 
 from .clip import clip_gradient
 
 
 class ScalarDoWG(torch.optim.Optimizer):
     def __init__(self, params, epsilon=1e-4, clip=0.5, *args, **kwargs):
-        defaults = dict(r_epsilon=epsilon, lr=1, clip=clip)
+        defaults = dict(epsilon=epsilon, lr=1, clip=clip)
         self.epsilon = epsilon
         super(ScalarDoWG, self).__init__(params, defaults)
 
     def step(self):
         state = self.state
 
         with torch.no_grad():
```

### Comparing `dowg-0.1.2/src/dowg/clip.py` & `dowg-0.1.3/src/dowg/clip.py`

 * *Files identical despite different names*

### Comparing `dowg-0.1.2/src/dowg.egg-info/PKG-INFO` & `dowg-0.1.3/src/dowg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.1.2
+Version: 0.1.3
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

