# Comparing `tmp/skytemple-rust-1.5.1.tar.gz` & `tmp/skytemple_rust-1.6.0a1-cp39-cp39-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skytemple-rust-1.5.1.tar", last modified: Thu May 18 18:29:58 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

