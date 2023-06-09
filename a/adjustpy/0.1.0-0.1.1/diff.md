# Comparing `tmp/adjustpy-0.1.0.tar.gz` & `tmp/adjustpy-0.1.1.tar.gz`

## Comparing `adjustpy-0.1.0.tar` & `adjustpy-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 adjustpy-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000      842 2023-06-09 19:31:18.000000 adjustpy-0.1.0/.github/workflows/workflow.yml
--rw-r--r--   0     1000     1000       19 2023-06-09 19:03:27.000000 adjustpy-0.1.0/.gitignore
--rw-r--r--   0     1000     1000     1070 2023-06-09 19:02:40.000000 adjustpy-0.1.0/LICENSE
--rw-r--r--   0     1000     1000     1325 2023-06-09 19:12:23.000000 adjustpy-0.1.0/README.md
--rw-r--r--   0     1000     1000      641 2023-06-09 19:35:19.000000 adjustpy-0.1.0/pyproject.toml
--rw-r--r--   0     1000     1000     1306 2023-06-09 19:13:02.000000 adjustpy-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000     2069 2023-06-09 19:21:52.000000 adjustpy-0.1.0/tests/test_adjustpy.py
--rw-r--r--   0     1000     1000     9556 2023-06-09 18:24:02.000000 adjustpy-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 adjustpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      274 1970-01-01 00:00:00.000000 adjustpy-0.1.1/Cargo.toml
+-rw-r--r--   0     1000     1000      842 2023-06-09 19:31:18.000000 adjustpy-0.1.1/.github/workflows/workflow.yml
+-rw-r--r--   0     1000     1000       36 2023-06-09 19:38:37.000000 adjustpy-0.1.1/.gitignore
+-rw-r--r--   0     1000     1000     1070 2023-06-09 19:02:40.000000 adjustpy-0.1.1/LICENSE
+-rw-r--r--   0     1000     1000     1325 2023-06-09 19:12:23.000000 adjustpy-0.1.1/README.md
+-rw-r--r--   0     1000     1000      641 2023-06-09 19:35:19.000000 adjustpy-0.1.1/pyproject.toml
+-rw-r--r--   0     1000     1000     1306 2023-06-09 19:13:02.000000 adjustpy-0.1.1/src/lib.rs
+-rw-r--r--   0     1000     1000     2069 2023-06-09 19:21:52.000000 adjustpy-0.1.1/tests/test_adjustpy.py
+-rw-r--r--   0     1000     1000     9556 2023-06-09 19:39:48.000000 adjustpy-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1870 1970-01-01 00:00:00.000000 adjustpy-0.1.1/PKG-INFO
```

### Comparing `adjustpy-0.1.0/.github/workflows/workflow.yml` & `adjustpy-0.1.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `adjustpy-0.1.0/LICENSE` & `adjustpy-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adjustpy-0.1.0/README.md` & `adjustpy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `adjustpy-0.1.0/pyproject.toml` & `adjustpy-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adjustpy-0.1.0/src/lib.rs` & `adjustpy-0.1.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `adjustpy-0.1.0/tests/test_adjustpy.py` & `adjustpy-0.1.1/tests/test_adjustpy.py`

 * *Files identical despite different names*

### Comparing `adjustpy-0.1.0/Cargo.lock` & `adjustpy-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "adjustp"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "151571bfc58e15241979bf8efb3b25506a437483101149cdcbc2ff56276da850"
 
 [[package]]
 name = "adjustpy"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "adjustp",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
```

### Comparing `adjustpy-0.1.0/PKG-INFO` & `adjustpy-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adjustpy
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: numpy >=1.17.0
 License-File: LICENSE
 Author-email: Noam Teyssier <noam.teyssier@ucsf.edu>
```

