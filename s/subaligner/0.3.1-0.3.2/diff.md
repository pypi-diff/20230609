# Comparing `tmp/subaligner-0.3.1.tar.gz` & `tmp/subaligner-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/subaligner-0.3.1.tar", last modified: Sat Apr 15 17:24:02 2023, max compression
+gzip compressed data, was "dist/subaligner-0.3.2.tar", last modified: Fri Jun  9 08:44:02 2023, max compression
```

## Comparing `subaligner-0.3.1.tar` & `subaligner-0.3.2.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.488037 subaligner-0.3.1/
--rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.1/LICENSE
--rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.1/MANIFEST.in
--rw-r--r--   0 macbook    (501) staff       (20)    10178 2023-04-15 17:24:02.487525 subaligner-0.3.1/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     9403 2023-04-15 17:08:17.000000 subaligner-0.3.1/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.360554 subaligner-0.3.1/bin/
--rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.1/bin/subaligner
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.1/bin/subaligner_1pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.1/bin/subaligner_2pass
--rwxr-xr-x   0 macbook    (501) staff       (20)    16659 2023-04-15 17:17:05.000000 subaligner-0.3.1/bin/subaligner_batch
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.1/bin/subaligner_convert
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.1/bin/subaligner_train
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.1/bin/subaligner_tune
--rw-r--r--   0 macbook    (501) staff       (20)     1181 2023-03-29 00:31:58.000000 subaligner-0.3.1/requirements.txt
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-04-15 17:24:02.488249 subaligner-0.3.1/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     3728 2023-03-10 19:10:53.000000 subaligner-0.3.1/setup.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.446659 subaligner-0.3.1/subaligner/
--rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.1/subaligner/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.1/subaligner/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)       64 2023-03-12 11:44:17.000000 subaligner-0.3.1/subaligner/_version.py
--rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/embedder.py
--rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.1/subaligner/exception.py
--rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/hparam_tuner.py
--rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/hyperparameters.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.460981 subaligner-0.3.1/subaligner/lib/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/lib/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/lib/language.py
--rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/lib/to_srt.py
--rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.1/subaligner/llm.py
--rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/logger.py
--rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.1/subaligner/media_helper.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.351528 subaligner-0.3.1/subaligner/models/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.352181 subaligner-0.3.1/subaligner/models/training/
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.462404 subaligner-0.3.1/subaligner/models/training/config/
--rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/config/hyperparameters.json
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.464136 subaligner-0.3.1/subaligner/models/training/model/
--rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/model/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/model/model.hdf5
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.472381 subaligner-0.3.1/subaligner/models/training/weights/
--rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/weights/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/models/training/weights/weights.hdf5
--rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/network.py
--rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/predictor.py
--rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/singleton.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.481047 subaligner-0.3.1/subaligner/subaligner_1pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_1pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/subaligner_1pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.482266 subaligner-0.3.1/subaligner/subaligner_2pass/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_2pass/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/subaligner_2pass/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.483305 subaligner-0.3.1/subaligner/subaligner_batch/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_batch/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    16659 2023-04-15 17:17:05.000000 subaligner-0.3.1/subaligner/subaligner_batch/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.484162 subaligner-0.3.1/subaligner/subaligner_convert/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_convert/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.1/subaligner/subaligner_convert/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.485320 subaligner-0.3.1/subaligner/subaligner_train/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_train/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.1/subaligner/subaligner_train/__main__.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.486733 subaligner-0.3.1/subaligner/subaligner_tune/
--rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_tune/__init__.py
--rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.1/subaligner/subaligner_tune/__main__.py
--rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.1/subaligner/subtitle.py
--rw-r--r--   0 macbook    (501) staff       (20)    15843 2023-03-07 23:41:51.000000 subaligner-0.3.1/subaligner/trainer.py
--rw-r--r--   0 macbook    (501) staff       (20)     4695 2023-03-21 00:12:01.000000 subaligner-0.3.1/subaligner/transcriber.py
--rw-r--r--   0 macbook    (501) staff       (20)    12131 2023-03-28 22:20:16.000000 subaligner-0.3.1/subaligner/translator.py
--rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.1/subaligner/utils.py
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-04-15 17:24:02.458857 subaligner-0.3.1/subaligner.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)    10178 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)      424 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/entry_points.txt
--rw-r--r--   0 macbook    (501) staff       (20)     2084 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)       11 2023-04-15 17:24:02.000000 subaligner-0.3.1/subaligner.egg-info/top_level.txt
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.924129 subaligner-0.3.2/
+-rw-r--r--   0 macbook    (501) staff       (20)     1074 2022-05-09 09:59:50.000000 subaligner-0.3.2/LICENSE
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2022-05-09 09:59:50.000000 subaligner-0.3.2/MANIFEST.in
+-rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 08:44:02.923299 subaligner-0.3.2/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     9247 2023-04-15 17:31:09.000000 subaligner-0.3.2/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.838080 subaligner-0.3.2/bin/
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.2/bin/subaligner
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.2/bin/subaligner_1pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.2/bin/subaligner_2pass
+-rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.2/bin/subaligner_batch
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.2/bin/subaligner_convert
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.2/bin/subaligner_train
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.2/bin/subaligner_tune
+-rw-r--r--   0 macbook    (501) staff       (20)     1185 2023-06-09 08:34:37.000000 subaligner-0.3.2/requirements.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-06-09 08:44:02.924259 subaligner-0.3.2/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     3748 2023-06-08 23:47:15.000000 subaligner-0.3.2/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.857194 subaligner-0.3.2/subaligner/
+-rw-r--r--   0 macbook    (501) staff       (20)      258 2023-03-11 16:33:37.000000 subaligner-0.3.2/subaligner/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    22502 2023-03-20 01:23:21.000000 subaligner-0.3.2/subaligner/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)       64 2023-06-08 23:53:14.000000 subaligner-0.3.2/subaligner/_version.py
+-rw-r--r--   0 macbook    (501) staff       (20)    11392 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/embedder.py
+-rw-r--r--   0 macbook    (501) staff       (20)      511 2023-03-11 23:58:14.000000 subaligner-0.3.2/subaligner/exception.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4595 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/hparam_tuner.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7193 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/hyperparameters.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.898772 subaligner-0.3.2/subaligner/lib/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/lib/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)     7848 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/lib/language.py
+-rw-r--r--   0 macbook    (501) staff       (20)    21337 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/lib/to_srt.py
+-rw-r--r--   0 macbook    (501) staff       (20)      709 2023-03-19 19:33:51.000000 subaligner-0.3.2/subaligner/llm.py
+-rw-r--r--   0 macbook    (501) staff       (20)     1842 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/logger.py
+-rw-r--r--   0 macbook    (501) staff       (20)    18286 2023-03-17 01:31:21.000000 subaligner-0.3.2/subaligner/media_helper.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.825985 subaligner-0.3.2/subaligner/models/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.826714 subaligner-0.3.2/subaligner/models/training/
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.899902 subaligner-0.3.2/subaligner/models/training/config/
+-rw-r--r--   0 macbook    (501) staff       (20)      754 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/config/hyperparameters.json
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.901364 subaligner-0.3.2/subaligner/models/training/model/
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/model/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/model/model.hdf5
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.909729 subaligner-0.3.2/subaligner/models/training/weights/
+-rw-r--r--   0 macbook    (501) staff       (20)       46 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/weights/__init__.py
+-rw-r--r--   0 macbook    (501) staff       (20)   685736 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/models/training/weights/weights.hdf5
+-rw-r--r--   0 macbook    (501) staff       (20)    24034 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/network.py
+-rw-r--r--   0 macbook    (501) staff       (20)    39332 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/predictor.py
+-rw-r--r--   0 macbook    (501) staff       (20)      413 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/singleton.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.917547 subaligner-0.3.2/subaligner/subaligner_1pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_1pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     9986 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/subaligner_1pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.918511 subaligner-0.3.2/subaligner/subaligner_2pass/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_2pass/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    12681 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/subaligner_2pass/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.919743 subaligner-0.3.2/subaligner/subaligner_batch/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_batch/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    18767 2023-04-14 17:04:30.000000 subaligner-0.3.2/subaligner/subaligner_batch/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.920607 subaligner-0.3.2/subaligner/subaligner_convert/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_convert/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6567 2023-03-10 19:10:53.000000 subaligner-0.3.2/subaligner/subaligner_convert/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.921531 subaligner-0.3.2/subaligner/subaligner_train/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_train/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)    15867 2023-03-07 23:41:51.000000 subaligner-0.3.2/subaligner/subaligner_train/__main__.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.922414 subaligner-0.3.2/subaligner/subaligner_tune/
+-rw-r--r--   0 macbook    (501) staff       (20)        0 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_tune/__init__.py
+-rwxr-xr-x   0 macbook    (501) staff       (20)     6350 2022-05-09 09:59:51.000000 subaligner-0.3.2/subaligner/subaligner_tune/__main__.py
+-rw-r--r--   0 macbook    (501) staff       (20)    32984 2023-04-15 16:48:57.000000 subaligner-0.3.2/subaligner/subtitle.py
+-rw-r--r--   0 macbook    (501) staff       (20)    15876 2023-06-06 00:57:05.000000 subaligner-0.3.2/subaligner/trainer.py
+-rw-r--r--   0 macbook    (501) staff       (20)     4745 2023-06-06 00:48:48.000000 subaligner-0.3.2/subaligner/transcriber.py
+-rw-r--r--   0 macbook    (501) staff       (20)    12182 2023-06-06 09:49:57.000000 subaligner-0.3.2/subaligner/translator.py
+-rw-r--r--   0 macbook    (501) staff       (20)    33741 2023-03-17 02:05:09.000000 subaligner-0.3.2/subaligner/utils.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-06-09 08:44:02.896669 subaligner-0.3.2/subaligner.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)    10046 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1628 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)      424 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/entry_points.txt
+-rw-r--r--   0 macbook    (501) staff       (20)     2015 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       11 2023-06-09 08:44:02.000000 subaligner-0.3.2/subaligner.egg-info/top_level.txt
```

### Comparing `subaligner-0.3.1/LICENSE` & `subaligner-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/PKG-INFO` & `subaligner-0.3.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,16 @@
-Metadata-Version: 2.1
-Name: subaligner
-Version: 0.3.1
-Summary: Automatically synchronize and translate subtitles with pretrained deep neural networks, forced alignments and transformers.
-Home-page: https://subaligner.readthedocs.io/en/latest/
-Author: Xi Bai
-Author-email: xi.bai.ed@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: harmony
-Provides-Extra: dev
-Provides-Extra: docs
-Provides-Extra: stretch
-Provides-Extra: translation
-Provides-Extra: llm
-License-File: LICENSE
-
 <div align="center">
   <img src="./figures/subaligner.png" alt="subaligner" width="300" />
 </div>
 
 [![Build Status](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml/badge.svg?branch=master)](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml?query=branch%3Amaster) ![Codecov](https://img.shields.io/codecov/c/github/baxtree/subaligner)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/subaligner/badge/?version=latest)](https://subaligner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/baxtree/subaligner)](https://github.com/baxtree/subaligner/blob/master/LICENSE)
 [![PyPI](https://badge.fury.io/py/subaligner.svg)](https://badge.fury.io/py/subaligner)
-[![Docker Build](https://img.shields.io/docker/cloud/build/baxtree/subaligner?label=Docker&style=flat)](https://hub.docker.com/r/baxtree/subaligner/builds)
 [![Docker Pulls](https://img.shields.io/docker/pulls/baxtree/subaligner)](https://hub.docker.com/r/baxtree/subaligner)
 [![Citation](https://zenodo.org/badge/228440472.svg)](https://doi.org/10.5281/zenodo.5603083)
 
 ## Supported Formats
 Subtitle: SubRip, TTML, WebVTT, (Advanced) SubStation Alpha, MicroDVD, MPL2, TMP, EBU STL, SAMI, SCC and SBV.
 
 Video/Audio: MP4, WebM, Ogg, 3GP, FLV, MOV, Matroska, MPEG TS, WAV, MP3, AAC, FLAC, etc.
@@ -222,9 +198,7 @@
 [pysrt](https://github.com/byroot/pysrt)
 [pysubs2](https://github.com/tkarabela/pysubs2)
 [aeneas](https://www.readbeyond.it/aeneas/)
 [transformers](https://huggingface.co/transformers/)
 [openai-whisper](https://github.com/openai/whisper).
 
 Thanks to Alan Robinson and Nigel Megitt for their invaluable feedback.
-
-
```

### Comparing `subaligner-0.3.1/README.md` & `subaligner-0.3.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,39 @@
+Metadata-Version: 2.1
+Name: subaligner
+Version: 0.3.2
+Summary: Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.
+Home-page: https://subaligner.readthedocs.io/en/latest/
+Author: Xi Bai
+Author-email: xi.bai.ed@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Intended Audience :: Developers
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: harmony
+Provides-Extra: dev
+Provides-Extra: docs
+Provides-Extra: stretch
+Provides-Extra: translation
+Provides-Extra: llm
+License-File: LICENSE
+
 <div align="center">
   <img src="./figures/subaligner.png" alt="subaligner" width="300" />
 </div>
 
 [![Build Status](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml/badge.svg?branch=master)](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml?query=branch%3Amaster) ![Codecov](https://img.shields.io/codecov/c/github/baxtree/subaligner)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/subaligner/badge/?version=latest)](https://subaligner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/baxtree/subaligner)](https://github.com/baxtree/subaligner/blob/master/LICENSE)
 [![PyPI](https://badge.fury.io/py/subaligner.svg)](https://badge.fury.io/py/subaligner)
-[![Docker Build](https://img.shields.io/docker/cloud/build/baxtree/subaligner?label=Docker&style=flat)](https://hub.docker.com/r/baxtree/subaligner/builds)
 [![Docker Pulls](https://img.shields.io/docker/pulls/baxtree/subaligner)](https://hub.docker.com/r/baxtree/subaligner)
 [![Citation](https://zenodo.org/badge/228440472.svg)](https://doi.org/10.5281/zenodo.5603083)
 
 ## Supported Formats
 Subtitle: SubRip, TTML, WebVTT, (Advanced) SubStation Alpha, MicroDVD, MPL2, TMP, EBU STL, SAMI, SCC and SBV.
 
 Video/Audio: MP4, WebM, Ogg, 3GP, FLV, MOV, Matroska, MPEG TS, WAV, MP3, AAC, FLAC, etc.
@@ -199,7 +221,9 @@
 [pysrt](https://github.com/byroot/pysrt)
 [pysubs2](https://github.com/tkarabela/pysubs2)
 [aeneas](https://www.readbeyond.it/aeneas/)
 [transformers](https://huggingface.co/transformers/)
 [openai-whisper](https://github.com/openai/whisper).
 
 Thanks to Alan Robinson and Nigel Megitt for their invaluable feedback.
+
+
```

### Comparing `subaligner-0.3.1/bin/subaligner` & `subaligner-0.3.2/bin/subaligner`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/bin/subaligner_1pass` & `subaligner-0.3.2/bin/subaligner_1pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/bin/subaligner_2pass` & `subaligner-0.3.2/bin/subaligner_2pass`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/bin/subaligner_batch` & `subaligner-0.3.2/bin/subaligner_batch`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 #!/usr/bin/env python
 """
-usage: subaligner_batch [-h] [-m {single,dual}] [-vd VIDEO_DIRECTORY] [-sd SUBTITLE_DIRECTORY] [-l MAX_LOGLOSS] [-so]
+usage: subaligner_batch [-h] [-m {single,dual,script,transcribe}] [-sd SUBTITLE_DIRECTORY] [-vd VIDEO_DIRECTORY] [-l MAX_LOGLOSS] [-so]
                         [-sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
-                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-od OUTPUT_DIRECTORY] [-t TRANSLATE] [-lgs] [-d] [-q] [-ver]
+                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-od OUTPUT_DIRECTORY] [-of {srt,ytt,ttml,txt,smi,xml,ssa,ass,dfxp,sub,scc,tmp,sami,vtt,stl,sbv}] [-t TRANSLATE]
+                        [-ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
+                        [-mr {whisper}] [-mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}] [-lgs] [-d] [-q] [-ver]
 
 Batch align multiple subtitle files and audiovisual files
 
 Subtitle files and their companion audiovisual files need to be stored in two separate directories.
 Each file pair needs to share the same base filename, the part before the extension.
 
 optional arguments:
   -h, --help            show this help message and exit
-  -vd VIDEO_DIRECTORY, --video_directory VIDEO_DIRECTORY
-                        Path to the video directory
   -sd SUBTITLE_DIRECTORY, --subtitle_directory SUBTITLE_DIRECTORY
                         Path to the subtitle directory
+  -vd VIDEO_DIRECTORY, --video_directory VIDEO_DIRECTORY
+                        Path to the video directory
   -l MAX_LOGLOSS, --max_logloss MAX_LOGLOSS
                         Max global log loss for alignment
-  -so, --stretch_on    Switch on stretch on subtitles
+  -so, --stretch_on     Switch on stretch on subtitles)
   -sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --stretch_in_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].
                         NB: This will be ignored if neither -so nor --stretch_on is present
   -fos, --exit_segfail  Exit on any segment alignment failures
   -tod TRAINING_OUTPUT_DIRECTORY, --training_output_directory TRAINING_OUTPUT_DIRECTORY
                         Path to the output directory containing training results
   -od OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
                         Path to the output subtitle directory
+  -of {srt,ytt,ttml,txt,smi,xml,ssa,ass,dfxp,sub,scc,tmp,sami,vtt,stl,sbv}, --output_format {srt,ytt,ttml,txt,smi,xml,ssa,ass,dfxp,sub,scc,tmp,sami,vtt,stl,sbv}
+                        File format of the output subtitles
   -t TRANSLATE, --translate TRANSLATE
                         Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)
+  -ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --main_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
+                        Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]
+  -mr {whisper}, --transcription_recipe {whisper}
+                        LLM recipe used for transcribing video files
+  -mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}, --transcription_flavour {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}
+                        Flavour variation for a specific LLM recipe supporting transcription
   -lgs, --languages     Print out language codes used for stretch and translation
   -d, --debug           Print out debugging information
   -q, --quiet           Switch off logging information
   -ver, --version       show program's version number and exit
 
 required arguments:
-  -m {single,dual}, --mode {single,dual}
+  -m {single,dual,script,transcribe}, --mode {single,dual,script,transcribe}
                         Alignment mode: either single or dual
 """
 
 import argparse
 import sys
 import traceback
 import os
```

### Comparing `subaligner-0.3.1/bin/subaligner_convert` & `subaligner-0.3.2/bin/subaligner_convert`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/bin/subaligner_train` & `subaligner-0.3.2/bin/subaligner_train`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/bin/subaligner_tune` & `subaligner-0.3.2/bin/subaligner_tune`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/requirements.txt` & `subaligner-0.3.2/requirements.txt`

 * *Files 9% similar despite different names*

```diff
@@ -39,33 +39,33 @@
 oauthlib==3.1.0
 pbr==4.0.2
 pluggy==0.13.1
 psutil==5.6.7
 py==1.10.0
 pyasn1==0.4.8
 pyasn1-modules==0.2.7
+pycountry~=20.7.3
 pydot==1.2.4
 pydot-ng==1.0.0
 pydotplus==2.0.2
 pyprof2calltree==1.4.3
 pysrt==1.1.1
 pysubs2<=1.4.2
 pystack-debugger==0.8.0
 pytz==2018.4
 PyYAML>=4.2b1
-requests~=2.25.1
+requests<3.0.0
 requests-oauthlib==1.3.0
 rsa==4.7
 scipy<=1.8.1
 scikit-learn<1.2.0
 setuptools>=41.0.0
 six~=1.15.0
 tblib==1.3.2
-tensorflow>=1.15.5,<2.12
+tensorflow>=1.15.5,<2.13
 termcolor==1.1.0
 toml==0.10.0
 toolz==0.9.0
 tornado==5.1.0
 urllib3~=1.26.5
 Werkzeug>=0.15.3
 zict==0.1.3
-zipp==0.6.0
```

### Comparing `subaligner-0.3.1/setup.py` & `subaligner-0.3.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,35 +27,35 @@
     dev_requirements = dev_requirements_file.read().splitlines()[::-1]
 
 EXTRA_DEPENDENCIES = {
     "harmony": stretch_requirements + llm_requirements,
     "dev": dev_requirements + stretch_requirements + llm_requirements + docs_requirements,
     "docs": docs_requirements,
     "stretch": stretch_requirements,
-    "translation": llm_requirements,    # for backward compatibility and will be deprecated with "llm"
+    "translation": llm_requirements,    # for backward compatibility and now deprecated with "llm"
     "llm": llm_requirements,
 }
 
 setup(name="subaligner",
       version=__version__,
       author="Xi Bai",
       author_email="xi.bai.ed@gmail.com",
       classifiers=[
           "License :: OSI Approved :: MIT License",
-          "Programming Language :: Python :: 3.7",
           "Programming Language :: Python :: 3.8",
           "Programming Language :: Python :: 3.9",
+          "Programming Language :: Python :: 3.10",
           "Intended Audience :: Developers",
       ],
       license="MIT",
       url="https://subaligner.readthedocs.io/en/latest/",
-      description="Automatically synchronize and translate subtitles with pretrained deep neural networks, forced alignments and transformers.",
+      description="Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.",
       long_description=readme + "\n\n",
       long_description_content_type='text/markdown',
-      python_requires=">=3.6",
+      python_requires=">=3.8",
       package_dir={"subaligner": "subaligner"},
       packages=[
           "subaligner",
           "subaligner.lib",
           "subaligner.subaligner_1pass",
           "subaligner.subaligner_2pass",
           "subaligner.subaligner_batch",
```

### Comparing `subaligner-0.3.1/subaligner/__main__.py` & `subaligner-0.3.2/subaligner/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/embedder.py` & `subaligner-0.3.2/subaligner/embedder.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/hparam_tuner.py` & `subaligner-0.3.2/subaligner/hparam_tuner.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/hyperparameters.py` & `subaligner-0.3.2/subaligner/hyperparameters.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/lib/language.py` & `subaligner-0.3.2/subaligner/lib/language.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/lib/to_srt.py` & `subaligner-0.3.2/subaligner/lib/to_srt.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/llm.py` & `subaligner-0.3.2/subaligner/llm.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/logger.py` & `subaligner-0.3.2/subaligner/logger.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/media_helper.py` & `subaligner-0.3.2/subaligner/media_helper.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/models/training/config/hyperparameters.json` & `subaligner-0.3.2/subaligner/models/training/config/hyperparameters.json`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/models/training/model/model.hdf5` & `subaligner-0.3.2/subaligner/models/training/model/model.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/models/training/weights/weights.hdf5` & `subaligner-0.3.2/subaligner/models/training/weights/weights.hdf5`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/network.py` & `subaligner-0.3.2/subaligner/network.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/predictor.py` & `subaligner-0.3.2/subaligner/predictor.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/subaligner_1pass/__main__.py` & `subaligner-0.3.2/subaligner/subaligner_1pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/subaligner_2pass/__main__.py` & `subaligner-0.3.2/subaligner/subaligner_2pass/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/subaligner_batch/__main__.py` & `subaligner-0.3.2/subaligner/subaligner_batch/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,54 @@
 #!/usr/bin/env python
 """
-usage: subaligner_batch [-h] [-m {single,dual}] [-vd VIDEO_DIRECTORY] [-sd SUBTITLE_DIRECTORY] [-l MAX_LOGLOSS] [-so]
+usage: subaligner_batch [-h] [-m {single,dual,script,transcribe}] [-sd SUBTITLE_DIRECTORY] [-vd VIDEO_DIRECTORY] [-l MAX_LOGLOSS] [-so]
                         [-sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
-                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-od OUTPUT_DIRECTORY] [-t TRANSLATE] [-lgs] [-d] [-q] [-ver]
+                        [-fos] [-tod TRAINING_OUTPUT_DIRECTORY] [-od OUTPUT_DIRECTORY] [-of {srt,ytt,ttml,txt,smi,xml,ssa,ass,dfxp,sub,scc,tmp,sami,vtt,stl,sbv}] [-t TRANSLATE]
+                        [-ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}]
+                        [-mr {whisper}] [-mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}] [-lgs] [-d] [-q] [-ver]
 
 Batch align multiple subtitle files and audiovisual files
 
 Subtitle files and their companion audiovisual files need to be stored in two separate directories.
 Each file pair needs to share the same base filename, the part before the extension.
 
 optional arguments:
   -h, --help            show this help message and exit
-  -vd VIDEO_DIRECTORY, --video_directory VIDEO_DIRECTORY
-                        Path to the video directory
   -sd SUBTITLE_DIRECTORY, --subtitle_directory SUBTITLE_DIRECTORY
                         Path to the subtitle directory
+  -vd VIDEO_DIRECTORY, --video_directory VIDEO_DIRECTORY
+                        Path to the video directory
   -l MAX_LOGLOSS, --max_logloss MAX_LOGLOSS
                         Max global log loss for alignment
-  -so, --stretch_on    Switch on stretch on subtitles
+  -so, --stretch_on     Switch on stretch on subtitles)
   -sil {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --stretch_in_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
                         Stretch the subtitle with the supported ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes].
                         NB: This will be ignored if neither -so nor --stretch_on is present
   -fos, --exit_segfail  Exit on any segment alignment failures
   -tod TRAINING_OUTPUT_DIRECTORY, --training_output_directory TRAINING_OUTPUT_DIRECTORY
                         Path to the output directory containing training results
   -od OUTPUT_DIRECTORY, --output_directory OUTPUT_DIRECTORY
                         Path to the output subtitle directory
+  -of {srt,ytt,ttml,txt,smi,xml,ssa,ass,dfxp,sub,scc,tmp,sami,vtt,stl,sbv}, --output_format {srt,ytt,ttml,txt,smi,xml,ssa,ass,dfxp,sub,scc,tmp,sami,vtt,stl,sbv}
+                        File format of the output subtitles
   -t TRANSLATE, --translate TRANSLATE
                         Source and target ISO 639-3 language codes separated by a comma (e.g., eng,zho)
+  -ml {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}, --main_language {afr,amh,ara,arg,asm,aze,ben,bos,bul,cat,ces,cmn,cym,dan,deu,ell,eng,epo,est,eus,fas,fin,fra,gla,gle,glg,grc,grn,guj,heb,hin,hrv,hun,hye,ina,ind,isl,ita,jbo,jpn,kal,kan,kat,kir,kor,kur,lat,lav,lfn,lit,mal,mar,mkd,mlt,msa,mya,nah,nep,nld,nor,ori,orm,pan,pap,pol,por,ron,rus,sin,slk,slv,spa,sqi,srp,swa,swe,tam,tat,tel,tha,tsn,tur,ukr,urd,vie,yue,zho}
+                        Target video's main language as an ISO 639-3 language code [https://en.wikipedia.org/wiki/List_of_ISO_639-3_codes]
+  -mr {whisper}, --transcription_recipe {whisper}
+                        LLM recipe used for transcribing video files
+  -mf {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}, --transcription_flavour {tiny,tiny.en,small,medium,medium.en,base,base.en,large-v1,large-v2,large}
+                        Flavour variation for a specific LLM recipe supporting transcription
   -lgs, --languages     Print out language codes used for stretch and translation
   -d, --debug           Print out debugging information
   -q, --quiet           Switch off logging information
   -ver, --version       show program's version number and exit
 
 required arguments:
-  -m {single,dual}, --mode {single,dual}
+  -m {single,dual,script,transcribe}, --mode {single,dual,script,transcribe}
                         Alignment mode: either single or dual
 """
 
 import argparse
 import sys
 import traceback
 import os
```

### Comparing `subaligner-0.3.1/subaligner/subaligner_convert/__main__.py` & `subaligner-0.3.2/subaligner/subaligner_convert/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/subaligner_train/__main__.py` & `subaligner-0.3.2/subaligner/subaligner_train/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/subaligner_tune/__main__.py` & `subaligner-0.3.2/subaligner/subaligner_tune/__main__.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/subtitle.py` & `subaligner-0.3.2/subaligner/subtitle.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner/trainer.py` & `subaligner-0.3.2/subaligner/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import threading
 import traceback
 import concurrent.futures
 import math
 import numpy as np
 import multiprocessing as mp
 
-from typing import List, Tuple, Optional
+from typing import List, Tuple, Optional, Union
 from .network import Network
 from .media_helper import MediaHelper
 from .hyperparameters import Hyperparameters
 from .embedder import FeatureEmbedder
 from .exception import TerminalException
 from .logger import Logger
 
@@ -326,16 +326,16 @@
         return train_data, labels
 
     def __extract_in_multithreads(
         self,
         index: int,
         av_file_path: str,
         subtitle_file_path: str,
-        train_data: np.ndarray,
-        labels: np.ndarray,
+        train_data: Union[np.ndarray, List],
+        labels: Union[np.ndarray, List],
         sound_effect_start_marker: Optional[str],
         sound_effect_end_marker: Optional[str]
     ) -> Tuple[str, str]:
         _, file_ext = os.path.splitext(av_file_path)
 
         try:
             if file_ext not in self.__media_helper.AUDIO_FILE_EXTENSION:
```

### Comparing `subaligner-0.3.1/subaligner/transcriber.py` & `subaligner-0.3.2/subaligner/transcriber.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             lang = Utils.get_iso_639_alpha_2(language_code)
             if lang not in LANGUAGES:
                 raise TranscriptionException(f'"{language_code}" is not supported by {self.__recipe} ({self.__flavour})')
             audio_file_path = self.__media_helper.extract_audio(video_file_path, True, 16000)
             try:
                 audio = whisper.load_audio(audio_file_path)
                 self.__LOGGER.debug("Start transcribing the audio...")
-                result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang])
+                result = self.__model.transcribe(audio, task="transcribe", language=LANGUAGES[lang], logprob_threshold=-1.2, no_speech_threshold=0.16)
                 self.__LOGGER.info("Finished transcribing the audio")
                 srt_str = ""
                 for i, segment in enumerate(result["segments"], start=1):
                     srt_str += f"{i}\n" \
                                f"{Utils.format_timestamp(segment['start'])} --> {Utils.format_timestamp(segment['end'])}\n" \
                                f"{segment['text'].strip().replace('-->', '->')}\n" \
                                "\n"
```

### Comparing `subaligner-0.3.1/subaligner/translator.py` & `subaligner-0.3.2/subaligner/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,34 +108,34 @@
             for index in range(len(new_subs)):
                 new_subs[index].text = translated_texts[index]
             self.__LOGGER.info("Subtitle translated")
             return new_subs
         elif self.__recipe == TranslationRecipe.WHISPER.value:
             assert video_file_path is not None
             lang = Utils.get_iso_639_alpha_2(self.__tgt_language)
-            if lang not in LANGUAGES:
-                raise TranslationException(f'"{self.__tgt_language}" is not supported by {self.__recipe}')
+            if lang not in LANGUAGES or lang != "en":
+                raise TranslationException(f'"{self.__tgt_language}" is not supported by {self.__recipe} as a translation target by {self.__recipe}')
             audio = whisper.load_audio(video_file_path)
             self.__LOGGER.debug("Start translating the audio...")
-            result = self.__lang_model.transcribe(audio, task="translate", language=LANGUAGES[lang])
+            result = self.__lang_model.transcribe(audio, task="translate")
             self.__LOGGER.info("Finished translating the audio")
             srt_str = ""
             for i, segment in enumerate(result["segments"], start=1):
                 srt_str += f"{i}\n" \
                            f"{Utils.format_timestamp(segment['start'])} --> {Utils.format_timestamp(segment['end'])}\n" \
                            f"{segment['text'].strip().replace('-->', '->')}\n" \
                            "\n"
             subtitle = Subtitle.load_subrip_str(srt_str)
             return subtitle.subs
         elif self.__recipe == TranslationRecipe.FACEBOOK_MBART.value:
             src_lang, tgt_lang = language_pair if language_pair is not None else (self.__src_language, self.__tgt_language)
             self.__tokenizer.src_lang = Translator.__MBART_LANGUAGE_CODE_MAPPER.get(src_lang, None)
             lang_code = Translator.__MBART_LANGUAGE_CODE_MAPPER.get(tgt_lang, None)
             if src_lang is None or tgt_lang is None:
-                raise NotImplementedError(f"Language pair of {src_lang} and {src_lang} is not supported")
+                raise NotImplementedError(f"Language pair of {src_lang} and {src_lang} is not supported by {self.__recipe}")
             translated_texts = []
             self.__lang_model.eval()
             new_subs = deepcopy(subs)
             src_texts = [sub.text for sub in new_subs]
             num_of_batches = math.ceil(len(src_texts) / Translator.__TRANSLATING_BATCH_SIZE)
             self.__LOGGER.info("Translating %s subtitle cue(s)..." % len(src_texts))
             for batch in tqdm(Translator.__batch(src_texts, Translator.__TRANSLATING_BATCH_SIZE), total=num_of_batches):
@@ -159,15 +159,15 @@
             if self.__download_mt_model(src_lang, tgt_lang, HelsinkiNLPFlavour.OPUS_MT.value):
                 return
             elif self.__download_mt_model(src_lang, tgt_lang, HelsinkiNLPFlavour.OPUS_TATOEBA.value):
                 return
             elif self.__download_mt_model(src_lang, tgt_lang, HelsinkiNLPFlavour.OPUS_MT_TC_BIG.value):
                 return
             else:
-                message = 'Cannot find the MT model for source language "{}" and destination language "{}"'.format(src_lang, tgt_lang)
+                message = f'Cannot find the {recipe} MT model for source language "{src_lang}" and destination language "{tgt_lang}"'
                 self.__LOGGER.error(message)
                 raise NotImplementedError(message)
         elif recipe == TranslationRecipe.WHISPER.value:
             if flavour in [f.value for f in WhisperFlavour]:
                 # self.__download_whisper_model(flavour)
                 self.__download_whisper_model("medium")  # works for translation target other than English
             else:
```

### Comparing `subaligner-0.3.1/subaligner/utils.py` & `subaligner-0.3.2/subaligner/utils.py`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner.egg-info/PKG-INFO` & `subaligner-0.3.2/subaligner.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: subaligner
-Version: 0.3.1
-Summary: Automatically synchronize and translate subtitles with pretrained deep neural networks, forced alignments and transformers.
+Version: 0.3.2
+Summary: Automatically synchronize and translate subtitles, or create new ones by transcribing, using pre-trained DNNs, Forced Alignments and Transformers.
 Home-page: https://subaligner.readthedocs.io/en/latest/
 Author: Xi Bai
 Author-email: xi.bai.ed@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: harmony
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: stretch
 Provides-Extra: translation
 Provides-Extra: llm
@@ -26,15 +26,14 @@
 </div>
 
 [![Build Status](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml/badge.svg?branch=master)](https://github.com/baxtree/subaligner/actions/workflows/ci-pipeline.yml?query=branch%3Amaster) ![Codecov](https://img.shields.io/codecov/c/github/baxtree/subaligner)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)](https://www.python.org/downloads/release/python-3100/) [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-390/) [![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)
 [![Documentation Status](https://readthedocs.org/projects/subaligner/badge/?version=latest)](https://subaligner.readthedocs.io/en/latest/?badge=latest)
 [![GitHub license](https://img.shields.io/github/license/baxtree/subaligner)](https://github.com/baxtree/subaligner/blob/master/LICENSE)
 [![PyPI](https://badge.fury.io/py/subaligner.svg)](https://badge.fury.io/py/subaligner)
-[![Docker Build](https://img.shields.io/docker/cloud/build/baxtree/subaligner?label=Docker&style=flat)](https://hub.docker.com/r/baxtree/subaligner/builds)
 [![Docker Pulls](https://img.shields.io/docker/pulls/baxtree/subaligner)](https://hub.docker.com/r/baxtree/subaligner)
 [![Citation](https://zenodo.org/badge/228440472.svg)](https://doi.org/10.5281/zenodo.5603083)
 
 ## Supported Formats
 Subtitle: SubRip, TTML, WebVTT, (Advanced) SubStation Alpha, MicroDVD, MPL2, TMP, EBU STL, SAMI, SCC and SBV.
 
 Video/Audio: MP4, WebM, Ogg, 3GP, FLV, MOV, Matroska, MPEG TS, WAV, MP3, AAC, FLAC, etc.
```

### Comparing `subaligner-0.3.1/subaligner.egg-info/SOURCES.txt` & `subaligner-0.3.2/subaligner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `subaligner-0.3.1/subaligner.egg-info/requires.txt` & `subaligner-0.3.2/subaligner.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-zipp==0.6.0
 zict==0.1.3
 Werkzeug>=0.15.3
 urllib3~=1.26.5
 tornado==5.1.0
 toolz==0.9.0
 toml==0.10.0
 termcolor==1.1.0
-tensorflow<2.12,>=1.15.5
+tensorflow<2.13,>=1.15.5
 tblib==1.3.2
 six~=1.15.0
 setuptools>=41.0.0
 scikit-learn<1.2.0
 scipy<=1.8.1
 rsa==4.7
 requests-oauthlib==1.3.0
-requests~=2.25.1
+requests<3.0.0
 PyYAML>=4.2b1
 pytz==2018.4
 pystack-debugger==0.8.0
 pysubs2<=1.4.2
 pysrt==1.1.1
 pyprof2calltree==1.4.3
 pydotplus==2.0.2
 pydot-ng==1.0.0
 pydot==1.2.4
+pycountry~=20.7.3
 pyasn1-modules==0.2.7
 pyasn1==0.4.8
 py==1.10.0
 psutil==5.6.7
 pluggy==0.13.1
 pbr==4.0.2
 oauthlib==3.1.0
@@ -73,31 +73,30 @@
 [dev]
 pygments==2.7.4
 pylint~=2.8.2
 parameterized==0.8.1
 typing-extensions<4.0.0
 types-setuptools==57.4.9
 types-requests==2.27.9
-mypy==0.931
+mypy==1.3.0
 pex<=2.1.80
 radish-bdd~=0.13.3
 scikit-build==0.11.1
 line-profiler==3.1.0
 snakeviz==2.1.0
-twine>=3.1.1
+twine<4.0.0
 pycodestyle==2.5.0
 tox~=3.23.0
 coverage==5.5
 mock==4.0.3
 aeneas~=1.7.3.0
 openai-whisper==20230124
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
-pycountry~=20.7.3
 docutils~=0.17.0
 sphinx-rtd-theme==0.5.0
 sphinx==3.3.1
 
 [docs]
 docutils~=0.17.0
 sphinx-rtd-theme==0.5.0
@@ -105,25 +104,22 @@
 
 [harmony]
 aeneas~=1.7.3.0
 openai-whisper==20230124
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
-pycountry~=20.7.3
 
 [llm]
 openai-whisper==20230124
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
-pycountry~=20.7.3
 
 [stretch]
 aeneas~=1.7.3.0
 
 [translation]
 openai-whisper==20230124
 transformers<4.27.0
 torch<1.13.0
 sentencepiece~=0.1.95
-pycountry~=20.7.3
```

