# Comparing `tmp/transphone-1.5.1.tar.gz` & `tmp/transphone-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/transphone-1.5.1.tar", last modified: Mon May 22 17:14:33 2023, max compression
+gzip compressed data, was "dist/transphone-1.5.3.tar", last modified: Fri Jun  9 20:51:07 2023, max compression
```

## Comparing `transphone-1.5.1.tar` & `transphone-1.5.3.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.5.1/LICENSE
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-22 17:14:33.000000 transphone-1.5.1/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.5.1/README.md
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-05-22 17:14:33.000000 transphone-1.5.1/setup.cfg
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      387 2023-05-22 17:14:30.000000 transphone-1.5.1/setup.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/test/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.5.1/test/test_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.5.1/transphone/__init__.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/bin/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.5.1/transphone/bin/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/download_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/eval_epitran.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/eval_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/eval_zsl_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/tokenize.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/train_g2p.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/bin/update_model.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/config.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/data/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.5.1/transphone/data/__init__.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/data/exp/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       86 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/data/exp/042801_base.yml
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/g2p.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2128 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/lang/base_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/cmn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/cmn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.5.1/transphone/lang/cmn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.5.1/transphone/lang/cmn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/eng/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/eng/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3341 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/lang/eng/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2284 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/lang/eng/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-15 13:58:49.000000 transphone-1.5.1/transphone/lang/epitran_tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1826 2023-05-19 07:10:11.000000 transphone-1.5.1/transphone/lang/g2p_tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/lang/jpn/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.1/transphone/lang/jpn/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.5.1/transphone/lang/jpn/conv_table.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.5.1/transphone/lang/jpn/jaconv.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/lang/jpn/kana2phoneme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/lang/jpn/normalizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.5.1/transphone/lang/jpn/tokenizer.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/model/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.5.1/transphone/model/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/checkpoint_utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/dataset.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.5.1/transphone/model/ensemble.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/grapheme.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/loader.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/lstm.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/transformer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/utils.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/model/vocab.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone/pretrained/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.5.1/transphone/pretrained/__init__.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2536 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/run.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.5.1/transphone/tokenizer.py
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.5.1/transphone/utils.py
-drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/PKG-INFO
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1514 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/SOURCES.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/dependency_links.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/requires.txt
--rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-05-22 17:14:33.000000 transphone-1.5.1/transphone.egg-info/top_level.txt
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1072 2022-10-27 20:49:08.000000 transphone-1.5.3/LICENSE
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-06-09 20:51:07.000000 transphone-1.5.3/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8168 2023-05-15 07:50:03.000000 transphone-1.5.3/README.md
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       38 2023-06-09 20:51:07.000000 transphone-1.5.3/setup.cfg
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      438 2023-06-09 20:51:00.000000 transphone-1.5.3/setup.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/test/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2730 2023-05-08 16:31:27.000000 transphone-1.5.3/test/test_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       47 2022-11-23 17:53:06.000000 transphone-1.5.3/transphone/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/bin/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:22.000000 transphone-1.5.3/transphone/bin/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1545 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/download_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3451 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/eval_epitran.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3551 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/eval_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3634 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/eval_zsl_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2844 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2679 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/tokenize.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3816 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/train_g2p.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1618 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/bin/update_model.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      325 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/config.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/data/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:30.000000 transphone-1.5.3/transphone/data/__init__.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/data/exp/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       86 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/data/exp/042801_base.yml
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:00.000000 transphone-1.5.3/transphone/data/exp/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9724 2023-06-09 20:51:00.000000 transphone-1.5.3/transphone/g2p.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/lang/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.3/transphone/lang/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2234 2023-06-09 20:51:00.000000 transphone-1.5.3/transphone/lang/base_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/lang/cmn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.3/transphone/lang/cmn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    55821 2022-11-24 02:03:19.000000 transphone-1.5.3/transphone/lang/cmn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1750 2023-05-15 07:50:03.000000 transphone-1.5.3/transphone/lang/cmn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/lang/eng/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.3/transphone/lang/eng/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     3342 2023-06-09 20:51:00.000000 transphone-1.5.3/transphone/lang/eng/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2412 2023-06-09 20:51:00.000000 transphone-1.5.3/transphone/lang/eng/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9371 2023-05-15 13:58:49.000000 transphone-1.5.3/transphone/lang/epitran_tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1826 2023-05-19 07:10:11.000000 transphone-1.5.3/transphone/lang/g2p_tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/lang/jpn/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-11-23 19:17:09.000000 transphone-1.5.3/transphone/lang/jpn/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9740 2022-11-25 20:08:08.000000 transphone-1.5.3/transphone/lang/jpn/conv_table.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    15327 2022-11-25 20:04:35.000000 transphone-1.5.3/transphone/lang/jpn/jaconv.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     9520 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/lang/jpn/kana2phoneme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5192 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/lang/jpn/normalizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2775 2023-05-15 07:50:03.000000 transphone-1.5.3/transphone/lang/jpn/tokenizer.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/model/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 17:58:35.000000 transphone-1.5.3/transphone/model/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)    13693 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/checkpoint_utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     6628 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/dataset.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     5388 2022-03-13 19:18:49.000000 transphone-1.5.3/transphone/model/ensemble.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1782 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/grapheme.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      409 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/loader.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     8331 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/lstm.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     7420 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/transformer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1722 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/utils.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1046 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/model/vocab.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone/pretrained/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        0 2022-09-08 18:28:14.000000 transphone-1.5.3/transphone/pretrained/__init__.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     2827 2023-06-09 20:51:00.000000 transphone-1.5.3/transphone/run.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1350 2023-05-15 07:50:03.000000 transphone-1.5.3/transphone/tokenizer.py
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      491 2023-05-08 16:31:27.000000 transphone-1.5.3/transphone/utils.py
+drwxrwxr-x   0 xinjianl  (1000) xinjianl  (1000)        0 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone.egg-info/
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      260 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone.egg-info/PKG-INFO
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)     1546 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone.egg-info/SOURCES.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)        1 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone.egg-info/dependency_links.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)      111 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone.egg-info/requires.txt
+-rw-rw-r--   0 xinjianl  (1000) xinjianl  (1000)       11 2023-06-09 20:51:07.000000 transphone-1.5.3/transphone.egg-info/top_level.txt
```

### Comparing `transphone-1.5.1/LICENSE` & `transphone-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/README.md` & `transphone-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/test/test_tokenizer.py` & `transphone-1.5.3/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/download_model.py` & `transphone-1.5.3/transphone/bin/download_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/eval_epitran.py` & `transphone-1.5.3/transphone/bin/eval_epitran.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/eval_g2p.py` & `transphone-1.5.3/transphone/bin/eval_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/eval_zsl_g2p.py` & `transphone-1.5.3/transphone/bin/eval_zsl_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/g2p.py` & `transphone-1.5.3/transphone/bin/g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/tokenize.py` & `transphone-1.5.3/transphone/bin/tokenize.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/train_g2p.py` & `transphone-1.5.3/transphone/bin/train_g2p.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/bin/update_model.py` & `transphone-1.5.3/transphone/bin/update_model.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/g2p.py` & `transphone-1.5.3/transphone/g2p.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,26 @@
 from itertools import groupby
 from transphone.model.utils import resolve_model_name
 
 
 def read_g2p(model_name='latest', device=None, checkpoint=None):
 
     if device is not None:
