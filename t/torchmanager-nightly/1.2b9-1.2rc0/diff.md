# Comparing `tmp/torchmanager_nightly-1.2b9.tar.gz` & `tmp/torchmanager_nightly-1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchmanager_nightly-1.2b9.tar", max compression
+gzip compressed data, was "torchmanager_nightly-1.2rc0.tar", max compression
```

## Comparing `torchmanager_nightly-1.2b9.tar` & `torchmanager_nightly-1.2rc0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1318 2023-03-14 14:54:20.813363 torchmanager_nightly-1.2b9/LICENSE
--rw-r--r--   0        0        0      672 2023-06-08 15:47:06.822835 torchmanager_nightly-1.2b9/pyproject.toml
--rw-r--r--   0        0        0      290 2023-06-08 13:42:56.795253 torchmanager_nightly-1.2b9/torchmanager/__init__.py
--rw-r--r--   0        0        0    11928 2023-06-08 15:47:06.823206 torchmanager_nightly-1.2b9/torchmanager/basic.py
--rw-r--r--   0        0        0      638 2023-06-08 13:42:56.796148 torchmanager_nightly-1.2b9/torchmanager/callbacks/__init__.py
--rw-r--r--   0        0        0     4444 2023-06-08 13:42:56.796532 torchmanager_nightly-1.2b9/torchmanager/callbacks/callback.py
--rw-r--r--   0        0        0     4628 2023-06-01 19:00:58.329930 torchmanager_nightly-1.2b9/torchmanager/callbacks/ckpt.py
--rw-r--r--   0        0        0     3523 2023-06-01 19:00:58.330042 torchmanager_nightly-1.2b9/torchmanager/callbacks/dynamic.py
--rw-r--r--   0        0        0     1608 2023-06-01 19:00:58.330150 torchmanager_nightly-1.2b9/torchmanager/callbacks/early_stop.py
--rw-r--r--   0        0        0     4642 2023-06-08 13:42:56.797025 torchmanager_nightly-1.2b9/torchmanager/callbacks/experiment.py
--rw-r--r--   0        0        0     2224 2023-06-01 19:00:58.330768 torchmanager_nightly-1.2b9/torchmanager/callbacks/lr.py
--rw-r--r--   0        0        0     2599 2023-06-08 13:42:56.797496 torchmanager_nightly-1.2b9/torchmanager/callbacks/tensorboard.py
--rw-r--r--   0        0        0      586 2023-06-08 15:47:06.823480 torchmanager_nightly-1.2b9/torchmanager/compatibility.py
--rw-r--r--   0        0        0       26 2023-06-08 13:42:56.798472 torchmanager_nightly-1.2b9/torchmanager/configs/__init__.py
--rw-r--r--   0        0        0     2980 2023-06-08 15:47:06.823739 torchmanager_nightly-1.2b9/torchmanager/configs/basic.py
--rw-r--r--   0        0        0       85 2023-06-01 19:00:58.331061 torchmanager_nightly-1.2b9/torchmanager/data/__init__.py
--rw-r--r--   0        0        0     6968 2023-06-08 13:42:56.799616 torchmanager_nightly-1.2b9/torchmanager/data/dataset.py
--rw-r--r--   0        0        0     2238 2023-06-08 13:42:56.799838 torchmanager_nightly-1.2b9/torchmanager/data/sliding.py
--rw-r--r--   0        0        0      156 2023-06-08 13:42:56.800621 torchmanager_nightly-1.2b9/torchmanager/losses/__init__.py
--rw-r--r--   0        0        0     5557 2023-06-08 15:47:06.823928 torchmanager_nightly-1.2b9/torchmanager/losses/cross_entropy.py
--rw-r--r--   0        0        0     1047 2023-06-08 13:42:56.801183 torchmanager_nightly-1.2b9/torchmanager/losses/dice.py
--rw-r--r--   0        0        0     5740 2023-06-08 15:47:06.824071 torchmanager_nightly-1.2b9/torchmanager/losses/loss.py
--rw-r--r--   0        0        0     3156 2023-06-08 15:47:06.824201 torchmanager_nightly-1.2b9/torchmanager/losses/mse.py
--rw-r--r--   0        0        0      351 2023-06-08 15:47:06.824339 torchmanager_nightly-1.2b9/torchmanager/metrics/__init__.py
--rw-r--r--   0        0        0     4098 2023-06-08 15:47:06.824464 torchmanager_nightly-1.2b9/torchmanager/metrics/accuracy.py
--rw-r--r--   0        0        0     3651 2023-06-08 15:47:06.824750 torchmanager_nightly-1.2b9/torchmanager/metrics/conf_met.py
--rw-r--r--   0        0        0     5139 2023-06-08 13:42:56.804542 torchmanager_nightly-1.2b9/torchmanager/metrics/extractor.py
--rw-r--r--   0        0        0     2070 2023-06-08 13:42:56.804802 torchmanager_nightly-1.2b9/torchmanager/metrics/iou.py
--rw-r--r--   0        0        0     3937 2023-06-08 15:47:06.824930 torchmanager_nightly-1.2b9/torchmanager/metrics/metric.py
--rw-r--r--   0        0        0     2307 2023-06-08 13:42:56.805688 torchmanager_nightly-1.2b9/torchmanager/metrics/similarity.py
--rw-r--r--   0        0        0     8702 2023-06-08 15:47:06.825235 torchmanager_nightly-1.2b9/torchmanager/testing.py
--rw-r--r--   0        0        0       96 2023-06-08 13:42:56.806384 torchmanager_nightly-1.2b9/torchmanager/train/__init__.py
--rw-r--r--   0        0        0     4964 2023-06-01 19:00:58.336017 torchmanager_nightly-1.2b9/torchmanager/train/checkpoint.py
--rw-r--r--   0        0        0      694 2023-06-08 13:42:56.806863 torchmanager_nightly-1.2b9/torchmanager/train/learning_rate.py
--rw-r--r--   0        0        0    13483 2023-06-08 15:47:06.825551 torchmanager_nightly-1.2b9/torchmanager/training.py
--rw-r--r--   0        0        0      459 2023-06-08 13:42:56.807626 torchmanager_nightly-1.2b9/torchmanager_core/__init__.py
--rw-r--r--   0        0        0      109 2023-06-08 13:42:56.808055 torchmanager_nightly-1.2b9/torchmanager_core/devices/__init__.py
--rw-r--r--   0        0        0     4879 2023-06-08 13:42:56.808230 torchmanager_nightly-1.2b9/torchmanager_core/devices/device.py
--rw-r--r--   0        0        0      264 2023-06-01 19:00:58.337503 torchmanager_nightly-1.2b9/torchmanager_core/devices/protocols.py
--rw-r--r--   0        0        0      153 2023-06-01 19:00:58.337794 torchmanager_nightly-1.2b9/torchmanager_core/errors/__init__.py
--rw-r--r--   0        0        0      350 2023-06-01 19:00:58.338065 torchmanager_nightly-1.2b9/torchmanager_core/errors/runtime.py
--rw-r--r--   0        0        0      669 2023-06-01 19:00:58.338329 torchmanager_nightly-1.2b9/torchmanager_core/errors/train.py
--rw-r--r--   0        0        0     3076 2023-06-08 15:47:06.825701 torchmanager_nightly-1.2b9/torchmanager_core/protocols.py
--rw-r--r--   0        0        0       44 2023-06-08 13:42:56.808831 torchmanager_nightly-1.2b9/torchmanager_core/random/__init__.py
--rw-r--r--   0        0        0     1029 2023-06-08 13:42:56.809065 torchmanager_nightly-1.2b9/torchmanager_core/random/seed.py
--rw-r--r--   0        0        0      204 2023-06-01 19:00:58.338499 torchmanager_nightly-1.2b9/torchmanager_core/typing.py
--rw-r--r--   0        0        0     5256 2023-06-08 15:47:06.825892 torchmanager_nightly-1.2b9/torchmanager_core/version.py
--rw-r--r--   0        0        0      439 2023-06-08 13:42:56.809755 torchmanager_nightly-1.2b9/torchmanager_core/view/__init__.py
--rw-r--r--   0        0        0      313 2023-06-01 19:00:58.338878 torchmanager_nightly-1.2b9/torchmanager_core/view/protocols.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2b9/PKG-INFO
+-rw-r--r--   0        0        0     1318 2023-03-14 14:54:20.813363 torchmanager_nightly-1.2rc0/LICENSE
+-rw-r--r--   0        0        0      670 2023-06-09 15:04:44.567465 torchmanager_nightly-1.2rc0/pyproject.toml
+-rw-r--r--   0        0        0      290 2023-06-09 15:04:44.567870 torchmanager_nightly-1.2rc0/torchmanager/__init__.py
+-rw-r--r--   0        0        0    11928 2023-06-09 15:04:44.568285 torchmanager_nightly-1.2rc0/torchmanager/basic.py
+-rw-r--r--   0        0        0      638 2023-06-09 15:04:44.568657 torchmanager_nightly-1.2rc0/torchmanager/callbacks/__init__.py
+-rw-r--r--   0        0        0     4444 2023-06-09 15:04:44.568985 torchmanager_nightly-1.2rc0/torchmanager/callbacks/callback.py
+-rw-r--r--   0        0        0     4628 2023-06-01 19:00:58.329930 torchmanager_nightly-1.2rc0/torchmanager/callbacks/ckpt.py
+-rw-r--r--   0        0        0     3523 2023-06-01 19:00:58.330042 torchmanager_nightly-1.2rc0/torchmanager/callbacks/dynamic.py
+-rw-r--r--   0        0        0     1608 2023-06-01 19:00:58.330150 torchmanager_nightly-1.2rc0/torchmanager/callbacks/early_stop.py
+-rw-r--r--   0        0        0     4642 2023-06-09 15:04:44.569313 torchmanager_nightly-1.2rc0/torchmanager/callbacks/experiment.py
+-rw-r--r--   0        0        0     2224 2023-06-01 19:00:58.330768 torchmanager_nightly-1.2rc0/torchmanager/callbacks/lr.py
+-rw-r--r--   0        0        0     2599 2023-06-09 15:04:44.569694 torchmanager_nightly-1.2rc0/torchmanager/callbacks/tensorboard.py
+-rw-r--r--   0        0        0      586 2023-06-09 15:04:44.570009 torchmanager_nightly-1.2rc0/torchmanager/compatibility.py
+-rw-r--r--   0        0        0       26 2023-06-09 15:04:44.570282 torchmanager_nightly-1.2rc0/torchmanager/configs/__init__.py
+-rw-r--r--   0        0        0     2980 2023-06-09 15:04:44.570764 torchmanager_nightly-1.2rc0/torchmanager/configs/basic.py
+-rw-r--r--   0        0        0       85 2023-06-01 19:00:58.331061 torchmanager_nightly-1.2rc0/torchmanager/data/__init__.py
+-rw-r--r--   0        0        0     6968 2023-06-09 15:04:44.571103 torchmanager_nightly-1.2rc0/torchmanager/data/dataset.py
+-rw-r--r--   0        0        0     2238 2023-06-09 15:04:44.571417 torchmanager_nightly-1.2rc0/torchmanager/data/sliding.py
+-rw-r--r--   0        0        0      156 2023-06-09 15:04:44.571764 torchmanager_nightly-1.2rc0/torchmanager/losses/__init__.py
+-rw-r--r--   0        0        0     5557 2023-06-09 15:04:44.572050 torchmanager_nightly-1.2rc0/torchmanager/losses/cross_entropy.py
+-rw-r--r--   0        0        0     1047 2023-06-09 15:04:44.572372 torchmanager_nightly-1.2rc0/torchmanager/losses/dice.py
+-rw-r--r--   0        0        0     5740 2023-06-09 15:04:44.572701 torchmanager_nightly-1.2rc0/torchmanager/losses/loss.py
+-rw-r--r--   0        0        0     3156 2023-06-09 15:04:44.573084 torchmanager_nightly-1.2rc0/torchmanager/losses/mse.py
+-rw-r--r--   0        0        0      351 2023-06-09 15:04:44.573433 torchmanager_nightly-1.2rc0/torchmanager/metrics/__init__.py
+-rw-r--r--   0        0        0     4145 2023-06-09 15:04:44.573765 torchmanager_nightly-1.2rc0/torchmanager/metrics/accuracy.py
+-rw-r--r--   0        0        0     3769 2023-06-09 15:04:44.574052 torchmanager_nightly-1.2rc0/torchmanager/metrics/conf_met.py
+-rw-r--r--   0        0        0     5139 2023-06-09 15:04:44.574289 torchmanager_nightly-1.2rc0/torchmanager/metrics/extractor.py
+-rw-r--r--   0        0        0     2070 2023-06-09 15:04:44.574441 torchmanager_nightly-1.2rc0/torchmanager/metrics/iou.py
+-rw-r--r--   0        0        0     3937 2023-06-09 15:04:44.574746 torchmanager_nightly-1.2rc0/torchmanager/metrics/metric.py
+-rw-r--r--   0        0        0     2307 2023-06-09 15:04:44.574988 torchmanager_nightly-1.2rc0/torchmanager/metrics/similarity.py
+-rw-r--r--   0        0        0     8710 2023-06-09 15:04:44.575236 torchmanager_nightly-1.2rc0/torchmanager/testing.py
+-rw-r--r--   0        0        0       96 2023-06-09 15:04:44.575522 torchmanager_nightly-1.2rc0/torchmanager/train/__init__.py
+-rw-r--r--   0        0        0     4964 2023-06-01 19:00:58.336017 torchmanager_nightly-1.2rc0/torchmanager/train/checkpoint.py
+-rw-r--r--   0        0        0      694 2023-06-09 15:04:44.575804 torchmanager_nightly-1.2rc0/torchmanager/train/learning_rate.py
+-rw-r--r--   0        0        0    13483 2023-06-09 15:04:44.576140 torchmanager_nightly-1.2rc0/torchmanager/training.py
+-rw-r--r--   0        0        0      459 2023-06-09 15:04:44.576450 torchmanager_nightly-1.2rc0/torchmanager_core/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-09 15:04:44.576756 torchmanager_nightly-1.2rc0/torchmanager_core/devices/__init__.py
+-rw-r--r--   0        0        0     4879 2023-06-09 15:04:44.576905 torchmanager_nightly-1.2rc0/torchmanager_core/devices/device.py
+-rw-r--r--   0        0        0      264 2023-06-01 19:00:58.337503 torchmanager_nightly-1.2rc0/torchmanager_core/devices/protocols.py
+-rw-r--r--   0        0        0      153 2023-06-01 19:00:58.337794 torchmanager_nightly-1.2rc0/torchmanager_core/errors/__init__.py
+-rw-r--r--   0        0        0      350 2023-06-01 19:00:58.338065 torchmanager_nightly-1.2rc0/torchmanager_core/errors/runtime.py
+-rw-r--r--   0        0        0      669 2023-06-01 19:00:58.338329 torchmanager_nightly-1.2rc0/torchmanager_core/errors/train.py
+-rw-r--r--   0        0        0     3076 2023-06-09 15:04:44.577160 torchmanager_nightly-1.2rc0/torchmanager_core/protocols.py
+-rw-r--r--   0        0        0       44 2023-06-09 15:04:44.577391 torchmanager_nightly-1.2rc0/torchmanager_core/random/__init__.py
+-rw-r--r--   0        0        0     1029 2023-06-09 15:04:44.577618 torchmanager_nightly-1.2rc0/torchmanager_core/random/seed.py
+-rw-r--r--   0        0        0      204 2023-06-01 19:00:58.338499 torchmanager_nightly-1.2rc0/torchmanager_core/typing.py
+-rw-r--r--   0        0        0     6017 2023-06-09 15:04:48.647525 torchmanager_nightly-1.2rc0/torchmanager_core/version.py
+-rw-r--r--   0        0        0      439 2023-06-09 15:04:44.578258 torchmanager_nightly-1.2rc0/torchmanager_core/view/__init__.py
+-rw-r--r--   0        0        0      313 2023-06-01 19:00:58.338878 torchmanager_nightly-1.2rc0/torchmanager_core/view/protocols.py
+-rw-r--r--   0        0        0      691 1970-01-01 00:00:00.000000 torchmanager_nightly-1.2rc0/PKG-INFO
```

### Comparing `torchmanager_nightly-1.2b9/LICENSE` & `torchmanager_nightly-1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/pyproject.toml` & `torchmanager_nightly-1.2rc0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "torchmanager-nightly"
-version = "1.2b9"
-description = "PyTorch Training Manager v1.2 (Beta 9)"
+version = "1.2rc"
+description = "PyTorch Training Manager v1.2 (Release Candidate)"
 authors = ["Qisheng He <Qisheng.He@wayne.edu>"]
 repository = "https://github.com/kisonho/torchmanager.git"
 packages = [
     { include = "torchmanager" },
     { include = "torchmanager_core" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-shutil = "*"
 torch = "*"
 tqdm = "*"
 
 [tool.poetry.optional-dependencies]
 scipy = { version = "*" }
 tensorboard = { version = "*" }
```

### Comparing `torchmanager_nightly-1.2b9/torchmanager/basic.py` & `torchmanager_nightly-1.2rc0/torchmanager/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/__init__.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/callback.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/ckpt.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/ckpt.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/dynamic.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/dynamic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/early_stop.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/early_stop.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/experiment.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/experiment.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/lr.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/lr.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/callbacks/tensorboard.py` & `torchmanager_nightly-1.2rc0/torchmanager/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/compatibility.py` & `torchmanager_nightly-1.2rc0/torchmanager/compatibility.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/configs/basic.py` & `torchmanager_nightly-1.2rc0/torchmanager/configs/basic.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/data/dataset.py` & `torchmanager_nightly-1.2rc0/torchmanager/data/dataset.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/data/sliding.py` & `torchmanager_nightly-1.2rc0/torchmanager/data/sliding.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/losses/cross_entropy.py` & `torchmanager_nightly-1.2rc0/torchmanager/losses/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/losses/dice.py` & `torchmanager_nightly-1.2rc0/torchmanager/losses/dice.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/losses/loss.py` & `torchmanager_nightly-1.2rc0/torchmanager/losses/loss.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/losses/mse.py` & `torchmanager_nightly-1.2rc0/torchmanager/losses/mse.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/metrics/accuracy.py` & `torchmanager_nightly-1.2rc0/torchmanager/metrics/accuracy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from torchmanager_core import torch, Version
 from torchmanager_core.protocols import Reduction
-from torchmanager_core.typing import Optional, Tuple
+from torchmanager_core.typing import Optional
 
 from .conf_met import BinaryConfusionMetric
 from .metric import Metric
 
 
 class Accuracy(Metric):
     """
@@ -71,15 +71,15 @@
         target = target.argmax(dim=self._dim)
         return super().forward(input, target)
 
 
 class F1(BinaryConfusionMetric):
     """The F1 metrics"""
 
-    def forward(self, tp: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
+    def forward(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
         # calculate precision and recall
         precision = tp / (tp + fp + self._eps)
         recall = tp / (tp + fn + self._eps)
 
         # calculate F1
         f1 = 2 * precision * recall / (precision + recall + self._eps)
         f1 = torch.mean(f1)
@@ -121,16 +121,16 @@
         else:
             return error
 
 
 class Precision(BinaryConfusionMetric):
     """The Precision metrics"""
 
-    def forward_metric(self, tp: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
+    def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
         return tp / (tp + fp + self._eps)
 
 
 class Recall(BinaryConfusionMetric):
     """The Recall metrics"""
 
-    def forward_metric(self, tp: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
+    def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
         return tp / (tp + fn + self._eps)
```

### Comparing `torchmanager_nightly-1.2b9/torchmanager/metrics/conf_met.py` & `torchmanager_nightly-1.2rc0/torchmanager/metrics/conf_met.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,31 +13,32 @@
 
     - Methods to implement:
         - forward_metric: The main method that accepts TP, FP, and FN as `torch.Tensor` and returns the final metric as `torch.Tensor`
     """
     _dim: int
     _eps: float
 
-    def __init__(self, dim: int = -1, *, eps: float=1e-7):
-        super().__init__()
+    def __init__(self, dim: int = -1, *, eps: float=1e-7, target: Optional[str] = None):
+        super().__init__(target=target)
         self._dim = dim
         self._eps = eps
 
     def forward(self, input: torch.Tensor, target: torch.Tensor) -> torch.Tensor:
         # argmax input
         input = input.argmax(dim=self._dim)
 
         # calculate TP, FP, and FN
         tp = torch.sum(target * input, dim=0)
+        tn = ((1 - target) * (1 - input)).sum(dim=0)
         fp = torch.sum((1 - target) * input, dim=0)
         fn = torch.sum(target * (1 - input), dim=0)
-        return self.forward_metric(tp, fp, fn)
+        return self.forward_metric(tp, tn, fp, fn)
 
     @abc.abstractmethod
-    def forward_metric(self, tp: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
+    def forward_metric(self, tp: torch.Tensor, tn: torch.Tensor, fp: torch.Tensor, fn: torch.Tensor) -> torch.Tensor:
         return NotImplemented
 
 
 class ConfusionMetrics(Metric, abc.ABC):
     """
     The metric that forward confusion metrics calculated by given `input` and `target` as final `input` in `forward` method
```

### Comparing `torchmanager_nightly-1.2b9/torchmanager/metrics/extractor.py` & `torchmanager_nightly-1.2rc0/torchmanager/metrics/extractor.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/metrics/iou.py` & `torchmanager_nightly-1.2rc0/torchmanager/metrics/iou.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/metrics/metric.py` & `torchmanager_nightly-1.2rc0/torchmanager/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/metrics/similarity.py` & `torchmanager_nightly-1.2rc0/torchmanager/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/testing.py` & `torchmanager_nightly-1.2rc0/torchmanager/testing.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
 
         - Parameters:
             - x_train: The testing data in `torch.Tensor`
             - y_train: The testing label in `torch.Tensor`
         - Returns: A `dict` of validation summary
         """
         # forward pass
-        y, _ = self.forward(x_test)
+        y, _ = self.forward(x_test, y_test)
 
         # forward metrics
         for name, fn in self.compiled_metrics.items():
             if name.startswith("val_"):
                 name = name.replace("val_", "")
             elif "loss" in name:
                 continue
```

### Comparing `torchmanager_nightly-1.2b9/torchmanager/train/checkpoint.py` & `torchmanager_nightly-1.2rc0/torchmanager/train/checkpoint.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/train/learning_rate.py` & `torchmanager_nightly-1.2rc0/torchmanager/train/learning_rate.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager/training.py` & `torchmanager_nightly-1.2rc0/torchmanager/training.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager_core/devices/device.py` & `torchmanager_nightly-1.2rc0/torchmanager_core/devices/device.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager_core/errors/train.py` & `torchmanager_nightly-1.2rc0/torchmanager_core/errors/train.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager_core/protocols.py` & `torchmanager_nightly-1.2rc0/torchmanager_core/protocols.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager_core/random/seed.py` & `torchmanager_nightly-1.2rc0/torchmanager_core/random/seed.py`

 * *Files identical despite different names*

### Comparing `torchmanager_nightly-1.2b9/torchmanager_core/version.py` & `torchmanager_nightly-1.2rc0/torchmanager_core/version.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,36 +4,40 @@
 from .view import warnings
 
 
 class Version:
     main_version: int
     minor_version: int
     pre_release: Optional[str]
+    pre_release_version: int
     sub_version: int
 
     def __init__(self, v: Any, /) -> None:
         # convert to string
         version_str = str(v)
 
         # format version
         if version_str.startswith('v'):
             version_str = version_str[1:]
 
         # split pre-release version
-        pre_release_parts = version_str.split('a')
-        if len(pre_release_parts) > 1:
-            self.pre_release = 'a' + pre_release_parts[1]
-            version_str = pre_release_parts[0]
-        else:
+        if 'a' in version_str:
+            pre_release_parts = version_str.split('a')
+            self.pre_release = 'a'
+        elif 'b' in version_str:
             pre_release_parts = version_str.split('b')
-            if len(pre_release_parts) > 1:
-                self.pre_release = 'b' + pre_release_parts[1]
-                version_str = pre_release_parts[0]
-            else:
-                self.pre_release = "0"
+            self.pre_release = 'b'
+        elif 'rc' in version_str:
+            pre_release_parts = version_str.split('rc')
+            self.pre_release = 'rc'
+        else:
+            pre_release_parts = [version_str, "0"]
+            self.pre_release = None
+        version_str = pre_release_parts[0]
+        self.pre_release_version = int(pre_release_parts[1]) if pre_release_parts[1] != '' else 1
 
         # split version
         version_parts = version_str.split('.')
         self.main_version = int(version_parts[0])
         self.minor_version = int(version_parts[1])
         self.sub_version = int(version_parts[2]) if len(version_parts) > 2 else 0
 
@@ -45,58 +49,64 @@
             version_str += f".{self.sub_version}"
         if self.pre_release is not None:
             version_str += self.pre_release
         return version_str
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, Version):
-            return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release
+            return self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release == other.pre_release and self.pre_release_version == other.pre_release_version
         else:
             other = Version(str(other))
             return self.__eq__(other)
 
     def __lt__(self, other: Any) -> bool:
-        if isinstance(other, Version):
-            if self.main_version < other.main_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version < other.minor_version:
-                    return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version < other.sub_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
-                return self.sub_version < other.sub_version
-            return False
-        else:
+        # convert to version
+        if not isinstance(other, Version):
             other = Version(str(other))
-            return self.__lt__(other)
 
-    def __gt__(self, other: Any) -> bool:
-        if isinstance(other, Version):
-            if self.main_version > other.main_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version > other.minor_version:
+        # check version
+        if self.main_version < other.main_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version < other.minor_version:
                 return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version > other.sub_version:
-                return True
-            elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
-                return self.sub_version > other.sub_version
-            return False
-        else:
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version < other.sub_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
+            return self.pre_release < other.pre_release or (self.pre_release == other.pre_release and self.pre_release_version < other.pre_release_version)
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None:
+            return True
+        return False
+
+    def __gt__(self, other: Any) -> bool:
+        # convert to version
+        if not isinstance(other, Version):
             other = Version(str(other))
-            return self.__gt__(other)
+
+        # check version
+        if self.main_version > other.main_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version > other.minor_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version > other.sub_version:
+            return True
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and self.pre_release is not None and other.pre_release is not None:
+            return self.pre_release > other.pre_release or (self.pre_release == other.pre_release and self.pre_release_version > other.pre_release_version)
+        elif self.main_version == other.main_version and self.minor_version == other.minor_version and self.sub_version == other.sub_version and other.pre_release is not None:
+            return True
+        return False
 
     def __le__(self, other: Any) -> bool:
         return self == other or self < other
 
     def __ge__(self, other: Any) -> bool:
         return self == other or self > other
 
 
 API = Version("v1.2")
-CURRENT = Version("v1.2b9")
+CURRENT = Version("v1.2rc")
 DESCRIPTION: str = "PyTorch Training Manager {CURRENT}"
 
 
 class VersionError(SystemError):
     def __init__(self, method_name: str, maximum_supported_version: str) -> None:
         super().__init__(f"`{method_name}` has been deprecated and removed from version {maximum_supported_version}. Current version: {CURRENT}.")
```

### Comparing `torchmanager_nightly-1.2b9/PKG-INFO` & `torchmanager_nightly-1.2rc0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: torchmanager-nightly
-Version: 1.2b9
-Summary: PyTorch Training Manager v1.2 (Beta 9)
+Version: 1.2rc0
+Summary: PyTorch Training Manager v1.2 (Release Candidate)
 Home-page: https://github.com/kisonho/torchmanager.git
 Author: Qisheng He
 Author-email: Qisheng.He@wayne.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: all
 Provides-Extra: scipy
 Provides-Extra: tensorboard
-Requires-Dist: shutil
 Requires-Dist: torch
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/kisonho/torchmanager.git
```

