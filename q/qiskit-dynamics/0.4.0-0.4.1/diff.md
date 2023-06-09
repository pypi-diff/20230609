# Comparing `tmp/qiskit-dynamics-0.4.0.tar.gz` & `tmp/qiskit-dynamics-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit-dynamics-0.4.0.tar", last modified: Tue Mar 14 18:17:30 2023, max compression
+gzip compressed data, was "qiskit-dynamics-0.4.1.tar", last modified: Fri Jun  9 21:53:00 2023, max compression
```

## Comparing `qiskit-dynamics-0.4.0.tar` & `qiskit-dynamics-0.4.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.807877 qiskit-dynamics-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-14 18:17:30.807877 qiskit-dynamics-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.799877 qiskit-dynamics-0.4.0/qiskit_dynamics/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.799877 qiskit-dynamics-0.4.0/qiskit_dynamics/array/
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/array/patch_qi.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/array/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py
--rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/regex_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    43697 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/dynamics_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/backend/dynamics_job.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/generator_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/hamiltonian_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/lindblad_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    62696 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/operator_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    26059 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/rotating_frame.py
--rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/models/rotating_wave_approximation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/array_polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/custom_binary_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    30495 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/dyson_magnus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/multiset_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/perturbation_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/perturbation_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/solve_lmde_perturbation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/pulse/
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/pulse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/pulse/pulse_to_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.803877 qiskit-dynamics-0.4.0/qiskit_dynamics/signals/
--rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/signals/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/signals/transfer_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.807877 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/diffrax_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/fixed_step_solvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/jax_odeint.py
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/lanczos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.807877 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/scipy_solve_ivp.py
--rw-r--r--   0 runner    (1001) docker     (123)    38811 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/solver_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/solver_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/solver_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/qiskit_dynamics/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-14 18:17:30.799877 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-03-14 18:17:30.000000 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-03-14 18:17:30.000000 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:17:30.000000 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-14 18:17:30.000000 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-14 18:17:30.000000 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-14 18:17:30.000000 qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-14 18:17:30.807877 qiskit-dynamics-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-03-14 18:17:23.000000 qiskit-dynamics-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.028999 qiskit-dynamics-0.4.1/qiskit_dynamics/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/array/
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/patch_qi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/array/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12497 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13994 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/regex_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9822 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44918 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_job.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11769 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21116 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/generator_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8531 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/hamiltonian_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29123 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/lindblad_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62696 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/operator_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26059 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12484 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_wave_approximation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/array_polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12155 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/custom_binary_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30869 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/dyson_magnus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/multiset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15298 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/solve_lmde_perturbation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15322 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/pulse_to_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.032999 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)     8818 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40271 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/signals/transfer_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/diffrax_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21554 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/fixed_step_solvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/jax_odeint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/lanczos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20128 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5368 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/scipy_solve_ivp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38811 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18579 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10587 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16654 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/qiskit_dynamics/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 21:53:00.028999 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-09 21:52:59.000000 qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 21:53:00.037000 qiskit-dynamics-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-09 21:52:51.000000 qiskit-dynamics-0.4.1/setup.py
```

### Comparing `qiskit-dynamics-0.4.0/LICENSE.txt` & `qiskit-dynamics-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/PKG-INFO` & `qiskit-dynamics-0.4.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: qiskit-dynamics
-Version: 0.4.0
+Version: 0.4.1
 Summary: Qiskit ODE solver
-Home-page: https://github.com/Qiskit/qiskit-dynamics
+Home-page: https://github.com/Qiskit-Extensions/qiskit-dynamics
 Author: Qiskit Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-dynamics/issues
