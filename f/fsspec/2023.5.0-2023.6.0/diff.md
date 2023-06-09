# Comparing `tmp/fsspec-2023.5.0.tar.gz` & `tmp/fsspec-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fsspec-2023.5.0.tar", last modified: Sun May  7 19:05:16 2023, max compression
+gzip compressed data, was "fsspec-2023.6.0.tar", last modified: Fri Jun  9 17:31:49 2023, max compression
```

## Comparing `fsspec-2023.5.0.tar` & `fsspec-2023.6.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.225273 fsspec-2023.5.0/
--rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2023.5.0/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      110 2022-09-16 19:17:16.000000 fsspec-2023.5.0/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-05-07 19:05:16.225369 fsspec-2023.5.0/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     3464 2023-05-02 18:08:10.000000 fsspec-2023.5.0/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.226142 fsspec-2023.5.0/fsspec/
--rw-r--r--   0 mdurant    (502) staff       (20)     1800 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-05-07 19:05:16.226195 fsspec-2023.5.0/fsspec/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2406 2023-01-20 20:07:35.000000 fsspec-2023.5.0/fsspec/archive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    32277 2023-04-01 20:24:09.000000 fsspec-2023.5.0/fsspec/asyn.py
--rw-r--r--   0 mdurant    (502) staff       (20)    26395 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/caching.py
--rw-r--r--   0 mdurant    (502) staff       (20)     6358 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/callbacks.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4856 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/compression.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4193 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/config.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2023.5.0/fsspec/conftest.py
--rw-r--r--   0 mdurant    (502) staff       (20)    21507 2023-04-01 20:24:09.000000 fsspec-2023.5.0/fsspec/core.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2717 2022-11-08 01:04:48.000000 fsspec-2023.5.0/fsspec/dircache.py
--rw-r--r--   0 mdurant    (502) staff       (20)      348 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/exceptions.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10187 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/fuse.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10211 2023-01-09 18:41:59.000000 fsspec-2023.5.0/fsspec/generic.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13766 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/gui.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.224169 fsspec-2023.5.0/fsspec/implementations/
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/implementations/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)     8240 2023-03-12 01:59:42.000000 fsspec-2023.5.0/fsspec/implementations/arrow.py
--rw-r--r--   0 mdurant    (502) staff       (20)    30448 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/implementations/cached.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-04-01 20:24:09.000000 fsspec-2023.5.0/fsspec/implementations/dask.py
--rw-r--r--   0 mdurant    (502) staff       (20)    14648 2022-09-21 20:03:17.000000 fsspec-2023.5.0/fsspec/implementations/dbfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10826 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/implementations/dirfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10993 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/implementations/ftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4034 2022-11-28 20:11:28.000000 fsspec-2023.5.0/fsspec/implementations/git.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7328 2022-09-21 20:03:17.000000 fsspec-2023.5.0/fsspec/implementations/github.py
--rw-r--r--   0 mdurant    (502) staff       (20)    29225 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/implementations/http.py
--rw-r--r--   0 mdurant    (502) staff       (20)     3816 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/implementations/jupyter.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7248 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/implementations/libarchive.py
--rw-r--r--   0 mdurant    (502) staff       (20)    13672 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/implementations/local.py
--rw-r--r--   0 mdurant    (502) staff       (20)     9631 2023-01-09 15:22:42.000000 fsspec-2023.5.0/fsspec/implementations/memory.py
--rw-r--r--   0 mdurant    (502) staff       (20)    41638 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/implementations/reference.py
--rw-r--r--   0 mdurant    (502) staff       (20)     5464 2022-12-21 18:27:04.000000 fsspec-2023.5.0/fsspec/implementations/sftp.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10023 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/implementations/smb.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4088 2023-01-09 15:00:42.000000 fsspec-2023.5.0/fsspec/implementations/tar.py
--rw-r--r--   0 mdurant    (502) staff       (20)    15391 2023-03-16 17:24:28.000000 fsspec-2023.5.0/fsspec/implementations/webhdfs.py
--rw-r--r--   0 mdurant    (502) staff       (20)     4216 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/implementations/zip.py
--rw-r--r--   0 mdurant    (502) staff       (20)     7879 2023-03-13 14:48:58.000000 fsspec-2023.5.0/fsspec/mapping.py
--rw-r--r--   0 mdurant    (502) staff       (20)    19516 2022-11-04 01:13:55.000000 fsspec-2023.5.0/fsspec/parquet.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10079 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/registry.py
--rw-r--r--   0 mdurant    (502) staff       (20)    62483 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/spec.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.208241 fsspec-2023.5.0/fsspec/tests/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.225102 fsspec-2023.5.0/fsspec/tests/abstract/
--rw-r--r--   0 mdurant    (502) staff       (20)     2179 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/tests/abstract/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)    10751 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/tests/abstract/copy.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1388 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/tests/abstract/get.py
--rw-r--r--   0 mdurant    (502) staff       (20)     1338 2023-05-02 18:08:10.000000 fsspec-2023.5.0/fsspec/tests/abstract/put.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2195 2022-09-16 19:17:16.000000 fsspec-2023.5.0/fsspec/transaction.py
--rw-r--r--   0 mdurant    (502) staff       (20)    17103 2023-05-07 18:51:32.000000 fsspec-2023.5.0/fsspec/utils.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-07 19:05:16.217688 fsspec-2023.5.0/fsspec.egg-info/
--rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)     1416 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/SOURCES.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/dependency_links.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-16 19:21:25.000000 fsspec-2023.5.0/fsspec.egg-info/not-zip-safe
--rw-r--r--   0 mdurant    (502) staff       (20)      599 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/requires.txt
--rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-05-07 19:05:16.000000 fsspec-2023.5.0/fsspec.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      506 2023-05-02 18:08:10.000000 fsspec-2023.5.0/pyproject.toml
--rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.5.0/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      723 2023-05-07 19:05:16.225771 fsspec-2023.5.0/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     2452 2023-05-02 18:08:10.000000 fsspec-2023.5.0/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    78323 2023-03-12 01:59:42.000000 fsspec-2023.5.0/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:31:49.572502 fsspec-2023.6.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1513 2022-09-16 19:17:16.000000 fsspec-2023.6.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      110 2022-09-16 19:17:16.000000 fsspec-2023.6.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-06-09 17:31:49.572596 fsspec-2023.6.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     3464 2023-05-02 18:08:10.000000 fsspec-2023.6.0/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:31:49.573639 fsspec-2023.6.0/fsspec/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1800 2023-05-02 18:08:10.000000 fsspec-2023.6.0/fsspec/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      500 2023-06-09 17:31:49.573683 fsspec-2023.6.0/fsspec/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2406 2023-01-20 20:07:35.000000 fsspec-2023.6.0/fsspec/archive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    33978 2023-05-29 15:15:25.000000 fsspec-2023.6.0/fsspec/asyn.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    26379 2023-05-29 15:15:25.000000 fsspec-2023.6.0/fsspec/caching.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     6358 2022-12-21 18:27:04.000000 fsspec-2023.6.0/fsspec/callbacks.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4856 2022-12-21 18:27:04.000000 fsspec-2023.6.0/fsspec/compression.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4279 2023-05-27 16:05:15.000000 fsspec-2023.6.0/fsspec/config.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     1245 2022-09-21 20:03:17.000000 fsspec-2023.6.0/fsspec/conftest.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    21578 2023-06-09 17:31:05.000000 fsspec-2023.6.0/fsspec/core.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2717 2022-11-08 01:04:48.000000 fsspec-2023.6.0/fsspec/dircache.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      348 2022-09-16 19:17:16.000000 fsspec-2023.6.0/fsspec/exceptions.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10187 2023-05-29 15:15:25.000000 fsspec-2023.6.0/fsspec/fuse.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10211 2023-01-09 18:41:59.000000 fsspec-2023.6.0/fsspec/generic.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13860 2023-05-27 16:05:15.000000 fsspec-2023.6.0/fsspec/gui.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:31:49.571300 fsspec-2023.6.0/fsspec/implementations/
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.6.0/fsspec/implementations/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     8240 2023-03-12 01:59:42.000000 fsspec-2023.6.0/fsspec/implementations/arrow.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    30534 2023-05-29 15:15:25.000000 fsspec-2023.6.0/fsspec/implementations/cached.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4466 2023-04-01 20:24:09.000000 fsspec-2023.6.0/fsspec/implementations/dask.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    14660 2023-06-09 17:31:05.000000 fsspec-2023.6.0/fsspec/implementations/dbfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11092 2023-05-25 16:53:20.000000 fsspec-2023.6.0/fsspec/implementations/dirfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11463 2023-06-09 17:31:05.000000 fsspec-2023.6.0/fsspec/implementations/ftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4034 2022-11-28 20:11:28.000000 fsspec-2023.6.0/fsspec/implementations/git.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7328 2022-09-21 20:03:17.000000 fsspec-2023.6.0/fsspec/implementations/github.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    29225 2023-03-13 14:48:58.000000 fsspec-2023.6.0/fsspec/implementations/http.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3816 2022-09-16 19:17:16.000000 fsspec-2023.6.0/fsspec/implementations/jupyter.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7248 2022-12-21 18:27:04.000000 fsspec-2023.6.0/fsspec/implementations/libarchive.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13797 2023-06-09 17:31:05.000000 fsspec-2023.6.0/fsspec/implementations/local.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     9703 2023-05-27 16:05:15.000000 fsspec-2023.6.0/fsspec/implementations/memory.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    40766 2023-05-31 02:41:51.000000 fsspec-2023.6.0/fsspec/implementations/reference.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     5464 2022-12-21 18:27:04.000000 fsspec-2023.6.0/fsspec/implementations/sftp.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10023 2022-09-16 19:17:16.000000 fsspec-2023.6.0/fsspec/implementations/smb.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4071 2023-05-27 16:05:15.000000 fsspec-2023.6.0/fsspec/implementations/tar.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    15391 2023-03-16 17:24:28.000000 fsspec-2023.6.0/fsspec/implementations/webhdfs.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     4216 2023-05-12 17:14:40.000000 fsspec-2023.6.0/fsspec/implementations/zip.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     7879 2023-03-13 14:48:58.000000 fsspec-2023.6.0/fsspec/mapping.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    19516 2022-11-04 01:13:55.000000 fsspec-2023.6.0/fsspec/parquet.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    10255 2023-05-27 16:05:15.000000 fsspec-2023.6.0/fsspec/registry.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    63999 2023-06-09 17:31:05.000000 fsspec-2023.6.0/fsspec/spec.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:31:49.556410 fsspec-2023.6.0/fsspec/tests/
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:31:49.572335 fsspec-2023.6.0/fsspec/tests/abstract/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4702 2023-05-25 14:23:00.000000 fsspec-2023.6.0/fsspec/tests/abstract/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    13844 2023-05-25 14:23:00.000000 fsspec-2023.6.0/fsspec/tests/abstract/copy.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    12310 2023-05-25 14:23:00.000000 fsspec-2023.6.0/fsspec/tests/abstract/get.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    15792 2023-05-25 14:23:00.000000 fsspec-2023.6.0/fsspec/tests/abstract/put.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2195 2022-09-16 19:17:16.000000 fsspec-2023.6.0/fsspec/transaction.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    17155 2023-05-27 16:05:15.000000 fsspec-2023.6.0/fsspec/utils.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-06-09 17:31:49.566018 fsspec-2023.6.0/fsspec.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)     4828 2023-06-09 17:31:49.000000 fsspec-2023.6.0/fsspec.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)     1416 2023-06-09 17:31:49.000000 fsspec-2023.6.0/fsspec.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-06-09 17:31:49.000000 fsspec-2023.6.0/fsspec.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2022-09-16 19:21:25.000000 fsspec-2023.6.0/fsspec.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)      599 2023-06-09 17:31:49.000000 fsspec-2023.6.0/fsspec.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        7 2023-06-09 17:31:49.000000 fsspec-2023.6.0/fsspec.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      506 2023-05-02 18:08:10.000000 fsspec-2023.6.0/pyproject.toml
+-rw-r--r--   0 mdurant    (502) staff       (20)        0 2022-09-16 19:17:16.000000 fsspec-2023.6.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)     1044 2023-06-09 17:31:49.573204 fsspec-2023.6.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     2452 2023-05-02 18:08:10.000000 fsspec-2023.6.0/setup.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    78323 2023-03-12 01:59:42.000000 fsspec-2023.6.0/versioneer.py
```

### Comparing `fsspec-2023.5.0/LICENSE` & `fsspec-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/PKG-INFO` & `fsspec-2023.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: File-system specification
 Home-page: http://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
