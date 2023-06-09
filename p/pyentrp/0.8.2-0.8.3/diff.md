# Comparing `tmp/pyentrp-0.8.2.tar.gz` & `tmp/pyentrp-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyentrp-0.8.2.tar", max compression
+gzip compressed data, was "pyentrp-0.8.3.tar", max compression
```

## Comparing `pyentrp-0.8.2.tar` & `pyentrp-0.8.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    12117 2023-06-05 12:02:45.510463 pyentrp-0.8.2/LICENSE
--rw-r--r--   0        0        0     1744 2023-06-05 12:02:45.510463 pyentrp-0.8.2/README.md
--rw-r--r--   0        0        0        0 2023-06-05 12:02:45.514463 pyentrp-0.8.2/pyentrp/__init__.py
--rw-r--r--   0        0        0    11701 2023-06-05 12:02:45.514463 pyentrp-0.8.2/pyentrp/entropy.py
--rw-r--r--   0        0        0     1612 2023-06-05 12:02:45.514463 pyentrp-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 pyentrp-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0    12117 2023-06-09 00:53:00.107336 pyentrp-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1744 2023-06-09 00:53:00.107336 pyentrp-0.8.3/README.md
+-rw-r--r--   0        0        0        0 2023-06-09 00:53:00.107336 pyentrp-0.8.3/pyentrp/__init__.py
+-rw-r--r--   0        0        0    11887 2023-06-09 00:53:00.107336 pyentrp-0.8.3/pyentrp/entropy.py
+-rw-r--r--   0        0        0     1612 2023-06-09 00:53:00.107336 pyentrp-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2367 1970-01-01 00:00:00.000000 pyentrp-0.8.3/PKG-INFO
```

### Comparing `pyentrp-0.8.2/LICENSE` & `pyentrp-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyentrp-0.8.2/README.md` & `pyentrp-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `pyentrp-0.8.2/pyentrp/entropy.py` & `pyentrp-0.8.3/pyentrp/entropy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import Counter
 from math import factorial
 
 import numpy as np
 
 
 def _embed(x, order=3, delay=1):
     """
@@ -83,34 +84,36 @@
 
     Args:
         time_series: Vector or string of the sample data
 
     Returns:
         The Shannon Entropy as float value
     """
+    if isinstance(time_series, str):
+        # Calculate frequency counts
+        counter = Counter(time_series)
+        total_count = len(time_series)
+
+        # Calculate frequencies and Shannon entropy
+        ent = 0.0
+        for count in counter.values():
+            freq = count / total_count
+            ent += freq * np.log2(freq)
+
+        ent = -ent
+        return ent
+
+    # Calculate frequency counts
+    unique_vals, counts = np.unique(time_series, return_counts=True)
+    total_count = len(time_series)
+
+    # Calculate frequencies and Shannon entropy
+    frequencies = counts / total_count
+    ent = -np.sum(frequencies * np.log2(frequencies))
 
-    # Check if string
-    if not isinstance(time_series, str):
-        time_series = list(time_series)
-
-    # Create a frequency data
-    data_set = list(set(time_series))
-    freq_list = []
-    for entry in data_set:
-        counter = 0.0
-        for i in time_series:
-            if i == entry:
-                counter += 1
-        freq_list.append(float(counter) / len(time_series))
-
-    # Shannon entropy
-    ent = 0.0
-    for freq in freq_list:
-        ent += freq * np.log2(freq)
-    ent = -ent
     return ent
 
 
 def sample_entropy(time_series, sample_length, tolerance=None):
     """
     Calculates the sample entropy of degree m of a time_series.
 
@@ -377,14 +380,14 @@
     Returns:
         Vector containing Composite Multiscale Entropy
 
     Reference:
         [1] Wu, Shuen-De, et al. "Time series analysis using
             composite multiscale entropy." Entropy 15.3 (2013): 1069-1084.
     """
-    cmse = np.zeros((1, scale))
+    cmse = np.zeros(scale)
 
     for i in range(scale):
         for j in range(i):
             tmp = util_granulate_time_series(time_series[j:], i + 1)
             cmse[i] += sample_entropy(tmp, sample_length, tolerance) / (i + 1)
     return cmse
```

### Comparing `pyentrp-0.8.2/pyproject.toml` & `pyentrp-0.8.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyentrp"
-version = "0.8.2"
+version = "0.8.3"
 description = "A Python library for computing entropy measures for time series analysis."
 authors = ["Nikolay Donets <nd@donets.org>"]
 license = "apache-2.0"
 readme = "README.md"
 packages = [
   {"include" = "pyentrp"}
 ]
```

### Comparing `pyentrp-0.8.2/PKG-INFO` & `pyentrp-0.8.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyentrp
-Version: 0.8.2
+Version: 0.8.3
 Summary: A Python library for computing entropy measures for time series analysis.
 License: Apache-2.0
 Author: Nikolay Donets
 Author-email: nd@donets.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

