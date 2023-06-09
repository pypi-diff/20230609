# Comparing `tmp/puan_pv_rs-0.1.2.tar.gz` & `tmp/puan_pv_rs-0.1.3.tar.gz`

## Comparing `puan_pv_rs-0.1.2.tar` & `puan_pv_rs-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.2/Cargo.toml
--rw-r--r--   0     1001      123     1500 2023-06-08 21:10:34.000000 puan_pv_rs-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-08 21:10:34.000000 puan_pv_rs-0.1.2/.gitignore
--rw-r--r--   0     1001      123      359 2023-06-08 21:10:34.000000 puan_pv_rs-0.1.2/pyproject.toml
--rw-r--r--   0     1001      123        0 2023-06-08 21:10:34.000000 puan_pv_rs-0.1.2/python/puan_pv_rs/__init__.py
--rwxr-xr-x   0     1001      123      833 2023-06-08 21:11:11.000000 puan_pv_rs-0.1.2/run-maturin-action.sh
--rw-r--r--   0     1001      123     9065 2023-06-08 21:10:34.000000 puan_pv_rs-0.1.2/src/lib.rs
--rw-r--r--   0     1001      123     7654 2023-06-08 21:10:34.000000 puan_pv_rs-0.1.2/Cargo.lock
--rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      123     1500 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/.gitignore
+-rw-r--r--   0     1001      123      359 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/pyproject.toml
+-rwxr-xr-x   0     1001      123      833 2023-06-09 06:39:06.000000 puan_pv_rs-0.1.3/run-maturin-action.sh
+-rw-r--r--   0     1001      123     9065 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      123     7654 2023-06-09 06:38:36.000000 puan_pv_rs-0.1.3/Cargo.lock
+-rw-r--r--   0        0        0      259 1970-01-01 00:00:00.000000 puan_pv_rs-0.1.3/PKG-INFO
```

### Comparing `puan_pv_rs-0.1.2/.github/workflows/CI.yml` & `puan_pv_rs-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.2/.gitignore` & `puan_pv_rs-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.2/run-maturin-action.sh` & `puan_pv_rs-0.1.3/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.2/src/lib.rs` & `puan_pv_rs-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `puan_pv_rs-0.1.2/Cargo.lock` & `puan_pv_rs-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "puan-pv-rs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.17.3"
```

