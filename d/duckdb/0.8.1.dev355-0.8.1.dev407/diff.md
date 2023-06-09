# Comparing `tmp/duckdb-0.8.1.dev355.tar.gz` & `tmp/duckdb-0.8.1.dev407-cp37-cp37m-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duckdb-0.8.1.dev355.tar", last modified: Thu Jun  8 02:57:12 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

