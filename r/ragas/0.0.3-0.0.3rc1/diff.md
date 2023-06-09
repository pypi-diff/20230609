# Comparing `tmp/ragas-0.0.3.tar.gz` & `tmp/ragas-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.3.tar", last modified: Fri Jun  9 14:26:11 2023, max compression
+gzip compressed data, was "ragas-0.0.3rc1.tar", last modified: Fri Jun  9 07:33:07 2023, max compression
```

## Comparing `ragas-0.0.3.tar` & `ragas-0.0.3rc1.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.235240 ragas-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 14:25:54.000000 ragas-0.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.227239 ragas-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-09 14:25:54.000000 ragas-0.0.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-09 14:25:54.000000 ragas-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-09 14:25:54.000000 ragas-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 14:25:54.000000 ragas-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-09 14:25:54.000000 ragas-0.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-09 14:26:11.235240 ragas-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-06-09 14:25:54.000000 ragas-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-06-09 14:25:54.000000 ragas-0.0.3/docs/assets/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 14:25:54.000000 ragas-0.0.3/docs/metrics.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 14:25:54.000000 ragas-0.0.3/examples/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    14860 2023-06-09 14:25:54.000000 ragas-0.0.3/examples/quickstart.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/experiments/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/experiments/assesments/
--rw-r--r--   0 runner    (1001) docker     (123)    22726 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/assesments/metrics_assesments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.227239 ragas-0.0.3/experiments/baselines/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/experiments/baselines/fiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    47250 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/fiqa/fiqa_baseline.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)    20978 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/fiqa/improving-baselines.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/experiments/baselines/hotpotqa/
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/hotpotqa/explore-dataset.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/experiments/baselines/wikiqa/
--rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/wikiqa/failed_wikis
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/wikiqa/wikiqa_docs.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 14:25:54.000000 ragas-0.0.3/experiments/baselines/wikiqa/wikiqa_llamaindex_baseline.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-09 14:25:54.000000 ragas-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 14:25:54.000000 ragas-0.0.3/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.231240 ragas-0.0.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-09 14:25:54.000000 ragas-0.0.3/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 14:25:54.000000 ragas-0.0.3/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 14:26:11.235240 ragas-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.227239 ragas-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.235240 ragas-0.0.3/src/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-09 14:26:10.000000 ragas-0.0.3/src/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.235240 ragas-0.0.3/src/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/metrics/answer_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/metrics/context_relevance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/metrics/llms.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-09 14:25:54.000000 ragas-0.0.3/src/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.235240 ragas-0.0.3/src/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-09 14:26:10.000000 ragas-0.0.3/src/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 14:26:11.000000 ragas-0.0.3/src/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:26:10.000000 ragas-0.0.3/src/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 14:26:10.000000 ragas-0.0.3/src/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 14:26:10.000000 ragas-0.0.3/src/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.227239 ragas-0.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.235240 ragas-0.0.3/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 14:25:54.000000 ragas-0.0.3/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-09 14:25:54.000000 ragas-0.0.3/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:26:11.235240 ragas-0.0.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-09 14:25:54.000000 ragas-0.0.3/tests/unit/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 14:25:54.000000 ragas-0.0.3/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.561436 ragas-0.0.3rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/docs/assets/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/docs/metrics.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/examples/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/examples/quickstart.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/assesments/
+-rw-r--r--   0 runner    (1001) docker     (123)    22724 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/assesments/metrics_assesments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.565436 ragas-0.0.3rc1/experiments/baselines/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/baselines/fiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    47444 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/fiqa/fiqa_baseline.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    19636 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/fiqa/improving-baselines.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.569436 ragas-0.0.3rc1/experiments/baselines/hotpotqa/
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/hotpotqa/explore-dataset.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/experiments/baselines/wikiqa/
+-rw-r--r--   0 runner    (1001) docker     (123)    34920 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/failed_wikis
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/wikiqa_docs.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/experiments/baselines/wikiqa/wikiqa_llamaindex_baseline.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/references.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.565436 ragas-0.0.3rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/src/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/src/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/answer_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/context_relevance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/factual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/metrics/llms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/src/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/src/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 07:33:07.000000 ragas-0.0.3rc1/src/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.565436 ragas-0.0.3rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.573436 ragas-0.0.3rc1/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/benchmarks/benchmark_eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 07:33:07.577437 ragas-0.0.3rc1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/unit/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-09 07:32:47.000000 ragas-0.0.3rc1/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.3/.github/workflows/ci.yaml` & `ragas-0.0.3rc1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/.github/workflows/python-publish.yml` & `ragas-0.0.3rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/.gitignore` & `ragas-0.0.3rc1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -162,8 +162,7 @@
 # Ragas specific
 ragas/_version.py
 experiments/**/data
 experiments/**/storage
 **/fil-result/
 experiments/baselines/fiqa/datasets
 src/ragas/_version.py
-.python-version
```

### Comparing `ragas-0.0.3/LICENSE` & `ragas-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/Makefile` & `ragas-0.0.3rc1/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/PKG-INFO` & `ragas-0.0.3rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.3
+Version: 0.0.3rc1
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
@@ -56,32 +56,28 @@
 ```
 
 ## :fire: Quickstart 
 
 This is a small example program you can run to see ragas in action!
 ```python
 
+from ragas.metrics import factuality, answer_relevancy, context_relevancy
 from ragas import evaluate
-from datasets import Dataset
 import os
 
 os.environ["OPENAI_API_KEY"] = "your-openai-key"
 
