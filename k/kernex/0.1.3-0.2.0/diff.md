# Comparing `tmp/kernex-0.1.3.tar.gz` & `tmp/kernex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kernex-0.1.3.tar", last modified: Thu Mar  2 12:29:18 2023, max compression
+gzip compressed data, was "kernex-0.2.0.tar", last modified: Fri Jun  9 21:12:01 2023, max compression
```

## Comparing `kernex-0.1.3.tar` & `kernex-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-02 12:29:04.000000 kernex-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-02 12:29:04.000000 kernex-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-03-02 12:29:18.607639 kernex-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14245 2023-03-02 12:29:04.000000 kernex-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.603639 kernex-0.1.3/kernex/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/kernex/_src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/_src/map.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/_src/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    10223 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/_src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/kernex/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/interface/kernel_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     5715 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/interface/named_axis.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-03-02 12:29:04.000000 kernex-0.1.3/kernex/interface/resolve_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/kernex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15107 2023-03-02 12:29:18.000000 kernex-0.1.3/kernex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-03-02 12:29:18.000000 kernex-0.1.3/kernex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:29:18.000000 kernex-0.1.3/kernex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 12:29:18.000000 kernex-0.1.3/kernex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-02 12:29:18.000000 kernex-0.1.3/kernex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-02 12:29:18.000000 kernex-0.1.3/kernex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-02 12:29:04.000000 kernex-0.1.3/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 12:29:18.607639 kernex-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-03-02 12:29:04.000000 kernex-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:04.000000 kernex-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8727 2023-03-02 12:29:04.000000 kernex-0.1.3/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    26081 2023-03-02 12:29:04.000000 kernex-0.1.3/tests/test_scan_and_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-03-02 12:29:04.000000 kernex-0.1.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:18.607639 kernex-0.1.3/tests_and_benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 12:29:04.000000 kernex-0.1.3/tests_and_benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-03-02 12:29:04.000000 kernex-0.1.3/tests_and_benchmarks/test_benchmark_conv2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-02 12:29:04.000000 kernex-0.1.3/tests_and_benchmarks/test_benchmark_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.724773 kernex-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-09 21:11:52.000000 kernex-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-09 21:11:52.000000 kernex-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-06-09 21:12:01.724773 kernex-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14054 2023-06-09 21:11:52.000000 kernex-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/kernex/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/kernex/_src/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/_src/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/_src/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11488 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/_src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/kernex/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18165 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/interface/kernel_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6262 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/interface/named_axis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-09 21:11:52.000000 kernex-0.2.0/kernex/interface/resolve_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/kernex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14916 2023-06-09 21:12:01.000000 kernex-0.2.0/kernex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-09 21:12:01.000000 kernex-0.2.0/kernex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:12:01.000000 kernex-0.2.0/kernex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:12:01.000000 kernex-0.2.0/kernex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-09 21:12:01.000000 kernex-0.2.0/kernex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 21:12:01.000000 kernex-0.2.0/kernex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-09 21:11:52.000000 kernex-0.2.0/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:12:01.724773 kernex-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-09 21:11:52.000000 kernex-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 21:11:52.000000 kernex-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-09 21:11:52.000000 kernex-0.2.0/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26117 2023-06-09 21:11:52.000000 kernex-0.2.0/tests/test_scan_and_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-06-09 21:11:52.000000 kernex-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:12:01.720773 kernex-0.2.0/tests_and_benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 21:11:52.000000 kernex-0.2.0/tests_and_benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-09 21:11:52.000000 kernex-0.2.0/tests_and_benchmarks/test_benchmark_conv2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-06-09 21:11:52.000000 kernex-0.2.0/tests_and_benchmarks/test_benchmark_patch.py
```

### Comparing `kernex-0.1.3/LICENSE` & `kernex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kernex-0.1.3/PKG-INFO` & `kernex-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kernex
-Version: 0.1.3
+Version: 0.2.0
 Summary: Stencil computations in JAX.
 Home-page: https://github.com/ASEM000/kernex
 Author: Mahmoud Asem
 Author-email: asem00@kaist.ac.kr
 License: MIT
 Keywords: python machine-learning pytorch jax
 Classifier: Development Status :: 5 - Production/Stable
@@ -20,27 +20,26 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <div align = "center">
 <img  width=400 src="assets/kernexlogo.svg" align="center">
 
