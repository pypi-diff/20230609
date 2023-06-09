# Comparing `tmp/ragas-0.0.2.tar.gz` & `tmp/ragas-0.0.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.2.tar", last modified: Tue May 23 06:41:03 2023, max compression
+gzip compressed data, was "ragas-0.0.3rc1.tar", last modified: Fri Jun  9 07:33:07 2023, max compression
```

## Comparing `ragas-0.0.2.tar` & `ragas-0.0.3rc1.tar`

### file list

```diff
@@ -1,46 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.800064 ragas-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-23 06:40:47.000000 ragas-0.0.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-23 06:40:47.000000 ragas-0.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-23 06:40:47.000000 ragas-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-23 06:40:47.000000 ragas-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-23 06:40:47.000000 ragas-0.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-23 06:41:03.796064 ragas-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-05-23 06:40:47.000000 ragas-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-23 06:40:47.000000 ragas-0.0.2/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-23 06:40:47.000000 ragas-0.0.2/examples/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-05-23 06:40:47.000000 ragas-0.0.2/examples/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-23 06:40:47.000000 ragas-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12676 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/metrics/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-23 06:40:47.000000 ragas-0.0.2/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-23 06:41:03.000000 ragas-0.0.2/ragas.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-23 06:40:47.000000 ragas-0.0.2/references.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-23 06:40:47.000000 ragas-0.0.2/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-23 06:40:47.000000 ragas-0.0.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:41:03.800064 ragas-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.792065 ragas-0.0.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/benchmarks/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/benchmarks/benchmark_eval.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:41:03.796064 ragas-0.0.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-23 06:40:47.000000 ragas-0.0.2/tests/unit/test_simple.py
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

### Comparing `ragas-0.0.2/.github/workflows/ci.yaml` & `ragas-0.0.3rc1/.github/workflows/ci.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -16,31 +16,31 @@
     shell: bash --noprofile --norc -exo pipefail {0}
 
 jobs:
   diff:
     runs-on: ubuntu-latest
     outputs:
       related: ${{ steps.filter.outputs.related }}
-      belar: ${{ steps.filter.outputs.belar }}
+      ragas: ${{ steps.filter.outputs.ragas }}
       docs: ${{ steps.filter.outputs.docs }}
     steps:
       - uses: actions/checkout@v3
       - uses: dorny/paths-filter@v2
         id: filter
         with:
           base: "main"
           token: ${{ github.token }}
           filters: |
             related: &related
               - .github/workflows/ci.yml
               - codecov.yml
               - pyproject.toml
               - requirements/test.txt
-            belar:
-              - "belar/**"
+            ragas:
+              - "src/ragas/**"
               - "tests/**"
               - "examples/**"
             docs:
               - *related
               - requirements/docs-requirements.txt
               - "docs/**"
 
@@ -50,15 +50,15 @@
 
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.7", "3.8", "3.9", "3.10"]
 
-    if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.belar == 'true') || github.event_name == 'push' }}
+    if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.ragas == 'true') || github.event_name == 'push' }}
     name: python${{ matrix.python-version }}_unit_tests (${{ matrix.os }})
     runs-on: ${{ matrix.os }}
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0 # fetch all tags and branches
@@ -97,15 +97,15 @@
           pytest tests/unit "${OPTS[@]}"
 
   codestyle_check:
     runs-on: ubuntu-latest
     needs:
       - diff
 
-    if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.belar == 'true') || github.event_name == 'push' }}
+    if: ${{ (github.event_name == 'pull_request' && needs.diff.outputs.ragas == 'true') || github.event_name == 'push' }}
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Setup python
         uses: actions/setup-python@v4
         with:
@@ -140,8 +140,8 @@
       - name: Format check
         run: |
           make format
       - name: Lint check
         run: make lint
       - name: Type check
         if: ${{ github.event_name == 'pull_request' }}
-        run: git diff --name-only --diff-filter=AM "origin/$GITHUB_BASE_REF" -z -- '**/*.py' '**/*.pyi' | xargs -0 --no-run-if-empty pyright
+        run: git diff --name-only --diff-filter=AM "origin/$GITHUB_BASE_REF" -z -- 'src/**/*.py' 'src/**/*.pyi' | xargs -0 --no-run-if-empty pyright
```

### Comparing `ragas-0.0.2/.github/workflows/python-publish.yml` & `ragas-0.0.3rc1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/.gitignore` & `ragas-0.0.3rc1/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -154,8 +154,15 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# Ragas specific
 ragas/_version.py
+experiments/**/data
+experiments/**/storage
+**/fil-result/
+experiments/baselines/fiqa/datasets
+src/ragas/_version.py
```

### Comparing `ragas-0.0.2/LICENSE` & `ragas-0.0.3rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/Makefile` & `ragas-0.0.3rc1/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 	@grep -E '^[a-zA-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[33m%-30s\033[0m %s\n", $$1, $$2}'
 
 .PHONY: format lint type style clean run-benchmarks
 format: ## Running code formatter: black and isort
 	@echo "(isort) Ordering imports..."
 	@isort .
 	@echo "(black) Formatting codebase..."
-	@black --config pyproject.toml ragas tests examples
+	@black --config pyproject.toml src tests examples experiments
 	@echo "(black) Formatting stubs..."
-	@find ragas -name "*.pyi" ! -name "*_pb2*" -exec black --pyi --config pyproject.toml {} \;
+	@find src -name "*.pyi" ! -name "*_pb2*" -exec black --pyi --config pyproject.toml {} \;
 	@echo "(ruff) Running fix only..."