-# prepare your huggingface dataset in the format
-# Dataset({
-#     features: ['question','contexts','answer'],
-#     num_rows: 25
-# })
-
-dataset: Dataset
-
-results = evaluate(dataset)
+ds = Dataset({
+    features: ['question','context','answer'],
+    num_rows: 25
+})
+results = evaluate(ds, metrics=[nli, answer_relevancy, context_relevancy])
 
 ```
-If you want a more in-depth explanation of core components, check out our [quick-start notebook](./examples/quickstart.ipynb)
+If you want a more in-depth explanation of core components, check out our quick-start notebook
 ## :luggage: Metrics
 
 Ragas measures your pipeline's performance against two dimensions
 1. **Factuality**: measures the factual consistency of the generated answer against the given context.
 2. **Relevancy**:  measures how relevant retrieved contexts and the generated answer are to the question. 
 
 Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.3 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.3rc1 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
        *** Installation | Quickstart | Metrics | FAQ | Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
@@ -12,22 +12,22 @@
 Assessment) comes in ragas provides you with the tools based on the latest
 research for evaluating LLM generated text to give you insights about your RAG
 pipeline. ragas can be integrated with your CI/CD to provide continuous check
 to ensure performance. ## :shield: Installation ```bash pip install ragas ```
 if you want to install from source ```bash git clone https://github.com/
 explodinggradients/ragas && cd ragas pip install -e . ``` ## :fire: Quickstart
 This is a small example program you can run to see ragas in action! ```python
-from ragas import evaluate from datasets import Dataset import os os.environ
-["OPENAI_API_KEY"] = "your-openai-key" # prepare your huggingface dataset in
-the format # Dataset({ # features: ['question','contexts','answer'], #
-num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) ``` If you want
-a more in-depth explanation of core components, check out our [quick-start
-notebook](./examples/quickstart.ipynb) ## :luggage: Metrics Ragas measures your
-pipeline's performance against two dimensions 1. **Factuality**: measures the
-factual consistency of the generated answer against the given context. 2.
+from ragas.metrics import factuality, answer_relevancy, context_relevancy from
+ragas import evaluate import os os.environ["OPENAI_API_KEY"] = "your-openai-
+key" ds = Dataset({ features: ['question','context','answer'], num_rows: 25 })
+results = evaluate(ds, metrics=[nli, answer_relevancy, context_relevancy]) ```
+If you want a more in-depth explanation of core components, check out our
+quick-start notebook ## :luggage: Metrics Ragas measures your pipeline's
+performance against two dimensions 1. **Factuality**: measures the factual
+consistency of the generated answer against the given context. 2.
 **Relevancy**: measures how relevant retrieved contexts and the generated
 answer are to the question. Through repeated experiments, we have found that
 the quality of a RAG pipeline is highly dependent on these two dimensions. The
 final `ragas_score` is the harmonic mean of these two factors. To read more
 about our metrics, checkout [docs](/docs/metrics.md). ## :question: How to use
 Ragas to improve your pipeline? *"Measurement is the first step that leads to
 control and eventually to improvement" - James Harrington* Here we assume that
```

### Comparing `ragas-0.0.3/README.md` & `ragas-0.0.3rc1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -50,32 +50,28 @@
 ```
 
 ## :fire: Quickstart 
 
 This is a small example program you can run to see ragas in action!
 ```python
 
+from ragas.metrics import factuality, answer_relevancy, context_relevancy
 from ragas import evaluate
-from datasets import Dataset
 import os
 
 os.environ["OPENAI_API_KEY"] = "your-openai-key"
 
-# prepare your huggingface dataset in the format
-# Dataset({
-#     features: ['question','contexts','answer'],
-#     num_rows: 25
-# })
-
-dataset: Dataset
-
-results = evaluate(dataset)
+ds = Dataset({
+    features: ['question','context','answer'],
+    num_rows: 25
+})
+results = evaluate(ds, metrics=[nli, answer_relevancy, context_relevancy])
 
 ```
-If you want a more in-depth explanation of core components, check out our [quick-start notebook](./examples/quickstart.ipynb)
+If you want a more in-depth explanation of core components, check out our quick-start notebook
 ## :luggage: Metrics
 
 Ragas measures your pipeline's performance against two dimensions
 1. **Factuality**: measures the factual consistency of the generated answer against the given context.
 2. **Relevancy**:  measures how relevant retrieved contexts and the generated answer are to the question. 
 
 Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors.
```

#### html2text {}

```diff
@@ -10,22 +10,22 @@
 Assessment) comes in ragas provides you with the tools based on the latest
 research for evaluating LLM generated text to give you insights about your RAG
 pipeline. ragas can be integrated with your CI/CD to provide continuous check
 to ensure performance. ## :shield: Installation ```bash pip install ragas ```
 if you want to install from source ```bash git clone https://github.com/
 explodinggradients/ragas && cd ragas pip install -e . ``` ## :fire: Quickstart
 This is a small example program you can run to see ragas in action! ```python
-from ragas import evaluate from datasets import Dataset import os os.environ
-["OPENAI_API_KEY"] = "your-openai-key" # prepare your huggingface dataset in
-the format # Dataset({ # features: ['question','contexts','answer'], #
-num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) ``` If you want
-a more in-depth explanation of core components, check out our [quick-start
-notebook](./examples/quickstart.ipynb) ## :luggage: Metrics Ragas measures your
-pipeline's performance against two dimensions 1. **Factuality**: measures the
-factual consistency of the generated answer against the given context. 2.
+from ragas.metrics import factuality, answer_relevancy, context_relevancy from
+ragas import evaluate import os os.environ["OPENAI_API_KEY"] = "your-openai-
+key" ds = Dataset({ features: ['question','context','answer'], num_rows: 25 })
+results = evaluate(ds, metrics=[nli, answer_relevancy, context_relevancy]) ```
+If you want a more in-depth explanation of core components, check out our
+quick-start notebook ## :luggage: Metrics Ragas measures your pipeline's
+performance against two dimensions 1. **Factuality**: measures the factual
+consistency of the generated answer against the given context. 2.
 **Relevancy**: measures how relevant retrieved contexts and the generated
 answer are to the question. Through repeated experiments, we have found that
 the quality of a RAG pipeline is highly dependent on these two dimensions. The
 final `ragas_score` is the harmonic mean of these two factors. To read more
 about our metrics, checkout [docs](/docs/metrics.md). ## :question: How to use
 Ragas to improve your pipeline? *"Measurement is the first step that leads to
 control and eventually to improvement" - James Harrington* Here we assume that
