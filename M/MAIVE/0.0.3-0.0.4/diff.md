# Comparing `tmp/MAIVE-0.0.3.tar.gz` & `tmp/MAIVE-0.0.4-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MAIVE-0.0.3.tar", last modified: Fri Jun  9 14:09:57 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

