# Comparing `tmp/pfizer_components-0.1.8.tar.gz` & `tmp/pfizer_components-0.1.9-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfizer_components-0.1.8.tar", last modified: Thu Jun  8 14:47:49 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