```

### Comparing `ragas-0.0.3/docs/assets/logo.png` & `ragas-0.0.3rc1/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/docs/metrics.md` & `ragas-0.0.3rc1/docs/metrics.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/examples/data_prep.py` & `ragas-0.0.3rc1/examples/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/experiments/README.md` & `ragas-0.0.3rc1/experiments/README.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/experiments/assesments/metrics_assesments.ipynb` & `ragas-0.0.3rc1/experiments/assesments/metrics_assesments.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997874149659864%*

 * *Differences: {"'cells'": '{2: {\'source\': ["os.chdir(\'/Users/shahules/belar/src/\')"]}}'}*

```diff
@@ -60,15 +60,15 @@
         {
             "cell_type": "code",
             "execution_count": 2,
             "id": "e4168502",
             "metadata": {},
             "outputs": [],
             "source": [
-                "os.chdir(\"/Users/shahules/belar/src/\")"
+                "os.chdir('/Users/shahules/belar/src/')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "9adac051",
             "metadata": {},
```

### Comparing `ragas-0.0.3/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.3rc1/experiments/baselines/fiqa/dataset-exploration-and-baseline.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.998383422609973%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(4, 'url = "*

 * *            '"https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/{}.zip".format(dataset)\\n\')], '*

 * *            "delete: [8, 7, 6, 5, 4]}}, 4: {'source': {insert: [(2, '    \\n')], delete: [2]}}, 5: "*

 * *            "{'source': {insert: [(0, 'corpus_df = corpus_df.rename(columns={\\n'), (1, '    "*

 * *            '"_id": "corpus-id", "text": "ground_truth"\\n\'), (2, \'})\\n\')], delete: [0]}}, 6: '*

 * *            "{'source': {insert: [(4, 'queries_df  […]*

