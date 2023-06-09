# Comparing `tmp/DeepBench-0.1.0.tar.gz` & `tmp/deepbench-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepBench-0.1.0.tar", max compression
+gzip compressed data, was "deepbench-0.1.1.tar", max compression
```

## Comparing `DeepBench-0.1.0.tar` & `deepbench-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,29 @@
--rw-r--r--   0        0        0     6148 2022-03-14 16:56:41.633609 DeepBench-0.1.0/deepbench/.DS_Store
--rw-r--r--   0        0        0        0 2022-03-14 16:43:43.155399 DeepBench-0.1.0/deepbench/README.rst
--rw-r--r--   0        0        0      315 2022-03-14 17:06:58.759005 DeepBench-0.1.0/deepbench/pyproject.toml
--rw-r--r--   0        0        0     6148 2022-03-14 16:55:43.779509 DeepBench-0.1.0/deepbench/src/.DS_Store
--rw-r--r--   0        0        0       22 2022-03-14 16:43:43.155335 DeepBench-0.1.0/deepbench/src/deepbench/__init__.py
--rw-r--r--   0        0        0        0 2022-03-14 16:43:43.155480 DeepBench-0.1.0/deepbench/tests/__init__.py
--rw-r--r--   0        0        0       90 2022-03-14 16:43:43.155551 DeepBench-0.1.0/deepbench/tests/test_deepbench.py
--rw-r--r--   0        0        0      456 2022-03-14 21:18:05.707628 DeepBench-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      674 2022-03-14 21:44:53.027403 DeepBench-0.1.0/setup.py
--rw-r--r--   0        0        0      401 2022-03-14 21:44:53.027525 DeepBench-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-09-23 14:25:03.589828 deepbench-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3359 2023-06-09 16:08:12.763220 deepbench-0.1.1/README.md
+-rw-r--r--   0        0        0      901 2023-06-09 16:15:21.068959 deepbench-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-03-20 16:19:16.528212 deepbench-0.1.1/src/deepbench/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-26 17:20:37.922821 deepbench-0.1.1/src/deepbench/astro_object/__init__.py
+-rw-r--r--   0        0        0     3493 2023-06-07 15:57:36.000784 deepbench-0.1.1/src/deepbench/astro_object/astro_object.py
+-rw-r--r--   0        0        0     3035 2023-06-09 15:55:07.028288 deepbench-0.1.1/src/deepbench/astro_object/galaxy_object.py
+-rw-r--r--   0        0        0     1076 2023-05-18 19:38:13.746668 deepbench-0.1.1/src/deepbench/astro_object/n_body_object.py
+-rw-r--r--   0        0        0     1759 2023-06-09 15:55:07.028646 deepbench-0.1.1/src/deepbench/astro_object/spiral_galaxy.py
+-rw-r--r--   0        0        0     3768 2023-06-07 15:57:36.001246 deepbench-0.1.1/src/deepbench/astro_object/star_object.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:57:36.001333 deepbench-0.1.1/src/deepbench/collection/__init__.py
+-rw-r--r--   0        0        0     6007 2023-06-07 15:57:36.001537 deepbench-0.1.1/src/deepbench/collection/collection.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:57:36.001583 deepbench-0.1.1/src/deepbench/collection/read_config.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:57:36.001634 deepbench-0.1.1/src/deepbench/collection/save.py
+-rw-r--r--   0        0        0      150 2023-06-07 15:57:36.001967 deepbench-0.1.1/src/deepbench/image/__init__.py
+-rw-r--r--   0        0        0     2560 2023-06-09 15:55:07.028990 deepbench-0.1.1/src/deepbench/image/image.py
+-rw-r--r--   0        0        0     2226 2023-06-09 15:55:07.029513 deepbench-0.1.1/src/deepbench/image/shape_image.py
+-rw-r--r--   0        0        0     2829 2023-06-09 15:55:07.029948 deepbench-0.1.1/src/deepbench/image/sky_image.py
+-rw-r--r--   0        0        0      141 2023-06-07 15:57:36.003274 deepbench-0.1.1/src/deepbench/physics_object/__init__.py
+-rw-r--r--   0        0        0     5646 2023-06-06 21:06:32.265679 deepbench-0.1.1/src/deepbench/physics_object/hamiltonian_pendulum.py
+-rw-r--r--   0        0        0    15450 2023-06-06 21:06:32.266222 deepbench-0.1.1/src/deepbench/physics_object/pendulum.py
+-rw-r--r--   0        0        0     1563 2023-06-06 21:01:29.305615 deepbench-0.1.1/src/deepbench/physics_object/physics_object.py
+-rw-r--r--   0        0        0        0 2023-06-07 15:57:36.003405 deepbench-0.1.1/src/deepbench/settings/default_astro_object.yaml
+-rw-r--r--   0        0        0      298 2023-06-07 15:57:36.003645 deepbench-0.1.1/src/deepbench/settings/default_physics_object.yaml
+-rw-r--r--   0        0        0      213 2023-06-07 15:57:36.003811 deepbench-0.1.1/src/deepbench/settings/default_shapes.yaml
+-rw-r--r--   0        0        0      317 2023-06-07 15:57:36.003958 deepbench-0.1.1/src/deepbench/settings/default_sky_object.yaml
+-rw-r--r--   0        0        0    11110 2023-06-07 15:57:36.004593 deepbench-0.1.1/src/deepbench/shape_generator/shape_generator.py
+-rw-r--r--   0        0        0     4434 1970-01-01 00:00:00.000000 deepbench-0.1.1/setup.py
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 deepbench-0.1.1/PKG-INFO
```

