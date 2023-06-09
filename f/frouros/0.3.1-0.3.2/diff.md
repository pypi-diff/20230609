# Comparing `tmp/frouros-0.3.1.tar.gz` & `tmp/frouros-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frouros-0.3.1.tar", last modified: Fri Jun  2 13:40:56 2023, max compression
+gzip compressed data, was "frouros-0.3.2.tar", last modified: Fri Jun  9 07:54:09 2023, max compression
```

## Comparing `frouros-0.3.1.tar` & `frouros-0.3.2.tar`

### file list

```diff
@@ -1,131 +1,131 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-02 13:40:40.000000 frouros-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-02 13:40:40.000000 frouros-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    21654 2023-06-02 13:40:56.146494 frouros-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    20033 2023-06-02 13:40:40.000000 frouros-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/callbacks/
--rw-r--r--   0 runner    (1001) docker     (122)      286 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/callbacks/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      211 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5625 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/permutation_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     2079 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/batch/reset_drift.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/callbacks/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      820 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2728 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/history.py
--rw-r--r--   0 runner    (1001) docker     (122)     6393 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/msprt.py
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/callbacks/streaming/warning_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/common/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/common/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/datasets/
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/real.py
--rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/datasets/synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/detectors/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/detectors/concept_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6194 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/base.py
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/
--rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5372 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
--rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/
--rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10816 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     4831 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
--rw-r--r--   0 runner    (1001) docker     (122)    12437 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
--rw-r--r--   0 runner    (1001) docker     (122)    23112 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9678 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/
--rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19342 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py
--rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     5977 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7896 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6460 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/batch/
--rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3450 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8810 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     1796 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/emd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2154 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/js.py
--rw-r--r--   0 runner    (1001) docker     (122)     2164 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/kl.py
--rw-r--r--   0 runner    (1001) docker     (122)     8167 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/mmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2368 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/psi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2514 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
--rw-r--r--   0 runner    (1001) docker     (122)     2445 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/ks.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/streaming/
--rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2666 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/base.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3135 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.142495 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/
--rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     7341 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/metrics/prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     9103 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (122)     5329 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_data_drift.py
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_real.py
--rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/integration/test_synthetic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/tests/unit/metrics/test_prequential_error.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.146494 frouros-0.3.1/frouros/utils/
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (122)      695 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-06-02 13:40:40.000000 frouros-0.3.1/frouros/utils/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-02 13:40:56.138495 frouros-0.3.1/frouros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21654 2023-06-02 13:40:55.000000 frouros-0.3.1/frouros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4713 2023-06-02 13:40:56.000000 frouros-0.3.1/frouros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 13:40:55.000000 frouros-0.3.1/frouros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-02 13:40:55.000000 frouros-0.3.1/frouros.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      350 2023-06-02 13:40:56.000000 frouros-0.3.1/frouros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-02 13:40:56.000000 frouros-0.3.1/frouros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-06-02 13:40:40.000000 frouros-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-02 13:40:56.146494 frouros-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-02 13:40:40.000000 frouros-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1548 2023-06-09 07:53:53.000000 frouros-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-06-09 07:53:53.000000 frouros-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    22236 2023-06-09 07:54:09.130316 frouros-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    20615 2023-06-09 07:53:53.000000 frouros-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.114316 frouros-0.3.2/frouros/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (122)      312 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/callbacks/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      735 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5629 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/permutation_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2118 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/batch/reset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/callbacks/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      232 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2647 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/history.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6295 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/msprt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2009 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/callbacks/streaming/warning_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/common/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/common/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/datasets/
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5703 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      466 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1214 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3041 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/datasets/synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/detectors/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2331 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros/detectors/concept_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6598 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      566 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      414 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5461 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1567 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1727 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10975 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2752 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4920 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12526 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23271 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9767 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      285 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19431 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6066 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7985 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/stepd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.122316 frouros-0.3.2/frouros/detectors/data_drift/
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6567 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/batch/
+-rw-r--r--   0 runner    (1001) docker     (122)      515 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3754 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      486 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8889 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1929 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1831 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/emd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2340 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2187 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2199 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/kl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8198 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/mmd.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2403 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/psi.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      271 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2489 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/ks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1542 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)      428 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/streaming/
+-rw-r--r--   0 runner    (1001) docker     (122)      183 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2952 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2019 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3224 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/mmd.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.126316 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/
+-rw-r--r--   0 runner    (1001) docker     (122)      144 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2288 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7430 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      135 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1456 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3758 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/metrics/prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12327 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (122)       30 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9163 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5329 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14909 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1620 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/integration/test_synthetic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)       25 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1493 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/tests/unit/metrics/test_prequential_error.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.130316 frouros-0.3.2/frouros/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      833 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21163 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (122)      140 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7750 2023-06-09 07:53:53.000000 frouros-0.3.2/frouros/utils/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-09 07:54:09.118316 frouros-0.3.2/frouros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    22236 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4703 2023-06-09 07:54:09.000000 frouros-0.3.2/frouros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      345 2023-06-09 07:54:08.000000 frouros-0.3.2/frouros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        8 2023-06-09 07:54:09.000000 frouros-0.3.2/frouros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2141 2023-06-09 07:53:53.000000 frouros-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-09 07:54:09.130316 frouros-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1854 2023-06-09 07:53:53.000000 frouros-0.3.2/setup.py
```

### Comparing `frouros-0.3.1/LICENSE` & `frouros-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/PKG-INFO` & `frouros-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.3.1
-Summary: An open source Python library for drift detection in machine Learning systems
+Version: 0.3.2
+Summary: An open source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
 Project-URL: homepage, https://frouros.readthedocs.io
@@ -409,14 +409,20 @@
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Incremental Kolmogorov-Smirnov test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1145/2939672.2939836">dos Reis et al. (2016)</a></td>
   </tr>
 </tbody>
 </table>
 