```diff
@@ -44,19 +44,15 @@
                 }
             ],
             "source": [
                 "from beir import util\n",
                 "from beir.datasets.data_loader import GenericDataLoader\n",
                 "\n",
                 "dataset = \"fiqa\"\n",
-                "url = (\n",
-                "    \"https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/{}.zip\".format(\n",
-                "        dataset\n",
-                "    )\n",
-                ")\n",
+                "url = \"https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/datasets/{}.zip\".format(dataset)\n",
                 "data_path = util.download_and_unzip(url, \"datasets\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "id": "ad0b72cf",
@@ -218,15 +214,15 @@
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "with open(os.path.join(data_path, \"corpus.jsonl\")) as f:\n",
                 "    cs = [pd.Series(json.loads(l)) for l in f.readlines()]\n",
-                "\n",
+                "    \n",
                 "corpus_df = pd.DataFrame(cs)\n",
                 "corpus_df"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
@@ -299,15 +295,17 @@
                     },
                     "execution_count": 5,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
-                "corpus_df = corpus_df.rename(columns={\"_id\": \"corpus-id\", \"text\": \"ground_truth\"})\n",
+                "corpus_df = corpus_df.rename(columns={\n",
+                "    \"_id\": \"corpus-id\", \"text\": \"ground_truth\"\n",
+                "})\n",
                 "corpus_df = corpus_df.drop(columns=[\"title\", \"metadata\"])\n",
                 "corpus_df[\"corpus-id\"] = corpus_df[\"corpus-id\"].astype(int)\n",
                 "corpus_df.head()"
             ]
         },
         {
             "cell_type": "code",
@@ -385,15 +383,17 @@
                 }
             ],
             "source": [
                 "with open(os.path.join(data_path, \"queries.jsonl\")) as f:\n",
                 "    qs = [pd.Series(json.loads(l)) for l in f.readlines()]\n",
                 "\n",
                 "queries_df = pd.DataFrame(qs)\n",
-                "queries_df = queries_df.rename(columns={\"_id\": \"query-id\", \"text\": \"question\"})\n",
+                "queries_df = queries_df.rename(columns={\n",
+                "    \"_id\": \"query-id\", \"text\": \"question\"\n",
+                "})\n",
                 "queries_df = queries_df.drop(columns=[\"metadata\"])\n",
                 "queries_df[\"query-id\"] = queries_df[\"query-id\"].astype(int)\n",
                 "queries_df.head()"
             ]
         },
         {
             "cell_type": "code",
@@ -470,18 +470,18 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "splits = [\"dev\", \"test\", \"train\"]\n",
                 "split_df = {}\n",
                 "for s in splits:\n",
-                "    split_df[s] = pd.read_csv(os.path.join(data_path, f\"qrels/{s}.tsv\"), sep=\"\\t\").drop(\n",
-                "        columns=[\"score\"]\n",
-                "    )\n",
-                "\n",
+                "    split_df[s] = pd.read_csv(\n",
+                "        os.path.join(data_path, f\"qrels/{s}.tsv\"), sep=\"\\t\"\n",
+                "    ).drop(columns=[\"score\"])\n",
+                "    \n",
                 "split_df[\"dev\"].head()"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "97ea4840",
@@ -511,22 +511,18 @@
             "outputs": [],
             "source": [
                 "final_split_df = {}\n",
                 "for split in split_df:\n",
                 "    df = queries_df.merge(split_df[split], on=\"query-id\")\n",
                 "    df = df.merge(corpus_df, on=\"corpus-id\")\n",
                 "    df = df.drop(columns=[\"corpus-id\"])\n",
-                "    grouped = df.groupby(\"query-id\").apply(\n",
-                "        lambda x: pd.Series(\n",
-                "            {\n",
-                "                \"question\": x[\"question\"].sample().values[0],\n",
-                "                \"ground_truths\": x[\"ground_truth\"].tolist(),\n",
-                "            }\n",
-                "        )\n",
-                "    )\n",
+                "    grouped = df.groupby('query-id').apply(lambda x: pd.Series({\n",
+                "        'question': x['question'].sample().values[0],\n",
+                "        'ground_truths': x['ground_truth'].tolist()\n",
+                "    }))\n",
                 "\n",
                 "    grouped = grouped.reset_index()\n",
                 "    grouped = grouped.drop(columns=\"query-id\")\n",
                 "    final_split_df[split] = grouped"
             ]
         },
         {
@@ -797,16 +793,19 @@
                 "# change if new\n",
                 "path_to_ds_repo = \"../../../../datasets/fiqa/\"\n",
                 "import os\n",
                 "\n",
                 "assert os.path.exists(path_to_ds_repo), f\"{path_to_ds_repo} doesnot exist!\"\n",
                 "\n",
                 "for s in final_split_df:\n",
-                "    final_split_df[s].to_csv(os.path.join(path_to_ds_repo, f\"{s}.csv\"), index=False)\n",
-                "\n",
+                "    final_split_df[s].to_csv(\n",
+                "        os.path.join(path_to_ds_repo, f\"{s}.csv\"),\n",
+                "        index=False\n",
+                "    )\n",
+                "    \n",
                 "corpus_df.to_csv(os.path.join(path_to_ds_repo, \"corpus.csv\"), index=False)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8a661977",
             "metadata": {},
@@ -1006,19 +1005,26 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "# make nodes\n",
                 "from llama_index.node_parser import SimpleNodeParser\n",
                 "from langchain.text_splitter import TokenTextSplitter\n",
                 "\n",
-                "spliter = TokenTextSplitter(chunk_size=100, chunk_overlap=50)\n",
+                "spliter = TokenTextSplitter(\n",
+                "    chunk_size = 100,\n",
+                "    chunk_overlap = 50\n",
+                ")\n",
                 "\n",
-                "parser = SimpleNodeParser(text_splitter=spliter)\n",
+                "parser = SimpleNodeParser(\n",
+                "    text_splitter=spliter\n",
+                ")\n",
                 "\n",
-                "nodes = parser.get_nodes_from_documents(documents=docs)"
+                "nodes = parser.get_nodes_from_documents(\n",
+                "    documents=docs\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 89,
             "id": "3bf6c119",
             "metadata": {},
@@ -1078,20 +1084,24 @@
             "execution_count": 92,
             "id": "66be5435",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# create index\n",
                 "index = GPTVectorStoreIndex.from_documents(\n",
-                "    documents=docs,\n",
+                "    documents=docs, \n",
                 "    service_context=openai_sc,\n",
                 ")\n",
                 "\n",
                 "# query with embed_model specified\n",
-                "qe = index.as_query_engine(mode=\"embedding\", verbose=True, service_context=openai_sc)"
+                "qe = index.as_query_engine(\n",
+                "    mode=\"embedding\", \n",
+                "    verbose=True, \n",
+                "    service_context=openai_sc\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 93,
             "id": "4b3d899a",
             "metadata": {},
@@ -1157,15 +1167,18 @@
                 "storage_context = StorageContext.from_defaults(persist_dir=\"./storage\")\n",
                 "\n",
                 "# load index\n",
                 "index = load_index_from_storage(storage_context)\n",
                 "\n",
                 "# query with embed_model specified\n",
                 "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", verbose=True, service_context=openai_sc, use_async=False\n",
+                "    mode=\"embedding\", \n",
+                "    verbose=True, \n",
+                "    service_context=openai_sc,\n",
+                "    use_async = False\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 94,
             "id": "9816be1b",
@@ -1178,21 +1191,23 @@
                 ")\n",
                 "from llama_index.retrievers import VectorIndexRetriever\n",
                 "from llama_index.query_engine import RetrieverQueryEngine\n",
                 "from llama_index.indices.postprocessor import SimilarityPostprocessor\n",
                 "\n",
                 "# configure retriever\n",
                 "retriever = VectorIndexRetriever(\n",
-                "    index=index,\n",
+                "    index=index, \n",
                 "    similarity_top_k=3,\n",
                 ")\n",
                 "\n",
                 "# configure response synthesizer\n",
                 "response_synthesizer = ResponseSynthesizer.from_args(\n",
-                "    node_postprocessors=[SimilarityPostprocessor(similarity_cutoff=0.7)]\n",
+                "    node_postprocessors=[\n",
+                "        SimilarityPostprocessor(similarity_cutoff=0.7)\n",
+                "    ]\n",
                 ")\n",
                 "\n",
                 "# assemble query engine\n",
                 "qe = RetrieverQueryEngine(\n",
                 "    retriever=retriever,\n",
                 "    response_synthesizer=response_synthesizer,\n",
                 ")"
@@ -1238,18 +1253,17 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "\n",
+                "    \n",
                 "    return row\n",
                 "\n",
-                "\n",
                 "# generate_response(test_ds[0])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 97,
             "id": "76037e00",
@@ -1512,15 +1526,18 @@
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
+                "evaluate(\n",
+                "    gen_ds, \n",
+                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "997df8cc",
             "metadata": {},
```