-
 <h3 align="center">Differentiable Stencil computations in JAX </h2>
 
 [**Installation**](#Installation)
 |[**Description**](#Description)
 |[**Quick example**](#QuickExample)
 |[**Function mesh**](#FunctionMesh)
 |[**More Examples**](#MoreExamples)
 |[**Benchmarking**](#Benchmarking)
 
 ![Tests](https://github.com/ASEM000/kernex/actions/workflows/tests.yml/badge.svg)
-![pyver](https://img.shields.io/badge/python-3.7%203.8%203.9%203.10-red)
-![codestyle](https://img.shields.io/badge/codestyle-black-lightgrey)
+![pyver](https://img.shields.io/badge/python-3.8%203.8%203.9%203.11-red)
+![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Downloads](https://pepy.tech/badge/kernex)](https://pepy.tech/project/kernex)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14UEqKzIyZsDzQ9IMeanvztXxbbbatTYV?usp=sharing)
 [![codecov](https://codecov.io/gh/ASEM000/kernex/branch/main/graph/badge.svg?token=3KLL24Z94I)](https://codecov.io/gh/ASEM000/kernex)
 [![DOI](https://zenodo.org/badge/512400616.svg)](https://zenodo.org/badge/latestdoi/512400616)
 
 </div>
 
@@ -48,56 +47,58 @@
 
 ```python
 pip install kernex
 ```
 
 ## 📖 Description<a id="Description"></a>
 
-Kernex extends `jax.vmap` and `jax.lax.scan` with `kmap` and `kscan` for general stencil computations.
+Kernex extends `jax.vmap`/`jax.lax.map`/`jax.pmap` with `kmap` and `jax.lax.scan` with `kscan` for general stencil computations.
 
 The prime motivation for this package is to blend the solution process of PDEs into a NN setting.
 
 ## ⏩ Quick Example <a id="QuickExample">
 
 <div align="center">
 <table>
 <tr>
 <td width="50%" align="center" > kmap </td> <td align="center" > kscan </td>
 </tr>
 <tr>
 <td>
 
 ```python
-import kernex as kex 
-import jax.numpy as jnp 
+
+import kernex as kex
+import jax.numpy as jnp
 
 @kex.kmap(kernel_size=(3,))
 def sum_all(x):
     return jnp.sum(x)
 
 >>> x = jnp.array([1,2,3,4,5])
 >>> print(sum_all(x))
 [ 6  9 12]
 ```
+
 </td>
 <td>
     
 ```python
 import kernex as kex 
-import jax.numpy as jnp 
+import jax.numpy as jnp
 
 @kex.kscan(kernel_size=(3,))
 def sum_all(x):
-    return jnp.sum(x)
+return jnp.sum(x)
 
->>> x = jnp.array([1,2,3,4,5])
->>> print(sum_all(x))
-[ 6 13 22]
+> > > x = jnp.array([1,2,3,4,5])
+> > > print(sum_all(x))
+> > > [ 6 13 22]
 
-```
+````
 </td>
 </tr>
 </table>
 
 <table>
 <tr>
 <td width="50%">
@@ -120,14 +121,15 @@
 
 The objective is to apply `f(x) = x^2  at index=0  and f(x) = x^3 at  index=(1,10)`
 
 To achieve the following operation with `jax.lax.switch` , we need a list of 10 functions correspoing to each cell of the example array.
 For this reason , kernex adopts a modified version of `jax.lax.switch` to reduce the number of branches required.
 
 ```python
+
 # function applies x^2 at boundaries, and applies x^3 to to the interior
 
         ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
   f =   │ x^2 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │
         └─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┘
 
         ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
@@ -179,14 +181,15 @@
 
 ```
 
 </td>
 <td>
 
 ```python
+
 def F(x):
     f1 = lambda x:x**2
     f2 = lambda x:x**3
     x = x.at[0].set(f1(x[0]))
     x = x.at[1:].set(f2(x[1:]))
     return x
 
@@ -209,31 +212,32 @@
 
 </div>
 
 </details>
 
 ## 🔢 More examples<a id="MoreExamples"></a>
 
-
 <details>
 <summary>1️⃣ Convolution operation</summary>
 
 ```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @jax.jit
 @kex.kmap(
     kernel_size= (3,3,3),
     padding = ('valid','same','same'))
 def kernex_conv2d(x,w):
-    # JAX channel first conv2d with 3x3x3 kernel_size 
+    # JAX channel first conv2d with 3x3x3 kernel_size
     return jnp.sum(x*w)
-````
+```
+
 </details>
 
 <details>
 <summary>2️⃣ Laplacian operation</summary>
 
 ```python
 # see also
@@ -266,14 +270,15 @@
 ```
 
 </details>
 
 <details><summary>3️⃣ Get Patches of an array</summary>
 
 ```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @kex.kmap(kernel_size=(3,3),relative=True)
 def identity(x):
     # similar to numba.stencil
@@ -330,15 +335,14 @@
 <img src="assets/linear_convection_view.png" width="500px">
 
 </td>
 </tr>
 </table>
 </div>
 
-
 ```python
 
 import jax
 import jax.numpy as jnp
 import kernex as kex
 import matplotlib.pyplot as plt
 
@@ -393,67 +397,64 @@
     plt.plot(jnp.linspace(0,xmax,nx),line)
 ```
 
 ![image](assets/linear_convection.svg)
 
 </details>
 
-    
 <details><summary>5️⃣ Gaussian blur</summary>
 
 ```python
-    
-import jax 
+
+import jax
 import jax.numpy as jnp
 import kernex as kex
 
 def gaussian_blur(image, sigma, kernel_size):
     x = jnp.linspace(-(kernel_size - 1) / 2.0, (kernel_size- 1) / 2.0, kernel_size)
     w = jnp.exp(-0.5 * jnp.square(x) * jax.lax.rsqrt(sigma))
     w = jnp.outer(w, w)
     w = w / w.sum()
 
     @kex.kmap(kernel_size=(kernel_size, kernel_size), padding="same")
     def conv(x):
-        return jnp.sum(x * w)    
-    
+        return jnp.sum(x * w)
+
     return conv(image)
-    
-    
+
+
 ```
-    
-</details>
 
+</details>
 
 <details > <summary>6️⃣ Depthwise convolution </summary>
      
-```python     
+```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @jax.jit
 @jax.vmap
 @kex.kmap(
-    kernel_size= (3,3),
-    padding = ('same','same'))
-def kernex_depthwise_conv2d(x,w):
-    # Channel-first depthwise convolution
-    # jax.debug.print("x=\n{a}\nw=\n{b} \n\n",a=x, b=w)
-    return jnp.sum(x*w)
-
+kernel_size= (3,3),
+padding = ('same','same'))
+def kernex_depthwise_conv2d(x,w): # Channel-first depthwise convolution # jax.debug.print("x=\n{a}\nw=\n{b} \n\n",a=x, b=w)
+return jnp.sum(x\*w)
 
 h,w,c = 5,5,2
 k=3
 
 x = jnp.arange(1,h*w*c+1).reshape(c,h,w)
 w = jnp.arange(1,k*k*c+1).reshape(c,k,k)
 print(kernex_depthwise_conv2d(x,w))</summary>
-```    
-        
+
+````
+
 </details>
 
 <details> <summary>7️⃣ Maxpooling2D and Averagepooling2D </summary>
 
 ```python
 @jax.vmap # vectorize over the channel dimension
 @kex.kmap(kernel_size=(3,3), strides=(2,2))
@@ -462,85 +463,69 @@
     return jnp.max(x)
 
 @jax.vmap # vectorize over the channel dimension
 @kex.kmap(kernel_size=(3,3), strides=(2,2))
 def avgpool_2d(x):
     # define the kernel for the Average pool operation over the spatial dimensions
     return jnp.mean(x)
-```
-
+````
 
 </details>
 
-
-
-## ⌛ Benchmarking<a id="Benchmarking"></a>
-
-<details><summary>Conv2D</summary>
+<details><summary>8️⃣ Runge-Kutta integration</summary>
 
 ```python
-# testing and benchmarking convolution
-# for complete benchmarking check /tests_and_benchmark
-
-# 3x1024x1024 Input
-C,H = 3,1024
 
-@jax.jit
-def jax_conv2d(x,w):
-    return jax.lax.conv_general_dilated(
-        lhs = x,
-        rhs = w,
-        window_strides = (1,1),
-        padding = 'SAME',
-        dimension_numbers = ('NCHW', 'OIHW', 'NCHW'),)[0]
-
-
-x = jax.random.normal(jax.random.PRNGKey(0),(C,H,H))
-xx = x[None]
-w = jax.random.normal(jax.random.PRNGKey(0),(C,3,3))
-ww = w[None]
-
-# assert equal
-np.testing.assert_allclose(kernex_conv2d(x,w),jax_conv2d(xx,ww),atol=1e-3)
+# lets solve dydt = y, where y0 = 1 and y(t)=e^t
+# using Runge-Kutta 4th order method
+# f(t,y) = y
+import jax.numpy as jnp
+import matplotlib.pyplot as plt
+import kernex as kex
 
-# Mac M1 CPU
-# check tests_and_benchmark folder for more.
 
-%timeit kernex_conv2d(x,w).block_until_ready()
-# 3.96 ms ± 272 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+t = jnp.linspace(0, 1, 5)
+y = jnp.zeros(5)
+x = jnp.stack([y, t], axis=0)
+dt = t[1] - t[0]  # 0.1
+f = lambda tn, yn: yn
+
+
+def ic(x):
+    """ initial condition y0 = 1 """
+    return 1.
+
+
+def rk4(x):
+    """ runge kutta 4th order integration step """
+    # ┌────┬────┬────┐      ┌──────┬──────┬──────┐
+    # │ y0 │*y1*│ y2 │      │[0,-1]│[0, 0]│[0, 1]│
+    # ├────┼────┼────┤ ==>  ├──────┼──────┼──────┤
+    # │ t0 │ t1 │ t2 │      │[1,-1]│[1, 0]│[1, 1]│
+    # └────┴────┴────┘      └──────┴──────┴──────┘
+    t0 = x[1, -1]
+    y0 = x[0, -1]
+    k1 = dt * f(t0, y0)
+    k2 = dt * f(t0 + dt / 2, y0 + 1 / 2 * k1)
+    k3 = dt * f(t0 + dt / 2, y0 + 1 / 2 * k2)
+    k4 = dt * f(t0 + dt, y0 + k3)
+    yn_1 = y0 + 1 / 6 * (k1 + 2 * k2 + 2 * k3 + k4)
+    return yn_1
+
+
+F = kex.kscan(kernel_size=(2, 3), relative=True, padding=((0, 1)))  # kernel size = 3
+
+F[0:1, 1:] = rk4
+F[0, 0] = ic
+# compile the solver
+solver = jax.jit(F.__call__)
+y = solver(x)[0, :]
+
+plt.plot(t, y, '-o', label='rk4')
+plt.plot(t, jnp.exp(t), '-o', label='analytical')
+plt.legend()
 
-%timeit jax_conv2d(xx,ww).block_until_ready()
-# 27.5 ms ± 993 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ```
 
-</details>
-
-<details><summary>get_patches</summary>
-
-```python
-# benchmarking `get_patches` with `jax.lax.conv_general_dilated_patches`
-# On Mac M1 CPU
-
-@jax.jit
-@kex.kmap(kernel_size=(3,),padding='same')
-def get_patches(x):
-    return x
-
-@jax.jit
-def jax_get_patches(x):
-    return jax.lax.conv_general_dilated_patches(x,(3,),(1,),padding='same')
-
-x = jnp.ones([1_000_000])
-xx = jnp.ones([1,1,1_000_000])
-
-np.testing.assert_allclose(
-    get_patches(x),
-    jax_get_patches(xx).reshape(-1,1_000_000).T)
-
->> %timeit get_patches(x).block_until_ready()
->> %timeit jax_get_patches(xx).block_until_ready()
-
-1.73 ms ± 92.7 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
-10.6 ms ± 337 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
-```
+![img](assets/rk4.svg)
 
 </details>
```

### Comparing `kernex-0.1.3/README.md` & `kernex-0.2.0/kernex.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,45 @@
+Metadata-Version: 2.1
+Name: kernex
+Version: 0.2.0
+Summary: Stencil computations in JAX.
+Home-page: https://github.com/ASEM000/kernex
+Author: Mahmoud Asem
+Author-email: asem00@kaist.ac.kr
+License: MIT
+Keywords: python machine-learning pytorch jax
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align = "center">
 <img  width=400 src="assets/kernexlogo.svg" align="center">
 
-
 <h3 align="center">Differentiable Stencil computations in JAX </h2>
 
 [**Installation**](#Installation)
 |[**Description**](#Description)
 |[**Quick example**](#QuickExample)
 |[**Function mesh**](#FunctionMesh)
 |[**More Examples**](#MoreExamples)
 |[**Benchmarking**](#Benchmarking)
 
 ![Tests](https://github.com/ASEM000/kernex/actions/workflows/tests.yml/badge.svg)
-![pyver](https://img.shields.io/badge/python-3.7%203.8%203.9%203.10-red)
-![codestyle](https://img.shields.io/badge/codestyle-black-lightgrey)
+![pyver](https://img.shields.io/badge/python-3.8%203.8%203.9%203.11-red)
+![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Downloads](https://pepy.tech/badge/kernex)](https://pepy.tech/project/kernex)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14UEqKzIyZsDzQ9IMeanvztXxbbbatTYV?usp=sharing)
 [![codecov](https://codecov.io/gh/ASEM000/kernex/branch/main/graph/badge.svg?token=3KLL24Z94I)](https://codecov.io/gh/ASEM000/kernex)
 [![DOI](https://zenodo.org/badge/512400616.svg)](https://zenodo.org/badge/latestdoi/512400616)
 
 </div>
 
@@ -25,56 +47,58 @@
 
 ```python
 pip install kernex
 ```
 
 ## 📖 Description<a id="Description"></a>
 
-Kernex extends `jax.vmap` and `jax.lax.scan` with `kmap` and `kscan` for general stencil computations.
+Kernex extends `jax.vmap`/`jax.lax.map`/`jax.pmap` with `kmap` and `jax.lax.scan` with `kscan` for general stencil computations.
 
 The prime motivation for this package is to blend the solution process of PDEs into a NN setting.
 
 ## ⏩ Quick Example <a id="QuickExample">
 
 <div align="center">
 <table>
 <tr>
 <td width="50%" align="center" > kmap </td> <td align="center" > kscan </td>
 </tr>
 <tr>
 <td>
 
 ```python
-import kernex as kex 
-import jax.numpy as jnp 
+
+import kernex as kex
+import jax.numpy as jnp
 
 @kex.kmap(kernel_size=(3,))
 def sum_all(x):
     return jnp.sum(x)
 
 >>> x = jnp.array([1,2,3,4,5])
 >>> print(sum_all(x))
 [ 6  9 12]
 ```
+
 </td>
 <td>
     
 ```python
 import kernex as kex 
-import jax.numpy as jnp 
+import jax.numpy as jnp
 
 @kex.kscan(kernel_size=(3,))
 def sum_all(x):
-    return jnp.sum(x)
+return jnp.sum(x)
 
->>> x = jnp.array([1,2,3,4,5])
->>> print(sum_all(x))
-[ 6 13 22]
+> > > x = jnp.array([1,2,3,4,5])
+> > > print(sum_all(x))
+> > > [ 6 13 22]
 
-```
+````
 </td>
 </tr>
 </table>
 
 <table>
 <tr>
 <td width="50%">
@@ -97,14 +121,15 @@
 
 The objective is to apply `f(x) = x^2  at index=0  and f(x) = x^3 at  index=(1,10)`
 
 To achieve the following operation with `jax.lax.switch` , we need a list of 10 functions correspoing to each cell of the example array.
 For this reason , kernex adopts a modified version of `jax.lax.switch` to reduce the number of branches required.
 
 ```python
+
 # function applies x^2 at boundaries, and applies x^3 to to the interior
 
         ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
   f =   │ x^2 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │
         └─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┘
 
         ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
@@ -156,14 +181,15 @@
 
 ```
 
 </td>
 <td>
 
 ```python
+
 def F(x):
     f1 = lambda x:x**2
     f2 = lambda x:x**3
     x = x.at[0].set(f1(x[0]))
     x = x.at[1:].set(f2(x[1:]))
     return x
 
@@ -186,31 +212,32 @@
 
 </div>
 
 </details>
 
 ## 🔢 More examples<a id="MoreExamples"></a>
 
-
 <details>
 <summary>1️⃣ Convolution operation</summary>
 
 ```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @jax.jit
 @kex.kmap(
     kernel_size= (3,3,3),
     padding = ('valid','same','same'))
 def kernex_conv2d(x,w):
-    # JAX channel first conv2d with 3x3x3 kernel_size 
+    # JAX channel first conv2d with 3x3x3 kernel_size
     return jnp.sum(x*w)
-````
+```
+
 </details>
 
 <details>
 <summary>2️⃣ Laplacian operation</summary>
 
 ```python
 # see also
@@ -243,14 +270,15 @@
 ```
 
 </details>
 
 <details><summary>3️⃣ Get Patches of an array</summary>
 
 ```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @kex.kmap(kernel_size=(3,3),relative=True)
 def identity(x):
     # similar to numba.stencil
@@ -307,15 +335,14 @@
 <img src="assets/linear_convection_view.png" width="500px">
 
 </td>
 </tr>
 </table>
 </div>
 
-
 ```python
 
 import jax
 import jax.numpy as jnp
 import kernex as kex
 import matplotlib.pyplot as plt
 
@@ -370,67 +397,64 @@
     plt.plot(jnp.linspace(0,xmax,nx),line)
 ```
 
 ![image](assets/linear_convection.svg)
 
 </details>
 
-    
 <details><summary>5️⃣ Gaussian blur</summary>
 
 ```python
-    
-import jax 
+
+import jax
 import jax.numpy as jnp
 import kernex as kex
 
 def gaussian_blur(image, sigma, kernel_size):
     x = jnp.linspace(-(kernel_size - 1) / 2.0, (kernel_size- 1) / 2.0, kernel_size)
     w = jnp.exp(-0.5 * jnp.square(x) * jax.lax.rsqrt(sigma))
     w = jnp.outer(w, w)
     w = w / w.sum()
 
     @kex.kmap(kernel_size=(kernel_size, kernel_size), padding="same")
     def conv(x):
-        return jnp.sum(x * w)    
-    
+        return jnp.sum(x * w)
+
     return conv(image)
-    
-    
+
+
 ```
-    
-</details>
 
+</details>
 
 <details > <summary>6️⃣ Depthwise convolution </summary>
      
-```python     
+```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @jax.jit
 @jax.vmap
 @kex.kmap(
-    kernel_size= (3,3),
-    padding = ('same','same'))
-def kernex_depthwise_conv2d(x,w):
-    # Channel-first depthwise convolution
-    # jax.debug.print("x=\n{a}\nw=\n{b} \n\n",a=x, b=w)
-    return jnp.sum(x*w)
-
+kernel_size= (3,3),
+padding = ('same','same'))
+def kernex_depthwise_conv2d(x,w): # Channel-first depthwise convolution # jax.debug.print("x=\n{a}\nw=\n{b} \n\n",a=x, b=w)
+return jnp.sum(x\*w)
 
 h,w,c = 5,5,2
 k=3
 
 x = jnp.arange(1,h*w*c+1).reshape(c,h,w)
 w = jnp.arange(1,k*k*c+1).reshape(c,k,k)
 print(kernex_depthwise_conv2d(x,w))</summary>
-```    
-        
+
+````
+
 </details>
 
 <details> <summary>7️⃣ Maxpooling2D and Averagepooling2D </summary>
 
 ```python
 @jax.vmap # vectorize over the channel dimension
 @kex.kmap(kernel_size=(3,3), strides=(2,2))
@@ -439,85 +463,69 @@
     return jnp.max(x)
 
 @jax.vmap # vectorize over the channel dimension
 @kex.kmap(kernel_size=(3,3), strides=(2,2))
 def avgpool_2d(x):
     # define the kernel for the Average pool operation over the spatial dimensions
     return jnp.mean(x)
-```
-
+````
 
 </details>
 
-
-
-## ⌛ Benchmarking<a id="Benchmarking"></a>
-
-<details><summary>Conv2D</summary>
+<details><summary>8️⃣ Runge-Kutta integration</summary>
 
 ```python
-# testing and benchmarking convolution
-# for complete benchmarking check /tests_and_benchmark
-
-# 3x1024x1024 Input
-C,H = 3,1024
 
-@jax.jit
-def jax_conv2d(x,w):
-    return jax.lax.conv_general_dilated(
-        lhs = x,
-        rhs = w,
-        window_strides = (1,1),
-        padding = 'SAME',
-        dimension_numbers = ('NCHW', 'OIHW', 'NCHW'),)[0]
-
-
-x = jax.random.normal(jax.random.PRNGKey(0),(C,H,H))
-xx = x[None]
-w = jax.random.normal(jax.random.PRNGKey(0),(C,3,3))
-ww = w[None]
-
-# assert equal
-np.testing.assert_allclose(kernex_conv2d(x,w),jax_conv2d(xx,ww),atol=1e-3)
+# lets solve dydt = y, where y0 = 1 and y(t)=e^t
+# using Runge-Kutta 4th order method
+# f(t,y) = y
+import jax.numpy as jnp
+import matplotlib.pyplot as plt
+import kernex as kex
 
-# Mac M1 CPU
-# check tests_and_benchmark folder for more.
 
-%timeit kernex_conv2d(x,w).block_until_ready()
-# 3.96 ms ± 272 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+t = jnp.linspace(0, 1, 5)
+y = jnp.zeros(5)
+x = jnp.stack([y, t], axis=0)
+dt = t[1] - t[0]  # 0.1
+f = lambda tn, yn: yn
+
+
+def ic(x):
+    """ initial condition y0 = 1 """
+    return 1.
+
+
+def rk4(x):
+    """ runge kutta 4th order integration step """
+    # ┌────┬────┬────┐      ┌──────┬──────┬──────┐
+    # │ y0 │*y1*│ y2 │      │[0,-1]│[0, 0]│[0, 1]│
+    # ├────┼────┼────┤ ==>  ├──────┼──────┼──────┤
+    # │ t0 │ t1 │ t2 │      │[1,-1]│[1, 0]│[1, 1]│
+    # └────┴────┴────┘      └──────┴──────┴──────┘
+    t0 = x[1, -1]
+    y0 = x[0, -1]
+    k1 = dt * f(t0, y0)
+    k2 = dt * f(t0 + dt / 2, y0 + 1 / 2 * k1)
+    k3 = dt * f(t0 + dt / 2, y0 + 1 / 2 * k2)
+    k4 = dt * f(t0 + dt, y0 + k3)
+    yn_1 = y0 + 1 / 6 * (k1 + 2 * k2 + 2 * k3 + k4)
+    return yn_1
+
+
+F = kex.kscan(kernel_size=(2, 3), relative=True, padding=((0, 1)))  # kernel size = 3
+
+F[0:1, 1:] = rk4
+F[0, 0] = ic
+# compile the solver
+solver = jax.jit(F.__call__)
+y = solver(x)[0, :]
+
+plt.plot(t, y, '-o', label='rk4')
+plt.plot(t, jnp.exp(t), '-o', label='analytical')
+plt.legend()
 
-%timeit jax_conv2d(xx,ww).block_until_ready()
-# 27.5 ms ± 993 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ```
 
-</details>
-
-<details><summary>get_patches</summary>
-
-```python
-# benchmarking `get_patches` with `jax.lax.conv_general_dilated_patches`
-# On Mac M1 CPU
-
-@jax.jit
-@kex.kmap(kernel_size=(3,),padding='same')
-def get_patches(x):
-    return x
-
-@jax.jit
-def jax_get_patches(x):
-    return jax.lax.conv_general_dilated_patches(x,(3,),(1,),padding='same')
-
-x = jnp.ones([1_000_000])
-xx = jnp.ones([1,1,1_000_000])
-
-np.testing.assert_allclose(
-    get_patches(x),
-    jax_get_patches(xx).reshape(-1,1_000_000).T)
-
->> %timeit get_patches(x).block_until_ready()
->> %timeit jax_get_patches(xx).block_until_ready()
-
-1.73 ms ± 92.7 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
-10.6 ms ± 337 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
-```
+![img](assets/rk4.svg)
 
 </details>
```

### Comparing `kernex-0.1.3/kernex/_src/utils.py` & `kernex-0.2.0/kernex/_src/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,38 @@
-# [credits] Mahmoud Asem@CVBML KAIST May 2022
-
+# Copyright 2023 Kernex authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from __future__ import annotations
 
 import functools as ft
+from typing import Sequence
 
 import jax
 import jax.numpy as jnp
-
-
-def ZIP(*args):
-    """assert all args have the same number of elements before zipping"""
-    n = len(args[0])
-    msg = f"zip arguments dont have the same length. Args length = {tuple(len(arg) for arg in args)}"
-    assert all(len(x) == n for x in args[1:]), msg
-    return zip(*args)
+import numpy as np
+from jax import lax
+from jax.util import safe_zip
+
+transform_func_map = {
+    "vmap": jax.vmap,
+    "lmap": lambda func, **k: (lambda xs: jax.lax.map(func, xs, **k)),
+    "pmap": jax.pmap,
+    "scan": jax.lax.scan,
+}
 
 
 def _calculate_pad_width(border: tuple[tuple[int, int], ...]):
     """Calcuate the positive padding from border value
 
     Returns:
         padding value passed to `pad_width` in `jnp.pad`
@@ -26,144 +40,176 @@
     # this function is cached because it is called multiple times
     # and it is expensive to calculate
     # if the border is negative, the padding is 0
     # if the border is positive, the padding is the border value
     return tuple([0, max(0, pi[0]) + max(0, pi[1])] for pi in border)
 
 
-def _get_index_from_view(view, kernel_size) -> tuple[int, ...]:
+def _get_index_from_view(
+    view: jax.Array,
+    kernel_size: tuple[tuple[int, int], ...],
+) -> tuple[int, ...]:
     """Get the index of array from the view
 
     Args:
-        view (tuple[jnp.ndarray,...]): patch indices for each dimension
+        view (tuple[jax.Array,...]): patch indices for each dimension
 
     Returns:
         tuple[int, ...]: index as a tuple of int for each dimension
     """
-
     return tuple(
         view[i][wi // 2] if wi % 2 == 1 else view[i][(wi - 1) // 2]
         for i, wi in enumerate(kernel_size)
     )
 
 
-@ft.partial(jax.jit, static_argnums=(0, 1, 2, 3))
-def _generate_views(shape, kernel_size, strides, border) -> tuple[jnp.ndarray, ...]:
+def _generate_views(
+    shape: tuple[int, ...],
+    kernel_size: tuple[int, ...],
+    strides: tuple[int, ...],
+    border: tuple[tuple[int, int], ...],
+) -> tuple[jax.Array, ...]:
     """Generate absolute sampling matrix"""
     # this function is cached because it is called multiple times
     # and it is expensive to calculate
     # the view is the indices of the array that is used to calculate
     # the output value
     dim_range = tuple(
         general_arange(di, ki, si, x0, xf)
         for (di, ki, si, (x0, xf)) in zip(shape, kernel_size, strides, border)
     )
     matrix = general_product(*dim_range)
     return tuple(map(lambda xi, wi: xi.reshape(-1, wi), matrix, kernel_size))
 
 
-def _calculate_output_shape(shape, kernel_size, strides, border) -> tuple[int, ...]:
+def _calculate_output_shape(
+    shape: tuple[int, ...],
+    kernel_size: tuple[int, ...],
+    strides: tuple[int, ...],
+    border: tuple[tuple[int, int], ...],
+) -> tuple[int, ...]:
     """Calculate the output shape of the kernel operation from
     the input shape, kernel size, stride and border.
 
     Returns:
         tuple[int, ...]: resulting shape of the kernel operation
     """
     # this function is cached because it is called multiple times
     # and it is expensive to calculate
     # the output shape is the shape of the array after the kernel operation
     # is applied to the input array
     return tuple(
         (xi + (li + ri) - ki) // si + 1
-        for xi, ki, si, (li, ri) in ZIP(shape, kernel_size, strides, border)
+        for xi, ki, si, (li, ri) in safe_zip(shape, kernel_size, strides, border)
     )
 
 
-def _offset_to_padding(input_argument, kernel_size):
+@ft.lru_cache(maxsize=128)
+def _offset_to_padding(input_argument, kernel_size: tuple[int, ...]):
     """convert offset argument to negative border values"""
     # for example for a kernel_size = (3,3) and offset = (1,1)
     # the padding will be (-1,-1) for each dimension
     padding = [[]] * len(kernel_size)
 
     # offset = 1 ==> padding= 0 for kernel_size =3
     same = lambda wi: ((wi - 1) // 2, wi // 2)
 
     for i, item in enumerate(input_argument):
 
         zero_offset_padding = same(kernel_size[i])
 
         if isinstance(item, tuple):
-            assert item >= (0, 0, ), f"offset must be non negative value.Found offset={item}"  # fmt: skip
-            padding[i] = tuple(ai - bi for ai, bi in ZIP(zero_offset_padding, item))
+            if item < (0, 0):
+                raise ValueError(f"Negative value found, offset={item}")
+            padding[i] = tuple(
+                ai - bi for ai, bi in safe_zip(zero_offset_padding, item)
+            )
 
         elif isinstance(item, int):
-            assert item >= 0, f"offset must be non negative value.Found offset={item}"
-            padding[i] = tuple(ai - bi for ai, bi in ZIP(zero_offset_padding, (item, item)))  # fmt: skip
+            if item < 0:
+                raise ValueError(f"Negative value found, offset={item}")
+            padding[i] = tuple(
+                ai - bi for ai, bi in safe_zip(zero_offset_padding, (item, item))
+            )
 
     # [TODO] throw an error if offset value is larger than kernel_size
     return tuple(padding)
 
 
+def roll(a: jax.Array, shift: Sequence[int], axis: Sequence[int]) -> jax.Array:
+    # https://github.com/jakevdp/jax/blob/5497bb03b6c353853b2ef6536e954898214736c8/jax/_src/numpy/lax_numpy.py
+    for ax, s in zip(*np.broadcast_arrays(axis, shift)):
+        if a.shape[ax] == 0:
+            continue
+        i = (-s) % a.shape[ax]
+        a = lax.concatenate(
+            [
+                lax.slice_in_dim(a, i, a.shape[ax], axis=ax),
+                lax.slice_in_dim(a, 0, i, axis=ax),
+            ],
+            dimension=ax,
+        )
+    return a
+
+
 @ft.partial(jax.profiler.annotate_function, name="roll_view")
-def roll_view(array: jnp.ndarray) -> jnp.ndarray:
+def roll_view(array: jax.Array) -> jax.Array:
     """Roll view along all axes
 
     Example:
     >>> x = jnp.arange(1,26).reshape(5,5)
     >>> print(roll_view(x))
         [[13 14 15 11 12]
         [18 19 20 16 17]
         [23 24 25 21 22]
         [ 3  4  5  1  2]
         [ 8  9 10  6  7]]
     """
     # this function is used to roll the view along all axes
     shape = jnp.array(array.shape)
     axes = tuple(range(len(shape)))  # list all axes
-    shift = tuple(
-        -(si // 2) if si % 2 == 1 else -((si - 1) // 2) for si in array.shape
-    )  # right padding>left padding
-    return jnp.roll(array, shift=shift, axis=axes)
+    # right padding>left padding
+    shift = tuple(-(si // 2) if si % 2 == 1 else -((si - 1) // 2) for si in array.shape)
+    return roll(array, shift=shift, axis=axes)
 
 
 def ix_(*args):
     """modified version of jnp.ix_"""
     n = len(args)
     output = []
     for i, a in enumerate(args):
         shape = [1] * n
         shape[i] = a.shape[0]
         output.append(jax.lax.broadcast_in_dim(a, shape, (i,)))
     return tuple(output)
 
 
-@ft.partial(jax.jit, static_argnums=(0, 1, 2))
 def _get_set_indices(shape, strides, offset):
     # the indices of the array that are set by the kernel operation
     # this is used to set the values of the array after the kernel operation
     # is applied
     return tuple(
-        jnp.arange(x0, di - xf, si) for di, si, (x0, xf) in ZIP(shape, strides, offset)
+        jnp.arange(x0, di - xf, si)
+        for di, si, (x0, xf) in safe_zip(shape, strides, offset)
     )
 
 
 @ft.partial(jax.profiler.annotate_function, name="general_arange")
-@ft.partial(jax.jit, static_argnums=(0, 1, 2, 3, 4))
-def general_arange(di: int, ki: int, si: int, x0: int, xf: int) -> jnp.ndarray:
+def general_arange(di: int, ki: int, si: int, x0: int, xf: int) -> jax.Array:
     """Calculate the windows indices for a given dimension.
 
     Args:
         di (int): shape of the dimension
         ki (int): kernel size
         si (int): stride
         x0 (int): left padding
         xf (int): rght padding
 
     Returns:
-        jnp.ndarray: array of windows indices
+        jax.Array: array of windows indices
 
     Example:
         >>> di = 5
         >>> ki = 3
         >>> si = 1
         >>> x0 = 0
         >>> xf = 0
@@ -171,24 +217,42 @@
             [[0 1 2]
             [1 2 3]
             [2 3 4]]
     """
     # this function is used to calculate the windows indices for a given dimension
     start, end = -x0 + ((ki - 1) // 2), di + xf - (ki // 2)
     size = end - start
-    lhs = jax.lax.broadcasted_iota(dtype=jnp.int32, shape=(size, ki), dimension=0) + (start)  # fmt: skip
-    rhs = jax.lax.broadcasted_iota(dtype=jnp.int32, shape=(ki, size), dimension=0).T - ((ki - 1) // 2)  # fmt: skip
-    res = lhs + rhs
+
+    res = (
+        lax.broadcasted_iota(dtype=jnp.int32, shape=(size, ki), dimension=0)
+        + lax.broadcasted_iota(dtype=jnp.int32, shape=(ki, size), dimension=0).T
+        + (start)
+        - ((ki - 1) // 2)
+    )
 
     # res[::si] is slightly slower.
     return (res) if si == 1 else (res)[::si]
 
 
+@ft.lru_cache(maxsize=128)
+def recursive_vmap(*, ndim: int):
+    def nvmap(n):
+        in_axes = [None] * ndim
+        in_axes[-n] = 0
+        return (
+            jax.vmap(lambda *x: x, in_axes=in_axes)
+            if n == 1
+            else jax.vmap(nvmap(n - 1), in_axes=in_axes)
+        )
+
+    return nvmap(ndim)
+
+
 @ft.partial(jax.profiler.annotate_function, name="general_product")
-def general_product(*args):
+def general_product(*args: jax.Array):
     """Equivalent to tuple(zip(*itertools.product(*args)))` for arrays
 
     Example:
     >>> general_product(
     ... jnp.array([[1,2],[3,4]]),
     ... jnp.array([[5,6],[7,8]]))
     (
@@ -200,63 +264,53 @@
     >>> tuple(zip(*(itertools.product([[1,2],[3,4]],[[5,6],[7,8]]))))
     (
         ([1, 2], [1, 2], [3, 4], [3, 4]),
         ([5, 6], [7, 8], [5, 6], [7, 8])
     )
 
     """
-
-    def nvmap(n):
-        in_axes = [None] * len(args)
-        in_axes[-n] = 0
-        return (
-            jax.vmap(lambda *x: x, in_axes=in_axes)
-            if n == 1
-            else jax.vmap(nvmap(n - 1), in_axes=in_axes)
-        )
-
-    return nvmap(len(args))(*args)
+    return recursive_vmap(ndim=len(args))(*args)
 
 
-@ft.partial(jax.jit, static_argnums=(0, 1))
 def _index_from_view(
-    view: tuple[jnp.ndarray, ...], kernel_size: tuple[int, ...]
+    view: tuple[jax.Array, ...],
+    kernel_size: tuple[int, ...],
 ) -> tuple[int, ...]:
     """Get the index of array from the view
 
     Args:
-        view (tuple[jnp.ndarray,...]): patch indices for each dimension
+        view (tuple[jax.Array,...]): patch indices for each dimension
         kernel_size (tuple[int,...]): kernel size for each dimension
 
     Returns:
         tuple[int, ...]: index as a tuple of int for each dimension
     """
     return tuple(
         view[i][wi // 2] if wi % 2 == 1 else view[i][(wi - 1) // 2]
         for i, wi in enumerate(kernel_size)
     )
 
 
-def _compare_key(x: tuple[jnp.ndarray, ...], y: tuple[jnp.ndarray, ...]) -> bool:
+def _compare_key(x: tuple[jax.Array, ...], y: tuple[jax.Array, ...]) -> bool:
     """check if index as array x is in the range of index as array y for all dimensions
 
     Args:
-        x (jnp.ndarray): lhs index
-        y (jnp.ndarray): rhs index
+        x (jax.Array): lhs index
+        y (jax.Array): rhs index
 
     Returns:
         bool: if x in range(y) or x == y
     """
 
-    def _compare_key_item(xi: jnp.ndarray, yi: jnp.ndarray) -> bool:
+    def _compare_key_item(xi: jax.Array, yi: jax.Array) -> bool:
         """check if index as array xi is in the range of index as array yi for single dimension
 
         Args:
-            xi (jnp.ndarray): lhs index
-            yi (jnp.ndarray): rhs index
+            xi (jax.Array): lhs index
+            yi (jax.Array): rhs index
 
         Returns:
             bool: if xi in range(yi) or xi == yi
         """
         # index style = (start,end,step)
         if yi.size == 3:
             return (yi[0] <= xi) * (xi < yi[1]) * (xi % yi[2] == 0)
@@ -268,23 +322,22 @@
         # index style = (index)
         if yi.size == 1:
             return jnp.where(yi == jnp.inf, True, xi == yi)
 
     return jnp.all(jnp.array([_compare_key_item(xi, yi) for (xi, yi) in zip(x, y)]))
 
 
-@jax.jit
-def _key_search(key: tuple[jnp.ndarray, ...], keys: tuple[jnp.ndarray]) -> int:
+def _key_search(key: tuple[jax.Array, ...], keys: tuple[jax.Array]) -> int:
     """returns the index of the key in the keys array if key is within the key range or equal to it.
 
     Args:
-        key (tuple[jnp.ndarray,...]):
+        key (tuple[jax.Array,...]):
             a tuple of jnp.arrays for each dimension ( {dim0},...,{dimN}) with size({dim}) == 1
 
-        keys (tuple[jnp.ndarray):
+        keys (tuple[jax.Array):
             a tuple of jnp.arrays for range of each dimension
             ( {dim0},...,{dimN}) with size({dim})with size ({dim}) in [1,2,3]
 
     Returns:
         int: index of the key in the keys array
     """
```

### Comparing `kernex-0.1.3/kernex/interface/named_axis.py` & `kernex-0.2.0/kernex/interface/named_axis.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,67 @@
-"""
-[credits] Mahmoud Asem@CVBML KAIST May 2022
-"""
+# Copyright 2023 Kernex authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
 
 from __future__ import annotations
 
 import copy
-import functools
+import functools as ft
 from itertools import product
 from typing import Callable
 
-import jax.numpy as jnp
+import jax
 
 
-class sortedDict(dict):
+class SortedDict(dict):
     """a class that sort a key before setting or getting an item"""
 
     # this dict is used to store the kernel values
     # the key is a tuple of the axis names
     # the value is the kernel values
     # for example if the kernel is 3x3 and the axis names are ['x', 'y']
     # the key will be ('x', 'y') and the value will be the kernel values
     def __getitem__(self, key: tuple[str, ...]):
         key = (key,) if isinstance(key, str) else tuple(sorted(key))
         return super().__getitem__(key)
 
-    def __setitem__(self, key: tuple[str, ...], val: jnp.ndarray):
+    def __setitem__(self, key: tuple[str, ...], val: jax.Array):
         key = (key,) if isinstance(key, str) else tuple(sorted(key))
         super().__setitem__(key, val)
 
 
 def generate_named_axis(
-    kernel_size: tuple[int, ...], named_axis: dict[int, str], relative: bool = True
+    kernel_size: tuple[int, ...],
+    named_axis: dict[int, str],
+    relative: bool = True,
 ) -> dict[str, tuple[int, ...]]:
     """Return a dict that maps named axis to their integer value indices
 
     Args:
         kernel_size (tuple[int, ...]): kernel_size
         named_axis (dict[int, str]): axis argnum and its corresponding name
         relative (bool, optional): relative indexing boolean. Defaults to True.
 
     Raises:
         ValueError: Not int/str in named_axis
 
     Returns:
         dict[str, tuple[int, ...]]:
             [1] fully named axes (len(keys)==len(kernel_size ))
-            return sortedDict object , where keys order is insignificant ( A['a','b']==A['b','a'])
+            return SortedDict object , where keys order is insignificant ( A['a','b']==A['b','a'])
 
             [2] partially named axes (len(keys)<len(kernel_size s))
             return dictionary object where key order matters.
 
     Examples:
         ### fully named axes case (inordered keys) :
         >>> generate_named_axis(named_axis={0:'b',1:'a'} , kernel_size =(2,3),relative=True)
@@ -76,15 +88,16 @@
             ('b+1', 0)  : (1, 0),
             ('b+1', 1)  : (1, 1),
             ('b+1', 2)  : (1, 2),
             ('b+2', 0)  : (2, 0),
             ('b+2', 1)  : (2, 1),
             ('b+2', 2)  : (2, 2)}
     """
-    # helper function to return range of sliding kernel_size  for a given dimension
+    # helper function to return range of sliding kernel_size  
+    # for a given dimension
     def range_func(wi):
         if relative:
             return tuple(range(-((wi - 1) // 2), (wi) // 2 + 1))
 
         else:
             return tuple(range(wi))
 
@@ -104,15 +117,16 @@
 
     keys = [[]] * len(kernel_size)
     vals = [[]] * len(kernel_size)
 
     # iterate over key,val in named_axis dict
     for dim, val in default_named_axis.items():
         if isinstance(val, str):
-            # get keys for each dimension : [ ['i-m' ,..,'i+m'] , ['j-n',...,'j+n'] , .. ]
+            # get keys for each dimension : [ ['i-m' ,..,'i+m'] , 
+            # ['j-n',...,'j+n'] , .. ]
             # single charater case for each dimensoon
             # example {0:'i'}
             # index is incremented and decremented
             keys[dim] = [
                 f"{val}{operator_func(idx)}" for idx in range_func(kernel_size[dim])
             ]
             vals[dim] = range_func(kernel_size[dim])
@@ -129,17 +143,18 @@
 
         else:
             raise ValueError("Wrong format for named_axis.")
 
     keys = product(*keys)
 
     # reserve order if the named_axis are partially passed , otherwise its not order
-    return_dict = dict() if partial_naming else sortedDict()
+    return_dict = dict() if partial_naming else SortedDict()
 
-    # multiply [-m,...,m ] x [-n,...n] = [(-m,n) (-m,n-1) , .. ] to get the mesh integer indices
+    # multiply [-m,...,m ] x [-n,...n] = [(-m,n) (-m,n-1) , .. ] to get 
+    # the mesh integer indices
     vals = product(*vals)
 
     for k, v in zip(keys, vals):
         return_dict[k] = v
 
     # print(return_dict,type(return_dict))
     return return_dict
@@ -147,16 +162,16 @@
 
 def named_axis_wrapper(kernel_size, named_axis):
 
     named_axis_dict = generate_named_axis(kernel_size, named_axis)
     x = copy.copy(named_axis_dict)
 
     def call(func: Callable):
-        @functools.wraps(func)
-        def inner(X: jnp.ndarray, *args, **kwargs):
+        @ft.wraps(func)
+        def inner(X: jax.Array, *args, **kwargs):
             # switch the input of the function to operate on dictionary
             for k, idx in named_axis_dict.items():
                 # assign the literal character keys to array numeric values
                 x[k] = X[idx]
             return func(x, *args, **kwargs)
 
         return inner
```

### Comparing `kernex-0.1.3/kernex/interface/resolve_utils.py` & `kernex-0.2.0/kernex/interface/resolve_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,29 @@
+# Copyright 2023 Kernex authors
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#     https://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 from __future__ import annotations
 
 import functools as ft
 from typing import Any, Callable
 
-import jax.numpy as jnp
+import jax
 import jax.tree_util as jtu
-
-from kernex._src.utils import ZIP
-
-# ---------------------- resolve_arguments ------------------------ #
+from jax.util import safe_zip
 
 
 def _resolve_padding_argument(
     input_argument: tuple[int | tuple[int, int] | str, ...] | int | str,
     kernel_size: tuple[int, ...],
 ):
     """Helper function to generate padding"""
@@ -139,16 +150,16 @@
     for i, (item, in_dim) in enumerate(zip(index, shape)):
         resolved_index[i] = _resolve_single_index(item, in_dim)
 
     return resolved_index
 
 
 def _normalize_slices(
-    container: dict[Callable, jnp.ndarray], in_dim: tuple[int, ...]
-) -> dict[Callable, jnp.ndarray]:
+    container: dict[Callable, jax.Array], in_dim: tuple[int, ...]
+) -> dict[Callable, jax.Array]:
     """Convert slice with partial range to tuple with determined range"""
 
     for func, slices in container.items():
         slices = [_resolve_index(index, in_dim) for index in slices]
         container[func] = slices
     return container
 
@@ -167,15 +178,15 @@
         msg += f"Found len({arg }) != len{(in_dim)}"
         assert len(arg) == len(in_dim), msg
 
         msg = f"{kw} shape must be less than array shape.\n"
         msg += f"Found {kw}  = {arg } array shape = {in_dim} "
         assert all(ai <= si for (ai, si) in zip(arg, in_dim)), msg
 
-        return tuple(si if wi == -1 else wi for si, wi in ZIP(in_dim, arg))
+        return tuple(si if wi == -1 else wi for si, wi in safe_zip(in_dim, arg))
 
     if isinstance(arg, int):
         return (in_dim if arg == -1 else arg) * len(in_dim)
 
     raise ValueError(f"{kw}  must be instance of int or tuple. Found {type(arg)}")
```

### Comparing `kernex-0.1.3/kernex.egg-info/PKG-INFO` & `kernex-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,22 @@
-Metadata-Version: 2.1
-Name: kernex
-Version: 0.1.3
-Summary: Stencil computations in JAX.
-Home-page: https://github.com/ASEM000/kernex
-Author: Mahmoud Asem
-Author-email: asem00@kaist.ac.kr
-License: MIT
-Keywords: python machine-learning pytorch jax
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <div align = "center">
 <img  width=400 src="assets/kernexlogo.svg" align="center">
 
-
 <h3 align="center">Differentiable Stencil computations in JAX </h2>
 
 [**Installation**](#Installation)
 |[**Description**](#Description)
 |[**Quick example**](#QuickExample)
 |[**Function mesh**](#FunctionMesh)
 |[**More Examples**](#MoreExamples)
 |[**Benchmarking**](#Benchmarking)
 
 ![Tests](https://github.com/ASEM000/kernex/actions/workflows/tests.yml/badge.svg)
-![pyver](https://img.shields.io/badge/python-3.7%203.8%203.9%203.10-red)
-![codestyle](https://img.shields.io/badge/codestyle-black-lightgrey)
+![pyver](https://img.shields.io/badge/python-3.8%203.8%203.9%203.11-red)
+![codestyle](https://img.shields.io/badge/codestyle-black-black)
 [![Downloads](https://pepy.tech/badge/kernex)](https://pepy.tech/project/kernex)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/14UEqKzIyZsDzQ9IMeanvztXxbbbatTYV?usp=sharing)
 [![codecov](https://codecov.io/gh/ASEM000/kernex/branch/main/graph/badge.svg?token=3KLL24Z94I)](https://codecov.io/gh/ASEM000/kernex)
 [![DOI](https://zenodo.org/badge/512400616.svg)](https://zenodo.org/badge/latestdoi/512400616)
 
 </div>
 
@@ -48,56 +24,58 @@
 
 ```python
 pip install kernex
 ```
 
 ## 📖 Description<a id="Description"></a>
 
-Kernex extends `jax.vmap` and `jax.lax.scan` with `kmap` and `kscan` for general stencil computations.
+Kernex extends `jax.vmap`/`jax.lax.map`/`jax.pmap` with `kmap` and `jax.lax.scan` with `kscan` for general stencil computations.
 
 The prime motivation for this package is to blend the solution process of PDEs into a NN setting.
 
 ## ⏩ Quick Example <a id="QuickExample">
 
 <div align="center">
 <table>
 <tr>
 <td width="50%" align="center" > kmap </td> <td align="center" > kscan </td>
 </tr>
 <tr>
 <td>
 
 ```python
-import kernex as kex 
-import jax.numpy as jnp 
+
+import kernex as kex
+import jax.numpy as jnp
 
 @kex.kmap(kernel_size=(3,))
 def sum_all(x):
     return jnp.sum(x)
 
 >>> x = jnp.array([1,2,3,4,5])
 >>> print(sum_all(x))
 [ 6  9 12]
 ```
+
 </td>
 <td>
     
 ```python
 import kernex as kex 
-import jax.numpy as jnp 
+import jax.numpy as jnp
 
 @kex.kscan(kernel_size=(3,))
 def sum_all(x):
-    return jnp.sum(x)
+return jnp.sum(x)
 
->>> x = jnp.array([1,2,3,4,5])
->>> print(sum_all(x))
-[ 6 13 22]
+> > > x = jnp.array([1,2,3,4,5])
+> > > print(sum_all(x))
+> > > [ 6 13 22]
 
-```
+````
 </td>
 </tr>
 </table>
 
 <table>
 <tr>
 <td width="50%">
@@ -120,14 +98,15 @@
 
 The objective is to apply `f(x) = x^2  at index=0  and f(x) = x^3 at  index=(1,10)`
 
 To achieve the following operation with `jax.lax.switch` , we need a list of 10 functions correspoing to each cell of the example array.
 For this reason , kernex adopts a modified version of `jax.lax.switch` to reduce the number of branches required.
 
 ```python
+
 # function applies x^2 at boundaries, and applies x^3 to to the interior
 
         ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
   f =   │ x^2 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │ x^3 │
         └─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┘
 
         ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
@@ -179,14 +158,15 @@
 
 ```
 
 </td>
 <td>
 
 ```python
+
 def F(x):
     f1 = lambda x:x**2
     f2 = lambda x:x**3
     x = x.at[0].set(f1(x[0]))
     x = x.at[1:].set(f2(x[1:]))
     return x
 
@@ -209,31 +189,32 @@
 
 </div>
 
 </details>
 
 ## 🔢 More examples<a id="MoreExamples"></a>
 
-
 <details>
 <summary>1️⃣ Convolution operation</summary>
 
 ```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @jax.jit
 @kex.kmap(
     kernel_size= (3,3,3),
     padding = ('valid','same','same'))
 def kernex_conv2d(x,w):
-    # JAX channel first conv2d with 3x3x3 kernel_size 
+    # JAX channel first conv2d with 3x3x3 kernel_size
     return jnp.sum(x*w)
-````
+```
+
 </details>
 
 <details>
 <summary>2️⃣ Laplacian operation</summary>
 
 ```python
 # see also
@@ -266,14 +247,15 @@
 ```
 
 </details>
 
 <details><summary>3️⃣ Get Patches of an array</summary>
 
 ```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @kex.kmap(kernel_size=(3,3),relative=True)
 def identity(x):
     # similar to numba.stencil
@@ -330,15 +312,14 @@
 <img src="assets/linear_convection_view.png" width="500px">
 
 </td>
 </tr>
 </table>
 </div>
 
-
 ```python
 
 import jax
 import jax.numpy as jnp
 import kernex as kex
 import matplotlib.pyplot as plt
 
@@ -393,67 +374,64 @@
     plt.plot(jnp.linspace(0,xmax,nx),line)
 ```
 
 ![image](assets/linear_convection.svg)
 
 </details>
 
-    
 <details><summary>5️⃣ Gaussian blur</summary>
 
 ```python
-    
-import jax 
+
+import jax
 import jax.numpy as jnp
 import kernex as kex
 
 def gaussian_blur(image, sigma, kernel_size):
     x = jnp.linspace(-(kernel_size - 1) / 2.0, (kernel_size- 1) / 2.0, kernel_size)
     w = jnp.exp(-0.5 * jnp.square(x) * jax.lax.rsqrt(sigma))
     w = jnp.outer(w, w)
     w = w / w.sum()
 
     @kex.kmap(kernel_size=(kernel_size, kernel_size), padding="same")
     def conv(x):
-        return jnp.sum(x * w)    
-    
+        return jnp.sum(x * w)
+
     return conv(image)
-    
-    
+
+
 ```
-    
-</details>
 
+</details>
 
 <details > <summary>6️⃣ Depthwise convolution </summary>
      
-```python     
+```python
+
 import jax
 import jax.numpy as jnp
 import kernex as kex
 
 @jax.jit
 @jax.vmap
 @kex.kmap(
-    kernel_size= (3,3),
-    padding = ('same','same'))
-def kernex_depthwise_conv2d(x,w):
-    # Channel-first depthwise convolution
-    # jax.debug.print("x=\n{a}\nw=\n{b} \n\n",a=x, b=w)
-    return jnp.sum(x*w)
-
+kernel_size= (3,3),
+padding = ('same','same'))
+def kernex_depthwise_conv2d(x,w): # Channel-first depthwise convolution # jax.debug.print("x=\n{a}\nw=\n{b} \n\n",a=x, b=w)
+return jnp.sum(x\*w)
 
 h,w,c = 5,5,2
 k=3
 
 x = jnp.arange(1,h*w*c+1).reshape(c,h,w)
 w = jnp.arange(1,k*k*c+1).reshape(c,k,k)
 print(kernex_depthwise_conv2d(x,w))</summary>
-```    
-        
+
+````
+
 </details>
 
 <details> <summary>7️⃣ Maxpooling2D and Averagepooling2D </summary>
 
 ```python
 @jax.vmap # vectorize over the channel dimension
 @kex.kmap(kernel_size=(3,3), strides=(2,2))
@@ -462,85 +440,69 @@
     return jnp.max(x)
 
 @jax.vmap # vectorize over the channel dimension
 @kex.kmap(kernel_size=(3,3), strides=(2,2))
 def avgpool_2d(x):
     # define the kernel for the Average pool operation over the spatial dimensions
     return jnp.mean(x)
-```
-
+````
 
 </details>
 
-
-
-## ⌛ Benchmarking<a id="Benchmarking"></a>
-
-<details><summary>Conv2D</summary>
+<details><summary>8️⃣ Runge-Kutta integration</summary>
 
 ```python
-# testing and benchmarking convolution
-# for complete benchmarking check /tests_and_benchmark
-
-# 3x1024x1024 Input
-C,H = 3,1024
 
-@jax.jit
-def jax_conv2d(x,w):
-    return jax.lax.conv_general_dilated(
-        lhs = x,
-        rhs = w,
-        window_strides = (1,1),
-        padding = 'SAME',
-        dimension_numbers = ('NCHW', 'OIHW', 'NCHW'),)[0]
-
-
-x = jax.random.normal(jax.random.PRNGKey(0),(C,H,H))
-xx = x[None]
-w = jax.random.normal(jax.random.PRNGKey(0),(C,3,3))
-ww = w[None]
-
-# assert equal
-np.testing.assert_allclose(kernex_conv2d(x,w),jax_conv2d(xx,ww),atol=1e-3)
+# lets solve dydt = y, where y0 = 1 and y(t)=e^t
+# using Runge-Kutta 4th order method
+# f(t,y) = y
+import jax.numpy as jnp
+import matplotlib.pyplot as plt
+import kernex as kex
 
-# Mac M1 CPU
-# check tests_and_benchmark folder for more.
 
-%timeit kernex_conv2d(x,w).block_until_ready()
-# 3.96 ms ± 272 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
+t = jnp.linspace(0, 1, 5)
+y = jnp.zeros(5)
+x = jnp.stack([y, t], axis=0)
+dt = t[1] - t[0]  # 0.1
+f = lambda tn, yn: yn
+
+
+def ic(x):
+    """ initial condition y0 = 1 """
+    return 1.
+
+
+def rk4(x):
+    """ runge kutta 4th order integration step """
+    # ┌────┬────┬────┐      ┌──────┬──────┬──────┐
+    # │ y0 │*y1*│ y2 │      │[0,-1]│[0, 0]│[0, 1]│
+    # ├────┼────┼────┤ ==>  ├──────┼──────┼──────┤
+    # │ t0 │ t1 │ t2 │      │[1,-1]│[1, 0]│[1, 1]│
+    # └────┴────┴────┘      └──────┴──────┴──────┘
+    t0 = x[1, -1]
+    y0 = x[0, -1]
+    k1 = dt * f(t0, y0)
+    k2 = dt * f(t0 + dt / 2, y0 + 1 / 2 * k1)
+    k3 = dt * f(t0 + dt / 2, y0 + 1 / 2 * k2)
+    k4 = dt * f(t0 + dt, y0 + k3)
+    yn_1 = y0 + 1 / 6 * (k1 + 2 * k2 + 2 * k3 + k4)
+    return yn_1
+
+
+F = kex.kscan(kernel_size=(2, 3), relative=True, padding=((0, 1)))  # kernel size = 3
+
+F[0:1, 1:] = rk4
+F[0, 0] = ic
+# compile the solver
+solver = jax.jit(F.__call__)
+y = solver(x)[0, :]
+
+plt.plot(t, y, '-o', label='rk4')
+plt.plot(t, jnp.exp(t), '-o', label='analytical')
+plt.legend()
 
-%timeit jax_conv2d(xx,ww).block_until_ready()
-# 27.5 ms ± 993 µs per loop (mean ± std. dev. of 7 runs, 10 loops each)
 ```
 
-</details>
-
-<details><summary>get_patches</summary>
-
-```python
-# benchmarking `get_patches` with `jax.lax.conv_general_dilated_patches`
-# On Mac M1 CPU
-
-@jax.jit
-@kex.kmap(kernel_size=(3,),padding='same')
-def get_patches(x):
-    return x
-
-@jax.jit
-def jax_get_patches(x):
-    return jax.lax.conv_general_dilated_patches(x,(3,),(1,),padding='same')
-
-x = jnp.ones([1_000_000])
-xx = jnp.ones([1,1,1_000_000])
-
-np.testing.assert_allclose(
-    get_patches(x),
-    jax_get_patches(xx).reshape(-1,1_000_000).T)
-
->> %timeit get_patches(x).block_until_ready()
->> %timeit jax_get_patches(xx).block_until_ready()
-
-1.73 ms ± 92.7 µs per loop (mean ± std. dev. of 7 runs, 1,000 loops each)
-10.6 ms ± 337 µs per loop (mean ± std. dev. of 7 runs, 100 loops each)
-```
+![img](assets/rk4.svg)
 
 </details>
```

### Comparing `kernex-0.1.3/kernex.egg-info/SOURCES.txt` & `kernex-0.2.0/kernex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kernex-0.1.3/setup.py` & `kernex-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `kernex-0.1.3/tests/test_interface.py` & `kernex-0.2.0/tests/test_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,28 @@
+from __future__ import annotations
+
+import os
+
+import pytest
+
+os.environ["XLA_FLAGS"] = "--xla_force_host_platform_device_count=256"
+
+# trunk-ignore(flake8/E402)
 import jax
+
+# trunk-ignore(flake8/E402)
 import jax.numpy as jnp
+
+# trunk-ignore(flake8/E402)
 import numpy as np
+
+# trunk-ignore(flake8/E402)
 from numpy.testing import assert_allclose
 
+# trunk-ignore(flake8/E402)
 import kernex as kex
 
 # # helper function to construct nd arrays
 # mat   = lambda *args : jnp.arange(1,reduce(lambda x,y:x*y,args)+1).reshape(*args)
 
 
 def test_Diffusion2D():
@@ -180,17 +196,23 @@
     # for line in kex_solution[::20]:
     #   plt.plot(jnp.linspace(0,xmax,nx),line)
     kex_solution = F(jnp.array(u))
 
     assert_allclose(kex_solution, fdm_solution.T, atol=1e-3)
 
 
-def test_mesh():
+@pytest.mark.parametrize("map_kind", ["vmap", "lmap", "pmap"])
+def test_mesh(map_kind):
 
-    Mesh = kex.kmap(kernel_size=(1,), relative=True, padding="same")
+    Mesh = kex.kmap(
+        kernel_size=(1,),
+        relative=True,
+        padding="same",
+        map_kind=map_kind,
+    )
 
     Mesh[0] = lambda x: x[0] * 10
     Mesh[1] = lambda x: x[0] * -10
     Mesh[2:] = lambda x: x[0] * 100
     array = jnp.arange(1, 11)
 
     np.testing.assert_allclose(
@@ -245,59 +267,76 @@
 
     u, _ = jax.lax.scan(scan_func, A, jnp.arange(2))
     np.testing.assert_allclose(
         u, jnp.array([1.0, 9.0, 21.0, 37.0, 57.0, 81.0, 109.0, 141.0, 159.0, 1.0])
     )
 
 
-def test_lax_scan_with_kmap():
+@pytest.mark.parametrize("map_kind", ["vmap", "lmap", "pmap"])
+def test_lax_scan_with_kmap(map_kind):
     A = jnp.ones([10])
-    F = kex.kmap(kernel_size=(1,), relative=True, padding="same")
+    F = kex.kmap(
+        kernel_size=(1,),
+        relative=True,
+        padding="same",
+        map_kind=map_kind,
+    )
     F[1:-1] = lambda x: x[0] + 1
     F[0] = F[-1] = lambda x: x[0]
 
     np.testing.assert_allclose(F(A), np.array([1, 2, 2, 2, 2, 2, 2, 2, 2, 1]))
 
     def scan_fn(carry, xs):
         return F(carry), None
 
     u, _ = jax.lax.scan(scan_fn, A, jnp.arange(9))
     np.testing.assert_allclose(u, np.array([1, 10, 10, 10, 10, 10, 10, 10, 10, 1]))
 
     A = jnp.ones([10])
-    F = kex.kmap(kernel_size=(3,), relative=True, padding="same")
+    F = kex.kmap(
+        kernel_size=(3,),
+        relative=True,
+        padding="same",
+        map_kind=map_kind,
+    )
     F[1:-1] = lambda x: x[0] + x[-1] + x[1]
     F[0] = F[-1] = lambda x: x[0]
 
     np.testing.assert_allclose(
         F(A), jnp.array([1.0, 3.0, 3.0, 3.0, 3.0, 3.0, 3.0, 3.0, 3.0, 1.0])
     )
 
     def scan_func(carry, xs):
         return F(carry), None
 
     u, _ = jax.lax.scan(scan_func, A, jnp.arange(2))
     np.testing.assert_allclose(u, jnp.array([1.0, 7.0, 9, 9, 9, 9, 9, 9, 7, 1.0]))
 
 
-def test_conv2d():
+@pytest.mark.parametrize("map_kind", ["vmap", "lmap", "pmap"])
+def test_conv2d(map_kind):
     C, H = 3, 16
 
     @jax.jit
     def jax_conv2d(x, w):
         return jax.lax.conv_general_dilated(
             lhs=x,
             rhs=w,
             window_strides=(1, 1),
             padding="SAME",
             dimension_numbers=("NCHW", "OIHW", "NCHW"),
         )[0]
 
     @jax.jit
-    @kex.kmap(kernel_size=(C, 3, 3), padding=("valid", "same", "same"), relative=False)
+    @kex.kmap(
+        kernel_size=(C, 3, 3),
+        padding=("valid", "same", "same"),
+        relative=False,
+        map_kind=map_kind,
+    )
     def kex_conv2d(x, w):
         return jnp.sum(x * w)
 
     x = jax.random.normal(jax.random.PRNGKey(0), (C, H, H))
     xx = x[None]
     w = jax.random.normal(jax.random.PRNGKey(0), (C, 3, 3))
     ww = w[None]
```

### Comparing `kernex-0.1.3/tests/test_scan_and_map.py` & `kernex-0.2.0/tests/test_scan_and_map.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import reduce
 
 import jax.numpy as jnp
 from numpy.testing import assert_array_equal
 
 from kernex._src.map import kernel_map, offset_kernel_map
 from kernex._src.scan import kernel_scan, offset_kernel_scan
```

### Comparing `kernex-0.1.3/tests/test_utils.py` & `kernex-0.2.0/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from functools import reduce
 
 import jax.numpy as jnp
 from numpy.testing import assert_array_equal
 
 from kernex._src.utils import roll_view
```

### Comparing `kernex-0.1.3/tests_and_benchmarks/test_benchmark_conv2d.py` & `kernex-0.2.0/tests_and_benchmarks/test_benchmark_conv2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import itertools
 import time
 from functools import reduce
 from statistics import mean, stdev
 
 import jax
 import jax.numpy as jnp
@@ -10,27 +12,24 @@
 import kernex as kex
 
 mat = lambda *args: jnp.arange(1, reduce(lambda x, y: x * y, args) + 1).reshape(*args)
 
 
 def test_and_time_conv2d():
 
-    print()
-    print("backend name = ", jax.devices())
+    print("\nbackend name = ", jax.devices())
 
     iters = 50
 
     dims = list(
         sorted(itertools.product([4, 8, 16, 32, 64], [16, 32, 64, 128, 256, 512, 1024]))
     )
 
     for C, H in dims:
 
-        print()
-
         @jax.jit
         def jax_conv2d(x, w):
             return jax.lax.conv_general_dilated(
                 lhs=x,
                 rhs=w,
                 window_strides=(1, 1),
                 padding="SAME",
@@ -57,15 +56,15 @@
 
         for _ in range(iters):
             t1 = time.time()
             kex_conv2d(x, w).block_until_ready()
             t2 = time.time()
             times += [(t2 - t1)]
 
-        print(f"[benchmarking]:\tconv2d @ dim={(C,H,H)}")
+        print(f"\n[benchmarking]:\tconv2d @ dim={(C,H,H)}")
         print("=" * 50)
 
         print(
             f"[kex] average : {mean(times)*1e6:.0f} us\t stddev : {stdev(times)*1e6:.3f}us"
         )
 
         times = []
```