+## ❗ What is and what is not Frouros?
+
+Unlike other libraries that in addition to provide drift detection algorithms, include other functionalities such as anomaly/outlier detection, adversarial detection, imbalance learning, among others, Frouros has and will **ONLY** have one purpose: **drift detection**.
+
+We firmly believe that machine learning related libraries or frameworks should not follow [Jack of all trades, master of none](https://en.wikipedia.org/wiki/Jack_of_all_trades,_master_of_none) principle. Instead, they should be focused on a single task and do it well.
+
 ## ✅ Who is using Frouros?
 
 Frouros is actively being used by the following projects to implement drift
 detection in machine learning pipelines:
 
  * [AI4EOSC](https://ai4eosc.eu).
  * [iMagine](https://imagine-ai.eu).
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.3.1 Summary: An open source
-Python library for drift detection in machine Learning systems Home-page:
+Metadata-Version: 2.1 Name: frouros Version: 0.3.2 Summary: An open source
+Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
 drift,data-drift,machine-learning,data-science,machine-learning-
@@ -122,23 +122,30 @@
                                                         test
                                U            N           Welch's T-Test      Welch_(1947)
                    Distance    M            N           MMD                 Gretton_et_al._(2012)
                    based
          Streaming Statistical                          Incremental
                    test        U            N           Kolmogorov-Smirnov  dos_Reis_et_al._(2016)
                                                         test
-## â Who is using Frouros? Frouros is actively being used by the following
-projects to implement drift detection in machine learning pipelines: *
-[AI4EOSC](https://ai4eosc.eu). * [iMagine](https://imagine-ai.eu). If you want
-your project listed here, do not hesitate to send us a pull request. ## ð
-Contributing Check out the [contribution](https://github.com/IFCA/frouros/blob/
-main/CONTRIBUTING.md) section. ## ð¬ Citation Although Frouros paper is still
-in preprint, if you want to cite it you can use the [preprint](https://
-arxiv.org/abs/2208.06868) version (to be replaced by the paper once is
-published). ```bibtex @article{cespedes2022frouros, title={Frouros: A Python
-library for drift detection in Machine Learning problems}, author={C{\'e}spedes
-Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro }, journal={arXiv
-preprint arXiv:2208.06868}, year={2022} } ``` ## ð License Frouros is an
-open-source software licensed under the [BSD-3-Clause license](https://
-github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements Frouros
-has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad de
-Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
+## â What is and what is not Frouros? Unlike other libraries that in addition
+to provide drift detection algorithms, include other functionalities such as
+anomaly/outlier detection, adversarial detection, imbalance learning, among
+others, Frouros has and will **ONLY** have one purpose: **drift detection**. We
+firmly believe that machine learning related libraries or frameworks should not
+follow [Jack of all trades, master of none](https://en.wikipedia.org/wiki/
+Jack_of_all_trades,_master_of_none) principle. Instead, they should be focused
+on a single task and do it well. ## â Who is using Frouros? Frouros is
+actively being used by the following projects to implement drift detection in
+machine learning pipelines: * [AI4EOSC](https://ai4eosc.eu). * [iMagine](https:
+//imagine-ai.eu). If you want your project listed here, do not hesitate to send
+us a pull request. ## ð Contributing Check out the [contribution](https://
+github.com/IFCA/frouros/blob/main/CONTRIBUTING.md) section. ## ð¬ Citation
+Although Frouros paper is still in preprint, if you want to cite it you can use
+the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the
+paper once is published). ```bibtex @article{cespedes2022frouros, title=
+{Frouros: A Python library for drift detection in Machine Learning problems},
+author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+journal={arXiv preprint arXiv:2208.06868}, year={2022} } ``` ## ð License
+Frouros is an open-source software licensed under the [BSD-3-Clause license]
+(https://github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements
+Frouros has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad
+de Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
```

### Comparing `frouros-0.3.1/README.md` & `frouros-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -373,14 +373,20 @@
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Incremental Kolmogorov-Smirnov test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1145/2939672.2939836">dos Reis et al. (2016)</a></td>
   </tr>
 </tbody>
 </table>
 
+## ❗ What is and what is not Frouros?
+
+Unlike other libraries that in addition to provide drift detection algorithms, include other functionalities such as anomaly/outlier detection, adversarial detection, imbalance learning, among others, Frouros has and will **ONLY** have one purpose: **drift detection**.
+
+We firmly believe that machine learning related libraries or frameworks should not follow [Jack of all trades, master of none](https://en.wikipedia.org/wiki/Jack_of_all_trades,_master_of_none) principle. Instead, they should be focused on a single task and do it well.
+
 ## ✅ Who is using Frouros?
 
 Frouros is actively being used by the following projects to implement drift
 detection in machine learning pipelines:
 
  * [AI4EOSC](https://ai4eosc.eu).
  * [iMagine](https://imagine-ai.eu).
```

#### html2text {}

```diff
@@ -100,23 +100,30 @@
                                                         test
                                U            N           Welch's T-Test      Welch_(1947)
                    Distance    M            N           MMD                 Gretton_et_al._(2012)
                    based
          Streaming Statistical                          Incremental
                    test        U            N           Kolmogorov-Smirnov  dos_Reis_et_al._(2016)
                                                         test
-## â Who is using Frouros? Frouros is actively being used by the following
-projects to implement drift detection in machine learning pipelines: *
-[AI4EOSC](https://ai4eosc.eu). * [iMagine](https://imagine-ai.eu). If you want
-your project listed here, do not hesitate to send us a pull request. ## ð
-Contributing Check out the [contribution](https://github.com/IFCA/frouros/blob/
-main/CONTRIBUTING.md) section. ## ð¬ Citation Although Frouros paper is still
-in preprint, if you want to cite it you can use the [preprint](https://
-arxiv.org/abs/2208.06868) version (to be replaced by the paper once is
-published). ```bibtex @article{cespedes2022frouros, title={Frouros: A Python
-library for drift detection in Machine Learning problems}, author={C{\'e}spedes
-Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro }, journal={arXiv
-preprint arXiv:2208.06868}, year={2022} } ``` ## ð License Frouros is an
-open-source software licensed under the [BSD-3-Clause license](https://
-github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements Frouros
-has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad de
-Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
+## â What is and what is not Frouros? Unlike other libraries that in addition
+to provide drift detection algorithms, include other functionalities such as
+anomaly/outlier detection, adversarial detection, imbalance learning, among
+others, Frouros has and will **ONLY** have one purpose: **drift detection**. We
+firmly believe that machine learning related libraries or frameworks should not
+follow [Jack of all trades, master of none](https://en.wikipedia.org/wiki/
+Jack_of_all_trades,_master_of_none) principle. Instead, they should be focused
+on a single task and do it well. ## â Who is using Frouros? Frouros is
+actively being used by the following projects to implement drift detection in
+machine learning pipelines: * [AI4EOSC](https://ai4eosc.eu). * [iMagine](https:
+//imagine-ai.eu). If you want your project listed here, do not hesitate to send
+us a pull request. ## ð Contributing Check out the [contribution](https://
+github.com/IFCA/frouros/blob/main/CONTRIBUTING.md) section. ## ð¬ Citation
+Although Frouros paper is still in preprint, if you want to cite it you can use
+the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the
+paper once is published). ```bibtex @article{cespedes2022frouros, title=
+{Frouros: A Python library for drift detection in Machine Learning problems},
+author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+journal={arXiv preprint arXiv:2208.06868}, year={2022} } ``` ## ð License
+Frouros is an open-source software licensed under the [BSD-3-Clause license]
+(https://github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements
+Frouros has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad
+de Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
```

### Comparing `frouros-0.3.1/frouros/callbacks/base.py` & `frouros-0.3.2/frouros/callbacks/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,14 @@
 
     def on_fit_start(self, **kwargs) -> None:
         """On fit start method."""
 
     def on_fit_end(self, **kwargs) -> None:
         """On fit end method."""
 
-    def on_drift_detected(self, **kwargs) -> None:
-        """On drift detected method."""
-
     @abc.abstractmethod
     def reset(self) -> None:
         """Reset method."""
 
     def __repr__(self) -> str:
         """Repr method.
```

### Comparing `frouros-0.3.1/frouros/callbacks/batch/base.py` & `frouros-0.3.2/frouros/callbacks/batch/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from frouros.callbacks.base import BaseCallback
 
 
 class BaseCallbackBatch(BaseCallback):
     """Callback batch class."""
 
-    def on_compare_start(self) -> None:
+    def on_compare_start(self, **kwargs) -> None:
         """On compare start method."""
 
     def on_compare_end(self, **kwargs) -> None:
         """On compare end method."""
 
     # FIXME: set_detector method as a workaround to  # pylint: disable=fixme
     #  avoid circular import problem. Make it an abstract method and
```

### Comparing `frouros-0.3.1/frouros/callbacks/batch/permutation_test.py` & `frouros-0.3.2/frouros/callbacks/batch/permutation_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Permutation test on batch data callback module."""
+"""Permutation test batch callback module."""
 
 import multiprocessing
 from typing import Any, Callable, Dict, List, Optional, Tuple
 
 import numpy as np  # type: ignore
 from scipy.stats import norm  # type: ignore
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.utils.stats import permutation, z_score
 
 
-class PermutationTestOnBatchData(BaseCallbackBatch):
-    """Permutation test on batch data callback class."""
+class PermutationTestDistanceBased(BaseCallbackBatch):
+    """Permutation test on distance based batch callback class."""
 
     def __init__(
         self,
         num_permutations: int,
         num_jobs: int = -1,
         name: Optional[str] = None,
         verbose: bool = False,
```

### Comparing `frouros-0.3.1/frouros/callbacks/batch/reset_drift.py` & `frouros-0.3.2/frouros/callbacks/batch/reset.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-"""Reset on batch data drift callback module."""
+"""Reset batch callback module."""
 
 from typing import Optional
 
 from frouros.callbacks.batch.base import BaseCallbackBatch
+from frouros.utils.logger import logger
 
 
-class ResetOnBatchDataDrift(BaseCallbackBatch):
-    """Reset on batch data drift callback class."""
+class ResetStatisticalTest(BaseCallbackBatch):
+    """Reset on statistical test batch callback class."""
 
     def __init__(self, alpha: float, name: Optional[str] = None) -> None:
         """Init method.
 
         :param alpha: significance value
         :type alpha: float
         :param name: name to be use
@@ -40,15 +41,15 @@
             raise ValueError("value must be greater than 0.")
         self._alpha = value
 
     def on_compare_end(self, **kwargs) -> None:
         """On compare end method."""
         p_value = kwargs["result"].p_value
         if p_value < self.alpha:
-            print("Drift detected. Resetting detector.")
+            logger.info("Drift detected. Resetting detector...")
             self.detector.reset()  # type: ignore
 
     # FIXME: set_detector method as a workaround to  # pylint: disable=fixme
     #  avoid circular import problem. Make it an abstract method and
     #  uncomment commented code when it is solved
 
     # def set_detector(self, detector) -> None:
```

### Comparing `frouros-0.3.1/frouros/callbacks/streaming/base.py` & `frouros-0.3.2/frouros/callbacks/streaming/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 """Base callback streaming module."""
 
 import abc
-from typing import Union
 
 from frouros.callbacks.base import BaseCallback
 
 
 class BaseCallbackStreaming(BaseCallback):
     """Callback streaming class."""
 
-    def on_update_start(self, value: Union[int, float], **kwargs) -> None:
+    def on_update_start(self, **kwargs) -> None:
         """On update start method."""
 
-    def on_update_end(self, value: Union[int, float], **kwargs) -> None:
+    def on_update_end(self, **kwargs) -> None:
         """On update end method."""
 
     # FIXME: set_detector method as a workaround to  # pylint: disable=fixme
     #  avoid circular import problem. Make it an abstract method and
     #  uncomment commented code when it is solved
 
     # @abc.abstractmethod
```

### Comparing `frouros-0.3.1/frouros/callbacks/streaming/history.py` & `frouros-0.3.2/frouros/callbacks/streaming/history.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """History callback module."""
 
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.utils.stats import BaseStat
 
 
-class History(BaseCallbackStreaming):
-    """History callback class."""
+class HistoryConceptDrift(BaseCallbackStreaming):
+    """HistoryConceptDrift callback class."""
 
     def __init__(self, name: Optional[str] = None) -> None:
         """Init method.
 
         :param name: name value
         :type name: Optional[str]
         """
@@ -28,21 +28,17 @@
 
         :param vars_: list of variables
         :type vars_: List[str]
         """
         self.additional_vars.extend(vars_)
         self.history = {**self.history, **{var: [] for var in self.additional_vars}}
 
-    def on_update_end(self, value: Union[int, float], **kwargs) -> None:
-        """On update end method.
-
-        :param value: value to update detector
-        :type value: int
-        """
-        self.history["value"].append(value)
+    def on_update_end(self, **kwargs) -> None:
+        """On update end method."""
+        self.history["value"].append(kwargs["value"])
         self.history["num_instances"].append(
             self.detector.num_instances  # type: ignore
         )
         self.history["drift"].append(self.detector.drift)  # type: ignore
         for var in self.additional_vars:
             additional_var = self.detector.additional_vars[var]  # type: ignore
             # FIXME: Extract isinstance check to be done when  # pylint: disable=fixme
```

### Comparing `frouros-0.3.1/frouros/callbacks/streaming/msprt.py` & `frouros-0.3.2/frouros/callbacks/streaming/msprt.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,21 +135,17 @@
         self._lambda_ = value
 
     def on_fit_end(self, **kwargs) -> None:
         """On fit end method."""
         self.mean = CircularMean(size=self.detector.window_size)  # type: ignore
         self.theta = self.detector.compare(X=kwargs["X"])[0].distance  # type: ignore
 
-    def on_update_end(self, value: Union[int, float], **kwargs) -> None:
-        """On update end method.
-
-        :param value: value to update detector
-        :type value: int
-        """
-        self.mean.update(value=value)  # type: ignore
+    def on_update_end(self, **kwargs) -> None:
+        """On update end method."""
+        self.mean.update(value=kwargs["value"])  # type: ignore
         self.p_value, likelihood = self._calculate_p_value()
 
         self.logs.update(
             {
                 "distance_mean": self.mean.get(),  # type: ignore
                 "likelihood": likelihood,
                 "p_value": self.p_value,
```

### Comparing `frouros-0.3.1/frouros/callbacks/streaming/warning_samples.py` & `frouros-0.3.2/frouros/callbacks/streaming/warning_samples.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Warning samples buffer callback module."""
 
 import copy
-from typing import Any, List, Optional, Union
+from typing import Any, List, Optional
 
 from frouros.callbacks.streaming.base import BaseCallbackStreaming
 
 
 class WarningSamplesBuffer(BaseCallbackStreaming):
     """Store warning samples as a buffer callback class."""
 
@@ -16,24 +16,20 @@
         :type name: Optional[str]
         """
         super().__init__(name=name)
         self.X: List[Any] = []
         self.y: List[Any] = []
         self._start_warning = False
 
-    def on_update_start(self, value: Union[int, float], **kwargs) -> None:
+    def on_update_start(self, **kwargs) -> None:
         """On update start method."""
         self._start_warning = not self.detector.warning  # type: ignore
 
-    def on_update_end(self, value: Union[int, float], **kwargs) -> None:
-        """On update end method.
-
-        :param value: value to update detector
-        :type value: int
-        """
+    def on_update_end(self, **kwargs) -> None:
+        """On update end method."""
         self.logs = {
             "X": copy.deepcopy(self.X),
             "y": copy.deepcopy(self.y),
         }
 
     def on_warning_detected(self, **kwargs) -> None:
         """On warning detected method."""
```

### Comparing `frouros-0.3.1/frouros/datasets/base.py` & `frouros-0.3.2/frouros/datasets/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/datasets/real.py` & `frouros-0.3.2/frouros/datasets/real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/datasets/synthetic.py` & `frouros-0.3.2/frouros/datasets/synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/base.py` & `frouros-0.3.2/frouros/detectors/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/__init__.py` & `frouros-0.3.2/frouros/detectors/concept_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/base.py` & `frouros-0.3.2/frouros/detectors/concept_drift/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Base concept drift module."""
 
 import abc
 from typing import Any, Dict, List, Optional, Union
 
-from frouros.callbacks import History
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks import HistoryConceptDrift
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.base import BaseDetector
+from frouros.utils.checks import check_callbacks
 
 
 class BaseConceptDriftConfig(abc.ABC):
     """Abstract class representing a concept drift configuration class."""
 
     def __init__(
         self,
@@ -60,35 +61,42 @@
     """Abstract class representing a concept drift streaming."""
 
     config_type = BaseConceptDriftConfig
 
     def __init__(
         self,
         config: Optional[BaseConceptDriftConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[BaseConceptDriftConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
-        super().__init__(callbacks=callbacks)
+        check_callbacks(
+            callbacks=callbacks,
+            expected_cls=BaseCallbackStreaming,  # type: ignore
+        )
+        super().__init__(callbacks=callbacks)  # type: ignore
         self.config = config  # type: ignore
         self.additional_vars = None
 
         self.num_instances = 0
         self.drift = False
         for callback in self.callbacks:  # type: ignore
             callback.set_detector(detector=self)
 
     def _set_additional_vars_callback(self) -> None:
         for callback in self.callbacks:  # type: ignore
-            if isinstance(callback, History):
+            if isinstance(callback, HistoryConceptDrift):
                 # callback.set_detector(detector=self)
                 callback.add_additional_vars(
                     vars_=self.additional_vars.keys(),  # type: ignore
                 )
 
     @property
     def additional_vars(self) -> Optional[Dict[str, Any]]:
@@ -174,18 +182,24 @@
     def update(self, value: Union[int, float], **kwargs) -> Dict[str, Any]:
         """Update method.
 
         :param value: value to update detector
         :type value: Union[int, float]
         """
         for callback in self.callbacks:  # type: ignore
-            callback.on_update_start(value=value, **kwargs)  # type: ignore
+            callback.on_update_start(  # type: ignore
+                value=value,
+                **kwargs,
+            )
         self._update(value=value, **kwargs)
         for callback in self.callbacks:  # type: ignore
-            callback.on_update_end(value=value, **kwargs)  # type: ignore
+            callback.on_update_end(  # type: ignore
+                value=value,
+                **kwargs,
+            )
 
         callbacks_logs = self._get_callbacks_logs()
         return callbacks_logs
 
     def _get_callbacks_logs(self) -> Dict[str, Any]:
         logs = {
             callback.name: callback.logs for callback in self.callbacks  # type: ignore
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/__init__.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/base.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/base.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base concept drift CUSUM based module."""
 
 import abc
 from typing import List, Optional, Union
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.base import (
     BaseConceptDriftStreaming,
     BaseConceptDriftStreamingConfig,
 )
 from frouros.utils.stats import Mean
 
 
@@ -128,22 +128,25 @@
     """CUSUM based algorithm class."""
 
     config_type = BaseCUSUMConfig
 
     def __init__(
         self,
         config: Optional[BaseCUSUMConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[BaseCUSUMConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "mean_error_rate": Mean(),
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/cusum.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/geometric_moving_average.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/cusum_based/page_hinkley.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Base concept drift SPC (statistical process control) module."""
 
 import abc
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.exceptions import InvalidAverageRunLengthError
 from frouros.detectors.concept_drift.streaming.base import (
     BaseConceptDriftStreamingConfig,
     BaseConceptDriftStreaming,
 )
 from frouros.utils.stats import Mean
 
@@ -86,22 +86,25 @@
     """Abstract class representing an SPC estimator."""
 
     config_type = BaseSPCConfig
 
     def __init__(
         self,
         config: Optional[BaseSPCConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[BaseSPCConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "warning": False,
@@ -149,22 +152,25 @@
     """Abstract class representing a SPC error estimator."""
 
     config_type = BaseSPCConfig
 
     def __init__(
         self,
         config: Optional[BaseSPCConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[BaseSPCConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "error_rate": Mean(),
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ddm.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/ecdd.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """ECDD (EWMA for Concept Drift Detection) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
     BaseSPC,
     BaseECDDConfig,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
@@ -34,22 +34,25 @@
     """
 
     config_type = ECDDWTConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[ECDDWTConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[ECDDWTConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,  # type: ignore
             callbacks=callbacks,
         )
         self.additional_vars = {
             "p": Mean(),
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/eddm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """EDDM (Early drift detection method) module."""
 
 import copy
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
     BaseSPCConfig,
     BaseSPC,
 )
 
 
 class EDDMConfig(BaseSPCConfig):
@@ -144,22 +144,25 @@
     """
 
     config_type = EDDMConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[EDDMConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[EDDMConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         # mean_distance_error = 0.0
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         mean_distance_error = 0.0
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/hddm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """HDDM (Hoeffding's inequality drift detection method) module."""
 
 import copy
 from typing import List, Optional, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
     BaseSPCConfig,
     BaseSPC,
 )
 from frouros.utils.stats import EWMA, Mean
 
 
@@ -330,22 +330,25 @@
     """
 
     config_type = HDDMAConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[HDDMAConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[HDDMAConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "test_type": (
@@ -626,22 +629,25 @@
     """
 
     config_type = HDDMWConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[HDDMWConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[HDDMWConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "test_type": (
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/statistical_process_control/rddm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """RDDM (Reactive Drift detection method) module."""
 
 from typing import List, Optional, Union
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.statistical_process_control.base import (
     BaseSPCConfig,
     BaseSPCError,
 )
 from frouros.utils.data_structures import CircularQueue
 from frouros.utils.stats import Mean
 
@@ -121,22 +121,25 @@
     """
 
     config_type = RDDMConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[RDDMConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[RDDMConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "num_warnings": 0,
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/adwin.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/adwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ADWIN (ADaptive WINdowing) module."""
 
 from collections import deque
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.window_based.base import (
     BaseWindowConfig,
     BaseWindow,
 )
 
 
 class Bucket:
@@ -291,22 +291,25 @@
     """
 
     config_type = ADWINConfig
 
     def __init__(
         self,
         config: Optional[ADWINConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[ADWINConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         num_buckets = 0
         self.additional_vars = {
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/base.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/kswin.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/kswin.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import itertools
 from collections import deque
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import ks_2samp  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.window_based.base import (
     BaseWindowConfig,
     BaseWindow,
 )
 
 
 class KSWINConfig(BaseWindowConfig):
@@ -112,22 +112,25 @@
     """
 
     config_type = KSWINConfig
 
     def __init__(
         self,
         config: Optional[KSWINConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[KSWINConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "window": deque(maxlen=self.config.min_num_instances),
```

### Comparing `frouros-0.3.1/frouros/detectors/concept_drift/streaming/window_based/stepd.py` & `frouros-0.3.2/frouros/detectors/concept_drift/streaming/window_based/stepd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """STEPD (Statistical test of equal proportions) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import norm  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.concept_drift.streaming.window_based.base import (
     BaseWindowConfig,
     BaseWindow,
 )
 from frouros.utils.data_structures import AccuracyQueue
 
 
@@ -99,22 +99,25 @@
     """
 
     config_type = STEPDConfig  # type: ignore
 
     def __init__(
         self,
         config: Optional[STEPDConfig] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param config: configuration parameters
         :type config: Optional[STEPDConfig]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             config=config,
             callbacks=callbacks,
         )
         self.additional_vars = {
             "correct_total": 0,
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/__init__.py` & `frouros-0.3.2/frouros/detectors/data_drift/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,18 +181,24 @@
         :param X: feature data
         :type X: numpy.ndarray
         :return: callbacks logs
         :rtype: Dict[str, Any]
         """
         self._check_fit_dimensions(X=X)
         for callback in self.callbacks:  # type: ignore
-            callback.on_fit_start()
+            callback.on_fit_start(
+                X=X,
+                **kwargs,
+            )
         self._fit(X=X, **kwargs)
         for callback in self.callbacks:  # type: ignore
-            callback.on_fit_end(X=X, **kwargs)
+            callback.on_fit_end(
+                X=X,
+                **kwargs,
+            )
 
         logs = self._get_callbacks_logs()
         return logs
 
     def reset(self) -> None:
         """Reset method."""
         self.X_ref = None
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/__init__.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 """Base data drift batch module."""
 
 import abc
 from typing import Any, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import (
     BaseDataDrift,
     BaseDataType,
     BaseStatisticalType,
 )
 from frouros.detectors.data_drift.exceptions import (
     MismatchDimensionError,
 )
+from frouros.utils.checks import check_callbacks
 
 
 class BaseDataDriftBatch(BaseDataDrift):
     """Abstract class representing a data drift batch detector."""
 
     def __init__(
         self,
         data_type: BaseDataType,
         statistical_type: BaseStatisticalType,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param data_type: data type
         :type data_type: BaseDataType
         :param statistical_type: statistical type
         :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback], List[BaseCallback]]
+        :type callbacks: Optional[Union[BaseCallbackBatch], List[BaseCallbackBatch]]
         """
-        super().__init__(
+        check_callbacks(
             callbacks=callbacks,
+            expected_cls=BaseCallbackBatch,  # type: ignore
+        )
+        super().__init__(
+            callbacks=callbacks,  # type: ignore
             data_type=data_type,
             statistical_type=statistical_type,
         )
         for callback in self.callbacks:  # type: ignore
             callback.set_detector(detector=self)
 
     def _fit(
@@ -54,18 +59,21 @@
         **kwargs,
     ) -> Tuple[np.ndarray, Dict[str, Any]]:
         """Compare values.
 
         :param X: feature data
         :type X: numpy.ndarray
         :return: compare result and callbacks logs
-        :rtype: Tuple[np.ndarray, Dict[str, Any]]
+        :rtype: Tuple[numpy.ndarray, Dict[str, Any]]
         """
         for callback in self.callbacks:  # type: ignore
-            callback.on_compare_start()  # type: ignore
+            callback.on_compare_start(  # type: ignore
+                X_ref=self.X_ref,
+                X_test=X,
+            )
         result = self._compare(X=X, **kwargs)
         for callback in self.callbacks:  # type: ignore
             callback.on_compare_end(  # type: ignore
                 result=result,
                 X_ref=self.X_ref,
                 X_test=X,
             )
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import abc
 from collections import namedtuple
 from typing import Any, Callable, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import rv_histogram  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import (
     NumericalData,
     BaseStatisticalType,
     UnivariateData,
 )
 from frouros.detectors.data_drift.batch.base import BaseDataDriftBatch
 
@@ -22,26 +22,26 @@
     """Abstract class representing a distance based detector."""
 
     def __init__(
         self,
         statistical_type: BaseStatisticalType,
         statistical_method: Callable,
         statistical_kwargs: Dict[str, Any],
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param statistical_type: statistical type
         :type statistical_type: BaseStatisticalType
         :param statistical_method: statistical method
         :type statistical_method: Callable
         :param statistical_kwargs: statistical kwargs
         :type statistical_kwargs: Dict[str, Any]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=statistical_type,
             callbacks=callbacks,
         )
         self.statistical_method = statistical_method
@@ -115,25 +115,25 @@
 class BaseDistanceBasedBins(BaseDistanceBased):
     """Abstract class representing a distance based bins detector."""
 
     def __init__(
         self,
         statistical_method,
         statistical_kwargs,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         num_bins: int = 10,
     ) -> None:
         """Init method.
 
         :param statistical_method: statistical method
         :type statistical_method: Callable
         :param statistical_kwargs: statistical kwargs
         :type statistical_kwargs: Dict[str, Any]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=statistical_method,
             statistical_kwargs={**statistical_kwargs, "num_bins": num_bins},
@@ -197,25 +197,25 @@
 class BaseDistanceBasedProbability(BaseDistanceBased):
     """Abstract class representing a distance based probability detector."""
 
     def __init__(
         self,
         statistical_method,
         statistical_kwargs,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         num_bins: int = 10,
     ) -> None:
         """Init method.
 
         :param statistical_method: statistical method
         :type statistical_method: Callable
         :param statistical_kwargs: statistical kwargs
         :type statistical_kwargs: Dict[str, Any]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=statistical_method,
             statistical_kwargs=statistical_kwargs,
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/bhattacharyya_distance.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Bhattacharyya distance module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
 )
 
 
 class BhattacharyyaDistance(BaseDistanceBasedBins):
     """Bhattacharyya distance [bhattacharyya1946measure]_ detector.
@@ -19,15 +19,15 @@
         "On a measure of divergence between two multinomial populations."
         Sankhyā: the indian journal of statistics (1946): 401-406.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
         :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/emd.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/emd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """EMD (Earth Mover's Distance) module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import wasserstein_distance  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import UnivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
 
 
@@ -21,21 +21,21 @@
     .. [rubner2000earth] Rubner, Yossi, Carlo Tomasi, and Leonidas J. Guibas.
         "The earth mover's distance as a metric for image retrieval."
         International journal of computer vision 40.2 (2000): 99.
     """
 
     def __init__(
         self,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         **kwargs,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             statistical_type=UnivariateData(),
             statistical_method=self._emd,
             statistical_kwargs=kwargs,
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hellinger_distance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Hellinger distance module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
 )
 
 
 class HellingerDistance(BaseDistanceBasedBins):
     """Hellinger distance [hellinger1909neue]_ detector.
@@ -20,22 +20,22 @@
         veränderlichen."
         Journal für die reine und angewandte Mathematik 1909.136 (1909): 210-271.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         sqrt_div = np.sqrt(2)
         super().__init__(
             statistical_method=self._hellinger,
             statistical_kwargs={
                 "num_bins": num_bins,
                 "sqrt_div": sqrt_div,
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/hi_normalized_complement.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """HI (Histogram intersection) normalized complement module."""
 
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
 )
 
 
 class HINormalizedComplement(BaseDistanceBasedBins):
     """HI (Histogram intersection) normalized complement [swain1991color]_ detector.
@@ -19,22 +19,22 @@
         "Color Indexing International Journal of Computer
         Vision 7." (1991): 11-32.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             statistical_method=self._hi_normalized_complement,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/js.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/js.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """JS (Jensen-Shannon distance) module."""
 
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.spatial.distance import jensenshannon  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedProbability,
     DistanceResult,
 )
 
 
 class JS(BaseDistanceBasedProbability):
@@ -21,23 +21,23 @@
         "Divergence measures based on the Shannon entropy."
         IEEE Transactions on Information theory 37.1 (1991): 145-151.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         **kwargs,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             statistical_method=self._js,
             statistical_kwargs={
                 "num_bins": num_bins,
                 **kwargs,
             },
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/kl.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/kl.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """KL (Kullback-Leibler divergence distance) module."""
 
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np  # type: ignore
 from scipy.special import rel_entr  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedProbability,
     DistanceResult,
 )
 
 
 class KL(BaseDistanceBasedProbability):
@@ -21,23 +21,23 @@
         "On information and sufficiency."
         The annals of mathematical statistics 22.1 (1951): 79-86.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
         **kwargs,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: number of bins in which to divide probabilities
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             statistical_method=self._kl,
             statistical_kwargs={**kwargs, "num_bins": num_bins},
             callbacks=callbacks,
         )
         self.num_bins = num_bins
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/mmd.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/mmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import math
 from typing import Callable, Generator, Optional, List, Union
 
 import numpy as np  # type: ignore
 import tqdm  # type: ignore
 from scipy.spatial.distance import cdist  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import MultivariateData
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
 
 
@@ -43,24 +43,24 @@
         The Journal of Machine Learning Research 13.1 (2012): 723-773.
     """
 
     def __init__(
         self,
         kernel: Callable = rbf_kernel,
         chunk_size: Optional[int] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param kernel: kernel function
         :type kernel: Callable
         :param chunk_size: chunk size value
         :type chunk_size: Optional[int]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             statistical_type=MultivariateData(),
             statistical_method=self._mmd,
             statistical_kwargs={
                 "kernel": kernel,
             },
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/distance_based/psi.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/distance_based/psi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """PSI (Population Stability Index) module."""
 
 import sys
 from typing import List, Optional, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.batch.distance_based.base import (
     BaseDistanceBasedBins,
     DistanceResult,
 )
 
 
 class PSI(BaseDistanceBasedBins):
@@ -21,22 +21,22 @@
         "Enterprise risk management: coping with model risk in a large bank."
         Journal of the Operational Research Society 61.2 (2010): 179-190.
     """
 
     def __init__(
         self,
         num_bins: int = 10,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param num_bins: number of bins in which to divide probabilities
         :type num_bins: int
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             statistical_method=self._psi,
             statistical_kwargs={
                 "num_bins": num_bins,
             },
             callbacks=callbacks,
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/chisquare.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/chisquare.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import collections
 from typing import Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import chi2_contingency  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import CategoricalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (  # type: ignore
     BaseStatisticalTest,
     StatisticalResult,
 )
 
 
@@ -24,20 +24,21 @@
         case of a correlated system of variables is such that it can be reasonably
         supposed to have arisen from random sampling."
         The London, Edinburgh, and Dublin Philosophical Magazine and Journal of
         Science 50.302 (1900): 157-175.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
+        self,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             data_type=CategoricalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/cvm.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/cvm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """CVMTest (Cramér-von Mises test) module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import cramervonmises_2samp  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
 from frouros.detectors.data_drift.exceptions import InsufficientSamplesError
 
@@ -21,20 +21,21 @@
 
     .. [cramer1928composition] Cramér, Harald.
         "On the composition of elementary errors: First paper: Mathematical deductions."
         Scandinavian Actuarial Journal 1928.1 (1928): 13-74.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
+        self,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/ks.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/ks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """KSTest (Kolmogorov-Smirnov test) module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import ks_2samp  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
 
 
@@ -20,20 +20,21 @@
 
     .. [massey1951kolmogorov] Massey Jr, Frank J.
         "The Kolmogorov-Smirnov test for goodness of fit."
         Journal of the American statistical Association 46.253 (1951): 68-78.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
+        self,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py` & `frouros-0.3.2/frouros/detectors/data_drift/batch/statistical_test/welch_t_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Welch's T-test module."""
 
 from typing import Optional, List, Union
 
 import numpy as np  # type: ignore
 from scipy.stats import ttest_ind  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.batch.base import BaseCallbackBatch
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.batch.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
 
 
@@ -21,20 +21,21 @@
     .. [welch1947generalization] Welch, Bernard L.
         "The generalization of ‘STUDENT'S’problem when several different population
         varlances are involved."
         Biometrika 34.1-2 (1947): 28-35.
     """
 
     def __init__(
-        self, callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None
+        self,
+        callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]] = None,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackBatch, List[BaseCallbackBatch]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
         )
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/streaming/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/streaming/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 """Base data drift batch module."""
 
 import abc
 from typing import Any, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.data_drift.base import (
     BaseDataDrift,
     BaseDataType,
     BaseResult,
     BaseStatisticalType,
 )
+from frouros.utils.checks import check_callbacks
 
 
 class BaseDataDriftStreaming(BaseDataDrift):
     """Abstract class representing a data drift streaming detector."""
 
     def __init__(
         self,
         data_type: BaseDataType,
         statistical_type: BaseStatisticalType,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param data_type: data type
         :type data_type: BaseDataType
         :param statistical_type: statistical type
         :type statistical_type: BaseStatisticalType
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback], List[BaseCallback]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming],
+        List[BaseCallbackStreaming]]
         """
-        super().__init__(
+        check_callbacks(
             callbacks=callbacks,
+            expected_cls=BaseCallbackStreaming,  # type: ignore
+        )
+        super().__init__(
+            callbacks=callbacks,  # type: ignore
             data_type=data_type,
             statistical_type=statistical_type,
         )
         self.num_instances = 0
         for callback in self.callbacks:  # type: ignore
             callback.set_detector(detector=self)
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/streaming/distance_based/mmd.py` & `frouros-0.3.2/frouros/detectors/data_drift/streaming/distance_based/mmd.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """MMD (Maximum Mean Discrepancy) module."""
 
 from typing import Any, Callable, Dict, Optional, List, Tuple, Union
 
 import numpy as np  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.data_drift.base import NumericalData, MultivariateData
 from frouros.detectors.data_drift.batch import MMD as MMDBatch  # noqa: N811
 from frouros.detectors.data_drift.batch.distance_based.mmd import rbf_kernel
 from frouros.detectors.data_drift.streaming.distance_based.base import (
     BaseDistanceBased,
     DistanceResult,
 )
@@ -26,26 +26,29 @@
     """
 
     def __init__(
         self,
         window_size: int,
         kernel: Callable = rbf_kernel,
         chunk_size: Optional[int] = None,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
     ) -> None:
         """Init method.
 
         :param window_size: window size
         :type window_size: int
         :param kernel: kernel function
         :type kernel: Callable
         :param chunk_size: chunk size value
         :type chunk_size: Optional[int]
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[Callback, List[BaseCallback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=MultivariateData(),
             callbacks=callbacks,
         )
         self.mmd = MMDBatch(
```

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/base.py` & `frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/detectors/data_drift/streaming/statistical_test/ks.py` & `frouros-0.3.2/frouros/detectors/data_drift/streaming/statistical_test/ks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import numpy as np  # type: ignore
 from scipy.stats._stats_py import (  # type: ignore
     _compute_prob_outside_square,
     _compute_outer_prob_inside_method,
 )
 from scipy.stats.distributions import kstwo  # type: ignore
 
-from frouros.callbacks.base import BaseCallback
+from frouros.callbacks.streaming.base import BaseCallbackStreaming
 from frouros.detectors.data_drift.base import NumericalData, UnivariateData
 from frouros.detectors.data_drift.streaming.statistical_test.base import (
     BaseStatisticalTest,
     StatisticalResult,
 )
 from frouros.utils.data_structures import CircularQueue
 
@@ -37,21 +37,24 @@
         test."
         Proceedings of the 22nd ACM SIGKDD international conference on knowledge
         discovery and data mining. 2016.
     """
 
     def __init__(
         self,
-        callbacks: Optional[Union[BaseCallback, List[BaseCallback]]] = None,
+        callbacks: Optional[
+            Union[BaseCallbackStreaming, List[BaseCallbackStreaming]]
+        ] = None,
         window_size: int = 10,
     ) -> None:
         """Init method.
 
         :param callbacks: callbacks
-        :type callbacks: Optional[Union[BaseCallback, List[Callback]]]
+        :type callbacks: Optional[Union[BaseCallbackStreaming,
+        List[BaseCallbackStreaming]]]
         :param window_size: window size
         :type window_size: int
         """
         super().__init__(
             data_type=NumericalData(),
             statistical_type=UnivariateData(),
             callbacks=callbacks,
```

### Comparing `frouros-0.3.1/frouros/metrics/base.py` & `frouros-0.3.2/frouros/metrics/base.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/metrics/prequential_error.py` & `frouros-0.3.2/frouros/metrics/prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/tests/conftest.py` & `frouros-0.3.2/frouros/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/tests/integration/test_callback.py` & `frouros-0.3.2/frouros/tests/integration/test_callback.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 from typing import List, Tuple
 
 import numpy as np  # type: ignore
 import pytest  # type: ignore
 import sklearn  # type: ignore # pylint: disable=import-error
 
 from frouros.callbacks.batch import (
-    PermutationTestOnBatchData,
-    ResetOnBatchDataDrift,
+    PermutationTestDistanceBased,
+    ResetStatisticalTest,
 )
 from frouros.callbacks.streaming import (
-    History,
+    HistoryConceptDrift,
     mSPRT,
     WarningSamplesBuffer,
 )
 from frouros.detectors.concept_drift import (
     ADWIN,
     CUSUM,
     DDM,
@@ -84,15 +84,15 @@
     :type expected_p_value: float
     """
     np.random.seed(seed=31)
 
     permutation_test_name = "permutation_test"
     detector = detector_class(  # type: ignore
         callbacks=[
-            PermutationTestOnBatchData(
+            PermutationTestDistanceBased(
                 num_permutations=100,
                 random_state=31,
                 num_jobs=-1,
                 name=permutation_test_name,
             )
         ]
     )
@@ -107,34 +107,34 @@
     )
 
 
 @pytest.mark.parametrize(
     "detector_class",
     [CVMTest, KSTest, WelchTTest],
 )
-def test_batch_reset_on_data_drift(
+def test_batch_reset_on_statistical_test_data_drift(
     X_ref_univariate,  # noqa: N803
     X_test_univariate,
     detector_class: BaseDataDriftBatch,
     mocker,
 ) -> None:
-    """Test batch reset on data drift callback.
+    """Test batch reset on statistical test data drift callback.
 
     :param X_ref_univariate: reference univariate data
     :type X_ref_univariate: numpy.ndarray
     :param X_test_univariate: test univariate data
     :type X_test_univariate: numpy.ndarray
     :param detector_class: detector distance
     :type detector_class: BaseDataDriftBatch
     """
     mocker.patch("frouros.detectors.data_drift.batch.base.BaseDataDriftBatch.reset")
 
     detector = detector_class(  # type: ignore
         callbacks=[
-            ResetOnBatchDataDrift(
+            ResetStatisticalTest(
                 alpha=0.01,
             ),
         ],
     )
     _ = detector.fit(X=X_ref_univariate)
     _ = detector.compare(X=X_test_univariate)
     detector.reset.assert_called_once()  # type: ignore # pylint: disable=no-member
@@ -165,15 +165,15 @@
 
     :param model_errors: model errors
     :type model_errors: List[int]
     :param detector_class: concept drift detector
     :type detector_class: BaseConceptDrift
     """
     name = "history"
-    detector = detector_class(callbacks=History(name=name))  # type: ignore
+    detector = detector_class(callbacks=HistoryConceptDrift(name=name))  # type: ignore
 
     for error in model_errors:
         history = detector.update(value=error)
         status = detector.status
         if status["drift"]:
             assert history[name]["drift"][-1]
             assert not any(history[name]["drift"][:-1])
```

### Comparing `frouros-0.3.1/frouros/tests/integration/test_concept_drift.py` & `frouros-0.3.2/frouros/tests/integration/test_concept_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/tests/integration/test_data_drift.py` & `frouros-0.3.2/frouros/tests/integration/test_data_drift.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/tests/integration/test_real.py` & `frouros-0.3.2/frouros/tests/integration/test_real.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/tests/integration/test_synthetic.py` & `frouros-0.3.2/frouros/tests/integration/test_synthetic.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/tests/unit/metrics/test_prequential_error.py` & `frouros-0.3.2/frouros/tests/unit/metrics/test_prequential_error.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/utils/data_structures.py` & `frouros-0.3.2/frouros/utils/data_structures.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros/utils/stats.py` & `frouros-0.3.2/frouros/utils/stats.py`

 * *Files identical despite different names*

### Comparing `frouros-0.3.1/frouros.egg-info/PKG-INFO` & `frouros-0.3.2/frouros.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: frouros
-Version: 0.3.1
-Summary: An open source Python library for drift detection in machine Learning systems
+Version: 0.3.2
+Summary: An open source Python library for drift detection in machine learning systems
 Home-page: https://github.com/IFCA/frouros
 Author: Jaime Céspedes Sisniega
 Author-email: cespedes@ifca.unican.es
 Maintainer: Jaime Céspedes Sisniega
 Maintainer-email: cespedes@ifca.unican.es
 License: BSD-3-Clause
 Project-URL: homepage, https://frouros.readthedocs.io
@@ -409,14 +409,20 @@
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">N</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;">Incremental Kolmogorov-Smirnov test</td>
     <td style="text-align: center; border: 1px solid grey; padding: 8px;"><a href="https://doi.org/10.1145/2939672.2939836">dos Reis et al. (2016)</a></td>
   </tr>
 </tbody>
 </table>
 
+## ❗ What is and what is not Frouros?
+
+Unlike other libraries that in addition to provide drift detection algorithms, include other functionalities such as anomaly/outlier detection, adversarial detection, imbalance learning, among others, Frouros has and will **ONLY** have one purpose: **drift detection**.
+
+We firmly believe that machine learning related libraries or frameworks should not follow [Jack of all trades, master of none](https://en.wikipedia.org/wiki/Jack_of_all_trades,_master_of_none) principle. Instead, they should be focused on a single task and do it well.
+
 ## ✅ Who is using Frouros?
 
 Frouros is actively being used by the following projects to implement drift
 detection in machine learning pipelines:
 
  * [AI4EOSC](https://ai4eosc.eu).
  * [iMagine](https://imagine-ai.eu).
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: frouros Version: 0.3.1 Summary: An open source
-Python library for drift detection in machine Learning systems Home-page:
+Metadata-Version: 2.1 Name: frouros Version: 0.3.2 Summary: An open source
+Python library for drift detection in machine learning systems Home-page:
 https://github.com/IFCA/frouros Author: Jaime CÃ©spedes Sisniega Author-email:
 cespedes@ifca.unican.es Maintainer: Jaime CÃ©spedes Sisniega Maintainer-email:
 cespedes@ifca.unican.es License: BSD-3-Clause Project-URL: homepage, https://
 frouros.readthedocs.io Project-URL: repository, https://github.com/IFCA/frouros
 Project-URL: documentation, https://frouros.readthedocs.io Project-URL:
 download, https://pypi.org/project/frouros/ Keywords: drift-detection,concept-
 drift,data-drift,machine-learning,data-science,machine-learning-
@@ -122,23 +122,30 @@
                                                         test
                                U            N           Welch's T-Test      Welch_(1947)
                    Distance    M            N           MMD                 Gretton_et_al._(2012)
                    based
          Streaming Statistical                          Incremental
                    test        U            N           Kolmogorov-Smirnov  dos_Reis_et_al._(2016)
                                                         test
-## â Who is using Frouros? Frouros is actively being used by the following
-projects to implement drift detection in machine learning pipelines: *
-[AI4EOSC](https://ai4eosc.eu). * [iMagine](https://imagine-ai.eu). If you want
-your project listed here, do not hesitate to send us a pull request. ## ð
-Contributing Check out the [contribution](https://github.com/IFCA/frouros/blob/
-main/CONTRIBUTING.md) section. ## ð¬ Citation Although Frouros paper is still
-in preprint, if you want to cite it you can use the [preprint](https://
-arxiv.org/abs/2208.06868) version (to be replaced by the paper once is
-published). ```bibtex @article{cespedes2022frouros, title={Frouros: A Python
-library for drift detection in Machine Learning problems}, author={C{\'e}spedes
-Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro }, journal={arXiv
-preprint arXiv:2208.06868}, year={2022} } ``` ## ð License Frouros is an
-open-source software licensed under the [BSD-3-Clause license](https://
-github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements Frouros
-has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad de
-Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
+## â What is and what is not Frouros? Unlike other libraries that in addition
+to provide drift detection algorithms, include other functionalities such as
+anomaly/outlier detection, adversarial detection, imbalance learning, among
+others, Frouros has and will **ONLY** have one purpose: **drift detection**. We
+firmly believe that machine learning related libraries or frameworks should not
+follow [Jack of all trades, master of none](https://en.wikipedia.org/wiki/
+Jack_of_all_trades,_master_of_none) principle. Instead, they should be focused
+on a single task and do it well. ## â Who is using Frouros? Frouros is
+actively being used by the following projects to implement drift detection in
+machine learning pipelines: * [AI4EOSC](https://ai4eosc.eu). * [iMagine](https:
+//imagine-ai.eu). If you want your project listed here, do not hesitate to send
+us a pull request. ## ð Contributing Check out the [contribution](https://
+github.com/IFCA/frouros/blob/main/CONTRIBUTING.md) section. ## ð¬ Citation
+Although Frouros paper is still in preprint, if you want to cite it you can use
+the [preprint](https://arxiv.org/abs/2208.06868) version (to be replaced by the
+paper once is published). ```bibtex @article{cespedes2022frouros, title=
+{Frouros: A Python library for drift detection in Machine Learning problems},
+author={C{\'e}spedes Sisniega, Jaime and L{\'o}pez Garc{\'\i}a, {\'A}lvaro },
+journal={arXiv preprint arXiv:2208.06868}, year={2022} } ``` ## ð License
+Frouros is an open-source software licensed under the [BSD-3-Clause license]
+(https://github.com/IFCA/frouros/blob/main/LICENSE). ## ð Acknowledgements
+Frouros has received funding from the Agencia Estatal de InvestigaciÃ³n, Unidad
+de Excelencia MarÃ­a de Maeztu, ref. MDM-2017-0765.
```

### Comparing `frouros-0.3.1/frouros.egg-info/SOURCES.txt` & `frouros-0.3.2/frouros.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 frouros.egg-info/requires.txt
 frouros.egg-info/top_level.txt
 frouros/callbacks/__init__.py
 frouros/callbacks/base.py
 frouros/callbacks/batch/__init__.py
 frouros/callbacks/batch/base.py
 frouros/callbacks/batch/permutation_test.py
-frouros/callbacks/batch/reset_drift.py
+frouros/callbacks/batch/reset.py
 frouros/callbacks/streaming/__init__.py
 frouros/callbacks/streaming/base.py
 frouros/callbacks/streaming/history.py
 frouros/callbacks/streaming/msprt.py
 frouros/callbacks/streaming/warning_samples.py
 frouros/common/__init__.py
 frouros/common/exceptions.py
@@ -92,11 +92,11 @@
 frouros/tests/integration/test_data_drift.py
 frouros/tests/integration/test_real.py
 frouros/tests/integration/test_synthetic.py
 frouros/tests/unit/__init__.py
 frouros/tests/unit/metrics/__init__.py
 frouros/tests/unit/metrics/test_prequential_error.py
 frouros/utils/__init__.py
+frouros/utils/checks.py
 frouros/utils/data_structures.py
-frouros/utils/decorators.py
 frouros/utils/logger.py
 frouros/utils/stats.py
```

### Comparing `frouros-0.3.1/pyproject.toml` & `frouros-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "frouros"
-version = "0.3.1"
-description = "An open source Python library for drift detection in machine Learning systems"
+version = "0.3.2"
+description = "An open source Python library for drift detection in machine learning systems"
 authors = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 maintainers = [
     {name = "Jaime Céspedes Sisniega", email = "cespedes@ifca.unican.es"}
 ]
 readme = "README.md"
@@ -36,15 +36,15 @@
 ]
 requires-python = ">=3.8,<3.12"
 dependencies = [
     "matplotlib>=3.6.0,<3.7",
     "numpy>=1.24.0,<1.25",
     "requests>=2.31.0,<2.32",
     "scipy>=1.10.0,<1.11",
-    "tqdm>=4.64.0,<4.65",
+    "tqdm>=4.65,<5",
 ]
 
 [project.optional-dependencies]
 docs = [
     "sphinx>=5.3.0,<5.4",
     "sphinx-book-theme>=1.0.0,<1.1",
     "sphinxcontrib-bibtex>=2.5.0,<2.6",
```

### Comparing `frouros-0.3.1/setup.py` & `frouros-0.3.2/setup.py`

 * *Files identical despite different names*

