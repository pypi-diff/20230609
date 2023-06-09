# Comparing `tmp/intel_sgx_ra-2.0a7.tar.gz` & `tmp/intel_sgx_ra-2.0a8-cp38-cp38-manylinux_2_34_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intel_sgx_ra-2.0a7.tar", last modified: Tue May 30 14:00:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

