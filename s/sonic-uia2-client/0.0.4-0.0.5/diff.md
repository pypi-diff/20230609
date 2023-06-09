# Comparing `tmp/sonic-uia2-client-0.0.4.tar.gz` & `tmp/sonic_uia2_client-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonic-uia2-client-0.0.4.tar", last modified: Thu Jun  8 07:39:08 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

