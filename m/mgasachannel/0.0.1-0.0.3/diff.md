# Comparing `tmp/mgasachannel-0.0.1.tar.gz` & `tmp/mgasachannel-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mgasachannel-0.0.1.tar", last modified: Fri Jun  9 10:49:33 2023, max compression
+gzip compressed data, was "mgasachannel-0.0.3.tar", last modified: Fri Jun  9 11:35:02 2023, max compression
```

## Comparing `mgasachannel-0.0.1.tar` & `mgasachannel-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 10:49:33.802303 mgasachannel-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-06-09 10:41:54.000000 mgasachannel-0.0.1/LICENCE
--rw-rw-rw-   0        0        0      490 2023-06-09 10:49:33.802303 mgasachannel-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-09 10:42:57.000000 mgasachannel-0.0.1/README.md
--rw-rw-rw-   0        0        0      108 2023-06-09 10:45:56.000000 mgasachannel-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      631 2023-06-09 10:49:33.805303 mgasachannel-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-09 10:49:33.771306 mgasachannel-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-09 10:49:33.801469 mgasachannel-0.0.1/src/mgasachannel.egg-info/
--rw-rw-rw-   0        0        0      490 2023-06-09 10:49:33.000000 mgasachannel-0.0.1/src/mgasachannel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-06-09 10:49:33.000000 mgasachannel-0.0.1/src/mgasachannel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:49:33.000000 mgasachannel-0.0.1/src/mgasachannel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 10:49:33.000000 mgasachannel-0.0.1/src/mgasachannel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-09 11:35:02.930578 mgasachannel-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-06-09 10:41:54.000000 mgasachannel-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0      490 2023-06-09 11:35:02.931579 mgasachannel-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-09 10:42:57.000000 mgasachannel-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-09 10:45:56.000000 mgasachannel-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      631 2023-06-09 11:35:02.949996 mgasachannel-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-09 11:35:02.898583 mgasachannel-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-06-09 11:35:02.929235 mgasachannel-0.0.3/src/mgasachannel.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-06-09 11:35:02.000000 mgasachannel-0.0.3/src/mgasachannel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-06-09 11:35:02.000000 mgasachannel-0.0.3/src/mgasachannel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:35:02.000000 mgasachannel-0.0.3/src/mgasachannel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-09 11:35:02.000000 mgasachannel-0.0.3/src/mgasachannel.egg-info/top_level.txt
```

### Comparing `mgasachannel-0.0.1/setup.cfg` & `mgasachannel-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 6761 7361 6368 616e 6e65 6c0d   = mgasachannel.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e31  .version = 0.0.1
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e30 2e33  .version = 0.0.3
 00000030: 0d0a 6175 7468 6f72 203d 206d 6761 7361  ..author = mgasa
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 206d 6761 7361 2e6c 6f75 6361 7431 4067   mgasa.loucat1@g
 00000060: 6d61 696c 2e63 6f6d 0d0a 6465 7363 7269  mail.com..descri
 00000070: 7074 696f 6e20 3d20 4120 736d 616c 6c20  ption = A small 
 00000080: 6578 616d 706c 6520 7061 636b 6167 650d  example package.
 00000090: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
```

