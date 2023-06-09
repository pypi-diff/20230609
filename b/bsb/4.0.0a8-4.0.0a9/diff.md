# Comparing `tmp/bsb-4.0.0a8.tar.gz` & `tmp/bsb-4.0.0a9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsb-4.0.0a8.tar", last modified: Fri May 13 10:40:39 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

