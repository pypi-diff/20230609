# Comparing `tmp/matgl-0.4.0.tar.gz` & `tmp/matgl-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matgl-0.4.0.tar", last modified: Tue Jun  6 23:35:35 2023, max compression
+gzip compressed data, was "matgl-0.5.0.tar", last modified: Fri Jun  9 03:19:42 2023, max compression
```

## Comparing `matgl-0.4.0.tar` & `matgl-0.5.0.tar`

### file list

```diff
@@ -1,54 +1,88 @@
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.995392 matgl-0.4.0/
--rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-04-22 15:15:07.000000 matgl-0.4.0/LICENSE
--rw-r--r--   0 shyue      (501) staff       (20)     7749 2023-06-06 23:35:35.995156 matgl-0.4.0/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)     6552 2023-06-06 21:45:12.000000 matgl-0.4.0/README.md
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.988373 matgl-0.4.0/matgl/
--rw-r--r--   0 shyue      (501) staff       (20)      128 2023-06-06 23:32:20.000000 matgl-0.4.0/matgl/__init__.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.989387 matgl-0.4.0/matgl/apps/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:14:12.000000 matgl-0.4.0/matgl/apps/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     3959 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/apps/pes.py
--rw-r--r--   0 shyue      (501) staff       (20)     2768 2023-05-08 21:40:46.000000 matgl-0.4.0/matgl/config.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.990024 matgl-0.4.0/matgl/ext/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:14:12.000000 matgl-0.4.0/matgl/ext/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    15940 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/ext/ase.py
--rw-r--r--   0 shyue      (501) staff       (20)     5317 2023-05-31 00:31:01.000000 matgl-0.4.0/matgl/ext/pymatgen.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.991109 matgl-0.4.0/matgl/graph/
--rw-r--r--   0 shyue      (501) staff       (20)       54 2023-04-22 15:15:07.000000 matgl-0.4.0/matgl/graph/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     5280 2023-05-31 00:31:01.000000 matgl-0.4.0/matgl/graph/compute.py
--rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/converters.py
--rw-r--r--   0 shyue      (501) staff       (20)    11012 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.991707 matgl-0.4.0/matgl/graph/tests/
--rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:22.000000 matgl-0.4.0/matgl/graph/tests/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/tests/test_compute.py
--rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/tests/test_converters.py
--rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/graph/tests/test_data.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.993134 matgl-0.4.0/matgl/layers/
--rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)     2047 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_activations.py
--rw-r--r--   0 shyue      (501) staff       (20)     3573 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_atom_ref.py
--rw-r--r--   0 shyue      (501) staff       (20)     2247 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_bond.py
--rw-r--r--   0 shyue      (501) staff       (20)     6123 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_core.py
--rw-r--r--   0 shyue      (501) staff       (20)     3572 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_embedding.py
--rw-r--r--   0 shyue      (501) staff       (20)    16522 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_graph_convolution.py
--rw-r--r--   0 shyue      (501) staff       (20)     3976 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/layers/_readout.py
--rw-r--r--   0 shyue      (501) staff       (20)     3691 2023-06-06 23:32:04.000000 matgl-0.4.0/matgl/layers/_three_body.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.993667 matgl-0.4.0/matgl/models/
--rw-r--r--   0 shyue      (501) staff       (20)      167 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/models/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)    10127 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/models/_m3gnet.py
--rw-r--r--   0 shyue      (501) staff       (20)     9613 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/models/_megnet.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.994830 matgl-0.4.0/matgl/utils/
--rw-r--r--   0 shyue      (501) staff       (20)       63 2023-04-22 15:15:07.000000 matgl-0.4.0/matgl/utils/__init__.py
--rw-r--r--   0 shyue      (501) staff       (20)      809 2023-05-08 21:40:46.000000 matgl-0.4.0/matgl/utils/cutoff.py
--rw-r--r--   0 shyue      (501) staff       (20)     6638 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/utils/io.py
--rw-r--r--   0 shyue      (501) staff       (20)    17730 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/utils/maths.py
--rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-04-22 15:15:07.000000 matgl-0.4.0/matgl/utils/sb_roots.npy
--rw-r--r--   0 shyue      (501) staff       (20)    12203 2023-06-06 21:45:12.000000 matgl-0.4.0/matgl/utils/training.py
-drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-06 23:35:35.989151 matgl-0.4.0/matgl.egg-info/
--rw-r--r--   0 shyue      (501) staff       (20)     7749 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/PKG-INFO
--rw-r--r--   0 shyue      (501) staff       (20)      992 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/SOURCES.txt
--rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/dependency_links.txt
--rw-r--r--   0 shyue      (501) staff       (20)       46 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/requires.txt
--rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-06 23:35:35.000000 matgl-0.4.0/matgl.egg-info/top_level.txt
--rw-r--r--   0 shyue      (501) staff       (20)     2639 2023-06-06 21:45:12.000000 matgl-0.4.0/pyproject.toml
--rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-06 23:35:35.995441 matgl-0.4.0/setup.cfg
--rw-r--r--   0 shyue      (501) staff       (20)     2144 2023-06-06 21:45:12.000000 matgl-0.4.0/setup.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.687366 matgl-0.5.0/
+-rw-r--r--   0 shyue      (501) staff       (20)     1529 2023-03-24 21:11:48.000000 matgl-0.5.0/LICENSE
+-rw-r--r--   0 shyue      (501) staff       (20)     8184 2023-06-09 03:19:42.687224 matgl-0.5.0/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     6987 2023-06-09 03:18:50.000000 matgl-0.5.0/README.md
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.676673 matgl-0.5.0/matgl/
+-rw-r--r--   0 shyue      (501) staff       (20)      162 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.677632 matgl-0.5.0/matgl/apps/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.0/matgl/apps/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4007 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/apps/pes.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.678029 matgl-0.5.0/matgl/apps/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/apps/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2355 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/apps/tests/test_pes.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1467 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/config.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.678368 matgl-0.5.0/matgl/data/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-07 18:46:06.000000 matgl-0.5.0/matgl/data/__init__.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.678590 matgl-0.5.0/matgl/data/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/data/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      412 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/data/tests/test_transformer.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1978 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/data/transformer.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.679060 matgl-0.5.0/matgl/ext/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:09:52.000000 matgl-0.5.0/matgl/ext/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    15940 2023-06-06 19:23:57.000000 matgl-0.5.0/matgl/ext/ase.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5317 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/ext/pymatgen.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.679464 matgl-0.5.0/matgl/ext/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/ext/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1126 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/ext/tests/test_ase.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.680169 matgl-0.5.0/matgl/graph/
+-rw-r--r--   0 shyue      (501) staff       (20)       54 2023-03-22 18:49:07.000000 matgl-0.5.0/matgl/graph/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5280 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)      538 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)    11015 2023-06-06 20:59:11.000000 matgl-0.5.0/matgl/graph/data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.680758 matgl-0.5.0/matgl/graph/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-05-04 22:28:02.000000 matgl-0.5.0/matgl/graph/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4939 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/tests/test_compute.py
+-rw-r--r--   0 shyue      (501) staff       (20)     5223 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/graph/tests/test_converters.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7731 2023-06-06 16:48:15.000000 matgl-0.5.0/matgl/graph/tests/test_data.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.682441 matgl-0.5.0/matgl/layers/
+-rw-r--r--   0 shyue      (501) staff       (20)      647 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2047 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3573 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2247 2023-06-06 19:25:00.000000 matgl-0.5.0/matgl/layers/_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     6123 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_core.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3572 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16522 2023-06-06 19:27:50.000000 matgl-0.5.0/matgl/layers/_graph_convolution.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3976 2023-06-06 19:29:16.000000 matgl-0.5.0/matgl/layers/_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3691 2023-06-06 20:17:54.000000 matgl-0.5.0/matgl/layers/_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.683800 matgl-0.5.0/matgl/layers/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/layers/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      852 2023-05-07 18:00:44.000000 matgl-0.5.0/matgl/layers/tests/test_activations.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1493 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_atom_ref.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1731 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_basis.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2489 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_bond.py
+-rw-r--r--   0 shyue      (501) staff       (20)     3653 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_core_and_embedding.py
+-rw-r--r--   0 shyue      (501) staff       (20)     7915 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_graph_conv.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4906 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_readout.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4284 2023-06-06 13:40:31.000000 matgl-0.5.0/matgl/layers/tests/test_three_body.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.684487 matgl-0.5.0/matgl/models/
+-rw-r--r--   0 shyue      (501) staff       (20)      189 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)    10127 2023-06-06 19:38:32.000000 matgl-0.5.0/matgl/models/_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     9181 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1773 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/_wrappers.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.685086 matgl-0.5.0/matgl/models/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1888 2023-06-06 14:14:17.000000 matgl-0.5.0/matgl/models/tests/test_m3gnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)     2473 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/tests/test_megnet.py
+-rw-r--r--   0 shyue      (501) staff       (20)      588 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/models/tests/test_wrapper.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.686117 matgl-0.5.0/matgl/utils/
+-rw-r--r--   0 shyue      (501) staff       (20)       63 2023-03-22 18:49:07.000000 matgl-0.5.0/matgl/utils/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)      809 2023-05-07 18:00:44.000000 matgl-0.5.0/matgl/utils/cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)     8680 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/io.py
+-rw-r--r--   0 shyue      (501) staff       (20)    16776 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)   131200 2023-03-22 18:49:07.000000 matgl-0.5.0/matgl/utils/sb_roots.npy
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.687019 matgl-0.5.0/matgl/utils/tests/
+-rw-r--r--   0 shyue      (501) staff       (20)        0 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/tests/__init__.py
+-rw-r--r--   0 shyue      (501) staff       (20)     1052 2023-05-07 18:00:44.000000 matgl-0.5.0/matgl/utils/tests/test_cutoff.py
+-rw-r--r--   0 shyue      (501) staff       (20)      686 2023-06-09 03:18:50.000000 matgl-0.5.0/matgl/utils/tests/test_io.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4052 2023-06-08 03:49:57.000000 matgl-0.5.0/matgl/utils/tests/test_maths.py
+-rw-r--r--   0 shyue      (501) staff       (20)     4102 2023-06-06 19:17:16.000000 matgl-0.5.0/matgl/utils/tests/test_training.py
+-rw-r--r--   0 shyue      (501) staff       (20)    12203 2023-06-06 19:49:36.000000 matgl-0.5.0/matgl/utils/training.py
+drwxr-xr-x   0 shyue      (501) staff       (20)        0 2023-06-09 03:19:42.677410 matgl-0.5.0/matgl.egg-info/
+-rw-r--r--   0 shyue      (501) staff       (20)     8184 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/PKG-INFO
+-rw-r--r--   0 shyue      (501) staff       (20)     1868 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/SOURCES.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        1 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/dependency_links.txt
+-rw-r--r--   0 shyue      (501) staff       (20)       46 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/requires.txt
+-rw-r--r--   0 shyue      (501) staff       (20)        6 2023-06-09 03:19:42.000000 matgl-0.5.0/matgl.egg-info/top_level.txt
+-rw-r--r--   0 shyue      (501) staff       (20)     2639 2023-06-06 13:40:32.000000 matgl-0.5.0/pyproject.toml
+-rw-r--r--   0 shyue      (501) staff       (20)       38 2023-06-09 03:19:42.687410 matgl-0.5.0/setup.cfg
+-rw-r--r--   0 shyue      (501) staff       (20)     2144 2023-06-06 13:40:32.000000 matgl-0.5.0/setup.py
```

### Comparing `matgl-0.4.0/LICENSE` & `matgl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/PKG-INFO` & `matgl-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.4.0
+Version: 0.5.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -39,28 +39,32 @@
 - [Installation](#installation)
 - [Usage](#usage)
 - [Docs](#docs)
 - [References](#references)
 
 ## Introduction
 
-MatGL (Materials Graph Library) is a graph deep learning library for materials. Mathematical graphs are a natural
-representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been shown
-to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
+MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
+natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
+shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
 and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
 The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
-implemented in TensorFlow.
+implemented in TensorFlow (TF). Here are some key improvements over the TF implementations:
+- A more intuitive API and class structure based on the Deep Graph Library.
+- Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 ## Status
 
+- Jun 7 2023: Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
+  available.
 - Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
 - Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
@@ -107,30 +111,38 @@
 
 ```bash
 python setup.py -e .
 ```
 
 ## Usage
 
-The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
+Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
+multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
+implemented convenience method:
+
+```python
+import matgl
+model = matgl.load_model(<name>)
+```
+
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
-from pymatgen.core import Structure, Lattice
-from matgl.models import MEGNet
+from pymatgen.core import Lattice, Structure
+import matgl
+
+model = matgl.load_model("MEGNet-MP-2018.6.1-Eform")
 
-## load the pre-trained MEGNet model for formation energy model.
-model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
-## This is the structure obtained from the Materials Project.
-struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-e_form = model.predict_structure(struct)
-print(f"The predicted formation energy for CsCl is {float(e_form):5f} eV/atom.")
+# This is the structure obtained from the Materials Project.
+struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
+eform = model.predict_structure(struct)
+print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-A full example is in [here](examples/Pre-trained%20MEGNet%20for%20Property%20Predictions.ipynb).
+More examples are available [here](examples).
 
 ## Docs
 
 <http://materialsvirtuallab.github.io/matgl>
 
 ## References
```

### Comparing `matgl-0.4.0/README.md` & `matgl-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,28 +13,32 @@
 - [Installation](#installation)
 - [Usage](#usage)
 - [Docs](#docs)
 - [References](#references)
 
 ## Introduction
 
-MatGL (Materials Graph Library) is a graph deep learning library for materials. Mathematical graphs are a natural
-representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been shown
-to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
+MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
+natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
+shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
 and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
 The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
-implemented in TensorFlow.
+implemented in TensorFlow (TF). Here are some key improvements over the TF implementations:
+- A more intuitive API and class structure based on the Deep Graph Library.
+- Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 ## Status
 
+- Jun 7 2023: Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
+  available.
 - Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
 - Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
@@ -81,30 +85,38 @@
 
 ```bash
 python setup.py -e .
 ```
 
 ## Usage
 
-The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
+Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
+multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
+implemented convenience method:
+
+```python
+import matgl
+model = matgl.load_model(<name>)
+```
+
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
-from pymatgen.core import Structure, Lattice
-from matgl.models import MEGNet
+from pymatgen.core import Lattice, Structure
+import matgl
+
+model = matgl.load_model("MEGNet-MP-2018.6.1-Eform")
 
-## load the pre-trained MEGNet model for formation energy model.
-model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
-## This is the structure obtained from the Materials Project.
-struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-e_form = model.predict_structure(struct)
-print(f"The predicted formation energy for CsCl is {float(e_form):5f} eV/atom.")
+# This is the structure obtained from the Materials Project.
+struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
+eform = model.predict_structure(struct)
+print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-A full example is in [here](examples/Pre-trained%20MEGNet%20for%20Property%20Predictions.ipynb).
+More examples are available [here](examples).
 
 ## Docs
 
 <http://materialsvirtuallab.github.io/matgl>
 
 ## References
```

### Comparing `matgl-0.4.0/matgl/apps/pes.py` & `matgl-0.5.0/matgl/apps/pes.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,25 @@
 import dgl
 import numpy as np
 import torch
 from torch import nn
 from torch.autograd import grad
 
 from matgl.layers import AtomRef
-from matgl.models import M3GNet
+from matgl.utils.io import IOMixIn
 
 
-class Potential(nn.Module):
+class Potential(nn.Module, IOMixIn):
     """
     A class representing an interatomic potential.
     """
 
     def __init__(
         self,
-        model: M3GNet,
+        model: nn.Module,
         data_mean: torch.tensor | None = None,
         data_std: torch.tensor | None = None,
         element_refs: np.ndarray | None = None,
         calc_forces: bool = True,
         calc_stresses: bool = True,
         calc_hessian: bool = False,
     ):
@@ -32,14 +32,15 @@
         :param model: M3GNet model
         :param element_refs: Element reference values for each element
         :param calc_forces: Enable force calculations
         :param calc_stresses: Enable stress calculations
         :param calc_hessian: Enable hessian calculations
         """
         super().__init__()
+        self.save_args(locals())
         self.model = model
         self.calc_forces = calc_forces
         self.calc_stresses = calc_stresses
         self.calc_hessian = calc_hessian
         self.element_refs: AtomRef | None
         if element_refs is not None:
             self.element_refs = AtomRef(property_offset=element_refs)
```

### Comparing `matgl-0.4.0/matgl/ext/ase.py` & `matgl-0.5.0/matgl/ext/ase.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/ext/pymatgen.py` & `matgl-0.5.0/matgl/ext/pymatgen.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/graph/compute.py` & `matgl-0.5.0/matgl/graph/compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/graph/converters.py` & `matgl-0.5.0/matgl/graph/converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/graph/data.py` & `matgl-0.5.0/matgl/graph/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Tools to construct a data for DGL grphs
+Tools to construct a dataset of DGL graphs
 """
 from __future__ import annotations
 
 import json
 import os
 from typing import TYPE_CHECKING, Callable
```

### Comparing `matgl-0.4.0/matgl/graph/tests/test_compute.py` & `matgl-0.5.0/matgl/graph/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/graph/tests/test_converters.py` & `matgl-0.5.0/matgl/graph/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/graph/tests/test_data.py` & `matgl-0.5.0/matgl/graph/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/__init__.py` & `matgl-0.5.0/matgl/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_activations.py` & `matgl-0.5.0/matgl/layers/_activations.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_atom_ref.py` & `matgl-0.5.0/matgl/layers/_atom_ref.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_bond.py` & `matgl-0.5.0/matgl/layers/_bond.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_core.py` & `matgl-0.5.0/matgl/layers/_core.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_embedding.py` & `matgl-0.5.0/matgl/layers/_embedding.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_graph_convolution.py` & `matgl-0.5.0/matgl/layers/_graph_convolution.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_readout.py` & `matgl-0.5.0/matgl/layers/_readout.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/layers/_three_body.py` & `matgl-0.5.0/matgl/layers/_three_body.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/models/_m3gnet.py` & `matgl-0.5.0/matgl/models/_m3gnet.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/models/_megnet.py` & `matgl-0.5.0/matgl/models/_megnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -198,37 +198,27 @@
         return output
 
     def predict_structure(
         self,
         structure: Structure,
         state_feats: torch.tensor | None = None,
         graph_converter: GraphConverter | None = None,
-        data_mean: float | None = None,
-        data_std: float | None = None,
     ):
         """
         Convenience method to directly predict property from structure.
 
         Args:
             structure (Structure): Pymatgen structure
             state_feats (torch.tensor): graph attributes
             graph_converter: Object that implements a get_graph_from_structure.
-            data_mean: Mean of the data. Used when the original data has been scaled.
-            data_std: Std of the data. Used when the original data has been scaled.
 
         Returns:
             output (torch.tensor): output property
         """
         if graph_converter is None:
             graph_converter = Structure2Graph(element_types=self.element_types, cutoff=self.cutoff)
         g, state_feats_default = graph_converter.get_graph(structure)
         if state_feats is None:
             state_feats = torch.tensor(state_feats_default)
-        if data_mean is None:
-            data_mean = torch.zeros(1)
-        if data_std is None:
-            data_std = torch.ones(1)
         bond_vec, bond_dist = compute_pair_vector_and_distance(g)
         g.edata["edge_attr"] = self.bond_expansion(bond_dist)
-        output = data_mean + data_std * self(g, g.edata["edge_attr"], g.ndata["node_type"], state_feats)
-
-        return output.detach()
+        return self(g, g.edata["edge_attr"], g.ndata["node_type"], state_feats).detach()
```

### Comparing `matgl-0.4.0/matgl/utils/cutoff.py` & `matgl-0.5.0/matgl/utils/cutoff.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/utils/io.py` & `matgl-0.5.0/matgl/utils/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -18,26 +18,33 @@
 
 
 class IOMixIn:
     """
     Mixin class for model saving and loading.
     """
 
-    def save_args(self, locals: dict, kwargs: dict) -> None:
+    def save_args(self, locals: dict, kwargs: dict | None = None) -> None:
         r"""
         Method to save args into a private _init_args variable. This should be called after super in the __init__
         method, e.g., `self.save_args(locals(), kwargs)`.
 
         Args:
             locals: The result of locals().
             kwargs: kwargs passed to the class.
         """
         args = inspect.getfullargspec(self.__class__.__init__).args
-        self._init_args = {k: v for k, v in locals.items() if k in args and k not in ("self", "__class__")}
-        self._init_args.update(kwargs)
+        d = {k: v for k, v in locals.items() if k in args and k not in ("self", "__class__")}
+        if kwargs is not None:
+            d.update(kwargs)
+
+        # If one of the args is a subclass of IOMixIn, we will serialize that class.
+        for k, v in d.items():
+            if issubclass(v.__class__, IOMixIn):
+                d[k] = {"@class": v.__class__.__name__, "@module": v.__class__.__module__, "init_args": v._init_args}
+        self._init_args = d
 
     def save(self, path: str | Path = ".", metadata: dict | None = None, makedirs: bool = True):
         """
         Save model to a directory. Three files will be saved.
         - path/model.pt, which contains the torch serialized model args.
         - path/state.pt, which contains the saved state_dict from the model.
         - path/model.json, a txt version of model.pt that is purely meant for ease of reference.
@@ -48,31 +55,34 @@
                 a description of model purpose, the training set used, etc.
             makedirs: Whether to create the directory using os.makedirs(exist_ok=True). Note that if the directory
                 already exists, makedirs will not do anything.
         """
         path = Path(path)
         if makedirs:
             os.makedirs(path, exist_ok=True)
+
         torch.save(self._init_args, path / "model.pt")  # type: ignore
         torch.save(self.state_dict(), path / "state.pt")  # type: ignore
-
-        # This json dump of model args is purely for ease of reference. It is not used to deserialize the model.
-        d = {"name": self.__class__.__name__, "metadata": metadata, "kwargs": self._init_args}  # type: ignore
+        d = {
+            "@class": self.__class__.__name__,
+            "@module": self.__class__.__module__,
+            "metadata": metadata,
+            "kwargs": self._init_args,
+        }  # type: ignore
         with open(path / "model.json", "w") as f:
             json.dump(d, f, default=lambda o: str(o), indent=4)
 
     @classmethod
     def load(cls, path: str | Path, include_json=False, **kwargs):
         """
         Load the model weights from a directory.
 
         Args:
-            path (str|path): Path to saved model or name of pre-trained model. The search order is
-                path, followed by model name in PRETRAINED_MODELS_PATH, followed by download from
-                PRETRAINED_MODELS_BASE_URL.
+            path (str|path): Path to saved model or name of pre-trained model. The search order is path, followed by
+                download from PRETRAINED_MODELS_BASE_URL (with caching).
             include_json (bool): If True, the "model.json" file is also loaded. This file can contain metadata about
                 the model, e.g., if scaling was performed in training the model, this file may contain the mean and
                 standard deviation of the models, which needs to be applied to the final predictions.
             kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
                 want to update the model.
 
         Returns: model_object if include_json is false. (model_object, dict) if include_json is True.
@@ -81,16 +91,14 @@
 
         fnames = ["model.pt", "state.pt"]
         if include_json:
             fnames.append("model.json")
 
         if all((path / fn).exists() for fn in fnames):
             fpaths = {fn: path / fn for fn in fnames}
-        elif all((MATGL_CACHE / path / fn).exists() for fn in fnames):
-            fpaths = {fn: MATGL_CACHE / path / fn for fn in fnames}
         else:
             try:
                 fpaths = {
                     fn: RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/{fn}", **kwargs).local_path for fn in fnames
                 }
             except BaseException:
                 raise ValueError(
@@ -98,15 +106,26 @@
                     f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
                 ) from None
 
         if not torch.cuda.is_available():
             state = torch.load(fpaths["state.pt"], map_location=torch.device("cpu"))
         else:
             state = torch.load(fpaths["state.pt"])
-        model = cls(**torch.load(fpaths["model.pt"]))
+        d = torch.load(fpaths["model.pt"])
+
+        # Deserialize any args that are IOMixIn subclasses.
+        for k, v in d.items():
+            if isinstance(v, dict) and "@class" in v and "@module" in v:
+                modname = v["@module"]
+                classname = v["@class"]
+                mod = __import__(modname, globals(), locals(), [classname], 0)
+                cls_ = getattr(mod, classname)
+                d[k] = cls_(**v["init_args"])
+        d = {k: v for k, v in d.items() if not k.startswith("@")}
+        model = cls(**d)
         model.load_state_dict(state)  # type: ignore
 
         if include_json:
             with open(fpaths["model.json"]) as f:
                 model_data = json.load(f)
 
             return model, model_data
@@ -163,7 +182,44 @@
 
         Args:
             exc_type: Usual meaning in __exit__.
             exc_val: Usual meaning in __exit__.
             exc_tb: Usual meaning in __exit__.
         """
         self.stream.close()
+
+
+def load_model(path: Path, **kwargs):
+    r"""
+    Convenience method to load a model from a directory or name.
+
+    Args:
+        path (str|path): Path to saved model or name of pre-trained model. The search order is path, followed by
+            download from PRETRAINED_MODELS_BASE_URL (with caching).
+        **kwargs: Additional kwargs passed to RemoteFile class. E.g., a useful one might be force_download if you
+            want to update the model.
+
+    Returns:
+        Returns: model_object if include_json is false. (model_object, dict) if include_json is True.
+    """
+    path = Path(path)
+
+    fnames = ["model.pt", "state.pt", "model.json"]
+
+    if all((path / fn).exists() for fn in fnames):
+        fpaths = {fn: path / fn for fn in fnames}
+    else:
+        try:
+            fpaths = {fn: RemoteFile(f"{PRETRAINED_MODELS_BASE_URL}{path}/{fn}", **kwargs).local_path for fn in fnames}
+        except BaseException:
+            raise ValueError(
+                f"No valid model found in {path} or among pre-trained_models at "
+                f"{MATGL_CACHE} or {PRETRAINED_MODELS_BASE_URL}."
+            ) from None
+
+    with open(fpaths["model.json"]) as f:
+        d = json.load(f)
+        modname = d["@module"]
+        classname = d["@class"]
+        mod = __import__(modname, globals(), locals(), [classname], 0)
+        cls_ = getattr(mod, classname)
+        return cls_.load(path, **kwargs)
```

### Comparing `matgl-0.4.0/matgl/utils/maths.py` & `matgl-0.5.0/matgl/utils/maths.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,23 +11,21 @@
 import numpy as np
 import sympy
 import torch
 from scipy.optimize import brentq
 from scipy.special import spherical_jn
 from torch import nn
 
-from matgl.config import DataType
-
 CWD = os.path.dirname(os.path.abspath(__file__))
 
 """
 Precomputed Spherical Bessel function roots in a 2D array with dimension [128, 128]. The n-th (0-based index) root of
 order l Spherical Bessel function is the `[l, n]` entry.
 """
-SPHERICAL_BESSEL_ROOTS = np.load(os.path.join(CWD, "sb_roots.npy"))
+SPHERICAL_BESSEL_ROOTS = torch.tensor(np.load(os.path.join(CWD, "sb_roots.npy")))
 
 
 class GaussianExpansion(nn.Module):
     r"""
     Gaussian Radial Expansion.
     The bond distance is expanded to a vector of shape [m],
     where m is the number of Gaussian basis centers
@@ -49,24 +47,23 @@
                 Location of final Gaussian basis center
         number : int
                 Number of Gaussian Basis functions
         width : float
                 Width of Gaussian Basis functions
         """
         super().__init__()
-        self.centers = np.linspace(initial, final, num_centers)
-        self.centers = nn.Parameter(torch.tensor(self.centers).float(), requires_grad=False)  # type: ignore
+        self.centers = nn.Parameter(torch.linspace(initial, final, num_centers), requires_grad=False)  # type: ignore
         if width is None:
-            self.width = float(1.0 / np.diff(self.centers).mean())
+            self.width = 1.0 / torch.diff(self.centers).mean()
         else:
             self.width = width
 
     def reset_parameters(self):
         """Reinitialize model parameters."""
-        self.centers = nn.Parameter(self.centers.clone().detach().float(), requires_grad=False)
+        self.centers = nn.Parameter(self.centers, requires_grad=False)
 
     def forward(self, bond_dists):
         """Expand distances.
 
         Parameters
         ----------
         bond_dists :
@@ -127,16 +124,14 @@
         self.cutoff = cutoff
         self.smooth = smooth
         if smooth:
             self.funcs = self._calculate_smooth_symbolic_funcs()
         else:
             self.funcs = self._calculate_symbolic_funcs()
 
-        self.zeros = torch.tensor(SPHERICAL_BESSEL_ROOTS, dtype=DataType.torch_float)
-
     @lru_cache(maxsize=128)
     def _calculate_symbolic_funcs(self) -> list:
         """
         Spherical basis functions based on Rayleigh formula. This function
         generates
         symbolic formula.
 
@@ -165,15 +160,15 @@
         return self._call_sbf(r)
 
     def _call_smooth_sbf(self, r):
         results = [i(r) for i in self.funcs]
         return torch.t(torch.stack(results))
 
     def _call_sbf(self, r):
-        roots = self.zeros[: self.max_l, : self.max_n]
+        roots = SPHERICAL_BESSEL_ROOTS[: self.max_l, : self.max_n]
 
         results = []
         factor = torch.tensor(sqrt(2.0 / self.cutoff**3))
         for i in range(self.max_l):
             root = roots[i]
             func = self.funcs[i]
             func_add1 = self.funcs[i + 1]
@@ -190,15 +185,15 @@
 
         Args:
             r: torch.tensor pytorch tensors
             cutoff: float, the cutoff radius
             max_n: int max number of basis
         Returns: basis function expansion using first spherical Bessel function
         """
-        n = (torch.arange(1, max_n + 1)).type(dtype=DataType.torch_float)[None, :]
+        n = (torch.arange(1, max_n + 1)).type(dtype=torch.float32)[None, :]
         r = r[:, None]
         return sqrt(2.0 / cutoff) * torch.sin(n * pi / cutoff * r) / r
 
 
 def _y00(theta, phi):
     r"""
     Spherical Harmonics with `l=m=0`
@@ -254,19 +249,19 @@
             costheta: Cosine of the azimuthal angle
             phi: torch.tensor, the polar angle
 
         Returns: [n, m] spherical harmonic results, where n is the number
             of angles. The column is arranged following
             `[Y_0^0, Y_1^{-1}, Y_1^{0}, Y_1^1, Y_2^{-2}, ...]`
         """
-        costheta = torch.tensor(costheta, dtype=torch.complex64)
-        phi = torch.tensor(phi, dtype=torch.complex64)
-        results = torch.stack([func(costheta, phi) for func in self.funcs], axis=1)
-        results = results.type(dtype=DataType.torch_float)
-        return results
+        # costheta = torch.tensor(costheta, dtype=torch.complex64)
+        # phi = torch.tensor(phi, dtype=torch.complex64)
+        return torch.stack([func(costheta, phi) for func in self.funcs], axis=1)
+        # results = results.type(dtype=DataType.torch_float)
+        # return results
 
 
 def _block_repeat(array, block_size, repeats):
     col_index = torch.arange(array.size()[1])
     indices = []
     start = 0
 
@@ -336,15 +331,15 @@
         r: torch.tensor distance tensor
         cutoff: float, cutoff radius
         max_n: int, max number of basis, expanded by the zero roots
 
     Returns: expanded spherical harmonics with derivatives smooth at boundary
 
     """
-    n = torch.arange(max_n).type(dtype=DataType.torch_float)[None, :]
+    n = torch.arange(max_n).type(dtype=torch.float32)[None, :]
     r = r[:, None]
     fnr = (
         (-1) ** n
         * sqrt(2.0)
         * pi
         / cutoff**1.5
         * (n + 1)
@@ -407,17 +402,16 @@
         ns: torch.tensor, the number of atoms/bonds array
 
     Returns:
         object:
 
     Returns: segment indices tensor
     """
-    B = ns
-    A = torch.arange(B.size(dim=0))
-    return A.repeat_interleave(B, dim=0)
+    a = torch.arange(ns.size(dim=0))
+    return a.repeat_interleave(ns, dim=0)
 
 
 def get_range_indices_from_n(ns):
     """
     Give ns = [2, 3], return [0, 1, 0, 1, 2]
 
     Args:
@@ -433,33 +427,14 @@
     )
     mask = torch.arange(max_n)[None, :] < ns[:, None]
 
     #    return matrix[mask]
     return torch.masked_select(matrix, mask)
 
 
-# def unsorted_segment_softmax(data, segment_ids, num_segments, weights=None):
-#    """
-#    Unsorted segment softmax with optional weights
-#    Args:
-#        data (tf.Tensor): original data
-#        segment_ids (tf.Tensor): tensor segment ids
-#        num_segments (int): number of segments
-#    Returns: tf.Tensor
-#    """
-#    if weights is None:
-#        weights = torch.ones(1)
-#    segment_max = scatter(data, segment_ids, dim=0, reduce="max")
-#    maxes = torch.gather(segment_max, 0, segment_ids)
-#    data -= maxes
-#    exp = torch.exp(data) * torch.squeeze(weights)
-#    softmax = torch.div(exp, torch.gather(scatter(exp, segment_ids, dim=0, reduce="sum"), 0, segment_ids))
-#    return softmax
-
-
 def repeat_with_n(ns, n):
     """
     Repeat the first dimension according to n array.
 
     Args:
         ns (torch.tensor): tensor
         n (torch.tensor): a list of replications
@@ -476,15 +451,14 @@
     bond attributes shape [Nb, Nstate]
 
     Args:
         g: DGL graph
         state_feat: state_feature
 
     Returns: broadcasted state attributes
-
     """
     return state_feat.repeat((g.num_edges(), 1))
 
 
 def broadcast_states_to_atoms(g, state_feat):
     """
     Broadcast state attributes of shape [Ns, Nstate] to
@@ -532,16 +506,15 @@
         segment_ids (torch.tensor): segment ids
         num_segments (torch.tensor): number of segments
     Returns:
         data (torch.tensor): data after fraction
     """
     segment_sum = scatter_sum(input_tensor=data, segment_ids=segment_ids, dim=0, num_segments=num_segments)
     sums = torch.gather(segment_sum, 0, segment_ids)
-    data = torch.div(data, sums)
-    return data
+    return torch.div(data, sums)
 
 
 def broadcast(input_tensor: torch.tensor, target_tensor: torch.tensor, dim: int):
     """
     Broadcast input tensor along a given dimension to match the shape of the target tensor.
     Modified from torch_scatter library (https://github.com/rusty1s/pytorch_scatter).
 
@@ -556,9 +529,8 @@
     if input_tensor.dim() == 1:
         for _ in range(0, dim):
             input_tensor = input_tensor.unsqueeze(0)
     for _ in range(input_tensor.dim(), target_tensor.dim()):
         input_tensor = input_tensor.unsqueeze(-1)
     target_shape = list(target_tensor.shape)
     target_shape[dim] = input_tensor.shape[dim]
-    input_tensor = input_tensor.expand(target_shape)
-    return input_tensor
+    return input_tensor.expand(target_shape)
```

### Comparing `matgl-0.4.0/matgl/utils/sb_roots.npy` & `matgl-0.5.0/matgl/utils/sb_roots.npy`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl/utils/training.py` & `matgl-0.5.0/matgl/utils/training.py`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/matgl.egg-info/PKG-INFO` & `matgl-0.5.0/matgl.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matgl
-Version: 0.4.0
+Version: 0.5.0
 Summary: MatGL (Materials Graph Library) is a framework for graph deep learning for materials science.
 Author: Tsz Wai Ko, Marcel Nassar, Ji Qi, Santiago Miret, Shyue Ping Ong
 Author-email: ongsp@eng.ucsd.edu
 Maintainer: Shyue Ping Ong
 Maintainer-email: ongsp@eng.ucsd.edu
 Keywords: materials,interatomic potential,force field,science,property prediction,AI,machine learning,graph,deep learning
 Classifier: Development Status :: 4 - Beta
@@ -39,28 +39,32 @@
 - [Installation](#installation)
 - [Usage](#usage)
 - [Docs](#docs)
 - [References](#references)
 
 ## Introduction
 
-MatGL (Materials Graph Library) is a graph deep learning library for materials. Mathematical graphs are a natural
-representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been shown
-to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
+MatGL (Materials Graph Library) is a graph deep learning library for materials science. Mathematical graphs are a
+natural representation for a collection of atoms (e.g., molecules or crystals). Graph deep learning models have been
+shown to consistently deliver exceptional performance as surrogate models for the prediction of materials properties.
 
 In this repository, we have reimplemented the [MatErials 3-body Graph Network (m3gnet)](https://github.com/materialsvirtuallab/m3gnet)
 and its predecessor, [MEGNet](https://github.com/materialsvirtuallab/megnet) using the [Deep Graph Library (DGL)](https://www.dgl.ai).
 The goal is to improve the usability, extensibility and scalability of these models. The original M3GNet and MEGNet were
-implemented in TensorFlow.
+implemented in TensorFlow (TF). Here are some key improvements over the TF implementations:
+- A more intuitive API and class structure based on the Deep Graph Library.
+- Multi-GPU support via PyTorch Lightning. A training utility module has been developed.
 
 This effort is a collaboration between the [Materials Virtual Lab](http://materialsvirtuallab.org) and Intel Labs
 (Santiago Miret, Marcel Nassar, Carmelo Gonzales).
 
 ## Status
 
+- Jun 7 2023: Near feature parity with original TF implementations. Re-trained M3Gnet universal potential now
+  available.
 - Apr 26 2023: Pre-trained MEGNet models now available for formation energies and band gaps!
 - Feb 16 2023: Both initial implementations of M3GNet and MEGNet architectures have been completed. Expect bugs!
 
 ## Architectures
 
 <img src="https://github.com/materialsvirtuallab/matgl/blob/main/assets/MxGNet.png?raw=true" alt="m3gnet_schematic" width="50%">
 
@@ -107,30 +111,38 @@
 
 ```bash
 python setup.py -e .
 ```
 
 ## Usage
 
-The pre-trained MEGNet models for the Materials Project formation energy and multi-fidelity band gap are now available.
+Pre-trained M3GNet universal potential and MEGNet models for the Materials Project formation energy and
+multi-fidelity band gap are now available. Users who just want to use the models out of the box should use the newly
+implemented convenience method:
+
+```python
+import matgl
+model = matgl.load_model(<name>)
+```
+
 The following is an example of a prediction of the formation energy for CsCl.
 
 ```python
-from pymatgen.core import Structure, Lattice
-from matgl.models import MEGNet
+from pymatgen.core import Lattice, Structure
+import matgl
+
+model = matgl.load_model("MEGNet-MP-2018.6.1-Eform")
 
-## load the pre-trained MEGNet model for formation energy model.
-model = MEGNet.load("MEGNet-MP-2018.6.1-Eform")
-## This is the structure obtained from the Materials Project.
-struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.14), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
-e_form = model.predict_structure(struct)
-print(f"The predicted formation energy for CsCl is {float(e_form):5f} eV/atom.")
+# This is the structure obtained from the Materials Project.
+struct = Structure.from_spacegroup("Pm-3m", Lattice.cubic(4.1437), ["Cs", "Cl"], [[0, 0, 0], [0.5, 0.5, 0.5]])
+eform = model.predict_structure(struct)
+print(f"The predicted formation energy for CsCl is {float(eform.numpy()):.3f} eV/atom.")
 ```
 
-A full example is in [here](examples/Pre-trained%20MEGNet%20for%20Property%20Predictions.ipynb).
+More examples are available [here](examples).
 
 ## Docs
 
 <http://materialsvirtuallab.github.io/matgl>
 
 ## References
```

### Comparing `matgl-0.4.0/pyproject.toml` & `matgl-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matgl-0.4.0/setup.py` & `matgl-0.5.0/setup.py`

 * *Files identical despite different names*

