# Comparing `tmp/py3d-0.0.99.tar.gz` & `tmp/py3d-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.99.tar", last modified: Wed Jun  7 15:17:26 2023, max compression
+gzip compressed data, was "py3d-0.1.0.tar", last modified: Fri Jun  9 00:54:13 2023, max compression
```

## Comparing `py3d-0.0.99.tar` & `py3d-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:17:26.029535 py3d-0.0.99/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-07 15:17:26.029535 py3d-0.0.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-07 15:17:04.000000 py3d-0.0.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:17:26.029535 py3d-0.0.99/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-07 15:16:21.000000 py3d-0.0.99/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    28362 2023-06-07 15:16:21.000000 py3d-0.0.99/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-06-07 15:16:21.000000 py3d-0.0.99/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-07 15:17:26.029535 py3d-0.0.99/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1969 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-07 15:17:26.000000 py3d-0.0.99/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-07 15:17:26.029535 py3d-0.0.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-07 15:16:21.000000 py3d-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:54:13.035212 py3d-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-09 00:54:13.035212 py3d-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1578 2023-06-09 00:53:51.000000 py3d-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:54:13.035212 py3d-0.1.0/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-06-09 00:53:09.000000 py3d-0.1.0/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28585 2023-06-09 00:53:09.000000 py3d-0.1.0/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22638 2023-06-09 00:53:09.000000 py3d-0.1.0/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 00:54:13.035212 py3d-0.1.0/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1968 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-09 00:54:13.000000 py3d-0.1.0/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 00:54:13.035212 py3d-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-06-09 00:53:09.000000 py3d-0.1.0/setup.py
```

### Comparing `py3d-0.0.99/PKG-INFO` & `py3d-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.99
+Version: 0.1.0
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.99/README.md` & `py3d-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.99/py3d/core.py` & `py3d-0.1.0/py3d/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Tumiz.
 # Distributed under the terms of the GPL-3.0 License.
 from __future__ import annotations
 import numpy
 from IPython.display import display, HTML
-from typing import Dict, Union
+from typing import Dict
 import pathlib
 import uuid
 import json
 import struct
 
 pi = numpy.arccos(-1)
 __module__ = __import__(__name__)
@@ -222,35 +222,35 @@
         return self[..., 0:3].view(Vector3)
 
     @xyz.setter
     def xyz(self, v):
         self[..., 0:3] = v
 
     @property
-    def U(self) -> Union[Vector, Vector2, Vector3, Vector4]:
+    def U(self) -> Vector | Vector2 | Vector3 | Vector4:
         '''
         unit vector, direction vector
         '''
         n = self.L
         return numpy.divide(self, n, where=n != 0)
 
     @property
-    def H(self) -> Union[Vector, Vector2, Vector3, Vector4]:
+    def H(self) -> Vector | Vector2 | Vector3 | Vector4:
         '''
         Homogeneous vector
         '''
         ret = numpy.insert(self, self.shape[-1], 1, axis=self.ndim-1)
         w = ret.shape[-1]
         if w in [2, 3, 4]:
             return ret.view(getattr(__module__, f"Vector{w}"))
         else:
             return ret.view(Vector)
 
     @property
-    def M(self) -> Union[Vector, Vector2, Vector3, Vector4]:
+    def M(self) -> Vector | Vector2 | Vector3 | Vector4:
         # mean vector
         return super().mean(axis=self.ndim-2)
 
     @property
     def L(self) -> Vector:
         # length
         return numpy.linalg.norm(self, axis=self.ndim - 1, keepdims=True)
@@ -789,15 +789,22 @@
             ret[..., 0] = r
             ret[..., 1] = g
             ret[..., 2] = b
             ret[..., 3] = a
             return ret.view(cls)
 
     @classmethod
-    def map(cls, value, start, end):
+    def map(cls, value: list | numpy.ndarray, start=None, end=None):
+        '''
+        Create a series of colors by giving a a series of value
+        '''
+        if start is None:
+            start = numpy.min(value)
+        if end is None:
+            end = numpy.max(value)
         center = (start + end)/2
         width = (end - start)/2
         r = numpy.maximum(value - center, 0)/width
         g = 1-numpy.abs(value - center)/width
         b = numpy.maximum(center - value, 0)/width
         return cls(r=r, g=g, b=b)
```

### Comparing `py3d-0.0.99/py3d/viewer.html` & `py3d-0.1.0/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.0.99/py3d.egg-info/PKG-INFO` & `py3d-0.1.0/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.99
+Version: 0.1.0
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.99/setup.py` & `py3d-0.1.0/setup.py`

 * *Files identical despite different names*

