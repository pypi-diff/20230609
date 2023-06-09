# Comparing `tmp/rs_distances-0.6.0.tar.gz` & `tmp/rs_distances-0.8.1.tar.gz`

## Comparing `rs_distances-0.6.0.tar` & `rs_distances-0.8.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      475 1970-01-01 00:00:00.000000 rs_distances-0.6.0/Cargo.toml
--rw-r--r--   0        0        0     2807 2023-06-03 05:19:15.000000 rs_distances-0.6.0/.github/workflows/CI.yml
--rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.6.0/.gitignore
--rw-r--r--   0        0        0     2313 2023-06-03 16:58:44.000000 rs_distances-0.6.0/README.md
--rw-r--r--   0        0        0      914 2023-06-03 18:38:08.000000 rs_distances-0.6.0/pyproject.toml
--rw-r--r--   0        0        0       13 2023-06-04 16:25:45.000000 rs_distances-0.6.0/src/lib.rs
--rw-r--r--   0        0        0       13 2023-06-05 11:46:40.000000 rs_distances-0.6.0/src/spkd/mod.rs
--rw-r--r--   0        0        0     5506 2023-06-05 22:38:31.000000 rs_distances-0.6.0/src/spkd/spkd.rs
--rw-r--r--   0        0        0    66783 2023-06-05 23:11:08.000000 rs_distances-0.6.0/Cargo.lock
--rw-r--r--   0        0        0     2784 1970-01-01 00:00:00.000000 rs_distances-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 rs_distances-0.8.1/Cargo.toml
+-rw-r--r--   0        0        0     3129 2023-06-09 17:18:17.000000 rs_distances-0.8.1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      764 2023-06-03 16:25:17.000000 rs_distances-0.8.1/.gitignore
+-rw-r--r--   0        0        0     3531 2023-06-08 05:09:16.000000 rs_distances-0.8.1/README.md
+-rw-r--r--   0        0        0     1211 2023-06-08 18:56:44.000000 rs_distances-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      841 2023-06-09 17:22:44.000000 rs_distances-0.8.1/rs-distances.pyi
+-rw-r--r--   0        0        0       13 2023-06-04 16:25:45.000000 rs_distances-0.8.1/src/lib.rs
+-rw-r--r--   0        0        0       13 2023-06-05 11:46:40.000000 rs_distances-0.8.1/src/spkd/mod.rs
+-rw-r--r--   0        0        0     6088 2023-06-08 18:53:17.000000 rs_distances-0.8.1/src/spkd/spkd.rs
+-rw-r--r--   0        0        0    66796 2023-06-08 18:57:25.000000 rs_distances-0.8.1/Cargo.lock
+-rw-r--r--   0        0        0     4322 1970-01-01 00:00:00.000000 rs_distances-0.8.1/PKG-INFO
```

### Comparing `rs_distances-0.6.0/.github/workflows/CI.yml` & `rs_distances-0.8.1/.github/workflows/CI.yml`

 * *Files 11% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 #    maturin generate-ci github
 #
 name: CI
 
 on:
   push:
     branches:
-      - main
       - master
     tags:
       - '*'
+    paths:
+      - 'src/**'
+      - 'Cargo.toml'
+      - '.github/workflows/CI.yml'
+      - 'rs-distances.pyi'
   pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
 
 jobs:
   linux:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        target: [x86_64, x86, aarch64, armv7, s390x, ppc64le]
+        target: [x86_64]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: '3.10'
       - name: Build wheels
         uses: PyO3/maturin-action@v1
@@ -101,20 +105,30 @@
         with:
           name: wheels
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
-    if: "startsWith(github.ref, 'refs/tags/')"
+    if: startsWith(github.ref, 'refs/tags/')
     needs: [linux, windows, macos, sdist]
+    strategy:
+      matrix:
+        python-version: ['3.6', '3.7', '3.8', '3.9', '3.10']
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: wheels
+      - name: Set up Python
+        uses: actions/setup-python@v2
+        with:
+          python-version: ${{ matrix.python-version }}
       - name: Publish to PyPI
         uses: PyO3/maturin-action@v1
         env:
           MATURIN_PYPI_TOKEN: ${{ secrets.PYPI_API_TOKEN }}
         with:
+          manylinux: '1,2010,2014'  
           command: upload
           args: --skip-existing *
+
+
```

