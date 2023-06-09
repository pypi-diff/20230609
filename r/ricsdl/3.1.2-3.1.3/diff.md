# Comparing `tmp/ricsdl-3.1.2.tar.gz` & `tmp/ricsdl-3.1.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ricsdl-3.1.2.tar", last modified: Mon Dec 12 15:49:57 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

