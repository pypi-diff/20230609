# Comparing `tmp/quantile-estimator-0.1.0.tar.gz` & `tmp/quantile-estimator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantile-estimator-0.1.0.tar", last modified: Fri Jun  9 10:54:07 2023, max compression
+gzip compressed data, was "quantile-estimator-0.1.1.tar", last modified: Fri Jun  9 14:28:02 2023, max compression
```

## Comparing `quantile-estimator-0.1.0.tar` & `quantile-estimator-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:54:07.898026 quantile-estimator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-09 10:53:58.000000 quantile-estimator-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 10:54:07.898026 quantile-estimator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 10:53:58.000000 quantile-estimator-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:54:07.898026 quantile-estimator-0.1.0/quantile_estimator/
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-09 10:53:58.000000 quantile-estimator-0.1.0/quantile_estimator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 10:53:58.000000 quantile-estimator-0.1.0/quantile_estimator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 10:54:07.898026 quantile-estimator-0.1.0/quantile_estimator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-09 10:54:07.000000 quantile-estimator-0.1.0/quantile_estimator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-09 10:54:07.000000 quantile-estimator-0.1.0/quantile_estimator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 10:54:07.000000 quantile-estimator-0.1.0/quantile_estimator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 10:54:07.000000 quantile-estimator-0.1.0/quantile_estimator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 10:54:07.898026 quantile-estimator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-09 10:53:58.000000 quantile-estimator-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/quantile_estimator/
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/quantile_estimator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/quantile_estimator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/quantile_estimator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-09 14:28:02.000000 quantile-estimator-0.1.1/quantile_estimator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:28:02.865799 quantile-estimator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-06-09 14:27:53.000000 quantile-estimator-0.1.1/setup.py
```

### Comparing `quantile-estimator-0.1.0/LICENSE` & `quantile-estimator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `quantile-estimator-0.1.0/PKG-INFO` & `quantile-estimator-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: quantile-estimator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE'05
 Home-page: https://github.com/RefaceAI/quantile-estimator
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 quantile-estimator
 ==========================
 
 Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE’05
 
 ## Installation
 ```
-pip install quantile-estimator==0.1.0
+pip install quantile-estimator==0.1.1
 ```
```

### Comparing `quantile-estimator-0.1.0/quantile_estimator/__init__.py` & `quantile-estimator-0.1.1/quantile_estimator/__init__.py`

 * *Files identical despite different names*

### Comparing `quantile-estimator-0.1.0/quantile_estimator.egg-info/PKG-INFO` & `quantile-estimator-0.1.1/quantile_estimator.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: quantile-estimator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE'05
 Home-page: https://github.com/RefaceAI/quantile-estimator
 Author: RefaceAI
 Author-email: github-support@reface.ai
 License: Apache License 2.0
 Platform: Platform Independent
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 quantile-estimator
 ==========================
 
 Python Implementation of Graham Cormode and S. Muthukrishnan's Effective Computation of Biased Quantiles over Data Streams in ICDE’05
 
 ## Installation
 ```
-pip install quantile-estimator==0.1.0
+pip install quantile-estimator==0.1.1
 ```
```

### Comparing `quantile-estimator-0.1.0/setup.py` & `quantile-estimator-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     author_email="github-support@reface.ai",
     description=(
         "Python Implementation of Graham Cormode and S. "
         "Muthukrishnan's Effective Computation of Biased "
         "Quantiles over Data Streams in ICDE'05"
     ),
     long_description=readfile("README.md"),
+    long_description_content_type="text/markdown",
     license="Apache License 2.0",
     url="https://github.com/RefaceAI/quantile-estimator",
     packages=["quantile_estimator"],
     platforms="Platform Independent",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
```