### Comparing `rs_distances-0.6.0/.gitignore` & `rs_distances-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `rs_distances-0.6.0/pyproject.toml` & `rs_distances-0.8.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -8,27 +8,34 @@
 authors = [{name = "Flynn OConnell", email = "flynnoconnell@gmail.com"}]
 readme = "README.md"
 homepage = "https://github.com/NeuroPyPy/rs-distances"
 license = "MIT"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
-    "Programming Language :: Python :: Implementation :: CPython",
-    "Programming Language :: Python :: Implementation :: PyPy",
+    "License :: OSI Approved :: MIT License",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Science/Research",
+    "Operating System :: OS Independent",
 ]
 
-
 [tool.maturin]
 features = ["pyo3/extension-module"]
 
 [package]
-version = "0.4.0"
+version = "0.8.1"
 edition = "2023"
 
 [package.metadata.maturin]
 rust-version = "1.56.0"
 requires-dist = ["numpy"]
 
 [package.metadata.maturin.dependencies]
 ndarray = "0.15.4"
 numpy = "0.14.1"
 pyo3 = { version = "0.15.1", features = ["extension-module"] }
+
+[project.urls]
+homepage = "https://github.com/NeuroPyPy/rs-distances"
+repository = "https://github.com/NeuroPyPy/rs-distances"
+documentation = "http://www-users.med.cornell.edu/~jdvicto/metricdf.html#algorithm"
```

### Comparing `rs_distances-0.6.0/src/spkd/spkd.rs` & `rs_distances-0.8.1/src/spkd/spkd.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use ndarray::Array2;
 use ndarray::{s, Array1, Array3, ArrayBase, ArrayView3, Dim, OwnedRepr};
-use numpy::{IntoPyArray, PyArray1, PyArray3};
+use numpy::{IntoPyArray, PyArray1};
 use pyo3::{prelude::*, types::PyList};
 
 pub fn iterate_spiketrains(scr: &mut Array3<f64>, sd: &ArrayView3<f64>) {
     let (num_qvals, num_spikes_xii, num_spikes_xjj) = scr.dim();
     for xii in 1..num_spikes_xii {
         for xjj in 1..num_spikes_xjj {
             for q in 0..num_qvals {
@@ -14,145 +14,165 @@
 
                 scr[[q, xii, xjj]] = a.min(b.min(c));
             }
         }
     }
 }
 
