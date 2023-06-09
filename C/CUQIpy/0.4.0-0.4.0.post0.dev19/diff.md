# Comparing `tmp/CUQIpy-0.4.0.tar.gz` & `tmp/CUQIpy-0.4.0.post0.dev19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CUQIpy-0.4.0.tar", last modified: Sat May 27 08:12:48 2023, max compression
+gzip compressed data, was "CUQIpy-0.4.0.post0.dev19.tar", last modified: Fri Jun  9 08:18:05 2023, max compression
```

## Comparing `CUQIpy-0.4.0.tar` & `CUQIpy-0.4.0.post0.dev19.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.543003 CUQIpy-0.4.0/CUQIpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-27 08:12:48.000000 CUQIpy-0.4.0/CUQIpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16376 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/cuqi/
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/cuqi/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.547003 CUQIpy-0.4.0/cuqi/array/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/array/_array.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.547003 CUQIpy-0.4.0/cuqi/data/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/_data.py
--rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/astronaut.npz
--rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/camera.npz
--rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/cat.npz
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/data/satellite.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.547003 CUQIpy-0.4.0/cuqi/density/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/density/_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_beta.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_cauchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_cmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_gmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_inverse_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_laplace.py
--rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_lmrf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_lognormal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_normal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_posterior.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/distribution/_uniform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/geometry/_geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/likelihood/
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/likelihood/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/likelihood/_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/model/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/model/_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/operator/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/operator/_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/pde/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/pde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10337 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/pde/_pde.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.551003 CUQIpy-0.4.0/cuqi/problem/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/problem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/problem/_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_conjugate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_conjugate_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_cwmh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_gibbs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_langevin_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_laplace_approximation.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_mh.py
--rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_pcn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_rto.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/sampler/_sampler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/samples/_samples.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/solver/_solver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/testproblem/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/testproblem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/testproblem/_testproblem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.555003 CUQIpy-0.4.0/cuqi/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/utilities/_get_python_variable_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/cuqi/utilities/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:12:48.559003 CUQIpy-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_abstract_distribution_density.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_bayesian_inversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    29794 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_joint_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    12386 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_pde.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_testproblem.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-27 08:12:39.000000 CUQIpy-0.4.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.920735 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 08:18:05.000000 CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10799 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16388 2023-06-09 08:18:05.952736 CUQIpy-0.4.0.post0.dev19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/cuqi/
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/cuqi/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.924735 CUQIpy-0.4.0.post0.dev19/cuqi/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3968 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/array/_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.928735 CUQIpy-0.4.0.post0.dev19/cuqi/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)   786696 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/astronaut.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   262408 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/camera.npz
+-rw-r--r--   0 runner    (1001) docker     (123)   406164 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/cat.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/data/satellite.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.928735 CUQIpy-0.4.0.post0.dev19/cuqi/density/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/density/_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_beta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cauchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10488 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15873 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32903 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10382 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_inverse_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15039 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_laplace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3061 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lmrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lognormal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_posterior.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39613 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/geometry/_geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24201 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/model/_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.932735 CUQIpy-0.4.0.post0.dev19/cuqi/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8856 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/operator/_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.936735 CUQIpy-0.4.0.post0.dev19/cuqi/pde/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/pde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12572 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/pde/_pde.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.936735 CUQIpy-0.4.0.post0.dev19/cuqi/problem/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/problem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28944 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/problem/_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7757 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_cwmh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_gibbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7860 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_langevin_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_laplace_approximation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_mh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8602 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_pcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6158 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_rto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/samples/_samples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19377 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/solver/_solver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.940735 CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52242 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/_testproblem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.944735 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_get_python_variable_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 08:18:05.956735 CUQIpy-0.4.0.post0.dev19/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 08:18:05.952736 CUQIpy-0.4.0.post0.dev19/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_abstract_distribution_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_bayesian_inversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29794 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14728 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10668 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_joint_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6163 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21330 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_pde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16757 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12418 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_testproblem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-09 08:17:43.000000 CUQIpy-0.4.0.post0.dev19/tests/test_utilities.py
```

### Comparing `CUQIpy-0.4.0/CUQIpy.egg-info/PKG-INFO` & `CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.4.0
+Version: 0.4.0.post0.dev19
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-0.4.0/CUQIpy.egg-info/SOURCES.txt` & `CUQIpy-0.4.0.post0.dev19/CUQIpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/LICENSE` & `CUQIpy-0.4.0.post0.dev19/LICENSE`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/PKG-INFO` & `CUQIpy-0.4.0.post0.dev19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CUQIpy
-Version: 0.4.0
+Version: 0.4.0.post0.dev19
 Summary: Computational Uncertainty Quantification for Inverse problems in Python
 Maintainer-email: "Nicolai A. B. Riis" <nabr@dtu.dk>, "Jakob S. Jørgensen" <jakj@dtu.dk>, "Amal M. Alghamdi" <amaal@dtu.dk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `CUQIpy-0.4.0/README.md` & `CUQIpy-0.4.0.post0.dev19/README.md`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/array/_array.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/array/_array.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/config.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/config.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/data/_data.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/data/_data.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/data/astronaut.npz` & `CUQIpy-0.4.0.post0.dev19/cuqi/data/astronaut.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/data/camera.npz` & `CUQIpy-0.4.0.post0.dev19/cuqi/data/camera.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/data/cat.npz` & `CUQIpy-0.4.0.post0.dev19/cuqi/data/cat.npz`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/data/satellite.mat` & `CUQIpy-0.4.0.post0.dev19/cuqi/data/satellite.mat`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/density/_density.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/density/_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/diagnostics.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/diagnostics.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/__init__.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_beta.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_beta.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_cauchy.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cauchy.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_cmrf.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_cmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_custom.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_custom.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_distribution.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_gamma.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_gaussian.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gaussian.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_gmrf.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_gmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_inverse_gamma.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_inverse_gamma.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_joint_distribution.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_laplace.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_laplace.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_lmrf.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lmrf.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_lognormal.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_lognormal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_normal.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_normal.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_posterior.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_posterior.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/distribution/_uniform.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/distribution/_uniform.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/geometry/__init__.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/geometry/_geometry.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/geometry/_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/likelihood/__init__.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/__init__.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/likelihood/_likelihood.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/likelihood/_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/model/_model.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/model/_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/operator/_operator.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/operator/_operator.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/pde/_pde.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/pde/_pde.py`

 * *Files 10% similar despite different names*