```

### Comparing `fsspec-2023.5.0/README.md` & `fsspec-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/__init__.py` & `fsspec-2023.6.0/fsspec/__init__.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/archive.py` & `fsspec-2023.6.0/fsspec/archive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/asyn.py` & `fsspec-2023.6.0/fsspec/asyn.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 import io
 import numbers
 import os
 import re
 import threading
 from contextlib import contextmanager
 from glob import has_magic
-from typing import Iterable
+from typing import TYPE_CHECKING, Iterable
 
 from .callbacks import _DEFAULT_CALLBACK
 from .exceptions import FSTimeoutError
+from .implementations.local import (
+    LocalFileSystem,
+    make_path_posix,
+    trailing_sep,
+    trailing_sep_maybe_asterisk,
+)
 from .spec import AbstractBufferedFile, AbstractFileSystem
 from .utils import is_exception, other_paths
 
 private = re.compile("_[^_]")
 iothread = [None]  # dedicated fsspec IO thread
 loop = [None]  # global event loop for any non-async instance
 _lock = None  # global lock placeholder
@@ -144,21 +150,26 @@
                 th = threading.Thread(target=loop[0].run_forever, name="fsspecIO")
                 th.daemon = True
                 th.start()
                 iothread[0] = th
     return loop[0]
 
 
-try:
+if TYPE_CHECKING:
     import resource
-except ImportError:
-    resource = None
-    ResourceError = OSError
+
+    ResourceError = resource.error
 else:
-    ResourceEror = resource.error
+    try:
+        import resource
+    except ImportError:
+        resource = None
+        ResourceError = OSError
+    else:
+        ResourceError = getattr(resource, "error", OSError)
 
 _DEFAULT_BATCH_SIZE = 128
 _NOFILES_DEFAULT_BATCH_SIZE = 1280
 
 
 def _get_batch_size(nofiles=False):
     from fsspec.config import conf
@@ -332,23 +343,31 @@
         **kwargs,
     ):
         if on_error is None and recursive:
             on_error = "ignore"
         elif on_error is None:
             on_error = "raise"
 
+        source_is_str = isinstance(path1, str)
         paths = await self._expand_path(path1, maxdepth=maxdepth, recursive=recursive)
+        if source_is_str and (not recursive or maxdepth is not None):
+            # Non-recursive glob does not copy directories
+            paths = [p for p in paths if not (trailing_sep(p) or await self._isdir(p))]
+            if not paths:
+                return
+
         isdir = isinstance(path2, str) and (
-            path2.endswith("/") or await self._isdir(path2)
+            trailing_sep(path2) or await self._isdir(path2)
         )
         path2 = other_paths(
             paths,
             path2,
-            exists=isdir and isinstance(path1, str) and not path1.endswith("/"),
+            exists=isdir and source_is_str and not trailing_sep_maybe_asterisk(path1),
             is_dir=isdir,
+            flatten=not source_is_str,
         )
         batch_size = batch_size or self.batch_size
         coros = [self._cp_file(p1, p2, **kwargs) for p1, p2 in zip(paths, path2)]
         result = await _run_coros_in_chunks(
             coros, batch_size=batch_size, return_exceptions=True, nofiles=True
         )
 
@@ -462,14 +481,15 @@
     async def _put(
         self,
         lpath,
         rpath,
         recursive=False,
         callback=_DEFAULT_CALLBACK,
         batch_size=None,
+        maxdepth=None,
         **kwargs,
     ):
         """Copy file(s) from local.
 
         Copies a specific file or tree of files (if recursive=True). If rpath
         ends with a "/", it will be assumed to be a directory, and target files
         will go within.
@@ -477,29 +497,35 @@
         The put_file method will be called concurrently on a batch of files. The
         batch_size option can configure the amount of futures that can be executed
         at the same time. If it is -1, then all the files will be uploaded concurrently.
         The default can be set for this instance by passing "batch_size" in the
         constructor, or for all instances by setting the "gather_batch_size" key
         in ``fsspec.config.conf``, falling back to 1/8th of the system limit .
         """
-        from .implementations.local import LocalFileSystem, make_path_posix
-
-        rpath = self._strip_protocol(rpath)
-        if isinstance(lpath, str):
+        source_is_str = isinstance(lpath, str)
+        if source_is_str:
             lpath = make_path_posix(lpath)
         fs = LocalFileSystem()
-        lpaths = fs.expand_path(lpath, recursive=recursive)
+        lpaths = fs.expand_path(lpath, recursive=recursive, maxdepth=maxdepth)
+        if source_is_str and (not recursive or maxdepth is not None):
+            # Non-recursive glob does not copy directories
+            lpaths = [p for p in lpaths if not (trailing_sep(p) or fs.isdir(p))]
+            if not lpaths:
+                return
+
         isdir = isinstance(rpath, str) and (
-            rpath.endswith("/") or await self._isdir(rpath)
+            trailing_sep(rpath) or await self._isdir(rpath)
         )
+        rpath = self._strip_protocol(rpath)
         rpaths = other_paths(
             lpaths,
             rpath,
-            exists=isdir and isinstance(lpath, str) and not lpath.endswith("/"),
+            exists=isdir and source_is_str and not trailing_sep_maybe_asterisk(lpath),
             is_dir=isdir,
+            flatten=not source_is_str,
         )
 
         is_dir = {l: os.path.isdir(l) for l in lpaths}
         rdirs = [r for l, r in zip(lpaths, rpaths) if is_dir[l]]
         file_pairs = [(l, r) for l, r in zip(lpaths, rpaths) if not is_dir[l]]
 
         await asyncio.gather(*[self._makedirs(d, exist_ok=True) for d in rdirs])
@@ -515,15 +541,21 @@
             coros, batch_size=batch_size, callback=callback
         )
 
     async def _get_file(self, rpath, lpath, **kwargs):
         raise NotImplementedError
 
     async def _get(
-        self, rpath, lpath, recursive=False, callback=_DEFAULT_CALLBACK, **kwargs
+        self,
+        rpath,
+        lpath,
+        recursive=False,
+        callback=_DEFAULT_CALLBACK,
+        maxdepth=None,
+        **kwargs,
     ):
         """Copy file(s) to local.
 
         Copies a specific file or tree of files (if recursive=True). If lpath
         ends with a "/", it will be assumed to be a directory, and target files
         will go within. Can submit a list of paths, which may be glob-patterns
         and will be expanded.
@@ -531,29 +563,39 @@
         The get_file method will be called concurrently on a batch of files. The
         batch_size option can configure the amount of futures that can be executed
         at the same time. If it is -1, then all the files will be uploaded concurrently.
         The default can be set for this instance by passing "batch_size" in the
         constructor, or for all instances by setting the "gather_batch_size" key
         in ``fsspec.config.conf``, falling back to 1/8th of the system limit .
         """
-        from fsspec.implementations.local import LocalFileSystem, make_path_posix
-
+        source_is_str = isinstance(rpath, str)
         # First check for rpath trailing slash as _strip_protocol removes it.
-        rpath_trailing_slash = isinstance(rpath, str) and rpath.endswith("/")
+        source_not_trailing_sep = source_is_str and not trailing_sep_maybe_asterisk(
+            rpath
+        )
         rpath = self._strip_protocol(rpath)
-        lpath = make_path_posix(lpath)
         rpaths = await self._expand_path(rpath, recursive=recursive)
+        if source_is_str and (not recursive or maxdepth is not None):
+            # Non-recursive glob does not copy directories
+            rpaths = [
+                p for p in rpaths if not (trailing_sep(p) or await self._isdir(p))
+            ]
+            if not rpaths:
+                return
+
+        lpath = make_path_posix(lpath)
         isdir = isinstance(lpath, str) and (
-            lpath.endswith("/") or LocalFileSystem().isdir(lpath)
+            trailing_sep(lpath) or LocalFileSystem().isdir(lpath)
         )
         lpaths = other_paths(
             rpaths,
             lpath,
-            exists=isdir and not rpath_trailing_slash,
+            exists=isdir and source_not_trailing_sep,
             is_dir=isdir,
+            flatten=not source_is_str,
         )
         [os.makedirs(os.path.dirname(lp), exist_ok=True) for lp in lpaths]
         batch_size = kwargs.pop("batch_size", self.batch_size)
 
         coros = []
         callback.set_size(len(lpaths))
         for lpath, rpath in zip(lpaths, rpaths):
