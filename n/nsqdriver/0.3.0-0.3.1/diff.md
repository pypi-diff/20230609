# Comparing `tmp/nsqdriver-0.3.0.tar.gz` & `tmp/nsqdriver-0.3.1-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nsqdriver-0.3.0.tar", last modified: Wed Jun  7 06:20:56 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

