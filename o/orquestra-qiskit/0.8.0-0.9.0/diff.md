# Comparing `tmp/orquestra-qiskit-0.8.0.tar.gz` & `tmp/orquestra-qiskit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "orquestra-qiskit-0.8.0.tar", last modified: Fri Jan 13 15:53:49 2023, max compression
+gzip compressed data, was "orquestra-qiskit-0.9.0.tar", last modified: Tue Feb  7 21:01:20 2023, max compression
```

## Comparing `orquestra-qiskit-0.8.0.tar` & `orquestra-qiskit-0.9.0.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.886284 orquestra-qiskit-0.8.0/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.817116 orquestra-qiskit-0.8.0/.github/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.817718 orquestra-qiskit-0.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.github/pull_request_template.md
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.818742 orquestra-qiskit-0.8.0/.github/workflows/
--rw-r--r--   0 maxradin   (501) staff       (20)     1013 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.github/workflows/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      876 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.github/workflows/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      945 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.github/workflows/style.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1799 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/.gitignore
--rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/LICENSE
--rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/MANIFEST.in
--rw-r--r--   0 maxradin   (501) staff       (20)      487 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     2187 2023-01-13 15:53:49.886490 orquestra-qiskit-0.8.0/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     1584 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/README.md
--rw-r--r--   0 maxradin   (501) staff       (20)     1328 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)      924 2023-01-13 15:53:49.887254 orquestra-qiskit-0.8.0/setup.cfg
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.810277 orquestra-qiskit-0.8.0/src/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.809120 orquestra-qiskit-0.8.0/src/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.809302 orquestra-qiskit-0.8.0/src/orquestra/integrations/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.819508 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/__init__.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.821454 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/
--rw-r--r--   0 maxradin   (501) staff       (20)      359 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)    12932 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_circuit_conversions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2941 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_pauli_conversions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2854 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_qiskit_expressions.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5221 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_symengine_expressions.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.823385 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/noise/
--rw-r--r--   0 maxradin   (501) staff       (20)      443 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/noise/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5721 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/noise/basic.py
--rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/py.typed
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.824771 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/runner/
--rw-r--r--   0 maxradin   (501) staff       (20)      295 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/runner/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1981 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/runner/_ibmq_runner.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3756 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/runner/_qiskit_runner.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.844946 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/simulator/
--rw-r--r--   0 maxradin   (501) staff       (20)      281 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/simulator/__init__.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2921 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/simulator/_qiskit_wavefunction_simulator.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.865836 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/
--rw-r--r--   0 maxradin   (501) staff       (20)     2187 2023-01-13 15:53:49.000000 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 maxradin   (501) staff       (20)     2869 2023-01-13 15:53:49.000000 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:53:49.000000 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-01-13 15:53:49.000000 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/not-zip-safe
--rw-r--r--   0 maxradin   (501) staff       (20)      116 2023-01-13 15:53:49.000000 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/requires.txt
--rw-r--r--   0 maxradin   (501) staff       (20)       10 2023-01-13 15:53:49.000000 orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.810763 orquestra-qiskit-0.8.0/subtrees/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.870259 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/
--rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/MANIFEST.in
--rw-r--r--   0 maxradin   (501) staff       (20)     3835 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/Makefile
--rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/README.rst
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.811860 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.870669 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/coverage/
--rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.871149 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/publish-release/
--rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.871543 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/
--rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.871838 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/style/
--rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/style/action.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.872129 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/bin/
--rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/pyproject.toml
--rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/pytest.ini
--rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/sample_setup.py
--rw-r--r--   0 maxradin   (501) staff       (20)      585 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/setup_extras.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.872442 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/tests/
--rw-r--r--   0 maxradin   (501) staff       (20)     1131 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
--rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/variables.mk
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.873277 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/
--rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
--rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
--rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.812991 orquestra-qiskit-0.8.0/tests/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.813165 orquestra-qiskit-0.8.0/tests/orquestra/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.813356 orquestra-qiskit-0.8.0/tests/orquestra/integrations/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.814009 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.879930 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/
--rw-r--r--   0 maxradin   (501) staff       (20)    19072 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/circuit_conversions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3313 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/pauli_conversions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     3287 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/qiskit_expressions_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     7398 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/symengine_expressions_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.881917 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/noise/
--rw-r--r--   0 maxradin   (501) staff       (20)     3029 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/noise/basic_test.py
-drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-01-13 15:53:49.885458 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/
--rw-r--r--   0 maxradin   (501) staff       (20)     1051 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/_ibmq_runner_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     5085 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/_qiskit_runner_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)     2084 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/_qiskit_wavefunction_simulator_test.py
--rw-r--r--   0 maxradin   (501) staff       (20)   552113 2023-01-13 15:53:42.000000 orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/jobs_and_batches_with_different_qubits.pickle
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.436706 orquestra-qiskit-0.9.0/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.418175 orquestra-qiskit-0.9.0/.github/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.418663 orquestra-qiskit-0.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 maxradin   (501) staff       (20)      605 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      600 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 maxradin   (501) staff       (20)      533 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.github/pull_request_template.md
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.419471 orquestra-qiskit-0.9.0/.github/workflows/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1013 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.github/workflows/coverage.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      876 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.github/workflows/publish_release.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      945 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.github/workflows/style.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1799 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/.gitignore
+-rw-r--r--   0 maxradin   (501) staff       (20)    11357 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/LICENSE
+-rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/MANIFEST.in
+-rw-r--r--   0 maxradin   (501) staff       (20)      487 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/Makefile
+-rw-r--r--   0 maxradin   (501) staff       (20)     2187 2023-02-07 21:01:20.436877 orquestra-qiskit-0.9.0/PKG-INFO
+-rw-r--r--   0 maxradin   (501) staff       (20)     1584 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/README.md
+-rw-r--r--   0 maxradin   (501) staff       (20)     1328 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/pyproject.toml
+-rw-r--r--   0 maxradin   (501) staff       (20)      924 2023-02-07 21:01:20.438303 orquestra-qiskit-0.9.0/setup.cfg
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.413587 orquestra-qiskit-0.9.0/src/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.412221 orquestra-qiskit-0.9.0/src/orquestra/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.412381 orquestra-qiskit-0.9.0/src/orquestra/integrations/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.420647 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/
+-rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/__init__.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.422289 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/
+-rw-r--r--   0 maxradin   (501) staff       (20)      359 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)    12932 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_circuit_conversions.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2941 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_pauli_conversions.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2854 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_qiskit_expressions.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5221 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_symengine_expressions.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.422997 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/noise/
+-rw-r--r--   0 maxradin   (501) staff       (20)      443 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/noise/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5721 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/noise/basic.py
+-rw-r--r--   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/py.typed
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.423994 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/runner/
+-rw-r--r--   0 maxradin   (501) staff       (20)      295 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/runner/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2082 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/runner/_ibmq_runner.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     4349 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/runner/_qiskit_runner.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.424636 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/simulator/
+-rw-r--r--   0 maxradin   (501) staff       (20)      281 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/simulator/__init__.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2921 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/simulator/_qiskit_wavefunction_simulator.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.427518 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/
+-rw-r--r--   0 maxradin   (501) staff       (20)     2187 2023-02-07 21:01:20.000000 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 maxradin   (501) staff       (20)     2869 2023-02-07 21:01:20.000000 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-07 21:01:20.000000 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)        1 2023-02-07 21:01:19.000000 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/not-zip-safe
+-rw-r--r--   0 maxradin   (501) staff       (20)      116 2023-02-07 21:01:20.000000 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/requires.txt
+-rw-r--r--   0 maxradin   (501) staff       (20)       10 2023-02-07 21:01:20.000000 orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.413864 orquestra-qiskit-0.9.0/subtrees/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.429782 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/
+-rw-r--r--   0 maxradin   (501) staff       (20)        9 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/MANIFEST.in
+-rw-r--r--   0 maxradin   (501) staff       (20)     3835 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/Makefile
+-rw-r--r--   0 maxradin   (501) staff       (20)     5600 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/README.rst
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.414670 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.430085 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/coverage/
+-rw-r--r--   0 maxradin   (501) staff       (20)      790 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.430439 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/publish-release/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3132 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.430736 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/
+-rw-r--r--   0 maxradin   (501) staff       (20)      458 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/ssh_setup/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.431054 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/style/
+-rw-r--r--   0 maxradin   (501) staff       (20)      467 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/style/action.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.431356 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/bin/
+-rwxr-xr-x   0 maxradin   (501) staff       (20)     2756 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     1253 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/pyproject.toml
+-rw-r--r--   0 maxradin   (501) staff       (20)       24 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/pytest.ini
+-rw-r--r--   0 maxradin   (501) staff       (20)     1526 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/sample_setup.py
+-rw-r--r--   0 maxradin   (501) staff       (20)      585 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/setup_extras.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.431654 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/tests/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1131 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py
+-rw-r--r--   0 maxradin   (501) staff       (20)       19 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/variables.mk
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.432635 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1233 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)      696 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml
+-rw-r--r--   0 maxradin   (501) staff       (20)     1248 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.415472 orquestra-qiskit-0.9.0/tests/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.415584 orquestra-qiskit-0.9.0/tests/orquestra/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.415698 orquestra-qiskit-0.9.0/tests/orquestra/integrations/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.416122 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.433992 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/
+-rw-r--r--   0 maxradin   (501) staff       (20)    19072 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/circuit_conversions_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3313 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/pauli_conversions_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     3287 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/qiskit_expressions_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     7398 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/symengine_expressions_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.434259 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/noise/
+-rw-r--r--   0 maxradin   (501) staff       (20)     3029 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/noise/basic_test.py
+drwxr-xr-x   0 maxradin   (501) staff       (20)        0 2023-02-07 21:01:20.435888 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/
+-rw-r--r--   0 maxradin   (501) staff       (20)     1569 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/_ibmq_runner_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     5655 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/_qiskit_runner_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)     2063 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/_qiskit_wavefunction_simulator_test.py
+-rw-r--r--   0 maxradin   (501) staff       (20)   552113 2023-02-07 21:01:12.000000 orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/jobs_and_batches_with_different_qubits.pickle
```

### Comparing `orquestra-qiskit-0.8.0/.github/ISSUE_TEMPLATE/bug_report.md` & `orquestra-qiskit-0.9.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/.github/ISSUE_TEMPLATE/feature_request.md` & `orquestra-qiskit-0.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/.github/pull_request_template.md` & `orquestra-qiskit-0.9.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/.github/workflows/coverage.yml` & `orquestra-qiskit-0.9.0/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/.github/workflows/publish_release.yml` & `orquestra-qiskit-0.9.0/.github/workflows/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/.github/workflows/style.yml` & `orquestra-qiskit-0.9.0/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/.gitignore` & `orquestra-qiskit-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/LICENSE` & `orquestra-qiskit-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/PKG-INFO` & `orquestra-qiskit-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-qiskit
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra Qiskit package"
 Home-page: https://github.com/zapatacomputing/orquestra-qiskit
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-qiskit-0.8.0/README.md` & `orquestra-qiskit-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/pyproject.toml` & `orquestra-qiskit-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/setup.cfg` & `orquestra-qiskit-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_circuit_conversions.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_circuit_conversions.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_pauli_conversions.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_pauli_conversions.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_qiskit_expressions.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_qiskit_expressions.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/conversions/_symengine_expressions.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/conversions/_symengine_expressions.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/noise/basic.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/noise/basic.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/runner/_ibmq_runner.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/runner/_ibmq_runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     project: str = "main",
     noise_model: Optional[NoiseModel] = None,
     basis_gates: Optional[List[str]] = None,
     optimization_level: int = 0,
     seed: Optional[int] = None,
     retry_delay_seconds: int = 60,
     retry_timeout_seconds: int = 24 * 60 * 60,  # default timeout of one day