@@ -568,15 +610,15 @@
             return (await self._info(path))["type"] == "file"
         except:  # noqa: E722
             return False
 
     async def _isdir(self, path):
         try:
             return (await self._info(path))["type"] == "directory"
-        except IOError:
+        except OSError:
             return False
 
     async def _size(self, path):
         return (await self._info(path)).get("size", None)
 
     async def _sizes(self, paths, batch_size=None):
         batch_size = batch_size or self.batch_size
@@ -605,29 +647,29 @@
         full_dirs = {}
         dirs = {}
         files = {}
 
         detail = kwargs.pop("detail", False)
         try:
             listing = await self._ls(path, detail=True, **kwargs)
-        except (FileNotFoundError, IOError):
+        except (FileNotFoundError, OSError):
             if detail:
                 yield path, {}, {}
             else:
                 yield path, [], []
             return
 
         for info in listing:
             # each info name must be at least [path]/part , but here
             # we check also for names like [path]/part/
             pathname = info["name"].rstrip("/")
             name = pathname.rsplit("/", 1)[-1]
             if info["type"] == "directory" and pathname != path:
                 # do not include "self" path
-                full_dirs[pathname] = info
+                full_dirs[name] = pathname
                 dirs[name] = info
             elif pathname == path:
                 # file-like with same name as give path
                 files[""] = info
             else:
                 files[name] = info
 
@@ -637,16 +679,18 @@
             yield path, list(dirs), list(files)
 
         if maxdepth is not None:
             maxdepth -= 1
             if maxdepth < 1:
                 return
 
-        for d in full_dirs:
-            async for _ in self._walk(d, maxdepth=maxdepth, detail=detail, **kwargs):
+        for d in dirs:
+            async for _ in self._walk(
+                full_dirs[d], maxdepth=maxdepth, detail=detail, **kwargs
+            ):
                 yield _
 
     async def _glob(self, path, **kwargs):
         import re
 
         ends = path.endswith("/")
         path = self._strip_protocol(path)
@@ -760,28 +804,33 @@
             out = set()
             path = [self._strip_protocol(p) for p in path]
             for p in path:  # can gather here
                 if has_magic(p):
                     bit = set(await self._glob(p))
                     out |= bit
                     if recursive:
+                        # glob call above expanded one depth so if maxdepth is defined
+                        # then decrement it in expand_path call below. If it is zero
+                        # after decrementing then avoid expand_path call.
+                        if maxdepth is not None and maxdepth <= 1:
+                            continue
                         out |= set(
                             await self._expand_path(
-                                list(bit), recursive=recursive, maxdepth=maxdepth
+                                list(bit),
+                                recursive=recursive,
+                                maxdepth=maxdepth - 1 if maxdepth is not None else None,
                             )
                         )
                     continue
                 elif recursive:
                     rec = set(await self._find(p, maxdepth=maxdepth, withdirs=True))
                     out |= rec
                 if p not in out and (recursive is False or (await self._exists(p))):
                     # should only check once, for the root
                     out.add(p)
-            # reduce depth on each recursion level unless None or 0
-            maxdepth = maxdepth if not maxdepth else maxdepth - 1
         if not out:
             raise FileNotFoundError(path)
         return list(sorted(out))
 
     async def _mkdir(self, path, create_parents=True, **kwargs):
         pass  # not necessary to implement, may not have directories
```

### Comparing `fsspec-2023.5.0/fsspec/caching.py` & `fsspec-2023.6.0/fsspec/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import collections
 import functools
-import io
 import logging
 import math
 import os
 import threading
 import warnings
 from concurrent.futures import ThreadPoolExecutor
 
@@ -70,20 +69,20 @@
 
         # posix version
         if self.location is None or not os.path.exists(self.location):
             if self.location is None:
                 fd = tempfile.TemporaryFile()
                 self.blocks = set()
             else:
-                fd = io.open(self.location, "wb+")
+                fd = open(self.location, "wb+")
             fd.seek(self.size - 1)
             fd.write(b"1")
             fd.flush()
         else:
-            fd = io.open(self.location, "rb+")
+            fd = open(self.location, "rb+")
 
         return mmap.mmap(fd.fileno(), self.size)
 
     def _fetch(self, start, end):
         logger.debug(f"MMap cache fetching {start}-{end}")
         if start is None:
             start = 0
```

### Comparing `fsspec-2023.5.0/fsspec/callbacks.py` & `fsspec-2023.6.0/fsspec/callbacks.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/compression.py` & `fsspec-2023.6.0/fsspec/compression.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/config.py` & `fsspec-2023.6.0/fsspec/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
+from __future__ import annotations
+
 import configparser
 import json
 import os
 import warnings
+from typing import Any
 
-conf = {}
+conf: dict[str, dict[str, Any]] = {}
 default_conf_dir = os.path.join(os.path.expanduser("~"), ".config/fsspec")
 conf_dir = os.environ.get("FSSPEC_CONFIG_DIR", default_conf_dir)
 
 
 def set_conf_env(conf_dict, envdict=os.environ):
     """Set config values from environment variables
```

### Comparing `fsspec-2023.5.0/fsspec/conftest.py` & `fsspec-2023.6.0/fsspec/conftest.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/core.py` & `fsspec-2023.6.0/fsspec/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -432,25 +432,28 @@
     they map across to see the latest online documentation:
 
     - For implementations built into ``fsspec`` see
       https://filesystem-spec.readthedocs.io/en/latest/api.html#built-in-implementations
     - For implementations in separate packages see
       https://filesystem-spec.readthedocs.io/en/latest/api.html#other-known-implementations
     """
-    return open_files(
+    out = open_files(
         urlpath=[urlpath],
         mode=mode,
         compression=compression,
         encoding=encoding,
         errors=errors,
         protocol=protocol,
         newline=newline,
         expand=False,
         **kwargs,
-    )[0]
+    )
+    if not out:
+        raise FileNotFoundError(urlpath)
+    return out[0]
 
 
 def open_local(url, mode="rb", **storage_options):
     """Open file(s) which can be resolved to local
 
     For files which either are local, or get downloaded upon open
     (e.g., by file caching)
```

### Comparing `fsspec-2023.5.0/fsspec/dircache.py` & `fsspec-2023.6.0/fsspec/dircache.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/fuse.py` & `fsspec-2023.6.0/fsspec/fuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         # maybe should be no-op since open with write sets size to zero anyway
         self.fs.touch(fn)
 
     def unlink(self, path):
         fn = "".join([self.root, path.lstrip("/")])
         try:
             self.fs.rm(fn, False)
-        except (IOError, FileNotFoundError):
+        except (OSError, FileNotFoundError):
             raise FuseOSError(EIO)
 
     def release(self, path, fh):
         try:
             if fh in self.cache:
                 f = self.cache[fh]
                 f.close()
```

### Comparing `fsspec-2023.5.0/fsspec/generic.py` & `fsspec-2023.6.0/fsspec/generic.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/gui.py` & `fsspec-2023.6.0/fsspec/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast
 import contextlib
 import logging
 import os
 import re
+from typing import ClassVar, Sequence
 
 import panel as pn
 
 from .core import OpenFile, get_filesystem_class, split_protocol
 from .registry import known_implementations
 
 pn.extension()
@@ -21,17 +22,19 @@
 
     The method ``_register`` should be called as widgets are added, and external
     code should call ``connect`` to associate callbacks.
 
     By default, all signals emit a DEBUG logging statement.
     """
 
-    signals = []  # names of signals that this class may emit
-    # each of which must be set by _register for any new instance
-    slots = []  # names of actions that this class may respond to
+    # names of signals that this class may emit each of which must be
+    # set by _register for any new instance
+    signals: ClassVar[Sequence[str]] = []
+    # names of actions that this class may respond to
+    slots: ClassVar[Sequence[str]] = []
 
     # each of which must be a method name
 
     def __init__(self):
         self._ignoring_events = False
         self._sigs = {}
         self._map = {}
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/arrow.py` & `fsspec-2023.6.0/fsspec/implementations/arrow.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/cached.py` & `fsspec-2023.6.0/fsspec/implementations/cached.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import contextlib
 import hashlib
 import inspect
 import logging
 import os
 import pickle
 import tempfile
 import time
 from shutil import rmtree
+from typing import ClassVar
 
 from fsspec import AbstractFileSystem, filesystem
 from fsspec.callbacks import _DEFAULT_CALLBACK
 from fsspec.compression import compr
 from fsspec.core import BaseCache, MMapCache
 from fsspec.exceptions import BlocksizeMismatchError
 from fsspec.spec import AbstractBufferedFile
