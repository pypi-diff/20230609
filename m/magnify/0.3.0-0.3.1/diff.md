# Comparing `tmp/magnify-0.3.0.tar.gz` & `tmp/magnify-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magnify-0.3.0.tar", max compression
+gzip compressed data, was "magnify-0.3.1.tar", max compression
```

## Comparing `magnify-0.3.0.tar` & `magnify-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.3.0/README.md
--rw-r--r--   0        0        0     1649 2023-06-02 00:28:59.358390 magnify-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      246 2023-06-02 00:26:47.659424 magnify-0.3.0/src/magnify/__init__.py
--rw-r--r--   0        0        0     4571 2023-06-02 00:21:13.635636 magnify-0.3.0/src/magnify/filter.py
--rw-r--r--   0        0        0    26578 2023-06-02 00:21:04.883425 magnify-0.3.0/src/magnify/find.py
--rw-r--r--   0        0        0     3573 2023-06-02 00:26:38.835224 magnify-0.3.0/src/magnify/identify.py
--rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.3.0/src/magnify/pipeline.py
--rw-r--r--   0        0        0      317 2023-05-31 18:04:36.204183 magnify-0.3.0/src/magnify/plot/__init__.py
--rw-r--r--   0        0        0     2339 2023-06-02 00:19:24.832979 magnify-0.3.0/src/magnify/plot/image.py
--rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.3.0/src/magnify/plot/ndplot.py
--rw-r--r--   0        0        0     2483 2023-05-31 18:00:09.258919 magnify-0.3.0/src/magnify/plot/relation.py
--rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.3.0/src/magnify/plot/style.py
--rw-r--r--   0        0        0     1017 2023-06-02 00:16:42.972866 magnify-0.3.0/src/magnify/postprocess.py
--rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.3.0/src/magnify/preprocess.py
--rw-r--r--   0        0        0    15093 2023-05-31 01:36:36.512603 magnify-0.3.0/src/magnify/reader.py
--rw-r--r--   0        0        0     3339 2023-06-02 00:16:33.476618 magnify-0.3.0/src/magnify/registry.py
--rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.3.0/src/magnify/stitch.py
--rw-r--r--   0        0        0     2639 2023-06-02 00:20:14.442200 magnify-0.3.0/src/magnify/utils.py
--rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 magnify-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       49 2023-03-06 19:55:56.379475 magnify-0.3.1/README.md
+-rw-r--r--   0        0        0     1649 2023-06-09 01:23:36.583799 magnify-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      246 2023-06-09 01:23:55.932244 magnify-0.3.1/src/magnify/__init__.py
+-rw-r--r--   0        0        0     4571 2023-06-02 00:21:13.635636 magnify-0.3.1/src/magnify/filter.py
+-rw-r--r--   0        0        0    26578 2023-06-02 00:21:04.883425 magnify-0.3.1/src/magnify/find.py
+-rw-r--r--   0        0        0     3757 2023-06-02 01:37:51.173200 magnify-0.3.1/src/magnify/identify.py
+-rw-r--r--   0        0        0     1406 2023-04-14 21:30:07.711891 magnify-0.3.1/src/magnify/pipeline.py
+-rw-r--r--   0        0        0      317 2023-05-31 18:04:36.204183 magnify-0.3.1/src/magnify/plot/__init__.py
+-rw-r--r--   0        0        0     2339 2023-06-02 00:19:24.832979 magnify-0.3.1/src/magnify/plot/image.py
+-rw-r--r--   0        0        0     1855 2023-05-11 01:21:29.027397 magnify-0.3.1/src/magnify/plot/ndplot.py
+-rw-r--r--   0        0        0     2483 2023-05-31 18:00:09.258919 magnify-0.3.1/src/magnify/plot/relation.py
+-rw-r--r--   0        0        0      650 2023-05-11 02:30:53.591879 magnify-0.3.1/src/magnify/plot/style.py
+-rw-r--r--   0        0        0     1017 2023-06-02 00:16:42.972866 magnify-0.3.1/src/magnify/postprocess.py
+-rw-r--r--   0        0        0     1736 2023-04-14 21:30:15.276066 magnify-0.3.1/src/magnify/preprocess.py
+-rw-r--r--   0        0        0    15093 2023-05-31 01:36:36.512603 magnify-0.3.1/src/magnify/reader.py
+-rw-r--r--   0        0        0     3339 2023-06-02 00:16:33.476618 magnify-0.3.1/src/magnify/registry.py
+-rw-r--r--   0        0        0     1077 2023-05-23 23:12:37.145369 magnify-0.3.1/src/magnify/stitch.py
+-rw-r--r--   0        0        0     2639 2023-06-02 00:20:14.442200 magnify-0.3.1/src/magnify/utils.py
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 magnify-0.3.1/PKG-INFO
```

### Comparing `magnify-0.3.0/pyproject.toml` & `magnify-0.3.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magnify"
-version = "0.3.0"
+version = "0.3.1"
 description = "A microscopy image processing toolkit."
 authors = ["Karl Krauth <karl.krauth@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
 opencv-python = [
```

### Comparing `magnify-0.3.0/src/magnify/filter.py` & `magnify-0.3.1/src/magnify/filter.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/find.py` & `magnify-0.3.1/src/magnify/find.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/identify.py` & `magnify-0.3.1/src/magnify/identify.py`

 * *Files 14% similar despite different names*

```diff
@@ -45,24 +45,30 @@
     intensities = sel.roi.where(sel.fg).mean(dim=["roi_x", "roi_y"]).to_numpy()
     volumes = np.linalg.lstsq(sp.T, intensities.T, rcond=None)[0].T
     ratios = volumes / volumes[:, ref_idx : ref_idx + 1]
     assay = assay.assign_coords(ln=("ln", df["name"]))
     assay["ln_vol"] = (("mark", "ln"), volumes)
     assay["ln_ratio"] = (("mark", "ln"), ratios)
 
-    tags = sklearn.cluster.DBSCAN(eps=1e-3, min_samples=5).fit_predict(ratios[:, 1:])
+    tags = sklearn.cluster.DBSCAN(eps=3e-3, min_samples=5).fit_predict(ratios[:, 1:])
     # tags = model.predict(ratios[:, 1:])
     X = ratios[:, 1:]
 
     means = np.zeros((num_codes, ratios.shape[1] - 1))
     covs = np.zeros((num_codes, ratios.shape[1] - 1, ratios.shape[1] - 1))
     unique_tags, counts = np.unique(tags[tags != -1], return_counts=True)
-    for i, t in enumerate(unique_tags[np.argsort(counts)][-num_codes:]):
-        means[i] = np.mean(X[tags == t], axis=0)
-        covs[i] = np.cov(X[tags == t], rowvar=False)
+    sorted_tags = unique_tags[np.argsort(counts)]
+    for i in range(num_codes):
+        if i <= len(sorted_tags):
+            t = sorted_tags[-i]
+            means[i] = np.mean(X[tags == t], axis=0)
+            covs[i] = np.cov(X[tags == t], rowvar=False)
+        else:
+            means[i] = np.mean(X, axis=0)
+            covs[i] = np.cov(X, rowvar=False)
     proportions = np.ones(num_codes + 1)
     proportions[-1] = 0.1
     proportions /= proportions.sum()
     lower = np.min(X, axis=0)
     upper = np.max(X, axis=0)
     for i in range(300):
         probs = []
```

### Comparing `magnify-0.3.0/src/magnify/pipeline.py` & `magnify-0.3.1/src/magnify/pipeline.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/plot/image.py` & `magnify-0.3.1/src/magnify/plot/image.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/plot/ndplot.py` & `magnify-0.3.1/src/magnify/plot/ndplot.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/plot/relation.py` & `magnify-0.3.1/src/magnify/plot/relation.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/plot/style.py` & `magnify-0.3.1/src/magnify/plot/style.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/postprocess.py` & `magnify-0.3.1/src/magnify/postprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/preprocess.py` & `magnify-0.3.1/src/magnify/preprocess.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/reader.py` & `magnify-0.3.1/src/magnify/reader.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/registry.py` & `magnify-0.3.1/src/magnify/registry.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/stitch.py` & `magnify-0.3.1/src/magnify/stitch.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/src/magnify/utils.py` & `magnify-0.3.1/src/magnify/utils.py`

 * *Files identical despite different names*

### Comparing `magnify-0.3.0/PKG-INFO` & `magnify-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magnify
-Version: 0.3.0
+Version: 0.3.1
 Summary: A microscopy image processing toolkit.
 Author: Karl Krauth
 Author-email: karl.krauth@gmail.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

