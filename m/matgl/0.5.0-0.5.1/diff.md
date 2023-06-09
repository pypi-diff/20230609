# Comparing `tmp/matgl-0.5.0.tar.gz` & `tmp/matgl-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.5.0.tar", last modified: Fri Jun  9 03:19:42 2023, max compression
+gzip compressed data, was "matgl-0.5.1.tar", last modified: Fri Jun  9 15:25:44 2023, max compression
```

## Comparing `matgl-0.5.0.tar` & `matgl-0.5.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.687366 matgl-0.5.0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     8184 2023-06-09 03:19:42.687224 matgl-0.5.0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     6987 2023-06-09 03:18:50.000000 matgl-0.5.0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.676673 matgl-0.5.0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      162 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.677632 matgl-0.5.0/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.0/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4007 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/apps/pes.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.678029 matgl-0.5.0/matgl/apps/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/apps/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2355 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/apps/tests/test_pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     1467 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.678368 matgl-0.5.0/matgl/data/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-07 18:46:06.000000 matgl-0.5.0/matgl/data/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.678590 matgl-0.5.0/matgl/data/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/data/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      412 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/data/tests/test_transformer.py
--rw-r--r--   0 shyue      (501) staff       (20)     1978 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/data/transformer.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.679060 matgl-0.5.0/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.0/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15940 2023-06-06 19:23:57.000000 matgl-0.5.0/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5317 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.679464 matgl-0.5.0/matgl/ext/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/ext/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1126 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/ext/tests/test_ase.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.680169 matgl-0.5.0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5280 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11015 2023-06-06 20:59:11.000000 matgl-0.5.0/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.680758 matgl-0.5.0/matgl/graph/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.5.0/matgl/graph/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/tests/test_compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/tests/test_converters.py
--rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 16:48:15.000000 matgl-0.5.0/matgl/graph/tests/test_data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.682441 matgl-0.5.0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2047 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3573 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2247 2023-06-06 19:25:00.000000 matgl-0.5.0/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6123 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3572 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16522 2023-06-06 19:27:50.000000 matgl-0.5.0/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3976 2023-06-06 19:29:16.000000 matgl-0.5.0/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3691 2023-06-06 20:17:54.000000 matgl-0.5.0/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.683800 matgl-0.5.0/matgl/layers/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/layers/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      852 2023-05-07 18:00:44.000000 matgl-0.5.0/matgl/layers/tests/test_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     1493 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     1731 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_basis.py
--rw-r--r--   0 shyue      (501) staff       (20)     2489 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     3653 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_core_and_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)     7915 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_graph_conv.py
--rw-r--r--   0 shyue      (501) staff       (20)     4906 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     4284 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.684487 matgl-0.5.0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    10127 2023-06-06 19:38:32.000000 matgl-0.5.0/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9181 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     1773 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/_wrappers.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.685086 matgl-0.5.0/matgl/models/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1888 2023-06-06 14:14:17.000000 matgl-0.5.0/matgl/models/tests/test_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     2473 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/tests/test_megnet.py
--rw-r--r--   0 shyue      (501) staff       (20)      588 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/tests/test_wrapper.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.686117 matgl-0.5.0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      809 2023-05-07 18:00:44.000000 matgl-0.5.0/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)     8680 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)    16776 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.0/matgl/utils/sb_roots.npy
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.687019 matgl-0.5.0/matgl/utils/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     1052 2023-05-07 18:00:44.000000 matgl-0.5.0/matgl/utils/tests/test_cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)      686 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/tests/test_io.py
--rw-r--r--   0 shyue      (501) staff       (20)     4052 2023-06-08 03:49:57.000000 matgl-0.5.0/matgl/utils/tests/test_maths.py
--rw-r--r--   0 shyue      (501) staff       (20)     4102 2023-06-06 19:17:16.000000 matgl-0.5.0/matgl/utils/tests/test_training.py
--rw-r--r--   0 shyue      (501) staff       (20)    12203 2023-06-06 19:49:36.000000 matgl-0.5.0/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.677410 matgl-0.5.0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     8184 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     1868 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       46 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2639 2023-06-06 13:40:32.000000 matgl-0.5.0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-09 03:19:42.687410 matgl-0.5.0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2144 2023-06-06 13:40:32.000000 matgl-0.5.0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.958579 matgl-0.5.1/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.1/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     8467 2023-06-09 15:25:44.958408 matgl-0.5.1/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     7310 2023-06-09 15:25:13.000000 matgl-0.5.1/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.946812 matgl-0.5.1/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      337 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.947702 matgl-0.5.1/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.1/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4008 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/apps/pes.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.948188 matgl-0.5.1/matgl/apps/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/apps/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2355 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/apps/tests/test_pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2029 2023-06-09 14:52:44.000000 matgl-0.5.1/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.948563 matgl-0.5.1/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-07 18:46:06.000000 matgl-0.5.1/matgl/data/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.948914 matgl-0.5.1/matgl/data/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/data/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      724 2023-06-09 03:29:05.000000 matgl-0.5.1/matgl/data/tests/test_transformer.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2653 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.949597 matgl-0.5.1/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.1/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15782 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5318 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.950015 matgl-0.5.1/matgl/ext/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/ext/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1126 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/ext/tests/test_ase.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.951002 matgl-0.5.1/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.1/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5285 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11705 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.951703 matgl-0.5.1/matgl/graph/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.5.1/matgl/graph/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/graph/tests/test_compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/graph/tests/test_converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 16:48:15.000000 matgl-0.5.1/matgl/graph/tests/test_data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.953256 matgl-0.5.1/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2051 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3567 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2250 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6124 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3576 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16673 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3983 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3694 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.954604 matgl-0.5.1/matgl/layers/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/layers/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      852 2023-05-07 18:00:44.000000 matgl-0.5.1/matgl/layers/tests/test_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1493 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1731 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2489 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3653 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_core_and_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7915 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_graph_conv.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4906 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4284 2023-06-06 13:40:31.000000 matgl-0.5.1/matgl/layers/tests/test_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.955394 matgl-0.5.1/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10129 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9181 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1774 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.955984 matgl-0.5.1/matgl/models/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1888 2023-06-06 14:14:17.000000 matgl-0.5.1/matgl/models/tests/test_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2473 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/tests/test_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)      588 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/models/tests/test_wrapper.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.957246 matgl-0.5.1/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.1/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      811 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9495 2023-06-09 14:54:15.000000 matgl-0.5.1/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16792 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.1/matgl/utils/sb_roots.npy
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.958091 matgl-0.5.1/matgl/utils/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/utils/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1052 2023-05-07 18:00:44.000000 matgl-0.5.1/matgl/utils/tests/test_cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)      686 2023-06-09 03:18:50.000000 matgl-0.5.1/matgl/utils/tests/test_io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4052 2023-06-08 03:49:57.000000 matgl-0.5.1/matgl/utils/tests/test_maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4102 2023-06-06 19:17:16.000000 matgl-0.5.1/matgl/utils/tests/test_training.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12848 2023-06-09 14:09:11.000000 matgl-0.5.1/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 15:25:44.947492 matgl-0.5.1/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     8467 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     1868 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       41 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-09 15:25:44.000000 matgl-0.5.1/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2551 2023-06-09 14:09:11.000000 matgl-0.5.1/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-09 15:25:44.958624 matgl-0.5.1/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     1901 2023-06-09 15:24:51.000000 matgl-0.5.1/setup.py
```

### Comparing `matgl-0.5.0/LICENSE` & `matgl-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/PKG-INFO` & `matgl-0.5.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,8 @@
-Metadata-Version: 2.1
-Name: matgl
-Version: 0.5.0
-Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
-Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
-Author-email: ongsp@eng.ucsd.edu
-Maintainer: Shyue Ping Ong
-Maintainer-email: ongsp@eng.ucsd.edu
-Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Chemistry
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Physics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Description-Content-Type: text/markdown
-Provides-Extra: munch
-Provides-Extra: pymatgen
-License-File: LICENSE
-
-# matGL
+# MatGL (Materials Graph Library)
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
 ## Table of Contents
@@ -55,18 +29,21 @@
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 ## Status
 