@@ -35,15 +38,15 @@
     - the block-size must be the same for each access of a given file, unless
       all blocks of the file have already been read
     - caching can only be applied to file-systems which produce files
       derived from fsspec.spec.AbstractBufferedFile ; LocalFileSystem is also
       allowed, for testing
     """
 
-    protocol = ("blockcache", "cached")
+    protocol: ClassVar[str | tuple[str, ...]] = ("blockcache", "cached")
 
     def __init__(
         self,
         target_protocol=None,
         cache_storage="TMP",
         cache_check=10,
         check_files=False,
@@ -394,15 +397,15 @@
         c = self.cached_files[-1][path]
         if c["blocks"] is not True and len(c["blocks"]) * f.blocksize >= f.size:
             c["blocks"] = True
         try:
             logger.debug("going to save")
             self.save_cache()
             logger.debug("saved")
-        except (IOError, OSError):
+        except OSError:
             logger.debug("Cache saving failed while closing file")
         except NameError:
             logger.debug("Cache save failed due to interpreter shutdown")
         close()
         f.closed = True
 
     def __getattribute__(self, item):
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/dask.py` & `fsspec-2023.6.0/fsspec/implementations/dask.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/dbfs.py` & `fsspec-2023.6.0/fsspec/implementations/dbfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,22 +436,22 @@
         if final:
             self.fs._close_handle(handle=self.handle)
             return True
 
     def _fetch_range(self, start, end):
         """Internal function to download a block of data"""
         return_buffer = b""
-
-        total_length = end - start
-        for chunk_start, chunk_end in self._to_sized_blocks(total_length):
+        length = end - start
+        for chunk_start, chunk_end in self._to_sized_blocks(length, start):
             return_buffer += self.fs._get_data(
                 path=self.path, start=chunk_start, end=chunk_end
             )
 
         return return_buffer
 
-    def _to_sized_blocks(self, total_length):
+    def _to_sized_blocks(self, length, start=0):
         """Helper function to split a range from 0 to total_length into bloksizes"""
-        for data_chunk in range(0, total_length, self.blocksize):
+        end = start + length
+        for data_chunk in range(start, end, self.blocksize):
             data_start = data_chunk
-            data_end = min(total_length, data_chunk + self.blocksize)
+            data_end = min(end, data_chunk + self.blocksize)
             yield data_start, data_end
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/dirfs.py` & `fsspec-2023.6.0/fsspec/implementations/dirfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from .. import filesystem
 from ..asyn import AsyncFileSystem
 
 
 class DirFileSystem(AsyncFileSystem):
+    """Directory prefix filesystem
+
+    The DirFileSystem is a filesystem-wrapper. It assumes every path it is dealing with
+    is relative to the `path`. After performing the necessary paths operation it
+    delegates everything to the wrapped filesystem.
+    """
+
     def __init__(
         self,
         path=None,
         fs=None,
         fo=None,
         target_protocol=None,
         target_options=None,
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/ftp.py` & `fsspec-2023.6.0/fsspec/implementations/ftp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import os
+import sys
 import uuid
+import warnings
 from ftplib import FTP, Error, error_perm
 from typing import Any
 
 from ..spec import AbstractBufferedFile, AbstractFileSystem
 from ..utils import infer_storage_options, isfilelike
 
 
@@ -20,14 +22,15 @@
         port=21,
         username=None,
         password=None,
         acct=None,
         block_size=None,
         tempdir=None,
         timeout=30,
+        encoding="utf-8",
         **kwargs,
     ):
         """
         You can use _get_kwargs_from_urls to get some kwargs from
         a reasonable FTP url.
 
         Authentication will be anonymous if username/password are not
@@ -47,29 +50,38 @@
             Some servers also need an "account" string for auth
         block_size: int or None
             If given, the read-ahead or write buffer size.
         tempdir: str
             Directory on remote to put temporary files when in a transaction
         timeout: int
             Timeout of the ftp connection in seconds
+        encoding: str
+            Encoding to use for directories and filenames in FTP connection
         """
         super(FTPFileSystem, self).__init__(**kwargs)
         self.host = host
         self.port = port
         self.tempdir = tempdir or "/tmp"
         self.cred = username, password, acct
         self.timeout = timeout
+        self.encoding = encoding
         if block_size is not None:
             self.blocksize = block_size
         else:
             self.blocksize = 2**16
         self._connect()
 
     def _connect(self):
-        self.ftp = FTP(timeout=self.timeout)
+        if sys.version_info >= (3, 9):
+            self.ftp = FTP(timeout=self.timeout, encoding=self.encoding)
+        elif self.encoding:
+            warnings.warn("`encoding` not supported for python<3.9, ignoring")
+            self.ftp = FTP(timeout=self.timeout)
+        else:
+            self.ftp = FTP(timeout=self.timeout)
         self.ftp.connect(self.host, self.port)
         self.ftp.login(*self.cred)
 
     @classmethod
     def _strip_protocol(cls, path):
         return "/" + infer_storage_options(path)["path"].lstrip("/").rstrip("/")
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/git.py` & `fsspec-2023.6.0/fsspec/implementations/git.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/github.py` & `fsspec-2023.6.0/fsspec/implementations/github.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/http.py` & `fsspec-2023.6.0/fsspec/implementations/http.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/jupyter.py` & `fsspec-2023.6.0/fsspec/implementations/jupyter.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/libarchive.py` & `fsspec-2023.6.0/fsspec/implementations/libarchive.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/local.py` & `fsspec-2023.6.0/fsspec/implementations/local.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         for field in ["mode", "uid", "gid", "mtime", "ino", "nlink"]:
             result[field] = getattr(out, "st_" + field)
         if result["islink"]:
             result["destination"] = os.readlink(path)
             try:
                 out2 = os.stat(path, follow_symlinks=True)
                 result["size"] = out2.st_size
-            except IOError:
+            except OSError:
                 result["size"] = 0
         return result
 
     def lexists(self, path, **kwargs):
         return osp.lexists(path)
 
     def cp_file(self, path1, path2, **kwargs):
@@ -152,24 +152,25 @@
         dst = self._strip_protocol(dst)
         os.symlink(src, dst, **kwargs)
 
     def islink(self, path) -> bool:
         return os.path.islink(self._strip_protocol(path))
 
     def rm_file(self, path):
-        os.remove(path)
+        os.remove(self._strip_protocol(path))
 
     def rm(self, path, recursive=False, maxdepth=None):
         if not isinstance(path, list):
             path = [path]
 
         for p in path:
             p = self._strip_protocol(p).rstrip("/")
-            if recursive and self.isdir(p):
-
+            if self.isdir(p):
+                if not recursive:
+                    raise ValueError("Cannot delete directory, set recursive=True")
                 if osp.abspath(p) == os.getcwd():
                     raise ValueError("Cannot delete current working directory")
                 shutil.rmtree(p)
             else:
                 os.remove(p)
 
     def unstrip_protocol(self, name):
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/memory.py` & `fsspec-2023.6.0/fsspec/implementations/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from __future__ import absolute_import, division, print_function
+from __future__ import absolute_import, annotations, division, print_function
 
 import logging
 from datetime import datetime
 from errno import ENOTEMPTY
 from io import BytesIO
+from typing import Any, ClassVar
 
 from fsspec import AbstractFileSystem
 
 logger = logging.Logger("fsspec.memoryfs")
 
 
 class MemoryFileSystem(AbstractFileSystem):
     """A filesystem based on a dict of BytesIO objects
 
     This is a global filesystem so instances of this class all point to the same
     in memory filesystem.
     """
 
-    store = {}  # global, do not overwrite!
+    store: ClassVar[dict[str, Any]] = {}  # global, do not overwrite!
     pseudo_dirs = [""]  # global, do not overwrite!
     protocol = "memory"
     root_marker = "/"
 
     @classmethod
     def _strip_protocol(cls, path):
         if path.startswith("memory://"):
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/reference.py` & `fsspec-2023.6.0/fsspec/implementations/reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import base64
 import collections
 import io
 import itertools
 import logging
+import math
 import os
 from functools import lru_cache
+from typing import TYPE_CHECKING
 
 import fsspec.core
 
 try:
     import ujson as json
 except ImportError:
-    import json
+    if not TYPE_CHECKING:
+        import json
 
 from ..asyn import AsyncFileSystem
 from ..callbacks import _DEFAULT_CALLBACK
 from ..core import filesystem, open, split_protocol
 from ..utils import isfilelike, merge_offset_ranges, other_paths
 
 logger = logging.getLogger("fsspec.reference")
@@ -54,25 +57,34 @@
 class RefsValuesView(collections.abc.ValuesView):
     def __iter__(self):
         for val in self._mapping.zmetadata.values():
             yield json.dumps(val).encode()
         yield from self._mapping._items.values()
         for field in self._mapping.listdir():
             chunk_sizes = self._mapping._get_chunk_sizes(field)
-            if chunk_sizes.size == 0:
+            if len(chunk_sizes) == 0:
                 yield self._mapping[field + "/0"]
                 continue
             yield from self._mapping._generate_all_records(field)
 
 
 class RefsItemsView(collections.abc.ItemsView):
     def __iter__(self):
         return zip(self._mapping.keys(), self._mapping.values())
 
 
+def ravel_multi_index(idx, sizes):
+    val = 0
+    mult = 1
+    for i, s in zip(idx[::-1], sizes[::-1]):
+        val += i * mult
+        mult *= s
+    return val
+
+
 class LazyReferenceMapper(collections.abc.MutableMapping):
     """Interface to read parquet store as if it were a standard kerchunk
     references dict."""
 
     # import is class level to prevent numpy dep requirement for fsspec
     @property
     def np(self):
@@ -83,19 +95,15 @@
     @property
     def pd(self):
         import pandas as pd
 
         return pd
 
     def __init__(
-        self,
-        root,
-        fs=None,
-        out_root=None,
-        cache_size=128,
+        self, root, fs=None, out_root=None, cache_size=128, categorical_threshold=10
     ):
         """
         Parameters
         ----------
         root : str
             Root of parquet store
         fs : fsspec.AbstractFileSystem
@@ -112,27 +120,27 @@
         with self.fs.open("/".join([self.root, ".zmetadata"]), "rb") as f:
             self._items[".zmetadata"] = f.read()
         met = json.loads(self._items[".zmetadata"])
         self.record_size = met["record_size"]
         self.zmetadata = met["metadata"]
         self.url = self.root + "/{field}/refs.{record}.parq"
         self.out_root = out_root or self.root
+        self.cat_thresh = categorical_threshold
 
         # Define function to open and decompress refs
         @lru_cache(maxsize=cache_size)
         def open_refs(field, record):
             """cached parquet file loader"""
             path = self.url.format(field=field, record=record)
             with self.fs.open(path) as f:
+                # TODO: since all we do is iterate, is arrow without pandas
+                #  better here?
                 df = self.pd.read_parquet(f, engine="fastparquet")
             refs = {c: df[c].values for c in df.columns}
-            # Return both df and dict of views because the former is
-            # more convenient for iterating sequentially while the latter
-            # is faster for random access.
-            return df, refs
+            return refs
 
         self.open_refs = open_refs
 
     @staticmethod
     def create(record_size, root, fs, **kwargs):
         met = {"metadata": {}, "record_size": record_size}
         fs.pipe("/".join([root, ".zmetadata"]), json.dumps(met).encode())
@@ -229,15 +237,15 @@
             return maybe
 
         # Chunk keys can be loaded from row group and cached in LRU cache
         try:
             record, ri, chunk_size = self._key_to_record(key)
             if chunk_size == 0:
                 return b""
-            _, refs = self.open_refs(field, record)
+            refs = self.open_refs(field, record)
         except (ValueError, TypeError, FileNotFoundError):
             raise KeyError(key)
         columns = ["path", "offset", "size", "raw"]
         selection = [refs[c][ri] if c in refs else None for c in columns]
         raw = selection[-1]
         if raw is not None:
             return raw
@@ -245,74 +253,80 @@
             raise KeyError("This reference has been deleted")
         if selection[1:3] == [0, 0]:
             # URL only
             return selection[:1]
         # URL, offset, size
         return selection[:3]
 
