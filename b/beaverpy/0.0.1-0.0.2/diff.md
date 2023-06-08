# Comparing `tmp/beaverpy-0.0.1.tar.gz` & `tmp/beaverpy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beaverpy-0.0.1.tar", last modified: Thu Jun  8 20:28:59 2023, max compression
+gzip compressed data, was "beaverpy-0.0.2.tar", last modified: Thu Jun  8 23:12:02 2023, max compression
```

## Comparing `beaverpy-0.0.1.tar` & `beaverpy-0.0.2.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 20:28:59.845263 beaverpy-0.0.1/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1083 2023-06-08 18:55:47.000000 beaverpy-0.0.1/LICENSE
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     9807 2023-06-08 20:28:59.844303 beaverpy-0.0.1/PKG-INFO
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     9257 2023-06-07 23:29:02.000000 beaverpy-0.0.1/README.md
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      642 2023-06-08 19:54:19.000000 beaverpy-0.0.1/pyproject.toml
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       38 2023-06-08 20:28:59.845573 beaverpy-0.0.1/setup.cfg
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 20:28:59.805676 beaverpy-0.0.1/src/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 19:56:08.000000 beaverpy-0.0.1/src/__init__.py
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 20:28:59.821030 beaverpy-0.0.1/src/beaverpy/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    11086 2023-06-01 22:30:07.000000 beaverpy-0.0.1/src/beaverpy/Conv2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2934 2023-06-07 23:29:02.000000 beaverpy-0.0.1/src/beaverpy/CosineSimilarity.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     3321 2023-06-01 22:30:07.000000 beaverpy-0.0.1/src/beaverpy/Linear.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2980 2023-06-02 22:53:59.000000 beaverpy-0.0.1/src/beaverpy/MSELoss.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    10307 2023-06-01 22:30:07.000000 beaverpy-0.0.1/src/beaverpy/MaxPool2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1869 2023-06-01 22:30:07.000000 beaverpy-0.0.1/src/beaverpy/ReLU.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1812 2023-06-06 21:38:34.000000 beaverpy-0.0.1/src/beaverpy/Sigmoid.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1982 2023-06-05 21:59:52.000000 beaverpy-0.0.1/src/beaverpy/Softmax.py
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 20:28:59.826082 beaverpy-0.0.1/src/beaverpy.egg-info/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     9807 2023-06-08 20:28:59.000000 beaverpy-0.0.1/src/beaverpy.egg-info/PKG-INFO
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      572 2023-06-08 20:28:59.000000 beaverpy-0.0.1/src/beaverpy.egg-info/SOURCES.txt
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        1 2023-06-08 20:28:59.000000 beaverpy-0.0.1/src/beaverpy.egg-info/dependency_links.txt
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       18 2023-06-08 20:28:59.000000 beaverpy-0.0.1/src/beaverpy.egg-info/top_level.txt
-drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 20:28:59.842496 beaverpy-0.0.1/tests/
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5251 2023-06-01 22:30:07.000000 beaverpy-0.0.1/tests/test_Conv2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2425 2023-06-07 23:29:02.000000 beaverpy-0.0.1/tests/test_CosineSimilarity.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2630 2023-06-01 22:30:07.000000 beaverpy-0.0.1/tests/test_Linear.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2152 2023-06-05 21:59:52.000000 beaverpy-0.0.1/tests/test_MSELoss.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5131 2023-06-01 22:30:07.000000 beaverpy-0.0.1/tests/test_MaxPool2D.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1680 2023-06-02 22:53:59.000000 beaverpy-0.0.1/tests/test_ReLU.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1714 2023-06-06 21:38:34.000000 beaverpy-0.0.1/tests/test_Sigmoid.py
--rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1840 2023-06-05 21:59:52.000000 beaverpy-0.0.1/tests/test_Softmax.py
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.885476 beaverpy-0.0.2/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1083 2023-06-08 21:14:50.000000 beaverpy-0.0.2/LICENSE
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8524 2023-06-08 23:12:02.884429 beaverpy-0.0.2/PKG-INFO
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     7969 2023-06-08 22:56:26.000000 beaverpy-0.0.2/README.md
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      647 2023-06-08 23:00:10.000000 beaverpy-0.0.2/pyproject.toml
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       38 2023-06-08 23:12:02.885748 beaverpy-0.0.2/setup.cfg
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.837113 beaverpy-0.0.2/src/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 21:45:49.000000 beaverpy-0.0.2/src/__init__.py
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.855703 beaverpy-0.0.2/src/beaverpy/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    11086 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Conv2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2934 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/CosineSimilarity.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     3321 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Linear.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2980 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/MSELoss.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)    10307 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/MaxPool2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1869 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/ReLU.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1812 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Sigmoid.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1982 2023-06-08 21:14:50.000000 beaverpy-0.0.2/src/beaverpy/Softmax.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      243 2023-06-08 21:56:02.000000 beaverpy-0.0.2/src/beaverpy/__init__.py
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.860492 beaverpy-0.0.2/src/beaverpy.egg-info/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     8524 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/PKG-INFO
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)      597 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/SOURCES.txt
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)        1 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/dependency_links.txt
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)       18 2023-06-08 23:12:02.000000 beaverpy-0.0.2/src/beaverpy.egg-info/top_level.txt
+drwxr-xr-x   0 saianuroopkesanapalli   (501) staff       (20)        0 2023-06-08 23:12:02.880407 beaverpy-0.0.2/tests/
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5251 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Conv2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2425 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_CosineSimilarity.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2630 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Linear.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     2152 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_MSELoss.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     5131 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_MaxPool2D.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1680 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_ReLU.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1714 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Sigmoid.py
+-rw-r--r--   0 saianuroopkesanapalli   (501) staff       (20)     1840 2023-06-08 21:14:35.000000 beaverpy-0.0.2/tests/test_Softmax.py
```

### Comparing `beaverpy-0.0.1/LICENSE` & `beaverpy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/PKG-INFO` & `beaverpy-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,78 +1,98 @@
 Metadata-Version: 2.1
 Name: beaverpy