### Comparing `ragas-0.0.3/experiments/baselines/fiqa/improving-baselines.ipynb` & `ragas-0.0.3rc1/experiments/baselines/fiqa/improving-baselines.ipynb`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9819807746468152%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['Found cached dataset fiqa "*

 * *            "(/home/jjmachan/.cache/huggingface/datasets/explodinggradients___fiqa/main/1.0.0/953cfddc4a440cf2e290172be2563e5b51a953f2e4266940fc2b311e135cea69)\\n']}}}, "*

 * *            '4: {\'source\': {insert: [(11, \'    mode="embedding", \\n\'), (12, \'    '*

 * *            "verbose=True, \\n'), (13, '    service_context=openai_sc,\\n'), (14, '    use_async = "*

 * *            "False\\n')], delete: [11]}}, 5: {'source': {insert: [(10, '    ind […]*

```diff
@@ -18,15 +18,15 @@
             "id": "25157da5",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "Found cached dataset fiqa (/home/jjmachan/.cache/huggingface/datasets/explodinggradients___fiqa/main/1.0.0/3dc7b639f5b4b16509a3299a2ceb78bf5fe98ee6b5fee25e7d5e4d290c88efb8)\n"
+                        "Found cached dataset fiqa (/home/jjmachan/.cache/huggingface/datasets/explodinggradients___fiqa/main/1.0.0/953cfddc4a440cf2e290172be2563e5b51a953f2e4266940fc2b311e135cea69)\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
                             "Dataset({\n",
                             "    features: ['question', 'ground_truths'],\n",
@@ -93,15 +93,18 @@
                 "storage_context = StorageContext.from_defaults(persist_dir=\"./storage\")\n",
                 "\n",
                 "# load index\n",
                 "index = load_index_from_storage(storage_context)\n",
                 "\n",
                 "# query with embed_model specified\n",
                 "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", verbose=True, service_context=openai_sc, use_async=False\n",
+                "    mode=\"embedding\", \n",
+                "    verbose=True, \n",
+                "    service_context=openai_sc,\n",
+                "    use_async = False\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "c149a4be",
@@ -114,21 +117,23 @@
                 ")\n",
                 "from llama_index.retrievers import VectorIndexRetriever\n",
                 "from llama_index.query_engine import RetrieverQueryEngine\n",
                 "from llama_index.indices.postprocessor import SimilarityPostprocessor\n",
                 "\n",
                 "# configure retriever\n",
                 "retriever = VectorIndexRetriever(\n",
-                "    index=index,\n",
+                "    index=index, \n",
                 "    similarity_top_k=1,\n",
                 ")\n",
                 "\n",
                 "# configure response synthesizer\n",
                 "response_synthesizer = ResponseSynthesizer.from_args(\n",
-                "    node_postprocessors=[SimilarityPostprocessor(similarity_cutoff=0.7)]\n",
+                "    node_postprocessors=[\n",
+                "        SimilarityPostprocessor(similarity_cutoff=0.7)\n",
+                "    ]\n",
                 ")\n",
                 "\n",
                 "# assemble query engine\n",
                 "qe = RetrieverQueryEngine(\n",
                 "    retriever=retriever,\n",
                 "    response_synthesizer=response_synthesizer,\n",
                 ")"
@@ -141,18 +146,17 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "\n",
+                "    \n",
                 "    return row\n",
                 "\n",
-                "\n",
                 "# generate_response(test_ds[0])"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 9,
             "id": "1d5afb7c",
@@ -264,15 +268,18 @@
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
+                "evaluate(\n",
+                "    gen_ds, \n",
+                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "43b21990",
             "metadata": {},
             "source": [
@@ -293,15 +300,18 @@
                 "storage_context = StorageContext.from_defaults(persist_dir=\"./storage\")\n",
                 "\n",
                 "# load index\n",
                 "index = load_index_from_storage(storage_context)\n",
                 "\n",
                 "# query with embed_model specified\n",
                 "qe = index.as_query_engine(\n",
-                "    mode=\"embedding\", verbose=True, service_context=openai_sc, use_async=False\n",
+                "    mode=\"embedding\", \n",
+                "    verbose=True, \n",
+                "    service_context=openai_sc,\n",
+                "    use_async = False\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 5,
             "id": "a2f5e91e",
@@ -314,21 +324,23 @@
                 ")\n",
                 "from llama_index.retrievers import VectorIndexRetriever\n",
                 "from llama_index.query_engine import RetrieverQueryEngine\n",
                 "from llama_index.indices.postprocessor import SimilarityPostprocessor\n",
                 "\n",
                 "# configure retriever\n",
                 "retriever = VectorIndexRetriever(\n",
-                "    index=index,\n",
+                "    index=index, \n",
                 "    similarity_top_k=1,\n",
                 ")\n",
                 "\n",
                 "# configure response synthesizer\n",
                 "response_synthesizer = ResponseSynthesizer.from_args(\n",
-                "    node_postprocessors=[SimilarityPostprocessor(similarity_cutoff=0.7)]\n",
+                "    node_postprocessors=[\n",
+                "        SimilarityPostprocessor(similarity_cutoff=0.7)\n",
+                "    ]\n",
                 ")\n",
                 "\n",
                 "# assemble query engine\n",
                 "qe = RetrieverQueryEngine(\n",
                 "    retriever=retriever,\n",
                 "    response_synthesizer=response_synthesizer,\n",
                 ")"
@@ -341,24 +353,23 @@
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "\n",
+                "    \n",
                 "    return row\n",
                 "\n",
-                "\n",
                 "# generate_response(test_ds[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 12,
             "id": "661ad12b",
             "metadata": {},
             "outputs": [
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
@@ -369,57 +380,56 @@
                             "Map:   0%|          | 0/30 [00:00<?, ? examples/s]"
                         ]
                     },
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
+                    "name": "stderr",
+                    "output_type": "stream",
+                    "text": [
+                        "Retrying langchain.llms.openai.completion_with_retry.<locals>._completion_with_retry in 4.0 seconds as it raised RateLimitError: You exceeded your current quota, please check your plan and billing details..\n"
+                    ]
+                },
+                {
                     "data": {
                         "text/plain": [
                             "Dataset({\n",
                             "    features: ['question', 'ground_truths', 'answer', 'contexts'],\n",
                             "    num_rows: 30\n",
                             "})"
                         ]
                     },
-                    "execution_count": 7,
+                    "execution_count": 12,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen_ds = fiqa_test.select(range(30)).map(generate_response)\n",
                 "gen_ds"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 8,
+            "execution_count": 13,
             "id": "96e08092",
             "metadata": {},
             "outputs": [
                 {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "46e26286ecbc4a0891f8ee228898ca20",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "Downloading model.safetensors:   0%|          | 0.00/892M [00:00<?, ?B/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2/2 [00:56<00:00, 28.39s/it]\n"
+                        "/home/jjmachan/miniconda3/envs/bench/lib/python3.10/site-packages/transformers/models/t5/tokenization_t5_fast.py:155: FutureWarning: This tokenizer was incorrectly instantiated with a model max length of 512 which will be corrected in Transformers v5.\n",
+                        "For now, this behavior is kept to avoid breaking backwards compatibility when padding/encoding with `truncation is True`.\n",
+                        "- Be aware that you SHOULD NOT rely on t5-base automatically truncating your input to 512 when padding/encoding.\n",
+                        "- If you want to encode/pad to sequences longer than 512 you can either instantiate this tokenizer with `model_max_length` or pass `max_length` when encoding/padding.\n",
+                        "- To avoid this warning, please instantiate this tokenizer with `model_max_length` set to your preferred value.\n",
+                        "  warnings.warn(\n",
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2/2 [00:57<00:00, 28.53s/it]\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
                             "version_major": 2,
@@ -432,15 +442,15 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:08<00:00,  8.04s/it]\n"
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:04<00:00,  4.47s/it]\n"
                     ]
                 },
                 {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
                             "version_major": 2,
@@ -453,134 +463,89 @@
                     "metadata": {},
                     "output_type": "display_data"
                 },
                 {
                     "name": "stderr",
                     "output_type": "stream",
                     "text": [
-                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:18<00:00, 18.73s/it]\n"
+                        "100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:11<00:00, 11.58s/it]\n"
                     ]
                 },
                 {
                     "data": {
                         "text/plain": [
-                            "{'ragas_score': 0.8386, 'factuality': 0.8289, 'answer_relevancy': 0.8646, 'context_relavency': 0.8236}"
+                            "{'NLI_score': 0.798888888888889, 'answer_relevancy': 0.8641, 'context_relavency': 0.8236333333333333, 'ragas_score': 0.8280100357048794}"
                         ]
                     },
-                    "execution_count": 8,
+                    "execution_count": 13,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 14,
-            "id": "87054feb",
-            "metadata": {},
-            "outputs": [
-                {
-                    "data": {
-                        "application/vnd.jupyter.widget-view+json": {
-                            "model_id": "da6babe02adf49369a6d708487eeb068",
-                            "version_major": 2,
-                            "version_minor": 0
-                        },
-                        "text/plain": [
-                            "Creating CSV from Arrow format:   0%|          | 0/1 [00:00<?, ?ba/s]"
-                        ]
-                    },
-                    "metadata": {},
-                    "output_type": "display_data"
-                },
-                {
-                    "data": {
-                        "text/plain": [
-                            "82699"
-                        ]
-                    },
-                    "execution_count": 14,
-                    "metadata": {},
-                    "output_type": "execute_result"
-                }
-            ],
-            "source": [
-                "# save to fiqa hub\n",
-                "import os\n",
-                "\n",
-                "path_to_dataset = \"../../../../datasets/fiqa/\"\n",
-                "\n",
-                "gen_ds.to_csv(os.path.join(path_to_dataset, \"baseline_chunk100_k1.csv\"))"
+                "evaluate(\n",
+                "    gen_ds, \n",
+                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
+                ")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "8b957401",
             "metadata": {},
             "source": [
                 "## Cohere Rerank"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 16,
+            "execution_count": 21,
             "id": "15f4c130",
             "metadata": {},
             "outputs": [],
             "source": [
                 "from llama_index.indices.postprocessor.cohere_rerank import CohereRerank\n",
                 "import os\n",
                 "\n",
-                "top_k = 4\n",
+                "top_k = 4  \n",
                 "cohere_rerank = CohereRerank(api_key=os.environ[\"COHERE_API_KEY\"], top_n=top_k)\n",
                 "reranking_qe = index.as_query_engine(\n",
                 "    similarity_top_k=top_k,\n",
                 "    node_postprocessors=[cohere_rerank],\n",
                 ")"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 17,
+            "execution_count": 22,
             "id": "6a73b189",
             "metadata": {},
             "outputs": [],
             "source": [
                 "def generate_response(row):\n",
                 "    r = reranking_qe.query(row[\"question\"])\n",
                 "    row[\"answer\"] = r.response\n",
                 "    row[\"contexts\"] = [sn.node.text for sn in r.source_nodes]\n",
-                "\n",
+                "    \n",
                 "    return row\n",
                 "\n",
-                "\n",
                 "# generate_response(fiqa_test[0])"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 18,
+            "execution_count": 23,
             "id": "32bd4281",
             "metadata": {},
             "outputs": [
                 {
-                    "name": "stderr",
-                    "output_type": "stream",
-                    "text": [
-                        "Parameter 'function'=<function generate_response at 0x7f832ef4f010> of the transform datasets.arrow_dataset.Dataset._map_single couldn't be hashed properly, a random hash was used instead. Make sure your transforms and parameters are serializable with pickle or dill for the dataset fingerprinting and caching to work. If you reuse this transform, the caching mechanism will consider it to be different from the previous calls and recompute everything. This warning is only showed once. Subsequent hashing failures won't be showed.\n"
-                    ]
-                },
-                {
                     "data": {
                         "application/vnd.jupyter.widget-view+json": {
                             "model_id": "",
                             "version_major": 2,
                             "version_minor": 0
                         },
                         "text/plain": [
@@ -595,15 +560,15 @@
                         "text/plain": [
                             "Dataset({\n",
                             "    features: ['question', 'ground_truths', 'answer', 'contexts'],\n",
                             "    num_rows: 30\n",
                             "})"
                         ]
                     },
-                    "execution_count": 18,
+                    "execution_count": 23,
                     "metadata": {},
                     "output_type": "execute_result"
                 }
             ],
             "source": [
                 "gen_ds = fiqa_test.select(range(30)).map(generate_response)\n",
                 "gen_ds"
@@ -676,44 +641,24 @@
                 }
             ],
             "source": [
                 "# evaluate\n",
                 "from ragas.metrics import factuality, answer_relevancy, context_relevancy\n",
                 "from ragas import evaluate\n",
                 "\n",
-                "evaluate(gen_ds, metrics=[factuality, answer_relevancy, context_relevancy])"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": 3,
-            "id": "4301895f",
-            "metadata": {},
-            "outputs": [
-                {
-                    "ename": "NameError",
-                    "evalue": "name 'gen_ds' is not defined",
-                    "output_type": "error",
-                    "traceback": [
-                        "\u001b[0;31m---------------------------------------------------------------------------\u001b[0m",
-                        "\u001b[0;31mNameError\u001b[0m                                 Traceback (most recent call last)",
-                        "Cell \u001b[0;32mIn[3], line 1\u001b[0m\n\u001b[0;32m----> 1\u001b[0m evals[\u001b[38;5;124m\"\u001b[39m\u001b[38;5;124mcohere_reranked\u001b[39m\u001b[38;5;124m\"\u001b[39m] \u001b[38;5;241m=\u001b[39m \u001b[43mgen_ds\u001b[49m\n\u001b[1;32m      2\u001b[0m evals\n",
-                        "\u001b[0;31mNameError\u001b[0m: name 'gen_ds' is not defined"
-                    ]
-                }
-            ],
-            "source": [
-                "evals[\"cohere_reranked\"] = gen_ds\n",
-                "evals"
+                "evaluate(\n",
+                "    gen_ds, \n",
+                "    metrics=[factuality, answer_relevancy, context_relevancy]\n",
+                ")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "02cb461c",
+            "id": "a0991e58",
             "metadata": {},
             "outputs": [],
             "source": []
         }
     ],
     "metadata": {
         "kernelspec": {
@@ -727,13 +672,13 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.10.12"
+            "version": "3.10.11"
         }
     },
     "nbformat": 4,
     "nbformat_minor": 5
 }
```

