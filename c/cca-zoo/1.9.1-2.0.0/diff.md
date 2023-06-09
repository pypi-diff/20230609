# Comparing `tmp/cca_zoo-1.9.1.tar.gz` & `tmp/cca_zoo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cca_zoo-1.9.1.tar", last modified: Sun Nov  7 17:40:01 2021, max compression
+gzip compressed data, was "dist/cca_zoo-2.0.0.tar", last modified: Fri Jun  9 14:21:14 2023, max compression
```

## Comparing `cca_zoo-1.9.1.tar` & `cca_zoo-2.0.0.tar`

### file list

```diff
@@ -1,57 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5398 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/
--rw-r--r--   0 runner    (1001) docker     (121)      196 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/benchmarks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/data/
--rw-r--r--   0 runner    (1001) docker     (121)      233 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8360 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/simulated.py
--rw-r--r--   0 runner    (1001) docker     (121)     9341 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/toy.py
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/
--rw-r--r--   0 runner    (1001) docker     (121)      307 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      862 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/_dcca_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13982 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/architectures.py
--rw-r--r--   0 runner    (1001) docker     (121)     1917 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     3176 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dcca_noi.py
--rw-r--r--   0 runner    (1001) docker     (121)     2575 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dccae.py
--rw-r--r--   0 runner    (1001) docker     (121)    13897 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/deepwrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1399 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dtcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     5780 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/dvcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     9836 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/objectives.py
--rw-r--r--   0 runner    (1001) docker     (121)     1566 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/deepmodels/splitae.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/model_selection/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/model_selection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    43156 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/model_selection/_search.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/models/
--rw-r--r--   0 runner    (1001) docker     (121)      340 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7738 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/cca_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     9647 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/gcca.py
--rw-r--r--   0 runner    (1001) docker     (121)    29499 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/innerloop.py
--rw-r--r--   0 runner    (1001) docker     (121)    29327 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/iterative.py
--rw-r--r--   0 runner    (1001) docker     (121)     8899 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/mcca.py
--rw-r--r--   0 runner    (1001) docker     (121)     4885 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/ncca.py
--rw-r--r--   0 runner    (1001) docker     (121)     8478 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/rcca.py
--rw-r--r--   0 runner    (1001) docker     (121)    11527 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/models/tcca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/probabilisticmodels/
--rw-r--r--   0 runner    (1001) docker     (121)       33 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/probabilisticmodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3808 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/probabilisticmodels/vcca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)    15510 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/test_deepmodels.py
--rw-r--r--   0 runner    (1001) docker     (121)    11239 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/test/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2849 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/utils/check_values.py
--rw-r--r--   0 runner    (1001) docker     (121)     5263 2021-11-07 17:39:51.000000 cca_zoo-1.9.1/cca_zoo/utils/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6905 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      169 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/cca_zoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1118 2021-11-07 17:40:01.000000 cca_zoo-1.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/data/deep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/data/simulated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_barlow_twins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_noi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_sdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dtcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dccae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5321 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_splitae.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9283 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/architectures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8126 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/deepmodels/objectives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/model_selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/model_selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11669 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/model_selection/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18413 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/model_selection/_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7232 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_gcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_grcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_altmaxvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15917 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13747 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_elasticnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_ey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_gh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_gradkcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_incrementalpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_pls_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_pmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_admm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_hsic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_parkhomenko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_scca_span.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_stochasticpls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_svd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_iterative/_swcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12574 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_kcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_mcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_ncca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_partialcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_pcacca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6201 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_plsmixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_prcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10059 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_rcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/models/_tcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/plotting/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/probabilisticmodels/
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/probabilisticmodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/probabilisticmodels/_probabilisticcca.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11645 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_deepmodels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_probabilistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_regularised.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_stochastic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_unregularized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/cca_zoo/utils/check_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5296 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/cca_zoo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dcca_custom_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dcca_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_dvcca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_hyperparameter_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_kernel_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_many_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_sparse_cca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-06-09 14:21:03.000000 cca_zoo-2.0.0/examples/plot_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:21:14.000000 cca_zoo-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-09 14:21:13.000000 cca_zoo-2.0.0/setup.py
```

### Comparing `cca_zoo-1.9.1/cca_zoo/deepmodels/architectures.py` & `cca_zoo-2.0.0/cca_zoo/deepmodels/architectures.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,188 +1,176 @@
 from abc import abstractmethod
 from math import sqrt
-from typing import Iterable, Tuple
+from typing import Iterable
 
 import torch
-from torch.nn import functional as F
+from torch import nn
 
 
-class BaseEncoder(torch.nn.Module):
+class _BaseEncoder(torch.nn.Module):
     @abstractmethod
     def __init__(self, latent_dims: int, variational: bool = False):
-        super(BaseEncoder, self).__init__()
+        super(_BaseEncoder, self).__init__()
         self.variational = variational
         self.latent_dims = latent_dims
 
     @abstractmethod
     def forward(self, x):
         pass
 
 
-class BaseDecoder(torch.nn.Module):
+class _BaseDecoder(torch.nn.Module):
     @abstractmethod
     def __init__(self, latent_dims: int):
-        super(BaseDecoder, self).__init__()
+        super(_BaseDecoder, self).__init__()
         self.latent_dims = latent_dims
 
     @abstractmethod
     def forward(self, x):
         pass
 
 
-class Encoder(BaseEncoder):
+class Encoder(_BaseEncoder):
     def __init__(
-            self,
-            latent_dims: int,
-            variational: bool = False,
-            feature_size: int = 784,
-            layer_sizes: Iterable = None,
+        self,
+        latent_dims: int,
+        variational: bool = False,
+        feature_size: int = 784,
+        layer_sizes: tuple = None,
+        activation=nn.LeakyReLU(),
+        dropout=0,
     ):
         super(Encoder, self).__init__(latent_dims, variational=variational)
         if layer_sizes is None:
-            layer_sizes = [128]
+            layer_sizes = (128,)
+        layer_sizes = (feature_size,) + layer_sizes + (latent_dims,)
         layers = []
-
-        # first layer
-        layers.append(
-            torch.nn.Sequential(
-                torch.nn.Linear(feature_size, layer_sizes[0]), torch.nn.ReLU()
-            )
-        )
-
         # other layers
-        for l_id in range(len(layer_sizes) - 1):
+        for l_id in range(len(layer_sizes) - 2):
             layers.append(
                 torch.nn.Sequential(
+                    nn.Dropout(p=dropout),
                     torch.nn.Linear(layer_sizes[l_id], layer_sizes[l_id + 1]),
-                    torch.nn.ReLU(),
+                    activation,
                 )
             )
         self.layers = torch.nn.Sequential(*layers)
 
         if self.variational:
-            self.fc_mu = torch.nn.Linear(layer_sizes[-1], latent_dims)
-            self.fc_var = torch.nn.Linear(layer_sizes[-1], latent_dims)
+            self.fc_mu = torch.nn.Sequential(
+                nn.Dropout(p=dropout), torch.nn.Linear(layer_sizes[-2], layer_sizes[-1])
+            )
+            self.fc_var = torch.nn.Sequential(
+                nn.Dropout(p=dropout), torch.nn.Linear(layer_sizes[-2], layer_sizes[-1])
+            )
         else:
-            self.fc = torch.nn.Linear(layer_sizes[-1], latent_dims)
+            self.fc = torch.nn.Sequential(
+                nn.Dropout(p=dropout), torch.nn.Linear(layer_sizes[-2], layer_sizes[-1])
+            )
 
     def forward(self, x):
         x = self.layers(x)
         if self.variational:
             mu = self.fc_mu(x)
             logvar = self.fc_var(x)
             return mu, logvar
         else:
             x = self.fc(x)
             return x
 
 
-class Decoder(BaseDecoder):
+class Decoder(_BaseDecoder):
     def __init__(
-            self,
-            latent_dims: int,
-            feature_size: int = 784,
-            layer_sizes: list = None,
-            norm_output: bool = False,
+        self,
+        latent_dims: int,
+        feature_size: int = 784,
+        layer_sizes: tuple = None,
+        activation=nn.LeakyReLU(),
+        dropout=0,
     ):
         super(Decoder, self).__init__(latent_dims)
         if layer_sizes is None:
-            layer_sizes = [128]
+            layer_sizes = (128,)
+        layer_sizes = (latent_dims,) + layer_sizes + (feature_size,)
         layers = []