+    @lru_cache(4096)
     def _key_to_record(self, key):
         """Details needed to construct a reference for one key"""
         field, chunk = key.split("/")
         chunk_sizes = self._get_chunk_sizes(field)
-        if chunk_sizes.size == 0:
+        if len(chunk_sizes) == 0:
             return 0, 0, 0
-        chunk_idx = self.np.array([int(c) for c in chunk.split(".")])
-        chunk_number = self.np.ravel_multi_index(chunk_idx, chunk_sizes)
+        chunk_idx = [int(c) for c in chunk.split(".")]
+        chunk_number = ravel_multi_index(chunk_idx, chunk_sizes)
         record = chunk_number // self.record_size
         ri = chunk_number % self.record_size
-        return record, ri, chunk_sizes.size
+        return record, ri, len(chunk_sizes)
 
     def _get_chunk_sizes(self, field):
         """The number of chunks along each axis for a given field"""
         if field not in self.chunk_sizes:
             zarray = self.zmetadata[f"{field}/.zarray"]
-            size_ratio = self.np.array(zarray["shape"]) / self.np.array(
-                zarray["chunks"]
-            )
-            self.chunk_sizes[field] = self.np.ceil(size_ratio).astype(int)
+            size_ratio = [
+                math.ceil(s / c) for s, c in zip(zarray["shape"], zarray["chunks"])
+            ]
+            self.chunk_sizes[field] = size_ratio
         return self.chunk_sizes[field]
 
     def _generate_record(self, field, record):
         """The references for a given parquet file of a given field"""
-        df, _ = self.open_refs(field, record)
-        it = df.itertuples(name=None, index=False)
-        if df.columns.size == 3:
+        refs = self.open_refs(field, record)
+        it = iter(zip(refs.values()))
+        if len(refs) == 3:
             # All urls
             return (list(t) for t in it)
-        elif df.columns.size == 1:
+        elif len(refs) == 1:
             # All raws
-            return (t[0] for t in it)
+            return refs["raw"]
         else:
             # Mix of urls and raws
             return (list(t[:3]) if not t[3] else t[3] for t in it)
 
     def _generate_all_records(self, field):
         """Load all the references within a field by iterating over the parquet files"""
-        chunk_size = self._get_chunk_sizes(field)
-        nrec = int(self.np.ceil(self.np.product(chunk_size) / self.record_size))
+        nrec = 1
+        for ch in self._get_chunk_sizes(field):
+            nrec *= ch
+        nrec = math.ceil(nrec / self.record_size)
         for record in range(nrec):
             yield from self._generate_record(field, record)
 
     def values(self):
         return RefsValuesView(self)
 
     def items(self):
         return RefsItemsView(self)
 
+    def __hash__(self):
+        return id(self)
+
+    @lru_cache(20)
     def __getitem__(self, key):
         return self._load_one_key(key)
 
     def __setitem__(self, key, value):
-        print(key, value)
         if "/" in key and not self._is_meta(key):
             field, chunk = key.split("/")
-            record, _, _ = self._key_to_record(key)
+            record, i, _ = self._key_to_record(key)
             subdict = self._items.setdefault((field, record), {})
-            subdict[chunk] = value
-            if len(subdict) == self._output_size(field, record):
+            subdict[i] = value
+            if len(subdict) == self.record_size:
                 self.write(field, record)
         else:
             # metadata or top-level
             self._items[key] = value
             self.zmetadata[key] = json.loads(
                 value.decode() if isinstance(value, bytes) else value
             )
@@ -328,66 +342,38 @@
             del self.zmetadata[key]
         else:
             if "/" in key and not self._is_meta(key):
                 field, chunk = key.split("/")
                 record, _, _ = self._key_to_record(key)
                 subdict = self._items.setdefault((field, record), {})
                 subdict[chunk] = None
-                if len(subdict) == self._output_size(field, record):
+                if len(subdict) == self.record_size:
                     self.write(field, record)
             else:
                 # metadata or top-level
                 self._items[key] = None
 
-    def _output_size(self, field, record):
-        np = self.np
-
-        zarray = json.loads(self[f"{field}/.zarray"])
-        chunk_sizes = np.ceil(np.array(zarray["shape"]) / np.array(zarray["chunks"]))
-        if chunk_sizes.size == 0:
-            chunk_sizes = np.array([0])
-        nchunks = int(np.product(chunk_sizes))
-        nrec = nchunks // self.record_size
-        rem = nchunks % self.record_size
-        if rem != 0:
-            nrec += 1
-        return self.record_size if record < nrec - 1 else rem
-
     def write(self, field, record, base_url=None, storage_options=None):
         # extra requirements if writing
         import kerchunk.df
         import numpy as np
         import pandas as pd
 
         # TODO: if the dict is incomplete, also load records and merge in
         partition = self._items[(field, record)]
         fn = f"{base_url or self.out_root}/{field}/refs.{record}.parq"
-        output_size = self._output_size(field, record)
 
         ####
         paths = np.full(self.record_size, np.nan, dtype="O")
         offsets = np.zeros(self.record_size, dtype="int64")
         sizes = np.zeros(self.record_size, dtype="int64")
         raws = np.full(self.record_size, np.nan, dtype="O")
-        zarray = json.loads(self[f"{field}/.zarray"])
-        shape = np.array(zarray["shape"])
-        chunks = np.array(zarray["chunks"])
         nraw = 0
         npath = 0
-        for key, data in partition.items():
-            chunk_id = key.rsplit("/", 1)[-1]
-            chunk_ints = [int(ch) for ch in chunk_id.split(".")]
-            i = 0
-            mult = 1
-            for chunk_int, sh, ch in zip(chunk_ints[::-1], shape[::-1], chunks[::-1]):
-                i += chunk_int * mult
-                mult *= sh // ch
-            j = i % self.record_size
-            # Make note if expected number of chunks differs from actual
-            # number found in references
+        for j, data in partition.items():
             if isinstance(data, list):
                 npath += 1
                 paths[j] = data[0]
                 if len(data) > 1:
                     offsets[j] = data[1]
                     sizes[j] = data[2]
             else:
@@ -398,15 +384,17 @@
             dict(
                 path=paths,
                 offset=offsets,
                 size=sizes,
                 raw=raws,
             ),
             copy=False,
