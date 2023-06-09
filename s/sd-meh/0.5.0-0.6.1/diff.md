# Comparing `tmp/sd_meh-0.5.0.tar.gz` & `tmp/sd_meh-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sd_meh-0.5.0.tar", max compression
+gzip compressed data, was "sd_meh-0.6.1.tar", max compression
```

## Comparing `sd_meh-0.5.0.tar` & `sd_meh-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-06-08 08:32:25.972422 sd_meh-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0     1896 2023-06-08 08:32:25.972422 sd_meh-0.5.0/README.md
--rw-r--r--   0        0        0      390 2023-06-08 08:32:25.972422 sd_meh-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       22 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/__init__.py
--rw-r--r--   0        0        0    11589 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/merge.py
--rw-r--r--   0        0        0     5353 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/merge_methods.py
--rw-r--r--   0        0        0     1521 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/model.py
--rw-r--r--   0        0        0    83404 2023-06-08 08:32:25.972422 sd_meh-0.5.0/sd_meh/rebasin.py
--rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 sd_meh-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-09 08:30:05.757563 sd_meh-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     1878 2023-06-09 08:30:05.757563 sd_meh-0.6.1/README.md
+-rw-r--r--   0        0        0      390 2023-06-09 08:30:05.757563 sd_meh-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/__init__.py
+-rw-r--r--   0        0        0    11653 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/merge.py
+-rw-r--r--   0        0        0     6566 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/merge_methods.py
+-rw-r--r--   0        0        0     1521 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/model.py
+-rw-r--r--   0        0        0    83404 2023-06-09 08:30:05.757563 sd_meh-0.6.1/sd_meh/rebasin.py
+-rw-r--r--   0        0        0     2402 1970-01-01 00:00:00.000000 sd_meh-0.6.1/PKG-INFO
```

### Comparing `sd_meh-0.5.0/LICENSE.txt` & `sd_meh-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sd_meh-0.5.0/README.md` & `sd_meh-0.6.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
-  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution|multiply_difference|distribution_crossover|euclidean_add_difference|ties_add_difference]
+  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|top_k_tensor_sum|multiply_difference|distribution_crossover|euclidean_add_difference|ties_add_difference]
   -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
@@ -50,9 +50,9 @@
 
 - gpu merging
 - prune model before merging (and un-prune at the end)
 - weights matching aka re-basin
 - weights clipping
 - registered pypi package
 - block merge
-- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`, `distribution_crossover`, `multiply_difference`, `euclidean_add_difference`, `ties_add_difference`
+- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `top_k_tensor_sum`, `distribution_crossover`, `multiply_difference`, `euclidean_add_difference`, `ties_add_difference`
 - `fp16` and `fp32`
```

### Comparing `sd_meh-0.5.0/sd_meh/merge.py` & `sd_meh-0.6.1/sd_meh/merge.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,17 @@
     "cond_stage_model.transformer.final_layer_norm.": "cond_stage_model.transformer.text_model.final_layer_norm.",
 }
 
 
 def fix_clip(model: Dict) -> Dict:
     if KEY_POSITION_IDS in model.keys():
         model[KEY_POSITION_IDS] = torch.tensor(
-            [list(range(MAX_TOKENS))], dtype=torch.int64
+            [list(range(MAX_TOKENS))],
+            dtype=torch.int64,
+            device=model[KEY_POSITION_IDS].device,
         )
 
     return model
 
 
 def fix_key(model: Dict, key: str) -> Dict:
     for nk in NAI_KEYS:
```

### Comparing `sd_meh-0.5.0/sd_meh/merge_methods.py` & `sd_meh-0.6.1/sd_meh/merge_methods.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import torch
 from torch import Tensor
+import math
+from typing import Tuple
 
 
 __all__ = [
     "weighted_sum",
     "weighted_subtraction",
     "tensor_sum",
     "add_difference",
     "sum_twice",
     "triple_sum",
     "euclidean_add_difference",
     "multiply_difference",
-    "transmogrify_distribution",
+    "top_k_tensor_sum",
     "similarity_add_difference",
     "distribution_crossover",
     "ties_add_difference",
 ]
 
 
 EPSILON = 1e-10  # Define a small constant EPSILON to prevent division by zero
@@ -64,45 +66,86 @@
 ) -> Tensor:
     return (1 - alpha - beta) * a + alpha * b + beta * c
 
 
 def euclidean_add_difference(
     a: Tensor, b: Tensor, c: Tensor, alpha: float, **kwargs
 ) -> Tensor:
-    distance = (a - c) ** 2 + alpha * (b - c) ** 2
-    try:
-        distance = torch.sqrt(distance)
-    except RuntimeError:
-        distance = torch.sqrt(distance.float()).half()
-    distance = torch.copysign(distance, (a - c) + alpha * (b - c))
-
-    a_norm = torch.linalg.norm(a - c)
-    b_norm = torch.linalg.norm(b - c)
-    target_norm = (1 - alpha / 2) * a_norm + (alpha / 2) * b_norm
+    a_diff = a.float() - c.float()
+    b_diff = b.float() - c.float()
+    a_diff /= torch.linalg.norm(a_diff)
+    b_diff /= torch.linalg.norm(b_diff)
+
+    distance = (1 - alpha) * a_diff**2 + alpha * b_diff**2
+    distance = torch.sqrt(distance)
+    sum_diff = weighted_sum(a.float(), b.float(), alpha) - c.float()
+    distance = torch.copysign(distance, sum_diff)
+
+    target_norm = torch.linalg.norm(sum_diff)
     return c + distance / torch.linalg.norm(distance) * target_norm
 
 
 def multiply_difference(
-    a: Tensor, b: Tensor, c: Tensor, alpha: float, **kwargs
+    a: Tensor, b: Tensor, c: Tensor, alpha: float, beta: float, **kwargs
 ) -> Tensor:
