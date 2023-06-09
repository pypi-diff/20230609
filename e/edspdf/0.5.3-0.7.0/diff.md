# Comparing `tmp/edspdf-0.5.3.tar.gz` & `tmp/edspdf-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edspdf-0.5.3.tar", max compression
+gzip compressed data, was "edspdf-0.7.0.tar", last modified: Fri Jun  9 14:12:13 2023, max compression
```

## Comparing `edspdf-0.5.3.tar` & `edspdf-0.7.0.tar`

### file list

```diff
@@ -1,38 +1,90 @@
--rw-r--r--   0        0        0     1485 2022-08-31 10:01:40.273957 edspdf-0.5.3/LICENSE
--rw-r--r--   0        0        0     1545 2022-08-31 10:01:40.273957 edspdf-0.5.3/README.md
--rw-r--r--   0        0        0      200 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/__init__.py
--rw-r--r--   0        0        0      107 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/aggregators/__init__.py
--rw-r--r--   0        0        0      426 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/aggregators/base.py
--rw-r--r--   0        0        0     1000 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/aggregators/functional.py
--rw-r--r--   0        0        0     1106 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/aggregators/simple.py
--rw-r--r--   0        0        0     1788 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/aggregators/styled.py
--rw-r--r--   0        0        0      216 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/__init__.py
--rw-r--r--   0        0        0     2008 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/align.py
--rw-r--r--   0        0        0      341 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/base.py
--rw-r--r--   0        0        0      388 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/dummy.py
--rw-r--r--   0        0        0     1863 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/mask.py
--rw-r--r--   0        0        0      940 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/random.py
--rw-r--r--   0        0        0      609 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/classifiers/sklearn.py
--rw-r--r--   0        0        0       72 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/__init__.py
--rw-r--r--   0        0        0      297 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/base.py
--rw-r--r--   0        0        0     3093 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/functional.py
--rw-r--r--   0        0        0      299 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/models.py
--rw-r--r--   0        0        0     3138 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/pdfminer.py
--rw-r--r--   0        0        0       33 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/style/__init__.py
--rw-r--r--   0        0        0     3834 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/style/models.py
--rw-r--r--   0        0        0     1393 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/extractors/style/style.py
--rw-r--r--   0        0        0      815 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/loading.py
--rw-r--r--   0        0        0       38 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/misc/__init__.py
--rw-r--r--   0        0        0      398 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/misc/package.py
--rw-r--r--   0        0        0       30 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/readers/__init__.py
--rw-r--r--   0        0        0     3459 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/readers/reader.py
--rw-r--r--   0        0        0     1356 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/reg.py
--rw-r--r--   0        0        0      106 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/transforms/__init__.py
--rw-r--r--   0        0        0      325 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/transforms/base.py
--rw-r--r--   0        0        0     1557 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/transforms/transforms.py
--rw-r--r--   0        0        0       90 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/visualization/__init__.py
--rw-r--r--   0        0        0     2065 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/visualization/annotations.py
--rw-r--r--   0        0        0     3568 2022-08-31 10:01:40.293957 edspdf-0.5.3/edspdf/visualization/merge.py
--rw-r--r--   0        0        0     1735 2022-08-31 10:01:40.293957 edspdf-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     2729 1970-01-01 00:00:00.000000 edspdf-0.5.3/setup.py
--rw-r--r--   0        0        0     2667 1970-01-01 00:00:00.000000 edspdf-0.5.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.730828 edspdf-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-09 14:12:05.000000 edspdf-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-09 14:12:13.730828 edspdf-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-06-09 14:12:05.000000 edspdf-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-09 14:12:05.000000 edspdf-0.7.0/demo/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.718828 edspdf-0.7.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-06-09 14:12:05.000000 edspdf-0.7.0/docs/scripts/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3218 2023-06-09 14:12:05.000000 edspdf-0.7.0/docs/scripts/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/edspdf/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/edspdf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10800 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/layers/box_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/layers/relative_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/layers/sinusoidal_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/layers/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30980 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/edspdf/pipes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/edspdf/pipes/aggregators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/aggregators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/aggregators/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/edspdf/pipes/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/classifiers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4971 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/classifiers/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/classifiers/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/classifiers/trainable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/edspdf/pipes/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/box_layout_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4458 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/box_layout_preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/box_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/embedding_combiner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/simple_text_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/embeddings/sub_box_cnn_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/edspdf/pipes/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6780 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/pipes/extractors/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13180 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/trainable_pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/edspdf/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/utils/alignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8555 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/utils/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/utils/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/utils/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/edspdf/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3677 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/visualization/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-06-09 14:12:06.000000 edspdf-0.7.0/edspdf/visualization/merge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/edspdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-06-09 14:12:13.000000 edspdf-0.7.0/edspdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-09 14:12:13.000000 edspdf-0.7.0/edspdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:12:13.000000 edspdf-0.7.0/edspdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-09 14:12:13.000000 edspdf-0.7.0/edspdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-09 14:12:13.000000 edspdf-0.7.0/edspdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 14:12:13.000000 edspdf-0.7.0/edspdf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-06-09 14:12:06.000000 edspdf-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:12:13.730828 edspdf-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     6900 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/core/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/core/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.722828 edspdf-0.7.0/tests/pipes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.726828 edspdf-0.7.0/tests/pipes/aggregators/
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/aggregators/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.730828 edspdf-0.7.0/tests/pipes/classifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/classifiers/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/classifiers/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/classifiers/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/classifiers/test_mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/classifiers/test_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.730828 edspdf-0.7.0/tests/pipes/extractors/
+-rw-r--r--   0 runner    (1001) docker     (123)    16837 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/extractors/blocks_ground_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/pipes/extractors/test_pdfminer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.730828 edspdf-0.7.0/tests/recipes/
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/recipes/test_train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.730828 edspdf-0.7.0/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/utils/test_py_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/utils/test_torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:12:13.730828 edspdf-0.7.0/tests/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/visualization/test_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-09 14:12:06.000000 edspdf-0.7.0/tests/visualization/test_merge.py
```

### Comparing `edspdf-0.5.3/LICENSE` & `edspdf-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edspdf-0.5.3/README.md` & `edspdf-0.7.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-![Tests](https://img.shields.io/github/workflow/status/aphp/edspdf/Tests%20and%20Linting?label=tests&style=flat-square)
-[![Documentation](https://img.shields.io/github/workflow/status/aphp/edspdf/Documentation?label=docs&style=flat-square)](https://aphp.github.io/edspdf/latest/)
+![Tests](https://img.shields.io/github/actions/workflow/status/aphp/edspdf/tests.yml?branch=main&label=tests&style=flat-square)
+[![Documentation](https://img.shields.io/github/actions/workflow/status/aphp/edspdf/documentation.yml?branch=main&label=docs&style=flat-square)](https://aphp.github.io/edspdf/latest/)
 [![PyPI](https://img.shields.io/pypi/v/edspdf?color=blue&style=flat-square)](https://pypi.org/project/edspdf/)
 [![Codecov](https://img.shields.io/codecov/c/github/aphp/edspdf?logo=codecov&style=flat-square)](https://codecov.io/gh/aphp/edspdf)
 [![DOI](https://zenodo.org/badge/517726737.svg)](https://zenodo.org/badge/latestdoi/517726737)
 
 # EDS-PDF
 
 EDS-PDF provides modular framework to extract text from PDF documents.
@@ -22,15 +22,15 @@
 
 </div>
 
 Visit the [documentation](https://aphp.github.io/edspdf/) for more information!
 
 ## Citation
 
-If you use EDS-NLP, please cite us as below.
+If you use EDS-PDF, please cite us as below.
 
 ```bibtex
 @software{edspdf,
   author  = {Dura, Basile and Wajsburt, Perceval and Calliger, Alice and Gérardin, Christel and Bey, Romain},
   doi     = {10.5281/zenodo.6902977},
   license = {BSD-3-Clause},
   title   = {{EDS-PDF: Smart text extraction from PDF documents}},
```

