# Comparing `tmp/scores-0.0.1.tar.gz` & `tmp/scores-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "scores-0.0.2.tar", last modified: Fri Jun  9 02:02:57 2023, max compression
```

## Comparing `scores-0.0.1.tar` & `scores-0.0.2.tar`

### file list

```diff
@@ -1,5 +1,52 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 scores-0.0.1/src/scores/__init__.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 scores-0.0.1/LICENSE
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 scores-0.0.1/README.md
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 scores-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 scores-0.0.1/PKG-INFO
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.445259 scores-0.0.2/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)       93 2023-06-08 23:04:06.000000 scores-0.0.2/.gitignore
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      762 2023-06-08 23:04:06.000000 scores-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     5482 2023-06-08 23:04:06.000000 scores-0.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      573 2023-06-08 23:04:06.000000 scores-0.0.2/LICENSE
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     5717 2023-06-09 02:02:57.445259 scores-0.0.2/PKG-INFO
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     5088 2023-06-09 01:54:05.000000 scores-0.0.2/README.md
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.441259 scores-0.0.2/docs/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      645 2023-06-08 23:04:06.000000 scores-0.0.2/docs/api.md
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    10184 2023-06-08 23:04:06.000000 scores-0.0.2/docs/contributing.md
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     3263 2023-06-08 23:04:06.000000 scores-0.0.2/docs/data.md
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      294 2023-06-08 23:04:06.000000 scores-0.0.2/docs/index.md
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     3310 2023-06-08 23:04:06.000000 scores-0.0.2/docs/userguide.md
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      232 2023-06-08 23:04:06.000000 scores-0.0.2/environment.yml
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      281 2023-06-08 23:04:06.000000 scores-0.0.2/mkdocs.yml
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)       72 2023-06-08 23:04:06.000000 scores-0.0.2/pylintrc
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     1494 2023-06-08 23:04:06.000000 scores-0.0.2/pyproject.toml
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)       38 2023-06-09 02:02:57.445259 scores-0.0.2/setup.cfg
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.439259 scores-0.0.2/src/
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.441259 scores-0.0.2/src/scores/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      209 2023-06-09 01:54:30.000000 scores-0.0.2/src/scores/__init__.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     4540 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/continuous.py
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.442259 scores-0.0.2/src/scores/probability/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      159 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/probability/__init__.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     1543 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/probability/checks.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    32176 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/probability/crps_impl.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    15250 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/probability/functions.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     3978 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/sample_data.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     5612 2023-06-08 23:04:06.000000 scores-0.0.2/src/scores/utils.py
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.441259 scores-0.0.2/src/scores.egg-info/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     5717 2023-06-09 02:02:57.000000 scores-0.0.2/src/scores.egg-info/PKG-INFO
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     1087 2023-06-09 02:02:57.000000 scores-0.0.2/src/scores.egg-info/SOURCES.txt
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)        1 2023-06-09 02:02:57.000000 scores-0.0.2/src/scores.egg-info/dependency_links.txt
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)      240 2023-06-09 02:02:57.000000 scores-0.0.2/src/scores.egg-info/requires.txt
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)        7 2023-06-09 02:02:57.000000 scores-0.0.2/src/scores.egg-info/top_level.txt
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.439259 scores-0.0.2/tests/
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.442259 scores-0.0.2/tests/scores/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     7703 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/assertions.py
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.443259 scores-0.0.2/tests/scores/probabilty/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    22860 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/probabilty/cdf_test_data.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    16435 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/probabilty/crps_test_data.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    15663 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/probabilty/test_crps.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     6657 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/probabilty/test_functions.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     7841 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/test_continuous.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     1541 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/test_sample_data.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    13521 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/test_utils.py
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)     9537 2023-06-08 23:04:06.000000 scores-0.0.2/tests/scores/utils_test_data.py
+drwxr-xr-x   0 tjl      (1556203457) domain users (1556200513)        0 2023-06-09 02:02:57.445259 scores-0.0.2/tutorials/
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)    89211 2023-06-08 23:04:06.000000 scores-0.0.2/tutorials/Continuous Ranked Probability Score.ipynb
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)  2261646 2023-06-08 23:04:06.000000 scores-0.0.2/tutorials/First - Data Fetching.ipynb
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)   891900 2023-06-08 23:04:06.000000 scores-0.0.2/tutorials/Mean Absolute Error.ipynb
+-rw-r--r--   0 tjl      (1556203457) domain users (1556200513)   463780 2023-06-08 23:04:06.000000 scores-0.0.2/tutorials/Mean Squared Error.ipynb
```

### Comparing `scores-0.0.1/LICENSE` & `scores-0.0.2/LICENSE`

 * *Files identical despite different names*

