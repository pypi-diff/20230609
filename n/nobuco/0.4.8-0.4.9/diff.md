# Comparing `tmp/nobuco-0.4.8.tar.gz` & `tmp/nobuco-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.8.tar", last modified: Tue Jun  6 19:07:02 2023, max compression
+gzip compressed data, was "nobuco-0.4.9.tar", last modified: Fri Jun  9 15:15:49 2023, max compression
```

## Comparing `nobuco-0.4.8.tar` & `nobuco-0.4.9.tar`

### file list

```diff
@@ -1,67 +1,68 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.8/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-06 19:07:02.904725 nobuco-0.4.8/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.8/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.896725 nobuco-0.4.8/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13632 2023-06-02 13:57:44.000000 nobuco-0.4.8/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.4.8/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.4.8/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     4060 2023-06-06 18:54:07.000000 nobuco-0.4.8/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.8/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.4.8/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.900725 nobuco-0.4.8/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.8/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.4.8/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.8/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.8/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13828 2023-06-01 14:04:11.000000 nobuco-0.4.8/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.8/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.4.8/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.4.8/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7504 2023-06-06 19:04:06.000000 nobuco-0.4.8/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.8/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-16 10:06:21.000000 nobuco-0.4.8/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-05-17 10:49:15.000000 nobuco-0.4.8/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.904725 nobuco-0.4.8/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.8/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-06 19:07:02.896725 nobuco-0.4.8/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-06 19:07:02.000000 nobuco-0.4.8/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-06 19:05:25.000000 nobuco-0.4.8/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-06 19:07:02.904725 nobuco-0.4.8/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.9/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-09 15:15:49.353446 nobuco-0.4.9/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.9/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13696 2023-06-09 15:12:04.000000 nobuco-0.4.9/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-06-02 13:56:50.000000 nobuco-0.4.9/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2256 2023-06-02 12:03:42.000000 nobuco-0.4.9/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4064 2023-06-06 20:42:12.000000 nobuco-0.4.9/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.9/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1069 2023-06-06 15:58:09.000000 nobuco-0.4.9/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.9/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.4.9/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.9/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1533 2023-06-06 20:30:38.000000 nobuco-0.4.9/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.9/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13838 2023-06-06 20:13:59.000000 nobuco-0.4.9/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.9/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.4.9/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1261 2023-06-07 02:32:02.000000 nobuco-0.4.9/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.4.9/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7966 2023-06-09 15:13:56.000000 nobuco-0.4.9/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.9/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5969 2023-06-07 02:44:23.000000 nobuco-0.4.9/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-06-06 20:13:14.000000 nobuco-0.4.9/nobuco/node_converters/tensor_manipulation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      369 2023-06-06 21:33:32.000000 nobuco-0.4.9/nobuco/node_converters/tensor_shape.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1378 2023-06-06 19:21:15.000000 nobuco-0.4.9/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10039 2023-06-09 15:11:00.000000 nobuco-0.4.9/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.353446 nobuco-0.4.9/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.9/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-09 15:15:49.349446 nobuco-0.4.9/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1628 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-09 15:15:49.000000 nobuco-0.4.9/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-09 15:14:07.000000 nobuco-0.4.9/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-09 15:15:49.353446 nobuco-0.4.9/setup.cfg
```

### Comparing `nobuco-0.4.8/LICENSE` & `nobuco-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/PKG-INFO` & `nobuco-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.8
+Version: 0.4.9
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.8/README.md` & `nobuco-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/__init__.py` & `nobuco-0.4.9/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/commons.py` & `nobuco-0.4.9/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/convert.py` & `nobuco-0.4.9/nobuco/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,30 +237,31 @@
         module: nn.Module,
         args: List[object] = None,
         kwargs: Dict[str, object] = None,
         input_shapes: Dict[torch.Tensor, Collection[Optional[int]]] = None,
         inputs_channel_order: Union[ChannelOrder, Dict[torch.Tensor, ChannelOrder]] = ChannelOrder.TENSORFLOW,
         outputs_channel_order: Union[ChannelOrder, Dict[int, ChannelOrder]] = None,
         converter_dict=CONVERTER_DICT,