-Version: 0.0.1
-Summary: An implementation of some PyTorch operators using only NumPy
+Version: 0.0.2
+Summary: `beaverpy` is an implementation of PyTorch operators using only NumPy
 Author-email: Sai Anuroop Kesanapalli <ksanu1998@gmail.com>
-Project-URL: Homepage, https://github.com/ksanu1998/conv-NumPy
-Project-URL: Bug Tracker, https://github.com/ksanu1998/conv-NumPy/issues
+Project-URL: Homepage, https://github.com/ksanu1998/beaverpy
+Project-URL: Bug Tracker, https://github.com/ksanu1998/beaverpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# conv-NumPy
-## An implementation of `Conv2D`, `MaxPool2D`, `Linear`, `MSELoss`, `CosineSimilarity`, `ReLU`, `Sigmoid`, and `Softmax` using only NumPy
-### (being made) compatible with PyTorch `torch.nn.Conv2d`, `torch.nn.MaxPool2d`, `torch.nn.Linear`, `torch.nn.MSELoss`, `torch.nn.CosineSimilarity`, `torch.nn.ReLU`, `torch.nn.Sigmoid`, and `torch.nn.Softmax` respectively
+# beaverpy :beaver:
+### 
 
 ### Description
-* This repo is organized into `.ipynb` notebooks and `.py` modules - users can run the notebooks directly or call classes implemented in the modules
-* `Conv2D` currently supports `stride`, `padding`, `dilation`, and `groups` options
-* `Conv2D` is tested for correctness against `torch.nn.functional.conv2d`
-* `MaxPool2D` currently supports `stride`, `padding`, `dilation`, and `return_indices` options
-* `MaxPool2D` is tested for correctness against `torch.nn.MaxPool2d`
-* `Linear` currently supports `bias` option
-* `Linear` is tested for correctness against `torch.nn.functional.linear`
-* `MSELoss` currently supports `reduction` option
-* `MSELoss` is tested for correctness against `torch.nn.MSELoss`
-* `CosineSimilarity` currently supports `dim`, and `eps` options
-* `CosineSimilarity` is tested for correctness against `torch.nn.CosineSimilarity`
-* `ReLU` is tested for correctness against `torch.nn.ReLU`
-* `Sigmoid` is tested for correctness against `torch.nn.Sigmoid`
-* `Softmax` currently supports `dim` option
-* `Softmax` is tested for correctness against `torch.nn.Softmax`
-* Test code that checks for correctness of the implementation is included in the respective notebooks and also available as standalone `Pytest` scripts
-* Users can take a glance through the notebooks to gain an overview of the logic - code is not optimized
-
-### How to use
-:warning: Please note that this code is under development <br>
-#### Following is an example to use `Conv2D`, similar to `torch.nn.Conv2d`: <br>
+`beaverpy` is an implementation of PyTorch operators using only NumPy. <br>
+Implemented operators (their PyTorch equivalents) include the following:
+* Layers
+   - `Conv2D` ([`torch.nn.Conv2d`](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html))
+   - `MaxPool2D` ([`torch.nn.MaxPool2d`](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html)) 
+   - `Linear` ([`torch.nn.Linear`](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html))
+* Loss/Distance Functions
+   - `MSELoss` ([`torch.nn.MSELoss`](https://pytorch.org/docs/stable/generated/torch.nn.MSELoss.html))
+   - `CosineSimilarity` ([`torch.nn.CosineSimilarity`](https://pytorch.org/docs/stable/generated/torch.nn.CosineSimilarity.html))
+* Activations
+   - `ReLU` ([`torch.nn.ReLU`](https://pytorch.org/docs/stable/generated/torch.nn.ReLU.htm))
+   - `Sigmoid` ([`torch.nn.Sigmoid`](https://pytorch.org/docs/stable/generated/torch.nn.Sigmoid.html)) 
+   - `Softmax` ([`torch.nn.Softmax`](https://pytorch.org/docs/stable/generated/torch.nn.Softmax.html))
+> **Note 1:** `[n, c, h, w]` format is used
+
+> **Note 2:** Test code that checks for correctness of the implementation is included in respective notebooks and is also available as standalone `pytest` scripts
+
+### Optional parameters supported
+* `Conv2D` &mdash; `stride`, `padding`, `dilation`, `groups`
+* `MaxPool2D` &mdash; `stride`, `padding`, `dilation`, `return_indices`
+* `Linear` &mdash; `bias`
+* `MSELoss` &mdash; `reduction`
+* `CosineSimilarity` &mdash; `dim`, `eps`
+* `Softmax` &mdash; `dim`
+
+### How to install?
+```console
+
+pip3 install beaverpy
+
+```
+### How to use?
+<!-- :warning: Please note that this code is under development <br> -->
+
+#### Import `beaverpy` and `numpy`
+``` python
+
+import beaverpy as bp
+import numpy as np
+
+```
+
+#### Following is an example to use `Conv2D`: <br>
+
 ##### Define input parameters 
 ``` python
 
 in_channels = 6 # input channels
 out_channels = 4 # output channels
 kernel_size = (2, 2) # kernel size
 
-padding = (1, 3) # padding (optional)
-stride = (2, 1) # stride (optional)
-dilation = (2, 3) # dilation factor (optional)
-groups = 2 # groups (optional)
+_stride = (2, 1) # stride (optional)
+_padding = (1, 3) # padding (optional)
+_dilation = (2, 3) # dilation factor (optional)
+_groups = 2 # groups (optional)
 
 in_batches = 2 # input batches
 in_h = 4 # input height
 in_w = 4 # input weight
 
 ```
 ##### Create a random input using the input parameters
 ``` python
 
 _input = np.random.rand(in_batches, in_channels, in_h, in_w)
 
 ```
-
 ##### Call an instance of `Conv2D` with the input parameters
 ``` python
 
-conv2d = Conv2D(in_channels, out_channels, kernel_size, stride = stride, padding = padding, dilation = dilation, groups = groups)
+conv2d = bp.Conv2D(in_channels, out_channels, kernel_size, stride = _stride, padding = _padding, dilation = _dilation, groups = _groups)
 
 ```
-
 ##### Perform convolution
 
 ``` python
 
 _output = conv2d.forward(_input) # perform convolution
 
 ``` 
@@ -84,25 +104,26 @@
 for k in range(out_channels):
     kernel = np.random.rand(int(in_channels / groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
     kernels.append(kernel)
 _output = conv2d.forward(_input, kernels) # perform convolution
 
 ```
 
-#### Following is an example to use `MaxPool2D`, similar to `torch.nn.MaxPool2d`: <br>
+#### Following is an example to use `MaxPool2D`: <br>
+
 ##### Define input parameters 
 ``` python
 
 in_channels = 3 # input channels
 kernel_size = (6, 6) # kernel size
 
-padding = (1, 2) # padding (optional)
-stride = (1, 5) # stride (optional)
-dilation = (2, 1) # dilation factor (optional)
-return_indices = True # return max indices (optional)
+_stride = (1, 5) # stride (optional)
+_padding = (1, 2) # padding (optional)
+_dilation = (2, 1) # dilation factor (optional)
+_return_indices = True # return max indices (optional)
 
 in_batches = 3 # input batches
 in_h = 11 # input height
 in_w = 8 # input weight
 
 ```
 ##### Create a random input using the input parameters
@@ -111,49 +132,48 @@
 _input = np.random.rand(in_batches, in_channels, in_h, in_w)
 
 ```
 
 ##### Call an instance of `MaxPool2D` with the input parameters
 ``` python
 
-maxpool2d = MaxPool2D(kernel_size, stride = stride, padding = padding, dilation = dilation)
+maxpool2d = bp.MaxPool2D(kernel_size, stride = _stride, padding = _padding, dilation = _dilation, return_indices = _return_indices)
 
 ```
 
 ##### Perform maxpooling
 
 ``` python
 
 _output = maxpool2d.forward(_input)
 
 ``` 
 
-#### Following is an example to use `Linear`, similar to `torch.nn.Linear`: <br>
+#### Following is an example to use `Linear`: <br>
+
 ##### Define input parameters 
 ``` python
 
 in_samples = 128 # input samples
 in_features = 20 # input features
 out_features = 30 # output features
 
 ```
 ##### Create a random input using the input parameters
 ``` python
 
 _input = np.random.rand(in_samples, in_features)
 
 ```
-
 ##### Call an instance of `Linear` with the input parameters
 ``` python
 
-linear = Linear(in_features, out_features)
+linear = bp.Linear(in_features, out_features)
 
 ```
-
 ##### Apply a linear transformation
 
 ``` python
 
 _output = linear.forward(_input)
 
 ``` 
@@ -163,146 +183,140 @@
 
 _weights = np.random.rand(out_features, in_features) # define random weights
 _bias = np.random.rand(out_features) # define random bias
 _output = linear.forward(_input, weights = _weights, bias_weights = _bias) # apply linear transformation
 
 ```
 
-#### Following is an example to use `MSELoss`, similar to `torch.nn.MSELoss`: <br>
+#### Following is an example to use `MSELoss`: <br>
+
 ##### Create a random input and target
 ``` python
 
 dimension = np.random.randint(500) # dimension of the input and target
 _input = np.random.rand(dimension) # define a random input of the above dimension
 _target= np.random.rand(dimension) # define a random target of the above dimension
 
 ```
 ##### Call an instance of `MSELoss` with the input parameters
 ``` python
 
-mseloss = MSELoss()
+mseloss = bp.MSELoss()
 
 ```
-
 ##### Compue MSE loss
 
 ``` python
 
 _output = mseloss.forward(_input, _target)
 
 ``` 
 
-#### Following is an example to use `CosineSimilarity`, similar to `torch.nn.CosineSimilarity`: <br>
+#### Following is an example to use `CosineSimilarity`: <br>
+
 ##### Create random input
 ``` python
 
 num_dim = np.random.randint(6) + 1 # number of input dimensions
 shape = tuple(np.random.randint(5) + 1 for _ in range(num_dim)) # shape of input
 _input1 = np.random.rand(*shape) # generate an input based on the dimensions and shape
 _input2 = np.random.rand(*shape) # generate another input based on the dimensions and shape
-_dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed
-_eps = np.random.uniform(low = 1e-10, high = 1e-6)
+_dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed (optional)
+_eps = np.random.uniform(low = 1e-10, high = 1e-6) (optional)
         
 ```
 ##### Call an instance of `CosineSimilarity` with the input parameters
 ``` python
 
-cosinesimilarity = CosineSimilarity(dim = _dim, eps = _eps)
+cosinesimilarity = bp.CosineSimilarity(dim = _dim, eps = _eps)
 
 ```
-
 ##### Compue CosineSimilarity
 
 ``` python
 
 _output = cosinesimilarity.forward(_input1, _input2)
 
 ``` 
 
-#### Following is an example to use `ReLU`, similar to `torch.nn.ReLU`: <br>
+#### Following is an example to use `ReLU`: <br>
+
 ##### Create a random input
 ``` python
 
 _input = np.random.rand(10, 20, 3)
 
 ```
 ##### Call an instance of `ReLU` with the input parameters
 ``` python
 
-relu = ReLU()
+relu = bp.ReLU()
 
 ```
 
 ##### Apply ReLU activation
 
 ``` python
 
 _output = relu.forward(_input)
 
 ``` 
 
-#### Following is an example to use `Sigmoid`, similar to `torch.nn.Sigmoid`: <br>
+#### Following is an example to use `Sigmoid`: <br>
+
 ##### Create a random input
 ``` python
 
 _input = np.random.rand(10, 20, 3)
 
 ```
 ##### Call an instance of `Sigmoid` with the input parameters
 ``` python
 
-sigmoid = Sigmoid()
+sigmoid = bp.Sigmoid()
 
 ```
-
 ##### Apply Sigmoid activation
 
 ``` python
 
 _output = sigmoid.forward(_input)
 
 ``` 
 
-#### Following is an example to use `Softmax`, similar to `torch.nn.Softmax`: <br>
+#### Following is an example to use `Softmax`: <br>
+
 ##### Create a random input and dimension 
 ``` python
 
 _input = np.random.rand(1, 2, 1, 3, 4)
-_dim = np.random.randint(len(_input))
+_dim = np.random.randint(len(_input)) (optional)
 
 ```
 ##### Call an instance of `Softmax` with the input parameters
 ``` python
 
-softmax = Softmax(dim = _dim)
+softmax = bp.Softmax(dim = _dim)
 
 ```
-
 ##### Apply Softmax activation
 
 ``` python
 
 _output = softmax.forward(_input)
 
 ``` 
 
-### Specifics
-* `[n, c, h, w]` format is used
-* For a description of the input parameters, refer to PyTorch documentation of <a href="https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html">`torch.nn.Conv2d`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html">`torch.nn.MaxPool2d`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.Linear.html#torch.nn.Linear">`torch.nn.Linear`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.MSELoss.html">`torch.nn.MSELoss`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.CosineSimilarity.html">`torch.nn.CosineSimilarity`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.ReLU.html">`torch.nn.ReLU`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.Sigmoid.html#torch.nn.Sigmoid">`torch.nn.Sigmoid`</a>, and <a href="https://pytorch.org/docs/stable/generated/torch.nn.Softmax.html">`torch.nn.Softmax`</a>
-
 ### Future work
 * Replace `torch.round()` with `np.allclose()` for tests
 * Implement other operators
 * Optimize code
-* Implement `padding = 'same'` mode for `Conv2D`
-* Implement `ceil_mode` for `MaxPool2D`
-* Provide code insights
 
 ### Acknowledgements
 This work is being done during my summer internship at <a href="https://www.degirum.ai/">DeGirum Corp.</a>, Santa Clara. 
 
-### Using this code for your projects
-* If you are using this code, please make sure to cite this repository and the author
-* If you find bugs, create a pull request with a description of the bug and the proposed changes (code optimization requests will not be entertained for now, for reasons that will be provided soon)
+### Using this code in your projects
+* If you are using this code in your projects, please make sure to cite this repository and the author
+* If you find bugs, create a pull request with a description of the bug and the proposed changes
 * Do have a look at the <a href="https://ksanu1998.github.io/">author's webpage</a> for other interesting works!
 
-`README` last updated on 06/07/2023
+`README` last updated on 06/08/2023
```

### Comparing `beaverpy-0.0.1/README.md` & `beaverpy-0.0.2/src/beaverpy.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,64 +1,98 @@
-# conv-NumPy
-## An implementation of `Conv2D`, `MaxPool2D`, `Linear`, `MSELoss`, `CosineSimilarity`, `ReLU`, `Sigmoid`, and `Softmax` using only NumPy
-### (being made) compatible with PyTorch `torch.nn.Conv2d`, `torch.nn.MaxPool2d`, `torch.nn.Linear`, `torch.nn.MSELoss`, `torch.nn.CosineSimilarity`, `torch.nn.ReLU`, `torch.nn.Sigmoid`, and `torch.nn.Softmax` respectively
+Metadata-Version: 2.1
+Name: beaverpy
+Version: 0.0.2
+Summary: `beaverpy` is an implementation of PyTorch operators using only NumPy
+Author-email: Sai Anuroop Kesanapalli <ksanu1998@gmail.com>
+Project-URL: Homepage, https://github.com/ksanu1998/beaverpy
+Project-URL: Bug Tracker, https://github.com/ksanu1998/beaverpy/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# beaverpy :beaver:
+### 
 
 ### Description
-* This repo is organized into `.ipynb` notebooks and `.py` modules - users can run the notebooks directly or call classes implemented in the modules
-* `Conv2D` currently supports `stride`, `padding`, `dilation`, and `groups` options
-* `Conv2D` is tested for correctness against `torch.nn.functional.conv2d`
-* `MaxPool2D` currently supports `stride`, `padding`, `dilation`, and `return_indices` options
-* `MaxPool2D` is tested for correctness against `torch.nn.MaxPool2d`
-* `Linear` currently supports `bias` option
-* `Linear` is tested for correctness against `torch.nn.functional.linear`
-* `MSELoss` currently supports `reduction` option
-* `MSELoss` is tested for correctness against `torch.nn.MSELoss`
-* `CosineSimilarity` currently supports `dim`, and `eps` options
-* `CosineSimilarity` is tested for correctness against `torch.nn.CosineSimilarity`
-* `ReLU` is tested for correctness against `torch.nn.ReLU`
-* `Sigmoid` is tested for correctness against `torch.nn.Sigmoid`
-* `Softmax` currently supports `dim` option
-* `Softmax` is tested for correctness against `torch.nn.Softmax`
-* Test code that checks for correctness of the implementation is included in the respective notebooks and also available as standalone `Pytest` scripts
-* Users can take a glance through the notebooks to gain an overview of the logic - code is not optimized
-
-### How to use
-:warning: Please note that this code is under development <br>
-#### Following is an example to use `Conv2D`, similar to `torch.nn.Conv2d`: <br>
+`beaverpy` is an implementation of PyTorch operators using only NumPy. <br>
+Implemented operators (their PyTorch equivalents) include the following:
+* Layers
+   - `Conv2D` ([`torch.nn.Conv2d`](https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html))
+   - `MaxPool2D` ([`torch.nn.MaxPool2d`](https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html)) 
+   - `Linear` ([`torch.nn.Linear`](https://pytorch.org/docs/stable/generated/torch.nn.Linear.html))
+* Loss/Distance Functions
+   - `MSELoss` ([`torch.nn.MSELoss`](https://pytorch.org/docs/stable/generated/torch.nn.MSELoss.html))
+   - `CosineSimilarity` ([`torch.nn.CosineSimilarity`](https://pytorch.org/docs/stable/generated/torch.nn.CosineSimilarity.html))
+* Activations
+   - `ReLU` ([`torch.nn.ReLU`](https://pytorch.org/docs/stable/generated/torch.nn.ReLU.htm))
+   - `Sigmoid` ([`torch.nn.Sigmoid`](https://pytorch.org/docs/stable/generated/torch.nn.Sigmoid.html)) 
+   - `Softmax` ([`torch.nn.Softmax`](https://pytorch.org/docs/stable/generated/torch.nn.Softmax.html))
+> **Note 1:** `[n, c, h, w]` format is used
+
+> **Note 2:** Test code that checks for correctness of the implementation is included in respective notebooks and is also available as standalone `pytest` scripts
+
+### Optional parameters supported
+* `Conv2D` &mdash; `stride`, `padding`, `dilation`, `groups`
+* `MaxPool2D` &mdash; `stride`, `padding`, `dilation`, `return_indices`
+* `Linear` &mdash; `bias`
+* `MSELoss` &mdash; `reduction`
+* `CosineSimilarity` &mdash; `dim`, `eps`
+* `Softmax` &mdash; `dim`
+
+### How to install?
+```console
+
+pip3 install beaverpy
+
+```
+### How to use?
+<!-- :warning: Please note that this code is under development <br> -->
+
+#### Import `beaverpy` and `numpy`
+``` python
+
+import beaverpy as bp
+import numpy as np
+
+```
+
+#### Following is an example to use `Conv2D`: <br>
+
 ##### Define input parameters 
 ``` python
 
 in_channels = 6 # input channels
 out_channels = 4 # output channels
 kernel_size = (2, 2) # kernel size
 
-padding = (1, 3) # padding (optional)
-stride = (2, 1) # stride (optional)
-dilation = (2, 3) # dilation factor (optional)
-groups = 2 # groups (optional)
+_stride = (2, 1) # stride (optional)
+_padding = (1, 3) # padding (optional)
+_dilation = (2, 3) # dilation factor (optional)
+_groups = 2 # groups (optional)
 
 in_batches = 2 # input batches
 in_h = 4 # input height
 in_w = 4 # input weight
 
 ```
 ##### Create a random input using the input parameters
 ``` python
 
 _input = np.random.rand(in_batches, in_channels, in_h, in_w)
 
 ```
-
 ##### Call an instance of `Conv2D` with the input parameters
 ``` python
 
-conv2d = Conv2D(in_channels, out_channels, kernel_size, stride = stride, padding = padding, dilation = dilation, groups = groups)
+conv2d = bp.Conv2D(in_channels, out_channels, kernel_size, stride = _stride, padding = _padding, dilation = _dilation, groups = _groups)
 
 ```
-
 ##### Perform convolution
 
 ``` python
 
 _output = conv2d.forward(_input) # perform convolution
 
 ``` 
@@ -70,25 +104,26 @@
 for k in range(out_channels):
     kernel = np.random.rand(int(in_channels / groups), kernel_size[0], kernel_size[1]) # define a random kernel based on the kernel parameters
     kernels.append(kernel)
 _output = conv2d.forward(_input, kernels) # perform convolution
 
 ```
 
-#### Following is an example to use `MaxPool2D`, similar to `torch.nn.MaxPool2d`: <br>
+#### Following is an example to use `MaxPool2D`: <br>
+
 ##### Define input parameters 
 ``` python
 
 in_channels = 3 # input channels
 kernel_size = (6, 6) # kernel size
 
-padding = (1, 2) # padding (optional)
-stride = (1, 5) # stride (optional)
-dilation = (2, 1) # dilation factor (optional)
-return_indices = True # return max indices (optional)
+_stride = (1, 5) # stride (optional)
+_padding = (1, 2) # padding (optional)
+_dilation = (2, 1) # dilation factor (optional)
+_return_indices = True # return max indices (optional)
 
 in_batches = 3 # input batches
 in_h = 11 # input height
 in_w = 8 # input weight
 
 ```
 ##### Create a random input using the input parameters
@@ -97,49 +132,48 @@
 _input = np.random.rand(in_batches, in_channels, in_h, in_w)
 
 ```
 
 ##### Call an instance of `MaxPool2D` with the input parameters
 ``` python
 
-maxpool2d = MaxPool2D(kernel_size, stride = stride, padding = padding, dilation = dilation)
+maxpool2d = bp.MaxPool2D(kernel_size, stride = _stride, padding = _padding, dilation = _dilation, return_indices = _return_indices)
 
 ```
 
 ##### Perform maxpooling
 
 ``` python
 
 _output = maxpool2d.forward(_input)
 
 ``` 
 
-#### Following is an example to use `Linear`, similar to `torch.nn.Linear`: <br>
+#### Following is an example to use `Linear`: <br>
+
 ##### Define input parameters 
 ``` python
 
 in_samples = 128 # input samples
 in_features = 20 # input features
 out_features = 30 # output features
 
 ```
 ##### Create a random input using the input parameters
 ``` python
 
 _input = np.random.rand(in_samples, in_features)
 
 ```
-
 ##### Call an instance of `Linear` with the input parameters
 ``` python
 
-linear = Linear(in_features, out_features)
+linear = bp.Linear(in_features, out_features)
 
 ```
-
 ##### Apply a linear transformation
 
 ``` python
 
 _output = linear.forward(_input)
 
 ``` 
@@ -149,146 +183,140 @@
 
 _weights = np.random.rand(out_features, in_features) # define random weights
 _bias = np.random.rand(out_features) # define random bias
 _output = linear.forward(_input, weights = _weights, bias_weights = _bias) # apply linear transformation
 
 ```
 
-#### Following is an example to use `MSELoss`, similar to `torch.nn.MSELoss`: <br>
+#### Following is an example to use `MSELoss`: <br>
+
 ##### Create a random input and target
 ``` python
 
 dimension = np.random.randint(500) # dimension of the input and target
 _input = np.random.rand(dimension) # define a random input of the above dimension
 _target= np.random.rand(dimension) # define a random target of the above dimension
 
 ```
 ##### Call an instance of `MSELoss` with the input parameters
 ``` python
 
-mseloss = MSELoss()
+mseloss = bp.MSELoss()
 
 ```
-
 ##### Compue MSE loss
 
 ``` python
 
 _output = mseloss.forward(_input, _target)
 
 ``` 
 
-#### Following is an example to use `CosineSimilarity`, similar to `torch.nn.CosineSimilarity`: <br>
+#### Following is an example to use `CosineSimilarity`: <br>
+
 ##### Create random input
 ``` python
 
 num_dim = np.random.randint(6) + 1 # number of input dimensions
 shape = tuple(np.random.randint(5) + 1 for _ in range(num_dim)) # shape of input
 _input1 = np.random.rand(*shape) # generate an input based on the dimensions and shape
 _input2 = np.random.rand(*shape) # generate another input based on the dimensions and shape
-_dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed
-_eps = np.random.uniform(low = 1e-10, high = 1e-6)
+_dim = np.random.randint(num_dim) # dimension along which CosineSimilarity is to be computed (optional)
+_eps = np.random.uniform(low = 1e-10, high = 1e-6) (optional)
         
 ```
 ##### Call an instance of `CosineSimilarity` with the input parameters
 ``` python
 
-cosinesimilarity = CosineSimilarity(dim = _dim, eps = _eps)
+cosinesimilarity = bp.CosineSimilarity(dim = _dim, eps = _eps)
 
 ```
-
 ##### Compue CosineSimilarity
 
 ``` python
 
 _output = cosinesimilarity.forward(_input1, _input2)
 
 ``` 
 
-#### Following is an example to use `ReLU`, similar to `torch.nn.ReLU`: <br>
+#### Following is an example to use `ReLU`: <br>
+
 ##### Create a random input
 ``` python
 
 _input = np.random.rand(10, 20, 3)
 
 ```
 ##### Call an instance of `ReLU` with the input parameters
 ``` python
 
-relu = ReLU()
+relu = bp.ReLU()
 
 ```
 
 ##### Apply ReLU activation
 
 ``` python
 
 _output = relu.forward(_input)
 
 ``` 
 
-#### Following is an example to use `Sigmoid`, similar to `torch.nn.Sigmoid`: <br>
+#### Following is an example to use `Sigmoid`: <br>
+
 ##### Create a random input
 ``` python
 
 _input = np.random.rand(10, 20, 3)
 
 ```
 ##### Call an instance of `Sigmoid` with the input parameters
 ``` python
 
-sigmoid = Sigmoid()
+sigmoid = bp.Sigmoid()
 
 ```
-
 ##### Apply Sigmoid activation
 
 ``` python
 
 _output = sigmoid.forward(_input)
 
 ``` 
 
-#### Following is an example to use `Softmax`, similar to `torch.nn.Softmax`: <br>
+#### Following is an example to use `Softmax`: <br>
+
 ##### Create a random input and dimension 
 ``` python
 
 _input = np.random.rand(1, 2, 1, 3, 4)
-_dim = np.random.randint(len(_input))
+_dim = np.random.randint(len(_input)) (optional)
 
 ```
 ##### Call an instance of `Softmax` with the input parameters
 ``` python
 
-softmax = Softmax(dim = _dim)
+softmax = bp.Softmax(dim = _dim)
 
 ```
-
 ##### Apply Softmax activation
 
 ``` python
 
 _output = softmax.forward(_input)
 
 ``` 
 
-### Specifics
-* `[n, c, h, w]` format is used
-* For a description of the input parameters, refer to PyTorch documentation of <a href="https://pytorch.org/docs/stable/generated/torch.nn.Conv2d.html">`torch.nn.Conv2d`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.MaxPool2d.html">`torch.nn.MaxPool2d`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.Linear.html#torch.nn.Linear">`torch.nn.Linear`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.MSELoss.html">`torch.nn.MSELoss`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.CosineSimilarity.html">`torch.nn.CosineSimilarity`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.ReLU.html">`torch.nn.ReLU`</a>, <a href="https://pytorch.org/docs/stable/generated/torch.nn.Sigmoid.html#torch.nn.Sigmoid">`torch.nn.Sigmoid`</a>, and <a href="https://pytorch.org/docs/stable/generated/torch.nn.Softmax.html">`torch.nn.Softmax`</a>
-
 ### Future work
 * Replace `torch.round()` with `np.allclose()` for tests
 * Implement other operators
 * Optimize code
-* Implement `padding = 'same'` mode for `Conv2D`
-* Implement `ceil_mode` for `MaxPool2D`
-* Provide code insights
 
 ### Acknowledgements
 This work is being done during my summer internship at <a href="https://www.degirum.ai/">DeGirum Corp.</a>, Santa Clara. 
 
-### Using this code for your projects
-* If you are using this code, please make sure to cite this repository and the author
-* If you find bugs, create a pull request with a description of the bug and the proposed changes (code optimization requests will not be entertained for now, for reasons that will be provided soon)
+### Using this code in your projects
+* If you are using this code in your projects, please make sure to cite this repository and the author
+* If you find bugs, create a pull request with a description of the bug and the proposed changes
 * Do have a look at the <a href="https://ksanu1998.github.io/">author's webpage</a> for other interesting works!
 
-`README` last updated on 06/07/2023
+`README` last updated on 06/08/2023
```

### Comparing `beaverpy-0.0.1/pyproject.toml` & `beaverpy-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,23 +3,23 @@
     "setuptools>=61.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "beaverpy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Sai Anuroop Kesanapalli", email="ksanu1998@gmail.com" },
 ]
-description = "An implementation of some PyTorch operators using only NumPy"
+description = "`beaverpy` is an implementation of PyTorch operators using only NumPy"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/ksanu1998/conv-NumPy"
-"Bug Tracker" = "https://github.com/ksanu1998/conv-NumPy/issues"
+"Homepage" = "https://github.com/ksanu1998/beaverpy"
+"Bug Tracker" = "https://github.com/ksanu1998/beaverpy/issues"
```

### Comparing `beaverpy-0.0.1/src/beaverpy/Conv2D.py` & `beaverpy-0.0.2/src/beaverpy/Conv2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/CosineSimilarity.py` & `beaverpy-0.0.2/src/beaverpy/CosineSimilarity.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/Linear.py` & `beaverpy-0.0.2/src/beaverpy/Linear.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/MSELoss.py` & `beaverpy-0.0.2/src/beaverpy/MSELoss.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/MaxPool2D.py` & `beaverpy-0.0.2/src/beaverpy/MaxPool2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/ReLU.py` & `beaverpy-0.0.2/src/beaverpy/ReLU.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/Sigmoid.py` & `beaverpy-0.0.2/src/beaverpy/Sigmoid.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy/Softmax.py` & `beaverpy-0.0.2/src/beaverpy/Softmax.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/src/beaverpy.egg-info/SOURCES.txt` & `beaverpy-0.0.2/src/beaverpy.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 src/beaverpy/CosineSimilarity.py
 src/beaverpy/Linear.py
 src/beaverpy/MSELoss.py
 src/beaverpy/MaxPool2D.py
 src/beaverpy/ReLU.py
 src/beaverpy/Sigmoid.py
 src/beaverpy/Softmax.py
+src/beaverpy/__init__.py
 src/beaverpy.egg-info/PKG-INFO
 src/beaverpy.egg-info/SOURCES.txt
 src/beaverpy.egg-info/dependency_links.txt
 src/beaverpy.egg-info/top_level.txt
 tests/test_Conv2D.py
 tests/test_CosineSimilarity.py
 tests/test_Linear.py
```

### Comparing `beaverpy-0.0.1/tests/test_Conv2D.py` & `beaverpy-0.0.2/tests/test_Conv2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_CosineSimilarity.py` & `beaverpy-0.0.2/tests/test_CosineSimilarity.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_Linear.py` & `beaverpy-0.0.2/tests/test_Linear.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_MSELoss.py` & `beaverpy-0.0.2/tests/test_MSELoss.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_MaxPool2D.py` & `beaverpy-0.0.2/tests/test_MaxPool2D.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_ReLU.py` & `beaverpy-0.0.2/tests/test_ReLU.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_Sigmoid.py` & `beaverpy-0.0.2/tests/test_Sigmoid.py`

 * *Files identical despite different names*

### Comparing `beaverpy-0.0.1/tests/test_Softmax.py` & `beaverpy-0.0.2/tests/test_Softmax.py`

 * *Files identical despite different names*