### Comparing `ragas-0.0.3/experiments/baselines/hotpotqa/explore-dataset.ipynb` & `ragas-0.0.3rc1/experiments/baselines/hotpotqa/explore-dataset.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb` & `ragas-0.0.3rc1/experiments/baselines/wikiqa/dataset-exploration-and-baseline.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/pyproject.toml` & `ragas-0.0.3rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/references.md` & `ragas-0.0.3rc1/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas/evaluation.py` & `ragas-0.0.3rc1/src/ragas/evaluation.py`

 * *Files 13% similar despite different names*

```diff
@@ -103,21 +103,35 @@
             self[cn] = value
             values.append(value)
 
         # harmonic mean of all the scores we have
         if len(values) == 3:
             self["ragas_score"] = len(values) / np.sum(1.0 / np.array(values))
 
+    def describe(self):
+        description = {}
+        for cn in self.scores.column_names:
+            description[cn] = {
+                "mean": np.mean(self.scores[cn]),
+                "25%": np.percentile(self.scores[cn], 25),
+                "50%": np.percentile(self.scores[cn], 50),
+                "75%": np.percentile(self.scores[cn], 75),
+                "min": np.min(self.scores[cn]),
+                "max": np.max(self.scores[cn]),
+                "std": np.std(self.scores[cn]),
+            }
+        return description
+
     def to_pandas(self, batch_size: int | None = None, batched: bool = False):
         if self.dataset is None:
             raise ValueError("dataset is not provided for the results class")
         assert self.scores.shape[0] == self.dataset.shape[0]
         result_ds = concatenate_datasets([self.dataset, self.scores], axis=1)
 
         return result_ds.to_pandas(batch_size=batch_size, batched=batched)
 
     def __repr__(self) -> str:
         scores = self.copy()
         ragas_score = scores.pop("ragas_score")
-        score_strs = [f"'ragas_score': {ragas_score:0.4f}"]
-        score_strs.extend([f"'{k}': {v:0.4f}" for k, v in scores.items()])
+        score_strs = [f"'ragas_score': {ragas_score:0.3f}"]
+        score_strs.extend([f"'{k}': {v:0.3f}" for k, v in scores.items()])
         return "{" + ", ".join(score_strs) + "}"
```