+        trace_shape: bool = False,
         constants_to_variables: bool = True,
         full_validation: bool = True,
         validation_tolerance=1e-4,
-        save_trace_html=False,
-        return_outputs_pt=False,
+        save_trace_html: bool = False,
+        return_outputs_pt: bool = False,
         debug_traces: TraceLevel = TraceLevel.DEFAULT,
 ) -> Union[keras.Model, Tuple[keras.Model, object]]:
 
     if args is None:
         args = []
 
     if kwargs is None:
         kwargs = {}
 
     start = time.time()
-    node_hierarchy = Tracer.trace(module, args, kwargs)
+    node_hierarchy = Tracer.trace(module, trace_shape, args, kwargs)
 
     keras_converted_node = convert_hierarchy(node_hierarchy, converter_dict,
                                              reuse_layers=True, full_validation=full_validation, constants_to_variables=constants_to_variables,
                                              tolerance=validation_tolerance,
                                              )
 
     validation_result_dict = collect_validation_results(keras_converted_node)
```

### Comparing `nobuco-0.4.8/nobuco/converters/channel_ordering.py` & `nobuco-0.4.9/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/converters/node_converter.py` & `nobuco-0.4.9/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/converters/tensor.py` & `nobuco-0.4.9/nobuco/converters/tensor.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/converters/type_cast.py` & `nobuco-0.4.9/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/converters/validation.py` & `nobuco-0.4.9/nobuco/converters/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,16 +81,16 @@
     if len(outputs_tf_converted) != len(outputs_pt):
         raise Exception(f"Number of outputs do not match: (Pytorch) {len(outputs_pt)} vs {len(outputs_tf_converted)} (Tensorflow)")
 
     for t_tf, t_pt in zip(outputs_tf_converted, outputs_pt):
         if t_tf.shape != t_pt.shape:
             raise Exception(f"Tensor shapes don't match: (Pytorch) {list(t_pt.shape)} vs {list(t_tf.shape)} (Tensorflow)")
 
-        if t_tf.dtype != t_pt.dtype:
-            raise Exception(f"Tensor dtypes don't match: (Pytorch) {t_pt.dtype} vs {t_tf.dtype} (Tensorflow)")
+        # if t_tf.dtype != t_pt.dtype:
+        #     raise Exception(f"Tensor dtypes don't match: (Pytorch) {t_pt.dtype} vs {t_tf.dtype} (Tensorflow)")
 
     def calc_diff(t1, t2):
         def calc_diff_numerical(t1, t2):
             diff = t1 - t2
             return diff.abs().max().detach().cpu().numpy()
 
         def calc_diff_boolean(t1, t2):
```

### Comparing `nobuco-0.4.8/nobuco/entity/keras.py` & `nobuco-0.4.9/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/entity/pytorch.py` & `nobuco-0.4.9/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/funcs.py` & `nobuco-0.4.9/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/layers/channel_order.py` & `nobuco-0.4.9/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/layers/container.py` & `nobuco-0.4.9/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/layers/weight.py` & `nobuco-0.4.9/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/locate/link.py` & `nobuco-0.4.9/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/locate/locate.py` & `nobuco-0.4.9/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/activation.py` & `nobuco-0.4.9/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/boolean.py` & `nobuco-0.4.9/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.9/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/comparison.py` & `nobuco-0.4.9/nobuco/node_converters/comparison.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/convolution.py` & `nobuco-0.4.9/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/dropout.py` & `nobuco-0.4.9/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/interpolation.py` & `nobuco-0.4.9/nobuco/node_converters/interpolation.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,32 +3,34 @@
 
 from tensorflow.python.ops.image_ops_impl import ResizeMethod
 from torch import Tensor
 
 import tensorflow as tf
 import torch
 import torch.nn.functional as F