-#[pyfunction]
-fn iterate_spiketrains_impl(
-    py: Python,
-    scr: &PyArray3<f64>,
-    sd: &PyArray3<f64>,
-) -> PyResult<PyObject> {
-    let mut scr: Array3<f64> = scr.to_owned_array();
-    let sd: Array3<f64> = sd.to_owned_array();
-
-    iterate_spiketrains(&mut scr, &sd.view());
-
-    // Convert the result to a PyArray
-    let res: Py<numpy::PyArray<f64, Dim<[usize; 3]>>> = scr.into_pyarray(py).to_owned();
-    Ok(res.into())
-}
-
-pub fn calculate_spkd(
+pub fn calculate_pairwise_distances(
+    numt: usize,
     cspks: &Vec<Array1<f64>>,
     qvals: &ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>,
-    _res: Option<f64>,
-) -> ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> {
-    let numt: usize = cspks.len(); // number of spike trains
-    let num_qvals: usize = qvals.len(); // number of q values
-
-    let mut d: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
-        Array3::<f64>::zeros((numt, numt, num_qvals));
+    num_qvals: usize,
+    d: &mut ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>,
+) {
 
     for xi in 0..numt - 1 {
         for xj in xi + 1..numt {
             let curcounts_xi: usize = cspks[xi].len();
             let curcounts_xj: usize = cspks[xj].len();
 
             if curcounts_xi != 0 && curcounts_xj != 0 {
-                let mut outer_diff = cspks[xi].clone().into_shape((curcounts_xi, 1)).unwrap()
-                    - cspks[xj].clone().into_shape((1, curcounts_xj)).unwrap();
+                let mut outer_diff: ArrayBase<OwnedRepr<f64>, Dim<[usize; 2]>> =
+                    cspks[xi].clone().into_shape((curcounts_xi, 1)).unwrap()
+                        - cspks[xj].clone().into_shape((1, curcounts_xj)).unwrap();
 
                 outer_diff.mapv_inplace(|x| x.abs());
 
-                let sd = qvals.clone().into_shape((qvals.len(), 1, 1)).unwrap() * &outer_diff;
-
-                let mut scr =
-                    Array3::<f64>::zeros((qvals.len(), curcounts_xi + 1, curcounts_xj + 1));
-                 let scr_len = scr.len();
+                let sd: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
+                    qvals.clone().into_shape((num_qvals, 1, 1)).unwrap() * &outer_diff.clone();
+                let mut scr: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
+                    Array3::<f64>::zeros((num_qvals, curcounts_xi + 1, curcounts_xj + 1));
 
                 scr.slice_mut(s![.., 1.., 0])
-                    .assign(&Array2::from_elem((qvals.len(), curcounts_xi), 1.0));
+                    .assign(&Array2::from_elem((num_qvals, curcounts_xi), 1.0));
                 scr.slice_mut(s![.., 0, 1..])
-                    .assign(&Array2::from_elem((qvals.len(), curcounts_xj), 1.0));
+                    .assign(&Array2::from_elem((num_qvals, curcounts_xj), 1.0));
 
                 iterate_spiketrains(&mut scr, &sd.view());
 
-                println!("scr's shape: {:?}", scr.dim());
-                // println!("d's slice shape: {:?}", d.slice(s![xi, xj, ..]).dim());
-               
-                d.slice_mut(s![xi, xj, ..]).assign(&scr.into_shape(scr_len).unwrap());
+                let final_values: Array1<f64> = Array1::from_shape_vec(
+                    num_qvals,
+                    (0..num_qvals)
+                        .map(|q| scr[[q, scr.shape()[1] - 1, scr.shape()[2] - 1]])
+                        .collect(),
+                )
+                .unwrap();
 
+                d.slice_mut(s![xi, xj, ..]).assign(&final_values);
             } else {
                 println!("d's shape: {:?}", d.dim());
                 d.slice_mut(s![xi, xj, ..])
                     .fill(curcounts_xi.max(curcounts_xj) as f64);
             }
         }
     }
-
-    // Transpose d
-    d = d.permuted_axes([1, 0, 2]);
-    d.mapv_inplace(|x| x.max(0.0));
-    d
 }
 
 #[pyfunction]
-fn calculate_spkd_impl(
-    py: Python,
-    cspks: &PyList,
-    qvals: &PyArray1<f64>,
-    res: Option<f64>,
-) -> PyResult<PyObject> {
-    let cspks: Vec<Array1<f64>> = cspks
-        .into_iter()
-        .map(|pyarray| {
-            let numpy_array: &PyArray1<f64> = pyarray.extract()?;
-            Ok(numpy_array.to_owned_array())
-        })
-        .collect::<PyResult<_>>()?;
+fn calculate_spkd(py: Python, cspks: &PyList, qvals: &PyArray1<f64>) -> PyResult<PyObject> {
+    let mut cspk_vectors: Vec<Array1<f64>> = Vec::new();
+    let mut num_vectors: usize = 0;
+
+    // Iterate over the spike trains and convert them to ndarrays
+    for pyarray in cspks.iter() {
+        let numpy_array: &PyArray1<f64> = pyarray.extract()?;
+        let array: Array1<f64> = numpy_array.to_owned_array();
+        let shape: &[usize] = array.shape();
+
+        if shape.is_empty() || shape[0] == 0 {
+            continue; // Skip empty arrays
+        }
+
+        num_vectors += 1;
+        cspk_vectors.push(array);
+    }
 
     let qvals: Array1<f64> = qvals.to_owned_array();
     let numqvals: usize = qvals.len();
     let q_reshaped: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
         qvals.into_shape((numqvals, 1, 1)).unwrap();
 
-    // Assume calculate_spkd returns ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>
-    let d: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> = calculate_spkd(&cspks, &q_reshaped, res);
+    let d: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
+        calculate_spkd_impl(&cspk_vectors, &q_reshaped, numqvals, num_vectors);
 
     // Convert the ArrayBase to a PyArray
     let py_array: &numpy::PyArray<f64, Dim<[usize; 3]>> = d.into_pyarray(py);
 
     // Convert the PyArray to a PyObject
     Ok(py_array.to_object(py))
 }
 
+pub fn calculate_spkd_impl(
+    cspks: &Vec<Array1<f64>>,
+    qvals: &ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>>,
+    num_qvals: usize,
+    num_vectors: usize,
+) -> ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> {
+    let numt: usize = num_vectors; // number of spike trains
+
+    let mut d: ArrayBase<OwnedRepr<f64>, Dim<[usize; 3]>> =
+        Array3::<f64>::zeros((numt, numt, num_qvals));
+    
+    calculate_pairwise_distances(numt, cspks, qvals, num_qvals, &mut d);
+
+    // Transpose d
+    d = d.permuted_axes([1, 0, 2]);
+    d.mapv_inplace(|x| x.max(0.0));
+    d
+}
+
+#[pyclass]
+struct Version {
+    version: String,
+}
+
+#[pymethods]
+impl Version {
+    #[getter]
+    fn version(&self) -> PyResult<String> {
+        Ok(self.version.clone())
+    }
+    #[new]
+    fn new() -> Self {
+        Version {
+            version: env!("CARGO_PKG_VERSION").to_string(),
+        }
+    }
+}
+    
 #[pymodule]
 fn rs_distances(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_wrapped(wrap_pyfunction!(calculate_spkd_impl))
-        .unwrap();
-    m.add_wrapped(wrap_pyfunction!(iterate_spiketrains_impl))
-        .unwrap();
+    m.add_wrapped(wrap_pyfunction!(calculate_spkd)).unwrap();
+    m.add_class::<Version>()?;
     Ok(())
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use env_logger::Builder;
     use log::LevelFilter;
     use ndarray::{ArrayBase, Dim, OwnedRepr};
     use std::env;
 
     #[test]
+    #[allow(dead_code)]
     fn test_calculate_spkd() {
         env::set_var("RUST_LOG", "debug");
         Builder::new().filter_level(LevelFilter::Debug).init();
 
         // Mock data - list of 1D np.ndarrays, 3 spike trains
-        let mut mock_data: Vec<ArrayBase<OwnedRepr<f64>, Dim<[usize; 1]>>> = vec![
+        let mut _mock_data: Vec<ArrayBase<OwnedRepr<f64>, Dim<[usize; 1]>>> = vec![
             ArrayBase::from(vec![0.1, 0.15, 0.2, 0.25, 0.3]),
             ArrayBase::from(vec![0.35, 0.4, 0.45, 0.5, 0.55]),
             ArrayBase::from(vec![0.6, 0.65, 0.7, 0.75, 0.8]),
         ];
 
         // simulate a view of data given from a numpy spike train
         let qvals = Array1::from(vec![1.0, 2.0, 3.0]);
 
         let numqvals = qvals.len();
-        let q_reshaped = qvals.into_shape((numqvals, 1, 1)).unwrap();
-
-        calculate_spkd(&mut mock_data, &q_reshaped, Option::None);
+        let _q_reshaped = qvals.into_shape((numqvals, 1, 1)).unwrap();
+        // calculate_spkd(&mut mock_data, &q_reshaped, Option::None);
     }
 }
```

### Comparing `rs_distances-0.6.0/Cargo.lock` & `rs_distances-0.8.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,17 @@
 checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.0.1"
+version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
+checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.3.2"
@@ -365,17 +365,17 @@
 dependencies = [
  "hashbrown",
  "stacker",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.1"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4ed2379f8603fa2b7509891660e802b88c70a79a6427a70abb5968054de2c28"
+checksum = "401a4694d2bf92537b6867d94de48c4842089645fdcdf6c71865b175d836e9c2"
 dependencies = [
  "clap_builder",
  "clap_derive",
  "once_cell",
 ]
 
 [[package]]
@@ -431,22 +431,22 @@
 dependencies = [
  "clap",
  "clap_complete",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.3.1"
+version = "4.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59e9ef9a08ee1c0e1f2e162121665ac45ac3783b0f897db7244ae75ad9a8f65b"
+checksum = "b8cd2b2a819ad6eec39e8f1d6b53001af1e5469f8c177579cdaeb313115b825f"
 dependencies = [
  "heck",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.19",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
@@ -710,17 +710,17 @@
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a9c384f161156f5260c24a097c56119f9be8c798586aecc13afbcbe7b7e26bf8"
+checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "fs-err"
 version = "2.9.0"
@@ -735,17 +735,17 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.9"
+version = "0.2.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
+checksum = "be4136b2a15dd319360be1c07d9933517ccf0be8f16bf62a3bee4f0d618df427"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -830,17 +830,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "idna"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14ddfc70884202db2244c223200c204c2bda1bc6e0998d11b5e024d657209e6"
+checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "ignore"
@@ -868,17 +868,17 @@
  "autocfg",
  "hashbrown",
  "serde",
 ]
 
 [[package]]
 name = "indicatif"
-version = "0.17.4"
+version = "0.17.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db45317f37ef454e6519b6c3ed7d377e5f23346f0823f86e65ca36912d1d0ef8"
+checksum = "8ff8cc23a7393a397ed1d7f56e6365cba772aba9f9912ab968b03043c395d057"
 dependencies = [
  "console",
  "instant",
  "number_prefix",
  "portable-atomic",
  "unicode-width",
 ]
@@ -960,29 +960,29 @@
  "fs-err",
  "glob",
  "goblin",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.144"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "linux-raw-sys"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
@@ -1280,17 +1280,17 @@
  "num-traits",
  "pyo3",
  "rustc-hash",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.17.2"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9670a07f94779e00908f3e686eab508878ebb390ba6e604d3a284c00e8d0487b"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "option-ext"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
 
@@ -1308,23 +1308,23 @@
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.7"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
- "redox_syscall 0.2.16",
+ "redox_syscall 0.3.5",
  "smallvec",
- "windows-sys 0.45.0",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "path-slash"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e91099d4268b0e11973f036e885d652fb0b21fedcf69738c627f94db6a44f42"
@@ -1356,17 +1356,17 @@
  "tracing",
  "unicode-width",
  "url",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
+checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
@@ -1610,19 +1610,19 @@
  "getrandom",
  "redox_syscall 0.2.16",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.3"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
- "aho-corasick 1.0.1",
+ "aho-corasick 1.0.2",
  "memchr",
  "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
@@ -1671,23 +1671,23 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rs-distances"
-version = "0.6.0"
+version = "0.8.1"
 dependencies = [
  "env_logger",
- "itertools",
  "log",
  "maturin",
  "ndarray",
  "numpy",
  "pyo3",
+ "rayon",
 ]
 
 [[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
@@ -1809,15 +1809,15 @@
 name = "serde_derive"
 version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.19",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -1931,17 +1931,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.18"
+version = "2.0.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+checksum = "a10b47e4921acc65b7d824cd92bc7b67a26382d8f4eadf3da65cb50aee6e6f3f"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -1959,23 +1959,24 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempfile"
-version = "3.5.0"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
+checksum = "31c0432476357e58790aaa47a8efb0c5138f137343f3b5f23bd36a27e3b0a6d6"
 dependencies = [
+ "autocfg",
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
  "rustix",
- "windows-sys 0.45.0",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
@@ -2017,32 +2018,32 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.19",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.21"
+version = "0.3.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
+checksum = "ea9e1b3cf1243ae005d9e74085d4d542f3125458f3a81af210d901dcd7411efd"
 dependencies = [
  "serde",
  "time-core",
 ]
 
 [[package]]
 name = "time-core"
@@ -2125,15 +2126,15 @@
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.19",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
@@ -2276,17 +2277,17 @@
  "url",
  "webpki",
  "webpki-roots",
 ]
 
 [[package]]
 name = "url"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d68c799ae75762b8c3fe375feb6600ef5602c883c5d21eb51c09f22b83c4643"
+checksum = "50bff7831e19200a85b17131d085c25d7811bc4e186efdaf54bbd132994a88cb"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
  "serde",
 ]
 
@@ -2357,15 +2358,15 @@
 checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.19",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
 version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2379,15 +2380,15 @@
 name = "wasm-bindgen-macro-support"
 version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.18",
+ "syn 2.0.19",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
 version = "0.2.86"
```