### Comparing `ragas-0.0.3/src/ragas/metrics/answer_relevance.py` & `ragas-0.0.3rc1/src/ragas/metrics/answer_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas/metrics/base.py` & `ragas-0.0.3rc1/src/ragas/metrics/base.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas/metrics/context_relevance.py` & `ragas-0.0.3rc1/src/ragas/metrics/context_relevance.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas/metrics/factual.py` & `ragas-0.0.3rc1/src/ragas/metrics/factual.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas/metrics/llms.py` & `ragas-0.0.3rc1/src/ragas/metrics/llms.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas/utils.py` & `ragas-0.0.3rc1/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/src/ragas.egg-info/PKG-INFO` & `ragas-0.0.3rc1/src/ragas.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ragas
-Version: 0.0.3
+Version: 0.0.3rc1
 Description-Content-Type: text/plain
 License-File: LICENSE
 
 <h1 align="center">
   <img style="vertical-align:middle" height="200"
   src="./docs/assets/logo.png">
 </h1>
@@ -56,32 +56,28 @@
 ```
 
 ## :fire: Quickstart 
 
 This is a small example program you can run to see ragas in action!
 ```python
 
+from ragas.metrics import factuality, answer_relevancy, context_relevancy
 from ragas import evaluate
-from datasets import Dataset
 import os
 
 os.environ["OPENAI_API_KEY"] = "your-openai-key"
 