-        assert device in ['cpu', 'cuda']
-        TransphoneConfig.device = device
+        if isinstance(device, str):
+            assert device in ['cpu', 'cuda']
+            TransphoneConfig.device = device
+        elif isinstance(device, int):
+            if device == -1:
+                TransphoneConfig.device = 'cpu'
+            else:
+                TransphoneConfig.device = f'cuda:{device}'
+
+        else:
+            assert isinstance(device, torch.device)
+            TransphoneConfig.device = device.type
 
     model_name = resolve_model_name(model_name)
     cache_path = None
 
     if checkpoint is None:
         model_path = TransphoneConfig.data_path / 'model' / model_name
```

### Comparing `transphone-1.5.1/transphone/lang/base_tokenizer.py` & `transphone-1.5.3/transphone/lang/base_tokenizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         if self.g2p is not None and self.g2p.cache_path is not None:
             lang_cache_path = self.g2p.cache_path / f"{lang_id}.txt"
             if lang_cache_path.exists():
                 for line in open(lang_cache_path, 'r'):
                     fields = line.strip().split()
                     self.cache[fields[0]] = fields[1:]
 
-        self.punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~'
+        self.punctuation = '!"#$%&\'()*+,-./:;<=>?@[\\]^_`{|}~0123456789'
         self.logger = TransphoneConfig.logger
 
     def add_cache(self, word, phonemes):
 
         self.cache[word] = phonemes
 
         if self.g2p is None or self.g2p.cache_path is None:
@@ -49,14 +49,17 @@
 
     def tokenize(self, text: str):
         raise NotImplementedError
 
     def tokenize_words(self, text:str):
         text = text.translate(str.maketrans('', '', self.punctuation)).lower()
 
+        words = text.split()
+        cleaned_words = [word for word in words if len(word) > 0]
+
         return text.split()
 
     def convert_tokens_to_ids(self, lst):
         lst = list(filter(lambda s: s!='<SPACE>', lst))
 
         return self.inventory.phoneme.atoi(lst)
```

### Comparing `transphone-1.5.1/transphone/lang/cmn/normalizer.py` & `transphone-1.5.3/transphone/lang/cmn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/cmn/tokenizer.py` & `transphone-1.5.3/transphone/lang/cmn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/eng/normalizer.py` & `transphone-1.5.3/transphone/lang/eng/normalizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 
         tokens = text.split()
 
         res = []
         for token in tokens:
             if str.isdigit(token):
                 # 1 Filter out anything that isn't a digit
