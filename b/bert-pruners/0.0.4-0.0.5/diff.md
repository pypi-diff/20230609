# Comparing `tmp/bert_pruners-0.0.4.tar.gz` & `tmp/bert_pruners-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bert_pruners-0.0.4.tar", last modified: Thu Jun  8 16:17:07 2023, max compression
+gzip compressed data, was "bert_pruners-0.0.5.tar", last modified: Fri Jun  9 08:48:26 2023, max compression
```

## Comparing `bert_pruners-0.0.4.tar` & `bert_pruners-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-08 16:17:07.774032 bert_pruners-0.0.4/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2023-06-08 16:12:26.000000 bert_pruners-0.0.4/MANIFEST.in
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      350 2023-06-08 16:17:07.774032 bert_pruners-0.0.4/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       86 2023-06-08 16:12:26.000000 bert_pruners-0.0.4/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-08 16:17:07.754032 bert_pruners-0.0.4/bert_pruners/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-08 16:15:58.000000 bert_pruners-0.0.4/bert_pruners/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1816 2023-06-08 16:12:26.000000 bert_pruners-0.0.4/bert_pruners/bert_pruner.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      688 2023-06-08 16:12:26.000000 bert_pruners-0.0.4/bert_pruners/main.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-08 16:17:07.774032 bert_pruners-0.0.4/bert_pruners.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      350 2023-06-08 16:17:07.000000 bert_pruners-0.0.4/bert_pruners.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      322 2023-06-08 16:17:07.000000 bert_pruners-0.0.4/bert_pruners.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-08 16:17:07.000000 bert_pruners-0.0.4/bert_pruners.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-06-08 16:17:07.000000 bert_pruners-0.0.4/bert_pruners.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2023-06-08 16:17:07.000000 bert_pruners-0.0.4/bert_pruners.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-06-08 16:17:07.000000 bert_pruners-0.0.4/bert_pruners.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-08 16:17:07.774032 bert_pruners-0.0.4/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      675 2023-06-08 16:12:26.000000 bert_pruners-0.0.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 08:48:26.536347 bert_pruners-0.0.5/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       43 2023-06-09 08:44:30.000000 bert_pruners-0.0.5/MANIFEST.in
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      350 2023-06-09 08:48:26.536347 bert_pruners-0.0.5/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       86 2023-06-09 08:44:30.000000 bert_pruners-0.0.5/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 08:48:26.532348 bert_pruners-0.0.5/bert_pruners/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-06-09 08:48:03.000000 bert_pruners-0.0.5/bert_pruners/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2044 2023-06-09 08:44:56.000000 bert_pruners-0.0.5/bert_pruners/bert_pruner.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    15039 2023-06-09 08:44:57.000000 bert_pruners-0.0.5/bert_pruners/factory.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      815 2023-06-09 08:44:58.000000 bert_pruners-0.0.5/bert_pruners/main.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-06-09 08:48:26.536347 bert_pruners-0.0.5/bert_pruners.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      350 2023-06-09 08:48:26.000000 bert_pruners-0.0.5/bert_pruners.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      346 2023-06-09 08:48:26.000000 bert_pruners-0.0.5/bert_pruners.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-06-09 08:48:26.000000 bert_pruners-0.0.5/bert_pruners.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       54 2023-06-09 08:48:26.000000 bert_pruners-0.0.5/bert_pruners.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       24 2023-06-09 08:48:26.000000 bert_pruners-0.0.5/bert_pruners.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       13 2023-06-09 08:48:26.000000 bert_pruners-0.0.5/bert_pruners.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-06-09 08:48:26.536347 bert_pruners-0.0.5/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      675 2023-06-09 08:44:55.000000 bert_pruners-0.0.5/setup.py
```

### Comparing `bert_pruners-0.0.4/bert_pruners/bert_pruner.py` & `bert_pruners-0.0.5/bert_pruners/bert_pruner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 from transformers import AutoModelForQuestionAnswering
 from torch.nn.utils import prune
 import torch
+from factory import MagnitudeModelFactory, PostPrunedModelFactory, BlockPrunedModelFactory
 
 class BertPruner:
-    def __init__(self, model_name: str, saved_dir: str, sparsity: float):
-        self.model = AutoModelForQuestionAnswering.from_pretrained(model_name)
+    def __init__(self, model_name: str, saved_dir: str, method: str, value: float):
+        self.model_name = model_name
         self.saved_dir = saved_dir
-        self.sparsity = sparsity
-    def prune_and_save(self):
-        for name, module in self.model.named_modules():
-            if isinstance(module, torch.nn.Linear):
-                # replace l1_unstructured pruning with l2structured for magnitude pruning
-                # prune.l1_unstructured(module, name='weight', amount=self.sparsity)
-                prune.ln_structured(module, name='weight', amount=self.sparsity, n=2, dim=0)
+        self.method = method
+        self.value = value
+        self.model = self.get_model()
+
+    def get_model(self):
+        if self.method == "magnitude":
+            factory = MagnitudeModelFactory(self.model_name, self.value)
+        elif self.method == "post":
+            factory = PostPrunedModelFactory(self.model_name, self.value)
+        elif self.method == "block":
+            factory = BlockPrunedModelFactory(self.model_name, self.value)
+        else:
+            raise ValueError(f"Unknown pruning method: {self.method}")
 
+        return factory.create_model()
+
+    def prune_and_save(self):
         # it fixed using previous code (2 potential changes: eval model/input_id)
         input_shape = (1, 512)
         input_ids = torch.zeros(input_shape, dtype=torch.long, device=self.model.device)
         attention_mask = torch.ones(input_shape, dtype=torch.long, device=self.model.device)
         token_type_ids = torch.zeros(input_shape, dtype=torch.long, device=self.model.device)
 
         torch.onnx.export(self.model, (input_ids, attention_mask, token_type_ids),
```

### Comparing `bert_pruners-0.0.4/bert_pruners/main.py` & `bert_pruners-0.0.5/bert_pruners/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,14 @@
 from .bert_pruner import BertPruner
 
 def main():
     parser = argparse.ArgumentParser(description='BERT pruner')
     parser.add_argument('--model_name', default='xihajun/krai-mlperf-inference-v3.0-bert-pytorch-fp32-squad-v1.1', type=str, help='Path to save the pruned model')
     parser.add_argument('--saved_dir', type=str, help='Path to save the pruned model')
     parser.add_argument('--sparsity', type=float, default=0.5, help='Desired sparsity of the pruned model')
+    parser.add_argument('--method', type=str, default='magnitude', help='Select different pruning methods')
     args = parser.parse_args()
-
-    pruner = BertPruner(model_name=args.model_name, saved_dir=args.saved_dir, sparsity=args.sparsity)
+    pruner = BertPruner(model_name=args.model_name, saved_dir=args.saved_dir, sparsity=args.sparsity, method=args.method)
     pruner.prune_and_save()
 
 if __name__ == "__main__":
     main()
```

### Comparing `bert_pruners-0.0.4/setup.py` & `bert_pruners-0.0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="bert_pruners",
-    version="0.0.4",
+    version="0.0.5",
     author="xihajun",
     author_email="junfan@krai.ai",
     description="Pruning BERT models",
     url="https://github.com/xihajun/bert_pruners",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

