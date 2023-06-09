# Comparing `tmp/hpolib_extractor-1.0.0-py3-none-any.whl.zip` & `tmp/hpolib_extractor-2.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,11 @@
-Zip file size: 6790 bytes, number of entries: 7
--rw-rw-r--  2.0 unx      330 b- defN 23-Jun-08 08:53 hpolib_extractor/__init__.py
--rw-rw-r--  2.0 unx     2720 b- defN 23-Jun-08 08:42 hpolib_extractor/extractor.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      312 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      601 b- defN 23-Jun-08 08:56 hpolib_extractor-1.0.0.dist-info/RECORD
-7 files, 14832 bytes uncompressed, 5714 bytes compressed:  61.5%
+Zip file size: 9680 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jun-09 13:14 hpolib_extractor/__init__.py
+-rw-rw-r--  2.0 unx     1791 b- defN 23-Jun-09 13:54 hpolib_extractor/base_extractor.py
+-rw-rw-r--  2.0 unx     4255 b- defN 23-Jun-09 14:01 hpolib_extractor/hpobench.py
+-rw-rw-r--  2.0 unx     2760 b- defN 23-Jun-09 13:49 hpolib_extractor/hpolib.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      335 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      774 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/RECORD
+9 files, 21211 bytes uncompressed, 8334 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -1,22 +1,28 @@
 Filename: hpolib_extractor/__init__.py
 Comment: 
 
-Filename: hpolib_extractor/extractor.py
+Filename: hpolib_extractor/base_extractor.py
 Comment: 
 
-Filename: hpolib_extractor-1.0.0.dist-info/LICENSE
+Filename: hpolib_extractor/hpobench.py
 Comment: 
 
-Filename: hpolib_extractor-1.0.0.dist-info/METADATA
+Filename: hpolib_extractor/hpolib.py
 Comment: 
 
-Filename: hpolib_extractor-1.0.0.dist-info/WHEEL
+Filename: hpolib_extractor-2.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: hpolib_extractor-1.0.0.dist-info/top_level.txt
+Filename: hpolib_extractor-2.0.0.dist-info/METADATA
 Comment: 
 
-Filename: hpolib_extractor-1.0.0.dist-info/RECORD
+Filename: hpolib_extractor-2.0.0.dist-info/WHEEL
+Comment: 
+
+Filename: hpolib_extractor-2.0.0.dist-info/top_level.txt
+Comment: 
+
+Filename: hpolib_extractor-2.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpolib_extractor/__init__.py

```diff
@@ -1,12 +1,16 @@
-from hpolib_extractor.extractor import extract
+from hpolib_extractor.hpobench import extract_hpobench
+from hpolib_extractor.hpolib import extract_hpolib
 
 
-__version__ = "1.0.0"
+__version__ = "2.0.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/hpolib-extractor/"
 
 
-__all__ = ["extract"]
+__all__ = [
+    "extract_hpobench",
+    "extract_hpolib",
+]
```

## Comparing `hpolib_extractor/extractor.py` & `hpolib_extractor/hpolib.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,71 @@
-import itertools
+from __future__ import annotations
+
 import json
 import os
 import pickle
-from typing import List
 
 import h5py
 
+from hpolib_extractor.base_extractor import BaseExtractor
+
 import numpy as np
 
 from tqdm import tqdm
 
 