+    discard_extra_measurements=False,
 ):
     try:
         IBMQ.enable_account(api_token)
     except IBMQAccountError as e:
         if (
             e.message
             != "An IBM Quantum Experience account is already in use for the session."
@@ -57,8 +58,9 @@
         noise_model=noise_model,
         basis_gates=basis_gates,
         optimization_level=optimization_level,
         seed=seed,
         execute_function=_execute_on_ibmq_with_retries(
             retry_delay_seconds, retry_timeout_seconds
         ),
+        discard_extra_measurements=discard_extra_measurements,
     )
```

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/runner/_qiskit_runner.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/runner/_qiskit_runner.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import List, Optional, Sequence, Union
 
 from orquestra.quantum.api import BaseCircuitRunner
 from orquestra.quantum.circuits import (
     Circuit,
-    combine_measurement_counts,
+    combine_bitstrings,
     expand_sample_sizes,
     split_into_batches,
 )
 from orquestra.quantum.measurements import Measurements
 from qiskit import ClassicalRegister, QuantumCircuit, execute
 from qiskit.providers import BackendV1, BackendV2
 from qiskit.transpiler import CouplingMap
@@ -34,14 +34,15 @@
         self,
         qiskit_backend: AnyQiskitBackend,
         noise_model: Optional[NoiseModel] = None,
         coupling_map: Optional[CouplingMap] = None,
         basis_gates: Optional[List[str]] = None,
         optimization_level: int = 0,
         seed: Optional[int] = None,
+        discard_extra_measurements: bool = False,
         execute_function=execute,
     ):
         super().__init__()
         self.backend = qiskit_backend
 
         self.seed = seed
         self.backend = qiskit_backend
@@ -52,14 +53,15 @@
             noise_model.basis_gates
             if basis_gates is None and noise_model is not None
             else basis_gates
         )
 
         self.coupling_map = coupling_map
         self._execute = execute_function
+        self.discard_extra_measurements = discard_extra_measurements
 
     def _run_and_measure(self, circuit: Circuit, n_samples: int) -> Measurements:
         return self._run_batch_and_measure([circuit], [n_samples])[0]
 
     def _run_batch_and_measure(
         self, batch: Sequence[Circuit], samples_per_circuit: Sequence[int]
     ):
@@ -86,26 +88,39 @@
                 shots=n_samples,
                 noise_model=self.noise_model,
                 coupling_map=self.coupling_map,
                 basis_gates=self.basis_gates,
                 optimization_level=self.optimization_level,
                 seed_simulator=self.seed,
                 seed_transpiler=self.seed,
+                memory=True,
             )
             for circuits, n_samples in batches
         ]
 
         # Qiskit runners return single dictionary with counts when there was
         # only one experiment. To simplify logic, we make sure to always have a
         # list of counts from a job.
-        all_counts = [
-            counts for job in jobs for counts in _listify(job.result().get_counts())
-        ]
 
-        combined_measurement_counts = [
-            Measurements.from_counts(
-                {key[::-1]: value for key, value in counts.items()}
-            )
-            for counts in combine_measurement_counts(all_counts, multiplicities)
+        # One can use job.result().get_counts() to get all counts, but
+        # job.result().get_memory() does require index of the experiment
+        # This is why the below list comprehension looks so clumsy.
+        all_bitstrings = [
+            job.result().get_memory(i)
+            for job in jobs
+            for i in range(len(job.result().results))
         ]
 
-        return combined_measurement_counts
+        combined_bitstrings = combine_bitstrings(all_bitstrings, multiplicities)
+
+        if self.discard_extra_measurements:
+            combined_bitstrings = [
+                bitstrings[:n_samples]
+                for bitstrings, n_samples in zip(
+                    combined_bitstrings, samples_per_circuit
+                )
+            ]
+
+        return [
+            Measurements([tuple(map(int, b[::-1])) for b in bitstrings])
+            for bitstrings in combined_bitstrings
+        ]
```