+
+from nobuco.commons import TF_TENSOR_CLASSES
 from nobuco.converters.node_converter import converter
 
 
 @converter(F.interpolate)
 def converter_interpolate(input: Tensor, size: Optional[int] = None, scale_factor: Optional[List[float]] = None, mode: str = 'nearest',
                 align_corners: Optional[bool] = None, recompute_scale_factor: Optional[bool] = None, antialias: bool = False):
     if mode == 'bilinear':
         method = ResizeMethod.BILINEAR
     elif mode == 'nearest':
         method = ResizeMethod.NEAREST_NEIGHBOR
     else:
         raise Exception('Unsupported mode: ', mode)
 
     def func(input, size=None, scale_factor=None, mode='nearest', align_corners=None, recompute_scale_factor=None, antialias=False):
-        if isinstance(scale_factor, numbers.Number):
+        if isinstance(scale_factor, numbers.Number) or (isinstance(scale_factor, TF_TENSOR_CLASSES) and tf.size(scale_factor) == 1):
             scale_factor = (scale_factor, scale_factor)
 
-        if isinstance(size, numbers.Number):
+        if isinstance(size, numbers.Number) or (isinstance(size, TF_TENSOR_CLASSES) and tf.size(size) == 1):
             size = (size, size)
 
         if size is None:
             _, h, w, _ = input.shape
             size = (int(h * scale_factor[0]), int(w * scale_factor[1]))
 
         return tf.image.resize(input, size=size, method=method, antialias=antialias)