-- Jun 7 2023: Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
+Major milestones are summarized below. Full change log is provided [here](https://materialsvirtuallab.github.io/matgl/changes).
+- v0.5.1 (Jun 9 2023): Model versioning implemented.
+- v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
+- v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
-- Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
-- Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+- v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
+  bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ## MEGNet
 
@@ -117,15 +94,15 @@
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
 implemented convenience method:
 
 ```python
 import matgl
-model = matgl.load_model(<name>)
+model = matgl.load_model("<model_name>")
 ```
 
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
@@ -134,15 +111,17 @@
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-More examples are available [here](examples).
+## Example notebooks
+
+Primary usage documentation will be done via Jupyter notes, which are available [here](examples).
 
 ## Docs
 
 <http://materialsvirtuallab.github.io/matgl>
 
 ## References
```

### Comparing `matgl-0.5.0/README.md` & `matgl-0.5.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,32 @@
-# matGL
+Metadata-Version: 2.1
+Name: matgl
+Version: 0.5.1
+Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
+Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
+Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
+Maintainer: Shyue Ping Ong
+Maintainer-email: ongsp@ucsd.edu
+Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Scientific/Engineering :: Chemistry
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# MatGL (Materials Graph Library)
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
 ## Table of Contents
@@ -29,18 +53,21 @@
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 ## Status
 
-- Jun 7 2023: Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
+Major milestones are summarized below. Full change log is provided [here](https://materialsvirtuallab.github.io/matgl/changes).
+- v0.5.1 (Jun 9 2023): Model versioning implemented.
+- v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
+- v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
-- Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
-- Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+- v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
+  bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ## MEGNet
 
@@ -91,15 +118,15 @@
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
 implemented convenience method:
 
 ```python
 import matgl
-model = matgl.load_model(<name>)
+model = matgl.load_model("<model_name>")
 ```
 
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
@@ -108,15 +135,17 @@
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-More examples are available [here](examples).
+## Example notebooks
+
+Primary usage documentation will be done via Jupyter notes, which are available [here](examples).
 
 ## Docs
 
 <http://materialsvirtuallab.github.io/matgl>
 
 ## References
```

### Comparing `matgl-0.5.0/matgl/apps/pes.py` & `matgl-0.5.1/matgl/apps/pes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Implementation of Interatomic Potentials
+Implementation of Interatomic Potentials.
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 from torch import nn
```

### Comparing `matgl-0.5.0/matgl/apps/tests/test_pes.py` & `matgl-0.5.1/matgl/apps/tests/test_pes.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/data/transformer.py` & `matgl-0.5.1/matgl/data/transformer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Module implementing various data transformers for PyTorch
+Module implementing various data transformers for PyTorch.
 """
 from __future__ import annotations
 
 import abc
 
 import torch
 
@@ -45,34 +45,34 @@
     Performs a scaling of the data by centering to the mean and dividing by the standard deviation.
     """
 
     def __init__(self, mean: float, std: float):
         """
         Args:
             mean: Mean of the data
-            std: Standard deviation of the data
+            std: Standard deviation of the data.
         """
         self.mean = mean
         self.std = std
 
     def transform(self, data):
         """
-        Scale the data.
+        z-score the data by subtracting the mean and dividing by the standard deviation.
 
         Args:
             data: Input data
 
         Returns:
             Scaled data
         """
         return (data - self.mean) / self.std
 
     def inverse_transform(self, data):
         """
-        Invert the scaling
+        Invert the scaling.
 
         Args:
             data: Scaled data
 
         Returns:
             Unscaled data
         """
@@ -80,16 +80,53 @@
 
     def __repr__(self):
         return f"Normalizer: Mean={self.mean}, Std: {self.std}"
 
     @classmethod
     def from_data(cls, data):
         """
-        Create Normalizer from data
+        Create Normalizer from data.
+
         Args:
-            data: Input data
+            data: Input data.
 
         Returns:
             Normalizer
         """
         data = torch.tensor(data)
         return Normalizer(torch.mean(data), torch.std(data))
+
+
+class LogTransformer(Transformer):
+    """
+    Performs a natural log of the data.
+    """
+
+    def __init__(self):
+        pass
+
+    def transform(self, data):
+        """
+        Take the log of the data.
+
+        Args:
+            data: Input data
+
+        Returns:
+            Scaled data
+        """
+        return torch.log(data)
+
+    def inverse_transform(self, data):
+        """
+        Invert the log (exp).
+
+        Args:
+            data: Input data
+
+        Returns:
+            exp(data)
+        """
+        return torch.exp(data)
+
+    def __repr__(self):
+        return "LogTransformer"
```

### Comparing `matgl-0.5.0/matgl/ext/ase.py` & `matgl-0.5.1/matgl/ext/ase.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         state_attr = [0.0, 0.0]
         g.edata["pbc_offshift"] = torch.matmul(tensor(images), tensor(lattice_matrix))
         return g, state_attr
 
 
 class M3GNetCalculator(Calculator):
     """
-    M3GNet calculator based on ase Calculator
+    M3GNet calculator based on ase Calculator.
     """
 
     implemented_properties = ["energy", "free_energy", "forces", "stress", "hessian"]
 
     def __init__(
         self,
         potential: Potential,
@@ -172,15 +172,15 @@
             self.results.update(stress=stresses.detach().cpu().numpy() * self.stress_weight)
         if self.compute_hessian:
             self.results.update(hessian=hessians.detach().cpu().numpy())
 
 
 class Relaxer:
     """
-    Relaxer is a class for structural relaxation
+    Relaxer is a class for structural relaxation.
     """
 
     def __init__(
         self,
         potential: Potential = None,
         state_attr: torch.tensor = None,
         optimizer: Optimizer | str = "FIRE",
@@ -191,15 +191,15 @@
         Args:
             potential (Potential): a M3GNet potential, a str path to a saved model or a short name for saved model
                 that comes with M3GNet distribution
             state_attr (torch.tensor): State attr.
             optimizer (str or ase Optimizer): the optimization algorithm.
                 Defaults to "FIRE"
             relax_cell (bool): whether to relax the lattice cell
-            stress_weight (float): the stress weight for relaxation
+            stress_weight (float): the stress weight for relaxation.
         """
         if isinstance(optimizer, str):
             optimizer_obj = OPTIMIZERS.get(optimizer, None)
         elif optimizer is None:
             raise ValueError("Optimizer cannot be None")
         else:
             optimizer_obj = optimizer
@@ -255,72 +255,65 @@
             "trajectory": obs,
         }
 
 
 class TrajectoryObserver:
     """
     Trajectory observer is a hook in the relaxation process that saves the
-    intermediate structures
+    intermediate structures.
     """
 
-    def __init__(self, atoms: Atoms):
+    def __init__(self, atoms: Atoms) -> None:
         """
         Args:
-            atoms (Atoms): the structure to observe
+            atoms (Atoms): the structure to observe.
         """
         self.atoms = atoms
         self.energies: list[float] = []
         self.forces: list[np.ndarray] = []
         self.stresses: list[np.ndarray] = []
         self.atom_positions: list[np.ndarray] = []
         self.cells: list[np.ndarray] = []
 
-    def __call__(self):
+    def __call__(self) -> None:
         """
-        The logic for saving the properties of an Atoms during the relaxation
-        Returns:
+        The logic for saving the properties of an Atoms during the relaxation.
         """
         self.energies.append(self.compute_energy())
         self.forces.append(self.atoms.get_forces())
         self.stresses.append(self.atoms.get_stress())
         self.atom_positions.append(self.atoms.get_positions())
         self.cells.append(self.atoms.get_cell()[:])
 
     def compute_energy(self) -> float:
-        """
-        calculate the energy, here we just use the potential energy
-        Returns:
-        """
+        """Calculate the potential energy."""
         energy = self.atoms.get_potential_energy()
         return energy
 
-    def save(self, filename: str):
+    def save(self, filename: str) -> None:
         """
         Save the trajectory to file
         Args:
-            filename (str): filename to save the trajectory
-        Returns:
+            filename (str): filename to save the trajectory.
         """
-        with open(filename, "wb") as f:
-            pickle.dump(
-                {
-                    "energy": self.energies,
-                    "forces": self.forces,
-                    "stresses": self.stresses,
-                    "atom_positions": self.atom_positions,
-                    "cell": self.cells,
-                    "atomic_number": self.atoms.get_atomic_numbers(),
-                },
-                f,
-            )
+        out = {
+            "energy": self.energies,
+            "forces": self.forces,
+            "stresses": self.stresses,
+            "atom_positions": self.atom_positions,
+            "cell": self.cells,
+            "atomic_number": self.atoms.get_atomic_numbers(),
+        }
+        with open(filename, "wb") as file:
+            pickle.dump(out, file)
 
 
 class MolecularDynamics:
     """
-    Molecular dynamics class
+    Molecular dynamics class.
     """
 
     def __init__(
         self,
         atoms: Atoms,
         potential: Potential,
         state_attr: torch.tensor = None,
@@ -349,15 +342,15 @@
             pressure (float): pressure in eV/A^3
             taut (float): time constant for Berendsen temperature coupling
             taup (float): time constant for pressure coupling
             compressibility_au (float): compressibility of the material in A^3/eV
             trajectory (str or Trajectory): Attach trajectory object
             logfile (str): open this file for recording MD outputs
             loginterval (int): write to log file every interval steps
-            append_trajectory (bool): Whether to append to prev trajectory
+            append_trajectory (bool): Whether to append to prev trajectory.
         """
         if isinstance(atoms, (Structure, Molecule)):
             atoms = AseAtomsAdaptor().get_atoms(atoms)
         self.atoms = atoms
         self.atoms.set_calculator(M3GNetCalculator(potential=potential, state_attr=state_attr))
 
         if taut is None:
@@ -429,25 +422,24 @@
         self.trajectory = trajectory
         self.logfile = logfile
         self.loginterval = loginterval
         self.timestep = timestep
 
     def run(self, steps: int):
         """
-        Thin wrapper of ase MD run
+        Thin wrapper of ase MD run.
+
         Args:
             steps (int): number of MD steps
-        Returns:
-
         """
         self.dyn.run(steps)
 
     def set_atoms(self, atoms: Atoms):
         """
         Set new atoms to run MD
         Args:
-            atoms (Atoms): new atoms for running MD
+            atoms (Atoms): new atoms for running MD.
         """
         calculator = self.atoms.calc
         self.atoms = atoms
         self.dyn.atoms = atoms
         self.dyn.atoms.set_calculator(calculator)
```

### Comparing `matgl-0.5.0/matgl/ext/pymatgen.py` & `matgl-0.5.1/matgl/ext/pymatgen.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from pymatgen.core import Element, Molecule, Structure
 from pymatgen.optimization.neighbors import find_points_in_spheres
 
 from matgl.graph.converters import GraphConverter
 
 
 def get_element_list(train_structures: list[Structure | Molecule]) -> tuple[str]:
-    """Get the dictionary containing elements in the training set for atomic features
+    """Get the dictionary containing elements in the training set for atomic features.
 
     Args:
         train_structures: pymatgen Molecule/Structure object
 
     Returns:
         Tuple of elements covered in training set
     """
```

### Comparing `matgl-0.5.0/matgl/ext/tests/test_ase.py` & `matgl-0.5.1/matgl/ext/tests/test_ase.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/graph/compute.py` & `matgl-0.5.1/matgl/graph/compute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-Computing various graph based operations
+Computing various graph based operations.
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 
 
 def compute_3body(g: dgl.DGLGraph):
     """
-    Calculate the three body indices from pair atom indices
+    Calculate the three body indices from pair atom indices.
 
     Args:
         g: DGL graph
 
     Returns:
         l_g: DGL graph containing three body information from graph
         triple_bond_indices (np.ndarray): bond indices that form three-body
@@ -70,15 +70,15 @@
     l_g.ndata["n_triple_ij"] = n_triple_ij
     n_triple_s = torch.tensor(n_triple_s, dtype=torch.int64)
     return l_g, triple_bond_indices, n_triple_ij, n_triple_i, n_triple_s
 
 
 def compute_pair_vector_and_distance(g: dgl.DGLGraph):
     """
-    Calculate bond vectors and distances using dgl graphs
+    Calculate bond vectors and distances using dgl graphs.
 
     Args:
     g: DGL graph
 
     Returns:
     bond_vec (torch.tensor): bond distance between two atoms
     bond_dist (torch.tensor): vector from src node to dst node
@@ -93,15 +93,15 @@
     bond_dist = torch.norm(bond_vec, dim=1)
 
     return bond_vec, bond_dist
 
 
 def compute_theta_and_phi(edges: dgl.udf.EdgeBatch):
     """
-    Calculate bond angle Theta and Phi using dgl graphs
+    Calculate bond angle Theta and Phi using dgl graphs.
 
     Args:
     edges: DGL graph edges
 
     Returns:
     cos_theta: torch.tensor
     phi: torch.tensor
@@ -115,15 +115,15 @@
         "phi": torch.zeros_like(cosine_theta),
         "triple_bond_lengths": edges.dst["bond_dist"],
     }
 
 
 def create_line_graph(g_batched: dgl.DGLGraph, threebody_cutoff: float):
     """
-    Calculate the three body indices from pair atom indices
+    Calculate the three body indices from pair atom indices.
 
     Args:
         g_batched: Batched DGL graph
         threebody_cutoff (float): cutoff for three-body interactions
 
     Returns:
         l_g: DGL graph containing three body information from graph
```

### Comparing `matgl-0.5.0/matgl/graph/converters.py` & `matgl-0.5.1/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/graph/data.py` & `matgl-0.5.1/matgl/graph/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Tools to construct a dataset of DGL graphs
+Tools to construct a dataset of DGL graphs.
 """
 from __future__ import annotations
 
 import json
 import os
 from typing import TYPE_CHECKING, Callable
 
@@ -20,26 +20,26 @@
 
 if TYPE_CHECKING:
     from matgl.graph.converters import GraphConverter
 
 
 def collate_fn(batch):
     """
-    Merge a list of dgl graphs to form a batch
+    Merge a list of dgl graphs to form a batch.
     """
     graphs, labels, state_attr = map(list, zip(*batch))
     g = dgl.batch(graphs)
     labels = torch.tensor(labels, dtype=torch.float32)
     state_attr = torch.stack(state_attr)
     return g, labels, state_attr
 
 
 def collate_fn_efs(batch):
     """
-    Merge a list of dgl graphs to form a batch
+    Merge a list of dgl graphs to form a batch.
     """
     graphs, line_graphs, state_attr, energies, forces, stresses = map(list, zip(*batch))
     g = dgl.batch(graphs)
     l_g = dgl.batch(line_graphs)
     e = torch.tensor(energies, dtype=torch.float32)
     f = torch.vstack(forces)
     s = torch.vstack(stresses)
@@ -53,22 +53,31 @@
     collate_fn: Callable,
     batch_size: int,
     num_workers: int,
     use_ddp: bool = False,
     pin_memory: bool = False,
     test_data: dgl.data.utils.Subset | None = None,
     generator: torch.Generator | None = None,
-):
-    """
-    Dataloader for MEGNet training
+) -> tuple[GraphDataLoader, ...]:
+    """Dataloader for MEGNet training.
+
     Args:
-    train_data: training data
-    val_data: validation data
-    test_data: testing data
-    collate_fn:
+        train_data (dgl.data.utils.Subset): Training dataset.
+        val_data (dgl.data.utils.Subset): Validation dataset.
+        collate_fn (Callable): Collate function.
+        batch_size (int): Batch size.
+        num_workers (int): Number of workers.
+        use_ddp (bool, optional): Whether to use DDP. Defaults to False.
+        pin_memory (bool, optional): Whether to pin memory. Defaults to False.
+        test_data (dgl.data.utils.Subset | None, optional): Test dataset. Defaults to None.
+        generator (torch.Generator | None, optional): Random number generator. Defaults to None.
+
+    Returns:
+        tuple[GraphDataLoader, ...]: Train, validation and test data loaders. Test data
+            loader is None if test_data is None.
     """
     train_loader = GraphDataLoader(
         train_data,
         batch_size=batch_size,
         shuffle=True,
         collate_fn=collate_fn,
         num_workers=num_workers,
@@ -96,15 +105,15 @@
         )
         return train_loader, val_loader, test_loader
     return train_loader, val_loader
 
 
 class MEGNetDataset(DGLDataset):
     """
-    Create a dataset including dgl graphs
+    Create a dataset including dgl graphs.
     """
 
     def __init__(
         self,
         structures: list,
         labels: list,
         label_name: str,
@@ -123,15 +132,15 @@
         label_name: label name
         converter: Transformer for converting structures to DGL graphs, e.g., Pmg2Graph.
         initial: initial distance for Gaussian expansions
         final: final distance for Gaussian expansions
         num_centers: number of Gaussian functions
         width: width of Gaussian functions
         name: Name of dataset
-        graph_labels: graph attributes either integers and floating point numbers
+        graph_labels: graph attributes either integers and floating point numbers.
         """
         self.converter = converter
         self.structures = structures
         self.labels = torch.FloatTensor(labels)
         self.label_name = label_name
         self.initial = initial
         self.final = final
@@ -148,15 +157,15 @@
             :filename: Name of file storing dgl graphs
         Returns: True if file exists.
         """
         return os.path.exists(filename)
 
     def process(self) -> tuple:
         """
-        Convert Pymatgen structure into dgl graphs
+        Convert Pymatgen structure into dgl graphs.
         """
         num_graphs = self.labels.shape[0]
         self.graphs = []
         self.state_attr = []
         bond_expansion = BondExpansion(
             rbf_type="Gaussian", initial=self.initial, final=self.final, num_centers=self.num_centers, width=self.width
         )
@@ -178,47 +187,47 @@
         return self.graphs, self.state_attr
 
     def save(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
         """
         Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
-        :filename_state_attr: Name of file storing graph attrs
+        :filename_state_attr: Name of file storing graph attrs.
         """
         labels_with_key = {self.label_name: self.labels}
         save_graphs(filename, self.graphs, labels_with_key)
         torch.save(self.state_attr, filename_state_attr)
 
     def load(self, filename: str = "dgl_graph.bin", filename_state_attr: str = "state_attr.pt"):
         """
         Load dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
-        :filename: Name of file storing state attrs
+        :filename: Name of file storing state attrs.
         """
         self.graphs, label_dict = load_graphs(filename)
         self.label = torch.stack([label_dict[key] for key in self.label_keys], dim=1)
         self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
         """
-        Get graph and label with idx
+        Get graph and label with idx.
         """
         return self.graphs[idx], self.labels[idx], self.state_attr[idx]
 
     def __len__(self):
         """
-        Get size of dataset
+        Get size of dataset.
         """
         return len(self.graphs)
 
 
 class M3GNetDataset(DGLDataset):
     """
-    Create a dataset including dgl graphs
+    Create a dataset including dgl graphs.
     """
 
     def __init__(
         self,
         structures: list,
         energies: list,
         forces: list,
@@ -233,15 +242,15 @@
         structures: Pymatgen strutcure
         energies: Target energies
         forces: Target forces
         stresses: Target stresses
         converter: dgl graph converter
         threebody_cutoff: cutoff for three body
         name: name of dataset
-        graph_labels: state attributes
+        graph_labels: state attributes.
         """
         self.converter = converter
         self.structures = structures
         self.energies = energies
         self.forces = forces
         self.threebody_cutoff = threebody_cutoff
         self.stresses = np.zeros(len(self.energies)) if stresses is None else stresses
@@ -255,15 +264,15 @@
             :filename: Name of file storing dgl graphs
         Returns: True if file exists.
         """
         return os.path.exists(filename)
 
     def process(self) -> tuple:
         """
-        Convert Pymatgen structure into dgl graphs
+        Convert Pymatgen structure into dgl graphs.
         """
         num_graphs = len(self.energies)
         self.graphs = []
         self.line_graphs = []
         self.state_attr = []
         for idx in trange(num_graphs):
             structure = self.structures[idx]
@@ -291,15 +300,15 @@
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
     ):
         """
         Save dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
-        :filename_state_attr: Name of file storing graph attrs
+        :filename_state_attr: Name of file storing graph attrs.
         """
         labels_with_key = {"energies": self.energies, "forces": self.forces, "stresses": self.stresses}
         save_graphs(filename, self.graphs)
         save_graphs(filename_line_graph, self.line_graphs)
         torch.save(self.state_attr, filename_state_attr)
         with open("labels.json", "w") as file:
             file.write("".join(str(labels_with_key).split("\n")))
@@ -310,36 +319,36 @@
         filename_line_graph: str = "dgl_line_graph.bin",
         filename_state_attr: str = "state_attr.pt",
     ):
         """
         Load dgl graphs
         Args:
         :filename: Name of file storing dgl graphs
-        :filename: Name of file storing state attrs
+        :filename: Name of file storing state attrs.
         """
         self.graphs = load_graphs(filename)
         self.line_graphs = load_graphs(filename_line_graph)
         with open("labels.json") as file:
             labels = json.load(file)
         self.energies = labels["energies"]
         self.forces = labels["forces"]
         self.stresses = labels["stresses"]
         self.state_attr = torch.load("state_attr.pt")
 
     def __getitem__(self, idx: int):
         """
-        Get graph and label with idx
+        Get graph and label with idx.
         """
         return (
             self.graphs[idx],
             self.line_graphs[idx],
             self.state_attr[idx],
             self.energies[idx],
             torch.tensor(self.forces[idx]),
             torch.tensor(self.stresses[idx]),
         )
 
     def __len__(self):
         """
-        Get size of dataset
+        Get size of dataset.
         """
         return len(self.graphs)
```

### Comparing `matgl-0.5.0/matgl/graph/tests/test_compute.py` & `matgl-0.5.1/matgl/graph/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/graph/tests/test_converters.py` & `matgl-0.5.1/matgl/graph/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/graph/tests/test_data.py` & `matgl-0.5.1/matgl/graph/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/__init__.py` & `matgl-0.5.1/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/_activations.py` & `matgl-0.5.1/matgl/layers/_activations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
-Custom activation functions
+Custom activation functions.
 """
 from __future__ import annotations
 
 import math
 
 import torch
 from torch import nn
 
 
 class SoftPlus2(nn.Module):
     """
     SoftPlus2 activation function:
     out = log(exp(x)+1) - log(2)
-    softplus function that is 0 at x=0, the implementation aims at avoiding overflow
+    softplus function that is 0 at x=0, the implementation aims at avoiding overflow.
     """
 
     def __init__(self) -> None:
         """Initializes the SoftPlus2 class."""
         super().__init__()
         self.ssp = nn.Softplus()
 
@@ -35,27 +35,27 @@
 
 
 class SoftExponential(nn.Module):
     """
     Soft exponential activation.
     When x < 0, SoftExponential(x,alpha) = -log(1-alpha(x+alpha))/alpha
     When x = 0, SoftExponential(x,alpha) = 0
-    When x > 0, SoftExponential(x,alpha) = (exp(alpha*x)-1)/alpha + alpha
+    When x > 0, SoftExponential(x,alpha) = (exp(alpha*x)-1)/alpha + alpha.
 
 
     References:
         - See related paper:
         https://arxiv.org/pdf/1602.01321.pdf
 
     """
 
     def __init__(self, alpha: float = None):
         """
         Args:
-            alpha (float): adjustable Torch parameter during the training
+            alpha (float): adjustable Torch parameter during the training.
         """
         super().__init__()
 
         # initialize alpha
         if alpha is None:
             self.alpha = nn.Parameter(torch.tensor(0.0))
         else:
```

### Comparing `matgl-0.5.0/matgl/layers/_atom_ref.py` & `matgl-0.5.1/matgl/layers/_atom_ref.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 """
-atomic energy offset. Used for predicting extensive properties.
+Atomic energy offset. Used for predicting extensive properties.
 """
 from __future__ import annotations
 
 import dgl
 import numpy as np
 import torch
 from pymatgen.core import Molecule, Structure
 from torch import nn
 
 
 class AtomRef(nn.Module):
-    """
-    Get total property offset for a system:
-    """
+    """Get total property offset for a system."""
 
     def __init__(
         self,
         property_offset: np.array,  # type: ignore
     ) -> None:
         """
         Args:
         -----------
-        property_offset (np.array): a array of elemental property offset
+        property_offset (np.array): a array of elemental property offset.
         """
         super().__init__()
         self.property_offset = torch.tensor(property_offset)
         self.max_z = self.property_offset.size(dim=0)
 
     def get_feature_matrix(self, structs_or_graphs: list, element_list: tuple[str]) -> np.typing.NDArray:
         """
-        Get the number of atoms for different elements in the structure
+        Get the number of atoms for different elements in the structure.
 
         Args:
         structs_or_graphs (list): a list of pymatgen Structure or dgl graph
         element_list: a dictionary containing element types in the training set
 
         Returns:
         features (np.array): a matrix (num_structures, num_elements)
@@ -48,28 +46,28 @@
                 one_hot_vecs = s.ndata["attr"]
                 atomic_numbers = ((one_hot_vecs == 1).nonzero(as_tuple=True)[0]).tolist()
             features[i] = np.bincount(atomic_numbers, minlength=self.max_z)
         return features
 
     def fit(self, structs_or_graphs: list, element_list: tuple[str], properties: np.typing.NDArray) -> None:
         """
-        Fit the elemental reference values for the properties
+        Fit the elemental reference values for the properties.
 
         Args:
             structs_or_graphs: pymatgen Structures or dgl graphs
             element_list (tuple): a list of element types
             properties (np.ndarray): array of extensive properties
         """
         features = self.get_feature_matrix(structs_or_graphs, element_list)
         self.property_offset = np.linalg.pinv(features.T.dot(features)).dot(features.T.dot(properties))
         self.property_offset = torch.tensor(self.property_offset)
 
     def forward(self, g: dgl.DGLGraph, state_attr: torch.tensor | None = None):
         """
-        Get the total property offset for a system
+        Get the total property offset for a system.
 
         Args:
         g: a batch of dgl graphs
         state_attr: state attributes
 
         Returns:
         offset_per_graph:
```

### Comparing `matgl-0.5.0/matgl/layers/_bond.py` & `matgl-0.5.1/matgl/layers/_bond.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Generate bond features based on spherical bessel functions or gaussian expansion
+Generate bond features based on spherical bessel functions or gaussian expansion.
 """
 from __future__ import annotations
 
 import torch
 from torch import nn
 
 from matgl.utils.maths import GaussianExpansion, SphericalBesselFunction
@@ -32,15 +32,15 @@
             max_n (int): order of radial part
             cutoff (float): cutoff radius
             rbf_type (str): type of radial basis function .i.e. either "SphericalBessel" or 'Gaussian'
             smooth (bool): whether apply the smooth version of spherical bessel functions or not
             initial (float): initial point for gaussian expansion
             final (float): final point for gaussian expansion
             num_centers (int): Number of centers for gaussian expansion.
-            width (float): width of gaussian function
+            width (float): width of gaussian function.
         """
         super().__init__()
 
         self.max_n = max_n
         self.cutoff = cutoff
         self.max_l = max_l
         self.smooth = smooth
@@ -55,15 +55,15 @@
         elif rbf_type == "Gaussian":
             self.rbf = GaussianExpansion(initial, final, num_centers, width)  # type: ignore
         else:
             raise Exception("undefined rbf_type, please use SphericalBessel or Gaussian instead.")
 
     def forward(self, bond_dist: torch.tensor):
         """
-        Forward
+        Forward.
 
         Args:
         bond_dist: Bond distance
 
         Return:
         bond_basis: Radial basis functions
         """
```

### Comparing `matgl-0.5.0/matgl/layers/_core.py` & `matgl-0.5.1/matgl/layers/_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     @property
     def depth(self) -> int:
         """Returns depth of MLP."""
         return self._depth
 
     @property
     def in_features(self) -> int:
-        """Return input features of MLP"""
+        """Return input features of MLP."""
         return self.layers[0].in_features
 
     @property
     def out_features(self) -> int:
         """Returns output features of MLP."""
         for layer in reversed(self.layers):
             if isinstance(layer, Linear):
```

### Comparing `matgl-0.5.0/matgl/layers/_embedding.py` & `matgl-0.5.1/matgl/layers/_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-Embedding node, edge and optional state attributes
+Embedding node, edge and optional state attributes.
 """
 from __future__ import annotations
 
 import torch
 from torch import nn
 
 from matgl.layers._core import MLP
 
 
 class EmbeddingBlock(nn.Module):
     """
-    Embedding block for generating node, bond and state features
+    Embedding block for generating node, bond and state features.
     """
 
     def __init__(
         self,
         degree_rbf: int,
         activation: nn.Module,
         dim_node_embedding: int,
@@ -33,15 +33,15 @@
             activation (nn.Module): activation type
             dim_node_embedding (int): dimensionality of node features
             dim_edge_embedding (int): dimensionality of edge features
             dim_state_feats: dimensionality of state features
             ntypes_node: number of node labels
             include_state: Whether to include state embedding
             ntypes_state: number of state labels
-            dim_state_embedding: dimensionality of state embedding
+            dim_state_embedding: dimensionality of state embedding.
         """
         super().__init__()
         self.include_state = include_state
         self.ntypes_state = ntypes_state
         self.dim_node_embedding = dim_node_embedding
         self.dim_edge_embedding = dim_edge_embedding
         self.dim_state_feats = dim_state_feats
@@ -54,15 +54,15 @@
             self.layer_node_embedding = nn.Embedding(ntypes_node, dim_node_embedding)
         if dim_edge_embedding is not None:
             dim_edges = [degree_rbf, dim_edge_embedding]
             self.layer_edge_embedding = MLP(dim_edges, activation=activation, activate_last=True)
 
     def forward(self, node_attr, edge_attr, state_attr):
         """
-        Output embedded features
+        Output embedded features.
 
         Args:
         node_attr: node attribute
         edge_attr: edge attribute
         state_attr: state attribute
 
         Returns:
```

### Comparing `matgl-0.5.0/matgl/layers/_graph_convolution.py` & `matgl-0.5.1/matgl/layers/_graph_convolution.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 
 from __future__ import annotations
 
 import dgl
 import dgl.function as fn
 import torch
-from torch import nn
+from torch import Tensor, nn
 from torch.nn import Dropout, Identity, Module
 
 from matgl.layers._core import MLP, GatedMLP
 
 
 class MEGNetGraphConv(Module):
     """
@@ -37,21 +37,24 @@
     @staticmethod
     def from_dims(
         edge_dims: list[int],
         node_dims: list[int],
         state_dims: list[int],
         activation: Module,
     ) -> MEGNetGraphConv:
-        """
-        TODO: Add docs.
-        :param edge_dims: dense layers for message functions
-        :param node_dims: dense layers for node update functions
-        :param state_dims: dense layers for state update functions
-        :param activation: activation function
-        :return:
+        """Create a MEGNet graph convolution layer from dimensions.
+
+        Args:
+            edge_dims (list[int]): Edge dimensions.
+            node_dims (list[int]): Node dimensions.
+            state_dims (list[int]): State dimensions.
+            activation (Module): Activation function.
+
+        Returns:
+            MEGNetGraphConv: MEGNet graph convolution layer.
         """
         # TODO(marcel): Softplus doesn't exactly match paper's SoftPlus2
         # TODO(marcel): Should we activate last?
         edge_update = MLP(edge_dims, activation, activate_last=True)
         node_update = MLP(node_dims, activation, activate_last=True)
         attr_update = MLP(state_dims, activation, activate_last=True)
         return MEGNetGraphConv(edge_update, node_update, attr_update)
@@ -61,41 +64,41 @@
         vj = edges.dst["v"]
         u = edges.src["u"]
         eij = edges.data.pop("e")
         inputs = torch.hstack([vi, vj, eij, u])
         mij = {"mij": self.edge_func(inputs)}
         return mij
 
-    def edge_update_(self, graph: dgl.DGLGraph) -> torch.Tensor:
+    def edge_update_(self, graph: dgl.DGLGraph) -> Tensor:
         """
         Perform edge update.
 
         :param graph: Input graph
         :return: Output tensor for edges.
         """
         graph.apply_edges(self._edge_udf)
         graph.edata["e"] = graph.edata.pop("mij")
         return graph.edata["e"]
 
-    def node_update_(self, graph: dgl.DGLGraph) -> torch.Tensor:
+    def node_update_(self, graph: dgl.DGLGraph) -> Tensor:
         """
         Perform node update.
 
         :param graph: Input graph
         :return: Output tensor for nodes.
         """
         graph.update_all(fn.copy_e("e", "e"), fn.mean("e", "ve"))
         ve = graph.ndata.pop("ve")
         v = graph.ndata.pop("v")
         u = graph.ndata.pop("u")
         inputs = torch.hstack([v, ve, u])
         graph.ndata["v"] = self.node_func(inputs)
         return graph.ndata["v"]
 
-    def state_update_(self, graph: dgl.DGLGraph, state_attrs: torch.Tensor) -> torch.Tensor:
+    def state_update_(self, graph: dgl.DGLGraph, state_attrs: Tensor) -> Tensor:
         """
         Perform attribute (global state) update.
 
         :param graph: Input graph
         :param state_attrs: Input attributes
         :return: Output tensor for attributes
         """
@@ -106,18 +109,18 @@
         inputs = torch.hstack([state_attrs.squeeze(), u_edge, u_vertex])
         state_attr = self.state_func(inputs)
         return state_attr
 
     def forward(
         self,
         graph: dgl.DGLGraph,
-        edge_feat: torch.Tensor,
-        node_feat: torch.Tensor,
-        state_attr: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        edge_feat: Tensor,
+        node_feat: Tensor,
+        state_attr: Tensor,
+    ) -> tuple[Tensor, Tensor, Tensor]:
         """
         Perform sequence of edge->node->attribute updates.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_attr: Graph attributes (global state)
@@ -146,15 +149,15 @@
         """
         TODO: Add docs.
         :param dims: architecture of dense layers before graph convolution
         :param conv_hiddens: architecture of graph convolution
         :param act: activation type
         :param dropout: Randomly zeroes some elements in the input tensor with given probability (0 < x < 1) according
             to a Bernoulli distribution
-        :param skip: residual block
+        :param skip: residual block.
         """
         super().__init__()
         self.has_dense = len(dims) > 1
         self.activation = act
         conv_dim = dims[-1]
         out_dim = conv_hiddens[-1]
 
@@ -182,25 +185,29 @@
         self.dropout = Dropout(dropout) if dropout else None
         # TODO(marcel): should this be an 1D dropout
         self.skip = skip
 
     def forward(
         self,
         graph: dgl.DGLGraph,
-        edge_feat: torch.Tensor,
-        node_feat: torch.Tensor,
-        state_attr: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
-        """
-        TODO: Add docs.
-        :param graph:
-        :param edge_feat:
-        :param node_feat:
-        :param state_attr:
-        :return:
+        edge_feat: Tensor,
+        node_feat: Tensor,
+        state_attr: Tensor,
+    ) -> tuple[Tensor, Tensor, Tensor]:
+        """MEGNetBlock forward pass.
+
+        Args:
+            graph (dgl.DGLGraph): A DGLGraph.
+            edge_feat (Tensor): Edge features.
+            node_feat (Tensor): Node features.
+            state_attr (Tensor): Graph attributes (global state).
+
+        Returns:
+            tuple[Tensor, Tensor, Tensor]: Updated (edge features,
+                node features, graph attributes)
         """
         inputs = (edge_feat, node_feat, state_attr)
         edge_feat = self.edge_func(edge_feat)
         node_feat = self.node_func(node_feat)
         state_attr = self.state_func(state_attr)
 
         edge_feat, node_feat, state_attr = self.conv(graph, edge_feat, node_feat, state_attr)
@@ -235,15 +242,15 @@
         """
         Parameters:
         include_state (bool): Whether including state
         edge_update_func (Module): Update function for edges (Eq. 4)
         edge_weight_func (Module): Weight function for radial basis functions (Eq. 4)
         node_update_func (Module): Update function for nodes (Eq. 5)
         node_weight_func (Module): Weight function for radial basis functions (Eq. 5)
-        attr_update_func (Module): Update function for state feats (Eq. 6)
+        attr_update_func (Module): Update function for state feats (Eq. 6).
         """
         super().__init__()
         self.include_states = include_states
         self.edge_update_func = edge_update_func
         self.edge_weight_func = edge_weight_func
         self.node_update_func = node_update_func
         self.node_weight_func = node_weight_func
@@ -255,15 +262,15 @@
         include_states,
         edge_dims: list[int],
         node_dims: list[int],
         state_dims: list[int] | None,
         activation: Module,
     ) -> M3GNetGraphConv:
         """
-        M3GNetGraphConv initialization
+        M3GNetGraphConv initialization.
 
         Args:
             degree (int): max_n*max_l
             include_states (bool): whether including state or not
             edge_dims (list): NN architecture for edge update function
             node_dims (list): NN architecture for node update function
             state_dims (list): NN architecture for state update function
@@ -280,15 +287,15 @@
         attr_update_func = MLP(state_dims, activation, activate_last=True) if include_states else None  # type: ignore
         return M3GNetGraphConv(
             include_states, edge_update_func, edge_weight_func, node_update_func, node_weight_func, attr_update_func
         )
 
     def _edge_udf(self, edges: dgl.udf.EdgeBatch):
         """
-        Edge update functions
+        Edge update functions.
 
         Args:
         edges (DGL graph): edges in dgl graph
 
         Returns:
         mij: message passing between node i and j
         """
@@ -299,29 +306,29 @@
         eij = edges.data.pop("e")
         rbf = edges.data["rbf"]
         rbf = rbf.float()
         inputs = torch.hstack([vi, vj, eij, u]) if self.include_states else torch.hstack([vi, vj, eij])
         mij = {"mij": self.edge_update_func(inputs) * self.edge_weight_func(rbf)}
         return mij
 
-    def edge_update_(self, graph: dgl.DGLGraph) -> torch.Tensor:
+    def edge_update_(self, graph: dgl.DGLGraph) -> Tensor:
         """
         Perform edge update.
 
         Args:
         graph: DGL graph
 
         Returns:
         edge_update: edge features update
         """
         graph.apply_edges(self._edge_udf)
         edge_update = graph.edata.pop("mij")
         return edge_update
 
-    def node_update_(self, graph: dgl.DGLGraph, state_attr: torch.Tensor) -> torch.Tensor:
+    def node_update_(self, graph: dgl.DGLGraph, state_attr: Tensor) -> Tensor:
         """
         Perform node update.
 
         Args:
             graph: DGL graph
             state_attr: State attributes
 
@@ -341,15 +348,15 @@
         else:
             inputs = torch.hstack([vi, vj, eij])
         graph.edata["mess"] = self.node_update_func(inputs) * self.node_weight_func(rbf)
         graph.update_all(fn.copy_e("mess", "mess"), fn.sum("mess", "ve"))
         node_update = graph.ndata.pop("ve")
         return node_update
 
-    def state_update_(self, graph: dgl.DGLGraph, state_attrs: torch.Tensor) -> torch.Tensor:
+    def state_update_(self, graph: dgl.DGLGraph, state_attrs: Tensor) -> Tensor:
         """
         Perform attribute (global state) update.
 
         Args:
             graph: DGL graph
             state_attrs: graph features
 
@@ -361,18 +368,18 @@
         inputs = torch.hstack([u, uv])
         state_attr = self.state_update_func(inputs)  # type: ignore
         return state_attr
 
     def forward(
         self,
         graph: dgl.DGLGraph,
-        edge_feat: torch.Tensor,
-        node_feat: torch.Tensor,
-        state_attr: torch.Tensor,
-    ) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor]:
+        edge_feat: Tensor,
+        node_feat: Tensor,
+        state_attr: Tensor,
+    ) -> tuple[Tensor, Tensor, Tensor]:
         """
         Perform sequence of edge->node->states updates.
 
         :param graph: Input graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_attr: Graph attributes (global state)
@@ -450,17 +457,17 @@
             )
 
         self.dropout = Dropout(dropout) if dropout else None
 
     def forward(
         self,
         graph: dgl.DGLGraph,
-        edge_feat: torch.tensor,
-        node_feat: torch.tensor,
-        state_feat: torch.tensor,
+        edge_feat: Tensor,
+        node_feat: Tensor,
+        state_feat: Tensor,
     ) -> tuple:
         """
         :param graph: DGL graph
         :param edge_feat: Edge features
         :param node_feat: Node features
         :param state_attr: State features
         :return: A tuple of updated features
```

### Comparing `matgl-0.5.0/matgl/layers/_readout.py` & `matgl-0.5.1/matgl/layers/_readout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 """
-Readout layer for M3GNet
+Readout layer for M3GNet.
 """
 
 from __future__ import annotations
 
 import dgl
 import torch
 from dgl.nn import Set2Set
 from torch import nn
 
 from matgl.layers._core import EdgeSet2Set, GatedMLP
 
 
 class Set2SetReadOut(nn.Module):
     """
-    The Set2Set readout function
+    The Set2Set readout function.
     """
 
     def __init__(
         self,
         num_steps: int,
         num_layers: int,
         field: str,
     ):
         """
         Args:
             num_steps (int): Number of LSTM steps
             num_layers (int): Number of layers.
-            field (str): Field of graph to perform the readout
+            field (str): Field of graph to perform the readout.
         """
         super().__init__()
         self.field = field
         self.num_steps = num_steps
         self.num_layers = num_layers
 
     def forward(self, g: dgl.DGLGraph):
@@ -53,26 +53,26 @@
     This could be summing up the atoms or bonds, or taking the mean, etc.
     """
 
     def __init__(self, op: str = "mean", field: str = "node_feat"):
         """
         Args:
             op (str): op for the reduction
-            field (str): Field of graph to perform the reduction
+            field (str): Field of graph to perform the reduction.
         """
         super().__init__()
         self.op = op
         self.field = field
 
     def forward(self, g: dgl.DGLGraph):
         """
         Args:
             g: DGL graph
         Returns:
-            torch.tensor
+            torch.tensor.
         """
         if self.field == "node_feat":
             reduced_tensor = dgl.readout_nodes(g, feat="node_feat", op=self.op)
         elif self.field == "edge_feat":
             reduced_tensor = dgl.readout_edges(g, feat="edge_feat", op=self.op)
         return reduced_tensor
 
@@ -83,27 +83,27 @@
     """
 
     def __init__(self, in_feats: int, dims: list[int], num_targets: int):
         """
         Args:
            in_feats: input features (nodes)
            dims: NN architecture for Gated MLP
-           num_targets: number of target properties
+           num_targets: number of target properties.
         """
         super().__init__()
         self.in_feats = in_feats
         self.dims = [in_feats, *dims, num_targets]
         self.gated = GatedMLP(in_feats=in_feats, dims=self.dims, activate_last=False)
 
     def forward(self, g: dgl.DGLGraph):
         """
         Args:
             g: DGL graph
         Returns:
-            atomic_properties: torch.tensor
+            atomic_properties: torch.tensor.
         """
         atomic_properties = self.gated(g.ndata["node_feat"])
         return atomic_properties
 
 
 class WeightedReadOutPair(nn.Module):
     """
```

### Comparing `matgl-0.5.0/matgl/layers/_three_body.py` & `matgl-0.5.1/matgl/layers/_three_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     get_segment_indices_from_n,
     scatter_sum,
 )
 
 
 class SphericalBesselWithHarmonics(nn.Module):
     """
-    Expansion of basis using Spherical Bessel and Harmonics
+    Expansion of basis using Spherical Bessel and Harmonics.
     """
 
     def __init__(self, max_n: int, max_l: int, cutoff: float, use_smooth: bool, use_phi: bool):
         """
         :param max_n: Degree of radial basis functions
         :param max_l: Degree of angular basis functions
         :param cutoff: Cutoff sphere
@@ -50,15 +50,15 @@
         sbf = self.sbf(line_graph.edata["triple_bond_lengths"])
         shf = self.shf(line_graph.edata["cos_theta"], line_graph.edata["phi"])
         return combine_sbf_shf(sbf, shf, max_n=self.max_n, max_l=self.max_l, use_phi=self.use_phi)
 
 
 class ThreeBodyInteractions(nn.Module):
     """
-    Include 3D interactions to the bond update
+    Include 3D interactions to the bond update.
     """
 
     def __init__(self, update_network_atom: nn.Module, update_network_bond: nn.Module, **kwargs):
         r"""
         Args:
             update_network_atom: MLP for node features in Eq.2
             update_network_bond: Gated-MLP for edge features in Eq.3
@@ -80,15 +80,15 @@
         """
         Args:
             graph: dgl graph
             line_graph: line graph.
             three_basis: three body basis expansion
             three_cutoff: cutoff radius
             node_feat: node features
-            edge_feat: edge features
+            edge_feat: edge features.
         """
         end_atom_index = torch.gather(graph.edges()[1], 0, line_graph.edges()[1].to(torch.int64))
         atoms = self.update_network_atom(node_feat)
         end_atom_index = torch.unsqueeze(end_atom_index, 1)
         atoms = torch.squeeze(atoms[end_atom_index])
         basis = three_basis * atoms
         three_cutoff = torch.unsqueeze(three_cutoff, dim=1)
```

### Comparing `matgl-0.5.0/matgl/layers/tests/test_activations.py` & `matgl-0.5.1/matgl/layers/tests/test_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_atom_ref.py` & `matgl-0.5.1/matgl/layers/tests/test_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_basis.py` & `matgl-0.5.1/matgl/layers/tests/test_basis.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_bond.py` & `matgl-0.5.1/matgl/layers/tests/test_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_core_and_embedding.py` & `matgl-0.5.1/matgl/layers/tests/test_core_and_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_graph_conv.py` & `matgl-0.5.1/matgl/layers/tests/test_graph_conv.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_readout.py` & `matgl-0.5.1/matgl/layers/tests/test_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/layers/tests/test_three_body.py` & `matgl-0.5.1/matgl/layers/tests/test_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/models/_m3gnet.py` & `matgl-0.5.1/matgl/models/_m3gnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Core M3GNet model
+Core M3GNet model.
 """
 from __future__ import annotations
 
 import logging
 
 import dgl
 import torch
@@ -33,15 +33,15 @@
 from matgl.utils.io import IOMixIn
 
 logger = logging.getLogger(__file__)
 
 
 class M3GNet(nn.Module, IOMixIn):
     """
-    The main M3GNet model
+    The main M3GNet model.
     """
 
     def __init__(
         self,
         element_types: tuple[str],
         dim_node_embedding: int = 64,
         dim_edge_embedding: int = 64,
```

### Comparing `matgl-0.5.0/matgl/models/_megnet.py` & `matgl-0.5.1/matgl/models/_megnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/models/_wrappers.py` & `matgl-0.5.1/matgl/models/_wrappers.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from matgl.data.transformer import Transformer
 from matgl.utils.io import IOMixIn
 
 
 class TransformedTargetModel(nn.Module, IOMixIn):
     """
     A model where the target is first transformed prior to training and the reverse transformation is performed for
-    predictions. This is modelled after scikit-learn's TransformedTargetRegressor
+    predictions. This is modelled after scikit-learn's TransformedTargetRegressor.
     """
 
     def __init__(self, model: nn.Module, target_transformer: Transformer):
         """
         Args:
             model: Input model
             target_transformer: Transformer for target.
```

### Comparing `matgl-0.5.0/matgl/models/tests/test_m3gnet.py` & `matgl-0.5.1/matgl/models/tests/test_m3gnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/models/tests/test_megnet.py` & `matgl-0.5.1/matgl/models/tests/test_megnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/models/tests/test_wrapper.py` & `matgl-0.5.1/matgl/models/tests/test_wrapper.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/utils/cutoff.py` & `matgl-0.5.1/matgl/utils/cutoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 
 
 def polynomial_cutoff(r, cutoff: float):
     """
     Polynomial cutoff function
     Args:
         r (torch.tensor): radius distance tensor
-        cutoff (float): cutoff distance
+        cutoff (float): cutoff distance.
 
     Returns: polynomial cutoff functions
 
     """
     ratio = r / cutoff
     return torch.where(r <= cutoff, 1 - 6 * ratio**5 + 15 * ratio**4 - 10 * ratio**3, 0.0)
 
 
 def cosine_cutoff(r: torch.Tensor, cutoff: float) -> torch.Tensor:
     """
     Cosine cutoff function
     Args:
         r (torch.tensor): radius distance tensor
-        cutoff (float): cutoff distance
+        cutoff (float): cutoff distance.
 
     Returns: cosine cutoff functions
 
     """
     return torch.where(r <= cutoff, 0.5 * (torch.cos(pi * r / cutoff) + 1), 0.0)
```

### Comparing `matgl-0.5.0/matgl/utils/io.py` & `matgl-0.5.1/matgl/utils/io.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 """
 from __future__ import annotations
 
 import inspect
 import json
 import logging
 import os
+import warnings
 from pathlib import Path
 
 import requests
 import torch
 
-from matgl.config import MATGL_CACHE, PRETRAINED_MODELS_BASE_URL
+from matgl.config import MATGL_CACHE, MODEL_VERSION, PRETRAINED_MODELS_BASE_URL
 
 logger = logging.getLogger(__file__)
 
 
 class IOMixIn:
     """
     Mixin class for model saving and loading.
@@ -35,15 +36,20 @@
         d = {k: v for k, v in locals.items() if k in args and k not in ("self", "__class__")}
         if kwargs is not None:
             d.update(kwargs)
 
         # If one of the args is a subclass of IOMixIn, we will serialize that class.
         for k, v in d.items():
             if issubclass(v.__class__, IOMixIn):
-                d[k] = {"@class": v.__class__.__name__, "@module": v.__class__.__module__, "init_args": v._init_args}
+                d[k] = {
+                    "@class": v.__class__.__name__,
+                    "@module": v.__class__.__module__,
+                    "@model_version": MODEL_VERSION,
+                    "init_args": v._init_args,
+                }
         self._init_args = d
 
     def save(self, path: str | Path = ".", metadata: dict | None = None, makedirs: bool = True):
         """
         Save model to a directory. Three files will be saved.
         - path/model.pt, which contains the torch serialized model args.
         - path/state.pt, which contains the saved state_dict from the model.
@@ -61,14 +67,15 @@
             os.makedirs(path, exist_ok=True)
 
         torch.save(self._init_args, path / "model.pt")  # type: ignore
         torch.save(self.state_dict(), path / "state.pt")  # type: ignore
         d = {
             "@class": self.__class__.__name__,
             "@module": self.__class__.__module__,
+            "@model_version": MODEL_VERSION,
             "metadata": metadata,
             "kwargs": self._init_args,
         }  # type: ignore
         with open(path / "model.json", "w") as f:
             json.dump(d, f, default=lambda o: str(o), indent=4)
 
     @classmethod
@@ -216,10 +223,20 @@
                 f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
             ) from None
 
     with open(fpaths["model.json"]) as f:
         d = json.load(f)
         modname = d["@module"]
         classname = d["@class"]
+        model_version = d.get("@model_version", 0)
+        if model_version < MODEL_VERSION:
+            warnings.warn(
+                "Incompatible model version detected! The code will continue to load the model but it is "
+                "recommended that you provide a path to an updated model, increment your @model_version in model.json "
+                "if you are confident that the changes are not problematic, or clear your ~/.matgl cache using "
+                '`python -c "import matgl; matgl.clear_cache()"`',
+                DeprecationWarning,
+                stacklevel=2,
+            )
         mod = __import__(modname, globals(), locals(), [classname], 0)
         cls_ = getattr(mod, classname)
         return cls_.load(path, **kwargs)
```

### Comparing `matgl-0.5.0/matgl/utils/maths.py` & `matgl-0.5.1/matgl/utils/maths.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 SPHERICAL_BESSEL_ROOTS = torch.tensor(np.load(os.path.join(CWD, "sb_roots.npy")))
 
 
 class GaussianExpansion(nn.Module):
     r"""
     Gaussian Radial Expansion.
     The bond distance is expanded to a vector of shape [m],
-    where m is the number of Gaussian basis centers
+    where m is the number of Gaussian basis centers.
     """
 
     def __init__(
         self,
         initial: float = 0.0,
         final: float = 4.0,
         num_centers: int = 20,
@@ -81,15 +81,15 @@
 def spherical_bessel_roots(max_l: int, max_n: int):
     """
     Calculate the spherical Bessel roots. The n-th root of the l-th
     spherical bessel function is the `[l, n]` entry of the return matrix.
     The calculation is based on the fact that the n-root for l-th
     spherical Bessel function `j_l`, i.e., `z_{j, n}` is in the range
     `[z_{j-1,n}, z_{j-1, n+1}]`. On the other hand we know precisely the
-    roots for j0, i.e., sinc(x)
+    roots for j0, i.e., sinc(x).
 
     Args:
         max_l: max order of spherical bessel function
         max_n: max number of roots
     Returns: root matrix of size [max_l, max_n]
     """
     temp_zeros = np.arange(1, max_l + max_n + 1) * pi  # j0
@@ -104,15 +104,15 @@
         temp_zeros = np.array(roots_temp)
         roots.append(temp_zeros[:max_n])
     return np.array(roots)
 
 
 class SphericalBesselFunction:
     """
-    Calculate the spherical Bessel function based on sympy + pytorch implementations
+    Calculate the spherical Bessel function based on sympy + pytorch implementations.
     """
 
     def __init__(self, max_l: int, max_n: int = 5, cutoff: float = 5.0, smooth: bool = False):
         """
         Args:
             max_l: int, max order (excluding l)
             max_n: int, max number of roots used in each l
@@ -145,15 +145,15 @@
     @lru_cache(maxsize=128)
     def _calculate_smooth_symbolic_funcs(self) -> list:
         return _get_lambda_func(max_n=self.max_n, cutoff=self.cutoff)
 
     def __call__(self, r):
         """
         Args:
-            r: torch.tensor, distance tensor, 1D
+            r: torch.tensor, distance tensor, 1D.
 
 
         Returns: [n, max_n * max_l] spherical Bessel function results
 
         """
         if self.smooth:
             return self._call_smooth_sbf(r)
@@ -177,30 +177,30 @@
             )
         return torch.cat(results, axis=1)
 
     @staticmethod
     def rbf_j0(r, cutoff: float = 5.0, max_n: int = 3):
         """
         Spherical Bessel function of order 0, ensuring the function value
-        vanishes at cutoff
+        vanishes at cutoff.
 
         Args:
             r: torch.tensor pytorch tensors
             cutoff: float, the cutoff radius
             max_n: int max number of basis
         Returns: basis function expansion using first spherical Bessel function
         """
         n = (torch.arange(1, max_n + 1)).type(dtype=torch.float32)[None, :]
         r = r[:, None]
         return sqrt(2.0 / cutoff) * torch.sin(n * pi / cutoff * r) / r
 
 
 def _y00(theta, phi):
     r"""
-    Spherical Harmonics with `l=m=0`
+    Spherical Harmonics with `l=m=0`.
 
     ..math::
         Y_0^0 = \frac{1}{2} \sqrt{\frac{1}{\pi}}
 
     Args:
         theta: torch.tensor, the azimuthal angle
         phi: torch.tensor, the polar angle
@@ -213,23 +213,23 @@
 
 def _conjugate(x):
     return torch.conj(x)
 
 
 class SphericalHarmonicsFunction:
     """
-    Spherical Harmonics function
+    Spherical Harmonics function.
     """
 
     def __init__(self, max_l: int, use_phi: bool = True):
         """
         Args:
             max_l: int, max l (excluding l)
             use_phi: bool, whether to use the polar angle. If not,
-                the function will compute `Y_l^0`
+                the function will compute `Y_l^0`.
         """
         self.max_l = max_l
         self.use_phi = use_phi
         funcs = []
         theta, phi = sympy.symbols("theta phi")
         for lval in range(self.max_l):
             m_list = range(-lval, lval + 1) if self.use_phi else [0]  # type: ignore
@@ -243,15 +243,15 @@
         self.funcs = [sympy.lambdify([costheta, phi], i, [{"conjugate": _conjugate}, torch]) for i in self.orig_funcs]
         self.funcs[0] = _y00
 
     def __call__(self, costheta, phi=None):
         """
         Args:
             costheta: Cosine of the azimuthal angle
-            phi: torch.tensor, the polar angle
+            phi: torch.tensor, the polar angle.
 
         Returns: [n, m] spherical harmonic results, where n is the number
             of angles. The column is arranged following
             `[Y_0^0, Y_1^{-1}, Y_1^{0}, Y_1^1, Y_2^{-2}, ...]`
         """
         # costheta = torch.tensor(costheta, dtype=torch.complex64)
         # phi = torch.tensor(phi, dtype=torch.complex64)
@@ -270,15 +270,15 @@
         start += b
     indices = torch.cat(indices, axis=0)
     return torch.index_select(array, 1, indices)
 
 
 def combine_sbf_shf(sbf, shf, max_n: int, max_l: int, use_phi: bool):
     """
-    Combine the spherical Bessel function and the spherical Harmonics function
+    Combine the spherical Bessel function and the spherical Harmonics function.
 
     For the spherical Bessel function, the column is ordered by
         [n=[0, ..., max_n-1], n=[0, ..., max_n-1], ...], max_l blocks,
 
     For the spherical Harmonics function, the column is ordered by
         [m=[0], m=[-1, 0, 1], m=[-2, -1, 0, 1, 2], ...] max_l blocks, and each
         block has 2*l + 1
@@ -318,15 +318,15 @@
 
 
 def spherical_bessel_smooth(r, cutoff: float = 5.0, max_n: int = 10):
     """
     This is an orthogonal basis with first
     and second derivative at the cutoff
     equals to zero. The function was derived from the order 0 spherical Bessel
-    function, and was expanded by the different zero roots
+    function, and was expanded by the different zero roots.
 
     Ref:
         https://arxiv.org/pdf/1907.02374.pdf
 
     Args:
         r: torch.tensor distance tensor
         cutoff: float, cutoff radius
@@ -392,15 +392,15 @@
         gnr.append(1 / sympy.sqrt(dn[i]) * (fnr[i] + sympy.sqrt(en[i] / dn[i - 1]) * gnr[-1]))
     return [sympy.lambdify([r], sympy.simplify(i), torch) for i in gnr]
 
 
 def get_segment_indices_from_n(ns):
     """
     Get segment indices from number array. For example if
-    ns = [2, 3], then the function will return [0, 0, 1, 1, 1]
+    ns = [2, 3], then the function will return [0, 0, 1, 1, 1].
 
     Args:
         ns: torch.tensor, the number of atoms/bonds array
 
     Returns:
         object:
 
@@ -408,15 +408,15 @@
     """
     a = torch.arange(ns.size(dim=0))
     return a.repeat_interleave(ns, dim=0)
 
 
 def get_range_indices_from_n(ns):
     """
-    Give ns = [2, 3], return [0, 1, 0, 1, 2]
+    Give ns = [2, 3], return [0, 1, 0, 1, 2].
 
     Args:
         ns: torch.tensor, the number of atoms/bonds array
 
     Returns: range indices
     """
     max_n = torch.max(ns)
@@ -444,29 +444,29 @@
     """
     return torch.repeat_interleave(ns, n, dim=0)
 
 
 def broadcast_states_to_bonds(g, state_feat):
     """
     Broadcast state attributes of shape [Ns, Nstate] to
-    bond attributes shape [Nb, Nstate]
+    bond attributes shape [Nb, Nstate].
 
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
     """
     return state_feat.repeat((g.num_edges(), 1))
 
 
 def broadcast_states_to_atoms(g, state_feat):
     """
     Broadcast state attributes of shape [Ns, Nstate] to
-    bond attributes shape [Nb, Nstate]
+    bond attributes shape [Nb, Nstate].
 
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
 
@@ -502,15 +502,15 @@
     """
     Segment fraction
     Args:
         data (torch.tensor): original data
         segment_ids (torch.tensor): segment ids
         num_segments (torch.tensor): number of segments
     Returns:
-        data (torch.tensor): data after fraction
+        data (torch.tensor): data after fraction.
     """
     segment_sum = scatter_sum(input_tensor=data, segment_ids=segment_ids, dim=0, num_segments=num_segments)
     sums = torch.gather(segment_sum, 0, segment_ids)
     return torch.div(data, sums)
 
 
 def broadcast(input_tensor: torch.tensor, target_tensor: torch.tensor, dim: int):
```

### Comparing `matgl-0.5.0/matgl/utils/sb_roots.npy` & `matgl-0.5.1/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/utils/tests/test_cutoff.py` & `matgl-0.5.1/matgl/utils/tests/test_cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/utils/tests/test_io.py` & `matgl-0.5.1/matgl/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/utils/tests/test_maths.py` & `matgl-0.5.1/matgl/utils/tests/test_maths.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/utils/tests/test_training.py` & `matgl-0.5.1/matgl/utils/tests/test_training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/matgl/utils/training.py` & `matgl-0.5.1/matgl/utils/training.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Utils for training MatGL models.
 """
 
 from __future__ import annotations
 
+import math
+
 import dgl
 import numpy as np
 import pytorch_lightning as pl
 import torch
 import torch.nn.functional as F
 import torchmetrics
 from torch import nn
@@ -40,15 +42,15 @@
             prog_bar=True,
         )
 
         return results["Total_Loss"]
 
     def on_train_epoch_end(self):
         """
-        Step scheduler every epoch
+        Step scheduler every epoch.
         """
         sch = self.lr_schedulers()
         sch.step()
 
     def validation_step(self, batch: tuple, batch_idx: int):
         """
         Args:
@@ -77,15 +79,15 @@
             on_epoch=True,
             on_step=False,
             prog_bar=True,
         )
 
     def configure_optimizers(self):
         """
-        Configure optimizers
+        Configure optimizers.
         """
         if self.optimizer is None:
             optimizer = torch.optim.Adam(
                 self.parameters(),
                 lr=self.lr,
                 eps=1e-8,
             )
@@ -105,15 +107,15 @@
             scheduler,
         ]
 
     def on_test_model_eval(self, *args, **kwargs):
         r"""
         Args:
             *args: Pass-through
-            **kwargs: Pass-through
+            **kwargs: Pass-through.
         """
         super().on_test_model_eval(*args, **kwargs)
         torch.set_grad_enabled(True)
 
     def predict_step(self, batch, batch_idx, dataloader_idx=0):
         """
         Args:
@@ -126,15 +128,15 @@
         """
         torch.set_grad_enabled(True)
         return self(batch)
 
 
 class ModelTrainer(TrainerMixin, pl.LightningModule):
     """
-    Trainer for MEGNet and M3GNet models
+    Trainer for MEGNet and M3GNet models.
     """
 
     def __init__(
         self,
         model,
         data_mean=None,
         data_std=None,
@@ -152,15 +154,15 @@
             data_mean: average of training data
             data_std: standard deviation of training data
             loss: loss function used for training
             optimizer: optimizer for training
             scheduler: scheduler for training
             lr: learning rate for training
             decay_steps: number of steps for decaying learning rate
-            decay_alpha: parameter determines the minimum learning rate
+            decay_alpha: parameter determines the minimum learning rate.
         """
         super().__init__()
 
         self.model = model
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
@@ -182,15 +184,15 @@
         self.save_hyperparameters()
 
     def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.tensor | None = None):
         """
         Args:
             g: dgl Graph
             l_g: Line graph
-            state_attr: State attribute
+            state_attr: State attribute.
 
         Returns:
             Model prediction.
         """
         if isinstance(self.model, M3GNet):
             return self.model(g=g, l_g=l_g, state_attr=state_attr)
 
@@ -261,15 +263,15 @@
             data_std: standard deviation of training data
             calc_stress: whether stress calculation is required
             loss: loss function used for training
             optimizer: optimizer for training
             scheduler: scheduler for training
             lr: learning rate for training
             decay_steps: number of steps for decaying learning rate
-            decay_alpha: parameter determines the minimum learning rate
+            decay_alpha: parameter determines the minimum learning rate.
         """
         super().__init__()
 
         self.model = Potential(model=model, element_refs=element_refs, calc_stresses=calc_stress)
 
         self.mae = torchmetrics.MeanAbsoluteError()
         self.rmse = torchmetrics.MeanSquaredError(squared=False)
@@ -294,15 +296,15 @@
         self.save_hyperparameters()
 
     def forward(self, g: dgl.DGLGraph, l_g: dgl.DGLGraph | None = None, state_attr: torch.tensor | None = None):
         """
         Args:
             g: dgl Graph
             l_g: Line graph
-            state_attr: State attr
+            state_attr: State attr.
 
         Returns:
             energy, force, stress, h
         """
         e, f, s, h = self.model(g=g, l_g=l_g, state_attr=state_attr)
         return e, f.float(), s, h
 
@@ -395,7 +397,25 @@
             "Energy_MAE": e_mae,
             "Force_MAE": f_mae,
             "Stress_MAE": s_mae,
             "Energy_RMSE": e_rmse,
             "Force_RMSE": f_rmse,
             "Stress_RMSE": s_rmse,
         }
