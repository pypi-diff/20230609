# Comparing `tmp/beaverpy-0.0.2.tar.gz` & `tmp/beaverpy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaverpy-0.0.2.tar", last modified: Thu Jun  8 23:12:02 2023, max compression
+gzip compressed data, was "beaverpy-0.1.0.tar", last modified: Thu Jun  8 23:20:11 2023, max compression
```

## Comparing `beaverpy-0.0.2.tar` & `beaverpy-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.885476 beaverpy-0.0.2/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1083 2023-06-08 21:14:50.000000 beaverpy-0.0.2/LICENSE
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8524 2023-06-08 23:12:02.884429 beaverpy-0.0.2/PKG-INFO
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     7969 2023-06-08 22:56:26.000000 beaverpy-0.0.2/README.md
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      647 2023-06-08 23:00:10.000000 beaverpy-0.0.2/pyproject.toml
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       38 2023-06-08 23:12:02.885748 beaverpy-0.0.2/setup.cfg
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.837113 beaverpy-0.0.2/src/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 21:45:49.000000 beaverpy-0.0.2/src/__init__.py
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.855703 beaverpy-0.0.2/src/beaverpy/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    11086 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Conv2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2934 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/CosineSimilarity.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     3321 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Linear.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2980 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/MSELoss.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    10307 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/MaxPool2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1869 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/ReLU.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1812 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Sigmoid.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1982 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Softmax.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      243 2023-06-08 21:56:02.000000 beaverpy-0.0.2/src/beaverpy/__init__.py
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.860492 beaverpy-0.0.2/src/beaverpy.egg-info/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8524 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/PKG-INFO
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      597 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/SOURCES.txt
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        1 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/dependency_links.txt
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       18 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/top_level.txt
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.880407 beaverpy-0.0.2/tests/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5251 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Conv2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2425 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_CosineSimilarity.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2630 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Linear.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2152 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_MSELoss.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5131 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_MaxPool2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1680 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_ReLU.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1714 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Sigmoid.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1840 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Softmax.py
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:20:11.588632 beaverpy-0.1.0/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1083 2023-06-08 21:14:50.000000 beaverpy-0.1.0/LICENSE
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8721 2023-06-08 23:20:11.587710 beaverpy-0.1.0/PKG-INFO
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8166 2023-06-08 23:19:57.000000 beaverpy-0.1.0/README.md
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      647 2023-06-08 23:18:27.000000 beaverpy-0.1.0/pyproject.toml
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       38 2023-06-08 23:20:11.589000 beaverpy-0.1.0/setup.cfg
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:20:11.546115 beaverpy-0.1.0/src/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 21:45:49.000000 beaverpy-0.1.0/src/__init__.py
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:20:11.562753 beaverpy-0.1.0/src/beaverpy/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    11086 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/Conv2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2934 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/CosineSimilarity.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     3321 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/Linear.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2980 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/MSELoss.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    10307 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/MaxPool2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1869 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/ReLU.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1812 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/Sigmoid.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1982 2023-06-08 21:14:50.000000 beaverpy-0.1.0/src/beaverpy/Softmax.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      243 2023-06-08 21:56:02.000000 beaverpy-0.1.0/src/beaverpy/__init__.py
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:20:11.568646 beaverpy-0.1.0/src/beaverpy.egg-info/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8721 2023-06-08 23:20:11.000000 beaverpy-0.1.0/src/beaverpy.egg-info/PKG-INFO
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      597 2023-06-08 23:20:11.000000 beaverpy-0.1.0/src/beaverpy.egg-info/SOURCES.txt
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        1 2023-06-08 23:20:11.000000 beaverpy-0.1.0/src/beaverpy.egg-info/dependency_links.txt
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       18 2023-06-08 23:20:11.000000 beaverpy-0.1.0/src/beaverpy.egg-info/top_level.txt
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:20:11.585425 beaverpy-0.1.0/tests/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5251 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_Conv2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2425 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_CosineSimilarity.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2630 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_Linear.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2152 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_MSELoss.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5131 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_MaxPool2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1680 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_ReLU.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1714 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_Sigmoid.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1840 2023-06-08 21:14:35.000000 beaverpy-0.1.0/tests/test_Softmax.py
```

### Comparing `beaverpy-0.0.2/LICENSE` & `beaverpy-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/PKG-INFO` & `beaverpy-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaverpy
-Version: 0.0.2
+Version: 0.1.0
 Summary: `beaverpy` is an implementation of PyTorch operators using only NumPy
 Author-email: Sai Anuroop Kesanapalli <ksanu1998@gmail.com>
 Project-URL: Homepage, https://github.com/ksanu1998/beaverpy
 Project-URL: Bug Tracker, https://github.com/ksanu1998/beaverpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # beaverpy :beaver:
 ### 
 
 ### Description