-# prepare your huggingface dataset in the format
-# Dataset({
-#     features: ['question','contexts','answer'],
-#     num_rows: 25
-# })
-
-dataset: Dataset
-
-results = evaluate(dataset)
+ds = Dataset({
+    features: ['question','context','answer'],
+    num_rows: 25
+})
+results = evaluate(ds, metrics=[nli, answer_relevancy, context_relevancy])
 
 ```
-If you want a more in-depth explanation of core components, check out our [quick-start notebook](./examples/quickstart.ipynb)
+If you want a more in-depth explanation of core components, check out our quick-start notebook
 ## :luggage: Metrics
 
 Ragas measures your pipeline's performance against two dimensions
 1. **Factuality**: measures the factual consistency of the generated answer against the given context.
 2. **Relevancy**:  measures how relevant retrieved contexts and the generated answer are to the question. 
 
 Through repeated experiments, we have found that the quality of a RAG pipeline is highly dependent on these two dimensions. The final `ragas_score` is the harmonic mean of these two factors.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ragas Version: 0.0.3 Description-Content-Type:
+Metadata-Version: 2.1 Name: ragas Version: 0.0.3rc1 Description-Content-Type:
 text/plain License-File: LICENSE
                     ****** [./docs/assets/logo.png] ******
        SOTA metrics for evaluating Retrieval Augmented Generation (RAG)
         [GitHub_release] [Build] [License] [Open_In_Colab] [Downloads]
        *** Installation | Quickstart | Metrics | FAQ | Hugging_Face ***
 ragas is a framework that helps you evaluate your Retrieval Augmented
 Generation (RAG) pipelines. RAG denotes a class of LLM applications that use
@@ -12,22 +12,22 @@
 Assessment) comes in ragas provides you with the tools based on the latest
 research for evaluating LLM generated text to give you insights about your RAG
 pipeline. ragas can be integrated with your CI/CD to provide continuous check
 to ensure performance. ## :shield: Installation ```bash pip install ragas ```
 if you want to install from source ```bash git clone https://github.com/
 explodinggradients/ragas && cd ragas pip install -e . ``` ## :fire: Quickstart
 This is a small example program you can run to see ragas in action! ```python
-from ragas import evaluate from datasets import Dataset import os os.environ
-["OPENAI_API_KEY"] = "your-openai-key" # prepare your huggingface dataset in
-the format # Dataset({ # features: ['question','contexts','answer'], #
-num_rows: 25 # }) dataset: Dataset results = evaluate(dataset) ``` If you want
-a more in-depth explanation of core components, check out our [quick-start
-notebook](./examples/quickstart.ipynb) ## :luggage: Metrics Ragas measures your
-pipeline's performance against two dimensions 1. **Factuality**: measures the
-factual consistency of the generated answer against the given context. 2.
+from ragas.metrics import factuality, answer_relevancy, context_relevancy from
+ragas import evaluate import os os.environ["OPENAI_API_KEY"] = "your-openai-
+key" ds = Dataset({ features: ['question','context','answer'], num_rows: 25 })
+results = evaluate(ds, metrics=[nli, answer_relevancy, context_relevancy]) ```
+If you want a more in-depth explanation of core components, check out our
+quick-start notebook ## :luggage: Metrics Ragas measures your pipeline's
+performance against two dimensions 1. **Factuality**: measures the factual
+consistency of the generated answer against the given context. 2.
 **Relevancy**: measures how relevant retrieved contexts and the generated
 answer are to the question. Through repeated experiments, we have found that
 the quality of a RAG pipeline is highly dependent on these two dimensions. The
 final `ragas_score` is the harmonic mean of these two factors. To read more
 about our metrics, checkout [docs](/docs/metrics.md). ## :question: How to use
 Ragas to improve your pipeline? *"Measurement is the first step that leads to
 control and eventually to improvement" - James Harrington* Here we assume that
```

### Comparing `ragas-0.0.3/src/ragas.egg-info/SOURCES.txt` & `ragas-0.0.3rc1/src/ragas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/tests/benchmarks/benchmark_eval.py` & `ragas-0.0.3rc1/tests/benchmarks/benchmark_eval.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.3/tests/benchmarks/utils.py` & `ragas-0.0.3rc1/tests/benchmarks/utils.py`

 * *Files identical despite different names*