```diff
@@ -80,14 +80,16 @@
         if hasattr(self,"_grid_obs"):
             return self._grid_obs
         else:
             return None
 
     @grid_obs.setter
     def grid_obs(self,value):
+        if value is None:
+            value = self.grid_sol
         self._grids_equal = self._compare_grid(value,self.grid_sol)
         self._grid_obs = value
 
     @property
     def grids_equal(self):
         return self._grids_equal
 
@@ -182,33 +184,49 @@
     
     Parameters
     -----------   
     PDE_form : callable function
         Callable function with signature `PDE_form(parameter, t)` where `parameter` is the Bayesian parameter and `t` is the time at which the PDE form is evaluated. The function returns a tuple of (`differential_operator`, `source_term`, `initial_condition`) where `differential_operator` is the linear operator at time `t`, `source_term` is the source term at time `t`, and `initial_condition` is the initial condition. The types of `differential_operator` and `source_term` are determined by what the method :meth:`linalg_solve` accepts as linear operator and right-hand side, respectively. The type of `initial_condition` should be the same type as the solution returned by :meth:`linalg_solve`.
 
     time_steps : ndarray 
-        An array of the discretized times corresponding to the time steps that starts with the initial time and ends with the final time.
+        An array of the discretized times corresponding to the time steps that starts with the initial time and ends with the final time
+        
+    time_obs : array_like or str
+        If passed as an array_like, it is an array of the times at which the solution is observed. If passed as a string it can be set to `final` to observe at the final time step, or `all` to observe at all time steps. Default is `final`.
 
     method: str
         Time stepping method. Currently two options are available `forward_euler` and  `backward_euler`.
 
     kwargs: 
         See :class:`~cuqi.pde.LinearPDE` for the remaining keyword arguments 
  
     Example
     -----------  
     See demos/demo34_TimeDependentLinearPDE.py for 1D heat and 1D wave equations.
     """
 
-    def __init__(self, PDE_form, time_steps, method='forward_euler', **kwargs):
+    def __init__(self, PDE_form, time_steps, time_obs='final', method='forward_euler', **kwargs):
         super().__init__(PDE_form, **kwargs)
 
         self.time_steps = time_steps
         self.method = method
 
+        # Set time_obs
+        if time_obs is None:
+            raise ValueError("time_obs cannot be None")
+        elif isinstance(time_obs, str):
+            if time_obs.lower() == 'final':
+                time_obs = time_steps[-1:]
+            elif time_obs.lower() == 'all':
+                time_obs = time_steps
+            else:
+                raise ValueError("if time_obs is a string, it can only be set "
+                                 +"to `final` or `all`")
+        self._time_obs = time_obs
+
     @property
     def method(self):
         return self._method
 
     @method.setter
     def method(self, value):
         if value.lower() != 'forward_euler' and value.lower() != 'backward_euler':
@@ -222,41 +240,66 @@
 
     def assemble_step(self, t):
         """Assemble time step at time t"""
         self.diff_op, self.rhs, self.initial_condition = self.PDE_form(self._parameter, t)
 
     def solve(self):
         """Solve PDE by time-stepping"""
+        # initialize time-dependent solution
+        self.assemble_step(self.time_steps[0])
+        u = np.empty((len(self.initial_condition), len(self.time_steps)))
+        u[:, 0] = self.initial_condition
 
         if self.method == 'forward_euler':
             for idx, t in enumerate(self.time_steps[:-1]):
                 dt = self.time_steps[idx+1] - t
                 self.assemble_step(t)
-                if idx == 0:
-                    u = self.initial_condition
-                u = (dt*self.diff_op + np.eye(len(u)))@u + dt*self.rhs  # from u at time t, gives u at t+dt
+                u_pre = u[:, idx]
+                u[:, idx+1] = (dt*self.diff_op + np.eye(len(u_pre)))@u_pre + dt*self.rhs  # from u at time t, gives u at t+dt
             info = None
 
         if self.method == 'backward_euler':
             for idx, t in enumerate(self.time_steps[1:]):
                 dt = t - self.time_steps[idx]
                 self.assemble_step(t)
-                if idx == 0:
-                    u = self.initial_condition
-                A = np.eye(len(u)) - dt*self.diff_op
+                u_pre = u[:, idx]
+                A = np.eye(len(u_pre)) - dt*self.diff_op
                 # from u at time t-dt, gives u at t
-                u, info = self._solve_linear_system(
-                    A, u + dt*self.rhs, self._linalg_solve, self._linalg_solve_kwargs)
+                u[:, idx+1], info = self._solve_linear_system(
+                    A, u_pre + dt*self.rhs, self._linalg_solve, self._linalg_solve_kwargs)
 
         return u, info
 
     def observe(self, solution):
-            
-        if self.grids_equal:
-            solution_obs = solution
+
+        # If observation grid is the same as solution grid and observation time
+        # is the final time step then no need to interpolate
+        if self.grids_equal and np.all(self.time_steps[-1:] == self._time_obs):
+            solution_obs = solution[..., -1]
+
+        # Interpolate solution in time and space to the observation
+        # time and space
         else:
-            solution_obs = interp1d(self.grid_sol, solution, kind='quadratic')(self.grid_obs)
+            # Raise error if solution is 2D or 3D in space 
+            if len(solution.shape) > 2:
+                raise ValueError("Interpolation of solutions of 2D and 3D "+ 
+                                 "space dimensions based on the provided "+
+                                 "grid_obs and time_obs are not supported. "+
+                                 "You can, instead, pass a custom "+
+                                 "observation_map and pass grid_obs and "+
+                                 "time_obs as None.")
+            
+            # Interpolate solution in space and time to the observation
+            # time and space
+            solution_obs = scipy.interpolate.RectBivariateSpline(
+                self.grid_sol, self.time_steps, solution)(self.grid_obs,
+                                                          self._time_obs)
 
+        # Apply observation map
         if self.observation_map is not None:
             solution_obs = self.observation_map(solution_obs)
-            
-        return solution_obs
+        
+        # squeeze if only one time observation
+        if len(self._time_obs) == 1:
+            solution_obs = solution_obs.squeeze()
+
+        return solution_obs
```

