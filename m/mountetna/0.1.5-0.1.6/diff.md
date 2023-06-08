# Comparing `tmp/mountetna-0.1.5.tar.gz` & `tmp/mountetna-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mountetna-0.1.5.tar", max compression
+gzip compressed data, was "mountetna-0.1.6.tar", max compression
```

## Comparing `mountetna-0.1.5.tar` & `mountetna-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0       73 2022-08-15 19:39:20.924985 mountetna-0.1.5/README.md
--rw-r--r--   0        0        0      740 2022-08-15 19:39:20.924985 mountetna-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       20 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/__init__.py
--rw-r--r--   0        0        0     1686 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/auth.py
--rw-r--r--   0        0        0      239 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/etna.py
--rw-r--r--   0        0        0     2567 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/etna_base.py
--rw-r--r--   0        0        0      629 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/janus.py
--rw-r--r--   0        0        0    10988 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/magma.py
--rw-r--r--   0        0        0    19946 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/metis.py
--rw-r--r--   0        0        0        0 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/tests/__init__.py
--rw-r--r--   0        0        0     1507 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/tests/conftest.py
--rw-r--r--   0        0        0      501 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/tests/test_janus.py
--rw-r--r--   0        0        0     2769 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/tests/test_magma.py
--rw-r--r--   0        0        0      844 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/tests/test_metis.py
--rw-r--r--   0        0        0        0 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/__init__.py
--rw-r--r--   0        0        0      403 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/gater.py
--rw-r--r--   0        0        0      481 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/inject.py
--rw-r--r--   0        0        0      363 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/iterables.py
--rw-r--r--   0        0        0     1542 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/multipart.py
--rw-r--r--   0        0        0     5263 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/parser.py
--rw-r--r--   0        0        0     1019 2022-08-15 19:39:20.924985 mountetna-0.1.5/src/mountetna/utils/streaming.py
--rw-r--r--   0        0        0      932 2022-08-15 19:39:29.647763 mountetna-0.1.5/setup.py
--rw-r--r--   0        0        0      924 2022-08-15 19:39:29.648045 mountetna-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       73 2023-06-08 22:46:21.087595 mountetna-0.1.6/README.md
+-rw-r--r--   0        0        0      740 2023-06-08 22:46:21.087595 mountetna-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/__init__.py
+-rw-r--r--   0        0        0     1686 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/auth.py
+-rw-r--r--   0        0        0      481 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/etna.py
+-rw-r--r--   0        0        0     2567 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/etna_base.py
+-rw-r--r--   0        0        0      673 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/gnomon.py
+-rw-r--r--   0        0        0      629 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/janus.py
+-rw-r--r--   0        0        0    10988 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/magma.py
+-rw-r--r--   0        0        0    19946 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/metis.py
+-rw-r--r--   0        0        0     2641 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/polyphemus.py
+-rw-r--r--   0        0        0        0 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/tests/__init__.py
+-rw-r--r--   0        0        0     1507 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/tests/conftest.py
+-rw-r--r--   0        0        0      501 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/tests/test_janus.py
+-rw-r--r--   0        0        0     2769 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/tests/test_magma.py
+-rw-r--r--   0        0        0      844 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/tests/test_metis.py
+-rw-r--r--   0        0        0     1062 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/tests/test_polyphemus.py
+-rw-r--r--   0        0        0        0 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/__init__.py
+-rw-r--r--   0        0        0      403 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/gater.py
+-rw-r--r--   0        0        0      481 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/inject.py
+-rw-r--r--   0        0        0      363 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/iterables.py
+-rw-r--r--   0        0        0     1542 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/multipart.py
+-rw-r--r--   0        0        0     5263 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/parser.py
+-rw-r--r--   0        0        0     1019 2023-06-08 22:46:21.087595 mountetna-0.1.6/src/mountetna/utils/streaming.py
+-rw-r--r--   0        0        0      975 1970-01-01 00:00:00.000000 mountetna-0.1.6/PKG-INFO
```

### Comparing `mountetna-0.1.5/pyproject.toml` & `mountetna-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mountetna"
-version = "0.1.5"
+version = "0.1.6"
 description = "Client package for Mount Etna data library"
 
 license = "GPL-2.0-only"
 
 authors = [
     "Zachary Collins <zachary.collins@ucsf.edu>",
     "Saurabh Asthana <saurabh.asthana@ucsf.edu>",
```

### Comparing `mountetna-0.1.5/src/mountetna/auth.py` & `mountetna-0.1.6/src/mountetna/auth.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/etna_base.py` & `mountetna-0.1.6/src/mountetna/etna_base.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/janus.py` & `mountetna-0.1.6/src/mountetna/janus.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/magma.py` & `mountetna-0.1.6/src/mountetna/magma.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/metis.py` & `mountetna-0.1.6/src/mountetna/metis.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/tests/conftest.py` & `mountetna-0.1.6/src/mountetna/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/tests/test_magma.py` & `mountetna-0.1.6/src/mountetna/tests/test_magma.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/tests/test_metis.py` & `mountetna-0.1.6/src/mountetna/tests/test_metis.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/utils/multipart.py` & `mountetna-0.1.6/src/mountetna/utils/multipart.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/utils/parser.py` & `mountetna-0.1.6/src/mountetna/utils/parser.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/src/mountetna/utils/streaming.py` & `mountetna-0.1.6/src/mountetna/utils/streaming.py`

 * *Files identical despite different names*

### Comparing `mountetna-0.1.5/PKG-INFO` & `mountetna-0.1.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: mountetna
-Version: 0.1.5
+Version: 0.1.6
 Summary: Client package for Mount Etna data library
 Home-page: https://github.com/mountetna/monoetna
 License: GPL-2.0-only
 Keywords: mount etna,data library
 Author: Zachary Collins
 Author-email: zachary.collins@ucsf.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: cryptography (>=37.0.3,<38.0.0)
 Requires-Dist: pandas (>=1.2.1,<2.0.0)
 Requires-Dist: pyserde (>=0.8.2,<0.9.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Project-URL: Repository, https://github.com/mountetna/monoetna/
 Description-Content-Type: text/markdown
```