-        )[:output_size]
+        )
+        if df.path.count() / (df.path.nunique() or 1) > self.cat_thresh:
+            df["path"] = df["path"].astype("category")
         object_encoding = dict(raw="bytes", path="utf8")
         has_nulls = ["path", "raw"]
 
         self.fs.mkdirs(f"{base_url or self.out_root}/{field}", exist_ok=True)
         df.to_parquet(
             fn,
             engine="fastparquet",
@@ -427,24 +415,23 @@
 
         Parameters
         ----------
         base_url: str
             Location of the output
         """
         # write what we have so far and clear sub chunks
-        for thing in self._items:
+        for thing in list(self._items):
             if isinstance(thing, tuple):
                 field, record = thing
-                if self._items.get((record, field)):
-                    self.write(
-                        field,
-                        record,
-                        base_url=base_url,
-                        storage_options=storage_options,
-                    )
+                self.write(
+                    field,
+                    record,
+                    base_url=base_url,
+                    storage_options=storage_options,
+                )
 
         # gather .zmetadata from self._items and write that too
         for k in list(self._items):
             if k != ".zmetadata" and ".z" in k:
                 self.zmetadata[k] = json.loads(self._items.pop(k))
         met = {"metadata": self.zmetadata, "record_size": self.record_size}
         self._items[".zmetadata"] = json.dumps(met).encode()
@@ -490,18 +477,18 @@
 
     def _keys_in_field(self, field):
         """List key names in given field
 
         Produces strings like "field/x.y" appropriate from the chunking of the array
         """
         chunk_sizes = self._get_chunk_sizes(field)
-        if chunk_sizes.size == 0:
+        if len(chunk_sizes) == 0:
             yield field + "/0"
             return
-        inds = self.np.ndindex(*chunk_sizes)
+        inds = itertools.product(*(range(i) for i in chunk_sizes))
         for ind in inds:
             yield field + "/" + ".".join([str(c) for c in ind])
 
 
 class ReferenceFileSystem(AsyncFileSystem):
     """View byte ranges of some other file as a file system
     Initial version: single file system target, which must support
@@ -602,25 +589,26 @@
         self._dircache = {}
         self.max_gap = max_gap
         self.max_block = max_block
         if isinstance(fo, str):
             dic = dict(
                 **(ref_storage_args or target_options or {}), protocol=target_protocol
             )
-            ref_fs, fo = fsspec.core.url_to_fs(fo, **dic)
+            ref_fs, fo2 = fsspec.core.url_to_fs(fo, **dic)
             if ref_fs.isfile(fo):
                 # text JSON
-                with ref_fs.open(fo, "rb") as f:
+                with fsspec.open(fo, "rb", **dic) as f:
                     logger.info("Read reference from URL %s", fo)
                     text = json.load(f)
                 self._process_references(text, template_overrides)
             else:
                 # Lazy parquet refs
+                logger.info("Open lazy reference dict from URL %s", fo)
                 self.references = LazyReferenceMapper(
-                    fo,
+                    fo2,
                     fs=ref_fs,
                     cache_size=cache_size,
                 )
         else:
             # dictionaries
             self._process_references(fo, template_overrides)
         if isinstance(fs, dict):
@@ -784,19 +772,19 @@
                 # find references or label not-found. Early exit if any not
                 # found and on_error is "raise"
                 try:
                     u, s, e = self._cat_common(p)
                     urls.append(u)
                     starts.append(s)
                     ends.append(e)
-                except FileNotFoundError as e:
+                except FileNotFoundError as err:
                     if on_error == "raise":
                         raise
                     if on_error != "omit":
-                        out[p] = e
+                        out[p] = err
 
             # process references into form for merging
             urls2 = []
             starts2 = []
             ends2 = []
             paths2 = []
             whole_files = set()
@@ -905,30 +893,28 @@
                         u = _render_jinja(u)
                 self.references[k] = [u] if len(v) == 1 else [u, v[1], v[2]]
             else:
                 self.references[k] = v
         self.references.update(self._process_gen(references.get("gen", [])))
 
     def _process_templates(self, tmp):
-
         self.templates = {}
         if self.template_overrides is not None:
             tmp.update(self.template_overrides)
         for k, v in tmp.items():
             if "{{" in v:
                 import jinja2
 
                 self.templates[k] = lambda temp=v, **kwargs: jinja2.Template(
                     temp
                 ).render(**kwargs)
             else:
                 self.templates[k] = v
 
     def _process_gen(self, gens):
-
         out = {}
         for gen in gens:
             dimension = {
                 k: v
                 if isinstance(v, list)
                 else range(v.get("start", 0), v["stop"], v.get("step", 1))
                 for k, v in gen["dimensions"].items()
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/sftp.py` & `fsspec-2023.6.0/fsspec/implementations/sftp.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/smb.py` & `fsspec-2023.6.0/fsspec/implementations/smb.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/tar.py` & `fsspec-2023.6.0/fsspec/implementations/tar.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if compression is not None:
             # TODO: tarfile already implements compression with modes like "'r:gz'",
             #  but then would seek to offset in the file work?
             fo = compr[compression](fo)
 
         self._fo_ref = fo
         self.fo = fo  # the whole instance is a context
-        self.tar: tarfile.TarFile = tarfile.TarFile(fileobj=self.fo)
+        self.tar = tarfile.TarFile(fileobj=self.fo)
         self.dir_cache = None
 
         self.index_store = index_store
         self.index = None
         self._index()
 
     def _index(self):
```

### Comparing `fsspec-2023.5.0/fsspec/implementations/webhdfs.py` & `fsspec-2023.6.0/fsspec/implementations/webhdfs.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/implementations/zip.py` & `fsspec-2023.6.0/fsspec/implementations/zip.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/mapping.py` & `fsspec-2023.6.0/fsspec/mapping.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/parquet.py` & `fsspec-2023.6.0/fsspec/parquet.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/registry.py` & `fsspec-2023.6.0/fsspec/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from __future__ import annotations
+
 import importlib
 import types
 import warnings
 
 __all__ = ["registry", "get_filesystem_class", "default"]
 
 # internal, mutable
-_registry = {}
+_registry: dict[str, type] = {}
 
 # external, immutable
 registry = types.MappingProxyType(_registry)
 default = "file"
 
 
 def register_implementation(name, cls, clobber=False, errtxt=None):
@@ -190,14 +192,18 @@
     "root": {
         "class": "fsspec_xrootd.XRootDFileSystem",
         "err": "Install fsspec-xrootd to access xrootd storage system."
         + " Note: 'root' is the protocol name for xrootd storage systems,"
         + " not referring to root directories",
     },
     "dir": {"class": "fsspec.implementations.dirfs.DirFileSystem"},
+    "box": {
+        "class": "boxfs.BoxFileSystem",
+        "err": "Please install boxfs to access BoxFileSystem",
+    },
 }
 
 
 def get_filesystem_class(protocol):
     """Fetch named protocol implementation from the registry
 
     The dict ``known_implementations`` maps protocol names to the locations
```

### Comparing `fsspec-2023.5.0/fsspec/spec.py` & `fsspec-2023.6.0/fsspec/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
+from __future__ import annotations
+
 import io
 import logging
 import os
 import threading
 import warnings
 import weakref
 from errno import ESPIPE
 from glob import has_magic
 from hashlib import sha256
+from typing import ClassVar
 
 from .callbacks import _DEFAULT_CALLBACK
 from .config import apply_config, conf
 from .dircache import DirCache
 from .transaction import Transaction
 from .utils import (
     _unstrip_protocol,
@@ -97,15 +100,15 @@
     from here.
     """
 
     cachable = True  # this class can be cached, instances reused
     _cached = False
     blocksize = 2**22
     sep = "/"
-    protocol = "abstract"
+    protocol: ClassVar[str | tuple[str, ...]] = "abstract"
     _latest = None
     async_impl = False
     mirror_sync_methods = False
     root_marker = ""  # For some FSs, may require leading '/' or other character
 
     #: Extra *class attributes* that should be considered when hashing.
     _extra_tokenize_attributes = ()
@@ -371,14 +374,22 @@
 
     def walk(self, path, maxdepth=None, topdown=True, **kwargs):
         """Return all files belows path
 
         List all files, recursing into subdirectories; output is iterator-style,
         like ``os.walk()``. For a simple list of files, ``find()`` is available.
 
+        When topdown is True, the caller can modify the dirnames list in-place (perhaps
+        using del or slice assignment), and walk() will
+        only recurse into the subdirectories whose names remain in dirnames;
+        this can be used to prune the search, impose a specific order of visiting,
+        or even to inform walk() about directories the caller creates or renames before
+        it resumes walk() again.
+        Modifying dirnames when topdown is False has no effect. (see os.walk)
+
         Note that the "files" outputted will include anything that is not
         a directory, such as links.
 
         Parameters
         ----------
         path: str
             Root to recurse into
@@ -397,27 +408,27 @@
         full_dirs = {}
         dirs = {}
         files = {}
 
         detail = kwargs.pop("detail", False)
         try:
             listing = self.ls(path, detail=True, **kwargs)
-        except (FileNotFoundError, IOError):
+        except (FileNotFoundError, OSError):
             if detail:
                 return path, {}, {}
             return path, [], []
 
         for info in listing:
             # each info name must be at least [path]/part , but here
             # we check also for names like [path]/part/
             pathname = info["name"].rstrip("/")
             name = pathname.rsplit("/", 1)[-1]
             if info["type"] == "directory" and pathname != path:
                 # do not include "self" path
-                full_dirs[pathname] = info
+                full_dirs[name] = pathname
                 dirs[name] = info
             elif pathname == path:
                 # file-like with same name as give path
                 files[""] = info
             else:
                 files[name] = info
 
@@ -432,17 +443,21 @@
         if maxdepth is not None:
             maxdepth -= 1
             if maxdepth < 1:
                 if not topdown:
                     yield path, dirs, files
                 return
 
-        for d in full_dirs:
+        for d in dirs:
             yield from self.walk(
-                d, maxdepth=maxdepth, detail=detail, topdown=topdown, **kwargs
+                full_dirs[d],
+                maxdepth=maxdepth,
+                detail=detail,
+                topdown=topdown,
+                **kwargs,
             )
 
         if not topdown:
             # Yield after recursion if walking bottom up
             yield path, dirs, files
 
     def find(self, path, maxdepth=None, withdirs=False, detail=False, **kwargs):
@@ -668,15 +683,15 @@
         """Size in bytes of each file in a list of paths"""
         return [self.size(p) for p in paths]
 
     def isdir(self, path):
         """Is this entry directory-like?"""
         try:
             return self.info(path)["type"] == "directory"
-        except IOError:
+        except OSError:
             return False
 
     def isfile(self, path):
         """Is this entry file-like?"""
         try:
             return self.info(path)["type"] == "file"
         except:  # noqa: E722
@@ -842,20 +857,24 @@
         else:
             return self.cat_file(paths[0], **kwargs)
 
     def get_file(
         self, rpath, lpath, callback=_DEFAULT_CALLBACK, outfile=None, **kwargs
     ):
         """Copy single remote file to local"""
+        from .implementations.local import LocalFileSystem
+
         if isfilelike(lpath):
             outfile = lpath
         elif self.isdir(rpath):
             os.makedirs(lpath, exist_ok=True)
             return None
 
+        LocalFileSystem(auto_mkdir=True).makedirs(self._parent(lpath), exist_ok=True)
+
         with self.open(rpath, "rb", **kwargs) as f1:
             if outfile is None:
                 outfile = open(lpath, "wb")
 
             try:
                 callback.set_size(getattr(f1, "size", None))
                 data = True
@@ -865,15 +884,23 @@
                     if segment_len is None:
                         segment_len = len(data)
                     callback.relative_update(segment_len)
             finally:
                 if not isfilelike(lpath):
                     outfile.close()
 
-    def get(self, rpath, lpath, recursive=False, callback=_DEFAULT_CALLBACK, **kwargs):
+    def get(
+        self,
+        rpath,
+        lpath,
+        recursive=False,
+        callback=_DEFAULT_CALLBACK,
+        maxdepth=None,
+        **kwargs,
+    ):
         """Copy file(s) to local.
 
         Copies a specific file or tree of files (if recursive=True). If lpath
         ends with a "/", it will be assumed to be a directory, and target files
         will go within. Can submit a list of paths, which may be glob-patterns
         and will be expanded.
 
@@ -883,16 +910,16 @@
             LocalFileSystem,
             make_path_posix,
             trailing_sep,
             trailing_sep_maybe_asterisk,
         )
 
         source_is_str = isinstance(rpath, str)
-        rpaths = self.expand_path(rpath, recursive=recursive)
-        if source_is_str and not recursive:
+        rpaths = self.expand_path(rpath, recursive=recursive, maxdepth=maxdepth)
+        if source_is_str and (not recursive or maxdepth is not None):
             # Non-recursive glob does not copy directories
             rpaths = [p for p in rpaths if not (trailing_sep(p) or self.isdir(p))]
             if not rpaths:
                 return
 
         if isinstance(lpath, str):
             lpath = make_path_posix(lpath)
@@ -928,15 +955,23 @@
                 while f1.tell() < size:
                     data = f1.read(self.blocksize)
                     segment_len = f2.write(data)
                     if segment_len is None:
                         segment_len = len(data)
                     callback.relative_update(segment_len)
 
