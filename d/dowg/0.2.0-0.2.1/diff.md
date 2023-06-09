# Comparing `tmp/dowg-0.2.0.tar.gz` & `tmp/dowg-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowg-0.2.0.tar", last modified: Fri Jun  9 03:09:26 2023, max compression
+gzip compressed data, was "dowg-0.2.1.tar", last modified: Fri Jun  9 14:33:36 2023, max compression
```

## Comparing `dowg-0.2.0.tar` & `dowg-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:26.450891 dowg-0.2.0/
--rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-09 03:09:26.449890 dowg-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.2.0/README.md
--rw-rw-rw-   0        0        0      552 2023-06-09 03:09:12.000000 dowg-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-09 03:09:26.450891 dowg-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:26.431377 dowg-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:26.437891 dowg-0.2.0/src/dowg/
--rw-rw-rw-   0        0        0     2035 2023-06-08 16:26:29.000000 dowg-0.2.0/src/dowg/CoordinateDoWG.py
--rw-rw-rw-   0        0        0     2028 2023-06-09 03:06:59.000000 dowg-0.2.0/src/dowg/ScalarDoWG.py
--rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.2.0/src/dowg/__init__.py
--rw-rw-rw-   0        0        0      838 2023-06-09 03:07:12.000000 dowg-0.2.0/src/dowg/clip.py
-drwxrwxrwx   0        0        0        0 2023-06-09 03:09:26.448891 dowg-0.2.0/src/dowg.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-09 03:09:26.000000 dowg-0.2.0/src/dowg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-09 03:09:26.000000 dowg-0.2.0/src/dowg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 03:09:26.000000 dowg-0.2.0/src/dowg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-09 03:09:26.000000 dowg-0.2.0/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.428413 dowg-0.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-09 14:33:36.428413 dowg-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.2.1/README.md
+-rw-rw-rw-   0        0        0      552 2023-06-09 14:33:23.000000 dowg-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-09 14:33:36.428413 dowg-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.389893 dowg-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.416412 dowg-0.2.1/src/dowg/
+-rw-rw-rw-   0        0        0     1997 2023-06-09 14:32:32.000000 dowg-0.2.1/src/dowg/CoordinateDoWG.py
+-rw-rw-rw-   0        0        0     2009 2023-06-09 14:32:56.000000 dowg-0.2.1/src/dowg/ScalarDoWG.py
+-rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.2.1/src/dowg/__init__.py
+-rw-rw-rw-   0        0        0      838 2023-06-09 03:07:12.000000 dowg-0.2.1/src/dowg/clip.py
+drwxrwxrwx   0        0        0        0 2023-06-09 14:33:36.427414 dowg-0.2.1/src/dowg.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-09 14:33:36.000000 dowg-0.2.1/src/dowg.egg-info/top_level.txt
```

### Comparing `dowg-0.2.0/LICENSE` & `dowg-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dowg-0.2.0/PKG-INFO` & `dowg-0.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.2.0
+Version: 0.2.1
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dowg-0.2.0/pyproject.toml` & `dowg-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dowg"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Patrick Shanahan", email="patrick.e.shanahan@gmail.com" },
 ]
 description = "DoWG parameter-free adaptive optimizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dowg-0.2.0/src/dowg/CoordinateDoWG.py` & `dowg-0.2.1/src/dowg/CoordinateDoWG.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,45 +9,45 @@
         Args:
             params (iterable): iterable of parameters to optimize or dicts defining
                 parameter groups
             eps (float, optional): term added to the denominator to improve
                 numerical stability (default: 1e-8)
         """
 
-    def __init__(self, params, epsilon=1e-8, clip=0.5, *args, **kwargs):
-        defaults = dict(epsilon=epsilon, lr=1, clip=clip)
+    def __init__(self, params, eps=1e-8, clip=0.5, *args, **kwargs):
+        defaults = dict(epsilon=1-eps, lr=1, clip=clip)
         super(CoordinateDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         """Performs a single optimization step.
 
         Args:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
         """
         loss = None
         if closure is not None:
             loss = closure()
 
         for group in self.param_groups:
-            with torch.no_grad():
-                for p in group['params']:
-                    if p.grad is None:
-                        continue
-                    grad = p.grad.data
-                    state = self.state[p]
-
-                    # Initialize state variables
-                    if 'x0' not in state:
-                        state['x0'] = torch.clone(p).detach()
-                    if 'rt2' not in state:
-                        state['rt2'] = torch.zeros_like(p.data).add_(1e-8)
-                    if 'vt' not in state:
-                        state['vt'] = torch.zeros_like(p.data)
+            for p in group['params']:
+                if p.grad is None:
+                    continue
+                grad = p.grad.data
+                state = self.state[p]
+
+                # Initialize state variables
+                if 'x0' not in state:
+                    state['x0'] = torch.clone(p).detach()
+                if 'rt2' not in state:
+                    state['rt2'] = torch.zeros_like(p.data).add_(group['epsilon'])
+                if 'vt' not in state:
+                    state['vt'] = torch.zeros_like(p.data)
 
+                with torch.no_grad():
                     state['rt2'] = torch.max(state['rt2'], (p - state['x0']) ** 2)
                     rt2, vt = state['rt2'], state['vt']
                     vt.add_(rt2 * grad ** 2)
                     gt_hat = rt2 * clip_gradient(p, group['clip'])
                     denom = vt.sqrt().add_(group['epsilon'])
                     p.data.addcdiv_(gt_hat, denom, value=-1.0)
         return loss
```

### Comparing `dowg-0.2.0/src/dowg/ScalarDoWG.py` & `dowg-0.2.1/src/dowg/ScalarDoWG.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import torch
 
 from .clip import clip_gradient
 
 
 class ScalarDoWG(torch.optim.Optimizer):
-    def __init__(self, params, epsilon=1e-4, clip=0.5, *args, **kwargs):
-        defaults = dict(epsilon=epsilon, lr=1, clip=clip)
-        self.epsilon = epsilon
+    def __init__(self, params, eps=1e-4, clip=0.5, *args, **kwargs):
+        defaults = dict(epsilon=1-eps, lr=1, clip=clip)
+        self.epsilon = 1-eps
         super(ScalarDoWG, self).__init__(params, defaults)
 
     def step(self, closure=None):
         
         state = self.state
         loss = None
         if closure is not None:
             loss = closure()
-        with torch.no_grad():
-            device = self.param_groups[0]["params"][0].device
     
             if "rt2" not in state:
-                state["rt2"] = torch.Tensor([self.epsilon]).to(device)
+                state["rt2"] = torch.Tensor([self.epsilon])
             if "vt" not in state:
-                state["vt"] = torch.Tensor([0]).to(device)
+                state["vt"] = torch.Tensor([0])
     
-            grad_sq_norm = torch.Tensor([0]).to(device)
-            curr_d2 = torch.Tensor([0]).to(device)
+            grad_sq_norm = torch.Tensor([0])
+            curr_d2 = torch.Tensor([0])
     
-            for idx, group in enumerate(self.param_groups):
-                group_state = state[str(idx)]  # convert idx to a string
-                if "x0" not in group_state:
-                    group_state["x0"] = [torch.clone(p) for p in group["params"]]
-    
-                grad_sq_norm += torch.stack(
-                    [(p.grad**2).sum() for p in group["params"]]
-                ).sum()
-                curr_d2 += torch.stack(
-                    [
-                        ((p - p0) ** 2).sum()
-                        for p, p0 in zip(group["params"], group_state["x0"])
-                    ]
-                ).sum()
-    
-            state["rt2"] = torch.max(state["rt2"], curr_d2)
-            state["vt"] += state["rt2"] * grad_sq_norm
-            rt2, vt = state["rt2"], state["vt"]
-    
-        for group in self.param_groups:
-            for p in group["params"]:
-                gt_hat = rt2 * clip_gradient(p.grad.data.clone(), group["clip"])
-                denom = torch.sqrt(vt).add_(group["epsilon"])
-                p.data.addcdiv_(gt_hat, denom, value=-1.0)
+            with torch.no_grad():
+                for idx, group in enumerate(self.param_groups):
+                    group_state = state[str(idx)]  # convert idx to a string
+                    if "x0" not in group_state:
+                        group_state["x0"] = [torch.clone(p) for p in group["params"]]
+        
+                    grad_sq_norm += torch.stack(
+                        [(p.grad**2).sum() for p in group["params"]]
+                    ).sum()
+                    curr_d2 += torch.stack(
+                        [
+                            ((p - p0) ** 2).sum()
+                            for p, p0 in zip(group["params"], group_state["x0"])
+                        ]
+                    ).sum()
+        
+                state["rt2"] = torch.max(state["rt2"], curr_d2)
+                state["vt"] += state["rt2"] * grad_sq_norm
+                rt2, vt = state["rt2"], state["vt"]
+    
+            for group in self.param_groups:
+                for p in group["params"]:
+                    gt_hat = rt2 * clip_gradient(p.grad.data.clone(), group["clip"])
+                    denom = torch.sqrt(vt).add_(group["epsilon"])
+                    p.data.addcdiv_(gt_hat, denom, value=-1.0)
         return loss
```

### Comparing `dowg-0.2.0/src/dowg/clip.py` & `dowg-0.2.1/src/dowg/clip.py`

 * *Files identical despite different names*

### Comparing `dowg-0.2.0/src/dowg.egg-info/PKG-INFO` & `dowg-0.2.1/src/dowg.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.2.0
+Version: 0.2.1
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