### Comparing `orquestra-qiskit-0.8.0/src/orquestra/integrations/qiskit/simulator/_qiskit_wavefunction_simulator.py` & `orquestra-qiskit-0.9.0/src/orquestra/integrations/qiskit/simulator/_qiskit_wavefunction_simulator.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/PKG-INFO` & `orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: orquestra-qiskit
-Version: 0.8.0
+Version: 0.9.0
 Summary: "Orquestra Qiskit package"
 Home-page: https://github.com/zapatacomputing/orquestra-qiskit
 Author: Zapata Computing Inc.
 Author-email: info@zapatacomputing.com,
 License: Apache Software License 2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `orquestra-qiskit-0.8.0/src/orquestra_qiskit.egg-info/SOURCES.txt` & `orquestra-qiskit-0.9.0/src/orquestra_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/Makefile` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/Makefile`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/README.rst` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/README.rst`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/coverage/action.yml` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/coverage/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/actions/publish-release/action.yml` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/actions/publish-release/action.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/bin/get_next_version.py` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/bin/get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/pyproject.toml` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/pyproject.toml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/sample_setup.py` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/sample_setup.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/setup_extras.py` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/setup_extras.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/tests/test_get_next_version.py` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/tests/test_get_next_version.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/coverage.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/publish_release.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/subtrees/z_quantum_actions/workflow-templates/style.yml` & `orquestra-qiskit-0.9.0/subtrees/z_quantum_actions/workflow-templates/style.yml`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/circuit_conversions_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/circuit_conversions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/pauli_conversions_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/pauli_conversions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/qiskit_expressions_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/qiskit_expressions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/conversions/symengine_expressions_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/conversions/symengine_expressions_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/noise/basic_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/noise/basic_test.py`

 * *Files identical despite different names*

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/_ibmq_runner_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/_ibmq_runner_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,7 +29,21 @@
     circuits = [
         Circuit([H(0), CNOT(0, 1)])
         for _ in range(max_native_batch_size + max_native_batch_size // 2)
     ]
 
     result = ibmq_runner.run_batch_and_measure(circuits, 1000)
     assert len(result) == len(circuits)
+
+
+def test_ibmq_runner_discards_extra_measurements_if_exact_num_measurements_is_true():
+    ibmq_runner = create_ibmq_runner(
+        api_token=os.getenv("ZAPATA_IBMQ_API_TOKEN"),
+        backend_name="ibmq_qasm_simulator",
+        retry_delay_seconds=1,
+        discard_extra_measurements=True,
+    )
+    circuits = [Circuit([H(0), CNOT(0, 1)])] * 3
+    n_samples = [5, 10, 15]
+    result = ibmq_runner.run_batch_and_measure(circuits, n_samples=n_samples)
+
+    assert [len(r.bitstrings) for r in result] == n_samples
```

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/_qiskit_runner_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/_qiskit_runner_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,16 +8,17 @@
     CIRCUIT_RUNNER_CONTRACTS,
     circuit_runner_gate_compatibility_contracts,
 )
 from orquestra.quantum.circuits import CNOT, Circuit, H, X
 from orquestra.quantum.estimation import estimate_expectation_values_by_averaging
 from orquestra.quantum.measurements import ExpectationValues
 from orquestra.quantum.operators import PauliTerm
-from qiskit import Aer, QiskitError, execute
+from qiskit import QiskitError, execute
 from qiskit.transpiler import CouplingMap
+from qiskit_aer import Aer
 
 from orquestra.integrations.qiskit.noise import get_qiskit_noise_model
 from orquestra.integrations.qiskit.runner import QiskitRunner
 
 
 def _test_id(val):
     return val.backend.name()
@@ -135,14 +136,34 @@
 def test_qiskit_runner_passes_coupling_map_to_execute_function():
     circuit = Circuit([X(0), CNOT(1, 2)])
 
     coupling_map = CouplingMap([(0, 2), (0, 1)])
     execute_func = Mock(wraps=execute)
 
     runner = QiskitRunner(
-        Aer.get_backend("statevector_simulator"),
+        Aer.get_backend("aer_simulator_statevector"),
         coupling_map=coupling_map,
         execute_function=execute_func,
     )
 
     runner.run_and_measure(circuit, n_samples=10)
     assert execute_func.call_args.kwargs["coupling_map"] == coupling_map
+
+
+@pytest.mark.parametrize(
+    "runner",
+    [
+        *[
+            QiskitRunner(Aer.get_backend(name), discard_extra_measurements=True)
+            for name in COMPATIBLE_BACKENDS
+        ]
+    ],
+    ids=_test_id,
+)
+def test_qiskit_runner_discards_extra_measurements_exact_num_measurements_is_true(
+    runner: QiskitRunner,
+):
+    circuits = [Circuit([X(0), CNOT(0, 1)])] * 3
+    n_samples = [5, 10, 15]
+    result = runner.run_batch_and_measure(circuits, n_samples=n_samples)
+
+    assert [len(r.bitstrings) for r in result] == n_samples
```

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/_qiskit_wavefunction_simulator_test.py` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/_qiskit_wavefunction_simulator_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 from orquestra.quantum.api.circuit_runner_contracts import CIRCUIT_RUNNER_CONTRACTS
 from orquestra.quantum.api.wavefunction_simulator_contracts import (
     simulator_contracts_for_tolerance,
     simulator_contracts_with_nontrivial_initial_state,
 )
 from orquestra.quantum.circuits import CNOT, Circuit, X
-from qiskit import Aer
+from qiskit_aer import Aer
 
 from orquestra.integrations.qiskit.simulator import QiskitWavefunctionSimulator
 
-STATEVECTOR_BACKENDS = ["aer_simulator_statevector", "statevector_simulator"]
+STATEVECTOR_BACKENDS = ["aer_simulator_statevector"]
 
 
 def _test_id(val):
     return val.backend.name()
 
 
 @pytest.fixture(params=STATEVECTOR_BACKENDS)
```

### Comparing `orquestra-qiskit-0.8.0/tests/orquestra/integrations/qiskit/runner/jobs_and_batches_with_different_qubits.pickle` & `orquestra-qiskit-0.9.0/tests/orquestra/integrations/qiskit/runner/jobs_and_batches_with_different_qubits.pickle`

 * *Files identical despite different names*