-SEARCH_SPACE = {
-    "init_lr": [5e-4, 1e-3, 5e-3, 1e-2, 5e-2, 1e-1],
-    "lr_schedule": ["cosine", "const"],
-    "batch_size": [8, 16, 32, 64],
+SEARCH_SPACE: dict[str, list[int | float | str]] = {
     "activation_fn_1": ["relu", "tanh"],
     "activation_fn_2": ["relu", "tanh"],
+    "batch_size": [8, 16, 32, 64],
     "dropout_1": [0.0, 0.3, 0.6],
     "dropout_2": [0.0, 0.3, 0.6],
+    "init_lr": [5e-4, 1e-3, 5e-3, 1e-2, 5e-2, 1e-1],
+    "lr_schedule": ["cosine", "const"],
     "n_units_1": [16, 32, 64, 128, 256, 512],
     "n_units_2": [16, 32, 64, 128, 256, 512],
 }
+VALUE_IDENTIFIERS = {k: {v: i for i, v in enumerate(vals)} for k, vals in SEARCH_SPACE.items()}
+KEY_ORDER: list[str] = list(SEARCH_SPACE.keys())
 DATASET_NAMES = ["slice_localization", "protein_structure", "naval_propulsion", "parkinsons_telemonitoring"]
-N_ENTRIES = np.prod([len(vs) for vs in SEARCH_SPACE.values()])
 
 
-class HPOLibExtractor:
-    def __init__(self, dataset_id: int, data_dir: str, epochs: List[int] = [100]):
+class HPOLibExtractor(BaseExtractor):
+    _URL = "http://ml4aad.org/wp-content/uploads/2019/01/fcnet_tabular_benchmarks.tar.gz"
+    _BUDGETS = list(range(1, 101))
+    _SEARCH_SPACE = SEARCH_SPACE.copy()
+    _N_SEEDS = 4
+    _KEY_ORDER = KEY_ORDER[:]
+    _VALUE_IDENTIFIERS = VALUE_IDENTIFIERS.copy()
+
+    def __init__(self, dataset_id: int, data_dir: str, epochs: list[int]):
         self._dataset_name = DATASET_NAMES[dataset_id]
-        path = os.path.join(data_dir, f"fcnet_{self._dataset_name}_data.hdf5")
-        if not os.path.exists(path):
-            raise FileNotFoundError(
-                f"{path} does not exist. Please make sure that you already download and "
-                f"locate the datasets at {path}"
-            )
-
-        self._db = h5py.File(path, "r")
-        epoch_array = np.array(epochs)
-        if not np.all((1 <= epoch_array) & (epoch_array) <= 100):
-            raise ValueError("Epoch must be in [1, 100].")
-
-        self._epochs_id = [e - 1 for e in np.sort(epochs)]
-        self._collected_data = {}
-
-    @property
-    def dataset_name(self) -> str:
-        return self._dataset_name
+        data_path = os.path.join(data_dir, f"fcnet_{self._dataset_name}_data.hdf5")
+        super().__init__(data_path=data_path, epochs=np.sort(epochs))
+
+        self._db = h5py.File(data_path, "r")
+        self._epochs -= 1
 
     def collect(self) -> None:
         # max_epoch: 99, min_epoch: 0
         loss_key = "valid_mse"
         runtime_key = "runtime"
         n_params_key = "n_params"
-        n_seeds = 4
-        for it in tqdm(itertools.product(*(list(v) for v in SEARCH_SPACE.values())), total=N_ENTRIES):
+        for it in tqdm(self._get_iterator(), total=self.n_total):
+            config_id = self._get_config_id(config=it)
             config = {k: v for k, v in zip(SEARCH_SPACE.keys(), it)}
             key = json.dumps(config, sort_keys=True)
             target_data = self._db[key]
-            self._collected_data[key] = {
-                loss_key: [{e: float(target_data[loss_key][s][e]) for e in self._epochs_id} for s in range(n_seeds)],
-                runtime_key: [float(target_data[runtime_key][s]) for s in range(n_seeds)],
+            self._collected_data[config_id] = {
+                loss_key: [{e: float(target_data[loss_key][s][e]) for e in self._epochs} for s in range(self._N_SEEDS)],
+                runtime_key: [float(target_data[runtime_key][s]) for s in range(self._N_SEEDS)],
                 n_params_key: float(target_data[n_params_key][0]),
             }
 
 
-def extract(data_dir: str, epochs: List[int]):
-    for i in range(4):
+def extract_hpolib(data_dir: str, epochs: list[int] = [11, 33, 100]) -> None:
+    for i in range(len(DATASET_NAMES)):
         extractor = HPOLibExtractor(dataset_id=i, epochs=epochs, data_dir=data_dir)
         print(f"Start extracting {extractor.dataset_name}")
         extractor.collect()
         pkl_path = os.path.join(data_dir, f"{extractor.dataset_name}.pkl")
         pickle.dump(extractor._collected_data, open(pkl_path, "wb"))
```

## Comparing `hpolib_extractor-1.0.0.dist-info/LICENSE` & `hpolib_extractor-2.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