-Project-URL: Source Code, https://github.com/Qiskit/qiskit-dynamics
-Project-URL: Documentation, https://qiskit.org/documentation/dynamics
+Project-URL: Bug Tracker, https://github.com/Qiskit-Extensions/qiskit-dynamics/issues
+Project-URL: Source Code, https://github.com/Qiskit-Extensions/qiskit-dynamics
+Project-URL: Documentation, https://qiskit.org/ecosystem/dynamics/
 Description: # Qiskit Dynamics
         
         [![License](https://img.shields.io/github/license/Qiskit/qiskit-dynamics.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
         
         **This repo is still in the early stages of development, there will be breaking API changes**
         
-        Qiskit Dynamics is an open-source project for building, transforming, and solving
-        time-dependent quantum systems in Qiskit.
+        Qiskit Dynamics is an open-source project for building, transforming, and solving time-dependent
+        quantum systems in Qiskit.
         
-        The goal of Qiskit Dynamics is to provide access to different numerical
-        methods for solving differential equations, and to automate common processes typically performed by hand,
-        e.g. applying frame transformations or rotating wave approximations to system and control Hamiltonians.
-        
-        Qiskit Dynamics can be configured to use either
-        [NumPy](https://github.com/numpy/numpy) or [JAX](https://github.com/google/jax)
-        as the backend for array operations. [NumPy](https://github.com/numpy/numpy) is the default,
-        and [JAX](https://github.com/google/jax) is an optional dependency.
-        [JAX](https://github.com/google/jax) provides just-in-time compilation, automatic differentiation,
-        and GPU execution, and therefore is well-suited to tasks involving repeated
-        evaluation of functions with different parameters; E.g. simulating a model of a quantum system
-        over a range of parameter values, or optimizing the parameters of control sequence.
-        
-        Reference documentation may be found [here](https://qiskit.org/documentation/dynamics/),
-        including [tutorials](https://qiskit.org/documentation/dynamics/tutorials),
-        [user guide](https://qiskit.org/documentation/dynamics/userguide),
-        and [API reference](https://qiskit.org/documentation/dynamics/apidocs).
+        The goal of Qiskit Dynamics is to provide access to different numerical methods for solving
+        differential equations, and to automate common processes typically performed by hand, e.g. applying
+        frame transformations or rotating wave approximations to system and control Hamiltonians.
+        
+        Qiskit Dynamics can be configured to use either [NumPy](https://github.com/numpy/numpy) or
+        [JAX](https://github.com/google/jax) as the backend for array operations.
+        [NumPy](https://github.com/numpy/numpy) is the default, and [JAX](https://github.com/google/jax) is
+        an optional dependency. [JAX](https://github.com/google/jax) provides just-in-time compilation,
+        automatic differentiation, and GPU execution, and therefore is well-suited to tasks involving
+        repeated evaluation of functions with different parameters; E.g. simulating a model of a quantum
+        system over a range of parameter values, or optimizing the parameters of control sequence.
+        
+        Reference documentation may be found [here](https://qiskit.org/ecosystem/dynamics/), including
+        [tutorials](https://qiskit.org/ecosystem/dynamics/tutorials/index.html),
+        [user guide](https://qiskit.org/ecosystem/dynamics/userguide/index.html),
+        [API reference](https://qiskit.org/ecosystem/dynamics/apidocs/index.html), and
+        [Discussions](https://qiskit.org/ecosystem/dynamics/discussions/index.html).
         
         ## Installation
         
         Qiskit Dynamics may be installed using pip via:
         
         ```
         pip install qiskit-dynamics
@@ -53,33 +53,30 @@
         
         Installing JAX with GPU support must be done manually, for instructions refer to the
         [JAX installation guide](https://github.com/google/jax#installation).
         
         
         ## Contribution Guidelines
         
-        If you'd like to contribute to Qiskit Dynamics, please take a look at our
-        [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's
-        [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
-        uphold this code.
-        
-        We use [GitHub issues](https://github.com/Qiskit/qiskit-dynamics/issues) for
-        tracking requests and bugs. Please
-        [join the Qiskit Slack community](https://qisk.it/join-slack)
-        and use our [#qiskit-dynamics](https://qiskit.slack.com/archives/C03E7UVCDEV) channel for discussion and
-        simple questions.
-        For questions that are more suited for a forum we use the Qiskit tag in the
+        If you'd like to contribute to Qiskit Dynamics, please take a look at our 
+        [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's 
+        [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
+        
+        We use [GitHub issues](https://github.com/Qiskit-Extensions/qiskit-dynamics/issues) for tracking
+        requests and bugs. Please [join the Qiskit Slack community](https://qisk.it/join-slack) and use our
+        [#qiskit-dynamics](https://qiskit.slack.com/archives/C03E7UVCDEV) channel for discussion and simple
+        questions. For questions that are more suited for a forum we use the Qiskit tag in the 
         [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
         
         ## Authors and Citation
         
-        Qiskit Dynamics is the work of
-        [many people](https://github.com/Qiskit/qiskit-dynamics/graphs/contributors) who contribute
-        to the project at different levels. If you use Qiskit, please cite as per the included
-        [BibTeX file](https://github.com/Qiskit/qiskit-dynamics/blob/main/CITATION.bib).
+        Qiskit Dynamics is the work of 
+        [many people](https://github.com/Qiskit-Extensions/qiskit-dynamics/graphs/contributors) who
+        contribute to the project at different levels. If you use Qiskit, please cite as per the included 
+        [BibTeX file](https://github.com/Qiskit-Extensions/qiskit-dynamics/blob/main/CITATION.bib).
         
         ## License
         
         [Apache License 2.0](LICENSE.txt)
         
 Keywords: qiskit sdk quantum
 Platform: UNKNOWN
```

### Comparing `qiskit-dynamics-0.4.0/README.md` & `qiskit-dynamics-0.4.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # Qiskit Dynamics
 
 [![License](https://img.shields.io/github/license/Qiskit/qiskit-dynamics.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
 
 **This repo is still in the early stages of development, there will be breaking API changes**
 
-Qiskit Dynamics is an open-source project for building, transforming, and solving
-time-dependent quantum systems in Qiskit.
+Qiskit Dynamics is an open-source project for building, transforming, and solving time-dependent
+quantum systems in Qiskit.
 
-The goal of Qiskit Dynamics is to provide access to different numerical
-methods for solving differential equations, and to automate common processes typically performed by hand,
-e.g. applying frame transformations or rotating wave approximations to system and control Hamiltonians.
-
-Qiskit Dynamics can be configured to use either
-[NumPy](https://github.com/numpy/numpy) or [JAX](https://github.com/google/jax)
-as the backend for array operations. [NumPy](https://github.com/numpy/numpy) is the default,
-and [JAX](https://github.com/google/jax) is an optional dependency.
-[JAX](https://github.com/google/jax) provides just-in-time compilation, automatic differentiation,
-and GPU execution, and therefore is well-suited to tasks involving repeated
-evaluation of functions with different parameters; E.g. simulating a model of a quantum system
-over a range of parameter values, or optimizing the parameters of control sequence.
-
-Reference documentation may be found [here](https://qiskit.org/documentation/dynamics/),
-including [tutorials](https://qiskit.org/documentation/dynamics/tutorials),
-[user guide](https://qiskit.org/documentation/dynamics/userguide),
-and [API reference](https://qiskit.org/documentation/dynamics/apidocs).
+The goal of Qiskit Dynamics is to provide access to different numerical methods for solving
+differential equations, and to automate common processes typically performed by hand, e.g. applying
+frame transformations or rotating wave approximations to system and control Hamiltonians.
+
+Qiskit Dynamics can be configured to use either [NumPy](https://github.com/numpy/numpy) or
+[JAX](https://github.com/google/jax) as the backend for array operations.
+[NumPy](https://github.com/numpy/numpy) is the default, and [JAX](https://github.com/google/jax) is
+an optional dependency. [JAX](https://github.com/google/jax) provides just-in-time compilation,
+automatic differentiation, and GPU execution, and therefore is well-suited to tasks involving
+repeated evaluation of functions with different parameters; E.g. simulating a model of a quantum
+system over a range of parameter values, or optimizing the parameters of control sequence.
+
+Reference documentation may be found [here](https://qiskit.org/ecosystem/dynamics/), including
+[tutorials](https://qiskit.org/ecosystem/dynamics/tutorials/index.html),
+[user guide](https://qiskit.org/ecosystem/dynamics/userguide/index.html),
+[API reference](https://qiskit.org/ecosystem/dynamics/apidocs/index.html), and
+[Discussions](https://qiskit.org/ecosystem/dynamics/discussions/index.html).
 
 ## Installation
 
 Qiskit Dynamics may be installed using pip via:
 
 ```
 pip install qiskit-dynamics
@@ -42,30 +42,27 @@
 
 Installing JAX with GPU support must be done manually, for instructions refer to the
 [JAX installation guide](https://github.com/google/jax#installation).
 
 
 ## Contribution Guidelines
 
-If you'd like to contribute to Qiskit Dynamics, please take a look at our
-[contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's
-[code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
-uphold this code.
-
-We use [GitHub issues](https://github.com/Qiskit/qiskit-dynamics/issues) for
-tracking requests and bugs. Please
-[join the Qiskit Slack community](https://qisk.it/join-slack)
-and use our [#qiskit-dynamics](https://qiskit.slack.com/archives/C03E7UVCDEV) channel for discussion and
-simple questions.
-For questions that are more suited for a forum we use the Qiskit tag in the
+If you'd like to contribute to Qiskit Dynamics, please take a look at our 
+[contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's 
+[code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
+
+We use [GitHub issues](https://github.com/Qiskit-Extensions/qiskit-dynamics/issues) for tracking
+requests and bugs. Please [join the Qiskit Slack community](https://qisk.it/join-slack) and use our
+[#qiskit-dynamics](https://qiskit.slack.com/archives/C03E7UVCDEV) channel for discussion and simple
+questions. For questions that are more suited for a forum we use the Qiskit tag in the 
 [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
 
 ## Authors and Citation
 
-Qiskit Dynamics is the work of
-[many people](https://github.com/Qiskit/qiskit-dynamics/graphs/contributors) who contribute
-to the project at different levels. If you use Qiskit, please cite as per the included
-[BibTeX file](https://github.com/Qiskit/qiskit-dynamics/blob/main/CITATION.bib).
+Qiskit Dynamics is the work of 
+[many people](https://github.com/Qiskit-Extensions/qiskit-dynamics/graphs/contributors) who
+contribute to the project at different levels. If you use Qiskit, please cite as per the included 
+[BibTeX file](https://github.com/Qiskit-Extensions/qiskit-dynamics/blob/main/CITATION.bib).
 
 ## License
 
 [Apache License 2.0](LICENSE.txt)
```

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/array/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/array/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/array/array.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/array/array.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/array/patch_qi.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/array/patch_qi.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/array/wrap.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/array/wrap.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/hamiltonian_string_parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/operator_from_string.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_string_parser/regex_parser.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_string_parser/regex_parser.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/backend_utils.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/backend_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/dynamics_backend.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -199,25 +199,26 @@
         if target is None:
             target = Target()
         else:
             target = copy.copy(target)
 
         # add default simulator measure instructions
         measure_properties = {}
+        instruction_schedule_map = target.instruction_schedule_map()
         for qubit in self.options.subsystem_labels:
-            instruction_schedule_map = target.instruction_schedule_map()
             if not instruction_schedule_map.has(instruction="measure", qubits=qubit):
                 with pulse.build() as meas_sched:
                     pulse.acquire(
                         duration=1, qubit_or_channel=qubit, register=pulse.MemorySlot(qubit)
                     )
 
-            measure_properties[(qubit,)] = InstructionProperties(calibration=meas_sched)
+                measure_properties[(qubit,)] = InstructionProperties(calibration=meas_sched)
 
-        target.add_instruction(Measure(), measure_properties)
+        if bool(measure_properties):
+            target.add_instruction(Measure(), measure_properties)
 
         target.dt = solver._dt
 
         self._target = target
 
     def _default_options(self):
         return Options(
@@ -678,14 +679,39 @@
         channel_freqs = _get_backend_channel_freqs(
             backend_target=backend_target,
             backend_config=backend_config,
             backend_defaults=backend_defaults,
             channels=hamiltonian_channels,
         )
 
+        # Add control_channel_map from backend (only if not specified before by user)
+        if "control_channel_map" not in options:
+            if hasattr(backend, "control_channels"):
+                control_channel_map_backend = {
+                    qubits: backend.control_channels[qubits][0].index
+                    for qubits in backend.control_channels
+                }
+
+            elif hasattr(backend.configuration(), "control_channels"):
+                control_channel_map_backend = {
+                    qubits: backend.configuration().control_channels[qubits][0].index
+                    for qubits in backend.configuration().control_channels
+                }
+
+            else:
+                control_channel_map_backend = {}
+
+            # Reduce control_channel_map based on which channels are in the model
+            if bool(control_channel_map_backend):
+                control_channel_map = {}
+                for label, idx in control_channel_map_backend.items():
+                    if f"u{idx}" in hamiltonian_channels:
+                        control_channel_map[label] = idx
+                options["control_channel_map"] = control_channel_map
+
         # build the solver
         if rotating_frame == "auto":
             if "dense" in evaluation_mode:
                 rotating_frame = static_hamiltonian
             else:
                 rotating_frame = np.diag(static_hamiltonian)
 
@@ -863,15 +889,15 @@
 
 
 def _get_acquire_instruction_timings(
     schedules: List[Schedule], valid_subsystem_labels: List[int], dt: float
 ) -> Tuple[List[List[float]], List[List[int]], List[List[int]]]:
     """Get the required data from the acquire commands in each schedule.
 
-    Additionally validates that each schedule has acquire instructions occurring at one time, at
+    Additionally validates that each schedule has Acquire instructions occurring at one time, at
     least one memory slot is being listed, and all measured subsystems exist in
     ``valid_subsystem_labels``.
 
     Args:
         schedules: A list of schedules.
         valid_subsystem_labels: Valid acquire channel indices.
         dt: The sample size.
```

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/backend/dynamics_job.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/backend/dynamics_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/jax.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/jax.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/backends/numpy.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/backends/numpy.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/dispatch.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/dispatch.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/dispatch/exceptions.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/dispatch/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/generator_model.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/generator_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/hamiltonian_model.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/hamiltonian_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/lindblad_model.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/lindblad_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/operator_collections.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/operator_collections.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/rotating_frame.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_frame.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/models/rotating_wave_approximation.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/models/rotating_wave_approximation.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/array_polynomial.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/array_polynomial.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/custom_binary_op.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/custom_binary_op.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/dyson_magnus.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/dyson_magnus.py`

 * *Files 2% similar despite different names*

```diff
@@ -800,21 +800,21 @@
 
     return q_terms
 
 
 def _get_dyson_lmult_rule(
     complete_index_multisets: List[Multiset], perturbation_labels: Optional[List[Multiset]] = None
 ) -> List:
-    """Given a complete list of index multisets, return
-    the lmult rule in the format required for ``CustomProduct``.
-    Note, the generator :math:`G(t)` is encoded as index ``-1``, as
-    it will be prepended to the list of A matrices.
+    """Given a complete list of index multisets, return the lmult rule in the format required for
+    ``CustomProduct``. Note, the generator :math:`G(t)` is encoded as index ``-1``, as it will be
+    prepended to the list of A matrices. Similarly the index of the solution to the LMDE with
+    generator :math:`G(t)` is encoded as ``-1``.
 
-    While not required within the logic of this function, the input
-    should be canonically ordered according to ``_get_all_submultisets``.
+    While not required within the logic of this function, the input should be canonically ordered
+    according to ``_get_all_submultisets``.
 
     Args:
         complete_index_multisets: List of complete multisets.
         perturbation_labels: List of index multisets describing perturbations.
 
     Returns:
         List: Left multiplication rule description.
@@ -830,16 +830,23 @@
             else:
                 break
 
     # construct multiplication rules
     lmult_rule = [(np.array([1.0]), np.array([[-1, -1]]))]
 
     for term_idx, term in enumerate(complete_index_multisets):
-        if len(term) == 1:
-            lmult_rule.append((np.array([1.0, 1.0]), np.array([[-1, term_idx], [term_idx, -1]])))
+        if len(term) == 1 and term in perturbation_labels:
+            # if term not in perturbation_labels for len(term) == 1 the corresponding Dyson integral
+            # will always be 0
+            lmult_rule.append(
+                (
+                    np.array([1.0, 1.0]),
+                    np.array([[-1, term_idx], [perturbation_labels.index(term), -1]]),
+                )
+            )
         else:
             # self multiplied by base generator
             lmult_indices = [[-1, term_idx]]
 
             for l_idx, l_term in enumerate(perturbation_labels):
                 if l_term <= term:
                     if len(l_term) == len(term):
```

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/multiset_utils.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/multiset_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # that they have been altered from the originals.
 # pylint: disable=invalid-name
 
 """
 Utility functions for working with multisets.
 """
 
-from typing import List, Optional, Tuple
+from typing import List, Optional, Tuple, Iterable
 import itertools
 
 from multiset import Multiset
 
 from qiskit import QiskitError
 
 
@@ -42,23 +42,59 @@
     sorted_list = []
     for elem in distinct_elems:
         sorted_list = sorted_list + [elem] * multiset[elem]
 
     return sorted_list
 
 
-def _sorted_multisets(multisets: List[Multiset]) -> List[Multiset]:
-    """Sort in non-decreasing order according to:
-
-    ms1 <= ms2 if len(ms1) < len(ms2), or if
-    len(ms1) == len(ms2) and if
-    str(_multiset_to_sorted_list(ms1)) <= str(_multiset_to_sorted_list(ms2)).
+class _MultisetSortKey:
+    """Dummy class for usage as a key when sorting Multiset instances. This assumes the elements
+    of the multisets can themselves be sorted.
     """
 
-    return sorted(multisets, key=lambda x: str(len(x)) + ", " + str(_multiset_to_sorted_list(x)))
+    __slots__ = ("multiset",)
+
+    def __init__(self, multiset: Multiset):
+        self.multiset = multiset
+
+    def __lt__(self, other: Multiset) -> bool:
+        """Implements an ordering on multisets.
+
+        This orders first according to length (the number of elements in each multiset). If ``self``
+        and ``other`` are the same length, ``self < other`` if, when written as fully expanded and
+        sorted lists, ``self < other`` in lexicographic ordering. E.g. it holds that ``Multiset({0:
+        2, 1: 1}) < Multiset({0: 1, 1: 2})``, as the list versions are ``x = [0, 0, 1]``, and ``y =
+        [0, 1, 1]``. Here ``x[0] == y[0]``, but ``x[1] < y[1]``, and hence ``x < y`` in this
+        ordering.
+        """
+        if len(self.multiset) < len(other.multiset):
+            return True
+
+        if len(other.multiset) < len(self.multiset):
+            return False
+
+        unique_entries = set(self.multiset.distinct_elements())
+        unique_entries.update(other.multiset.distinct_elements())
+        unique_entries = sorted(unique_entries)
+
+        for element in unique_entries:
+            self_count = self.multiset[element]
+            other_count = other.multiset[element]
+
+            if self_count != other_count:
+                return self_count > other_count
+
+        return False
+
+
+def _sorted_multisets(multisets: Iterable[Multiset]) -> List[Multiset]:
+    """Sort in non-decreasing order according to the ordering described in the dummy class
+    _MultisetSort.
+    """
+    return sorted(multisets, key=_MultisetSortKey)
 
 
 def _clean_multisets(multisets: List[Multiset]) -> List[Multiset]:
     """Given a list of multisets, remove duplicates, and sort in non-decreasing order
     according to the _sorted_multisets function.
     """
```

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/perturbation_data.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_data.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/perturbation_utils.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/perturbation_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/perturbation/solve_lmde_perturbation.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/perturbation/solve_lmde_perturbation.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/pulse/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/pulse/pulse_to_signals.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/pulse/pulse_to_signals.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/signals/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/signals/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/signals/signals.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/signals/signals.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/signals/transfer_functions.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/signals/transfer_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/diffrax_solver.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/diffrax_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/fixed_step_solvers.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/fixed_step_solvers.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/jax_odeint.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/jax_odeint.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/lanczos.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/lanczos.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/__init__.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/dyson_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/expansion_model.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/magnus_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/perturbative_solvers/perturbative_solver.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/scipy_solve_ivp.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/scipy_solve_ivp.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/solver_classes.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_classes.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/solver_functions.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_functions.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/solvers/solver_utils.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/solvers/solver_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/type_utils.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/type_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics/version.py` & `qiskit-dynamics-0.4.1/qiskit_dynamics/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/PKG-INFO` & `qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 Metadata-Version: 2.1
 Name: qiskit-dynamics
-Version: 0.4.0
+Version: 0.4.1
 Summary: Qiskit ODE solver
-Home-page: https://github.com/Qiskit/qiskit-dynamics
+Home-page: https://github.com/Qiskit-Extensions/qiskit-dynamics
 Author: Qiskit Development Team
 Author-email: qiskit@qiskit.org
 License: Apache 2.0
-Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-dynamics/issues
-Project-URL: Source Code, https://github.com/Qiskit/qiskit-dynamics
-Project-URL: Documentation, https://qiskit.org/documentation/dynamics
+Project-URL: Bug Tracker, https://github.com/Qiskit-Extensions/qiskit-dynamics/issues
+Project-URL: Source Code, https://github.com/Qiskit-Extensions/qiskit-dynamics
+Project-URL: Documentation, https://qiskit.org/ecosystem/dynamics/
 Description: # Qiskit Dynamics
         
         [![License](https://img.shields.io/github/license/Qiskit/qiskit-dynamics.svg?style=popout-square)](https://opensource.org/licenses/Apache-2.0)
         
         **This repo is still in the early stages of development, there will be breaking API changes**
         
-        Qiskit Dynamics is an open-source project for building, transforming, and solving
-        time-dependent quantum systems in Qiskit.
+        Qiskit Dynamics is an open-source project for building, transforming, and solving time-dependent
+        quantum systems in Qiskit.
         
-        The goal of Qiskit Dynamics is to provide access to different numerical
-        methods for solving differential equations, and to automate common processes typically performed by hand,
-        e.g. applying frame transformations or rotating wave approximations to system and control Hamiltonians.
-        
-        Qiskit Dynamics can be configured to use either
-        [NumPy](https://github.com/numpy/numpy) or [JAX](https://github.com/google/jax)
-        as the backend for array operations. [NumPy](https://github.com/numpy/numpy) is the default,
-        and [JAX](https://github.com/google/jax) is an optional dependency.
-        [JAX](https://github.com/google/jax) provides just-in-time compilation, automatic differentiation,
-        and GPU execution, and therefore is well-suited to tasks involving repeated
-        evaluation of functions with different parameters; E.g. simulating a model of a quantum system
-        over a range of parameter values, or optimizing the parameters of control sequence.
-        
-        Reference documentation may be found [here](https://qiskit.org/documentation/dynamics/),
-        including [tutorials](https://qiskit.org/documentation/dynamics/tutorials),
-        [user guide](https://qiskit.org/documentation/dynamics/userguide),
-        and [API reference](https://qiskit.org/documentation/dynamics/apidocs).
+        The goal of Qiskit Dynamics is to provide access to different numerical methods for solving
+        differential equations, and to automate common processes typically performed by hand, e.g. applying
+        frame transformations or rotating wave approximations to system and control Hamiltonians.
+        
+        Qiskit Dynamics can be configured to use either [NumPy](https://github.com/numpy/numpy) or
+        [JAX](https://github.com/google/jax) as the backend for array operations.
+        [NumPy](https://github.com/numpy/numpy) is the default, and [JAX](https://github.com/google/jax) is
+        an optional dependency. [JAX](https://github.com/google/jax) provides just-in-time compilation,
+        automatic differentiation, and GPU execution, and therefore is well-suited to tasks involving
+        repeated evaluation of functions with different parameters; E.g. simulating a model of a quantum
+        system over a range of parameter values, or optimizing the parameters of control sequence.
+        
+        Reference documentation may be found [here](https://qiskit.org/ecosystem/dynamics/), including
+        [tutorials](https://qiskit.org/ecosystem/dynamics/tutorials/index.html),
+        [user guide](https://qiskit.org/ecosystem/dynamics/userguide/index.html),
+        [API reference](https://qiskit.org/ecosystem/dynamics/apidocs/index.html), and
+        [Discussions](https://qiskit.org/ecosystem/dynamics/discussions/index.html).
         
         ## Installation
         
         Qiskit Dynamics may be installed using pip via:
         
         ```
         pip install qiskit-dynamics
@@ -53,33 +53,30 @@
         
         Installing JAX with GPU support must be done manually, for instructions refer to the
         [JAX installation guide](https://github.com/google/jax#installation).
         
         
         ## Contribution Guidelines
         
-        If you'd like to contribute to Qiskit Dynamics, please take a look at our
-        [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's
-        [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to
-        uphold this code.
-        
-        We use [GitHub issues](https://github.com/Qiskit/qiskit-dynamics/issues) for
-        tracking requests and bugs. Please
-        [join the Qiskit Slack community](https://qisk.it/join-slack)
-        and use our [#qiskit-dynamics](https://qiskit.slack.com/archives/C03E7UVCDEV) channel for discussion and
-        simple questions.
-        For questions that are more suited for a forum we use the Qiskit tag in the
+        If you'd like to contribute to Qiskit Dynamics, please take a look at our 
+        [contribution guidelines](CONTRIBUTING.md). This project adheres to Qiskit's 
+        [code of conduct](CODE_OF_CONDUCT.md). By participating, you are expected to uphold this code.
+        
+        We use [GitHub issues](https://github.com/Qiskit-Extensions/qiskit-dynamics/issues) for tracking
+        requests and bugs. Please [join the Qiskit Slack community](https://qisk.it/join-slack) and use our
+        [#qiskit-dynamics](https://qiskit.slack.com/archives/C03E7UVCDEV) channel for discussion and simple
+        questions. For questions that are more suited for a forum we use the Qiskit tag in the 
         [Stack Exchange](https://quantumcomputing.stackexchange.com/questions/tagged/qiskit).
         
         ## Authors and Citation
         
-        Qiskit Dynamics is the work of
-        [many people](https://github.com/Qiskit/qiskit-dynamics/graphs/contributors) who contribute
-        to the project at different levels. If you use Qiskit, please cite as per the included
-        [BibTeX file](https://github.com/Qiskit/qiskit-dynamics/blob/main/CITATION.bib).
+        Qiskit Dynamics is the work of 
+        [many people](https://github.com/Qiskit-Extensions/qiskit-dynamics/graphs/contributors) who
+        contribute to the project at different levels. If you use Qiskit, please cite as per the included 
+        [BibTeX file](https://github.com/Qiskit-Extensions/qiskit-dynamics/blob/main/CITATION.bib).
         
         ## License
         
         [Apache License 2.0](LICENSE.txt)
         
 Keywords: qiskit sdk quantum
 Platform: UNKNOWN
```

### Comparing `qiskit-dynamics-0.4.0/qiskit_dynamics.egg-info/SOURCES.txt` & `qiskit-dynamics-0.4.1/qiskit_dynamics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit-dynamics-0.4.0/setup.py` & `qiskit-dynamics-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,16 @@
     "numpy>=1.17",
     "scipy>=1.4",
     "matplotlib>=3.0",
     "qiskit-terra>=0.23.0",
     "multiset>=3.0.1",
 ]
 
-jax_extras = ['jax>=0.2.26',
-              'jaxlib>=0.1.75']
+jax_extras = ['jax>=0.2.26, <= 0.4.6',
+              'jaxlib>=0.1.75, <= 0.4.6']
 
 PACKAGES = setuptools.find_packages(exclude=['test*'])
 
 version_path = os.path.abspath(
     os.path.join(os.path.dirname(__file__), 'qiskit_dynamics',
                  'VERSION.txt'))
 
@@ -43,15 +43,15 @@
 setuptools.setup(
     name="qiskit-dynamics",
     version=version,
     packages=PACKAGES,
     description="Qiskit ODE solver",
     long_description=README,
     long_description_content_type='text/markdown',
-    url="https://github.com/Qiskit/qiskit-dynamics",
+    url="https://github.com/Qiskit-Extensions/qiskit-dynamics",
     author="Qiskit Development Team",
     author_email="qiskit@qiskit.org",
     license="Apache 2.0",
     classifiers=[
         "Environment :: Console",
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
@@ -64,17 +64,17 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Scientific/Engineering",
     ],
     keywords="qiskit sdk quantum",
     project_urls={
-        "Bug Tracker": "https://github.com/Qiskit/qiskit-dynamics/issues",
-        "Source Code": "https://github.com/Qiskit/qiskit-dynamics",
-        "Documentation": "https://qiskit.org/documentation/dynamics",
+        "Bug Tracker": "https://github.com/Qiskit-Extensions/qiskit-dynamics/issues",
+        "Source Code": "https://github.com/Qiskit-Extensions/qiskit-dynamics",
+        "Documentation": "https://qiskit.org/ecosystem/dynamics/",
     },
     install_requires=requirements,
     include_package_data=True,
     python_requires=">=3.8",
     extras_require={
         "jax": jax_extras
     },
```

