# Comparing `tmp/dowg-0.2.1.tar.gz` & `tmp/dowg-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowg-0.2.1.tar", last modified: Fri Jun  9 14:33:36 2023, max compression
+gzip compressed data, was "dowg-0.2.2.tar", last modified: Fri Jun  9 15:46:06 2023, max compression
```

## Comparing `dowg-0.2.1.tar` & `dowg-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.428413 dowg-0.2.1/
--rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-09 14:33:36.428413 dowg-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.2.1/README.md
--rw-rw-rw-   0        0        0      552 2023-06-09 14:33:23.000000 dowg-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 14:33:36.428413 dowg-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.389893 dowg-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.416412 dowg-0.2.1/src/dowg/
--rw-rw-rw-   0        0        0     1997 2023-06-09 14:32:32.000000 dowg-0.2.1/src/dowg/CoordinateDoWG.py
--rw-rw-rw-   0        0        0     2009 2023-06-09 14:32:56.000000 dowg-0.2.1/src/dowg/ScalarDoWG.py
--rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.2.1/src/dowg/__init__.py
--rw-rw-rw-   0        0        0      838 2023-06-09 03:07:12.000000 dowg-0.2.1/src/dowg/clip.py
-drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.427414 dowg-0.2.1/src/dowg.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.458937 dowg-0.2.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-09 15:46:06.457936 dowg-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.2.2/README.md
+-rw-rw-rw-   0        0        0      552 2023-06-09 15:45:46.000000 dowg-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 15:46:06.458937 dowg-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.431882 dowg-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.446417 dowg-0.2.2/src/dowg/
+-rw-rw-rw-   0        0        0     1988 2023-06-09 15:43:56.000000 dowg-0.2.2/src/dowg/CoordinateDoWG.py
+-rw-rw-rw-   0        0        0     2005 2023-06-09 15:45:29.000000 dowg-0.2.2/src/dowg/ScalarDoWG.py
+-rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.2.2/src/dowg/__init__.py
+-rw-rw-rw-   0        0        0      660 2023-06-09 15:41:00.000000 dowg-0.2.2/src/dowg/clip.py
+drwxrwxrwx   0        0        0        0 2023-06-09 15:46:06.456938 dowg-0.2.2/src/dowg.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 15:46:06.000000 dowg-0.2.2/src/dowg.egg-info/top_level.txt
```

### Comparing `dowg-0.2.1/LICENSE` & `dowg-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dowg-0.2.1/PKG-INFO` & `dowg-0.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.2.1
+Version: 0.2.2
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dowg-0.2.1/pyproject.toml` & `dowg-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dowg"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Patrick Shanahan", email="patrick.e.shanahan@gmail.com" },
 ]
 description = "DoWG parameter-free adaptive optimizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dowg-0.2.1/src/dowg/CoordinateDoWG.py` & `dowg-0.2.2/src/dowg/CoordinateDoWG.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,12 +45,12 @@
 
                 with torch.no_grad():
                     state['rt2'] = torch.max(state['rt2'], (p - state['x0']) ** 2)
                     rt2, vt = state['rt2'], state['vt']
                     vt.add_(rt2 * grad ** 2)
                     gt_hat = rt2 * clip_gradient(p, group['clip'])
                     denom = vt.sqrt().add_(group['epsilon'])
-                    p.data.addcdiv_(gt_hat, denom, value=-1.0)
+                p.addcdiv_(gt_hat, denom, value=-1.0)
         return loss
```

### Comparing `dowg-0.2.1/src/dowg/ScalarDoWG.py` & `dowg-0.2.2/src/dowg/ScalarDoWG.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 
 from .clip import clip_gradient
 
 
 class ScalarDoWG(torch.optim.Optimizer):
-    def __init__(self, params, eps=1e-4, clip=0.5, *args, **kwargs):
+    def __init__(self, params, eps=1e-4, clip=0.01, *args, **kwargs):
         defaults = dict(epsilon=1-eps, lr=1, clip=clip)
         self.epsilon = 1-eps
         super(ScalarDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         
         state = self.state
@@ -44,9 +44,9 @@
                 state["vt"] += state["rt2"] * grad_sq_norm
                 rt2, vt = state["rt2"], state["vt"]
     
             for group in self.param_groups:
                 for p in group["params"]:
                     gt_hat = rt2 * clip_gradient(p.grad.data.clone(), group["clip"])
                     denom = torch.sqrt(vt).add_(group["epsilon"])
-                    p.data.addcdiv_(gt_hat, denom, value=-1.0)
+                    p.addcdiv_(gt_hat, denom, value=-1.0)
         return loss
```

### Comparing `dowg-0.2.1/src/dowg/clip.py` & `dowg-0.2.2/src/dowg/clip.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 import torch
 
 
-def clip_gradient(grad, k):
-    """Clips the top k% of the gradients in terms of absolute value.
-
+def clip_gradient(grad:torch.tensor, k: float = 1.0):
+    """Clips the gradients based on the kth percentile of their absolute values.
+    
     Args:
         grad (torch.Tensor): The gradients to be clipped.
-        k (float): The percentage of gradients to keep.
+        k (float): The percentile of gradients to keep.
 
     Returns:
         torch.Tensor: The clipped gradients.
     """
-    if len(grad.size()) < 2 or grad.size(1) < 2:
-        return grad
-
-    if k >= 1.0:
-        return grad
-
-    # Compute the threshold
-    #print(f"grad: {grad}, k: {k}, grad.size(1): {grad.size(1)}, int(grad.size(1) * (1 - k))): {int(grad.size(1) * (1 - k))}")
-    threshold = torch.kthvalue(torch.abs(grad), int(grad.size(1) * k), dim=1)[0]
-
-    # Clip the gradients
-    clipped_grad = torch.clamp(torch.abs(grad), max=threshold.unsqueeze(1))
-    clipped_grad *= torch.sign(grad)
+    assert k >= 0 and k <= 1, "k must be between 0 and 1. Got {}".format(k)
 
-    return clipped_grad
+    grad = grad.flatten()
+    kth = int(k * len(grad))
+    threshold = torch.topk(torch.abs(grad), kth)[0][-1]
+    clipped_grad = torch.clamp(grad, -threshold, threshold)
+    return clipped_grad.reshape(grad.shape)
```

### Comparing `dowg-0.2.1/src/dowg.egg-info/PKG-INFO` & `dowg-0.2.2/src/dowg.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.2.1
+Version: 0.2.2
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