-                token = self.filter_regex.sub("", text)
+                token = self.filter_regex.sub("", token)
                 # 2 Check for special case
                 if token == "007":
                     return "double o seven"
 
                 token = number_to_words(int(token))
 
             res.append(token)
```

### Comparing `transphone-1.5.1/transphone/lang/eng/tokenizer.py` & `transphone-1.5.3/transphone/lang/eng/tokenizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,19 @@
 
         # import jieba and pypinyin for segmentation
         cmudict_module = import_with_auto_install('cmudict', 'cmudict')
         self.cmudict = cmudict_module.dict()
         self.converter = ArpaConverter()
         self.normalizer = ENGNormalizer()
 
+    def tokenize_words(self, text:str):
+        text = self.normalizer(text)
+        words = text.split()
+        return words
+
     def tokenize(self, text, use_g2p=True, use_space=False, verbose=False):
 
         norm_text = self.normalizer(text)
 
         log = f"normalization: {text} -> {norm_text}"
         self.logger.info(log)
         if verbose:
```

### Comparing `transphone-1.5.1/transphone/lang/epitran_tokenizer.py` & `transphone-1.5.3/transphone/lang/epitran_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/g2p_tokenizer.py` & `transphone-1.5.3/transphone/lang/g2p_tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/jpn/conv_table.py` & `transphone-1.5.3/transphone/lang/jpn/conv_table.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/jpn/jaconv.py` & `transphone-1.5.3/transphone/lang/jpn/jaconv.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/jpn/kana2phoneme.py` & `transphone-1.5.3/transphone/lang/jpn/kana2phoneme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/jpn/normalizer.py` & `transphone-1.5.3/transphone/lang/jpn/normalizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/lang/jpn/tokenizer.py` & `transphone-1.5.3/transphone/lang/jpn/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/checkpoint_utils.py` & `transphone-1.5.3/transphone/model/checkpoint_utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/dataset.py` & `transphone-1.5.3/transphone/model/dataset.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/ensemble.py` & `transphone-1.5.3/transphone/model/ensemble.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/grapheme.py` & `transphone-1.5.3/transphone/model/grapheme.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/lstm.py` & `transphone-1.5.3/transphone/model/lstm.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/transformer.py` & `transphone-1.5.3/transphone/model/transformer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/utils.py` & `transphone-1.5.3/transphone/model/utils.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/model/vocab.py` & `transphone-1.5.3/transphone/model/vocab.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone/run.py` & `transphone-1.5.3/transphone/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     parser.add_argument('-m', '--model', type=str, default='latest',
                         help='specify which model to use. default is to use the latest local model')
     parser.add_argument('-l', '--lang', type=str, default='eng',
                         help='specify which language inventory to use for recognition. default is to use all phone inventory')
     parser.add_argument('-i', '--input', type=str, required=True, help='specify your input wav file/directory')
     parser.add_argument('-o', '--output', type=str, default='stdout',
                         help='specify output file. the default will be stdout')
+    parser.add_argument('-d', '--device', help='specify device to use, if not specified, it will try using gpu when applicable')
     parser.add_argument('-f', '--format', type=str, default='text', help='kaldi or text')
     parser.add_argument('-c', '--combine', type=bool, default=False,
                         help='write outputs by including both grapheme inputs and phonemes in the same line, delimited by space')
 
     args = parser.parse_args()
 
     # resolve model's name
@@ -30,16 +31,20 @@
 
     if args.combine:
         assert file_format == 'text'
 
     # download specified model automatically if no model exists
     download_model(model_name)
 
+    device = None
+    if args.device is not None and isinstance(args.device, str) and str.isdigit(args.device):
+        device = int(args.device)
+
     # create model
-    tokenizer = read_tokenizer(args.lang, g2p_model=model_name)
+    tokenizer = read_tokenizer(args.lang, g2p_model=model_name, device=device)
 
     # output file descriptor
     output_fd = None
     if args.output != 'stdout':
         output_fd = open(args.output, 'w', encoding='utf-8')
 
     # input file/path
```

### Comparing `transphone-1.5.1/transphone/tokenizer.py` & `transphone-1.5.3/transphone/tokenizer.py`

 * *Files identical despite different names*

### Comparing `transphone-1.5.1/transphone.egg-info/SOURCES.txt` & `transphone-1.5.3/transphone.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 transphone/bin/eval_zsl_g2p.py
 transphone/bin/g2p.py
 transphone/bin/tokenize.py
 transphone/bin/train_g2p.py
 transphone/bin/update_model.py
 transphone/data/__init__.py
 transphone/data/exp/042801_base.yml
+transphone/data/exp/__init__.py
 transphone/lang/__init__.py
 transphone/lang/base_tokenizer.py
 transphone/lang/epitran_tokenizer.py
 transphone/lang/g2p_tokenizer.py
 transphone/lang/cmn/__init__.py
 transphone/lang/cmn/normalizer.py
 transphone/lang/cmn/tokenizer.py
```