-    def put(self, lpath, rpath, recursive=False, callback=_DEFAULT_CALLBACK, **kwargs):
+    def put(
+        self,
+        lpath,
+        rpath,
+        recursive=False,
+        callback=_DEFAULT_CALLBACK,
+        maxdepth=None,
+        **kwargs,
+    ):
         """Copy file(s) from local.
 
         Copies a specific file or tree of files (if recursive=True). If rpath
         ends with a "/", it will be assumed to be a directory, and target files
         will go within.
 
         Calls put_file for each source.
@@ -944,31 +979,31 @@
         from .implementations.local import (
             LocalFileSystem,
             make_path_posix,
             trailing_sep,
             trailing_sep_maybe_asterisk,
         )
 
-        if isinstance(lpath, str):
+        source_is_str = isinstance(lpath, str)
+        if source_is_str:
             lpath = make_path_posix(lpath)
         fs = LocalFileSystem()
-        source_is_str = isinstance(lpath, str)
-        lpaths = fs.expand_path(lpath, recursive=recursive)
-        if source_is_str and not recursive:
+        lpaths = fs.expand_path(lpath, recursive=recursive, maxdepth=maxdepth)
+        if source_is_str and (not recursive or maxdepth is not None):
             # Non-recursive glob does not copy directories
-            lpaths = [p for p in lpaths if not (trailing_sep(p) or self.isdir(p))]
+            lpaths = [p for p in lpaths if not (trailing_sep(p) or fs.isdir(p))]
             if not lpaths:
                 return
 
+        isdir = isinstance(rpath, str) and (trailing_sep(rpath) or self.isdir(rpath))
         rpath = (
             self._strip_protocol(rpath)
             if isinstance(rpath, str)
             else [self._strip_protocol(p) for p in rpath]
         )
-        isdir = isinstance(rpath, str) and (trailing_sep(rpath) or self.isdir(rpath))
         rpaths = other_paths(
             lpaths,
             rpath,
             exists=isdir and source_is_str and not trailing_sep_maybe_asterisk(lpath),
             is_dir=isdir,
             flatten=not source_is_str,
         )
@@ -988,15 +1023,17 @@
         with self.open(path, "rb") as f:
             f.seek(max(-size, -f.size), 2)
             return f.read()
 
     def cp_file(self, path1, path2, **kwargs):
         raise NotImplementedError
 
-    def copy(self, path1, path2, recursive=False, on_error=None, **kwargs):
+    def copy(
+        self, path1, path2, recursive=False, maxdepth=None, on_error=None, **kwargs
+    ):
         """Copy within two locations in the filesystem
 
         on_error : "raise", "ignore"
             If raise, any not-found exceptions will be raised; if ignore any
             not-found exceptions will cause the path to be skipped; defaults to
             raise unless recursive is true, where the default is ignore
         """
@@ -1004,16 +1041,16 @@
 
         if on_error is None and recursive:
             on_error = "ignore"
         elif on_error is None:
             on_error = "raise"
 
         source_is_str = isinstance(path1, str)
-        paths = self.expand_path(path1, recursive=recursive)
-        if source_is_str and not recursive:
+        paths = self.expand_path(path1, recursive=recursive, maxdepth=maxdepth)
+        if source_is_str and (not recursive or maxdepth is not None):
             # Non-recursive glob does not copy directories
             paths = [p for p in paths if not (trailing_sep(p) or self.isdir(p))]
             if not paths:
                 return
 
         isdir = isinstance(path2, str) and (trailing_sep(path2) or self.isdir(path2))
         path2 = other_paths(
@@ -1047,19 +1084,24 @@
             out = set()
             path = [self._strip_protocol(p) for p in path]
             for p in path:
                 if has_magic(p):
                     bit = set(self.glob(p, **kwargs))
                     out |= bit
                     if recursive:
+                        # glob call above expanded one depth so if maxdepth is defined
+                        # then decrement it in expand_path call below. If it is zero
+                        # after decrementing then avoid expand_path call.
+                        if maxdepth is not None and maxdepth <= 1:
+                            continue
                         out |= set(
                             self.expand_path(
                                 list(bit),
                                 recursive=recursive,
-                                maxdepth=maxdepth,
+                                maxdepth=maxdepth - 1 if maxdepth is not None else None,
                                 **kwargs,
                             )
                         )
                     continue
                 elif recursive:
                     rec = set(
                         self.find(
```

### Comparing `fsspec-2023.5.0/fsspec/tests/abstract/copy.py` & `fsspec-2023.6.0/fsspec/tests/abstract/copy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 class AbstractCopyTests:
     def test_copy_file_to_existing_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 1a
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
         if not self.supports_empty_directories():
+            # Force target directory to exist by adding a dummy file
             fs.touch(fs_join(target, "dummy"))
         assert fs.isdir(target)
 
         target_file2 = fs_join(target, "file2")
         target_subfile1 = fs_join(target, "subfile1")
 
         # Copy from source directory
@@ -31,110 +32,126 @@
         fs.cp(fs_join(source, "file2"), target + "/")
         assert fs.isdir(target)
         assert fs.isfile(target_file2)
 
         fs.cp(fs_join(source, "subdir", "subfile1"), target + "/")
         assert fs.isfile(target_subfile1)
 
-    def test_copy_file_to_new_directory(self, fs, fs_join, fs_path, fs_scenario_cp):
+    def test_copy_file_to_new_directory(
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
+    ):
         # Copy scenario 1b
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         fs.cp(
             fs_join(source, "subdir", "subfile1"), fs_join(target, "newdir/")
         )  # Note trailing slash
         assert fs.isdir(target)
         assert fs.isdir(fs_join(target, "newdir"))
         assert fs.isfile(fs_join(target, "newdir", "subfile1"))
 
     def test_copy_file_to_file_in_existing_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 1c
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         fs.cp(fs_join(source, "subdir", "subfile1"), fs_join(target, "newfile"))
         assert fs.isfile(fs_join(target, "newfile"))
 
     def test_copy_file_to_file_in_new_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 1d
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         fs.cp(
             fs_join(source, "subdir", "subfile1"), fs_join(target, "newdir", "newfile")
         )
         assert fs.isdir(fs_join(target, "newdir"))
         assert fs.isfile(fs_join(target, "newdir", "newfile"))
 
     def test_copy_directory_to_existing_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 1e
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
+        if not self.supports_empty_directories():
+            # Force target directory to exist by adding a dummy file
+            dummy = fs_join(target, "dummy")
+            fs.touch(dummy)
+        assert fs.isdir(target)
 
         for source_slash, target_slash in zip([False, True], [False, True]):
             s = fs_join(source, "subdir")
             if source_slash:
                 s += "/"
             t = target + "/" if target_slash else target
 
             # Without recursive does nothing
             fs.cp(s, t)
-            assert fs.ls(target) == []
+            assert fs.ls(target) == [] if self.supports_empty_directories() else [dummy]
 
             # With recursive
             fs.cp(s, t, recursive=True)
             if source_slash:
                 assert fs.isfile(fs_join(target, "subfile1"))
                 assert fs.isfile(fs_join(target, "subfile2"))
                 assert fs.isdir(fs_join(target, "nesteddir"))
                 assert fs.isfile(fs_join(target, "nesteddir", "nestedfile"))
+                assert not fs.exists(fs_join(target, "subdir"))
 
-                fs.rm(
-                    [
-                        fs_join(target, "subfile1"),
-                        fs_join(target, "subfile2"),
-                        fs_join(target, "nesteddir"),
-                    ],
-                    recursive=True,
-                )
+                fs.rm(fs.ls(target, detail=False), recursive=True)
             else:
                 assert fs.isdir(fs_join(target, "subdir"))
                 assert fs.isfile(fs_join(target, "subdir", "subfile1"))
                 assert fs.isfile(fs_join(target, "subdir", "subfile2"))
                 assert fs.isdir(fs_join(target, "subdir", "nesteddir"))
                 assert fs.isfile(fs_join(target, "subdir", "nesteddir", "nestedfile"))
 
                 fs.rm(fs_join(target, "subdir"), recursive=True)
-            assert fs.ls(target) == []
+            assert fs.ls(target) == [] if self.supports_empty_directories() else [dummy]
 
-            # Limit by maxdepth
-            # ERROR: maxdepth ignored here
+            # Limit recursive by maxdepth
+            fs.cp(s, t, recursive=True, maxdepth=1)
+            if source_slash:
+                assert fs.isfile(fs_join(target, "subfile1"))
+                assert fs.isfile(fs_join(target, "subfile2"))
+                assert not fs.exists(fs_join(target, "nesteddir"))
+                assert not fs.exists(fs_join(target, "subdir"))
+
+                fs.rm(fs.ls(target, detail=False), recursive=True)
+            else:
+                assert fs.isdir(fs_join(target, "subdir"))
+                assert fs.isfile(fs_join(target, "subdir", "subfile1"))
+                assert fs.isfile(fs_join(target, "subdir", "subfile2"))
+                assert not fs.exists(fs_join(target, "subdir", "nesteddir"))
+
+                fs.rm(fs_join(target, "subdir"), recursive=True)
+            assert fs.ls(target) == [] if self.supports_empty_directories() else [dummy]
 
     def test_copy_directory_to_new_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 1f
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         for source_slash, target_slash in zip([False, True], [False, True]):
             s = fs_join(source, "subdir")
             if source_slash:
                 s += "/"
             t = fs_join(target, "newdir")
@@ -148,28 +165,37 @@
             # With recursive
             fs.cp(s, t, recursive=True)
             assert fs.isdir(fs_join(target, "newdir"))
             assert fs.isfile(fs_join(target, "newdir", "subfile1"))
             assert fs.isfile(fs_join(target, "newdir", "subfile2"))
             assert fs.isdir(fs_join(target, "newdir", "nesteddir"))
             assert fs.isfile(fs_join(target, "newdir", "nesteddir", "nestedfile"))
+            assert not fs.exists(fs_join(target, "subdir"))
 
             fs.rm(fs_join(target, "newdir"), recursive=True)
-            assert fs.ls(target) == []
+            assert not fs.exists(fs_join(target, "newdir"))
 
-            # Limit by maxdepth
-            # ERROR: maxdepth ignored here
+            # Limit recursive by maxdepth
+            fs.cp(s, t, recursive=True, maxdepth=1)
+            assert fs.isdir(fs_join(target, "newdir"))
+            assert fs.isfile(fs_join(target, "newdir", "subfile1"))
+            assert fs.isfile(fs_join(target, "newdir", "subfile2"))
+            assert not fs.exists(fs_join(target, "newdir", "nesteddir"))
+            assert not fs.exists(fs_join(target, "subdir"))
+
+            fs.rm(fs_join(target, "newdir"), recursive=True)
+            assert not fs.exists(fs_join(target, "newdir"))
 
     def test_copy_glob_to_existing_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 1g
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         for target_slash in [False, True]:
             t = target + "/" if target_slash else target
 
             # Without recursive
             fs.cp(fs_join(source, "subdir", "*"), t)
@@ -189,22 +215,31 @@
             assert fs.isdir(fs_join(target, "nesteddir"))
             assert fs.isfile(fs_join(target, "nesteddir", "nestedfile"))
             assert not fs.exists(fs_join(target, "subdir"))
 
             fs.rm(fs.ls(target, detail=False), recursive=True)
             assert fs.ls(target) == []
 
-            # Limit by maxdepth
-            # ERROR: maxdepth ignored here
+            # Limit recursive by maxdepth
+            fs.cp(fs_join(source, "subdir", "*"), t, recursive=True, maxdepth=1)
+            assert fs.isfile(fs_join(target, "subfile1"))
+            assert fs.isfile(fs_join(target, "subfile2"))
+            assert not fs.exists(fs_join(target, "nesteddir"))
+            assert not fs.exists(fs_join(target, "subdir"))
 
-    def test_copy_glob_to_new_directory(self, fs, fs_join, fs_path, fs_scenario_cp):
+            fs.rm(fs.ls(target, detail=False), recursive=True)
+            assert fs.ls(target) == []
+
+    def test_copy_glob_to_new_directory(
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
+    ):
         # Copy scenario 1h
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         for target_slash in [False, True]:
             t = fs_join(target, "newdir")
             if target_slash:
                 t += "/"
 
@@ -215,40 +250,54 @@
             assert fs.isfile(fs_join(target, "newdir", "subfile2"))
             assert not fs.exists(fs_join(target, "newdir", "nesteddir"))
             assert not fs.exists(fs_join(target, "newdir", "nesteddir", "nestedfile"))
             assert not fs.exists(fs_join(target, "subdir"))
             assert not fs.exists(fs_join(target, "newdir", "subdir"))
 
             fs.rm(fs_join(target, "newdir"), recursive=True)
-            assert fs.ls(target) == []
+            assert not fs.exists(fs_join(target, "newdir"))
 
             # With recursive
             fs.cp(fs_join(source, "subdir", "*"), t, recursive=True)
             assert fs.isdir(fs_join(target, "newdir"))
             assert fs.isfile(fs_join(target, "newdir", "subfile1"))
             assert fs.isfile(fs_join(target, "newdir", "subfile2"))
             assert fs.isdir(fs_join(target, "newdir", "nesteddir"))
             assert fs.isfile(fs_join(target, "newdir", "nesteddir", "nestedfile"))
             assert not fs.exists(fs_join(target, "subdir"))
             assert not fs.exists(fs_join(target, "newdir", "subdir"))
 
             fs.rm(fs_join(target, "newdir"), recursive=True)
-            assert fs.ls(target) == []
+            assert not fs.exists(fs_join(target, "newdir"))
+
+            # Limit recursive by maxdepth
+            fs.cp(fs_join(source, "subdir", "*"), t, recursive=True, maxdepth=1)
+            assert fs.isdir(fs_join(target, "newdir"))
+            assert fs.isfile(fs_join(target, "newdir", "subfile1"))
+            assert fs.isfile(fs_join(target, "newdir", "subfile2"))
+            assert not fs.exists(fs_join(target, "newdir", "nesteddir"))
+            assert not fs.exists(fs_join(target, "subdir"))
+            assert not fs.exists(fs_join(target, "newdir", "subdir"))
 
-            # Limit by maxdepth
-            # ERROR: this is not correct
+            fs.rm(fs.ls(target, detail=False), recursive=True)
+            assert not fs.exists(fs_join(target, "newdir"))
 
     def test_copy_list_of_files_to_existing_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 2a
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
+        if not self.supports_empty_directories():
+            # Force target directory to exist by adding a dummy file
+            dummy = fs_join(target, "dummy")
+            fs.touch(dummy)
+        assert fs.isdir(target)
 
         source_files = [
             fs_join(source, "file1"),
             fs_join(source, "file2"),
             fs_join(source, "subdir", "subfile1"),
         ]
 
@@ -257,42 +306,44 @@
 
             fs.cp(source_files, t)
             assert fs.isfile(fs_join(target, "file1"))
             assert fs.isfile(fs_join(target, "file2"))
             assert fs.isfile(fs_join(target, "subfile1"))
 
             fs.rm(fs.find(target))
-            assert fs.ls(target) == []
+            assert fs.ls(target) == [] if self.supports_empty_directories() else [dummy]
 
     def test_copy_list_of_files_to_new_directory(
-        self, fs, fs_join, fs_path, fs_scenario_cp
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
     ):
         # Copy scenario 2b
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         fs.mkdir(target)
 
         source_files = [
             fs_join(source, "file1"),
             fs_join(source, "file2"),
             fs_join(source, "subdir", "subfile1"),
         ]
 
         fs.cp(source_files, fs_join(target, "newdir") + "/")  # Note trailing slash
         assert fs.isdir(fs_join(target, "newdir"))
         assert fs.isfile(fs_join(target, "newdir", "file1"))
         assert fs.isfile(fs_join(target, "newdir", "file2"))
         assert fs.isfile(fs_join(target, "newdir", "subfile1"))
 
-    def test_copy_two_files_new_directory(self, fs, fs_join, fs_path, fs_scenario_cp):
+    def test_copy_two_files_new_directory(
+        self, fs, fs_join, fs_bulk_operations_scenario_0, fs_target
+    ):
         # This is a duplicate of test_copy_list_of_files_to_new_directory and
         # can eventually be removed.
-        source = fs_scenario_cp
+        source = fs_bulk_operations_scenario_0
 
-        target = fs_join(fs_path, "target")
+        target = fs_target
         assert not fs.exists(target)
         fs.cp([fs_join(source, "file1"), fs_join(source, "file2")], target)
 
         assert fs.isdir(target)
         assert fs.isfile(fs_join(target, "file1"))
         assert fs.isfile(fs_join(target, "file2"))
```

### Comparing `fsspec-2023.5.0/fsspec/transaction.py` & `fsspec-2023.6.0/fsspec/transaction.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec/utils.py` & `fsspec-2023.6.0/fsspec/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import math
 import os
 import pathlib
 import re
 import sys
 from contextlib import contextmanager
@@ -106,15 +108,15 @@
                     "Collision between inferred and specified storage "
                     "option:\n%s" % collision
                 )
     options.update(inherited)
 
 
 # Compression extensions registered via fsspec.compression.register_compression
-compressions = {}
+compressions: dict[str, str] = {}
 
 
 def infer_compression(filename):
     """Infer compression, if available, from filename.
 
     Infer a named compression type, if registered and available, from filename
     extension. This includes builtin (gz, bz2, zip) compressions, as well as