+
+
+def xavier_init(model: nn.Module) -> None:
+    """Xavier initialization scheme for the model.
+
+    Args:
+        model (nn.Module): The model to be Xavier-initialized.
+    """
+    for name, param in model.named_parameters():
+        if name.endswith(".bias"):
+            param.data.fill_(0)
+        else:
+            if param.dim() < 2:
+                bound = math.sqrt(6) / math.sqrt(param.shape[0] + param.shape[0])
+                param.data.uniform_(-bound, bound)
+            else:
+                bound = math.sqrt(6) / math.sqrt(param.shape[0] + param.shape[1])
+                param.data.uniform_(-bound, bound)
```

### Comparing `matgl-0.5.0/matgl.egg-info/PKG-INFO` & `matgl-0.5.1/matgl.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.5.0
+Version: 0.5.1
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
-Author-email: ongsp@eng.ucsd.edu
+Author-email: t1ko@ucsd.edu, ongsp@ucsd.edu
 Maintainer: Shyue Ping Ong
-Maintainer-email: ongsp@eng.ucsd.edu
+Maintainer-email: ongsp@ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
-Provides-Extra: munch
-Provides-Extra: pymatgen
 License-File: LICENSE
 
-# matGL
+# MatGL (Materials Graph Library)
 
 [![GitHub license](https://img.shields.io/github/license/materialsvirtuallab/matgl)](https://github.com/materialsvirtuallab/matgl/blob/main/LICENSE)
 [![Linting](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Linting/badge.svg)
 [![Testing](https://github.com/materialsvirtuallab/matgl/workflows/Testing%20-%20main/badge.svg)](https://github.com/materialsvirtuallab/matgl/workflows/Testing/badge.svg)
 [![Downloads](https://pepy.tech/badge/matgl)](https://pepy.tech/project/matgl)
 
 ## Table of Contents
@@ -55,18 +53,21 @@
 - Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 ## Status
 
-- Jun 7 2023: Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
+Major milestones are summarized below. Full change log is provided [here](https://materialsvirtuallab.github.io/matgl/changes).
+- v0.5.1 (Jun 9 2023): Model versioning implemented.
+- v0.5.0 (Jun 8 2023): Simplified saving and loading of models. Now models can be loaded with one line of code!
+- v0.4.0 (Jun 7 2023): Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
   available.
-- Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
-- Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
+- v0.1.0 (Feb 16 2023): Initial implementations of M3GNet and MEGNet architectures have been completed. Expect
+  bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
 ## MEGNet
 
@@ -117,15 +118,15 @@
 
 Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
 multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
 implemented convenience method:
 
 ```python
 import matgl
-model = matgl.load_model(<name>)
+model = matgl.load_model("<model_name>")
 ```
 
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
 from pymatgen.core import Lattice, Structure
 import matgl
@@ -134,15 +135,17 @@
 
 # This is the structure obtained from the Materials Project.
 struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
 eform = model.predict_structure(struct)
 print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-More examples are available [here](examples).
+## Example notebooks
+
+Primary usage documentation will be done via Jupyter notes, which are available [here](examples).
 
 ## Docs
 
 <http://materialsvirtuallab.github.io/matgl>
 
 ## References
```

### Comparing `matgl-0.5.0/matgl.egg-info/SOURCES.txt` & `matgl-0.5.1/matgl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matgl-0.5.0/pyproject.toml` & `matgl-0.5.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,14 @@
   "D100",    # Missing docstring in public module
   "D104",    # Missing docstring in public package
   "D105",    # Missing docstring in magic method
   "D107",    # Missing docstring in __init__
   "D200",    # One-line docstring should fit on one line with quotes
   "D205",    # 1 blank line required between summary line and description
   "D212",    # Multi-line docstring summary should start at the first line
-  "D415",    # First line should end with a period, question mark, or exclamation point
   "PLR",     # pylint refactor
   "PLW0603", # Using the global statement to update variables is discouraged
   "PLW2901", # redefined-loop-name
   "RET504",  # unnecessary-assign
   "SIM105",  # Use contextlib.suppress(OSError) instead of try-except-pass
 ]
 pydocstyle.convention = "google"
```

### Comparing `matgl-0.5.0/setup.py` & `matgl-0.5.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 from __future__ import annotations
 
 import os
-import re
 
 import numpy as np
 from setuptools import find_packages, setup
 
 this_dir = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(this_dir, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
-with open("matgl/__init__.py", encoding="utf-8") as fd:
-    for line in fd.readlines():
-        m = re.search('__version__ = "(.*)"', line)
-        if m:
-            version = m.group(1)
-            break
-
 setup(
     name="matgl",
-    version=version,
+    version="0.5.1",
     author="Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong",
-    author_email="ongsp@eng.ucsd.edu",
+    author_email="t1ko@ucsd.edu, ongsp@ucsd.edu",
     maintainer="Shyue Ping Ong",
-    maintainer_email="ongsp@eng.ucsd.edu",
+    maintainer_email="ongsp@ucsd.edu",
     description="MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=[
         "materials",
         "interatomic potential",
         "force field",
@@ -40,20 +32,21 @@
         "deep learning",
     ],
     packages=find_packages(),
     package_data={
         "matgl": ["*.json", "*.md"],
         "matgl.utils": ["*.npy"],
     },
-    include_package_data=True,
-    install_requires=("torch", "dgl"),
-    extras_require={
-        "munch": ["munch"],
-        "pymatgen": ["pymatgen"],
-    },
+    install_requires=(
+        "ase",
+        "dgl",
+        "pymatgen",
+        "pytorch_lightning",
+        "torch",
+    ),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