-    difference = torch.abs((a - c) * (b - c))
-    try:
-        difference = torch.sqrt(difference)
-    except RuntimeError:
-        difference = torch.sqrt(difference.float()).half()
-    difference = torch.copysign(torch.sqrt(difference), a + b - 2 * c)
-    return c + alpha * difference
+    diff_a = torch.pow(torch.abs(a.float() - c), (1 - alpha))
+    diff_b = torch.pow(torch.abs(b.float() - c), alpha)
+    difference = torch.copysign(diff_a * diff_b, weighted_sum(a, b, beta) - c)
+    return c + difference.to(c.dtype)
 
 
-def transmogrify_distribution(a: Tensor, b: Tensor, alpha: float, **kwargs) -> Tensor:
-    a_dist = torch.msort(torch.flatten(a))
+def top_k_tensor_sum(
+    a: Tensor, b: Tensor, alpha: float, beta: float, **kwargs
+) -> Tensor:
+    a_flat = torch.flatten(a)
+    a_dist = torch.msort(a_flat)
     b_indices = torch.argsort(torch.flatten(b), stable=True)
-    a_redist = torch.gather(a_dist, 0, torch.argsort(b_indices))
-    a_trans = a_redist.reshape(a.shape)
-    return (1 - alpha) * b + alpha * a_trans
+    redist_indices = torch.argsort(b_indices)
+
+    start_i, end_i, region_is_inverted = ratio_to_region(alpha, beta, torch.numel(a))
+    start_top_k = kth_abs_value(a_dist, start_i)
+    end_top_k = kth_abs_value(a_dist, end_i)
+
+    indices_mask = (start_top_k < torch.abs(a_dist)) & (torch.abs(a_dist) <= end_top_k)
+    if region_is_inverted:
+        indices_mask = ~indices_mask
+    indices_mask = torch.gather(indices_mask.float(), 0, redist_indices)
+
+    a_redist = torch.gather(a_dist, 0, redist_indices)
+    a_redist = (1 - indices_mask) * a_flat + indices_mask * a_redist
+    return a_redist.reshape_as(a)
+
+
+def kth_abs_value(a: Tensor, k: int) -> Tensor:
+    if k <= 0:
+        return torch.tensor(-1, device=a.device)
+    else:
+        return torch.kthvalue(torch.abs(a), k)[0]
+
+
+def ratio_to_region(width: float, offset: float, n: int) -> Tuple[int, int, bool]:
+    if width < 0:
+        offset += width
+        width = -width
+    width = min(width, 1)
+
+    if offset < 0:
+        offset = 1 + offset - int(offset)
+    offset = math.fmod(offset, 1.0)
+
+    if width + offset <= 1:
+        inverted = False
+        start = offset * n
+        end = (width + offset) * n
+    else:
+        inverted = True
+        start = (width + offset - 1) * n
+        end = offset * n
+
+    return round(start), round(end), inverted
 
 
 def similarity_add_difference(
     a: Tensor, b: Tensor, c: Tensor, alpha: float, beta: float, **kwargs
 ) -> Tensor:
     threshold = torch.maximum(torch.abs(a), torch.abs(b))
     similarity = ((a * b / threshold**2) + 1) / 2
```

### Comparing `sd_meh-0.5.0/sd_meh/model.py` & `sd_meh-0.6.1/sd_meh/model.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.5.0/sd_meh/rebasin.py` & `sd_meh-0.6.1/sd_meh/rebasin.py`

 * *Files identical despite different names*

### Comparing `sd_meh-0.5.0/PKG-INFO` & `sd_meh-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sd-meh
-Version: 0.5.0
+Version: 0.6.1
 Summary: stable diffusion merging execution helper
 Home-page: https://github.com/s1dlx/meh
 License: MIT
 Author: s1dlx
 Author-email: s1dlx@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -42,15 +42,15 @@
 ```
 Usage: merge_models.py [OPTIONS]
 
 Options:
   -a, --model_a TEXT
   -b, --model_b TEXT
   -c, --model_c TEXT
-  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|transmogrify_distribution|multiply_difference|distribution_crossover|euclidean_add_difference|ties_add_difference]
+  -m, --merging_method [weighted_sum|add_difference|weighted_subtraction|sum_twice|triple_sum|tensor_sum|similarity_add_difference|top_k_tensor_sum|multiply_difference|distribution_crossover|euclidean_add_difference|ties_add_difference]
   -wc, --weights_clip
   -p, --precision INTEGER
   -o, --output_path TEXT
   -f, --output_format [safetensors|ckpt]
   -wa, --weights_alpha TEXT
   -ba, --base_alpha FLOAT
   -wb, --weights_beta TEXT
@@ -66,10 +66,10 @@
 
 - gpu merging
 - prune model before merging (and un-prune at the end)
 - weights matching aka re-basin
 - weights clipping
 - registered pypi package
 - block merge
-- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `transmogrify_distribution`, `distribution_crossover`, `multiply_difference`, `euclidean_add_difference`, `ties_add_difference`
+- merging methods: `weighted_sum`, `add_difference`, `weighted_subtraction`, `sum_twice`, `triple_sum`, `tensor_sum`, `similarity_add_difference`, `top_k_tensor_sum`, `distribution_crossover`, `multiply_difference`, `euclidean_add_difference`, `ties_add_difference`
 - `fp16` and `fp32`
```

