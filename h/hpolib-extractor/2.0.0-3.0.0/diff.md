# Comparing `tmp/hpolib_extractor-2.0.0-py3-none-any.whl.zip` & `tmp/hpolib_extractor-3.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9680 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      427 b- defN 23-Jun-09 13:14 hpolib_extractor/__init__.py
+Zip file size: 9695 bytes, number of entries: 9
+-rw-rw-r--  2.0 unx      427 b- defN 23-Jun-09 15:46 hpolib_extractor/__init__.py
 -rw-rw-r--  2.0 unx     1791 b- defN 23-Jun-09 13:54 hpolib_extractor/base_extractor.py
--rw-rw-r--  2.0 unx     4255 b- defN 23-Jun-09 14:01 hpolib_extractor/hpobench.py
--rw-rw-r--  2.0 unx     2760 b- defN 23-Jun-09 13:49 hpolib_extractor/hpolib.py
--rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx      335 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       17 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      774 b- defN 23-Jun-09 14:07 hpolib_extractor-2.0.0.dist-info/RECORD
-9 files, 21211 bytes uncompressed, 8334 bytes compressed:  60.7%
+-rw-rw-r--  2.0 unx     4255 b- defN 23-Jun-09 15:46 hpolib_extractor/hpobench.py
+-rw-rw-r--  2.0 unx     2802 b- defN 23-Jun-09 15:46 hpolib_extractor/hpolib.py
+-rw-rw-r--  2.0 unx    10760 b- defN 23-Jun-09 15:47 hpolib_extractor-3.0.0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      335 b- defN 23-Jun-09 15:47 hpolib_extractor-3.0.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-09 15:47 hpolib_extractor-3.0.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       17 b- defN 23-Jun-09 15:47 hpolib_extractor-3.0.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      774 b- defN 23-Jun-09 15:47 hpolib_extractor-3.0.0.dist-info/RECORD
+9 files, 21253 bytes uncompressed, 8349 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: hpolib_extractor/hpobench.py
 Comment: 
 
 Filename: hpolib_extractor/hpolib.py
 Comment: 
 
-Filename: hpolib_extractor-2.0.0.dist-info/LICENSE
+Filename: hpolib_extractor-3.0.0.dist-info/LICENSE
 Comment: 
 
-Filename: hpolib_extractor-2.0.0.dist-info/METADATA
+Filename: hpolib_extractor-3.0.0.dist-info/METADATA
 Comment: 
 
-Filename: hpolib_extractor-2.0.0.dist-info/WHEEL
+Filename: hpolib_extractor-3.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: hpolib_extractor-2.0.0.dist-info/top_level.txt
+Filename: hpolib_extractor-3.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: hpolib_extractor-2.0.0.dist-info/RECORD
+Filename: hpolib_extractor-3.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hpolib_extractor/__init__.py

```diff
@@ -1,12 +1,12 @@
 from hpolib_extractor.hpobench import extract_hpobench
 from hpolib_extractor.hpolib import extract_hpolib
 
 
-__version__ = "2.0.0"
+__version__ = "3.0.0"
 __copyright__ = "Copyright (C) 2023 Shuhei Watanabe"
 __licence__ = "Apache-2.0 License"
 __author__ = "Shuhei Watanabe"
 __author_email__ = "shuhei.watanabe.utokyo@gmail.com"
 __url__ = "https://github.com/nabenabe0928/hpolib-extractor/"
```

## hpolib_extractor/hpobench.py

```diff
@@ -90,17 +90,17 @@
 
         # subsample has only one value (subsample=1.0)
         self._db = pq.read_table(data_path)["result"].to_pylist()
         self._target_keys = target_keys[:]
 
     def collect(self) -> None:
         start = 0
-        indices = np.array([
-            np.arange(self._N_SEEDS) + self._N_SEEDS * self._BUDGETS.index(e) for e in self._epochs
-        ]).flatten()
+        indices = np.array(
+            [np.arange(self._N_SEEDS) + self._N_SEEDS * self._BUDGETS.index(e) for e in self._epochs]
+        ).flatten()
 
         for it in tqdm(self._get_iterator(), total=self.n_total):
             config_id = self._get_config_id(config=it)
             entry = {k: [{} for _ in range(self._N_SEEDS)] for k in self._target_keys}
 
             results = self._db[start:start + N_FOR_CONFIG]
             assert len(results) == N_FOR_CONFIG
```

## hpolib_extractor/hpolib.py

```diff
@@ -52,15 +52,17 @@
         n_params_key = "n_params"
         for it in tqdm(self._get_iterator(), total=self.n_total):
             config_id = self._get_config_id(config=it)
             config = {k: v for k, v in zip(SEARCH_SPACE.keys(), it)}
             key = json.dumps(config, sort_keys=True)
             target_data = self._db[key]
             self._collected_data[config_id] = {
-                loss_key: [{e: float(target_data[loss_key][s][e]) for e in self._epochs} for s in range(self._N_SEEDS)],
+                loss_key: [
+                    {e + 1: float(target_data[loss_key][s][e]) for e in self._epochs} for s in range(self._N_SEEDS)
+                ],
                 runtime_key: [float(target_data[runtime_key][s]) for s in range(self._N_SEEDS)],
                 n_params_key: float(target_data[n_params_key][0]),
             }
 
 
 def extract_hpolib(data_dir: str, epochs: list[int] = [11, 33, 100]) -> None:
     for i in range(len(DATASET_NAMES)):
```

## Comparing `hpolib_extractor-2.0.0.dist-info/LICENSE` & `hpolib_extractor-3.0.0.dist-info/LICENSE`

 * *Files identical despite different names*