-
-        layers.append(
-            torch.nn.Sequential(
-                torch.nn.Linear(latent_dims, layer_sizes[0]), torch.nn.Sigmoid()
-            )
-        )
-
-        for l_id in range(len(layer_sizes)):
-            if l_id == len(layer_sizes) - 1:
-                if norm_output:
-                    layers.append(
-                        torch.nn.Sequential(
-                            torch.nn.Linear(layer_sizes[l_id], feature_size),
-                            torch.nn.Sigmoid(),
-                        )
-                    )
-                else:
-                    layers.append(
-                        torch.nn.Sequential(
-                            torch.nn.Linear(layer_sizes[l_id], feature_size),
-                        )
-                    )
-            else:
-                layers.append(
-                    torch.nn.Sequential(
-                        torch.nn.Linear(layer_sizes[l_id], layer_sizes[l_id + 1]),
-                        torch.nn.ReLU(),
-                    )
+        for l_id in range(len(layer_sizes) - 1):
+            layers.append(
+                torch.nn.Sequential(
+                    nn.Dropout(p=dropout),
+                    torch.nn.Linear(layer_sizes[l_id], layer_sizes[l_id + 1]),
+                    activation,
                 )
+            )
         self.layers = torch.nn.Sequential(*layers)
 
     def forward(self, x):
         x = self.layers(x)
         return x
 
 
-class CNNEncoder(BaseEncoder):
+class CNNEncoder(_BaseEncoder):
     def __init__(
-            self,
-            latent_dims: int,
-            variational: bool = False,
-            feature_size: Iterable = (28, 28),
-            channels: list = None,
-            kernel_sizes: list = None,
-            stride: list = None,
-            padding: list = None,
+        self,
+        latent_dims: int,
+        variational: bool = False,
+        feature_size: Iterable = (28, 28),
+        channels: tuple = None,
+        kernel_sizes: tuple = None,
+        stride: tuple = None,
+        padding: tuple = None,
+        activation=nn.LeakyReLU(),
+        dropout=0,
     ):
         super(CNNEncoder, self).__init__(latent_dims, variational=variational)
         if channels is None:
-            channels = [1, 1]
+            channels = (1, 1)
         if kernel_sizes is None:
-            kernel_sizes = [5] * (len(channels))
+            kernel_sizes = (5,) * (len(channels))
         if stride is None:
-            stride = [1] * (len(channels))
+            stride = (1,) * (len(channels))
         if padding is None:
-            padding = [2] * (len(channels))
+            padding = (2,) * (len(channels))
         # assume square input
         conv_layers = []
         current_size = feature_size[0]
         current_channels = 1
         for l_id in range(len(channels) - 1):
             conv_layers.append(
-                torch.nn.Sequential(  # input shape (1, current_size, current_size)
+                torch.nn.Sequential(
                     torch.nn.Conv2d(
                         in_channels=current_channels,  # input height
                         out_channels=channels[l_id],  # n_filters
                         kernel_size=kernel_sizes[l_id],  # filter size
                         stride=stride[l_id],  # filter movement/step
                         padding=padding[l_id],
                         # if want same width and length of this image after Conv2d, padding=(kernel_size-1)/2 if
                         # stride=1
                     ),  # output shape (out_channels, current_size, current_size)
-                    torch.nn.ReLU(),  # activation
+                    activation,  # activation
                 )
             )
             current_size = current_size
             current_channels = channels[l_id]
 
         if self.variational:
             self.fc_mu = torch.nn.Sequential(
+                nn.Dropout(p=dropout),
                 torch.nn.Linear(
                     int(current_size * current_size * current_channels), latent_dims
                 ),
             )
             self.fc_var = torch.nn.Sequential(
+                nn.Dropout(p=dropout),
                 torch.nn.Linear(
                     int(current_size * current_size * current_channels), latent_dims
                 ),
             )
         else:
             self.fc = torch.nn.Sequential(
+                nn.Dropout(p=dropout),
                 torch.nn.Linear(
                     int(current_size * current_size * current_channels), latent_dims
                 ),
             )
         self.conv_layers = torch.nn.Sequential(*conv_layers)
 
     def forward(self, x):
@@ -193,47 +181,40 @@
             logvar = self.fc_var(x)
             return mu, logvar
         else:
             x = self.fc(x)
             return x
 
 
-class CNNDecoder(BaseDecoder):
+class CNNDecoder(_BaseDecoder):
     def __init__(
-            self,
-            latent_dims: int,
-            feature_size: Iterable = (28, 28),
-            channels: list = None,
-            kernel_sizes=None,
-            strides=None,
-            paddings=None,
-            norm_output: bool = False,
+        self,
+        latent_dims: int,
+        feature_size: Iterable = (28, 28),
+        channels: tuple = None,
+        kernel_sizes=None,
+        strides=None,
+        paddings=None,
+        activation=nn.LeakyReLU(),
+        dropout=0,
     ):
         super(CNNDecoder, self).__init__(latent_dims)
         if channels is None:
-            channels = [1, 1]
+            channels = (1, 1)
         if kernel_sizes is None:
-            kernel_sizes = [5] * len(channels)
+            kernel_sizes = (5,) * len(channels)
         if strides is None:
-            strides = [1] * len(channels)
+            strides = (1,) * len(channels)
         if paddings is None:
-            paddings = [2] * len(channels)
-
-        if norm_output:
-            activation = torch.nn.Sigmoid()
-        else:
-            activation = torch.nn.ReLU()
-
+            paddings = (2,) * len(channels)
         conv_layers = []
         current_channels = 1
         current_size = feature_size[0]
-        # Loop backward through decoding layers in order to work out the dimensions at each layer - in particular the first
-        # linear layer needs to know B*current_size*current_size*channels
         for l_id, (channel, kernel, stride, padding) in reversed(
-                list(enumerate(zip(channels, kernel_sizes, strides, paddings)))
+            list(enumerate(zip(channels, kernel_sizes, strides, paddings)))
         ):
             conv_layers.append(
                 torch.nn.Sequential(
                     torch.nn.ConvTranspose2d(
                         in_channels=channel,  # input height
                         out_channels=current_channels,
                         kernel_size=kernel_sizes[l_id],
@@ -247,17 +228,19 @@
             )
             current_size = current_size
             current_channels = channel
 
         # reverse layers as constructed in reverse
         self.conv_layers = torch.nn.Sequential(*conv_layers[::-1])
         self.fc_layer = torch.nn.Sequential(
+            nn.Dropout(p=dropout),
             torch.nn.Linear(
                 latent_dims, int(current_size * current_size * current_channels)
             ),
+            activation,
         )
 
     def forward(self, x):
         x = self.fc_layer(x)
         x = x.reshape((x.shape[0], self.conv_layers[0][0].in_channels, -1))
         x = x.reshape(
             (
@@ -267,101 +250,15 @@
                 int(sqrt(x.shape[-1])),
             )
         )
         x = self.conv_layers(x)
         return x
 
 
-# https://github.com/nicofarr/brainnetcnnVis_pytorch/blob/master/BrainNetCnnGoldMSI.py
-class E2EBlock(torch.nn.Module):
-    def __init__(self, in_planes, planes, size, bias=False):
-        super(E2EBlock, self).__init__()
-        self.d = size
-        self.cnn1 = torch.nn.Conv2d(in_planes, planes, (1, self.d), bias=bias)
-        self.cnn2 = torch.nn.Conv2d(in_planes, planes, (self.d, 1), bias=bias)
-
-    def forward(self, x):
-        a = self.cnn1(x)
-        b = self.cnn2(x)
-        return torch.cat([a] * self.d, 3) + torch.cat([b] * self.d, 2)
-
-
-class E2EBlockReverse(torch.nn.Module):
-    def __init__(self, in_planes, planes, size, bias=False):
-        super(E2EBlockReverse, self).__init__()
-
-        self.d = size
-        self.cnn1 = torch.nn.ConvTranspose2d(in_planes, planes, (1, self.d), bias=bias)
-        self.cnn2 = torch.nn.ConvTranspose2d(in_planes, planes, (self.d, 1), bias=bias)
-
-    def forward(self, x):
-        a = self.cnn1(x)
-        b = self.cnn2(x)
-        return torch.cat([a] * self.d, 3) + torch.cat([b] * self.d, 2)
-
-
-# BrainNetCNN Network for fitting Gold-MSI on LSD dataset
-class BrainNetEncoder(BaseEncoder):
-    def __init__(
-            self,
-            latent_dims: int,
-            variational: bool = False,
-            feature_size: Tuple[int] = (200, ...),
-    ):
-        super(BrainNetEncoder, self).__init__(latent_dims, variational=variational)
-        _check_feature_size(feature_size)
-        self.d = feature_size[0]
-        self.e2econv1 = E2EBlock(1, 32, self.d, bias=True)
-        self.e2econv2 = E2EBlock(32, 64, self.d, bias=True)
-        self.E2N = torch.nn.Conv2d(64, 1, (1, self.d))
-        self.N2G = torch.nn.Conv2d(1, 256, (self.d, 1))
-        self.dense1 = torch.nn.Linear(256, 128)
-        self.dense2 = torch.nn.Linear(128, 30)
-        self.dense3 = torch.nn.Linear(30, latent_dims)
-
-    def forward(self, x):
-        out = F.leaky_relu(self.e2econv1(x), negative_slope=0.33)  # B,32,200,200
-        out = F.leaky_relu(self.e2econv2(out), negative_slope=0.33)  # B,64,200,200
-        out = F.leaky_relu(self.E2N(out), negative_slope=0.33)  # B,1,200,1
-        out = F.dropout(
-            F.leaky_relu(self.N2G(out), negative_slope=0.33), p=0.5
-        )  # B,256,1,1
-        out = out.view(out.shape[0], -1)  # B,256
-        out = F.dropout(F.leaky_relu(self.dense1(out), negative_slope=0.33), p=0.5)
-        out = F.dropout(F.leaky_relu(self.dense2(out), negative_slope=0.33), p=0.5)
-        out = F.leaky_relu(self.dense3(out), negative_slope=0.33)
-        return out
-
-
-class BrainNetDecoder(BaseDecoder):
-    def __init__(self, latent_dims: int, feature_size: Tuple[int] = (200, ...)):
-        super(BrainNetDecoder, self).__init__(latent_dims)
-        _check_feature_size(feature_size)
-        self.d = feature_size[0]
-        self.e2econv1 = E2EBlock(32, 1, self.d, bias=True)
-        self.e2econv2 = E2EBlock(64, 32, self.d, bias=True)
-        self.E2N = torch.nn.ConvTranspose2d(1, 64, (1, self.d))
-        self.N2G = torch.nn.ConvTranspose2d(256, 1, (self.d, 1))
-        self.dense1 = torch.nn.Linear(128, 256)
-        self.dense2 = torch.nn.Linear(30, 128)
-        self.dense3 = torch.nn.Linear(latent_dims, 30)
-
-    def forward(self, x):
-        out = F.dropout(F.leaky_relu(self.dense3(x), negative_slope=0.33), p=0.5)
-        out = F.dropout(F.leaky_relu(self.dense2(out), negative_slope=0.33), p=0.5)
-        out = F.leaky_relu(self.dense1(out), negative_slope=0.33)
-        out = out.view(out.size(0), out.size(1), 1, 1)
-        out = F.dropout(F.leaky_relu(self.N2G(out), negative_slope=0.33), p=0.5)
-        out = F.leaky_relu(self.E2N(out), negative_slope=0.33)
-        out = F.leaky_relu(self.e2econv2(out), negative_slope=0.33)
-        out = F.leaky_relu(self.e2econv1(out), negative_slope=0.33)
-        return out
-
-
-class LinearEncoder(BaseEncoder):
+class LinearEncoder(_BaseEncoder):
     def __init__(self, latent_dims: int, feature_size: int, variational: bool = False):
         super(LinearEncoder, self).__init__(latent_dims, variational=variational)
         self.variational = variational
 
         if self.variational:
             self.fc_mu = torch.nn.Linear(feature_size, latent_dims)
             self.fc_var = torch.nn.Linear(feature_size, latent_dims)
@@ -374,23 +271,15 @@
             logvar = self.fc_var(x)
             return mu, logvar
         else:
             x = self.fc(x)
             return x
 
 
-class LinearDecoder(BaseDecoder):
+class LinearDecoder(_BaseDecoder):
     def __init__(self, latent_dims: int, feature_size: int):
         super(LinearDecoder, self).__init__(latent_dims)
         self.linear = torch.nn.Linear(latent_dims, feature_size)
 
     def forward(self, x):
         out = self.linear(x)
         return out
-
-
-def _check_feature_size(feature_size):
-    if feature_size[0] != feature_size[1]:
-        raise ValueError(
-            "BrainNetCNN requires a pair of feature_size of the"
-            f"same value. feature_size={feature_size}."
-        )
```

### Comparing `cca_zoo-1.9.1/cca_zoo/deepmodels/dcca.py` & `cca_zoo-2.0.0/cca_zoo/deepmodels/_discriminative/_dcca_sdl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,82 @@
 import torch
+import torch.nn.functional as F
 
-from cca_zoo.deepmodels import objectives
-from cca_zoo.deepmodels.architectures import Encoder
-from cca_zoo.models import MCCA
-from ._dcca_base import _DCCA_base
+from ._dcca_noi import DCCA_NOI
 
 
-class DCCA(_DCCA_base):
+class DCCA_SDL(DCCA_NOI):
     """
-    A class used to fit a DCCA model.
+    A class used to fit a Deep CCA by Stochastic Decorrelation model.
+
+    References
+    ----------
+    Chang, Xiaobin, Tao Xiang, and Timothy M. Hospedales. "Scalable and effective deep CCA via soft decorrelation." Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition. 2018.
 
-    Examples
-    --------
-    >>> from cca_zoo.deepmodels import DCCA
-    >>> model = DCCA()
     """
 
     def __init__(
-            self,
-            latent_dims: int,
-            objective=objectives.MCCA,
-            encoders=None,
-            r: float = 0,
-            eps: float = 1e-3,
+        self,
+        latent_dims: int,
+        N: int,
+        encoders=None,
+        r: float = 0,
+        rho: float = 0.2,
+        eps: float = 1e-5,
+        shared_target: bool = False,
+        lam=0.5,
+        **kwargs
     ):
-        """
-        Constructor class for DCCA
-
-        :param latent_dims: # latent dimensions
-        :param objective: # CCA objective: normal tracenorm CCA by default
-        :param encoders: list of encoder networks
-        :param r: regularisation parameter of tracenorm CCA like ridge CCA. Needs to be VERY SMALL. If you get errors make this smaller
-        :param eps: epsilon used throughout. Needs to be VERY SMALL. If you get errors make this smaller
-        """
-        super().__init__(latent_dims=latent_dims)
-        if encoders is None:
-            encoders = [Encoder, Encoder]
-        self.encoders = torch.nn.ModuleList(encoders)
-        self.objective = objective(latent_dims, r=r, eps=eps)
+        super().__init__(
+            latent_dims=latent_dims,
+            N=N,
+            encoders=encoders,
+            r=r,
+            rho=rho,
+            eps=eps,
+            shared_target=shared_target,
+            **kwargs
+        )
+        self.c = None
+        self.cross_cov = None
+        self.lam = lam
+        self.bns = torch.nn.ModuleList(
+            [torch.nn.BatchNorm1d(latent_dims, affine=False) for _ in self.encoders]
+        )
 
-    def forward(self, *args):
+    def forward(self, views, **kwargs):
         z = []
-        for i, encoder in enumerate(self.encoders):
-            z.append(encoder(args[i]))
+        for i, (encoder, bn) in enumerate(zip(self.encoders, self.bns)):
+            z.append(bn(encoder(views[i])))
         return z
 
-    def loss(self, *args):
-        """
-        Define the loss function for the model. This is used by the DeepWrapper class
-
-        :param args:
-        :return:
-        """
-        z = self(*args)
-        return self.objective.loss(*z)
-
-    def post_transform(self, *z_list, train=False):
+    def loss(self, views, **kwargs):
+        z = self(views)
+        l2_loss = F.mse_loss(z[0], z[1])
+        self._update_covariances(z, train=self.training)
+        SDL_loss = self._sdl_loss(self.covs)
+        loss = l2_loss + self.lam * SDL_loss
+        self.covs = [cov.detach() for cov in self.covs]
+        return {"objective": loss, "l2": l2_loss, "sdl": SDL_loss}
+
+    def _sdl_loss(self, covs):
+        loss = 0
+        for cov in covs:
+            sgn = torch.sign(cov)
+            sgn.fill_diagonal_(0)
+            loss += torch.mean(cov * sgn)
+        return loss
+
+    def _update_covariances(self, z, train=True):
+        b = z[0].shape[0]
+        batch_covs = [self.N * z_.T @ z_ / b for z_ in z]
         if train:
-            self.cca = MCCA(latent_dims=self.latent_dims)
-            z_list = self.cca.fit_transform(z_list)
-        else:
-            z_list = self.cca.transform(z_list)
-        return z_list
+            if self.covs is not None:
+                self.covs = [
+                    self.rho * self.covs[i] + (1 - self.rho) * batch_cov
+                    for i, batch_cov in enumerate(batch_covs)
+                ]
+            else:
+                self.covs = batch_covs
+        # pytorch-lightning runs validation once so this just fixes the bug
+        elif self.covs is None:
+            self.covs = batch_covs
```

### Comparing `cca_zoo-1.9.1/cca_zoo/deepmodels/dcca_noi.py` & `cca_zoo-2.0.0/cca_zoo/models/_gcca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,94 +1,111 @@
-import torch
+from typing import Iterable, Union
 
-from cca_zoo.deepmodels import objectives
-from cca_zoo.deepmodels.dcca import DCCA
+import numpy as np
 
+from cca_zoo.models._mcca import MCCA
+from cca_zoo.utils.check_values import _process_parameter
+
+
+class GCCA(MCCA):
+    r"""
+    A class used to fit GCCA model. This model extends CCA to more than two views by optimizing the sum of correlations with a shared auxiliary vector.
+
+    The objective function of GCCA is:
+
+    .. math::
+
+        w_{opt}=\underset{w}{\mathrm{argmax}}\{ \sum_iw_i^TX_i^TT  \}\\
+
+        \text{subject to:}
+
+        T^TT=1
+
+    where :math:`T` is the auxiliary vector.
 
-class DCCA_NOI(DCCA):
-    """
-    A class used to fit a DCCA model by non-linear orthogonal iterations
 
+    References
+    ----------
+    Tenenhaus, Arthur, and Michel Tenenhaus. "Regularized generalized canonical correlation analysis." Psychometrika 76.2 (2011): 257.
+
+    Examples
+    --------
+    >>> from cca_zoo.models import GCCA
+    >>> import numpy as np
+    >>> rng=np.random.RandomState(0)
+    >>> X1 = rng.random((10,5))
+    >>> X2 = rng.random((10,5))
+    >>> X3 = rng.random((10,5))
+    >>> model = GCCA()
+    >>> model.fit((X1,X2,X3)).score((X1,X2,X3))
+    array([0.97229856])
     """
 
     def __init__(
-            self,
-            latent_dims: int,
-            N: int,
-            encoders=None,
-            r: float = 0,
-            rho: float = 0.2,
-            eps: float = 1e-3,
-            shared_target: bool = False,
+        self,
+        latent_dims: int = 1,
+        copy_data=True,
+        random_state=None,
+        c: Union[Iterable[float], float] = None,
+        view_weights: Iterable[float] = None,
+        eps: float = 1e-6,
     ):
-        """
-        Constructor class for DCCA
+        super().__init__(
+            latent_dims=latent_dims,
+            copy_data=copy_data,
+            accept_sparse=["csc", "csr"],
+            random_state=random_state,
+            c=c,
+            eps=eps,
+            pca=False,
+        )
+        self.view_weights = view_weights
 
-        :param latent_dims: # latent dimensions
-        :param N: # samples used to estimate covariance
-        :param encoders: list of encoder networks
-        :param r: regularisation parameter of tracenorm CCA like ridge CCA
-        :param rho: covariance memory like DCCA non-linear orthogonal iterations paper
-        :param eps: epsilon used throughout
-        :param shared_target: not used
+    def fit(self, views: Iterable[np.ndarray], y=None, K=None, **kwargs):
         """
-        super().__init__(latent_dims=latent_dims, encoders=encoders, r=r, eps=eps)
-        self.N = N
-        self.covs = None
-        if rho < 0 or rho > 1:
-            raise ValueError(f"rho should be between 0 and 1. rho={rho}")
-        self.eps = eps
-        self.rho = rho
-        self.shared_target = shared_target
-        self.mse = torch.nn.MSELoss()
-        # Authors state that a final linear layer is an important part of their algorithmic implementation
-        self.linear_layers = torch.nn.ModuleList(
-            [
-                torch.nn.Linear(latent_dims, latent_dims, bias=False)
-                for _ in range(len(encoders))
-            ]
+        Parameters
+        ----------
+        views : Iterable[np.ndarray]
+            Views to fit the model with.
+        y : None
+            Not used in this model.
+        K : None
+            Observation matrix
+        """
+        return super().fit(views, y=y, K=K, **kwargs)
+
+    def _check_params(self):
+        self.c = _process_parameter("c", self.c, 0, self.n_views_)
+
+    def C(self, views, K=None):
+        if K is None:
+            # just use identity when all rows are observed in all views.
+            K = np.ones((len(views), views[0].shape[0]))
+        Q = []
+        self.view_weights = _process_parameter(
+            "view_weights", self.view_weights, 1, self.n_views_
+        )
+        for i, (view, view_weight) in enumerate(zip(views, self.view_weights)):
+            view_cov = (1 - self.c[i]) * np.cov(view, rowvar=False) + self.c[
+                i
+            ] * np.eye(view.shape[1])
+            smallest_eig = min(0, np.linalg.eigvalsh(view_cov).min()) - self.eps
+            view_cov = view_cov - smallest_eig * np.eye(view_cov.shape[0])
+            Q.append(view_weight * view @ np.linalg.inv(view_cov) @ view.T)
+        Q = np.sum(Q, axis=0)
+        Q = (
+            np.diag(np.sqrt(np.sum(K, axis=0)))
+            @ Q
+            @ np.diag(np.sqrt(np.sum(K, axis=0)))
         )
-        self.rand = torch.rand(N, self.latent_dims)
+        return Q
 
-    def forward(self, *args):
-        z = []
-        # Users architecture + final linear layer
-        for i, (encoder, linear_layer) in enumerate(
-                zip(self.encoders, self.linear_layers)
-        ):
-            z.append(linear_layer(encoder(args[i])))
-        return z
-
-    def loss(self, *args):
-        z = self(*args)
-        z_copy = [z_.detach().clone() for z_ in z]
-        self.update_covariances(*z_copy)
-        covariance_inv = [
-            torch.linalg.inv(objectives.MatrixSquareRoot.apply(cov))
-            for cov in self.covs
+    def D(self, views, **kwargs):
+        return None
+
+    def _weights(self, eigvals, eigvecs, views, **kwargs):
+        self.weights = [
+            np.linalg.pinv(view) @ eigvecs[:, : self.latent_dims] for view in views
         ]
-        preds = [z_ @ covariance_inv[i] for i, z_ in enumerate(z_copy)]
-        loss = self.mse(z[0], preds[1]) + self.mse(z[1], preds[0])
-        return loss
-
-    def update_mean(self, *z):
-        batch_means = [torch.mean(z_, dim=0) for z_ in z]
-        if self.means is not None:
-            self.means = [
-                self.rho * self.means[i].detach() + (1 - self.rho) * batch_mean
-                for i, batch_mean in enumerate(batch_means)
-            ]
-        else:
-            self.means = batch_means
-        z = [z_ - mean for (z_, mean) in zip(z, self.means)]
-        return z
-
-    def update_covariances(self, *z):
-        b = z[0].shape[0]
-        batch_covs = [self.N * z_.T @ z_ / b for z_ in z]
-        if self.covs is not None:
-            self.covs = [
-                self.rho * self.covs[i] + (1 - self.rho) * batch_cov
-                for i, batch_cov in enumerate(batch_covs)
-            ]
-        else:
-            self.covs = batch_covs
+
+    def _more_tags(self):
+        return {"multiview": True}
```

### Comparing `cca_zoo-1.9.1/cca_zoo/deepmodels/dccae.py` & `cca_zoo-2.0.0/cca_zoo/deepmodels/_generative/_dccae.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,78 +1,86 @@
 import torch
-from torch.nn import functional as F
 
-from cca_zoo.deepmodels import objectives
-from cca_zoo.deepmodels.architectures import Encoder, Decoder
-from cca_zoo.deepmodels.dcca import _DCCA_base
+from .. import objectives
+from .._discriminative._dcca import DCCA
+from .._generative._base import _GenerativeMixin
 
 
-class DCCAE(_DCCA_base):
+class DCCAE(DCCA, _GenerativeMixin):
     """
     A class used to fit a DCCAE model.
 
-    Examples
-    --------
-    >>> from cca_zoo.deepmodels import DCCAE
-    >>> model = DCCAE()
+    References
+    ----------
+    Wang, Weiran, et al. "On deep multi-view representation learning." International conference on machine learning. PMLR, 2015.
+
     """
 
     def __init__(
-            self,
-            latent_dims: int,
-            objective=objectives.MCCA,
-            encoders=None,
-            decoders=None,
-            r: float = 0,
-            eps: float = 1e-3,
-            lam=0.5,
+        self,
+        latent_dims: int,
+        objective=objectives.MCCA,
+        encoders=None,
+        decoders=None,
+        r: float = 0,
+        eps: float = 1e-5,
+        lam=0.5,
+        latent_dropout=0,
+        img_dim=None,
+        recon_loss_type="mse",
+        **kwargs,
     ):
-        """
-        :param latent_dims: # latent dimensions
-        :param objective: # CCA objective: normal tracenorm CCA by default
-        :param encoders: list of encoder networks
-        :param decoders:  list of decoder networks
-        :param r: regularisation parameter of tracenorm CCA like ridge CCA. Needs to be VERY SMALL. If you get errors make this smaller
-        :param eps: epsilon used throughout. Needs to be VERY SMALL. If you get errors make this smaller
-        :param lam: weight of reconstruction loss (1 minus weight of correlation loss)
-        """
-        super().__init__(latent_dims=latent_dims)
-        if decoders is None:
-            decoders = [Decoder, Decoder]
-        if encoders is None:
-            encoders = [Encoder, Encoder]
-        self.encoders = torch.nn.ModuleList(encoders)
+        super().__init__(
+            latent_dims=latent_dims,
+            objective=objective,
+            encoders=encoders,
+            r=r,
+            eps=eps,
+            **kwargs,
+        )
+        self.img_dim = img_dim
         self.decoders = torch.nn.ModuleList(decoders)
         if lam < 0 or lam > 1:
             raise ValueError(f"lam should be between 0 and 1. rho={lam}")
         self.lam = lam
         self.objective = objective(latent_dims, r=r, eps=eps)
+        self.latent_dropout = torch.nn.Dropout(p=latent_dropout)
+        self.recon_loss_type = recon_loss_type
 
-    def forward(self, *args):
+    def forward(self, views, **kwargs):
+        """
+        Forward method for the model. Outputs latent encoding for each view
+
+        :param views:
+        :param kwargs:
+        :return:
+        """
         z = []
         for i, encoder in enumerate(self.encoders):
-            z.append(encoder(args[i]))
+            z.append(encoder(views[i]))
         return z
 
-    def decode(self, *z):
+    def _decode(self, z, **kwargs):
         """
         This method is used to decode from the latent space to the best prediction of the original views
 
-        :param args:
         """
         recon = []
         for i, decoder in enumerate(self.decoders):
-            recon.append(decoder(z[i]))
+            recon.append(decoder(self.latent_dropout(z[i])))
         return recon
 
-    def loss(self, *args):
-        z = self(*args)
-        recon = self.decode(*z)
-        recon_loss = self.recon_loss(args[: len(recon)], recon)
-        return self.lam * recon_loss + self.objective.loss(*z)
-
-    @staticmethod
-    def recon_loss(x, recon):
-        recons = [
-            F.mse_loss(recon_, x_, reduction="mean") for recon_, x_ in zip(recon, x)
-        ]
-        return torch.stack(recons).sum(dim=0)
+    def loss(self, views, **kwargs):
+        z = self(views)
+        recons = self._decode(z)
+        loss = dict()
+        loss["reconstruction"] = torch.stack(
+            [
+                self.recon_loss(x, recon, loss_type=self.recon_loss_type)
+                for x, recon in zip(views, recons)
+            ]
+        ).sum()
+        loss["correlation"] = self.objective.loss(z)
+        loss["objective"] = (
+            self.lam * loss["reconstruction"] + (1 - self.lam) * loss["correlation"]
+        )
+        return loss
```

### Comparing `cca_zoo-1.9.1/cca_zoo/deepmodels/objectives.py` & `cca_zoo-2.0.0/cca_zoo/deepmodels/objectives.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,22 @@
-import numpy as np
-import scipy.linalg
 import tensorly as tl
 import torch
 from tensorly.cp_tensor import cp_to_tensor
 from tensorly.decomposition import parafac
-from torch.autograd import Function
 
 
-class MatrixSquareRoot(Function):
-    """Square root of a positive definite matrix.
-    NOTE: matrix square root is not differentiable for matrices with
-          zero eigenvalues.
-    """
-
-    @staticmethod
-    def forward(ctx, input):
-        m = input.detach().cpu().numpy().astype(np.float_)
-        sqrtm = torch.from_numpy(scipy.linalg.sqrtm(m).real).to(input)
-        ctx.save_for_backward(sqrtm)
-        return sqrtm
-
-    @staticmethod
-    def backward(ctx, grad_output):
-        grad_input = None
-        if ctx.needs_input_grad[0]:
-            (sqrtm,) = ctx.saved_tensors
-            sqrtm = sqrtm.data.cpu().numpy().astype(np.float_)
-            gm = grad_output.data.cpu().numpy().astype(np.float_)
-
-            # Given a positive semi-definite matrix X,
-            # since X = X^{1/2}X^{1/2}, we can compute the gradient of the
-            # matrix square root dX^{1/2} by solving the Sylvester equation:
-            # dX = (d(X^{1/2})X^{1/2} + X^{1/2}(dX^{1/2}).
-            grad_sqrtm = scipy.linalg.solve_sylvester(sqrtm, sqrtm, gm)
-
-            grad_input = torch.from_numpy(grad_sqrtm).to(grad_output)
-        return grad_input
-
-
-def _minimal_regularisation(M, eps):
-    M_smallest_eig = torch.relu(-torch.min(torch.linalg.eigvalsh(M))) + eps
-    M = M + M_smallest_eig * torch.eye(M.shape[0], device=M.device)
-    return M
+def _mat_pow(mat, pow_, epsilon):
+    # Computing matrix to the power of pow (pow can be negative as well)
+    [D, V] = torch.linalg.eigh(mat)
+    mat_pow = V @ torch.diag((D + epsilon).pow(pow_)) @ V.T
+    mat_pow[mat_pow != mat_pow] = epsilon  # For stability
+    return mat_pow
 
 
-def _demean(*views):
+def _demean(views):
     return tuple([view - view.mean(dim=0) for view in views])
 
 
 class MCCA:
     """
 
     Differentiable MCCA Loss.
@@ -65,37 +33,34 @@
         the number of latent dimensions
         :param eps: an epsilon parameter used in some operations
         """
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, *views):
+    def loss(self, views):
         # Subtract the mean from each output
-        views = _demean(*views)
+        views = _demean(views)
 
         # Concatenate all views and from this get the cross-covariance matrix
         all_views = torch.cat(views, dim=1)
-        C = all_views.T @ all_views
+        C = torch.cov(all_views.T)
 
         # Get the block covariance matrix placing Xi^TX_i on the diagonal
         D = torch.block_diag(
             *[
-                (1 - self.r) * m.T @ m + self.r * torch.eye(m.shape[1], device=m.device)
-                for i, m in enumerate(views)
+                (1 - self.r) * torch.cov(view.T)
+                + self.r * torch.eye(view.shape[1], device=view.device)
+                for i, view in enumerate(views)
             ]
         )
 
-        C = C - torch.block_diag(*[view.T @ view for view in views]) + D
+        C = C - torch.block_diag(*[torch.cov(view.T) for view in views]) + D
 
-        D = _minimal_regularisation(D, self.eps)
-
-        R = torch.linalg.inv(
-            MatrixSquareRoot.apply(_minimal_regularisation(D, self.eps))
-        )
+        R = _mat_pow(D, -0.5, self.eps)
 
         # In MCCA our eigenvalue problem Cv = lambda Dv
         C_whitened = R @ C @ R.T
 
         eigvals = torch.linalg.eigvalsh(C_whitened)
 
         # Sort eigenvalues so lviewest first
@@ -128,24 +93,22 @@
         the number of latent dimensions
         :param eps: an epsilon parameter used in some operations
         """
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, *views):
+    def loss(self, views):
         # https: // www.uta.edu / math / _docs / preprint / 2014 / rep2014_04.pdf
+
         # H is n_views * n_samples * k
-        views = _demean(*views)
+        views = _demean(views)
 
         eigen_views = [
-            view
-            @ torch.inverse(_minimal_regularisation(view.T @ view, self.eps))
-            @ view.T
-            for view in views
+            view @ _mat_pow(torch.cov(view.T), -1, self.eps) @ view.T for view in views
         ]
 
         Q = torch.stack(eigen_views, dim=0).sum(dim=0)
         eigvals = torch.linalg.eigvalsh(Q)
 
         idx = torch.argsort(eigvals, descending=True)
 
@@ -166,14 +129,15 @@
 # Permission is hereby granted, free of chviewe, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"),
 # to deal in the Software without restriction, including without limitation
 # the rights to use, copy, modify, merge, publish, distribute, sublicense,
 # and/or sell copies of the Software, and to permit persons to whom the
 # Software is furnished to do so, subject to the following conditions:
 
+
 # The above copyright notice and this permission notice shall be included in
 # all copies or substantial portions of the Software.
 class CCA:
     """
     Differentiable CCA Loss.
     Loss() method takes the outputs of each view's network and solves the CCA problem as in Andrew's original paper
 
@@ -185,37 +149,35 @@
         :param r: regularisation as in regularized CCA. Makes the problem well posed when batch size is similar to the number of latent dimensions
         :param eps: an epsilon parameter used in some operations
         """
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, H1, H2):
-        o1 = H1.shape[1]
-        o2 = H2.shape[1]
-
-        n = H1.shape[0]
-
-        H1bar, H2bar = _demean(H1, H2)
-
-        SigmaHat12 = (1.0 / (n - 1)) * H1bar.T @ H2bar
-        SigmaHat11 = (1 - self.r) * (
-                1.0 / (n - 1)
-        ) * H1bar.T @ H1bar + self.r * torch.eye(o1, device=H1.device)
-        SigmaHat22 = (1 - self.r) * (
-                1.0 / (n - 1)
-        ) * H2bar.T @ H2bar + self.r * torch.eye(o2, device=H2.device)
-
-        SigmaHat11RootInv = torch.linalg.inv(
-            MatrixSquareRoot.apply(_minimal_regularisation(SigmaHat11, self.eps))
+    def loss(self, views):
+        o1 = views[0].shape[1]
+        o2 = views[1].shape[1]
+
+        n = views[0].shape[0]
+
+        views = _demean(views)
+
+        SigmaHat12 = torch.cov(torch.hstack((views[0], views[1])).T)[
+            : self.latent_dims, self.latent_dims :
+        ]  # views[0].T @ views[1] / (n - 1)
+        SigmaHat11 = torch.cov(views[0].T) + self.r * torch.eye(
+            o1, device=views[0].device
         )
-        SigmaHat22RootInv = torch.linalg.inv(
-            MatrixSquareRoot.apply(_minimal_regularisation(SigmaHat22, self.eps))
+        SigmaHat22 = torch.cov(views[1].T) + self.r * torch.eye(
+            o2, device=views[1].device
         )
 
+        SigmaHat11RootInv = _mat_pow(SigmaHat11, -0.5, self.eps)
+        SigmaHat22RootInv = _mat_pow(SigmaHat22, -0.5, self.eps)
+
         Tval = SigmaHat11RootInv @ SigmaHat12 @ SigmaHat22RootInv
         trace_TT = Tval.T @ Tval
         eigvals = torch.linalg.eigvalsh(trace_TT)
 
         # leaky relu encourages the gradient to be driven by positively correlated dimensions while also encouraging
         # dimensions associated with spurious negative correlations to become more positive
         eigvals = eigvals[torch.gt(eigvals, self.eps)]
@@ -227,39 +189,28 @@
 
 class TCCA:
     """
     Differentiable TCCA Loss.
 
     """
 
-    def __init__(self, latent_dims: int, r: float = 0, eps: float = 1e-3):
-        """
-
-        :param latent_dims: the number of latent dimensions
-        :param r: regularisation as in regularized CCA. Makes the problem well posed when batch size is similar to the number of latent dimensions
-        :param eps: an epsilon parameter used in some operations
-        """
+    def __init__(self, latent_dims: int, r: float = 0, eps: float = 1e-4):
         self.latent_dims = latent_dims
         self.r = r
         self.eps = eps
 
-    def loss(self, *z):
-        m = z[0].size(0)
-        z = [z_ - z_.mean(dim=0).unsqueeze(dim=0) for z_ in z]
+    def loss(self, views):
+        views = _demean(views)
         covs = [
-            (1 - self.r) * (1.0 / (m - 1)) * z_.T @ z_
-            + self.r * torch.eye(z_.size(1), device=z_.device)
-            for z_ in z
+            (1 - self.r) * torch.cov(view.T)
+            + self.r * torch.eye(view.size(1), device=view.device)
+            for view in views
         ]
         whitened_z = [
-            z_
-            @ torch.linalg.inv(
-                MatrixSquareRoot.apply(_minimal_regularisation(cov, self.eps))
-            )
-            for z_, cov in zip(z, covs)
+            view @ _mat_pow(cov, -0.5, self.eps) for view, cov in zip(views, covs)
         ]
         # The idea here is to form a matrix with M dimensions one for each view where at index
         # M[p_i,p_j,p_k...] we have the sum over n samples of the product of the pth feature of the
         # ith, jth, kth view etc.
         for i, el in enumerate(whitened_z):
             # To achieve this we start with the first view so M is nxp.
             if i == 0:
@@ -269,10 +220,13 @@
                 for _ in range(len(M.size()) - 1):
                     el = torch.unsqueeze(el, 1)
                 # Then we perform an outer product by expanding the dimensionality of M and
                 # outer product with the expanded el
                 M = torch.unsqueeze(M, -1) @ el
         M = torch.mean(M, 0)
         tl.set_backend("pytorch")
-        M_parafac = parafac(M.detach(), self.latent_dims)
+        M_parafac = parafac(
+            M.detach(), self.latent_dims, verbose=False, normalize_factors=True
+        )
+        M_parafac.weights = 1
         M_hat = cp_to_tensor(M_parafac)
-        return torch.norm(M - M_hat)
+        return torch.linalg.norm(M - M_hat)
```

### Comparing `cca_zoo-1.9.1/cca_zoo/models/ncca.py` & `cca_zoo-2.0.0/cca_zoo/probabilisticmodels/_probabilisticcca.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,111 +1,121 @@
-from typing import Union, Iterable
+from typing import Iterable
 
+import jax.numpy as jnp
 import numpy as np
-from sklearn.metrics import pairwise_kernels
-from sklearn.neighbors import NearestNeighbors
+import numpyro
+import numpyro.distributions as dist
+from jax.random import PRNGKey
+from numpyro.infer import MCMC, NUTS, Predictive
 from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models.cca_base import _CCA_Base
-from cca_zoo.utils.check_values import _process_parameter, check_views
+from cca_zoo.models._base import BaseModel
 
 
-class NCCA(_CCA_Base):
+class ProbabilisticCCA(BaseModel):
     """
-    A class used to fit nonparametric (NCCA) model.
+    A class used to fit a Probabilistic CCA. Not quite the same due to using VI methods rather than EM
+
+    Parameters
+    ----------
+    latent_dims : int, optional
+        Number of latent dimensions to use, by default 1
+    copy_data : bool, optional
+        Whether to copy the data, by default True
+    random_state : int, optional
+        Random state, by default 0
+    num_samples : int, optional
+        Number of samples to use in VI, by default 100
+    num_warmup : int, optional
+        Number of warmup samples to use in VI, by default 100
+
+
+    References
+    ----------
+    Bach, Francis R., and Michael I. Jordan. "A probabilistic interpretation of canonical correlation analysis." (2005).
+    Wang, Chong. "Variational Bayesian approach to canonical correlation analysis." IEEE Transactions on Neural Networks 18.3 (2007): 905-910.
 
-    Citation
-    --------
-    Michaeli, Tomer, Weiran Wang, and Karen Livescu. "Nonparametric canonical correlation analysis." International conference on machine learning. PMLR, 2016.
-
-    :Example:
-    >>> from cca_zoo.experimental import NCCA
-    >>> X1 = np.random.rand(10,5)
-    >>> X2 = np.random.rand(10,5)
-    >>> model = NCCA()
-    >>> model.fit([X1,X2])
     """
 
-    def __init__(self, latent_dims: int = 1, scale=True, centre=True, copy_data=True, accept_sparse=False,
-                 random_state: Union[int, np.random.RandomState] = None, nearest_neighbors=None,
-                 gamma: Iterable[float] = None,
-                 ):
-        """
-        Constructor for NCCA
+    def __init__(
+        self,
+        latent_dims: int = 1,
+        copy_data=True,
+        random_state: int = 0,
+        num_samples=100,
+        num_warmup=100,
+    ):
+        super().__init__(
+            latent_dims=latent_dims,
+            copy_data=copy_data,
+            accept_sparse=False,
+            random_state=random_state,
+        )
+        self.num_samples = num_samples
+        self.num_warmup = num_warmup
+        self.rng_key = PRNGKey(random_state)
 
-        :param latent_dims: number of latent dimensions to fit
-        :param scale: normalize variance in each column before fitting
-        :param centre: demean data by column before fitting (and before transforming out of sample
-        :param copy_data: If True, X will be copied; else, it may be overwritten
-        :param accept_sparse: Whether model can take sparse data as input
-        :param random_state: Pass for reproducible output across multiple function calls
-        :param nearest_neighbors: Number of nearest neighbors (l2 distance) to consider when constructing affinity
-        :param gamma: Bandwidth parameter for rbf kernel
+    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
         """
-        super().__init__(latent_dims, scale, centre, copy_data, accept_sparse, random_state)
-        self.nearest_neighbors = nearest_neighbors
-        self.gamma = gamma
-
-    def _check_params(self):
-        self.nearest_neighbors = _process_parameter("nearest_neighbors", self.nearest_neighbors, 1, self.n_views)
-        self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views)
-        self.kernel = _process_parameter("kernel", None, "rbf", self.n_views)
+        Infer the parameters (mu: mean, psi: within view variance) and latent variables (z) of the generative CCA model
 
-    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        views = check_views(
-            *views, copy=self.copy_data, accept_sparse=self.accept_sparse
+        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
+        """
+        nuts_kernel = NUTS(self._model)
+        self.mcmc = MCMC(
+            nuts_kernel, num_samples=self.num_samples, num_warmup=self.num_warmup
         )
-        views = self._centre_scale(views)
-        self.n_views = len(views)
-        self.n = views[0].shape[0]
-        self._check_params()
-        self.train_views = views
-        self.KNs = [NearestNeighbors(n_neighbors=self.nearest_neighbors[i]).fit(view) for i, view in
-                    enumerate(views)]
-        NNs = [self.KNs[i].kneighbors(view, self.nearest_neighbors[i]) for i, view in enumerate(views)]
-        kernels = [self._get_kernel(i, view) for i, view in enumerate(self.train_views)]
-        self.Ws = [fill_W(kernel, inds) for kernel, (dists, inds) in zip(kernels, NNs)]
-        self.Ws = [self.Ws[0] / self.Ws[0].sum(axis=1, keepdims=True),
-                   self.Ws[1] / self.Ws[1].sum(axis=0, keepdims=True)]
-        S = self.Ws[0] @ self.Ws[1]
-        U, S, Vt = np.linalg.svd(S)
-        self.f = U[:, 1:self.latent_dims + 1] * np.sqrt(self.n)
-        self.g = Vt[1:self.latent_dims + 1, :].T * np.sqrt(self.n)
-        self.S = S[1:self.latent_dims + 1]
+        self.mcmc.run(self.rng_key, views)
+        self.posterior_samples = self.mcmc.get_samples()
         return self
 
     def transform(self, views: Iterable[np.ndarray], y=None, **kwargs):
         """
-        Transforms data given a fit model
+        Predict the latent variables that generate the data in views using the sampled model parameters
 
-        :param views: numpy arrays with the same number of rows (samples) separated by commas
-        :param kwargs: any additional keyword arguments required by the given model
+        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
         """
-        check_is_fitted(self, attributes=["U", "V", "f", "g"])
-        views = check_views(
-            *views, copy=self.copy_data, accept_sparse=self.accept_sparse
-        )
-        views = self._centre_scale_transform(views)
-        NNs = [self.KNs[i].kneighbors(view, self.nearest_neighbors[i]) for i, view in enumerate(views)]
-        kernels = [
-            self._get_kernel(i, self.train_views[i], Y=view)
-            for i, view in enumerate(views)
+        check_is_fitted(self, attributes=["posterior_samples"])
+        return Predictive(self._model, self.posterior_samples, return_sites=["z"])(
+            self.rng_key, views
+        )["z"]
+
+    def _model(self, views: Iterable[np.ndarray]):
+        n = views[0].shape[0]
+        p = [view.shape[1] for view in views]
+        # parameter representing the mean of column in each view of data
+        mu = [
+            numpyro.sample(
+                "mu_" + str(i), dist.MultivariateNormal(0.0, 10 * jnp.eye(p_))
+            )
+            for i, p_ in enumerate(p)
         ]
-        Wst = [fill_W(kernel, inds) for kernel, (dists, inds) in zip(kernels, NNs)]
-        Wst = [Wst[0] / Wst[0].sum(axis=1, keepdims=True), Wst[1] / Wst[1].sum(axis=1, keepdims=True)]
-        St = [Wst[0] @ self.Ws[1], Wst[1] @ self.Ws[0]]
-        return St[0] @ self.g * (1 / self.S), St[1] @ self.f * (1 / self.S)
-
-    def _get_kernel(self, view, X, Y=None):
-        params = {
-            "gamma": self.gamma[view],
-        }
-        return pairwise_kernels(
-            X, Y, metric=self.kernel[view], filter_params=True, **params
-        )
-
-
-def fill_W(kernels, inds):
-    W = np.zeros_like(kernels)
-    for i, ind in enumerate(inds):
-        W[ind, i] = kernels[ind, i]
-    return W.T
+        # parameter representing the within view variance for each view of data
+        psi = [
+            numpyro.sample("psi_" + str(i), dist.LKJCholesky(p_))
+            for i, p_ in enumerate(p)
+        ]
+        # parameter representing weights applied to latent variables
+        with numpyro.plate("plate_views", self.latent_dims):
+            self.weights_list = [
+                numpyro.sample(
+                    "W_" + str(i),
+                    dist.MultivariateNormal(0.0, 10 * jnp.diag(jnp.ones(p_))),
+                )
+                for i, p_ in enumerate(p)
+            ]
+        with numpyro.plate("plate_i", n):
+            # sample from latent z: the latent variables of the model
+            z = numpyro.sample(
+                "z", dist.MultivariateNormal(0.0, jnp.diag(jnp.ones(self.latent_dims)))
+            )
+            # sample from multivariate normal and observe data
+            [
+                numpyro.sample(
+                    "obs" + str(i),
+                    dist.MultivariateNormal((z @ W_) + mu_, scale_tril=psi_),
+                    obs=X_,
+                )
+                for i, (X_, psi_, mu_, W_) in enumerate(
+                    zip(views, psi, mu, self.weights_list)
+                )
+            ]
```

### Comparing `cca_zoo-1.9.1/cca_zoo/models/rcca.py` & `cca_zoo-2.0.0/cca_zoo/models/_iterative/_ey.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,257 +1,251 @@
-from abc import abstractmethod
-from typing import Iterable, Union
+from typing import Union
 
 import numpy as np
-from scipy.linalg import block_diag, eigh
+import torch
 
-from .cca_base import _CCA_Base
-from ..utils.check_values import _process_parameter, check_views
+from cca_zoo.models._plsmixin import PLSMixin
+from cca_zoo.models._iterative._base import BaseGradientLoop, BaseIterative
 
 
-# from hyperopt import fmin, tpe, Trials
-
-
-class rCCA(_CCA_Base):
+class CCAEY(BaseIterative):
     """
-    A class used to fit Regularised CCA (canonical ridge) model. Uses PCA to perform the optimization efficiently for high dimensional data.
-
-    Citation
-    --------
-    Vinod, Hrishikesh D. "Canonical ridge and econometrics of joint production." Journal of econometrics 4.2 (1976): 147-166.
-
-    :Example:
-
-    >>> from cca_zoo.models import rCCA
-    >>> X1 = np.random.rand(10,5)
-    >>> X2 = np.random.rand(10,5)
-    >>> model = rCCA(c=[0.1,0.1])
-    >>> model.fit([X1,X2])
+    A class used to fit Regularized CCA by Delta-EigenGame
+
+    Parameters
+    ----------
+    latent_dims : int, optional
+        Number of latent dimensions to use, by default 1
+    copy_data : bool, optional
+        Whether to copy the data, by default True
+    random_state : int, optional
+        Random state to use, by default None
+    accept_sparse : bool, optional
+        Whether to accept sparse data, by default None
+    batch_size : int, optional
+        Batch size to use, by default 1
+    epochs : int, optional
+        Number of epochs to use, by default 1
+    learning_rate : float, optional
+        Learning rate to use, by default 0.01
+
+    References
+    ----------
+    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(
-            self,
-            latent_dims: int = 1,
-            scale: bool = True,
-            centre=True,
-            copy_data=True,
-            random_state=None,
-            c: Union[Iterable[float], float] = None,
-            eps=1e-3,
-            accept_sparse=None,
+        self,
+        latent_dims: int = 1,
+        copy_data=True,
+        random_state=None,
+        tol=1e-9,
+        accept_sparse=None,
+        batch_size=None,
+        epochs=100,
+        learning_rate=1e-1,
+        initialization: Union[str, callable] = "random",
+        dataloader_kwargs=None,
+        optimizer_kwargs=None,
+        convergence_checking=False,
+        patience=10,
+        track=False,
+        verbose=False,
     ):
-        """
-        Constructor for rCCA
-
-        :param latent_dims: number of latent dimensions to fit
-        :param scale: normalize variance in each column before fitting
-        :param centre: demean data by column before fitting (and before transforming out of sample
-        :param copy_data: If True, X will be copied; else, it may be overwritten
-        :param random_state: Pass for reproducible output across multiple function calls
-        :param c: Iterable of regularisation parameters for each view (between 0:CCA and 1:PLS)
-        :param eps: epsilon for stability
-        :param accept_sparse: which forms are accepted for sparse data
-        """
-        if accept_sparse is None:
-            accept_sparse = ["csc", "csr"]
+        self.optimizer_kwargs = optimizer_kwargs
         super().__init__(
             latent_dims=latent_dims,
-            scale=scale,
-            centre=centre,
             copy_data=copy_data,
             accept_sparse=accept_sparse,
             random_state=random_state,
-        )
-        self.c = c
-        self.eps = eps
-
-    def _check_params(self):
-        self.c = _process_parameter("c", self.c, 0, self.n_views)
-
-    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        """
-        Fits a regularised CCA (canonical ridge) model
-
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        """
-        views = check_views(
-            *views, copy=self.copy_data, accept_sparse=self.accept_sparse
-        )
-        views = self._centre_scale(views)
-        self.n_views = len(views)
-        self.n = views[0].shape[0]
-        self._check_params()
-        views, C, D = self._setup_evp(views, **kwargs)
-        self._solve_evp(views, C, D, **kwargs)
-        return self
-
-    @abstractmethod
-    def _setup_evp(self, views: Iterable[np.ndarray], **kwargs):
-        Us, Ss, Vts = _pca_data(*views)
-        self.Bs = [
-            (1 - self.c[i]) * S * S / self.n + self.c[i] for i, S in enumerate(Ss)
-        ]
-        if len(views) == 2:
-            self._two_view = True
-            C, D = self._two_view_evp(Us, Ss)
-        else:
-            self._two_view = False
-            C, D = self._multi_view_evp(Us, Ss)
-        return Vts, C, D
-
-    @abstractmethod
-    def _solve_evp(self, views: Iterable[np.ndarray], C, D=None, **kwargs):
-        p = C.shape[0]
-        if self._two_view:
-            [eigvals, eigvecs] = eigh(C, subset_by_index=[p - self.latent_dims, p - 1])
-            eigvecs = eigvecs
-            idx = np.argsort(eigvals, axis=0)[::-1][: self.latent_dims]
-            eigvecs = eigvecs[:, idx].real
-            w_y = views[1].T @ np.diag(1 / np.sqrt(self.Bs[1])) @ eigvecs
-            w_x = (
-                    views[0].T
-                    @ np.diag(1 / self.Bs[0])
-                    @ self.R_12
-                    @ np.diag(1 / np.sqrt(self.Bs[1]))
-                    @ eigvecs
-                    / np.sqrt(eigvals[idx])
-            )
-            self.weights = [w_x, w_y]
-        else:
-            [eigvals, eigvecs] = eigh(
-                C, D, subset_by_index=[p - self.latent_dims, p - 1]
-            )
-            idx = np.argsort(eigvals, axis=0)[::-1]
-            eigvecs = eigvecs[:, idx].real
-            self.weights = [
-                Vt.T
-                @ np.diag(1 / np.sqrt(B))
-                @ eigvecs[split: self.splits[i + 1], : self.latent_dims]
-                for i, (split, Vt, B) in enumerate(
-                    zip(self.splits[:-1], views, self.Bs)
-                )
-            ]
-
-    def _two_view_evp(self, Us, Ss):
-        Rs = [U @ np.diag(S) for U, S in zip(Us, Ss)]
-        self.R_12 = Rs[0].T @ Rs[1]
-        M = (
-                np.diag(1 / np.sqrt(self.Bs[1]))
-                @ self.R_12.T
-                @ np.diag(1 / self.Bs[0])
-                @ self.R_12
-                @ np.diag(1 / np.sqrt(self.Bs[1]))
-        )
-        return M, None
-
-    def _multi_view_evp(self, Us, Ss):
-        D = block_diag(
-            *[np.diag((1 - self.c[i]) * S * S + self.c[i]) for i, S in enumerate(Ss)]
-        )
-        C = np.concatenate([U @ np.diag(S) for U, S in zip(Us, Ss)], axis=1)
-        C = C.T @ C
-        C -= block_diag(*[np.diag(S ** 2) for U, S in zip(Us, Ss)]) - D
-        D_smallest_eig = min(0, np.linalg.eigvalsh(D).min()) - self.eps
-        D = D - D_smallest_eig * np.eye(D.shape[0])
-        self.splits = np.cumsum([0] + [U.shape[1] for U in Us])
-        return C, D
-
-
-class CCA(rCCA):
-    """
-    A class used to fit a simple CCA model
-
-    Implements CCA by inheriting regularised CCA with 0 regularisation
-
-    Citation
-    --------
-    Hotelling, Harold. "Relations between two sets of variates." Breakthroughs in statistics. Springer, New York, NY, 1992. 162-190.
-
-    :Example:
-
-    >>> from cca_zoo.models import CCA
-    >>> X1 = np.random.rand(10,5)
-    >>> X2 = np.random.rand(10,5)
-    >>> model = CCA()
-    >>> model.fit(X1,X2)
+            tol=tol,
+            batch_size=batch_size,
+            epochs=epochs,
+            learning_rate=learning_rate,
+            initialization=initialization,
+            dataloader_kwargs=dataloader_kwargs,
+            convergence_checking=convergence_checking,
+            patience=patience,
+            track=track,
+            verbose=verbose,
+        )
+        # ensure dataloader_kwargs['shuffle'] is True
+        self.dataloader_kwargs["shuffle"] = True
+
+    def _get_module(self, weights=None, k=None):
+        return EYLoop(
+            weights=weights,
+            k=k,
+            learning_rate=self.learning_rate,
+            optimizer_kwargs=self.optimizer_kwargs,
+            objective="cca",
+        )
+
+    def _more_tags(self):
+        return {"multiview": True, "stochastic": True}
+
+
+class PLSEY(CCAEY, PLSMixin):
+    """
+    A class used to fit Regularized CCA by Delta-EigenGame
+
+    Parameters
+    ----------
+    latent_dims : int, optional
+        Number of latent dimensions to use, by default 1
+    copy_data : bool, optional
+        Whether to copy the data, by default True
+    random_state : int, optional
+        Random state to use, by default None
+    accept_sparse : bool, optional
+        Whether to accept sparse data, by default None
+    batch_size : int, optional
+        Batch size to use, by default 1
+    epochs : int, optional
+        Number of epochs to use, by default 1
+    learning_rate : float, optional
+        Learning rate to use, by default 0.01
+
+    References
+    ----------
+    Chapman, James, Ana Lawry Aguila, and Lennie Wells. "A Generalized EigenGame with Extensions to Multiview Representation Learning." arXiv preprint arXiv:2211.11323 (2022).
     """
 
     def __init__(
-            self,
-            latent_dims: int = 1,
-            scale: bool = True,
-            centre=True,
-            copy_data=True,
-            random_state=None,
+        self,
+        latent_dims: int = 1,
+        copy_data=True,
+        random_state=None,
+        tol=1e-9,
+        accept_sparse=None,
+        batch_size=None,
+        epochs=1,
+        learning_rate=1,
+        initialization: Union[str, callable] = "random",
+        dataloader_kwargs=None,
+        convergence_checking=False,
+        patience=10,
+        track=False,
+        verbose=False,
     ):
-        """
-        Constructor for CCA
-        :param latent_dims: number of latent dimensions to fit
-        :param scale: normalize variance in each column before fitting
-        :param centre: demean data by column before fitting (and before transforming out of sample
-        :param copy_data: If True, X will be copied; else, it may be overwritten
-        :param random_state: Pass for reproducible output across multiple function calls
-        """
         super().__init__(
             latent_dims=latent_dims,
-            scale=scale,
-            centre=centre,
             copy_data=copy_data,
-            c=[0.0, 0.0],
+            accept_sparse=accept_sparse,
             random_state=random_state,
+            tol=tol,
+            batch_size=batch_size,
+            epochs=epochs,
+            learning_rate=learning_rate,
+            initialization=initialization,
+            dataloader_kwargs=dataloader_kwargs,
+            convergence_checking=convergence_checking,
+            patience=patience,
+            track=track,
+            verbose=verbose,
+        )
+        self.previous_views = None
+
+    def _get_module(self, weights=None, k=None):
+        return EYLoop(
+            weights=weights,
+            k=k,
+            learning_rate=self.learning_rate,
+            optimizer_kwargs=self.optimizer_kwargs,
+            objective="pls",
         )
 
+    def _more_tags(self):
+        return {"multiview": True, "stochastic": True}
 
-class PLS(rCCA):
-    """
-    A class used to fit a simple PLS model
-
-    Implements PLS by inheriting regularised CCA with maximal regularisation
-
-    :Example:
-
-    >>> from cca_zoo.models import PLS
-    >>> X1 = np.random.rand(10,5)
-    >>> X2 = np.random.rand(10,5)
-    >>> model = CCA()
-    >>> model.fit([X1,X2])
-    """
 
+class EYLoop(BaseGradientLoop):
     def __init__(
-            self,
-            latent_dims: int = 1,
-            scale: bool = True,
-            centre=True,
-            copy_data=True,
-            random_state=None,
+        self,
+        weights=None,
+        k=None,
+        learning_rate=1e-3,
+        optimizer_kwargs=None,
+        objective="cca",
     ):
-        """
-        Constructor for CCA
-        :param latent_dims: number of latent dimensions to fit
-        :param scale: normalize variance in each column before fitting
-        :param centre: demean data by column before fitting (and before transforming out of sample
-        :param copy_data: If True, X will be copied; else, it may be overwritten
-        :param random_state: Pass for reproducible output across multiple function calls
-        """
         super().__init__(
-            latent_dims=latent_dims,
-            scale=scale,
-            centre=centre,
-            copy_data=copy_data,
-            c=[1.0, 1.0],
-            random_state=random_state,
-        )
-
+            weights=weights,
+            k=k,
+            learning_rate=learning_rate,
+            optimizer_kwargs=optimizer_kwargs,
+        )
+        self.objective = objective
+        self.batch_queue = []
+        self.val_batch_queue = []
+
+    def training_step(self, batch, batch_idx):
+        # Checking if the queue has at least one batch
+        if len(self.batch_queue) < 1:
+            # Adding the current batch to the queue
+            self.batch_queue.append(batch)
+            # Returning a zero loss
+            loss = {
+                "loss": torch.tensor(0, requires_grad=True, dtype=torch.float32),
+            }
+        else:
+            # randomly select a batch from the queue
+            batch2 = self.batch_queue[np.random.randint(0, len(self.batch_queue))]
+            # Computing the loss with the current batch and the oldest batch in the queue
+            loss = self.loss(batch["views"], batch2["views"])
+            # Adding the current batch to the queue and removing the oldest batch
+            self.batch_queue.append(batch)
+            self.batch_queue.pop(0)
+        # Logging the loss components
+        for k, v in loss.items():
+            self.log(k, v, prog_bar=False)
+        return loss
+
+    def get_AB(self, z):
+        latent_dims = z[0].shape[1]
+        A = torch.zeros(
+            latent_dims, latent_dims, device=z[0].device
+        )  # initialize the cross-covariance matrix
+        B = torch.zeros(
+            latent_dims, latent_dims, device=z[0].device
+        )  # initialize the auto-covariance matrix
+        for i, zi in enumerate(z):
+            for j, zj in enumerate(z):
+                if i == j:
+                    if self.objective == "cca":
+                        B += torch.cov(
+                            zi.T
+                        )  # add the auto-covariance of each view to B
+                    elif self.objective == "pls":
+                        B += self.weights[i].T @ self.weights[i]
+                else:
+                    A += torch.cov(torch.hstack((zi, zj)).T)[
+                        latent_dims:, :latent_dims
+                    ]  # add the cross-covariance of each pair of views to A
+        return A / len(z), B / len(
+            z
+        )  # return the normalized matrices (divided by the number of views)
+
+    def loss(self, views, views2=None, **kwargs):
+        # Encoding the views with the forward method
+        z = self(views)
+        # Getting A and B matrices from z
+        A, B = self.get_AB(z)
+
+        if views2 is None:
+            # Computing rewards and penalties using A and B only
+            rewards = torch.trace(2 * A)
+            penalties = torch.trace(B @ B)
 
-def _pca_data(*views: np.ndarray):
-    """
-    :param views: numpy arrays with the same number of rows (samples) separated by commas
-    """
-    views_U = []
-    views_S = []
-    views_Vt = []
-    for i, view in enumerate(views):
-        U, S, Vt = np.linalg.svd(view, full_matrices=False)
-        views_U.append(U)
-        views_S.append(S)
-        views_Vt.append(Vt)
-    return views_U, views_S, views_Vt
+        else:
+            # Encoding another set of views with the forward method
+            z2 = self(views2)
+            # Getting A' and B' matrices from z2
+            A_, B_ = self.get_AB(z2)
+            # Computing rewards and penalties using A and B'
+            rewards = torch.trace(2 * A)
+            penalties = torch.trace(B @ B_)
+
+        return {
+            "loss": -rewards + penalties,
+            "rewards": rewards,
+            "penalties": penalties,
+        }
```

### Comparing `cca_zoo-1.9.1/cca_zoo/models/tcca.py` & `cca_zoo-2.0.0/cca_zoo/model_selection/_search.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,273 +1,302 @@
-from typing import Iterable, Union
+# Author: James Chapman
+# This code heavily leans on the scikit-learn original
+# Original Authors:
+#         Alexandre Gramfort <alexandre.gramfort@inria.fr>,
+#         Gael Varoquaux <gael.varoquaux@normalesup.org>
+#         Andreas Mueller <amueller@ais.uni-bonn.de>
+#         Olivier Grisel <olivier.grisel@ensta.org>
+#         Raghav RV <rvraghav93@gmail.com>
+
+import itertools
+from typing import Iterable
 
 import numpy as np
-import tensorly as tl
-from scipy.linalg import sqrtm
-from sklearn.metrics.pairwise import pairwise_kernels
-from sklearn.utils.validation import check_is_fitted
-from tensorly.decomposition import parafac
+from mvlearn.compose import SimpleSplitter
+from sklearn import clone
+from sklearn.model_selection import ParameterGrid
+from sklearn.model_selection._search import BaseSearchCV, ParameterSampler
+from sklearn.pipeline import Pipeline
+from sklearn.utils import check_random_state
 
-from .cca_base import _CCA_Base
-from ..utils.check_values import _process_parameter, check_views
 
+def param2grid(params):
+    """
+    Converts parameters with a list for each view into a scikit-learn friendly form
+    Parameters
 
-class TCCA(_CCA_Base):
+    :param params : a dictionary of parameters where some parameters may contain a list of lists (one list for each 'view')
+    Returns : a parameter grid in the form expected by scikit-learn where each element is a single candidate
+    (a single value or a list with one value for each view)
+
+    Example
+    -------
+    >>> params = {'regs': [[1, 2], [3, 4]]}
+    >>> param2grid(params)
+    {'regs': [[1, 3], [1, 4], [2, 3], [2, 4]]}
     """
-    Fits a Tensor CCA model. Tensor CCA maximises higher order correlations
+    params = params.copy()
+    for k, v in params.items():
+        if any([isinstance(v_, list) for v_ in v]):
+            # itertools expects all lists to perform product
+            v = [[v_] if not isinstance(v_, list) else v_ for v_ in v]
+            params[k] = list(map(list, itertools.product(*v)))
+    return ParameterGrid(params)
 
-    Citation
-    --------
-    Kim, Tae-Kyun, Shu-Fai Wong, and Roberto Cipolla. "Tensor canonical correlation analysis for action classification." 2007 IEEE Conference on Computer Vision and Pattern Recognition. IEEE, 2007
 
-    My own port from https://github.com/rciszek/mdr_tcca
+class ParameterSampler_(ParameterSampler):
+    """
+    Generator on parameters sampled from given distributions.
+    Non-deterministic iterable over random candidate combinations for hyper-
+    parameter search. If all parameters are presented as a list,
+    sampling without replacement is performed. If at least one parameter
+    is given as a distribution, sampling with replacement is used.
+    It is highly recommended to use continuous distributions for continuous
+    parameters.
+    Read more in the :ref:`User Guide <grid_search>`.
+
+    :param param_distributions: dict
+        Dictionary with parameters names (`str`) as keys and distributions
+        or lists of parameters to try. Distributions must provide a ``rvs``
+        method for sampling (such as those from scipy.stats.distributions).
+        If a list is given, it is sampled uniformly.
+        If a list of dicts is given, first a dict is sampled uniformly, and
+        then a parameter is sampled using that dict as above.
+    :param n_iter: int
+        Number of parameter settings that are produced.
+    :param random_state: int, RandomState instance or None, default=None
+        Pseudo random number generator state used for random uniform sampling
+        from lists of possible values instead of scipy.stats distributions.
+        Pass an int for reproducible output across multiple
+        function calls.
+        See :term:`Glossary <random_state>`.
 
     :Example:
+    >>> from sklearn.model_selection import ParameterSampler
+    >>> from scipy.stats.distributions import expon
+    >>> import numpy as np
+    >>> rng = np.random.RandomState(0)
+    >>> param_grid = {'a':[1, 2], 'b': expon()}
+    >>> param_list = list(ParameterSampler(param_grid, n_iter=4,
+    ...                                    random_state=rng))
+    >>> rounded_list = [dict((k, round(v, 6)) for (k, v) in d.items())
+    ...                 for d in param_list]
+    >>> rounded_list == [{'b': 0.89856, 'a': 1},
+    ...                  {'b': 0.923223, 'a': 1},
+    ...                  {'b': 1.878964, 'a': 2},
+    ...                  {'b': 1.038159, 'a': 2}]
+    True
+    """
+
+    def __iter__(self):
+        rng = check_random_state(self.random_state)
+        for _ in range(self.n_iter):
+            dist = rng.choice(self.param_distributions)
+            # Always sort the keys of a dictionary, for reproducibility
+            items = sorted(dist.items())
+            params = dict()
+            for k, v in items:
+                # if value is an iterable then either the elements are the distribution or each element is a distribution
+                # for each view.
+                if isinstance(v, Iterable):
+                    # if each element is a distribution for each view (i.e. it is a non-string Iterable) then call return_param for each view
+                    if any(
+                        [
+                            (isinstance(v_, Iterable) and not isinstance(v_, str))
+                            or hasattr(v_, "rvs")
+                            for v_ in v
+                        ]
+                    ):
+                        params[k] = [self.return_param(v_) for v_ in v]
+                    # if the parameter is shared across views then the list will just contain non-iterable values
+                    else:
+                        params[k] = self.return_param(v)
+                # if value is not iterable then it is either a distribution or a value in which case call return param on it.
+                else:
+                    params[k] = self.return_param(v)
+            yield params
+
+    def return_param(self, v):
+        rng = check_random_state(self.random_state)
+        if hasattr(v, "rvs"):
+            param = v.rvs(random_state=rng)
+        elif isinstance(v, Iterable) and not isinstance(v, str):
+            param = v[rng.randint(len(v))]
+        else:
+            param = v
+        return param
+
+    def __len__(self):
+        """Number of points that will be sampled."""
+        return self.n_iter
+
 
-    >>> from cca_zoo.models import TCCA
-    >>> X1 = np.random.rand(10,5)
-    >>> X2 = np.random.rand(10,5)
-    >>> model = TCCA()
-    >>> model.fit([X1,X2])
+class GridSearchCV(BaseSearchCV):
     """
 
+    :Example:
+    >>> from cca_zoo.model_selection import GridSearchCV
+    >>> from cca_zoo.models import MCCA
+    >>> X1 = [[0, 0, 1], [1, 0, 0], [2, 2, 2], [3, 5, 4]]
+    >>> X2 = [[0.1, -0.2], [0.9, 1.1], [6.2, 5.9], [11.9, 12.3]]
+    >>> X3 = [[0, 1, 0], [1, 9, 0], [4, 3, 3,], [12, 8, 10]]
+    >>> model = MCCA()
+    >>> params = {'c': [[0.1, 0.2], [0.3, 0.4], 0.1]}
+    >>> GridSearchCV(model,param_grid=params, cv=3).fit([X1,X2,X3]).best_estimator_.c
+    [0.1, 0.3, 0.1]
+
+    :Notes:
+
+    The parameters selected are those that maximize the score of the left out
+    data, unless an explicit score is passed in which case it is used instead.
+    If `n_jobs` was set to a value higher than one, the data is copied for each
+    point in the grid (and not `n_jobs` times). This is done for efficiency
+    reasons if individual jobs take very little time, but may raise errors if
+    the dataset is large and not enough memory is available.  A workaround in
+    this case is to set `pre_dispatch`. Then, the memory is copied only
+    `pre_dispatch` many times. A reasonable value for `pre_dispatch` is `2 *
+    n_jobs`.
+    """
+
+    _required_parameters = ["estimator", "param_grid"]
+
     def __init__(
-            self,
-            latent_dims: int = 1,
-            scale=True,
-            centre=True,
-            copy_data=True,
-            random_state=None,
-            c: Union[Iterable[float], float] = None,
+        self,
+        estimator,
+        param_grid,
+        *,
+        scoring=None,
+        n_jobs=None,
+        refit=True,
+        cv=None,
+        verbose=0,
+        pre_dispatch="2*n_jobs",
+        error_score=np.nan,
+        return_train_score=False,
     ):
-        """
-        Constructor for TCCA
-
-        :param latent_dims: number of latent dimensions to fit
-        :param scale: normalize variance in each column before fitting
-        :param centre: demean data by column before fitting (and before transforming out of sample
-        :param copy_data: If True, X will be copied; else, it may be overwritten
-        :param random_state: Pass for reproducible output across multiple function calls
-        :param c: Iterable of regularisation parameters for each view (between 0:CCA and 1:PLS)
-        """
         super().__init__(
-            latent_dims=latent_dims,
-            scale=scale,
-            centre=centre,
-            copy_data=copy_data,
-            accept_sparse=["csc", "csr"],
-            random_state=random_state,
+            estimator=estimator,
+            scoring=scoring,
+            n_jobs=n_jobs,
+            refit=refit,
+            cv=cv,
+            verbose=verbose,
+            pre_dispatch=pre_dispatch,
+            error_score=error_score,
+            return_train_score=return_train_score,
         )
-        self.c = c
-
-    def _check_params(self):
-        self.c = _process_parameter("c", self.c, 0, self.n_views)
+        if not isinstance(param_grid, ParameterGrid):
+            self.param_grid = param2grid(param_grid)
+        else:
+            self.param_grid = param_grid
 
-    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        """
+    def _run_search(self, evaluate_candidates):
+        """Search all candidates in param_grid"""
+        param_grid = self.param_grid
+        param_grid.param_grid = [
+            {f"estimator__{key}": val for key, val in subgrid.items()}
+            for subgrid in param_grid.param_grid
+        ]
+        evaluate_candidates(param_grid)
 
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        """
-        views = check_views(
-            *views, copy=self.copy_data, accept_sparse=self.accept_sparse
+    def fit(self, X, y=None, *, groups=None, **fit_params):
+        self.estimator = Pipeline(
+            [
+                ("splitter", SimpleSplitter([X_.shape[1] for X_ in X])),
+                ("estimator", clone(self.estimator)),
+            ]
         )
-        views = self._centre_scale(views)
-        self.n_views = len(views)
-        self.n = views[0].shape[0]
-        self._check_params()
-        # returns whitened views along with whitening matrices
-        whitened_views, covs_invsqrt = self._setup_tensor(*views)
-        # The idea here is to form a matrix with M dimensions one for each view where at index
-        # M[p_i,p_j,p_k...] we have the sum over n samples of the product of the pth feature of the
-        # ith, jth, kth view etc.
-        for i, el in enumerate(whitened_views):
-            # To achieve this we start with the first view so M is nxp.
-            if i == 0:
-                M = el
-            # For the remaining views we expand their dimensions to match M i.e. nx1x...x1xp
-            else:
-                for _ in range(len(M.shape) - 1):
-                    el = np.expand_dims(el, 1)
-                # Then we perform an outer product by expanding the dimensionality of M and
-                # outer product with the expanded el
-                M = np.expand_dims(M, -1) @ el
-        M = np.mean(M, 0)
-        tl.set_backend("numpy")
-        M_parafac = parafac(M, self.latent_dims, verbose=True)
-        self.weights = [
-            cov_invsqrt @ fac
-            for i, (view, cov_invsqrt, fac) in enumerate(
-                zip(whitened_views, covs_invsqrt, M_parafac.factors)
-            )
-        ]
+        self = BaseSearchCV.fit(self, np.hstack(X), y=y, groups=groups, **fit_params)
+        self.best_estimator_ = self.best_estimator_["estimator"]
+        self.best_params_ = {
+            key[len("estimator__") :]: val for key, val in self.best_params_.items()
+        }
         return self
 
-    def correlations(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        """
-        Predicts the correlation for the given data using the fit model
-
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        :param kwargs: any additional keyword arguments required by the given model
-        """
-        transformed_views = self.transform(views, **kwargs)
-        transformed_views = [
-            transformed_view - transformed_view.mean(axis=0)
-            for transformed_view in transformed_views
-        ]
-        multiplied_views = np.stack(transformed_views, axis=0).prod(axis=0).mean(axis=0)
-        stds = np.stack(
-            [transformed_view.std(axis=0) for transformed_view in transformed_views],
-            axis=0,
-        ).prod(axis=0)
-        corrs = multiplied_views / stds
-        return corrs
-
-    def score(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        """
-        Returns the higher order correlations in each dimension
-
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        :param kwargs: any additional keyword arguments required by the given model
-        """
-        dim_corrs = self.correlations(views, **kwargs)
-        return dim_corrs
-
-    def _setup_tensor(self, *views: np.ndarray, **kwargs):
-        train_views = self._centre_scale(views)
-        n = train_views[0].shape[0]
-        covs = [
-            (1 - self.c[i]) * view.T @ view / (self.n)
-            + self.c[i] * np.eye(view.shape[1])
-            for i, view in enumerate(train_views)
-        ]
-        covs_invsqrt = [np.linalg.inv(sqrtm(cov)) for cov in covs]
-        train_views = [
-            train_view @ cov_invsqrt
-            for train_view, cov_invsqrt in zip(train_views, covs_invsqrt)
-        ]
-        return train_views, covs_invsqrt
-
 
-class KTCCA(TCCA):
+class RandomizedSearchCV(BaseSearchCV):
     """
-    Fits a Kernel Tensor CCA model. Tensor CCA maximises higher order correlations
-
-    Citation
-    --------
-    Kim, Tae-Kyun, Shu-Fai Wong, and Roberto Cipolla. "Tensor canonical correlation analysis for action classification." 2007 IEEE Conference on Computer Vision and Pattern Recognition. IEEE, 2007
 
     :Example:
-
-    >>> from cca_zoo.models import KTCCA
-    >>> X1 = np.random.rand(10,5)
-    >>> X2 = np.random.rand(10,5)
-    >>> model = KTCCA()
-    >>> model.fit([X1,X2])
+    >>> from cca_zoo.model_selection import RandomizedSearchCV
+    >>> from cca_zoo.models import MCCA
+    >>> from sklearn._utils.fixes import loguniform
+    >>> X1 = [[0, 0, 1], [1, 0, 0], [2, 2, 2], [3, 5, 4]]
+    >>> X2 = [[0.1, -0.2], [0.9, 1.1], [6.2, 5.9], [11.9, 12.3]]
+    >>> X3 = [[0, 1, 0], [1, 9, 0], [4, 3, 3,], [12, 8, 10]]
+    >>> model = MCCA()
+    >>> params = {'c': [loguniform(1e-4, 1e0), loguniform(1e-4, 1e0), [0.1]]}
+    >>> def scorer(estimator, views):
+    ...    scores = estimator.score(views)
+    ...    return np.mean(scores)
+    >>> RandomizedSearchCV(model,param_distributions=params, cv=3, scoring=scorer,n_iter=10).fit([X1,X2,X3]).n_iter
+    10
+
+    :Notes:
+
+    The parameters selected are those that maximize the score of the held-out
+    data, according to the scoring parameter.
+    If `n_jobs` was set to a value higher than one, the data is copied for each
+    parameter setting(and not `n_jobs` times). This is done for efficiency
+    reasons if individual jobs take very little time, but may raise errors if
+    the dataset is large and not enough memory is available.  A workaround in
+    this case is to set `pre_dispatch`. Then, the memory is copied only
+    `pre_dispatch` many times. A reasonable value for `pre_dispatch` is `2 *
+    n_jobs`.
     """
 
+    _required_parameters = ["estimator", "param_distributions"]
+
     def __init__(
-            self,
-            latent_dims: int = 1,
-            scale: bool = True,
-            centre=True,
-            copy_data=True,
-            random_state=None,
-            eps=1e-3,
-            c: Union[Iterable[float], float] = None,
-            kernel: Iterable[Union[float, callable]] = None,
-            gamma: Iterable[float] = None,
-            degree: Iterable[float] = None,
-            coef0: Iterable[float] = None,
-            kernel_params: Iterable[dict] = None,
+        self,
+        estimator,
+        param_distributions,
+        *,
+        n_iter=10,
+        scoring=None,
+        n_jobs=None,
+        refit=True,
+        cv=None,
+        verbose=0,
+        pre_dispatch="2*n_jobs",
+        random_state=None,
+        error_score=np.nan,
+        return_train_score=False,
     ):
-        """
-        Constructor for TCCA
-
-        :param latent_dims: number of latent dimensions to fit
-        :param scale: normalize variance in each column before fitting
-        :param centre: demean data by column before fitting (and before transforming out of sample
-        :param copy_data: If True, X will be copied; else, it may be overwritten
-        :param random_state: Pass for reproducible output across multiple function calls
-        :param c: Iterable of regularisation parameters for each view (between 0:CCA and 1:PLS)
-        :param kernel: Iterable of kernel mappings used internally. This parameter is directly passed to :class:`~sklearn.metrics.pairwise.pairwise_kernel`. If element of `kernel` is a string, it must be one of the metrics in `pairwise.PAIRWISE_KERNEL_FUNCTIONS`. Alternatively, if element of `kernel` is a callable function, it is called on each pair of instances (rows) and the resulting value recorded. The callable should take two rows from X as input and return the corresponding kernel value as a single number. This means that callables from :mod:`sklearn.metrics.pairwise` are not allowed, as they operate on matrices, not single samples. Use the string identifying the kernel instead.
-        :param gamma: Iterable of gamma parameters for the RBF, laplacian, polynomial, exponential chi2 and sigmoid kernels. Interpretation of the default value is left to the kernel; see the documentation for sklearn.metrics.pairwise. Ignored by other kernels.
-        :param degree: Iterable of degree parameters of the polynomial kernel. Ignored by other kernels.
-        :param coef0: Iterable of zero coefficients for polynomial and sigmoid kernels. Ignored by other kernels.
-        :param kernel_params: Iterable of additional parameters (keyword arguments) for kernel function passed as callable object.
-        :param eps: epsilon value to ensure stability
-        """
+        self.param_distributions = {
+            f"estimator__{key}": val for key, val in param_distributions.items()
+        }
+        self.n_iter = n_iter
+        self.random_state = random_state
         super().__init__(
-            latent_dims=latent_dims,
-            scale=scale,
-            centre=centre,
-            copy_data=copy_data,
-            random_state=random_state,
-        )
-        self.kernel_params = kernel_params
-        self.gamma = gamma
-        self.coef0 = coef0
-        self.kernel = kernel
-        self.degree = degree
-        self.c = c
-        self.eps = eps
-
-    def _check_params(self):
-        self.kernel = _process_parameter("kernel", self.kernel, "linear", self.n_views)
-        self.gamma = _process_parameter("gamma", self.gamma, None, self.n_views)
-        self.coef0 = _process_parameter("coef0", self.coef0, 1, self.n_views)
-        self.degree = _process_parameter("degree", self.degree, 1, self.n_views)
-        self.c = _process_parameter("c", self.c, 0, self.n_views)
-
-    def _get_kernel(self, view, X, Y=None):
-        if callable(self.kernel):
-            params = self.kernel_params[view] or {}
-        else:
-            params = {
-                "gamma": self.gamma[view],
-                "degree": self.degree[view],
-                "coef0": self.coef0[view],
-            }
-        return pairwise_kernels(
-            X, Y, metric=self.kernel[view], filter_params=True, **params
+            estimator=estimator,
+            scoring=scoring,
+            n_jobs=n_jobs,
+            refit=refit,
+            cv=cv,
+            verbose=verbose,
+            pre_dispatch=pre_dispatch,
+            error_score=error_score,
+            return_train_score=return_train_score,
         )
 
-    def _setup_tensor(self, *views: np.ndarray):
-        self.train_views = views
-        kernels = [self._get_kernel(i, view) for i, view in enumerate(self.train_views)]
-        covs = [
-            (1 - self.c[i]) * kernel @ kernel.T / (self.n - 1) + self.c[i] * kernel
-            for i, kernel in enumerate(kernels)
-        ]
-        smallest_eigs = [
-            min(0, np.linalg.eigvalsh(cov).min()) - self.eps for cov in covs
-        ]
-        covs = [
-            cov - smallest_eig * np.eye(cov.shape[0])
-            for cov, smallest_eig in zip(covs, smallest_eigs)
-        ]
-        self.covs_invsqrt = [np.linalg.inv(sqrtm(cov)).real for cov in covs]
-        kernels = [
-            kernel @ cov_invsqrt
-            for kernel, cov_invsqrt in zip(kernels, self.covs_invsqrt)
-        ]
-        return kernels, self.covs_invsqrt
+    def _run_search(self, evaluate_candidates):
+        """Search n_iter candidates from param_distributions"""
+        evaluate_candidates(
+            ParameterSampler_(
+                self.param_distributions, self.n_iter, random_state=self.random_state
+            )
+        )
 
-    def transform(self, views: np.ndarray, y=None, **kwargs):
-        """
-        Transforms data given a fit k=KCCA model
-
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        :param kwargs: any additional keyword arguments required by the given model
-        """
-        check_is_fitted(self, attributes=["weights"])
-        views = check_views(
-            *views, copy=self.copy_data, accept_sparse=self.accept_sparse
+    def fit(self, X, y=None, *, groups=None, **fit_params):
+        self.estimator = Pipeline(
+            [
+                ("splitter", SimpleSplitter([X_.shape[1] for X_ in X])),
+                ("estimator", clone(self.estimator)),
+            ]
         )
-        views = self._centre_scale_transform(views)
-        Ktest = [
-            self._get_kernel(i, self.train_views[i], Y=view)
-            for i, view in enumerate(views)
-        ]
-        transformed_views = [
-            kernel.T @ self.weights[i] for i, kernel in enumerate(Ktest)
-        ]
-        return transformed_views
+        self = BaseSearchCV.fit(self, np.hstack(X), y=y, groups=groups, **fit_params)
+        self.best_estimator_ = self.best_estimator_["estimator"]
+        self.best_params_ = {
+            key[len("estimator__") :]: val for key, val in self.best_params_.items()
+        }
+        return self
```

### Comparing `cca_zoo-1.9.1/cca_zoo/probabilisticmodels/vcca.py` & `cca_zoo-2.0.0/cca_zoo/models/_iterative/_incrementalpls.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,115 @@
-from typing import Iterable
+from typing import Union
 
-import jax.numpy as jnp
 import numpy as np
-import numpyro
-import numpyro.distributions as dist
-from jax.random import PRNGKey
-from numpyro.infer import MCMC, NUTS, Predictive
-from sklearn.utils.validation import check_is_fitted
 
-from cca_zoo.models import _CCA_Base
-
-
-class VariationalCCA(_CCA_Base):
-    """
-    A class used to fit a variational bayesian CCA
-
-    Citation
-    --------
-    Wang, Chong. "Variational Bayesian approach to canonical correlation analysis." IEEE Transactions on Neural Networks 18.3 (2007): 905-910.
-
-    :Example:
+from cca_zoo.models._iterative._base import BaseIterative
 
 
+class IncrementalPLS(BaseIterative):
+    r"""
+    A class used to fit Incremental PLS
+
+    Parameters
+    ----------
+    latent_dims : int, optional
+        Number of latent dimensions to use, by default 1
+    copy_data : bool, optional
+        Whether to copy the data, by default True
+    random_state : int, optional
+        Random state to use, by default None
+    accept_sparse : bool, optional
+        Whether to accept sparse data, by default None
+    batch_size : int, optional
+        Batch size to use, by default 1
+    epochs : int, optional
+        Number of epochs to use, by default 1
+    simple : bool, optional
+        Whether to use the simple update, by default False
+
+    References
+    ----------
+    Arora, Raman, et al. "Stochastic optimization for PCA and PLS." 2012 50th Annual Allerton Conference on Communication, Control, and Computing (Allerton). IEEE, 2012.
     """
 
     def __init__(
-            self,
-            latent_dims: int = 1,
-            copy_data=True,
-            random_state: int = 0,
-            num_samples=100,
-            num_warmup=100,
+        self,
+        latent_dims: int = 1,
+        copy_data=True,
+        random_state=None,
+        accept_sparse=None,
+        batch_size=1,
+        epochs=1,
+        simple=False,
+        initialization: Union[str, callable] = "random",
     ):
         super().__init__(
             latent_dims=latent_dims,
             copy_data=copy_data,
-            accept_sparse=False,
+            accept_sparse=accept_sparse,
             random_state=random_state,
+            batch_size=batch_size,
+            epochs=epochs,
+            initialization=initialization,
         )
-        self.num_samples = num_samples
-        self.num_warmup = num_warmup
-        self.rng_key = PRNGKey(random_state)
-
-    def fit(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        """
-        Infer the parameters (mu: mean, psi: within view variance) and latent variables (z) of the generative CCA model
-
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        """
-        nuts_kernel = NUTS(self._model)
-        self.mcmc = MCMC(
-            nuts_kernel, num_samples=self.num_samples, num_warmup=self.num_warmup
-        )
-        self.mcmc.run(self.rng_key, views)
-        self.posterior_samples = self.mcmc.get_samples()
-        return self
-
-    def transform(self, views: Iterable[np.ndarray], y=None, **kwargs):
-        """
-        Predict the latent variables that generate the data in views using the sampled model parameters
-
-        :param views: list/tuple of numpy arrays or array likes with the same number of rows (samples)
-        """
-        check_is_fitted(self, attributes=["posterior_samples"])
-        return Predictive(self._model, self.posterior_samples, return_sites=["z"])(
-            self.rng_key, views
-        )["z"]
-
-    def _model(self, views: Iterable[np.ndarray]):
-        n = views[0].shape[0]
-        p = [view.shape[1] for view in views]
-        # parameter representing the mean of column in each view of data
-        mu = [
-            numpyro.sample(
-                "mu_" + str(i), dist.MultivariateNormal(0.0, 10 * jnp.eye(p_))
-            )
-            for i, p_ in enumerate(p)
-        ]
-        # parameter representing the within view variance for each view of data
-        psi = [
-            numpyro.sample("psi_" + str(i), dist.LKJCholesky(p_))
-            for i, p_ in enumerate(p)
+        self.simple = simple
+
+    def _update(self, views):
+        if not hasattr(self, "S"):
+            self.S = np.zeros(self.latent_dims)
+            self.count = 0
+        if self.simple:
+            self.simple_update(views)
+        else:
+            self.incremental_update(views)
+        return False
+
+    def incremental_update(self, views):
+        hats = np.stack([view @ weight for view, weight in zip(views, self.weights)])
+        orths = [
+            view - hat @ weight.T
+            for view, weight, hat in zip(views, self.weights, hats)
         ]
-        # parameter representing weights applied to latent variables
-        with numpyro.plate("plate_views", self.latent_dims):
-            self.weights_list = [
-                numpyro.sample(
-                    "W_" + str(i),
-                    dist.MultivariateNormal(0.0, 10 * jnp.diag(jnp.ones(p_))),
-                )
-                for i, p_ in enumerate(p)
-            ]
-        with numpyro.plate("plate_i", n):
-            # sample from latent z: the latent variables of the model
-            z = numpyro.sample(
-                "z", dist.MultivariateNormal(0.0, jnp.diag(jnp.ones(self.latent_dims)))
-            )
-            # sample from multivariate normal and observe data
-            [
-                numpyro.sample(
-                    "obs" + str(i),
-                    dist.MultivariateNormal((z @ W_) + mu_, scale_tril=psi_),
-                    obs=X_,
-                )
-                for i, (X_, psi_, mu_, W_) in enumerate(
-                zip(views, psi, mu, self.weights_list)
+        self.incrsvd(hats, orths)
+
+    def simple_update(self, views):
+        if not hasattr(self, "M"):
+            self.M = np.zeros((views[0].shape[1], views[1].shape[1]))
+        self.M = (
+            views[0].T @ views[1]
+            + self.weights[0] @ np.diag(self.S) @ self.weights[1].T
+        )
+        U, S, Vt = np.linalg.svd(self.M)
+        self.weights[0] = U[:, : self.latent_dims]
+        self.weights[1] = Vt.T[:, : self.latent_dims]
+        self.S = S[: self.latent_dims]
+
+    def incrsvd(self, hats, orths):
+        Q = np.vstack(
+            (
+                np.hstack(
+                    (
+                        np.diag(self.S) + hats[0].T @ hats[1],
+                        np.linalg.norm(orths[1], axis=1).T * hats[0].T,
+                    )
+                ),
+                np.hstack(
+                    (
+                        (np.linalg.norm(orths[0], axis=1).T * hats[1].T).T,
+                        np.atleast_2d(
+                            np.linalg.norm(orths[0], axis=1, keepdims=True)
+                            @ np.linalg.norm(orths[1], axis=1, keepdims=True).T
+                        ),
+                    )
+                ),
             )
-            ]
+        )
+        U, S, Vt = np.linalg.svd(Q)
+        self.weights[0] = (
+            np.hstack((self.weights[0], orths[0].T / np.linalg.norm(orths[0])))
+            @ U[:, : self.latent_dims]
+        )
+        self.weights[1] = (
+            np.hstack((self.weights[1], orths[1].T / np.linalg.norm(orths[1])))
+            @ Vt.T[:, : self.latent_dims]
+        )
+        self.S = S[: self.latent_dims]
```

### Comparing `cca_zoo-1.9.1/cca_zoo/utils/check_values.py` & `cca_zoo-2.0.0/cca_zoo/utils/check_values.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,10 @@
 import warnings
-from typing import Iterable
 
 import numpy as np
-from sklearn.utils import check_array
-
-
-def check_views(*views: Iterable[np.ndarray], copy=False, accept_sparse=False):
-    """
-
-    :param views:
-    :param copy:
-    """
-    if len(views) == 2:
-        # This is a bit of a hack to try to match up with the way mvlearn takes views which in turn is a bit of a hack to match up with sklearn.
-        # Sklearn expects fit(X,y) so if we want multiview X in sklearn functions we need X to be a list
-        if isinstance(views[0], list) and views[1] is None:
-            views = views[0]
-
-    n_views = len(views)
-    if n_views < 2:
-        raise ValueError("Require at least 2 views")
-
-    views = [
-        check_array(view, allow_nd=False, copy=copy, accept_sparse=accept_sparse)
-        for view in views
-    ]
-
-    if not len(set([view.shape[0] for view in views])) == 1:
-        msg = "All views must have the same number of samples"
-        raise ValueError(msg)
-
-    return views
 
 
 def _process_parameter(parameter_name: str, parameter, default, n_views: int):
     if parameter is None:
         parameter = [default] * n_views
     elif not isinstance(parameter, (list, tuple)):
         parameter = [parameter] * n_views
@@ -50,15 +20,15 @@
             f"len({parameter_name})={len(parameter)}"
         )
 
 
 def _check_converged_weights(weights, view_index):
     """check the converged weights are not zero."""
     if np.linalg.norm(weights) <= 0:
-        raise ValueError(
+        warnings.warn(
             f"All result weights are zero in view {view_index}. "
             "Try less regularisation or another initialisation"
         )
 
 
 def _check_Parikh2014(mus, lams, views):
     """Return index of the view which the data not matching the condition
@@ -67,15 +37,15 @@
         i
         for i, (mu, lam, view) in enumerate(zip(mus, lams, views))
         if mu < lam / np.linalg.norm(view) ** 2
     ]
     if failed_check:
         raise ValueError(
             "mu, lam, view not matching condition specified "
-            "from Parikh 2014 (mu<lam/frobenius(X)**2)."
+            "from Parikh 2014 (mu<lam/frobenius(views)**2)."
             "Index of view(s) not meeting the condition: "
             f"{failed_check}."
         )
 
 
 def _check_batch_size(batch_size, latent_dimensions):
     """check batch size greater than number of latent dimensions and warn user otherwise"""
```

### Comparing `cca_zoo-1.9.1/setup.py` & `cca_zoo-2.0.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,38 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-with open("./requirements/basic.txt", "r") as f:
+with open("requirements.txt", "r") as f:
     REQUIRED_PACKAGES = f.read()
 
-EXTRA_PACKAGES = {}
-with open("./requirements/deep.txt", "r") as f:
-    EXTRA_PACKAGES['deep'] = f.read()
-with open("./requirements/probabilistic.txt", "r") as f:
-    EXTRA_PACKAGES['probabilistic'] = f.read()
+EXTRA_PACKAGES = {
+    "deep": ["torch", "torchvision", "pytorch-lightning"],
+    "probabilistic": ["jax", "numpyro", "arviz"],
+}
+EXTRA_PACKAGES["all"] = EXTRA_PACKAGES["deep"] + EXTRA_PACKAGES["probabilistic"]
 
 setup(
-    name='cca_zoo',
-    version='1.9.1',
+    name="cca_zoo",
+    version="2.0.0",
     include_package_data=True,
-    keywords='cca',
+    keywords="cca",
     packages=find_packages(),
-    url='https://github.com/jameschapman19/cca_zoo',
-    license='MIT',
-    author='jameschapman',
+    url="https://github.com/jameschapman19/cca_zoo",
+    license="MIT",
+    author="jameschapman",
     description=(
-        'Canonical Correlation Analysis Zoo: CCA, GCCA, MCCA, DCCA, DGCCA, DVCCA, DCCAE, KCCA and regularised variants including sparse CCA , ridge CCA and elastic CCA'
+        "Canonical Correlation Analysis Zoo: A collection of Regularized, Deep Learning based, Kernel, and Probabilistic methods in a scikit-learn style framework"
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
-    author_email='james.chapman.19@ucl.ac.uk',
-    python_requires='>=3.6',
+    author_email="james.chapman.19@ucl.ac.uk",
+    python_requires=">=3.8",
     install_requires=REQUIRED_PACKAGES,
     extras_require=EXTRA_PACKAGES,
-    test_suite='test',
+    test_suite="test",
     tests_require=[],
 )
+
+with open("requirements.txt", "r") as f:
+    REQUIRED_PACKAGES = f.read()
```