+#### v0.1.0
 `beaverpy` is an implementation of PyTorch operators using only NumPy. <br>
 Implemented operators (their PyTorch equivalents) include the following:
 * Layers
    - `Conv2D` ([`torch.nn.Conv2d`](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html))
    - `MaxPool2D` ([`torch.nn.MaxPool2d`](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html)) 
    - `Linear` ([`torch.nn.Linear`](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html))
 * Loss/Distance Functions
@@ -98,15 +99,15 @@
 ``` 
 ##### In case you wish to provide your own kernel, then define the same and pass it as an argument to `forward()` :
 
 ``` python
 
 kernels = []
 for k in range(out_channels):
-    kernel = np.random.rand(int(in_channels / groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
+    kernel = np.random.rand(int(in_channels / _groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
     kernels.append(kernel)
 _output = conv2d.forward(_input, kernels) # perform convolution
 
 ```
 
 #### Following is an example to use `MaxPool2D`: <br>
 
@@ -217,15 +218,15 @@
 ``` python
 
 num_dim = np.random.randint(6) + 1 # number of input dimensions
 shape = tuple(np.random.randint(5) + 1 for _ in range(num_dim)) # shape of input
 _input1 = np.random.rand(*shape) # generate an input based on the dimensions and shape
 _input2 = np.random.rand(*shape) # generate another input based on the dimensions and shape
 _dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed (optional)
-_eps = np.random.uniform(low = 1e-10, high = 1e-6) (optional)
+_eps = np.random.uniform(low = 1e-10, high = 1e-6) # (optional)
         
 ```
 ##### Call an instance of `CosineSimilarity` with the input parameters
 ``` python
 
 cosinesimilarity = bp.CosineSimilarity(dim = _dim, eps = _eps)
 
@@ -285,15 +286,15 @@
 
 #### Following is an example to use `Softmax`: <br>
 
 ##### Create a random input and dimension 
 ``` python
 
 _input = np.random.rand(1, 2, 1, 3, 4)
-_dim = np.random.randint(len(_input)) (optional)
+_dim = np.random.randint(len(_input)) # (optional)
 
 ```
 ##### Call an instance of `Softmax` with the input parameters
 ``` python
 
 softmax = bp.Softmax(dim = _dim)
 
@@ -306,14 +307,15 @@
 
 ``` 
 
 ### Future work
 * Replace `torch.round()` with `np.allclose()` for tests
 * Implement other operators
 * Optimize code
+* For newer builds of this package that are under development and not yet available on PyPI, please visit the <a href="https://github.com/ksanu1998/beaverpy">GitHub repository</a>
 
 ### Acknowledgements
 This work is being done during my summer internship at <a href="https://www.degirum.ai/">DeGirum Corp.</a>, Santa Clara. 
 
 ### Using this code in your projects
 * If you are using this code in your projects, please make sure to cite this repository and the author
 * If you find bugs, create a pull request with a description of the bug and the proposed changes
```

### Comparing `beaverpy-0.0.2/README.md` & `beaverpy-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # beaverpy :beaver:
 ### 
 
 ### Description
+#### v0.1.0
 `beaverpy` is an implementation of PyTorch operators using only NumPy. <br>
 Implemented operators (their PyTorch equivalents) include the following:
 * Layers
    - `Conv2D` ([`torch.nn.Conv2d`](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html))
    - `MaxPool2D` ([`torch.nn.MaxPool2d`](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html)) 
    - `Linear` ([`torch.nn.Linear`](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html))
 * Loss/Distance Functions
@@ -84,15 +85,15 @@
 ``` 
 ##### In case you wish to provide your own kernel, then define the same and pass it as an argument to `forward()` :
 
 ``` python
 
 kernels = []
 for k in range(out_channels):
-    kernel = np.random.rand(int(in_channels / groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
+    kernel = np.random.rand(int(in_channels / _groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
     kernels.append(kernel)
 _output = conv2d.forward(_input, kernels) # perform convolution
 
 ```
 
 #### Following is an example to use `MaxPool2D`: <br>
 
@@ -203,15 +204,15 @@
 ``` python
 
 num_dim = np.random.randint(6) + 1 # number of input dimensions
 shape = tuple(np.random.randint(5) + 1 for _ in range(num_dim)) # shape of input
 _input1 = np.random.rand(*shape) # generate an input based on the dimensions and shape
 _input2 = np.random.rand(*shape) # generate another input based on the dimensions and shape
 _dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed (optional)
-_eps = np.random.uniform(low = 1e-10, high = 1e-6) (optional)
+_eps = np.random.uniform(low = 1e-10, high = 1e-6) # (optional)
         
 ```
 ##### Call an instance of `CosineSimilarity` with the input parameters
 ``` python
 
 cosinesimilarity = bp.CosineSimilarity(dim = _dim, eps = _eps)
 
@@ -271,15 +272,15 @@
 
 #### Following is an example to use `Softmax`: <br>
 
 ##### Create a random input and dimension 
 ``` python
 
 _input = np.random.rand(1, 2, 1, 3, 4)
-_dim = np.random.randint(len(_input)) (optional)
+_dim = np.random.randint(len(_input)) # (optional)
 
 ```
 ##### Call an instance of `Softmax` with the input parameters
 ``` python
 
 softmax = bp.Softmax(dim = _dim)
 
@@ -292,14 +293,15 @@
 
 ``` 
 
 ### Future work
 * Replace `torch.round()` with `np.allclose()` for tests
 * Implement other operators
 * Optimize code
+* For newer builds of this package that are under development and not yet available on PyPI, please visit the <a href="https://github.com/ksanu1998/beaverpy">GitHub repository</a>
 
 ### Acknowledgements
 This work is being done during my summer internship at <a href="https://www.degirum.ai/">DeGirum Corp.</a>, Santa Clara. 
 
 ### Using this code in your projects
 * If you are using this code in your projects, please make sure to cite this repository and the author
 * If you find bugs, create a pull request with a description of the bug and the proposed changes
```

### Comparing `beaverpy-0.0.2/pyproject.toml` & `beaverpy-0.1.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beaverpy"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
   { name="Sai Anuroop Kesanapalli", email="ksanu1998@gmail.com" },
 ]
 description = "`beaverpy` is an implementation of PyTorch operators using only NumPy"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `beaverpy-0.0.2/src/beaverpy/Conv2D.py` & `beaverpy-0.1.0/src/beaverpy/Conv2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/CosineSimilarity.py` & `beaverpy-0.1.0/src/beaverpy/CosineSimilarity.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/Linear.py` & `beaverpy-0.1.0/src/beaverpy/Linear.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/MSELoss.py` & `beaverpy-0.1.0/src/beaverpy/MSELoss.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/MaxPool2D.py` & `beaverpy-0.1.0/src/beaverpy/MaxPool2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/ReLU.py` & `beaverpy-0.1.0/src/beaverpy/ReLU.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/Sigmoid.py` & `beaverpy-0.1.0/src/beaverpy/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy/Softmax.py` & `beaverpy-0.1.0/src/beaverpy/Softmax.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/src/beaverpy.egg-info/PKG-INFO` & `beaverpy-0.1.0/src/beaverpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beaverpy
-Version: 0.0.2
+Version: 0.1.0
 Summary: `beaverpy` is an implementation of PyTorch operators using only NumPy
 Author-email: Sai Anuroop Kesanapalli <ksanu1998@gmail.com>
 Project-URL: Homepage, https://github.com/ksanu1998/beaverpy
 Project-URL: Bug Tracker, https://github.com/ksanu1998/beaverpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # beaverpy :beaver:
 ### 
 
 ### Description
+#### v0.1.0
 `beaverpy` is an implementation of PyTorch operators using only NumPy. <br>
 Implemented operators (their PyTorch equivalents) include the following:
 * Layers
    - `Conv2D` ([`torch.nn.Conv2d`](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html))
    - `MaxPool2D` ([`torch.nn.MaxPool2d`](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html)) 
    - `Linear` ([`torch.nn.Linear`](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html))
 * Loss/Distance Functions
@@ -98,15 +99,15 @@
 ``` 
 ##### In case you wish to provide your own kernel, then define the same and pass it as an argument to `forward()` :
 
 ``` python
 
 kernels = []
 for k in range(out_channels):
-    kernel = np.random.rand(int(in_channels / groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
+    kernel = np.random.rand(int(in_channels / _groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
     kernels.append(kernel)
 _output = conv2d.forward(_input, kernels) # perform convolution
 
 ```
 
 #### Following is an example to use `MaxPool2D`: <br>
 
@@ -217,15 +218,15 @@
 ``` python
 
 num_dim = np.random.randint(6) + 1 # number of input dimensions
 shape = tuple(np.random.randint(5) + 1 for _ in range(num_dim)) # shape of input
 _input1 = np.random.rand(*shape) # generate an input based on the dimensions and shape
 _input2 = np.random.rand(*shape) # generate another input based on the dimensions and shape
 _dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed (optional)
-_eps = np.random.uniform(low = 1e-10, high = 1e-6) (optional)
+_eps = np.random.uniform(low = 1e-10, high = 1e-6) # (optional)
         
 ```
 ##### Call an instance of `CosineSimilarity` with the input parameters
 ``` python
 
 cosinesimilarity = bp.CosineSimilarity(dim = _dim, eps = _eps)
 
@@ -285,15 +286,15 @@
 
 #### Following is an example to use `Softmax`: <br>
 
 ##### Create a random input and dimension 
 ``` python
 
 _input = np.random.rand(1, 2, 1, 3, 4)
-_dim = np.random.randint(len(_input)) (optional)
+_dim = np.random.randint(len(_input)) # (optional)
 
 ```
 ##### Call an instance of `Softmax` with the input parameters
 ``` python
 
 softmax = bp.Softmax(dim = _dim)
 
@@ -306,14 +307,15 @@
 
 ``` 
 
 ### Future work
 * Replace `torch.round()` with `np.allclose()` for tests
 * Implement other operators
 * Optimize code
+* For newer builds of this package that are under development and not yet available on PyPI, please visit the <a href="https://github.com/ksanu1998/beaverpy">GitHub repository</a>
 
 ### Acknowledgements
 This work is being done during my summer internship at <a href="https://www.degirum.ai/">DeGirum Corp.</a>, Santa Clara. 
 
 ### Using this code in your projects
 * If you are using this code in your projects, please make sure to cite this repository and the author
 * If you find bugs, create a pull request with a description of the bug and the proposed changes
```

### Comparing `beaverpy-0.0.2/src/beaverpy.egg-info/SOURCES.txt` & `beaverpy-0.1.0/src/beaverpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_Conv2D.py` & `beaverpy-0.1.0/tests/test_Conv2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_CosineSimilarity.py` & `beaverpy-0.1.0/tests/test_CosineSimilarity.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_Linear.py` & `beaverpy-0.1.0/tests/test_Linear.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_MSELoss.py` & `beaverpy-0.1.0/tests/test_MSELoss.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_MaxPool2D.py` & `beaverpy-0.1.0/tests/test_MaxPool2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_ReLU.py` & `beaverpy-0.1.0/tests/test_ReLU.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_Sigmoid.py` & `beaverpy-0.1.0/tests/test_Sigmoid.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.2/tests/test_Softmax.py` & `beaverpy-0.1.0/tests/test_Softmax.py`

 * *Files identical despite different names*