-	@ruff check ragas examples tests --fix-only
+	@ruff check src examples tests --fix-only
 lint: ## Running lint checker: ruff
 	@echo "(ruff) Linting development project..."
-	@ruff check ragas examples tests
+	@ruff check src examples tests
 type: ## Running type checker: pyright
 	@echo "(pyright) Typechecking codebase..."
-	@pyright ragas
+	@pyright src
 clean: ## Clean all generated files
 	@echo "Cleaning all generated files..."
 	@cd $(GIT_ROOT)/docs && make clean
 	@cd $(GIT_ROOT) || exit 1
 	@find . -type f -name '*.py[co]' -delete -o -type d -name __pycache__ -delete
 run-ci: format lint type ## Running all CI checks
 run-benchmarks: ## Run benchmarks
 	@echo "Running benchmarks..."
 	@cd $(GIT_ROOT)/tests/benchmarks && python benchmark.py 
+test: ## Run tests
+	@echo "Running tests..."
+	@pytest tests/unit
```

### Comparing `ragas-0.0.2/docs/assets/logo.png` & `ragas-0.0.3rc1/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/examples/data_prep.py` & `ragas-0.0.3rc1/examples/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/examples/quickstart.ipynb` & `ragas-0.0.3rc1/examples/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/ragas/metrics/similarity.py` & `ragas-0.0.3rc1/src/ragas/metrics/context_relevance.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,66 +1,63 @@
 from __future__ import annotations
 
 import typing as t
 from dataclasses import dataclass
 
-import numpy as np
-from numpy.linalg import norm
-from sentence_transformers import SentenceTransformer
+import torch
+from datasets import Dataset
+from pandas import DataFrame
 
+from ragas.metrics.answer_relevance import QGen
 from ragas.metrics.base import Metric
 
-BERT_METRIC = t.Literal["cosine", "euclidean"]
-
 
 @dataclass
-class BERTScore(Metric):
-    similarity_metric: t.Literal[BERT_METRIC] = "cosine"
-    model_path: str = "all-MiniLM-L6-v2"
-    batch_size: int = 1000
-
-    def init_model(self):
-        self.model = SentenceTransformer(self.model_path)
-
-    @property
-    def name(
-        self,
-    ):
-        return f"BERTScore_{self.similarity_metric}"
-
-    @property
-    def is_batchable(self):
-        return True
-
-    def score(
-        self,
-        ground_truth: list[str],
-        generated_text: list[str],
-    ):
-        gndtruth_emb = self.model.encode(
-            ground_truth, batch_size=self.batch_size, convert_to_numpy=True
-        )
-        gentext_emb = self.model.encode(
-            generated_text, batch_size=self.batch_size, convert_to_numpy=True
+class ContextRelevancy(Metric):
+    batch_size: int = 32
+    name: str = "context_relavency"
+    model_name: str = "t5-base"
+
+    def init_model(self: t.Self):
+        self.device = "cuda" if torch.cuda.is_available() else "cpu"
+        self.model = QGen(self.model_name, self.device)
+
+    @staticmethod
+    def _make_question_context_rank_pairs(row: dict) -> dict:
+        q_id = row["q_id"]
+        q = row["question"]
+        cs = row["contexts"]
+        new_q_ids = []
+        sentences = []
+        for i, q_id in enumerate(q_id):
+            for c in cs[i]:
+                sentences.append([q[i], c])
+                new_q_ids.append(q_id)
+
+        return {"q_id": new_q_ids, "sentences": sentences}
+
+    def score(self: t.Self, dataset: Dataset) -> Dataset:
+        """
+        dataset: Dataset[question: list[str], contexts: list[list[str]]]
+        """
+
+        num_qs, _ = dataset.shape
+        dataset = dataset.add_column("q_id", list(range(num_qs)))  # type: ignore
+        sentence_ds = dataset.map(
+            self._make_question_context_rank_pairs,
+            batched=True,
+            batch_size=10,
+            remove_columns=dataset.column_names,
         )
-        assert isinstance(gentext_emb, np.ndarray) and isinstance(
-            gndtruth_emb, np.ndarray
-        ), (
-            f"Both gndtruth_emb[{type(gentext_emb)}], gentext_emb[{type(gentext_emb)}]"
-            " should be numpy ndarray."
-        )
-
-        if self.similarity_metric == "cosine":
-            score = np.sum(gndtruth_emb * gentext_emb, axis=1) / (
-                norm(gndtruth_emb, axis=1) * norm(gentext_emb, axis=1)
-            )
 
-        elif self.similarity_metric == "euclidean":
-            score = norm(gndtruth_emb - gentext_emb, ord=2)
+        # we loose memory here because we have to make it py_list
+        scores = self.model.predict(sentence_ds["sentences"])
 
-        else:
-            raise ValueError(f"Unkown metrics {self.similarity_metric}")
+        sentence_ds = sentence_ds.add_column(self.name, scores)  # type: ignore
+        df = sentence_ds.to_pandas()
+        assert isinstance(df, DataFrame)
+        score_ds = Dataset.from_dict({self.name: df.groupby("q_id")[self.name].mean()})
 
-        return score
+        return score_ds
 
 
-bert_score = BERTScore()
+context_relevancy = ContextRelevancy()
```

### Comparing `ragas-0.0.2/ragas/utils.py` & `ragas-0.0.3rc1/src/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/references.md` & `ragas-0.0.3rc1/references.md`

 * *Files identical despite different names*

### Comparing `ragas-0.0.2/tests/benchmarks/utils.py` & `ragas-0.0.3rc1/tests/benchmarks/utils.py`

 * *Files identical despite different names*

