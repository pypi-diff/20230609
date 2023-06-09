# Comparing `tmp/bischoff_and_ratcliff_1995-0.0.1.tar.gz` & `tmp/bischoff_and_ratcliff_1995-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bischoff_and_ratcliff_1995-0.0.1.tar", last modified: Thu Jun  8 19:28:46 2023, max compression
+gzip compressed data, was "bischoff_and_ratcliff_1995-0.1.0.tar", last modified: Fri Jun  9 14:46:40 2023, max compression
```

## Comparing `bischoff_and_ratcliff_1995-0.0.1.tar` & `bischoff_and_ratcliff_1995-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.028236 bischoff_and_ratcliff_1995-0.0.1/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)     1070 2023-06-08 14:26:14.000000 bischoff_and_ratcliff_1995-0.0.1/LICENSE
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-08 19:28:46.027236 bischoff_and_ratcliff_1995-0.0.1/PKG-INFO
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      733 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.0.1/README.md
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.026236 bischoff_and_ratcliff_1995-0.0.1/bin/
--rwxr-xr-x   0 unicamp   (1001) unicamp   (1001)     2433 2023-06-08 19:25:19.000000 bischoff_and_ratcliff_1995-0.0.1/bin/generate_all_instances
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.026236 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)     3038 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/Instance.py
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      448 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/Random.py
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)       58 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/__init__.py
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.027236 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/PKG-INFO
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      474 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/SOURCES.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)        1 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/dependency_links.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)        7 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/requires.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)       27 2023-06-08 19:28:46.000000 bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/top_level.txt
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      116 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.0.1/pyproject.toml
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)       38 2023-06-08 19:28:46.028236 bischoff_and_ratcliff_1995-0.0.1/setup.cfg
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      801 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.0.1/setup.py
-drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-08 19:28:46.027236 bischoff_and_ratcliff_1995-0.0.1/test/
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)     2119 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/test/test_Instance.py
--rw-r--r--   0 unicamp   (1001) unicamp   (1001)      569 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.0.1/test/test_Random.py
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-09 14:46:40.107987 bischoff_and_ratcliff_1995-0.1.0/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)     1070 2023-06-08 14:26:14.000000 bischoff_and_ratcliff_1995-0.1.0/LICENSE
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-09 14:46:40.107987 bischoff_and_ratcliff_1995-0.1.0/PKG-INFO
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      733 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.1.0/README.md
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-09 14:46:40.105987 bischoff_and_ratcliff_1995-0.1.0/bin/
+-rwxr-xr-x   0 unicamp   (1001) unicamp   (1001)     2433 2023-06-08 19:25:19.000000 bischoff_and_ratcliff_1995-0.1.0/bin/generate_all_instances
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-09 14:46:40.106988 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)     3566 2023-06-09 14:38:39.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995/Instance.py
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      448 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995/Random.py
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)       58 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995/__init__.py
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-09 14:46:40.106988 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      582 2023-06-09 14:46:40.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/PKG-INFO
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      474 2023-06-09 14:46:40.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/SOURCES.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)        1 2023-06-09 14:46:40.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/dependency_links.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)        7 2023-06-09 14:46:40.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/requires.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)       27 2023-06-09 14:46:40.000000 bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/top_level.txt
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      116 2023-06-08 19:27:04.000000 bischoff_and_ratcliff_1995-0.1.0/pyproject.toml
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)       38 2023-06-09 14:46:40.107987 bischoff_and_ratcliff_1995-0.1.0/setup.cfg
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      801 2023-06-09 14:39:14.000000 bischoff_and_ratcliff_1995-0.1.0/setup.py
+drwxr-xr-x   0 unicamp   (1001) unicamp   (1001)        0 2023-06-09 14:46:40.106988 bischoff_and_ratcliff_1995-0.1.0/test/
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      840 2023-06-09 14:38:39.000000 bischoff_and_ratcliff_1995-0.1.0/test/test_Instance.py
+-rw-r--r--   0 unicamp   (1001) unicamp   (1001)      569 2023-06-08 18:32:24.000000 bischoff_and_ratcliff_1995-0.1.0/test/test_Random.py
```

### Comparing `bischoff_and_ratcliff_1995-0.0.1/LICENSE` & `bischoff_and_ratcliff_1995-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bischoff_and_ratcliff_1995-0.0.1/PKG-INFO` & `bischoff_and_ratcliff_1995-0.1.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,26 @@
-Metadata-Version: 2.1
-Name: bischoff_and_ratcliff_1995
-Version: 0.0.1
-Summary: Instance generator, as described in the paper of Bischoff and Ratcliff (1995)
-Home-page: https://github.com/lucasguesserts/bischoff-and-ratcliff-1995
-Author: Lucas Guesser
-Author-email: lucasguesserts@gmail.com
-Keywords: container loading problem,knapsack problem,single large object placement problem (slopp),packing problem
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.0
-License-File: LICENSE
+from setuptools import setup
+
+setup(
+    # Metadata
+    name="bischoff_and_ratcliff_1995",
+    version="0.1.0",
+    description="Instance generator, as described in the paper of Bischoff and Ratcliff (1995)",
+    url="https://github.com/lucasguesserts/bischoff-and-ratcliff-1995",
+    author="Lucas Guesser",
+    author_email="lucasguesserts@gmail.com",
+    classifiers=[
+        "Natural Language :: English",
+        "Programming Language :: Python :: 3",
+        "Topic :: Scientific/Engineering",
+    ],
+    keywords=[
+        "container loading problem",
+        "knapsack problem",
+        "single large object placement problem (slopp)",
+        "packing problem",
+    ],
+    # Options
+    install_requires=["pytest"],
+    python_requires=">=3.0",
+    scripts=["bin/generate_all_instances"],
+)
```

### Comparing `bischoff_and_ratcliff_1995-0.0.1/README.md` & `bischoff_and_ratcliff_1995-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bischoff_and_ratcliff_1995-0.0.1/bin/generate_all_instances` & `bischoff_and_ratcliff_1995-0.1.0/bin/generate_all_instances`

 * *Files identical despite different names*

### Comparing `bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995/Instance.py` & `bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995/Instance.py`

 * *Files 24% similar despite different names*

```diff
@@ -82,23 +82,37 @@
         self.m = m
 
         return
 
     def to_dict(self):
         return {
             "type": "input",
-            "version": "0.0.0",
+            "version": "0.3.0",
             "large_object": {
-                "length": self.C["length"],
-                "width": self.C["width"],
-                "height": self.C["height"],
+                "measurement": {
+                    "x": self.C["length"],
+                    "y": self.C["width"],
+                    "z": self.C["height"],
+                }
             },
             "small_items": [
                 {
-                    "length": self.d[i][0],
-                    "width": self.d[i][1],
-                    "height": self.d[i][2],
+                    "measurement": {
+                        "x": self.d[i][0],
+                        "y": self.d[i][1],
+                        "z": self.d[i][2],
+                    },
                     "quantity": self.m[i],
+                    "constraint": {
+                        "orientation": {
+                            "xyz": self.o[i][2],
+                            "yxz": self.o[i][2],
+                            "zyx": self.o[i][0],
+                            "xzy": self.o[i][1],
+                            "zxy": self.o[i][1],
+                            "yzx": self.o[i][0],
+                        },
+                    },
                 }
                 for i in range(self.n)
             ],
         }
```

### Comparing `bischoff_and_ratcliff_1995-0.0.1/bischoff_and_ratcliff_1995.egg-info/PKG-INFO` & `bischoff_and_ratcliff_1995-0.1.0/bischoff_and_ratcliff_1995.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bischoff-and-ratcliff-1995
-Version: 0.0.1
+Version: 0.1.0
 Summary: Instance generator, as described in the paper of Bischoff and Ratcliff (1995)
 Home-page: https://github.com/lucasguesserts/bischoff-and-ratcliff-1995
 Author: Lucas Guesser
 Author-email: lucasguesserts@gmail.com
 Keywords: container loading problem,knapsack problem,single large object placement problem (slopp),packing problem
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bischoff_and_ratcliff_1995-0.0.1/test/test_Random.py` & `bischoff_and_ratcliff_1995-0.1.0/test/test_Random.py`

 * *Files identical despite different names*