### Comparing `CUQIpy-0.4.0/cuqi/problem/_problem.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/problem/_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_conjugate.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_conjugate_approx.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_conjugate_approx.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_cwmh.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_cwmh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_gibbs.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_gibbs.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_hmc.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_hmc.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_langevin_algorithm.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_langevin_algorithm.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_laplace_approximation.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_laplace_approximation.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_mh.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_mh.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_pcn.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_pcn.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_rto.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_rto.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/sampler/_sampler.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/sampler/_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/samples/_samples.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/samples/_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/solver/_solver.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/solver/_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/testproblem/_testproblem.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/testproblem/_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/utilities/_get_python_variable_name.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_get_python_variable_name.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/cuqi/utilities/_utilities.py` & `CUQIpy-0.4.0.post0.dev19/cuqi/utilities/_utilities.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/pyproject.toml` & `CUQIpy-0.4.0.post0.dev19/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_abstract_distribution_density.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_abstract_distribution_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_bayesian_inversion.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_bayesian_inversion.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_density.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_density.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_distribution.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_geometry.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_joint_distribution.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_joint_distribution.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_likelihood.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_model.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_pde.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_pde.py`

 * *Files 22% similar despite different names*

```diff
@@ -177,30 +177,43 @@
     observed_sol = CUQI_pde.observe(sol)
 
     expected_observed_sol =  scipy.linalg.solve(diff_operator, source(2))[5:]**2
 
     assert(np.all(np.isclose(observed_sol, expected_observed_sol)))
 
 
-@pytest.mark.parametrize("method, time_steps, parametrization, expected_sol",
-                         [('forward_euler', 'fixed', 'initial_condition', 'sol1'),
-                          ('backward_euler', 'fixed', 'initial_condition', 'sol2'),
-                             ('backward_euler', 'varying',
-                              'initial_condition', 'sol3'),
-                             ('backward_euler', 'fixed', 'source_term1', 'sol4'),
-                             ('backward_euler', 'fixed', 'source_term2', 'sol5')])
-def test_TimeDependentLinearPDE_heat1D(copy_reference, method, time_steps, parametrization, expected_sol):
+@pytest.mark.parametrize(
+    "method, time_steps, parametrization, expected_sol",
+    [('forward_euler', 'fixed', 'initial_condition', 'sol1'),
+     ('backward_euler', 'fixed', 'initial_condition', 'sol2'),
+     ('backward_euler', 'varying',
+      'initial_condition', 'sol3'),
+     ('backward_euler', 'fixed', 'source_term1', 'sol4'),
+     ('backward_euler', 'fixed', 'source_term2', 'sol5')])
+@pytest.mark.parametrize(
+    "grid_obs, time_obs, observation_map, expected_obs",
+    [(None, 'final', None, 'obs1'),
+     (None, 'final', lambda x: x**2, 'obs2'),
+     ('half_grid', 'FINAL', None, 'obs3'),
+     ('half_grid', 'every_5', None, 'obs4'),
+     (None, 'every_5', lambda x: x**2, 'obs5'),
+     (np.array([3, 4.9]), np.array([0.9, 1]), lambda x: x**2, 'obs6')])
+def test_TimeDependentLinearPDE_heat1D(copy_reference, method, time_steps,
+                                       parametrization, expected_sol,
+                                       grid_obs, time_obs, observation_map,
+                                       expected_obs):
     """ Compute the final time solution of a 1D heat equation and
         compare it with previously stored solution (for 5 different set up choices).
     """
     # 1. Time and space parameters
     dim = 200   # Number of solution nodes
     L = 5  # 1D domain length
     max_time = 1  # Final time
     dx = L/(dim+1)   # Space step size
+    grid_sol = np.linspace(dx, L-dx, dim)  # Solution grid
 
     if method == 'forward_euler':
         cfl = 5/11  # The cfl condition to have a stable solution
         max_iter = int(max_time/(cfl*dx**2))  # Number of time steps
     elif method == 'backward_euler':
         dt_approx = 0.006  # Approximate time step
         max_iter = int(max_time/dt_approx)  # Number of time steps
@@ -230,26 +243,86 @@
         def PDE_form(source_term, t): return (
             Dxx, source_term, np.ones(dim))
         if parametrization == 'source_term1':
             parameters = np.zeros(dim)
         elif parametrization == 'source_term2':
             parameters = np.ones(dim)
 
-    # 4. Create a PDE object
+    # 4. Set up the observation parameters
+    if grid_obs == 'half_grid':
+        grid_obs = grid_sol[int(dim/2):]
+
+    if time_obs == 'every_5':
+        time_obs = time_steps[::5]
+
+    # 5. Create a PDE object
     PDE = cuqi.pde.TimeDependentLinearPDE(
-        PDE_form, time_steps, method=method)
+        PDE_form, time_steps, method=method,
+        grid_sol=grid_sol,
+        grid_obs=grid_obs, time_obs=time_obs,
+        observation_map=observation_map)
 
-    # 5 Solve the PDE
+    # 6. Solve the PDE
     PDE.assemble(parameters)
     sol, info = PDE.solve()
 
-    # 6 Compare the obtained solution with previously stored solution
-    solution_file = copy_reference("data/Heat1D_5solutions.npz")
+    # 7. Compare the obtained solution with previously stored solution
+    solution_file = copy_reference("data/Heat1D_data/Heat1D_5solutions.npz")
     expected_sols = np.load(solution_file)
-    assert(np.allclose(sol, expected_sols[expected_sol]))
+    assert (np.allclose(sol[:, -1], expected_sols[expected_sol]))
+
+    # 8. Compute the observed solution and compare it with previously
+    # stored solution
+
+    # compute the observed solution using the PDE object
+    obs_sol = PDE.observe(sol)
+
+    # compute the expected observed solution (for comparison)
+    if isinstance(time_obs, str) and time_obs.lower() == 'final':
+        time_obs = time_steps[-1:]
+    if grid_obs is None:
+        grid_obs = grid_sol
+
+    idx_x = [True if x in grid_obs else False for x in grid_sol]
+    idx_t = [True if t in time_obs else False for t in time_steps]
+
+    if sum(idx_x) != len(grid_obs) or sum(idx_t) != len(time_obs):
+        expected_observed_sol = scipy.interpolate.RectBivariateSpline(
+            grid_sol, time_steps, sol)(grid_obs, time_obs
+                                       )
+    else:
+        expected_observed_sol = sol[idx_x, :][:, idx_t]
+
+    if observation_map is not None:
+        expected_observed_sol = observation_map(expected_observed_sol)
+
+    if len(PDE._time_obs) == 1:
+        expected_observed_sol = expected_observed_sol.squeeze()
+
+    # load expected observed solution (for comparison)
+    # Skip sol1 due to its large size (not stored in file to save space)
+    if expected_sol != 'sol1':
+        obs_sol_file = copy_reference("data/Heat1D_data/Heat1D_obs_sol_"
+                                      + expected_sol+"_"
+                                      + expected_obs+".npz")
+        expected_observed_sol_from_file = np.load(obs_sol_file)["obs_sol"]
+
+        if len(PDE._time_obs) == 1:
+            expected_observed_sol_from_file = \
+                expected_observed_sol_from_file.squeeze()
+
+    # Compare the observed solution with the two expected observed solution
+    # (computed and loaded from file)
+    assert (np.allclose(obs_sol, expected_observed_sol))
+
+    if expected_sol != 'sol1':
+        assert (np.allclose(obs_sol, expected_observed_sol_from_file))
+    else:
+        assert expected_sol == 'sol1'
+
 
 @pytest.mark.xfail(reason="Test fails due to difficult to compare values (1e-6 to 1e-42)")
 def test_TimeDependentLinearPDE_wave1D(copy_reference):
     """ Compute the final time solution of a 1D wave equation and
         compare it with previously stored solution.
     """
     # 1. Time and space parameters
```

### Comparing `CUQIpy-0.4.0/tests/test_problem.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_problem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_sampler.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_sampler.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_samples.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_samples.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_solver.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_testproblem.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_testproblem.py`

 * *Files identical despite different names*

### Comparing `CUQIpy-0.4.0/tests/test_utilities.py` & `CUQIpy-0.4.0.post0.dev19/tests/test_utilities.py`

 * *Files identical despite different names*