```

### Comparing `fsspec-2023.5.0/fsspec.egg-info/PKG-INFO` & `fsspec-2023.6.0/fsspec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fsspec
-Version: 2023.5.0
+Version: 2023.6.0
 Summary: File-system specification
 Home-page: http://github.com/fsspec/filesystem_spec
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
 Project-URL: Changelog, https://filesystem-spec.readthedocs.io/en/latest/changelog.html
 Project-URL: Documentation, https://filesystem-spec.readthedocs.io/en/latest/
```

### Comparing `fsspec-2023.5.0/fsspec.egg-info/SOURCES.txt` & `fsspec-2023.6.0/fsspec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/fsspec.egg-info/requires.txt` & `fsspec-2023.6.0/fsspec.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/setup.cfg` & `fsspec-2023.6.0/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -36,11 +36,31 @@
 00000230: 6170 203d 2030 0a63 6f6d 6269 6e65 5f61  ap = 0.combine_a
 00000240: 735f 696d 706f 7274 7320 3d20 5472 7565  s_imports = True
 00000250: 0a6c 696e 655f 6c65 6e67 7468 203d 2038  .line_length = 8
 00000260: 380a 736b 6970 203d 200a 092e 746f 780a  8.skip = ...tox.
 00000270: 0962 7569 6c64 0a09 646f 6373 2f73 6f75  .build..docs/sou
 00000280: 7263 652f 636f 6e66 2e70 790a 0976 6572  rce/conf.py..ver
 00000290: 7369 6f6e 6565 722e 7079 0a09 6673 7370  sioneer.py..fssp
-000002a0: 6563 2f5f 7665 7273 696f 6e0a 0a5b 6567  ec/_version..[eg
-000002b0: 675f 696e 666f 5d0a 7461 675f 6275 696c  g_info].tag_buil
-000002c0: 6420 3d20 0a74 6167 5f64 6174 6520 3d20  d = .tag_date = 
-000002d0: 300a 0a                                  0..
+000002a0: 6563 2f5f 7665 7273 696f 6e0a 0a5b 6d79  ec/_version..[my
+000002b0: 7079 5d0a 666f 6c6c 6f77 5f69 6d70 6f72  py].follow_impor
+000002c0: 7473 203d 206e 6f72 6d61 6c0a 6967 6e6f  ts = normal.igno
+000002d0: 7265 5f6d 6973 7369 6e67 5f69 6d70 6f72  re_missing_impor
+000002e0: 7473 203d 2054 7275 650a 656e 6162 6c65  ts = True.enable
+000002f0: 5f65 7272 6f72 5f63 6f64 6520 3d20 6967  _error_code = ig
+00000300: 6e6f 7265 2d77 6974 686f 7574 2d63 6f64  nore-without-cod
+00000310: 652c 7472 7574 6879 2d62 6f6f 6c2c 7472  e,truthy-bool,tr
+00000320: 7574 6879 2d69 7465 7261 626c 652c 756e  uthy-iterable,un
+00000330: 7573 6564 2d61 7761 6974 6162 6c65 0a64  used-awaitable.d
+00000340: 6973 616c 6c6f 775f 756e 7479 7065 645f  isallow_untyped_
+00000350: 6465 636f 7261 746f 7273 203d 2054 7275  decorators = Tru
+00000360: 650a 7374 7269 6374 5f65 7175 616c 6974  e.strict_equalit
+00000370: 7920 3d20 5472 7565 0a77 6172 6e5f 7265  y = True.warn_re
+00000380: 6475 6e64 616e 745f 6361 7374 7320 3d20  dundant_casts = 
+00000390: 5472 7565 0a77 6172 6e5f 756e 7573 6564  True.warn_unused
+000003a0: 5f63 6f6e 6669 6773 203d 2054 7275 650a  _configs = True.
+000003b0: 7761 726e 5f75 6e75 7365 645f 6967 6e6f  warn_unused_igno
+000003c0: 7265 7320 3d20 5472 7565 0a65 7863 6c75  res = True.exclu
+000003d0: 6465 203d 2028 7465 7374 5f2e 2a7c 636f  de = (test_.*|co
+000003e0: 6e66 7465 7374 295c 2e70 7924 0a0a 5b65  nftest)\.py$..[e
+000003f0: 6767 5f69 6e66 6f5d 0a74 6167 5f62 7569  gg_info].tag_bui
+00000400: 6c64 203d 200a 7461 675f 6461 7465 203d  ld = .tag_date =
+00000410: 2030 0a0a                                 0..
```

### Comparing `fsspec-2023.5.0/setup.py` & `fsspec-2023.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `fsspec-2023.5.0/versioneer.py` & `fsspec-2023.6.0/versioneer.py`

 * *Files identical despite different names*