```

### Comparing `nobuco-0.4.8/nobuco/node_converters/linear.py` & `nobuco-0.4.9/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/math.py` & `nobuco-0.4.9/nobuco/node_converters/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,11 +311,11 @@
         if get_channel_order(input) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, n_dims)
         return tf.keras.backend.argmax(input, axis=dim)
     return func
 
 
 @converter(torch.arange, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
-def converter_arange(start: Number, end: Number, step: Number=1, *, out: Optional[Tensor]=None, dtype: Optional[_dtype]=None, layout: Optional[_layout]=None, device: Optional[Union[_device, str, None]]=None, pin_memory: Optional[_bool]=False, requires_grad: Optional[_bool]=False):
-    def func(start, end, step=1, *, out=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
+def converter_arange(start: Number, end: Number=None, step: Number=1, *, out: Optional[Tensor]=None, dtype: Optional[_dtype]=None, layout: Optional[_layout]=None, device: Optional[Union[_device, str, None]]=None, pin_memory: Optional[_bool]=False, requires_grad: Optional[_bool]=False):
+    def func(start, end=None, step=1, *, out=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
         return tf.range(start, limit=end, delta=step)
     return func
```

### Comparing `nobuco-0.4.8/nobuco/node_converters/misc.py` & `nobuco-0.4.9/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/normalization.py` & `nobuco-0.4.9/nobuco/node_converters/normalization.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/padding.py` & `nobuco-0.4.9/nobuco/node_converters/padding.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,28 +11,26 @@
 from nobuco.converters.tensor import permute_pytorch2keras
 
 
 # TODO: add support for 'negative' paddings
 @converter(F.pad, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_pad(input: Tensor, pad: List[int], mode: str = "constant", value: float = 0.0):
     n_dims = input.dim()
-    pad_dims = len(pad) // 2
-    assert len(pad) % 2 == 0
-    assert pad_dims <= n_dims
 
-    pad_full = []
-    for i in range(pad_dims):
-        pad_full.append(pad[2*i:2*i + 2])
-    for i in range(n_dims - pad_dims):
-        pad_full.append([0, 0])
-    pad_full = list(reversed(pad_full))
+    def func(input, pad, mode="constant", value=0.0):
+        pad_dims = len(pad) // 2
+        assert len(pad) % 2 == 0
+        assert pad_dims <= n_dims
 
-    # pad_full_pos = [(max(s, 0), max(e, 0)) for s, e in pad_full]
-    # pad_full_neg = [(max(-s, 0), max(-e, 0)) for s, e in pad_full]
+        pad_full = []
+        for i in range(pad_dims):
+            pad_full.append(pad[2 * i:2 * i + 2])
+        for i in range(n_dims - pad_dims):
+            pad_full.append([0, 0])
+        pad_full = list(reversed(pad_full))
 
-    def func(input, pad, mode="constant", value=0.0):
         pad = pad_full
         if get_channel_order(input) == ChannelOrder.TENSORFLOW:
             pad = permute_pytorch2keras(pad)
         x = tf.pad(input, pad)
         return x
     return func
```

### Comparing `nobuco-0.4.8/nobuco/node_converters/pooling.py` & `nobuco-0.4.9/nobuco/node_converters/pooling.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/recurrent.py` & `nobuco-0.4.9/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/slice.py` & `nobuco-0.4.9/nobuco/node_converters/slice.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     shape = tensors[0].shape
     for tens in tensors:
         shape = tf.broadcast_dynamic_shape(shape, tens.shape)
     tensors = [tf.broadcast_to(t, shape) for t in tensors]
     return tensors
 
 
-def slice_assign(sliced_tensor, assigned_tensor, slice_args):
+def slice_assign(sliced_tensor, assigned_tensor, slice_args, is_scatter=False):
     slice_args = _ensure_iterable(slice_args)
     """Assign a tensor to the slice of another tensor.
     No broadcast is performed.
     Args:
         - sliced_tensor (tf.Tensor): the tensor whose slice you want changed.
         - assigned_tensor (tf.Tensor): the tensor which you want assigned.
         - *slice_args (str or slice): the slices arguments. Can be ':', '...'
@@ -113,16 +113,19 @@
         tf.reshape(slicing_range, (-1,))
         for slicing_range in mesh_ranges
     ], axis=-1)
 
     if isinstance(assigned_tensor, TF_TENSOR_CLASSES) and len(assigned_tensor.shape) == len(scatted_nd_perm):
         assigned_tensor = tf.transpose(assigned_tensor, scatted_nd_perm)
 
-    assigned_tensor_reshaped = to_shape_and_dtype(assigned_tensor, sliced_shape, sliced_tensor.dtype)
-    assigned_tensor_reshaped = tf.reshape(assigned_tensor_reshaped, [-1] + left_out_shape)
+    if is_scatter:
+        assigned_tensor_reshaped = assigned_tensor
+    else:
+        assigned_tensor_reshaped = to_shape_and_dtype(assigned_tensor, sliced_shape, sliced_tensor.dtype)
+        assigned_tensor_reshaped = tf.reshape(assigned_tensor_reshaped, [-1] + left_out_shape)
 
     # NOTE: the tensors are reshaped to allow for easier indexing with
     sliced_tensor_reshaped = tf.transpose(sliced_tensor, perm=scatted_nd_perm)
 
     # finalisation
     sliced_tensor_reshaped = tf.tensor_scatter_nd_update(
         tensor=sliced_tensor_reshaped,
@@ -192,7 +195,16 @@
 
     def func(sliced_tensor, slice_args, assigned_tensor):
         if get_channel_order(sliced_tensor) == ChannelOrder.TENSORFLOW:
             slice_args = slices_make_full(slice_args, n_dims)
             slice_args = permute_pytorch2keras(slice_args)
         return slice_assign(sliced_tensor, assigned_tensor, slice_args)
     return func
+
+
+# @converter(torch.Tensor.scatter, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+# def converter_scatter(self, dim, index, src):
+#     assert dim == 0
+#     def func(self, dim, index, src):
+#         slice_args = (tf.reshape(index, -1),)
+#         return slice_assign(self, src, slice_args, is_scatter=True)
+#     return func
```

### Comparing `nobuco-0.4.8/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.9/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.9/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/trace/tensor_storage.py` & `nobuco-0.4.9/nobuco/trace/tensor_storage.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,11 +35,10 @@
 
     def replace_func(tensor):
         cached = storage.get(tensor)
         if cached is None:
             cached = clone(tensor)
             storage.add(cached)
         return cached
-        # return clone(tensor)
 
     replace_dict = {id(c): replace_func(c) for c in collected}
     return deepcopy(obj, memo=replace_dict)
```

### Comparing `nobuco-0.4.8/nobuco/trace/trace.py` & `nobuco-0.4.9/nobuco/trace/trace.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from copy import deepcopy
 from typing import List, Collection, Callable, Union
 
 import torch
 import torchvision
 from torch import nn
 
+import nobuco
 from nobuco.entity.pytorch import PytorchNode, WrappedOp, PytorchNodeHierarchy
 from nobuco.trace.tensor_storage import clone_torch_tensors_recursively_with_cache, TensorStorage
 from nobuco.util import collect_recursively
 
 
 def traceable(func_to_trace: Callable):
     if Tracer.is_decorated(func_to_trace):
@@ -33,30 +34,31 @@
     ]
 
     op_blacklist = [
         torch.Tensor.__init__,
         torch.Tensor._make_subclass,
     ]
 
-    op_whitelist_dict = {
-        torch.Tensor: torch.Tensor.__setitem__
+    op_whitelist = {
+        (torch.Tensor, torch.Tensor.__setitem__),
     }
 
     _tracing_enabled = False
     _parent_list = []
     _node_list = []
 
     _tensor_storage: TensorStorage = None
+    _trace_shape = False
 
     @staticmethod
     def is_decorated(callable) -> bool:
         return hasattr(callable, '__undecorated_func__')
 
     @staticmethod
-    def op_unwrap(callable) -> bool:
+    def op_unwrap(callable: Callable) -> Callable:
         if Tracer.is_decorated(callable):
             return callable.__undecorated_func__
         else:
             return callable
 
     @staticmethod
     def are_equal(tensors1, tensors2):
@@ -105,42 +107,53 @@
 
     @staticmethod
     def op_tracing_decorator(orig_method, op_cls, module_suffix=None, is_whitelist_op=False):
 
         def decorator(*args, **kwargs):
             if Tracer._tracing_enabled:
                 Tracer._tracing_enabled = False
+                need_trace_deeper = True
 
-                wrapped_op = WrappedOp(orig_method)
+                call_method = orig_method
+                call_op_cls = op_cls
+
+                if Tracer._trace_shape:
+                    if orig_method == Tracer.op_unwrap(torch.Tensor.__getattribute__) and 'shape' in args:
+                        call_method = Tracer.op_unwrap(nobuco.shape)
+                        call_op_cls = nobuco
+                        args = args[:1]
+                        need_trace_deeper = False
+
+                wrapped_op = WrappedOp(call_method)
 
                 # Protection from external modification
                 args_clone, kwargs_clone = clone_torch_tensors_recursively_with_cache((args, kwargs), Tracer._tensor_storage)
 
                 # Inner function may change the input structure, ensure against that
                 args_inner, kwargs_inner = deepcopy((args, kwargs), memo={id(t): t for t in collect_recursively(args, torch.Tensor)})
 
                 num_input_tensors = len(collect_recursively((args, kwargs), torch.Tensor))
 
                 Tracer._parent_list.append(wrapped_op)
-                Tracer._tracing_enabled = True
-                outputs = orig_method(*args_inner, **kwargs_inner)
+                Tracer._tracing_enabled = need_trace_deeper
+                outputs = call_method(*args_inner, **kwargs_inner)
                 Tracer._tracing_enabled = False
                 Tracer._parent_list = Tracer._parent_list[:-1]
 
+                # __setitem__ method is sorta special
+                if orig_method == Tracer.op_unwrap(torch.Tensor.__setitem__):
+                    outputs = args[0]
+
                 num_output_tensors = len(collect_recursively(outputs, torch.Tensor))
 
                 if is_whitelist_op or (num_input_tensors > 0 and num_output_tensors > 0):
-                    module_name = op_cls.__name__ if isinstance(op_cls, types.ModuleType) else f'{op_cls.__module__}.{op_cls.__name__}'
+                    module_name = call_op_cls.__name__ if isinstance(call_op_cls, types.ModuleType) else f'{call_op_cls.__module__}.{call_op_cls.__name__}'
                     if module_suffix:
                         module_name += '.' + module_suffix
 
-                    # __setitem__ method is sorta special
-                    if '__setitem__' in str(orig_method):
-                        outputs = args[0]
-
                     # Protection from external modification
                     outputs_clone = clone_torch_tensors_recursively_with_cache(outputs, Tracer._tensor_storage)
                     is_inplace = not Tracer.are_equal((args, kwargs), (args_clone, kwargs_clone))
 
                     summary: traceback.FrameSummary = traceback.extract_stack()[-2]
                     node = PytorchNode(wrapped_op, module_name, Tracer._parent_list.copy(), None, args_clone, kwargs_clone, outputs_clone, is_inplace, summary)
                     Tracer._node_list.append(node)
@@ -182,21 +195,22 @@
     @staticmethod
     def decorate_ops():
         torch.jit._state.disable()
 
         for op_cls in Tracer.op_tracing_classes:
             Tracer.op_tracing_decorator_for_class(op_cls)
 
-        for op_cls, op in Tracer.op_whitelist_dict.items():
+        for op_cls, op in Tracer.op_whitelist:
             if not Tracer.is_decorated(op):
                 decorated = Tracer.op_tracing_decorator(op, op_cls, is_whitelist_op=True)
                 setattr(op_cls, op.__name__, decorated)
 
     @staticmethod
-    def trace(module_or_function: Union[nn.Module, Callable], args, kwargs) -> PytorchNodeHierarchy:
+    def trace(module_or_function: Union[nn.Module, Callable], trace_shape: bool, args, kwargs) -> PytorchNodeHierarchy:
+        Tracer._trace_shape = trace_shape
 
         ### Module tracing routines
         def apply_module_tracing_recursively(module):
             for child in module.children():
                 apply_module_tracing_recursively(child)
 
             if not Tracer.is_decorated(module.forward):
@@ -211,14 +225,15 @@
         Tracer._parent_list = []
         Tracer._tensor_storage = TensorStorage()
 
         if isinstance(module_or_function, nn.Module):
             apply_module_tracing_recursively(module_or_function)
         else:
             module_or_function = traceable(module_or_function)
+
         with torch.no_grad():
             module_or_function(*args, **kwargs)
 
         Tracer._tracing_enabled = False
 
         hierarchy = Tracer.build_hierarchy(Tracer._node_list)
         return hierarchy
```

### Comparing `nobuco-0.4.8/nobuco/util.py` & `nobuco-0.4.9/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/vis/console_stylizer.py` & `nobuco-0.4.9/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco/vis/html_stylizer.py` & `nobuco-0.4.9/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.8/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.9/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.8
+Version: 0.4.9
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.8/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.9/nobuco.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -43,13 +43,14 @@
 nobuco/node_converters/padding.py
 nobuco/node_converters/pooling.py
 nobuco/node_converters/recurrent.py
 nobuco/node_converters/slice.py
 nobuco/node_converters/tensor_cast.py
 nobuco/node_converters/tensor_creation.py
 nobuco/node_converters/tensor_manipulation.py
+nobuco/node_converters/tensor_shape.py
 nobuco/trace/__init__.py
 nobuco/trace/tensor_storage.py
 nobuco/trace/trace.py
 nobuco/vis/__init__.py
 nobuco/vis/console_stylizer.py
 nobuco/vis/html_stylizer.py
```

### Comparing `nobuco-0.4.8/pyproject.toml` & `nobuco-0.4.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.8"
+version = "0.4.9"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

