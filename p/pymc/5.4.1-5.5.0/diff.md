# Comparing `tmp/pymc-5.4.1.tar.gz` & `tmp/pymc-5.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pymc-5.4.1.tar", last modified: Tue May 30 09:46:27 2023, max compression
+gzip compressed data, was "dist/pymc-5.5.0.tar", last modified: Fri Jun  9 14:56:28 2023, max compression
```

## Comparing `pymc-5.4.1.tar` & `pymc-5.5.0.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-30 09:46:19.000000 pymc-5.4.1/ARCHITECTURE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-30 09:46:19.000000 pymc-5.4.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-30 09:46:19.000000 pymc-5.4.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-05-30 09:46:19.000000 pymc-5.4.1/GOVERNANCE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-05-30 09:46:19.000000 pymc-5.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 09:46:19.000000 pymc-5.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-30 09:46:27.000000 pymc-5.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-05-30 09:46:19.000000 pymc-5.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-05-30 09:46:19.000000 pymc-5.4.1/RELEASE-NOTES.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/arviz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/mcbackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/backends/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/blocking.py
--rw-r--r--   0 runner    (1001) docker     (123)    16749 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9882 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/censored.py
--rw-r--r--   0 runner    (1001) docker     (123)   116464 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/continuous.py
--rw-r--r--   0 runner    (1001) docker     (123)    42225 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/discrete.py
--rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/dist_math.py
--rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    36499 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    89379 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/multivariate.py
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/shape_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    39568 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/distributions/truncated.py
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/func_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/gp/
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/cov.py
--rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/gp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/hsgp_approx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/mean.py
--rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/gp/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/initial_point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/logprob/
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     9476 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/censoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/cumsum.py
--rw-r--r--   0 runner    (1001) docker     (123)    20564 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/mixture.py
--rw-r--r--   0 runner    (1001) docker     (123)    14922 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/rewriting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24280 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    36986 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    11559 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/logprob/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/math.py
--rw-r--r--   0 runner    (1001) docker     (123)    90135 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/model_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/ode/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/ode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/ode/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/ode/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/plots/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39312 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/pytensorf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/sampling/
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/forward.py
--rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/jax.py
--rw-r--r--   0 runner    (1001) docker     (123)    50490 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/mcmc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/sampling_jax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/smc/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/smc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/smc/kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/smc/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/stats/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/stats/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/stats/log_likelihood.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/step_methods/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/arraystep.py
--rw-r--r--   0 runner    (1001) docker     (123)    10623 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/step_methods/hmc/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/base_hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/hmc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/nuts.py
--rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/hmc/quadpotential.py
--rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/metropolis.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/step_methods/step_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)    36397 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/tuning/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/tuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/tuning/scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/tuning/starting.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc/variational/
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13163 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/approximations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/minibatch_rv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/opvi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/stein.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/variational/updates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-30 09:46:19.000000 pymc-5.4.1/pymc/vartypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-30 09:46:27.000000 pymc-5.4.1/pymc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-30 09:46:19.000000 pymc-5.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-30 09:46:19.000000 pymc-5.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 09:46:27.000000 pymc-5.4.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-05-30 09:46:19.000000 pymc-5.4.1/scripts/docker_container.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-05-30 09:46:19.000000 pymc-5.4.1/scripts/test.sh
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-30 09:46:27.000000 pymc-5.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-05-30 09:46:19.000000 pymc-5.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-05-30 09:46:19.000000 pymc-5.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-09 14:56:17.000000 pymc-5.5.0/ARCHITECTURE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-06-09 14:56:17.000000 pymc-5.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-06-09 14:56:17.000000 pymc-5.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    42347 2023-06-09 14:56:17.000000 pymc-5.5.0/GOVERNANCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12865 2023-06-09 14:56:17.000000 pymc-5.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-09 14:56:17.000000 pymc-5.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-09 14:56:28.000000 pymc-5.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8928 2023-06-09 14:56:17.000000 pymc-5.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    81106 2023-06-09 14:56:17.000000 pymc-5.5.0/RELEASE-NOTES.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     4522 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21386 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/arviz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19525 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/mcbackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8127 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/backends/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16569 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/censored.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116464 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42225 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15229 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/dist_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40140 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36243 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89110 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/multivariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/shape_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12579 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38767 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12769 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14747 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/distributions/truncated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7579 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/func_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/gp/
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32081 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/cov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49766 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14494 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/hsgp_approx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/mean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7734 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/gp/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/initial_point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/logprob/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8678 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/censoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/cumsum.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20392 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/mixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19901 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/rewriting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22586 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33914 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9828 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/logprob/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15013 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)    90171 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16575 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/model_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/ode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/ode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9657 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/ode/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4767 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/ode/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10014 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39241 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/pytensorf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29883 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25904 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/jax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51405 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/mcmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15599 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15011 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/sampling_jax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/smc/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/smc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24432 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/smc/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14868 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/smc/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/stats/convergence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/stats/log_likelihood.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/step_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/arraystep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/step_methods/hmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9044 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/base_hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/hmc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17591 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/nuts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27526 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/hmc/quadpotential.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35731 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/metropolis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/step_methods/step_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36022 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/tuning/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/tuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/tuning/scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9296 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/tuning/starting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc/variational/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/approximations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28608 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/minibatch_rv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57336 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/opvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/stein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37930 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/variational/updates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-06-09 14:56:17.000000 pymc-5.5.0/pymc/vartypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11308 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-09 14:56:28.000000 pymc-5.5.0/pymc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-09 14:56:17.000000 pymc-5.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-09 14:56:17.000000 pymc-5.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 14:56:28.000000 pymc-5.5.0/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      833 2023-06-09 14:56:17.000000 pymc-5.5.0/scripts/docker_container.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      181 2023-06-09 14:56:17.000000 pymc-5.5.0/scripts/test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-09 14:56:28.000000 pymc-5.5.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2698 2023-06-09 14:56:17.000000 pymc-5.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81282 2023-06-09 14:56:17.000000 pymc-5.5.0/versioneer.py
```

### Comparing `pymc-5.4.1/ARCHITECTURE.md` & `pymc-5.5.0/ARCHITECTURE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/CODE_OF_CONDUCT.md` & `pymc-5.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/CONTRIBUTING.md` & `pymc-5.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/GOVERNANCE.md` & `pymc-5.5.0/GOVERNANCE.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/LICENSE` & `pymc-5.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/PKG-INFO` & `pymc-5.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.4.1
+Version: 5.5.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.4.1/README.rst` & `pymc-5.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/RELEASE-NOTES.md` & `pymc-5.5.0/RELEASE-NOTES.md`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/__init__.py` & `pymc-5.5.0/pymc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/backends/__init__.py` & `pymc-5.5.0/pymc/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/backends/arviz.py` & `pymc-5.5.0/pymc/backends/arviz.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/backends/base.py` & `pymc-5.5.0/pymc/backends/base.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/backends/mcbackend.py` & `pymc-5.5.0/pymc/backends/mcbackend.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/backends/ndarray.py` & `pymc-5.5.0/pymc/backends/ndarray.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/backends/report.py` & `pymc-5.5.0/pymc/backends/report.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/blocking.py` & `pymc-5.5.0/pymc/blocking.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/data.py` & `pymc-5.5.0/pymc/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 from pytensor.tensor.random.basic import IntegersRV
 from pytensor.tensor.subtensor import AdvancedSubtensor
 from pytensor.tensor.type import TensorType
 from pytensor.tensor.var import TensorConstant, TensorVariable
 
 import pymc as pm
 
-from pymc.logprob.abstract import _get_measurable_outputs
 from pymc.pytensorf import convert_observed_data
 
 __all__ = [
     "get_data",
     "GeneratorAdapter",
     "Minibatch",
     "Data",
@@ -131,19 +130,14 @@
     # Work-around for https://github.com/pymc-devs/pytensor/issues/97
     def make_node(self, rng, *args, **kwargs):
         if rng is None:
             rng = pytensor.shared(np.random.default_rng())
         return super().make_node(rng, *args, **kwargs)
 
 
-@_get_measurable_outputs.register(MinibatchIndexRV)
-def minibatch_index_rv_measuarable_outputs(op, node):
-    return []
-
-
 minibatch_index = MinibatchIndexRV()
 
 
 def is_minibatch(v: TensorVariable) -> bool:
     return (
         isinstance(v.owner.op, AdvancedSubtensor)
         and isinstance(v.owner.inputs[1].owner.op, MinibatchIndexRV)
```

### Comparing `pymc-5.4.1/pymc/distributions/__init__.py` & `pymc-5.5.0/pymc/distributions/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/bound.py` & `pymc-5.5.0/pymc/distributions/bound.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 from pymc.distributions.continuous import BoundedContinuous, bounded_cont_transform
 from pymc.distributions.dist_math import check_parameters
 from pymc.distributions.distribution import Continuous, Discrete
 from pymc.distributions.shape_utils import to_tuple
 from pymc.distributions.transforms import _default_transform
 from pymc.logprob.basic import logp
-from pymc.logprob.utils import ignore_logprob
 from pymc.model import modelcontext
 from pymc.pytensorf import floatX, intX
 from pymc.util import check_dist_not_registered
 
 __all__ = ["Bound"]
 
 
@@ -198,15 +197,14 @@
             if dims in model.coords:
                 dim_obj = np.asarray(model.coords[dims])
                 size = dim_obj.shape
             else:
                 raise ValueError("Given dims do not exist in model coordinates.")
 
         lower, upper, initval = cls._set_values(lower, upper, size, shape, initval)
-        dist = ignore_logprob(dist)
 
         if isinstance(dist.owner.op, Continuous):
             res = _ContinuousBounded(
                 name,
                 [dist, lower, upper],
                 initval=floatX(initval),
                 size=size,
@@ -232,15 +230,14 @@
         upper=None,
         size=None,
         shape=None,
         **kwargs,
     ):
         cls._argument_checks(dist, **kwargs)
         lower, upper, initval = cls._set_values(lower, upper, size, shape, initval=None)
-        dist = ignore_logprob(dist)
         if isinstance(dist.owner.op, Continuous):
             res = _ContinuousBounded.dist(
                 [dist, lower, upper],
                 size=size,
                 shape=shape,
                 **kwargs,
             )
```

### Comparing `pymc-5.4.1/pymc/distributions/censored.py` & `pymc-5.5.0/pymc/distributions/censored.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/continuous.py` & `pymc-5.5.0/pymc/distributions/continuous.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/discrete.py` & `pymc-5.5.0/pymc/distributions/discrete.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/dist_math.py` & `pymc-5.5.0/pymc/distributions/dist_math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/distribution.py` & `pymc-5.5.0/pymc/distributions/distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from pytensor.graph import node_rewriter
 from pytensor.graph.basic import Node, Variable
 from pytensor.graph.replace import clone_replace
 from pytensor.graph.rewriting.basic import in2out
 from pytensor.graph.utils import MetaType
 from pytensor.tensor.basic import as_tensor_variable
 from pytensor.tensor.random.op import RandomVariable
-from pytensor.tensor.random.type import RandomType
 from pytensor.tensor.random.utils import normalize_size_param
 from pytensor.tensor.var import TensorVariable
 from typing_extensions import TypeAlias
 
 from pymc.distributions.shape_utils import (
     Dims,
     Shape,
@@ -45,21 +44,15 @@
     convert_shape,
     convert_size,
     find_size,
     rv_size_is_none,
     shape_from_dims,
 )
 from pymc.exceptions import BlockModelAccessError
-from pymc.logprob.abstract import (
-    MeasurableVariable,
-    _get_measurable_outputs,
-    _icdf,
-    _logcdf,
-    _logprob,
-)
+from pymc.logprob.abstract import MeasurableVariable, _icdf, _logcdf, _logprob
 from pymc.logprob.rewriting import logprob_rewrites_db
 from pymc.model import BlockModelAccess
 from pymc.printing import str_for_dist
 from pymc.pytensorf import collect_default_updates, convert_observed_data, floatX
 from pymc.util import UNSET, _add_future_warning_tag
 from pymc.vartypes import continuous_types, string_types
 
@@ -397,28 +390,14 @@
         return rv_out
 
 
 # Let PyMC know that the SymbolicRandomVariable has a logprob.
 MeasurableVariable.register(SymbolicRandomVariable)
 
 
-@_get_measurable_outputs.register(SymbolicRandomVariable)
-def _get_measurable_outputs_symbolic_random_variable(op, node):
-    # This tells PyMC that any non RandomType outputs are measurable
-
-    # Assume that if there is one default_output, that's the only one that is measurable
-    # In the rare case this is not what one wants, a specialized _get_measuarable_outputs
-    # can dispatch for a subclassed Op
-    if op.default_output is not None:
-        return [node.default_output()]
-
-    # Otherwise assume that any outputs that are not of RandomType are measurable
-    return [out for out in node.outputs if not isinstance(out.type, RandomType)]
-
-
 @node_rewriter([SymbolicRandomVariable])
 def inline_symbolic_random_variable(fgraph, node):
     """
     Optimization that expands the internal graph of a SymbolicRV when obtaining the logp
     graph, if the flag `inline_logprob` is True.
     """
     op = node.op
```

### Comparing `pymc-5.4.1/pymc/distributions/mixture.py` & `pymc-5.5.0/pymc/distributions/mixture.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     SymbolicRandomVariable,
     _moment,
     moment,
 )
 from pymc.distributions.shape_utils import _change_dist_size, change_dist_size
 from pymc.distributions.transforms import _default_transform
 from pymc.distributions.truncated import Truncated
-from pymc.logprob.abstract import _logcdf, _logcdf_helper, _logprob, _logprob_helper
+from pymc.logprob.abstract import _logcdf, _logcdf_helper, _logprob
+from pymc.logprob.basic import logp
 from pymc.logprob.transforms import IntervalTransform
-from pymc.logprob.utils import ignore_logprob
 from pymc.pytensorf import floatX
 from pymc.util import check_dist_not_registered
 from pymc.vartypes import continuous_types, discrete_types
 
 __all__ = [
     "HurdleGamma",
     "HurdleLogNormal",
@@ -263,18 +263,14 @@
             ndim_batch = components[0].ndim - ndim_supp
             if single_component:
                 ndim_batch -= 1
             weights_ndim_batch = max(0, weights.ndim - ndim_batch - 1)
 
         assert weights_ndim_batch == 0
 
-        # Component RVs terms are accounted by the Mixture logprob, so they can be
-        # safely ignored in the logprob graph
-        components = [ignore_logprob(component) for component in components]
-
         # Create a OpFromGraph that encapsulates the random generating process
         # Create dummy input variables with the same type as the ones provided
         weights_ = weights.type()
         components_ = [component.type() for component in components]
         mix_indexes_rng_ = mix_indexes_rng.type()
 
         mix_axis = -ndim_supp - 1
@@ -346,18 +342,18 @@
 def marginal_mixture_logprob(op, values, rng, weights, *components, **kwargs):
     (value,) = values
 
     # single component
     if len(components) == 1:
         # Need to broadcast value across mixture axis
         mix_axis = -components[0].owner.op.ndim_supp - 1
-        components_logp = _logprob_helper(components[0], pt.expand_dims(value, mix_axis))
+        components_logp = logp(components[0], pt.expand_dims(value, mix_axis))
     else:
         components_logp = pt.stack(
-            [_logprob_helper(component, value) for component in components],
+            [logp(component, value) for component in components],
             axis=-1,
         )
 
     mix_logp = pt.logsumexp(pt.log(weights) + components_logp, axis=-1)
 
     mix_logp = check_parameters(
         mix_logp,
```

### Comparing `pymc-5.4.1/pymc/distributions/multivariate.py` & `pymc-5.5.0/pymc/distributions/multivariate.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,5456 +132,5439 @@
 00000830: 6f72 6d73 2069 6d70 6f72 7420 496e 7465  orms import Inte
 00000840: 7276 616c 2c20 5a65 726f 5375 6d54 7261  rval, ZeroSumTra
 00000850: 6e73 666f 726d 2c20 5f64 6566 6175 6c74  nsform, _default
 00000860: 5f74 7261 6e73 666f 726d 0a66 726f 6d20  _transform.from 
 00000870: 7079 6d63 2e6c 6f67 7072 6f62 2e61 6273  pymc.logprob.abs
 00000880: 7472 6163 7420 696d 706f 7274 205f 6c6f  tract import _lo
 00000890: 6770 726f 620a 6672 6f6d 2070 796d 632e  gprob.from pymc.
-000008a0: 6c6f 6770 726f 622e 7574 696c 7320 696d  logprob.utils im
-000008b0: 706f 7274 2069 676e 6f72 655f 6c6f 6770  port ignore_logp
-000008c0: 726f 620a 6672 6f6d 2070 796d 632e 6d61  rob.from pymc.ma
-000008d0: 7468 2069 6d70 6f72 7420 6b72 6f6e 5f64  th import kron_d
-000008e0: 6961 672c 206b 726f 6e5f 646f 740a 6672  iag, kron_dot.fr
-000008f0: 6f6d 2070 796d 632e 7079 7465 6e73 6f72  om pymc.pytensor
-00000900: 6620 696d 706f 7274 2066 6c6f 6174 582c  f import floatX,
-00000910: 2069 6e74 580a 6672 6f6d 2070 796d 632e   intX.from pymc.
-00000920: 7574 696c 2069 6d70 6f72 7420 6368 6563  util import chec
-00000930: 6b5f 6469 7374 5f6e 6f74 5f72 6567 6973  k_dist_not_regis
-00000940: 7465 7265 640a 0a5f 5f61 6c6c 5f5f 203d  tered..__all__ =
-00000950: 205b 0a20 2020 2022 4d76 4e6f 726d 616c   [.    "MvNormal
-00000960: 222c 0a20 2020 2022 5a65 726f 5375 6d4e  ",.    "ZeroSumN
-00000970: 6f72 6d61 6c22 2c0a 2020 2020 224d 7653  ormal",.    "MvS
-00000980: 7475 6465 6e74 5422 2c0a 2020 2020 2244  tudentT",.    "D
-00000990: 6972 6963 686c 6574 222c 0a20 2020 2022  irichlet",.    "
-000009a0: 4d75 6c74 696e 6f6d 6961 6c22 2c0a 2020  Multinomial",.  
-000009b0: 2020 2244 6972 6963 686c 6574 4d75 6c74    "DirichletMult
-000009c0: 696e 6f6d 6961 6c22 2c0a 2020 2020 224f  inomial",.    "O
-000009d0: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
-000009e0: 6c22 2c0a 2020 2020 2257 6973 6861 7274  l",.    "Wishart
-000009f0: 222c 0a20 2020 2022 5769 7368 6172 7442  ",.    "WishartB
-00000a00: 6172 746c 6574 7422 2c0a 2020 2020 224c  artlett",.    "L
-00000a10: 4b4a 436f 7272 222c 0a20 2020 2022 4c4b  KJCorr",.    "LK
-00000a20: 4a43 686f 6c65 736b 7943 6f76 222c 0a20  JCholeskyCov",. 
-00000a30: 2020 2022 4d61 7472 6978 4e6f 726d 616c     "MatrixNormal
-00000a40: 222c 0a20 2020 2022 4b72 6f6e 6563 6b65  ",.    "Kronecke
-00000a50: 724e 6f72 6d61 6c22 2c0a 2020 2020 2243  rNormal",.    "C
-00000a60: 4152 222c 0a20 2020 2022 5374 6963 6b42  AR",.    "StickB
-00000a70: 7265 616b 696e 6757 6569 6768 7473 222c  reakingWeights",
-00000a80: 0a5d 0a0a 736f 6c76 655f 6c6f 7765 7220  .]..solve_lower 
-00000a90: 3d20 536f 6c76 6554 7269 616e 6775 6c61  = SolveTriangula
-00000aa0: 7228 6c6f 7765 723d 5472 7565 290a 736f  r(lower=True).so
-00000ab0: 6c76 655f 7570 7065 7220 3d20 536f 6c76  lve_upper = Solv
-00000ac0: 6554 7269 616e 6775 6c61 7228 6c6f 7765  eTriangular(lowe
-00000ad0: 723d 4661 6c73 6529 0a0a 0a63 6c61 7373  r=False)...class
-00000ae0: 2053 696d 706c 6578 436f 6e74 696e 756f   SimplexContinuo
-00000af0: 7573 2843 6f6e 7469 6e75 6f75 7329 3a0a  us(Continuous):.
-00000b00: 2020 2020 2222 2242 6173 6520 636c 6173      """Base clas
-00000b10: 7320 666f 7220 7369 6d70 6c65 7820 636f  s for simplex co
-00000b20: 6e74 696e 756f 7573 2064 6973 7472 6962  ntinuous distrib
-00000b30: 7574 696f 6e73 2222 220a 0a0a 405f 6465  utions"""...@_de
-00000b40: 6661 756c 745f 7472 616e 7366 6f72 6d2e  fault_transform.
-00000b50: 7265 6769 7374 6572 2853 696d 706c 6578  register(Simplex
-00000b60: 436f 6e74 696e 756f 7573 290a 6465 6620  Continuous).def 
-00000b70: 7369 6d70 6c65 785f 636f 6e74 5f74 7261  simplex_cont_tra
-00000b80: 6e73 666f 726d 286f 702c 2072 7629 3a0a  nsform(op, rv):.
-00000b90: 2020 2020 7265 7475 726e 2074 7261 6e73      return trans
-00000ba0: 666f 726d 732e 7369 6d70 6c65 780a 0a0a  forms.simplex...
-00000bb0: 2320 5374 6570 206d 6574 686f 6473 2061  # Step methods a
-00000bc0: 6e64 2061 6476 6920 646f 206e 6f74 2063  nd advi do not c
-00000bd0: 6174 6368 204c 696e 416c 6745 7272 6f72  atch LinAlgError
-00000be0: 7320 6174 2074 6865 0a23 206d 6f6d 656e  s at the.# momen
-00000bf0: 742e 2057 6520 776f 726b 2061 726f 756e  t. We work aroun
-00000c00: 6420 7468 6174 2062 7920 7573 696e 6720  d that by using 
-00000c10: 6120 6368 6f6c 6573 6b79 206f 700a 2320  a cholesky op.# 
-00000c20: 7468 6174 2072 6574 7572 6e73 2061 206e  that returns a n
-00000c30: 616e 2061 7320 6669 7273 7420 656e 7472  an as first entr
-00000c40: 7920 696e 7374 6561 6420 6f66 2072 6169  y instead of rai
-00000c50: 7369 6e67 0a23 2061 6e20 6572 726f 722e  sing.# an error.
-00000c60: 0a63 686f 6c65 736b 7920 3d20 4368 6f6c  .cholesky = Chol
-00000c70: 6573 6b79 286c 6f77 6572 3d54 7275 652c  esky(lower=True,
-00000c80: 206f 6e5f 6572 726f 723d 226e 616e 2229   on_error="nan")
-00000c90: 0a0a 0a64 6566 2071 7561 6464 6973 745f  ...def quaddist_
-00000ca0: 6d61 7472 6978 2863 6f76 3d4e 6f6e 652c  matrix(cov=None,
-00000cb0: 2063 686f 6c3d 4e6f 6e65 2c20 7461 753d   chol=None, tau=
-00000cc0: 4e6f 6e65 2c20 6c6f 7765 723d 5472 7565  None, lower=True
-00000cd0: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00000ce0: 7329 3a0a 2020 2020 6966 2063 686f 6c20  s):.    if chol 
-00000cf0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-00000d00: 6e6f 7420 6c6f 7765 723a 0a20 2020 2020  not lower:.     
-00000d10: 2020 2063 686f 6c20 3d20 6368 6f6c 2e54     chol = chol.T
-00000d20: 0a0a 2020 2020 6966 206c 656e 285b 6920  ..    if len([i 
-00000d30: 666f 7220 6920 696e 205b 7461 752c 2063  for i in [tau, c
-00000d40: 6f76 2c20 6368 6f6c 5d20 6966 2069 2069  ov, chol] if i i
-00000d50: 7320 6e6f 7420 4e6f 6e65 5d29 2021 3d20  s not None]) != 
-00000d60: 313a 0a20 2020 2020 2020 2072 6169 7365  1:.        raise
-00000d70: 2056 616c 7565 4572 726f 7228 2249 6e63   ValueError("Inc
-00000d80: 6f6d 7061 7469 626c 6520 7061 7261 6d65  ompatible parame
-00000d90: 7465 7269 7a61 7469 6f6e 2e20 5370 6563  terization. Spec
-00000da0: 6966 7920 6578 6163 746c 7920 6f6e 6520  ify exactly one 
-00000db0: 6f66 2074 6175 2c20 636f 762c 206f 7220  of tau, cov, or 
-00000dc0: 6368 6f6c 2e22 290a 0a20 2020 2069 6620  chol.")..    if 
-00000dd0: 636f 7620 6973 206e 6f74 204e 6f6e 653a  cov is not None:
-00000de0: 0a20 2020 2020 2020 2063 6f76 203d 2070  .        cov = p
-00000df0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00000e00: 6162 6c65 2863 6f76 290a 2020 2020 2020  able(cov).      
-00000e10: 2020 6966 2063 6f76 2e6e 6469 6d20 213d    if cov.ndim !=
-00000e20: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00000e30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00000e40: 2822 636f 7620 6d75 7374 2062 6520 7477  ("cov must be tw
-00000e50: 6f20 6469 6d65 6e73 696f 6e61 6c2e 2229  o dimensional.")
-00000e60: 0a20 2020 2065 6c69 6620 7461 7520 6973  .    elif tau is
-00000e70: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00000e80: 2020 2074 6175 203d 2070 742e 6173 5f74     tau = pt.as_t
-00000e90: 656e 736f 725f 7661 7269 6162 6c65 2874  ensor_variable(t
-00000ea0: 6175 290a 2020 2020 2020 2020 6966 2074  au).        if t
-00000eb0: 6175 2e6e 6469 6d20 213d 2032 3a0a 2020  au.ndim != 2:.  
-00000ec0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00000ed0: 5661 6c75 6545 7272 6f72 2822 7461 7520  ValueError("tau 
-00000ee0: 6d75 7374 2062 6520 7477 6f20 6469 6d65  must be two dime
-00000ef0: 6e73 696f 6e61 6c2e 2229 0a20 2020 2020  nsional.").     
-00000f00: 2020 2023 2054 4f44 4f3a 2057 6861 7427     # TODO: What'
-00000f10: 7320 7468 6520 636f 7272 6563 7420 6f72  s the correct or
-00000f20: 6465 722f 6170 7072 6f61 6368 2028 696e  der/approach (in
-00000f30: 2074 6865 206e 6f6e 2d73 7175 6172 6520   the non-square 
-00000f40: 6361 7365 293f 0a20 2020 2020 2020 2023  case)?.        #
-00000f50: 2060 7079 7465 6e73 6f72 2e74 656e 736f   `pytensor.tenso
-00000f60: 722e 6e6c 696e 616c 672e 7465 6e73 6f72  r.nlinalg.tensor
-00000f70: 696e 7660 3f0a 2020 2020 2020 2020 636f  inv`?.        co
-00000f80: 7620 3d20 6d61 7472 6978 5f69 6e76 6572  v = matrix_inver
-00000f90: 7365 2874 6175 290a 2020 2020 656c 7365  se(tau).    else
-00000fa0: 3a0a 2020 2020 2020 2020 2320 544f 444f  :.        # TODO
-00000fb0: 3a20 5768 6174 2773 2074 6865 2063 6f72  : What's the cor
-00000fc0: 7265 6374 206f 7264 6572 2f61 7070 726f  rect order/appro
-00000fd0: 6163 6820 2869 6e20 7468 6520 6e6f 6e2d  ach (in the non-
-00000fe0: 7371 7561 7265 2063 6173 6529 3f0a 2020  square case)?.  
-00000ff0: 2020 2020 2020 6368 6f6c 203d 2070 742e        chol = pt.
-00001000: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-00001010: 6c65 2863 686f 6c29 0a20 2020 2020 2020  le(chol).       
-00001020: 2069 6620 6368 6f6c 2e6e 6469 6d20 213d   if chol.ndim !=
-00001030: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00001040: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00001050: 2822 6368 6f6c 206d 7573 7420 6265 2074  ("chol must be t
-00001060: 776f 2064 696d 656e 7369 6f6e 616c 2e22  wo dimensional."
-00001070: 290a 2020 2020 2020 2020 636f 7620 3d20  ).        cov = 
-00001080: 6368 6f6c 2e64 6f74 2863 686f 6c2e 5429  chol.dot(chol.T)
-00001090: 0a0a 2020 2020 7265 7475 726e 2063 6f76  ..    return cov
-000010a0: 0a0a 0a64 6566 2071 7561 6464 6973 745f  ...def quaddist_
-000010b0: 7061 7273 6528 7661 6c75 652c 206d 752c  parse(value, mu,
-000010c0: 2063 6f76 2c20 6d61 745f 7479 7065 3d22   cov, mat_type="
-000010d0: 636f 7622 293a 0a20 2020 2022 2222 436f  cov"):.    """Co
-000010e0: 6d70 7574 6520 2878 202d 206d 7529 2e54  mpute (x - mu).T
-000010f0: 2040 2053 6967 6d61 5e2d 3120 4020 2878   @ Sigma^-1 @ (x
-00001100: 202d 206d 7529 2061 6e64 2074 6865 206c   - mu) and the l
-00001110: 6f67 6465 7420 6f66 2053 6967 6d61 2e22  ogdet of Sigma."
-00001120: 2222 0a20 2020 2069 6620 7661 6c75 652e  "".    if value.
-00001130: 6e64 696d 203e 2032 206f 7220 7661 6c75  ndim > 2 or valu
-00001140: 652e 6e64 696d 203d 3d20 303a 0a20 2020  e.ndim == 0:.   
-00001150: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-00001160: 4572 726f 7228 2249 6e76 616c 6964 2064  Error("Invalid d
-00001170: 696d 656e 7369 6f6e 2066 6f72 2076 616c  imension for val
-00001180: 7565 3a20 2573 2220 2520 7661 6c75 652e  ue: %s" % value.
-00001190: 6e64 696d 290a 2020 2020 6966 2076 616c  ndim).    if val
-000011a0: 7565 2e6e 6469 6d20 3d3d 2031 3a0a 2020  ue.ndim == 1:.  
-000011b0: 2020 2020 2020 6f6e 6564 696d 203d 2054        onedim = T
-000011c0: 7275 650a 2020 2020 2020 2020 7661 6c75  rue.        valu
-000011d0: 6520 3d20 7661 6c75 655b 4e6f 6e65 2c20  e = value[None, 
-000011e0: 3a5d 0a20 2020 2065 6c73 653a 0a20 2020  :].    else:.   
-000011f0: 2020 2020 206f 6e65 6469 6d20 3d20 4661       onedim = Fa
-00001200: 6c73 650a 0a20 2020 2064 656c 7461 203d  lse..    delta =
-00001210: 2076 616c 7565 202d 206d 750a 2020 2020   value - mu.    
-00001220: 2320 5573 6520 7468 6973 2077 6865 6e20  # Use this when 
-00001230: 5468 6561 6e6f 2335 3930 3820 6973 2072  Theano#5908 is r
-00001240: 656c 6561 7365 642e 0a20 2020 2023 2072  eleased..    # r
-00001250: 6574 7572 6e20 4d76 4e6f 726d 616c 4c6f  eturn MvNormalLo
-00001260: 6770 2829 2873 656c 662e 636f 762c 2064  gp()(self.cov, d
-00001270: 656c 7461 290a 2020 2020 6368 6f6c 5f63  elta).    chol_c
-00001280: 6f76 203d 2063 686f 6c65 736b 7928 636f  ov = cholesky(co
-00001290: 7629 0a20 2020 2069 6620 6d61 745f 7479  v).    if mat_ty
-000012a0: 7065 2021 3d20 2274 6175 223a 0a20 2020  pe != "tau":.   
-000012b0: 2020 2020 2064 6973 742c 206c 6f67 6465       dist, logde
-000012c0: 742c 206f 6b20 3d20 7175 6164 6469 7374  t, ok = quaddist
-000012d0: 5f63 686f 6c28 6465 6c74 612c 2063 686f  _chol(delta, cho
-000012e0: 6c5f 636f 7629 0a20 2020 2065 6c73 653a  l_cov).    else:
-000012f0: 0a20 2020 2020 2020 2064 6973 742c 206c  .        dist, l
-00001300: 6f67 6465 742c 206f 6b20 3d20 7175 6164  ogdet, ok = quad
-00001310: 6469 7374 5f74 6175 2864 656c 7461 2c20  dist_tau(delta, 
-00001320: 6368 6f6c 5f63 6f76 290a 2020 2020 6966  chol_cov).    if
-00001330: 206f 6e65 6469 6d3a 0a20 2020 2020 2020   onedim:.       
-00001340: 2072 6574 7572 6e20 6469 7374 5b30 5d2c   return dist[0],
-00001350: 206c 6f67 6465 742c 206f 6b0a 0a20 2020   logdet, ok..   
-00001360: 2072 6574 7572 6e20 6469 7374 2c20 6c6f   return dist, lo
-00001370: 6764 6574 2c20 6f6b 0a0a 0a64 6566 2071  gdet, ok...def q
-00001380: 7561 6464 6973 745f 6368 6f6c 2864 656c  uaddist_chol(del
-00001390: 7461 2c20 6368 6f6c 5f6d 6174 293a 0a20  ta, chol_mat):. 
-000013a0: 2020 2064 6961 6720 3d20 7074 2e64 6961     diag = pt.dia
-000013b0: 6728 6368 6f6c 5f6d 6174 290a 2020 2020  g(chol_mat).    
-000013c0: 2320 4368 6563 6b20 6966 2074 6865 2063  # Check if the c
-000013d0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-000013e0: 2069 7320 706f 7369 7469 7665 2064 6566   is positive def
-000013f0: 696e 6974 652e 0a20 2020 206f 6b20 3d20  inite..    ok = 
-00001400: 7074 2e61 6c6c 2864 6961 6720 3e20 3029  pt.all(diag > 0)
-00001410: 0a20 2020 2023 2049 6620 6e6f 742c 2072  .    # If not, r
-00001420: 6570 6c61 6365 2074 6865 2064 6961 676f  eplace the diago
-00001430: 6e61 6c2e 2057 6520 7265 7475 726e 202d  nal. We return -
-00001440: 696e 6620 6c61 7465 722c 2062 7574 0a20  inf later, but. 
-00001450: 2020 2023 206e 6565 6420 746f 2070 7265     # need to pre
-00001460: 7665 6e74 2073 6f6c 7665 5f6c 6f77 6572  vent solve_lower
-00001470: 2066 726f 6d20 7468 726f 7769 6e67 2061   from throwing a
-00001480: 6e20 6578 6365 7074 696f 6e2e 0a20 2020  n exception..   
-00001490: 2063 686f 6c5f 636f 7620 3d20 7074 2e73   chol_cov = pt.s
-000014a0: 7769 7463 6828 6f6b 2c20 6368 6f6c 5f6d  witch(ok, chol_m
-000014b0: 6174 2c20 3129 0a0a 2020 2020 6465 6c74  at, 1)..    delt
-000014c0: 615f 7472 616e 7320 3d20 736f 6c76 655f  a_trans = solve_
-000014d0: 6c6f 7765 7228 6368 6f6c 5f63 6f76 2c20  lower(chol_cov, 
-000014e0: 6465 6c74 612e 5429 2e54 0a20 2020 2071  delta.T).T.    q
-000014f0: 7561 6464 6973 7420 3d20 2864 656c 7461  uaddist = (delta
-00001500: 5f74 7261 6e73 2a2a 3229 2e73 756d 2861  _trans**2).sum(a
-00001510: 7869 733d 2d31 290a 2020 2020 6c6f 6764  xis=-1).    logd
-00001520: 6574 203d 2070 742e 7375 6d28 7074 2e6c  et = pt.sum(pt.l
-00001530: 6f67 2864 6961 6729 290a 2020 2020 7265  og(diag)).    re
-00001540: 7475 726e 2071 7561 6464 6973 742c 206c  turn quaddist, l
-00001550: 6f67 6465 742c 206f 6b0a 0a0a 6465 6620  ogdet, ok...def 
-00001560: 7175 6164 6469 7374 5f74 6175 2864 656c  quaddist_tau(del
-00001570: 7461 2c20 6368 6f6c 5f6d 6174 293a 0a20  ta, chol_mat):. 
-00001580: 2020 2064 6961 6720 3d20 7074 2e6e 6c69     diag = pt.nli
-00001590: 6e61 6c67 2e64 6961 6728 6368 6f6c 5f6d  nalg.diag(chol_m
-000015a0: 6174 290a 2020 2020 2320 4368 6563 6b20  at).    # Check 
-000015b0: 6966 2074 6865 2070 7265 6369 7369 6f6e  if the precision
-000015c0: 206d 6174 7269 7820 6973 2070 6f73 6974   matrix is posit
-000015d0: 6976 6520 6465 6669 6e69 7465 2e0a 2020  ive definite..  
-000015e0: 2020 6f6b 203d 2070 742e 616c 6c28 6469    ok = pt.all(di
-000015f0: 6167 203e 2030 290a 2020 2020 2320 4966  ag > 0).    # If
-00001600: 206e 6f74 2c20 7265 706c 6163 6520 7468   not, replace th
-00001610: 6520 6469 6167 6f6e 616c 2e20 5765 2072  e diagonal. We r
-00001620: 6574 7572 6e20 2d69 6e66 206c 6174 6572  eturn -inf later
-00001630: 2c20 6275 740a 2020 2020 2320 6e65 6564  , but.    # need
-00001640: 2074 6f20 7072 6576 656e 7420 736f 6c76   to prevent solv
-00001650: 655f 6c6f 7765 7220 6672 6f6d 2074 6872  e_lower from thr
-00001660: 6f77 696e 6720 616e 2065 7863 6570 7469  owing an excepti
-00001670: 6f6e 2e0a 2020 2020 6368 6f6c 5f74 6175  on..    chol_tau
-00001680: 203d 2070 742e 7377 6974 6368 286f 6b2c   = pt.switch(ok,
-00001690: 2063 686f 6c5f 6d61 742c 2031 290a 0a20   chol_mat, 1).. 
-000016a0: 2020 2064 656c 7461 5f74 7261 6e73 203d     delta_trans =
-000016b0: 2070 742e 646f 7428 6465 6c74 612c 2063   pt.dot(delta, c
-000016c0: 686f 6c5f 7461 7529 0a20 2020 2071 7561  hol_tau).    qua
-000016d0: 6464 6973 7420 3d20 2864 656c 7461 5f74  ddist = (delta_t
-000016e0: 7261 6e73 2a2a 3229 2e73 756d 2861 7869  rans**2).sum(axi
-000016f0: 733d 2d31 290a 2020 2020 6c6f 6764 6574  s=-1).    logdet
-00001700: 203d 202d 7074 2e73 756d 2870 742e 6c6f   = -pt.sum(pt.lo
-00001710: 6728 6469 6167 2929 0a20 2020 2072 6574  g(diag)).    ret
-00001720: 7572 6e20 7175 6164 6469 7374 2c20 6c6f  urn quaddist, lo
-00001730: 6764 6574 2c20 6f6b 0a0a 0a63 6c61 7373  gdet, ok...class
-00001740: 204d 764e 6f72 6d61 6c28 436f 6e74 696e   MvNormal(Contin
-00001750: 756f 7573 293a 0a20 2020 2072 2222 220a  uous):.    r""".
-00001760: 2020 2020 4d75 6c74 6976 6172 6961 7465      Multivariate
-00001770: 206e 6f72 6d61 6c20 6c6f 672d 6c69 6b65   normal log-like
-00001780: 6c69 686f 6f64 2e0a 0a20 2020 202e 2e20  lihood...    .. 
-00001790: 6d61 7468 3a3a 0a0a 2020 2020 2020 2066  math::..       f
-000017a0: 2878 205c 6d69 6420 5c70 692c 2054 2920  (x \mid \pi, T) 
-000017b0: 3d0a 2020 2020 2020 2020 2020 205c 6672  =.           \fr
-000017c0: 6163 7b7c 547c 5e7b 312f 327d 7d7b 2832  ac{|T|^{1/2}}{(2
-000017d0: 5c70 6929 5e7b 6b2f 327d 7d0a 2020 2020  \pi)^{k/2}}.    
-000017e0: 2020 2020 2020 205c 6578 705c 6c65 6674         \exp\left
-000017f0: 5c7b 202d 5c66 7261 637b 317d 7b32 7d20  \{ -\frac{1}{2} 
-00001800: 2878 2d5c 6d75 295e 7b5c 7072 696d 657d  (x-\mu)^{\prime}
-00001810: 2054 2028 782d 5c6d 7529 205c 7269 6768   T (x-\mu) \righ
-00001820: 745c 7d0a 0a20 2020 203d 3d3d 3d3d 3d3d  t\}..    =======
-00001830: 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =  =============
-00001840: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
-00001850: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
-00001860: 683a 6078 205c 696e 205c 6d61 7468 6262  h:`x \in \mathbb
-00001870: 7b52 7d5e 6b60 0a20 2020 204d 6561 6e20  {R}^k`.    Mean 
-00001880: 2020 2020 203a 6d61 7468 3a60 5c6d 7560       :math:`\mu`
-00001890: 0a20 2020 2056 6172 6961 6e63 6520 203a  .    Variance  :
-000018a0: 6d61 7468 3a60 545e 7b2d 317d 600a 2020  math:`T^{-1}`.  
-000018b0: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
-000018c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000018d0: 3d3d 3d3d 3d3d 0a0a 2020 2020 5061 7261  ======..    Para
-000018e0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-000018f0: 2d2d 2d2d 2d0a 2020 2020 6d75 203a 2074  -----.    mu : t
-00001900: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-00001910: 6f61 740a 2020 2020 2020 2020 5665 6374  oat.        Vect
-00001920: 6f72 206f 6620 6d65 616e 732e 0a20 2020  or of means..   
-00001930: 2063 6f76 203a 2074 656e 736f 725f 6c69   cov : tensor_li
-00001940: 6b65 206f 6620 666c 6f61 742c 206f 7074  ke of float, opt
-00001950: 696f 6e61 6c0a 2020 2020 2020 2020 436f  ional.        Co
-00001960: 7661 7269 616e 6365 206d 6174 7269 782e  variance matrix.
-00001970: 2045 7861 6374 6c79 206f 6e65 206f 6620   Exactly one of 
-00001980: 636f 762c 2074 6175 2c20 6f72 2063 686f  cov, tau, or cho
-00001990: 6c20 6973 206e 6565 6465 642e 0a20 2020  l is needed..   
-000019a0: 2074 6175 203a 2074 656e 736f 725f 6c69   tau : tensor_li
-000019b0: 6b65 206f 6620 666c 6f61 742c 206f 7074  ke of float, opt
-000019c0: 696f 6e61 6c0a 2020 2020 2020 2020 5072  ional.        Pr
-000019d0: 6563 6973 696f 6e20 6d61 7472 6978 2e20  ecision matrix. 
-000019e0: 4578 6163 746c 7920 6f6e 6520 6f66 2063  Exactly one of c
-000019f0: 6f76 2c20 7461 752c 206f 7220 6368 6f6c  ov, tau, or chol
-00001a00: 2069 7320 6e65 6564 6564 2e0a 2020 2020   is needed..    
-00001a10: 6368 6f6c 203a 2074 656e 736f 725f 6c69  chol : tensor_li
-00001a20: 6b65 206f 6620 666c 6f61 742c 206f 7074  ke of float, opt
-00001a30: 696f 6e61 6c0a 2020 2020 2020 2020 4368  ional.        Ch
-00001a40: 6f6c 6573 6b79 2064 6563 6f6d 706f 7369  olesky decomposi
-00001a50: 7469 6f6e 206f 6620 636f 7661 7269 616e  tion of covarian
-00001a60: 6365 206d 6174 7269 782e 2045 7861 6374  ce matrix. Exact
-00001a70: 6c79 206f 6e65 206f 6620 636f 762c 0a20  ly one of cov,. 
-00001a80: 2020 2020 2020 2074 6175 2c20 6f72 2063         tau, or c
-00001a90: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
-00001aa0: 2020 206c 6f77 6572 3a20 626f 6f6c 2c20     lower: bool, 
-00001ab0: 6465 6661 756c 743d 5472 7565 0a20 2020  default=True.   
-00001ac0: 2020 2020 2057 6865 7468 6572 2063 686f       Whether cho
-00001ad0: 6c20 6973 2074 6865 206c 6f77 6572 2074  l is the lower t
-00001ae0: 7269 6469 6167 6f6e 616c 2063 686f 6c65  ridiagonal chole
-00001af0: 736b 7920 6661 6374 6f72 2e0a 0a20 2020  sky factor...   
-00001b00: 2045 7861 6d70 6c65 730a 2020 2020 2d2d   Examples.    --
-00001b10: 2d2d 2d2d 2d2d 0a20 2020 2044 6566 696e  ------.    Defin
-00001b20: 6520 6120 6d75 6c74 6976 6172 6961 7465  e a multivariate
-00001b30: 206e 6f72 6d61 6c20 7661 7269 6162 6c65   normal variable
-00001b40: 2066 6f72 2061 2067 6976 656e 2063 6f76   for a given cov
-00001b50: 6172 6961 6e63 650a 2020 2020 6d61 7472  ariance.    matr
-00001b60: 6978 3a3a 0a0a 2020 2020 2020 2020 636f  ix::..        co
-00001b70: 7620 3d20 6e70 2e61 7272 6179 285b 5b31  v = np.array([[1
-00001b80: 2e2c 2030 2e35 5d2c 205b 302e 352c 2032  ., 0.5], [0.5, 2
-00001b90: 5d5d 290a 2020 2020 2020 2020 6d75 203d  ]]).        mu =
-00001ba0: 206e 702e 7a65 726f 7328 3229 0a20 2020   np.zeros(2).   
-00001bb0: 2020 2020 2076 616c 7320 3d20 706d 2e4d       vals = pm.M
-00001bc0: 764e 6f72 6d61 6c28 2776 616c 7327 2c20  vNormal('vals', 
-00001bd0: 6d75 3d6d 752c 2063 6f76 3d63 6f76 2c20  mu=mu, cov=cov, 
-00001be0: 7368 6170 653d 2835 2c20 3229 290a 0a20  shape=(5, 2)).. 
-00001bf0: 2020 204d 6f73 7420 6f66 2074 6865 2074     Most of the t
-00001c00: 696d 6520 6974 2069 7320 7072 6566 6572  ime it is prefer
-00001c10: 6162 6c65 2074 6f20 7370 6563 6966 7920  able to specify 
-00001c20: 7468 6520 6368 6f6c 6573 6b79 0a20 2020  the cholesky.   
-00001c30: 2066 6163 746f 7220 6f66 2074 6865 2063   factor of the c
-00001c40: 6f76 6172 6961 6e63 6520 696e 7374 6561  ovariance instea
-00001c50: 642e 2046 6f72 2065 7861 6d70 6c65 2c20  d. For example, 
-00001c60: 7765 2063 6f75 6c64 0a20 2020 2066 6974  we could.    fit
-00001c70: 2061 206d 756c 7469 7661 7269 6174 6520   a multivariate 
-00001c80: 6f75 7463 6f6d 6520 6c69 6b65 2074 6869  outcome like thi
-00001c90: 7320 2873 6565 2074 6865 2064 6f63 7374  s (see the docst
-00001ca0: 7269 6e67 0a20 2020 206f 6620 604c 4b4a  ring.    of `LKJ
-00001cb0: 4368 6f6c 6573 6b79 436f 7660 2066 6f72  CholeskyCov` for
-00001cc0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
-00001cd0: 6e20 6162 6f75 7420 7468 6973 293a 3a0a  n about this)::.
-00001ce0: 0a20 2020 2020 2020 206d 7520 3d20 6e70  .        mu = np
-00001cf0: 2e7a 6572 6f73 2833 290a 2020 2020 2020  .zeros(3).      
-00001d00: 2020 7472 7565 5f63 6f76 203d 206e 702e    true_cov = np.
-00001d10: 6172 7261 7928 5b5b 312e 302c 2030 2e35  array([[1.0, 0.5
-00001d20: 2c20 302e 315d 2c0a 2020 2020 2020 2020  , 0.1],.        
+000008a0: 6d61 7468 2069 6d70 6f72 7420 6b72 6f6e  math import kron
+000008b0: 5f64 6961 672c 206b 726f 6e5f 646f 740a  _diag, kron_dot.
+000008c0: 6672 6f6d 2070 796d 632e 7079 7465 6e73  from pymc.pytens
+000008d0: 6f72 6620 696d 706f 7274 2066 6c6f 6174  orf import float
+000008e0: 582c 2069 6e74 580a 6672 6f6d 2070 796d  X, intX.from pym
+000008f0: 632e 7574 696c 2069 6d70 6f72 7420 6368  c.util import ch
+00000900: 6563 6b5f 6469 7374 5f6e 6f74 5f72 6567  eck_dist_not_reg
+00000910: 6973 7465 7265 640a 0a5f 5f61 6c6c 5f5f  istered..__all__
+00000920: 203d 205b 0a20 2020 2022 4d76 4e6f 726d   = [.    "MvNorm
+00000930: 616c 222c 0a20 2020 2022 5a65 726f 5375  al",.    "ZeroSu
+00000940: 6d4e 6f72 6d61 6c22 2c0a 2020 2020 224d  mNormal",.    "M
+00000950: 7653 7475 6465 6e74 5422 2c0a 2020 2020  vStudentT",.    
+00000960: 2244 6972 6963 686c 6574 222c 0a20 2020  "Dirichlet",.   
+00000970: 2022 4d75 6c74 696e 6f6d 6961 6c22 2c0a   "Multinomial",.
+00000980: 2020 2020 2244 6972 6963 686c 6574 4d75      "DirichletMu
+00000990: 6c74 696e 6f6d 6961 6c22 2c0a 2020 2020  ltinomial",.    
+000009a0: 224f 7264 6572 6564 4d75 6c74 696e 6f6d  "OrderedMultinom
+000009b0: 6961 6c22 2c0a 2020 2020 2257 6973 6861  ial",.    "Wisha
+000009c0: 7274 222c 0a20 2020 2022 5769 7368 6172  rt",.    "Wishar
+000009d0: 7442 6172 746c 6574 7422 2c0a 2020 2020  tBartlett",.    
+000009e0: 224c 4b4a 436f 7272 222c 0a20 2020 2022  "LKJCorr",.    "
+000009f0: 4c4b 4a43 686f 6c65 736b 7943 6f76 222c  LKJCholeskyCov",
+00000a00: 0a20 2020 2022 4d61 7472 6978 4e6f 726d  .    "MatrixNorm
+00000a10: 616c 222c 0a20 2020 2022 4b72 6f6e 6563  al",.    "Kronec
+00000a20: 6b65 724e 6f72 6d61 6c22 2c0a 2020 2020  kerNormal",.    
+00000a30: 2243 4152 222c 0a20 2020 2022 5374 6963  "CAR",.    "Stic
+00000a40: 6b42 7265 616b 696e 6757 6569 6768 7473  kBreakingWeights
+00000a50: 222c 0a5d 0a0a 736f 6c76 655f 6c6f 7765  ",.]..solve_lowe
+00000a60: 7220 3d20 536f 6c76 6554 7269 616e 6775  r = SolveTriangu
+00000a70: 6c61 7228 6c6f 7765 723d 5472 7565 290a  lar(lower=True).
+00000a80: 736f 6c76 655f 7570 7065 7220 3d20 536f  solve_upper = So
+00000a90: 6c76 6554 7269 616e 6775 6c61 7228 6c6f  lveTriangular(lo
+00000aa0: 7765 723d 4661 6c73 6529 0a0a 0a63 6c61  wer=False)...cla
+00000ab0: 7373 2053 696d 706c 6578 436f 6e74 696e  ss SimplexContin
+00000ac0: 756f 7573 2843 6f6e 7469 6e75 6f75 7329  uous(Continuous)
+00000ad0: 3a0a 2020 2020 2222 2242 6173 6520 636c  :.    """Base cl
+00000ae0: 6173 7320 666f 7220 7369 6d70 6c65 7820  ass for simplex 
+00000af0: 636f 6e74 696e 756f 7573 2064 6973 7472  continuous distr
+00000b00: 6962 7574 696f 6e73 2222 220a 0a0a 405f  ibutions"""...@_
+00000b10: 6465 6661 756c 745f 7472 616e 7366 6f72  default_transfor
+00000b20: 6d2e 7265 6769 7374 6572 2853 696d 706c  m.register(Simpl
+00000b30: 6578 436f 6e74 696e 756f 7573 290a 6465  exContinuous).de
+00000b40: 6620 7369 6d70 6c65 785f 636f 6e74 5f74  f simplex_cont_t
+00000b50: 7261 6e73 666f 726d 286f 702c 2072 7629  ransform(op, rv)
+00000b60: 3a0a 2020 2020 7265 7475 726e 2074 7261  :.    return tra
+00000b70: 6e73 666f 726d 732e 7369 6d70 6c65 780a  nsforms.simplex.
+00000b80: 0a0a 2320 5374 6570 206d 6574 686f 6473  ..# Step methods
+00000b90: 2061 6e64 2061 6476 6920 646f 206e 6f74   and advi do not
+00000ba0: 2063 6174 6368 204c 696e 416c 6745 7272   catch LinAlgErr
+00000bb0: 6f72 7320 6174 2074 6865 0a23 206d 6f6d  ors at the.# mom
+00000bc0: 656e 742e 2057 6520 776f 726b 2061 726f  ent. We work aro
+00000bd0: 756e 6420 7468 6174 2062 7920 7573 696e  und that by usin
+00000be0: 6720 6120 6368 6f6c 6573 6b79 206f 700a  g a cholesky op.
+00000bf0: 2320 7468 6174 2072 6574 7572 6e73 2061  # that returns a
+00000c00: 206e 616e 2061 7320 6669 7273 7420 656e   nan as first en
+00000c10: 7472 7920 696e 7374 6561 6420 6f66 2072  try instead of r
+00000c20: 6169 7369 6e67 0a23 2061 6e20 6572 726f  aising.# an erro
+00000c30: 722e 0a63 686f 6c65 736b 7920 3d20 4368  r..cholesky = Ch
+00000c40: 6f6c 6573 6b79 286c 6f77 6572 3d54 7275  olesky(lower=Tru
+00000c50: 652c 206f 6e5f 6572 726f 723d 226e 616e  e, on_error="nan
+00000c60: 2229 0a0a 0a64 6566 2071 7561 6464 6973  ")...def quaddis
+00000c70: 745f 6d61 7472 6978 2863 6f76 3d4e 6f6e  t_matrix(cov=Non
+00000c80: 652c 2063 686f 6c3d 4e6f 6e65 2c20 7461  e, chol=None, ta
+00000c90: 753d 4e6f 6e65 2c20 6c6f 7765 723d 5472  u=None, lower=Tr
+00000ca0: 7565 2c20 2a61 7267 732c 202a 2a6b 7761  ue, *args, **kwa
+00000cb0: 7267 7329 3a0a 2020 2020 6966 2063 686f  rgs):.    if cho
+00000cc0: 6c20 6973 206e 6f74 204e 6f6e 6520 616e  l is not None an
+00000cd0: 6420 6e6f 7420 6c6f 7765 723a 0a20 2020  d not lower:.   
+00000ce0: 2020 2020 2063 686f 6c20 3d20 6368 6f6c       chol = chol
+00000cf0: 2e54 0a0a 2020 2020 6966 206c 656e 285b  .T..    if len([
+00000d00: 6920 666f 7220 6920 696e 205b 7461 752c  i for i in [tau,
+00000d10: 2063 6f76 2c20 6368 6f6c 5d20 6966 2069   cov, chol] if i
+00000d20: 2069 7320 6e6f 7420 4e6f 6e65 5d29 2021   is not None]) !
+00000d30: 3d20 313a 0a20 2020 2020 2020 2072 6169  = 1:.        rai
+00000d40: 7365 2056 616c 7565 4572 726f 7228 2249  se ValueError("I
+00000d50: 6e63 6f6d 7061 7469 626c 6520 7061 7261  ncompatible para
+00000d60: 6d65 7465 7269 7a61 7469 6f6e 2e20 5370  meterization. Sp
+00000d70: 6563 6966 7920 6578 6163 746c 7920 6f6e  ecify exactly on
+00000d80: 6520 6f66 2074 6175 2c20 636f 762c 206f  e of tau, cov, o
+00000d90: 7220 6368 6f6c 2e22 290a 0a20 2020 2069  r chol.")..    i
+00000da0: 6620 636f 7620 6973 206e 6f74 204e 6f6e  f cov is not Non
+00000db0: 653a 0a20 2020 2020 2020 2063 6f76 203d  e:.        cov =
+00000dc0: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+00000dd0: 7269 6162 6c65 2863 6f76 290a 2020 2020  riable(cov).    
+00000de0: 2020 2020 6966 2063 6f76 2e6e 6469 6d20      if cov.ndim 
+00000df0: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
+00000e00: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00000e10: 6f72 2822 636f 7620 6d75 7374 2062 6520  or("cov must be 
+00000e20: 7477 6f20 6469 6d65 6e73 696f 6e61 6c2e  two dimensional.
+00000e30: 2229 0a20 2020 2065 6c69 6620 7461 7520  ").    elif tau 
+00000e40: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00000e50: 2020 2020 2074 6175 203d 2070 742e 6173       tau = pt.as
+00000e60: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00000e70: 2874 6175 290a 2020 2020 2020 2020 6966  (tau).        if
+00000e80: 2074 6175 2e6e 6469 6d20 213d 2032 3a0a   tau.ndim != 2:.
+00000e90: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00000ea0: 6520 5661 6c75 6545 7272 6f72 2822 7461  e ValueError("ta
+00000eb0: 7520 6d75 7374 2062 6520 7477 6f20 6469  u must be two di
+00000ec0: 6d65 6e73 696f 6e61 6c2e 2229 0a20 2020  mensional.").   
+00000ed0: 2020 2020 2023 2054 4f44 4f3a 2057 6861       # TODO: Wha
+00000ee0: 7427 7320 7468 6520 636f 7272 6563 7420  t's the correct 
+00000ef0: 6f72 6465 722f 6170 7072 6f61 6368 2028  order/approach (
+00000f00: 696e 2074 6865 206e 6f6e 2d73 7175 6172  in the non-squar
+00000f10: 6520 6361 7365 293f 0a20 2020 2020 2020  e case)?.       
+00000f20: 2023 2060 7079 7465 6e73 6f72 2e74 656e   # `pytensor.ten
+00000f30: 736f 722e 6e6c 696e 616c 672e 7465 6e73  sor.nlinalg.tens
+00000f40: 6f72 696e 7660 3f0a 2020 2020 2020 2020  orinv`?.        
+00000f50: 636f 7620 3d20 6d61 7472 6978 5f69 6e76  cov = matrix_inv
+00000f60: 6572 7365 2874 6175 290a 2020 2020 656c  erse(tau).    el
+00000f70: 7365 3a0a 2020 2020 2020 2020 2320 544f  se:.        # TO
+00000f80: 444f 3a20 5768 6174 2773 2074 6865 2063  DO: What's the c
+00000f90: 6f72 7265 6374 206f 7264 6572 2f61 7070  orrect order/app
+00000fa0: 726f 6163 6820 2869 6e20 7468 6520 6e6f  roach (in the no
+00000fb0: 6e2d 7371 7561 7265 2063 6173 6529 3f0a  n-square case)?.
+00000fc0: 2020 2020 2020 2020 6368 6f6c 203d 2070          chol = p
+00000fd0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00000fe0: 6162 6c65 2863 686f 6c29 0a20 2020 2020  able(chol).     
+00000ff0: 2020 2069 6620 6368 6f6c 2e6e 6469 6d20     if chol.ndim 
+00001000: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
+00001010: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00001020: 6f72 2822 6368 6f6c 206d 7573 7420 6265  or("chol must be
+00001030: 2074 776f 2064 696d 656e 7369 6f6e 616c   two dimensional
+00001040: 2e22 290a 2020 2020 2020 2020 636f 7620  .").        cov 
+00001050: 3d20 6368 6f6c 2e64 6f74 2863 686f 6c2e  = chol.dot(chol.
+00001060: 5429 0a0a 2020 2020 7265 7475 726e 2063  T)..    return c
+00001070: 6f76 0a0a 0a64 6566 2071 7561 6464 6973  ov...def quaddis
+00001080: 745f 7061 7273 6528 7661 6c75 652c 206d  t_parse(value, m
+00001090: 752c 2063 6f76 2c20 6d61 745f 7479 7065  u, cov, mat_type
+000010a0: 3d22 636f 7622 293a 0a20 2020 2022 2222  ="cov"):.    """
+000010b0: 436f 6d70 7574 6520 2878 202d 206d 7529  Compute (x - mu)
+000010c0: 2e54 2040 2053 6967 6d61 5e2d 3120 4020  .T @ Sigma^-1 @ 
+000010d0: 2878 202d 206d 7529 2061 6e64 2074 6865  (x - mu) and the
+000010e0: 206c 6f67 6465 7420 6f66 2053 6967 6d61   logdet of Sigma
+000010f0: 2e22 2222 0a20 2020 2069 6620 7661 6c75  .""".    if valu
+00001100: 652e 6e64 696d 203e 2032 206f 7220 7661  e.ndim > 2 or va
+00001110: 6c75 652e 6e64 696d 203d 3d20 303a 0a20  lue.ndim == 0:. 
+00001120: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00001130: 7565 4572 726f 7228 2249 6e76 616c 6964  ueError("Invalid
+00001140: 2064 696d 656e 7369 6f6e 2066 6f72 2076   dimension for v
+00001150: 616c 7565 3a20 2573 2220 2520 7661 6c75  alue: %s" % valu
+00001160: 652e 6e64 696d 290a 2020 2020 6966 2076  e.ndim).    if v
+00001170: 616c 7565 2e6e 6469 6d20 3d3d 2031 3a0a  alue.ndim == 1:.
+00001180: 2020 2020 2020 2020 6f6e 6564 696d 203d          onedim =
+00001190: 2054 7275 650a 2020 2020 2020 2020 7661   True.        va
+000011a0: 6c75 6520 3d20 7661 6c75 655b 4e6f 6e65  lue = value[None
+000011b0: 2c20 3a5d 0a20 2020 2065 6c73 653a 0a20  , :].    else:. 
+000011c0: 2020 2020 2020 206f 6e65 6469 6d20 3d20         onedim = 
+000011d0: 4661 6c73 650a 0a20 2020 2064 656c 7461  False..    delta
+000011e0: 203d 2076 616c 7565 202d 206d 750a 2020   = value - mu.  
+000011f0: 2020 2320 5573 6520 7468 6973 2077 6865    # Use this whe
+00001200: 6e20 5468 6561 6e6f 2335 3930 3820 6973  n Theano#5908 is
+00001210: 2072 656c 6561 7365 642e 0a20 2020 2023   released..    #
+00001220: 2072 6574 7572 6e20 4d76 4e6f 726d 616c   return MvNormal
+00001230: 4c6f 6770 2829 2873 656c 662e 636f 762c  Logp()(self.cov,
+00001240: 2064 656c 7461 290a 2020 2020 6368 6f6c   delta).    chol
+00001250: 5f63 6f76 203d 2063 686f 6c65 736b 7928  _cov = cholesky(
+00001260: 636f 7629 0a20 2020 2069 6620 6d61 745f  cov).    if mat_
+00001270: 7479 7065 2021 3d20 2274 6175 223a 0a20  type != "tau":. 
+00001280: 2020 2020 2020 2064 6973 742c 206c 6f67         dist, log
+00001290: 6465 742c 206f 6b20 3d20 7175 6164 6469  det, ok = quaddi
+000012a0: 7374 5f63 686f 6c28 6465 6c74 612c 2063  st_chol(delta, c
+000012b0: 686f 6c5f 636f 7629 0a20 2020 2065 6c73  hol_cov).    els
+000012c0: 653a 0a20 2020 2020 2020 2064 6973 742c  e:.        dist,
+000012d0: 206c 6f67 6465 742c 206f 6b20 3d20 7175   logdet, ok = qu
+000012e0: 6164 6469 7374 5f74 6175 2864 656c 7461  addist_tau(delta
+000012f0: 2c20 6368 6f6c 5f63 6f76 290a 2020 2020  , chol_cov).    
+00001300: 6966 206f 6e65 6469 6d3a 0a20 2020 2020  if onedim:.     
+00001310: 2020 2072 6574 7572 6e20 6469 7374 5b30     return dist[0
+00001320: 5d2c 206c 6f67 6465 742c 206f 6b0a 0a20  ], logdet, ok.. 
+00001330: 2020 2072 6574 7572 6e20 6469 7374 2c20     return dist, 
+00001340: 6c6f 6764 6574 2c20 6f6b 0a0a 0a64 6566  logdet, ok...def
+00001350: 2071 7561 6464 6973 745f 6368 6f6c 2864   quaddist_chol(d
+00001360: 656c 7461 2c20 6368 6f6c 5f6d 6174 293a  elta, chol_mat):
+00001370: 0a20 2020 2064 6961 6720 3d20 7074 2e64  .    diag = pt.d
+00001380: 6961 6728 6368 6f6c 5f6d 6174 290a 2020  iag(chol_mat).  
+00001390: 2020 2320 4368 6563 6b20 6966 2074 6865    # Check if the
+000013a0: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
+000013b0: 6978 2069 7320 706f 7369 7469 7665 2064  ix is positive d
+000013c0: 6566 696e 6974 652e 0a20 2020 206f 6b20  efinite..    ok 
+000013d0: 3d20 7074 2e61 6c6c 2864 6961 6720 3e20  = pt.all(diag > 
+000013e0: 3029 0a20 2020 2023 2049 6620 6e6f 742c  0).    # If not,
+000013f0: 2072 6570 6c61 6365 2074 6865 2064 6961   replace the dia
+00001400: 676f 6e61 6c2e 2057 6520 7265 7475 726e  gonal. We return
+00001410: 202d 696e 6620 6c61 7465 722c 2062 7574   -inf later, but
+00001420: 0a20 2020 2023 206e 6565 6420 746f 2070  .    # need to p
+00001430: 7265 7665 6e74 2073 6f6c 7665 5f6c 6f77  revent solve_low
+00001440: 6572 2066 726f 6d20 7468 726f 7769 6e67  er from throwing
+00001450: 2061 6e20 6578 6365 7074 696f 6e2e 0a20   an exception.. 
+00001460: 2020 2063 686f 6c5f 636f 7620 3d20 7074     chol_cov = pt
+00001470: 2e73 7769 7463 6828 6f6b 2c20 6368 6f6c  .switch(ok, chol
+00001480: 5f6d 6174 2c20 3129 0a0a 2020 2020 6465  _mat, 1)..    de
+00001490: 6c74 615f 7472 616e 7320 3d20 736f 6c76  lta_trans = solv
+000014a0: 655f 6c6f 7765 7228 6368 6f6c 5f63 6f76  e_lower(chol_cov
+000014b0: 2c20 6465 6c74 612e 5429 2e54 0a20 2020  , delta.T).T.   
+000014c0: 2071 7561 6464 6973 7420 3d20 2864 656c   quaddist = (del
+000014d0: 7461 5f74 7261 6e73 2a2a 3229 2e73 756d  ta_trans**2).sum
+000014e0: 2861 7869 733d 2d31 290a 2020 2020 6c6f  (axis=-1).    lo
+000014f0: 6764 6574 203d 2070 742e 7375 6d28 7074  gdet = pt.sum(pt
+00001500: 2e6c 6f67 2864 6961 6729 290a 2020 2020  .log(diag)).    
+00001510: 7265 7475 726e 2071 7561 6464 6973 742c  return quaddist,
+00001520: 206c 6f67 6465 742c 206f 6b0a 0a0a 6465   logdet, ok...de
+00001530: 6620 7175 6164 6469 7374 5f74 6175 2864  f quaddist_tau(d
+00001540: 656c 7461 2c20 6368 6f6c 5f6d 6174 293a  elta, chol_mat):
+00001550: 0a20 2020 2064 6961 6720 3d20 7074 2e6e  .    diag = pt.n
+00001560: 6c69 6e61 6c67 2e64 6961 6728 6368 6f6c  linalg.diag(chol
+00001570: 5f6d 6174 290a 2020 2020 2320 4368 6563  _mat).    # Chec
+00001580: 6b20 6966 2074 6865 2070 7265 6369 7369  k if the precisi
+00001590: 6f6e 206d 6174 7269 7820 6973 2070 6f73  on matrix is pos
+000015a0: 6974 6976 6520 6465 6669 6e69 7465 2e0a  itive definite..
+000015b0: 2020 2020 6f6b 203d 2070 742e 616c 6c28      ok = pt.all(
+000015c0: 6469 6167 203e 2030 290a 2020 2020 2320  diag > 0).    # 
+000015d0: 4966 206e 6f74 2c20 7265 706c 6163 6520  If not, replace 
+000015e0: 7468 6520 6469 6167 6f6e 616c 2e20 5765  the diagonal. We
+000015f0: 2072 6574 7572 6e20 2d69 6e66 206c 6174   return -inf lat
+00001600: 6572 2c20 6275 740a 2020 2020 2320 6e65  er, but.    # ne
+00001610: 6564 2074 6f20 7072 6576 656e 7420 736f  ed to prevent so
+00001620: 6c76 655f 6c6f 7765 7220 6672 6f6d 2074  lve_lower from t
+00001630: 6872 6f77 696e 6720 616e 2065 7863 6570  hrowing an excep
+00001640: 7469 6f6e 2e0a 2020 2020 6368 6f6c 5f74  tion..    chol_t
+00001650: 6175 203d 2070 742e 7377 6974 6368 286f  au = pt.switch(o
+00001660: 6b2c 2063 686f 6c5f 6d61 742c 2031 290a  k, chol_mat, 1).
+00001670: 0a20 2020 2064 656c 7461 5f74 7261 6e73  .    delta_trans
+00001680: 203d 2070 742e 646f 7428 6465 6c74 612c   = pt.dot(delta,
+00001690: 2063 686f 6c5f 7461 7529 0a20 2020 2071   chol_tau).    q
+000016a0: 7561 6464 6973 7420 3d20 2864 656c 7461  uaddist = (delta
+000016b0: 5f74 7261 6e73 2a2a 3229 2e73 756d 2861  _trans**2).sum(a
+000016c0: 7869 733d 2d31 290a 2020 2020 6c6f 6764  xis=-1).    logd
+000016d0: 6574 203d 202d 7074 2e73 756d 2870 742e  et = -pt.sum(pt.
+000016e0: 6c6f 6728 6469 6167 2929 0a20 2020 2072  log(diag)).    r
+000016f0: 6574 7572 6e20 7175 6164 6469 7374 2c20  eturn quaddist, 
+00001700: 6c6f 6764 6574 2c20 6f6b 0a0a 0a63 6c61  logdet, ok...cla
+00001710: 7373 204d 764e 6f72 6d61 6c28 436f 6e74  ss MvNormal(Cont
+00001720: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
+00001730: 220a 2020 2020 4d75 6c74 6976 6172 6961  ".    Multivaria
+00001740: 7465 206e 6f72 6d61 6c20 6c6f 672d 6c69  te normal log-li
+00001750: 6b65 6c69 686f 6f64 2e0a 0a20 2020 202e  kelihood...    .
+00001760: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
+00001770: 2066 2878 205c 6d69 6420 5c70 692c 2054   f(x \mid \pi, T
+00001780: 2920 3d0a 2020 2020 2020 2020 2020 205c  ) =.           \
+00001790: 6672 6163 7b7c 547c 5e7b 312f 327d 7d7b  frac{|T|^{1/2}}{
+000017a0: 2832 5c70 6929 5e7b 6b2f 327d 7d0a 2020  (2\pi)^{k/2}}.  
+000017b0: 2020 2020 2020 2020 205c 6578 705c 6c65           \exp\le
+000017c0: 6674 5c7b 202d 5c66 7261 637b 317d 7b32  ft\{ -\frac{1}{2
+000017d0: 7d20 2878 2d5c 6d75 295e 7b5c 7072 696d  } (x-\mu)^{\prim
+000017e0: 657d 2054 2028 782d 5c6d 7529 205c 7269  e} T (x-\mu) \ri
+000017f0: 6768 745c 7d0a 0a20 2020 203d 3d3d 3d3d  ght\}..    =====
+00001800: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
+00001810: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00001820: 2020 2020 5375 7070 6f72 7420 2020 3a6d      Support   :m
+00001830: 6174 683a 6078 205c 696e 205c 6d61 7468  ath:`x \in \math
+00001840: 6262 7b52 7d5e 6b60 0a20 2020 204d 6561  bb{R}^k`.    Mea
+00001850: 6e20 2020 2020 203a 6d61 7468 3a60 5c6d  n      :math:`\m
+00001860: 7560 0a20 2020 2056 6172 6961 6e63 6520  u`.    Variance 
+00001870: 203a 6d61 7468 3a60 545e 7b2d 317d 600a   :math:`T^{-1}`.
+00001880: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
+00001890: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000018a0: 3d3d 3d3d 3d3d 3d3d 0a0a 2020 2020 5061  ========..    Pa
+000018b0: 7261 6d65 7465 7273 0a20 2020 202d 2d2d  rameters.    ---
+000018c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 6d75 203a  -------.    mu :
+000018d0: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
+000018e0: 666c 6f61 740a 2020 2020 2020 2020 5665  float.        Ve
+000018f0: 6374 6f72 206f 6620 6d65 616e 732e 0a20  ctor of means.. 
+00001900: 2020 2063 6f76 203a 2074 656e 736f 725f     cov : tensor_
+00001910: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
+00001920: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00001930: 436f 7661 7269 616e 6365 206d 6174 7269  Covariance matri
+00001940: 782e 2045 7861 6374 6c79 206f 6e65 206f  x. Exactly one o
+00001950: 6620 636f 762c 2074 6175 2c20 6f72 2063  f cov, tau, or c
+00001960: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
+00001970: 2020 2074 6175 203a 2074 656e 736f 725f     tau : tensor_
+00001980: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
+00001990: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+000019a0: 5072 6563 6973 696f 6e20 6d61 7472 6978  Precision matrix
+000019b0: 2e20 4578 6163 746c 7920 6f6e 6520 6f66  . Exactly one of
+000019c0: 2063 6f76 2c20 7461 752c 206f 7220 6368   cov, tau, or ch
+000019d0: 6f6c 2069 7320 6e65 6564 6564 2e0a 2020  ol is needed..  
+000019e0: 2020 6368 6f6c 203a 2074 656e 736f 725f    chol : tensor_
+000019f0: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
+00001a00: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00001a10: 4368 6f6c 6573 6b79 2064 6563 6f6d 706f  Cholesky decompo
+00001a20: 7369 7469 6f6e 206f 6620 636f 7661 7269  sition of covari
+00001a30: 616e 6365 206d 6174 7269 782e 2045 7861  ance matrix. Exa
+00001a40: 6374 6c79 206f 6e65 206f 6620 636f 762c  ctly one of cov,
+00001a50: 0a20 2020 2020 2020 2074 6175 2c20 6f72  .        tau, or
+00001a60: 2063 686f 6c20 6973 206e 6565 6465 642e   chol is needed.
+00001a70: 0a20 2020 206c 6f77 6572 3a20 626f 6f6c  .    lower: bool
+00001a80: 2c20 6465 6661 756c 743d 5472 7565 0a20  , default=True. 
+00001a90: 2020 2020 2020 2057 6865 7468 6572 2063         Whether c
+00001aa0: 686f 6c20 6973 2074 6865 206c 6f77 6572  hol is the lower
+00001ab0: 2074 7269 6469 6167 6f6e 616c 2063 686f   tridiagonal cho
+00001ac0: 6c65 736b 7920 6661 6374 6f72 2e0a 0a20  lesky factor... 
+00001ad0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
+00001ae0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6566  --------.    Def
+00001af0: 696e 6520 6120 6d75 6c74 6976 6172 6961  ine a multivaria
+00001b00: 7465 206e 6f72 6d61 6c20 7661 7269 6162  te normal variab
+00001b10: 6c65 2066 6f72 2061 2067 6976 656e 2063  le for a given c
+00001b20: 6f76 6172 6961 6e63 650a 2020 2020 6d61  ovariance.    ma
+00001b30: 7472 6978 3a3a 0a0a 2020 2020 2020 2020  trix::..        
+00001b40: 636f 7620 3d20 6e70 2e61 7272 6179 285b  cov = np.array([
+00001b50: 5b31 2e2c 2030 2e35 5d2c 205b 302e 352c  [1., 0.5], [0.5,
+00001b60: 2032 5d5d 290a 2020 2020 2020 2020 6d75   2]]).        mu
+00001b70: 203d 206e 702e 7a65 726f 7328 3229 0a20   = np.zeros(2). 
+00001b80: 2020 2020 2020 2076 616c 7320 3d20 706d         vals = pm
+00001b90: 2e4d 764e 6f72 6d61 6c28 2776 616c 7327  .MvNormal('vals'
+00001ba0: 2c20 6d75 3d6d 752c 2063 6f76 3d63 6f76  , mu=mu, cov=cov
+00001bb0: 2c20 7368 6170 653d 2835 2c20 3229 290a  , shape=(5, 2)).
+00001bc0: 0a20 2020 204d 6f73 7420 6f66 2074 6865  .    Most of the
+00001bd0: 2074 696d 6520 6974 2069 7320 7072 6566   time it is pref
+00001be0: 6572 6162 6c65 2074 6f20 7370 6563 6966  erable to specif
+00001bf0: 7920 7468 6520 6368 6f6c 6573 6b79 0a20  y the cholesky. 
+00001c00: 2020 2066 6163 746f 7220 6f66 2074 6865     factor of the
+00001c10: 2063 6f76 6172 6961 6e63 6520 696e 7374   covariance inst
+00001c20: 6561 642e 2046 6f72 2065 7861 6d70 6c65  ead. For example
+00001c30: 2c20 7765 2063 6f75 6c64 0a20 2020 2066  , we could.    f
+00001c40: 6974 2061 206d 756c 7469 7661 7269 6174  it a multivariat
+00001c50: 6520 6f75 7463 6f6d 6520 6c69 6b65 2074  e outcome like t
+00001c60: 6869 7320 2873 6565 2074 6865 2064 6f63  his (see the doc
+00001c70: 7374 7269 6e67 0a20 2020 206f 6620 604c  string.    of `L
+00001c80: 4b4a 4368 6f6c 6573 6b79 436f 7660 2066  KJCholeskyCov` f
+00001c90: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
+00001ca0: 696f 6e20 6162 6f75 7420 7468 6973 293a  ion about this):
+00001cb0: 3a0a 0a20 2020 2020 2020 206d 7520 3d20  :..        mu = 
+00001cc0: 6e70 2e7a 6572 6f73 2833 290a 2020 2020  np.zeros(3).    
+00001cd0: 2020 2020 7472 7565 5f63 6f76 203d 206e      true_cov = n
+00001ce0: 702e 6172 7261 7928 5b5b 312e 302c 2030  p.array([[1.0, 0
+00001cf0: 2e35 2c20 302e 315d 2c0a 2020 2020 2020  .5, 0.1],.      
+00001d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001d10: 2020 2020 2020 205b 302e 352c 2032 2e30         [0.5, 2.0
+00001d20: 2c20 302e 325d 2c0a 2020 2020 2020 2020  , 0.2],.        
 00001d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d40: 2020 2020 205b 302e 352c 2032 2e30 2c20       [0.5, 2.0, 
-00001d50: 302e 325d 2c0a 2020 2020 2020 2020 2020  0.2],.          
-00001d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001d70: 2020 205b 302e 312c 2030 2e32 2c20 312e     [0.1, 0.2, 1.
-00001d80: 305d 5d29 0a20 2020 2020 2020 2064 6174  0]]).        dat
-00001d90: 6120 3d20 6e70 2e72 616e 646f 6d2e 6d75  a = np.random.mu
-00001da0: 6c74 6976 6172 6961 7465 5f6e 6f72 6d61  ltivariate_norma
-00001db0: 6c28 6d75 2c20 7472 7565 5f63 6f76 2c20  l(mu, true_cov, 
-00001dc0: 3130 290a 0a20 2020 2020 2020 2073 645f  10)..        sd_
-00001dd0: 6469 7374 203d 2070 6d2e 4578 706f 6e65  dist = pm.Expone
-00001de0: 6e74 6961 6c2e 6469 7374 2831 2e30 2c20  ntial.dist(1.0, 
-00001df0: 7368 6170 653d 3329 0a20 2020 2020 2020  shape=3).       
-00001e00: 2063 686f 6c2c 2063 6f72 722c 2073 7464   chol, corr, std
-00001e10: 7320 3d20 706d 2e4c 4b4a 4368 6f6c 6573  s = pm.LKJCholes
-00001e20: 6b79 436f 7628 2763 686f 6c5f 636f 7627  kyCov('chol_cov'
-00001e30: 2c20 6e3d 332c 2065 7461 3d32 2c0a 2020  , n=3, eta=2,.  
-00001e40: 2020 2020 2020 2020 2020 7364 5f64 6973            sd_dis
-00001e50: 743d 7364 5f64 6973 742c 2063 6f6d 7075  t=sd_dist, compu
-00001e60: 7465 5f63 6f72 723d 5472 7565 290a 2020  te_corr=True).  
-00001e70: 2020 2020 2020 7661 6c73 203d 2070 6d2e        vals = pm.
-00001e80: 4d76 4e6f 726d 616c 2827 7661 6c73 272c  MvNormal('vals',
-00001e90: 206d 753d 6d75 2c20 6368 6f6c 3d63 686f   mu=mu, chol=cho
-00001ea0: 6c2c 206f 6273 6572 7665 643d 6461 7461  l, observed=data
-00001eb0: 290a 0a20 2020 2046 6f72 2075 6e6f 6273  )..    For unobs
-00001ec0: 6572 7665 6420 7661 6c75 6573 2069 7420  erved values it 
-00001ed0: 6361 6e20 6265 2062 6574 7465 7220 746f  can be better to
-00001ee0: 2075 7365 2061 206e 6f6e 2d63 656e 7465   use a non-cente
-00001ef0: 7265 640a 2020 2020 7061 7261 6d65 7472  red.    parametr
-00001f00: 697a 6174 696f 6e3a 3a0a 0a20 2020 2020  ization::..     
-00001f10: 2020 2073 645f 6469 7374 203d 2070 6d2e     sd_dist = pm.
-00001f20: 4578 706f 6e65 6e74 6961 6c2e 6469 7374  Exponential.dist
-00001f30: 2831 2e30 2c20 7368 6170 653d 3329 0a20  (1.0, shape=3). 
-00001f40: 2020 2020 2020 2063 686f 6c2c 205f 2c20         chol, _, 
-00001f50: 5f20 3d20 706d 2e4c 4b4a 4368 6f6c 6573  _ = pm.LKJCholes
-00001f60: 6b79 436f 7628 2763 686f 6c5f 636f 7627  kyCov('chol_cov'
-00001f70: 2c20 6e3d 332c 2065 7461 3d32 2c0a 2020  , n=3, eta=2,.  
-00001f80: 2020 2020 2020 2020 2020 7364 5f64 6973            sd_dis
-00001f90: 743d 7364 5f64 6973 742c 2063 6f6d 7075  t=sd_dist, compu
-00001fa0: 7465 5f63 6f72 723d 5472 7565 290a 2020  te_corr=True).  
-00001fb0: 2020 2020 2020 7661 6c73 5f72 6177 203d        vals_raw =
-00001fc0: 2070 6d2e 4e6f 726d 616c 2827 7661 6c73   pm.Normal('vals
-00001fd0: 5f72 6177 272c 206d 753d 302c 2073 6967  _raw', mu=0, sig
-00001fe0: 6d61 3d31 2c20 7368 6170 653d 2835 2c20  ma=1, shape=(5, 
-00001ff0: 3329 290a 2020 2020 2020 2020 7661 6c73  3)).        vals
-00002000: 203d 2070 6d2e 4465 7465 726d 696e 6973   = pm.Determinis
-00002010: 7469 6328 2776 616c 7327 2c20 7074 2e64  tic('vals', pt.d
-00002020: 6f74 2863 686f 6c2c 2076 616c 735f 7261  ot(chol, vals_ra
-00002030: 772e 5429 2e54 290a 2020 2020 2222 220a  w.T).T).    """.
-00002040: 2020 2020 7276 5f6f 7020 3d20 6d75 6c74      rv_op = mult
-00002050: 6976 6172 6961 7465 5f6e 6f72 6d61 6c0a  ivariate_normal.
-00002060: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00002070: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
-00002080: 6c73 2c20 6d75 2c20 636f 763d 4e6f 6e65  ls, mu, cov=None
-00002090: 2c20 7461 753d 4e6f 6e65 2c20 6368 6f6c  , tau=None, chol
-000020a0: 3d4e 6f6e 652c 206c 6f77 6572 3d54 7275  =None, lower=Tru
-000020b0: 652c 202a 2a6b 7761 7267 7329 3a0a 2020  e, **kwargs):.  
-000020c0: 2020 2020 2020 6d75 203d 2070 742e 6173        mu = pt.as
-000020d0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-000020e0: 286d 7529 0a20 2020 2020 2020 2063 6f76  (mu).        cov
-000020f0: 203d 2071 7561 6464 6973 745f 6d61 7472   = quaddist_matr
-00002100: 6978 2863 6f76 2c20 6368 6f6c 2c20 7461  ix(cov, chol, ta
-00002110: 752c 206c 6f77 6572 290a 2020 2020 2020  u, lower).      
-00002120: 2020 2320 5079 5465 6e73 6f72 2069 7320    # PyTensor is 
-00002130: 7374 7269 6374 6572 2061 626f 7574 2074  stricter about t
-00002140: 6865 2073 6861 7065 206f 6620 6d75 2c20  he shape of mu, 
-00002150: 7468 616e 2050 794d 4320 7573 6564 2074  than PyMC used t
-00002160: 6f20 6265 0a20 2020 2020 2020 206d 7520  o be.        mu 
-00002170: 3d20 7074 2e62 726f 6164 6361 7374 5f61  = pt.broadcast_a
-00002180: 7272 6179 7328 6d75 2c20 636f 765b 2e2e  rrays(mu, cov[..
-00002190: 2e2c 202d 315d 295b 305d 0a20 2020 2020  ., -1])[0].     
-000021a0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-000021b0: 292e 6469 7374 285b 6d75 2c20 636f 765d  ).dist([mu, cov]
-000021c0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
-000021d0: 2064 6566 206d 6f6d 656e 7428 7276 2c20   def moment(rv, 
-000021e0: 7369 7a65 2c20 6d75 2c20 636f 7629 3a0a  size, mu, cov):.
-000021f0: 2020 2020 2020 2020 6d6f 6d65 6e74 203d          moment =
-00002200: 206d 750a 2020 2020 2020 2020 6966 206e   mu.        if n
-00002210: 6f74 2072 765f 7369 7a65 5f69 735f 6e6f  ot rv_size_is_no
-00002220: 6e65 2873 697a 6529 3a0a 2020 2020 2020  ne(size):.      
-00002230: 2020 2020 2020 6d6f 6d65 6e74 5f73 697a        moment_siz
-00002240: 6520 3d20 7074 2e63 6f6e 6361 7465 6e61  e = pt.concatena
-00002250: 7465 285b 7369 7a65 2c20 5b6d 752e 7368  te([size, [mu.sh
-00002260: 6170 655b 2d31 5d5d 5d29 0a20 2020 2020  ape[-1]]]).     
-00002270: 2020 2020 2020 206d 6f6d 656e 7420 3d20         moment = 
-00002280: 7074 2e66 756c 6c28 6d6f 6d65 6e74 5f73  pt.full(moment_s
-00002290: 697a 652c 206d 7529 0a20 2020 2020 2020  ize, mu).       
-000022a0: 2072 6574 7572 6e20 6d6f 6d65 6e74 0a0a   return moment..
-000022b0: 2020 2020 6465 6620 6c6f 6770 2876 616c      def logp(val
-000022c0: 7565 2c20 6d75 2c20 636f 7629 3a0a 2020  ue, mu, cov):.  
-000022d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000022e0: 2020 4361 6c63 756c 6174 6520 6c6f 672d    Calculate log-
-000022f0: 7072 6f62 6162 696c 6974 7920 6f66 204d  probability of M
-00002300: 756c 7469 7661 7269 6174 6520 4e6f 726d  ultivariate Norm
-00002310: 616c 2064 6973 7472 6962 7574 696f 6e0a  al distribution.
-00002320: 2020 2020 2020 2020 6174 2073 7065 6369          at speci
-00002330: 6669 6564 2076 616c 7565 2e0a 0a20 2020  fied value...   
-00002340: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00002350: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-00002360: 2d2d 0a20 2020 2020 2020 2076 616c 7565  --.        value
-00002370: 3a20 6e75 6d65 7269 630a 2020 2020 2020  : numeric.      
-00002380: 2020 2020 2020 5661 6c75 6520 666f 7220        Value for 
-00002390: 7768 6963 6820 6c6f 672d 7072 6f62 6162  which log-probab
-000023a0: 696c 6974 7920 6973 2063 616c 6375 6c61  ility is calcula
-000023b0: 7465 642e 0a0a 2020 2020 2020 2020 5265  ted...        Re
-000023c0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-000023d0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5465  -----.        Te
-000023e0: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
-000023f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00002400: 2071 7561 6464 6973 742c 206c 6f67 6465   quaddist, logde
-00002410: 742c 206f 6b20 3d20 7175 6164 6469 7374  t, ok = quaddist
-00002420: 5f70 6172 7365 2876 616c 7565 2c20 6d75  _parse(value, mu
-00002430: 2c20 636f 7629 0a20 2020 2020 2020 206b  , cov).        k
-00002440: 203d 2066 6c6f 6174 5828 7661 6c75 652e   = floatX(value.
-00002450: 7368 6170 655b 2d31 5d29 0a20 2020 2020  shape[-1]).     
-00002460: 2020 206e 6f72 6d20 3d20 2d30 2e35 202a     norm = -0.5 *
-00002470: 206b 202a 2070 6d2e 666c 6f61 7458 286e   k * pm.floatX(n
-00002480: 702e 6c6f 6728 3220 2a20 6e70 2e70 6929  p.log(2 * np.pi)
-00002490: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000024a0: 2063 6865 636b 5f70 6172 616d 6574 6572   check_parameter
-000024b0: 7328 0a20 2020 2020 2020 2020 2020 206e  s(.            n
-000024c0: 6f72 6d20 2d20 302e 3520 2a20 7175 6164  orm - 0.5 * quad
-000024d0: 6469 7374 202d 206c 6f67 6465 742c 0a20  dist - logdet,. 
-000024e0: 2020 2020 2020 2020 2020 206f 6b2c 0a20             ok,. 
-000024f0: 2020 2020 2020 2020 2020 206d 7367 3d22             msg="
-00002500: 706f 7364 6566 222c 0a20 2020 2020 2020  posdef",.       
-00002510: 2029 0a0a 0a63 6c61 7373 204d 7653 7475   )...class MvStu
-00002520: 6465 6e74 5452 5628 5261 6e64 6f6d 5661  dentTRV(RandomVa
-00002530: 7269 6162 6c65 293a 0a20 2020 206e 616d  riable):.    nam
-00002540: 6520 3d20 226d 756c 7469 7661 7269 6174  e = "multivariat
-00002550: 655f 7374 7564 656e 7474 220a 2020 2020  e_studentt".    
-00002560: 6e64 696d 5f73 7570 7020 3d20 310a 2020  ndim_supp = 1.  
-00002570: 2020 6e64 696d 735f 7061 7261 6d73 203d    ndims_params =
-00002580: 205b 302c 2031 2c20 325d 0a20 2020 2064   [0, 1, 2].    d
-00002590: 7479 7065 203d 2022 666c 6f61 7458 220a  type = "floatX".
-000025a0: 2020 2020 5f70 7269 6e74 5f6e 616d 6520      _print_name 
-000025b0: 3d20 2822 4d76 5374 7564 656e 7454 222c  = ("MvStudentT",
-000025c0: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-000025d0: 7b4d 7653 7475 6465 6e74 547d 2229 0a0a  {MvStudentT}")..
-000025e0: 2020 2020 6465 6620 6d61 6b65 5f6e 6f64      def make_nod
-000025f0: 6528 7365 6c66 2c20 726e 672c 2073 697a  e(self, rng, siz
-00002600: 652c 2064 7479 7065 2c20 6e75 2c20 6d75  e, dtype, nu, mu
-00002610: 2c20 636f 7629 3a0a 2020 2020 2020 2020  , cov):.        
-00002620: 6e75 203d 2070 742e 6173 5f74 656e 736f  nu = pt.as_tenso
-00002630: 725f 7661 7269 6162 6c65 286e 7529 0a20  r_variable(nu). 
-00002640: 2020 2020 2020 2069 6620 6e6f 7420 6e75         if not nu
-00002650: 2e6e 6469 6d20 3d3d 2030 3a0a 2020 2020  .ndim == 0:.    
-00002660: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00002670: 6c75 6545 7272 6f72 2822 6e75 206d 7573  lueError("nu mus
-00002680: 7420 6265 2061 2073 6361 6c61 7220 286e  t be a scalar (n
-00002690: 6469 6d3d 3029 2e22 290a 0a20 2020 2020  dim=0).")..     
-000026a0: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
-000026b0: 292e 6d61 6b65 5f6e 6f64 6528 726e 672c  ).make_node(rng,
-000026c0: 2073 697a 652c 2064 7479 7065 2c20 6e75   size, dtype, nu
-000026d0: 2c20 6d75 2c20 636f 7629 0a0a 2020 2020  , mu, cov)..    
-000026e0: 6465 6620 5f5f 6361 6c6c 5f5f 2873 656c  def __call__(sel
-000026f0: 662c 206e 752c 206d 753d 4e6f 6e65 2c20  f, nu, mu=None, 
-00002700: 636f 763d 4e6f 6e65 2c20 7369 7a65 3d4e  cov=None, size=N
-00002710: 6f6e 652c 202a 2a6b 7761 7267 7329 3a0a  one, **kwargs):.
-00002720: 2020 2020 2020 2020 6474 7970 6520 3d20          dtype = 
-00002730: 7079 7465 6e73 6f72 2e63 6f6e 6669 672e  pytensor.config.
-00002740: 666c 6f61 7458 2069 6620 7365 6c66 2e64  floatX if self.d
-00002750: 7479 7065 203d 3d20 2266 6c6f 6174 5822  type == "floatX"
-00002760: 2065 6c73 6520 7365 6c66 2e64 7479 7065   else self.dtype
-00002770: 0a0a 2020 2020 2020 2020 6966 206d 7520  ..        if mu 
-00002780: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00002790: 2020 2020 206d 7520 3d20 6e70 2e61 7272       mu = np.arr
-000027a0: 6179 285b 302e 305d 2c20 6474 7970 653d  ay([0.0], dtype=
-000027b0: 6474 7970 6529 0a20 2020 2020 2020 2069  dtype).        i
-000027c0: 6620 636f 7620 6973 204e 6f6e 653a 0a20  f cov is None:. 
-000027d0: 2020 2020 2020 2020 2020 2063 6f76 203d             cov =
-000027e0: 206e 702e 6172 7261 7928 5b5b 312e 305d   np.array([[1.0]
-000027f0: 5d2c 2064 7479 7065 3d64 7479 7065 290a  ], dtype=dtype).
-00002800: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00002810: 7570 6572 2829 2e5f 5f63 616c 6c5f 5f28  uper().__call__(
-00002820: 6e75 2c20 6d75 2c20 636f 762c 2073 697a  nu, mu, cov, siz
-00002830: 653d 7369 7a65 2c20 2a2a 6b77 6172 6773  e=size, **kwargs
-00002840: 290a 0a20 2020 2064 6566 205f 7375 7070  )..    def _supp
-00002850: 5f73 6861 7065 5f66 726f 6d5f 7061 7261  _shape_from_para
-00002860: 6d73 2873 656c 662c 2064 6973 745f 7061  ms(self, dist_pa
-00002870: 7261 6d73 2c20 7265 705f 7061 7261 6d5f  rams, rep_param_
-00002880: 6964 783d 312c 2070 6172 616d 5f73 6861  idx=1, param_sha
-00002890: 7065 733d 4e6f 6e65 293a 0a20 2020 2020  pes=None):.     
-000028a0: 2020 2072 6574 7572 6e20 6465 6661 756c     return defaul
-000028b0: 745f 7375 7070 5f73 6861 7065 5f66 726f  t_supp_shape_fro
-000028c0: 6d5f 7061 7261 6d73 280a 2020 2020 2020  m_params(.      
-000028d0: 2020 2020 2020 7365 6c66 2e6e 6469 6d5f        self.ndim_
-000028e0: 7375 7070 2c20 6469 7374 5f70 6172 616d  supp, dist_param
-000028f0: 732c 2072 6570 5f70 6172 616d 5f69 6478  s, rep_param_idx
-00002900: 2c20 7061 7261 6d5f 7368 6170 6573 0a20  , param_shapes. 
-00002910: 2020 2020 2020 2029 0a0a 2020 2020 4063         )..    @c
-00002920: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00002930: 6566 2072 6e67 5f66 6e28 636c 732c 2072  ef rng_fn(cls, r
-00002940: 6e67 2c20 6e75 2c20 6d75 2c20 636f 762c  ng, nu, mu, cov,
-00002950: 2073 697a 6529 3a0a 2020 2020 2020 2020   size):.        
-00002960: 6d76 5f73 616d 706c 6573 203d 206d 756c  mv_samples = mul
-00002970: 7469 7661 7269 6174 655f 6e6f 726d 616c  tivariate_normal
-00002980: 2e72 6e67 5f66 6e28 726e 673d 726e 672c  .rng_fn(rng=rng,
-00002990: 206d 6561 6e3d 6e70 2e7a 6572 6f73 5f6c   mean=np.zeros_l
-000029a0: 696b 6528 6d75 292c 2063 6f76 3d63 6f76  ike(mu), cov=cov
-000029b0: 2c20 7369 7a65 3d73 697a 6529 0a0a 2020  , size=size)..  
-000029c0: 2020 2020 2020 2320 5461 6b65 2063 6869        # Take chi
-000029d0: 3220 6472 6177 7320 616e 6420 6164 6420  2 draws and add 
-000029e0: 616e 2061 7869 7320 6f66 206c 656e 6774  an axis of lengt
-000029f0: 6820 3120 746f 2074 6865 2072 6967 6874  h 1 to the right
-00002a00: 2066 6f72 2063 6f72 7265 6374 2062 726f   for correct bro
-00002a10: 6164 6361 7374 696e 6720 6265 6c6f 770a  adcasting below.
-00002a20: 2020 2020 2020 2020 6368 6932 5f73 616d          chi2_sam
-00002a30: 706c 6573 203d 206e 702e 7371 7274 2872  ples = np.sqrt(r
-00002a40: 6e67 2e63 6869 7371 7561 7265 286e 752c  ng.chisquare(nu,
-00002a50: 2073 697a 653d 7369 7a65 2920 2f20 6e75   size=size) / nu
-00002a60: 295b 2e2e 2e2c 204e 6f6e 655d 0a0a 2020  )[..., None]..  
-00002a70: 2020 2020 2020 6966 2073 697a 653a 0a20        if size:. 
-00002a80: 2020 2020 2020 2020 2020 206d 7520 3d20             mu = 
-00002a90: 6e70 2e62 726f 6164 6361 7374 5f74 6f28  np.broadcast_to(
-00002aa0: 6d75 2c20 7369 7a65 202b 2028 6d75 2e73  mu, size + (mu.s
-00002ab0: 6861 7065 5b2d 315d 2c29 290a 0a20 2020  hape[-1],))..   
-00002ac0: 2020 2020 2072 6574 7572 6e20 286d 765f       return (mv_
-00002ad0: 7361 6d70 6c65 7320 2f20 6368 6932 5f73  samples / chi2_s
-00002ae0: 616d 706c 6573 2920 2b20 6d75 0a0a 0a6d  amples) + mu...m
-00002af0: 765f 7374 7564 656e 7474 203d 204d 7653  v_studentt = MvS
-00002b00: 7475 6465 6e74 5452 5628 290a 0a0a 636c  tudentTRV()...cl
-00002b10: 6173 7320 4d76 5374 7564 656e 7454 2843  ass MvStudentT(C
-00002b20: 6f6e 7469 6e75 6f75 7329 3a0a 2020 2020  ontinuous):.    
-00002b30: 7222 2222 0a20 2020 204d 756c 7469 7661  r""".    Multiva
-00002b40: 7269 6174 6520 5374 7564 656e 742d 5420  riate Student-T 
-00002b50: 6c6f 672d 6c69 6b65 6c69 686f 6f64 2e0a  log-likelihood..
-00002b60: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a20  .    .. math::. 
-00002b70: 2020 2020 2020 2066 285c 6d61 7468 6266         f(\mathbf
-00002b80: 7b78 7d7c 205c 6e75 2c5c 6d75 2c5c 5369  {x}| \nu,\mu,\Si
-00002b90: 676d 6129 203d 0a20 2020 2020 2020 205c  gma) =.        \
-00002ba0: 6672 6163 0a20 2020 2020 2020 2020 2020  frac.           
-00002bb0: 207b 5c47 616d 6d61 5c6c 6566 745b 285c   {\Gamma\left[(\
-00002bc0: 6e75 2b70 292f 325c 7269 6768 745d 7d0a  nu+p)/2\right]}.
-00002bd0: 2020 2020 2020 2020 2020 2020 7b5c 4761              {\Ga
-00002be0: 6d6d 6128 5c6e 752f 3229 5c6e 755e 7b70  mma(\nu/2)\nu^{p
-00002bf0: 2f32 7d5c 7069 5e7b 702f 327d 0a20 2020  /2}\pi^{p/2}.   
-00002c00: 2020 2020 2020 2020 2020 5c6c 6566 747c            \left|
-00002c10: 7b5c 5369 676d 617d 5c72 6967 6874 7c5e  {\Sigma}\right|^
-00002c20: 7b31 2f32 7d0a 2020 2020 2020 2020 2020  {1/2}.          
-00002c30: 2020 205c 6c65 6674 5b0a 2020 2020 2020     \left[.      
-00002c40: 2020 2020 2020 2020 2031 2b5c 6672 6163           1+\frac
-00002c50: 7b31 7d7b 5c6e 757d 0a20 2020 2020 2020  {1}{\nu}.       
-00002c60: 2020 2020 2020 2020 287b 5c6d 6174 6862          ({\mathb
-00002c70: 6620 787d 2d7b 5c6d 757d 295e 540a 2020  f x}-{\mu})^T.  
-00002c80: 2020 2020 2020 2020 2020 2020 207b 5c53               {\S
-00002c90: 6967 6d61 7d5e 7b2d 317d 287b 5c6d 6174  igma}^{-1}({\mat
-00002ca0: 6862 6620 787d 2d7b 5c6d 757d 290a 2020  hbf x}-{\mu}).  
-00002cb0: 2020 2020 2020 2020 2020 205c 7269 6768             \righ
-00002cc0: 745d 5e7b 2d28 5c6e 752b 7029 2f32 7d7d  t]^{-(\nu+p)/2}}
-00002cd0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  ..    ========  
-00002ce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002cf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002d00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
-00002d10: 2020 5375 7070 6f72 7420 2020 3a6d 6174    Support   :mat
-00002d20: 683a 6078 205c 696e 205c 6d61 7468 6262  h:`x \in \mathbb
-00002d30: 7b52 7d5e 7060 0a20 2020 204d 6561 6e20  {R}^p`.    Mean 
-00002d40: 2020 2020 203a 6d61 7468 3a60 5c6d 7560       :math:`\mu`
-00002d50: 2069 6620 3a6d 6174 683a 605c 6e75 203e   if :math:`\nu >
-00002d60: 2031 6020 656c 7365 2075 6e64 6566 696e   1` else undefin
-00002d70: 6564 0a20 2020 2056 6172 6961 6e63 6520  ed.    Variance 
-00002d80: 203a 6d61 7468 3a60 5c66 7261 637b 5c6e   :math:`\frac{\n
-00002d90: 757d 7b5c 6d75 2d32 7d5c 5369 676d 6160  u}{\mu-2}\Sigma`
-00002da0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002db0: 2020 2069 6620 3a6d 6174 683a 605c 6e75     if :math:`\nu
-00002dc0: 3e32 6020 656c 7365 2075 6e64 6566 696e  >2` else undefin
-00002dd0: 6564 0a20 2020 203d 3d3d 3d3d 3d3d 3d20  ed.    ======== 
-00002de0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00002df0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00002e00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  ==============..
-00002e10: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
-00002e20: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00002e30: 2020 6e75 203a 2074 656e 736f 725f 6c69    nu : tensor_li
-00002e40: 6b65 206f 6620 666c 6f61 740a 2020 2020  ke of float.    
-00002e50: 2020 2020 4465 6772 6565 7320 6f66 2066      Degrees of f
-00002e60: 7265 6564 6f6d 2c20 7368 6f75 6c64 2062  reedom, should b
-00002e70: 6520 6120 706f 7369 7469 7665 2073 6361  e a positive sca
-00002e80: 6c61 722e 0a20 2020 2053 6967 6d61 203a  lar..    Sigma :
-00002e90: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-00002ea0: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
-00002eb0: 2020 2020 2020 2020 5363 616c 6520 6d61          Scale ma
-00002ec0: 7472 6978 2e20 5573 6520 6073 6361 6c65  trix. Use `scale
-00002ed0: 6020 696e 206e 6577 2063 6f64 652e 0a20  ` in new code.. 
-00002ee0: 2020 206d 7520 3a20 7465 6e73 6f72 5f6c     mu : tensor_l
-00002ef0: 696b 6520 6f66 2066 6c6f 6174 2c20 6f70  ike of float, op
-00002f00: 7469 6f6e 616c 0a20 2020 2020 2020 2056  tional.        V
-00002f10: 6563 746f 7220 6f66 206d 6561 6e73 2e0a  ector of means..
-00002f20: 2020 2020 7363 616c 6520 3a20 7465 6e73      scale : tens
-00002f30: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-00002f40: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-00002f50: 2020 2054 6865 2073 6361 6c65 206d 6174     The scale mat
-00002f60: 7269 782e 0a20 2020 2074 6175 203a 2074  rix..    tau : t
-00002f70: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-00002f80: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-00002f90: 2020 2020 2020 5468 6520 7072 6563 6973        The precis
-00002fa0: 696f 6e20 6d61 7472 6978 2e0a 2020 2020  ion matrix..    
-00002fb0: 6368 6f6c 203a 2074 656e 736f 725f 6c69  chol : tensor_li
-00002fc0: 6b65 206f 6620 666c 6f61 742c 206f 7074  ke of float, opt
-00002fd0: 696f 6e61 6c0a 2020 2020 2020 2020 5468  ional.        Th
-00002fe0: 6520 6368 6f6c 6573 6b79 2066 6163 746f  e cholesky facto
-00002ff0: 7220 6f66 2074 6865 2073 6361 6c65 206d  r of the scale m
-00003000: 6174 7269 782e 0a20 2020 206c 6f77 6572  atrix..    lower
-00003010: 203a 2062 6f6f 6c2c 2064 6566 6175 6c74   : bool, default
-00003020: 3d54 7275 650a 2020 2020 2020 2020 5768  =True.        Wh
-00003030: 6574 6865 7220 7468 6520 6368 6f6c 6573  ether the choles
-00003040: 6b79 2066 6174 636f 7220 6973 2067 6976  ky fatcor is giv
-00003050: 656e 2061 7320 6120 6c6f 7765 7220 7472  en as a lower tr
-00003060: 6961 6e67 756c 6172 206d 6174 7269 782e  iangular matrix.
-00003070: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
-00003080: 6f70 203d 206d 765f 7374 7564 656e 7474  op = mv_studentt
-00003090: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-000030a0: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
-000030b0: 636c 732c 206e 752c 2053 6967 6d61 3d4e  cls, nu, Sigma=N
-000030c0: 6f6e 652c 206d 753d 4e6f 6e65 2c20 7363  one, mu=None, sc
-000030d0: 616c 653d 4e6f 6e65 2c20 7461 753d 4e6f  ale=None, tau=No
-000030e0: 6e65 2c20 6368 6f6c 3d4e 6f6e 652c 206c  ne, chol=None, l
-000030f0: 6f77 6572 3d54 7275 652c 202a 2a6b 7761  ower=True, **kwa
-00003100: 7267 7329 3a0a 2020 2020 2020 2020 636f  rgs):.        co
-00003110: 7620 3d20 6b77 6172 6773 2e70 6f70 2822  v = kwargs.pop("
-00003120: 636f 7622 2c20 4e6f 6e65 290a 2020 2020  cov", None).    
-00003130: 2020 2020 6966 2063 6f76 2069 7320 6e6f      if cov is no
-00003140: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00003150: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
-00003160: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
-00003170: 2020 2022 5573 6520 7468 6520 7363 616c     "Use the scal
-00003180: 6520 6172 6775 6d65 6e74 2074 6f20 7370  e argument to sp
-00003190: 6563 6966 7920 7468 6520 7363 616c 6520  ecify the scale 
-000031a0: 6d61 7472 6978 2e20 220a 2020 2020 2020  matrix. ".      
-000031b0: 2020 2020 2020 2020 2020 2263 6f76 2077            "cov w
-000031c0: 696c 6c20 6265 2072 656d 6f76 6564 2069  ill be removed i
-000031d0: 6e20 6675 7475 7265 2076 6572 7369 6f6e  n future version
-000031e0: 732e 222c 0a20 2020 2020 2020 2020 2020  s.",.           
-000031f0: 2020 2020 2046 7574 7572 6557 6172 6e69       FutureWarni
-00003200: 6e67 2c0a 2020 2020 2020 2020 2020 2020  ng,.            
-00003210: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
-00003220: 616c 6520 3d20 636f 760a 2020 2020 2020  ale = cov.      
-00003230: 2020 6966 2053 6967 6d61 2069 7320 6e6f    if Sigma is no
-00003240: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
-00003250: 2020 2020 6966 2073 6361 6c65 2069 7320      if scale is 
-00003260: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00003270: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00003280: 5661 6c75 6545 7272 6f72 2822 5370 6563  ValueError("Spec
-00003290: 6966 7920 6f6e 6c79 206f 6e65 206f 6620  ify only one of 
-000032a0: 7363 616c 6520 616e 6420 5369 676d 6122  scale and Sigma"
-000032b0: 290a 2020 2020 2020 2020 2020 2020 7363  ).            sc
-000032c0: 616c 6520 3d20 5369 676d 610a 2020 2020  ale = Sigma.    
-000032d0: 2020 2020 6e75 203d 2070 742e 6173 5f74      nu = pt.as_t
-000032e0: 656e 736f 725f 7661 7269 6162 6c65 2866  ensor_variable(f
-000032f0: 6c6f 6174 5828 6e75 2929 0a20 2020 2020  loatX(nu)).     
-00003300: 2020 206d 7520 3d20 7074 2e61 735f 7465     mu = pt.as_te
-00003310: 6e73 6f72 5f76 6172 6961 626c 6528 666c  nsor_variable(fl
-00003320: 6f61 7458 286d 7529 290a 2020 2020 2020  oatX(mu)).      
-00003330: 2020 7363 616c 6520 3d20 7175 6164 6469    scale = quaddi
-00003340: 7374 5f6d 6174 7269 7828 7363 616c 652c  st_matrix(scale,
-00003350: 2063 686f 6c2c 2074 6175 2c20 6c6f 7765   chol, tau, lowe
-00003360: 7229 0a20 2020 2020 2020 2023 2050 7954  r).        # PyT
-00003370: 656e 736f 7220 6973 2073 7472 6963 7465  ensor is stricte
-00003380: 7220 6162 6f75 7420 7468 6520 7368 6170  r about the shap
-00003390: 6520 6f66 206d 752c 2074 6861 6e20 5079  e of mu, than Py
-000033a0: 4d43 2075 7365 6420 746f 2062 650a 2020  MC used to be.  
-000033b0: 2020 2020 2020 6d75 203d 2070 742e 6272        mu = pt.br
-000033c0: 6f61 6463 6173 745f 6172 7261 7973 286d  oadcast_arrays(m
-000033d0: 752c 2073 6361 6c65 5b2e 2e2e 2c20 2d31  u, scale[..., -1
-000033e0: 5d29 5b30 5d0a 0a20 2020 2020 2020 2072  ])[0]..        r
-000033f0: 6574 7572 6e20 7375 7065 7228 292e 6469  eturn super().di
-00003400: 7374 285b 6e75 2c20 6d75 2c20 7363 616c  st([nu, mu, scal
-00003410: 655d 2c20 2a2a 6b77 6172 6773 290a 0a20  e], **kwargs).. 
-00003420: 2020 2064 6566 206d 6f6d 656e 7428 7276     def moment(rv
-00003430: 2c20 7369 7a65 2c20 6e75 2c20 6d75 2c20  , size, nu, mu, 
-00003440: 7363 616c 6529 3a0a 2020 2020 2020 2020  scale):.        
-00003450: 6d6f 6d65 6e74 203d 206d 750a 2020 2020  moment = mu.    
-00003460: 2020 2020 6966 206e 6f74 2072 765f 7369      if not rv_si
-00003470: 7a65 5f69 735f 6e6f 6e65 2873 697a 6529  ze_is_none(size)
-00003480: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-00003490: 6d65 6e74 5f73 697a 6520 3d20 7074 2e63  ment_size = pt.c
-000034a0: 6f6e 6361 7465 6e61 7465 285b 7369 7a65  oncatenate([size
-000034b0: 2c20 5b6d 752e 7368 6170 655b 2d31 5d5d  , [mu.shape[-1]]
-000034c0: 5d29 0a20 2020 2020 2020 2020 2020 206d  ]).            m
-000034d0: 6f6d 656e 7420 3d20 7074 2e66 756c 6c28  oment = pt.full(
-000034e0: 6d6f 6d65 6e74 5f73 697a 652c 206d 6f6d  moment_size, mom
-000034f0: 656e 7429 0a20 2020 2020 2020 2072 6574  ent).        ret
-00003500: 7572 6e20 6d6f 6d65 6e74 0a0a 2020 2020  urn moment..    
-00003510: 6465 6620 6c6f 6770 2876 616c 7565 2c20  def logp(value, 
-00003520: 6e75 2c20 6d75 2c20 7363 616c 6529 3a0a  nu, mu, scale):.
-00003530: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003540: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
-00003550: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
-00003560: 204d 756c 7469 7661 7269 6174 6520 5374   Multivariate St
-00003570: 7564 656e 7427 7320 5420 6469 7374 7269  udent's T distri
-00003580: 6275 7469 6f6e 0a20 2020 2020 2020 2061  bution.        a
-00003590: 7420 7370 6563 6966 6965 6420 7661 6c75  t specified valu
-000035a0: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-000035b0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-000035c0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-000035d0: 2020 7661 6c75 653a 206e 756d 6572 6963    value: numeric
-000035e0: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-000035f0: 7565 2066 6f72 2077 6869 6368 206c 6f67  ue for which log
-00003600: 2d70 726f 6261 6269 6c69 7479 2069 7320  -probability is 
-00003610: 6361 6c63 756c 6174 6564 2e0a 0a20 2020  calculated...   
-00003620: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00003630: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00003640: 2020 2020 2054 656e 736f 7256 6172 6961       TensorVaria
-00003650: 626c 650a 2020 2020 2020 2020 2222 220a  ble.        """.
-00003660: 2020 2020 2020 2020 7175 6164 6469 7374          quaddist
-00003670: 2c20 6c6f 6764 6574 2c20 6f6b 203d 2071  , logdet, ok = q
-00003680: 7561 6464 6973 745f 7061 7273 6528 7661  uaddist_parse(va
-00003690: 6c75 652c 206d 752c 2073 6361 6c65 290a  lue, mu, scale).
-000036a0: 2020 2020 2020 2020 6b20 3d20 666c 6f61          k = floa
-000036b0: 7458 2876 616c 7565 2e73 6861 7065 5b2d  tX(value.shape[-
-000036c0: 315d 290a 0a20 2020 2020 2020 206e 6f72  1])..        nor
-000036d0: 6d20 3d20 6761 6d6d 616c 6e28 286e 7520  m = gammaln((nu 
-000036e0: 2b20 6b29 202f 2032 2e30 2920 2d20 6761  + k) / 2.0) - ga
-000036f0: 6d6d 616c 6e28 6e75 202f 2032 2e30 2920  mmaln(nu / 2.0) 
-00003700: 2d20 302e 3520 2a20 6b20 2a20 7074 2e6c  - 0.5 * k * pt.l
-00003710: 6f67 286e 7520 2a20 6e70 2e70 6929 0a20  og(nu * np.pi). 
-00003720: 2020 2020 2020 2069 6e6e 6572 203d 202d         inner = -
-00003730: 286e 7520 2b20 6b29 202f 2032 2e30 202a  (nu + k) / 2.0 *
-00003740: 2070 742e 6c6f 6731 7028 7175 6164 6469   pt.log1p(quaddi
-00003750: 7374 202f 206e 7529 0a20 2020 2020 2020  st / nu).       
-00003760: 2072 6573 203d 206e 6f72 6d20 2b20 696e   res = norm + in
-00003770: 6e65 7220 2d20 6c6f 6764 6574 0a0a 2020  ner - logdet..  
-00003780: 2020 2020 2020 7265 7475 726e 2063 6865        return che
-00003790: 636b 5f70 6172 616d 6574 6572 7328 7265  ck_parameters(re
-000037a0: 732c 206f 6b2c 206e 7520 3e20 302c 206d  s, ok, nu > 0, m
-000037b0: 7367 3d22 706f 7364 6566 2c20 6e75 203e  sg="posdef, nu >
-000037c0: 2030 2229 0a0a 0a63 6c61 7373 2044 6972   0")...class Dir
-000037d0: 6963 686c 6574 2853 696d 706c 6578 436f  ichlet(SimplexCo
-000037e0: 6e74 696e 756f 7573 293a 0a20 2020 2072  ntinuous):.    r
-000037f0: 2222 220a 2020 2020 4469 7269 6368 6c65  """.    Dirichle
-00003800: 7420 6c6f 672d 6c69 6b65 6c69 686f 6f64  t log-likelihood
-00003810: 2e0a 0a20 2020 202e 2e20 6d61 7468 3a3a  ...    .. math::
-00003820: 0a0a 2020 2020 2020 2066 285c 6d61 7468  ..       f(\math
-00003830: 6266 7b78 7d7c 5c6d 6174 6862 667b 617d  bf{x}|\mathbf{a}
-00003840: 2920 3d0a 2020 2020 2020 2020 2020 205c  ) =.           \
-00003850: 6672 6163 7b5c 4761 6d6d 6128 5c73 756d  frac{\Gamma(\sum
-00003860: 5f7b 693d 317d 5e6b 2061 5f69 297d 7b5c  _{i=1}^k a_i)}{\
-00003870: 7072 6f64 5f7b 693d 317d 5e6b 205c 4761  prod_{i=1}^k \Ga
-00003880: 6d6d 6128 615f 6929 7d0a 2020 2020 2020  mma(a_i)}.      
-00003890: 2020 2020 205c 7072 6f64 5f7b 693d 317d       \prod_{i=1}
-000038a0: 5e6b 2078 5f69 5e7b 615f 6920 2d20 317d  ^k x_i^{a_i - 1}
-000038b0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 2020  ..    ========  
-000038c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000038d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000038e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-000038f0: 2020 2020 5375 7070 6f72 7420 2020 3a6d      Support   :m
-00003900: 6174 683a 6078 5f69 205c 696e 2028 302c  ath:`x_i \in (0,
-00003910: 2031 2960 2066 6f72 203a 6d61 7468 3a60   1)` for :math:`
-00003920: 6920 5c69 6e20 5c7b 312c 205c 6c64 6f74  i \in \{1, \ldot
-00003930: 732c 204b 5c7d 600a 2020 2020 2020 2020  s, K\}`.        
-00003940: 2020 2020 2020 7375 6368 2074 6861 7420        such that 
-00003950: 3a6d 6174 683a 605c 7375 6d20 785f 6920  :math:`\sum x_i 
-00003960: 3d20 3160 0a20 2020 204d 6561 6e20 2020  = 1`.    Mean   
-00003970: 2020 203a 6d61 7468 3a60 5c64 6672 6163     :math:`\dfrac
-00003980: 7b61 5f69 7d7b 5c73 756d 2061 5f69 7d60  {a_i}{\sum a_i}`
-00003990: 0a20 2020 2056 6172 6961 6e63 6520 203a  .    Variance  :
-000039a0: 6d61 7468 3a60 5c64 6672 6163 7b61 5f69  math:`\dfrac{a_i
-000039b0: 202d 205c 7375 6d20 615f 307d 7b61 5f30   - \sum a_0}{a_0
-000039c0: 5e32 2028 615f 3020 2b20 3129 7d60 0a20  ^2 (a_0 + 1)}`. 
-000039d0: 2020 2020 2020 2020 2020 2020 2077 6865               whe
-000039e0: 7265 203a 6d61 7468 3a60 615f 3020 3d20  re :math:`a_0 = 
-000039f0: 5c73 756d 2061 5f69 600a 2020 2020 3d3d  \sum a_i`.    ==
-00003a00: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
-00003a10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003a20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00003a30: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
-00003a40: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00003a50: 2d2d 2d2d 2d2d 0a20 2020 2061 203a 2074  ------.    a : t
-00003a60: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-00003a70: 6f61 740a 2020 2020 2020 2020 436f 6e63  oat.        Conc
-00003a80: 656e 7472 6174 696f 6e20 7061 7261 6d65  entration parame
-00003a90: 7465 7273 2028 6120 3e20 3029 2e20 5468  ters (a > 0). Th
-00003aa0: 6520 6e75 6d62 6572 206f 6620 6361 7465  e number of cate
-00003ab0: 676f 7269 6573 2069 7320 6769 7665 6e20  gories is given 
-00003ac0: 6279 2074 6865 0a20 2020 2020 2020 206c  by the.        l
-00003ad0: 656e 6774 6820 6f66 2074 6865 206c 6173  ength of the las
-00003ae0: 7420 6178 6973 2e0a 2020 2020 2222 220a  t axis..    """.
-00003af0: 2020 2020 7276 5f6f 7020 3d20 6469 7269      rv_op = diri
-00003b00: 6368 6c65 740a 0a20 2020 2040 636c 6173  chlet..    @clas
-00003b10: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00003b20: 6469 7374 2863 6c73 2c20 612c 202a 2a6b  dist(cls, a, **k
-00003b30: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00003b40: 6120 3d20 7074 2e61 735f 7465 6e73 6f72  a = pt.as_tensor
-00003b50: 5f76 6172 6961 626c 6528 6129 0a20 2020  _variable(a).   
-00003b60: 2020 2020 2023 206d 6561 6e20 3d20 6120       # mean = a 
-00003b70: 2f20 7074 2e73 756d 2861 290a 2020 2020  / pt.sum(a).    
-00003b80: 2020 2020 2320 6d6f 6465 203d 2070 742e      # mode = pt.
-00003b90: 7377 6974 6368 2870 742e 616c 6c28 6120  switch(pt.all(a 
-00003ba0: 3e20 3129 2c20 2861 202d 2031 2920 2f20  > 1), (a - 1) / 
-00003bb0: 7074 2e73 756d 2861 202d 2031 292c 206e  pt.sum(a - 1), n
-00003bc0: 702e 6e61 6e29 0a0a 2020 2020 2020 2020  p.nan)..        
-00003bd0: 7265 7475 726e 2073 7570 6572 2829 2e64  return super().d
-00003be0: 6973 7428 5b61 5d2c 202a 2a6b 7761 7267  ist([a], **kwarg
-00003bf0: 7329 0a0a 2020 2020 6465 6620 6d6f 6d65  s)..    def mome
-00003c00: 6e74 2872 762c 2073 697a 652c 2061 293a  nt(rv, size, a):
-00003c10: 0a20 2020 2020 2020 206e 6f72 6d5f 636f  .        norm_co
-00003c20: 6e73 7461 6e74 203d 2070 742e 7375 6d28  nstant = pt.sum(
-00003c30: 612c 2061 7869 733d 2d31 295b 2e2e 2e2c  a, axis=-1)[...,
-00003c40: 204e 6f6e 655d 0a20 2020 2020 2020 206d   None].        m
-00003c50: 6f6d 656e 7420 3d20 6120 2f20 6e6f 726d  oment = a / norm
-00003c60: 5f63 6f6e 7374 616e 740a 2020 2020 2020  _constant.      
-00003c70: 2020 6966 206e 6f74 2072 765f 7369 7a65    if not rv_size
-00003c80: 5f69 735f 6e6f 6e65 2873 697a 6529 3a0a  _is_none(size):.
-00003c90: 2020 2020 2020 2020 2020 2020 6d6f 6d65              mome
-00003ca0: 6e74 203d 2070 742e 6675 6c6c 2870 742e  nt = pt.full(pt.
-00003cb0: 636f 6e63 6174 656e 6174 6528 5b73 697a  concatenate([siz
-00003cc0: 652c 205b 612e 7368 6170 655b 2d31 5d5d  e, [a.shape[-1]]
-00003cd0: 5d29 2c20 6d6f 6d65 6e74 290a 2020 2020  ]), moment).    
-00003ce0: 2020 2020 7265 7475 726e 206d 6f6d 656e      return momen
-00003cf0: 740a 0a20 2020 2064 6566 206c 6f67 7028  t..    def logp(
-00003d00: 7661 6c75 652c 2061 293a 0a20 2020 2020  value, a):.     
-00003d10: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-00003d20: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
-00003d30: 6261 6269 6c69 7479 206f 6620 4469 7269  bability of Diri
-00003d40: 6368 6c65 7420 6469 7374 7269 6275 7469  chlet distributi
-00003d50: 6f6e 0a20 2020 2020 2020 2061 7420 7370  on.        at sp
-00003d60: 6563 6966 6965 6420 7661 6c75 652e 0a0a  ecified value...
-00003d70: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-00003d80: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-00003d90: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
-00003da0: 6c75 653a 206e 756d 6572 6963 0a20 2020  lue: numeric.   
-00003db0: 2020 2020 2020 2020 2056 616c 7565 2066           Value f
-00003dc0: 6f72 2077 6869 6368 206c 6f67 2d70 726f  or which log-pro
-00003dd0: 6261 6269 6c69 7479 2069 7320 6361 6c63  bability is calc
-00003de0: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
-00003df0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00003e00: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00003e10: 2054 656e 736f 7256 6172 6961 626c 650a   TensorVariable.
-00003e20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003e30: 2020 2020 2320 6f6e 6c79 2064 6566 696e      # only defin
-00003e40: 6564 2066 6f72 2073 756d 2876 616c 7565  ed for sum(value
-00003e50: 2920 3d3d 2031 0a20 2020 2020 2020 2072  ) == 1.        r
-00003e60: 6573 203d 2070 742e 7375 6d28 6c6f 6770  es = pt.sum(logp
-00003e70: 6f77 2876 616c 7565 2c20 6120 2d20 3129  ow(value, a - 1)
-00003e80: 202d 2067 616d 6d61 6c6e 2861 292c 2061   - gammaln(a), a
-00003e90: 7869 733d 2d31 2920 2b20 6761 6d6d 616c  xis=-1) + gammal
-00003ea0: 6e28 7074 2e73 756d 2861 2c20 6178 6973  n(pt.sum(a, axis
-00003eb0: 3d2d 3129 290a 2020 2020 2020 2020 7265  =-1)).        re
-00003ec0: 7320 3d20 7074 2e73 7769 7463 6828 0a20  s = pt.switch(. 
-00003ed0: 2020 2020 2020 2020 2020 2070 742e 6f72             pt.or
-00003ee0: 5f28 0a20 2020 2020 2020 2020 2020 2020  _(.             
-00003ef0: 2020 2070 742e 616e 7928 7074 2e6c 7428     pt.any(pt.lt(
-00003f00: 7661 6c75 652c 2030 292c 2061 7869 733d  value, 0), axis=
-00003f10: 2d31 292c 0a20 2020 2020 2020 2020 2020  -1),.           
-00003f20: 2020 2020 2070 742e 616e 7928 7074 2e67       pt.any(pt.g
-00003f30: 7428 7661 6c75 652c 2031 292c 2061 7869  t(value, 1), axi
-00003f40: 733d 2d31 292c 0a20 2020 2020 2020 2020  s=-1),.         
-00003f50: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00003f60: 2020 2d6e 702e 696e 662c 0a20 2020 2020    -np.inf,.     
-00003f70: 2020 2020 2020 2072 6573 2c0a 2020 2020         res,.    
-00003f80: 2020 2020 290a 2020 2020 2020 2020 7265      ).        re
-00003f90: 7475 726e 2063 6865 636b 5f70 6172 616d  turn check_param
-00003fa0: 6574 6572 7328 0a20 2020 2020 2020 2020  eters(.         
-00003fb0: 2020 2072 6573 2c0a 2020 2020 2020 2020     res,.        
-00003fc0: 2020 2020 6120 3e20 302c 0a20 2020 2020      a > 0,.     
-00003fd0: 2020 2020 2020 206d 7367 3d22 6120 3e20         msg="a > 
-00003fe0: 3022 2c0a 2020 2020 2020 2020 290a 0a0a  0",.        )...
-00003ff0: 636c 6173 7320 4d75 6c74 696e 6f6d 6961  class Multinomia
-00004000: 6c28 4469 7363 7265 7465 293a 0a20 2020  l(Discrete):.   
-00004010: 2072 2222 220a 2020 2020 4d75 6c74 696e   r""".    Multin
-00004020: 6f6d 6961 6c20 6c6f 672d 6c69 6b65 6c69  omial log-likeli
-00004030: 686f 6f64 2e0a 0a20 2020 2047 656e 6572  hood...    Gener
-00004040: 616c 697a 6573 2062 696e 6f6d 6961 6c20  alizes binomial 
-00004050: 6469 7374 7269 6275 7469 6f6e 2c20 6275  distribution, bu
-00004060: 7420 696e 7374 6561 6420 6f66 2065 6163  t instead of eac
-00004070: 6820 7472 6961 6c20 7265 7375 6c74 696e  h trial resultin
-00004080: 670a 2020 2020 696e 2022 7375 6363 6573  g.    in "succes
-00004090: 7322 206f 7220 2266 6169 6c75 7265 222c  s" or "failure",
-000040a0: 2065 6163 6820 6f6e 6520 7265 7375 6c74   each one result
-000040b0: 7320 696e 2065 7861 6374 6c79 206f 6e65  s in exactly one
-000040c0: 206f 6620 736f 6d65 0a20 2020 2066 6978   of some.    fix
-000040d0: 6564 2066 696e 6974 6520 6e75 6d62 6572  ed finite number
-000040e0: 206b 206f 6620 706f 7373 6962 6c65 206f   k of possible o
-000040f0: 7574 636f 6d65 7320 6f76 6572 206e 2069  utcomes over n i
-00004100: 6e64 6570 656e 6465 6e74 2074 7269 616c  ndependent trial
-00004110: 732e 0a20 2020 2027 785b 695d 2720 696e  s..    'x[i]' in
-00004120: 6469 6361 7465 7320 7468 6520 6e75 6d62  dicates the numb
-00004130: 6572 206f 6620 7469 6d65 7320 6f75 7463  er of times outc
-00004140: 6f6d 6520 6e75 6d62 6572 2069 2077 6173  ome number i was
-00004150: 206f 6273 6572 7665 640a 2020 2020 6f76   observed.    ov
-00004160: 6572 2074 6865 206e 2074 7269 616c 732e  er the n trials.
-00004170: 0a0a 2020 2020 2e2e 206d 6174 683a 3a0a  ..    .. math::.
-00004180: 0a20 2020 2020 2020 6628 7820 5c6d 6964  .       f(x \mid
-00004190: 206e 2c20 7029 203d 205c 6672 6163 7b6e   n, p) = \frac{n
-000041a0: 217d 7b5c 7072 6f64 5f7b 693d 317d 5e6b  !}{\prod_{i=1}^k
-000041b0: 2078 5f69 217d 205c 7072 6f64 5f7b 693d   x_i!} \prod_{i=
-000041c0: 317d 5e6b 2070 5f69 5e7b 785f 697d 0a0a  1}^k p_i^{x_i}..
-000041d0: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 2020      ==========  
-000041e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000041f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004200: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-00004210: 5375 7070 6f72 7420 2020 2020 3a6d 6174  Support     :mat
-00004220: 683a 6078 205c 696e 205c 7b30 2c20 312c  h:`x \in \{0, 1,
-00004230: 205c 6c64 6f74 732c 206e 5c7d 6020 7375   \ldots, n\}` su
-00004240: 6368 2074 6861 740a 2020 2020 2020 2020  ch that.        
-00004250: 2020 2020 2020 2020 3a6d 6174 683a 605c          :math:`\
-00004260: 7375 6d20 785f 6920 3d20 6e60 0a20 2020  sum x_i = n`.   
-00004270: 204d 6561 6e20 2020 2020 2020 203a 6d61   Mean        :ma
-00004280: 7468 3a60 6e20 705f 6960 0a20 2020 2056  th:`n p_i`.    V
-00004290: 6172 6961 6e63 6520 2020 203a 6d61 7468  ariance    :math
-000042a0: 3a60 6e20 705f 6920 2831 202d 2070 5f69  :`n p_i (1 - p_i
-000042b0: 2960 0a20 2020 2043 6f76 6172 6961 6e63  )`.    Covarianc
-000042c0: 6520 203a 6d61 7468 3a60 2d6e 2070 5f69  e  :math:`-n p_i
-000042d0: 2070 5f6a 6020 666f 7220 3a6d 6174 683a   p_j` for :math:
-000042e0: 6069 205c 6e65 206a 600a 2020 2020 3d3d  `i \ne j`.    ==
-000042f0: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-00004300: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004310: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00004320: 3d3d 3d3d 3d0a 0a20 2020 2050 6172 616d  =====..    Param
-00004330: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-00004340: 2d2d 2d2d 0a20 2020 206e 203a 2074 656e  ----.    n : ten
-00004350: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
-00004360: 2020 2020 2020 2020 546f 7461 6c20 636f          Total co
-00004370: 756e 7473 2069 6e20 6561 6368 2072 6570  unts in each rep
-00004380: 6c69 6361 7465 2028 6e20 3e20 3029 2e0a  licate (n > 0)..
-00004390: 2020 2020 7020 3a20 7465 6e73 6f72 5f6c      p : tensor_l
-000043a0: 696b 6520 6f66 2066 6c6f 6174 0a20 2020  ike of float.   
-000043b0: 2020 2020 2050 726f 6261 6269 6c69 7479       Probability
-000043c0: 206f 6620 6561 6368 206f 6e65 206f 6620   of each one of 
-000043d0: 7468 6520 6469 6666 6572 656e 7420 6f75  the different ou
-000043e0: 7463 6f6d 6573 2028 3020 3c3d 2070 203c  tcomes (0 <= p <
-000043f0: 3d20 3129 2e20 5468 6520 6e75 6d62 6572  = 1). The number
-00004400: 206f 660a 2020 2020 2020 2020 6361 7465   of.        cate
-00004410: 676f 7269 6573 2069 7320 6769 7665 6e20  gories is given 
-00004420: 6279 2074 6865 206c 656e 6774 6820 6f66  by the length of
-00004430: 2074 6865 206c 6173 7420 6178 6973 2e20   the last axis. 
-00004440: 456c 656d 656e 7473 2061 7265 2065 7870  Elements are exp
-00004450: 6563 7465 6420 746f 2073 756d 0a20 2020  ected to sum.   
-00004460: 2020 2020 2074 6f20 3120 616c 6f6e 6720       to 1 along 
-00004470: 7468 6520 6c61 7374 2061 7869 732e 0a20  the last axis.. 
-00004480: 2020 2022 2222 0a20 2020 2072 765f 6f70     """.    rv_op
-00004490: 203d 206d 756c 7469 6e6f 6d69 616c 0a0a   = multinomial..
-000044a0: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-000044b0: 0a20 2020 2064 6566 2064 6973 7428 636c  .    def dist(cl
-000044c0: 732c 206e 2c20 702c 202a 6172 6773 2c20  s, n, p, *args, 
-000044d0: 2a2a 6b77 6172 6773 293a 0a20 2020 2020  **kwargs):.     
-000044e0: 2020 2070 203d 2070 742e 6173 5f74 656e     p = pt.as_ten
-000044f0: 736f 725f 7661 7269 6162 6c65 2870 290a  sor_variable(p).
-00004500: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00004510: 7461 6e63 6528 702c 2054 656e 736f 7243  tance(p, TensorC
-00004520: 6f6e 7374 616e 7429 3a0a 2020 2020 2020  onstant):.      
-00004530: 2020 2020 2020 705f 203d 206e 702e 6173        p_ = np.as
-00004540: 6172 7261 7928 702e 6461 7461 290a 2020  array(p.data).  
-00004550: 2020 2020 2020 2020 2020 6966 206e 702e            if np.
-00004560: 616e 7928 705f 203c 2030 293a 0a20 2020  any(p_ < 0):.   
-00004570: 2020 2020 2020 2020 2020 2020 2072 6169               rai
-00004580: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
-00004590: 4e65 6761 7469 7665 2060 7060 2070 6172  Negative `p` par
-000045a0: 616d 6574 6572 7320 6172 6520 6e6f 7420  ameters are not 
-000045b0: 7661 6c69 642c 2067 6f74 3a20 7b70 5f7d  valid, got: {p_}
-000045c0: 2229 0a20 2020 2020 2020 2020 2020 2070  ").            p
-000045d0: 5f73 756d 5f20 3d20 6e70 2e73 756d 285b  _sum_ = np.sum([
-000045e0: 705f 5d2c 2061 7869 733d 2d31 290a 2020  p_], axis=-1).  
-000045f0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00004600: 206e 702e 616c 6c28 6e70 2e69 7363 6c6f   np.all(np.isclo
-00004610: 7365 2870 5f73 756d 5f2c 2031 2e30 2929  se(p_sum_, 1.0))
-00004620: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004630: 2020 7761 726e 696e 6773 2e77 6172 6e28    warnings.warn(
-00004640: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004650: 2020 2020 2066 2260 7060 2070 6172 616d       f"`p` param
-00004660: 6574 6572 7320 7375 6d20 746f 207b 705f  eters sum to {p_
-00004670: 7375 6d5f 7d2c 2069 6e73 7465 6164 206f  sum_}, instead o
-00004680: 6620 312e 302e 2022 0a20 2020 2020 2020  f 1.0. ".       
-00004690: 2020 2020 2020 2020 2020 2020 2022 5468               "Th
-000046a0: 6579 2077 696c 6c20 6265 2061 7574 6f6d  ey will be autom
-000046b0: 6174 6963 616c 6c79 2072 6573 6361 6c65  atically rescale
-000046c0: 642e 2022 0a20 2020 2020 2020 2020 2020  d. ".           
-000046d0: 2020 2020 2020 2020 2022 596f 7520 6361           "You ca
-000046e0: 6e20 7265 7363 616c 6520 7468 656d 2064  n rescale them d
-000046f0: 6972 6563 746c 7920 746f 2067 6574 2072  irectly to get r
-00004700: 6964 206f 6620 7468 6973 2077 6172 6e69  id of this warni
-00004710: 6e67 2e22 2c0a 2020 2020 2020 2020 2020  ng.",.          
-00004720: 2020 2020 2020 2020 2020 5573 6572 5761            UserWa
-00004730: 726e 696e 672c 0a20 2020 2020 2020 2020  rning,.         
-00004740: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00004750: 2020 2020 2020 2020 2070 5f20 3d20 705f           p_ = p_
-00004760: 202f 2070 742e 7375 6d28 705f 2c20 6178   / pt.sum(p_, ax
-00004770: 6973 3d2d 312c 206b 6565 7064 696d 733d  is=-1, keepdims=
-00004780: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
-00004790: 2020 2020 2020 7020 3d20 7074 2e61 735f        p = pt.as_
-000047a0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-000047b0: 705f 290a 2020 2020 2020 2020 6e20 3d20  p_).        n = 
-000047c0: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
-000047d0: 6961 626c 6528 6e29 0a20 2020 2020 2020  iable(n).       
-000047e0: 2070 203d 2070 742e 6173 5f74 656e 736f   p = pt.as_tenso
-000047f0: 725f 7661 7269 6162 6c65 2870 290a 2020  r_variable(p).  
-00004800: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-00004810: 6572 2829 2e64 6973 7428 5b6e 2c20 705d  er().dist([n, p]
-00004820: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
-00004830: 7329 0a0a 2020 2020 6465 6620 6d6f 6d65  s)..    def mome
-00004840: 6e74 2872 762c 2073 697a 652c 206e 2c20  nt(rv, size, n, 
-00004850: 7029 3a0a 2020 2020 2020 2020 6e20 3d20  p):.        n = 
-00004860: 7074 2e73 6861 7065 5f70 6164 7269 6768  pt.shape_padrigh
-00004870: 7428 6e29 0a20 2020 2020 2020 206d 6f64  t(n).        mod
-00004880: 6520 3d20 7074 2e72 6f75 6e64 286e 202a  e = pt.round(n *
-00004890: 2070 290a 2020 2020 2020 2020 6469 6666   p).        diff
-000048a0: 203d 206e 202d 2070 742e 7375 6d28 6d6f   = n - pt.sum(mo
-000048b0: 6465 2c20 6178 6973 3d2d 312c 206b 6565  de, axis=-1, kee
-000048c0: 7064 696d 733d 5472 7565 290a 2020 2020  pdims=True).    
-000048d0: 2020 2020 696e 635f 626f 6f6c 5f61 7272      inc_bool_arr
-000048e0: 203d 2070 742e 6162 7328 6469 6666 2920   = pt.abs(diff) 
-000048f0: 3e20 300a 2020 2020 2020 2020 6d6f 6465  > 0.        mode
-00004900: 203d 2070 742e 696e 635f 7375 6274 656e   = pt.inc_subten
-00004910: 736f 7228 6d6f 6465 5b69 6e63 5f62 6f6f  sor(mode[inc_boo
-00004920: 6c5f 6172 722e 6e6f 6e7a 6572 6f28 295d  l_arr.nonzero()]
-00004930: 2c20 6469 6666 5b69 6e63 5f62 6f6f 6c5f  , diff[inc_bool_
-00004940: 6172 722e 6e6f 6e7a 6572 6f28 295d 290a  arr.nonzero()]).
-00004950: 2020 2020 2020 2020 6966 206e 6f74 2072          if not r
-00004960: 765f 7369 7a65 5f69 735f 6e6f 6e65 2873  v_size_is_none(s
-00004970: 697a 6529 3a0a 2020 2020 2020 2020 2020  ize):.          
-00004980: 2020 6f75 7470 7574 5f73 697a 6520 3d20    output_size = 
-00004990: 7074 2e63 6f6e 6361 7465 6e61 7465 285b  pt.concatenate([
-000049a0: 7369 7a65 2c20 5b70 2e73 6861 7065 5b2d  size, [p.shape[-
-000049b0: 315d 5d5d 290a 2020 2020 2020 2020 2020  1]]]).          
-000049c0: 2020 6d6f 6465 203d 2070 742e 6675 6c6c    mode = pt.full
-000049d0: 286f 7574 7075 745f 7369 7a65 2c20 6d6f  (output_size, mo
-000049e0: 6465 290a 2020 2020 2020 2020 7265 7475  de).        retu
-000049f0: 726e 206d 6f64 650a 0a20 2020 2064 6566  rn mode..    def
-00004a00: 206c 6f67 7028 7661 6c75 652c 206e 2c20   logp(value, n, 
-00004a10: 7029 3a0a 2020 2020 2020 2020 2222 220a  p):.        """.
-00004a20: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
-00004a30: 6520 6c6f 672d 7072 6f62 6162 696c 6974  e log-probabilit
-00004a40: 7920 6f66 204d 756c 7469 6e6f 6d69 616c  y of Multinomial
-00004a50: 2064 6973 7472 6962 7574 696f 6e0a 2020   distribution.  
-00004a60: 2020 2020 2020 6174 2073 7065 6369 6669        at specifi
-00004a70: 6564 2076 616c 7565 2e0a 0a20 2020 2020  ed value...     
-00004a80: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00004a90: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00004aa0: 0a20 2020 2020 2020 2076 616c 7565 3a20  .        value: 
-00004ab0: 6e75 6d65 7269 630a 2020 2020 2020 2020  numeric.        
-00004ac0: 2020 2020 5661 6c75 6520 666f 7220 7768      Value for wh
-00004ad0: 6963 6820 6c6f 672d 7072 6f62 6162 696c  ich log-probabil
-00004ae0: 6974 7920 6973 2063 616c 6375 6c61 7465  ity is calculate
-00004af0: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
-00004b00: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00004b10: 2d2d 2d0a 2020 2020 2020 2020 5465 6e73  ---.        Tens
-00004b20: 6f72 5661 7269 6162 6c65 0a20 2020 2020  orVariable.     
-00004b30: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-00004b40: 7265 7320 3d20 6661 6374 6c6e 286e 2920  res = factln(n) 
-00004b50: 2b20 7074 2e73 756d 282d 6661 6374 6c6e  + pt.sum(-factln
-00004b60: 2876 616c 7565 2920 2b20 6c6f 6770 6f77  (value) + logpow
-00004b70: 2870 2c20 7661 6c75 6529 2c20 6178 6973  (p, value), axis
-00004b80: 3d2d 3129 0a20 2020 2020 2020 2072 6573  =-1).        res
-00004b90: 203d 2070 742e 7377 6974 6368 280a 2020   = pt.switch(.  
-00004ba0: 2020 2020 2020 2020 2020 7074 2e6f 725f            pt.or_
-00004bb0: 2870 742e 616e 7928 7074 2e6c 7428 7661  (pt.any(pt.lt(va
-00004bc0: 6c75 652c 2030 292c 2061 7869 733d 2d31  lue, 0), axis=-1
-00004bd0: 292c 2070 742e 6e65 7128 7074 2e73 756d  ), pt.neq(pt.sum
-00004be0: 2876 616c 7565 2c20 6178 6973 3d2d 3129  (value, axis=-1)
-00004bf0: 2c20 6e29 292c 0a20 2020 2020 2020 2020  , n)),.         
-00004c00: 2020 202d 6e70 2e69 6e66 2c0a 2020 2020     -np.inf,.    
-00004c10: 2020 2020 2020 2020 7265 732c 0a20 2020          res,.   
-00004c20: 2020 2020 2029 0a20 2020 2020 2020 2072       ).        r
-00004c30: 6574 7572 6e20 6368 6563 6b5f 7061 7261  eturn check_para
-00004c40: 6d65 7465 7273 280a 2020 2020 2020 2020  meters(.        
-00004c50: 2020 2020 7265 732c 0a20 2020 2020 2020      res,.       
-00004c60: 2020 2020 2030 203c 3d20 702c 0a20 2020       0 <= p,.   
-00004c70: 2020 2020 2020 2020 2070 203c 3d20 312c           p <= 1,
-00004c80: 0a20 2020 2020 2020 2020 2020 2070 742e  .            pt.
-00004c90: 6973 636c 6f73 6528 7074 2e73 756d 2870  isclose(pt.sum(p
-00004ca0: 2c20 6178 6973 3d2d 3129 2c20 3129 2c0a  , axis=-1), 1),.
-00004cb0: 2020 2020 2020 2020 2020 2020 7074 2e67              pt.g
-00004cc0: 6528 6e2c 2030 292c 0a20 2020 2020 2020  e(n, 0),.       
-00004cd0: 2020 2020 206d 7367 3d22 3020 3c3d 2070       msg="0 <= p
-00004ce0: 203c 3d20 312c 2073 756d 2870 2920 3d20   <= 1, sum(p) = 
-00004cf0: 312c 206e 203e 3d20 3022 2c0a 2020 2020  1, n >= 0",.    
-00004d00: 2020 2020 290a 0a0a 636c 6173 7320 4469      )...class Di
-00004d10: 7269 6368 6c65 744d 756c 7469 6e6f 6d69  richletMultinomi
-00004d20: 616c 5256 2852 616e 646f 6d56 6172 6961  alRV(RandomVaria
-00004d30: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
-00004d40: 2022 6469 7269 6368 6c65 745f 6d75 6c74   "dirichlet_mult
-00004d50: 696e 6f6d 6961 6c22 0a20 2020 206e 6469  inomial".    ndi
-00004d60: 6d5f 7375 7070 203d 2031 0a20 2020 206e  m_supp = 1.    n
-00004d70: 6469 6d73 5f70 6172 616d 7320 3d20 5b30  dims_params = [0
-00004d80: 2c20 315d 0a20 2020 2064 7479 7065 203d  , 1].    dtype =
-00004d90: 2022 696e 7436 3422 0a20 2020 205f 7072   "int64".    _pr
-00004da0: 696e 745f 6e61 6d65 203d 2028 2244 6972  int_name = ("Dir
-00004db0: 6963 686c 6574 4d4e 222c 2022 5c5c 6f70  ichletMN", "\\op
-00004dc0: 6572 6174 6f72 6e61 6d65 7b44 6972 6963  eratorname{Diric
-00004dd0: 686c 6574 4d4e 7d22 290a 0a20 2020 2064  hletMN}")..    d
-00004de0: 6566 205f 7375 7070 5f73 6861 7065 5f66  ef _supp_shape_f
-00004df0: 726f 6d5f 7061 7261 6d73 2873 656c 662c  rom_params(self,
-00004e00: 2064 6973 745f 7061 7261 6d73 2c20 7265   dist_params, re
-00004e10: 705f 7061 7261 6d5f 6964 783d 312c 2070  p_param_idx=1, p
-00004e20: 6172 616d 5f73 6861 7065 733d 4e6f 6e65  aram_shapes=None
-00004e30: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00004e40: 6e20 6465 6661 756c 745f 7375 7070 5f73  n default_supp_s
-00004e50: 6861 7065 5f66 726f 6d5f 7061 7261 6d73  hape_from_params
-00004e60: 280a 2020 2020 2020 2020 2020 2020 7365  (.            se
-00004e70: 6c66 2e6e 6469 6d5f 7375 7070 2c20 6469  lf.ndim_supp, di
-00004e80: 7374 5f70 6172 616d 732c 2072 6570 5f70  st_params, rep_p
-00004e90: 6172 616d 5f69 6478 2c20 7061 7261 6d5f  aram_idx, param_
-00004ea0: 7368 6170 6573 0a20 2020 2020 2020 2029  shapes.        )
-00004eb0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
-00004ec0: 6f64 0a20 2020 2064 6566 2072 6e67 5f66  od.    def rng_f
-00004ed0: 6e28 636c 732c 2072 6e67 2c20 6e2c 2061  n(cls, rng, n, a
-00004ee0: 2c20 7369 7a65 293a 0a20 2020 2020 2020  , size):.       
-00004ef0: 2069 6620 6e2e 6e64 696d 203e 2030 206f   if n.ndim > 0 o
-00004f00: 7220 612e 6e64 696d 203e 2031 3a0a 2020  r a.ndim > 1:.  
-00004f10: 2020 2020 2020 2020 2020 6e2c 2061 203d            n, a =
-00004f20: 2062 726f 6164 6361 7374 5f70 6172 616d   broadcast_param
-00004f30: 7328 5b6e 2c20 615d 2c20 636c 732e 6e64  s([n, a], cls.nd
-00004f40: 696d 735f 7061 7261 6d73 290a 2020 2020  ims_params).    
-00004f50: 2020 2020 2020 2020 7369 7a65 203d 2074          size = t
-00004f60: 7570 6c65 2873 697a 6520 6f72 2028 2929  uple(size or ())
-00004f70: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00004f80: 2073 697a 653a 0a20 2020 2020 2020 2020   size:.         
-00004f90: 2020 2020 2020 206e 203d 206e 702e 6272         n = np.br
-00004fa0: 6f61 6463 6173 745f 746f 286e 2c20 7369  oadcast_to(n, si
-00004fb0: 7a65 290a 2020 2020 2020 2020 2020 2020  ze).            
-00004fc0: 2020 2020 6120 3d20 6e70 2e62 726f 6164      a = np.broad
-00004fd0: 6361 7374 5f74 6f28 612c 2073 697a 6520  cast_to(a, size 
-00004fe0: 2b20 2861 2e73 6861 7065 5b2d 315d 2c29  + (a.shape[-1],)
-00004ff0: 290a 0a20 2020 2020 2020 2020 2020 2072  )..            r
-00005000: 6573 203d 206e 702e 656d 7074 7928 612e  es = np.empty(a.
-00005010: 7368 6170 6529 0a20 2020 2020 2020 2020  shape).         
-00005020: 2020 2066 6f72 2069 6478 2069 6e20 6e70     for idx in np
-00005030: 2e6e 6469 6e64 6578 2861 2e73 6861 7065  .ndindex(a.shape
-00005040: 5b3a 2d31 5d29 3a0a 2020 2020 2020 2020  [:-1]):.        
-00005050: 2020 2020 2020 2020 7020 3d20 726e 672e          p = rng.
-00005060: 6469 7269 6368 6c65 7428 615b 6964 785d  dirichlet(a[idx]
-00005070: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00005080: 2020 7265 735b 6964 785d 203d 2072 6e67    res[idx] = rng
-00005090: 2e6d 756c 7469 6e6f 6d69 616c 286e 5b69  .multinomial(n[i
-000050a0: 6478 5d2c 2070 290a 2020 2020 2020 2020  dx], p).        
-000050b0: 2020 2020 7265 7475 726e 2072 6573 0a20      return res. 
-000050c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000050d0: 2020 2020 2020 2020 2023 206e 2069 7320           # n is 
-000050e0: 6120 7363 616c 6172 2c20 6120 6973 2061  a scalar, a is a
-000050f0: 2031 6420 6172 7261 790a 2020 2020 2020   1d array.      
-00005100: 2020 2020 2020 7020 3d20 726e 672e 6469        p = rng.di
-00005110: 7269 6368 6c65 7428 612c 2073 697a 653d  richlet(a, size=
-00005120: 7369 7a65 2920 2023 2028 7369 7a65 2c20  size)  # (size, 
-00005130: 612e 7368 6170 6529 0a0a 2020 2020 2020  a.shape)..      
-00005140: 2020 2020 2020 7265 7320 3d20 6e70 2e65        res = np.e
-00005150: 6d70 7479 2870 2e73 6861 7065 290a 2020  mpty(p.shape).  
-00005160: 2020 2020 2020 2020 2020 666f 7220 6964            for id
-00005170: 7820 696e 206e 702e 6e64 696e 6465 7828  x in np.ndindex(
-00005180: 702e 7368 6170 655b 3a2d 315d 293a 0a20  p.shape[:-1]):. 
-00005190: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000051a0: 6573 5b69 6478 5d20 3d20 726e 672e 6d75  es[idx] = rng.mu
-000051b0: 6c74 696e 6f6d 6961 6c28 6e2c 2070 5b69  ltinomial(n, p[i
-000051c0: 6478 5d29 0a0a 2020 2020 2020 2020 2020  dx])..          
-000051d0: 2020 7265 7475 726e 2072 6573 0a0a 0a64    return res...d
-000051e0: 6972 6963 686c 6574 5f6d 756c 7469 6e6f  irichlet_multino
-000051f0: 6d69 616c 203d 2044 6972 6963 686c 6574  mial = Dirichlet
-00005200: 4d75 6c74 696e 6f6d 6961 6c52 5628 290a  MultinomialRV().
-00005210: 0a0a 636c 6173 7320 4469 7269 6368 6c65  ..class Dirichle
-00005220: 744d 756c 7469 6e6f 6d69 616c 2844 6973  tMultinomial(Dis
-00005230: 6372 6574 6529 3a0a 2020 2020 7222 2222  crete):.    r"""
-00005240: 4469 7269 6368 6c65 7420 4d75 6c74 696e  Dirichlet Multin
-00005250: 6f6d 6961 6c20 6c6f 672d 6c69 6b65 6c69  omial log-likeli
-00005260: 686f 6f64 2e0a 0a20 2020 2044 6972 6963  hood...    Diric
-00005270: 686c 6574 206d 6978 7475 7265 206f 6620  hlet mixture of 
-00005280: 4d75 6c74 696e 6f6d 6961 6c73 2064 6973  Multinomials dis
-00005290: 7472 6962 7574 696f 6e2c 2077 6974 6820  tribution, with 
-000052a0: 6120 6d61 7267 696e 616c 697a 6564 2050  a marginalized P
-000052b0: 4d46 2e0a 0a20 2020 202e 2e20 6d61 7468  MF...    .. math
-000052c0: 3a3a 0a0a 2020 2020 2020 2020 6628 7820  ::..        f(x 
-000052d0: 5c6d 6964 206e 2c20 6129 203d 205c 6672  \mid n, a) = \fr
-000052e0: 6163 7b5c 4761 6d6d 6128 6e20 2b20 3129  ac{\Gamma(n + 1)
-000052f0: 5c47 616d 6d61 285c 7375 6d20 615f 6b29  \Gamma(\sum a_k)
-00005300: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+00001d40: 2020 2020 205b 302e 312c 2030 2e32 2c20       [0.1, 0.2, 
+00001d50: 312e 305d 5d29 0a20 2020 2020 2020 2064  1.0]]).        d
+00001d60: 6174 6120 3d20 6e70 2e72 616e 646f 6d2e  ata = np.random.
+00001d70: 6d75 6c74 6976 6172 6961 7465 5f6e 6f72  multivariate_nor
+00001d80: 6d61 6c28 6d75 2c20 7472 7565 5f63 6f76  mal(mu, true_cov
+00001d90: 2c20 3130 290a 0a20 2020 2020 2020 2073  , 10)..        s
+00001da0: 645f 6469 7374 203d 2070 6d2e 4578 706f  d_dist = pm.Expo
+00001db0: 6e65 6e74 6961 6c2e 6469 7374 2831 2e30  nential.dist(1.0
+00001dc0: 2c20 7368 6170 653d 3329 0a20 2020 2020  , shape=3).     
+00001dd0: 2020 2063 686f 6c2c 2063 6f72 722c 2073     chol, corr, s
+00001de0: 7464 7320 3d20 706d 2e4c 4b4a 4368 6f6c  tds = pm.LKJChol
+00001df0: 6573 6b79 436f 7628 2763 686f 6c5f 636f  eskyCov('chol_co
+00001e00: 7627 2c20 6e3d 332c 2065 7461 3d32 2c0a  v', n=3, eta=2,.
+00001e10: 2020 2020 2020 2020 2020 2020 7364 5f64              sd_d
+00001e20: 6973 743d 7364 5f64 6973 742c 2063 6f6d  ist=sd_dist, com
+00001e30: 7075 7465 5f63 6f72 723d 5472 7565 290a  pute_corr=True).
+00001e40: 2020 2020 2020 2020 7661 6c73 203d 2070          vals = p
+00001e50: 6d2e 4d76 4e6f 726d 616c 2827 7661 6c73  m.MvNormal('vals
+00001e60: 272c 206d 753d 6d75 2c20 6368 6f6c 3d63  ', mu=mu, chol=c
+00001e70: 686f 6c2c 206f 6273 6572 7665 643d 6461  hol, observed=da
+00001e80: 7461 290a 0a20 2020 2046 6f72 2075 6e6f  ta)..    For uno
+00001e90: 6273 6572 7665 6420 7661 6c75 6573 2069  bserved values i
+00001ea0: 7420 6361 6e20 6265 2062 6574 7465 7220  t can be better 
+00001eb0: 746f 2075 7365 2061 206e 6f6e 2d63 656e  to use a non-cen
+00001ec0: 7465 7265 640a 2020 2020 7061 7261 6d65  tered.    parame
+00001ed0: 7472 697a 6174 696f 6e3a 3a0a 0a20 2020  trization::..   
+00001ee0: 2020 2020 2073 645f 6469 7374 203d 2070       sd_dist = p
+00001ef0: 6d2e 4578 706f 6e65 6e74 6961 6c2e 6469  m.Exponential.di
+00001f00: 7374 2831 2e30 2c20 7368 6170 653d 3329  st(1.0, shape=3)
+00001f10: 0a20 2020 2020 2020 2063 686f 6c2c 205f  .        chol, _
+00001f20: 2c20 5f20 3d20 706d 2e4c 4b4a 4368 6f6c  , _ = pm.LKJChol
+00001f30: 6573 6b79 436f 7628 2763 686f 6c5f 636f  eskyCov('chol_co
+00001f40: 7627 2c20 6e3d 332c 2065 7461 3d32 2c0a  v', n=3, eta=2,.
+00001f50: 2020 2020 2020 2020 2020 2020 7364 5f64              sd_d
+00001f60: 6973 743d 7364 5f64 6973 742c 2063 6f6d  ist=sd_dist, com
+00001f70: 7075 7465 5f63 6f72 723d 5472 7565 290a  pute_corr=True).
+00001f80: 2020 2020 2020 2020 7661 6c73 5f72 6177          vals_raw
+00001f90: 203d 2070 6d2e 4e6f 726d 616c 2827 7661   = pm.Normal('va
+00001fa0: 6c73 5f72 6177 272c 206d 753d 302c 2073  ls_raw', mu=0, s
+00001fb0: 6967 6d61 3d31 2c20 7368 6170 653d 2835  igma=1, shape=(5
+00001fc0: 2c20 3329 290a 2020 2020 2020 2020 7661  , 3)).        va
+00001fd0: 6c73 203d 2070 6d2e 4465 7465 726d 696e  ls = pm.Determin
+00001fe0: 6973 7469 6328 2776 616c 7327 2c20 7074  istic('vals', pt
+00001ff0: 2e64 6f74 2863 686f 6c2c 2076 616c 735f  .dot(chol, vals_
+00002000: 7261 772e 5429 2e54 290a 2020 2020 2222  raw.T).T).    ""
+00002010: 220a 2020 2020 7276 5f6f 7020 3d20 6d75  ".    rv_op = mu
+00002020: 6c74 6976 6172 6961 7465 5f6e 6f72 6d61  ltivariate_norma
+00002030: 6c0a 0a20 2020 2040 636c 6173 736d 6574  l..    @classmet
+00002040: 686f 640a 2020 2020 6465 6620 6469 7374  hod.    def dist
+00002050: 2863 6c73 2c20 6d75 2c20 636f 763d 4e6f  (cls, mu, cov=No
+00002060: 6e65 2c20 7461 753d 4e6f 6e65 2c20 6368  ne, tau=None, ch
+00002070: 6f6c 3d4e 6f6e 652c 206c 6f77 6572 3d54  ol=None, lower=T
+00002080: 7275 652c 202a 2a6b 7761 7267 7329 3a0a  rue, **kwargs):.
+00002090: 2020 2020 2020 2020 6d75 203d 2070 742e          mu = pt.
+000020a0: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+000020b0: 6c65 286d 7529 0a20 2020 2020 2020 2063  le(mu).        c
+000020c0: 6f76 203d 2071 7561 6464 6973 745f 6d61  ov = quaddist_ma
+000020d0: 7472 6978 2863 6f76 2c20 6368 6f6c 2c20  trix(cov, chol, 
+000020e0: 7461 752c 206c 6f77 6572 290a 2020 2020  tau, lower).    
+000020f0: 2020 2020 2320 5079 5465 6e73 6f72 2069      # PyTensor i
+00002100: 7320 7374 7269 6374 6572 2061 626f 7574  s stricter about
+00002110: 2074 6865 2073 6861 7065 206f 6620 6d75   the shape of mu
+00002120: 2c20 7468 616e 2050 794d 4320 7573 6564  , than PyMC used
+00002130: 2074 6f20 6265 0a20 2020 2020 2020 206d   to be.        m
+00002140: 7520 3d20 7074 2e62 726f 6164 6361 7374  u = pt.broadcast
+00002150: 5f61 7272 6179 7328 6d75 2c20 636f 765b  _arrays(mu, cov[
+00002160: 2e2e 2e2c 202d 315d 295b 305d 0a20 2020  ..., -1])[0].   
+00002170: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00002180: 7228 292e 6469 7374 285b 6d75 2c20 636f  r().dist([mu, co
+00002190: 765d 2c20 2a2a 6b77 6172 6773 290a 0a20  v], **kwargs).. 
+000021a0: 2020 2064 6566 206d 6f6d 656e 7428 7276     def moment(rv
+000021b0: 2c20 7369 7a65 2c20 6d75 2c20 636f 7629  , size, mu, cov)
+000021c0: 3a0a 2020 2020 2020 2020 6d6f 6d65 6e74  :.        moment
+000021d0: 203d 206d 750a 2020 2020 2020 2020 6966   = mu.        if
+000021e0: 206e 6f74 2072 765f 7369 7a65 5f69 735f   not rv_size_is_
+000021f0: 6e6f 6e65 2873 697a 6529 3a0a 2020 2020  none(size):.    
+00002200: 2020 2020 2020 2020 6d6f 6d65 6e74 5f73          moment_s
+00002210: 697a 6520 3d20 7074 2e63 6f6e 6361 7465  ize = pt.concate
+00002220: 6e61 7465 285b 7369 7a65 2c20 5b6d 752e  nate([size, [mu.
+00002230: 7368 6170 655b 2d31 5d5d 5d29 0a20 2020  shape[-1]]]).   
+00002240: 2020 2020 2020 2020 206d 6f6d 656e 7420           moment 
+00002250: 3d20 7074 2e66 756c 6c28 6d6f 6d65 6e74  = pt.full(moment
+00002260: 5f73 697a 652c 206d 7529 0a20 2020 2020  _size, mu).     
+00002270: 2020 2072 6574 7572 6e20 6d6f 6d65 6e74     return moment
+00002280: 0a0a 2020 2020 6465 6620 6c6f 6770 2876  ..    def logp(v
+00002290: 616c 7565 2c20 6d75 2c20 636f 7629 3a0a  alue, mu, cov):.
+000022a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000022b0: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
+000022c0: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
+000022d0: 204d 756c 7469 7661 7269 6174 6520 4e6f   Multivariate No
+000022e0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
+000022f0: 6e0a 2020 2020 2020 2020 6174 2073 7065  n.        at spe
+00002300: 6369 6669 6564 2076 616c 7565 2e0a 0a20  cified value... 
+00002310: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00002320: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00002330: 2d2d 2d2d 0a20 2020 2020 2020 2076 616c  ----.        val
+00002340: 7565 3a20 6e75 6d65 7269 630a 2020 2020  ue: numeric.    
+00002350: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
+00002360: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
+00002370: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
+00002380: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
+00002390: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000023a0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000023b0: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
+000023c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000023d0: 2020 2071 7561 6464 6973 742c 206c 6f67     quaddist, log
+000023e0: 6465 742c 206f 6b20 3d20 7175 6164 6469  det, ok = quaddi
+000023f0: 7374 5f70 6172 7365 2876 616c 7565 2c20  st_parse(value, 
+00002400: 6d75 2c20 636f 7629 0a20 2020 2020 2020  mu, cov).       
+00002410: 206b 203d 2066 6c6f 6174 5828 7661 6c75   k = floatX(valu
+00002420: 652e 7368 6170 655b 2d31 5d29 0a20 2020  e.shape[-1]).   
+00002430: 2020 2020 206e 6f72 6d20 3d20 2d30 2e35       norm = -0.5
+00002440: 202a 206b 202a 2070 6d2e 666c 6f61 7458   * k * pm.floatX
+00002450: 286e 702e 6c6f 6728 3220 2a20 6e70 2e70  (np.log(2 * np.p
+00002460: 6929 290a 2020 2020 2020 2020 7265 7475  i)).        retu
+00002470: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
+00002480: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
+00002490: 206e 6f72 6d20 2d20 302e 3520 2a20 7175   norm - 0.5 * qu
+000024a0: 6164 6469 7374 202d 206c 6f67 6465 742c  addist - logdet,
+000024b0: 0a20 2020 2020 2020 2020 2020 206f 6b2c  .            ok,
+000024c0: 0a20 2020 2020 2020 2020 2020 206d 7367  .            msg
+000024d0: 3d22 706f 7364 6566 222c 0a20 2020 2020  ="posdef",.     
+000024e0: 2020 2029 0a0a 0a63 6c61 7373 204d 7653     )...class MvS
+000024f0: 7475 6465 6e74 5452 5628 5261 6e64 6f6d  tudentTRV(Random
+00002500: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
+00002510: 616d 6520 3d20 226d 756c 7469 7661 7269  ame = "multivari
+00002520: 6174 655f 7374 7564 656e 7474 220a 2020  ate_studentt".  
+00002530: 2020 6e64 696d 5f73 7570 7020 3d20 310a    ndim_supp = 1.
+00002540: 2020 2020 6e64 696d 735f 7061 7261 6d73      ndims_params
+00002550: 203d 205b 302c 2031 2c20 325d 0a20 2020   = [0, 1, 2].   
+00002560: 2064 7479 7065 203d 2022 666c 6f61 7458   dtype = "floatX
+00002570: 220a 2020 2020 5f70 7269 6e74 5f6e 616d  ".    _print_nam
+00002580: 6520 3d20 2822 4d76 5374 7564 656e 7454  e = ("MvStudentT
+00002590: 222c 2022 5c5c 6f70 6572 6174 6f72 6e61  ", "\\operatorna
+000025a0: 6d65 7b4d 7653 7475 6465 6e74 547d 2229  me{MvStudentT}")
+000025b0: 0a0a 2020 2020 6465 6620 6d61 6b65 5f6e  ..    def make_n
+000025c0: 6f64 6528 7365 6c66 2c20 726e 672c 2073  ode(self, rng, s
+000025d0: 697a 652c 2064 7479 7065 2c20 6e75 2c20  ize, dtype, nu, 
+000025e0: 6d75 2c20 636f 7629 3a0a 2020 2020 2020  mu, cov):.      
+000025f0: 2020 6e75 203d 2070 742e 6173 5f74 656e    nu = pt.as_ten
+00002600: 736f 725f 7661 7269 6162 6c65 286e 7529  sor_variable(nu)
+00002610: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00002620: 6e75 2e6e 6469 6d20 3d3d 2030 3a0a 2020  nu.ndim == 0:.  
+00002630: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00002640: 5661 6c75 6545 7272 6f72 2822 6e75 206d  ValueError("nu m
+00002650: 7573 7420 6265 2061 2073 6361 6c61 7220  ust be a scalar 
+00002660: 286e 6469 6d3d 3029 2e22 290a 0a20 2020  (ndim=0).")..   
+00002670: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
+00002680: 7228 292e 6d61 6b65 5f6e 6f64 6528 726e  r().make_node(rn
+00002690: 672c 2073 697a 652c 2064 7479 7065 2c20  g, size, dtype, 
+000026a0: 6e75 2c20 6d75 2c20 636f 7629 0a0a 2020  nu, mu, cov)..  
+000026b0: 2020 6465 6620 5f5f 6361 6c6c 5f5f 2873    def __call__(s
+000026c0: 656c 662c 206e 752c 206d 753d 4e6f 6e65  elf, nu, mu=None
+000026d0: 2c20 636f 763d 4e6f 6e65 2c20 7369 7a65  , cov=None, size
+000026e0: 3d4e 6f6e 652c 202a 2a6b 7761 7267 7329  =None, **kwargs)
+000026f0: 3a0a 2020 2020 2020 2020 6474 7970 6520  :.        dtype 
+00002700: 3d20 7079 7465 6e73 6f72 2e63 6f6e 6669  = pytensor.confi
+00002710: 672e 666c 6f61 7458 2069 6620 7365 6c66  g.floatX if self
+00002720: 2e64 7479 7065 203d 3d20 2266 6c6f 6174  .dtype == "float
+00002730: 5822 2065 6c73 6520 7365 6c66 2e64 7479  X" else self.dty
+00002740: 7065 0a0a 2020 2020 2020 2020 6966 206d  pe..        if m
+00002750: 7520 6973 204e 6f6e 653a 0a20 2020 2020  u is None:.     
+00002760: 2020 2020 2020 206d 7520 3d20 6e70 2e61         mu = np.a
+00002770: 7272 6179 285b 302e 305d 2c20 6474 7970  rray([0.0], dtyp
+00002780: 653d 6474 7970 6529 0a20 2020 2020 2020  e=dtype).       
+00002790: 2069 6620 636f 7620 6973 204e 6f6e 653a   if cov is None:
+000027a0: 0a20 2020 2020 2020 2020 2020 2063 6f76  .            cov
+000027b0: 203d 206e 702e 6172 7261 7928 5b5b 312e   = np.array([[1.
+000027c0: 305d 5d2c 2064 7479 7065 3d64 7479 7065  0]], dtype=dtype
+000027d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+000027e0: 2073 7570 6572 2829 2e5f 5f63 616c 6c5f   super().__call_
+000027f0: 5f28 6e75 2c20 6d75 2c20 636f 762c 2073  _(nu, mu, cov, s
+00002800: 697a 653d 7369 7a65 2c20 2a2a 6b77 6172  ize=size, **kwar
+00002810: 6773 290a 0a20 2020 2064 6566 205f 7375  gs)..    def _su
+00002820: 7070 5f73 6861 7065 5f66 726f 6d5f 7061  pp_shape_from_pa
+00002830: 7261 6d73 2873 656c 662c 2064 6973 745f  rams(self, dist_
+00002840: 7061 7261 6d73 2c20 7265 705f 7061 7261  params, rep_para
+00002850: 6d5f 6964 783d 312c 2070 6172 616d 5f73  m_idx=1, param_s
+00002860: 6861 7065 733d 4e6f 6e65 293a 0a20 2020  hapes=None):.   
+00002870: 2020 2020 2072 6574 7572 6e20 6465 6661       return defa
+00002880: 756c 745f 7375 7070 5f73 6861 7065 5f66  ult_supp_shape_f
+00002890: 726f 6d5f 7061 7261 6d73 280a 2020 2020  rom_params(.    
+000028a0: 2020 2020 2020 2020 7365 6c66 2e6e 6469          self.ndi
+000028b0: 6d5f 7375 7070 2c20 6469 7374 5f70 6172  m_supp, dist_par
+000028c0: 616d 732c 2072 6570 5f70 6172 616d 5f69  ams, rep_param_i
+000028d0: 6478 2c20 7061 7261 6d5f 7368 6170 6573  dx, param_shapes
+000028e0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+000028f0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+00002900: 2064 6566 2072 6e67 5f66 6e28 636c 732c   def rng_fn(cls,
+00002910: 2072 6e67 2c20 6e75 2c20 6d75 2c20 636f   rng, nu, mu, co
+00002920: 762c 2073 697a 6529 3a0a 2020 2020 2020  v, size):.      
+00002930: 2020 6d76 5f73 616d 706c 6573 203d 206d    mv_samples = m
+00002940: 756c 7469 7661 7269 6174 655f 6e6f 726d  ultivariate_norm
+00002950: 616c 2e72 6e67 5f66 6e28 726e 673d 726e  al.rng_fn(rng=rn
+00002960: 672c 206d 6561 6e3d 6e70 2e7a 6572 6f73  g, mean=np.zeros
+00002970: 5f6c 696b 6528 6d75 292c 2063 6f76 3d63  _like(mu), cov=c
+00002980: 6f76 2c20 7369 7a65 3d73 697a 6529 0a0a  ov, size=size)..
+00002990: 2020 2020 2020 2020 2320 5461 6b65 2063          # Take c
+000029a0: 6869 3220 6472 6177 7320 616e 6420 6164  hi2 draws and ad
+000029b0: 6420 616e 2061 7869 7320 6f66 206c 656e  d an axis of len
+000029c0: 6774 6820 3120 746f 2074 6865 2072 6967  gth 1 to the rig
+000029d0: 6874 2066 6f72 2063 6f72 7265 6374 2062  ht for correct b
+000029e0: 726f 6164 6361 7374 696e 6720 6265 6c6f  roadcasting belo
+000029f0: 770a 2020 2020 2020 2020 6368 6932 5f73  w.        chi2_s
+00002a00: 616d 706c 6573 203d 206e 702e 7371 7274  amples = np.sqrt
+00002a10: 2872 6e67 2e63 6869 7371 7561 7265 286e  (rng.chisquare(n
+00002a20: 752c 2073 697a 653d 7369 7a65 2920 2f20  u, size=size) / 
+00002a30: 6e75 295b 2e2e 2e2c 204e 6f6e 655d 0a0a  nu)[..., None]..
+00002a40: 2020 2020 2020 2020 6966 2073 697a 653a          if size:
+00002a50: 0a20 2020 2020 2020 2020 2020 206d 7520  .            mu 
+00002a60: 3d20 6e70 2e62 726f 6164 6361 7374 5f74  = np.broadcast_t
+00002a70: 6f28 6d75 2c20 7369 7a65 202b 2028 6d75  o(mu, size + (mu
+00002a80: 2e73 6861 7065 5b2d 315d 2c29 290a 0a20  .shape[-1],)).. 
+00002a90: 2020 2020 2020 2072 6574 7572 6e20 286d         return (m
+00002aa0: 765f 7361 6d70 6c65 7320 2f20 6368 6932  v_samples / chi2
+00002ab0: 5f73 616d 706c 6573 2920 2b20 6d75 0a0a  _samples) + mu..
+00002ac0: 0a6d 765f 7374 7564 656e 7474 203d 204d  .mv_studentt = M
+00002ad0: 7653 7475 6465 6e74 5452 5628 290a 0a0a  vStudentTRV()...
+00002ae0: 636c 6173 7320 4d76 5374 7564 656e 7454  class MvStudentT
+00002af0: 2843 6f6e 7469 6e75 6f75 7329 3a0a 2020  (Continuous):.  
+00002b00: 2020 7222 2222 0a20 2020 204d 756c 7469    r""".    Multi
+00002b10: 7661 7269 6174 6520 5374 7564 656e 742d  variate Student-
+00002b20: 5420 6c6f 672d 6c69 6b65 6c69 686f 6f64  T log-likelihood
+00002b30: 2e0a 0a20 2020 202e 2e20 6d61 7468 3a3a  ...    .. math::
+00002b40: 0a20 2020 2020 2020 2066 285c 6d61 7468  .        f(\math
+00002b50: 6266 7b78 7d7c 205c 6e75 2c5c 6d75 2c5c  bf{x}| \nu,\mu,\
+00002b60: 5369 676d 6129 203d 0a20 2020 2020 2020  Sigma) =.       
+00002b70: 205c 6672 6163 0a20 2020 2020 2020 2020   \frac.         
+00002b80: 2020 207b 5c47 616d 6d61 5c6c 6566 745b     {\Gamma\left[
+00002b90: 285c 6e75 2b70 292f 325c 7269 6768 745d  (\nu+p)/2\right]
+00002ba0: 7d0a 2020 2020 2020 2020 2020 2020 7b5c  }.            {\
+00002bb0: 4761 6d6d 6128 5c6e 752f 3229 5c6e 755e  Gamma(\nu/2)\nu^
+00002bc0: 7b70 2f32 7d5c 7069 5e7b 702f 327d 0a20  {p/2}\pi^{p/2}. 
+00002bd0: 2020 2020 2020 2020 2020 2020 5c6c 6566              \lef
+00002be0: 747c 7b5c 5369 676d 617d 5c72 6967 6874  t|{\Sigma}\right
+00002bf0: 7c5e 7b31 2f32 7d0a 2020 2020 2020 2020  |^{1/2}.        
+00002c00: 2020 2020 205c 6c65 6674 5b0a 2020 2020       \left[.    
+00002c10: 2020 2020 2020 2020 2020 2031 2b5c 6672             1+\fr
+00002c20: 6163 7b31 7d7b 5c6e 757d 0a20 2020 2020  ac{1}{\nu}.     
+00002c30: 2020 2020 2020 2020 2020 287b 5c6d 6174            ({\mat
+00002c40: 6862 6620 787d 2d7b 5c6d 757d 295e 540a  hbf x}-{\mu})^T.
+00002c50: 2020 2020 2020 2020 2020 2020 2020 207b                 {
+00002c60: 5c53 6967 6d61 7d5e 7b2d 317d 287b 5c6d  \Sigma}^{-1}({\m
+00002c70: 6174 6862 6620 787d 2d7b 5c6d 757d 290a  athbf x}-{\mu}).
+00002c80: 2020 2020 2020 2020 2020 2020 205c 7269               \ri
+00002c90: 6768 745d 5e7b 2d28 5c6e 752b 7029 2f32  ght]^{-(\nu+p)/2
+00002ca0: 7d7d 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  }}..    ========
+00002cb0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
+00002cc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002cd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00002ce0: 2020 2020 5375 7070 6f72 7420 2020 3a6d      Support   :m
+00002cf0: 6174 683a 6078 205c 696e 205c 6d61 7468  ath:`x \in \math
+00002d00: 6262 7b52 7d5e 7060 0a20 2020 204d 6561  bb{R}^p`.    Mea
+00002d10: 6e20 2020 2020 203a 6d61 7468 3a60 5c6d  n      :math:`\m
+00002d20: 7560 2069 6620 3a6d 6174 683a 605c 6e75  u` if :math:`\nu
+00002d30: 203e 2031 6020 656c 7365 2075 6e64 6566   > 1` else undef
+00002d40: 696e 6564 0a20 2020 2056 6172 6961 6e63  ined.    Varianc
+00002d50: 6520 203a 6d61 7468 3a60 5c66 7261 637b  e  :math:`\frac{
+00002d60: 5c6e 757d 7b5c 6d75 2d32 7d5c 5369 676d  \nu}{\mu-2}\Sigm
+00002d70: 6160 0a20 2020 2020 2020 2020 2020 2020  a`.             
+00002d80: 2020 2020 2069 6620 3a6d 6174 683a 605c       if :math:`\
+00002d90: 6e75 3e32 6020 656c 7365 2075 6e64 6566  nu>2` else undef
+00002da0: 696e 6564 0a20 2020 203d 3d3d 3d3d 3d3d  ined.    =======
+00002db0: 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  =  =============
+00002dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002dd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00002de0: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00002df0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
+00002e00: 2020 2020 6e75 203a 2074 656e 736f 725f      nu : tensor_
+00002e10: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
+00002e20: 2020 2020 2020 4465 6772 6565 7320 6f66        Degrees of
+00002e30: 2066 7265 6564 6f6d 2c20 7368 6f75 6c64   freedom, should
+00002e40: 2062 6520 6120 706f 7369 7469 7665 2073   be a positive s
+00002e50: 6361 6c61 722e 0a20 2020 2053 6967 6d61  calar..    Sigma
+00002e60: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+00002e70: 6620 666c 6f61 742c 206f 7074 696f 6e61  f float, optiona
+00002e80: 6c0a 2020 2020 2020 2020 5363 616c 6520  l.        Scale 
+00002e90: 6d61 7472 6978 2e20 5573 6520 6073 6361  matrix. Use `sca
+00002ea0: 6c65 6020 696e 206e 6577 2063 6f64 652e  le` in new code.
+00002eb0: 0a20 2020 206d 7520 3a20 7465 6e73 6f72  .    mu : tensor
+00002ec0: 5f6c 696b 6520 6f66 2066 6c6f 6174 2c20  _like of float, 
+00002ed0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
+00002ee0: 2056 6563 746f 7220 6f66 206d 6561 6e73   Vector of means
+00002ef0: 2e0a 2020 2020 7363 616c 6520 3a20 7465  ..    scale : te
+00002f00: 6e73 6f72 5f6c 696b 6520 6f66 2066 6c6f  nsor_like of flo
+00002f10: 6174 2c20 6f70 7469 6f6e 616c 0a20 2020  at, optional.   
+00002f20: 2020 2020 2054 6865 2073 6361 6c65 206d       The scale m
+00002f30: 6174 7269 782e 0a20 2020 2074 6175 203a  atrix..    tau :
+00002f40: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
+00002f50: 666c 6f61 742c 206f 7074 696f 6e61 6c0a  float, optional.
+00002f60: 2020 2020 2020 2020 5468 6520 7072 6563          The prec
+00002f70: 6973 696f 6e20 6d61 7472 6978 2e0a 2020  ision matrix..  
+00002f80: 2020 6368 6f6c 203a 2074 656e 736f 725f    chol : tensor_
+00002f90: 6c69 6b65 206f 6620 666c 6f61 742c 206f  like of float, o
+00002fa0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00002fb0: 5468 6520 6368 6f6c 6573 6b79 2066 6163  The cholesky fac
+00002fc0: 746f 7220 6f66 2074 6865 2073 6361 6c65  tor of the scale
+00002fd0: 206d 6174 7269 782e 0a20 2020 206c 6f77   matrix..    low
+00002fe0: 6572 203a 2062 6f6f 6c2c 2064 6566 6175  er : bool, defau
+00002ff0: 6c74 3d54 7275 650a 2020 2020 2020 2020  lt=True.        
+00003000: 5768 6574 6865 7220 7468 6520 6368 6f6c  Whether the chol
+00003010: 6573 6b79 2066 6174 636f 7220 6973 2067  esky fatcor is g
+00003020: 6976 656e 2061 7320 6120 6c6f 7765 7220  iven as a lower 
+00003030: 7472 6961 6e67 756c 6172 206d 6174 7269  triangular matri
+00003040: 782e 0a20 2020 2022 2222 0a20 2020 2072  x..    """.    r
+00003050: 765f 6f70 203d 206d 765f 7374 7564 656e  v_op = mv_studen
+00003060: 7474 0a0a 2020 2020 4063 6c61 7373 6d65  tt..    @classme
+00003070: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
+00003080: 7428 636c 732c 206e 752c 2053 6967 6d61  t(cls, nu, Sigma
+00003090: 3d4e 6f6e 652c 206d 753d 4e6f 6e65 2c20  =None, mu=None, 
+000030a0: 7363 616c 653d 4e6f 6e65 2c20 7461 753d  scale=None, tau=
+000030b0: 4e6f 6e65 2c20 6368 6f6c 3d4e 6f6e 652c  None, chol=None,
+000030c0: 206c 6f77 6572 3d54 7275 652c 202a 2a6b   lower=True, **k
+000030d0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+000030e0: 636f 7620 3d20 6b77 6172 6773 2e70 6f70  cov = kwargs.pop
+000030f0: 2822 636f 7622 2c20 4e6f 6e65 290a 2020  ("cov", None).  
+00003100: 2020 2020 2020 6966 2063 6f76 2069 7320        if cov is 
+00003110: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003120: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
+00003130: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
+00003140: 2020 2020 2022 5573 6520 7468 6520 7363       "Use the sc
+00003150: 616c 6520 6172 6775 6d65 6e74 2074 6f20  ale argument to 
+00003160: 7370 6563 6966 7920 7468 6520 7363 616c  specify the scal
+00003170: 6520 6d61 7472 6978 2e20 220a 2020 2020  e matrix. ".    
+00003180: 2020 2020 2020 2020 2020 2020 2263 6f76              "cov
+00003190: 2077 696c 6c20 6265 2072 656d 6f76 6564   will be removed
+000031a0: 2069 6e20 6675 7475 7265 2076 6572 7369   in future versi
+000031b0: 6f6e 732e 222c 0a20 2020 2020 2020 2020  ons.",.         
+000031c0: 2020 2020 2020 2046 7574 7572 6557 6172         FutureWar
+000031d0: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
+000031e0: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+000031f0: 7363 616c 6520 3d20 636f 760a 2020 2020  scale = cov.    
+00003200: 2020 2020 6966 2053 6967 6d61 2069 7320      if Sigma is 
+00003210: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00003220: 2020 2020 2020 6966 2073 6361 6c65 2069        if scale i
+00003230: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00003240: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00003250: 6520 5661 6c75 6545 7272 6f72 2822 5370  e ValueError("Sp
+00003260: 6563 6966 7920 6f6e 6c79 206f 6e65 206f  ecify only one o
+00003270: 6620 7363 616c 6520 616e 6420 5369 676d  f scale and Sigm
+00003280: 6122 290a 2020 2020 2020 2020 2020 2020  a").            
+00003290: 7363 616c 6520 3d20 5369 676d 610a 2020  scale = Sigma.  
+000032a0: 2020 2020 2020 6e75 203d 2070 742e 6173        nu = pt.as
+000032b0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+000032c0: 2866 6c6f 6174 5828 6e75 2929 0a20 2020  (floatX(nu)).   
+000032d0: 2020 2020 206d 7520 3d20 7074 2e61 735f       mu = pt.as_
+000032e0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
+000032f0: 666c 6f61 7458 286d 7529 290a 2020 2020  floatX(mu)).    
+00003300: 2020 2020 7363 616c 6520 3d20 7175 6164      scale = quad
+00003310: 6469 7374 5f6d 6174 7269 7828 7363 616c  dist_matrix(scal
+00003320: 652c 2063 686f 6c2c 2074 6175 2c20 6c6f  e, chol, tau, lo
+00003330: 7765 7229 0a20 2020 2020 2020 2023 2050  wer).        # P
+00003340: 7954 656e 736f 7220 6973 2073 7472 6963  yTensor is stric
+00003350: 7465 7220 6162 6f75 7420 7468 6520 7368  ter about the sh
+00003360: 6170 6520 6f66 206d 752c 2074 6861 6e20  ape of mu, than 
+00003370: 5079 4d43 2075 7365 6420 746f 2062 650a  PyMC used to be.
+00003380: 2020 2020 2020 2020 6d75 203d 2070 742e          mu = pt.
+00003390: 6272 6f61 6463 6173 745f 6172 7261 7973  broadcast_arrays
+000033a0: 286d 752c 2073 6361 6c65 5b2e 2e2e 2c20  (mu, scale[..., 
+000033b0: 2d31 5d29 5b30 5d0a 0a20 2020 2020 2020  -1])[0]..       
+000033c0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+000033d0: 6469 7374 285b 6e75 2c20 6d75 2c20 7363  dist([nu, mu, sc
+000033e0: 616c 655d 2c20 2a2a 6b77 6172 6773 290a  ale], **kwargs).
+000033f0: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
+00003400: 7276 2c20 7369 7a65 2c20 6e75 2c20 6d75  rv, size, nu, mu
+00003410: 2c20 7363 616c 6529 3a0a 2020 2020 2020  , scale):.      
+00003420: 2020 6d6f 6d65 6e74 203d 206d 750a 2020    moment = mu.  
+00003430: 2020 2020 2020 6966 206e 6f74 2072 765f        if not rv_
+00003440: 7369 7a65 5f69 735f 6e6f 6e65 2873 697a  size_is_none(siz
+00003450: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
+00003460: 6d6f 6d65 6e74 5f73 697a 6520 3d20 7074  moment_size = pt
+00003470: 2e63 6f6e 6361 7465 6e61 7465 285b 7369  .concatenate([si
+00003480: 7a65 2c20 5b6d 752e 7368 6170 655b 2d31  ze, [mu.shape[-1
+00003490: 5d5d 5d29 0a20 2020 2020 2020 2020 2020  ]]]).           
+000034a0: 206d 6f6d 656e 7420 3d20 7074 2e66 756c   moment = pt.ful
+000034b0: 6c28 6d6f 6d65 6e74 5f73 697a 652c 206d  l(moment_size, m
+000034c0: 6f6d 656e 7429 0a20 2020 2020 2020 2072  oment).        r
+000034d0: 6574 7572 6e20 6d6f 6d65 6e74 0a0a 2020  eturn moment..  
+000034e0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
+000034f0: 2c20 6e75 2c20 6d75 2c20 7363 616c 6529  , nu, mu, scale)
+00003500: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00003510: 2020 2020 2020 4361 6c63 756c 6174 6520        Calculate 
+00003520: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
+00003530: 6f66 204d 756c 7469 7661 7269 6174 6520  of Multivariate 
+00003540: 5374 7564 656e 7427 7320 5420 6469 7374  Student's T dist
+00003550: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
+00003560: 2061 7420 7370 6563 6966 6965 6420 7661   at specified va
+00003570: 6c75 652e 0a0a 2020 2020 2020 2020 5061  lue...        Pa
+00003580: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00003590: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+000035a0: 2020 2020 7661 6c75 653a 206e 756d 6572      value: numer
+000035b0: 6963 0a20 2020 2020 2020 2020 2020 2056  ic.            V
+000035c0: 616c 7565 2066 6f72 2077 6869 6368 206c  alue for which l
+000035d0: 6f67 2d70 726f 6261 6269 6c69 7479 2069  og-probability i
+000035e0: 7320 6361 6c63 756c 6174 6564 2e0a 0a20  s calculated... 
+000035f0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00003600: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00003610: 2020 2020 2020 2054 656e 736f 7256 6172         TensorVar
+00003620: 6961 626c 650a 2020 2020 2020 2020 2222  iable.        ""
+00003630: 220a 2020 2020 2020 2020 7175 6164 6469  ".        quaddi
+00003640: 7374 2c20 6c6f 6764 6574 2c20 6f6b 203d  st, logdet, ok =
+00003650: 2071 7561 6464 6973 745f 7061 7273 6528   quaddist_parse(
+00003660: 7661 6c75 652c 206d 752c 2073 6361 6c65  value, mu, scale
+00003670: 290a 2020 2020 2020 2020 6b20 3d20 666c  ).        k = fl
+00003680: 6f61 7458 2876 616c 7565 2e73 6861 7065  oatX(value.shape
+00003690: 5b2d 315d 290a 0a20 2020 2020 2020 206e  [-1])..        n
+000036a0: 6f72 6d20 3d20 6761 6d6d 616c 6e28 286e  orm = gammaln((n
+000036b0: 7520 2b20 6b29 202f 2032 2e30 2920 2d20  u + k) / 2.0) - 
+000036c0: 6761 6d6d 616c 6e28 6e75 202f 2032 2e30  gammaln(nu / 2.0
+000036d0: 2920 2d20 302e 3520 2a20 6b20 2a20 7074  ) - 0.5 * k * pt
+000036e0: 2e6c 6f67 286e 7520 2a20 6e70 2e70 6929  .log(nu * np.pi)
+000036f0: 0a20 2020 2020 2020 2069 6e6e 6572 203d  .        inner =
+00003700: 202d 286e 7520 2b20 6b29 202f 2032 2e30   -(nu + k) / 2.0
+00003710: 202a 2070 742e 6c6f 6731 7028 7175 6164   * pt.log1p(quad
+00003720: 6469 7374 202f 206e 7529 0a20 2020 2020  dist / nu).     
+00003730: 2020 2072 6573 203d 206e 6f72 6d20 2b20     res = norm + 
+00003740: 696e 6e65 7220 2d20 6c6f 6764 6574 0a0a  inner - logdet..
+00003750: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00003760: 6865 636b 5f70 6172 616d 6574 6572 7328  heck_parameters(
+00003770: 7265 732c 206f 6b2c 206e 7520 3e20 302c  res, ok, nu > 0,
+00003780: 206d 7367 3d22 706f 7364 6566 2c20 6e75   msg="posdef, nu
+00003790: 203e 2030 2229 0a0a 0a63 6c61 7373 2044   > 0")...class D
+000037a0: 6972 6963 686c 6574 2853 696d 706c 6578  irichlet(Simplex
+000037b0: 436f 6e74 696e 756f 7573 293a 0a20 2020  Continuous):.   
+000037c0: 2072 2222 220a 2020 2020 4469 7269 6368   r""".    Dirich
+000037d0: 6c65 7420 6c6f 672d 6c69 6b65 6c69 686f  let log-likeliho
+000037e0: 6f64 2e0a 0a20 2020 202e 2e20 6d61 7468  od...    .. math
+000037f0: 3a3a 0a0a 2020 2020 2020 2066 285c 6d61  ::..       f(\ma
+00003800: 7468 6266 7b78 7d7c 5c6d 6174 6862 667b  thbf{x}|\mathbf{
+00003810: 617d 2920 3d0a 2020 2020 2020 2020 2020  a}) =.          
+00003820: 205c 6672 6163 7b5c 4761 6d6d 6128 5c73   \frac{\Gamma(\s
+00003830: 756d 5f7b 693d 317d 5e6b 2061 5f69 297d  um_{i=1}^k a_i)}
+00003840: 7b5c 7072 6f64 5f7b 693d 317d 5e6b 205c  {\prod_{i=1}^k \
+00003850: 4761 6d6d 6128 615f 6929 7d0a 2020 2020  Gamma(a_i)}.    
+00003860: 2020 2020 2020 205c 7072 6f64 5f7b 693d         \prod_{i=
+00003870: 317d 5e6b 2078 5f69 5e7b 615f 6920 2d20  1}^k x_i^{a_i - 
+00003880: 317d 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  1}..    ========
+00003890: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
+000038a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000038b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000038c0: 3d0a 2020 2020 5375 7070 6f72 7420 2020  =.    Support   
+000038d0: 3a6d 6174 683a 6078 5f69 205c 696e 2028  :math:`x_i \in (
+000038e0: 302c 2031 2960 2066 6f72 203a 6d61 7468  0, 1)` for :math
+000038f0: 3a60 6920 5c69 6e20 5c7b 312c 205c 6c64  :`i \in \{1, \ld
+00003900: 6f74 732c 204b 5c7d 600a 2020 2020 2020  ots, K\}`.      
+00003910: 2020 2020 2020 2020 7375 6368 2074 6861          such tha
+00003920: 7420 3a6d 6174 683a 605c 7375 6d20 785f  t :math:`\sum x_
+00003930: 6920 3d20 3160 0a20 2020 204d 6561 6e20  i = 1`.    Mean 
+00003940: 2020 2020 203a 6d61 7468 3a60 5c64 6672       :math:`\dfr
+00003950: 6163 7b61 5f69 7d7b 5c73 756d 2061 5f69  ac{a_i}{\sum a_i
+00003960: 7d60 0a20 2020 2056 6172 6961 6e63 6520  }`.    Variance 
+00003970: 203a 6d61 7468 3a60 5c64 6672 6163 7b61   :math:`\dfrac{a
+00003980: 5f69 202d 205c 7375 6d20 615f 307d 7b61  _i - \sum a_0}{a
+00003990: 5f30 5e32 2028 615f 3020 2b20 3129 7d60  _0^2 (a_0 + 1)}`
+000039a0: 0a20 2020 2020 2020 2020 2020 2020 2077  .              w
+000039b0: 6865 7265 203a 6d61 7468 3a60 615f 3020  here :math:`a_0 
+000039c0: 3d20 5c73 756d 2061 5f69 600a 2020 2020  = \sum a_i`.    
+000039d0: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
+000039e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000039f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00003a00: 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050  =========..    P
+00003a10: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00003a20: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2061 203a  --------.    a :
+00003a30: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
+00003a40: 666c 6f61 740a 2020 2020 2020 2020 436f  float.        Co
+00003a50: 6e63 656e 7472 6174 696f 6e20 7061 7261  ncentration para
+00003a60: 6d65 7465 7273 2028 6120 3e20 3029 2e20  meters (a > 0). 
+00003a70: 5468 6520 6e75 6d62 6572 206f 6620 6361  The number of ca
+00003a80: 7465 676f 7269 6573 2069 7320 6769 7665  tegories is give
+00003a90: 6e20 6279 2074 6865 0a20 2020 2020 2020  n by the.       
+00003aa0: 206c 656e 6774 6820 6f66 2074 6865 206c   length of the l
+00003ab0: 6173 7420 6178 6973 2e0a 2020 2020 2222  ast axis..    ""
+00003ac0: 220a 2020 2020 7276 5f6f 7020 3d20 6469  ".    rv_op = di
+00003ad0: 7269 6368 6c65 740a 0a20 2020 2040 636c  richlet..    @cl
+00003ae0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00003af0: 6620 6469 7374 2863 6c73 2c20 612c 202a  f dist(cls, a, *
+00003b00: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+00003b10: 2020 6120 3d20 7074 2e61 735f 7465 6e73    a = pt.as_tens
+00003b20: 6f72 5f76 6172 6961 626c 6528 6129 0a20  or_variable(a). 
+00003b30: 2020 2020 2020 2023 206d 6561 6e20 3d20         # mean = 
+00003b40: 6120 2f20 7074 2e73 756d 2861 290a 2020  a / pt.sum(a).  
+00003b50: 2020 2020 2020 2320 6d6f 6465 203d 2070        # mode = p
+00003b60: 742e 7377 6974 6368 2870 742e 616c 6c28  t.switch(pt.all(
+00003b70: 6120 3e20 3129 2c20 2861 202d 2031 2920  a > 1), (a - 1) 
+00003b80: 2f20 7074 2e73 756d 2861 202d 2031 292c  / pt.sum(a - 1),
+00003b90: 206e 702e 6e61 6e29 0a0a 2020 2020 2020   np.nan)..      
+00003ba0: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+00003bb0: 2e64 6973 7428 5b61 5d2c 202a 2a6b 7761  .dist([a], **kwa
+00003bc0: 7267 7329 0a0a 2020 2020 6465 6620 6d6f  rgs)..    def mo
+00003bd0: 6d65 6e74 2872 762c 2073 697a 652c 2061  ment(rv, size, a
+00003be0: 293a 0a20 2020 2020 2020 206e 6f72 6d5f  ):.        norm_
+00003bf0: 636f 6e73 7461 6e74 203d 2070 742e 7375  constant = pt.su
+00003c00: 6d28 612c 2061 7869 733d 2d31 295b 2e2e  m(a, axis=-1)[..
+00003c10: 2e2c 204e 6f6e 655d 0a20 2020 2020 2020  ., None].       
+00003c20: 206d 6f6d 656e 7420 3d20 6120 2f20 6e6f   moment = a / no
+00003c30: 726d 5f63 6f6e 7374 616e 740a 2020 2020  rm_constant.    
+00003c40: 2020 2020 6966 206e 6f74 2072 765f 7369      if not rv_si
+00003c50: 7a65 5f69 735f 6e6f 6e65 2873 697a 6529  ze_is_none(size)
+00003c60: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
+00003c70: 6d65 6e74 203d 2070 742e 6675 6c6c 2870  ment = pt.full(p
+00003c80: 742e 636f 6e63 6174 656e 6174 6528 5b73  t.concatenate([s
+00003c90: 697a 652c 205b 612e 7368 6170 655b 2d31  ize, [a.shape[-1
+00003ca0: 5d5d 5d29 2c20 6d6f 6d65 6e74 290a 2020  ]]]), moment).  
+00003cb0: 2020 2020 2020 7265 7475 726e 206d 6f6d        return mom
+00003cc0: 656e 740a 0a20 2020 2064 6566 206c 6f67  ent..    def log
+00003cd0: 7028 7661 6c75 652c 2061 293a 0a20 2020  p(value, a):.   
+00003ce0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00003cf0: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
+00003d00: 726f 6261 6269 6c69 7479 206f 6620 4469  robability of Di
+00003d10: 7269 6368 6c65 7420 6469 7374 7269 6275  richlet distribu
+00003d20: 7469 6f6e 0a20 2020 2020 2020 2061 7420  tion.        at 
+00003d30: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
+00003d40: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00003d50: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00003d60: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00003d70: 7661 6c75 653a 206e 756d 6572 6963 0a20  value: numeric. 
+00003d80: 2020 2020 2020 2020 2020 2056 616c 7565             Value
+00003d90: 2066 6f72 2077 6869 6368 206c 6f67 2d70   for which log-p
+00003da0: 726f 6261 6269 6c69 7479 2069 7320 6361  robability is ca
+00003db0: 6c63 756c 6174 6564 2e0a 0a20 2020 2020  lculated...     
+00003dc0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00003dd0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00003de0: 2020 2054 656e 736f 7256 6172 6961 626c     TensorVariabl
+00003df0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
+00003e00: 2020 2020 2020 2320 6f6e 6c79 2064 6566        # only def
+00003e10: 696e 6564 2066 6f72 2073 756d 2876 616c  ined for sum(val
+00003e20: 7565 2920 3d3d 2031 0a20 2020 2020 2020  ue) == 1.       
+00003e30: 2072 6573 203d 2070 742e 7375 6d28 6c6f   res = pt.sum(lo
+00003e40: 6770 6f77 2876 616c 7565 2c20 6120 2d20  gpow(value, a - 
+00003e50: 3129 202d 2067 616d 6d61 6c6e 2861 292c  1) - gammaln(a),
+00003e60: 2061 7869 733d 2d31 2920 2b20 6761 6d6d   axis=-1) + gamm
+00003e70: 616c 6e28 7074 2e73 756d 2861 2c20 6178  aln(pt.sum(a, ax
+00003e80: 6973 3d2d 3129 290a 2020 2020 2020 2020  is=-1)).        
+00003e90: 7265 7320 3d20 7074 2e73 7769 7463 6828  res = pt.switch(
+00003ea0: 0a20 2020 2020 2020 2020 2020 2070 742e  .            pt.
+00003eb0: 6f72 5f28 0a20 2020 2020 2020 2020 2020  or_(.           
+00003ec0: 2020 2020 2070 742e 616e 7928 7074 2e6c       pt.any(pt.l
+00003ed0: 7428 7661 6c75 652c 2030 292c 2061 7869  t(value, 0), axi
+00003ee0: 733d 2d31 292c 0a20 2020 2020 2020 2020  s=-1),.         
+00003ef0: 2020 2020 2020 2070 742e 616e 7928 7074         pt.any(pt
+00003f00: 2e67 7428 7661 6c75 652c 2031 292c 2061  .gt(value, 1), a
+00003f10: 7869 733d 2d31 292c 0a20 2020 2020 2020  xis=-1),.       
+00003f20: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00003f30: 2020 2020 2d6e 702e 696e 662c 0a20 2020      -np.inf,.   
+00003f40: 2020 2020 2020 2020 2072 6573 2c0a 2020           res,.  
+00003f50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+00003f60: 7265 7475 726e 2063 6865 636b 5f70 6172  return check_par
+00003f70: 616d 6574 6572 7328 0a20 2020 2020 2020  ameters(.       
+00003f80: 2020 2020 2072 6573 2c0a 2020 2020 2020       res,.      
+00003f90: 2020 2020 2020 6120 3e20 302c 0a20 2020        a > 0,.   
+00003fa0: 2020 2020 2020 2020 206d 7367 3d22 6120           msg="a 
+00003fb0: 3e20 3022 2c0a 2020 2020 2020 2020 290a  > 0",.        ).
+00003fc0: 0a0a 636c 6173 7320 4d75 6c74 696e 6f6d  ..class Multinom
+00003fd0: 6961 6c28 4469 7363 7265 7465 293a 0a20  ial(Discrete):. 
+00003fe0: 2020 2072 2222 220a 2020 2020 4d75 6c74     r""".    Mult
+00003ff0: 696e 6f6d 6961 6c20 6c6f 672d 6c69 6b65  inomial log-like
+00004000: 6c69 686f 6f64 2e0a 0a20 2020 2047 656e  lihood...    Gen
+00004010: 6572 616c 697a 6573 2062 696e 6f6d 6961  eralizes binomia
+00004020: 6c20 6469 7374 7269 6275 7469 6f6e 2c20  l distribution, 
+00004030: 6275 7420 696e 7374 6561 6420 6f66 2065  but instead of e
+00004040: 6163 6820 7472 6961 6c20 7265 7375 6c74  ach trial result
+00004050: 696e 670a 2020 2020 696e 2022 7375 6363  ing.    in "succ
+00004060: 6573 7322 206f 7220 2266 6169 6c75 7265  ess" or "failure
+00004070: 222c 2065 6163 6820 6f6e 6520 7265 7375  ", each one resu
+00004080: 6c74 7320 696e 2065 7861 6374 6c79 206f  lts in exactly o
+00004090: 6e65 206f 6620 736f 6d65 0a20 2020 2066  ne of some.    f
+000040a0: 6978 6564 2066 696e 6974 6520 6e75 6d62  ixed finite numb
+000040b0: 6572 206b 206f 6620 706f 7373 6962 6c65  er k of possible
+000040c0: 206f 7574 636f 6d65 7320 6f76 6572 206e   outcomes over n
+000040d0: 2069 6e64 6570 656e 6465 6e74 2074 7269   independent tri
+000040e0: 616c 732e 0a20 2020 2027 785b 695d 2720  als..    'x[i]' 
+000040f0: 696e 6469 6361 7465 7320 7468 6520 6e75  indicates the nu
+00004100: 6d62 6572 206f 6620 7469 6d65 7320 6f75  mber of times ou
+00004110: 7463 6f6d 6520 6e75 6d62 6572 2069 2077  tcome number i w
+00004120: 6173 206f 6273 6572 7665 640a 2020 2020  as observed.    
+00004130: 6f76 6572 2074 6865 206e 2074 7269 616c  over the n trial
+00004140: 732e 0a0a 2020 2020 2e2e 206d 6174 683a  s...    .. math:
+00004150: 3a0a 0a20 2020 2020 2020 6628 7820 5c6d  :..       f(x \m
+00004160: 6964 206e 2c20 7029 203d 205c 6672 6163  id n, p) = \frac
+00004170: 7b6e 217d 7b5c 7072 6f64 5f7b 693d 317d  {n!}{\prod_{i=1}
+00004180: 5e6b 2078 5f69 217d 205c 7072 6f64 5f7b  ^k x_i!} \prod_{
+00004190: 693d 317d 5e6b 2070 5f69 5e7b 785f 697d  i=1}^k p_i^{x_i}
+000041a0: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ..    ==========
+000041b0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
+000041c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000041d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+000041e0: 2020 5375 7070 6f72 7420 2020 2020 3a6d    Support     :m
+000041f0: 6174 683a 6078 205c 696e 205c 7b30 2c20  ath:`x \in \{0, 
+00004200: 312c 205c 6c64 6f74 732c 206e 5c7d 6020  1, \ldots, n\}` 
+00004210: 7375 6368 2074 6861 740a 2020 2020 2020  such that.      
+00004220: 2020 2020 2020 2020 2020 3a6d 6174 683a            :math:
+00004230: 605c 7375 6d20 785f 6920 3d20 6e60 0a20  `\sum x_i = n`. 
+00004240: 2020 204d 6561 6e20 2020 2020 2020 203a     Mean        :
+00004250: 6d61 7468 3a60 6e20 705f 6960 0a20 2020  math:`n p_i`.   
+00004260: 2056 6172 6961 6e63 6520 2020 203a 6d61   Variance    :ma
+00004270: 7468 3a60 6e20 705f 6920 2831 202d 2070  th:`n p_i (1 - p
+00004280: 5f69 2960 0a20 2020 2043 6f76 6172 6961  _i)`.    Covaria
+00004290: 6e63 6520 203a 6d61 7468 3a60 2d6e 2070  nce  :math:`-n p
+000042a0: 5f69 2070 5f6a 6020 666f 7220 3a6d 6174  _i p_j` for :mat
+000042b0: 683a 6069 205c 6e65 206a 600a 2020 2020  h:`i \ne j`.    
+000042c0: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
+000042d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000042e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000042f0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
+00004300: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00004310: 2d2d 2d2d 2d2d 0a20 2020 206e 203a 2074  ------.    n : t
+00004320: 656e 736f 725f 6c69 6b65 206f 6620 696e  ensor_like of in
+00004330: 740a 2020 2020 2020 2020 546f 7461 6c20  t.        Total 
+00004340: 636f 756e 7473 2069 6e20 6561 6368 2072  counts in each r
+00004350: 6570 6c69 6361 7465 2028 6e20 3e20 3029  eplicate (n > 0)
+00004360: 2e0a 2020 2020 7020 3a20 7465 6e73 6f72  ..    p : tensor
+00004370: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
+00004380: 2020 2020 2020 2050 726f 6261 6269 6c69         Probabili
+00004390: 7479 206f 6620 6561 6368 206f 6e65 206f  ty of each one o
+000043a0: 6620 7468 6520 6469 6666 6572 656e 7420  f the different 
+000043b0: 6f75 7463 6f6d 6573 2028 3020 3c3d 2070  outcomes (0 <= p
+000043c0: 203c 3d20 3129 2e20 5468 6520 6e75 6d62   <= 1). The numb
+000043d0: 6572 206f 660a 2020 2020 2020 2020 6361  er of.        ca
+000043e0: 7465 676f 7269 6573 2069 7320 6769 7665  tegories is give
+000043f0: 6e20 6279 2074 6865 206c 656e 6774 6820  n by the length 
+00004400: 6f66 2074 6865 206c 6173 7420 6178 6973  of the last axis
+00004410: 2e20 456c 656d 656e 7473 2061 7265 2065  . Elements are e
+00004420: 7870 6563 7465 6420 746f 2073 756d 0a20  xpected to sum. 
+00004430: 2020 2020 2020 2074 6f20 3120 616c 6f6e         to 1 alon
+00004440: 6720 7468 6520 6c61 7374 2061 7869 732e  g the last axis.
+00004450: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
+00004460: 6f70 203d 206d 756c 7469 6e6f 6d69 616c  op = multinomial
+00004470: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+00004480: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
+00004490: 636c 732c 206e 2c20 702c 202a 6172 6773  cls, n, p, *args
+000044a0: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+000044b0: 2020 2020 2070 203d 2070 742e 6173 5f74       p = pt.as_t
+000044c0: 656e 736f 725f 7661 7269 6162 6c65 2870  ensor_variable(p
+000044d0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+000044e0: 6e73 7461 6e63 6528 702c 2054 656e 736f  nstance(p, Tenso
+000044f0: 7243 6f6e 7374 616e 7429 3a0a 2020 2020  rConstant):.    
+00004500: 2020 2020 2020 2020 705f 203d 206e 702e          p_ = np.
+00004510: 6173 6172 7261 7928 702e 6461 7461 290a  asarray(p.data).
+00004520: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00004530: 702e 616e 7928 705f 203c 2030 293a 0a20  p.any(p_ < 0):. 
+00004540: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00004550: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00004560: 6622 4e65 6761 7469 7665 2060 7060 2070  f"Negative `p` p
+00004570: 6172 616d 6574 6572 7320 6172 6520 6e6f  arameters are no
+00004580: 7420 7661 6c69 642c 2067 6f74 3a20 7b70  t valid, got: {p
+00004590: 5f7d 2229 0a20 2020 2020 2020 2020 2020  _}").           
+000045a0: 2070 5f73 756d 5f20 3d20 6e70 2e73 756d   p_sum_ = np.sum
+000045b0: 285b 705f 5d2c 2061 7869 733d 2d31 290a  ([p_], axis=-1).
+000045c0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000045d0: 6f74 206e 702e 616c 6c28 6e70 2e69 7363  ot np.all(np.isc
+000045e0: 6c6f 7365 2870 5f73 756d 5f2c 2031 2e30  lose(p_sum_, 1.0
+000045f0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00004600: 2020 2020 7761 726e 696e 6773 2e77 6172      warnings.war
+00004610: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00004620: 2020 2020 2020 2066 2260 7060 2070 6172         f"`p` par
+00004630: 616d 6574 6572 7320 7375 6d20 746f 207b  ameters sum to {
+00004640: 705f 7375 6d5f 7d2c 2069 6e73 7465 6164  p_sum_}, instead
+00004650: 206f 6620 312e 302e 2022 0a20 2020 2020   of 1.0. ".     
+00004660: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00004670: 5468 6579 2077 696c 6c20 6265 2061 7574  They will be aut
+00004680: 6f6d 6174 6963 616c 6c79 2072 6573 6361  omatically resca
+00004690: 6c65 642e 2022 0a20 2020 2020 2020 2020  led. ".         
+000046a0: 2020 2020 2020 2020 2020 2022 596f 7520             "You 
+000046b0: 6361 6e20 7265 7363 616c 6520 7468 656d  can rescale them
+000046c0: 2064 6972 6563 746c 7920 746f 2067 6574   directly to get
+000046d0: 2072 6964 206f 6620 7468 6973 2077 6172   rid of this war
+000046e0: 6e69 6e67 2e22 2c0a 2020 2020 2020 2020  ning.",.        
+000046f0: 2020 2020 2020 2020 2020 2020 5573 6572              User
+00004700: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
+00004710: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00004720: 2020 2020 2020 2020 2020 2070 5f20 3d20             p_ = 
+00004730: 705f 202f 2070 742e 7375 6d28 705f 2c20  p_ / pt.sum(p_, 
+00004740: 6178 6973 3d2d 312c 206b 6565 7064 696d  axis=-1, keepdim
+00004750: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
+00004760: 2020 2020 2020 2020 7020 3d20 7074 2e61          p = pt.a
+00004770: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
+00004780: 6528 705f 290a 2020 2020 2020 2020 6e20  e(p_).        n 
+00004790: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+000047a0: 6172 6961 626c 6528 6e29 0a20 2020 2020  ariable(n).     
+000047b0: 2020 2070 203d 2070 742e 6173 5f74 656e     p = pt.as_ten
+000047c0: 736f 725f 7661 7269 6162 6c65 2870 290a  sor_variable(p).
+000047d0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000047e0: 7570 6572 2829 2e64 6973 7428 5b6e 2c20  uper().dist([n, 
+000047f0: 705d 2c20 2a61 7267 732c 202a 2a6b 7761  p], *args, **kwa
+00004800: 7267 7329 0a0a 2020 2020 6465 6620 6d6f  rgs)..    def mo
+00004810: 6d65 6e74 2872 762c 2073 697a 652c 206e  ment(rv, size, n
+00004820: 2c20 7029 3a0a 2020 2020 2020 2020 6e20  , p):.        n 
+00004830: 3d20 7074 2e73 6861 7065 5f70 6164 7269  = pt.shape_padri
+00004840: 6768 7428 6e29 0a20 2020 2020 2020 206d  ght(n).        m
+00004850: 6f64 6520 3d20 7074 2e72 6f75 6e64 286e  ode = pt.round(n
+00004860: 202a 2070 290a 2020 2020 2020 2020 6469   * p).        di
+00004870: 6666 203d 206e 202d 2070 742e 7375 6d28  ff = n - pt.sum(
+00004880: 6d6f 6465 2c20 6178 6973 3d2d 312c 206b  mode, axis=-1, k
+00004890: 6565 7064 696d 733d 5472 7565 290a 2020  eepdims=True).  
+000048a0: 2020 2020 2020 696e 635f 626f 6f6c 5f61        inc_bool_a
+000048b0: 7272 203d 2070 742e 6162 7328 6469 6666  rr = pt.abs(diff
+000048c0: 2920 3e20 300a 2020 2020 2020 2020 6d6f  ) > 0.        mo
+000048d0: 6465 203d 2070 742e 696e 635f 7375 6274  de = pt.inc_subt
+000048e0: 656e 736f 7228 6d6f 6465 5b69 6e63 5f62  ensor(mode[inc_b
+000048f0: 6f6f 6c5f 6172 722e 6e6f 6e7a 6572 6f28  ool_arr.nonzero(
+00004900: 295d 2c20 6469 6666 5b69 6e63 5f62 6f6f  )], diff[inc_boo
+00004910: 6c5f 6172 722e 6e6f 6e7a 6572 6f28 295d  l_arr.nonzero()]
+00004920: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
+00004930: 2072 765f 7369 7a65 5f69 735f 6e6f 6e65   rv_size_is_none
+00004940: 2873 697a 6529 3a0a 2020 2020 2020 2020  (size):.        
+00004950: 2020 2020 6f75 7470 7574 5f73 697a 6520      output_size 
+00004960: 3d20 7074 2e63 6f6e 6361 7465 6e61 7465  = pt.concatenate
+00004970: 285b 7369 7a65 2c20 5b70 2e73 6861 7065  ([size, [p.shape
+00004980: 5b2d 315d 5d5d 290a 2020 2020 2020 2020  [-1]]]).        
+00004990: 2020 2020 6d6f 6465 203d 2070 742e 6675      mode = pt.fu
+000049a0: 6c6c 286f 7574 7075 745f 7369 7a65 2c20  ll(output_size, 
+000049b0: 6d6f 6465 290a 2020 2020 2020 2020 7265  mode).        re
+000049c0: 7475 726e 206d 6f64 650a 0a20 2020 2064  turn mode..    d
+000049d0: 6566 206c 6f67 7028 7661 6c75 652c 206e  ef logp(value, n
+000049e0: 2c20 7029 3a0a 2020 2020 2020 2020 2222  , p):.        ""
+000049f0: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
+00004a00: 6174 6520 6c6f 672d 7072 6f62 6162 696c  ate log-probabil
+00004a10: 6974 7920 6f66 204d 756c 7469 6e6f 6d69  ity of Multinomi
+00004a20: 616c 2064 6973 7472 6962 7574 696f 6e0a  al distribution.
+00004a30: 2020 2020 2020 2020 6174 2073 7065 6369          at speci
+00004a40: 6669 6564 2076 616c 7565 2e0a 0a20 2020  fied value...   
+00004a50: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00004a60: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00004a70: 2d2d 0a20 2020 2020 2020 2076 616c 7565  --.        value
+00004a80: 3a20 6e75 6d65 7269 630a 2020 2020 2020  : numeric.      
+00004a90: 2020 2020 2020 5661 6c75 6520 666f 7220        Value for 
+00004aa0: 7768 6963 6820 6c6f 672d 7072 6f62 6162  which log-probab
+00004ab0: 696c 6974 7920 6973 2063 616c 6375 6c61  ility is calcula
+00004ac0: 7465 642e 0a0a 2020 2020 2020 2020 5265  ted...        Re
+00004ad0: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00004ae0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5465  -----.        Te
+00004af0: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
+00004b00: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00004b10: 2020 7265 7320 3d20 6661 6374 6c6e 286e    res = factln(n
+00004b20: 2920 2b20 7074 2e73 756d 282d 6661 6374  ) + pt.sum(-fact
+00004b30: 6c6e 2876 616c 7565 2920 2b20 6c6f 6770  ln(value) + logp
+00004b40: 6f77 2870 2c20 7661 6c75 6529 2c20 6178  ow(p, value), ax
+00004b50: 6973 3d2d 3129 0a20 2020 2020 2020 2072  is=-1).        r
+00004b60: 6573 203d 2070 742e 7377 6974 6368 280a  es = pt.switch(.
+00004b70: 2020 2020 2020 2020 2020 2020 7074 2e6f              pt.o
+00004b80: 725f 2870 742e 616e 7928 7074 2e6c 7428  r_(pt.any(pt.lt(
+00004b90: 7661 6c75 652c 2030 292c 2061 7869 733d  value, 0), axis=
+00004ba0: 2d31 292c 2070 742e 6e65 7128 7074 2e73  -1), pt.neq(pt.s
+00004bb0: 756d 2876 616c 7565 2c20 6178 6973 3d2d  um(value, axis=-
+00004bc0: 3129 2c20 6e29 292c 0a20 2020 2020 2020  1), n)),.       
+00004bd0: 2020 2020 202d 6e70 2e69 6e66 2c0a 2020       -np.inf,.  
+00004be0: 2020 2020 2020 2020 2020 7265 732c 0a20            res,. 
+00004bf0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00004c00: 2072 6574 7572 6e20 6368 6563 6b5f 7061   return check_pa
+00004c10: 7261 6d65 7465 7273 280a 2020 2020 2020  rameters(.      
+00004c20: 2020 2020 2020 7265 732c 0a20 2020 2020        res,.     
+00004c30: 2020 2020 2020 2030 203c 3d20 702c 0a20         0 <= p,. 
+00004c40: 2020 2020 2020 2020 2020 2070 203c 3d20             p <= 
+00004c50: 312c 0a20 2020 2020 2020 2020 2020 2070  1,.            p
+00004c60: 742e 6973 636c 6f73 6528 7074 2e73 756d  t.isclose(pt.sum
+00004c70: 2870 2c20 6178 6973 3d2d 3129 2c20 3129  (p, axis=-1), 1)
+00004c80: 2c0a 2020 2020 2020 2020 2020 2020 7074  ,.            pt
+00004c90: 2e67 6528 6e2c 2030 292c 0a20 2020 2020  .ge(n, 0),.     
+00004ca0: 2020 2020 2020 206d 7367 3d22 3020 3c3d         msg="0 <=
+00004cb0: 2070 203c 3d20 312c 2073 756d 2870 2920   p <= 1, sum(p) 
+00004cc0: 3d20 312c 206e 203e 3d20 3022 2c0a 2020  = 1, n >= 0",.  
+00004cd0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
+00004ce0: 4469 7269 6368 6c65 744d 756c 7469 6e6f  DirichletMultino
+00004cf0: 6d69 616c 5256 2852 616e 646f 6d56 6172  mialRV(RandomVar
+00004d00: 6961 626c 6529 3a0a 2020 2020 6e61 6d65  iable):.    name
+00004d10: 203d 2022 6469 7269 6368 6c65 745f 6d75   = "dirichlet_mu
+00004d20: 6c74 696e 6f6d 6961 6c22 0a20 2020 206e  ltinomial".    n
+00004d30: 6469 6d5f 7375 7070 203d 2031 0a20 2020  dim_supp = 1.   
+00004d40: 206e 6469 6d73 5f70 6172 616d 7320 3d20   ndims_params = 
+00004d50: 5b30 2c20 315d 0a20 2020 2064 7479 7065  [0, 1].    dtype
+00004d60: 203d 2022 696e 7436 3422 0a20 2020 205f   = "int64".    _
+00004d70: 7072 696e 745f 6e61 6d65 203d 2028 2244  print_name = ("D
+00004d80: 6972 6963 686c 6574 4d4e 222c 2022 5c5c  irichletMN", "\\
+00004d90: 6f70 6572 6174 6f72 6e61 6d65 7b44 6972  operatorname{Dir
+00004da0: 6963 686c 6574 4d4e 7d22 290a 0a20 2020  ichletMN}")..   
+00004db0: 2064 6566 205f 7375 7070 5f73 6861 7065   def _supp_shape
+00004dc0: 5f66 726f 6d5f 7061 7261 6d73 2873 656c  _from_params(sel
+00004dd0: 662c 2064 6973 745f 7061 7261 6d73 2c20  f, dist_params, 
+00004de0: 7265 705f 7061 7261 6d5f 6964 783d 312c  rep_param_idx=1,
+00004df0: 2070 6172 616d 5f73 6861 7065 733d 4e6f   param_shapes=No
+00004e00: 6e65 293a 0a20 2020 2020 2020 2072 6574  ne):.        ret
+00004e10: 7572 6e20 6465 6661 756c 745f 7375 7070  urn default_supp
+00004e20: 5f73 6861 7065 5f66 726f 6d5f 7061 7261  _shape_from_para
+00004e30: 6d73 280a 2020 2020 2020 2020 2020 2020  ms(.            
+00004e40: 7365 6c66 2e6e 6469 6d5f 7375 7070 2c20  self.ndim_supp, 
+00004e50: 6469 7374 5f70 6172 616d 732c 2072 6570  dist_params, rep
+00004e60: 5f70 6172 616d 5f69 6478 2c20 7061 7261  _param_idx, para
+00004e70: 6d5f 7368 6170 6573 0a20 2020 2020 2020  m_shapes.       
+00004e80: 2029 0a0a 2020 2020 4063 6c61 7373 6d65   )..    @classme
+00004e90: 7468 6f64 0a20 2020 2064 6566 2072 6e67  thod.    def rng
+00004ea0: 5f66 6e28 636c 732c 2072 6e67 2c20 6e2c  _fn(cls, rng, n,
+00004eb0: 2061 2c20 7369 7a65 293a 0a20 2020 2020   a, size):.     
+00004ec0: 2020 2069 6620 6e2e 6e64 696d 203e 2030     if n.ndim > 0
+00004ed0: 206f 7220 612e 6e64 696d 203e 2031 3a0a   or a.ndim > 1:.
+00004ee0: 2020 2020 2020 2020 2020 2020 6e2c 2061              n, a
+00004ef0: 203d 2062 726f 6164 6361 7374 5f70 6172   = broadcast_par
+00004f00: 616d 7328 5b6e 2c20 615d 2c20 636c 732e  ams([n, a], cls.
+00004f10: 6e64 696d 735f 7061 7261 6d73 290a 2020  ndims_params).  
+00004f20: 2020 2020 2020 2020 2020 7369 7a65 203d            size =
+00004f30: 2074 7570 6c65 2873 697a 6520 6f72 2028   tuple(size or (
+00004f40: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00004f50: 6966 2073 697a 653a 0a20 2020 2020 2020  if size:.       
+00004f60: 2020 2020 2020 2020 206e 203d 206e 702e           n = np.
+00004f70: 6272 6f61 6463 6173 745f 746f 286e 2c20  broadcast_to(n, 
+00004f80: 7369 7a65 290a 2020 2020 2020 2020 2020  size).          
+00004f90: 2020 2020 2020 6120 3d20 6e70 2e62 726f        a = np.bro
+00004fa0: 6164 6361 7374 5f74 6f28 612c 2073 697a  adcast_to(a, siz
+00004fb0: 6520 2b20 2861 2e73 6861 7065 5b2d 315d  e + (a.shape[-1]
+00004fc0: 2c29 290a 0a20 2020 2020 2020 2020 2020  ,))..           
+00004fd0: 2072 6573 203d 206e 702e 656d 7074 7928   res = np.empty(
+00004fe0: 612e 7368 6170 6529 0a20 2020 2020 2020  a.shape).       
+00004ff0: 2020 2020 2066 6f72 2069 6478 2069 6e20       for idx in 
+00005000: 6e70 2e6e 6469 6e64 6578 2861 2e73 6861  np.ndindex(a.sha
+00005010: 7065 5b3a 2d31 5d29 3a0a 2020 2020 2020  pe[:-1]):.      
+00005020: 2020 2020 2020 2020 2020 7020 3d20 726e            p = rn
+00005030: 672e 6469 7269 6368 6c65 7428 615b 6964  g.dirichlet(a[id
+00005040: 785d 290a 2020 2020 2020 2020 2020 2020  x]).            
+00005050: 2020 2020 7265 735b 6964 785d 203d 2072      res[idx] = r
+00005060: 6e67 2e6d 756c 7469 6e6f 6d69 616c 286e  ng.multinomial(n
+00005070: 5b69 6478 5d2c 2070 290a 2020 2020 2020  [idx], p).      
+00005080: 2020 2020 2020 7265 7475 726e 2072 6573        return res
+00005090: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+000050a0: 2020 2020 2020 2020 2020 2023 206e 2069             # n i
+000050b0: 7320 6120 7363 616c 6172 2c20 6120 6973  s a scalar, a is
+000050c0: 2061 2031 6420 6172 7261 790a 2020 2020   a 1d array.    
+000050d0: 2020 2020 2020 2020 7020 3d20 726e 672e          p = rng.
+000050e0: 6469 7269 6368 6c65 7428 612c 2073 697a  dirichlet(a, siz
+000050f0: 653d 7369 7a65 2920 2023 2028 7369 7a65  e=size)  # (size
+00005100: 2c20 612e 7368 6170 6529 0a0a 2020 2020  , a.shape)..    
+00005110: 2020 2020 2020 2020 7265 7320 3d20 6e70          res = np
+00005120: 2e65 6d70 7479 2870 2e73 6861 7065 290a  .empty(p.shape).
+00005130: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00005140: 6964 7820 696e 206e 702e 6e64 696e 6465  idx in np.ndinde
+00005150: 7828 702e 7368 6170 655b 3a2d 315d 293a  x(p.shape[:-1]):
+00005160: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005170: 2072 6573 5b69 6478 5d20 3d20 726e 672e   res[idx] = rng.
+00005180: 6d75 6c74 696e 6f6d 6961 6c28 6e2c 2070  multinomial(n, p
+00005190: 5b69 6478 5d29 0a0a 2020 2020 2020 2020  [idx])..        
+000051a0: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+000051b0: 0a64 6972 6963 686c 6574 5f6d 756c 7469  .dirichlet_multi
+000051c0: 6e6f 6d69 616c 203d 2044 6972 6963 686c  nomial = Dirichl
+000051d0: 6574 4d75 6c74 696e 6f6d 6961 6c52 5628  etMultinomialRV(
+000051e0: 290a 0a0a 636c 6173 7320 4469 7269 6368  )...class Dirich
+000051f0: 6c65 744d 756c 7469 6e6f 6d69 616c 2844  letMultinomial(D
+00005200: 6973 6372 6574 6529 3a0a 2020 2020 7222  iscrete):.    r"
+00005210: 2222 4469 7269 6368 6c65 7420 4d75 6c74  ""Dirichlet Mult
+00005220: 696e 6f6d 6961 6c20 6c6f 672d 6c69 6b65  inomial log-like
+00005230: 6c69 686f 6f64 2e0a 0a20 2020 2044 6972  lihood...    Dir
+00005240: 6963 686c 6574 206d 6978 7475 7265 206f  ichlet mixture o
+00005250: 6620 4d75 6c74 696e 6f6d 6961 6c73 2064  f Multinomials d
+00005260: 6973 7472 6962 7574 696f 6e2c 2077 6974  istribution, wit
+00005270: 6820 6120 6d61 7267 696e 616c 697a 6564  h a marginalized
+00005280: 2050 4d46 2e0a 0a20 2020 202e 2e20 6d61   PMF...    .. ma
+00005290: 7468 3a3a 0a0a 2020 2020 2020 2020 6628  th::..        f(
+000052a0: 7820 5c6d 6964 206e 2c20 6129 203d 205c  x \mid n, a) = \
+000052b0: 6672 6163 7b5c 4761 6d6d 6128 6e20 2b20  frac{\Gamma(n + 
+000052c0: 3129 5c47 616d 6d61 285c 7375 6d20 615f  1)\Gamma(\sum a_
+000052d0: 6b29 7d0a 2020 2020 2020 2020 2020 2020  k)}.            
+000052e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052f0: 2020 7b5c 4761 6d6d 6128 6e20 2b20 5c73    {\Gamma(n + \s
+00005300: 756d 2061 5f6b 297d 0a20 2020 2020 2020  um a_k)}.       
 00005310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005320: 7b5c 4761 6d6d 6128 6e20 2b20 5c73 756d  {\Gamma(n + \sum
-00005330: 2061 5f6b 297d 0a20 2020 2020 2020 2020   a_k)}.         
-00005340: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005350: 5c70 726f 645f 7b6b 3d31 7d5e 4b0a 2020  \prod_{k=1}^K.  
-00005360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005370: 2020 2020 2020 205c 6672 6163 7b5c 4761         \frac{\Ga
-00005380: 6d6d 6128 785f 6b20 2b20 2061 5f6b 297d  mma(x_k +  a_k)}
-00005390: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000053a0: 2020 2020 2020 2020 2020 2020 2020 207b                 {
-000053b0: 5c47 616d 6d61 2878 5f6b 202b 2031 295c  \Gamma(x_k + 1)\
-000053c0: 4761 6d6d 6128 615f 6b29 7d0a 0a20 2020  Gamma(a_k)}..   
-000053d0: 203d 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d   ==========  ===
-000053e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000053f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00005400: 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053 7570  ========.    Sup
-00005410: 706f 7274 2020 2020 203a 6d61 7468 3a60  port     :math:`
-00005420: 7820 5c69 6e20 5c7b 302c 2031 2c20 5c6c  x \in \{0, 1, \l
-00005430: 646f 7473 2c20 6e5c 7d60 2073 7563 6820  dots, n\}` such 
-00005440: 7468 6174 0a20 2020 2020 2020 2020 2020  that.           
-00005450: 2020 2020 203a 6d61 7468 3a60 5c73 756d       :math:`\sum
-00005460: 2078 5f69 203d 206e 600a 2020 2020 4d65   x_i = n`.    Me
-00005470: 616e 2020 2020 2020 2020 3a6d 6174 683a  an        :math:
-00005480: 606e 205c 6672 6163 7b61 5f69 7d7b 5c73  `n \frac{a_i}{\s
-00005490: 756d 7b61 5f6b 7d7d 600a 2020 2020 3d3d  um{a_k}}`.    ==
-000054a0: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-000054b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000054c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000054d0: 3d3d 3d3d 3d0a 0a20 2020 2050 6172 616d  =====..    Param
-000054e0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
-000054f0: 2d2d 2d2d 0a20 2020 206e 203a 2074 656e  ----.    n : ten
-00005500: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
-00005510: 2020 2020 2020 2020 546f 7461 6c20 636f          Total co
-00005520: 756e 7473 2069 6e20 6561 6368 2072 6570  unts in each rep
-00005530: 6c69 6361 7465 2028 6e20 3e20 3029 2e0a  licate (n > 0)..
-00005540: 0a20 2020 2061 203a 2074 656e 736f 725f  .    a : tensor_
-00005550: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
-00005560: 2020 2020 2020 4469 7269 6368 6c65 7420        Dirichlet 
-00005570: 636f 6e63 656e 7472 6174 696f 6e20 7061  concentration pa
-00005580: 7261 6d65 7465 7273 2028 6120 3e20 3029  rameters (a > 0)
-00005590: 2e20 5468 6520 6e75 6d62 6572 206f 6620  . The number of 
-000055a0: 6361 7465 676f 7269 6573 2069 7320 6769  categories is gi
-000055b0: 7665 6e20 6279 0a20 2020 2020 2020 2074  ven by.        t
-000055c0: 6865 206c 656e 6774 6820 6f66 2074 6865  he length of the
-000055d0: 206c 6173 7420 6178 6973 2e0a 2020 2020   last axis..    
-000055e0: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
-000055f0: 6469 7269 6368 6c65 745f 6d75 6c74 696e  dirichlet_multin
-00005600: 6f6d 6961 6c0a 0a20 2020 2040 636c 6173  omial..    @clas
-00005610: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
-00005620: 6469 7374 2863 6c73 2c20 6e2c 2061 2c20  dist(cls, n, a, 
-00005630: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00005640: 3a0a 2020 2020 2020 2020 6e20 3d20 696e  :.        n = in
-00005650: 7458 286e 290a 2020 2020 2020 2020 6120  tX(n).        a 
-00005660: 3d20 666c 6f61 7458 2861 290a 0a20 2020  = floatX(a)..   
-00005670: 2020 2020 2072 6574 7572 6e20 7375 7065       return supe
-00005680: 7228 292e 6469 7374 285b 6e2c 2061 5d2c  r().dist([n, a],
-00005690: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
-000056a0: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
-000056b0: 697a 652c 206e 2c20 6129 3a0a 2020 2020  ize, n, a):.    
-000056c0: 2020 2020 7020 3d20 6120 2f20 7074 2e73      p = a / pt.s
-000056d0: 756d 2861 2c20 6178 6973 3d2d 312c 206b  um(a, axis=-1, k
-000056e0: 6565 7064 696d 733d 5472 7565 290a 2020  eepdims=True).  
-000056f0: 2020 2020 2020 7265 7475 726e 206d 6f6d        return mom
-00005700: 656e 7428 4d75 6c74 696e 6f6d 6961 6c2e  ent(Multinomial.
-00005710: 6469 7374 286e 3d6e 2c20 703d 702c 2073  dist(n=n, p=p, s
-00005720: 697a 653d 7369 7a65 2929 0a0a 2020 2020  ize=size))..    
-00005730: 6465 6620 6c6f 6770 2876 616c 7565 2c20  def logp(value, 
-00005740: 6e2c 2061 293a 0a20 2020 2020 2020 2022  n, a):.        "
-00005750: 2222 0a20 2020 2020 2020 2043 616c 6375  "".        Calcu
-00005760: 6c61 7465 206c 6f67 2d70 726f 6261 6269  late log-probabi
-00005770: 6c69 7479 206f 6620 4469 7269 6368 6c65  lity of Dirichle
-00005780: 744d 756c 7469 6e6f 6d69 616c 2064 6973  tMultinomial dis
-00005790: 7472 6962 7574 696f 6e0a 2020 2020 2020  tribution.      
-000057a0: 2020 6174 2073 7065 6369 6669 6564 2076    at specified v
-000057b0: 616c 7565 2e0a 0a20 2020 2020 2020 2050  alue...        P
-000057c0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-000057d0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
-000057e0: 2020 2020 2076 616c 7565 3a20 696e 7465       value: inte
-000057f0: 6765 7220 6172 7261 790a 2020 2020 2020  ger array.      
-00005800: 2020 2020 2020 5661 6c75 6520 666f 7220        Value for 
-00005810: 7768 6963 6820 6c6f 672d 7072 6f62 6162  which log-probab
-00005820: 696c 6974 7920 6973 2063 616c 6375 6c61  ility is calcula
-00005830: 7465 642e 0a0a 2020 2020 2020 2020 5265  ted...        Re
-00005840: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
-00005850: 2d2d 2d2d 2d0a 2020 2020 2020 2020 5465  -----.        Te
-00005860: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
-00005870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005880: 2073 756d 5f61 203d 2061 2e73 756d 2861   sum_a = a.sum(a
-00005890: 7869 733d 2d31 290a 2020 2020 2020 2020  xis=-1).        
-000058a0: 636f 6e73 7420 3d20 2867 616d 6d61 6c6e  const = (gammaln
-000058b0: 286e 202b 2031 2920 2b20 6761 6d6d 616c  (n + 1) + gammal
-000058c0: 6e28 7375 6d5f 6129 2920 2d20 6761 6d6d  n(sum_a)) - gamm
-000058d0: 616c 6e28 6e20 2b20 7375 6d5f 6129 0a20  aln(n + sum_a). 
-000058e0: 2020 2020 2020 2073 6572 6965 7320 3d20         series = 
-000058f0: 6761 6d6d 616c 6e28 7661 6c75 6520 2b20  gammaln(value + 
-00005900: 6129 202d 2028 6761 6d6d 616c 6e28 7661  a) - (gammaln(va
-00005910: 6c75 6520 2b20 3129 202b 2067 616d 6d61  lue + 1) + gamma
-00005920: 6c6e 2861 2929 0a20 2020 2020 2020 2072  ln(a)).        r
-00005930: 6573 203d 2063 6f6e 7374 202b 2073 6572  es = const + ser
-00005940: 6965 732e 7375 6d28 6178 6973 3d2d 3129  ies.sum(axis=-1)
-00005950: 0a0a 2020 2020 2020 2020 7265 7320 3d20  ..        res = 
-00005960: 7074 2e73 7769 7463 6828 0a20 2020 2020  pt.switch(.     
-00005970: 2020 2020 2020 2070 742e 6f72 5f28 0a20         pt.or_(. 
-00005980: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-00005990: 742e 616e 7928 7074 2e6c 7428 7661 6c75  t.any(pt.lt(valu
-000059a0: 652c 2030 292c 2061 7869 733d 2d31 292c  e, 0), axis=-1),
-000059b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000059c0: 2070 742e 6e65 7128 7074 2e73 756d 2876   pt.neq(pt.sum(v
-000059d0: 616c 7565 2c20 6178 6973 3d2d 3129 2c20  alue, axis=-1), 
-000059e0: 6e29 2c0a 2020 2020 2020 2020 2020 2020  n),.            
-000059f0: 292c 0a20 2020 2020 2020 2020 2020 202d  ),.            -
-00005a00: 6e70 2e69 6e66 2c0a 2020 2020 2020 2020  np.inf,.        
-00005a10: 2020 2020 7265 732c 0a20 2020 2020 2020      res,.       
-00005a20: 2029 0a0a 2020 2020 2020 2020 7265 7475   )..        retu
-00005a30: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
-00005a40: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
-00005a50: 2072 6573 2c0a 2020 2020 2020 2020 2020   res,.          
-00005a60: 2020 6120 3e20 302c 0a20 2020 2020 2020    a > 0,.       
-00005a70: 2020 2020 206e 203e 3d20 302c 0a20 2020       n >= 0,.   
-00005a80: 2020 2020 2020 2020 206d 7367 3d22 6120           msg="a 
-00005a90: 3e20 302c 206e 203e 3d20 3022 2c0a 2020  > 0, n >= 0",.  
-00005aa0: 2020 2020 2020 290a 0a0a 636c 6173 7320        )...class 
-00005ab0: 5f4f 7264 6572 6564 4d75 6c74 696e 6f6d  _OrderedMultinom
-00005ac0: 6961 6c28 4d75 6c74 696e 6f6d 6961 6c29  ial(Multinomial)
-00005ad0: 3a0a 2020 2020 7222 2222 0a20 2020 2055  :.    r""".    U
-00005ae0: 6e64 6572 6c79 696e 6720 636c 6173 7320  nderlying class 
-00005af0: 666f 7220 6f72 6465 7265 6420 6d75 6c74  for ordered mult
-00005b00: 696e 6f6d 6961 6c20 6469 7374 7269 6275  inomial distribu
-00005b10: 7469 6f6e 732e 0a20 2020 2053 6565 2064  tions..    See d
-00005b20: 6f63 7320 666f 7220 7468 6520 4f72 6465  ocs for the Orde
-00005b30: 7265 644d 756c 7469 6e6f 6d69 616c 2077  redMultinomial w
-00005b40: 7261 7070 6572 2063 6c61 7373 2066 6f72  rapper class for
-00005b50: 206d 6f72 6520 6465 7461 696c 7320 6f6e   more details on
-00005b60: 2068 6f77 2074 6f20 7573 6520 6974 2069   how to use it i
-00005b70: 6e20 6d6f 6465 6c73 2e0a 2020 2020 2222  n models..    ""
-00005b80: 220a 2020 2020 7276 5f6f 7020 3d20 6d75  ".    rv_op = mu
-00005b90: 6c74 696e 6f6d 6961 6c0a 0a20 2020 2040  ltinomial..    @
-00005ba0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
-00005bb0: 6465 6620 6469 7374 2863 6c73 2c20 6574  def dist(cls, et
-00005bc0: 612c 2063 7574 706f 696e 7473 2c20 6e2c  a, cutpoints, n,
-00005bd0: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00005be0: 293a 0a20 2020 2020 2020 2065 7461 203d  ):.        eta =
-00005bf0: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00005c00: 7269 6162 6c65 2866 6c6f 6174 5828 6574  riable(floatX(et
-00005c10: 6129 290a 2020 2020 2020 2020 6375 7470  a)).        cutp
-00005c20: 6f69 6e74 7320 3d20 7074 2e61 735f 7465  oints = pt.as_te
-00005c30: 6e73 6f72 5f76 6172 6961 626c 6528 6375  nsor_variable(cu
-00005c40: 7470 6f69 6e74 7329 0a20 2020 2020 2020  tpoints).       
-00005c50: 206e 203d 2070 742e 6173 5f74 656e 736f   n = pt.as_tenso
-00005c60: 725f 7661 7269 6162 6c65 2869 6e74 5828  r_variable(intX(
-00005c70: 6e29 290a 0a20 2020 2020 2020 2070 6120  n))..        pa 
-00005c80: 3d20 7369 676d 6f69 6428 6375 7470 6f69  = sigmoid(cutpoi
-00005c90: 6e74 7320 2d20 7074 2e73 6861 7065 5f70  nts - pt.shape_p
-00005ca0: 6164 7269 6768 7428 6574 6129 290a 2020  adright(eta)).  
-00005cb0: 2020 2020 2020 705f 6375 6d20 3d20 7074        p_cum = pt
-00005cc0: 2e63 6f6e 6361 7465 6e61 7465 280a 2020  .concatenate(.  
-00005cd0: 2020 2020 2020 2020 2020 5b0a 2020 2020            [.    
-00005ce0: 2020 2020 2020 2020 2020 2020 7074 2e7a              pt.z
-00005cf0: 6572 6f73 5f6c 696b 6528 7074 2e73 6861  eros_like(pt.sha
-00005d00: 7065 5f70 6164 7269 6768 7428 7061 5b2e  pe_padright(pa[.
-00005d10: 2e2e 2c20 305d 2929 2c0a 2020 2020 2020  .., 0])),.      
-00005d20: 2020 2020 2020 2020 2020 7061 2c0a 2020            pa,.  
-00005d30: 2020 2020 2020 2020 2020 2020 2020 7074                pt
-00005d40: 2e6f 6e65 735f 6c69 6b65 2870 742e 7368  .ones_like(pt.sh
-00005d50: 6170 655f 7061 6472 6967 6874 2870 615b  ape_padright(pa[
-00005d60: 2e2e 2e2c 2030 5d29 292c 0a20 2020 2020  ..., 0])),.     
-00005d70: 2020 2020 2020 205d 2c0a 2020 2020 2020         ],.      
-00005d80: 2020 2020 2020 6178 6973 3d2d 312c 0a20        axis=-1,. 
-00005d90: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00005da0: 2070 203d 2070 5f63 756d 5b2e 2e2e 2c20   p = p_cum[..., 
-00005db0: 313a 5d20 2d20 705f 6375 6d5b 2e2e 2e2c  1:] - p_cum[...,
-00005dc0: 203a 2d31 5d0a 0a20 2020 2020 2020 2072   :-1]..        r
-00005dd0: 6574 7572 6e20 7375 7065 7228 292e 6469  eturn super().di
-00005de0: 7374 286e 2c20 702c 202a 6172 6773 2c20  st(n, p, *args, 
-00005df0: 2a2a 6b77 6172 6773 290a 0a0a 636c 6173  **kwargs)...clas
-00005e00: 7320 4f72 6465 7265 644d 756c 7469 6e6f  s OrderedMultino
-00005e10: 6d69 616c 3a0a 2020 2020 7222 2222 0a20  mial:.    r""". 
-00005e20: 2020 2057 7261 7070 6572 2063 6c61 7373     Wrapper class
-00005e30: 2066 6f72 204f 7264 6572 6564 204d 756c   for Ordered Mul
-00005e40: 7469 6e6f 6d69 616c 2064 6973 7472 6962  tinomial distrib
-00005e50: 7574 696f 6e73 2e0a 0a20 2020 2055 7365  utions...    Use
-00005e60: 6675 6c20 666f 7220 7265 6772 6573 7369  ful for regressi
-00005e70: 6f6e 206f 6e20 6f72 6469 6e61 6c20 6461  on on ordinal da
-00005e80: 7461 2077 686f 7365 2076 616c 7565 7320  ta whose values 
-00005e90: 7261 6e67 650a 2020 2020 6672 6f6d 2031  range.    from 1
-00005ea0: 2074 6f20 4b20 6173 2061 2066 756e 6374   to K as a funct
-00005eb0: 696f 6e20 6f66 2073 6f6d 6520 7072 6564  ion of some pred
-00005ec0: 6963 746f 722c 203a 6d61 7468 3a60 5c65  ictor, :math:`\e
-00005ed0: 7461 602c 2062 7574 0a20 2020 2020 7768  ta`, but.     wh
-00005ee0: 6963 6820 6172 6520 5f61 6767 7265 6761  ich are _aggrega
-00005ef0: 7465 645f 2062 7920 7472 6961 6c2c 206c  ted_ by trial, l
-00005f00: 696b 6520 6d75 6c74 696e 6f6d 6961 6c20  ike multinomial 
-00005f10: 6f62 7365 7276 6174 696f 6e73 2028 696e  observations (in
-00005f20: 0a20 2020 2020 636f 6e74 7261 7374 2074  .     contrast t
-00005f30: 6f20 6070 6d2e 4f72 6465 7265 644c 6f67  o `pm.OrderedLog
-00005f40: 6973 7469 6360 2c20 7768 6963 6820 6f6e  istic`, which on
-00005f50: 6c79 2061 6363 6570 7473 206f 7264 696e  ly accepts ordin
-00005f60: 616c 2064 6174 610a 2020 2020 2069 6e20  al data.     in 
-00005f70: 6120 5f64 6973 6167 6772 6567 6174 6564  a _disaggregated
-00005f80: 5f20 666f 726d 6174 2c20 6c69 6b65 2063  _ format, like c
-00005f90: 6174 6567 6f72 6963 616c 206f 6273 6572  ategorical obser
-00005fa0: 7661 7469 6f6e 7329 2e0a 2020 2020 2054  vations)..     T
-00005fb0: 6865 2063 7574 706f 696e 7473 2c20 3a6d  he cutpoints, :m
-00005fc0: 6174 683a 6063 602c 2073 6570 6172 6174  ath:`c`, separat
-00005fd0: 6520 7768 6963 6820 7261 6e67 6573 206f  e which ranges o
-00005fe0: 6620 3a6d 6174 683a 605c 6574 6160 2061  f :math:`\eta` a
-00005ff0: 7265 0a20 2020 206d 6170 7065 6420 746f  re.    mapped to
-00006000: 2077 6869 6368 206f 6620 7468 6520 4b20   which of the K 
-00006010: 6f62 7365 7276 6564 2064 6570 656e 6465  observed depende
-00006020: 6e74 2076 6172 6961 626c 6573 2e20 5468  nt variables. Th
-00006030: 6520 6e75 6d62 6572 0a20 2020 206f 6620  e number.    of 
-00006040: 6375 7470 6f69 6e74 7320 6973 204b 202d  cutpoints is K -
-00006050: 2031 2e20 4974 2069 7320 7265 636f 6d6d   1. It is recomm
-00006060: 656e 6465 6420 7468 6174 2074 6865 2063  ended that the c
-00006070: 7574 706f 696e 7473 2061 7265 0a20 2020  utpoints are.   
-00006080: 2063 6f6e 7374 7261 696e 6564 2074 6f20   constrained to 
-00006090: 6265 206f 7264 6572 6564 2e0a 0a20 2020  be ordered...   
-000060a0: 202e 2e20 6d61 7468 3a3a 0a0a 2020 2020   .. math::..    
-000060b0: 2020 2066 286b 205c 6d69 6420 5c65 7461     f(k \mid \eta
-000060c0: 2c20 6329 203d 205c 6c65 6674 5c7b 0a20  , c) = \left\{. 
-000060d0: 2020 2020 2020 2020 5c62 6567 696e 7b61          \begin{a
-000060e0: 7272 6179 7d7b 6c7d 0a20 2020 2020 2020  rray}{l}.       
-000060f0: 2020 2020 3120 2d20 5c74 6578 747b 6c6f      1 - \text{lo
-00006100: 6769 747d 5e7b 2d31 7d28 5c65 7461 202d  git}^{-1}(\eta -
-00006110: 2063 5f31 290a 2020 2020 2020 2020 2020   c_1).          
-00006120: 2020 205c 2c2c 205c 7465 7874 7b69 6620     \,, \text{if 
-00006130: 7d20 6b20 3d20 3020 5c5c 0a20 2020 2020  } k = 0 \\.     
-00006140: 2020 2020 2020 5c74 6578 747b 6c6f 6769        \text{logi
-00006150: 747d 5e7b 2d31 7d28 5c65 7461 202d 2063  t}^{-1}(\eta - c
-00006160: 5f7b 6b20 2d20 317d 2920 2d0a 2020 2020  _{k - 1}) -.    
-00006170: 2020 2020 2020 205c 7465 7874 7b6c 6f67         \text{log
-00006180: 6974 7d5e 7b2d 317d 285c 6574 6120 2d20  it}^{-1}(\eta - 
-00006190: 635f 7b6b 7d29 0a20 2020 2020 2020 2020  c_{k}).         
-000061a0: 2020 2020 5c2c 2c20 5c74 6578 747b 6966      \,, \text{if
-000061b0: 207d 2030 203c 206b 203c 204b 205c 5c0a   } 0 < k < K \\.
-000061c0: 2020 2020 2020 2020 2020 205c 7465 7874             \text
-000061d0: 7b6c 6f67 6974 7d5e 7b2d 317d 285c 6574  {logit}^{-1}(\et
-000061e0: 6120 2d20 635f 7b4b 202d 2031 7d29 0a20  a - c_{K - 1}). 
-000061f0: 2020 2020 2020 2020 2020 2020 5c2c 2c20              \,, 
-00006200: 5c74 6578 747b 6966 207d 206b 203d 204b  \text{if } k = K
-00006210: 205c 5c0a 2020 2020 2020 2020 205c 656e   \\.         \en
-00006220: 647b 6172 7261 797d 0a20 2020 2020 2020  d{array}.       
-00006230: 5c72 6967 6874 2e0a 0a20 2020 2050 6172  \right...    Par
-00006240: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00006250: 2d2d 2d2d 2d2d 0a20 2020 2065 7461 203a  ------.    eta :
-00006260: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-00006270: 666c 6f61 740a 2020 2020 2020 2020 5468  float.        Th
-00006280: 6520 7072 6564 6963 746f 722e 0a20 2020  e predictor..   
-00006290: 2063 7574 706f 696e 7473 203a 2074 656e   cutpoints : ten
-000062a0: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
-000062b0: 740a 2020 2020 2020 2020 5468 6520 6c65  t.        The le
-000062c0: 6e67 7468 204b 202d 2031 2061 7272 6179  ngth K - 1 array
-000062d0: 206f 6620 6375 7470 6f69 6e74 7320 7768   of cutpoints wh
-000062e0: 6963 6820 6272 6561 6b20 3a6d 6174 683a  ich break :math:
-000062f0: 605c 6574 6160 2069 6e74 6f0a 2020 2020  `\eta` into.    
-00006300: 2020 2020 7261 6e67 6573 2e20 446f 206e      ranges. Do n
-00006310: 6f74 2065 7870 6c69 6369 746c 7920 7365  ot explicitly se
-00006320: 7420 7468 6520 6669 7273 7420 616e 6420  t the first and 
-00006330: 6c61 7374 2065 6c65 6d65 6e74 7320 6f66  last elements of
-00006340: 0a20 2020 2020 2020 203a 6d61 7468 3a60  .        :math:`
-00006350: 6360 2074 6f20 6e65 6761 7469 7665 2061  c` to negative a
-00006360: 6e64 2070 6f73 6974 6976 6520 696e 6669  nd positive infi
-00006370: 6e69 7479 2e0a 2020 2020 6e20 3a20 7465  nity..    n : te
-00006380: 6e73 6f72 5f6c 696b 6520 6f66 2069 6e74  nsor_like of int
-00006390: 0a20 2020 2020 2020 2054 6865 2074 6f74  .        The tot
-000063a0: 616c 206e 756d 6265 7220 6f66 206d 756c  al number of mul
-000063b0: 7469 6e6f 6d69 616c 2074 7269 616c 732e  tinomial trials.
-000063c0: 0a20 2020 2063 6f6d 7075 7465 5f70 203a  .    compute_p :
-000063d0: 2062 6f6f 6c65 616e 2c20 6465 6661 756c   boolean, defaul
-000063e0: 743d 5472 7565 0a20 2020 2020 2020 2057  t=True.        W
-000063f0: 6865 7468 6572 2074 6f20 636f 6d70 7574  hether to comput
-00006400: 6520 616e 6420 7374 6f72 6520 696e 2074  e and store in t
-00006410: 6865 2074 7261 6365 2074 6865 2069 6e66  he trace the inf
-00006420: 6572 7265 6420 7072 6f62 6162 696c 6974  erred probabilit
-00006430: 6965 7320 6f66 2065 6163 680a 2020 2020  ies of each.    
-00006440: 2020 2020 6361 7465 676f 7269 6573 2c0a      categories,.
-00006450: 2020 2020 2020 2020 6261 7365 6420 6f6e          based on
-00006460: 2074 6865 2063 7574 706f 696e 7473 2720   the cutpoints' 
-00006470: 7661 6c75 6573 2e20 4465 6661 756c 7473  values. Defaults
-00006480: 2074 6f20 5472 7565 2e0a 2020 2020 2020   to True..      
-00006490: 2020 4d69 6768 7420 6265 2075 7365 6675    Might be usefu
-000064a0: 6c20 746f 2064 6973 6162 6c65 2069 7420  l to disable it 
-000064b0: 6966 206d 656d 6f72 7920 7573 6167 6520  if memory usage 
-000064c0: 6973 206f 6620 696e 7465 7265 7374 2e0a  is of interest..
-000064d0: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-000064e0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e    --------.    .
-000064f0: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2070  . code-block:: p
-00006500: 7974 686f 6e0a 0a20 2020 2020 2020 2023  ython..        #
-00006510: 2047 656e 6572 6174 6520 6461 7461 2066   Generate data f
-00006520: 6f72 2061 2073 696d 706c 6520 3120 6469  or a simple 1 di
-00006530: 6d65 6e73 696f 6e61 6c20 6578 616d 706c  mensional exampl
-00006540: 6520 7072 6f62 6c65 6d0a 2020 2020 2020  e problem.      
-00006550: 2020 7472 7565 5f63 756d 5f70 203d 206e    true_cum_p = n
-00006560: 702e 6172 7261 7928 5b30 2e31 2c20 302e  p.array([0.1, 0.
-00006570: 3135 2c20 302e 3235 2c20 302e 3530 2c20  15, 0.25, 0.50, 
-00006580: 302e 3635 2c20 302e 3930 2c20 312e 305d  0.65, 0.90, 1.0]
-00006590: 290a 2020 2020 2020 2020 7472 7565 5f70  ).        true_p
-000065a0: 203d 206e 702e 6873 7461 636b 285b 7472   = np.hstack([tr
-000065b0: 7565 5f63 756d 5f70 5b30 5d2c 2074 7275  ue_cum_p[0], tru
-000065c0: 655f 6375 6d5f 705b 313a 5d20 2d20 7472  e_cum_p[1:] - tr
-000065d0: 7565 5f63 756d 5f70 5b3a 2d31 5d5d 290a  ue_cum_p[:-1]]).
-000065e0: 2020 2020 2020 2020 6661 6b65 5f65 6c65          fake_ele
-000065f0: 6374 696f 6e73 203d 206e 702e 7261 6e64  ctions = np.rand
-00006600: 6f6d 2e6d 756c 7469 6e6f 6d69 616c 286e  om.multinomial(n
-00006610: 3d31 5f30 3030 2c20 7076 616c 733d 7472  =1_000, pvals=tr
-00006620: 7565 5f70 2c20 7369 7a65 3d36 3029 0a0a  ue_p, size=60)..
-00006630: 2020 2020 2020 2020 2320 4f72 6465 7265          # Ordere
-00006640: 6420 6d75 6c74 696e 6f6d 6961 6c20 7265  d multinomial re
-00006650: 6772 6573 7369 6f6e 0a20 2020 2020 2020  gression.       
-00006660: 2077 6974 6820 706d 2e4d 6f64 656c 2829   with pm.Model()
-00006670: 2061 7320 6d6f 6465 6c3a 0a20 2020 2020   as model:.     
-00006680: 2020 2020 2020 2063 7574 706f 696e 7473         cutpoints
-00006690: 203d 2070 6d2e 4e6f 726d 616c 280a 2020   = pm.Normal(.  
-000066a0: 2020 2020 2020 2020 2020 2020 2020 2263                "c
-000066b0: 7574 706f 696e 7473 222c 0a20 2020 2020  utpoints",.     
-000066c0: 2020 2020 2020 2020 2020 206d 753d 6e70             mu=np
-000066d0: 2e61 7261 6e67 6528 3629 202d 2032 2e35  .arange(6) - 2.5
-000066e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000066f0: 2020 7369 676d 613d 312e 352c 0a20 2020    sigma=1.5,.   
-00006700: 2020 2020 2020 2020 2020 2020 2069 6e69               ini
-00006710: 7476 616c 3d6e 702e 6172 616e 6765 2836  tval=np.arange(6
-00006720: 2920 2d20 322e 352c 0a20 2020 2020 2020  ) - 2.5,.       
-00006730: 2020 2020 2020 2020 2074 7261 6e73 666f           transfo
-00006740: 726d 3d70 6d2e 6469 7374 7269 6275 7469  rm=pm.distributi
-00006750: 6f6e 732e 7472 616e 7366 6f72 6d73 2e6f  ons.transforms.o
-00006760: 7264 6572 6564 2c0a 2020 2020 2020 2020  rdered,.        
-00006770: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
-00006780: 2020 2070 6d2e 4f72 6465 7265 644d 756c     pm.OrderedMul
-00006790: 7469 6e6f 6d69 616c 280a 2020 2020 2020  tinomial(.      
-000067a0: 2020 2020 2020 2020 2020 2272 6573 756c            "resul
-000067b0: 7473 222c 0a20 2020 2020 2020 2020 2020  ts",.           
-000067c0: 2020 2020 2065 7461 3d30 2e30 2c0a 2020       eta=0.0,.  
-000067d0: 2020 2020 2020 2020 2020 2020 2020 6375                cu
-000067e0: 7470 6f69 6e74 733d 6375 7470 6f69 6e74  tpoints=cutpoint
-000067f0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
-00006800: 2020 206e 3d66 616b 655f 656c 6563 7469     n=fake_electi
-00006810: 6f6e 732e 7375 6d28 3129 2c0a 2020 2020  ons.sum(1),.    
-00006820: 2020 2020 2020 2020 2020 2020 6f62 7365              obse
-00006830: 7276 6564 3d66 616b 655f 656c 6563 7469  rved=fake_electi
-00006840: 6f6e 732c 0a20 2020 2020 2020 2020 2020  ons,.           
-00006850: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00006860: 7472 6163 6520 3d20 706d 2e73 616d 706c  trace = pm.sampl
-00006870: 6528 290a 0a20 2020 2020 2020 2023 2050  e()..        # P
-00006880: 6c6f 7420 7468 6520 7265 7375 6c74 730a  lot the results.
-00006890: 2020 2020 2020 2020 6172 7669 7a2e 706c          arviz.pl
-000068a0: 6f74 5f70 6f73 7465 7269 6f72 2874 7261  ot_posterior(tra
-000068b0: 6365 5f31 325f 342c 2076 6172 5f6e 616d  ce_12_4, var_nam
-000068c0: 6573 3d5b 2263 6f6d 706c 6574 655f 7022  es=["complete_p"
-000068d0: 5d2c 2072 6566 5f76 616c 3d6c 6973 7428  ], ref_val=list(
-000068e0: 7472 7565 5f70 2929 3b0a 2020 2020 2222  true_p));.    ""
-000068f0: 220a 0a20 2020 2064 6566 205f 5f6e 6577  "..    def __new
-00006900: 5f5f 2863 6c73 2c20 6e61 6d65 2c20 2a61  __(cls, name, *a
-00006910: 7267 732c 2063 6f6d 7075 7465 5f70 3d54  rgs, compute_p=T
-00006920: 7275 652c 202a 2a6b 7761 7267 7329 3a0a  rue, **kwargs):.
-00006930: 2020 2020 2020 2020 6f75 745f 7276 203d          out_rv =
-00006940: 205f 4f72 6465 7265 644d 756c 7469 6e6f   _OrderedMultino
-00006950: 6d69 616c 286e 616d 652c 202a 6172 6773  mial(name, *args
-00006960: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-00006970: 2020 2020 6966 2063 6f6d 7075 7465 5f70      if compute_p
-00006980: 3a0a 2020 2020 2020 2020 2020 2020 706d  :.            pm
-00006990: 2e44 6574 6572 6d69 6e69 7374 6963 2866  .Deterministic(f
-000069a0: 227b 6e61 6d65 7d5f 7072 6f62 7322 2c20  "{name}_probs", 
-000069b0: 6f75 745f 7276 2e6f 776e 6572 2e69 6e70  out_rv.owner.inp
-000069c0: 7574 735b 345d 2c20 6469 6d73 3d6b 7761  uts[4], dims=kwa
-000069d0: 7267 732e 6765 7428 2264 696d 7322 2929  rgs.get("dims"))
-000069e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000069f0: 6f75 745f 7276 0a0a 2020 2020 4063 6c61  out_rv..    @cla
-00006a00: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00006a10: 2064 6973 7428 636c 732c 202a 6172 6773   dist(cls, *args
-00006a20: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
-00006a30: 2020 2020 2072 6574 7572 6e20 5f4f 7264       return _Ord
-00006a40: 6572 6564 4d75 6c74 696e 6f6d 6961 6c2e  eredMultinomial.
-00006a50: 6469 7374 282a 6172 6773 2c20 2a2a 6b77  dist(*args, **kw
-00006a60: 6172 6773 290a 0a0a 6465 6620 706f 7364  args)...def posd
-00006a70: 6566 2841 4129 3a0a 2020 2020 7472 793a  ef(AA):.    try:
-00006a80: 0a20 2020 2020 2020 206c 696e 616c 672e  .        linalg.
-00006a90: 6368 6f6c 6573 6b79 2841 4129 0a20 2020  cholesky(AA).   
-00006aa0: 2020 2020 2072 6574 7572 6e20 310a 2020       return 1.  
-00006ab0: 2020 6578 6365 7074 206c 696e 616c 672e    except linalg.
-00006ac0: 4c69 6e41 6c67 4572 726f 723a 0a20 2020  LinAlgError:.   
-00006ad0: 2020 2020 2072 6574 7572 6e20 300a 0a0a       return 0...
-00006ae0: 636c 6173 7320 506f 7344 6566 4d61 7472  class PosDefMatr
-00006af0: 6978 284f 7029 3a0a 2020 2020 2222 220a  ix(Op):.    """.
-00006b00: 2020 2020 4368 6563 6b20 6966 2069 6e70      Check if inp
-00006b10: 7574 2069 7320 706f 7369 7469 7665 2064  ut is positive d
-00006b20: 6566 696e 6974 652e 2049 6e70 7574 2073  efinite. Input s
-00006b30: 686f 756c 6420 6265 2061 2073 7175 6172  hould be a squar
-00006b40: 6520 6d61 7472 6978 2e0a 0a20 2020 2022  e matrix...    "
-00006b50: 2222 0a0a 2020 2020 2320 5072 6f70 6572  ""..    # Proper
-00006b60: 7469 6573 2061 7474 7269 6275 7465 0a20  ties attribute. 
-00006b70: 2020 205f 5f70 726f 7073 5f5f 203d 2028     __props__ = (
-00006b80: 290a 0a20 2020 2023 2043 6f6d 7075 6c73  )..    # Compuls
-00006b90: 6f72 7920 6966 2069 7479 7065 7320 616e  ory if itypes an
-00006ba0: 6420 6f74 7970 6573 2061 7265 206e 6f74  d otypes are not
-00006bb0: 2064 6566 696e 6564 0a0a 2020 2020 6465   defined..    de
-00006bc0: 6620 6d61 6b65 5f6e 6f64 6528 7365 6c66  f make_node(self
-00006bd0: 2c20 7829 3a0a 2020 2020 2020 2020 7820  , x):.        x 
-00006be0: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
-00006bf0: 6172 6961 626c 6528 7829 0a20 2020 2020  ariable(x).     
-00006c00: 2020 2061 7373 6572 7420 782e 6e64 696d     assert x.ndim
-00006c10: 203d 3d20 320a 2020 2020 2020 2020 6f20   == 2.        o 
-00006c20: 3d20 5465 6e73 6f72 5479 7065 2864 7479  = TensorType(dty
-00006c30: 7065 3d22 696e 7438 222c 2073 6861 7065  pe="int8", shape
-00006c40: 3d5b 5d29 2829 0a20 2020 2020 2020 2072  =[])().        r
-00006c50: 6574 7572 6e20 4170 706c 7928 7365 6c66  eturn Apply(self
-00006c60: 2c20 5b78 5d2c 205b 6f5d 290a 0a20 2020  , [x], [o])..   
-00006c70: 2023 2050 7974 686f 6e20 696d 706c 656d   # Python implem
-00006c80: 656e 7461 7469 6f6e 3a0a 2020 2020 6465  entation:.    de
-00006c90: 6620 7065 7266 6f72 6d28 7365 6c66 2c20  f perform(self, 
-00006ca0: 6e6f 6465 2c20 696e 7075 7473 2c20 6f75  node, inputs, ou
-00006cb0: 7470 7574 7329 3a0a 2020 2020 2020 2020  tputs):.        
-00006cc0: 2878 2c29 203d 2069 6e70 7574 730a 2020  (x,) = inputs.  
-00006cd0: 2020 2020 2020 287a 2c29 203d 206f 7574        (z,) = out
-00006ce0: 7075 7473 0a20 2020 2020 2020 2074 7279  puts.        try
-00006cf0: 3a0a 2020 2020 2020 2020 2020 2020 7a5b  :.            z[
-00006d00: 305d 203d 206e 702e 6172 7261 7928 706f  0] = np.array(po
-00006d10: 7364 6566 2878 292c 2064 7479 7065 3d22  sdef(x), dtype="
-00006d20: 696e 7438 2229 0a20 2020 2020 2020 2065  int8").        e
-00006d30: 7863 6570 7420 4578 6365 7074 696f 6e3a  xcept Exception:
-00006d40: 0a20 2020 2020 2020 2020 2020 2070 6d2e  .            pm.
-00006d50: 5f6c 6f67 2e65 7863 6570 7469 6f6e 2822  _log.exception("
-00006d60: 4661 696c 6564 2074 6f20 6368 6563 6b20  Failed to check 
-00006d70: 6966 2025 7320 706f 7369 7469 7665 2064  if %s positive d
-00006d80: 6566 696e 6974 6522 2c20 7829 0a20 2020  efinite", x).   
-00006d90: 2020 2020 2020 2020 2072 6169 7365 0a0a           raise..
-00006da0: 2020 2020 6465 6620 696e 6665 725f 7368      def infer_sh
-00006db0: 6170 6528 7365 6c66 2c20 6667 7261 7068  ape(self, fgraph
-00006dc0: 2c20 6e6f 6465 2c20 7368 6170 6573 293a  , node, shapes):
-00006dd0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00006de0: 5b5b 5d5d 0a0a 2020 2020 6465 6620 6772  [[]]..    def gr
-00006df0: 6164 2873 656c 662c 2069 6e70 2c20 6772  ad(self, inp, gr
-00006e00: 6164 7329 3a0a 2020 2020 2020 2020 2878  ads):.        (x
-00006e10: 2c29 203d 2069 6e70 0a20 2020 2020 2020  ,) = inp.       
-00006e20: 2072 6574 7572 6e20 5b78 2e7a 6572 6f73   return [x.zeros
-00006e30: 5f6c 696b 6528 7079 7465 6e73 6f72 2e63  _like(pytensor.c
-00006e40: 6f6e 6669 672e 666c 6f61 7458 295d 0a0a  onfig.floatX)]..
-00006e50: 2020 2020 6465 6620 5f5f 7374 725f 5f28      def __str__(
-00006e60: 7365 6c66 293a 0a20 2020 2020 2020 2072  self):.        r
-00006e70: 6574 7572 6e20 224d 6174 7269 7849 7350  eturn "MatrixIsP
-00006e80: 6f73 6974 6976 6544 6566 696e 6974 6522  ositiveDefinite"
-00006e90: 0a0a 0a6d 6174 7269 785f 706f 735f 6465  ...matrix_pos_de
-00006ea0: 6620 3d20 506f 7344 6566 4d61 7472 6978  f = PosDefMatrix
-00006eb0: 2829 0a0a 0a63 6c61 7373 2057 6973 6861  ()...class Wisha
-00006ec0: 7274 5256 2852 616e 646f 6d56 6172 6961  rtRV(RandomVaria
-00006ed0: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
-00006ee0: 2022 7769 7368 6172 7422 0a20 2020 206e   "wishart".    n
-00006ef0: 6469 6d5f 7375 7070 203d 2032 0a20 2020  dim_supp = 2.   
-00006f00: 206e 6469 6d73 5f70 6172 616d 7320 3d20   ndims_params = 
-00006f10: 5b30 2c20 325d 0a20 2020 2064 7479 7065  [0, 2].    dtype
-00006f20: 203d 2022 666c 6f61 7458 220a 2020 2020   = "floatX".    
-00006f30: 5f70 7269 6e74 5f6e 616d 6520 3d20 2822  _print_name = ("
-00006f40: 5769 7368 6172 7422 2c20 225c 5c6f 7065  Wishart", "\\ope
-00006f50: 7261 746f 726e 616d 657b 5769 7368 6172  ratorname{Wishar
-00006f60: 747d 2229 0a0a 2020 2020 6465 6620 5f73  t}")..    def _s
-00006f70: 7570 705f 7368 6170 655f 6672 6f6d 5f70  upp_shape_from_p
-00006f80: 6172 616d 7328 7365 6c66 2c20 6469 7374  arams(self, dist
-00006f90: 5f70 6172 616d 732c 2072 6570 5f70 6172  _params, rep_par
-00006fa0: 616d 5f69 6478 3d31 2c20 7061 7261 6d5f  am_idx=1, param_
-00006fb0: 7368 6170 6573 3d4e 6f6e 6529 3a0a 2020  shapes=None):.  
-00006fc0: 2020 2020 2020 2320 5468 6520 7368 6170        # The shap
-00006fd0: 6520 6f66 2073 6563 6f6e 6420 7061 7261  e of second para
-00006fe0: 6d65 7465 7220 6056 6020 6465 6669 6e65  meter `V` define
-00006ff0: 7320 7468 6520 7368 6170 6520 6f66 2074  s the shape of t
-00007000: 6865 206f 7574 7075 742e 0a20 2020 2020  he output..     
-00007010: 2020 2072 6574 7572 6e20 6469 7374 5f70     return dist_p
-00007020: 6172 616d 735b 315d 2e73 6861 7065 5b2d  arams[1].shape[-
-00007030: 323a 5d0a 0a20 2020 2040 636c 6173 736d  2:]..    @classm
-00007040: 6574 686f 640a 2020 2020 6465 6620 726e  ethod.    def rn
-00007050: 675f 666e 2863 6c73 2c20 726e 672c 206e  g_fn(cls, rng, n
-00007060: 752c 2056 2c20 7369 7a65 293a 0a20 2020  u, V, size):.   
-00007070: 2020 2020 2073 6369 7079 5f73 697a 6520       scipy_size 
-00007080: 3d20 7369 7a65 2069 6620 7369 7a65 2065  = size if size e
-00007090: 6c73 6520 3120 2023 2044 6566 6175 6c74  lse 1  # Default
-000070a0: 2073 697a 6520 666f 7220 5363 6970 7927   size for Scipy'
-000070b0: 7320 7769 7368 6172 742e 7276 7320 6973  s wishart.rvs is
-000070c0: 2031 0a20 2020 2020 2020 2072 6573 756c   1.        resul
-000070d0: 7420 3d20 7374 6174 732e 7769 7368 6172  t = stats.wishar
-000070e0: 742e 7276 7328 696e 7428 6e75 292c 2056  t.rvs(int(nu), V
-000070f0: 2c20 7369 7a65 3d73 6369 7079 5f73 697a  , size=scipy_siz
-00007100: 652c 2072 616e 646f 6d5f 7374 6174 653d  e, random_state=
-00007110: 726e 6729 0a20 2020 2020 2020 2069 6620  rng).        if 
-00007120: 7369 7a65 203d 3d20 2831 2c29 3a0a 2020  size == (1,):.  
-00007130: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00007140: 2072 6573 756c 745b 6e70 2e6e 6577 6178   result[np.newax
-00007150: 6973 2c20 2e2e 2e5d 0a20 2020 2020 2020  is, ...].       
-00007160: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00007170: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00007180: 0a0a 0a77 6973 6861 7274 203d 2057 6973  ...wishart = Wis
-00007190: 6861 7274 5256 2829 0a0a 0a63 6c61 7373  hartRV()...class
-000071a0: 2057 6973 6861 7274 2843 6f6e 7469 6e75   Wishart(Continu
-000071b0: 6f75 7329 3a0a 2020 2020 7222 2222 0a20  ous):.    r""". 
-000071c0: 2020 2057 6973 6861 7274 206c 6f67 2d6c     Wishart log-l
-000071d0: 696b 656c 6968 6f6f 642e 0a0a 2020 2020  ikelihood...    
-000071e0: 5468 6520 5769 7368 6172 7420 6469 7374  The Wishart dist
-000071f0: 7269 6275 7469 6f6e 2069 7320 7468 6520  ribution is the 
-00007200: 7072 6f62 6162 696c 6974 7920 6469 7374  probability dist
-00007210: 7269 6275 7469 6f6e 206f 6620 7468 650a  ribution of the.
-00007220: 2020 2020 6d61 7869 6d75 6d2d 6c69 6b65      maximum-like
-00007230: 6c69 686f 6f64 2065 7374 696d 6174 6f72  lihood estimator
-00007240: 2028 4d4c 4529 206f 6620 7468 6520 7072   (MLE) of the pr
-00007250: 6563 6973 696f 6e20 6d61 7472 6978 206f  ecision matrix o
-00007260: 6620 610a 2020 2020 6d75 6c74 6976 6172  f a.    multivar
-00007270: 6961 7465 206e 6f72 6d61 6c20 6469 7374  iate normal dist
-00007280: 7269 6275 7469 6f6e 2e20 2049 6620 563d  ribution.  If V=
-00007290: 312c 2074 6865 2064 6973 7472 6962 7574  1, the distribut
-000072a0: 696f 6e20 6973 0a20 2020 2069 6465 6e74  ion is.    ident
-000072b0: 6963 616c 2074 6f20 7468 6520 6368 692d  ical to the chi-
-000072c0: 7371 7561 7265 2064 6973 7472 6962 7574  square distribut
-000072d0: 696f 6e20 7769 7468 206e 7520 6465 6772  ion with nu degr
-000072e0: 6565 7320 6f66 0a20 2020 2066 7265 6564  ees of.    freed
-000072f0: 6f6d 2e0a 0a20 2020 202e 2e20 6d61 7468  om...    .. math
-00007300: 3a3a 0a0a 2020 2020 2020 2066 2858 205c  ::..       f(X \
-00007310: 6d69 6420 6e75 2c20 5429 203d 0a20 2020  mid nu, T) =.   
-00007320: 2020 2020 2020 2020 5c66 7261 637b 7b5c          \frac{{\
-00007330: 6d69 6420 5420 5c6d 6964 7d5e 7b6e 752f  mid T \mid}^{nu/
-00007340: 327d 7b5c 6d69 6420 5820 5c6d 6964 7d5e  2}{\mid X \mid}^
-00007350: 7b28 6e75 2d6b 2d31 292f 327d 7d7b 325e  {(nu-k-1)/2}}{2^
-00007360: 7b6e 7520 6b2f 327d 0a20 2020 2020 2020  {nu k/2}.       
-00007370: 2020 2020 5c47 616d 6d61 5f70 286e 752f      \Gamma_p(nu/
-00007380: 3229 7d20 5c65 7870 5c6c 6566 745c 7b20  2)} \exp\left\{ 
-00007390: 2d5c 6672 6163 7b31 7d7b 327d 2054 7228  -\frac{1}{2} Tr(
-000073a0: 5458 2920 5c72 6967 6874 5c7d 0a0a 2020  TX) \right\}..  
-000073b0: 2020 7768 6572 6520 3a6d 6174 683a 606b    where :math:`k
-000073c0: 6020 6973 2074 6865 2072 616e 6b20 6f66  ` is the rank of
-000073d0: 203a 6d61 7468 3a60 5860 2e0a 0a20 2020   :math:`X`...   
-000073e0: 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d   ========  =====
-000073f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00007410: 3d3d 3d3d 0a20 2020 2053 7570 706f 7274  ====.    Support
-00007420: 2020 203a 6d61 7468 3a60 5828 7020 7820     :math:`X(p x 
-00007430: 7029 6020 706f 7369 7469 7665 2064 6566  p)` positive def
-00007440: 696e 6974 6520 6d61 7472 6978 0a20 2020  inite matrix.   
-00007450: 204d 6561 6e20 2020 2020 203a 6d61 7468   Mean      :math
-00007460: 3a60 6e75 2056 600a 2020 2020 5661 7269  :`nu V`.    Vari
-00007470: 616e 6365 2020 3a6d 6174 683a 606e 7520  ance  :math:`nu 
-00007480: 2876 5f7b 696a 7d5e 3220 2b20 765f 7b69  (v_{ij}^2 + v_{i
-00007490: 697d 2076 5f7b 6a6a 7d29 600a 2020 2020  i} v_{jj})`.    
-000074a0: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-000074b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000074c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000074d0: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
-000074e0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-000074f0: 2d2d 0a20 2020 206e 7520 3a20 7465 6e73  --.    nu : tens
-00007500: 6f72 5f6c 696b 6520 6f66 2069 6e74 0a20  or_like of int. 
-00007510: 2020 2020 2020 2044 6567 7265 6573 206f         Degrees o
-00007520: 6620 6672 6565 646f 6d2c 203e 2030 2e0a  f freedom, > 0..
-00007530: 2020 2020 5620 3a20 7465 6e73 6f72 5f6c      V : tensor_l
-00007540: 696b 6520 6f66 2066 6c6f 6174 0a20 2020  ike of float.   
-00007550: 2020 2020 2070 2078 2070 2070 6f73 6974       p x p posit
-00007560: 6976 6520 6465 6669 6e69 7465 206d 6174  ive definite mat
-00007570: 7269 782e 0a0a 2020 2020 4e6f 7465 730a  rix...    Notes.
-00007580: 2020 2020 2d2d 2d2d 2d0a 2020 2020 5468      -----.    Th
-00007590: 6973 2064 6973 7472 6962 7574 696f 6e20  is distribution 
-000075a0: 6973 2075 6e75 7361 626c 6520 696e 2061  is unusable in a
-000075b0: 2050 794d 4320 6d6f 6465 6c2e 2059 6f75   PyMC model. You
-000075c0: 2073 686f 756c 6420 696e 7374 6561 640a   should instead.
-000075d0: 2020 2020 7573 6520 4c4b 4a43 686f 6c65      use LKJChole
-000075e0: 736b 7943 6f76 206f 7220 4c4b 4a43 6f72  skyCov or LKJCor
-000075f0: 722e 0a20 2020 2022 2222 0a20 2020 2072  r..    """.    r
-00007600: 765f 6f70 203d 2077 6973 6861 7274 0a0a  v_op = wishart..
-00007610: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-00007620: 0a20 2020 2064 6566 2064 6973 7428 636c  .    def dist(cl
-00007630: 732c 206e 752c 2056 2c20 2a61 7267 732c  s, nu, V, *args,
-00007640: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00007650: 2020 2020 6e75 203d 2070 742e 6173 5f74      nu = pt.as_t
-00007660: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
-00007670: 6e74 5828 6e75 2929 0a20 2020 2020 2020  ntX(nu)).       
-00007680: 2056 203d 2070 742e 6173 5f74 656e 736f   V = pt.as_tenso
-00007690: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
-000076a0: 5828 5629 290a 0a20 2020 2020 2020 2077  X(V))..        w
-000076b0: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
-000076c0: 2020 2020 2020 2020 2020 2254 6865 2057            "The W
-000076d0: 6973 6861 7274 2064 6973 7472 6962 7574  ishart distribut
-000076e0: 696f 6e20 6361 6e20 6375 7272 656e 746c  ion can currentl
-000076f0: 7920 6e6f 7420 6265 2075 7365 6420 220a  y not be used ".
-00007700: 2020 2020 2020 2020 2020 2020 2266 6f72              "for
-00007710: 204d 434d 4320 7361 6d70 6c69 6e67 2e20   MCMC sampling. 
-00007720: 5468 6520 7072 6f62 6162 696c 6974 7920  The probability 
-00007730: 6f66 2073 616d 706c 696e 6720 6120 220a  of sampling a ".
-00007740: 2020 2020 2020 2020 2020 2020 2273 796d              "sym
-00007750: 6d65 7472 6963 206d 6174 7269 7820 6973  metric matrix is
-00007760: 2062 6173 6963 616c 6c79 207a 6572 6f2e   basically zero.
-00007770: 2049 6e73 7465 6164 2c20 706c 6561 7365   Instead, please
-00007780: 2022 0a20 2020 2020 2020 2020 2020 2022   ".            "
-00007790: 7573 6520 4c4b 4a43 686f 6c65 736b 7943  use LKJCholeskyC
-000077a0: 6f76 206f 7220 4c4b 4a43 6f72 722e 2046  ov or LKJCorr. F
-000077b0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-000077c0: 696f 6e20 220a 2020 2020 2020 2020 2020  ion ".          
-000077d0: 2020 226f 6e20 7468 6520 6973 7375 6573    "on the issues
-000077e0: 2073 7572 726f 756e 6469 6e67 2074 6865   surrounding the
-000077f0: 2057 6973 6861 7274 2073 6565 2068 6572   Wishart see her
-00007800: 653a 2022 0a20 2020 2020 2020 2020 2020  e: ".           
-00007810: 2022 6874 7470 733a 2f2f 6769 7468 7562   "https://github
-00007820: 2e63 6f6d 2f70 796d 632d 6465 7673 2f70  .com/pymc-devs/p
-00007830: 796d 632f 6973 7375 6573 2f35 3338 2e22  ymc/issues/538."
-00007840: 2c0a 2020 2020 2020 2020 2020 2020 5573  ,.            Us
-00007850: 6572 5761 726e 696e 672c 0a20 2020 2020  erWarning,.     
-00007860: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-00007870: 6d65 616e 203d 206e 7520 2a20 560a 2020  mean = nu * V.  
-00007880: 2020 2020 2020 2320 7020 3d20 562e 7368        # p = V.sh
-00007890: 6170 655b 305d 0a20 2020 2020 2020 2023  ape[0].        #
-000078a0: 206d 6f64 6520 3d20 7074 2e73 7769 7463   mode = pt.switc
-000078b0: 6828 7074 2e67 6528 6e75 2c20 7020 2b20  h(pt.ge(nu, p + 
-000078c0: 3129 2c20 286e 7520 2d20 7020 2d20 3129  1), (nu - p - 1)
-000078d0: 202a 2056 2c20 6e70 2e6e 616e 290a 2020   * V, np.nan).  
-000078e0: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-000078f0: 6572 2829 2e64 6973 7428 5b6e 752c 2056  er().dist([nu, V
-00007900: 5d2c 202a 6172 6773 2c20 2a2a 6b77 6172  ], *args, **kwar
-00007910: 6773 290a 0a20 2020 2064 6566 206c 6f67  gs)..    def log
-00007920: 7028 582c 206e 752c 2056 293a 0a20 2020  p(X, nu, V):.   
-00007930: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007940: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
-00007950: 726f 6261 6269 6c69 7479 206f 6620 5769  robability of Wi
-00007960: 7368 6172 7420 6469 7374 7269 6275 7469  shart distributi
-00007970: 6f6e 0a20 2020 2020 2020 2061 7420 7370  on.        at sp
-00007980: 6563 6966 6965 6420 7661 6c75 652e 0a0a  ecified value...
-00007990: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000079a0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000079b0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 583a  -----.        X:
-000079c0: 206e 756d 6572 6963 0a20 2020 2020 2020   numeric.       
-000079d0: 2020 2020 2056 616c 7565 2066 6f72 2077       Value for w
-000079e0: 6869 6368 206c 6f67 2d70 726f 6261 6269  hich log-probabi
-000079f0: 6c69 7479 2069 7320 6361 6c63 756c 6174  lity is calculat
-00007a00: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
-00007a10: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00007a20: 2d2d 2d2d 0a20 2020 2020 2020 2054 656e  ----.        Ten
-00007a30: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
-00007a40: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00007a50: 2070 203d 2056 2e73 6861 7065 5b30 5d0a   p = V.shape[0].
-00007a60: 0a20 2020 2020 2020 2049 5649 203d 2064  .        IVI = d
-00007a70: 6574 2856 290a 2020 2020 2020 2020 4958  et(V).        IX
-00007a80: 4920 3d20 6465 7428 5829 0a0a 2020 2020  I = det(X)..    
-00007a90: 2020 2020 7265 7475 726e 2063 6865 636b      return check
-00007aa0: 5f70 6172 616d 6574 6572 7328 0a20 2020  _parameters(.   
-00007ab0: 2020 2020 2020 2020 2028 0a20 2020 2020           (.     
-00007ac0: 2020 2020 2020 2020 2020 2028 6e75 202d             (nu -
-00007ad0: 2070 202d 2031 2920 2a20 7074 2e6c 6f67   p - 1) * pt.log
-00007ae0: 2849 5849 290a 2020 2020 2020 2020 2020  (IXI).          
-00007af0: 2020 2020 2020 2d20 7472 6163 6528 6d61        - trace(ma
-00007b00: 7472 6978 5f69 6e76 6572 7365 2856 292e  trix_inverse(V).
-00007b10: 646f 7428 5829 290a 2020 2020 2020 2020  dot(X)).        
-00007b20: 2020 2020 2020 2020 2d20 6e75 202a 2070          - nu * p
-00007b30: 202a 2070 742e 6c6f 6728 3229 0a20 2020   * pt.log(2).   
-00007b40: 2020 2020 2020 2020 2020 2020 202d 206e               - n
-00007b50: 7520 2a20 7074 2e6c 6f67 2849 5649 290a  u * pt.log(IVI).
-00007b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b70: 2d20 3220 2a20 6d75 6c74 6967 616d 6d61  - 2 * multigamma
-00007b80: 6c6e 286e 7520 2f20 322e 302c 2070 290a  ln(nu / 2.0, p).
-00007b90: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00007ba0: 2020 2020 2020 2020 2020 2f20 322c 0a20            / 2,. 
-00007bb0: 2020 2020 2020 2020 2020 206d 6174 7269             matri
-00007bc0: 785f 706f 735f 6465 6628 5829 2c0a 2020  x_pos_def(X),.  
-00007bd0: 2020 2020 2020 2020 2020 7074 2e65 7128            pt.eq(
-00007be0: 582c 2058 2e54 292c 0a20 2020 2020 2020  X, X.T),.       
-00007bf0: 2020 2020 206e 7520 3e20 2870 202d 2031       nu > (p - 1
-00007c00: 292c 0a20 2020 2020 2020 2029 0a0a 0a64  ),.        )...d
-00007c10: 6566 2057 6973 6861 7274 4261 7274 6c65  ef WishartBartle
-00007c20: 7474 286e 616d 652c 2053 2c20 6e75 2c20  tt(name, S, nu, 
-00007c30: 6973 5f63 686f 6c65 736b 793d 4661 6c73  is_cholesky=Fals
-00007c40: 652c 2072 6574 7572 6e5f 6368 6f6c 6573  e, return_choles
-00007c50: 6b79 3d46 616c 7365 2c20 696e 6974 7661  ky=False, initva
-00007c60: 6c3d 4e6f 6e65 293a 0a20 2020 2072 2222  l=None):.    r""
-00007c70: 220a 2020 2020 4261 7274 6c65 7474 2064  ".    Bartlett d
-00007c80: 6563 6f6d 706f 7369 7469 6f6e 206f 6620  ecomposition of 
-00007c90: 7468 6520 5769 7368 6172 7420 6469 7374  the Wishart dist
-00007ca0: 7269 6275 7469 6f6e 2e20 4173 2074 6865  ribution. As the
-00007cb0: 2057 6973 6861 7274 0a20 2020 2064 6973   Wishart.    dis
-00007cc0: 7472 6962 7574 696f 6e20 7265 7175 6972  tribution requir
-00007cd0: 6573 2074 6865 206d 6174 7269 7820 746f  es the matrix to
-00007ce0: 2062 6520 7379 6d6d 6574 7269 6320 706f   be symmetric po
-00007cf0: 7369 7469 7665 2073 656d 692d 6465 6669  sitive semi-defi
-00007d00: 6e69 7465 0a20 2020 2069 7420 6973 2069  nite.    it is i
-00007d10: 6d70 6f73 7369 626c 6520 666f 7220 4d43  mpossible for MC
-00007d20: 4d43 2074 6f20 6576 6572 2070 726f 706f  MC to ever propo
-00007d30: 7365 2061 6363 6570 7461 626c 6520 6d61  se acceptable ma
-00007d40: 7472 6963 6573 2e0a 0a20 2020 2049 6e73  trices...    Ins
-00007d50: 7465 6164 2c20 7765 2063 616e 2075 7365  tead, we can use
-00007d60: 2074 6865 2042 6172 6c65 7474 2064 6563   the Barlett dec
-00007d70: 6f6d 706f 7369 7469 6f6e 2077 6869 6368  omposition which
-00007d80: 2073 616d 706c 6573 2061 206c 6f77 6572   samples a lower
-00007d90: 0a20 2020 2064 6961 676f 6e61 6c20 6d61  .    diagonal ma
-00007da0: 7472 6978 2e20 5370 6563 6966 6963 616c  trix. Specifical
-00007db0: 6c79 3a0a 0a20 2020 202e 2e20 6d61 7468  ly:..    .. math
-00007dc0: 3a3a 0a20 2020 2020 2020 205c 7465 7874  ::.        \text
-00007dd0: 7b49 667d 204c 205c 7369 6d20 5c62 6567  {If} L \sim \beg
-00007de0: 696e 7b70 6d61 7472 6978 7d0a 2020 2020  in{pmatrix}.    
-00007df0: 2020 2020 5c73 7172 747b 635f 317d 2026      \sqrt{c_1} &
-00007e00: 2030 2026 2030 205c 5c0a 2020 2020 2020   0 & 0 \\.      
-00007e10: 2020 7a5f 7b32 317d 2026 205c 7371 7274    z_{21} & \sqrt
-00007e20: 7b63 5f32 7d20 2620 3020 5c5c 0a20 2020  {c_2} & 0 \\.   
-00007e30: 2020 2020 207a 5f7b 3331 7d20 2620 7a5f       z_{31} & z_
-00007e40: 7b33 327d 2026 205c 7371 7274 7b63 5f33  {32} & \sqrt{c_3
-00007e50: 7d0a 2020 2020 2020 2020 5c65 6e64 7b70  }.        \end{p
-00007e60: 6d61 7472 6978 7d0a 0a20 2020 2020 2020  matrix}..       
-00007e70: 205c 7465 7874 7b77 6974 687d 2063 5f69   \text{with} c_i
-00007e80: 205c 7369 6d20 5c63 6869 5e32 286e 2d69   \sim \chi^2(n-i
-00007e90: 2b31 2920 5c74 6578 747b 2061 6e64 207d  +1) \text{ and }
-00007ea0: 206e 5f7b 696a 7d20 5c73 696d 205c 6d61   n_{ij} \sim \ma
-00007eb0: 7468 6361 6c7b 4e7d 2830 2c20 3129 2c20  thcal{N}(0, 1), 
-00007ec0: 5c74 6578 747b 7468 656e 7d20 5c5c 0a20  \text{then} \\. 
-00007ed0: 2020 2020 2020 204c 205c 7469 6d65 7320         L \times 
-00007ee0: 4120 5c74 696d 6573 2041 2e54 205c 7469  A \times A.T \ti
-00007ef0: 6d65 7320 4c2e 5420 5c73 696d 205c 7465  mes L.T \sim \te
-00007f00: 7874 7b57 6973 6861 7274 7d28 4c20 5c74  xt{Wishart}(L \t
-00007f10: 696d 6573 204c 2e54 2c20 5c6e 7529 0a0a  imes L.T, \nu)..
-00007f20: 2020 2020 5365 6520 6874 7470 3a2f 2f65      See http://e
-00007f30: 6e2e 7769 6b69 7065 6469 612e 6f72 672f  n.wikipedia.org/
-00007f40: 7769 6b69 2f57 6973 6861 7274 5f64 6973  wiki/Wishart_dis
-00007f50: 7472 6962 7574 696f 6e23 4261 7274 6c65  tribution#Bartle
-00007f60: 7474 5f64 6563 6f6d 706f 7369 7469 6f6e  tt_decomposition
-00007f70: 0a20 2020 2066 6f72 206d 6f72 6520 696e  .    for more in
-00007f80: 666f 726d 6174 696f 6e2e 0a0a 2020 2020  formation...    
-00007f90: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
-00007fa0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 5320  ---------.    S 
-00007fb0: 3a20 6e64 6172 7261 790a 2020 2020 2020  : ndarray.      
-00007fc0: 2020 7020 7820 7020 706f 7369 7469 7665    p x p positive
-00007fd0: 2064 6566 696e 6974 6520 6d61 7472 6978   definite matrix
-00007fe0: 0a20 2020 2020 2020 204f 723a 0a20 2020  .        Or:.   
-00007ff0: 2020 2020 2070 2078 2070 206c 6f77 6572       p x p lower
-00008000: 2d74 7269 616e 6775 6c61 7220 6d61 7472  -triangular matr
-00008010: 6978 2074 6861 7420 6973 2074 6865 2043  ix that is the C
-00008020: 686f 6c65 736b 7920 6661 6374 6f72 0a20  holesky factor. 
-00008030: 2020 2020 2020 206f 6620 7468 6520 636f         of the co
-00008040: 7661 7269 616e 6365 206d 6174 7269 782e  variance matrix.
-00008050: 0a20 2020 206e 7520 3a20 7465 6e73 6f72  .    nu : tensor
-00008060: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
-00008070: 2020 2020 2044 6567 7265 6573 206f 6620       Degrees of 
-00008080: 6672 6565 646f 6d2c 203e 2064 696d 2853  freedom, > dim(S
-00008090: 292e 0a20 2020 2069 735f 6368 6f6c 6573  )..    is_choles
-000080a0: 6b79 203a 2062 6f6f 6c2c 2064 6566 6175  ky : bool, defau
-000080b0: 6c74 3d46 616c 7365 0a20 2020 2020 2020  lt=False.       
-000080c0: 2049 6e70 7574 206d 6174 7269 7820 5320   Input matrix S 
-000080d0: 6973 2061 6c72 6561 6479 2043 686f 6c65  is already Chole
-000080e0: 736b 7920 6465 636f 6d70 6f73 6564 2061  sky decomposed a
-000080f0: 7320 532e 5420 2a20 530a 2020 2020 7265  s S.T * S.    re
-00008100: 7475 726e 5f63 686f 6c65 736b 7920 3a20  turn_cholesky : 
-00008110: 626f 6f6c 2c20 6465 6661 756c 743d 4661  bool, default=Fa
-00008120: 6c73 650a 2020 2020 2020 2020 4f6e 6c79  lse.        Only
-00008130: 2072 6574 7572 6e20 7468 6520 4368 6f6c   return the Chol
-00008140: 6573 6b79 2064 6563 6f6d 706f 7365 6420  esky decomposed 
-00008150: 6d61 7472 6978 2e0a 2020 2020 696e 6974  matrix..    init
-00008160: 7661 6c20 3a20 6e64 6172 7261 790a 2020  val : ndarray.  
-00008170: 2020 2020 2020 7020 7820 7020 706f 7369        p x p posi
-00008180: 7469 7665 2064 6566 696e 6974 6520 6d61  tive definite ma
-00008190: 7472 6978 2075 7365 6420 746f 2069 6e69  trix used to ini
-000081a0: 7469 616c 697a 650a 0a20 2020 204e 6f74  tialize..    Not
-000081b0: 6573 0a20 2020 202d 2d2d 2d2d 0a20 2020  es.    -----.   
-000081c0: 2054 6869 7320 6973 206e 6f74 2061 2073   This is not a s
-000081d0: 7461 6e64 6172 6420 4469 7374 7269 6275  tandard Distribu
-000081e0: 7469 6f6e 2063 6c61 7373 2062 7574 2066  tion class but f
-000081f0: 6f6c 6c6f 7773 2061 2073 696d 696c 6172  ollows a similar
-00008200: 0a20 2020 2069 6e74 6572 6661 6365 2e20  .    interface. 
-00008210: 4265 7369 6465 7320 7468 6520 5769 7368  Besides the Wish
-00008220: 6172 7420 6469 7374 7269 6275 7469 6f6e  art distribution
-00008230: 2c20 6974 2077 696c 6c20 6164 6420 5256  , it will add RV
-00008240: 730a 2020 2020 6e61 6d65 5f63 2061 6e64  s.    name_c and
-00008250: 206e 616d 655f 7a20 746f 2079 6f75 7220   name_z to your 
-00008260: 6d6f 6465 6c20 7768 6963 6820 6d61 6b65  model which make
-00008270: 2075 7020 7468 6520 6d61 7472 6978 2e0a   up the matrix..
-00008280: 0a20 2020 2054 6869 7320 6469 7374 7269  .    This distri
-00008290: 6275 7469 6f6e 2069 7320 7573 7561 6c6c  bution is usuall
-000082a0: 7920 6120 6261 6420 6964 6561 2074 6f20  y a bad idea to 
-000082b0: 7573 6520 6173 2061 2070 7269 6f72 2066  use as a prior f
-000082c0: 6f72 206d 756c 7469 7661 7269 6174 650a  or multivariate.
-000082d0: 2020 2020 6e6f 726d 616c 2e20 596f 7520      normal. You 
-000082e0: 7368 6f75 6c64 2069 6e73 7465 6164 2075  should instead u
-000082f0: 7365 204c 4b4a 4368 6f6c 6573 6b79 436f  se LKJCholeskyCo
-00008300: 7620 6f72 204c 4b4a 436f 7272 2e0a 2020  v or LKJCorr..  
-00008310: 2020 2222 220a 0a20 2020 204c 203d 2053    """..    L = S
-00008320: 2069 6620 6973 5f63 686f 6c65 736b 7920   if is_cholesky 
-00008330: 656c 7365 2073 6369 7079 2e6c 696e 616c  else scipy.linal
-00008340: 672e 6368 6f6c 6573 6b79 2853 290a 2020  g.cholesky(S).  
-00008350: 2020 6469 6167 5f69 6478 203d 206e 702e    diag_idx = np.
-00008360: 6469 6167 5f69 6e64 6963 6573 5f66 726f  diag_indices_fro
-00008370: 6d28 5329 0a20 2020 2074 7269 6c5f 6964  m(S).    tril_id
-00008380: 7820 3d20 6e70 2e74 7269 6c5f 696e 6469  x = np.tril_indi
-00008390: 6365 735f 6672 6f6d 2853 2c20 6b3d 2d31  ces_from(S, k=-1
-000083a0: 290a 2020 2020 6e5f 6469 6167 203d 206c  ).    n_diag = l
-000083b0: 656e 2864 6961 675f 6964 785b 305d 290a  en(diag_idx[0]).
-000083c0: 2020 2020 6e5f 7472 696c 203d 206c 656e      n_tril = len
-000083d0: 2874 7269 6c5f 6964 785b 305d 290a 0a20  (tril_idx[0]).. 
-000083e0: 2020 2069 6620 696e 6974 7661 6c20 6973     if initval is
-000083f0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00008400: 2020 2023 2049 6e76 6572 7365 2074 7261     # Inverse tra
-00008410: 6e73 666f 726d 0a20 2020 2020 2020 2069  nsform.        i
-00008420: 6e69 7476 616c 203d 206e 702e 646f 7428  nitval = np.dot(
-00008430: 6e70 2e64 6f74 286e 702e 6c69 6e61 6c67  np.dot(np.linalg
-00008440: 2e69 6e76 284c 292c 2069 6e69 7476 616c  .inv(L), initval
-00008450: 292c 206e 702e 6c69 6e61 6c67 2e69 6e76  ), np.linalg.inv
-00008460: 284c 2e54 2929 0a20 2020 2020 2020 2069  (L.T)).        i
-00008470: 6e69 7476 616c 203d 206c 696e 616c 672e  nitval = linalg.
-00008480: 6368 6f6c 6573 6b79 2869 6e69 7476 616c  cholesky(initval
-00008490: 2c20 6c6f 7765 723d 5472 7565 290a 2020  , lower=True).  
-000084a0: 2020 2020 2020 6469 6167 5f74 6573 7476        diag_testv
-000084b0: 616c 203d 2069 6e69 7476 616c 5b64 6961  al = initval[dia
-000084c0: 675f 6964 785d 202a 2a20 320a 2020 2020  g_idx] ** 2.    
-000084d0: 2020 2020 7472 696c 5f74 6573 7476 616c      tril_testval
-000084e0: 203d 2069 6e69 7476 616c 5b74 7269 6c5f   = initval[tril_
-000084f0: 6964 785d 0a20 2020 2065 6c73 653a 0a20  idx].    else:. 
-00008500: 2020 2020 2020 2064 6961 675f 7465 7374         diag_test
-00008510: 7661 6c20 3d20 4e6f 6e65 0a20 2020 2020  val = None.     
-00008520: 2020 2074 7269 6c5f 7465 7374 7661 6c20     tril_testval 
-00008530: 3d20 4e6f 6e65 0a0a 2020 2020 6320 3d20  = None..    c = 
-00008540: 7074 2e73 7172 7428 0a20 2020 2020 2020  pt.sqrt(.       
-00008550: 2043 6869 5371 7561 7265 6428 2225 735f   ChiSquared("%s_
-00008560: 6322 2025 206e 616d 652c 206e 7520 2d20  c" % name, nu - 
-00008570: 6e70 2e61 7261 6e67 6528 322c 2032 202b  np.arange(2, 2 +
-00008580: 206e 5f64 6961 6729 2c20 7368 6170 653d   n_diag), shape=
-00008590: 6e5f 6469 6167 2c20 696e 6974 7661 6c3d  n_diag, initval=
-000085a0: 6469 6167 5f74 6573 7476 616c 290a 2020  diag_testval).  
-000085b0: 2020 290a 2020 2020 706d 2e5f 6c6f 672e    ).    pm._log.
-000085c0: 696e 666f 2822 4164 6465 6420 6e65 7720  info("Added new 
-000085d0: 7661 7269 6162 6c65 2025 735f 6320 746f  variable %s_c to
-000085e0: 206d 6f64 656c 2064 6961 676f 6e61 6c20   model diagonal 
-000085f0: 6f66 2057 6973 6861 7274 2e22 2025 206e  of Wishart." % n
-00008600: 616d 6529 0a20 2020 207a 203d 204e 6f72  ame).    z = Nor
-00008610: 6d61 6c28 2225 735f 7a22 2025 206e 616d  mal("%s_z" % nam
-00008620: 652c 2030 2e30 2c20 312e 302c 2073 6861  e, 0.0, 1.0, sha
-00008630: 7065 3d6e 5f74 7269 6c2c 2069 6e69 7476  pe=n_tril, initv
-00008640: 616c 3d74 7269 6c5f 7465 7374 7661 6c29  al=tril_testval)
-00008650: 0a20 2020 2070 6d2e 5f6c 6f67 2e69 6e66  .    pm._log.inf
-00008660: 6f28 2241 6464 6564 206e 6577 2076 6172  o("Added new var
-00008670: 6961 626c 6520 2573 5f7a 2074 6f20 6d6f  iable %s_z to mo
-00008680: 6465 6c20 6f66 662d 6469 6167 6f6e 616c  del off-diagonal
-00008690: 7320 6f66 2057 6973 6861 7274 2e22 2025  s of Wishart." %
-000086a0: 206e 616d 6529 0a20 2020 2023 2043 6f6e   name).    # Con
-000086b0: 7374 7275 6374 2041 206d 6174 7269 780a  struct A matrix.
-000086c0: 2020 2020 4120 3d20 7074 2e7a 6572 6f73      A = pt.zeros
-000086d0: 2853 2e73 6861 7065 2c20 6474 7970 653d  (S.shape, dtype=
-000086e0: 6e70 2e66 6c6f 6174 3332 290a 2020 2020  np.float32).    
-000086f0: 4120 3d20 7074 2e73 6574 5f73 7562 7465  A = pt.set_subte
-00008700: 6e73 6f72 2841 5b64 6961 675f 6964 785d  nsor(A[diag_idx]
-00008710: 2c20 6329 0a20 2020 2041 203d 2070 742e  , c).    A = pt.
-00008720: 7365 745f 7375 6274 656e 736f 7228 415b  set_subtensor(A[
-00008730: 7472 696c 5f69 6478 5d2c 207a 290a 0a20  tril_idx], z).. 
-00008740: 2020 2023 204c 202a 2041 202a 2041 2e54     # L * A * A.T
-00008750: 202a 204c 2e54 207e 2057 6973 6861 7274   * L.T ~ Wishart
-00008760: 284c 2a4c 2e54 2c20 6e75 290a 2020 2020  (L*L.T, nu).    
-00008770: 6966 2072 6574 7572 6e5f 6368 6f6c 6573  if return_choles
-00008780: 6b79 3a0a 2020 2020 2020 2020 7265 7475  ky:.        retu
-00008790: 726e 2070 6d2e 4465 7465 726d 696e 6973  rn pm.Determinis
-000087a0: 7469 6328 6e61 6d65 2c20 7074 2e64 6f74  tic(name, pt.dot
-000087b0: 284c 2c20 4129 290a 2020 2020 656c 7365  (L, A)).    else
-000087c0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000087d0: 2070 6d2e 4465 7465 726d 696e 6973 7469   pm.Deterministi
-000087e0: 6328 6e61 6d65 2c20 7074 2e64 6f74 2870  c(name, pt.dot(p
-000087f0: 742e 646f 7428 7074 2e64 6f74 284c 2c20  t.dot(pt.dot(L, 
-00008800: 4129 2c20 412e 5429 2c20 4c2e 5429 290a  A), A.T), L.T)).
-00008810: 0a0a 6465 6620 5f6c 6b6a 5f6e 6f72 6d61  ..def _lkj_norma
-00008820: 6c69 7a69 6e67 5f63 6f6e 7374 616e 7428  lizing_constant(
-00008830: 6574 612c 206e 293a 0a20 2020 2023 2054  eta, n):.    # T
-00008840: 4f44 4f3a 2054 6869 7320 6973 206d 6978  ODO: This is mix
-00008850: 696e 6720 7079 7468 6f6e 2062 7261 6e63  ing python branc
-00008860: 6869 6e67 2077 6974 6820 7468 6520 706f  hing with the po
-00008870: 7465 6e74 6961 6c6c 7920 7379 6d62 6f6c  tentially symbol
-00008880: 6963 206e 2061 6e64 2065 7461 2076 6172  ic n and eta var
-00008890: 6961 626c 6573 0a20 2020 2069 6620 6e6f  iables.    if no
-000088a0: 7420 6973 696e 7374 616e 6365 2865 7461  t isinstance(eta
-000088b0: 2c20 2869 6e74 2c20 666c 6f61 7429 293a  , (int, float)):
-000088c0: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-000088d0: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-000088e0: 6f72 2822 6574 6120 6d75 7374 2062 6520  or("eta must be 
-000088f0: 616e 2069 6e74 206f 7220 666c 6f61 7422  an int or float"
-00008900: 290a 2020 2020 6966 206e 6f74 2069 7369  ).    if not isi
-00008910: 6e73 7461 6e63 6528 6e2c 2069 6e74 293a  nstance(n, int):
-00008920: 0a20 2020 2020 2020 2072 6169 7365 204e  .        raise N
-00008930: 6f74 496d 706c 656d 656e 7465 6445 7272  otImplementedErr
-00008940: 6f72 2822 6e20 6d75 7374 2062 6520 616e  or("n must be an
-00008950: 2069 6e74 6567 6572 2229 0a20 2020 2069   integer").    i
-00008960: 6620 6574 6120 3d3d 2031 3a0a 2020 2020  f eta == 1:.    
-00008970: 2020 2020 7265 7375 6c74 203d 2067 616d      result = gam
-00008980: 6d61 6c6e 2832 2e30 202a 2070 742e 6172  maln(2.0 * pt.ar
-00008990: 616e 6765 2831 2c20 696e 7428 286e 202d  ange(1, int((n -
-000089a0: 2031 2920 2f20 3229 202b 2031 2929 2e73   1) / 2) + 1)).s
-000089b0: 756d 2829 0a20 2020 2020 2020 2069 6620  um().        if 
-000089c0: 6e20 2520 3220 3d3d 2031 3a0a 2020 2020  n % 2 == 1:.    
-000089d0: 2020 2020 2020 2020 7265 7375 6c74 202b          result +
-000089e0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-000089f0: 2020 2020 302e 3235 202a 2028 6e2a 2a32      0.25 * (n**2
-00008a00: 202d 2031 2920 2a20 7074 2e6c 6f67 286e   - 1) * pt.log(n
-00008a10: 702e 7069 290a 2020 2020 2020 2020 2020  p.pi).          
-00008a20: 2020 2020 2020 2d20 302e 3235 202a 2028        - 0.25 * (
-00008a30: 6e20 2d20 3129 202a 2a20 3220 2a20 7074  n - 1) ** 2 * pt
-00008a40: 2e6c 6f67 2832 2e30 290a 2020 2020 2020  .log(2.0).      
-00008a50: 2020 2020 2020 2020 2020 2d20 286e 202d            - (n -
-00008a60: 2031 2920 2a20 6761 6d6d 616c 6e28 696e   1) * gammaln(in
-00008a70: 7428 286e 202b 2031 2920 2f20 3229 290a  t((n + 1) / 2)).
-00008a80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00008a90: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00008aa0: 2020 2020 2020 2020 7265 7375 6c74 202b          result +
-00008ab0: 3d20 280a 2020 2020 2020 2020 2020 2020  = (.            
-00008ac0: 2020 2020 302e 3235 202a 206e 202a 2028      0.25 * n * (
-00008ad0: 6e20 2d20 3229 202a 2070 742e 6c6f 6728  n - 2) * pt.log(
-00008ae0: 6e70 2e70 6929 0a20 2020 2020 2020 2020  np.pi).         
-00008af0: 2020 2020 2020 202b 2030 2e32 3520 2a20         + 0.25 * 
-00008b00: 2833 202a 206e 2a2a 3220 2d20 3420 2a20  (3 * n**2 - 4 * 
-00008b10: 6e29 202a 2070 742e 6c6f 6728 322e 3029  n) * pt.log(2.0)
-00008b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008b30: 202b 206e 202a 2067 616d 6d61 6c6e 286e   + n * gammaln(n
-00008b40: 202f 2032 290a 2020 2020 2020 2020 2020   / 2).          
-00008b50: 2020 2020 2020 2d20 286e 202d 2031 2920        - (n - 1) 
-00008b60: 2a20 6761 6d6d 616c 6e28 6e29 0a20 2020  * gammaln(n).   
-00008b70: 2020 2020 2020 2020 2029 0a20 2020 2065           ).    e
-00008b80: 6c73 653a 0a20 2020 2020 2020 2072 6573  lse:.        res
-00008b90: 756c 7420 3d20 2d28 6e20 2d20 3129 202a  ult = -(n - 1) *
-00008ba0: 2067 616d 6d61 6c6e 2865 7461 202b 2030   gammaln(eta + 0
-00008bb0: 2e35 202a 2028 6e20 2d20 3129 290a 2020  .5 * (n - 1)).  
-00008bc0: 2020 2020 2020 6b20 3d20 7074 2e61 7261        k = pt.ara
-00008bd0: 6e67 6528 312c 206e 290a 2020 2020 2020  nge(1, n).      
-00008be0: 2020 7265 7375 6c74 202b 3d20 2830 2e35    result += (0.5
-00008bf0: 202a 206b 202a 2070 742e 6c6f 6728 6e70   * k * pt.log(np
-00008c00: 2e70 6929 202b 2067 616d 6d61 6c6e 2865  .pi) + gammaln(e
-00008c10: 7461 202b 2030 2e35 202a 2028 6e20 2d20  ta + 0.5 * (n - 
-00008c20: 3120 2d20 6b29 2929 2e73 756d 2829 0a20  1 - k))).sum(). 
-00008c30: 2020 2072 6574 7572 6e20 7265 7375 6c74     return result
-00008c40: 0a0a 0a63 6c61 7373 205f 4c4b 4a43 686f  ...class _LKJCho
-00008c50: 6c65 736b 7943 6f76 4261 7365 5256 2852  leskyCovBaseRV(R
-00008c60: 616e 646f 6d56 6172 6961 626c 6529 3a0a  andomVariable):.
-00008c70: 2020 2020 6e61 6d65 203d 2022 5f6c 6b6a      name = "_lkj
-00008c80: 6368 6f6c 6573 6b79 636f 7662 6173 6522  choleskycovbase"
-00008c90: 0a20 2020 206e 6469 6d5f 7375 7070 203d  .    ndim_supp =
-00008ca0: 2031 0a20 2020 206e 6469 6d73 5f70 6172   1.    ndims_par
-00008cb0: 616d 7320 3d20 5b30 2c20 302c 2031 5d0a  ams = [0, 0, 1].
-00008cc0: 2020 2020 6474 7970 6520 3d20 2266 6c6f      dtype = "flo
-00008cd0: 6174 5822 0a20 2020 205f 7072 696e 745f  atX".    _print_
-00008ce0: 6e61 6d65 203d 2028 225f 6c6b 6a63 686f  name = ("_lkjcho
-00008cf0: 6c65 736b 7963 6f76 6261 7365 222c 2022  leskycovbase", "
-00008d00: 5c5c 6f70 6572 6174 6f72 6e61 6d65 7b5f  \\operatorname{_
-00008d10: 6c6b 6a63 686f 6c65 736b 7963 6f76 6261  lkjcholeskycovba
-00008d20: 7365 7d22 290a 0a20 2020 2064 6566 206d  se}")..    def m
-00008d30: 616b 655f 6e6f 6465 2873 656c 662c 2072  ake_node(self, r
-00008d40: 6e67 2c20 7369 7a65 2c20 6474 7970 652c  ng, size, dtype,
-00008d50: 206e 2c20 6574 612c 2044 293a 0a20 2020   n, eta, D):.   
-00008d60: 2020 2020 206e 203d 2070 742e 6173 5f74       n = pt.as_t
-00008d70: 656e 736f 725f 7661 7269 6162 6c65 286e  ensor_variable(n
-00008d80: 290a 2020 2020 2020 2020 6966 206e 6f74  ).        if not
-00008d90: 206e 2e6e 6469 6d20 3d3d 2030 3a0a 2020   n.ndim == 0:.  
-00008da0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00008db0: 5661 6c75 6545 7272 6f72 2822 6e20 6d75  ValueError("n mu
-00008dc0: 7374 2062 6520 6120 7363 616c 6172 2028  st be a scalar (
-00008dd0: 6e64 696d 3d30 292e 2229 0a0a 2020 2020  ndim=0).")..    
-00008de0: 2020 2020 6574 6120 3d20 7074 2e61 735f      eta = pt.as_
-00008df0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-00008e00: 6574 6129 0a20 2020 2020 2020 2069 6620  eta).        if 
-00008e10: 6e6f 7420 6574 612e 6e64 696d 203d 3d20  not eta.ndim == 
-00008e20: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
-00008e30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00008e40: 2265 7461 206d 7573 7420 6265 2061 2073  "eta must be a s
-00008e50: 6361 6c61 7220 286e 6469 6d3d 3029 2e22  calar (ndim=0)."
-00008e60: 290a 0a20 2020 2020 2020 2044 203d 2070  )..        D = p
-00008e70: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00008e80: 6162 6c65 2844 290a 0a20 2020 2020 2020  able(D)..       
-00008e90: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
-00008ea0: 6d61 6b65 5f6e 6f64 6528 726e 672c 2073  make_node(rng, s
-00008eb0: 697a 652c 2064 7479 7065 2c20 6e2c 2065  ize, dtype, n, e
-00008ec0: 7461 2c20 4429 0a0a 2020 2020 6465 6620  ta, D)..    def 
-00008ed0: 5f73 7570 705f 7368 6170 655f 6672 6f6d  _supp_shape_from
-00008ee0: 5f70 6172 616d 7328 7365 6c66 2c20 6469  _params(self, di
-00008ef0: 7374 5f70 6172 616d 732c 2070 6172 616d  st_params, param
-00008f00: 5f73 6861 7065 7329 3a0a 2020 2020 2020  _shapes):.      
-00008f10: 2020 6e20 3d20 6469 7374 5f70 6172 616d    n = dist_param
-00008f20: 735b 305d 0a20 2020 2020 2020 2072 6574  s[0].        ret
-00008f30: 7572 6e20 2828 6e20 2a20 286e 202b 2031  urn ((n * (n + 1
-00008f40: 2929 202f 2f20 322c 290a 0a20 2020 2064  )) // 2,)..    d
-00008f50: 6566 2072 6e67 5f66 6e28 7365 6c66 2c20  ef rng_fn(self, 
-00008f60: 726e 672c 206e 2c20 6574 612c 2044 2c20  rng, n, eta, D, 
-00008f70: 7369 7a65 293a 0a20 2020 2020 2020 2023  size):.        #
-00008f80: 2057 6520 666c 6174 7465 6e20 7468 6520   We flatten the 
-00008f90: 7369 7a65 2074 6f20 6d61 6b65 206f 7065  size to make ope
-00008fa0: 7261 7469 6f6e 7320 6561 7369 6572 2c20  rations easier, 
-00008fb0: 616e 6420 7468 656e 2072 6562 7569 6c64  and then rebuild
-00008fc0: 2069 740a 2020 2020 2020 2020 6966 2073   it.        if s
-00008fd0: 697a 6520 6973 204e 6f6e 653a 0a20 2020  ize is None:.   
-00008fe0: 2020 2020 2020 2020 2073 697a 6520 3d20           size = 
-00008ff0: 442e 7368 6170 655b 3a2d 315d 0a20 2020  D.shape[:-1].   
-00009000: 2020 2020 2066 6c61 745f 7369 7a65 203d       flat_size =
-00009010: 206e 702e 7072 6f64 2873 697a 6529 2e61   np.prod(size).a
-00009020: 7374 7970 6528 696e 7429 0a0a 2020 2020  stype(int)..    
-00009030: 2020 2020 4320 3d20 4c4b 4a43 6f72 7252      C = LKJCorrR
-00009040: 562e 5f72 616e 646f 6d5f 636f 7272 5f6d  V._random_corr_m
-00009050: 6174 7269 7828 726e 673d 726e 672c 206e  atrix(rng=rng, n
-00009060: 3d6e 2c20 6574 613d 6574 612c 2066 6c61  =n, eta=eta, fla
-00009070: 745f 7369 7a65 3d66 6c61 745f 7369 7a65  t_size=flat_size
-00009080: 290a 2020 2020 2020 2020 4420 3d20 442e  ).        D = D.
-00009090: 7265 7368 6170 6528 666c 6174 5f73 697a  reshape(flat_siz
-000090a0: 652c 206e 290a 2020 2020 2020 2020 4320  e, n).        C 
-000090b0: 2a3d 2044 5b2e 2e2e 2c20 3a2c 206e 702e  *= D[..., :, np.
-000090c0: 6e65 7761 7869 735d 202a 2044 5b2e 2e2e  newaxis] * D[...
-000090d0: 2c20 6e70 2e6e 6577 6178 6973 2c20 3a5d  , np.newaxis, :]
-000090e0: 0a0a 2020 2020 2020 2020 7472 696c 5f69  ..        tril_i
-000090f0: 6478 203d 206e 702e 7472 696c 5f69 6e64  dx = np.tril_ind
-00009100: 6963 6573 286e 2c20 6b3d 3029 0a20 2020  ices(n, k=0).   
-00009110: 2020 2020 2073 616d 706c 6573 203d 206e       samples = n
-00009120: 702e 6c69 6e61 6c67 2e63 686f 6c65 736b  p.linalg.cholesk
-00009130: 7928 4329 5b2e 2e2e 2c20 7472 696c 5f69  y(C)[..., tril_i
-00009140: 6478 5b30 5d2c 2074 7269 6c5f 6964 785b  dx[0], tril_idx[
-00009150: 315d 5d0a 0a20 2020 2020 2020 2069 6620  1]]..        if 
-00009160: 7369 7a65 2069 7320 4e6f 6e65 3a0a 2020  size is None:.  
-00009170: 2020 2020 2020 2020 2020 7361 6d70 6c65            sample
-00009180: 7320 3d20 7361 6d70 6c65 735b 305d 0a20  s = samples[0]. 
-00009190: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000091a0: 2020 2020 2020 2020 2064 6973 745f 7368           dist_sh
-000091b0: 6170 6520 3d20 286e 202a 2028 6e20 2b20  ape = (n * (n + 
-000091c0: 3129 2920 2f2f 2032 0a20 2020 2020 2020  1)) // 2.       
-000091d0: 2020 2020 2073 616d 706c 6573 203d 206e       samples = n
-000091e0: 702e 7265 7368 6170 6528 7361 6d70 6c65  p.reshape(sample
-000091f0: 732c 2028 2a73 697a 652c 2064 6973 745f  s, (*size, dist_
-00009200: 7368 6170 6529 290a 0a20 2020 2020 2020  shape))..       
-00009210: 2072 6574 7572 6e20 7361 6d70 6c65 730a   return samples.
-00009220: 0a0a 5f6c 6a6b 5f63 686f 6c65 736b 795f  .._ljk_cholesky_
-00009230: 636f 765f 6261 7365 203d 205f 4c4b 4a43  cov_base = _LKJC
-00009240: 686f 6c65 736b 7943 6f76 4261 7365 5256  holeskyCovBaseRV
-00009250: 2829 0a0a 0a23 205f 4c4b 4a43 686f 6c65  ()...# _LKJChole
-00009260: 736b 7943 6f76 4261 7365 5256 2072 6571  skyCovBaseRV req
-00009270: 7569 7265 7320 6120 7072 6f70 6572 6c79  uires a properly
-00009280: 2073 6861 7065 6420 6044 602c 2077 6869   shaped `D`, whi
-00009290: 6368 206d 6561 6e73 2074 6865 2076 6172  ch means the var
-000092a0: 6961 626c 6520 6361 6e27 740a 2320 6265  iable can't.# be
-000092b0: 2073 6166 656c 7920 7265 7369 7a65 642e   safely resized.
-000092c0: 2042 6563 6175 7365 206f 6620 7468 6973   Because of this
-000092d0: 2c20 7765 2061 6464 2074 6865 2074 6869  , we add the thi
-000092e0: 6e20 5379 6d62 6f6c 6963 5261 6e64 6f6d  n SymbolicRandom
-000092f0: 5661 7269 6162 6c65 2077 7261 7070 6572  Variable wrapper
-00009300: 0a63 6c61 7373 205f 4c4b 4a43 686f 6c65  .class _LKJChole
-00009310: 736b 7943 6f76 5256 2853 796d 626f 6c69  skyCovRV(Symboli
-00009320: 6352 616e 646f 6d56 6172 6961 626c 6529  cRandomVariable)
-00009330: 3a0a 2020 2020 6465 6661 756c 745f 6f75  :.    default_ou
-00009340: 7470 7574 203d 2031 0a20 2020 205f 7072  tput = 1.    _pr
-00009350: 696e 745f 6e61 6d65 203d 2028 225f 6c6b  int_name = ("_lk
-00009360: 6a63 686f 6c65 736b 7963 6f76 222c 2022  jcholeskycov", "
-00009370: 5c5c 6f70 6572 6174 6f72 6e61 6d65 7b5f  \\operatorname{_
-00009380: 6c6b 6a63 686f 6c65 736b 7963 6f76 7d22  lkjcholeskycov}"
-00009390: 290a 0a20 2020 2064 6566 2075 7064 6174  )..    def updat
-000093a0: 6528 7365 6c66 2c20 6e6f 6465 293a 0a20  e(self, node):. 
-000093b0: 2020 2020 2020 2072 6574 7572 6e20 7b6e         return {n
-000093c0: 6f64 652e 696e 7075 7473 5b30 5d3a 206e  ode.inputs[0]: n
-000093d0: 6f64 652e 6f75 7470 7574 735b 305d 7d0a  ode.outputs[0]}.
-000093e0: 0a0a 636c 6173 7320 5f4c 4b4a 4368 6f6c  ..class _LKJChol
-000093f0: 6573 6b79 436f 7628 4469 7374 7269 6275  eskyCov(Distribu
-00009400: 7469 6f6e 293a 0a20 2020 2072 2222 2255  tion):.    r"""U
-00009410: 6e64 6572 6c79 696e 6720 636c 6173 7320  nderlying class 
-00009420: 666f 7220 636f 7661 7269 616e 6365 206d  for covariance m
-00009430: 6174 7269 7820 7769 7468 204c 4b4a 2064  atrix with LKJ d
-00009440: 6973 7472 6962 7574 6564 2063 6f72 7265  istributed corre
-00009450: 6c61 7469 6f6e 732e 0a20 2020 2053 6565  lations..    See
-00009460: 2064 6f63 7320 666f 7220 4c4b 4a43 686f   docs for LKJCho
-00009470: 6c65 736b 7943 6f76 2066 756e 6374 696f  leskyCov functio
-00009480: 6e20 666f 7220 6d6f 7265 2064 6574 6169  n for more detai
-00009490: 6c73 206f 6e20 686f 7720 746f 2075 7365  ls on how to use
-000094a0: 2069 7420 696e 206d 6f64 656c 732e 0a20   it in models.. 
-000094b0: 2020 2022 2222 0a0a 2020 2020 7276 5f74     """..    rv_t
-000094c0: 7970 6520 3d20 5f4c 4b4a 4368 6f6c 6573  ype = _LKJCholes
-000094d0: 6b79 436f 7652 560a 0a20 2020 2040 636c  kyCovRV..    @cl
-000094e0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000094f0: 6620 6469 7374 2863 6c73 2c20 6e2c 2065  f dist(cls, n, e
-00009500: 7461 2c20 7364 5f64 6973 742c 202a 2a6b  ta, sd_dist, **k
-00009510: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
-00009520: 6e20 3d20 7074 2e61 735f 7465 6e73 6f72  n = pt.as_tensor
-00009530: 5f76 6172 6961 626c 6528 696e 7458 286e  _variable(intX(n
-00009540: 2929 0a20 2020 2020 2020 2065 7461 203d  )).        eta =
-00009550: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
-00009560: 7269 6162 6c65 2866 6c6f 6174 5828 6574  riable(floatX(et
-00009570: 6129 290a 0a20 2020 2020 2020 2069 6620  a))..        if 
-00009580: 6e6f 7420 280a 2020 2020 2020 2020 2020  not (.          
-00009590: 2020 6973 696e 7374 616e 6365 2873 645f    isinstance(sd_
-000095a0: 6469 7374 2c20 5661 7269 6162 6c65 290a  dist, Variable).
-000095b0: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-000095c0: 7364 5f64 6973 742e 6f77 6e65 7220 6973  sd_dist.owner is
-000095d0: 206e 6f74 204e 6f6e 650a 2020 2020 2020   not None.      
-000095e0: 2020 2020 2020 616e 6420 6973 696e 7374        and isinst
-000095f0: 616e 6365 2873 645f 6469 7374 2e6f 776e  ance(sd_dist.own
-00009600: 6572 2e6f 702c 2028 5261 6e64 6f6d 5661  er.op, (RandomVa
-00009610: 7269 6162 6c65 2c20 5379 6d62 6f6c 6963  riable, Symbolic
-00009620: 5261 6e64 6f6d 5661 7269 6162 6c65 2929  RandomVariable))
-00009630: 0a20 2020 2020 2020 2020 2020 2061 6e64  .            and
-00009640: 2073 645f 6469 7374 2e6f 776e 6572 2e6f   sd_dist.owner.o
-00009650: 702e 6e64 696d 5f73 7570 7020 3c20 320a  p.ndim_supp < 2.
-00009660: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00009670: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00009680: 6545 7272 6f72 2822 7364 5f64 6973 7420  eError("sd_dist 
-00009690: 6d75 7374 2062 6520 6120 7363 616c 6172  must be a scalar
-000096a0: 206f 7220 7665 6374 6f72 2064 6973 7472   or vector distr
-000096b0: 6962 7574 696f 6e20 7661 7269 6162 6c65  ibution variable
-000096c0: 2229 0a0a 2020 2020 2020 2020 6368 6563  ")..        chec
-000096d0: 6b5f 6469 7374 5f6e 6f74 5f72 6567 6973  k_dist_not_regis
-000096e0: 7465 7265 6428 7364 5f64 6973 7429 0a20  tered(sd_dist). 
-000096f0: 2020 2020 2020 2023 2073 645f 6469 7374         # sd_dist
-00009700: 2069 7320 7061 7274 206f 6620 7468 6520   is part of the 
-00009710: 6765 6e65 7261 7469 7665 2067 7261 7068  generative graph
-00009720: 2c20 6275 7420 7368 6f75 6c64 2062 6520  , but should be 
-00009730: 636f 6d70 6c65 7465 6c79 2069 676e 6f72  completely ignor
-00009740: 6564 0a20 2020 2020 2020 2023 2062 7920  ed.        # by 
-00009750: 7468 6520 6c6f 6770 2067 7261 7068 2c20  the logp graph, 
-00009760: 7369 6e63 6520 7468 6520 4c4b 4a20 6c6f  since the LKJ lo
-00009770: 6770 2065 7870 6c69 6369 746c 7920 696e  gp explicitly in
-00009780: 636c 7564 6573 2074 6865 7365 2074 6572  cludes these ter
-00009790: 6d73 2e0a 2020 2020 2020 2020 7364 5f64  ms..        sd_d
-000097a0: 6973 7420 3d20 6967 6e6f 7265 5f6c 6f67  ist = ignore_log
-000097b0: 7072 6f62 2873 645f 6469 7374 290a 2020  prob(sd_dist).  
-000097c0: 2020 2020 2020 7265 7475 726e 2073 7570        return sup
-000097d0: 6572 2829 2e64 6973 7428 5b6e 2c20 6574  er().dist([n, et
-000097e0: 612c 2073 645f 6469 7374 5d2c 202a 2a6b  a, sd_dist], **k
-000097f0: 7761 7267 7329 0a0a 2020 2020 4063 6c61  wargs)..    @cla
-00009800: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00009810: 2072 765f 6f70 2863 6c73 2c20 6e2c 2065   rv_op(cls, n, e
-00009820: 7461 2c20 7364 5f64 6973 742c 2073 697a  ta, sd_dist, siz
-00009830: 653d 4e6f 6e65 293a 0a20 2020 2020 2020  e=None):.       
-00009840: 2023 2057 6520 7265 7369 7a65 2074 6865   # We resize the
-00009850: 2073 645f 6469 7374 2061 7574 6f6d 6174   sd_dist automat
-00009860: 6963 616c 6c79 2073 6f20 7468 6174 2069  ically so that i
-00009870: 7420 6861 7320 2873 697a 6520 7820 6e29  t has (size x n)
-00009880: 2069 6e64 6570 656e 6465 6e74 0a20 2020   independent.   
-00009890: 2020 2020 2023 2064 7261 7773 2077 6869       # draws whi
-000098a0: 6368 2069 7320 7768 6174 2074 6865 2060  ch is what the `
-000098b0: 5f4c 4b4a 4368 6f6c 6573 6b79 436f 7642  _LKJCholeskyCovB
-000098c0: 6173 6552 562e 726e 675f 666e 6020 6578  aseRV.rng_fn` ex
-000098d0: 7065 6374 732e 2054 6869 7320 6d61 6b65  pects. This make
-000098e0: 7320 7468 650a 2020 2020 2020 2020 2320  s the.        # 
-000098f0: 7261 6e64 6f6d 2061 6e64 206c 6f67 7020  random and logp 
-00009900: 6d65 7468 6f64 7320 6571 7569 7661 6c65  methods equivale
-00009910: 6e74 2c20 6173 2074 6865 206c 6174 7465  nt, as the latte
-00009920: 7220 616c 736f 2061 7373 756d 6573 2061  r also assumes a
-00009930: 2075 6e69 7175 6520 7661 6c75 650a 2020   unique value.  
-00009940: 2020 2020 2020 2320 666f 7220 6561 6368        # for each
-00009950: 2064 6961 676f 6e61 6c20 656c 656d 656e   diagonal elemen
-00009960: 742e 0a20 2020 2020 2020 2023 2053 696e  t..        # Sin
-00009970: 6365 2060 6574 6160 2061 6e64 2060 6e60  ce `eta` and `n`
-00009980: 2061 7265 2066 6f72 6365 6420 746f 2062   are forced to b
-00009990: 6520 7363 616c 6172 7320 7765 2064 6f6e  e scalars we don
-000099a0: 2774 206e 6565 6420 746f 2077 6f72 7279  't need to worry
-000099b0: 2061 626f 7574 0a20 2020 2020 2020 2023   about.        #
-000099c0: 2069 6d70 6c69 6564 2062 6174 6368 6564   implied batched
-000099d0: 2064 696d 656e 7369 6f6e 7320 6672 6f6d   dimensions from
-000099e0: 2074 686f 7365 2066 6f72 2074 6865 2074   those for the t
-000099f0: 696d 6520 6265 696e 672e 0a20 2020 2020  ime being..     
-00009a00: 2020 2069 6620 7369 7a65 2069 7320 4e6f     if size is No
-00009a10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00009a20: 7369 7a65 203d 2073 645f 6469 7374 2e73  size = sd_dist.s
-00009a30: 6861 7065 5b3a 2d31 5d0a 2020 2020 2020  hape[:-1].      
-00009a40: 2020 7368 6170 6520 3d20 7475 706c 6528    shape = tuple(
-00009a50: 7369 7a65 2920 2b20 286e 2c29 0a20 2020  size) + (n,).   
-00009a60: 2020 2020 2069 6620 7364 5f64 6973 742e       if sd_dist.
-00009a70: 6f77 6e65 722e 6f70 2e6e 6469 6d5f 7375  owner.op.ndim_su
-00009a80: 7070 203d 3d20 303a 0a20 2020 2020 2020  pp == 0:.       
-00009a90: 2020 2020 2073 645f 6469 7374 203d 2063       sd_dist = c
-00009aa0: 6861 6e67 655f 6469 7374 5f73 697a 6528  hange_dist_size(
-00009ab0: 7364 5f64 6973 742c 2073 6861 7065 290a  sd_dist, shape).
-00009ac0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00009ad0: 2020 2020 2020 2020 2020 2320 5468 6520            # The 
-00009ae0: 7375 7070 6f72 7420 7368 6170 6520 6d75  support shape mu
-00009af0: 7374 2062 6520 606e 6020 6275 7420 7765  st be `n` but we
-00009b00: 2068 6176 6520 6e6f 2077 6179 206f 6620   have no way of 
-00009b10: 636f 6e74 726f 6c6c 696e 6720 6974 0a20  controlling it. 
-00009b20: 2020 2020 2020 2020 2020 2073 645f 6469             sd_di
-00009b30: 7374 203d 2063 6861 6e67 655f 6469 7374  st = change_dist
-00009b40: 5f73 697a 6528 7364 5f64 6973 742c 2073  _size(sd_dist, s
-00009b50: 6861 7065 5b3a 2d31 5d29 0a0a 2020 2020  hape[:-1])..    
-00009b60: 2020 2020 2320 4372 6561 7465 206e 6577      # Create new
-00009b70: 2072 6e67 2066 6f72 2074 6865 205f 6c6b   rng for the _lk
-00009b80: 6a63 686f 6c65 736b 7963 6f76 2069 6e74  jcholeskycov int
-00009b90: 6572 6e61 6c20 5256 0a20 2020 2020 2020  ernal RV.       
-00009ba0: 2072 6e67 203d 2070 7974 656e 736f 722e   rng = pytensor.
-00009bb0: 7368 6172 6564 286e 702e 7261 6e64 6f6d  shared(np.random
-00009bc0: 2e64 6566 6175 6c74 5f72 6e67 2829 290a  .default_rng()).
-00009bd0: 0a20 2020 2020 2020 2072 6e67 5f2c 206e  .        rng_, n
-00009be0: 5f2c 2065 7461 5f2c 2073 645f 6469 7374  _, eta_, sd_dist
-00009bf0: 5f20 3d20 726e 672e 7479 7065 2829 2c20  _ = rng.type(), 
-00009c00: 6e2e 7479 7065 2829 2c20 6574 612e 7479  n.type(), eta.ty
-00009c10: 7065 2829 2c20 7364 5f64 6973 742e 7479  pe(), sd_dist.ty
-00009c20: 7065 2829 0a20 2020 2020 2020 206e 6578  pe().        nex
-00009c30: 745f 726e 675f 2c20 6c6b 6a63 6f76 5f20  t_rng_, lkjcov_ 
-00009c40: 3d20 5f6c 6a6b 5f63 686f 6c65 736b 795f  = _ljk_cholesky_
-00009c50: 636f 765f 6261 7365 286e 5f2c 2065 7461  cov_base(n_, eta
-00009c60: 5f2c 2073 645f 6469 7374 5f2c 2072 6e67  _, sd_dist_, rng
-00009c70: 3d72 6e67 5f29 2e6f 776e 6572 2e6f 7574  =rng_).owner.out
-00009c80: 7075 7473 0a0a 2020 2020 2020 2020 7265  puts..        re
-00009c90: 7475 726e 205f 4c4b 4a43 686f 6c65 736b  turn _LKJCholesk
-00009ca0: 7943 6f76 5256 280a 2020 2020 2020 2020  yCovRV(.        
-00009cb0: 2020 2020 696e 7075 7473 3d5b 726e 675f      inputs=[rng_
-00009cc0: 2c20 6e5f 2c20 6574 615f 2c20 7364 5f64  , n_, eta_, sd_d
-00009cd0: 6973 745f 5d2c 0a20 2020 2020 2020 2020  ist_],.         
-00009ce0: 2020 206f 7574 7075 7473 3d5b 6e65 7874     outputs=[next
-00009cf0: 5f72 6e67 5f2c 206c 6b6a 636f 765f 5d2c  _rng_, lkjcov_],
-00009d00: 0a20 2020 2020 2020 2020 2020 206e 6469  .            ndi
-00009d10: 6d5f 7375 7070 3d31 2c0a 2020 2020 2020  m_supp=1,.      
-00009d20: 2020 2928 726e 672c 206e 2c20 6574 612c    )(rng, n, eta,
-00009d30: 2073 645f 6469 7374 290a 0a0a 405f 6368   sd_dist)...@_ch
-00009d40: 616e 6765 5f64 6973 745f 7369 7a65 2e72  ange_dist_size.r
-00009d50: 6567 6973 7465 7228 5f4c 4b4a 4368 6f6c  egister(_LKJChol
-00009d60: 6573 6b79 436f 7652 5629 0a64 6566 2063  eskyCovRV).def c
-00009d70: 6861 6e67 655f 4c4b 4a43 686f 6c65 6b73  hange_LKJCholeks
-00009d80: 7943 6f76 5256 5f73 697a 6528 6f70 2c20  yCovRV_size(op, 
-00009d90: 6469 7374 2c20 6e65 775f 7369 7a65 2c20  dist, new_size, 
-00009da0: 6578 7061 6e64 3d46 616c 7365 293a 0a20  expand=False):. 
-00009db0: 2020 206e 2c20 6574 612c 2073 645f 6469     n, eta, sd_di
-00009dc0: 7374 203d 2064 6973 742e 6f77 6e65 722e  st = dist.owner.
-00009dd0: 696e 7075 7473 5b31 3a5d 0a0a 2020 2020  inputs[1:]..    
-00009de0: 6966 2065 7870 616e 643a 0a20 2020 2020  if expand:.     
-00009df0: 2020 206f 6c64 5f73 697a 6520 3d20 7364     old_size = sd
-00009e00: 5f64 6973 742e 7368 6170 655b 3a2d 315d  _dist.shape[:-1]
-00009e10: 0a20 2020 2020 2020 206e 6577 5f73 697a  .        new_siz
-00009e20: 6520 3d20 7475 706c 6528 6e65 775f 7369  e = tuple(new_si
-00009e30: 7a65 2920 2b20 7475 706c 6528 6f6c 645f  ze) + tuple(old_
-00009e40: 7369 7a65 290a 0a20 2020 2072 6574 7572  size)..    retur
-00009e50: 6e20 5f4c 4b4a 4368 6f6c 6573 6b79 436f  n _LKJCholeskyCo
-00009e60: 762e 7276 5f6f 7028 6e2c 2065 7461 2c20  v.rv_op(n, eta, 
-00009e70: 7364 5f64 6973 742c 2073 697a 653d 6e65  sd_dist, size=ne
-00009e80: 775f 7369 7a65 290a 0a0a 405f 6d6f 6d65  w_size)...@_mome
-00009e90: 6e74 2e72 6567 6973 7465 7228 5f4c 4b4a  nt.register(_LKJ
-00009ea0: 4368 6f6c 6573 6b79 436f 7652 5629 0a64  CholeskyCovRV).d
-00009eb0: 6566 205f 4c4b 4a43 686f 6c65 6b73 7943  ef _LKJCholeksyC
-00009ec0: 6f76 5256 5f6d 6f6d 656e 7428 6f70 2c20  ovRV_moment(op, 
-00009ed0: 7276 2c20 726e 672c 206e 2c20 6574 612c  rv, rng, n, eta,
-00009ee0: 2073 645f 6469 7374 293a 0a20 2020 2064   sd_dist):.    d
-00009ef0: 6961 675f 6964 7873 203d 2028 7074 2e63  iag_idxs = (pt.c
-00009f00: 756d 7375 6d28 7074 2e61 7261 6e67 6528  umsum(pt.arange(
-00009f10: 312c 206e 202b 2031 2929 202d 2031 292e  1, n + 1)) - 1).
-00009f20: 6173 7479 7065 2822 696e 7433 3222 290a  astype("int32").
-00009f30: 2020 2020 6d6f 6d65 6e74 203d 2070 742e      moment = pt.
-00009f40: 7a65 726f 735f 6c69 6b65 2872 7629 0a20  zeros_like(rv). 
-00009f50: 2020 206d 6f6d 656e 7420 3d20 7074 2e73     moment = pt.s
-00009f60: 6574 5f73 7562 7465 6e73 6f72 286d 6f6d  et_subtensor(mom
-00009f70: 656e 745b 2e2e 2e2c 2064 6961 675f 6964  ent[..., diag_id
-00009f80: 7873 5d2c 2031 290a 2020 2020 7265 7475  xs], 1).    retu
-00009f90: 726e 206d 6f6d 656e 740a 0a0a 405f 6465  rn moment...@_de
-00009fa0: 6661 756c 745f 7472 616e 7366 6f72 6d2e  fault_transform.
-00009fb0: 7265 6769 7374 6572 285f 4c4b 4a43 686f  register(_LKJCho
-00009fc0: 6c65 736b 7943 6f76 5256 290a 6465 6620  leskyCovRV).def 
-00009fd0: 5f4c 4b4a 4368 6f6c 656b 7379 436f 7652  _LKJCholeksyCovR
-00009fe0: 565f 6465 6661 756c 745f 7472 616e 7366  V_default_transf
-00009ff0: 6f72 6d28 6f70 2c20 7276 293a 0a20 2020  orm(op, rv):.   
-0000a000: 205f 2c20 6e2c 205f 2c20 5f20 3d20 7276   _, n, _, _ = rv
-0000a010: 2e6f 776e 6572 2e69 6e70 7574 730a 2020  .owner.inputs.  
-0000a020: 2020 7265 7475 726e 2074 7261 6e73 666f    return transfo
-0000a030: 726d 732e 4368 6f6c 6573 6b79 436f 7650  rms.CholeskyCovP
-0000a040: 6163 6b65 6428 6e29 0a0a 0a40 5f6c 6f67  acked(n)...@_log
-0000a050: 7072 6f62 2e72 6567 6973 7465 7228 5f4c  prob.register(_L
-0000a060: 4b4a 4368 6f6c 6573 6b79 436f 7652 5629  KJCholeskyCovRV)
-0000a070: 0a64 6566 205f 4c4b 4a43 686f 6c65 6b73  .def _LKJCholeks
-0000a080: 7943 6f76 5256 5f6c 6f67 7028 6f70 2c20  yCovRV_logp(op, 
-0000a090: 7661 6c75 6573 2c20 726e 672c 206e 2c20  values, rng, n, 
-0000a0a0: 6574 612c 2073 645f 6469 7374 2c20 2a2a  eta, sd_dist, **
-0000a0b0: 6b77 6172 6773 293a 0a20 2020 2028 7661  kwargs):.    (va
-0000a0c0: 6c75 652c 2920 3d20 7661 6c75 6573 0a0a  lue,) = values..
-0000a0d0: 2020 2020 6966 2076 616c 7565 2e6e 6469      if value.ndi
-0000a0e0: 6d20 3e20 313a 0a20 2020 2020 2020 2072  m > 1:.        r
-0000a0f0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-0000a100: 225f 4c4b 4a43 686f 6c65 736b 7943 6f76  "_LKJCholeskyCov
-0000a110: 206c 6f67 7020 6973 206f 6e6c 7920 696d   logp is only im
-0000a120: 706c 656d 656e 7465 6420 666f 7220 7665  plemented for ve
-0000a130: 6374 6f72 2076 616c 7565 7320 286e 6469  ctor values (ndi
-0000a140: 6d3d 3129 2229 0a0a 2020 2020 6469 6167  m=1)")..    diag
-0000a150: 5f69 6478 7320 3d20 7074 2e63 756d 7375  _idxs = pt.cumsu
-0000a160: 6d28 7074 2e61 7261 6e67 6528 312c 206e  m(pt.arange(1, n
-0000a170: 202b 2031 2929 202d 2031 0a20 2020 2063   + 1)) - 1.    c
-0000a180: 756d 7375 6d20 3d20 7074 2e63 756d 7375  umsum = pt.cumsu
-0000a190: 6d28 7661 6c75 652a 2a32 290a 2020 2020  m(value**2).    
-0000a1a0: 7661 7269 616e 6365 203d 2070 742e 7a65  variance = pt.ze
-0000a1b0: 726f 7328 7074 2e61 746c 6561 7374 5f31  ros(pt.atleast_1
-0000a1c0: 6428 6e29 290a 2020 2020 7661 7269 616e  d(n)).    varian
-0000a1d0: 6365 203d 2070 742e 696e 635f 7375 6274  ce = pt.inc_subt
-0000a1e0: 656e 736f 7228 7661 7269 616e 6365 5b30  ensor(variance[0
-0000a1f0: 5d2c 2076 616c 7565 5b30 5d20 2a2a 2032  ], value[0] ** 2
-0000a200: 290a 2020 2020 7661 7269 616e 6365 203d  ).    variance =
-0000a210: 2070 742e 696e 635f 7375 6274 656e 736f   pt.inc_subtenso
-0000a220: 7228 7661 7269 616e 6365 5b31 3a5d 2c20  r(variance[1:], 
-0000a230: 6375 6d73 756d 5b64 6961 675f 6964 7873  cumsum[diag_idxs
-0000a240: 5b31 3a5d 5d20 2d20 6375 6d73 756d 5b64  [1:]] - cumsum[d
-0000a250: 6961 675f 6964 7873 5b3a 2d31 5d5d 290a  iag_idxs[:-1]]).
-0000a260: 2020 2020 7364 5f76 616c 7320 3d20 7074      sd_vals = pt
-0000a270: 2e73 7172 7428 7661 7269 616e 6365 290a  .sqrt(variance).
-0000a280: 0a20 2020 206c 6f67 705f 7364 203d 2070  .    logp_sd = p
-0000a290: 6d2e 6c6f 6770 2873 645f 6469 7374 2c20  m.logp(sd_dist, 
-0000a2a0: 7364 5f76 616c 7329 2e73 756d 2829 0a20  sd_vals).sum(). 
-0000a2b0: 2020 2063 6f72 725f 6469 6167 203d 2076     corr_diag = v
-0000a2c0: 616c 7565 5b64 6961 675f 6964 7873 5d20  alue[diag_idxs] 
-0000a2d0: 2f20 7364 5f76 616c 730a 0a20 2020 206c  / sd_vals..    l
-0000a2e0: 6f67 705f 6c6b 6a20 3d20 2832 202a 2065  ogp_lkj = (2 * e
-0000a2f0: 7461 202d 2033 202b 206e 202d 2070 742e  ta - 3 + n - pt.
-0000a300: 6172 616e 6765 286e 2929 202a 2070 742e  arange(n)) * pt.
-0000a310: 6c6f 6728 636f 7272 5f64 6961 6729 0a20  log(corr_diag). 
-0000a320: 2020 206c 6f67 705f 6c6b 6a20 3d20 7074     logp_lkj = pt
-0000a330: 2e73 756d 286c 6f67 705f 6c6b 6a29 0a0a  .sum(logp_lkj)..
-0000a340: 2020 2020 2320 436f 6d70 7574 6520 7468      # Compute th
-0000a350: 6520 6c6f 6720 6465 7420 6a61 636f 6269  e log det jacobi
-0000a360: 616e 206f 6620 7468 6520 7365 636f 6e64  an of the second
-0000a370: 2074 7261 6e73 666f 726d 6174 696f 6e0a   transformation.
-0000a380: 2020 2020 2320 6465 7363 7269 6265 6420      # described 
-0000a390: 696e 2074 6865 2064 6f63 7374 7269 6e67  in the docstring
-0000a3a0: 2e0a 2020 2020 6964 7820 3d20 7074 2e61  ..    idx = pt.a
-0000a3b0: 7261 6e67 6528 6e29 0a20 2020 2064 6574  range(n).    det
-0000a3c0: 5f69 6e76 6a61 6320 3d20 7074 2e6c 6f67  _invjac = pt.log
-0000a3d0: 2863 6f72 725f 6469 6167 2920 2d20 6964  (corr_diag) - id
-0000a3e0: 7820 2a20 7074 2e6c 6f67 2873 645f 7661  x * pt.log(sd_va
-0000a3f0: 6c73 290a 2020 2020 6465 745f 696e 766a  ls).    det_invj
-0000a400: 6163 203d 2064 6574 5f69 6e76 6a61 632e  ac = det_invjac.
-0000a410: 7375 6d28 290a 0a20 2020 2023 2054 4f44  sum()..    # TOD
-0000a420: 4f3a 205f 6c6b 6a5f 6e6f 726d 616c 697a  O: _lkj_normaliz
-0000a430: 696e 675f 636f 6e73 7461 6e74 2063 7572  ing_constant cur
-0000a440: 7265 6e74 6c79 2072 6571 7569 7265 7320  rently requires 
-0000a450: 6065 7461 6020 616e 6420 606e 6020 746f  `eta` and `n` to
-0000a460: 2062 6520 636f 6e73 7461 6e74 730a 2020   be constants.  
-0000a470: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-0000a480: 6e63 6528 6e2c 2043 6f6e 7374 616e 7429  nce(n, Constant)
-0000a490: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
-0000a4a0: 4e6f 7449 6d70 6c65 6d65 6e74 6564 4572  NotImplementedEr
-0000a4b0: 726f 7228 226c 6f67 7020 6f6e 6c79 2069  ror("logp only i
-0000a4c0: 6d70 6c65 6d65 6e74 6564 2066 6f72 2063  mplemented for c
-0000a4d0: 6f6e 7374 616e 7420 606e 6022 290a 2020  onstant `n`").  
-0000a4e0: 2020 6e20 3d20 696e 7428 6e2e 6461 7461    n = int(n.data
-0000a4f0: 290a 0a20 2020 2069 6620 6e6f 7420 6973  )..    if not is
-0000a500: 696e 7374 616e 6365 2865 7461 2c20 436f  instance(eta, Co
-0000a510: 6e73 7461 6e74 293a 0a20 2020 2020 2020  nstant):.       
-0000a520: 2072 6169 7365 204e 6f74 496d 706c 656d   raise NotImplem
-0000a530: 656e 7465 6445 7272 6f72 2822 6c6f 6770  entedError("logp
-0000a540: 206f 6e6c 7920 696d 706c 656d 656e 7465   only implemente
-0000a550: 6420 666f 7220 636f 6e73 7461 6e74 2060  d for constant `
-0000a560: 6574 6160 2229 0a20 2020 2065 7461 203d  eta`").    eta =
-0000a570: 2066 6c6f 6174 2865 7461 2e64 6174 6129   float(eta.data)
-0000a580: 0a0a 2020 2020 6e6f 726d 203d 205f 6c6b  ..    norm = _lk
-0000a590: 6a5f 6e6f 726d 616c 697a 696e 675f 636f  j_normalizing_co
-0000a5a0: 6e73 7461 6e74 2865 7461 2c20 6e29 0a0a  nstant(eta, n)..
-0000a5b0: 2020 2020 7265 7475 726e 206e 6f72 6d20      return norm 
-0000a5c0: 2b20 6c6f 6770 5f6c 6b6a 202b 206c 6f67  + logp_lkj + log
-0000a5d0: 705f 7364 202b 2064 6574 5f69 6e76 6a61  p_sd + det_invja
-0000a5e0: 630a 0a0a 636c 6173 7320 4c4b 4a43 686f  c...class LKJCho
-0000a5f0: 6c65 736b 7943 6f76 3a0a 2020 2020 7222  leskyCov:.    r"
-0000a600: 2222 5772 6170 7065 7220 636c 6173 7320  ""Wrapper class 
-0000a610: 666f 7220 636f 7661 7269 616e 6365 206d  for covariance m
-0000a620: 6174 7269 7820 7769 7468 204c 4b4a 2064  atrix with LKJ d
-0000a630: 6973 7472 6962 7574 6564 2063 6f72 7265  istributed corre
-0000a640: 6c61 7469 6f6e 732e 0a0a 2020 2020 5468  lations...    Th
-0000a650: 6973 2064 6566 696e 6573 2061 2064 6973  is defines a dis
-0000a660: 7472 6962 7574 696f 6e20 6f76 6572 2043  tribution over C
-0000a670: 686f 6c65 736b 7920 6465 636f 6d70 6f73  holesky decompos
-0000a680: 6564 2063 6f76 6172 6961 6e63 650a 2020  ed covariance.  
-0000a690: 2020 6d61 7472 6963 6573 2c20 7375 6368    matrices, such
-0000a6a0: 2074 6861 7420 7468 6520 756e 6465 726c   that the underl
-0000a6b0: 7969 6e67 2063 6f72 7265 6c61 7469 6f6e  ying correlation
-0000a6c0: 206d 6174 7269 6365 7320 666f 6c6c 6f77   matrices follow
-0000a6d0: 2061 6e0a 2020 2020 4c4b 4a20 6469 7374   an.    LKJ dist
-0000a6e0: 7269 6275 7469 6f6e 205b 315d 2061 6e64  ribution [1] and
-0000a6f0: 2074 6865 2073 7461 6e64 6172 6420 6465   the standard de
-0000a700: 7669 6174 696f 6e73 2066 6f6c 6c6f 7720  viations follow 
-0000a710: 616e 2061 7262 6974 7261 7279 0a20 2020  an arbitrary.   
-0000a720: 2064 6973 7472 6962 7574 696f 6e20 7370   distribution sp
-0000a730: 6563 6966 6965 6420 6279 2074 6865 2075  ecified by the u
-0000a740: 7365 722e 0a0a 2020 2020 5061 7261 6d65  ser...    Parame
-0000a750: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000a760: 2d2d 2d0a 2020 2020 6e61 6d65 203a 2073  ---.    name : s
-0000a770: 7472 0a20 2020 2020 2020 2054 6865 206e  tr.        The n
-0000a780: 616d 6520 6769 7665 6e20 746f 2074 6865  ame given to the
-0000a790: 2076 6172 6961 626c 6520 696e 2074 6865   variable in the
-0000a7a0: 206d 6f64 656c 2e0a 2020 2020 6574 6120   model..    eta 
-0000a7b0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
-0000a7c0: 2066 6c6f 6174 0a20 2020 2020 2020 2054   float.        T
-0000a7d0: 6865 2073 6861 7065 2070 6172 616d 6574  he shape paramet
-0000a7e0: 6572 2028 6574 6120 3e20 3029 206f 6620  er (eta > 0) of 
-0000a7f0: 7468 6520 4c4b 4a20 6469 7374 7269 6275  the LKJ distribu
-0000a800: 7469 6f6e 2e20 6574 6120 3d20 310a 2020  tion. eta = 1.  
-0000a810: 2020 2020 2020 696d 706c 6965 7320 6120        implies a 
-0000a820: 756e 6966 6f72 6d20 6469 7374 7269 6275  uniform distribu
-0000a830: 7469 6f6e 206f 6620 7468 6520 636f 7272  tion of the corr
-0000a840: 656c 6174 696f 6e20 6d61 7472 6963 6573  elation matrices
-0000a850: 3b0a 2020 2020 2020 2020 6c61 7267 6572  ;.        larger
-0000a860: 2076 616c 7565 7320 7075 7420 6d6f 7265   values put more
-0000a870: 2077 6569 6768 7420 6f6e 206d 6174 7269   weight on matri
-0000a880: 6365 7320 7769 7468 2066 6577 2063 6f72  ces with few cor
-0000a890: 7265 6c61 7469 6f6e 732e 0a20 2020 206e  relations..    n
-0000a8a0: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-0000a8b0: 6620 696e 740a 2020 2020 2020 2020 4469  f int.        Di
-0000a8c0: 6d65 6e73 696f 6e20 6f66 2074 6865 2063  mension of the c
-0000a8d0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
-0000a8e0: 2028 6e20 3e20 3129 2e0a 2020 2020 7364   (n > 1)..    sd
-0000a8f0: 5f64 6973 7420 3a20 4469 7374 7269 6275  _dist : Distribu
-0000a900: 7469 6f6e 0a20 2020 2020 2020 2041 2070  tion.        A p
-0000a910: 6f73 6974 6976 6520 7363 616c 6172 206f  ositive scalar o
-0000a920: 7220 7665 6374 6f72 2064 6973 7472 6962  r vector distrib
-0000a930: 7574 696f 6e20 666f 7220 7468 6520 7374  ution for the st
-0000a940: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-0000a950: 732c 2063 7265 6174 6564 0a20 2020 2020  s, created.     
-0000a960: 2020 2077 6974 6820 7468 6520 602e 6469     with the `.di
-0000a970: 7374 2829 6020 4150 492e 2053 686f 756c  st()` API. Shoul
-0000a980: 6420 6861 7665 2060 7368 6170 655b 2d31  d have `shape[-1
-0000a990: 5d3d 6e60 2e20 5363 616c 6172 2064 6973  ]=n`. Scalar dis
-0000a9a0: 7472 6962 7574 696f 6e73 2077 696c 6c20  tributions will 
-0000a9b0: 6265 0a20 2020 2020 2020 2061 7574 6f6d  be.        autom
-0000a9c0: 6174 6963 616c 6c79 2072 6573 697a 6564  atically resized
-0000a9d0: 2074 6f20 656e 7375 7265 2074 6869 732e   to ensure this.
-0000a9e0: 0a0a 2020 2020 2020 2020 2e2e 2077 6172  ..        .. war
-0000a9f0: 6e69 6e67 3a3a 2073 645f 6469 7374 2077  ning:: sd_dist w
-0000aa00: 696c 6c20 6265 2063 6c6f 6e65 642c 2072  ill be cloned, r
-0000aa10: 656e 6465 7269 6e67 2069 7420 696e 6465  endering it inde
-0000aa20: 7065 6e64 656e 7420 6f66 2074 6865 206f  pendent of the o
-0000aa30: 6e65 2070 6173 7365 6420 6173 2069 6e70  ne passed as inp
-0000aa40: 7574 2e0a 0a20 2020 2063 6f6d 7075 7465  ut...    compute
-0000aa50: 5f63 6f72 7220 3a20 626f 6f6c 2c20 6465  _corr : bool, de
-0000aa60: 6661 756c 743d 5472 7565 0a20 2020 2020  fault=True.     
-0000aa70: 2020 2049 6620 6054 7275 6560 2c20 7265     If `True`, re
-0000aa80: 7475 726e 7320 7468 7265 6520 7661 6c75  turns three valu
-0000aa90: 6573 3a20 7468 6520 4368 6f6c 6573 6b79  es: the Cholesky
-0000aaa0: 2064 6563 6f6d 706f 7369 7469 6f6e 2c20   decomposition, 
-0000aab0: 7468 6520 636f 7272 656c 6174 696f 6e73  the correlations
-0000aac0: 0a20 2020 2020 2020 2061 6e64 2074 6865  .        and the
-0000aad0: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
-0000aae0: 696f 6e73 206f 6620 7468 6520 636f 7661  ions of the cova
-0000aaf0: 7269 616e 6365 206d 6174 7269 782e 204f  riance matrix. O
-0000ab00: 7468 6572 7769 7365 2c20 6f6e 6c79 2072  therwise, only r
-0000ab10: 6574 7572 6e73 0a20 2020 2020 2020 2074  eturns.        t
-0000ab20: 6865 2070 6163 6b65 6420 4368 6f6c 6573  he packed Choles
-0000ab30: 6b79 2064 6563 6f6d 706f 7369 7469 6f6e  ky decomposition
-0000ab40: 2e20 4465 6661 756c 7473 2074 6f20 6054  . Defaults to `T
-0000ab50: 7275 6560 2e0a 2020 2020 2020 2020 636f  rue`..        co
-0000ab60: 6d70 6174 6962 696c 6974 792e 0a20 2020  mpatibility..   
-0000ab70: 2073 746f 7265 5f69 6e5f 7472 6163 6520   store_in_trace 
-0000ab80: 3a20 626f 6f6c 2c20 6465 6661 756c 743d  : bool, default=
-0000ab90: 5472 7565 0a20 2020 2020 2020 2057 6865  True.        Whe
-0000aba0: 7468 6572 2074 6f20 7374 6f72 6520 7468  ther to store th
-0000abb0: 6520 636f 7272 656c 6174 696f 6e73 2061  e correlations a
-0000abc0: 6e64 2073 7461 6e64 6172 6420 6465 7669  nd standard devi
-0000abd0: 6174 696f 6e73 206f 6620 7468 6520 636f  ations of the co
-0000abe0: 7661 7269 616e 6365 0a20 2020 2020 2020  variance.       
-0000abf0: 206d 6174 7269 7820 696e 2074 6865 2070   matrix in the p
-0000ac00: 6f73 7465 7269 6f72 2074 7261 6365 2e20  osterior trace. 
-0000ac10: 4966 2060 5472 7565 602c 2074 6865 7920  If `True`, they 
-0000ac20: 7769 6c6c 2061 7574 6f6d 6174 6963 616c  will automatical
-0000ac30: 6c79 2062 6520 6e61 6d65 6420 6173 0a20  ly be named as. 
-0000ac40: 2020 2020 2020 2060 7b6e 616d 657d 5f63         `{name}_c
-0000ac50: 6f72 7260 2061 6e64 2060 7b6e 616d 657d  orr` and `{name}
-0000ac60: 5f73 7464 7360 2072 6573 7065 6374 6976  _stds` respectiv
-0000ac70: 656c 792e 2045 6666 6563 7469 7665 206f  ely. Effective o
-0000ac80: 6e6c 7920 7768 656e 0a20 2020 2020 2020  nly when.       
-0000ac90: 2060 636f 6d70 7574 655f 636f 7272 3d54   `compute_corr=T
-0000aca0: 7275 6560 2e0a 0a20 2020 2052 6574 7572  rue`...    Retur
-0000acb0: 6e73 0a20 2020 202d 2d2d 2d2d 2d2d 0a20  ns.    -------. 
-0000acc0: 2020 2063 686f 6c20 3a20 2054 656e 736f     chol :  Tenso
-0000acd0: 7256 6172 6961 626c 650a 2020 2020 2020  rVariable.      
-0000ace0: 2020 4966 2060 636f 6d70 7574 655f 636f    If `compute_co
-0000acf0: 7272 3d54 7275 6560 2e20 5468 6520 756e  rr=True`. The un
-0000ad00: 7061 636b 6564 2043 686f 6c65 736b 7920  packed Cholesky 
-0000ad10: 636f 7661 7269 616e 6365 2064 6563 6f6d  covariance decom
-0000ad20: 706f 7369 7469 6f6e 2e0a 2020 2020 636f  position..    co
-0000ad30: 7272 203a 2054 656e 736f 7256 6172 6961  rr : TensorVaria
-0000ad40: 626c 650a 2020 2020 2020 2020 4966 2060  ble.        If `
-0000ad50: 636f 6d70 7574 655f 636f 7272 3d54 7275  compute_corr=Tru
-0000ad60: 6560 2e20 5468 6520 636f 7272 656c 6174  e`. The correlat
-0000ad70: 696f 6e73 206f 6620 7468 6520 636f 7661  ions of the cova
-0000ad80: 7269 616e 6365 206d 6174 7269 782e 0a20  riance matrix.. 
-0000ad90: 2020 2073 7464 7320 3a20 5465 6e73 6f72     stds : Tensor
-0000ada0: 5661 7269 6162 6c65 0a20 2020 2020 2020  Variable.       
-0000adb0: 2049 6620 6063 6f6d 7075 7465 5f63 6f72   If `compute_cor
-0000adc0: 723d 5472 7565 602e 2054 6865 2073 7461  r=True`. The sta
-0000add0: 6e64 6172 6420 6465 7669 6174 696f 6e73  ndard deviations
-0000ade0: 206f 6620 7468 6520 636f 7661 7269 616e   of the covarian
-0000adf0: 6365 206d 6174 7269 782e 0a20 2020 2070  ce matrix..    p
-0000ae00: 6163 6b65 645f 6368 6f6c 203a 2054 656e  acked_chol : Ten
-0000ae10: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
-0000ae20: 2020 2020 4966 2060 636f 6d70 7574 655f      If `compute_
-0000ae30: 636f 7272 3d46 616c 7365 6020 5468 6520  corr=False` The 
-0000ae40: 7061 636b 6564 2043 686f 6c65 736b 7920  packed Cholesky 
-0000ae50: 636f 7661 7269 616e 6365 2064 6563 6f6d  covariance decom
-0000ae60: 706f 7369 7469 6f6e 2e0a 0a20 2020 204e  position...    N
-0000ae70: 6f74 6573 0a20 2020 202d 2d2d 2d2d 0a20  otes.    -----. 
-0000ae80: 2020 2053 696e 6365 2074 6865 2043 686f     Since the Cho
-0000ae90: 6c65 736b 7920 6661 6374 6f72 2069 7320  lesky factor is 
-0000aea0: 6120 6c6f 7765 7220 7472 6961 6e67 756c  a lower triangul
-0000aeb0: 6172 206d 6174 7269 782c 2077 6520 7573  ar matrix, we us
-0000aec0: 6520 7061 636b 6564 2073 746f 7261 6765  e packed storage
-0000aed0: 2066 6f72 0a20 2020 2074 6865 206d 6174   for.    the mat
-0000aee0: 7269 783a 2057 6520 7374 6f72 6520 7468  rix: We store th
-0000aef0: 6520 7661 6c75 6573 206f 6620 7468 6520  e values of the 
-0000af00: 6c6f 7765 7220 7472 6961 6e67 756c 6172  lower triangular
-0000af10: 206d 6174 7269 7820 696e 2061 206f 6e65   matrix in a one
-0000af20: 2d64 696d 656e 7369 6f6e 616c 0a20 2020  -dimensional.   
-0000af30: 2061 7272 6179 2c20 6e75 6d62 6572 6564   array, numbered
-0000af40: 2062 7920 726f 773a 3a0a 0a20 2020 2020   by row::..     
-0000af50: 2020 205b 5b30 202d 202d 202d 5d0a 2020     [[0 - - -].  
-0000af60: 2020 2020 2020 205b 3120 3220 2d20 2d5d         [1 2 - -]
-0000af70: 0a20 2020 2020 2020 2020 5b33 2034 2035  .         [3 4 5
-0000af80: 202d 5d0a 2020 2020 2020 2020 205b 3620   -].         [6 
-0000af90: 3720 3820 395d 5d0a 0a20 2020 2054 6865  7 8 9]]..    The
-0000afa0: 2075 6e70 6163 6b65 6420 4368 6f6c 6573   unpacked Choles
-0000afb0: 6b79 2063 6f76 6172 6961 6e63 6520 6d61  ky covariance ma
-0000afc0: 7472 6978 2069 7320 6175 746f 6d61 7469  trix is automati
-0000afd0: 6361 6c6c 7920 636f 6d70 7574 6564 2061  cally computed a
-0000afe0: 6e64 2072 6574 7572 6e65 6420 7768 656e  nd returned when
-0000aff0: 0a20 2020 2079 6f75 2073 7065 6369 6679  .    you specify
-0000b000: 2060 636f 6d70 7574 655f 636f 7272 3d54   `compute_corr=T
-0000b010: 7275 6560 2069 6e20 6070 6d2e 4c4b 4a43  rue` in `pm.LKJC
-0000b020: 686f 6c65 736b 7943 6f76 6020 2873 6565  holeskyCov` (see
-0000b030: 2065 7861 6d70 6c65 2062 656c 6f77 292e   example below).
-0000b040: 0a20 2020 204f 7468 6572 7769 7365 2c20  .    Otherwise, 
-0000b050: 796f 7520 6361 6e20 7573 6520 6070 6d2e  you can use `pm.
-0000b060: 6578 7061 6e64 5f70 6163 6b65 645f 7472  expand_packed_tr
-0000b070: 6961 6e67 756c 6172 2870 6163 6b65 645f  iangular(packed_
-0000b080: 636f 762c 206c 6f77 6572 3d54 7275 6529  cov, lower=True)
-0000b090: 600a 2020 2020 746f 2063 6f6e 7665 7274  `.    to convert
-0000b0a0: 2074 6865 2070 6163 6b65 6420 4368 6f6c   the packed Chol
-0000b0b0: 6573 6b79 206d 6174 7269 7820 746f 2061  esky matrix to a
-0000b0c0: 2072 6567 756c 6172 2074 776f 2d64 696d   regular two-dim
-0000b0d0: 656e 7369 6f6e 616c 2061 7272 6179 2e0a  ensional array..
-0000b0e0: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
-0000b0f0: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e    --------.    .
-0000b100: 2e20 636f 6465 3a3a 2070 7974 686f 6e0a  . code:: python.
-0000b110: 0a20 2020 2020 2020 2077 6974 6820 706d  .        with pm
-0000b120: 2e4d 6f64 656c 2829 2061 7320 6d6f 6465  .Model() as mode
-0000b130: 6c3a 0a20 2020 2020 2020 2020 2020 2023  l:.            #
-0000b140: 204e 6f74 6520 7468 6174 2077 6520 6163   Note that we ac
-0000b150: 6365 7373 2074 6865 2064 6973 7472 6962  cess the distrib
-0000b160: 7574 696f 6e20 666f 7220 7468 6520 7374  ution for the st
-0000b170: 616e 6461 7264 0a20 2020 2020 2020 2020  andard.         
-0000b180: 2020 2023 2064 6576 6961 7469 6f6e 732c     # deviations,
-0000b190: 2061 6e64 2064 6f20 6e6f 7420 6372 6561   and do not crea
-0000b1a0: 7465 2061 206e 6577 2072 616e 646f 6d20  te a new random 
-0000b1b0: 7661 7269 6162 6c65 2e0a 2020 2020 2020  variable..      
-0000b1c0: 2020 2020 2020 7364 5f64 6973 7420 3d20        sd_dist = 
-0000b1d0: 706d 2e45 7870 6f6e 656e 7469 616c 2e64  pm.Exponential.d
-0000b1e0: 6973 7428 312e 302c 2073 697a 653d 3130  ist(1.0, size=10
-0000b1f0: 290a 2020 2020 2020 2020 2020 2020 6368  ).            ch
-0000b200: 6f6c 2c20 636f 7272 2c20 7369 676d 6173  ol, corr, sigmas
-0000b210: 203d 2070 6d2e 4c4b 4a43 686f 6c65 736b   = pm.LKJCholesk
-0000b220: 7943 6f76 280a 2020 2020 2020 2020 2020  yCov(.          
-0000b230: 2020 2020 2020 2763 686f 6c5f 636f 7627        'chol_cov'
-0000b240: 2c20 6574 613d 342c 206e 3d31 302c 2073  , eta=4, n=10, s
-0000b250: 645f 6469 7374 3d73 645f 6469 7374 0a20  d_dist=sd_dist. 
-0000b260: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-0000b270: 2020 2020 2020 2020 2020 2320 6966 2079            # if y
-0000b280: 6f75 206f 6e6c 7920 7761 6e74 2074 6865  ou only want the
-0000b290: 2070 6163 6b65 6420 4368 6f6c 6573 6b79   packed Cholesky
-0000b2a0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-0000b2b0: 7061 636b 6564 5f63 686f 6c20 3d20 706d  packed_chol = pm
-0000b2c0: 2e4c 4b4a 4368 6f6c 6573 6b79 436f 7628  .LKJCholeskyCov(
-0000b2d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b2e0: 2027 6368 6f6c 5f63 6f76 272c 2065 7461   'chol_cov', eta
-0000b2f0: 3d34 2c20 6e3d 3130 2c20 7364 5f64 6973  =4, n=10, sd_dis
-0000b300: 743d 7364 5f64 6973 742c 2063 6f6d 7075  t=sd_dist, compu
-0000b310: 7465 5f63 6f72 723d 4661 6c73 650a 2020  te_corr=False.  
-0000b320: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000b330: 2020 2020 2020 2020 2320 6368 6f6c 203d          # chol =
-0000b340: 2070 6d2e 6578 7061 6e64 5f70 6163 6b65   pm.expand_packe
-0000b350: 645f 7472 6961 6e67 756c 6172 2831 302c  d_triangular(10,
-0000b360: 2070 6163 6b65 645f 6368 6f6c 2c20 6c6f   packed_chol, lo
-0000b370: 7765 723d 5472 7565 290a 0a20 2020 2020  wer=True)..     
-0000b380: 2020 2020 2020 2023 2044 6566 696e 6520         # Define 
-0000b390: 6120 6e65 7720 4d76 4e6f 726d 616c 2077  a new MvNormal w
-0000b3a0: 6974 6820 7468 6520 6769 7665 6e20 636f  ith the given co
-0000b3b0: 7661 7269 616e 6365 0a20 2020 2020 2020  variance.       
-0000b3c0: 2020 2020 2076 616c 7320 3d20 706d 2e4d       vals = pm.M
-0000b3d0: 764e 6f72 6d61 6c28 2776 616c 7327 2c20  vNormal('vals', 
-0000b3e0: 6d75 3d6e 702e 7a65 726f 7328 3130 292c  mu=np.zeros(10),
-0000b3f0: 2063 686f 6c3d 6368 6f6c 2c20 7368 6170   chol=chol, shap
-0000b400: 653d 3130 290a 0a20 2020 2020 2020 2020  e=10)..         
-0000b410: 2020 2023 204f 7220 7472 616e 7366 6f72     # Or transfor
-0000b420: 6d20 616e 2075 6e63 6f72 7265 6c61 7465  m an uncorrelate
-0000b430: 6420 6e6f 726d 616c 3a0a 2020 2020 2020  d normal:.      
-0000b440: 2020 2020 2020 7661 6c73 5f72 6177 203d        vals_raw =
-0000b450: 2070 6d2e 4e6f 726d 616c 2827 7661 6c73   pm.Normal('vals
-0000b460: 5f72 6177 272c 206d 753d 302c 2073 6967  _raw', mu=0, sig
-0000b470: 6d61 3d31 2c20 7368 6170 653d 3130 290a  ma=1, shape=10).
-0000b480: 2020 2020 2020 2020 2020 2020 7661 6c73              vals
-0000b490: 203d 2070 742e 646f 7428 6368 6f6c 2c20   = pt.dot(chol, 
-0000b4a0: 7661 6c73 5f72 6177 290a 0a20 2020 2020  vals_raw)..     
-0000b4b0: 2020 2020 2020 2023 204f 7220 636f 6d70         # Or comp
-0000b4c0: 7574 6520 7468 6520 636f 7661 7269 616e  ute the covarian
-0000b4d0: 6365 206d 6174 7269 780a 2020 2020 2020  ce matrix.      
-0000b4e0: 2020 2020 2020 636f 7620 3d20 7074 2e64        cov = pt.d
-0000b4f0: 6f74 2863 686f 6c2c 2063 686f 6c2e 5429  ot(chol, chol.T)
-0000b500: 0a0a 2020 2020 2a2a 496d 706c 656d 656e  ..    **Implemen
-0000b510: 7461 7469 6f6e 2a2a 2049 6e20 7468 6520  tation** In the 
-0000b520: 756e 636f 6e73 7472 6169 6e65 6420 7370  unconstrained sp
-0000b530: 6163 6520 616c 6c20 7661 6c75 6573 206f  ace all values o
-0000b540: 6620 7468 6520 6368 6f6c 6573 6b79 2066  f the cholesky f
-0000b550: 6163 746f 720a 2020 2020 6172 6520 7374  actor.    are st
-0000b560: 6f72 6564 2075 6e74 7261 6e73 666f 726d  ored untransform
-0000b570: 6564 2c20 6578 6365 7074 2066 6f72 2074  ed, except for t
-0000b580: 6865 2064 6961 676f 6e61 6c20 656e 7472  he diagonal entr
-0000b590: 6965 732c 2077 6865 7265 0a20 2020 2077  ies, where.    w
-0000b5a0: 6520 7573 6520 6120 6c6f 672d 7472 616e  e use a log-tran
-0000b5b0: 7366 6f72 6d20 746f 2072 6573 7472 6963  sform to restric
-0000b5c0: 7420 7468 656d 2074 6f20 706f 7369 7469  t them to positi
-0000b5d0: 7665 2076 616c 7565 732e 0a0a 2020 2020  ve values...    
-0000b5e0: 546f 2063 6f72 7265 6374 6c79 2063 6f6d  To correctly com
-0000b5f0: 7075 7465 206c 6f67 2d6c 696b 656c 6968  pute log-likelih
-0000b600: 6f6f 6473 2066 6f72 2074 6865 2073 7461  oods for the sta
-0000b610: 6e64 6172 6420 6465 7669 6174 696f 6e73  ndard deviations
-0000b620: 0a20 2020 2061 6e64 2074 6865 2063 6f72  .    and the cor
-0000b630: 7265 6c61 7469 6f6e 206d 6174 7269 7820  relation matrix 
-0000b640: 7365 7061 7261 7465 6c79 2c20 7765 206e  separately, we n
-0000b650: 6565 6420 746f 2063 6f6e 7369 6465 7220  eed to consider 
-0000b660: 610a 2020 2020 7365 636f 6e64 2074 7261  a.    second tra
-0000b670: 6e73 666f 726d 6174 696f 6e3a 2047 6976  nsformation: Giv
-0000b680: 656e 2061 2063 686f 6c65 736b 7920 6661  en a cholesky fa
-0000b690: 6374 6f72 697a 6174 696f 6e0a 2020 2020  ctorization.    
-0000b6a0: 3a6d 6174 683a 604c 4c5e 5420 3d20 5c53  :math:`LL^T = \S
-0000b6b0: 6967 6d61 6020 6f66 2061 2063 6f76 6172  igma` of a covar
-0000b6c0: 6961 6e63 6520 6d61 7472 6978 2077 6520  iance matrix we 
-0000b6d0: 6361 6e20 7265 636f 7665 7220 7468 650a  can recover the.
-0000b6e0: 2020 2020 7374 616e 6461 7264 2064 6576      standard dev
-0000b6f0: 6961 7469 6f6e 7320 3a6d 6174 683a 605c  iations :math:`\
-0000b700: 7369 676d 6160 2061 7320 7468 6520 6575  sigma` as the eu
-0000b710: 636c 6964 6561 6e20 6c65 6e67 7468 7320  clidean lengths 
-0000b720: 6f66 0a20 2020 2074 6865 2072 6f77 7320  of.    the rows 
-0000b730: 6f66 203a 6d61 7468 3a60 4c60 2c20 616e  of :math:`L`, an
-0000b740: 6420 7468 6520 6368 6f6c 6573 6b79 2066  d the cholesky f
-0000b750: 6163 746f 7220 6f66 2074 6865 0a20 2020  actor of the.   
-0000b760: 2063 6f72 7265 6c61 7469 6f6e 206d 6174   correlation mat
-0000b770: 7269 7820 6173 203a 6d61 7468 3a60 5520  rix as :math:`U 
-0000b780: 3d20 5c74 6578 747b 6469 6167 7d28 5c73  = \text{diag}(\s
-0000b790: 6967 6d61 295e 7b2d 317d 4c60 2e0a 2020  igma)^{-1}L`..  
-0000b7a0: 2020 5369 6e63 6520 6561 6368 2072 6f77    Since each row
-0000b7b0: 206f 6620 3a6d 6174 683a 6055 6020 6861   of :math:`U` ha
-0000b7c0: 7320 6c65 6e67 7468 2031 2c20 7765 2064  s length 1, we d
-0000b7d0: 6f20 6e6f 7420 6e65 6564 2074 6f0a 2020  o not need to.  
-0000b7e0: 2020 7374 6f72 6520 7468 6520 6469 6167    store the diag
-0000b7f0: 6f6e 616c 2e20 5765 2064 6566 696e 6520  onal. We define 
-0000b800: 6120 7472 616e 7366 6f72 6d61 7469 6f6e  a transformation
-0000b810: 203a 6d61 7468 3a60 5c70 6869 600a 2020   :math:`\phi`.  
-0000b820: 2020 7375 6368 2074 6861 7420 3a6d 6174    such that :mat
-0000b830: 683a 605c 7068 6928 4c29 6020 6973 2074  h:`\phi(L)` is t
-0000b840: 6865 206c 6f77 6572 2074 7269 616e 6775  he lower triangu
-0000b850: 6c61 7220 6d61 7472 6978 2063 6f6e 7461  lar matrix conta
-0000b860: 696e 696e 670a 2020 2020 7468 6520 7374  ining.    the st
-0000b870: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
-0000b880: 7320 3a6d 6174 683a 605c 7369 676d 6160  s :math:`\sigma`
-0000b890: 206f 6e20 7468 6520 6469 6167 6f6e 616c   on the diagonal
-0000b8a0: 2061 6e64 2074 6865 0a20 2020 2063 6f72   and the.    cor
-0000b8b0: 7265 6c61 7469 6f6e 206d 6174 7269 7820  relation matrix 
-0000b8c0: 3a6d 6174 683a 6055 6020 6265 6c6f 772e  :math:`U` below.
-0000b8d0: 2049 6e20 7468 6973 2066 6f72 6d20 7765   In this form we
-0000b8e0: 2063 616e 2065 6173 696c 790a 2020 2020   can easily.    
-0000b8f0: 636f 6d70 7574 6520 7468 6520 6469 6666  compute the diff
-0000b900: 6572 656e 7420 6c69 6b65 6c69 686f 6f64  erent likelihood
-0000b910: 7320 7365 7061 7261 7465 6c79 2c20 6173  s separately, as
-0000b920: 2074 6865 206c 696b 656c 6968 6f6f 640a   the likelihood.
-0000b930: 2020 2020 6f66 2074 6865 2063 6f72 7265      of the corre
-0000b940: 6c61 7469 6f6e 206d 6174 7269 7820 6f6e  lation matrix on
-0000b950: 6c79 2064 6570 656e 6473 206f 6e20 7468  ly depends on th
-0000b960: 6520 7661 6c75 6573 2062 656c 6f77 2074  e values below t
-0000b970: 6865 0a20 2020 2064 6961 676f 6e61 6c2c  he.    diagonal,
-0000b980: 2061 6e64 2074 6865 206c 696b 656c 6968   and the likelih
-0000b990: 6f6f 6420 6f66 2074 6865 2073 7461 6e64  ood of the stand
-0000b9a0: 6172 6420 6465 7669 6174 696f 6e20 6465  ard deviation de
-0000b9b0: 7065 6e64 730a 2020 2020 6f6e 6c79 206f  pends.    only o
-0000b9c0: 6e20 7468 6520 6469 6167 6f6e 616c 2076  n the diagonal v
-0000b9d0: 616c 7565 732e 0a0a 2020 2020 5765 2073  alues...    We s
-0000b9e0: 7469 6c6c 206e 6565 6420 7468 6520 6465  till need the de
-0000b9f0: 7465 726d 696e 616e 7420 6f66 2074 6865  terminant of the
-0000ba00: 206a 6163 6f62 6961 6e20 6f66 203a 6d61   jacobian of :ma
-0000ba10: 7468 3a60 5c70 6869 5e7b 2d31 7d60 2e0a  th:`\phi^{-1}`..
-0000ba20: 2020 2020 4966 2077 6520 7468 696e 6b20      If we think 
-0000ba30: 6f66 203a 6d61 7468 3a60 5c70 6869 6020  of :math:`\phi` 
-0000ba40: 6173 2061 6e20 6175 746f 6d6f 7270 6869  as an automorphi
-0000ba50: 736d 206f 6e0a 2020 2020 3a6d 6174 683a  sm on.    :math:
-0000ba60: 605c 6d61 7468 6262 7b52 7d5e 7b5c 7466  `\mathbb{R}^{\tf
-0000ba70: 7261 637b 6e28 6e2b 3129 7d7b 327d 7d60  rac{n(n+1)}{2}}`
-0000ba80: 2c20 7768 6572 6520 7765 206f 7264 6572  , where we order
-0000ba90: 0a20 2020 2074 6865 2064 696d 656e 7369  .    the dimensi
-0000baa0: 6f6e 7320 6173 2064 6573 6372 6962 6564  ons as described
-0000bab0: 2069 6e20 7468 6520 6e6f 7465 7320 6162   in the notes ab
-0000bac0: 6f76 652c 2074 6865 206a 6163 6f62 6961  ove, the jacobia
-0000bad0: 6e0a 2020 2020 6973 2061 2062 6c6f 636b  n.    is a block
-0000bae0: 2d64 6961 676f 6e61 6c20 6d61 7472 6978  -diagonal matrix
-0000baf0: 2c20 7768 6572 6520 6561 6368 2062 6c6f  , where each blo
-0000bb00: 636b 2063 6f72 7265 7370 6f6e 6473 2074  ck corresponds t
-0000bb10: 6f0a 2020 2020 6f6e 6520 726f 7720 6f66  o.    one row of
-0000bb20: 203a 6d61 7468 3a60 5560 2e20 4561 6368   :math:`U`. Each
-0000bb30: 2062 6c6f 636b 2068 6173 2061 7272 6f77   block has arrow
-0000bb40: 6865 6164 2073 6861 7065 2c20 616e 6420  head shape, and 
-0000bb50: 7765 0a20 2020 2063 616e 2063 6f6d 7075  we.    can compu
-0000bb60: 7465 2074 6865 2064 6574 6572 6d69 6e61  te the determina
-0000bb70: 6e74 206f 6620 7468 6174 2061 7320 6465  nt of that as de
-0000bb80: 7363 7269 6265 6420 696e 205b 325d 2e20  scribed in [2]. 
-0000bb90: 5369 6e63 650a 2020 2020 7468 6520 6465  Since.    the de
-0000bba0: 7465 726d 696e 616e 7420 6f66 2061 2062  terminant of a b
-0000bbb0: 6c6f 636b 2d64 6961 676f 6e61 6c20 6d61  lock-diagonal ma
-0000bbc0: 7472 6978 2069 7320 7468 6520 7072 6f64  trix is the prod
-0000bbd0: 7563 740a 2020 2020 6f66 2074 6865 2064  uct.    of the d
-0000bbe0: 6574 6572 6d69 6e61 6e74 7320 6f66 2074  eterminants of t
-0000bbf0: 6865 2062 6c6f 636b 732c 2077 6520 6765  he blocks, we ge
-0000bc00: 740a 0a20 2020 202e 2e20 6d61 7468 3a3a  t..    .. math::
-0000bc10: 0a0a 2020 2020 2020 205c 7465 7874 7b64  ..       \text{d
-0000bc20: 6574 7d28 4a5f 7b5c 7068 695e 7b2d 317d  et}(J_{\phi^{-1}
-0000bc30: 7d28 5529 2920 3d0a 2020 2020 2020 205c  }(U)) =.       \
-0000bc40: 6c65 6674 5b0a 2020 2020 2020 2020 205c  left[.         \
-0000bc50: 7072 6f64 5f7b 693d 327d 5e4e 2075 5f7b  prod_{i=2}^N u_{
-0000bc60: 6969 7d5e 7b69 202d 2031 7d20 4c5f 7b69  ii}^{i - 1} L_{i
-0000bc70: 697d 0a20 2020 2020 2020 5c72 6967 6874  i}.       \right
-0000bc80: 5d5e 7b2d 317d 0a0a 2020 2020 5265 6665  ]^{-1}..    Refe
-0000bc90: 7265 6e63 6573 0a20 2020 202d 2d2d 2d2d  rences.    -----
-0000bca0: 2d2d 2d2d 2d0a 2020 2020 2e2e 205b 315d  -----.    .. [1]
-0000bcb0: 204c 6577 616e 646f 7773 6b69 2c20 442e   Lewandowski, D.
-0000bcc0: 2c20 4b75 726f 7769 636b 612c 2044 2e20  , Kurowicka, D. 
-0000bcd0: 616e 6420 4a6f 652c 2048 2e20 2832 3030  and Joe, H. (200
-0000bce0: 3929 2e0a 2020 2020 2020 2022 4765 6e65  9)..       "Gene
-0000bcf0: 7261 7469 6e67 2072 616e 646f 6d20 636f  rating random co
-0000bd00: 7272 656c 6174 696f 6e20 6d61 7472 6963  rrelation matric
-0000bd10: 6573 2062 6173 6564 206f 6e20 7669 6e65  es based on vine
-0000bd20: 7320 616e 640a 2020 2020 2020 2065 7874  s and.       ext
-0000bd30: 656e 6465 6420 6f6e 696f 6e20 6d65 7468  ended onion meth
-0000bd40: 6f64 2e22 204a 6f75 726e 616c 206f 6620  od." Journal of 
-0000bd50: 6d75 6c74 6976 6172 6961 7465 2061 6e61  multivariate ana
-0000bd60: 6c79 7369 732c 0a20 2020 2020 2020 3130  lysis,.       10
-0000bd70: 3028 3929 2c20 7070 2e31 3938 392d 3230  0(9), pp.1989-20
-0000bd80: 3031 2e0a 0a20 2020 202e 2e20 5b32 5d20  01...    .. [2] 
-0000bd90: 4a2e 204d 2e20 6973 6e27 7420 6120 6d61  J. M. isn't a ma
-0000bda0: 7468 656d 6174 6963 6961 6e20 2868 7474  thematician (htt
-0000bdb0: 703a 2f2f 6d61 7468 2e73 7461 636b 6578  p://math.stackex
-0000bdc0: 6368 616e 6765 2e63 6f6d 2f75 7365 7273  change.com/users
-0000bdd0: 2f34 3938 2f0a 2020 2020 2020 206a 2d6d  /498/.       j-m
-0000bde0: 2d69 736e 742d 612d 6d61 7468 656d 6174  -isnt-a-mathemat
-0000bdf0: 6963 6961 6e29 2c20 4469 6666 6572 656e  ician), Differen
-0000be00: 7420 6170 7072 6f61 6368 6573 2074 6f20  t approaches to 
-0000be10: 6576 616c 7561 7465 2074 6869 730a 2020  evaluate this.  
-0000be20: 2020 2020 2064 6574 6572 6d69 6e61 6e74       determinant
-0000be30: 2c20 5552 4c20 2876 6572 7369 6f6e 3a20  , URL (version: 
-0000be40: 3230 3132 2d30 342d 3134 293a 0a20 2020  2012-04-14):.   
-0000be50: 2020 2020 6874 7470 3a2f 2f6d 6174 682e      http://math.
-0000be60: 7374 6163 6b65 7863 6861 6e67 652e 636f  stackexchange.co
-0000be70: 6d2f 712f 3133 3030 3236 0a20 2020 2022  m/q/130026.    "
-0000be80: 2222 0a0a 2020 2020 6465 6620 5f5f 6e65  ""..    def __ne
-0000be90: 775f 5f28 636c 732c 206e 616d 652c 2065  w__(cls, name, e
-0000bea0: 7461 2c20 6e2c 2073 645f 6469 7374 2c20  ta, n, sd_dist, 
-0000beb0: 2a2c 2063 6f6d 7075 7465 5f63 6f72 723d  *, compute_corr=
-0000bec0: 5472 7565 2c20 7374 6f72 655f 696e 5f74  True, store_in_t
-0000bed0: 7261 6365 3d54 7275 652c 202a 2a6b 7761  race=True, **kwa
-0000bee0: 7267 7329 3a0a 2020 2020 2020 2020 7061  rgs):.        pa
-0000bef0: 636b 6564 5f63 686f 6c20 3d20 5f4c 4b4a  cked_chol = _LKJ
-0000bf00: 4368 6f6c 6573 6b79 436f 7628 6e61 6d65  CholeskyCov(name
-0000bf10: 2c20 6574 613d 6574 612c 206e 3d6e 2c20  , eta=eta, n=n, 
-0000bf20: 7364 5f64 6973 743d 7364 5f64 6973 742c  sd_dist=sd_dist,
-0000bf30: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
-0000bf40: 2020 2069 6620 6e6f 7420 636f 6d70 7574     if not comput
-0000bf50: 655f 636f 7272 3a0a 2020 2020 2020 2020  e_corr:.        
-0000bf60: 2020 2020 7265 7475 726e 2070 6163 6b65      return packe
-0000bf70: 645f 6368 6f6c 0a20 2020 2020 2020 2065  d_chol.        e
-0000bf80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000bf90: 2063 686f 6c2c 2063 6f72 722c 2073 7464   chol, corr, std
-0000bfa0: 7320 3d20 636c 732e 6865 6c70 6572 5f64  s = cls.helper_d
-0000bfb0: 6574 6572 6d69 6e69 7374 6963 7328 6e2c  eterministics(n,
-0000bfc0: 2070 6163 6b65 645f 6368 6f6c 290a 2020   packed_chol).  
-0000bfd0: 2020 2020 2020 2020 2020 6966 2073 746f            if sto
-0000bfe0: 7265 5f69 6e5f 7472 6163 653a 0a20 2020  re_in_trace:.   
-0000bff0: 2020 2020 2020 2020 2020 2020 2063 6f72               cor
-0000c000: 7220 3d20 706d 2e44 6574 6572 6d69 6e69  r = pm.Determini
-0000c010: 7374 6963 2866 227b 6e61 6d65 7d5f 636f  stic(f"{name}_co
-0000c020: 7272 222c 2063 6f72 7229 0a20 2020 2020  rr", corr).     
-0000c030: 2020 2020 2020 2020 2020 2073 7464 7320             stds 
-0000c040: 3d20 706d 2e44 6574 6572 6d69 6e69 7374  = pm.Determinist
-0000c050: 6963 2866 227b 6e61 6d65 7d5f 7374 6473  ic(f"{name}_stds
-0000c060: 222c 2073 7464 7329 0a20 2020 2020 2020  ", stds).       
-0000c070: 2020 2020 2072 6574 7572 6e20 6368 6f6c       return chol
-0000c080: 2c20 636f 7272 2c20 7374 6473 0a0a 2020  , corr, stds..  
-0000c090: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
-0000c0a0: 2020 2064 6566 2064 6973 7428 636c 732c     def dist(cls,
-0000c0b0: 2065 7461 2c20 6e2c 2073 645f 6469 7374   eta, n, sd_dist
-0000c0c0: 2c20 2a2c 2063 6f6d 7075 7465 5f63 6f72  , *, compute_cor
-0000c0d0: 723d 5472 7565 2c20 2a2a 6b77 6172 6773  r=True, **kwargs
-0000c0e0: 293a 0a20 2020 2020 2020 2023 2063 6f6d  ):.        # com
-0000c0f0: 7075 7465 2043 686f 6c65 736b 7920 6465  pute Cholesky de
-0000c100: 636f 6d70 6f73 6974 696f 6e0a 2020 2020  composition.    
-0000c110: 2020 2020 7061 636b 6564 5f63 686f 6c20      packed_chol 
-0000c120: 3d20 5f4c 4b4a 4368 6f6c 6573 6b79 436f  = _LKJCholeskyCo
-0000c130: 762e 6469 7374 2865 7461 3d65 7461 2c20  v.dist(eta=eta, 
-0000c140: 6e3d 6e2c 2073 645f 6469 7374 3d73 645f  n=n, sd_dist=sd_
-0000c150: 6469 7374 2c20 2a2a 6b77 6172 6773 290a  dist, **kwargs).
-0000c160: 2020 2020 2020 2020 6966 206e 6f74 2063          if not c
-0000c170: 6f6d 7075 7465 5f63 6f72 723a 0a20 2020  ompute_corr:.   
-0000c180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000c190: 7061 636b 6564 5f63 686f 6c0a 2020 2020  packed_chol.    
-0000c1a0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-0000c1b0: 2020 2020 2020 7265 7475 726e 2063 6c73        return cls
-0000c1c0: 2e68 656c 7065 725f 6465 7465 726d 696e  .helper_determin
-0000c1d0: 6973 7469 6373 286e 2c20 7061 636b 6564  istics(n, packed
-0000c1e0: 5f63 686f 6c29 0a0a 2020 2020 4063 6c61  _chol)..    @cla
-0000c1f0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-0000c200: 2068 656c 7065 725f 6465 7465 726d 696e   helper_determin
-0000c210: 6973 7469 6373 2863 6c73 2c20 6e2c 2070  istics(cls, n, p
-0000c220: 6163 6b65 645f 6368 6f6c 293a 0a20 2020  acked_chol):.   
-0000c230: 2020 2020 2063 686f 6c20 3d20 706d 2e65       chol = pm.e
-0000c240: 7870 616e 645f 7061 636b 6564 5f74 7269  xpand_packed_tri
-0000c250: 616e 6775 6c61 7228 6e2c 2070 6163 6b65  angular(n, packe
-0000c260: 645f 6368 6f6c 2c20 6c6f 7765 723d 5472  d_chol, lower=Tr
-0000c270: 7565 290a 2020 2020 2020 2020 2320 636f  ue).        # co
-0000c280: 6d70 7574 6520 636f 7661 7269 616e 6365  mpute covariance
-0000c290: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-0000c2a0: 636f 7620 3d20 7074 2e64 6f74 2863 686f  cov = pt.dot(cho
-0000c2b0: 6c2c 2063 686f 6c2e 5429 0a20 2020 2020  l, chol.T).     
-0000c2c0: 2020 2023 2065 7874 7261 6374 2073 7461     # extract sta
-0000c2d0: 6e64 6172 6420 6465 7669 6174 696f 6e73  ndard deviations
-0000c2e0: 2061 6e64 2072 686f 0a20 2020 2020 2020   and rho.       
-0000c2f0: 2073 7464 7320 3d20 7074 2e73 7172 7428   stds = pt.sqrt(
-0000c300: 7074 2e64 6961 6728 636f 7629 290a 2020  pt.diag(cov)).  
-0000c310: 2020 2020 2020 696e 765f 7374 6473 203d        inv_stds =
-0000c320: 2031 202f 2073 7464 730a 2020 2020 2020   1 / stds.      
-0000c330: 2020 636f 7272 203d 2069 6e76 5f73 7464    corr = inv_std
-0000c340: 735b 4e6f 6e65 2c20 3a5d 202a 2063 6f76  s[None, :] * cov
-0000c350: 202a 2069 6e76 5f73 7464 735b 3a2c 204e   * inv_stds[:, N
-0000c360: 6f6e 655d 0a20 2020 2020 2020 2072 6574  one].        ret
-0000c370: 7572 6e20 6368 6f6c 2c20 636f 7272 2c20  urn chol, corr, 
-0000c380: 7374 6473 0a0a 0a63 6c61 7373 204c 4b4a  stds...class LKJ
-0000c390: 436f 7272 5256 2852 616e 646f 6d56 6172  CorrRV(RandomVar
-0000c3a0: 6961 626c 6529 3a0a 2020 2020 6e61 6d65  iable):.    name
-0000c3b0: 203d 2022 6c6b 6a63 6f72 7222 0a20 2020   = "lkjcorr".   
-0000c3c0: 206e 6469 6d5f 7375 7070 203d 2031 0a20   ndim_supp = 1. 
-0000c3d0: 2020 206e 6469 6d73 5f70 6172 616d 7320     ndims_params 
-0000c3e0: 3d20 5b30 2c20 305d 0a20 2020 2064 7479  = [0, 0].    dty
-0000c3f0: 7065 203d 2022 666c 6f61 7458 220a 2020  pe = "floatX".  
-0000c400: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
-0000c410: 2822 4c4b 4a43 6f72 7252 5622 2c20 225c  ("LKJCorrRV", "\
-0000c420: 5c6f 7065 7261 746f 726e 616d 657b 4c4b  \operatorname{LK
-0000c430: 4a43 6f72 7252 567d 2229 0a0a 2020 2020  JCorrRV}")..    
-0000c440: 6465 6620 6d61 6b65 5f6e 6f64 6528 7365  def make_node(se
-0000c450: 6c66 2c20 726e 672c 2073 697a 652c 2064  lf, rng, size, d
-0000c460: 7479 7065 2c20 6e2c 2065 7461 293a 0a20  type, n, eta):. 
-0000c470: 2020 2020 2020 206e 203d 2070 742e 6173         n = pt.as
-0000c480: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-0000c490: 286e 290a 2020 2020 2020 2020 6966 206e  (n).        if n
-0000c4a0: 6f74 206e 2e6e 6469 6d20 3d3d 2030 3a0a  ot n.ndim == 0:.
-0000c4b0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000c4c0: 6520 5661 6c75 6545 7272 6f72 2822 6e20  e ValueError("n 
-0000c4d0: 6d75 7374 2062 6520 6120 7363 616c 6172  must be a scalar
-0000c4e0: 2028 6e64 696d 3d30 292e 2229 0a0a 2020   (ndim=0).")..  
-0000c4f0: 2020 2020 2020 6574 6120 3d20 7074 2e61        eta = pt.a
-0000c500: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-0000c510: 6528 6574 6129 0a20 2020 2020 2020 2069  e(eta).        i
-0000c520: 6620 6e6f 7420 6574 612e 6e64 696d 203d  f not eta.ndim =
-0000c530: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-0000c540: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000c550: 7228 2265 7461 206d 7573 7420 6265 2061  r("eta must be a
-0000c560: 2073 6361 6c61 7220 286e 6469 6d3d 3029   scalar (ndim=0)
-0000c570: 2e22 290a 0a20 2020 2020 2020 2072 6574  .")..        ret
-0000c580: 7572 6e20 7375 7065 7228 292e 6d61 6b65  urn super().make
-0000c590: 5f6e 6f64 6528 726e 672c 2073 697a 652c  _node(rng, size,
-0000c5a0: 2064 7479 7065 2c20 6e2c 2065 7461 290a   dtype, n, eta).
-0000c5b0: 0a20 2020 2064 6566 205f 7375 7070 5f73  .    def _supp_s
-0000c5c0: 6861 7065 5f66 726f 6d5f 7061 7261 6d73  hape_from_params
-0000c5d0: 2873 656c 662c 2064 6973 745f 7061 7261  (self, dist_para
-0000c5e0: 6d73 2c20 2a2a 6b77 6172 6773 293a 0a20  ms, **kwargs):. 
-0000c5f0: 2020 2020 2020 206e 203d 2064 6973 745f         n = dist_
-0000c600: 7061 7261 6d73 5b30 5d0a 2020 2020 2020  params[0].      
-0000c610: 2020 6469 7374 5f73 6861 7065 203d 2028    dist_shape = (
-0000c620: 286e 202a 2028 6e20 2d20 3129 2920 2f2f  (n * (n - 1)) //
-0000c630: 2032 2c29 0a20 2020 2020 2020 2072 6574   2,).        ret
-0000c640: 7572 6e20 6469 7374 5f73 6861 7065 0a0a  urn dist_shape..
-0000c650: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
-0000c660: 0a20 2020 2064 6566 2072 6e67 5f66 6e28  .    def rng_fn(
-0000c670: 636c 732c 2072 6e67 2c20 6e2c 2065 7461  cls, rng, n, eta
-0000c680: 2c20 7369 7a65 293a 0a20 2020 2020 2020  , size):.       
-0000c690: 2023 2057 6520 666c 6174 7465 6e20 7468   # We flatten th
-0000c6a0: 6520 7369 7a65 2074 6f20 6d61 6b65 206f  e size to make o
-0000c6b0: 7065 7261 7469 6f6e 7320 6561 7369 6572  perations easier
-0000c6c0: 2c20 616e 6420 7468 656e 2072 6562 7569  , and then rebui
-0000c6d0: 6c64 2069 740a 2020 2020 2020 2020 6966  ld it.        if
-0000c6e0: 2073 697a 6520 6973 204e 6f6e 653a 0a20   size is None:. 
-0000c6f0: 2020 2020 2020 2020 2020 2066 6c61 745f             flat_
-0000c700: 7369 7a65 203d 2031 0a20 2020 2020 2020  size = 1.       
-0000c710: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000c720: 2020 2066 6c61 745f 7369 7a65 203d 206e     flat_size = n
-0000c730: 702e 7072 6f64 2873 697a 6529 0a0a 2020  p.prod(size)..  
-0000c740: 2020 2020 2020 4320 3d20 636c 732e 5f72        C = cls._r
-0000c750: 616e 646f 6d5f 636f 7272 5f6d 6174 7269  andom_corr_matri
-0000c760: 7828 726e 673d 726e 672c 206e 3d6e 2c20  x(rng=rng, n=n, 
-0000c770: 6574 613d 6574 612c 2066 6c61 745f 7369  eta=eta, flat_si
-0000c780: 7a65 3d66 6c61 745f 7369 7a65 290a 0a20  ze=flat_size).. 
-0000c790: 2020 2020 2020 2074 7269 755f 6964 7820         triu_idx 
-0000c7a0: 3d20 6e70 2e74 7269 755f 696e 6469 6365  = np.triu_indice
-0000c7b0: 7328 6e2c 206b 3d31 290a 2020 2020 2020  s(n, k=1).      
-0000c7c0: 2020 7361 6d70 6c65 7320 3d20 435b 2e2e    samples = C[..
-0000c7d0: 2e2c 2074 7269 755f 6964 785b 305d 2c20  ., triu_idx[0], 
-0000c7e0: 7472 6975 5f69 6478 5b31 5d5d 0a0a 2020  triu_idx[1]]..  
-0000c7f0: 2020 2020 2020 6966 2073 697a 6520 6973        if size is
-0000c800: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000c810: 2020 2073 616d 706c 6573 203d 2073 616d     samples = sam
-0000c820: 706c 6573 5b30 5d0a 2020 2020 2020 2020  ples[0].        
-0000c830: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000c840: 2020 6469 7374 5f73 6861 7065 203d 2028    dist_shape = (
-0000c850: 6e20 2a20 286e 202d 2031 2929 202f 2f20  n * (n - 1)) // 
-0000c860: 320a 2020 2020 2020 2020 2020 2020 7361  2.            sa
-0000c870: 6d70 6c65 7320 3d20 6e70 2e72 6573 6861  mples = np.resha
-0000c880: 7065 2873 616d 706c 6573 2c20 282a 7369  pe(samples, (*si
-0000c890: 7a65 2c20 6469 7374 5f73 6861 7065 2929  ze, dist_shape))
-0000c8a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c8b0: 7361 6d70 6c65 730a 0a20 2020 2040 636c  samples..    @cl
-0000c8c0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-0000c8d0: 6620 5f72 616e 646f 6d5f 636f 7272 5f6d  f _random_corr_m
-0000c8e0: 6174 7269 7828 636c 732c 2072 6e67 2c20  atrix(cls, rng, 
-0000c8f0: 6e2c 2065 7461 2c20 666c 6174 5f73 697a  n, eta, flat_siz
-0000c900: 6529 3a0a 2020 2020 2020 2020 2320 6f72  e):.        # or
-0000c910: 6967 696e 616c 2069 6d70 6c65 6d65 6e74  iginal implement
-0000c920: 6174 696f 6e20 696e 2052 2073 6565 3a0a  ation in R see:.
-0000c930: 2020 2020 2020 2020 2320 6874 7470 733a          # https:
-0000c940: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6d63  //github.com/rmc
-0000c950: 656c 7265 6174 682f 7265 7468 696e 6b69  elreath/rethinki
-0000c960: 6e67 2f62 6c6f 622f 6d61 7374 6572 2f52  ng/blob/master/R
-0000c970: 2f64 6973 7472 6962 7574 696f 6e73 2e72  /distributions.r
-0000c980: 0a20 2020 2020 2020 2062 6574 6120 3d20  .        beta = 
-0000c990: 6574 6120 2d20 312e 3020 2b20 6e20 2f20  eta - 1.0 + n / 
-0000c9a0: 322e 300a 2020 2020 2020 2020 7231 3220  2.0.        r12 
-0000c9b0: 3d20 322e 3020 2a20 7374 6174 732e 6265  = 2.0 * stats.be
-0000c9c0: 7461 2e72 7673 2861 3d62 6574 612c 2062  ta.rvs(a=beta, b
-0000c9d0: 3d62 6574 612c 2073 697a 653d 666c 6174  =beta, size=flat
-0000c9e0: 5f73 697a 652c 2072 616e 646f 6d5f 7374  _size, random_st
-0000c9f0: 6174 653d 726e 6729 202d 2031 2e30 0a20  ate=rng) - 1.0. 
-0000ca00: 2020 2020 2020 2050 203d 206e 702e 6675         P = np.fu
-0000ca10: 6c6c 2828 666c 6174 5f73 697a 652c 206e  ll((flat_size, n
-0000ca20: 2c20 6e29 2c20 6e70 2e65 7965 286e 2929  , n), np.eye(n))
-0000ca30: 0a20 2020 2020 2020 2050 5b2e 2e2e 2c20  .        P[..., 
-0000ca40: 302c 2031 5d20 3d20 7231 320a 2020 2020  0, 1] = r12.    
-0000ca50: 2020 2020 505b 2e2e 2e2c 2031 2c20 315d      P[..., 1, 1]
-0000ca60: 203d 206e 702e 7371 7274 2831 2e30 202d   = np.sqrt(1.0 -
-0000ca70: 2072 3132 2a2a 3229 0a20 2020 2020 2020   r12**2).       
-0000ca80: 2066 6f72 206d 7031 2069 6e20 7261 6e67   for mp1 in rang
-0000ca90: 6528 322c 206e 293a 0a20 2020 2020 2020  e(2, n):.       
-0000caa0: 2020 2020 2062 6574 6120 2d3d 2030 2e35       beta -= 0.5
-0000cab0: 0a20 2020 2020 2020 2020 2020 2079 203d  .            y =
-0000cac0: 2073 7461 7473 2e62 6574 612e 7276 7328   stats.beta.rvs(
-0000cad0: 613d 6d70 3120 2f20 322e 302c 2062 3d62  a=mp1 / 2.0, b=b
-0000cae0: 6574 612c 2073 697a 653d 666c 6174 5f73  eta, size=flat_s
-0000caf0: 697a 652c 2072 616e 646f 6d5f 7374 6174  ize, random_stat
-0000cb00: 653d 726e 6729 0a20 2020 2020 2020 2020  e=rng).         
-0000cb10: 2020 207a 203d 2073 7461 7473 2e6e 6f72     z = stats.nor
-0000cb20: 6d2e 7276 7328 6c6f 633d 302c 2073 6361  m.rvs(loc=0, sca
-0000cb30: 6c65 3d31 2c20 7369 7a65 3d28 666c 6174  le=1, size=(flat
-0000cb40: 5f73 697a 652c 206d 7031 292c 2072 616e  _size, mp1), ran
-0000cb50: 646f 6d5f 7374 6174 653d 726e 6729 0a20  dom_state=rng). 
-0000cb60: 2020 2020 2020 2020 2020 207a 203d 207a             z = z
-0000cb70: 202f 206e 702e 7371 7274 286e 702e 6569   / np.sqrt(np.ei
-0000cb80: 6e73 756d 2822 696a 2c69 6a2d 3e69 222c  nsum("ij,ij->i",
-0000cb90: 207a 2c20 7a29 295b 2e2e 2e2c 206e 702e   z, z))[..., np.
-0000cba0: 6e65 7761 7869 735d 0a20 2020 2020 2020  newaxis].       
-0000cbb0: 2020 2020 2050 5b2e 2e2e 2c20 303a 6d70       P[..., 0:mp
-0000cbc0: 312c 206d 7031 5d20 3d20 6e70 2e73 7172  1, mp1] = np.sqr
-0000cbd0: 7428 795b 2e2e 2e2c 206e 702e 6e65 7761  t(y[..., np.newa
-0000cbe0: 7869 735d 2920 2a20 7a0a 2020 2020 2020  xis]) * z.      
-0000cbf0: 2020 2020 2020 505b 2e2e 2e2c 206d 7031        P[..., mp1
-0000cc00: 2c20 6d70 315d 203d 206e 702e 7371 7274  , mp1] = np.sqrt
-0000cc10: 2831 2e30 202d 2079 290a 2020 2020 2020  (1.0 - y).      
-0000cc20: 2020 4320 3d20 6e70 2e65 696e 7375 6d28    C = np.einsum(
-0000cc30: 222e 2e2e 6a69 2c2e 2e2e 6a6b 2d3e 2e2e  "...ji,...jk->..
-0000cc40: 2e69 6b22 2c20 502c 2050 290a 2020 2020  .ik", P, P).    
-0000cc50: 2020 2020 7265 7475 726e 2043 0a0a 0a6c      return C...l
-0000cc60: 6b6a 636f 7272 203d 204c 4b4a 436f 7272  kjcorr = LKJCorr
-0000cc70: 5256 2829 0a0a 0a63 6c61 7373 204c 4b4a  RV()...class LKJ
-0000cc80: 436f 7272 2842 6f75 6e64 6564 436f 6e74  Corr(BoundedCont
-0000cc90: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
-0000cca0: 220a 2020 2020 5468 6520 4c4b 4a20 284c  ".    The LKJ (L
-0000ccb0: 6577 616e 646f 7773 6b69 2c20 4b75 726f  ewandowski, Kuro
-0000ccc0: 7769 636b 6120 616e 6420 4a6f 6529 206c  wicka and Joe) l
-0000ccd0: 6f67 2d6c 696b 656c 6968 6f6f 642e 0a0a  og-likelihood...
-0000cce0: 2020 2020 5468 6520 4c4b 4a20 6469 7374      The LKJ dist
-0000ccf0: 7269 6275 7469 6f6e 2069 7320 6120 7072  ribution is a pr
-0000cd00: 696f 7220 6469 7374 7269 6275 7469 6f6e  ior distribution
-0000cd10: 2066 6f72 2063 6f72 7265 6c61 7469 6f6e   for correlation
-0000cd20: 206d 6174 7269 6365 732e 0a20 2020 2049   matrices..    I
-0000cd30: 6620 6574 6120 3d20 3120 7468 6973 2063  f eta = 1 this c
-0000cd40: 6f72 7265 7370 6f6e 6473 2074 6f20 7468  orresponds to th
-0000cd50: 6520 756e 6966 6f72 6d20 6469 7374 7269  e uniform distri
-0000cd60: 6275 7469 6f6e 206f 7665 7220 636f 7272  bution over corr
-0000cd70: 656c 6174 696f 6e0a 2020 2020 6d61 7472  elation.    matr
-0000cd80: 6963 6573 2e20 466f 7220 6574 6120 2d3e  ices. For eta ->
-0000cd90: 206f 6f20 7468 6520 4c4b 4a20 7072 696f   oo the LKJ prio
-0000cda0: 7220 6170 7072 6f61 6368 6573 2074 6865  r approaches the
-0000cdb0: 2069 6465 6e74 6974 7920 6d61 7472 6978   identity matrix
-0000cdc0: 2e0a 0a20 2020 203d 3d3d 3d3d 3d3d 3d20  ...    ======== 
-0000cdd0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-0000cde0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000cdf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-0000ce00: 2020 2020 5375 7070 6f72 7420 2020 5570      Support   Up
-0000ce10: 7065 7220 7472 6961 6e67 756c 6172 206d  per triangular m
-0000ce20: 6174 7269 7820 7769 7468 2076 616c 7565  atrix with value
-0000ce30: 7320 696e 205b 2d31 2c20 315d 0a20 2020  s in [-1, 1].   
-0000ce40: 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d   ========  =====
-0000ce50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ce60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000ce70: 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050  =========..    P
-0000ce80: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
-0000ce90: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206e 203a  --------.    n :
-0000cea0: 2074 656e 736f 725f 6c69 6b65 206f 6620   tensor_like of 
-0000ceb0: 696e 740a 2020 2020 2020 2020 4469 6d65  int.        Dime
-0000cec0: 6e73 696f 6e20 6f66 2074 6865 2063 6f76  nsion of the cov
-0000ced0: 6172 6961 6e63 6520 6d61 7472 6978 2028  ariance matrix (
-0000cee0: 6e20 3e20 3129 2e0a 2020 2020 6574 6120  n > 1)..    eta 
-0000cef0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
-0000cf00: 2066 6c6f 6174 0a20 2020 2020 2020 2054   float.        T
-0000cf10: 6865 2073 6861 7065 2070 6172 616d 6574  he shape paramet
-0000cf20: 6572 2028 6574 6120 3e20 3029 206f 6620  er (eta > 0) of 
-0000cf30: 7468 6520 4c4b 4a20 6469 7374 7269 6275  the LKJ distribu
-0000cf40: 7469 6f6e 2e20 6574 6120 3d20 310a 2020  tion. eta = 1.  
-0000cf50: 2020 2020 2020 696d 706c 6965 7320 6120        implies a 
-0000cf60: 756e 6966 6f72 6d20 6469 7374 7269 6275  uniform distribu
-0000cf70: 7469 6f6e 206f 6620 7468 6520 636f 7272  tion of the corr
-0000cf80: 656c 6174 696f 6e20 6d61 7472 6963 6573  elation matrices
-0000cf90: 3b0a 2020 2020 2020 2020 6c61 7267 6572  ;.        larger
-0000cfa0: 2076 616c 7565 7320 7075 7420 6d6f 7265   values put more
-0000cfb0: 2077 6569 6768 7420 6f6e 206d 6174 7269   weight on matri
-0000cfc0: 6365 7320 7769 7468 2066 6577 2063 6f72  ces with few cor
-0000cfd0: 7265 6c61 7469 6f6e 732e 0a0a 2020 2020  relations...    
-0000cfe0: 4e6f 7465 730a 2020 2020 2d2d 2d2d 2d0a  Notes.    -----.
-0000cff0: 2020 2020 5468 6973 2069 6d70 6c65 6d65      This impleme
-0000d000: 6e74 6174 696f 6e20 6f6e 6c79 2072 6574  ntation only ret
-0000d010: 7572 6e73 2074 6865 2076 616c 7565 7320  urns the values 
-0000d020: 6f66 2074 6865 2075 7070 6572 2074 7269  of the upper tri
-0000d030: 616e 6775 6c61 720a 2020 2020 6d61 7472  angular.    matr
-0000d040: 6978 2065 7863 6c75 6469 6e67 2074 6865  ix excluding the
-0000d050: 2064 6961 676f 6e61 6c2e 2048 6572 6520   diagonal. Here 
-0000d060: 6973 2061 2073 6368 656d 6174 6963 2066  is a schematic f
-0000d070: 6f72 206e 203d 2035 2c20 7368 6f77 696e  or n = 5, showin
-0000d080: 670a 2020 2020 7468 6520 696e 6465 7865  g.    the indexe
-0000d090: 7320 6f66 2074 6865 2065 6c65 6d65 6e74  s of the element
-0000d0a0: 733a 3a0a 0a20 2020 2020 2020 205b 5b2d  s::..        [[-
-0000d0b0: 2030 2031 2032 2033 5d0a 2020 2020 2020   0 1 2 3].      
-0000d0c0: 2020 205b 2d20 2d20 3420 3520 365d 0a20     [- - 4 5 6]. 
-0000d0d0: 2020 2020 2020 2020 5b2d 202d 202d 2037          [- - - 7
-0000d0e0: 2038 5d0a 2020 2020 2020 2020 205b 2d20   8].         [- 
-0000d0f0: 2d20 2d20 2d20 395d 0a20 2020 2020 2020  - - - 9].       
-0000d100: 2020 5b2d 202d 202d 202d 202d 5d5d 0a0a    [- - - - -]]..
-0000d110: 0a20 2020 2052 6566 6572 656e 6365 730a  .    References.
-0000d120: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
-0000d130: 2020 202e 2e20 5b4c 4b4a 3230 3039 5d20     .. [LKJ2009] 
-0000d140: 4c65 7761 6e64 6f77 736b 692c 2044 2e2c  Lewandowski, D.,
-0000d150: 204b 7572 6f77 6963 6b61 2c20 442e 2061   Kurowicka, D. a
-0000d160: 6e64 204a 6f65 2c20 482e 2028 3230 3039  nd Joe, H. (2009
-0000d170: 292e 0a20 2020 2020 2020 2022 4765 6e65  )..        "Gene
-0000d180: 7261 7469 6e67 2072 616e 646f 6d20 636f  rating random co
-0000d190: 7272 656c 6174 696f 6e20 6d61 7472 6963  rrelation matric
-0000d1a0: 6573 2062 6173 6564 206f 6e20 7669 6e65  es based on vine
-0000d1b0: 7320 616e 640a 2020 2020 2020 2020 6578  s and.        ex
-0000d1c0: 7465 6e64 6564 206f 6e69 6f6e 206d 6574  tended onion met
-0000d1d0: 686f 642e 2220 4a6f 7572 6e61 6c20 6f66  hod." Journal of
-0000d1e0: 206d 756c 7469 7661 7269 6174 6520 616e   multivariate an
-0000d1f0: 616c 7973 6973 2c0a 2020 2020 2020 2020  alysis,.        
-0000d200: 3130 3028 3929 2c20 7070 2e31 3938 392d  100(9), pp.1989-
-0000d210: 3230 3031 2e0a 2020 2020 2222 220a 0a20  2001..    """.. 
-0000d220: 2020 2072 765f 6f70 203d 206c 6b6a 636f     rv_op = lkjco
-0000d230: 7272 0a0a 2020 2020 4063 6c61 7373 6d65  rr..    @classme
-0000d240: 7468 6f64 0a20 2020 2064 6566 2064 6973  thod.    def dis
-0000d250: 7428 636c 732c 206e 2c20 6574 612c 202a  t(cls, n, eta, *
-0000d260: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-0000d270: 2020 6e20 3d20 7074 2e61 735f 7465 6e73    n = pt.as_tens
-0000d280: 6f72 5f76 6172 6961 626c 6528 696e 7458  or_variable(intX
-0000d290: 286e 2929 0a20 2020 2020 2020 2065 7461  (n)).        eta
-0000d2a0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-0000d2b0: 7661 7269 6162 6c65 2866 6c6f 6174 5828  variable(floatX(
-0000d2c0: 6574 6129 290a 2020 2020 2020 2020 7265  eta)).        re
-0000d2d0: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
-0000d2e0: 7428 5b6e 2c20 6574 615d 2c20 2a2a 6b77  t([n, eta], **kw
-0000d2f0: 6172 6773 290a 0a20 2020 2064 6566 206d  args)..    def m
-0000d300: 6f6d 656e 7428 7276 2c20 2a61 7267 7329  oment(rv, *args)
-0000d310: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-0000d320: 2070 742e 7a65 726f 735f 6c69 6b65 2872   pt.zeros_like(r
-0000d330: 7629 0a0a 2020 2020 6465 6620 6c6f 6770  v)..    def logp
-0000d340: 2876 616c 7565 2c20 6e2c 2065 7461 293a  (value, n, eta):
-0000d350: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d360: 2020 2020 2043 616c 6375 6c61 7465 206c       Calculate l
-0000d370: 6f67 2d70 726f 6261 6269 6c69 7479 206f  og-probability o
-0000d380: 6620 4c4b 4a20 6469 7374 7269 6275 7469  f LKJ distributi
-0000d390: 6f6e 2061 7420 7370 6563 6966 6965 640a  on at specified.
-0000d3a0: 2020 2020 2020 2020 7661 6c75 652e 0a0a          value...
-0000d3b0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-0000d3c0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-0000d3d0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7661  -----.        va
-0000d3e0: 6c75 653a 206e 756d 6572 6963 0a20 2020  lue: numeric.   
-0000d3f0: 2020 2020 2020 2020 2056 616c 7565 2066           Value f
-0000d400: 6f72 2077 6869 6368 206c 6f67 2d70 726f  or which log-pro
-0000d410: 6261 6269 6c69 7479 2069 7320 6361 6c63  bability is calc
-0000d420: 756c 6174 6564 2e0a 0a20 2020 2020 2020  ulated...       
-0000d430: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-0000d440: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-0000d450: 2054 656e 736f 7256 6172 6961 626c 650a   TensorVariable.
-0000d460: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-0000d470: 2020 2020 2023 2054 4f44 4f3a 2050 7954       # TODO: PyT
-0000d480: 656e 736f 7220 646f 6573 206e 6f74 2068  ensor does not h
-0000d490: 6176 6520 6120 6074 7269 755f 696e 6469  ave a `triu_indi
-0000d4a0: 6365 7360 2c20 736f 2077 6520 6361 6e20  ces`, so we can 
-0000d4b0: 6f6e 6c79 2077 6f72 6b20 7769 7468 2063  only work with c
-0000d4c0: 6f6e 7374 616e 740a 2020 2020 2020 2020  onstant.        
-0000d4d0: 2320 206e 2028 6f72 2065 6c73 6520 6669  #  n (or else fi
-0000d4e0: 6e64 2061 2064 6966 6665 7265 6e74 2065  nd a different e
-0000d4f0: 7870 7265 7373 696f 6e29 0a20 2020 2020  xpression).     
-0000d500: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-0000d510: 616e 6365 286e 2c20 436f 6e73 7461 6e74  ance(n, Constant
-0000d520: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-0000d530: 6169 7365 204e 6f74 496d 706c 656d 656e  aise NotImplemen
-0000d540: 7465 6445 7272 6f72 2822 6c6f 6770 206f  tedError("logp o
-0000d550: 6e6c 7920 696d 706c 656d 656e 7465 6420  nly implemented 
-0000d560: 666f 7220 636f 6e73 7461 6e74 2060 6e60  for constant `n`
-0000d570: 2229 0a0a 2020 2020 2020 2020 6e20 3d20  ")..        n = 
-0000d580: 696e 7428 6e2e 6461 7461 290a 2020 2020  int(n.data).    
-0000d590: 2020 2020 7368 6170 6520 3d20 6e20 2a20      shape = n * 
-0000d5a0: 286e 202d 2031 2920 2f2f 2032 0a20 2020  (n - 1) // 2.   
-0000d5b0: 2020 2020 2074 7269 5f69 6e64 6578 203d       tri_index =
-0000d5c0: 206e 702e 7a65 726f 7328 286e 2c20 6e29   np.zeros((n, n)
-0000d5d0: 2c20 6474 7970 653d 2269 6e74 3332 2229  , dtype="int32")
-0000d5e0: 0a20 2020 2020 2020 2074 7269 5f69 6e64  .        tri_ind
-0000d5f0: 6578 5b6e 702e 7472 6975 5f69 6e64 6963  ex[np.triu_indic
-0000d600: 6573 286e 2c20 6b3d 3129 5d20 3d20 6e70  es(n, k=1)] = np
-0000d610: 2e61 7261 6e67 6528 7368 6170 6529 0a20  .arange(shape). 
-0000d620: 2020 2020 2020 2074 7269 5f69 6e64 6578         tri_index
-0000d630: 5b6e 702e 7472 6975 5f69 6e64 6963 6573  [np.triu_indices
-0000d640: 286e 2c20 6b3d 3129 5b3a 3a2d 315d 5d20  (n, k=1)[::-1]] 
-0000d650: 3d20 6e70 2e61 7261 6e67 6528 7368 6170  = np.arange(shap
-0000d660: 6529 0a0a 2020 2020 2020 2020 7661 6c75  e)..        valu
-0000d670: 6520 3d20 7074 2e74 616b 6528 7661 6c75  e = pt.take(valu
-0000d680: 652c 2074 7269 5f69 6e64 6578 290a 2020  e, tri_index).  
-0000d690: 2020 2020 2020 7661 6c75 6520 3d20 7074        value = pt
-0000d6a0: 2e66 696c 6c5f 6469 6167 6f6e 616c 2876  .fill_diagonal(v
-0000d6b0: 616c 7565 2c20 3129 0a0a 2020 2020 2020  alue, 1)..      
-0000d6c0: 2020 2320 544f 444f 3a20 5f6c 6b6a 5f6e    # TODO: _lkj_n
-0000d6d0: 6f72 6d61 6c69 7a69 6e67 5f63 6f6e 7374  ormalizing_const
-0000d6e0: 616e 7420 6375 7272 656e 746c 7920 7265  ant currently re
-0000d6f0: 7175 6972 6573 2060 6574 6160 2061 6e64  quires `eta` and
-0000d700: 2060 6e60 2074 6f20 6265 2063 6f6e 7374   `n` to be const
-0000d710: 616e 7473 0a20 2020 2020 2020 2069 6620  ants.        if 
-0000d720: 6e6f 7420 6973 696e 7374 616e 6365 2865  not isinstance(e
-0000d730: 7461 2c20 436f 6e73 7461 6e74 293a 0a20  ta, Constant):. 
-0000d740: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000d750: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-0000d760: 7272 6f72 2822 6c6f 6770 206f 6e6c 7920  rror("logp only 
-0000d770: 696d 706c 656d 656e 7465 6420 666f 7220  implemented for 
-0000d780: 636f 6e73 7461 6e74 2060 6574 6160 2229  constant `eta`")
-0000d790: 0a20 2020 2020 2020 2065 7461 203d 2066  .        eta = f
-0000d7a0: 6c6f 6174 2865 7461 2e64 6174 6129 0a20  loat(eta.data). 
-0000d7b0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000d7c0: 5f6c 6b6a 5f6e 6f72 6d61 6c69 7a69 6e67  _lkj_normalizing
-0000d7d0: 5f63 6f6e 7374 616e 7428 6574 612c 206e  _constant(eta, n
-0000d7e0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
-0000d7f0: 202b 3d20 2865 7461 202d 2031 2e30 2920   += (eta - 1.0) 
-0000d800: 2a20 7074 2e6c 6f67 2864 6574 2876 616c  * pt.log(det(val
-0000d810: 7565 2929 0a20 2020 2020 2020 2072 6574  ue)).        ret
-0000d820: 7572 6e20 6368 6563 6b5f 7061 7261 6d65  urn check_parame
-0000d830: 7465 7273 280a 2020 2020 2020 2020 2020  ters(.          
-0000d840: 2020 7265 7375 6c74 2c0a 2020 2020 2020    result,.      
-0000d850: 2020 2020 2020 7661 6c75 6520 3e3d 202d        value >= -
-0000d860: 312c 0a20 2020 2020 2020 2020 2020 2076  1,.            v
-0000d870: 616c 7565 203c 3d20 312c 0a20 2020 2020  alue <= 1,.     
-0000d880: 2020 2020 2020 206d 6174 7269 785f 706f         matrix_po
-0000d890: 735f 6465 6628 7661 6c75 6529 2c0a 2020  s_def(value),.  
-0000d8a0: 2020 2020 2020 2020 2020 6574 6120 3e20            eta > 
-0000d8b0: 302c 0a20 2020 2020 2020 2029 0a0a 0a40  0,.        )...@
-0000d8c0: 5f64 6566 6175 6c74 5f74 7261 6e73 666f  _default_transfo
-0000d8d0: 726d 2e72 6567 6973 7465 7228 4c4b 4a43  rm.register(LKJC
-0000d8e0: 6f72 7229 0a64 6566 206c 6b6a 636f 7272  orr).def lkjcorr
-0000d8f0: 5f64 6566 6175 6c74 5f74 7261 6e73 666f  _default_transfo
-0000d900: 726d 286f 702c 2072 7629 3a0a 2020 2020  rm(op, rv):.    
-0000d910: 7265 7475 726e 2049 6e74 6572 7661 6c28  return Interval(
-0000d920: 666c 6f61 7458 282d 312e 3029 2c20 666c  floatX(-1.0), fl
-0000d930: 6f61 7458 2831 2e30 2929 0a0a 0a63 6c61  oatX(1.0))...cla
-0000d940: 7373 204d 6174 7269 784e 6f72 6d61 6c52  ss MatrixNormalR
-0000d950: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
-0000d960: 293a 0a20 2020 206e 616d 6520 3d20 226d  ):.    name = "m
-0000d970: 6174 7269 786e 6f72 6d61 6c22 0a20 2020  atrixnormal".   
-0000d980: 206e 6469 6d5f 7375 7070 203d 2032 0a20   ndim_supp = 2. 
-0000d990: 2020 206e 6469 6d73 5f70 6172 616d 7320     ndims_params 
-0000d9a0: 3d20 5b32 2c20 322c 2032 5d0a 2020 2020  = [2, 2, 2].    
-0000d9b0: 6474 7970 6520 3d20 2266 6c6f 6174 5822  dtype = "floatX"
-0000d9c0: 0a20 2020 205f 7072 696e 745f 6e61 6d65  .    _print_name
-0000d9d0: 203d 2028 224d 6174 7269 784e 6f72 6d61   = ("MatrixNorma
-0000d9e0: 6c22 2c20 225c 5c6f 7065 7261 746f 726e  l", "\\operatorn
-0000d9f0: 616d 657b 4d61 7472 6978 4e6f 726d 616c  ame{MatrixNormal
-0000da00: 7d22 290a 0a20 2020 2064 6566 205f 696e  }")..    def _in
-0000da10: 6665 725f 7368 6170 6528 7365 6c66 2c20  fer_shape(self, 
-0000da20: 7369 7a65 2c20 6469 7374 5f70 6172 616d  size, dist_param
-0000da30: 732c 2070 6172 616d 5f73 6861 7065 733d  s, param_shapes=
-0000da40: 4e6f 6e65 293a 0a20 2020 2020 2020 2073  None):.        s
-0000da50: 6861 7065 203d 2074 7570 6c65 2873 697a  hape = tuple(siz
-0000da60: 6529 202b 2074 7570 6c65 2864 6973 745f  e) + tuple(dist_
-0000da70: 7061 7261 6d73 5b30 5d2e 7368 6170 655b  params[0].shape[
-0000da80: 2d32 3a5d 290a 2020 2020 2020 2020 7265  -2:]).        re
-0000da90: 7475 726e 2073 6861 7065 0a0a 2020 2020  turn shape..    
-0000daa0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-0000dab0: 2064 6566 2072 6e67 5f66 6e28 636c 732c   def rng_fn(cls,
-0000dac0: 2072 6e67 2c20 6d75 2c20 726f 7763 686f   rng, mu, rowcho
-0000dad0: 6c2c 2063 6f6c 6368 6f6c 2c20 7369 7a65  l, colchol, size
-0000dae0: 3d4e 6f6e 6529 3a0a 2020 2020 2020 2020  =None):.        
-0000daf0: 7369 7a65 203d 2074 6f5f 7475 706c 6528  size = to_tuple(
-0000db00: 7369 7a65 290a 2020 2020 2020 2020 6469  size).        di
-0000db10: 7374 5f73 6861 7065 203d 2074 6f5f 7475  st_shape = to_tu
-0000db20: 706c 6528 5b72 6f77 6368 6f6c 2e73 6861  ple([rowchol.sha
-0000db30: 7065 5b30 5d2c 2063 6f6c 6368 6f6c 2e73  pe[0], colchol.s
-0000db40: 6861 7065 5b30 5d5d 290a 2020 2020 2020  hape[0]]).      
-0000db50: 2020 6f75 7470 7574 5f73 6861 7065 203d    output_shape =
-0000db60: 2073 697a 6520 2b20 6469 7374 5f73 6861   size + dist_sha
-0000db70: 7065 0a0a 2020 2020 2020 2020 2320 4272  pe..        # Br
-0000db80: 6f61 6463 6173 7469 6e67 2061 6c6c 2070  oadcasting all p
-0000db90: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000dba0: 2020 7368 6170 6573 203d 205b 6d75 2e73    shapes = [mu.s
-0000dbb0: 6861 7065 2c20 6f75 7470 7574 5f73 6861  hape, output_sha
-0000dbc0: 7065 5d0a 2020 2020 2020 2020 6272 6f61  pe].        broa
-0000dbd0: 6463 6173 7461 626c 655f 7368 6170 6520  dcastable_shape 
-0000dbe0: 3d20 6272 6f61 6463 6173 745f 6469 7374  = broadcast_dist
-0000dbf0: 5f73 616d 706c 6573 5f73 6861 7065 2873  _samples_shape(s
-0000dc00: 6861 7065 732c 2073 697a 653d 7369 7a65  hapes, size=size
-0000dc10: 290a 2020 2020 2020 2020 6d75 203d 206e  ).        mu = n
-0000dc20: 702e 6272 6f61 6463 6173 745f 746f 286d  p.broadcast_to(m
-0000dc30: 752c 2073 6861 7065 3d62 726f 6164 6361  u, shape=broadca
-0000dc40: 7374 6162 6c65 5f73 6861 7065 290a 2020  stable_shape).  
-0000dc50: 2020 2020 2020 726f 7763 686f 6c20 3d20        rowchol = 
-0000dc60: 6e70 2e62 726f 6164 6361 7374 5f74 6f28  np.broadcast_to(
-0000dc70: 726f 7763 686f 6c2c 2073 6861 7065 3d73  rowchol, shape=s
-0000dc80: 697a 6520 2b20 726f 7763 686f 6c2e 7368  ize + rowchol.sh
-0000dc90: 6170 655b 2d32 3a5d 290a 0a20 2020 2020  ape[-2:])..     
-0000dca0: 2020 2063 6f6c 6368 6f6c 203d 206e 702e     colchol = np.
-0000dcb0: 6272 6f61 6463 6173 745f 746f 2863 6f6c  broadcast_to(col
-0000dcc0: 6368 6f6c 2c20 7368 6170 653d 7369 7a65  chol, shape=size
-0000dcd0: 202b 2063 6f6c 6368 6f6c 2e73 6861 7065   + colchol.shape
-0000dce0: 5b2d 323a 5d29 0a20 2020 2020 2020 2063  [-2:]).        c
-0000dcf0: 6f6c 6368 6f6c 203d 206e 702e 7377 6170  olchol = np.swap
-0000dd00: 6178 6573 2863 6f6c 6368 6f6c 2c20 2d31  axes(colchol, -1
-0000dd10: 2c20 2d32 2920 2023 2054 616b 6520 7472  , -2)  # Take tr
-0000dd20: 616e 7370 6f73 650a 0a20 2020 2020 2020  anspose..       
-0000dd30: 2073 7461 6e64 6172 645f 6e6f 726d 616c   standard_normal
-0000dd40: 203d 2072 6e67 2e73 7461 6e64 6172 645f   = rng.standard_
-0000dd50: 6e6f 726d 616c 286f 7574 7075 745f 7368  normal(output_sh
-0000dd60: 6170 6529 0a20 2020 2020 2020 2073 616d  ape).        sam
-0000dd70: 706c 6573 203d 206d 7520 2b20 6e70 2e6d  ples = mu + np.m
-0000dd80: 6174 6d75 6c28 726f 7763 686f 6c2c 206e  atmul(rowchol, n
-0000dd90: 702e 6d61 746d 756c 2873 7461 6e64 6172  p.matmul(standar
-0000dda0: 645f 6e6f 726d 616c 2c20 636f 6c63 686f  d_normal, colcho
-0000ddb0: 6c29 290a 0a20 2020 2020 2020 2072 6574  l))..        ret
-0000ddc0: 7572 6e20 7361 6d70 6c65 730a 0a0a 6d61  urn samples...ma
-0000ddd0: 7472 6978 6e6f 726d 616c 203d 204d 6174  trixnormal = Mat
-0000dde0: 7269 784e 6f72 6d61 6c52 5628 290a 0a0a  rixNormalRV()...
-0000ddf0: 636c 6173 7320 4d61 7472 6978 4e6f 726d  class MatrixNorm
-0000de00: 616c 2843 6f6e 7469 6e75 6f75 7329 3a0a  al(Continuous):.
-0000de10: 2020 2020 7222 2222 0a20 2020 204d 6174      r""".    Mat
-0000de20: 7269 782d 7661 6c75 6564 206e 6f72 6d61  rix-valued norma
-0000de30: 6c20 6c6f 672d 6c69 6b65 6c69 686f 6f64  l log-likelihood
-0000de40: 2e0a 0a20 2020 202e 2e20 6d61 7468 3a3a  ...    .. math::
-0000de50: 0a20 2020 2020 2020 6628 7820 5c6d 6964  .       f(x \mid
-0000de60: 205c 6d75 2c20 552c 2056 2920 3d0a 2020   \mu, U, V) =.  
-0000de70: 2020 2020 2020 2020 205c 6672 6163 7b31           \frac{1
-0000de80: 7d7b 2832 5c70 695e 7b6d 206e 7d20 7c55  }{(2\pi^{m n} |U
-0000de90: 7c5e 6e20 7c56 7c5e 6d29 5e7b 312f 327d  |^n |V|^m)^{1/2}
-0000dea0: 7d0a 2020 2020 2020 2020 2020 205c 6578  }.           \ex
-0000deb0: 705c 6c65 6674 5c7b 0a20 2020 2020 2020  p\left\{.       
-0000dec0: 2020 2020 2020 2020 202d 5c66 7261 637b           -\frac{
-0000ded0: 317d 7b32 7d20 5c6d 6174 6872 6d7b 5472  1}{2} \mathrm{Tr
-0000dee0: 7d5b 2056 5e7b 2d31 7d20 2878 2d5c 6d75  }[ V^{-1} (x-\mu
-0000def0: 295e 7b5c 7072 696d 657d 2055 5e7b 2d31  )^{\prime} U^{-1
-0000df00: 7d20 2878 2d5c 6d75 295d 0a20 2020 2020  } (x-\mu)].     
-0000df10: 2020 2020 2020 205c 7269 6768 745c 7d0a         \right\}.
-0000df20: 0a20 2020 203d 3d3d 3d3d 3d3d 3d3d 3d3d  .    ===========
-0000df30: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
-0000df40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000df50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-0000df60: 5375 7070 6f72 7420 2020 2020 2020 2020  Support         
-0000df70: 203a 6d61 7468 3a60 7820 5c69 6e20 5c6d   :math:`x \in \m
-0000df80: 6174 6862 627b 527d 5e7b 6d20 5c74 696d  athbb{R}^{m \tim
-0000df90: 6573 206e 7d60 0a20 2020 204d 6561 6e20  es n}`.    Mean 
-0000dfa0: 2020 2020 2020 2020 2020 2020 3a6d 6174              :mat
-0000dfb0: 683a 605c 6d75 600a 2020 2020 526f 7720  h:`\mu`.    Row 
-0000dfc0: 5661 7269 616e 6365 2020 2020 203a 6d61  Variance     :ma
-0000dfd0: 7468 3a60 5560 0a20 2020 2043 6f6c 756d  th:`U`.    Colum
-0000dfe0: 6e20 5661 7269 616e 6365 2020 3a6d 6174  n Variance  :mat
-0000dff0: 683a 6056 600a 2020 2020 3d3d 3d3d 3d3d  h:`V`.    ======
-0000e000: 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d  =========  =====
-0000e010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000e020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000e030: 0a0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0000e040: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-0000e050: 2020 2020 6d75 203a 2074 656e 736f 725f      mu : tensor_
-0000e060: 6c69 6b65 206f 6620 666c 6f61 740a 2020  like of float.  
-0000e070: 2020 2020 2020 4172 7261 7920 6f66 206d        Array of m
-0000e080: 6561 6e73 2e20 4d75 7374 2062 6520 6272  eans. Must be br
-0000e090: 6f61 6463 6173 7461 626c 6520 7769 7468  oadcastable with
-0000e0a0: 2074 6865 2072 616e 646f 6d20 7661 7269   the random vari
-0000e0b0: 6162 6c65 2058 2073 7563 680a 2020 2020  able X such.    
-0000e0c0: 2020 2020 7468 6174 2074 6865 2073 6861      that the sha
-0000e0d0: 7065 206f 6620 6d75 202b 2058 2069 7320  pe of mu + X is 
-0000e0e0: 284d 2c20 4e29 2e0a 2020 2020 726f 7763  (M, N)..    rowc
-0000e0f0: 6f76 203a 2028 4d2c 204d 2920 7465 6e73  ov : (M, M) tens
-0000e100: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
-0000e110: 2c20 6f70 7469 6f6e 616c 0a20 2020 2020  , optional.     
-0000e120: 2020 2041 6d6f 6e67 2d72 6f77 2063 6f76     Among-row cov
-0000e130: 6172 6961 6e63 6520 6d61 7472 6978 2e20  ariance matrix. 
-0000e140: 4465 6669 6e65 7320 7661 7269 616e 6365  Defines variance
-0000e150: 2077 6974 6869 6e0a 2020 2020 2020 2020   within.        
-0000e160: 636f 6c75 6d6e 732e 2045 7861 6374 6c79  columns. Exactly
-0000e170: 206f 6e65 206f 6620 726f 7763 6f76 206f   one of rowcov o
-0000e180: 7220 726f 7763 686f 6c20 6973 206e 6565  r rowchol is nee
-0000e190: 6465 642e 0a20 2020 2072 6f77 6368 6f6c  ded..    rowchol
-0000e1a0: 203a 2028 4d2c 204d 2920 7465 6e73 6f72   : (M, M) tensor
-0000e1b0: 5f6c 696b 6520 6f66 2066 6c6f 6174 2c20  _like of float, 
-0000e1c0: 6f70 7469 6f6e 616c 0a20 2020 2020 2020  optional.       
-0000e1d0: 2043 686f 6c65 736b 7920 6465 636f 6d70   Cholesky decomp
-0000e1e0: 6f73 6974 696f 6e20 6f66 2061 6d6f 6e67  osition of among
-0000e1f0: 2d72 6f77 2063 6f76 6172 6961 6e63 6520  -row covariance 
-0000e200: 6d61 7472 6978 2e20 4578 6163 746c 7920  matrix. Exactly 
-0000e210: 6f6e 6520 6f66 0a20 2020 2020 2020 2072  one of.        r
-0000e220: 6f77 636f 7620 6f72 2072 6f77 6368 6f6c  owcov or rowchol
-0000e230: 2069 7320 6e65 6564 6564 2e0a 2020 2020   is needed..    
-0000e240: 636f 6c63 6f76 203a 2028 4e2c 204e 2920  colcov : (N, N) 
-0000e250: 7465 6e73 6f72 5f6c 696b 6520 6f66 2066  tensor_like of f
-0000e260: 6c6f 6174 2c20 6f70 7469 6f6e 616c 0a20  loat, optional. 
-0000e270: 2020 2020 2020 2041 6d6f 6e67 2d63 6f6c         Among-col
-0000e280: 756d 6e20 636f 7661 7269 616e 6365 206d  umn covariance m
-0000e290: 6174 7269 782e 2049 6620 726f 7763 6f76  atrix. If rowcov
-0000e2a0: 2069 7320 7468 6520 6964 656e 7469 7479   is the identity
-0000e2b0: 206d 6174 7269 782c 0a20 2020 2020 2020   matrix,.       
-0000e2c0: 2074 6869 7320 6675 6e63 7469 6f6e 7320   this functions 
-0000e2d0: 6173 2060 636f 7660 2069 6e20 4d76 4e6f  as `cov` in MvNo
-0000e2e0: 726d 616c 2e0a 2020 2020 2020 2020 4578  rmal..        Ex
-0000e2f0: 6163 746c 7920 6f6e 6520 6f66 2063 6f6c  actly one of col
-0000e300: 636f 7620 6f72 2063 6f6c 6368 6f6c 2069  cov or colchol i
-0000e310: 7320 6e65 6564 6564 2e0a 2020 2020 636f  s needed..    co
-0000e320: 6c63 686f 6c20 3a20 284e 2c20 4e29 2074  lchol : (N, N) t
-0000e330: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-0000e340: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
-0000e350: 2020 2020 2020 4368 6f6c 6573 6b79 2064        Cholesky d
-0000e360: 6563 6f6d 706f 7369 7469 6f6e 206f 6620  ecomposition of 
-0000e370: 616d 6f6e 672d 636f 6c75 6d6e 2063 6f76  among-column cov
-0000e380: 6172 6961 6e63 6520 6d61 7472 6978 2e20  ariance matrix. 
-0000e390: 4578 6163 746c 7920 6f6e 650a 2020 2020  Exactly one.    
-0000e3a0: 2020 2020 6f66 2063 6f6c 636f 7620 6f72      of colcov or
-0000e3b0: 2063 6f6c 6368 6f6c 2069 7320 6e65 6564   colchol is need
-0000e3c0: 6564 2e0a 0a20 2020 2045 7861 6d70 6c65  ed...    Example
-0000e3d0: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20  s.    --------. 
-0000e3e0: 2020 2044 6566 696e 6520 6120 6d61 7472     Define a matr
-0000e3f0: 6978 7661 7269 6174 6520 6e6f 726d 616c  ixvariate normal
-0000e400: 2076 6172 6961 626c 6520 666f 7220 6769   variable for gi
-0000e410: 7665 6e20 726f 7720 616e 6420 636f 6c75  ven row and colu
-0000e420: 6d6e 2063 6f76 6172 6961 6e63 650a 2020  mn covariance.  
-0000e430: 2020 6d61 7472 6963 6573 3a3a 0a0a 2020    matrices::..  
-0000e440: 2020 2020 2020 636f 6c63 6f76 203d 206e        colcov = n
-0000e450: 702e 6172 7261 7928 5b5b 312e 2c20 302e  p.array([[1., 0.
-0000e460: 355d 2c20 5b30 2e35 2c20 325d 5d29 0a20  5], [0.5, 2]]). 
-0000e470: 2020 2020 2020 2072 6f77 636f 7620 3d20         rowcov = 
-0000e480: 6e70 2e61 7272 6179 285b 5b31 2c20 302c  np.array([[1, 0,
-0000e490: 2030 5d2c 205b 302c 2034 2c20 305d 2c20   0], [0, 4, 0], 
-0000e4a0: 5b30 2c20 302c 2031 365d 5d29 0a20 2020  [0, 0, 16]]).   
-0000e4b0: 2020 2020 206d 203d 2072 6f77 636f 762e       m = rowcov.
-0000e4c0: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
-0000e4d0: 206e 203d 2063 6f6c 636f 762e 7368 6170   n = colcov.shap
-0000e4e0: 655b 305d 0a20 2020 2020 2020 206d 7520  e[0].        mu 
-0000e4f0: 3d20 6e70 2e7a 6572 6f73 2828 6d2c 206e  = np.zeros((m, n
-0000e500: 2929 0a20 2020 2020 2020 2076 616c 7320  )).        vals 
-0000e510: 3d20 706d 2e4d 6174 7269 784e 6f72 6d61  = pm.MatrixNorma
-0000e520: 6c28 2776 616c 7327 2c20 6d75 3d6d 752c  l('vals', mu=mu,
-0000e530: 2063 6f6c 636f 763d 636f 6c63 6f76 2c0a   colcov=colcov,.
-0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e550: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000e560: 6f77 636f 763d 726f 7763 6f76 290a 0a20  owcov=rowcov).. 
-0000e570: 2020 2041 626f 7665 2c20 7468 6520 6974     Above, the it
-0000e580: 6820 726f 7720 696e 2076 616c 7320 6861  h row in vals ha
-0000e590: 7320 6120 7661 7269 616e 6365 2074 6861  s a variance tha
-0000e5a0: 7420 6973 2073 6361 6c65 6420 6279 2034  t is scaled by 4
-0000e5b0: 5e69 2e0a 2020 2020 416c 7465 726e 6174  ^i..    Alternat
-0000e5c0: 6976 656c 792c 2072 6f77 206f 7220 636f  ively, row or co
-0000e5d0: 6c75 6d6e 2063 686f 6c65 736b 7920 6d61  lumn cholesky ma
-0000e5e0: 7472 6963 6573 2063 6f75 6c64 2062 6520  trices could be 
-0000e5f0: 7375 6273 7469 7475 7465 6420 666f 720a  substituted for.
-0000e600: 2020 2020 6569 7468 6572 2063 6f76 6172      either covar
-0000e610: 6961 6e63 6520 6d61 7472 6978 2e20 5468  iance matrix. Th
-0000e620: 6520 4d61 7472 6978 4e6f 726d 616c 2069  e MatrixNormal i
-0000e630: 7320 7175 6963 6b65 7220 7761 7920 636f  s quicker way co
-0000e640: 6d70 7574 650a 2020 2020 4d76 4e6f 726d  mpute.    MvNorm
-0000e650: 616c 286d 752c 206e 702e 6b72 6f6e 2872  al(mu, np.kron(r
-0000e660: 6f77 636f 762c 2063 6f6c 636f 7629 2920  owcov, colcov)) 
-0000e670: 7468 6174 2074 616b 6573 2061 6476 616e  that takes advan
-0000e680: 7461 6765 206f 6620 6b72 6f6e 6563 6b65  tage of kronecke
-0000e690: 7220 7072 6f64 7563 740a 2020 2020 7072  r product.    pr
-0000e6a0: 6f70 6572 7469 6573 2066 6f72 2069 6e76  operties for inv
-0000e6b0: 6572 7369 6f6e 2e20 466f 7220 6578 616d  ersion. For exam
-0000e6c0: 706c 652c 2069 6620 6472 6177 7320 6672  ple, if draws fr
-0000e6d0: 6f6d 204d 764e 6f72 6d61 6c20 6861 6420  om MvNormal had 
-0000e6e0: 7468 6520 7361 6d65 0a20 2020 2063 6f76  the same.    cov
-0000e6f0: 6172 6961 6e63 6520 7374 7275 6374 7572  ariance structur
-0000e700: 652c 2062 7574 2077 6572 6520 7363 616c  e, but were scal
-0000e710: 6564 2062 7920 6469 6666 6572 656e 7420  ed by different 
-0000e720: 706f 7765 7273 206f 6620 616e 2075 6e6b  powers of an unk
-0000e730: 6e6f 776e 0a20 2020 2063 6f6e 7374 616e  nown.    constan
-0000e740: 742c 2062 6f74 6820 7468 6520 636f 7661  t, both the cova
-0000e750: 7269 616e 6365 2061 6e64 2073 6361 6c69  riance and scali
-0000e760: 6e67 2063 6f75 6c64 2062 6520 6c65 6172  ng could be lear
-0000e770: 6e65 6420 6173 2066 6f6c 6c6f 7773 0a20  ned as follows. 
-0000e780: 2020 2028 7365 6520 7468 6520 646f 6373     (see the docs
-0000e790: 7472 696e 6720 6f66 2060 4c4b 4a43 686f  tring of `LKJCho
-0000e7a0: 6c65 736b 7943 6f76 6020 666f 7220 6d6f  leskyCov` for mo
-0000e7b0: 7265 2069 6e66 6f72 6d61 7469 6f6e 2061  re information a
-0000e7c0: 626f 7574 2074 6869 7329 0a0a 2020 2020  bout this)..    
-0000e7d0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-0000e7e0: 0a0a 2020 2020 2020 2020 2320 5365 7475  ..        # Setu
-0000e7f0: 7020 6461 7461 0a20 2020 2020 2020 2074  p data.        t
-0000e800: 7275 655f 636f 6c63 6f76 203d 206e 702e  rue_colcov = np.
-0000e810: 6172 7261 7928 5b5b 312e 302c 2030 2e35  array([[1.0, 0.5
-0000e820: 2c20 302e 315d 2c0a 2020 2020 2020 2020  , 0.1],.        
-0000e830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e840: 2020 2020 2020 2020 5b30 2e35 2c20 312e          [0.5, 1.
-0000e850: 302c 2030 2e32 5d2c 0a20 2020 2020 2020  0, 0.2],.       
-0000e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e870: 2020 2020 2020 2020 205b 302e 312c 2030           [0.1, 0
-0000e880: 2e32 2c20 312e 305d 5d29 0a20 2020 2020  .2, 1.0]]).     
-0000e890: 2020 206d 203d 2033 0a20 2020 2020 2020     m = 3.       
-0000e8a0: 206e 203d 2074 7275 655f 636f 6c63 6f76   n = true_colcov
-0000e8b0: 2e73 6861 7065 5b30 5d0a 2020 2020 2020  .shape[0].      
-0000e8c0: 2020 7472 7565 5f73 6361 6c65 203d 2033    true_scale = 3
-0000e8d0: 0a20 2020 2020 2020 2074 7275 655f 726f  .        true_ro
-0000e8e0: 7763 6f76 203d 206e 702e 6469 6167 285b  wcov = np.diag([
-0000e8f0: 7472 7565 5f73 6361 6c65 2a2a 2832 2a69  true_scale**(2*i
-0000e900: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
-0000e910: 286d 295d 290a 2020 2020 2020 2020 6d75  (m)]).        mu
-0000e920: 203d 206e 702e 7a65 726f 7328 286d 2c20   = np.zeros((m, 
-0000e930: 6e29 290a 2020 2020 2020 2020 7472 7565  n)).        true
-0000e940: 5f6b 726f 6e20 3d20 6e70 2e6b 726f 6e28  _kron = np.kron(
-0000e950: 7472 7565 5f72 6f77 636f 762c 2074 7275  true_rowcov, tru
-0000e960: 655f 636f 6c63 6f76 290a 2020 2020 2020  e_colcov).      
-0000e970: 2020 6461 7461 203d 206e 702e 7261 6e64    data = np.rand
-0000e980: 6f6d 2e6d 756c 7469 7661 7269 6174 655f  om.multivariate_
-0000e990: 6e6f 726d 616c 286d 752e 666c 6174 7465  normal(mu.flatte
-0000e9a0: 6e28 292c 2074 7275 655f 6b72 6f6e 290a  n(), true_kron).
-0000e9b0: 2020 2020 2020 2020 6461 7461 203d 2064          data = d
-0000e9c0: 6174 612e 7265 7368 6170 6528 6d2c 206e  ata.reshape(m, n
-0000e9d0: 290a 0a20 2020 2020 2020 2077 6974 6820  )..        with 
-0000e9e0: 706d 2e4d 6f64 656c 2829 2061 7320 6d6f  pm.Model() as mo
-0000e9f0: 6465 6c3a 0a20 2020 2020 2020 2020 2020  del:.           
-0000ea00: 2023 2053 6574 7570 2072 6967 6874 2063   # Setup right c
-0000ea10: 686f 6c65 736b 7920 6d61 7472 6978 0a20  holesky matrix. 
-0000ea20: 2020 2020 2020 2020 2020 2073 645f 6469             sd_di
-0000ea30: 7374 203d 2070 6d2e 4861 6c66 4361 7563  st = pm.HalfCauc
-0000ea40: 6879 2e64 6973 7428 6265 7461 3d32 2e35  hy.dist(beta=2.5
-0000ea50: 2c20 7368 6170 653d 3329 0a20 2020 2020  , shape=3).     
-0000ea60: 2020 2020 2020 2063 6f6c 6368 6f6c 5f70         colchol_p
-0000ea70: 6163 6b65 6420 3d20 706d 2e4c 4b4a 4368  acked = pm.LKJCh
-0000ea80: 6f6c 6573 6b79 436f 7628 2763 6f6c 6368  oleskyCov('colch
-0000ea90: 6f6c 7061 636b 6564 272c 206e 3d33 2c20  olpacked', n=3, 
-0000eaa0: 6574 613d 322c 0a20 2020 2020 2020 2020  eta=2,.         
-0000eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ead0: 2020 2020 2020 7364 5f64 6973 743d 7364        sd_dist=sd
-0000eae0: 5f64 6973 7429 0a20 2020 2020 2020 2020  _dist).         
-0000eaf0: 2020 2063 6f6c 6368 6f6c 203d 2070 6d2e     colchol = pm.
-0000eb00: 6578 7061 6e64 5f70 6163 6b65 645f 7472  expand_packed_tr
-0000eb10: 6961 6e67 756c 6172 2833 2c20 636f 6c63  iangular(3, colc
-0000eb20: 686f 6c5f 7061 636b 6564 290a 0a20 2020  hol_packed)..   
-0000eb30: 2020 2020 2020 2020 2023 2053 6574 7570           # Setup
-0000eb40: 206c 6566 7420 636f 7661 7269 616e 6365   left covariance
-0000eb50: 206d 6174 7269 780a 2020 2020 2020 2020   matrix.        
-0000eb60: 2020 2020 7363 616c 6520 3d20 706d 2e4c      scale = pm.L
-0000eb70: 6f67 4e6f 726d 616c 2827 7363 616c 6527  ogNormal('scale'
-0000eb80: 2c20 6d75 3d6e 702e 6c6f 6728 7472 7565  , mu=np.log(true
-0000eb90: 5f73 6361 6c65 292c 2073 6967 6d61 3d30  _scale), sigma=0
-0000eba0: 2e35 290a 2020 2020 2020 2020 2020 2020  .5).            
-0000ebb0: 726f 7763 6f76 203d 2070 742e 6469 6167  rowcov = pt.diag
-0000ebc0: 285b 7363 616c 652a 2a28 322a 6929 2066  ([scale**(2*i) f
-0000ebd0: 6f72 2069 2069 6e20 7261 6e67 6528 6d29  or i in range(m)
-0000ebe0: 5d29 0a0a 2020 2020 2020 2020 2020 2020  ])..            
-0000ebf0: 7661 6c73 203d 2070 6d2e 4d61 7472 6978  vals = pm.Matrix
-0000ec00: 4e6f 726d 616c 2827 7661 6c73 272c 206d  Normal('vals', m
-0000ec10: 753d 6d75 2c20 636f 6c63 686f 6c3d 636f  u=mu, colchol=co
-0000ec20: 6c63 686f 6c2c 2072 6f77 636f 763d 726f  lchol, rowcov=ro
-0000ec30: 7763 6f76 2c0a 2020 2020 2020 2020 2020  wcov,.          
-0000ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec50: 2020 2020 2020 2020 206f 6273 6572 7665           observe
-0000ec60: 643d 6461 7461 290a 2020 2020 2222 220a  d=data).    """.
-0000ec70: 2020 2020 7276 5f6f 7020 3d20 6d61 7472      rv_op = matr
-0000ec80: 6978 6e6f 726d 616c 0a0a 2020 2020 4063  ixnormal..    @c
-0000ec90: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-0000eca0: 6566 2064 6973 7428 0a20 2020 2020 2020  ef dist(.       
-0000ecb0: 2063 6c73 2c0a 2020 2020 2020 2020 6d75   cls,.        mu
-0000ecc0: 2c0a 2020 2020 2020 2020 726f 7763 6f76  ,.        rowcov
-0000ecd0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2072  =None,.        r
-0000ece0: 6f77 6368 6f6c 3d4e 6f6e 652c 0a20 2020  owchol=None,.   
-0000ecf0: 2020 2020 2063 6f6c 636f 763d 4e6f 6e65       colcov=None
-0000ed00: 2c0a 2020 2020 2020 2020 636f 6c63 686f  ,.        colcho
-0000ed10: 6c3d 4e6f 6e65 2c0a 2020 2020 2020 2020  l=None,.        
-0000ed20: 2a61 7267 732c 0a20 2020 2020 2020 202a  *args,.        *
-0000ed30: 2a6b 7761 7267 732c 0a20 2020 2029 3a0a  *kwargs,.    ):.
-0000ed40: 2020 2020 2020 2020 6368 6f6c 6573 6b79          cholesky
-0000ed50: 203d 2043 686f 6c65 736b 7928 6c6f 7765   = Cholesky(lowe
-0000ed60: 723d 5472 7565 2c20 6f6e 5f65 7272 6f72  r=True, on_error
-0000ed70: 3d22 7261 6973 6522 290a 0a20 2020 2020  ="raise")..     
-0000ed80: 2020 2023 2041 6d6f 6e67 2d72 6f77 206d     # Among-row m
-0000ed90: 6174 7269 6365 730a 2020 2020 2020 2020  atrices.        
-0000eda0: 6966 206c 656e 285b 6920 666f 7220 6920  if len([i for i 
-0000edb0: 696e 205b 726f 7763 6f76 2c20 726f 7763  in [rowcov, rowc
-0000edc0: 686f 6c5d 2069 6620 6920 6973 206e 6f74  hol] if i is not
-0000edd0: 204e 6f6e 655d 2920 213d 2031 3a0a 2020   None]) != 1:.  
-0000ede0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000edf0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
-0000ee00: 2020 2020 2020 2020 2020 2020 2249 6e63              "Inc
-0000ee10: 6f6d 7061 7469 626c 6520 7061 7261 6d65  ompatible parame
-0000ee20: 7465 7269 7a61 7469 6f6e 2e20 5370 6563  terization. Spec
-0000ee30: 6966 7920 6578 6163 746c 7920 6f6e 6520  ify exactly one 
-0000ee40: 6f66 2072 6f77 636f 762c 206f 7220 726f  of rowcov, or ro
-0000ee50: 7763 686f 6c2e 220a 2020 2020 2020 2020  wchol.".        
-0000ee60: 2020 2020 290a 2020 2020 2020 2020 6966      ).        if
-0000ee70: 2072 6f77 636f 7620 6973 206e 6f74 204e   rowcov is not N
-0000ee80: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000ee90: 2069 6620 726f 7763 6f76 2e6e 6469 6d20   if rowcov.ndim 
-0000eea0: 213d 2032 3a0a 2020 2020 2020 2020 2020  != 2:.          
-0000eeb0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000eec0: 6545 7272 6f72 2822 726f 7763 6f76 206d  eError("rowcov m
-0000eed0: 7573 7420 6265 2074 776f 2064 696d 656e  ust be two dimen
-0000eee0: 7369 6f6e 616c 2e22 290a 2020 2020 2020  sional.").      
-0000eef0: 2020 2020 2020 726f 7763 686f 6c5f 636f        rowchol_co
-0000ef00: 7620 3d20 6368 6f6c 6573 6b79 2872 6f77  v = cholesky(row
-0000ef10: 636f 7629 0a20 2020 2020 2020 2065 6c73  cov).        els
-0000ef20: 653a 0a20 2020 2020 2020 2020 2020 2069  e:.            i
-0000ef30: 6620 726f 7763 686f 6c2e 6e64 696d 2021  f rowchol.ndim !
-0000ef40: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-0000ef50: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000ef60: 4572 726f 7228 2272 6f77 6368 6f6c 206d  Error("rowchol m
-0000ef70: 7573 7420 6265 2074 776f 2064 696d 656e  ust be two dimen
-0000ef80: 7369 6f6e 616c 2e22 290a 2020 2020 2020  sional.").      
-0000ef90: 2020 2020 2020 726f 7763 686f 6c5f 636f        rowchol_co
-0000efa0: 7620 3d20 7074 2e61 735f 7465 6e73 6f72  v = pt.as_tensor
-0000efb0: 5f76 6172 6961 626c 6528 726f 7763 686f  _variable(rowcho
-0000efc0: 6c29 0a0a 2020 2020 2020 2020 2320 416d  l)..        # Am
-0000efd0: 6f6e 672d 636f 6c75 6d6e 206d 6174 7269  ong-column matri
-0000efe0: 6365 730a 2020 2020 2020 2020 6966 206c  ces.        if l
-0000eff0: 656e 285b 6920 666f 7220 6920 696e 205b  en([i for i in [
-0000f000: 636f 6c63 6f76 2c20 636f 6c63 686f 6c5d  colcov, colchol]
-0000f010: 2069 6620 6920 6973 206e 6f74 204e 6f6e   if i is not Non
-0000f020: 655d 2920 213d 2031 3a0a 2020 2020 2020  e]) != 1:.      
-0000f030: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-0000f040: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-0000f050: 2020 2020 2020 2020 2249 6e63 6f6d 7061          "Incompa
-0000f060: 7469 626c 6520 7061 7261 6d65 7465 7269  tible parameteri
-0000f070: 7a61 7469 6f6e 2e20 5370 6563 6966 7920  zation. Specify 
-0000f080: 6578 6163 746c 7920 6f6e 6520 6f66 2063  exactly one of c
-0000f090: 6f6c 636f 762c 206f 7220 636f 6c63 686f  olcov, or colcho
-0000f0a0: 6c2e 220a 2020 2020 2020 2020 2020 2020  l.".            
-0000f0b0: 290a 2020 2020 2020 2020 6966 2063 6f6c  ).        if col
-0000f0c0: 636f 7620 6973 206e 6f74 204e 6f6e 653a  cov is not None:
-0000f0d0: 0a20 2020 2020 2020 2020 2020 2063 6f6c  .            col
-0000f0e0: 636f 7620 3d20 7074 2e61 735f 7465 6e73  cov = pt.as_tens
-0000f0f0: 6f72 5f76 6172 6961 626c 6528 636f 6c63  or_variable(colc
-0000f100: 6f76 290a 2020 2020 2020 2020 2020 2020  ov).            
-0000f110: 6966 2063 6f6c 636f 762e 6e64 696d 2021  if colcov.ndim !
-0000f120: 3d20 323a 0a20 2020 2020 2020 2020 2020  = 2:.           
-0000f130: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000f140: 4572 726f 7228 2263 6f6c 636f 7620 6d75  Error("colcov mu
-0000f150: 7374 2062 6520 7477 6f20 6469 6d65 6e73  st be two dimens
-0000f160: 696f 6e61 6c2e 2229 0a20 2020 2020 2020  ional.").       
-0000f170: 2020 2020 2063 6f6c 6368 6f6c 5f63 6f76       colchol_cov
-0000f180: 203d 2063 686f 6c65 736b 7928 636f 6c63   = cholesky(colc
-0000f190: 6f76 290a 2020 2020 2020 2020 656c 7365  ov).        else
-0000f1a0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-0000f1b0: 2063 6f6c 6368 6f6c 2e6e 6469 6d20 213d   colchol.ndim !=
-0000f1c0: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-0000f1d0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-0000f1e0: 7272 6f72 2822 636f 6c63 686f 6c20 6d75  rror("colchol mu
-0000f1f0: 7374 2062 6520 7477 6f20 6469 6d65 6e73  st be two dimens
-0000f200: 696f 6e61 6c2e 2229 0a20 2020 2020 2020  ional.").       
-0000f210: 2020 2020 2063 6f6c 6368 6f6c 5f63 6f76       colchol_cov
-0000f220: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
-0000f230: 7661 7269 6162 6c65 2863 6f6c 6368 6f6c  variable(colchol
-0000f240: 290a 0a20 2020 2020 2020 2064 6973 745f  )..        dist_
-0000f250: 7368 6170 6520 3d20 2872 6f77 6368 6f6c  shape = (rowchol
-0000f260: 5f63 6f76 2e73 6861 7065 5b2d 315d 2c20  _cov.shape[-1], 
-0000f270: 636f 6c63 686f 6c5f 636f 762e 7368 6170  colchol_cov.shap
-0000f280: 655b 2d31 5d29 0a0a 2020 2020 2020 2020  e[-1])..        
-0000f290: 2320 4272 6f61 6463 6173 7469 6e67 206d  # Broadcasting m
-0000f2a0: 750a 2020 2020 2020 2020 6d75 203d 2070  u.        mu = p
-0000f2b0: 742e 6578 7472 615f 6f70 732e 6272 6f61  t.extra_ops.broa
-0000f2c0: 6463 6173 745f 746f 286d 752c 2073 6861  dcast_to(mu, sha
-0000f2d0: 7065 3d64 6973 745f 7368 6170 6529 0a20  pe=dist_shape). 
-0000f2e0: 2020 2020 2020 206d 7520 3d20 7074 2e61         mu = pt.a
-0000f2f0: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-0000f300: 6528 666c 6f61 7458 286d 7529 290a 0a20  e(floatX(mu)).. 
-0000f310: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-0000f320: 7065 7228 292e 6469 7374 285b 6d75 2c20  per().dist([mu, 
-0000f330: 726f 7763 686f 6c5f 636f 762c 2063 6f6c  rowchol_cov, col
-0000f340: 6368 6f6c 5f63 6f76 5d2c 202a 2a6b 7761  chol_cov], **kwa
-0000f350: 7267 7329 0a0a 2020 2020 6465 6620 6d6f  rgs)..    def mo
-0000f360: 6d65 6e74 2872 762c 2073 697a 652c 206d  ment(rv, size, m
-0000f370: 752c 2072 6f77 6368 6f6c 2c20 636f 6c63  u, rowchol, colc
-0000f380: 686f 6c29 3a0a 2020 2020 2020 2020 7265  hol):.        re
-0000f390: 7475 726e 2070 742e 6675 6c6c 5f6c 696b  turn pt.full_lik
-0000f3a0: 6528 7276 2c20 6d75 290a 0a20 2020 2064  e(rv, mu)..    d
-0000f3b0: 6566 206c 6f67 7028 7661 6c75 652c 206d  ef logp(value, m
-0000f3c0: 752c 2072 6f77 6368 6f6c 2c20 636f 6c63  u, rowchol, colc
-0000f3d0: 686f 6c29 3a0a 2020 2020 2020 2020 2222  hol):.        ""
-0000f3e0: 220a 2020 2020 2020 2020 4361 6c63 756c  ".        Calcul
-0000f3f0: 6174 6520 6c6f 672d 7072 6f62 6162 696c  ate log-probabil
-0000f400: 6974 7920 6f66 204d 6174 7269 782d 7661  ity of Matrix-va
-0000f410: 6c75 6564 204e 6f72 6d61 6c20 6469 7374  lued Normal dist
-0000f420: 7269 6275 7469 6f6e 0a20 2020 2020 2020  ribution.       
-0000f430: 2061 7420 7370 6563 6966 6965 6420 7661   at specified va
-0000f440: 6c75 652e 0a0a 2020 2020 2020 2020 5061  lue...        Pa
-0000f450: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-0000f460: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-0000f470: 2020 2020 7661 6c75 653a 206e 756d 6572      value: numer
-0000f480: 6963 0a20 2020 2020 2020 2020 2020 2056  ic.            V
-0000f490: 616c 7565 2066 6f72 2077 6869 6368 206c  alue for which l
-0000f4a0: 6f67 2d70 726f 6261 6269 6c69 7479 2069  og-probability i
-0000f4b0: 7320 6361 6c63 756c 6174 6564 2e0a 0a20  s calculated... 
-0000f4c0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-0000f4d0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-0000f4e0: 2020 2020 2020 2054 656e 736f 7256 6172         TensorVar
-0000f4f0: 6961 626c 650a 2020 2020 2020 2020 2222  iable.        ""
-0000f500: 220a 0a20 2020 2020 2020 2069 6620 7661  "..        if va
-0000f510: 6c75 652e 6e64 696d 2021 3d20 323a 0a20  lue.ndim != 2:. 
-0000f520: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000f530: 2056 616c 7565 4572 726f 7228 2256 616c   ValueError("Val
-0000f540: 7565 206d 7573 7420 6265 2074 776f 2064  ue must be two d
-0000f550: 696d 656e 7369 6f6e 616c 2e22 290a 0a20  imensional.").. 
-0000f560: 2020 2020 2020 2023 2043 6f6d 7075 7465         # Compute
-0000f570: 2054 725b 636f 6c63 6f76 5e2d 3120 4020   Tr[colcov^-1 @ 
-0000f580: 2878 202d 206d 7529 2e54 2040 2072 6f77  (x - mu).T @ row
-0000f590: 636f 765e 2d31 2040 2028 7820 2d20 6d75  cov^-1 @ (x - mu
-0000f5a0: 295d 2061 6e64 0a20 2020 2020 2020 2023  )] and.        #
-0000f5b0: 2074 6865 206c 6f67 6465 7420 6f66 2063   the logdet of c
-0000f5c0: 6f6c 636f 7620 616e 6420 726f 7763 6f76  olcov and rowcov
-0000f5d0: 2e0a 2020 2020 2020 2020 6465 6c74 6120  ..        delta 
-0000f5e0: 3d20 7661 6c75 6520 2d20 6d75 0a0a 2020  = value - mu..  
-0000f5f0: 2020 2020 2020 2320 4669 6e64 2065 7870        # Find exp
-0000f600: 6f6e 656e 7420 7069 6563 6520 6279 2070  onent piece by p
-0000f610: 6965 6365 0a20 2020 2020 2020 2072 6967  iece.        rig
-0000f620: 6874 5f71 7561 6464 6973 7420 3d20 736f  ht_quaddist = so
-0000f630: 6c76 655f 6c6f 7765 7228 726f 7763 686f  lve_lower(rowcho
-0000f640: 6c2c 2064 656c 7461 290a 2020 2020 2020  l, delta).      
-0000f650: 2020 7175 6164 6469 7374 203d 2070 742e    quaddist = pt.
-0000f660: 6e6c 696e 616c 672e 6d61 7472 6978 5f64  nlinalg.matrix_d
-0000f670: 6f74 2872 6967 6874 5f71 7561 6464 6973  ot(right_quaddis
-0000f680: 742e 542c 2072 6967 6874 5f71 7561 6464  t.T, right_quadd
-0000f690: 6973 7429 0a20 2020 2020 2020 2071 7561  ist).        qua
-0000f6a0: 6464 6973 7420 3d20 736f 6c76 655f 6c6f  ddist = solve_lo
-0000f6b0: 7765 7228 636f 6c63 686f 6c2c 2071 7561  wer(colchol, qua
-0000f6c0: 6464 6973 7429 0a20 2020 2020 2020 2071  ddist).        q
-0000f6d0: 7561 6464 6973 7420 3d20 736f 6c76 655f  uaddist = solve_
-0000f6e0: 7570 7065 7228 636f 6c63 686f 6c2e 542c  upper(colchol.T,
-0000f6f0: 2071 7561 6464 6973 7429 0a20 2020 2020   quaddist).     
-0000f700: 2020 2074 7271 7561 6464 6973 7420 3d20     trquaddist = 
-0000f710: 7074 2e6e 6c69 6e61 6c67 2e74 7261 6365  pt.nlinalg.trace
-0000f720: 2871 7561 6464 6973 7429 0a0a 2020 2020  (quaddist)..    
-0000f730: 2020 2020 636f 6c64 6961 6720 3d20 7074      coldiag = pt
-0000f740: 2e64 6961 6728 636f 6c63 686f 6c29 0a20  .diag(colchol). 
-0000f750: 2020 2020 2020 2072 6f77 6469 6167 203d         rowdiag =
-0000f760: 2070 742e 6469 6167 2872 6f77 6368 6f6c   pt.diag(rowchol
-0000f770: 290a 2020 2020 2020 2020 6861 6c66 5f63  ).        half_c
-0000f780: 6f6c 6c6f 6764 6574 203d 2070 742e 7375  ollogdet = pt.su
-0000f790: 6d28 7074 2e6c 6f67 2863 6f6c 6469 6167  m(pt.log(coldiag
-0000f7a0: 2929 2020 2320 6c6f 6764 6574 284d 2920  ))  # logdet(M) 
-0000f7b0: 3d20 322a 5472 286c 6f67 284c 2929 0a20  = 2*Tr(log(L)). 
-0000f7c0: 2020 2020 2020 2068 616c 665f 726f 776c         half_rowl
-0000f7d0: 6f67 6465 7420 3d20 7074 2e73 756d 2870  ogdet = pt.sum(p
-0000f7e0: 742e 6c6f 6728 726f 7764 6961 6729 2920  t.log(rowdiag)) 
-0000f7f0: 2023 2055 7369 6e67 2043 686f 6c65 736b   # Using Cholesk
-0000f800: 793a 204d 203d 204c 204c 5e54 0a0a 2020  y: M = L L^T..  
-0000f810: 2020 2020 2020 6d20 3d20 726f 7763 686f        m = rowcho
-0000f820: 6c2e 7368 6170 655b 305d 0a20 2020 2020  l.shape[0].     
-0000f830: 2020 206e 203d 2063 6f6c 6368 6f6c 2e73     n = colchol.s
-0000f840: 6861 7065 5b30 5d0a 0a20 2020 2020 2020  hape[0]..       
-0000f850: 206e 6f72 6d20 3d20 2d30 2e35 202a 206d   norm = -0.5 * m
-0000f860: 202a 206e 202a 2070 6d2e 666c 6f61 7458   * n * pm.floatX
-0000f870: 286e 702e 6c6f 6728 3220 2a20 6e70 2e70  (np.log(2 * np.p
-0000f880: 6929 290a 2020 2020 2020 2020 7265 7475  i)).        retu
-0000f890: 726e 206e 6f72 6d20 2d20 302e 3520 2a20  rn norm - 0.5 * 
-0000f8a0: 7472 7175 6164 6469 7374 202d 206d 202a  trquaddist - m *
-0000f8b0: 2068 616c 665f 636f 6c6c 6f67 6465 7420   half_collogdet 
-0000f8c0: 2d20 6e20 2a20 6861 6c66 5f72 6f77 6c6f  - n * half_rowlo
-0000f8d0: 6764 6574 0a0a 0a63 6c61 7373 204b 726f  gdet...class Kro
-0000f8e0: 6e65 636b 6572 4e6f 726d 616c 5256 2852  neckerNormalRV(R
-0000f8f0: 616e 646f 6d56 6172 6961 626c 6529 3a0a  andomVariable):.
-0000f900: 2020 2020 6e61 6d65 203d 2022 6b72 6f6e      name = "kron
-0000f910: 6563 6b65 726e 6f72 6d61 6c22 0a20 2020  eckernormal".   
-0000f920: 206e 6469 6d5f 7375 7070 203d 2031 0a20   ndim_supp = 1. 
-0000f930: 2020 206e 6469 6d73 5f70 6172 616d 7320     ndims_params 
-0000f940: 3d20 5b31 2c20 302c 2032 5d0a 2020 2020  = [1, 0, 2].    
-0000f950: 6474 7970 6520 3d20 2266 6c6f 6174 5822  dtype = "floatX"
-0000f960: 0a20 2020 205f 7072 696e 745f 6e61 6d65  .    _print_name
-0000f970: 203d 2028 224b 726f 6e65 636b 6572 4e6f   = ("KroneckerNo
-0000f980: 726d 616c 222c 2022 5c5c 6f70 6572 6174  rmal", "\\operat
-0000f990: 6f72 6e61 6d65 7b4b 726f 6e65 636b 6572  orname{Kronecker
-0000f9a0: 4e6f 726d 616c 7d22 290a 0a20 2020 2064  Normal}")..    d
-0000f9b0: 6566 2072 6e67 5f66 6e28 7365 6c66 2c20  ef rng_fn(self, 
-0000f9c0: 726e 672c 206d 752c 2073 6967 6d61 2c20  rng, mu, sigma, 
-0000f9d0: 2a63 6f76 732c 2073 697a 653d 4e6f 6e65  *covs, size=None
-0000f9e0: 293a 0a20 2020 2020 2020 2073 697a 6520  ):.        size 
-0000f9f0: 3d20 7369 7a65 2069 6620 7369 7a65 2065  = size if size e
-0000fa00: 6c73 6520 636f 7673 5b2d 315d 0a20 2020  lse covs[-1].   
-0000fa10: 2020 2020 2063 6f76 7320 3d20 636f 7673       covs = covs
-0000fa20: 5b3a 2d31 5d20 6966 2063 6f76 735b 2d31  [:-1] if covs[-1
-0000fa30: 5d20 3d3d 2073 697a 6520 656c 7365 2063  ] == size else c
-0000fa40: 6f76 730a 0a20 2020 2020 2020 2063 6f76  ovs..        cov
-0000fa50: 203d 2072 6564 7563 6528 6c69 6e61 6c67   = reduce(linalg
-0000fa60: 2e6b 726f 6e2c 2063 6f76 7329 0a0a 2020  .kron, covs)..  
-0000fa70: 2020 2020 2020 6966 2073 6967 6d61 3a0a        if sigma:.
-0000fa80: 2020 2020 2020 2020 2020 2020 636f 7620              cov 
-0000fa90: 3d20 636f 7620 2b20 7369 676d 612a 2a32  = cov + sigma**2
-0000faa0: 202a 206e 702e 6579 6528 636f 762e 7368   * np.eye(cov.sh
-0000fab0: 6170 655b 305d 290a 0a20 2020 2020 2020  ape[0])..       
-0000fac0: 2078 203d 206d 756c 7469 7661 7269 6174   x = multivariat
-0000fad0: 655f 6e6f 726d 616c 2e72 6e67 5f66 6e28  e_normal.rng_fn(
-0000fae0: 726e 673d 726e 672c 206d 6561 6e3d 6d75  rng=rng, mean=mu
-0000faf0: 2c20 636f 763d 636f 762c 2073 697a 653d  , cov=cov, size=
-0000fb00: 7369 7a65 290a 2020 2020 2020 2020 7265  size).        re
-0000fb10: 7475 726e 2078 0a0a 0a6b 726f 6e65 636b  turn x...kroneck
-0000fb20: 6572 6e6f 726d 616c 203d 204b 726f 6e65  ernormal = Krone
-0000fb30: 636b 6572 4e6f 726d 616c 5256 2829 0a0a  ckerNormalRV()..
-0000fb40: 0a63 6c61 7373 204b 726f 6e65 636b 6572  .class Kronecker
-0000fb50: 4e6f 726d 616c 2843 6f6e 7469 6e75 6f75  Normal(Continuou
-0000fb60: 7329 3a0a 2020 2020 7222 2222 0a20 2020  s):.    r""".   
-0000fb70: 204d 756c 7469 7661 7269 6174 6520 6e6f   Multivariate no
-0000fb80: 726d 616c 206c 6f67 2d6c 696b 656c 6968  rmal log-likelih
-0000fb90: 6f6f 6420 7769 7468 204b 726f 6e65 636b  ood with Kroneck
-0000fba0: 6572 2d73 7472 7563 7475 7265 6420 636f  er-structured co
-0000fbb0: 7661 7269 616e 6365 2e0a 0a20 2020 202e  variance...    .
-0000fbc0: 2e20 6d61 7468 3a3a 0a0a 2020 2020 2020  . math::..      
-0000fbd0: 2066 2878 205c 6d69 6420 5c6d 752c 204b   f(x \mid \mu, K
-0000fbe0: 2920 3d0a 2020 2020 2020 2020 2020 205c  ) =.           \
-0000fbf0: 6672 6163 7b31 7d7b 2832 5c70 6920 7c4b  frac{1}{(2\pi |K
-0000fc00: 7c29 5e7b 312f 327d 7d0a 2020 2020 2020  |)^{1/2}}.      
-0000fc10: 2020 2020 205c 6578 705c 6c65 6674 5c7b       \exp\left\{
-0000fc20: 202d 5c66 7261 637b 317d 7b32 7d20 2878   -\frac{1}{2} (x
-0000fc30: 2d5c 6d75 295e 7b5c 7072 696d 657d 204b  -\mu)^{\prime} K
-0000fc40: 5e7b 2d31 7d20 2878 2d5c 6d75 2920 5c72  ^{-1} (x-\mu) \r
-0000fc50: 6967 6874 5c7d 0a0a 2020 2020 3d3d 3d3d  ight\}..    ====
-0000fc60: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
-0000fc70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fc80: 0a20 2020 2053 7570 706f 7274 2020 203a  .    Support   :
-0000fc90: 6d61 7468 3a60 7820 5c69 6e20 5c6d 6174  math:`x \in \mat
-0000fca0: 6862 627b 527d 5e4e 600a 2020 2020 4d65  hbb{R}^N`.    Me
-0000fcb0: 616e 2020 2020 2020 3a6d 6174 683a 605c  an      :math:`\
-0000fcc0: 6d75 600a 2020 2020 5661 7269 616e 6365  mu`.    Variance
-0000fcd0: 2020 3a6d 6174 683a 604b 203d 205c 6269    :math:`K = \bi
-0000fce0: 676f 7469 6d65 7320 4b5f 6920 2b20 5c73  gotimes K_i + \s
-0000fcf0: 6967 6d61 5e32 2049 5f4e 600a 2020 2020  igma^2 I_N`.    
-0000fd00: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-0000fd10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0000fd20: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
-0000fd30: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-0000fd40: 2d2d 2d0a 2020 2020 6d75 203a 2074 656e  ---.    mu : ten
-0000fd50: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
-0000fd60: 740a 2020 2020 2020 2020 5665 6374 6f72  t.        Vector
-0000fd70: 206f 6620 6d65 616e 732c 206a 7573 7420   of means, just 
-0000fd80: 6173 2069 6e20 604d 764e 6f72 6d61 6c60  as in `MvNormal`
-0000fd90: 2e0a 2020 2020 636f 7673 203a 206c 6973  ..    covs : lis
-0000fda0: 7420 6f66 2061 7272 6179 730a 2020 2020  t of arrays.    
-0000fdb0: 2020 2020 5468 6520 7365 7420 6f66 2063      The set of c
-0000fdc0: 6f76 6172 6961 6e63 6520 6d61 7472 6963  ovariance matric
-0000fdd0: 6573 203a 6d61 7468 3a60 5b4b 5f31 2c20  es :math:`[K_1, 
-0000fde0: 4b5f 322c 202e 2e2e 5d60 2074 6f20 6265  K_2, ...]` to be
-0000fdf0: 0a20 2020 2020 2020 204b 726f 6e65 636b  .        Kroneck
-0000fe00: 6572 6564 2069 6e20 7468 6520 6f72 6465  ered in the orde
-0000fe10: 7220 7072 6f76 6964 6564 203a 6d61 7468  r provided :math
-0000fe20: 3a60 5c62 6967 6f74 696d 6573 204b 5f69  :`\bigotimes K_i
-0000fe30: 602e 0a20 2020 2063 686f 6c73 203a 206c  `..    chols : l
-0000fe40: 6973 7420 6f66 2061 7272 6179 730a 2020  ist of arrays.  
-0000fe50: 2020 2020 2020 5468 6520 7365 7420 6f66        The set of
-0000fe60: 206c 6f77 6572 2063 686f 6c65 736b 7920   lower cholesky 
-0000fe70: 6d61 7472 6963 6573 203a 6d61 7468 3a60  matrices :math:`
-0000fe80: 5b4c 5f31 2c20 4c5f 322c 202e 2e2e 5d60  [L_1, L_2, ...]`
-0000fe90: 2073 7563 6820 7468 6174 0a20 2020 2020   such that.     
-0000fea0: 2020 203a 6d61 7468 3a60 4b5f 6920 3d20     :math:`K_i = 
-0000feb0: 4c5f 6920 4c5f 6927 602e 0a20 2020 2065  L_i L_i'`..    e
-0000fec0: 7664 7320 3a20 6c69 7374 206f 6620 7475  vds : list of tu
-0000fed0: 706c 6573 0a20 2020 2020 2020 2054 6865  ples.        The
-0000fee0: 2073 6574 206f 6620 6569 6765 6e76 616c   set of eigenval
-0000fef0: 7565 2d76 6563 746f 722c 2065 6967 656e  ue-vector, eigen
-0000ff00: 7665 6374 6f72 2d6d 6174 7269 7820 7061  vector-matrix pa
-0000ff10: 6972 730a 2020 2020 2020 2020 3a6d 6174  irs.        :mat
-0000ff20: 683a 605b 2876 5f31 2c20 515f 3129 2c20  h:`[(v_1, Q_1), 
-0000ff30: 2876 5f32 2c20 515f 3229 2c20 2e2e 2e5d  (v_2, Q_2), ...]
-0000ff40: 6020 7375 6368 2074 6861 740a 2020 2020  ` such that.    
-0000ff50: 2020 2020 3a6d 6174 683a 604b 5f69 203d      :math:`K_i =
-0000ff60: 2051 5f69 205c 7465 7874 7b64 6961 677d   Q_i \text{diag}
-0000ff70: 2876 5f69 2920 515f 6927 602e 2046 6f72  (v_i) Q_i'`. For
-0000ff80: 2065 7861 6d70 6c65 3a3a 0a0a 2020 2020   example::..    
-0000ff90: 2020 2020 2020 2020 765f 692c 2051 5f69          v_i, Q_i
-0000ffa0: 203d 2070 742e 6e6c 696e 616c 672e 6569   = pt.nlinalg.ei
-0000ffb0: 6768 284b 5f69 290a 2020 2020 7369 676d  gh(K_i).    sigm
-0000ffc0: 6120 3a20 7363 616c 6172 2c20 6f70 7469  a : scalar, opti
-0000ffd0: 6f6e 616c 0a20 2020 2020 2020 2053 7461  onal.        Sta
-0000ffe0: 6e64 6172 6420 6465 7669 6174 696f 6e20  ndard deviation 
-0000fff0: 6f66 2074 6865 2047 6175 7373 6961 6e20  of the Gaussian 
-00010000: 7768 6974 6520 6e6f 6973 652e 0a0a 2020  white noise...  
-00010010: 2020 4578 616d 706c 6573 0a20 2020 202d    Examples.    -
-00010020: 2d2d 2d2d 2d2d 2d0a 2020 2020 4465 6669  -------.    Defi
-00010030: 6e65 2061 206d 756c 7469 7661 7269 6174  ne a multivariat
-00010040: 6520 6e6f 726d 616c 2076 6172 6961 626c  e normal variabl
-00010050: 6520 7769 7468 2061 2063 6f76 6172 6961  e with a covaria
-00010060: 6e63 650a 2020 2020 3a6d 6174 683a 604b  nce.    :math:`K
-00010070: 203d 204b 5f31 205c 6f74 696d 6573 204b   = K_1 \otimes K
-00010080: 5f32 600a 0a20 2020 202e 2e20 636f 6465  _2`..    .. code
-00010090: 3a3a 2070 7974 686f 6e0a 0a20 2020 2020  :: python..     
-000100a0: 2020 204b 3120 3d20 6e70 2e61 7272 6179     K1 = np.array
-000100b0: 285b 5b31 2e2c 2030 2e35 5d2c 205b 302e  ([[1., 0.5], [0.
-000100c0: 352c 2032 5d5d 290a 2020 2020 2020 2020  5, 2]]).        
-000100d0: 4b32 203d 206e 702e 6172 7261 7928 5b5b  K2 = np.array([[
-000100e0: 312e 2c20 302e 342c 2030 2e32 5d2c 205b  1., 0.4, 0.2], [
-000100f0: 302e 342c 2032 2c20 302e 335d 2c20 5b30  0.4, 2, 0.3], [0
-00010100: 2e32 2c20 302e 332c 2031 5d5d 290a 2020  .2, 0.3, 1]]).  
-00010110: 2020 2020 2020 636f 7673 203d 205b 4b31        covs = [K1
-00010120: 2c20 4b32 5d0a 2020 2020 2020 2020 4e20  , K2].        N 
-00010130: 3d20 360a 2020 2020 2020 2020 6d75 203d  = 6.        mu =
-00010140: 206e 702e 7a65 726f 7328 4e29 0a20 2020   np.zeros(N).   
-00010150: 2020 2020 2077 6974 6820 706d 2e4d 6f64       with pm.Mod
-00010160: 656c 2829 2061 7320 6d6f 6465 6c3a 0a20  el() as model:. 
-00010170: 2020 2020 2020 2020 2020 2076 616c 7320             vals 
-00010180: 3d20 706d 2e4b 726f 6e65 636b 6572 4e6f  = pm.KroneckerNo
-00010190: 726d 616c 2827 7661 6c73 272c 206d 753d  rmal('vals', mu=
-000101a0: 6d75 2c20 636f 7673 3d63 6f76 732c 2073  mu, covs=covs, s
-000101b0: 6861 7065 3d4e 290a 0a20 2020 2045 6666  hape=N)..    Eff
-000101c0: 6963 6965 6e63 7920 6761 696e 7320 6172  iciency gains ar
-000101d0: 6520 6d61 6465 2062 7920 6368 6f6c 6573  e made by choles
-000101e0: 6b79 2064 6563 6f6d 706f 7369 6e67 203a  ky decomposing :
-000101f0: 6d61 7468 3a60 4b5f 3160 2061 6e64 0a20  math:`K_1` and. 
-00010200: 2020 203a 6d61 7468 3a60 4b5f 3260 2069     :math:`K_2` i
-00010210: 6e64 6976 6964 7561 6c6c 7920 7261 7468  ndividually rath
-00010220: 6572 2074 6861 6e20 7468 6520 6c61 7267  er than the larg
-00010230: 6572 203a 6d61 7468 3a60 4b60 206d 6174  er :math:`K` mat
-00010240: 7269 782e 2041 6c74 686f 7567 680a 2020  rix. Although.  
-00010250: 2020 6f6e 6c79 2074 776f 206d 6174 7269    only two matri
-00010260: 6365 7320 3a6d 6174 683a 604b 5f31 6020  ces :math:`K_1` 
-00010270: 616e 6420 3a6d 6174 683a 604b 5f32 6020  and :math:`K_2` 
-00010280: 6172 6520 7368 6f77 6e20 6865 7265 2c20  are shown here, 
-00010290: 616e 2061 7262 6974 7261 7279 0a20 2020  an arbitrary.   
-000102a0: 206e 756d 6265 7220 6f66 2073 7562 6d61   number of subma
-000102b0: 7472 6963 6573 2063 616e 2062 6520 636f  trices can be co
-000102c0: 6d62 696e 6564 2069 6e20 7468 6973 2077  mbined in this w
-000102d0: 6179 2e20 4368 6f6c 6573 6b79 7320 616e  ay. Choleskys an
-000102e0: 640a 2020 2020 6569 6765 6e64 6563 6f6d  d.    eigendecom
-000102f0: 706f 7369 7469 6f6e 7320 6361 6e20 6265  positions can be
-00010300: 2070 726f 7669 6465 6420 696e 7374 6561   provided instea
-00010310: 640a 0a20 2020 202e 2e20 636f 6465 3a3a  d..    .. code::
-00010320: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
-00010330: 2063 686f 6c73 203d 205b 6e70 2e6c 696e   chols = [np.lin
-00010340: 616c 672e 6368 6f6c 6573 6b79 284b 6929  alg.cholesky(Ki)
-00010350: 2066 6f72 204b 6920 696e 2063 6f76 735d   for Ki in covs]
-00010360: 0a20 2020 2020 2020 2065 7664 7320 3d20  .        evds = 
-00010370: 5b6e 702e 6c69 6e61 6c67 2e65 6967 6828  [np.linalg.eigh(
-00010380: 4b69 2920 666f 7220 4b69 2069 6e20 636f  Ki) for Ki in co
-00010390: 7673 5d0a 2020 2020 2020 2020 7769 7468  vs].        with
-000103a0: 2070 6d2e 4d6f 6465 6c28 2920 6173 206d   pm.Model() as m
-000103b0: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
-000103c0: 2020 7661 6c73 3220 3d20 706d 2e4b 726f    vals2 = pm.Kro
-000103d0: 6e65 636b 6572 4e6f 726d 616c 2827 7661  neckerNormal('va
-000103e0: 6c73 3227 2c20 6d75 3d6d 752c 2063 686f  ls2', mu=mu, cho
-000103f0: 6c73 3d63 686f 6c73 2c20 7368 6170 653d  ls=chols, shape=
-00010400: 4e29 0a20 2020 2020 2020 2020 2020 2023  N).            #
-00010410: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
-00010420: 7661 6c73 3320 3d20 706d 2e4b 726f 6e65  vals3 = pm.Krone
-00010430: 636b 6572 4e6f 726d 616c 2827 7661 6c73  ckerNormal('vals
-00010440: 3327 2c20 6d75 3d6d 752c 2065 7664 733d  3', mu=mu, evds=
-00010450: 6576 6473 2c20 7368 6170 653d 4e29 0a0a  evds, shape=N)..
-00010460: 2020 2020 6e65 6974 6865 7220 6f66 2077      neither of w
-00010470: 6869 6368 2077 696c 6c20 6265 2063 6f6e  hich will be con
-00010480: 7665 7274 6564 2e20 4469 6167 6f6e 616c  verted. Diagonal
-00010490: 206e 6f69 7365 2063 616e 2061 6c73 6f20   noise can also 
-000104a0: 6265 2061 6464 6564 2074 6f0a 2020 2020  be added to.    
-000104b0: 7468 6520 636f 7661 7269 616e 6365 206d  the covariance m
-000104c0: 6174 7269 782c 203a 6d61 7468 3a60 4b20  atrix, :math:`K 
-000104d0: 3d20 4b5f 3120 5c6f 7469 6d65 7320 4b5f  = K_1 \otimes K_
-000104e0: 3220 2b20 5c73 6967 6d61 5e32 2049 5f4e  2 + \sigma^2 I_N
-000104f0: 602e 0a20 2020 2044 6573 7069 7465 2074  `..    Despite t
-00010500: 6865 206e 6f69 7365 2072 656d 6f76 696e  he noise removin
-00010510: 6720 7468 6520 6f76 6572 616c 6c20 4b72  g the overall Kr
-00010520: 6f6e 6563 6b65 7220 7374 7275 6374 7572  onecker structur
-00010530: 6520 6f66 2074 6865 206d 6174 7269 782c  e of the matrix,
-00010540: 0a20 2020 2060 4b72 6f6e 6563 6b65 724e  .    `KroneckerN
-00010550: 6f72 6d61 6c60 2063 616e 2063 6f6e 7469  ormal` can conti
-00010560: 6e75 6520 746f 206d 616b 6520 6566 6669  nue to make effi
-00010570: 6369 656e 7420 6361 6c63 756c 6174 696f  cient calculatio
-00010580: 6e73 2062 790a 2020 2020 7574 696c 697a  ns by.    utiliz
-00010590: 696e 6720 6569 6765 6e64 6563 6f6d 706f  ing eigendecompo
-000105a0: 7369 746f 6e73 206f 6620 7468 6520 7375  sitons of the su
-000105b0: 626d 6174 7269 6365 7320 6265 6869 6e64  bmatrices behind
-000105c0: 2074 6865 2073 6365 6e65 7320 5b31 5d2e   the scenes [1].
-000105d0: 0a20 2020 2054 6875 732c 0a0a 2020 2020  .    Thus,..    
-000105e0: 2e2e 2063 6f64 653a 3a20 7079 7468 6f6e  .. code:: python
-000105f0: 0a0a 2020 2020 2020 2020 7369 676d 6120  ..        sigma 
-00010600: 3d20 302e 310a 2020 2020 2020 2020 7769  = 0.1.        wi
-00010610: 7468 2070 6d2e 4d6f 6465 6c28 2920 6173  th pm.Model() as
-00010620: 206e 6f69 7365 5f6d 6f64 656c 3a0a 2020   noise_model:.  
-00010630: 2020 2020 2020 2020 2020 7661 6c73 203d            vals =
-00010640: 2070 6d2e 4b72 6f6e 6563 6b65 724e 6f72   pm.KroneckerNor
-00010650: 6d61 6c28 2776 616c 7327 2c20 6d75 3d6d  mal('vals', mu=m
-00010660: 752c 2063 6f76 733d 636f 7673 2c20 7369  u, covs=covs, si
-00010670: 676d 613d 7369 676d 612c 2073 6861 7065  gma=sigma, shape
-00010680: 3d4e 290a 2020 2020 2020 2020 2020 2020  =N).            
-00010690: 7661 6c73 3220 3d20 706d 2e4b 726f 6e65  vals2 = pm.Krone
-000106a0: 636b 6572 4e6f 726d 616c 2827 7661 6c73  ckerNormal('vals
-000106b0: 3227 2c20 6d75 3d6d 752c 2063 686f 6c73  2', mu=mu, chols
-000106c0: 3d63 686f 6c73 2c20 7369 676d 613d 7369  =chols, sigma=si
-000106d0: 676d 612c 2073 6861 7065 3d4e 290a 2020  gma, shape=N).  
-000106e0: 2020 2020 2020 2020 2020 7661 6c73 3320            vals3 
-000106f0: 3d20 706d 2e4b 726f 6e65 636b 6572 4e6f  = pm.KroneckerNo
-00010700: 726d 616c 2827 7661 6c73 3327 2c20 6d75  rmal('vals3', mu
-00010710: 3d6d 752c 2065 7664 733d 6576 6473 2c20  =mu, evds=evds, 
-00010720: 7369 676d 613d 7369 676d 612c 2073 6861  sigma=sigma, sha
-00010730: 7065 3d4e 290a 0a20 2020 2061 7265 2069  pe=N)..    are i
-00010740: 6465 6e74 6963 616c 2c20 7769 7468 2060  dentical, with `
-00010750: 636f 7673 6020 616e 6420 6063 686f 6c73  covs` and `chols
-00010760: 6020 6561 6368 2063 6f6e 7665 7274 6564  ` each converted
-00010770: 2074 6f0a 2020 2020 6569 6765 6e64 6563   to.    eigendec
-00010780: 6f6d 706f 7369 7469 6f6e 732e 0a0a 2020  ompositions...  
-00010790: 2020 5265 6665 7265 6e63 6573 0a20 2020    References.   
-000107a0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000107b0: 2e2e 205b 315d 2053 6161 7463 6869 2c20  .. [1] Saatchi, 
-000107c0: 592e 2028 3230 3131 292e 2022 5363 616c  Y. (2011). "Scal
-000107d0: 6162 6c65 2069 6e66 6572 656e 6365 2066  able inference f
-000107e0: 6f72 2073 7472 7563 7475 7265 6420 4761  or structured Ga
-000107f0: 7573 7369 616e 2070 726f 6365 7373 206d  ussian process m
-00010800: 6f64 656c 7322 0a20 2020 2022 2222 0a20  odels".    """. 
-00010810: 2020 2072 765f 6f70 203d 206b 726f 6e65     rv_op = krone
-00010820: 636b 6572 6e6f 726d 616c 0a0a 2020 2020  ckernormal..    
-00010830: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00010840: 2064 6566 2064 6973 7428 636c 732c 206d   def dist(cls, m
-00010850: 752c 2063 6f76 733d 4e6f 6e65 2c20 6368  u, covs=None, ch
-00010860: 6f6c 733d 4e6f 6e65 2c20 6576 6473 3d4e  ols=None, evds=N
-00010870: 6f6e 652c 2073 6967 6d61 3d4e 6f6e 652c  one, sigma=None,
-00010880: 202a 6172 6773 2c20 2a2a 6b77 6172 6773   *args, **kwargs
-00010890: 293a 0a20 2020 2020 2020 2069 6620 6c65  ):.        if le
-000108a0: 6e28 5b69 2066 6f72 2069 2069 6e20 5b63  n([i for i in [c
-000108b0: 6f76 732c 2063 686f 6c73 2c20 6576 6473  ovs, chols, evds
-000108c0: 5d20 6966 2069 2069 7320 6e6f 7420 4e6f  ] if i is not No
-000108d0: 6e65 5d29 2021 3d20 313a 0a20 2020 2020  ne]) != 1:.     
-000108e0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
-000108f0: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
-00010900: 2020 2020 2020 2020 2022 496e 636f 6d70           "Incomp
-00010910: 6174 6962 6c65 2070 6172 616d 6574 6572  atible parameter
-00010920: 697a 6174 696f 6e2e 2053 7065 6369 6679  ization. Specify
-00010930: 2065 7861 6374 6c79 206f 6e65 206f 6620   exactly one of 
-00010940: 636f 7673 2c20 6368 6f6c 732c 206f 7220  covs, chols, or 
-00010950: 6576 6473 2e22 0a20 2020 2020 2020 2020  evds.".         
-00010960: 2020 2029 0a0a 2020 2020 2020 2020 7369     )..        si
-00010970: 676d 6120 3d20 7369 676d 6120 6966 2073  gma = sigma if s
-00010980: 6967 6d61 2065 6c73 6520 300a 0a20 2020  igma else 0..   
-00010990: 2020 2020 2069 6620 6368 6f6c 7320 6973       if chols is
-000109a0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-000109b0: 2020 2020 2020 2063 6f76 7320 3d20 5b63         covs = [c
-000109c0: 686f 6c2e 646f 7428 6368 6f6c 2e54 2920  hol.dot(chol.T) 
-000109d0: 666f 7220 6368 6f6c 2069 6e20 6368 6f6c  for chol in chol
-000109e0: 735d 0a20 2020 2020 2020 2065 6c69 6620  s].        elif 
-000109f0: 6576 6473 2069 7320 6e6f 7420 4e6f 6e65  evds is not None
-00010a00: 3a0a 2020 2020 2020 2020 2020 2020 6569  :.            ei
-00010a10: 6768 5f69 7465 7261 626c 6520 3d20 6576  gh_iterable = ev
-00010a20: 6473 0a20 2020 2020 2020 2020 2020 2063  ds.            c
-00010a30: 6f76 7320 3d20 5b5d 0a20 2020 2020 2020  ovs = [].       
-00010a40: 2020 2020 2065 6967 735f 7365 702c 2051       eigs_sep, Q
-00010a50: 7320 3d20 7a69 7028 2a65 6967 685f 6974  s = zip(*eigh_it
-00010a60: 6572 6162 6c65 2920 2023 2055 6e7a 6970  erable)  # Unzip
-00010a70: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00010a80: 2065 6967 2c20 5120 696e 207a 6970 2865   eig, Q in zip(e
-00010a90: 6967 735f 7365 702c 2051 7329 3a0a 2020  igs_sep, Qs):.  
-00010aa0: 2020 2020 2020 2020 2020 2020 2020 636f                co
-00010ab0: 765f 6920 3d20 7074 2e64 6f74 2851 2c20  v_i = pt.dot(Q, 
-00010ac0: 7074 2e64 6f74 2870 742e 6469 6167 2865  pt.dot(pt.diag(e
-00010ad0: 6967 292c 2051 2e54 2929 0a20 2020 2020  ig), Q.T)).     
-00010ae0: 2020 2020 2020 2020 2020 2063 6f76 732e             covs.
-00010af0: 6170 7065 6e64 2863 6f76 5f69 290a 0a20  append(cov_i).. 
-00010b00: 2020 2020 2020 206d 7520 3d20 7074 2e61         mu = pt.a
-00010b10: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
-00010b20: 6528 6d75 290a 0a20 2020 2020 2020 2072  e(mu)..        r
-00010b30: 6574 7572 6e20 7375 7065 7228 292e 6469  eturn super().di
-00010b40: 7374 285b 6d75 2c20 7369 676d 612c 202a  st([mu, sigma, *
-00010b50: 636f 7673 5d2c 202a 2a6b 7761 7267 7329  covs], **kwargs)
-00010b60: 0a0a 2020 2020 6465 6620 6d6f 6d65 6e74  ..    def moment
-00010b70: 2872 762c 2073 697a 652c 206d 752c 2063  (rv, size, mu, c
-00010b80: 6f76 732c 2063 686f 6c73 2c20 6576 6473  ovs, chols, evds
-00010b90: 293a 0a20 2020 2020 2020 206d 6561 6e20  ):.        mean 
-00010ba0: 3d20 6d75 0a20 2020 2020 2020 2069 6620  = mu.        if 
-00010bb0: 6e6f 7420 7276 5f73 697a 655f 6973 5f6e  not rv_size_is_n
-00010bc0: 6f6e 6528 7369 7a65 293a 0a20 2020 2020  one(size):.     
-00010bd0: 2020 2020 2020 206d 6f6d 656e 745f 7369         moment_si
-00010be0: 7a65 203d 2070 742e 636f 6e63 6174 656e  ze = pt.concaten
-00010bf0: 6174 6528 5b73 697a 652c 206d 752e 7368  ate([size, mu.sh
-00010c00: 6170 655d 290a 2020 2020 2020 2020 2020  ape]).          
-00010c10: 2020 6d65 616e 203d 2070 742e 6675 6c6c    mean = pt.full
-00010c20: 286d 6f6d 656e 745f 7369 7a65 2c20 6d75  (moment_size, mu
-00010c30: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00010c40: 206d 6561 6e0a 0a20 2020 2064 6566 206c   mean..    def l
-00010c50: 6f67 7028 7661 6c75 652c 206d 752c 2073  ogp(value, mu, s
-00010c60: 6967 6d61 2c20 2a63 6f76 7329 3a0a 2020  igma, *covs):.  
-00010c70: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010c80: 2020 4361 6c63 756c 6174 6520 6c6f 672d    Calculate log-
-00010c90: 7072 6f62 6162 696c 6974 7920 6f66 204d  probability of M
-00010ca0: 756c 7469 7661 7269 6174 6520 4e6f 726d  ultivariate Norm
-00010cb0: 616c 2064 6973 7472 6962 7574 696f 6e0a  al distribution.
-00010cc0: 2020 2020 2020 2020 7769 7468 204b 726f          with Kro
-00010cd0: 6e65 636b 6572 2d73 7472 7563 7475 7265  necker-structure
-00010ce0: 6420 636f 7661 7269 616e 6365 2061 7420  d covariance at 
-00010cf0: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
-00010d00: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
-00010d10: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00010d20: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00010d30: 7661 6c75 653a 206e 756d 6572 6963 0a20  value: numeric. 
-00010d40: 2020 2020 2020 2020 2020 2056 616c 7565             Value
-00010d50: 2066 6f72 2077 6869 6368 206c 6f67 2d70   for which log-p
-00010d60: 726f 6261 6269 6c69 7479 2069 7320 6361  robability is ca
-00010d70: 6c63 756c 6174 6564 2e0a 0a20 2020 2020  lculated...     
-00010d80: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00010d90: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00010da0: 2020 2054 656e 736f 7256 6172 6961 626c     TensorVariabl
-00010db0: 650a 2020 2020 2020 2020 2222 220a 2020  e.        """.  
-00010dc0: 2020 2020 2020 2320 436f 6d70 7574 6573        # Computes
-00010dd0: 2074 6865 2071 7561 6472 6174 6963 2028   the quadratic (
-00010de0: 782d 6d75 295e 5420 4020 4b5e 2d31 2040  x-mu)^T @ K^-1 @
-00010df0: 2028 782d 6d75 2920 616e 6420 6c6f 6728   (x-mu) and log(
-00010e00: 6465 7428 4b29 290a 2020 2020 2020 2020  det(K)).        
-00010e10: 6966 2076 616c 7565 2e6e 6469 6d20 3e20  if value.ndim > 
-00010e20: 3220 6f72 2076 616c 7565 2e6e 6469 6d20  2 or value.ndim 
-00010e30: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
-00010e40: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00010e50: 6f72 2866 2249 6e76 616c 6964 2064 696d  or(f"Invalid dim
-00010e60: 656e 7369 6f6e 2066 6f72 2076 616c 7565  ension for value
-00010e70: 3a20 7b76 616c 7565 2e6e 6469 6d7d 2229  : {value.ndim}")
-00010e80: 0a20 2020 2020 2020 2069 6620 7661 6c75  .        if valu
-00010e90: 652e 6e64 696d 203d 3d20 313a 0a20 2020  e.ndim == 1:.   
-00010ea0: 2020 2020 2020 2020 206f 6e65 6469 6d20           onedim 
-00010eb0: 3d20 5472 7565 0a20 2020 2020 2020 2020  = True.         
-00010ec0: 2020 2076 616c 7565 203d 2076 616c 7565     value = value
-00010ed0: 5b4e 6f6e 652c 203a 5d0a 2020 2020 2020  [None, :].      
-00010ee0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00010ef0: 2020 2020 6f6e 6564 696d 203d 2046 616c      onedim = Fal
-00010f00: 7365 0a0a 2020 2020 2020 2020 6465 6c74  se..        delt
-00010f10: 6120 3d20 7661 6c75 6520 2d20 6d75 0a0a  a = value - mu..
-00010f20: 2020 2020 2020 2020 6569 6768 5f69 7465          eigh_ite
-00010f30: 7261 626c 6520 3d20 6d61 7028 6569 6768  rable = map(eigh
-00010f40: 2c20 636f 7673 290a 2020 2020 2020 2020  , covs).        
-00010f50: 6569 6773 5f73 6570 2c20 5173 203d 207a  eigs_sep, Qs = z
-00010f60: 6970 282a 6569 6768 5f69 7465 7261 626c  ip(*eigh_iterabl
-00010f70: 6529 2020 2320 556e 7a69 700a 2020 2020  e)  # Unzip.    
-00010f80: 2020 2020 5173 203d 206c 6973 7428 6d61      Qs = list(ma
-00010f90: 7028 7074 2e61 735f 7465 6e73 6f72 5f76  p(pt.as_tensor_v
-00010fa0: 6172 6961 626c 652c 2051 7329 290a 2020  ariable, Qs)).  
-00010fb0: 2020 2020 2020 5154 7320 3d20 6c69 7374        QTs = list
-00010fc0: 286d 6170 2870 742e 7472 616e 7370 6f73  (map(pt.transpos
-00010fd0: 652c 2051 7329 290a 0a20 2020 2020 2020  e, Qs))..       
-00010fe0: 2065 6967 735f 7365 7020 3d20 6c69 7374   eigs_sep = list
-00010ff0: 286d 6170 2870 742e 6173 5f74 656e 736f  (map(pt.as_tenso
-00011000: 725f 7661 7269 6162 6c65 2c20 6569 6773  r_variable, eigs
-00011010: 5f73 6570 2929 0a20 2020 2020 2020 2065  _sep)).        e
-00011020: 6967 7320 3d20 6b72 6f6e 5f64 6961 6728  igs = kron_diag(
-00011030: 2a65 6967 735f 7365 7029 2020 2320 436f  *eigs_sep)  # Co
-00011040: 6d62 696e 6520 7365 7061 7261 7465 2065  mbine separate e
-00011050: 6967 730a 2020 2020 2020 2020 6569 6773  igs.        eigs
-00011060: 202b 3d20 7369 676d 612a 2a32 0a20 2020   += sigma**2.   
-00011070: 2020 2020 204e 203d 2065 6967 732e 7368       N = eigs.sh
-00011080: 6170 655b 305d 0a0a 2020 2020 2020 2020  ape[0]..        
-00011090: 7371 7274 5f71 7561 6420 3d20 6b72 6f6e  sqrt_quad = kron
-000110a0: 5f64 6f74 2851 5473 2c20 6465 6c74 612e  _dot(QTs, delta.
-000110b0: 5429 0a20 2020 2020 2020 2073 7172 745f  T).        sqrt_
-000110c0: 7175 6164 203d 2073 7172 745f 7175 6164  quad = sqrt_quad
-000110d0: 202f 2070 742e 7371 7274 2865 6967 735b   / pt.sqrt(eigs[
-000110e0: 3a2c 204e 6f6e 655d 290a 2020 2020 2020  :, None]).      
-000110f0: 2020 6c6f 6764 6574 203d 2070 742e 7375    logdet = pt.su
-00011100: 6d28 7074 2e6c 6f67 2865 6967 7329 290a  m(pt.log(eigs)).
-00011110: 0a20 2020 2020 2020 2023 2053 7175 6172  .        # Squar
-00011120: 6520 6561 6368 2073 616d 706c 650a 2020  e each sample.  
-00011130: 2020 2020 2020 7175 6164 203d 2070 742e        quad = pt.
-00011140: 6261 7463 6865 645f 646f 7428 7371 7274  batched_dot(sqrt
-00011150: 5f71 7561 642e 542c 2073 7172 745f 7175  _quad.T, sqrt_qu
-00011160: 6164 2e54 290a 2020 2020 2020 2020 6966  ad.T).        if
-00011170: 206f 6e65 6469 6d3a 0a20 2020 2020 2020   onedim:.       
-00011180: 2020 2020 2071 7561 6420 3d20 7175 6164       quad = quad
-00011190: 5b30 5d0a 0a20 2020 2020 2020 2061 203d  [0]..        a =
-000111a0: 202d 2871 7561 6420 2b20 6c6f 6764 6574   -(quad + logdet
-000111b0: 202b 204e 202a 2070 742e 6c6f 6728 3220   + N * pt.log(2 
-000111c0: 2a20 6e70 2e70 6929 2920 2f20 322e 300a  * np.pi)) / 2.0.
-000111d0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-000111e0: 0a0a 0a63 6c61 7373 2043 4152 5256 2852  ...class CARRV(R
-000111f0: 616e 646f 6d56 6172 6961 626c 6529 3a0a  andomVariable):.
-00011200: 2020 2020 6e61 6d65 203d 2022 6361 7222      name = "car"
-00011210: 0a20 2020 206e 6469 6d5f 7375 7070 203d  .    ndim_supp =
-00011220: 2031 0a20 2020 206e 6469 6d73 5f70 6172   1.    ndims_par
-00011230: 616d 7320 3d20 5b31 2c20 322c 2030 2c20  ams = [1, 2, 0, 
-00011240: 305d 0a20 2020 2064 7479 7065 203d 2022  0].    dtype = "
-00011250: 666c 6f61 7458 220a 2020 2020 5f70 7269  floatX".    _pri
-00011260: 6e74 5f6e 616d 6520 3d20 2822 4341 5222  nt_name = ("CAR"
-00011270: 2c20 225c 5c6f 7065 7261 746f 726e 616d  , "\\operatornam
-00011280: 657b 4341 527d 2229 0a0a 2020 2020 6465  e{CAR}")..    de
-00011290: 6620 6d61 6b65 5f6e 6f64 6528 7365 6c66  f make_node(self
-000112a0: 2c20 726e 672c 2073 697a 652c 2064 7479  , rng, size, dty
-000112b0: 7065 2c20 6d75 2c20 572c 2061 6c70 6861  pe, mu, W, alpha
-000112c0: 2c20 7461 7529 3a0a 2020 2020 2020 2020  , tau):.        
-000112d0: 6d75 203d 2070 742e 6173 5f74 656e 736f  mu = pt.as_tenso
-000112e0: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
-000112f0: 5828 6d75 2929 0a0a 2020 2020 2020 2020  X(mu))..        
-00011300: 5720 3d20 7079 7465 6e73 6f72 2e73 7061  W = pytensor.spa
-00011310: 7273 652e 6173 5f73 7061 7273 655f 6f72  rse.as_sparse_or
-00011320: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
-00011330: 2866 6c6f 6174 5828 5729 290a 2020 2020  (floatX(W)).    
-00011340: 2020 2020 6966 206e 6f74 2057 2e6e 6469      if not W.ndi
-00011350: 6d20 3d3d 2032 3a0a 2020 2020 2020 2020  m == 2:.        
-00011360: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00011370: 7272 6f72 2822 5720 6d75 7374 2062 6520  rror("W must be 
-00011380: 6120 6d61 7472 6978 2028 6e64 696d 3d32  a matrix (ndim=2
-00011390: 292e 2229 0a0a 2020 2020 2020 2020 7370  ).")..        sp
-000113a0: 6172 7365 203d 2069 7369 6e73 7461 6e63  arse = isinstanc
-000113b0: 6528 572c 2070 7974 656e 736f 722e 7370  e(W, pytensor.sp
-000113c0: 6172 7365 2e53 7061 7273 6556 6172 6961  arse.SparseVaria
-000113d0: 626c 6529 0a20 2020 2020 2020 206d 7367  ble).        msg
-000113e0: 203d 2022 5720 6d75 7374 2062 6520 6120   = "W must be a 
-000113f0: 7379 6d6d 6574 7269 6320 6164 6a61 6365  symmetric adjace
-00011400: 6e63 7920 6d61 7472 6978 2e22 0a20 2020  ncy matrix.".   
-00011410: 2020 2020 2069 6620 7370 6172 7365 3a0a       if sparse:.
-00011420: 2020 2020 2020 2020 2020 2020 6162 735f              abs_
-00011430: 6469 6666 203d 2070 7974 656e 736f 722e  diff = pytensor.
-00011440: 7370 6172 7365 2e62 6173 6963 2e6d 756c  sparse.basic.mul
-00011450: 2870 7974 656e 736f 722e 7370 6172 7365  (pytensor.sparse
-00011460: 2e73 6967 6e28 5720 2d20 572e 5429 2c20  .sign(W - W.T), 
-00011470: 5720 2d20 572e 5429 0a20 2020 2020 2020  W - W.T).       
-00011480: 2020 2020 2057 203d 2041 7373 6572 7428       W = Assert(
-00011490: 6d73 6729 2857 2c20 7074 2e69 7363 6c6f  msg)(W, pt.isclo
-000114a0: 7365 2870 7974 656e 736f 722e 7370 6172  se(pytensor.spar
-000114b0: 7365 2e73 705f 7375 6d28 6162 735f 6469  se.sp_sum(abs_di
-000114c0: 6666 292c 2030 2929 0a20 2020 2020 2020  ff), 0)).       
-000114d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-000114e0: 2020 2057 203d 2041 7373 6572 7428 6d73     W = Assert(ms
-000114f0: 6729 2857 2c20 7074 2e61 6c6c 636c 6f73  g)(W, pt.allclos
-00011500: 6528 572c 2057 2e54 2929 0a0a 2020 2020  e(W, W.T))..    
-00011510: 2020 2020 7461 7520 3d20 7074 2e61 735f      tau = pt.as_
-00011520: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
-00011530: 666c 6f61 7458 2874 6175 2929 0a20 2020  floatX(tau)).   
-00011540: 2020 2020 2061 6c70 6861 203d 2070 742e       alpha = pt.
-00011550: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
-00011560: 6c65 2866 6c6f 6174 5828 616c 7068 6129  le(floatX(alpha)
-00011570: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
-00011580: 6e20 7375 7065 7228 292e 6d61 6b65 5f6e  n super().make_n
-00011590: 6f64 6528 726e 672c 2073 697a 652c 2064  ode(rng, size, d
-000115a0: 7479 7065 2c20 6d75 2c20 572c 2061 6c70  type, mu, W, alp
-000115b0: 6861 2c20 7461 7529 0a0a 2020 2020 6465  ha, tau)..    de
-000115c0: 6620 5f69 6e66 6572 5f73 6861 7065 2873  f _infer_shape(s
-000115d0: 656c 662c 2073 697a 652c 2064 6973 745f  elf, size, dist_
-000115e0: 7061 7261 6d73 2c20 7061 7261 6d5f 7368  params, param_sh
-000115f0: 6170 6573 3d4e 6f6e 6529 3a0a 2020 2020  apes=None):.    
-00011600: 2020 2020 7368 6170 6520 3d20 7475 706c      shape = tupl
-00011610: 6528 7369 7a65 2920 2b20 2864 6973 745f  e(size) + (dist_
-00011620: 7061 7261 6d73 5b30 5d2e 7368 6170 655b  params[0].shape[
-00011630: 2d31 5d2c 290a 2020 2020 2020 2020 7265  -1],).        re
-00011640: 7475 726e 2073 6861 7065 0a0a 2020 2020  turn shape..    
-00011650: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
-00011660: 2064 6566 2072 6e67 5f66 6e28 636c 732c   def rng_fn(cls,
-00011670: 2072 6e67 3a20 6e70 2e72 616e 646f 6d2e   rng: np.random.
-00011680: 5261 6e64 6f6d 5374 6174 652c 206d 752c  RandomState, mu,
-00011690: 2057 2c20 616c 7068 612c 2074 6175 2c20   W, alpha, tau, 
-000116a0: 7369 7a65 293a 0a20 2020 2020 2020 2022  size):.        "
-000116b0: 2222 0a20 2020 2020 2020 2049 6d70 6c65  "".        Imple
-000116c0: 6d65 6e74 6174 696f 6e20 6f66 2061 6c67  mentation of alg
-000116d0: 6f72 6974 686d 2066 726f 6d20 7061 7065  orithm from pape
-000116e0: 720a 2020 2020 2020 2020 4861 7661 7264  r.        Havard
-000116f0: 2052 7565 2c20 3230 3031 2e20 2246 6173   Rue, 2001. "Fas
-00011700: 7420 7361 6d70 6c69 6e67 206f 6620 4761  t sampling of Ga
-00011710: 7573 7369 616e 204d 6172 6b6f 7620 7261  ussian Markov ra
-00011720: 6e64 6f6d 2066 6965 6c64 732c 220a 2020  ndom fields,".  
-00011730: 2020 2020 2020 4a6f 7572 6e61 6c20 6f66        Journal of
-00011740: 2074 6865 2052 6f79 616c 2053 7461 7469   the Royal Stati
-00011750: 7374 6963 616c 2053 6f63 6965 7479 2053  stical Society S
-00011760: 6572 6965 7320 422c 2052 6f79 616c 2053  eries B, Royal S
-00011770: 7461 7469 7374 6963 616c 2053 6f63 6965  tatistical Socie
-00011780: 7479 2c0a 2020 2020 2020 2020 766f 6c2e  ty,.        vol.
-00011790: 2036 3328 3229 2c20 7061 6765 7320 3332   63(2), pages 32
-000117a0: 352d 3333 382e 2044 4f49 3a20 3130 2e31  5-338. DOI: 10.1
-000117b0: 3131 312f 3134 3637 2d39 3836 382e 3030  111/1467-9868.00
-000117c0: 3238 380a 2020 2020 2020 2020 2222 220a  288.        """.
-000117d0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
-000117e0: 6369 7079 2e73 7061 7273 652e 6973 7370  cipy.sparse.issp
-000117f0: 6172 7365 2857 293a 0a20 2020 2020 2020  arse(W):.       
-00011800: 2020 2020 2057 203d 2073 6369 7079 2e73       W = scipy.s
-00011810: 7061 7273 652e 6373 725f 6d61 7472 6978  parse.csr_matrix
-00011820: 2857 290a 2020 2020 2020 2020 7320 3d20  (W).        s = 
-00011830: 6e70 2e61 7361 7272 6179 2857 2e73 756d  np.asarray(W.sum
-00011840: 2861 7869 733d 3029 295b 305d 0a20 2020  (axis=0))[0].   
-00011850: 2020 2020 2044 203d 2073 6369 7079 2e73       D = scipy.s
-00011860: 7061 7273 652e 6469 6167 7328 7329 0a20  parse.diags(s). 
-00011870: 2020 2020 2020 2074 6175 203d 2073 6369         tau = sci
-00011880: 7079 2e73 7061 7273 652e 6373 725f 6d61  py.sparse.csr_ma
-00011890: 7472 6978 2874 6175 290a 2020 2020 2020  trix(tau).      
-000118a0: 2020 616c 7068 6120 3d20 7363 6970 792e    alpha = scipy.
-000118b0: 7370 6172 7365 2e63 7372 5f6d 6174 7269  sparse.csr_matri
-000118c0: 7828 616c 7068 6129 0a0a 2020 2020 2020  x(alpha)..      
-000118d0: 2020 5120 3d20 7461 752e 6d75 6c74 6970    Q = tau.multip
-000118e0: 6c79 2844 202d 2061 6c70 6861 2e6d 756c  ly(D - alpha.mul
-000118f0: 7469 706c 7928 5729 290a 0a20 2020 2020  tiply(W))..     
-00011900: 2020 2070 6572 6d5f 6172 7261 7920 3d20     perm_array = 
-00011910: 7363 6970 792e 7370 6172 7365 2e63 7367  scipy.sparse.csg
-00011920: 7261 7068 2e72 6576 6572 7365 5f63 7574  raph.reverse_cut
-00011930: 6869 6c6c 5f6d 636b 6565 2851 2c20 7379  hill_mckee(Q, sy
-00011940: 6d6d 6574 7269 635f 6d6f 6465 3d54 7275  mmetric_mode=Tru
-00011950: 6529 0a20 2020 2020 2020 2069 6e76 5f70  e).        inv_p
-00011960: 6572 6d20 3d20 6e70 2e61 7267 736f 7274  erm = np.argsort
-00011970: 2870 6572 6d5f 6172 7261 7929 0a0a 2020  (perm_array)..  
-00011980: 2020 2020 2020 5120 3d20 515b 7065 726d        Q = Q[perm
-00011990: 5f61 7272 6179 2c20 3a5d 5b3a 2c20 7065  _array, :][:, pe
-000119a0: 726d 5f61 7272 6179 5d0a 0a20 2020 2020  rm_array]..     
-000119b0: 2020 2051 6220 3d20 512e 6469 6167 6f6e     Qb = Q.diagon
-000119c0: 616c 2829 0a20 2020 2020 2020 2075 203d  al().        u =
-000119d0: 2031 0a20 2020 2020 2020 2077 6869 6c65   1.        while
-000119e0: 206e 702e 636f 756e 745f 6e6f 6e7a 6572   np.count_nonzer
-000119f0: 6f28 512e 6469 6167 6f6e 616c 2875 2929  o(Q.diagonal(u))
-00011a00: 203e 2030 3a0a 2020 2020 2020 2020 2020   > 0:.          
-00011a10: 2020 5162 203d 206e 702e 7673 7461 636b    Qb = np.vstack
-00011a20: 2828 6e70 2e70 6164 2851 2e64 6961 676f  ((np.pad(Q.diago
-00011a30: 6e61 6c28 7529 2c20 2875 2c20 3029 2c20  nal(u), (u, 0), 
-00011a40: 636f 6e73 7461 6e74 5f76 616c 7565 733d  constant_values=
-00011a50: 2830 2c20 3029 292c 2051 6229 290a 2020  (0, 0)), Qb)).  
-00011a60: 2020 2020 2020 2020 2020 7520 2b3d 2031            u += 1
-00011a70: 0a0a 2020 2020 2020 2020 4c20 3d20 7363  ..        L = sc
-00011a80: 6970 792e 6c69 6e61 6c67 2e63 686f 6c65  ipy.linalg.chole
-00011a90: 736b 795f 6261 6e64 6564 2851 622c 206c  sky_banded(Qb, l
-00011aa0: 6f77 6572 3d46 616c 7365 290a 0a20 2020  ower=False)..   
-00011ab0: 2020 2020 2073 697a 6520 3d20 7475 706c       size = tupl
-00011ac0: 6528 7369 7a65 206f 7220 2829 290a 2020  e(size or ()).  
-00011ad0: 2020 2020 2020 6966 2073 697a 653a 0a20        if size:. 
-00011ae0: 2020 2020 2020 2020 2020 206d 7520 3d20             mu = 
-00011af0: 6e70 2e62 726f 6164 6361 7374 5f74 6f28  np.broadcast_to(
-00011b00: 6d75 2c20 7369 7a65 202b 2028 6d75 2e73  mu, size + (mu.s
-00011b10: 6861 7065 5b2d 315d 2c29 290a 2020 2020  hape[-1],)).    
-00011b20: 2020 2020 7a20 3d20 726e 672e 6e6f 726d      z = rng.norm
-00011b30: 616c 2873 697a 653d 6d75 2e73 6861 7065  al(size=mu.shape
-00011b40: 290a 2020 2020 2020 2020 7361 6d70 6c65  ).        sample
-00011b50: 7320 3d20 6e70 2e65 6d70 7479 287a 2e73  s = np.empty(z.s
-00011b60: 6861 7065 290a 2020 2020 2020 2020 666f  hape).        fo
-00011b70: 7220 6964 7820 696e 206e 702e 6e64 696e  r idx in np.ndin
-00011b80: 6465 7828 6d75 2e73 6861 7065 5b3a 2d31  dex(mu.shape[:-1
-00011b90: 5d29 3a0a 2020 2020 2020 2020 2020 2020  ]):.            
-00011ba0: 7361 6d70 6c65 735b 6964 785d 203d 2073  samples[idx] = s
-00011bb0: 6369 7079 2e6c 696e 616c 672e 6368 6f5f  cipy.linalg.cho_
-00011bc0: 736f 6c76 655f 6261 6e64 6564 2828 4c2c  solve_banded((L,
-00011bd0: 2046 616c 7365 292c 207a 5b69 6478 5d29   False), z[idx])
-00011be0: 202b 206d 755b 6964 785d 5b70 6572 6d5f   + mu[idx][perm_
-00011bf0: 6172 7261 795d 0a20 2020 2020 2020 2073  array].        s
-00011c00: 616d 706c 6573 203d 2073 616d 706c 6573  amples = samples
-00011c10: 5b2e 2e2e 2c20 696e 765f 7065 726d 5d0a  [..., inv_perm].
-00011c20: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00011c30: 616d 706c 6573 0a0a 0a63 6172 203d 2043  amples...car = C
-00011c40: 4152 5256 2829 0a0a 0a63 6c61 7373 2043  ARRV()...class C
-00011c50: 4152 2843 6f6e 7469 6e75 6f75 7329 3a0a  AR(Continuous):.
-00011c60: 2020 2020 7222 2222 0a20 2020 204c 696b      r""".    Lik
-00011c70: 656c 6968 6f6f 6420 666f 7220 6120 636f  elihood for a co
-00011c80: 6e64 6974 696f 6e61 6c20 6175 746f 7265  nditional autore
-00011c90: 6772 6573 7369 6f6e 2e20 5468 6973 2069  gression. This i
-00011ca0: 7320 6120 7370 6563 6961 6c20 6361 7365  s a special case
-00011cb0: 206f 6620 7468 650a 2020 2020 6d75 6c74   of the.    mult
-00011cc0: 6976 6172 6961 7465 206e 6f72 6d61 6c20  ivariate normal 
-00011cd0: 7769 7468 2061 6e20 6164 6a61 6365 6e63  with an adjacenc
-00011ce0: 792d 7374 7275 6374 7572 6564 2063 6f76  y-structured cov
-00011cf0: 6172 6961 6e63 6520 6d61 7472 6978 2e0a  ariance matrix..
-00011d00: 0a20 2020 202e 2e20 6d61 7468 3a3a 0a0a  .    .. math::..
-00011d10: 2020 2020 2020 2066 2878 205c 6d69 6420         f(x \mid 
-00011d20: 572c 205c 616c 7068 612c 205c 7461 7529  W, \alpha, \tau)
-00011d30: 203d 0a20 2020 2020 2020 2020 2020 5c66   =.           \f
-00011d40: 7261 637b 7c54 7c5e 7b31 2f32 7d7d 7b28  rac{|T|^{1/2}}{(
-00011d50: 325c 7069 295e 7b6b 2f32 7d7d 0a20 2020  2\pi)^{k/2}}.   
-00011d60: 2020 2020 2020 2020 5c65 7870 5c6c 6566          \exp\lef
-00011d70: 745c 7b20 2d5c 6672 6163 7b31 7d7b 327d  t\{ -\frac{1}{2}
-00011d80: 2028 782d 5c6d 7529 5e7b 5c70 7269 6d65   (x-\mu)^{\prime
-00011d90: 7d20 545e 7b2d 317d 2028 782d 5c6d 7529  } T^{-1} (x-\mu)
-00011da0: 205c 7269 6768 745c 7d0a 0a20 2020 2077   \right\}..    w
-00011db0: 6865 7265 203a 6d61 7468 3a60 5420 3d20  here :math:`T = 
-00011dc0: 285c 7461 7520 4428 492d 5c61 6c70 6861  (\tau D(I-\alpha
-00011dd0: 2057 2929 5e7b 2d31 7d60 2061 6e64 203a   W))^{-1}` and :
-00011de0: 6d61 7468 3a60 4420 3d20 6469 6167 285c  math:`D = diag(\
-00011df0: 7375 6d5f 6920 575f 7b69 6a7d 2960 2e0a  sum_i W_{ij})`..
-00011e00: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
-00011e10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011e20: 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020 5375  =========.    Su
-00011e30: 7070 6f72 7420 2020 3a6d 6174 683a 6078  pport   :math:`x
-00011e40: 205c 696e 205c 6d61 7468 6262 7b52 7d5e   \in \mathbb{R}^
-00011e50: 6b60 0a20 2020 204d 6561 6e20 2020 2020  k`.    Mean     
-00011e60: 203a 6d61 7468 3a60 5c6d 7520 5c69 6e20   :math:`\mu \in 
-00011e70: 5c6d 6174 6862 627b 527d 5e6b 600a 2020  \mathbb{R}^k`.  
-00011e80: 2020 5661 7269 616e 6365 2020 3a6d 6174    Variance  :mat
-00011e90: 683a 6028 5c74 6175 2044 2849 2d5c 616c  h:`(\tau D(I-\al
-00011ea0: 7068 6120 5729 295e 7b2d 317d 600a 2020  pha W))^{-1}`.  
-00011eb0: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
-00011ec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00011ed0: 3d3d 3d3d 3d3d 0a0a 2020 2020 5061 7261  ======..    Para
-00011ee0: 6d65 7465 7273 0a20 2020 202d 2d2d 2d2d  meters.    -----
-00011ef0: 2d2d 2d2d 2d0a 2020 2020 6d75 203a 2074  -----.    mu : t
-00011f00: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-00011f10: 6f61 740a 2020 2020 2020 2020 5265 616c  oat.        Real
-00011f20: 2d76 616c 7565 6420 6d65 616e 2076 6563  -valued mean vec
-00011f30: 746f 720a 2020 2020 5720 3a20 284d 2c20  tor.    W : (M, 
-00011f40: 4d29 2074 656e 736f 725f 6c69 6b65 206f  M) tensor_like o
-00011f50: 6620 696e 740a 2020 2020 2020 2020 5379  f int.        Sy
-00011f60: 6d6d 6574 7269 6320 6164 6a61 6365 6e63  mmetric adjacenc
-00011f70: 7920 6d61 7472 6978 206f 6620 3173 2061  y matrix of 1s a
-00011f80: 6e64 2030 7320 696e 6469 6361 7469 6e67  nd 0s indicating
-00011f90: 0a20 2020 2020 2020 2061 646a 6163 656e  .        adjacen
-00011fa0: 6379 2062 6574 7765 656e 2065 6c65 6d65  cy between eleme
-00011fb0: 6e74 732e 2049 6620 706f 7373 6962 6c65  nts. If possible
-00011fc0: 2c20 2a57 2a20 6973 2063 6f6e 7665 7274  , *W* is convert
-00011fd0: 6564 0a20 2020 2020 2020 2074 6f20 6120  ed.        to a 
-00011fe0: 7370 6172 7365 206d 6174 7269 782c 2066  sparse matrix, f
-00011ff0: 616c 6c69 6e67 2062 6163 6b20 746f 2061  alling back to a
-00012000: 2064 656e 7365 2076 6172 6961 626c 652e   dense variable.
-00012010: 0a20 2020 2020 2020 203a 6675 6e63 3a60  .        :func:`
-00012020: 7e70 7974 656e 736f 722e 7370 6172 7365  ~pytensor.sparse
-00012030: 2e62 6173 6963 2e61 735f 7370 6172 7365  .basic.as_sparse
-00012040: 5f6f 725f 7465 6e73 6f72 5f76 6172 6961  _or_tensor_varia
-00012050: 626c 6560 2069 730a 2020 2020 2020 2020  ble` is.        
-00012060: 7573 6564 2066 6f72 2074 6869 7320 7370  used for this sp
-00012070: 6172 7365 206f 7220 7465 6e73 6f72 7661  arse or tensorva
-00012080: 7269 6162 6c65 2063 6f6e 7665 7273 696f  riable conversio
-00012090: 6e2e 0a20 2020 2061 6c70 6861 203a 2074  n..    alpha : t
-000120a0: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-000120b0: 6f61 740a 2020 2020 2020 2020 4175 746f  oat.        Auto
-000120c0: 7265 6772 6573 7369 6f6e 2070 6172 616d  regression param
-000120d0: 6574 6572 2074 616b 696e 6720 7661 6c75  eter taking valu
-000120e0: 6573 2062 6574 7765 656e 202d 3120 616e  es between -1 an
-000120f0: 6420 312e 2056 616c 7565 7320 636c 6f73  d 1. Values clos
-00012100: 6572 2074 6f20 3020 696e 6469 6361 7465  er to 0 indicate
-00012110: 2077 6561 6b65 720a 2020 2020 2020 2020   weaker.        
-00012120: 636f 7272 656c 6174 696f 6e20 616e 6420  correlation and 
-00012130: 7661 6c75 6573 2063 6c6f 7365 7220 746f  values closer to
-00012140: 2031 2069 6e64 6963 6174 6520 6869 6768   1 indicate high
-00012150: 6572 2061 7574 6f63 6f72 7265 6c61 7469  er autocorrelati
-00012160: 6f6e 2e20 466f 7220 6d6f 7374 2075 7365  on. For most use
-00012170: 2063 6173 6573 2c20 7468 650a 2020 2020   cases, the.    
-00012180: 2020 2020 7375 7070 6f72 7420 6f66 2061      support of a
-00012190: 6c70 6861 2073 686f 756c 6420 6265 2072  lpha should be r
-000121a0: 6573 7472 6963 7465 6420 746f 2028 302c  estricted to (0,
-000121b0: 2031 292e 0a20 2020 2074 6175 203a 2074   1)..    tau : t
-000121c0: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
-000121d0: 6f61 740a 2020 2020 2020 2020 506f 7369  oat.        Posi
-000121e0: 7469 7665 2070 7265 6369 7369 6f6e 2076  tive precision v
-000121f0: 6172 6961 626c 6520 636f 6e74 726f 6c6c  ariable controll
-00012200: 696e 6720 7468 6520 7363 616c 6520 6f66  ing the scale of
-00012210: 2074 6865 2075 6e64 6572 6c79 696e 6720   the underlying 
-00012220: 6e6f 726d 616c 2076 6172 6961 7465 732e  normal variates.
-00012230: 0a0a 2020 2020 5265 6665 7265 6e63 6573  ..    References
-00012240: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a  .    ----------.
-00012250: 2020 2020 2e2e 2020 4a69 6e2c 2058 2e2c      ..  Jin, X.,
-00012260: 2043 6172 6c69 6e2c 2042 2e2c 2042 616e   Carlin, B., Ban
-00012270: 6572 6a65 652c 2053 2e0a 2020 2020 2020  erjee, S..      
-00012280: 2020 2247 656e 6572 616c 697a 6564 2048    "Generalized H
-00012290: 6965 7261 7263 6869 6361 6c20 4d75 6c74  ierarchical Mult
-000122a0: 6976 6172 6961 7465 2043 4152 204d 6f64  ivariate CAR Mod
-000122b0: 656c 7320 666f 7220 4172 6561 6c20 4461  els for Areal Da
-000122c0: 7461 220a 2020 2020 2020 2020 4269 6f6d  ta".        Biom
-000122d0: 6574 7269 6373 2c20 566f 6c2e 2036 312c  etrics, Vol. 61,
-000122e0: 204e 6f2e 2034 2028 4465 632e 2c20 3230   No. 4 (Dec., 20
-000122f0: 3035 292c 2070 702e 2039 3530 2d39 3631  05), pp. 950-961
-00012300: 0a20 2020 2022 2222 0a20 2020 2072 765f  .    """.    rv_
-00012310: 6f70 203d 2063 6172 0a0a 2020 2020 4063  op = car..    @c
-00012320: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00012330: 6566 2064 6973 7428 636c 732c 206d 752c  ef dist(cls, mu,
-00012340: 2057 2c20 616c 7068 612c 2074 6175 2c20   W, alpha, tau, 
-00012350: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
-00012360: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-00012370: 2073 7570 6572 2829 2e64 6973 7428 5b6d   super().dist([m
-00012380: 752c 2057 2c20 616c 7068 612c 2074 6175  u, W, alpha, tau
-00012390: 5d2c 202a 2a6b 7761 7267 7329 0a0a 2020  ], **kwargs)..  
-000123a0: 2020 6465 6620 6d6f 6d65 6e74 2872 762c    def moment(rv,
-000123b0: 2073 697a 652c 206d 752c 2057 2c20 616c   size, mu, W, al
-000123c0: 7068 612c 2074 6175 293a 0a20 2020 2020  pha, tau):.     
-000123d0: 2020 2072 6574 7572 6e20 7074 2e66 756c     return pt.ful
-000123e0: 6c5f 6c69 6b65 2872 762c 206d 7529 0a0a  l_like(rv, mu)..
-000123f0: 2020 2020 6465 6620 6c6f 6770 2876 616c      def logp(val
-00012400: 7565 2c20 6d75 2c20 572c 2061 6c70 6861  ue, mu, W, alpha
-00012410: 2c20 7461 7529 3a0a 2020 2020 2020 2020  , tau):.        
-00012420: 2222 220a 2020 2020 2020 2020 4361 6c63  """.        Calc
-00012430: 756c 6174 6520 6c6f 672d 7072 6f62 6162  ulate log-probab
-00012440: 696c 6974 7920 6f66 2061 2043 4152 2d64  ility of a CAR-d
-00012450: 6973 7472 6962 7574 6564 2076 6563 746f  istributed vecto
-00012460: 720a 2020 2020 2020 2020 6174 2073 7065  r.        at spe
-00012470: 6369 6669 6564 2076 616c 7565 2e20 5468  cified value. Th
-00012480: 6973 206c 6f67 2070 726f 6261 6269 6c69  is log probabili
-00012490: 7479 2066 756e 6374 696f 6e20 6469 6666  ty function diff
-000124a0: 6572 7320 6672 6f6d 0a20 2020 2020 2020  ers from.       
-000124b0: 2074 6865 2074 7275 6520 4341 5220 6c6f   the true CAR lo
-000124c0: 6720 6465 6e73 6974 7920 2841 4b41 2061  g density (AKA a
-000124d0: 206d 756c 7469 7661 7269 6174 6520 6e6f   multivariate no
-000124e0: 726d 616c 2077 6974 6820 4341 522d 7374  rmal with CAR-st
-000124f0: 7275 6374 7572 6564 0a20 2020 2020 2020  ructured.       
-00012500: 2063 6f76 6172 6961 6e63 6520 6d61 7472   covariance matr
-00012510: 6978 2920 6279 2061 6e20 6164 6469 7469  ix) by an additi
-00012520: 7665 2063 6f6e 7374 616e 742e 0a0a 2020  ve constant...  
-00012530: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-00012540: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-00012550: 2d2d 2d0a 2020 2020 2020 2020 7661 6c75  ---.        valu
-00012560: 653a 2061 7272 6179 0a20 2020 2020 2020  e: array.       
-00012570: 2020 2020 2056 616c 7565 2066 6f72 2077       Value for w
-00012580: 6869 6368 206c 6f67 2d70 726f 6261 6269  hich log-probabi
-00012590: 6c69 7479 2069 7320 6361 6c63 756c 6174  lity is calculat
-000125a0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
-000125b0: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-000125c0: 2d2d 2d2d 0a20 2020 2020 2020 2054 656e  ----.        Ten
-000125d0: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
-000125e0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-000125f0: 2073 7061 7273 6520 3d20 6973 696e 7374   sparse = isinst
-00012600: 616e 6365 2857 2c20 2870 7974 656e 736f  ance(W, (pytenso
-00012610: 722e 7370 6172 7365 2e53 7061 7273 6543  r.sparse.SparseC
-00012620: 6f6e 7374 616e 742c 2070 7974 656e 736f  onstant, pytenso
-00012630: 722e 7370 6172 7365 2e53 7061 7273 6556  r.sparse.SparseV
-00012640: 6172 6961 626c 6529 290a 0a20 2020 2020  ariable))..     
-00012650: 2020 2069 6620 7370 6172 7365 3a0a 2020     if sparse:.  
-00012660: 2020 2020 2020 2020 2020 4420 3d20 7370            D = sp
-00012670: 5f73 756d 2857 2c20 6178 6973 3d30 290a  _sum(W, axis=0).
-00012680: 2020 2020 2020 2020 2020 2020 4469 6e76              Dinv
-00012690: 5f73 7172 7420 3d20 7074 2e64 6961 6728  _sqrt = pt.diag(
-000126a0: 3120 2f20 7074 2e73 7172 7428 4429 290a  1 / pt.sqrt(D)).
-000126b0: 2020 2020 2020 2020 2020 2020 4457 4420              DWD 
-000126c0: 3d20 7074 2e64 6f74 2870 7974 656e 736f  = pt.dot(pytenso
-000126d0: 722e 7370 6172 7365 2e64 6f74 2844 696e  r.sparse.dot(Din
-000126e0: 765f 7371 7274 2c20 5729 2c20 4469 6e76  v_sqrt, W), Dinv
-000126f0: 5f73 7172 7429 0a20 2020 2020 2020 2065  _sqrt).        e
-00012700: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00012710: 2044 203d 2057 2e73 756d 2861 7869 733d   D = W.sum(axis=
-00012720: 3029 0a20 2020 2020 2020 2020 2020 2044  0).            D
-00012730: 696e 765f 7371 7274 203d 2070 742e 6469  inv_sqrt = pt.di
-00012740: 6167 2831 202f 2070 742e 7371 7274 2844  ag(1 / pt.sqrt(D
-00012750: 2929 0a20 2020 2020 2020 2020 2020 2044  )).            D
-00012760: 5744 203d 2070 742e 646f 7428 7074 2e64  WD = pt.dot(pt.d
-00012770: 6f74 2844 696e 765f 7371 7274 2c20 5729  ot(Dinv_sqrt, W)
-00012780: 2c20 4469 6e76 5f73 7172 7429 0a20 2020  , Dinv_sqrt).   
-00012790: 2020 2020 206c 616d 203d 2070 742e 736c       lam = pt.sl
-000127a0: 696e 616c 672e 6569 6776 616c 7368 2844  inalg.eigvalsh(D
-000127b0: 5744 2c20 7074 2e65 7965 2844 5744 2e73  WD, pt.eye(DWD.s
-000127c0: 6861 7065 5b30 5d29 290a 0a20 2020 2020  hape[0]))..     
-000127d0: 2020 2064 2c20 5f20 3d20 572e 7368 6170     d, _ = W.shap
-000127e0: 650a 0a20 2020 2020 2020 2069 6620 7661  e..        if va
-000127f0: 6c75 652e 6e64 696d 203d 3d20 313a 0a20  lue.ndim == 1:. 
-00012800: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00012810: 203d 2076 616c 7565 5b4e 6f6e 652c 203a   = value[None, :
-00012820: 5d0a 0a20 2020 2020 2020 206c 6f67 7461  ]..        logta
-00012830: 7520 3d20 6420 2a20 7074 2e6c 6f67 2874  u = d * pt.log(t
-00012840: 6175 292e 7375 6d28 290a 2020 2020 2020  au).sum().      
-00012850: 2020 6c6f 6764 6574 203d 2070 742e 6c6f    logdet = pt.lo
-00012860: 6728 3120 2d20 616c 7068 612e 5420 2a20  g(1 - alpha.T * 
-00012870: 6c61 6d5b 3a2c 204e 6f6e 655d 292e 7375  lam[:, None]).su
-00012880: 6d28 290a 2020 2020 2020 2020 6465 6c74  m().        delt
-00012890: 6120 3d20 7661 6c75 6520 2d20 6d75 0a0a  a = value - mu..
-000128a0: 2020 2020 2020 2020 6966 2073 7061 7273          if spars
-000128b0: 653a 0a20 2020 2020 2020 2020 2020 2057  e:.            W
-000128c0: 6465 6c74 6120 3d20 7079 7465 6e73 6f72  delta = pytensor
-000128d0: 2e73 7061 7273 652e 646f 7428 6465 6c74  .sparse.dot(delt
-000128e0: 612c 2057 290a 2020 2020 2020 2020 656c  a, W).        el
-000128f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00012900: 5764 656c 7461 203d 2070 742e 646f 7428  Wdelta = pt.dot(
-00012910: 6465 6c74 612c 2057 290a 0a20 2020 2020  delta, W)..     
-00012920: 2020 2074 6175 5f64 6f74 5f64 656c 7461     tau_dot_delta
-00012930: 203d 2044 5b4e 6f6e 652c 203a 5d20 2a20   = D[None, :] * 
-00012940: 6465 6c74 6120 2d20 616c 7068 6120 2a20  delta - alpha * 
-00012950: 5764 656c 7461 0a20 2020 2020 2020 206c  Wdelta.        l
-00012960: 6f67 7175 6164 203d 2028 7461 7520 2a20  ogquad = (tau * 
-00012970: 6465 6c74 6120 2a20 7461 755f 646f 745f  delta * tau_dot_
-00012980: 6465 6c74 6129 2e73 756d 2861 7869 733d  delta).sum(axis=
-00012990: 2d31 290a 2020 2020 2020 2020 7265 7475  -1).        retu
-000129a0: 726e 2063 6865 636b 5f70 6172 616d 6574  rn check_paramet
-000129b0: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
-000129c0: 2030 2e35 202a 2028 6c6f 6774 6175 202b   0.5 * (logtau +
-000129d0: 206c 6f67 6465 7420 2d20 6c6f 6771 7561   logdet - logqua
-000129e0: 6429 2c0a 2020 2020 2020 2020 2020 2020  d),.            
-000129f0: 2d31 203c 3d20 616c 7068 612c 0a20 2020  -1 <= alpha,.   
-00012a00: 2020 2020 2020 2020 2061 6c70 6861 203c           alpha <
-00012a10: 3d20 312c 0a20 2020 2020 2020 2020 2020  = 1,.           
-00012a20: 2074 6175 203e 2030 2c0a 2020 2020 2020   tau > 0,.      
-00012a30: 2020 2020 2020 6d73 673d 222d 3120 3c3d        msg="-1 <=
-00012a40: 2061 6c70 6861 203c 3d20 312c 2074 6175   alpha <= 1, tau
-00012a50: 203e 2030 222c 0a20 2020 2020 2020 2029   > 0",.        )
-00012a60: 0a0a 0a63 6c61 7373 2053 7469 636b 4272  ...class StickBr
-00012a70: 6561 6b69 6e67 5765 6967 6874 7352 5628  eakingWeightsRV(
-00012a80: 5261 6e64 6f6d 5661 7269 6162 6c65 293a  RandomVariable):
-00012a90: 0a20 2020 206e 616d 6520 3d20 2273 7469  .    name = "sti
-00012aa0: 636b 5f62 7265 616b 696e 675f 7765 6967  ck_breaking_weig
-00012ab0: 6874 7322 0a20 2020 206e 6469 6d5f 7375  hts".    ndim_su
-00012ac0: 7070 203d 2031 0a20 2020 206e 6469 6d73  pp = 1.    ndims
-00012ad0: 5f70 6172 616d 7320 3d20 5b30 2c20 305d  _params = [0, 0]
-00012ae0: 0a20 2020 2064 7479 7065 203d 2022 666c  .    dtype = "fl
-00012af0: 6f61 7458 220a 2020 2020 5f70 7269 6e74  oatX".    _print
-00012b00: 5f6e 616d 6520 3d20 2822 5374 6963 6b42  _name = ("StickB
-00012b10: 7265 616b 696e 6757 6569 6768 7473 222c  reakingWeights",
-00012b20: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-00012b30: 7b53 7469 636b 4272 6561 6b69 6e67 5765  {StickBreakingWe
-00012b40: 6967 6874 737d 2229 0a0a 2020 2020 6465  ights}")..    de
-00012b50: 6620 6d61 6b65 5f6e 6f64 6528 7365 6c66  f make_node(self
-00012b60: 2c20 726e 672c 2073 697a 652c 2064 7479  , rng, size, dty
-00012b70: 7065 2c20 616c 7068 612c 204b 293a 0a20  pe, alpha, K):. 
-00012b80: 2020 2020 2020 2061 6c70 6861 203d 2070         alpha = p
-00012b90: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
-00012ba0: 6162 6c65 2861 6c70 6861 290a 2020 2020  able(alpha).    
-00012bb0: 2020 2020 4b20 3d20 7074 2e61 735f 7465      K = pt.as_te
-00012bc0: 6e73 6f72 5f76 6172 6961 626c 6528 696e  nsor_variable(in
-00012bd0: 7458 284b 2929 0a0a 2020 2020 2020 2020  tX(K))..        
-00012be0: 6966 204b 2e6e 6469 6d20 3e20 303a 0a20  if K.ndim > 0:. 
-00012bf0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00012c00: 2056 616c 7565 4572 726f 7228 224b 206d   ValueError("K m
-00012c10: 7573 7420 6265 2061 2073 6361 6c61 722e  ust be a scalar.
-00012c20: 2229 0a0a 2020 2020 2020 2020 7265 7475  ")..        retu
-00012c30: 726e 2073 7570 6572 2829 2e6d 616b 655f  rn super().make_
-00012c40: 6e6f 6465 2872 6e67 2c20 7369 7a65 2c20  node(rng, size, 
-00012c50: 6474 7970 652c 2061 6c70 6861 2c20 4b29  dtype, alpha, K)
-00012c60: 0a0a 2020 2020 6465 6620 5f73 7570 705f  ..    def _supp_
-00012c70: 7368 6170 655f 6672 6f6d 5f70 6172 616d  shape_from_param
-00012c80: 7328 7365 6c66 2c20 6469 7374 5f70 6172  s(self, dist_par
-00012c90: 616d 732c 202a 2a6b 7761 7267 7329 3a0a  ams, **kwargs):.
-00012ca0: 2020 2020 2020 2020 4b20 3d20 6469 7374          K = dist
-00012cb0: 5f70 6172 616d 735b 315d 0a20 2020 2020  _params[1].     
-00012cc0: 2020 2072 6574 7572 6e20 284b 202b 2031     return (K + 1
-00012cd0: 2c29 0a0a 2020 2020 4063 6c61 7373 6d65  ,)..    @classme
-00012ce0: 7468 6f64 0a20 2020 2064 6566 2072 6e67  thod.    def rng
-00012cf0: 5f66 6e28 636c 732c 2072 6e67 2c20 616c  _fn(cls, rng, al
-00012d00: 7068 612c 204b 2c20 7369 7a65 293a 0a20  pha, K, size):. 
-00012d10: 2020 2020 2020 2069 6620 4b20 3c20 303a         if K < 0:
-00012d20: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00012d30: 7365 2056 616c 7565 4572 726f 7228 224b  se ValueError("K
-00012d40: 206e 6565 6473 2074 6f20 6265 2070 6f73   needs to be pos
-00012d50: 6974 6976 652e 2229 0a0a 2020 2020 2020  itive.")..      
-00012d60: 2020 7369 7a65 203d 2074 6f5f 7475 706c    size = to_tupl
-00012d70: 6528 7369 7a65 2920 6966 2073 697a 6520  e(size) if size 
-00012d80: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-00012d90: 2061 6c70 6861 2e73 6861 7065 0a20 2020   alpha.shape.   
-00012da0: 2020 2020 2073 697a 6520 3d20 7369 7a65       size = size
-00012db0: 202b 2028 4b2c 290a 2020 2020 2020 2020   + (K,).        
-00012dc0: 616c 7068 6120 3d20 616c 7068 615b 2e2e  alpha = alpha[..
-00012dd0: 2e2c 206e 702e 6e65 7761 7869 735d 0a0a  ., np.newaxis]..
-00012de0: 2020 2020 2020 2020 6265 7461 7320 3d20          betas = 
-00012df0: 726e 672e 6265 7461 2831 2c20 616c 7068  rng.beta(1, alph
-00012e00: 612c 2073 697a 653d 7369 7a65 290a 0a20  a, size=size).. 
-00012e10: 2020 2020 2020 2073 7469 636b 7320 3d20         sticks = 
-00012e20: 6e70 2e63 6f6e 6361 7465 6e61 7465 280a  np.concatenate(.
-00012e30: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-00012e40: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-00012e50: 2e6f 6e65 7328 7368 6170 653d 2873 697a  .ones(shape=(siz
-00012e60: 655b 3a2d 315d 202b 2028 312c 2929 292c  e[:-1] + (1,))),
-00012e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012e80: 206e 702e 6375 6d70 726f 6428 3120 2d20   np.cumprod(1 - 
-00012e90: 6265 7461 735b 2e2e 2e2c 203a 2d31 5d2c  betas[..., :-1],
-00012ea0: 2061 7869 733d 2d31 292c 0a20 2020 2020   axis=-1),.     
-00012eb0: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
-00012ec0: 2020 2020 2020 6178 6973 3d2d 312c 0a20        axis=-1,. 
-00012ed0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-00012ee0: 2020 7765 6967 6874 7320 3d20 7374 6963    weights = stic
-00012ef0: 6b73 202a 2062 6574 6173 0a20 2020 2020  ks * betas.     
-00012f00: 2020 2077 6569 6768 7473 203d 206e 702e     weights = np.
-00012f10: 636f 6e63 6174 656e 6174 6528 0a20 2020  concatenate(.   
-00012f20: 2020 2020 2020 2020 2028 7765 6967 6874           (weight
-00012f30: 732c 2031 202d 2077 6569 6768 7473 2e73  s, 1 - weights.s
-00012f40: 756d 2861 7869 733d 2d31 295b 2e2e 2e2c  um(axis=-1)[...,
-00012f50: 206e 702e 6e65 7761 7869 735d 292c 0a20   np.newaxis]),. 
-00012f60: 2020 2020 2020 2020 2020 2061 7869 733d             axis=
-00012f70: 2d31 2c0a 2020 2020 2020 2020 290a 0a20  -1,.        ).. 
-00012f80: 2020 2020 2020 2072 6574 7572 6e20 7765         return we
-00012f90: 6967 6874 730a 0a0a 7374 6963 6b62 7265  ights...stickbre
-00012fa0: 616b 696e 6777 6569 6768 7473 203d 2053  akingweights = S
-00012fb0: 7469 636b 4272 6561 6b69 6e67 5765 6967  tickBreakingWeig
-00012fc0: 6874 7352 5628 290a 0a0a 636c 6173 7320  htsRV()...class 
-00012fd0: 5374 6963 6b42 7265 616b 696e 6757 6569  StickBreakingWei
-00012fe0: 6768 7473 2853 696d 706c 6578 436f 6e74  ghts(SimplexCont
-00012ff0: 696e 756f 7573 293a 0a20 2020 2072 2222  inuous):.    r""
-00013000: 220a 2020 2020 4c69 6b65 6c69 686f 6f64  ".    Likelihood
-00013010: 206f 6620 7472 756e 6361 7465 6420 7374   of truncated st
-00013020: 6963 6b2d 6272 6561 6b69 6e67 2077 6569  ick-breaking wei
-00013030: 6768 7473 2e20 5468 6520 7765 6967 6874  ghts. The weight
-00013040: 7320 6172 6520 6765 6e65 7261 7465 6420  s are generated 
-00013050: 6672 6f6d 2061 0a20 2020 2073 7469 636b  from a.    stick
-00013060: 2d62 7265 616b 696e 6720 7072 6f63 6564  -breaking proced
-00013070: 7563 6520 7768 6572 6520 3a6d 6174 683a  uce where :math:
-00013080: 6078 5f6b 203d 2076 5f6b 205c 7072 6f64  `x_k = v_k \prod
-00013090: 5f7b 5c65 6c6c 203c 206b 7d20 2831 202d  _{\ell < k} (1 -
-000130a0: 2076 5f5c 656c 6c29 6020 666f 720a 2020   v_\ell)` for.  
-000130b0: 2020 3a6d 6174 683a 606b 205c 696e 205c    :math:`k \in \
-000130c0: 7b31 2c20 5c6c 646f 7473 2c20 4b5c 7d60  {1, \ldots, K\}`
-000130d0: 2061 6e64 203a 6d61 7468 3a60 785f 4b20   and :math:`x_K 
-000130e0: 3d20 5c70 726f 645f 7b5c 656c 6c20 3d20  = \prod_{\ell = 
-000130f0: 317d 5e7b 4b7d 2028 3120 2d20 765f 5c65  1}^{K} (1 - v_\e
-00013100: 6c6c 2920 3d20 3120 2d20 5c73 756d 5f7b  ll) = 1 - \sum_{
-00013110: 5c65 6c6c 3d31 7d5e 4b20 785f 5c65 6c6c  \ell=1}^K x_\ell
-00013120: 600a 2020 2020 7769 7468 203a 6d61 7468  `.    with :math
-00013130: 3a60 765f 6b20 5c73 7461 636b 7265 6c7b  :`v_k \stackrel{
-00013140: 5c74 6578 747b 692e 692e 642e 7d7d 7b5c  \text{i.i.d.}}{\
-00013150: 7369 6d7d 205c 7465 7874 7b42 6574 617d  sim} \text{Beta}
-00013160: 2831 2c20 5c61 6c70 6861 2960 2e0a 0a20  (1, \alpha)`... 
-00013170: 2020 202e 2e20 6d61 7468 3a0a 0a20 2020     .. math:..   
-00013180: 2020 2020 2066 285c 6d61 7468 6266 7b78       f(\mathbf{x
-00013190: 7d7c 5c61 6c70 6861 2c20 4b29 203d 0a20  }|\alpha, K) =. 
-000131a0: 2020 2020 2020 2020 2020 2042 2831 2c20             B(1, 
-000131b0: 5c61 6c70 6861 295e 7b2d 4b7d 785f 7b4b  \alpha)^{-K}x_{K
-000131c0: 2b31 7d5e 5c61 6c70 6861 205c 7072 6f64  +1}^\alpha \prod
-000131d0: 5f7b 6b3d 317d 5e7b 4b2b 317d 5c6c 6566  _{k=1}^{K+1}\lef
-000131e0: 745c 7b5c 7375 6d5f 7b6a 3d6b 7d5e 7b4b  t\{\sum_{j=k}^{K
-000131f0: 2b31 7d20 785f 6a5c 7269 6768 745c 7d5e  +1} x_j\right\}^
-00013200: 7b2d 317d 0a0a 2020 2020 3d3d 3d3d 3d3d  {-1}..    ======
-00013210: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
-00013220: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013230: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00013240: 3d3d 3d0a 2020 2020 5375 7070 6f72 7420  ===.    Support 
-00013250: 2020 3a6d 6174 683a 6078 5f6b 205c 696e    :math:`x_k \in
-00013260: 2028 302c 2031 2960 2066 6f72 203a 6d61   (0, 1)` for :ma
-00013270: 7468 3a60 6b20 5c69 6e20 5c7b 312c 205c  th:`k \in \{1, \
-00013280: 6c64 6f74 732c 204b 2b31 5c7d 600a 2020  ldots, K+1\}`.  
-00013290: 2020 2020 2020 2020 2020 2020 7375 6368              such
-000132a0: 2074 6861 7420 3a6d 6174 683a 605c 7375   that :math:`\su
-000132b0: 6d20 785f 6b20 3d20 3160 0a20 2020 204d  m x_k = 1`.    M
-000132c0: 6561 6e20 2020 2020 203a 6d61 7468 3a60  ean      :math:`
-000132d0: 5c6d 6174 6862 627b 457d 5b78 5f6b 5d20  \mathbb{E}[x_k] 
-000132e0: 3d20 5c64 6672 6163 7b31 7d7b 3120 2b20  = \dfrac{1}{1 + 
-000132f0: 5c61 6c70 6861 7d5c 6c65 6674 285c 6466  \alpha}\left(\df
-00013300: 7261 637b 5c61 6c70 6861 7d7b 3120 2b20  rac{\alpha}{1 + 
-00013310: 5c61 6c70 6861 7d5c 7269 6768 7429 5e7b  \alpha}\right)^{
-00013320: 6b20 2d20 317d 600a 2020 2020 2020 2020  k - 1}`.        
-00013330: 2020 2020 2020 666f 7220 3a6d 6174 683a        for :math:
-00013340: 606b 205c 696e 205c 7b31 2c20 5c6c 646f  `k \in \{1, \ldo
-00013350: 7473 2c20 4b5c 7d60 2061 6e64 203a 6d61  ts, K\}` and :ma
-00013360: 7468 3a60 5c6d 6174 6862 627b 457d 5b78  th:`\mathbb{E}[x
-00013370: 5f7b 4b2b 317d 5d20 3d20 5c6c 6566 7428  _{K+1}] = \left(
-00013380: 5c64 6672 6163 7b5c 616c 7068 617d 7b31  \dfrac{\alpha}{1
-00013390: 202b 205c 616c 7068 617d 5c72 6967 6874   + \alpha}\right
-000133a0: 295e 7b4b 7d60 0a20 2020 203d 3d3d 3d3d  )^{K}`.    =====
-000133b0: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 3d3d  ===  ===========
-000133c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000133d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000133e0: 3d3d 3d3d 0a0a 2020 2020 5061 7261 6d65  ====..    Parame
-000133f0: 7465 7273 0a20 2020 202d 2d2d 2d2d 2d2d  ters.    -------
-00013400: 2d2d 2d0a 2020 2020 616c 7068 6120 3a20  ---.    alpha : 
-00013410: 7465 6e73 6f72 5f6c 696b 6520 6f66 2066  tensor_like of f
-00013420: 6c6f 6174 0a20 2020 2020 2020 2043 6f6e  loat.        Con
-00013430: 6365 6e74 7261 7469 6f6e 2070 6172 616d  centration param
-00013440: 6574 6572 2028 616c 7068 6120 3e20 3029  eter (alpha > 0)
-00013450: 2e0a 2020 2020 4b20 3a20 7465 6e73 6f72  ..    K : tensor
-00013460: 5f6c 696b 6520 6f66 2069 6e74 0a20 2020  _like of int.   
-00013470: 2020 2020 2054 6865 206e 756d 6265 7220       The number 
-00013480: 6f66 2022 7374 6963 6b73 2220 746f 2062  of "sticks" to b
-00013490: 7265 616b 206f 6666 2066 726f 6d20 616e  reak off from an
-000134a0: 2069 6e69 7469 616c 206f 6e65 2d75 6e69   initial one-uni
-000134b0: 7420 7374 6963 6b2e 2054 6865 206c 656e  t stick. The len
-000134c0: 6774 6820 6f66 2074 6865 2077 6569 6768  gth of the weigh
-000134d0: 740a 2020 2020 2020 2020 7665 6374 6f72  t.        vector
-000134e0: 2069 7320 4b20 2b20 312c 2077 6865 7265   is K + 1, where
-000134f0: 2074 6865 206c 6173 7420 7765 6967 6874   the last weight
-00013500: 2069 7320 6f6e 6520 6d69 6e75 7320 7468   is one minus th
-00013510: 6520 7375 6d20 6f66 2061 6c6c 2074 6865  e sum of all the
-00013520: 2066 6972 7374 2073 7469 636b 732e 0a0a   first sticks...
-00013530: 2020 2020 5265 6665 7265 6e63 6573 0a20      References. 
-00013540: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00013550: 2020 2e2e 205b 315d 2049 7368 7761 7261    .. [1] Ishwara
-00013560: 6e2c 2048 2e2c 2026 204a 616d 6573 2c20  n, H., & James, 
-00013570: 4c2e 2046 2e20 2832 3030 3129 2e20 4769  L. F. (2001). Gi
-00013580: 6262 7320 7361 6d70 6c69 6e67 206d 6574  bbs sampling met
-00013590: 686f 6473 2066 6f72 2073 7469 636b 2d62  hods for stick-b
-000135a0: 7265 616b 696e 6720 7072 696f 7273 2e0a  reaking priors..
-000135b0: 2020 2020 2020 2020 2020 204a 6f75 726e             Journ
-000135c0: 616c 206f 6620 7468 6520 416d 6572 6963  al of the Americ
-000135d0: 616e 2053 7461 7469 7374 6963 616c 2041  an Statistical A
-000135e0: 7373 6f63 6961 7469 6f6e 2c20 3936 2834  ssociation, 96(4
-000135f0: 3533 292c 2031 3631 2d31 3733 2e0a 0a20  53), 161-173... 
-00013600: 2020 202e 2e20 5b32 5d20 4dc3 bc6c 6c65     .. [2] M..lle
-00013610: 722c 2050 2e2c 2051 7569 6e74 616e 612c  r, P., Quintana,
-00013620: 2046 2e20 412e 2c20 4a61 7261 2c20 412e   F. A., Jara, A.
-00013630: 2c20 2620 4861 6e73 6f6e 2c20 542e 2028  , & Hanson, T. (
-00013640: 3230 3135 292e 2042 6179 6573 6961 6e20  2015). Bayesian 
-00013650: 6e6f 6e70 6172 616d 6574 7269 6320 6461  nonparametric da
-00013660: 7461 0a20 2020 2020 2020 2020 2020 616e  ta.           an
-00013670: 616c 7973 6973 2e20 4e65 7720 596f 726b  alysis. New York
-00013680: 3a20 5370 7269 6e67 6572 2e0a 2020 2020  : Springer..    
-00013690: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
-000136a0: 7374 6963 6b62 7265 616b 696e 6777 6569  stickbreakingwei
-000136b0: 6768 7473 0a0a 2020 2020 4063 6c61 7373  ghts..    @class
-000136c0: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-000136d0: 6973 7428 636c 732c 2061 6c70 6861 2c20  ist(cls, alpha, 
-000136e0: 4b2c 202a 6172 6773 2c20 2a2a 6b77 6172  K, *args, **kwar
-000136f0: 6773 293a 0a20 2020 2020 2020 2061 6c70  gs):.        alp
-00013700: 6861 203d 2070 742e 6173 5f74 656e 736f  ha = pt.as_tenso
-00013710: 725f 7661 7269 6162 6c65 2866 6c6f 6174  r_variable(float
-00013720: 5828 616c 7068 6129 290a 2020 2020 2020  X(alpha)).      
-00013730: 2020 4b20 3d20 7074 2e61 735f 7465 6e73    K = pt.as_tens
-00013740: 6f72 5f76 6172 6961 626c 6528 696e 7458  or_variable(intX
-00013750: 284b 2929 0a0a 2020 2020 2020 2020 7265  (K))..        re
-00013760: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
-00013770: 7428 5b61 6c70 6861 2c20 4b5d 2c20 2a2a  t([alpha, K], **
-00013780: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-00013790: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
-000137a0: 2c20 616c 7068 612c 204b 293a 0a20 2020  , alpha, K):.   
-000137b0: 2020 2020 2061 6c70 6861 203d 2061 6c70       alpha = alp
-000137c0: 6861 5b2e 2e2e 2c20 6e70 2e6e 6577 6178  ha[..., np.newax
-000137d0: 6973 5d0a 2020 2020 2020 2020 6d6f 6d65  is].        mome
-000137e0: 6e74 203d 2028 616c 7068 6120 2f20 2831  nt = (alpha / (1
-000137f0: 202b 2061 6c70 6861 2929 202a 2a20 7074   + alpha)) ** pt
-00013800: 2e61 7261 6e67 6528 4b29 0a20 2020 2020  .arange(K).     
-00013810: 2020 206d 6f6d 656e 7420 2a3d 2031 202f     moment *= 1 /
-00013820: 2028 3120 2b20 616c 7068 6129 0a20 2020   (1 + alpha).   
-00013830: 2020 2020 206d 6f6d 656e 7420 3d20 7074       moment = pt
-00013840: 2e63 6f6e 6361 7465 6e61 7465 285b 6d6f  .concatenate([mo
-00013850: 6d65 6e74 2c20 2861 6c70 6861 202f 2028  ment, (alpha / (
-00013860: 3120 2b20 616c 7068 6129 2920 2a2a 204b  1 + alpha)) ** K
-00013870: 5d2c 2061 7869 733d 2d31 290a 2020 2020  ], axis=-1).    
-00013880: 2020 2020 6966 206e 6f74 2072 765f 7369      if not rv_si
-00013890: 7a65 5f69 735f 6e6f 6e65 2873 697a 6529  ze_is_none(size)
-000138a0: 3a0a 2020 2020 2020 2020 2020 2020 6d6f  :.            mo
-000138b0: 6d65 6e74 5f73 697a 6520 3d20 7074 2e63  ment_size = pt.c
-000138c0: 6f6e 6361 7465 6e61 7465 280a 2020 2020  oncatenate(.    
-000138d0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
-000138e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000138f0: 2020 7369 7a65 2c0a 2020 2020 2020 2020    size,.        
-00013900: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
-00013910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013920: 2020 2020 2020 4b20 2b20 312c 0a20 2020        K + 1,.   
-00013930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013940: 205d 2c0a 2020 2020 2020 2020 2020 2020   ],.            
-00013950: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
-00013960: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00013970: 6d6f 6d65 6e74 203d 2070 742e 6675 6c6c  moment = pt.full
-00013980: 286d 6f6d 656e 745f 7369 7a65 2c20 6d6f  (moment_size, mo
-00013990: 6d65 6e74 290a 0a20 2020 2020 2020 2072  ment)..        r
-000139a0: 6574 7572 6e20 6d6f 6d65 6e74 0a0a 2020  eturn moment..  
-000139b0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
-000139c0: 2c20 616c 7068 612c 204b 293a 0a20 2020  , alpha, K):.   
-000139d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000139e0: 2043 616c 6375 6c61 7465 206c 6f67 2d70   Calculate log-p
-000139f0: 726f 6261 6269 6c69 7479 206f 6620 7468  robability of th
-00013a00: 6520 6469 7374 7269 6275 7469 6f6e 2069  e distribution i
-00013a10: 6e64 7563 6564 2066 726f 6d20 7468 6520  nduced from the 
-00013a20: 7374 6963 6b2d 6272 6561 6b69 6e67 2070  stick-breaking p
-00013a30: 726f 6365 7373 0a20 2020 2020 2020 2061  rocess.        a
-00013a40: 7420 7370 6563 6966 6965 6420 7661 6c75  t specified valu
-00013a50: 652e 0a0a 2020 2020 2020 2020 5061 7261  e...        Para
-00013a60: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-00013a70: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00013a80: 2020 7661 6c75 653a 206e 756d 6572 6963    value: numeric
-00013a90: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-00013aa0: 7565 2066 6f72 2077 6869 6368 206c 6f67  ue for which log
-00013ab0: 2d70 726f 6261 6269 6c69 7479 2069 7320  -probability is 
-00013ac0: 6361 6c63 756c 6174 6564 2e0a 0a20 2020  calculated...   
-00013ad0: 2020 2020 2052 6574 7572 6e73 0a20 2020       Returns.   
-00013ae0: 2020 2020 202d 2d2d 2d2d 2d2d 0a20 2020       -------.   
-00013af0: 2020 2020 2054 656e 736f 7256 6172 6961       TensorVaria
-00013b00: 626c 650a 2020 2020 2020 2020 2222 220a  ble.        """.
-00013b10: 2020 2020 2020 2020 6c6f 6770 203d 202d          logp = -
-00013b20: 7074 2e73 756d 280a 2020 2020 2020 2020  pt.sum(.        
-00013b30: 2020 2020 7074 2e6c 6f67 280a 2020 2020      pt.log(.    
-00013b40: 2020 2020 2020 2020 2020 2020 7074 2e63              pt.c
-00013b50: 756d 7375 6d28 0a20 2020 2020 2020 2020  umsum(.         
-00013b60: 2020 2020 2020 2020 2020 2076 616c 7565             value
-00013b70: 5b2e 2e2e 2c20 3a3a 2d31 5d2c 0a20 2020  [..., ::-1],.   
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b90: 2061 7869 733d 2d31 2c0a 2020 2020 2020   axis=-1,.      
-00013ba0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00013bb0: 2020 2020 2020 2020 292c 0a20 2020 2020          ),.     
-00013bc0: 2020 2020 2020 2061 7869 733d 2d31 2c0a         axis=-1,.
-00013bd0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-00013be0: 2020 6c6f 6770 202b 3d20 2d4b 202a 2062    logp += -K * b
-00013bf0: 6574 616c 6e28 312c 2061 6c70 6861 290a  etaln(1, alpha).
-00013c00: 2020 2020 2020 2020 6c6f 6770 202b 3d20          logp += 
-00013c10: 616c 7068 6120 2a20 7074 2e6c 6f67 2876  alpha * pt.log(v
-00013c20: 616c 7565 5b2e 2e2e 2c20 2d31 5d29 0a0a  alue[..., -1])..
-00013c30: 2020 2020 2020 2020 6c6f 6770 203d 2070          logp = p
-00013c40: 742e 7377 6974 6368 280a 2020 2020 2020  t.switch(.      
-00013c50: 2020 2020 2020 7074 2e6f 725f 280a 2020        pt.or_(.  
-00013c60: 2020 2020 2020 2020 2020 2020 2020 7074                pt
-00013c70: 2e61 6e79 280a 2020 2020 2020 2020 2020  .any(.          
-00013c80: 2020 2020 2020 2020 2020 7074 2e61 6e64            pt.and
-00013c90: 5f28 7074 2e6c 6528 7661 6c75 652c 2030  _(pt.le(value, 0
-00013ca0: 292c 2070 742e 6765 2876 616c 7565 2c20  ), pt.ge(value, 
-00013cb0: 3129 292c 0a20 2020 2020 2020 2020 2020  1)),.           
-00013cc0: 2020 2020 2020 2020 2061 7869 733d 2d31           axis=-1
-00013cd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00013ce0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
-00013cf0: 2020 2020 2070 742e 6f72 5f28 0a20 2020       pt.or_(.   
-00013d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d10: 2070 742e 6269 7477 6973 655f 6e6f 7428   pt.bitwise_not(
-00013d20: 7074 2e61 6c6c 636c 6f73 6528 7661 6c75  pt.allclose(valu
-00013d30: 652e 7375 6d28 2d31 292c 2031 2929 2c0a  e.sum(-1), 1)),.
-00013d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d50: 2020 2020 7074 2e6e 6571 2876 616c 7565      pt.neq(value
-00013d60: 2e73 6861 7065 5b2d 315d 2c20 4b20 2b20  .shape[-1], K + 
-00013d70: 3129 2c0a 2020 2020 2020 2020 2020 2020  1),.            
-00013d80: 2020 2020 292c 0a20 2020 2020 2020 2020      ),.         
-00013d90: 2020 2029 2c0a 2020 2020 2020 2020 2020     ),.          
-00013da0: 2020 2d6e 702e 696e 662c 0a20 2020 2020    -np.inf,.     
-00013db0: 2020 2020 2020 206c 6f67 702c 0a20 2020         logp,.   
-00013dc0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-00013dd0: 7265 7475 726e 2063 6865 636b 5f70 6172  return check_par
-00013de0: 616d 6574 6572 7328 0a20 2020 2020 2020  ameters(.       
-00013df0: 2020 2020 206c 6f67 702c 0a20 2020 2020       logp,.     
-00013e00: 2020 2020 2020 2061 6c70 6861 203e 2030         alpha > 0
-00013e10: 2c0a 2020 2020 2020 2020 2020 2020 4b20  ,.            K 
-00013e20: 3e20 302c 0a20 2020 2020 2020 2020 2020  > 0,.           
-00013e30: 206d 7367 3d22 616c 7068 6120 3e20 302c   msg="alpha > 0,
-00013e40: 204b 203e 2030 222c 0a20 2020 2020 2020   K > 0",.       
-00013e50: 2029 0a0a 0a63 6c61 7373 205a 6572 6f53   )...class ZeroS
-00013e60: 756d 4e6f 726d 616c 5256 2853 796d 626f  umNormalRV(Symbo
-00013e70: 6c69 6352 616e 646f 6d56 6172 6961 626c  licRandomVariabl
-00013e80: 6529 3a0a 2020 2020 2222 225a 6572 6f53  e):.    """ZeroS
-00013e90: 756d 4e6f 726d 616c 2072 616e 646f 6d20  umNormal random 
-00013ea0: 7661 7269 6162 6c65 2222 220a 0a20 2020  variable"""..   
-00013eb0: 205f 7072 696e 745f 6e61 6d65 203d 2028   _print_name = (
-00013ec0: 225a 6572 6f53 756d 4e6f 726d 616c 222c  "ZeroSumNormal",
-00013ed0: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
-00013ee0: 7b5a 6572 6f53 756d 4e6f 726d 616c 7d22  {ZeroSumNormal}"
-00013ef0: 290a 2020 2020 6465 6661 756c 745f 6f75  ).    default_ou
-00013f00: 7470 7574 203d 2030 0a0a 0a63 6c61 7373  tput = 0...class
-00013f10: 205a 6572 6f53 756d 4e6f 726d 616c 2844   ZeroSumNormal(D
-00013f20: 6973 7472 6962 7574 696f 6e29 3a0a 2020  istribution):.  
-00013f30: 2020 7222 2222 0a20 2020 205a 6572 6f53    r""".    ZeroS
-00013f40: 756d 4e6f 726d 616c 2064 6973 7472 6962  umNormal distrib
-00013f50: 7574 696f 6e2c 2069 2e65 204e 6f72 6d61  ution, i.e Norma
-00013f60: 6c20 6469 7374 7269 6275 7469 6f6e 2077  l distribution w
-00013f70: 6865 7265 206f 6e65 206f 720a 2020 2020  here one or.    
-00013f80: 7365 7665 7261 6c20 6178 6573 2061 7265  several axes are
-00013f90: 2063 6f6e 7374 7261 696e 6564 2074 6f20   constrained to 
-00013fa0: 7375 6d20 746f 207a 6572 6f2e 0a20 2020  sum to zero..   
-00013fb0: 2042 7920 6465 6661 756c 742c 2074 6865   By default, the
-00013fc0: 206c 6173 7420 6178 6973 2069 7320 636f   last axis is co
-00013fd0: 6e73 7472 6169 6e65 6420 746f 2073 756d  nstrained to sum
-00013fe0: 2074 6f20 7a65 726f 2e0a 2020 2020 5365   to zero..    Se
-00013ff0: 6520 606e 5f7a 6572 6f73 756d 5f61 7865  e `n_zerosum_axe
-00014000: 7360 206b 7761 7267 2066 6f72 206d 6f72  s` kwarg for mor
-00014010: 6520 6465 7461 696c 732e 0a0a 2020 2020  e details...    
-00014020: 2e2e 206d 6174 683a 3a0a 0a20 2020 2020  .. math::..     
-00014030: 2020 205c 6265 6769 6e7b 616c 6967 6e2a     \begin{align*
-00014040: 7d0a 2020 2020 2020 2020 2020 2020 5a53  }.            ZS
-00014050: 4e28 5c73 6967 6d61 2920 3d20 4e20 5c42  N(\sigma) = N \B
-00014060: 6967 2820 302c 205c 7369 676d 615e 3220  ig( 0, \sigma^2 
-00014070: 2849 202d 205c 7466 7261 637b 317d 7b6e  (I - \tfrac{1}{n
-00014080: 7d4a 2920 5c42 6967 2920 5c5c 0a20 2020  }J) \Big) \\.   
-00014090: 2020 2020 2020 2020 205c 7465 7874 7b77           \text{w
-000140a0: 6865 7265 7d20 5c20 7e20 4a5f 7b69 6a7d  here} \ ~ J_{ij}
-000140b0: 203d 2031 205c 207e 205c 7465 7874 7b61   = 1 \ ~ \text{a
-000140c0: 6e64 7d20 5c5c 0a20 2020 2020 2020 2020  nd} \\.         
-000140d0: 2020 206e 203d 205c 7465 7874 7b6e 6272     n = \text{nbr
-000140e0: 206f 6620 7a65 726f 2d73 756d 2061 7865   of zero-sum axe
-000140f0: 737d 0a20 2020 2020 2020 205c 656e 647b  s}.        \end{
-00014100: 616c 6967 6e2a 7d0a 0a20 2020 2050 6172  align*}..    Par
-00014110: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
-00014120: 2d2d 2d2d 2d2d 0a20 2020 2073 6967 6d61  ------.    sigma
-00014130: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
-00014140: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
-00014150: 5363 616c 6520 7061 7261 6d65 7465 7220  Scale parameter 
-00014160: 2873 6967 6d61 203e 2030 292e 0a20 2020  (sigma > 0)..   
-00014170: 2020 2020 2049 7427 7320 6163 7475 616c       It's actual
-00014180: 6c79 2074 6865 2073 7461 6e64 6172 6420  ly the standard 
-00014190: 6465 7669 6174 696f 6e20 6f66 2074 6865  deviation of the
-000141a0: 2075 6e64 6572 6c79 696e 672c 2075 6e63   underlying, unc
-000141b0: 6f6e 7374 7261 696e 6564 204e 6f72 6d61  onstrained Norma
-000141c0: 6c20 6469 7374 7269 6275 7469 6f6e 2e0a  l distribution..
-000141d0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-000141e0: 2074 6f20 3120 6966 206e 6f74 2073 7065   to 1 if not spe
-000141f0: 6369 6669 6564 2e0a 2020 2020 2020 2020  cified..        
-00014200: 466f 7220 6e6f 772c 2060 6073 6967 6d61  For now, ``sigma
-00014210: 6060 2068 6173 2074 6f20 6265 2061 2073  `` has to be a s
-00014220: 6361 6c61 722c 2074 6f20 656e 7375 7265  calar, to ensure
-00014230: 2074 6865 207a 6572 6f2d 7375 6d20 636f   the zero-sum co
-00014240: 6e73 7472 6169 6e74 2e0a 2020 2020 6e5f  nstraint..    n_
-00014250: 7a65 726f 7375 6d5f 6178 6573 3a20 696e  zerosum_axes: in
-00014260: 742c 2064 6566 6175 6c74 7320 746f 2031  t, defaults to 1
-00014270: 0a20 2020 2020 2020 204e 756d 6265 7220  .        Number 
-00014280: 6f66 2061 7865 7320 616c 6f6e 6720 7768  of axes along wh
-00014290: 6963 6820 7468 6520 7a65 726f 2d73 756d  ich the zero-sum
-000142a0: 2063 6f6e 7374 7261 696e 7420 6973 2065   constraint is e
-000142b0: 6e66 6f72 6365 642c 2073 7461 7274 696e  nforced, startin
-000142c0: 6720 6672 6f6d 2074 6865 2072 6967 6874  g from the right
-000142d0: 6d6f 7374 2070 6f73 6974 696f 6e2e 0a20  most position.. 
-000142e0: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-000142f0: 746f 2031 2c20 692e 6520 7468 6520 7269  to 1, i.e the ri
-00014300: 6768 746d 6f73 7420 6178 6973 2e0a 2020  ghtmost axis..  
-00014310: 2020 7a65 726f 7375 6d5f 6178 6573 3a20    zerosum_axes: 
-00014320: 696e 742c 2064 6570 7265 6361 7465 6420  int, deprecated 
-00014330: 706c 6561 7365 2075 7365 206e 5f7a 6572  please use n_zer
-00014340: 6f73 756d 5f61 7865 7320 6173 2069 7473  osum_axes as its
-00014350: 2073 7563 6365 7373 6f72 0a20 2020 2064   successor.    d
-00014360: 696d 733a 2073 6571 7565 6e63 6520 6f66  ims: sequence of
-00014370: 2073 7472 696e 6773 2c20 6f70 7469 6f6e   strings, option
-00014380: 616c 0a20 2020 2020 2020 2044 696d 656e  al.        Dimen
-00014390: 7369 6f6e 206e 616d 6573 206f 6620 7468  sion names of th
-000143a0: 6520 6469 7374 7269 6275 7469 6f6e 2e20  e distribution. 
-000143b0: 576f 726b 7320 7468 6520 7361 6d65 2061  Works the same a
-000143c0: 7320 666f 7220 6f74 6865 7220 5079 4d43  s for other PyMC
-000143d0: 2064 6973 7472 6962 7574 696f 6e73 2e0a   distributions..
-000143e0: 2020 2020 2020 2020 4e65 6365 7373 6172          Necessar
-000143f0: 7920 6966 2060 6073 6861 7065 6060 2069  y if ``shape`` i
-00014400: 7320 6e6f 7420 7061 7373 6564 2e0a 2020  s not passed..  
-00014410: 2020 7368 6170 653a 2074 7570 6c65 206f    shape: tuple o
-00014420: 6620 696e 7465 6765 7273 2c20 6f70 7469  f integers, opti
-00014430: 6f6e 616c 0a20 2020 2020 2020 2053 6861  onal.        Sha
-00014440: 7065 206f 6620 7468 6520 6469 7374 7269  pe of the distri
-00014450: 6275 7469 6f6e 2e20 576f 726b 7320 7468  bution. Works th
-00014460: 6520 7361 6d65 2061 7320 666f 7220 6f74  e same as for ot
-00014470: 6865 7220 5079 4d43 2064 6973 7472 6962  her PyMC distrib
-00014480: 7574 696f 6e73 2e0a 2020 2020 2020 2020  utions..        
-00014490: 4e65 6365 7373 6172 7920 6966 2060 6064  Necessary if ``d
-000144a0: 696d 7360 6020 6f72 2060 606f 6273 6572  ims`` or ``obser
-000144b0: 7665 6460 6020 6973 206e 6f74 2070 6173  ved`` is not pas
-000144c0: 7365 642e 0a0a 2020 2020 5761 726e 696e  sed...    Warnin
-000144d0: 6773 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  gs.    --------.
-000144e0: 2020 2020 6060 7369 676d 6160 6020 6861      ``sigma`` ha
-000144f0: 7320 746f 2062 6520 6120 7363 616c 6172  s to be a scalar
-00014500: 2c20 746f 2065 6e73 7572 6520 7468 6520  , to ensure the 
-00014510: 7a65 726f 2d73 756d 2063 6f6e 7374 7261  zero-sum constra
-00014520: 696e 742e 0a20 2020 2054 6865 2061 6269  int..    The abi
-00014530: 6c69 7479 2074 6f20 7370 6563 6966 7920  lity to specify 
-00014540: 6120 7665 6374 6f72 206f 6620 6060 7369  a vector of ``si
-00014550: 676d 6160 6020 6d61 7920 6265 2061 6464  gma`` may be add
-00014560: 6564 2069 6e20 6675 7475 7265 2076 6572  ed in future ver
-00014570: 7369 6f6e 732e 0a0a 2020 2020 6060 6e5f  sions...    ``n_
-00014580: 7a65 726f 7375 6d5f 6178 6573 6060 2068  zerosum_axes`` h
-00014590: 6173 2074 6f20 6265 203e 2030 2e20 4966  as to be > 0. If
-000145a0: 2079 6f75 2077 616e 7420 7468 6520 6265   you want the be
-000145b0: 6861 7669 6f72 206f 6620 6060 6e5f 7a65  havior of ``n_ze
-000145c0: 726f 7375 6d5f 6178 6573 203d 2030 6060  rosum_axes = 0``
-000145d0: 2c0a 2020 2020 6a75 7374 2075 7365 2060  ,.    just use `
-000145e0: 6070 6d2e 4e6f 726d 616c 6060 2e0a 0a20  `pm.Normal``... 
-000145f0: 2020 2045 7861 6d70 6c65 730a 2020 2020     Examples.    
-00014600: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044 6566  --------.    Def
-00014610: 696e 6520 6120 605a 6572 6f53 756d 4e6f  ine a `ZeroSumNo
-00014620: 726d 616c 6020 7661 7269 6162 6c65 2c20  rmal` variable, 
-00014630: 7769 7468 2060 7369 676d 613d 3160 2061  with `sigma=1` a
-00014640: 6e64 0a20 2020 2060 6e5f 7a65 726f 7375  nd.    `n_zerosu
-00014650: 6d5f 6178 6573 3d31 6020 2062 7920 6465  m_axes=1`  by de
-00014660: 6661 756c 743a 3a0a 0a20 2020 2020 2020  fault::..       
-00014670: 2043 4f4f 5244 5320 3d20 7b0a 2020 2020   COORDS = {.    
-00014680: 2020 2020 2020 2020 2272 6567 696f 6e73          "regions
-00014690: 223a 205b 2261 222c 2022 6222 2c20 2263  ": ["a", "b", "c
-000146a0: 225d 2c0a 2020 2020 2020 2020 2020 2020  "],.            
-000146b0: 2261 6e73 7765 7273 223a 205b 2279 6573  "answers": ["yes
-000146c0: 222c 2022 6e6f 222c 2022 7768 6174 6576  ", "no", "whatev
-000146d0: 6572 222c 2022 646f 6e27 7420 756e 6465  er", "don't unde
-000146e0: 7273 7461 6e64 2071 7565 7374 696f 6e22  rstand question"
-000146f0: 5d2c 0a20 2020 2020 2020 207d 0a20 2020  ],.        }.   
-00014700: 2020 2020 2077 6974 6820 706d 2e4d 6f64       with pm.Mod
-00014710: 656c 2863 6f6f 7264 733d 434f 4f52 4453  el(coords=COORDS
-00014720: 2920 6173 206d 3a0a 2020 2020 2020 2020  ) as m:.        
-00014730: 2020 2020 2320 7468 6520 7a65 726f 2073      # the zero s
-00014740: 756d 2061 7869 7320 7769 6c6c 2062 6520  um axis will be 
-00014750: 2761 6e73 7765 7273 270a 2020 2020 2020  'answers'.      
-00014760: 2020 2020 2020 7620 3d20 706d 2e5a 6572        v = pm.Zer
-00014770: 6f53 756d 4e6f 726d 616c 2822 7622 2c20  oSumNormal("v", 
-00014780: 6469 6d73 3d28 2272 6567 696f 6e73 222c  dims=("regions",
-00014790: 2022 616e 7377 6572 7322 2929 0a0a 2020   "answers"))..  
-000147a0: 2020 2020 2020 7769 7468 2070 6d2e 4d6f        with pm.Mo
-000147b0: 6465 6c28 636f 6f72 6473 3d43 4f4f 5244  del(coords=COORD
-000147c0: 5329 2061 7320 6d3a 0a20 2020 2020 2020  S) as m:.       
-000147d0: 2020 2020 2023 2074 6865 207a 6572 6f20       # the zero 
-000147e0: 7375 6d20 6178 6573 2077 696c 6c20 6265  sum axes will be
-000147f0: 2027 616e 7377 6572 7327 2061 6e64 2027   'answers' and '
-00014800: 7265 6769 6f6e 7327 0a20 2020 2020 2020  regions'.       
-00014810: 2020 2020 2076 203d 2070 6d2e 5a65 726f       v = pm.Zero
-00014820: 5375 6d4e 6f72 6d61 6c28 2276 222c 2064  SumNormal("v", d
-00014830: 696d 733d 2822 7265 6769 6f6e 7322 2c20  ims=("regions", 
-00014840: 2261 6e73 7765 7273 2229 2c20 6e5f 7a65  "answers"), n_ze
-00014850: 726f 7375 6d5f 6178 6573 3d32 290a 0a20  rosum_axes=2).. 
-00014860: 2020 2020 2020 2077 6974 6820 706d 2e4d         with pm.M
-00014870: 6f64 656c 2863 6f6f 7264 733d 434f 4f52  odel(coords=COOR
-00014880: 4453 2920 6173 206d 3a0a 2020 2020 2020  DS) as m:.      
-00014890: 2020 2020 2020 2320 7468 6520 7a65 726f        # the zero
-000148a0: 2073 756d 2061 7865 7320 7769 6c6c 2062   sum axes will b
-000148b0: 6520 7468 6520 6c61 7374 2074 776f 0a20  e the last two. 
-000148c0: 2020 2020 2020 2020 2020 2076 203d 2070             v = p
-000148d0: 6d2e 5a65 726f 5375 6d4e 6f72 6d61 6c28  m.ZeroSumNormal(
-000148e0: 2276 222c 2073 6861 7065 3d28 332c 2034  "v", shape=(3, 4
-000148f0: 2c20 3529 2c20 6e5f 7a65 726f 7375 6d5f  , 5), n_zerosum_
-00014900: 6178 6573 3d32 290a 2020 2020 2222 220a  axes=2).    """.
-00014910: 2020 2020 7276 5f74 7970 6520 3d20 5a65      rv_type = Ze
-00014920: 726f 5375 6d4e 6f72 6d61 6c52 560a 0a20  roSumNormalRV.. 
-00014930: 2020 2064 6566 205f 5f6e 6577 5f5f 280a     def __new__(.
-00014940: 2020 2020 2020 2020 636c 732c 202a 6172          cls, *ar
-00014950: 6773 2c20 7a65 726f 7375 6d5f 6178 6573  gs, zerosum_axes
-00014960: 3d4e 6f6e 652c 206e 5f7a 6572 6f73 756d  =None, n_zerosum
-00014970: 5f61 7865 733d 4e6f 6e65 2c20 7375 7070  _axes=None, supp
-00014980: 6f72 745f 7368 6170 653d 4e6f 6e65 2c20  ort_shape=None, 
-00014990: 6469 6d73 3d4e 6f6e 652c 202a 2a6b 7761  dims=None, **kwa
-000149a0: 7267 730a 2020 2020 293a 0a20 2020 2020  rgs.    ):.     
-000149b0: 2020 2069 6620 7a65 726f 7375 6d5f 6178     if zerosum_ax
-000149c0: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
-000149d0: 2020 2020 2020 2020 2020 2020 6e5f 7a65              n_ze
-000149e0: 726f 7375 6d5f 6178 6573 203d 207a 6572  rosum_axes = zer
-000149f0: 6f73 756d 5f61 7865 730a 2020 2020 2020  osum_axes.      
-00014a00: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-00014a10: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-00014a20: 2020 2020 2022 5468 6520 277a 6572 6f73       "The 'zeros
-00014a30: 756d 5f61 7865 7327 2070 6172 616d 6574  um_axes' paramet
-00014a40: 6572 2069 7320 6465 7072 6563 6174 6564  er is deprecated
-00014a50: 2e20 5573 6520 276e 5f7a 6572 6f73 756d  . Use 'n_zerosum
-00014a60: 5f61 7865 7327 2069 6e73 7465 6164 2e22  _axes' instead."
-00014a70: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00014a80: 2020 4465 7072 6563 6174 696f 6e57 6172    DeprecationWar
-00014a90: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
-00014aa0: 2020 290a 2020 2020 2020 2020 6966 2064    ).        if d
-00014ab0: 696d 7320 6973 206e 6f74 204e 6f6e 6520  ims is not None 
-00014ac0: 6f72 206b 7761 7267 732e 6765 7428 226f  or kwargs.get("o
-00014ad0: 6273 6572 7665 6422 2920 6973 206e 6f74  bserved") is not
-00014ae0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00014af0: 2020 206e 5f7a 6572 6f73 756d 5f61 7865     n_zerosum_axe
-00014b00: 7320 3d20 636c 732e 6368 6563 6b5f 7a65  s = cls.check_ze
-00014b10: 726f 7375 6d5f 6178 6573 286e 5f7a 6572  rosum_axes(n_zer
-00014b20: 6f73 756d 5f61 7865 7329 0a0a 2020 2020  osum_axes)..    
-00014b30: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
-00014b40: 7368 6170 6520 3d20 6765 745f 7375 7070  shape = get_supp
-00014b50: 6f72 745f 7368 6170 6528 0a20 2020 2020  ort_shape(.     
-00014b60: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
-00014b70: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
-00014b80: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
-00014b90: 2020 2020 2020 2020 7368 6170 653d 4e6f          shape=No
-00014ba0: 6e65 2c20 2023 2053 6861 7065 2077 696c  ne,  # Shape wil
-00014bb0: 6c20 6265 2063 6865 636b 6564 2069 6e20  l be checked in 
-00014bc0: 6063 6c73 2e64 6973 7460 0a20 2020 2020  `cls.dist`.     
-00014bd0: 2020 2020 2020 2020 2020 2064 696d 733d             dims=
-00014be0: 6469 6d73 2c0a 2020 2020 2020 2020 2020  dims,.          
-00014bf0: 2020 2020 2020 6f62 7365 7276 6564 3d6b        observed=k
-00014c00: 7761 7267 732e 6765 7428 226f 6273 6572  wargs.get("obser
-00014c10: 7665 6422 2c20 4e6f 6e65 292c 0a20 2020  ved", None),.   
-00014c20: 2020 2020 2020 2020 2020 2020 206e 6469               ndi
-00014c30: 6d5f 7375 7070 3d6e 5f7a 6572 6f73 756d  m_supp=n_zerosum
-00014c40: 5f61 7865 732c 0a20 2020 2020 2020 2020  _axes,.         
-00014c50: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
-00014c60: 7475 726e 2073 7570 6572 2829 2e5f 5f6e  turn super().__n
-00014c70: 6577 5f5f 280a 2020 2020 2020 2020 2020  ew__(.          
-00014c80: 2020 636c 732c 0a20 2020 2020 2020 2020    cls,.         
-00014c90: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
-00014ca0: 2020 2020 2020 6e5f 7a65 726f 7375 6d5f        n_zerosum_
-00014cb0: 6178 6573 3d6e 5f7a 6572 6f73 756d 5f61  axes=n_zerosum_a
-00014cc0: 7865 732c 0a20 2020 2020 2020 2020 2020  xes,.           
-00014cd0: 2073 7570 706f 7274 5f73 6861 7065 3d73   support_shape=s
-00014ce0: 7570 706f 7274 5f73 6861 7065 2c0a 2020  upport_shape,.  
-00014cf0: 2020 2020 2020 2020 2020 6469 6d73 3d64            dims=d
-00014d00: 696d 732c 0a20 2020 2020 2020 2020 2020  ims,.           
-00014d10: 202a 2a6b 7761 7267 732c 0a20 2020 2020   **kwargs,.     
-00014d20: 2020 2029 0a0a 2020 2020 4063 6c61 7373     )..    @class
-00014d30: 6d65 7468 6f64 0a20 2020 2064 6566 2064  method.    def d
-00014d40: 6973 7428 636c 732c 2073 6967 6d61 3d31  ist(cls, sigma=1
-00014d50: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
-00014d60: 3d4e 6f6e 652c 2073 7570 706f 7274 5f73  =None, support_s
-00014d70: 6861 7065 3d4e 6f6e 652c 202a 2a6b 7761  hape=None, **kwa
-00014d80: 7267 7329 3a0a 2020 2020 2020 2020 6e5f  rgs):.        n_
-00014d90: 7a65 726f 7375 6d5f 6178 6573 203d 2063  zerosum_axes = c
-00014da0: 6c73 2e63 6865 636b 5f7a 6572 6f73 756d  ls.check_zerosum
-00014db0: 5f61 7865 7328 6e5f 7a65 726f 7375 6d5f  _axes(n_zerosum_
-00014dc0: 6178 6573 290a 0a20 2020 2020 2020 2073  axes)..        s
-00014dd0: 6967 6d61 203d 2070 742e 6173 5f74 656e  igma = pt.as_ten
-00014de0: 736f 725f 7661 7269 6162 6c65 2866 6c6f  sor_variable(flo
-00014df0: 6174 5828 7369 676d 6129 290a 2020 2020  atX(sigma)).    
-00014e00: 2020 2020 6966 2073 6967 6d61 2e6e 6469      if sigma.ndi
-00014e10: 6d20 3e20 303a 0a20 2020 2020 2020 2020  m > 0:.         
-00014e20: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00014e30: 726f 7228 2273 6967 6d61 2068 6173 2074  ror("sigma has t
-00014e40: 6f20 6265 2061 2073 6361 6c61 7222 290a  o be a scalar").
-00014e50: 0a20 2020 2020 2020 2073 7570 706f 7274  .        support
-00014e60: 5f73 6861 7065 203d 2067 6574 5f73 7570  _shape = get_sup
-00014e70: 706f 7274 5f73 6861 7065 280a 2020 2020  port_shape(.    
-00014e80: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
-00014e90: 7368 6170 653d 7375 7070 6f72 745f 7368  shape=support_sh
-00014ea0: 6170 652c 0a20 2020 2020 2020 2020 2020  ape,.           
-00014eb0: 2073 6861 7065 3d6b 7761 7267 732e 6765   shape=kwargs.ge
-00014ec0: 7428 2273 6861 7065 2229 2c0a 2020 2020  t("shape"),.    
-00014ed0: 2020 2020 2020 2020 6e64 696d 5f73 7570          ndim_sup
-00014ee0: 703d 6e5f 7a65 726f 7375 6d5f 6178 6573  p=n_zerosum_axes
-00014ef0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
-00014f00: 2020 2020 2069 6620 7375 7070 6f72 745f       if support_
-00014f10: 7368 6170 6520 6973 204e 6f6e 653a 0a20  shape is None:. 
-00014f20: 2020 2020 2020 2020 2020 2069 6620 6e5f             if n_
-00014f30: 7a65 726f 7375 6d5f 6178 6573 203e 2030  zerosum_axes > 0
-00014f40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014f50: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00014f60: 6f72 2822 596f 7520 6d75 7374 2073 7065  or("You must spe
-00014f70: 6369 6679 2064 696d 732c 2073 6861 7065  cify dims, shape
-00014f80: 206f 7220 7375 7070 6f72 745f 7368 6170   or support_shap
-00014f90: 6520 7061 7261 6d65 7465 7222 290a 2020  e parameter").  
-00014fa0: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
-00014fb0: 3a20 6564 6765 2d63 6173 6520 646f 6573  : edge-case does
-00014fc0: 6e27 7420 776f 726b 2066 6f72 206e 6f77  n't work for now
-00014fd0: 2c20 6265 6361 7573 6520 7074 2e73 7461  , because pt.sta
-00014fe0: 636b 2069 6e20 6765 745f 7375 7070 6f72  ck in get_suppor
-00014ff0: 745f 7368 6170 6520 6661 696c 730a 2020  t_shape fails.  
-00015000: 2020 2020 2020 2020 2020 2320 656c 7365            # else
-00015010: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00015020: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
-00015030: 6520 3d20 2829 2023 2062 6563 6175 7365  e = () # because
-00015040: 2069 7427 7320 6a75 7374 2061 204e 6f72   it's just a Nor
-00015050: 6d61 6c20 696e 2074 6861 7420 6361 7365  mal in that case
-00015060: 0a20 2020 2020 2020 2073 7570 706f 7274  .        support
-00015070: 5f73 6861 7065 203d 2070 742e 6173 5f74  _shape = pt.as_t
-00015080: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
-00015090: 6e74 5828 7375 7070 6f72 745f 7368 6170  ntX(support_shap
-000150a0: 6529 290a 0a20 2020 2020 2020 2061 7373  e))..        ass
-000150b0: 6572 7420 6e5f 7a65 726f 7375 6d5f 6178  ert n_zerosum_ax
-000150c0: 6573 203d 3d20 7074 2e67 6574 5f76 6563  es == pt.get_vec
-000150d0: 746f 725f 6c65 6e67 7468 280a 2020 2020  tor_length(.    
-000150e0: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
-000150f0: 7368 6170 650a 2020 2020 2020 2020 292c  shape.        ),
-00015100: 2022 7375 7070 6f72 745f 7368 6170 6520   "support_shape 
-00015110: 6861 7320 746f 2062 6520 6173 206c 6f6e  has to be as lon
-00015120: 6720 6173 206e 5f7a 6572 6f73 756d 5f61  g as n_zerosum_a
-00015130: 7865 7322 0a0a 2020 2020 2020 2020 7265  xes"..        re
-00015140: 7475 726e 2073 7570 6572 2829 2e64 6973  turn super().dis
-00015150: 7428 0a20 2020 2020 2020 2020 2020 205b  t(.            [
-00015160: 7369 676d 615d 2c20 6e5f 7a65 726f 7375  sigma], n_zerosu
-00015170: 6d5f 6178 6573 3d6e 5f7a 6572 6f73 756d  m_axes=n_zerosum
-00015180: 5f61 7865 732c 2073 7570 706f 7274 5f73  _axes, support_s
-00015190: 6861 7065 3d73 7570 706f 7274 5f73 6861  hape=support_sha
-000151a0: 7065 2c20 2a2a 6b77 6172 6773 0a20 2020  pe, **kwargs.   
-000151b0: 2020 2020 2029 0a0a 2020 2020 4063 6c61       )..    @cla
-000151c0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-000151d0: 2063 6865 636b 5f7a 6572 6f73 756d 5f61   check_zerosum_a
-000151e0: 7865 7328 636c 732c 206e 5f7a 6572 6f73  xes(cls, n_zeros
-000151f0: 756d 5f61 7865 733a 204f 7074 696f 6e61  um_axes: Optiona
-00015200: 6c5b 696e 745d 2920 2d3e 2069 6e74 3a0a  l[int]) -> int:.
-00015210: 2020 2020 2020 2020 6966 206e 5f7a 6572          if n_zer
-00015220: 6f73 756d 5f61 7865 7320 6973 204e 6f6e  osum_axes is Non
-00015230: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
-00015240: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
-00015250: 310a 2020 2020 2020 2020 6966 206e 6f74  1.        if not
-00015260: 2069 7369 6e73 7461 6e63 6528 6e5f 7a65   isinstance(n_ze
-00015270: 726f 7375 6d5f 6178 6573 2c20 696e 7429  rosum_axes, int)
-00015280: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
-00015290: 6973 6520 5479 7065 4572 726f 7228 226e  ise TypeError("n
-000152a0: 5f7a 6572 6f73 756d 5f61 7865 7320 6861  _zerosum_axes ha
-000152b0: 7320 746f 2062 6520 616e 2069 6e74 6567  s to be an integ
-000152c0: 6572 2229 0a20 2020 2020 2020 2069 6620  er").        if 
-000152d0: 6e6f 7420 6e5f 7a65 726f 7375 6d5f 6178  not n_zerosum_ax
-000152e0: 6573 203e 2030 3a0a 2020 2020 2020 2020  es > 0:.        
-000152f0: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00015300: 7272 6f72 2822 6e5f 7a65 726f 7375 6d5f  rror("n_zerosum_
-00015310: 6178 6573 2068 6173 2074 6f20 6265 203e  axes has to be >
-00015320: 2030 2229 0a20 2020 2020 2020 2072 6574   0").        ret
-00015330: 7572 6e20 6e5f 7a65 726f 7375 6d5f 6178  urn n_zerosum_ax
-00015340: 6573 0a0a 2020 2020 4063 6c61 7373 6d65  es..    @classme
-00015350: 7468 6f64 0a20 2020 2064 6566 2072 765f  thod.    def rv_
-00015360: 6f70 2863 6c73 2c20 7369 676d 612c 206e  op(cls, sigma, n
-00015370: 5f7a 6572 6f73 756d 5f61 7865 732c 2073  _zerosum_axes, s
-00015380: 7570 706f 7274 5f73 6861 7065 2c20 7369  upport_shape, si
-00015390: 7a65 3d4e 6f6e 6529 3a0a 2020 2020 2020  ze=None):.      
-000153a0: 2020 7368 6170 6520 3d20 746f 5f74 7570    shape = to_tup
-000153b0: 6c65 2873 697a 6529 202b 2074 7570 6c65  le(size) + tuple
-000153c0: 2873 7570 706f 7274 5f73 6861 7065 290a  (support_shape).
-000153d0: 2020 2020 2020 2020 6e6f 726d 616c 5f64          normal_d
-000153e0: 6973 7420 3d20 6967 6e6f 7265 5f6c 6f67  ist = ignore_log
-000153f0: 7072 6f62 2870 6d2e 4e6f 726d 616c 2e64  prob(pm.Normal.d
-00015400: 6973 7428 7369 676d 613d 7369 676d 612c  ist(sigma=sigma,
-00015410: 2073 6861 7065 3d73 6861 7065 2929 0a0a   shape=shape))..
-00015420: 2020 2020 2020 2020 6966 206e 5f7a 6572          if n_zer
-00015430: 6f73 756d 5f61 7865 7320 3e20 6e6f 726d  osum_axes > norm
-00015440: 616c 5f64 6973 742e 6e64 696d 3a0a 2020  al_dist.ndim:.  
-00015450: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00015460: 5661 6c75 6545 7272 6f72 2822 5368 6170  ValueError("Shap
-00015470: 6520 6f66 2064 6973 7472 6962 7574 696f  e of distributio
-00015480: 6e20 6973 2074 6f6f 2073 6d61 6c6c 2066  n is too small f
-00015490: 6f72 2074 6865 206e 756d 6265 7220 6f66  or the number of
-000154a0: 207a 6572 6f73 756d 2061 7865 7322 290a   zerosum axes").
-000154b0: 0a20 2020 2020 2020 206e 6f72 6d61 6c5f  .        normal_
-000154c0: 6469 7374 5f2c 2073 6967 6d61 5f2c 2073  dist_, sigma_, s
-000154d0: 7570 706f 7274 5f73 6861 7065 5f20 3d20  upport_shape_ = 
-000154e0: 280a 2020 2020 2020 2020 2020 2020 6e6f  (.            no
-000154f0: 726d 616c 5f64 6973 742e 7479 7065 2829  rmal_dist.type()
-00015500: 2c0a 2020 2020 2020 2020 2020 2020 7369  ,.            si
-00015510: 676d 612e 7479 7065 2829 2c0a 2020 2020  gma.type(),.    
-00015520: 2020 2020 2020 2020 7375 7070 6f72 745f          support_
-00015530: 7368 6170 652e 7479 7065 2829 2c0a 2020  shape.type(),.  
-00015540: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00015550: 2023 205a 6572 6f73 756d 2d6e 6f72 6d61   # Zerosum-norma
-00015560: 6c69 6e67 2069 7320 6163 6869 6576 6564  ling is achieved
-00015570: 2062 7920 7375 6274 7261 6374 696e 6720   by subtracting 
-00015580: 7468 6520 6d65 616e 2061 6c6f 6e67 2074  the mean along t
-00015590: 6865 2067 6976 656e 206e 5f7a 6572 6f73  he given n_zeros
-000155a0: 756d 5f61 7865 730a 2020 2020 2020 2020  um_axes.        
-000155b0: 7a65 726f 7375 6d5f 7276 5f20 3d20 6e6f  zerosum_rv_ = no
-000155c0: 726d 616c 5f64 6973 745f 0a20 2020 2020  rmal_dist_.     
-000155d0: 2020 2066 6f72 2061 7869 7320 696e 2072     for axis in r
-000155e0: 616e 6765 286e 5f7a 6572 6f73 756d 5f61  ange(n_zerosum_a
-000155f0: 7865 7329 3a0a 2020 2020 2020 2020 2020  xes):.          
-00015600: 2020 7a65 726f 7375 6d5f 7276 5f20 2d3d    zerosum_rv_ -=
-00015610: 207a 6572 6f73 756d 5f72 765f 2e6d 6561   zerosum_rv_.mea
-00015620: 6e28 6178 6973 3d2d 6178 6973 202d 2031  n(axis=-axis - 1
-00015630: 2c20 6b65 6570 6469 6d73 3d54 7275 6529  , keepdims=True)
-00015640: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00015650: 205a 6572 6f53 756d 4e6f 726d 616c 5256   ZeroSumNormalRV
-00015660: 280a 2020 2020 2020 2020 2020 2020 696e  (.            in
-00015670: 7075 7473 3d5b 6e6f 726d 616c 5f64 6973  puts=[normal_dis
-00015680: 745f 2c20 7369 676d 615f 2c20 7375 7070  t_, sigma_, supp
-00015690: 6f72 745f 7368 6170 655f 5d2c 0a20 2020  ort_shape_],.   
-000156a0: 2020 2020 2020 2020 206f 7574 7075 7473           outputs
-000156b0: 3d5b 7a65 726f 7375 6d5f 7276 5f2c 2073  =[zerosum_rv_, s
-000156c0: 7570 706f 7274 5f73 6861 7065 5f5d 2c0a  upport_shape_],.
-000156d0: 2020 2020 2020 2020 2020 2020 6e64 696d              ndim
-000156e0: 5f73 7570 703d 6e5f 7a65 726f 7375 6d5f  _supp=n_zerosum_
-000156f0: 6178 6573 2c0a 2020 2020 2020 2020 2928  axes,.        )(
-00015700: 6e6f 726d 616c 5f64 6973 742c 2073 6967  normal_dist, sig
-00015710: 6d61 2c20 7375 7070 6f72 745f 7368 6170  ma, support_shap
-00015720: 6529 0a0a 0a40 5f63 6861 6e67 655f 6469  e)...@_change_di
-00015730: 7374 5f73 697a 652e 7265 6769 7374 6572  st_size.register
-00015740: 285a 6572 6f53 756d 4e6f 726d 616c 5256  (ZeroSumNormalRV
-00015750: 290a 6465 6620 6368 616e 6765 5f7a 6572  ).def change_zer
-00015760: 6f73 756d 5f73 697a 6528 6f70 2c20 6e6f  osum_size(op, no
-00015770: 726d 616c 5f64 6973 742c 206e 6577 5f73  rmal_dist, new_s
-00015780: 697a 652c 2065 7870 616e 643d 4661 6c73  ize, expand=Fals
-00015790: 6529 3a0a 2020 2020 6e6f 726d 616c 5f64  e):.    normal_d
-000157a0: 6973 742c 2073 6967 6d61 2c20 7375 7070  ist, sigma, supp
-000157b0: 6f72 745f 7368 6170 6520 3d20 6e6f 726d  ort_shape = norm
-000157c0: 616c 5f64 6973 742e 6f77 6e65 722e 696e  al_dist.owner.in
-000157d0: 7075 7473 0a0a 2020 2020 6966 2065 7870  puts..    if exp
-000157e0: 616e 643a 0a20 2020 2020 2020 206f 7269  and:.        ori
-000157f0: 6769 6e61 6c5f 7368 6170 6520 3d20 7475  ginal_shape = tu
-00015800: 706c 6528 6e6f 726d 616c 5f64 6973 742e  ple(normal_dist.
-00015810: 7368 6170 6529 0a20 2020 2020 2020 206f  shape).        o
-00015820: 6c64 5f73 697a 6520 3d20 6f72 6967 696e  ld_size = origin
-00015830: 616c 5f73 6861 7065 5b3a 206c 656e 286f  al_shape[: len(o
-00015840: 7269 6769 6e61 6c5f 7368 6170 6529 202d  riginal_shape) -
-00015850: 206f 702e 6e64 696d 5f73 7570 705d 0a20   op.ndim_supp]. 
-00015860: 2020 2020 2020 206e 6577 5f73 697a 6520         new_size 
-00015870: 3d20 7475 706c 6528 6e65 775f 7369 7a65  = tuple(new_size
-00015880: 2920 2b20 6f6c 645f 7369 7a65 0a0a 2020  ) + old_size..  
-00015890: 2020 7265 7475 726e 205a 6572 6f53 756d    return ZeroSum
-000158a0: 4e6f 726d 616c 2e72 765f 6f70 280a 2020  Normal.rv_op(.  
-000158b0: 2020 2020 2020 7369 676d 613d 7369 676d        sigma=sigm
-000158c0: 612c 206e 5f7a 6572 6f73 756d 5f61 7865  a, n_zerosum_axe
-000158d0: 733d 6f70 2e6e 6469 6d5f 7375 7070 2c20  s=op.ndim_supp, 
-000158e0: 7375 7070 6f72 745f 7368 6170 653d 7375  support_shape=su
-000158f0: 7070 6f72 745f 7368 6170 652c 2073 697a  pport_shape, siz
-00015900: 653d 6e65 775f 7369 7a65 0a20 2020 2029  e=new_size.    )
-00015910: 0a0a 0a40 5f6d 6f6d 656e 742e 7265 6769  ...@_moment.regi
-00015920: 7374 6572 285a 6572 6f53 756d 4e6f 726d  ster(ZeroSumNorm
-00015930: 616c 5256 290a 6465 6620 7a65 726f 7375  alRV).def zerosu
-00015940: 6d6e 6f72 6d61 6c5f 6d6f 6d65 6e74 286f  mnormal_moment(o
-00015950: 702c 2072 762c 202a 7276 5f69 6e70 7574  p, rv, *rv_input
-00015960: 7329 3a0a 2020 2020 7265 7475 726e 2070  s):.    return p
-00015970: 742e 7a65 726f 735f 6c69 6b65 2872 7629  t.zeros_like(rv)
-00015980: 0a0a 0a40 5f64 6566 6175 6c74 5f74 7261  ...@_default_tra
-00015990: 6e73 666f 726d 2e72 6567 6973 7465 7228  nsform.register(
-000159a0: 5a65 726f 5375 6d4e 6f72 6d61 6c52 5629  ZeroSumNormalRV)
-000159b0: 0a64 6566 207a 6572 6f73 756d 5f64 6566  .def zerosum_def
-000159c0: 6175 6c74 5f74 7261 6e73 666f 726d 286f  ault_transform(o
-000159d0: 702c 2072 7629 3a0a 2020 2020 6e5f 7a65  p, rv):.    n_ze
-000159e0: 726f 7375 6d5f 6178 6573 203d 2074 7570  rosum_axes = tup
-000159f0: 6c65 286e 702e 6172 616e 6765 282d 6f70  le(np.arange(-op
-00015a00: 2e6e 6469 6d5f 7375 7070 2c20 3029 290a  .ndim_supp, 0)).
-00015a10: 2020 2020 7265 7475 726e 205a 6572 6f53      return ZeroS
-00015a20: 756d 5472 616e 7366 6f72 6d28 6e5f 7a65  umTransform(n_ze
-00015a30: 726f 7375 6d5f 6178 6573 290a 0a0a 405f  rosum_axes)...@_
-00015a40: 6c6f 6770 726f 622e 7265 6769 7374 6572  logprob.register
-00015a50: 285a 6572 6f53 756d 4e6f 726d 616c 5256  (ZeroSumNormalRV
-00015a60: 290a 6465 6620 7a65 726f 7375 6d6e 6f72  ).def zerosumnor
-00015a70: 6d61 6c5f 6c6f 6770 286f 702c 2076 616c  mal_logp(op, val
-00015a80: 7565 732c 206e 6f72 6d61 6c5f 6469 7374  ues, normal_dist
-00015a90: 2c20 7369 676d 612c 2073 7570 706f 7274  , sigma, support
-00015aa0: 5f73 6861 7065 2c20 2a2a 6b77 6172 6773  _shape, **kwargs
-00015ab0: 293a 0a20 2020 2028 7661 6c75 652c 2920  ):.    (value,) 
-00015ac0: 3d20 7661 6c75 6573 0a20 2020 2073 6861  = values.    sha
-00015ad0: 7065 203d 2076 616c 7565 2e73 6861 7065  pe = value.shape
-00015ae0: 0a20 2020 206e 5f7a 6572 6f73 756d 5f61  .    n_zerosum_a
-00015af0: 7865 7320 3d20 6f70 2e6e 6469 6d5f 7375  xes = op.ndim_su
-00015b00: 7070 0a0a 2020 2020 5f64 6567 5f66 7265  pp..    _deg_fre
-00015b10: 655f 7375 7070 6f72 745f 7368 6170 6520  e_support_shape 
-00015b20: 3d20 7074 2e69 6e63 5f73 7562 7465 6e73  = pt.inc_subtens
-00015b30: 6f72 2873 6861 7065 5b2d 6e5f 7a65 726f  or(shape[-n_zero
-00015b40: 7375 6d5f 6178 6573 3a5d 2c20 2d31 290a  sum_axes:], -1).
-00015b50: 2020 2020 5f66 756c 6c5f 7369 7a65 203d      _full_size =
-00015b60: 2070 742e 7072 6f64 2873 6861 7065 290a   pt.prod(shape).
-00015b70: 2020 2020 5f64 6567 7265 6573 5f6f 665f      _degrees_of_
-00015b80: 6672 6565 646f 6d20 3d20 7074 2e70 726f  freedom = pt.pro
-00015b90: 6428 5f64 6567 5f66 7265 655f 7375 7070  d(_deg_free_supp
-00015ba0: 6f72 745f 7368 6170 6529 0a0a 2020 2020  ort_shape)..    
-00015bb0: 7a65 726f 7375 6d73 203d 205b 0a20 2020  zerosums = [.   
-00015bc0: 2020 2020 2070 742e 616c 6c28 7074 2e69       pt.all(pt.i
-00015bd0: 7363 6c6f 7365 2870 742e 6d65 616e 2876  sclose(pt.mean(v
-00015be0: 616c 7565 2c20 6178 6973 3d2d 6178 6973  alue, axis=-axis
-00015bf0: 202d 2031 292c 2030 2c20 6174 6f6c 3d31   - 1), 0, atol=1
-00015c00: 652d 3929 290a 2020 2020 2020 2020 666f  e-9)).        fo
-00015c10: 7220 6178 6973 2069 6e20 7261 6e67 6528  r axis in range(
-00015c20: 6e5f 7a65 726f 7375 6d5f 6178 6573 290a  n_zerosum_axes).
-00015c30: 2020 2020 5d0a 0a20 2020 206f 7574 203d      ]..    out =
-00015c40: 2070 742e 7375 6d28 0a20 2020 2020 2020   pt.sum(.       
-00015c50: 2070 6d2e 6c6f 6770 286e 6f72 6d61 6c5f   pm.logp(normal_
-00015c60: 6469 7374 2c20 7661 6c75 6529 202a 205f  dist, value) * _
-00015c70: 6465 6772 6565 735f 6f66 5f66 7265 6564  degrees_of_freed
-00015c80: 6f6d 202f 205f 6675 6c6c 5f73 697a 652c  om / _full_size,
-00015c90: 0a20 2020 2020 2020 2061 7869 733d 7475  .        axis=tu
-00015ca0: 706c 6528 6e70 2e61 7261 6e67 6528 2d6e  ple(np.arange(-n
-00015cb0: 5f7a 6572 6f73 756d 5f61 7865 732c 2030  _zerosum_axes, 0
-00015cc0: 2929 2c0a 2020 2020 290a 0a20 2020 2072  )),.    )..    r
-00015cd0: 6574 7572 6e20 6368 6563 6b5f 7061 7261  eturn check_para
-00015ce0: 6d65 7465 7273 286f 7574 2c20 2a7a 6572  meters(out, *zer
-00015cf0: 6f73 756d 732c 206d 7367 3d22 6d65 616e  osums, msg="mean
-00015d00: 2876 616c 7565 2c20 6178 6973 3d6e 5f7a  (value, axis=n_z
-00015d10: 6572 6f73 756d 5f61 7865 7329 203d 2030  erosum_axes) = 0
-00015d20: 2229 0a                                  ").
+00005320: 2020 5c70 726f 645f 7b6b 3d31 7d5e 4b0a    \prod_{k=1}^K.
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 2020 205c 6672 6163 7b5c           \frac{\
+00005350: 4761 6d6d 6128 785f 6b20 2b20 2061 5f6b  Gamma(x_k +  a_k
+00005360: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
+00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005380: 207b 5c47 616d 6d61 2878 5f6b 202b 2031   {\Gamma(x_k + 1
+00005390: 295c 4761 6d6d 6128 615f 6b29 7d0a 0a20  )\Gamma(a_k)}.. 
+000053a0: 2020 203d 3d3d 3d3d 3d3d 3d3d 3d20 203d     ==========  =
+000053b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000053c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000053d0: 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020 2053  ==========.    S
+000053e0: 7570 706f 7274 2020 2020 203a 6d61 7468  upport     :math
+000053f0: 3a60 7820 5c69 6e20 5c7b 302c 2031 2c20  :`x \in \{0, 1, 
+00005400: 5c6c 646f 7473 2c20 6e5c 7d60 2073 7563  \ldots, n\}` suc
+00005410: 6820 7468 6174 0a20 2020 2020 2020 2020  h that.         
+00005420: 2020 2020 2020 203a 6d61 7468 3a60 5c73         :math:`\s
+00005430: 756d 2078 5f69 203d 206e 600a 2020 2020  um x_i = n`.    
+00005440: 4d65 616e 2020 2020 2020 2020 3a6d 6174  Mean        :mat
+00005450: 683a 606e 205c 6672 6163 7b61 5f69 7d7b  h:`n \frac{a_i}{
+00005460: 5c73 756d 7b61 5f6b 7d7d 600a 2020 2020  \sum{a_k}}`.    
+00005470: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
+00005480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00005490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000054a0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
+000054b0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+000054c0: 2d2d 2d2d 2d2d 0a20 2020 206e 203a 2074  ------.    n : t
+000054d0: 656e 736f 725f 6c69 6b65 206f 6620 696e  ensor_like of in
+000054e0: 740a 2020 2020 2020 2020 546f 7461 6c20  t.        Total 
+000054f0: 636f 756e 7473 2069 6e20 6561 6368 2072  counts in each r
+00005500: 6570 6c69 6361 7465 2028 6e20 3e20 3029  eplicate (n > 0)
+00005510: 2e0a 0a20 2020 2061 203a 2074 656e 736f  ...    a : tenso
+00005520: 725f 6c69 6b65 206f 6620 666c 6f61 740a  r_like of float.
+00005530: 2020 2020 2020 2020 4469 7269 6368 6c65          Dirichle
+00005540: 7420 636f 6e63 656e 7472 6174 696f 6e20  t concentration 
+00005550: 7061 7261 6d65 7465 7273 2028 6120 3e20  parameters (a > 
+00005560: 3029 2e20 5468 6520 6e75 6d62 6572 206f  0). The number o
+00005570: 6620 6361 7465 676f 7269 6573 2069 7320  f categories is 
+00005580: 6769 7665 6e20 6279 0a20 2020 2020 2020  given by.       
+00005590: 2074 6865 206c 656e 6774 6820 6f66 2074   the length of t
+000055a0: 6865 206c 6173 7420 6178 6973 2e0a 2020  he last axis..  
+000055b0: 2020 2222 220a 2020 2020 7276 5f6f 7020    """.    rv_op 
+000055c0: 3d20 6469 7269 6368 6c65 745f 6d75 6c74  = dirichlet_mult
+000055d0: 696e 6f6d 6961 6c0a 0a20 2020 2040 636c  inomial..    @cl
+000055e0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+000055f0: 6620 6469 7374 2863 6c73 2c20 6e2c 2061  f dist(cls, n, a
+00005600: 2c20 2a61 7267 732c 202a 2a6b 7761 7267  , *args, **kwarg
+00005610: 7329 3a0a 2020 2020 2020 2020 6e20 3d20  s):.        n = 
+00005620: 696e 7458 286e 290a 2020 2020 2020 2020  intX(n).        
+00005630: 6120 3d20 666c 6f61 7458 2861 290a 0a20  a = floatX(a).. 
+00005640: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
+00005650: 7065 7228 292e 6469 7374 285b 6e2c 2061  per().dist([n, a
+00005660: 5d2c 202a 2a6b 7761 7267 7329 0a0a 2020  ], **kwargs)..  
+00005670: 2020 6465 6620 6d6f 6d65 6e74 2872 762c    def moment(rv,
+00005680: 2073 697a 652c 206e 2c20 6129 3a0a 2020   size, n, a):.  
+00005690: 2020 2020 2020 7020 3d20 6120 2f20 7074        p = a / pt
+000056a0: 2e73 756d 2861 2c20 6178 6973 3d2d 312c  .sum(a, axis=-1,
+000056b0: 206b 6565 7064 696d 733d 5472 7565 290a   keepdims=True).
+000056c0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+000056d0: 6f6d 656e 7428 4d75 6c74 696e 6f6d 6961  oment(Multinomia
+000056e0: 6c2e 6469 7374 286e 3d6e 2c20 703d 702c  l.dist(n=n, p=p,
+000056f0: 2073 697a 653d 7369 7a65 2929 0a0a 2020   size=size))..  
+00005700: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
+00005710: 2c20 6e2c 2061 293a 0a20 2020 2020 2020  , n, a):.       
+00005720: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+00005730: 6375 6c61 7465 206c 6f67 2d70 726f 6261  culate log-proba
+00005740: 6269 6c69 7479 206f 6620 4469 7269 6368  bility of Dirich
+00005750: 6c65 744d 756c 7469 6e6f 6d69 616c 2064  letMultinomial d
+00005760: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
+00005770: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
+00005780: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+00005790: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+000057a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000057b0: 2020 2020 2020 2076 616c 7565 3a20 696e         value: in
+000057c0: 7465 6765 7220 6172 7261 790a 2020 2020  teger array.    
+000057d0: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
+000057e0: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
+000057f0: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
+00005800: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
+00005810: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00005820: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00005830: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
+00005840: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00005850: 2020 2073 756d 5f61 203d 2061 2e73 756d     sum_a = a.sum
+00005860: 2861 7869 733d 2d31 290a 2020 2020 2020  (axis=-1).      
+00005870: 2020 636f 6e73 7420 3d20 2867 616d 6d61    const = (gamma
+00005880: 6c6e 286e 202b 2031 2920 2b20 6761 6d6d  ln(n + 1) + gamm
+00005890: 616c 6e28 7375 6d5f 6129 2920 2d20 6761  aln(sum_a)) - ga
+000058a0: 6d6d 616c 6e28 6e20 2b20 7375 6d5f 6129  mmaln(n + sum_a)
+000058b0: 0a20 2020 2020 2020 2073 6572 6965 7320  .        series 
+000058c0: 3d20 6761 6d6d 616c 6e28 7661 6c75 6520  = gammaln(value 
+000058d0: 2b20 6129 202d 2028 6761 6d6d 616c 6e28  + a) - (gammaln(
+000058e0: 7661 6c75 6520 2b20 3129 202b 2067 616d  value + 1) + gam
+000058f0: 6d61 6c6e 2861 2929 0a20 2020 2020 2020  maln(a)).       
+00005900: 2072 6573 203d 2063 6f6e 7374 202b 2073   res = const + s
+00005910: 6572 6965 732e 7375 6d28 6178 6973 3d2d  eries.sum(axis=-
+00005920: 3129 0a0a 2020 2020 2020 2020 7265 7320  1)..        res 
+00005930: 3d20 7074 2e73 7769 7463 6828 0a20 2020  = pt.switch(.   
+00005940: 2020 2020 2020 2020 2070 742e 6f72 5f28           pt.or_(
+00005950: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005960: 2070 742e 616e 7928 7074 2e6c 7428 7661   pt.any(pt.lt(va
+00005970: 6c75 652c 2030 292c 2061 7869 733d 2d31  lue, 0), axis=-1
+00005980: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00005990: 2020 2070 742e 6e65 7128 7074 2e73 756d     pt.neq(pt.sum
+000059a0: 2876 616c 7565 2c20 6178 6973 3d2d 3129  (value, axis=-1)
+000059b0: 2c20 6e29 2c0a 2020 2020 2020 2020 2020  , n),.          
+000059c0: 2020 292c 0a20 2020 2020 2020 2020 2020    ),.           
+000059d0: 202d 6e70 2e69 6e66 2c0a 2020 2020 2020   -np.inf,.      
+000059e0: 2020 2020 2020 7265 732c 0a20 2020 2020        res,.     
+000059f0: 2020 2029 0a0a 2020 2020 2020 2020 7265     )..        re
+00005a00: 7475 726e 2063 6865 636b 5f70 6172 616d  turn check_param
+00005a10: 6574 6572 7328 0a20 2020 2020 2020 2020  eters(.         
+00005a20: 2020 2072 6573 2c0a 2020 2020 2020 2020     res,.        
+00005a30: 2020 2020 6120 3e20 302c 0a20 2020 2020      a > 0,.     
+00005a40: 2020 2020 2020 206e 203e 3d20 302c 0a20         n >= 0,. 
+00005a50: 2020 2020 2020 2020 2020 206d 7367 3d22             msg="
+00005a60: 6120 3e20 302c 206e 203e 3d20 3022 2c0a  a > 0, n >= 0",.
+00005a70: 2020 2020 2020 2020 290a 0a0a 636c 6173          )...clas
+00005a80: 7320 5f4f 7264 6572 6564 4d75 6c74 696e  s _OrderedMultin
+00005a90: 6f6d 6961 6c28 4d75 6c74 696e 6f6d 6961  omial(Multinomia
+00005aa0: 6c29 3a0a 2020 2020 7222 2222 0a20 2020  l):.    r""".   
+00005ab0: 2055 6e64 6572 6c79 696e 6720 636c 6173   Underlying clas
+00005ac0: 7320 666f 7220 6f72 6465 7265 6420 6d75  s for ordered mu
+00005ad0: 6c74 696e 6f6d 6961 6c20 6469 7374 7269  ltinomial distri
+00005ae0: 6275 7469 6f6e 732e 0a20 2020 2053 6565  butions..    See
+00005af0: 2064 6f63 7320 666f 7220 7468 6520 4f72   docs for the Or
+00005b00: 6465 7265 644d 756c 7469 6e6f 6d69 616c  deredMultinomial
+00005b10: 2077 7261 7070 6572 2063 6c61 7373 2066   wrapper class f
+00005b20: 6f72 206d 6f72 6520 6465 7461 696c 7320  or more details 
+00005b30: 6f6e 2068 6f77 2074 6f20 7573 6520 6974  on how to use it
+00005b40: 2069 6e20 6d6f 6465 6c73 2e0a 2020 2020   in models..    
+00005b50: 2222 220a 2020 2020 7276 5f6f 7020 3d20  """.    rv_op = 
+00005b60: 6d75 6c74 696e 6f6d 6961 6c0a 0a20 2020  multinomial..   
+00005b70: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00005b80: 2020 6465 6620 6469 7374 2863 6c73 2c20    def dist(cls, 
+00005b90: 6574 612c 2063 7574 706f 696e 7473 2c20  eta, cutpoints, 
+00005ba0: 6e2c 202a 6172 6773 2c20 2a2a 6b77 6172  n, *args, **kwar
+00005bb0: 6773 293a 0a20 2020 2020 2020 2065 7461  gs):.        eta
+00005bc0: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
+00005bd0: 7661 7269 6162 6c65 2866 6c6f 6174 5828  variable(floatX(
+00005be0: 6574 6129 290a 2020 2020 2020 2020 6375  eta)).        cu
+00005bf0: 7470 6f69 6e74 7320 3d20 7074 2e61 735f  tpoints = pt.as_
+00005c00: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
+00005c10: 6375 7470 6f69 6e74 7329 0a20 2020 2020  cutpoints).     
+00005c20: 2020 206e 203d 2070 742e 6173 5f74 656e     n = pt.as_ten
+00005c30: 736f 725f 7661 7269 6162 6c65 2869 6e74  sor_variable(int
+00005c40: 5828 6e29 290a 0a20 2020 2020 2020 2070  X(n))..        p
+00005c50: 6120 3d20 7369 676d 6f69 6428 6375 7470  a = sigmoid(cutp
+00005c60: 6f69 6e74 7320 2d20 7074 2e73 6861 7065  oints - pt.shape
+00005c70: 5f70 6164 7269 6768 7428 6574 6129 290a  _padright(eta)).
+00005c80: 2020 2020 2020 2020 705f 6375 6d20 3d20          p_cum = 
+00005c90: 7074 2e63 6f6e 6361 7465 6e61 7465 280a  pt.concatenate(.
+00005ca0: 2020 2020 2020 2020 2020 2020 5b0a 2020              [.  
+00005cb0: 2020 2020 2020 2020 2020 2020 2020 7074                pt
+00005cc0: 2e7a 6572 6f73 5f6c 696b 6528 7074 2e73  .zeros_like(pt.s
+00005cd0: 6861 7065 5f70 6164 7269 6768 7428 7061  hape_padright(pa
+00005ce0: 5b2e 2e2e 2c20 305d 2929 2c0a 2020 2020  [..., 0])),.    
+00005cf0: 2020 2020 2020 2020 2020 2020 7061 2c0a              pa,.
+00005d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005d10: 7074 2e6f 6e65 735f 6c69 6b65 2870 742e  pt.ones_like(pt.
+00005d20: 7368 6170 655f 7061 6472 6967 6874 2870  shape_padright(p
+00005d30: 615b 2e2e 2e2c 2030 5d29 292c 0a20 2020  a[..., 0])),.   
+00005d40: 2020 2020 2020 2020 205d 2c0a 2020 2020           ],.    
+00005d50: 2020 2020 2020 2020 6178 6973 3d2d 312c          axis=-1,
+00005d60: 0a20 2020 2020 2020 2029 0a20 2020 2020  .        ).     
+00005d70: 2020 2070 203d 2070 5f63 756d 5b2e 2e2e     p = p_cum[...
+00005d80: 2c20 313a 5d20 2d20 705f 6375 6d5b 2e2e  , 1:] - p_cum[..
+00005d90: 2e2c 203a 2d31 5d0a 0a20 2020 2020 2020  ., :-1]..       
+00005da0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00005db0: 6469 7374 286e 2c20 702c 202a 6172 6773  dist(n, p, *args
+00005dc0: 2c20 2a2a 6b77 6172 6773 290a 0a0a 636c  , **kwargs)...cl
+00005dd0: 6173 7320 4f72 6465 7265 644d 756c 7469  ass OrderedMulti
+00005de0: 6e6f 6d69 616c 3a0a 2020 2020 7222 2222  nomial:.    r"""
+00005df0: 0a20 2020 2057 7261 7070 6572 2063 6c61  .    Wrapper cla
+00005e00: 7373 2066 6f72 204f 7264 6572 6564 204d  ss for Ordered M
+00005e10: 756c 7469 6e6f 6d69 616c 2064 6973 7472  ultinomial distr
+00005e20: 6962 7574 696f 6e73 2e0a 0a20 2020 2055  ibutions...    U
+00005e30: 7365 6675 6c20 666f 7220 7265 6772 6573  seful for regres
+00005e40: 7369 6f6e 206f 6e20 6f72 6469 6e61 6c20  sion on ordinal 
+00005e50: 6461 7461 2077 686f 7365 2076 616c 7565  data whose value
+00005e60: 7320 7261 6e67 650a 2020 2020 6672 6f6d  s range.    from
+00005e70: 2031 2074 6f20 4b20 6173 2061 2066 756e   1 to K as a fun
+00005e80: 6374 696f 6e20 6f66 2073 6f6d 6520 7072  ction of some pr
+00005e90: 6564 6963 746f 722c 203a 6d61 7468 3a60  edictor, :math:`
+00005ea0: 5c65 7461 602c 2062 7574 0a20 2020 2020  \eta`, but.     
+00005eb0: 7768 6963 6820 6172 6520 5f61 6767 7265  which are _aggre
+00005ec0: 6761 7465 645f 2062 7920 7472 6961 6c2c  gated_ by trial,
+00005ed0: 206c 696b 6520 6d75 6c74 696e 6f6d 6961   like multinomia
+00005ee0: 6c20 6f62 7365 7276 6174 696f 6e73 2028  l observations (
+00005ef0: 696e 0a20 2020 2020 636f 6e74 7261 7374  in.     contrast
+00005f00: 2074 6f20 6070 6d2e 4f72 6465 7265 644c   to `pm.OrderedL
+00005f10: 6f67 6973 7469 6360 2c20 7768 6963 6820  ogistic`, which 
+00005f20: 6f6e 6c79 2061 6363 6570 7473 206f 7264  only accepts ord
+00005f30: 696e 616c 2064 6174 610a 2020 2020 2069  inal data.     i
+00005f40: 6e20 6120 5f64 6973 6167 6772 6567 6174  n a _disaggregat
+00005f50: 6564 5f20 666f 726d 6174 2c20 6c69 6b65  ed_ format, like
+00005f60: 2063 6174 6567 6f72 6963 616c 206f 6273   categorical obs
+00005f70: 6572 7661 7469 6f6e 7329 2e0a 2020 2020  ervations)..    
+00005f80: 2054 6865 2063 7574 706f 696e 7473 2c20   The cutpoints, 
+00005f90: 3a6d 6174 683a 6063 602c 2073 6570 6172  :math:`c`, separ
+00005fa0: 6174 6520 7768 6963 6820 7261 6e67 6573  ate which ranges
+00005fb0: 206f 6620 3a6d 6174 683a 605c 6574 6160   of :math:`\eta`
+00005fc0: 2061 7265 0a20 2020 206d 6170 7065 6420   are.    mapped 
+00005fd0: 746f 2077 6869 6368 206f 6620 7468 6520  to which of the 
+00005fe0: 4b20 6f62 7365 7276 6564 2064 6570 656e  K observed depen
+00005ff0: 6465 6e74 2076 6172 6961 626c 6573 2e20  dent variables. 
+00006000: 5468 6520 6e75 6d62 6572 0a20 2020 206f  The number.    o
+00006010: 6620 6375 7470 6f69 6e74 7320 6973 204b  f cutpoints is K
+00006020: 202d 2031 2e20 4974 2069 7320 7265 636f   - 1. It is reco
+00006030: 6d6d 656e 6465 6420 7468 6174 2074 6865  mmended that the
+00006040: 2063 7574 706f 696e 7473 2061 7265 0a20   cutpoints are. 
+00006050: 2020 2063 6f6e 7374 7261 696e 6564 2074     constrained t
+00006060: 6f20 6265 206f 7264 6572 6564 2e0a 0a20  o be ordered... 
+00006070: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
+00006080: 2020 2020 2066 286b 205c 6d69 6420 5c65       f(k \mid \e
+00006090: 7461 2c20 6329 203d 205c 6c65 6674 5c7b  ta, c) = \left\{
+000060a0: 0a20 2020 2020 2020 2020 5c62 6567 696e  .         \begin
+000060b0: 7b61 7272 6179 7d7b 6c7d 0a20 2020 2020  {array}{l}.     
+000060c0: 2020 2020 2020 3120 2d20 5c74 6578 747b        1 - \text{
+000060d0: 6c6f 6769 747d 5e7b 2d31 7d28 5c65 7461  logit}^{-1}(\eta
+000060e0: 202d 2063 5f31 290a 2020 2020 2020 2020   - c_1).        
+000060f0: 2020 2020 205c 2c2c 205c 7465 7874 7b69       \,, \text{i
+00006100: 6620 7d20 6b20 3d20 3020 5c5c 0a20 2020  f } k = 0 \\.   
+00006110: 2020 2020 2020 2020 5c74 6578 747b 6c6f          \text{lo
+00006120: 6769 747d 5e7b 2d31 7d28 5c65 7461 202d  git}^{-1}(\eta -
+00006130: 2063 5f7b 6b20 2d20 317d 2920 2d0a 2020   c_{k - 1}) -.  
+00006140: 2020 2020 2020 2020 205c 7465 7874 7b6c           \text{l
+00006150: 6f67 6974 7d5e 7b2d 317d 285c 6574 6120  ogit}^{-1}(\eta 
+00006160: 2d20 635f 7b6b 7d29 0a20 2020 2020 2020  - c_{k}).       
+00006170: 2020 2020 2020 5c2c 2c20 5c74 6578 747b        \,, \text{
+00006180: 6966 207d 2030 203c 206b 203c 204b 205c  if } 0 < k < K \
+00006190: 5c0a 2020 2020 2020 2020 2020 205c 7465  \.           \te
+000061a0: 7874 7b6c 6f67 6974 7d5e 7b2d 317d 285c  xt{logit}^{-1}(\
+000061b0: 6574 6120 2d20 635f 7b4b 202d 2031 7d29  eta - c_{K - 1})
+000061c0: 0a20 2020 2020 2020 2020 2020 2020 5c2c  .             \,
+000061d0: 2c20 5c74 6578 747b 6966 207d 206b 203d  , \text{if } k =
+000061e0: 204b 205c 5c0a 2020 2020 2020 2020 205c   K \\.         \
+000061f0: 656e 647b 6172 7261 797d 0a20 2020 2020  end{array}.     
+00006200: 2020 5c72 6967 6874 2e0a 0a20 2020 2050    \right...    P
+00006210: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00006220: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2065 7461  --------.    eta
+00006230: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+00006240: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+00006250: 5468 6520 7072 6564 6963 746f 722e 0a20  The predictor.. 
+00006260: 2020 2063 7574 706f 696e 7473 203a 2074     cutpoints : t
+00006270: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
+00006280: 6f61 740a 2020 2020 2020 2020 5468 6520  oat.        The 
+00006290: 6c65 6e67 7468 204b 202d 2031 2061 7272  length K - 1 arr
+000062a0: 6179 206f 6620 6375 7470 6f69 6e74 7320  ay of cutpoints 
+000062b0: 7768 6963 6820 6272 6561 6b20 3a6d 6174  which break :mat
+000062c0: 683a 605c 6574 6160 2069 6e74 6f0a 2020  h:`\eta` into.  
+000062d0: 2020 2020 2020 7261 6e67 6573 2e20 446f        ranges. Do
+000062e0: 206e 6f74 2065 7870 6c69 6369 746c 7920   not explicitly 
+000062f0: 7365 7420 7468 6520 6669 7273 7420 616e  set the first an
+00006300: 6420 6c61 7374 2065 6c65 6d65 6e74 7320  d last elements 
+00006310: 6f66 0a20 2020 2020 2020 203a 6d61 7468  of.        :math
+00006320: 3a60 6360 2074 6f20 6e65 6761 7469 7665  :`c` to negative
+00006330: 2061 6e64 2070 6f73 6974 6976 6520 696e   and positive in
+00006340: 6669 6e69 7479 2e0a 2020 2020 6e20 3a20  finity..    n : 
+00006350: 7465 6e73 6f72 5f6c 696b 6520 6f66 2069  tensor_like of i
+00006360: 6e74 0a20 2020 2020 2020 2054 6865 2074  nt.        The t
+00006370: 6f74 616c 206e 756d 6265 7220 6f66 206d  otal number of m
+00006380: 756c 7469 6e6f 6d69 616c 2074 7269 616c  ultinomial trial
+00006390: 732e 0a20 2020 2063 6f6d 7075 7465 5f70  s..    compute_p
+000063a0: 203a 2062 6f6f 6c65 616e 2c20 6465 6661   : boolean, defa
+000063b0: 756c 743d 5472 7565 0a20 2020 2020 2020  ult=True.       
+000063c0: 2057 6865 7468 6572 2074 6f20 636f 6d70   Whether to comp
+000063d0: 7574 6520 616e 6420 7374 6f72 6520 696e  ute and store in
+000063e0: 2074 6865 2074 7261 6365 2074 6865 2069   the trace the i
+000063f0: 6e66 6572 7265 6420 7072 6f62 6162 696c  nferred probabil
+00006400: 6974 6965 7320 6f66 2065 6163 680a 2020  ities of each.  
+00006410: 2020 2020 2020 6361 7465 676f 7269 6573        categories
+00006420: 2c0a 2020 2020 2020 2020 6261 7365 6420  ,.        based 
+00006430: 6f6e 2074 6865 2063 7574 706f 696e 7473  on the cutpoints
+00006440: 2720 7661 6c75 6573 2e20 4465 6661 756c  ' values. Defaul
+00006450: 7473 2074 6f20 5472 7565 2e0a 2020 2020  ts to True..    
+00006460: 2020 2020 4d69 6768 7420 6265 2075 7365      Might be use
+00006470: 6675 6c20 746f 2064 6973 6162 6c65 2069  ful to disable i
+00006480: 7420 6966 206d 656d 6f72 7920 7573 6167  t if memory usag
+00006490: 6520 6973 206f 6620 696e 7465 7265 7374  e is of interest
+000064a0: 2e0a 0a20 2020 2045 7861 6d70 6c65 730a  ...    Examples.
+000064b0: 2020 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020      --------.   
+000064c0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
+000064d0: 2070 7974 686f 6e0a 0a20 2020 2020 2020   python..       
+000064e0: 2023 2047 656e 6572 6174 6520 6461 7461   # Generate data
+000064f0: 2066 6f72 2061 2073 696d 706c 6520 3120   for a simple 1 
+00006500: 6469 6d65 6e73 696f 6e61 6c20 6578 616d  dimensional exam
+00006510: 706c 6520 7072 6f62 6c65 6d0a 2020 2020  ple problem.    
+00006520: 2020 2020 7472 7565 5f63 756d 5f70 203d      true_cum_p =
+00006530: 206e 702e 6172 7261 7928 5b30 2e31 2c20   np.array([0.1, 
+00006540: 302e 3135 2c20 302e 3235 2c20 302e 3530  0.15, 0.25, 0.50
+00006550: 2c20 302e 3635 2c20 302e 3930 2c20 312e  , 0.65, 0.90, 1.
+00006560: 305d 290a 2020 2020 2020 2020 7472 7565  0]).        true
+00006570: 5f70 203d 206e 702e 6873 7461 636b 285b  _p = np.hstack([
+00006580: 7472 7565 5f63 756d 5f70 5b30 5d2c 2074  true_cum_p[0], t
+00006590: 7275 655f 6375 6d5f 705b 313a 5d20 2d20  rue_cum_p[1:] - 
+000065a0: 7472 7565 5f63 756d 5f70 5b3a 2d31 5d5d  true_cum_p[:-1]]
+000065b0: 290a 2020 2020 2020 2020 6661 6b65 5f65  ).        fake_e
+000065c0: 6c65 6374 696f 6e73 203d 206e 702e 7261  lections = np.ra
+000065d0: 6e64 6f6d 2e6d 756c 7469 6e6f 6d69 616c  ndom.multinomial
+000065e0: 286e 3d31 5f30 3030 2c20 7076 616c 733d  (n=1_000, pvals=
+000065f0: 7472 7565 5f70 2c20 7369 7a65 3d36 3029  true_p, size=60)
+00006600: 0a0a 2020 2020 2020 2020 2320 4f72 6465  ..        # Orde
+00006610: 7265 6420 6d75 6c74 696e 6f6d 6961 6c20  red multinomial 
+00006620: 7265 6772 6573 7369 6f6e 0a20 2020 2020  regression.     
+00006630: 2020 2077 6974 6820 706d 2e4d 6f64 656c     with pm.Model
+00006640: 2829 2061 7320 6d6f 6465 6c3a 0a20 2020  () as model:.   
+00006650: 2020 2020 2020 2020 2063 7574 706f 696e           cutpoin
+00006660: 7473 203d 2070 6d2e 4e6f 726d 616c 280a  ts = pm.Normal(.
+00006670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006680: 2263 7574 706f 696e 7473 222c 0a20 2020  "cutpoints",.   
+00006690: 2020 2020 2020 2020 2020 2020 206d 753d               mu=
+000066a0: 6e70 2e61 7261 6e67 6528 3629 202d 2032  np.arange(6) - 2
+000066b0: 2e35 2c0a 2020 2020 2020 2020 2020 2020  .5,.            
+000066c0: 2020 2020 7369 676d 613d 312e 352c 0a20      sigma=1.5,. 
+000066d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+000066e0: 6e69 7476 616c 3d6e 702e 6172 616e 6765  nitval=np.arange
+000066f0: 2836 2920 2d20 322e 352c 0a20 2020 2020  (6) - 2.5,.     
+00006700: 2020 2020 2020 2020 2020 2074 7261 6e73             trans
+00006710: 666f 726d 3d70 6d2e 6469 7374 7269 6275  form=pm.distribu
+00006720: 7469 6f6e 732e 7472 616e 7366 6f72 6d73  tions.transforms
+00006730: 2e6f 7264 6572 6564 2c0a 2020 2020 2020  .ordered,.      
+00006740: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00006750: 2020 2020 2070 6d2e 4f72 6465 7265 644d       pm.OrderedM
+00006760: 756c 7469 6e6f 6d69 616c 280a 2020 2020  ultinomial(.    
+00006770: 2020 2020 2020 2020 2020 2020 2272 6573              "res
+00006780: 756c 7473 222c 0a20 2020 2020 2020 2020  ults",.         
+00006790: 2020 2020 2020 2065 7461 3d30 2e30 2c0a         eta=0.0,.
+000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000067b0: 6375 7470 6f69 6e74 733d 6375 7470 6f69  cutpoints=cutpoi
+000067c0: 6e74 732c 0a20 2020 2020 2020 2020 2020  nts,.           
+000067d0: 2020 2020 206e 3d66 616b 655f 656c 6563       n=fake_elec
+000067e0: 7469 6f6e 732e 7375 6d28 3129 2c0a 2020  tions.sum(1),.  
+000067f0: 2020 2020 2020 2020 2020 2020 2020 6f62                ob
+00006800: 7365 7276 6564 3d66 616b 655f 656c 6563  served=fake_elec
+00006810: 7469 6f6e 732c 0a20 2020 2020 2020 2020  tions,.         
+00006820: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
+00006830: 2020 7472 6163 6520 3d20 706d 2e73 616d    trace = pm.sam
+00006840: 706c 6528 290a 0a20 2020 2020 2020 2023  ple()..        #
+00006850: 2050 6c6f 7420 7468 6520 7265 7375 6c74   Plot the result
+00006860: 730a 2020 2020 2020 2020 6172 7669 7a2e  s.        arviz.
+00006870: 706c 6f74 5f70 6f73 7465 7269 6f72 2874  plot_posterior(t
+00006880: 7261 6365 5f31 325f 342c 2076 6172 5f6e  race_12_4, var_n
+00006890: 616d 6573 3d5b 2263 6f6d 706c 6574 655f  ames=["complete_
+000068a0: 7022 5d2c 2072 6566 5f76 616c 3d6c 6973  p"], ref_val=lis
+000068b0: 7428 7472 7565 5f70 2929 3b0a 2020 2020  t(true_p));.    
+000068c0: 2222 220a 0a20 2020 2064 6566 205f 5f6e  """..    def __n
+000068d0: 6577 5f5f 2863 6c73 2c20 6e61 6d65 2c20  ew__(cls, name, 
+000068e0: 2a61 7267 732c 2063 6f6d 7075 7465 5f70  *args, compute_p
+000068f0: 3d54 7275 652c 202a 2a6b 7761 7267 7329  =True, **kwargs)
+00006900: 3a0a 2020 2020 2020 2020 6f75 745f 7276  :.        out_rv
+00006910: 203d 205f 4f72 6465 7265 644d 756c 7469   = _OrderedMulti
+00006920: 6e6f 6d69 616c 286e 616d 652c 202a 6172  nomial(name, *ar
+00006930: 6773 2c20 2a2a 6b77 6172 6773 290a 2020  gs, **kwargs).  
+00006940: 2020 2020 2020 6966 2063 6f6d 7075 7465        if compute
+00006950: 5f70 3a0a 2020 2020 2020 2020 2020 2020  _p:.            
+00006960: 706d 2e44 6574 6572 6d69 6e69 7374 6963  pm.Deterministic
+00006970: 2866 227b 6e61 6d65 7d5f 7072 6f62 7322  (f"{name}_probs"
+00006980: 2c20 6f75 745f 7276 2e6f 776e 6572 2e69  , out_rv.owner.i
+00006990: 6e70 7574 735b 345d 2c20 6469 6d73 3d6b  nputs[4], dims=k
+000069a0: 7761 7267 732e 6765 7428 2264 696d 7322  wargs.get("dims"
+000069b0: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
+000069c0: 6e20 6f75 745f 7276 0a0a 2020 2020 4063  n out_rv..    @c
+000069d0: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+000069e0: 6566 2064 6973 7428 636c 732c 202a 6172  ef dist(cls, *ar
+000069f0: 6773 2c20 2a2a 6b77 6172 6773 293a 0a20  gs, **kwargs):. 
+00006a00: 2020 2020 2020 2072 6574 7572 6e20 5f4f         return _O
+00006a10: 7264 6572 6564 4d75 6c74 696e 6f6d 6961  rderedMultinomia
+00006a20: 6c2e 6469 7374 282a 6172 6773 2c20 2a2a  l.dist(*args, **
+00006a30: 6b77 6172 6773 290a 0a0a 6465 6620 706f  kwargs)...def po
+00006a40: 7364 6566 2841 4129 3a0a 2020 2020 7472  sdef(AA):.    tr
+00006a50: 793a 0a20 2020 2020 2020 206c 696e 616c  y:.        linal
+00006a60: 672e 6368 6f6c 6573 6b79 2841 4129 0a20  g.cholesky(AA). 
+00006a70: 2020 2020 2020 2072 6574 7572 6e20 310a         return 1.
+00006a80: 2020 2020 6578 6365 7074 206c 696e 616c      except linal
+00006a90: 672e 4c69 6e41 6c67 4572 726f 723a 0a20  g.LinAlgError:. 
+00006aa0: 2020 2020 2020 2072 6574 7572 6e20 300a         return 0.
+00006ab0: 0a0a 636c 6173 7320 506f 7344 6566 4d61  ..class PosDefMa
+00006ac0: 7472 6978 284f 7029 3a0a 2020 2020 2222  trix(Op):.    ""
+00006ad0: 220a 2020 2020 4368 6563 6b20 6966 2069  ".    Check if i
+00006ae0: 6e70 7574 2069 7320 706f 7369 7469 7665  nput is positive
+00006af0: 2064 6566 696e 6974 652e 2049 6e70 7574   definite. Input
+00006b00: 2073 686f 756c 6420 6265 2061 2073 7175   should be a squ
+00006b10: 6172 6520 6d61 7472 6978 2e0a 0a20 2020  are matrix...   
+00006b20: 2022 2222 0a0a 2020 2020 2320 5072 6f70   """..    # Prop
+00006b30: 6572 7469 6573 2061 7474 7269 6275 7465  erties attribute
+00006b40: 0a20 2020 205f 5f70 726f 7073 5f5f 203d  .    __props__ =
+00006b50: 2028 290a 0a20 2020 2023 2043 6f6d 7075   ()..    # Compu
+00006b60: 6c73 6f72 7920 6966 2069 7479 7065 7320  lsory if itypes 
+00006b70: 616e 6420 6f74 7970 6573 2061 7265 206e  and otypes are n
+00006b80: 6f74 2064 6566 696e 6564 0a0a 2020 2020  ot defined..    
+00006b90: 6465 6620 6d61 6b65 5f6e 6f64 6528 7365  def make_node(se
+00006ba0: 6c66 2c20 7829 3a0a 2020 2020 2020 2020  lf, x):.        
+00006bb0: 7820 3d20 7074 2e61 735f 7465 6e73 6f72  x = pt.as_tensor
+00006bc0: 5f76 6172 6961 626c 6528 7829 0a20 2020  _variable(x).   
+00006bd0: 2020 2020 2061 7373 6572 7420 782e 6e64       assert x.nd
+00006be0: 696d 203d 3d20 320a 2020 2020 2020 2020  im == 2.        
+00006bf0: 6f20 3d20 5465 6e73 6f72 5479 7065 2864  o = TensorType(d
+00006c00: 7479 7065 3d22 696e 7438 222c 2073 6861  type="int8", sha
+00006c10: 7065 3d5b 5d29 2829 0a20 2020 2020 2020  pe=[])().       
+00006c20: 2072 6574 7572 6e20 4170 706c 7928 7365   return Apply(se
+00006c30: 6c66 2c20 5b78 5d2c 205b 6f5d 290a 0a20  lf, [x], [o]).. 
+00006c40: 2020 2023 2050 7974 686f 6e20 696d 706c     # Python impl
+00006c50: 656d 656e 7461 7469 6f6e 3a0a 2020 2020  ementation:.    
+00006c60: 6465 6620 7065 7266 6f72 6d28 7365 6c66  def perform(self
+00006c70: 2c20 6e6f 6465 2c20 696e 7075 7473 2c20  , node, inputs, 
+00006c80: 6f75 7470 7574 7329 3a0a 2020 2020 2020  outputs):.      
+00006c90: 2020 2878 2c29 203d 2069 6e70 7574 730a    (x,) = inputs.
+00006ca0: 2020 2020 2020 2020 287a 2c29 203d 206f          (z,) = o
+00006cb0: 7574 7075 7473 0a20 2020 2020 2020 2074  utputs.        t
+00006cc0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
+00006cd0: 7a5b 305d 203d 206e 702e 6172 7261 7928  z[0] = np.array(
+00006ce0: 706f 7364 6566 2878 292c 2064 7479 7065  posdef(x), dtype
+00006cf0: 3d22 696e 7438 2229 0a20 2020 2020 2020  ="int8").       
+00006d00: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+00006d10: 6e3a 0a20 2020 2020 2020 2020 2020 2070  n:.            p
+00006d20: 6d2e 5f6c 6f67 2e65 7863 6570 7469 6f6e  m._log.exception
+00006d30: 2822 4661 696c 6564 2074 6f20 6368 6563  ("Failed to chec
+00006d40: 6b20 6966 2025 7320 706f 7369 7469 7665  k if %s positive
+00006d50: 2064 6566 696e 6974 6522 2c20 7829 0a20   definite", x). 
+00006d60: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00006d70: 0a0a 2020 2020 6465 6620 696e 6665 725f  ..    def infer_
+00006d80: 7368 6170 6528 7365 6c66 2c20 6667 7261  shape(self, fgra
+00006d90: 7068 2c20 6e6f 6465 2c20 7368 6170 6573  ph, node, shapes
+00006da0: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
+00006db0: 6e20 5b5b 5d5d 0a0a 2020 2020 6465 6620  n [[]]..    def 
+00006dc0: 6772 6164 2873 656c 662c 2069 6e70 2c20  grad(self, inp, 
+00006dd0: 6772 6164 7329 3a0a 2020 2020 2020 2020  grads):.        
+00006de0: 2878 2c29 203d 2069 6e70 0a20 2020 2020  (x,) = inp.     
+00006df0: 2020 2072 6574 7572 6e20 5b78 2e7a 6572     return [x.zer
+00006e00: 6f73 5f6c 696b 6528 7079 7465 6e73 6f72  os_like(pytensor
+00006e10: 2e63 6f6e 6669 672e 666c 6f61 7458 295d  .config.floatX)]
+00006e20: 0a0a 2020 2020 6465 6620 5f5f 7374 725f  ..    def __str_
+00006e30: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00006e40: 2072 6574 7572 6e20 224d 6174 7269 7849   return "MatrixI
+00006e50: 7350 6f73 6974 6976 6544 6566 696e 6974  sPositiveDefinit
+00006e60: 6522 0a0a 0a6d 6174 7269 785f 706f 735f  e"...matrix_pos_
+00006e70: 6465 6620 3d20 506f 7344 6566 4d61 7472  def = PosDefMatr
+00006e80: 6978 2829 0a0a 0a63 6c61 7373 2057 6973  ix()...class Wis
+00006e90: 6861 7274 5256 2852 616e 646f 6d56 6172  hartRV(RandomVar
+00006ea0: 6961 626c 6529 3a0a 2020 2020 6e61 6d65  iable):.    name
+00006eb0: 203d 2022 7769 7368 6172 7422 0a20 2020   = "wishart".   
+00006ec0: 206e 6469 6d5f 7375 7070 203d 2032 0a20   ndim_supp = 2. 
+00006ed0: 2020 206e 6469 6d73 5f70 6172 616d 7320     ndims_params 
+00006ee0: 3d20 5b30 2c20 325d 0a20 2020 2064 7479  = [0, 2].    dty
+00006ef0: 7065 203d 2022 666c 6f61 7458 220a 2020  pe = "floatX".  
+00006f00: 2020 5f70 7269 6e74 5f6e 616d 6520 3d20    _print_name = 
+00006f10: 2822 5769 7368 6172 7422 2c20 225c 5c6f  ("Wishart", "\\o
+00006f20: 7065 7261 746f 726e 616d 657b 5769 7368  peratorname{Wish
+00006f30: 6172 747d 2229 0a0a 2020 2020 6465 6620  art}")..    def 
+00006f40: 5f73 7570 705f 7368 6170 655f 6672 6f6d  _supp_shape_from
+00006f50: 5f70 6172 616d 7328 7365 6c66 2c20 6469  _params(self, di
+00006f60: 7374 5f70 6172 616d 732c 2072 6570 5f70  st_params, rep_p
+00006f70: 6172 616d 5f69 6478 3d31 2c20 7061 7261  aram_idx=1, para
+00006f80: 6d5f 7368 6170 6573 3d4e 6f6e 6529 3a0a  m_shapes=None):.
+00006f90: 2020 2020 2020 2020 2320 5468 6520 7368          # The sh
+00006fa0: 6170 6520 6f66 2073 6563 6f6e 6420 7061  ape of second pa
+00006fb0: 7261 6d65 7465 7220 6056 6020 6465 6669  rameter `V` defi
+00006fc0: 6e65 7320 7468 6520 7368 6170 6520 6f66  nes the shape of
+00006fd0: 2074 6865 206f 7574 7075 742e 0a20 2020   the output..   
+00006fe0: 2020 2020 2072 6574 7572 6e20 6469 7374       return dist
+00006ff0: 5f70 6172 616d 735b 315d 2e73 6861 7065  _params[1].shape
+00007000: 5b2d 323a 5d0a 0a20 2020 2040 636c 6173  [-2:]..    @clas
+00007010: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00007020: 726e 675f 666e 2863 6c73 2c20 726e 672c  rng_fn(cls, rng,
+00007030: 206e 752c 2056 2c20 7369 7a65 293a 0a20   nu, V, size):. 
+00007040: 2020 2020 2020 2073 6369 7079 5f73 697a         scipy_siz
+00007050: 6520 3d20 7369 7a65 2069 6620 7369 7a65  e = size if size
+00007060: 2065 6c73 6520 3120 2023 2044 6566 6175   else 1  # Defau
+00007070: 6c74 2073 697a 6520 666f 7220 5363 6970  lt size for Scip
+00007080: 7927 7320 7769 7368 6172 742e 7276 7320  y's wishart.rvs 
+00007090: 6973 2031 0a20 2020 2020 2020 2072 6573  is 1.        res
+000070a0: 756c 7420 3d20 7374 6174 732e 7769 7368  ult = stats.wish
+000070b0: 6172 742e 7276 7328 696e 7428 6e75 292c  art.rvs(int(nu),
+000070c0: 2056 2c20 7369 7a65 3d73 6369 7079 5f73   V, size=scipy_s
+000070d0: 697a 652c 2072 616e 646f 6d5f 7374 6174  ize, random_stat
+000070e0: 653d 726e 6729 0a20 2020 2020 2020 2069  e=rng).        i
+000070f0: 6620 7369 7a65 203d 3d20 2831 2c29 3a0a  f size == (1,):.
+00007100: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00007110: 726e 2072 6573 756c 745b 6e70 2e6e 6577  rn result[np.new
+00007120: 6178 6973 2c20 2e2e 2e5d 0a20 2020 2020  axis, ...].     
+00007130: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00007140: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00007150: 6c74 0a0a 0a77 6973 6861 7274 203d 2057  lt...wishart = W
+00007160: 6973 6861 7274 5256 2829 0a0a 0a63 6c61  ishartRV()...cla
+00007170: 7373 2057 6973 6861 7274 2843 6f6e 7469  ss Wishart(Conti
+00007180: 6e75 6f75 7329 3a0a 2020 2020 7222 2222  nuous):.    r"""
+00007190: 0a20 2020 2057 6973 6861 7274 206c 6f67  .    Wishart log
+000071a0: 2d6c 696b 656c 6968 6f6f 642e 0a0a 2020  -likelihood...  
+000071b0: 2020 5468 6520 5769 7368 6172 7420 6469    The Wishart di
+000071c0: 7374 7269 6275 7469 6f6e 2069 7320 7468  stribution is th
+000071d0: 6520 7072 6f62 6162 696c 6974 7920 6469  e probability di
+000071e0: 7374 7269 6275 7469 6f6e 206f 6620 7468  stribution of th
+000071f0: 650a 2020 2020 6d61 7869 6d75 6d2d 6c69  e.    maximum-li
+00007200: 6b65 6c69 686f 6f64 2065 7374 696d 6174  kelihood estimat
+00007210: 6f72 2028 4d4c 4529 206f 6620 7468 6520  or (MLE) of the 
+00007220: 7072 6563 6973 696f 6e20 6d61 7472 6978  precision matrix
+00007230: 206f 6620 610a 2020 2020 6d75 6c74 6976   of a.    multiv
+00007240: 6172 6961 7465 206e 6f72 6d61 6c20 6469  ariate normal di
+00007250: 7374 7269 6275 7469 6f6e 2e20 2049 6620  stribution.  If 
+00007260: 563d 312c 2074 6865 2064 6973 7472 6962  V=1, the distrib
+00007270: 7574 696f 6e20 6973 0a20 2020 2069 6465  ution is.    ide
+00007280: 6e74 6963 616c 2074 6f20 7468 6520 6368  ntical to the ch
+00007290: 692d 7371 7561 7265 2064 6973 7472 6962  i-square distrib
+000072a0: 7574 696f 6e20 7769 7468 206e 7520 6465  ution with nu de
+000072b0: 6772 6565 7320 6f66 0a20 2020 2066 7265  grees of.    fre
+000072c0: 6564 6f6d 2e0a 0a20 2020 202e 2e20 6d61  edom...    .. ma
+000072d0: 7468 3a3a 0a0a 2020 2020 2020 2066 2858  th::..       f(X
+000072e0: 205c 6d69 6420 6e75 2c20 5429 203d 0a20   \mid nu, T) =. 
+000072f0: 2020 2020 2020 2020 2020 5c66 7261 637b            \frac{
+00007300: 7b5c 6d69 6420 5420 5c6d 6964 7d5e 7b6e  {\mid T \mid}^{n
+00007310: 752f 327d 7b5c 6d69 6420 5820 5c6d 6964  u/2}{\mid X \mid
+00007320: 7d5e 7b28 6e75 2d6b 2d31 292f 327d 7d7b  }^{(nu-k-1)/2}}{
+00007330: 325e 7b6e 7520 6b2f 327d 0a20 2020 2020  2^{nu k/2}.     
+00007340: 2020 2020 2020 5c47 616d 6d61 5f70 286e        \Gamma_p(n
+00007350: 752f 3229 7d20 5c65 7870 5c6c 6566 745c  u/2)} \exp\left\
+00007360: 7b20 2d5c 6672 6163 7b31 7d7b 327d 2054  { -\frac{1}{2} T
+00007370: 7228 5458 2920 5c72 6967 6874 5c7d 0a0a  r(TX) \right\}..
+00007380: 2020 2020 7768 6572 6520 3a6d 6174 683a      where :math:
+00007390: 606b 6020 6973 2074 6865 2072 616e 6b20  `k` is the rank 
+000073a0: 6f66 203a 6d61 7468 3a60 5860 2e0a 0a20  of :math:`X`... 
+000073b0: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
+000073c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000073d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000073e0: 3d3d 3d3d 3d3d 0a20 2020 2053 7570 706f  ======.    Suppo
+000073f0: 7274 2020 203a 6d61 7468 3a60 5828 7020  rt   :math:`X(p 
+00007400: 7820 7029 6020 706f 7369 7469 7665 2064  x p)` positive d
+00007410: 6566 696e 6974 6520 6d61 7472 6978 0a20  efinite matrix. 
+00007420: 2020 204d 6561 6e20 2020 2020 203a 6d61     Mean      :ma
+00007430: 7468 3a60 6e75 2056 600a 2020 2020 5661  th:`nu V`.    Va
+00007440: 7269 616e 6365 2020 3a6d 6174 683a 606e  riance  :math:`n
+00007450: 7520 2876 5f7b 696a 7d5e 3220 2b20 765f  u (v_{ij}^2 + v_
+00007460: 7b69 697d 2076 5f7b 6a6a 7d29 600a 2020  {ii} v_{jj})`.  
+00007470: 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d    ========  ====
+00007480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00007490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000074a0: 3d3d 3d3d 3d0a 0a20 2020 2050 6172 616d  =====..    Param
+000074b0: 6574 6572 730a 2020 2020 2d2d 2d2d 2d2d  eters.    ------
+000074c0: 2d2d 2d2d 0a20 2020 206e 7520 3a20 7465  ----.    nu : te
+000074d0: 6e73 6f72 5f6c 696b 6520 6f66 2069 6e74  nsor_like of int
+000074e0: 0a20 2020 2020 2020 2044 6567 7265 6573  .        Degrees
+000074f0: 206f 6620 6672 6565 646f 6d2c 203e 2030   of freedom, > 0
+00007500: 2e0a 2020 2020 5620 3a20 7465 6e73 6f72  ..    V : tensor
+00007510: 5f6c 696b 6520 6f66 2066 6c6f 6174 0a20  _like of float. 
+00007520: 2020 2020 2020 2070 2078 2070 2070 6f73         p x p pos
+00007530: 6974 6976 6520 6465 6669 6e69 7465 206d  itive definite m
+00007540: 6174 7269 782e 0a0a 2020 2020 4e6f 7465  atrix...    Note
+00007550: 730a 2020 2020 2d2d 2d2d 2d0a 2020 2020  s.    -----.    
+00007560: 5468 6973 2064 6973 7472 6962 7574 696f  This distributio
+00007570: 6e20 6973 2075 6e75 7361 626c 6520 696e  n is unusable in
+00007580: 2061 2050 794d 4320 6d6f 6465 6c2e 2059   a PyMC model. Y
+00007590: 6f75 2073 686f 756c 6420 696e 7374 6561  ou should instea
+000075a0: 640a 2020 2020 7573 6520 4c4b 4a43 686f  d.    use LKJCho
+000075b0: 6c65 736b 7943 6f76 206f 7220 4c4b 4a43  leskyCov or LKJC
+000075c0: 6f72 722e 0a20 2020 2022 2222 0a20 2020  orr..    """.   
+000075d0: 2072 765f 6f70 203d 2077 6973 6861 7274   rv_op = wishart
+000075e0: 0a0a 2020 2020 4063 6c61 7373 6d65 7468  ..    @classmeth
+000075f0: 6f64 0a20 2020 2064 6566 2064 6973 7428  od.    def dist(
+00007600: 636c 732c 206e 752c 2056 2c20 2a61 7267  cls, nu, V, *arg
+00007610: 732c 202a 2a6b 7761 7267 7329 3a0a 2020  s, **kwargs):.  
+00007620: 2020 2020 2020 6e75 203d 2070 742e 6173        nu = pt.as
+00007630: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00007640: 2869 6e74 5828 6e75 2929 0a20 2020 2020  (intX(nu)).     
+00007650: 2020 2056 203d 2070 742e 6173 5f74 656e     V = pt.as_ten
+00007660: 736f 725f 7661 7269 6162 6c65 2866 6c6f  sor_variable(flo
+00007670: 6174 5828 5629 290a 0a20 2020 2020 2020  atX(V))..       
+00007680: 2077 6172 6e69 6e67 732e 7761 726e 280a   warnings.warn(.
+00007690: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+000076a0: 2057 6973 6861 7274 2064 6973 7472 6962   Wishart distrib
+000076b0: 7574 696f 6e20 6361 6e20 6375 7272 656e  ution can curren
+000076c0: 746c 7920 6e6f 7420 6265 2075 7365 6420  tly not be used 
+000076d0: 220a 2020 2020 2020 2020 2020 2020 2266  ".            "f
+000076e0: 6f72 204d 434d 4320 7361 6d70 6c69 6e67  or MCMC sampling
+000076f0: 2e20 5468 6520 7072 6f62 6162 696c 6974  . The probabilit
+00007700: 7920 6f66 2073 616d 706c 696e 6720 6120  y of sampling a 
+00007710: 220a 2020 2020 2020 2020 2020 2020 2273  ".            "s
+00007720: 796d 6d65 7472 6963 206d 6174 7269 7820  ymmetric matrix 
+00007730: 6973 2062 6173 6963 616c 6c79 207a 6572  is basically zer
+00007740: 6f2e 2049 6e73 7465 6164 2c20 706c 6561  o. Instead, plea
+00007750: 7365 2022 0a20 2020 2020 2020 2020 2020  se ".           
+00007760: 2022 7573 6520 4c4b 4a43 686f 6c65 736b   "use LKJCholesk
+00007770: 7943 6f76 206f 7220 4c4b 4a43 6f72 722e  yCov or LKJCorr.
+00007780: 2046 6f72 206d 6f72 6520 696e 666f 726d   For more inform
+00007790: 6174 696f 6e20 220a 2020 2020 2020 2020  ation ".        
+000077a0: 2020 2020 226f 6e20 7468 6520 6973 7375      "on the issu
+000077b0: 6573 2073 7572 726f 756e 6469 6e67 2074  es surrounding t
+000077c0: 6865 2057 6973 6861 7274 2073 6565 2068  he Wishart see h
+000077d0: 6572 653a 2022 0a20 2020 2020 2020 2020  ere: ".         
+000077e0: 2020 2022 6874 7470 733a 2f2f 6769 7468     "https://gith
+000077f0: 7562 2e63 6f6d 2f70 796d 632d 6465 7673  ub.com/pymc-devs
+00007800: 2f70 796d 632f 6973 7375 6573 2f35 3338  /pymc/issues/538
+00007810: 2e22 2c0a 2020 2020 2020 2020 2020 2020  .",.            
+00007820: 5573 6572 5761 726e 696e 672c 0a20 2020  UserWarning,.   
+00007830: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+00007840: 2320 6d65 616e 203d 206e 7520 2a20 560a  # mean = nu * V.
+00007850: 2020 2020 2020 2020 2320 7020 3d20 562e          # p = V.
+00007860: 7368 6170 655b 305d 0a20 2020 2020 2020  shape[0].       
+00007870: 2023 206d 6f64 6520 3d20 7074 2e73 7769   # mode = pt.swi
+00007880: 7463 6828 7074 2e67 6528 6e75 2c20 7020  tch(pt.ge(nu, p 
+00007890: 2b20 3129 2c20 286e 7520 2d20 7020 2d20  + 1), (nu - p - 
+000078a0: 3129 202a 2056 2c20 6e70 2e6e 616e 290a  1) * V, np.nan).
+000078b0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+000078c0: 7570 6572 2829 2e64 6973 7428 5b6e 752c  uper().dist([nu,
+000078d0: 2056 5d2c 202a 6172 6773 2c20 2a2a 6b77   V], *args, **kw
+000078e0: 6172 6773 290a 0a20 2020 2064 6566 206c  args)..    def l
+000078f0: 6f67 7028 582c 206e 752c 2056 293a 0a20  ogp(X, nu, V):. 
+00007900: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007910: 2020 2043 616c 6375 6c61 7465 206c 6f67     Calculate log
+00007920: 2d70 726f 6261 6269 6c69 7479 206f 6620  -probability of 
+00007930: 5769 7368 6172 7420 6469 7374 7269 6275  Wishart distribu
+00007940: 7469 6f6e 0a20 2020 2020 2020 2061 7420  tion.        at 
+00007950: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
+00007960: 0a0a 2020 2020 2020 2020 5061 7261 6d65  ..        Parame
+00007970: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
+00007980: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00007990: 583a 206e 756d 6572 6963 0a20 2020 2020  X: numeric.     
+000079a0: 2020 2020 2020 2056 616c 7565 2066 6f72         Value for
+000079b0: 2077 6869 6368 206c 6f67 2d70 726f 6261   which log-proba
+000079c0: 6269 6c69 7479 2069 7320 6361 6c63 756c  bility is calcul
+000079d0: 6174 6564 2e0a 0a20 2020 2020 2020 2052  ated...        R
+000079e0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+000079f0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2054  ------.        T
+00007a00: 656e 736f 7256 6172 6961 626c 650a 2020  ensorVariable.  
+00007a10: 2020 2020 2020 2222 220a 0a20 2020 2020        """..     
+00007a20: 2020 2070 203d 2056 2e73 6861 7065 5b30     p = V.shape[0
+00007a30: 5d0a 0a20 2020 2020 2020 2049 5649 203d  ]..        IVI =
+00007a40: 2064 6574 2856 290a 2020 2020 2020 2020   det(V).        
+00007a50: 4958 4920 3d20 6465 7428 5829 0a0a 2020  IXI = det(X)..  
+00007a60: 2020 2020 2020 7265 7475 726e 2063 6865        return che
+00007a70: 636b 5f70 6172 616d 6574 6572 7328 0a20  ck_parameters(. 
+00007a80: 2020 2020 2020 2020 2020 2028 0a20 2020             (.   
+00007a90: 2020 2020 2020 2020 2020 2020 2028 6e75               (nu
+00007aa0: 202d 2070 202d 2031 2920 2a20 7074 2e6c   - p - 1) * pt.l
+00007ab0: 6f67 2849 5849 290a 2020 2020 2020 2020  og(IXI).        
+00007ac0: 2020 2020 2020 2020 2d20 7472 6163 6528          - trace(
+00007ad0: 6d61 7472 6978 5f69 6e76 6572 7365 2856  matrix_inverse(V
+00007ae0: 292e 646f 7428 5829 290a 2020 2020 2020  ).dot(X)).      
+00007af0: 2020 2020 2020 2020 2020 2d20 6e75 202a            - nu *
+00007b00: 2070 202a 2070 742e 6c6f 6728 3229 0a20   p * pt.log(2). 
+00007b10: 2020 2020 2020 2020 2020 2020 2020 202d                 -
+00007b20: 206e 7520 2a20 7074 2e6c 6f67 2849 5649   nu * pt.log(IVI
+00007b30: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00007b40: 2020 2d20 3220 2a20 6d75 6c74 6967 616d    - 2 * multigam
+00007b50: 6d61 6c6e 286e 7520 2f20 322e 302c 2070  maln(nu / 2.0, p
+00007b60: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00007b70: 2020 2020 2020 2020 2020 2020 2f20 322c              / 2,
+00007b80: 0a20 2020 2020 2020 2020 2020 206d 6174  .            mat
+00007b90: 7269 785f 706f 735f 6465 6628 5829 2c0a  rix_pos_def(X),.
+00007ba0: 2020 2020 2020 2020 2020 2020 7074 2e65              pt.e
+00007bb0: 7128 582c 2058 2e54 292c 0a20 2020 2020  q(X, X.T),.     
+00007bc0: 2020 2020 2020 206e 7520 3e20 2870 202d         nu > (p -
+00007bd0: 2031 292c 0a20 2020 2020 2020 2029 0a0a   1),.        )..
+00007be0: 0a64 6566 2057 6973 6861 7274 4261 7274  .def WishartBart
+00007bf0: 6c65 7474 286e 616d 652c 2053 2c20 6e75  lett(name, S, nu
+00007c00: 2c20 6973 5f63 686f 6c65 736b 793d 4661  , is_cholesky=Fa
+00007c10: 6c73 652c 2072 6574 7572 6e5f 6368 6f6c  lse, return_chol
+00007c20: 6573 6b79 3d46 616c 7365 2c20 696e 6974  esky=False, init
+00007c30: 7661 6c3d 4e6f 6e65 293a 0a20 2020 2072  val=None):.    r
+00007c40: 2222 220a 2020 2020 4261 7274 6c65 7474  """.    Bartlett
+00007c50: 2064 6563 6f6d 706f 7369 7469 6f6e 206f   decomposition o
+00007c60: 6620 7468 6520 5769 7368 6172 7420 6469  f the Wishart di
+00007c70: 7374 7269 6275 7469 6f6e 2e20 4173 2074  stribution. As t
+00007c80: 6865 2057 6973 6861 7274 0a20 2020 2064  he Wishart.    d
+00007c90: 6973 7472 6962 7574 696f 6e20 7265 7175  istribution requ
+00007ca0: 6972 6573 2074 6865 206d 6174 7269 7820  ires the matrix 
+00007cb0: 746f 2062 6520 7379 6d6d 6574 7269 6320  to be symmetric 
+00007cc0: 706f 7369 7469 7665 2073 656d 692d 6465  positive semi-de
+00007cd0: 6669 6e69 7465 0a20 2020 2069 7420 6973  finite.    it is
+00007ce0: 2069 6d70 6f73 7369 626c 6520 666f 7220   impossible for 
+00007cf0: 4d43 4d43 2074 6f20 6576 6572 2070 726f  MCMC to ever pro
+00007d00: 706f 7365 2061 6363 6570 7461 626c 6520  pose acceptable 
+00007d10: 6d61 7472 6963 6573 2e0a 0a20 2020 2049  matrices...    I
+00007d20: 6e73 7465 6164 2c20 7765 2063 616e 2075  nstead, we can u
+00007d30: 7365 2074 6865 2042 6172 6c65 7474 2064  se the Barlett d
+00007d40: 6563 6f6d 706f 7369 7469 6f6e 2077 6869  ecomposition whi
+00007d50: 6368 2073 616d 706c 6573 2061 206c 6f77  ch samples a low
+00007d60: 6572 0a20 2020 2064 6961 676f 6e61 6c20  er.    diagonal 
+00007d70: 6d61 7472 6978 2e20 5370 6563 6966 6963  matrix. Specific
+00007d80: 616c 6c79 3a0a 0a20 2020 202e 2e20 6d61  ally:..    .. ma
+00007d90: 7468 3a3a 0a20 2020 2020 2020 205c 7465  th::.        \te
+00007da0: 7874 7b49 667d 204c 205c 7369 6d20 5c62  xt{If} L \sim \b
+00007db0: 6567 696e 7b70 6d61 7472 6978 7d0a 2020  egin{pmatrix}.  
+00007dc0: 2020 2020 2020 5c73 7172 747b 635f 317d        \sqrt{c_1}
+00007dd0: 2026 2030 2026 2030 205c 5c0a 2020 2020   & 0 & 0 \\.    
+00007de0: 2020 2020 7a5f 7b32 317d 2026 205c 7371      z_{21} & \sq
+00007df0: 7274 7b63 5f32 7d20 2620 3020 5c5c 0a20  rt{c_2} & 0 \\. 
+00007e00: 2020 2020 2020 207a 5f7b 3331 7d20 2620         z_{31} & 
+00007e10: 7a5f 7b33 327d 2026 205c 7371 7274 7b63  z_{32} & \sqrt{c
+00007e20: 5f33 7d0a 2020 2020 2020 2020 5c65 6e64  _3}.        \end
+00007e30: 7b70 6d61 7472 6978 7d0a 0a20 2020 2020  {pmatrix}..     
+00007e40: 2020 205c 7465 7874 7b77 6974 687d 2063     \text{with} c
+00007e50: 5f69 205c 7369 6d20 5c63 6869 5e32 286e  _i \sim \chi^2(n
+00007e60: 2d69 2b31 2920 5c74 6578 747b 2061 6e64  -i+1) \text{ and
+00007e70: 207d 206e 5f7b 696a 7d20 5c73 696d 205c   } n_{ij} \sim \
+00007e80: 6d61 7468 6361 6c7b 4e7d 2830 2c20 3129  mathcal{N}(0, 1)
+00007e90: 2c20 5c74 6578 747b 7468 656e 7d20 5c5c  , \text{then} \\
+00007ea0: 0a20 2020 2020 2020 204c 205c 7469 6d65  .        L \time
+00007eb0: 7320 4120 5c74 696d 6573 2041 2e54 205c  s A \times A.T \
+00007ec0: 7469 6d65 7320 4c2e 5420 5c73 696d 205c  times L.T \sim \
+00007ed0: 7465 7874 7b57 6973 6861 7274 7d28 4c20  text{Wishart}(L 
+00007ee0: 5c74 696d 6573 204c 2e54 2c20 5c6e 7529  \times L.T, \nu)
+00007ef0: 0a0a 2020 2020 5365 6520 6874 7470 3a2f  ..    See http:/
+00007f00: 2f65 6e2e 7769 6b69 7065 6469 612e 6f72  /en.wikipedia.or
+00007f10: 672f 7769 6b69 2f57 6973 6861 7274 5f64  g/wiki/Wishart_d
+00007f20: 6973 7472 6962 7574 696f 6e23 4261 7274  istribution#Bart
+00007f30: 6c65 7474 5f64 6563 6f6d 706f 7369 7469  lett_decompositi
+00007f40: 6f6e 0a20 2020 2066 6f72 206d 6f72 6520  on.    for more 
+00007f50: 696e 666f 726d 6174 696f 6e2e 0a0a 2020  information...  
+00007f60: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00007f70: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00007f80: 5320 3a20 6e64 6172 7261 790a 2020 2020  S : ndarray.    
+00007f90: 2020 2020 7020 7820 7020 706f 7369 7469      p x p positi
+00007fa0: 7665 2064 6566 696e 6974 6520 6d61 7472  ve definite matr
+00007fb0: 6978 0a20 2020 2020 2020 204f 723a 0a20  ix.        Or:. 
+00007fc0: 2020 2020 2020 2070 2078 2070 206c 6f77         p x p low
+00007fd0: 6572 2d74 7269 616e 6775 6c61 7220 6d61  er-triangular ma
+00007fe0: 7472 6978 2074 6861 7420 6973 2074 6865  trix that is the
+00007ff0: 2043 686f 6c65 736b 7920 6661 6374 6f72   Cholesky factor
+00008000: 0a20 2020 2020 2020 206f 6620 7468 6520  .        of the 
+00008010: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+00008020: 782e 0a20 2020 206e 7520 3a20 7465 6e73  x..    nu : tens
+00008030: 6f72 5f6c 696b 6520 6f66 2069 6e74 0a20  or_like of int. 
+00008040: 2020 2020 2020 2044 6567 7265 6573 206f         Degrees o
+00008050: 6620 6672 6565 646f 6d2c 203e 2064 696d  f freedom, > dim
+00008060: 2853 292e 0a20 2020 2069 735f 6368 6f6c  (S)..    is_chol
+00008070: 6573 6b79 203a 2062 6f6f 6c2c 2064 6566  esky : bool, def
+00008080: 6175 6c74 3d46 616c 7365 0a20 2020 2020  ault=False.     
+00008090: 2020 2049 6e70 7574 206d 6174 7269 7820     Input matrix 
+000080a0: 5320 6973 2061 6c72 6561 6479 2043 686f  S is already Cho
+000080b0: 6c65 736b 7920 6465 636f 6d70 6f73 6564  lesky decomposed
+000080c0: 2061 7320 532e 5420 2a20 530a 2020 2020   as S.T * S.    
+000080d0: 7265 7475 726e 5f63 686f 6c65 736b 7920  return_cholesky 
+000080e0: 3a20 626f 6f6c 2c20 6465 6661 756c 743d  : bool, default=
+000080f0: 4661 6c73 650a 2020 2020 2020 2020 4f6e  False.        On
+00008100: 6c79 2072 6574 7572 6e20 7468 6520 4368  ly return the Ch
+00008110: 6f6c 6573 6b79 2064 6563 6f6d 706f 7365  olesky decompose
+00008120: 6420 6d61 7472 6978 2e0a 2020 2020 696e  d matrix..    in
+00008130: 6974 7661 6c20 3a20 6e64 6172 7261 790a  itval : ndarray.
+00008140: 2020 2020 2020 2020 7020 7820 7020 706f          p x p po
+00008150: 7369 7469 7665 2064 6566 696e 6974 6520  sitive definite 
+00008160: 6d61 7472 6978 2075 7365 6420 746f 2069  matrix used to i
+00008170: 6e69 7469 616c 697a 650a 0a20 2020 204e  nitialize..    N
+00008180: 6f74 6573 0a20 2020 202d 2d2d 2d2d 0a20  otes.    -----. 
+00008190: 2020 2054 6869 7320 6973 206e 6f74 2061     This is not a
+000081a0: 2073 7461 6e64 6172 6420 4469 7374 7269   standard Distri
+000081b0: 6275 7469 6f6e 2063 6c61 7373 2062 7574  bution class but
+000081c0: 2066 6f6c 6c6f 7773 2061 2073 696d 696c   follows a simil
+000081d0: 6172 0a20 2020 2069 6e74 6572 6661 6365  ar.    interface
+000081e0: 2e20 4265 7369 6465 7320 7468 6520 5769  . Besides the Wi
+000081f0: 7368 6172 7420 6469 7374 7269 6275 7469  shart distributi
+00008200: 6f6e 2c20 6974 2077 696c 6c20 6164 6420  on, it will add 
+00008210: 5256 730a 2020 2020 6e61 6d65 5f63 2061  RVs.    name_c a
+00008220: 6e64 206e 616d 655f 7a20 746f 2079 6f75  nd name_z to you
+00008230: 7220 6d6f 6465 6c20 7768 6963 6820 6d61  r model which ma
+00008240: 6b65 2075 7020 7468 6520 6d61 7472 6978  ke up the matrix
+00008250: 2e0a 0a20 2020 2054 6869 7320 6469 7374  ...    This dist
+00008260: 7269 6275 7469 6f6e 2069 7320 7573 7561  ribution is usua
+00008270: 6c6c 7920 6120 6261 6420 6964 6561 2074  lly a bad idea t
+00008280: 6f20 7573 6520 6173 2061 2070 7269 6f72  o use as a prior
+00008290: 2066 6f72 206d 756c 7469 7661 7269 6174   for multivariat
+000082a0: 650a 2020 2020 6e6f 726d 616c 2e20 596f  e.    normal. Yo
+000082b0: 7520 7368 6f75 6c64 2069 6e73 7465 6164  u should instead
+000082c0: 2075 7365 204c 4b4a 4368 6f6c 6573 6b79   use LKJCholesky
+000082d0: 436f 7620 6f72 204c 4b4a 436f 7272 2e0a  Cov or LKJCorr..
+000082e0: 2020 2020 2222 220a 0a20 2020 204c 203d      """..    L =
+000082f0: 2053 2069 6620 6973 5f63 686f 6c65 736b   S if is_cholesk
+00008300: 7920 656c 7365 2073 6369 7079 2e6c 696e  y else scipy.lin
+00008310: 616c 672e 6368 6f6c 6573 6b79 2853 290a  alg.cholesky(S).
+00008320: 2020 2020 6469 6167 5f69 6478 203d 206e      diag_idx = n
+00008330: 702e 6469 6167 5f69 6e64 6963 6573 5f66  p.diag_indices_f
+00008340: 726f 6d28 5329 0a20 2020 2074 7269 6c5f  rom(S).    tril_
+00008350: 6964 7820 3d20 6e70 2e74 7269 6c5f 696e  idx = np.tril_in
+00008360: 6469 6365 735f 6672 6f6d 2853 2c20 6b3d  dices_from(S, k=
+00008370: 2d31 290a 2020 2020 6e5f 6469 6167 203d  -1).    n_diag =
+00008380: 206c 656e 2864 6961 675f 6964 785b 305d   len(diag_idx[0]
+00008390: 290a 2020 2020 6e5f 7472 696c 203d 206c  ).    n_tril = l
+000083a0: 656e 2874 7269 6c5f 6964 785b 305d 290a  en(tril_idx[0]).
+000083b0: 0a20 2020 2069 6620 696e 6974 7661 6c20  .    if initval 
+000083c0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000083d0: 2020 2020 2023 2049 6e76 6572 7365 2074       # Inverse t
+000083e0: 7261 6e73 666f 726d 0a20 2020 2020 2020  ransform.       
+000083f0: 2069 6e69 7476 616c 203d 206e 702e 646f   initval = np.do
+00008400: 7428 6e70 2e64 6f74 286e 702e 6c69 6e61  t(np.dot(np.lina
+00008410: 6c67 2e69 6e76 284c 292c 2069 6e69 7476  lg.inv(L), initv
+00008420: 616c 292c 206e 702e 6c69 6e61 6c67 2e69  al), np.linalg.i
+00008430: 6e76 284c 2e54 2929 0a20 2020 2020 2020  nv(L.T)).       
+00008440: 2069 6e69 7476 616c 203d 206c 696e 616c   initval = linal
+00008450: 672e 6368 6f6c 6573 6b79 2869 6e69 7476  g.cholesky(initv
+00008460: 616c 2c20 6c6f 7765 723d 5472 7565 290a  al, lower=True).
+00008470: 2020 2020 2020 2020 6469 6167 5f74 6573          diag_tes
+00008480: 7476 616c 203d 2069 6e69 7476 616c 5b64  tval = initval[d
+00008490: 6961 675f 6964 785d 202a 2a20 320a 2020  iag_idx] ** 2.  
+000084a0: 2020 2020 2020 7472 696c 5f74 6573 7476        tril_testv
+000084b0: 616c 203d 2069 6e69 7476 616c 5b74 7269  al = initval[tri
+000084c0: 6c5f 6964 785d 0a20 2020 2065 6c73 653a  l_idx].    else:
+000084d0: 0a20 2020 2020 2020 2064 6961 675f 7465  .        diag_te
+000084e0: 7374 7661 6c20 3d20 4e6f 6e65 0a20 2020  stval = None.   
+000084f0: 2020 2020 2074 7269 6c5f 7465 7374 7661       tril_testva
+00008500: 6c20 3d20 4e6f 6e65 0a0a 2020 2020 6320  l = None..    c 
+00008510: 3d20 7074 2e73 7172 7428 0a20 2020 2020  = pt.sqrt(.     
+00008520: 2020 2043 6869 5371 7561 7265 6428 2225     ChiSquared("%
+00008530: 735f 6322 2025 206e 616d 652c 206e 7520  s_c" % name, nu 
+00008540: 2d20 6e70 2e61 7261 6e67 6528 322c 2032  - np.arange(2, 2
+00008550: 202b 206e 5f64 6961 6729 2c20 7368 6170   + n_diag), shap
+00008560: 653d 6e5f 6469 6167 2c20 696e 6974 7661  e=n_diag, initva
+00008570: 6c3d 6469 6167 5f74 6573 7476 616c 290a  l=diag_testval).
+00008580: 2020 2020 290a 2020 2020 706d 2e5f 6c6f      ).    pm._lo
+00008590: 672e 696e 666f 2822 4164 6465 6420 6e65  g.info("Added ne
+000085a0: 7720 7661 7269 6162 6c65 2025 735f 6320  w variable %s_c 
+000085b0: 746f 206d 6f64 656c 2064 6961 676f 6e61  to model diagona
+000085c0: 6c20 6f66 2057 6973 6861 7274 2e22 2025  l of Wishart." %
+000085d0: 206e 616d 6529 0a20 2020 207a 203d 204e   name).    z = N
+000085e0: 6f72 6d61 6c28 2225 735f 7a22 2025 206e  ormal("%s_z" % n
+000085f0: 616d 652c 2030 2e30 2c20 312e 302c 2073  ame, 0.0, 1.0, s
+00008600: 6861 7065 3d6e 5f74 7269 6c2c 2069 6e69  hape=n_tril, ini
+00008610: 7476 616c 3d74 7269 6c5f 7465 7374 7661  tval=tril_testva
+00008620: 6c29 0a20 2020 2070 6d2e 5f6c 6f67 2e69  l).    pm._log.i
+00008630: 6e66 6f28 2241 6464 6564 206e 6577 2076  nfo("Added new v
+00008640: 6172 6961 626c 6520 2573 5f7a 2074 6f20  ariable %s_z to 
+00008650: 6d6f 6465 6c20 6f66 662d 6469 6167 6f6e  model off-diagon
+00008660: 616c 7320 6f66 2057 6973 6861 7274 2e22  als of Wishart."
+00008670: 2025 206e 616d 6529 0a20 2020 2023 2043   % name).    # C
+00008680: 6f6e 7374 7275 6374 2041 206d 6174 7269  onstruct A matri
+00008690: 780a 2020 2020 4120 3d20 7074 2e7a 6572  x.    A = pt.zer
+000086a0: 6f73 2853 2e73 6861 7065 2c20 6474 7970  os(S.shape, dtyp
+000086b0: 653d 6e70 2e66 6c6f 6174 3332 290a 2020  e=np.float32).  
+000086c0: 2020 4120 3d20 7074 2e73 6574 5f73 7562    A = pt.set_sub
+000086d0: 7465 6e73 6f72 2841 5b64 6961 675f 6964  tensor(A[diag_id
+000086e0: 785d 2c20 6329 0a20 2020 2041 203d 2070  x], c).    A = p
+000086f0: 742e 7365 745f 7375 6274 656e 736f 7228  t.set_subtensor(
+00008700: 415b 7472 696c 5f69 6478 5d2c 207a 290a  A[tril_idx], z).
+00008710: 0a20 2020 2023 204c 202a 2041 202a 2041  .    # L * A * A
+00008720: 2e54 202a 204c 2e54 207e 2057 6973 6861  .T * L.T ~ Wisha
+00008730: 7274 284c 2a4c 2e54 2c20 6e75 290a 2020  rt(L*L.T, nu).  
+00008740: 2020 6966 2072 6574 7572 6e5f 6368 6f6c    if return_chol
+00008750: 6573 6b79 3a0a 2020 2020 2020 2020 7265  esky:.        re
+00008760: 7475 726e 2070 6d2e 4465 7465 726d 696e  turn pm.Determin
+00008770: 6973 7469 6328 6e61 6d65 2c20 7074 2e64  istic(name, pt.d
+00008780: 6f74 284c 2c20 4129 290a 2020 2020 656c  ot(L, A)).    el
+00008790: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
+000087a0: 726e 2070 6d2e 4465 7465 726d 696e 6973  rn pm.Determinis
+000087b0: 7469 6328 6e61 6d65 2c20 7074 2e64 6f74  tic(name, pt.dot
+000087c0: 2870 742e 646f 7428 7074 2e64 6f74 284c  (pt.dot(pt.dot(L
+000087d0: 2c20 4129 2c20 412e 5429 2c20 4c2e 5429  , A), A.T), L.T)
+000087e0: 290a 0a0a 6465 6620 5f6c 6b6a 5f6e 6f72  )...def _lkj_nor
+000087f0: 6d61 6c69 7a69 6e67 5f63 6f6e 7374 616e  malizing_constan
+00008800: 7428 6574 612c 206e 293a 0a20 2020 2023  t(eta, n):.    #
+00008810: 2054 4f44 4f3a 2054 6869 7320 6973 206d   TODO: This is m
+00008820: 6978 696e 6720 7079 7468 6f6e 2062 7261  ixing python bra
+00008830: 6e63 6869 6e67 2077 6974 6820 7468 6520  nching with the 
+00008840: 706f 7465 6e74 6961 6c6c 7920 7379 6d62  potentially symb
+00008850: 6f6c 6963 206e 2061 6e64 2065 7461 2076  olic n and eta v
+00008860: 6172 6961 626c 6573 0a20 2020 2069 6620  ariables.    if 
+00008870: 6e6f 7420 6973 696e 7374 616e 6365 2865  not isinstance(e
+00008880: 7461 2c20 2869 6e74 2c20 666c 6f61 7429  ta, (int, float)
+00008890: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+000088a0: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+000088b0: 7272 6f72 2822 6574 6120 6d75 7374 2062  rror("eta must b
+000088c0: 6520 616e 2069 6e74 206f 7220 666c 6f61  e an int or floa
+000088d0: 7422 290a 2020 2020 6966 206e 6f74 2069  t").    if not i
+000088e0: 7369 6e73 7461 6e63 6528 6e2c 2069 6e74  sinstance(n, int
+000088f0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
+00008900: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
+00008910: 7272 6f72 2822 6e20 6d75 7374 2062 6520  rror("n must be 
+00008920: 616e 2069 6e74 6567 6572 2229 0a20 2020  an integer").   
+00008930: 2069 6620 6574 6120 3d3d 2031 3a0a 2020   if eta == 1:.  
+00008940: 2020 2020 2020 7265 7375 6c74 203d 2067        result = g
+00008950: 616d 6d61 6c6e 2832 2e30 202a 2070 742e  ammaln(2.0 * pt.
+00008960: 6172 616e 6765 2831 2c20 696e 7428 286e  arange(1, int((n
+00008970: 202d 2031 2920 2f20 3229 202b 2031 2929   - 1) / 2) + 1))
+00008980: 2e73 756d 2829 0a20 2020 2020 2020 2069  .sum().        i
+00008990: 6620 6e20 2520 3220 3d3d 2031 3a0a 2020  f n % 2 == 1:.  
+000089a0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+000089b0: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
+000089c0: 2020 2020 2020 302e 3235 202a 2028 6e2a        0.25 * (n*
+000089d0: 2a32 202d 2031 2920 2a20 7074 2e6c 6f67  *2 - 1) * pt.log
+000089e0: 286e 702e 7069 290a 2020 2020 2020 2020  (np.pi).        
+000089f0: 2020 2020 2020 2020 2d20 302e 3235 202a          - 0.25 *
+00008a00: 2028 6e20 2d20 3129 202a 2a20 3220 2a20   (n - 1) ** 2 * 
+00008a10: 7074 2e6c 6f67 2832 2e30 290a 2020 2020  pt.log(2.0).    
+00008a20: 2020 2020 2020 2020 2020 2020 2d20 286e              - (n
+00008a30: 202d 2031 2920 2a20 6761 6d6d 616c 6e28   - 1) * gammaln(
+00008a40: 696e 7428 286e 202b 2031 2920 2f20 3229  int((n + 1) / 2)
+00008a50: 290a 2020 2020 2020 2020 2020 2020 290a  ).            ).
+00008a60: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00008a70: 2020 2020 2020 2020 2020 7265 7375 6c74            result
+00008a80: 202b 3d20 280a 2020 2020 2020 2020 2020   += (.          
+00008a90: 2020 2020 2020 302e 3235 202a 206e 202a        0.25 * n *
+00008aa0: 2028 6e20 2d20 3229 202a 2070 742e 6c6f   (n - 2) * pt.lo
+00008ab0: 6728 6e70 2e70 6929 0a20 2020 2020 2020  g(np.pi).       
+00008ac0: 2020 2020 2020 2020 202b 2030 2e32 3520           + 0.25 
+00008ad0: 2a20 2833 202a 206e 2a2a 3220 2d20 3420  * (3 * n**2 - 4 
+00008ae0: 2a20 6e29 202a 2070 742e 6c6f 6728 322e  * n) * pt.log(2.
+00008af0: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+00008b00: 2020 202b 206e 202a 2067 616d 6d61 6c6e     + n * gammaln
+00008b10: 286e 202f 2032 290a 2020 2020 2020 2020  (n / 2).        
+00008b20: 2020 2020 2020 2020 2d20 286e 202d 2031          - (n - 1
+00008b30: 2920 2a20 6761 6d6d 616c 6e28 6e29 0a20  ) * gammaln(n). 
+00008b40: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00008b50: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+00008b60: 6573 756c 7420 3d20 2d28 6e20 2d20 3129  esult = -(n - 1)
+00008b70: 202a 2067 616d 6d61 6c6e 2865 7461 202b   * gammaln(eta +
+00008b80: 2030 2e35 202a 2028 6e20 2d20 3129 290a   0.5 * (n - 1)).
+00008b90: 2020 2020 2020 2020 6b20 3d20 7074 2e61          k = pt.a
+00008ba0: 7261 6e67 6528 312c 206e 290a 2020 2020  range(1, n).    
+00008bb0: 2020 2020 7265 7375 6c74 202b 3d20 2830      result += (0
+00008bc0: 2e35 202a 206b 202a 2070 742e 6c6f 6728  .5 * k * pt.log(
+00008bd0: 6e70 2e70 6929 202b 2067 616d 6d61 6c6e  np.pi) + gammaln
+00008be0: 2865 7461 202b 2030 2e35 202a 2028 6e20  (eta + 0.5 * (n 
+00008bf0: 2d20 3120 2d20 6b29 2929 2e73 756d 2829  - 1 - k))).sum()
+00008c00: 0a20 2020 2072 6574 7572 6e20 7265 7375  .    return resu
+00008c10: 6c74 0a0a 0a63 6c61 7373 205f 4c4b 4a43  lt...class _LKJC
+00008c20: 686f 6c65 736b 7943 6f76 4261 7365 5256  holeskyCovBaseRV
+00008c30: 2852 616e 646f 6d56 6172 6961 626c 6529  (RandomVariable)
+00008c40: 3a0a 2020 2020 6e61 6d65 203d 2022 5f6c  :.    name = "_l
+00008c50: 6b6a 6368 6f6c 6573 6b79 636f 7662 6173  kjcholeskycovbas
+00008c60: 6522 0a20 2020 206e 6469 6d5f 7375 7070  e".    ndim_supp
+00008c70: 203d 2031 0a20 2020 206e 6469 6d73 5f70   = 1.    ndims_p
+00008c80: 6172 616d 7320 3d20 5b30 2c20 302c 2031  arams = [0, 0, 1
+00008c90: 5d0a 2020 2020 6474 7970 6520 3d20 2266  ].    dtype = "f
+00008ca0: 6c6f 6174 5822 0a20 2020 205f 7072 696e  loatX".    _prin
+00008cb0: 745f 6e61 6d65 203d 2028 225f 6c6b 6a63  t_name = ("_lkjc
+00008cc0: 686f 6c65 736b 7963 6f76 6261 7365 222c  holeskycovbase",
+00008cd0: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
+00008ce0: 7b5f 6c6b 6a63 686f 6c65 736b 7963 6f76  {_lkjcholeskycov
+00008cf0: 6261 7365 7d22 290a 0a20 2020 2064 6566  base}")..    def
+00008d00: 206d 616b 655f 6e6f 6465 2873 656c 662c   make_node(self,
+00008d10: 2072 6e67 2c20 7369 7a65 2c20 6474 7970   rng, size, dtyp
+00008d20: 652c 206e 2c20 6574 612c 2044 293a 0a20  e, n, eta, D):. 
+00008d30: 2020 2020 2020 206e 203d 2070 742e 6173         n = pt.as
+00008d40: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00008d50: 286e 290a 2020 2020 2020 2020 6966 206e  (n).        if n
+00008d60: 6f74 206e 2e6e 6469 6d20 3d3d 2030 3a0a  ot n.ndim == 0:.
+00008d70: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00008d80: 6520 5661 6c75 6545 7272 6f72 2822 6e20  e ValueError("n 
+00008d90: 6d75 7374 2062 6520 6120 7363 616c 6172  must be a scalar
+00008da0: 2028 6e64 696d 3d30 292e 2229 0a0a 2020   (ndim=0).")..  
+00008db0: 2020 2020 2020 6574 6120 3d20 7074 2e61        eta = pt.a
+00008dc0: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
+00008dd0: 6528 6574 6129 0a20 2020 2020 2020 2069  e(eta).        i
+00008de0: 6620 6e6f 7420 6574 612e 6e64 696d 203d  f not eta.ndim =
+00008df0: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00008e00: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00008e10: 7228 2265 7461 206d 7573 7420 6265 2061  r("eta must be a
+00008e20: 2073 6361 6c61 7220 286e 6469 6d3d 3029   scalar (ndim=0)
+00008e30: 2e22 290a 0a20 2020 2020 2020 2044 203d  .")..        D =
+00008e40: 2070 742e 6173 5f74 656e 736f 725f 7661   pt.as_tensor_va
+00008e50: 7269 6162 6c65 2844 290a 0a20 2020 2020  riable(D)..     
+00008e60: 2020 2072 6574 7572 6e20 7375 7065 7228     return super(
+00008e70: 292e 6d61 6b65 5f6e 6f64 6528 726e 672c  ).make_node(rng,
+00008e80: 2073 697a 652c 2064 7479 7065 2c20 6e2c   size, dtype, n,
+00008e90: 2065 7461 2c20 4429 0a0a 2020 2020 6465   eta, D)..    de
+00008ea0: 6620 5f73 7570 705f 7368 6170 655f 6672  f _supp_shape_fr
+00008eb0: 6f6d 5f70 6172 616d 7328 7365 6c66 2c20  om_params(self, 
+00008ec0: 6469 7374 5f70 6172 616d 732c 2070 6172  dist_params, par
+00008ed0: 616d 5f73 6861 7065 7329 3a0a 2020 2020  am_shapes):.    
+00008ee0: 2020 2020 6e20 3d20 6469 7374 5f70 6172      n = dist_par
+00008ef0: 616d 735b 305d 0a20 2020 2020 2020 2072  ams[0].        r
+00008f00: 6574 7572 6e20 2828 6e20 2a20 286e 202b  eturn ((n * (n +
+00008f10: 2031 2929 202f 2f20 322c 290a 0a20 2020   1)) // 2,)..   
+00008f20: 2064 6566 2072 6e67 5f66 6e28 7365 6c66   def rng_fn(self
+00008f30: 2c20 726e 672c 206e 2c20 6574 612c 2044  , rng, n, eta, D
+00008f40: 2c20 7369 7a65 293a 0a20 2020 2020 2020  , size):.       
+00008f50: 2023 2057 6520 666c 6174 7465 6e20 7468   # We flatten th
+00008f60: 6520 7369 7a65 2074 6f20 6d61 6b65 206f  e size to make o
+00008f70: 7065 7261 7469 6f6e 7320 6561 7369 6572  perations easier
+00008f80: 2c20 616e 6420 7468 656e 2072 6562 7569  , and then rebui
+00008f90: 6c64 2069 740a 2020 2020 2020 2020 6966  ld it.        if
+00008fa0: 2073 697a 6520 6973 204e 6f6e 653a 0a20   size is None:. 
+00008fb0: 2020 2020 2020 2020 2020 2073 697a 6520             size 
+00008fc0: 3d20 442e 7368 6170 655b 3a2d 315d 0a20  = D.shape[:-1]. 
+00008fd0: 2020 2020 2020 2066 6c61 745f 7369 7a65         flat_size
+00008fe0: 203d 206e 702e 7072 6f64 2873 697a 6529   = np.prod(size)
+00008ff0: 2e61 7374 7970 6528 696e 7429 0a0a 2020  .astype(int)..  
+00009000: 2020 2020 2020 4320 3d20 4c4b 4a43 6f72        C = LKJCor
+00009010: 7252 562e 5f72 616e 646f 6d5f 636f 7272  rRV._random_corr
+00009020: 5f6d 6174 7269 7828 726e 673d 726e 672c  _matrix(rng=rng,
+00009030: 206e 3d6e 2c20 6574 613d 6574 612c 2066   n=n, eta=eta, f
+00009040: 6c61 745f 7369 7a65 3d66 6c61 745f 7369  lat_size=flat_si
+00009050: 7a65 290a 2020 2020 2020 2020 4420 3d20  ze).        D = 
+00009060: 442e 7265 7368 6170 6528 666c 6174 5f73  D.reshape(flat_s
+00009070: 697a 652c 206e 290a 2020 2020 2020 2020  ize, n).        
+00009080: 4320 2a3d 2044 5b2e 2e2e 2c20 3a2c 206e  C *= D[..., :, n
+00009090: 702e 6e65 7761 7869 735d 202a 2044 5b2e  p.newaxis] * D[.
+000090a0: 2e2e 2c20 6e70 2e6e 6577 6178 6973 2c20  .., np.newaxis, 
+000090b0: 3a5d 0a0a 2020 2020 2020 2020 7472 696c  :]..        tril
+000090c0: 5f69 6478 203d 206e 702e 7472 696c 5f69  _idx = np.tril_i
+000090d0: 6e64 6963 6573 286e 2c20 6b3d 3029 0a20  ndices(n, k=0). 
+000090e0: 2020 2020 2020 2073 616d 706c 6573 203d         samples =
+000090f0: 206e 702e 6c69 6e61 6c67 2e63 686f 6c65   np.linalg.chole
+00009100: 736b 7928 4329 5b2e 2e2e 2c20 7472 696c  sky(C)[..., tril
+00009110: 5f69 6478 5b30 5d2c 2074 7269 6c5f 6964  _idx[0], tril_id
+00009120: 785b 315d 5d0a 0a20 2020 2020 2020 2069  x[1]]..        i
+00009130: 6620 7369 7a65 2069 7320 4e6f 6e65 3a0a  f size is None:.
+00009140: 2020 2020 2020 2020 2020 2020 7361 6d70              samp
+00009150: 6c65 7320 3d20 7361 6d70 6c65 735b 305d  les = samples[0]
+00009160: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00009170: 2020 2020 2020 2020 2020 2064 6973 745f             dist_
+00009180: 7368 6170 6520 3d20 286e 202a 2028 6e20  shape = (n * (n 
+00009190: 2b20 3129 2920 2f2f 2032 0a20 2020 2020  + 1)) // 2.     
+000091a0: 2020 2020 2020 2073 616d 706c 6573 203d         samples =
+000091b0: 206e 702e 7265 7368 6170 6528 7361 6d70   np.reshape(samp
+000091c0: 6c65 732c 2028 2a73 697a 652c 2064 6973  les, (*size, dis
+000091d0: 745f 7368 6170 6529 290a 0a20 2020 2020  t_shape))..     
+000091e0: 2020 2072 6574 7572 6e20 7361 6d70 6c65     return sample
+000091f0: 730a 0a0a 5f6c 6a6b 5f63 686f 6c65 736b  s..._ljk_cholesk
+00009200: 795f 636f 765f 6261 7365 203d 205f 4c4b  y_cov_base = _LK
+00009210: 4a43 686f 6c65 736b 7943 6f76 4261 7365  JCholeskyCovBase
+00009220: 5256 2829 0a0a 0a23 205f 4c4b 4a43 686f  RV()...# _LKJCho
+00009230: 6c65 736b 7943 6f76 4261 7365 5256 2072  leskyCovBaseRV r
+00009240: 6571 7569 7265 7320 6120 7072 6f70 6572  equires a proper
+00009250: 6c79 2073 6861 7065 6420 6044 602c 2077  ly shaped `D`, w
+00009260: 6869 6368 206d 6561 6e73 2074 6865 2076  hich means the v
+00009270: 6172 6961 626c 6520 6361 6e27 740a 2320  ariable can't.# 
+00009280: 6265 2073 6166 656c 7920 7265 7369 7a65  be safely resize
+00009290: 642e 2042 6563 6175 7365 206f 6620 7468  d. Because of th
+000092a0: 6973 2c20 7765 2061 6464 2074 6865 2074  is, we add the t
+000092b0: 6869 6e20 5379 6d62 6f6c 6963 5261 6e64  hin SymbolicRand
+000092c0: 6f6d 5661 7269 6162 6c65 2077 7261 7070  omVariable wrapp
+000092d0: 6572 0a63 6c61 7373 205f 4c4b 4a43 686f  er.class _LKJCho
+000092e0: 6c65 736b 7943 6f76 5256 2853 796d 626f  leskyCovRV(Symbo
+000092f0: 6c69 6352 616e 646f 6d56 6172 6961 626c  licRandomVariabl
+00009300: 6529 3a0a 2020 2020 6465 6661 756c 745f  e):.    default_
+00009310: 6f75 7470 7574 203d 2031 0a20 2020 205f  output = 1.    _
+00009320: 7072 696e 745f 6e61 6d65 203d 2028 225f  print_name = ("_
+00009330: 6c6b 6a63 686f 6c65 736b 7963 6f76 222c  lkjcholeskycov",
+00009340: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
+00009350: 7b5f 6c6b 6a63 686f 6c65 736b 7963 6f76  {_lkjcholeskycov
+00009360: 7d22 290a 0a20 2020 2064 6566 2075 7064  }")..    def upd
+00009370: 6174 6528 7365 6c66 2c20 6e6f 6465 293a  ate(self, node):
+00009380: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009390: 7b6e 6f64 652e 696e 7075 7473 5b30 5d3a  {node.inputs[0]:
+000093a0: 206e 6f64 652e 6f75 7470 7574 735b 305d   node.outputs[0]
+000093b0: 7d0a 0a0a 636c 6173 7320 5f4c 4b4a 4368  }...class _LKJCh
+000093c0: 6f6c 6573 6b79 436f 7628 4469 7374 7269  oleskyCov(Distri
+000093d0: 6275 7469 6f6e 293a 0a20 2020 2072 2222  bution):.    r""
+000093e0: 2255 6e64 6572 6c79 696e 6720 636c 6173  "Underlying clas
+000093f0: 7320 666f 7220 636f 7661 7269 616e 6365  s for covariance
+00009400: 206d 6174 7269 7820 7769 7468 204c 4b4a   matrix with LKJ
+00009410: 2064 6973 7472 6962 7574 6564 2063 6f72   distributed cor
+00009420: 7265 6c61 7469 6f6e 732e 0a20 2020 2053  relations..    S
+00009430: 6565 2064 6f63 7320 666f 7220 4c4b 4a43  ee docs for LKJC
+00009440: 686f 6c65 736b 7943 6f76 2066 756e 6374  holeskyCov funct
+00009450: 696f 6e20 666f 7220 6d6f 7265 2064 6574  ion for more det
+00009460: 6169 6c73 206f 6e20 686f 7720 746f 2075  ails on how to u
+00009470: 7365 2069 7420 696e 206d 6f64 656c 732e  se it in models.
+00009480: 0a20 2020 2022 2222 0a0a 2020 2020 7276  .    """..    rv
+00009490: 5f74 7970 6520 3d20 5f4c 4b4a 4368 6f6c  _type = _LKJChol
+000094a0: 6573 6b79 436f 7652 560a 0a20 2020 2040  eskyCovRV..    @
+000094b0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+000094c0: 6465 6620 6469 7374 2863 6c73 2c20 6e2c  def dist(cls, n,
+000094d0: 2065 7461 2c20 7364 5f64 6973 742c 202a   eta, sd_dist, *
+000094e0: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
+000094f0: 2020 6e20 3d20 7074 2e61 735f 7465 6e73    n = pt.as_tens
+00009500: 6f72 5f76 6172 6961 626c 6528 696e 7458  or_variable(intX
+00009510: 286e 2929 0a20 2020 2020 2020 2065 7461  (n)).        eta
+00009520: 203d 2070 742e 6173 5f74 656e 736f 725f   = pt.as_tensor_
+00009530: 7661 7269 6162 6c65 2866 6c6f 6174 5828  variable(floatX(
+00009540: 6574 6129 290a 0a20 2020 2020 2020 2069  eta))..        i
+00009550: 6620 6e6f 7420 280a 2020 2020 2020 2020  f not (.        
+00009560: 2020 2020 6973 696e 7374 616e 6365 2873      isinstance(s
+00009570: 645f 6469 7374 2c20 5661 7269 6162 6c65  d_dist, Variable
+00009580: 290a 2020 2020 2020 2020 2020 2020 616e  ).            an
+00009590: 6420 7364 5f64 6973 742e 6f77 6e65 7220  d sd_dist.owner 
+000095a0: 6973 206e 6f74 204e 6f6e 650a 2020 2020  is not None.    
+000095b0: 2020 2020 2020 2020 616e 6420 6973 696e          and isin
+000095c0: 7374 616e 6365 2873 645f 6469 7374 2e6f  stance(sd_dist.o
+000095d0: 776e 6572 2e6f 702c 2028 5261 6e64 6f6d  wner.op, (Random
+000095e0: 5661 7269 6162 6c65 2c20 5379 6d62 6f6c  Variable, Symbol
+000095f0: 6963 5261 6e64 6f6d 5661 7269 6162 6c65  icRandomVariable
+00009600: 2929 0a20 2020 2020 2020 2020 2020 2061  )).            a
+00009610: 6e64 2073 645f 6469 7374 2e6f 776e 6572  nd sd_dist.owner
+00009620: 2e6f 702e 6e64 696d 5f73 7570 7020 3c20  .op.ndim_supp < 
+00009630: 320a 2020 2020 2020 2020 293a 0a20 2020  2.        ):.   
+00009640: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+00009650: 7970 6545 7272 6f72 2822 7364 5f64 6973  ypeError("sd_dis
+00009660: 7420 6d75 7374 2062 6520 6120 7363 616c  t must be a scal
+00009670: 6172 206f 7220 7665 6374 6f72 2064 6973  ar or vector dis
+00009680: 7472 6962 7574 696f 6e20 7661 7269 6162  tribution variab
+00009690: 6c65 2229 0a0a 2020 2020 2020 2020 6368  le")..        ch
+000096a0: 6563 6b5f 6469 7374 5f6e 6f74 5f72 6567  eck_dist_not_reg
+000096b0: 6973 7465 7265 6428 7364 5f64 6973 7429  istered(sd_dist)
+000096c0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000096d0: 7375 7065 7228 292e 6469 7374 285b 6e2c  super().dist([n,
+000096e0: 2065 7461 2c20 7364 5f64 6973 745d 2c20   eta, sd_dist], 
+000096f0: 2a2a 6b77 6172 6773 290a 0a20 2020 2040  **kwargs)..    @
+00009700: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00009710: 6465 6620 7276 5f6f 7028 636c 732c 206e  def rv_op(cls, n
+00009720: 2c20 6574 612c 2073 645f 6469 7374 2c20  , eta, sd_dist, 
+00009730: 7369 7a65 3d4e 6f6e 6529 3a0a 2020 2020  size=None):.    
+00009740: 2020 2020 2320 5765 2072 6573 697a 6520      # We resize 
+00009750: 7468 6520 7364 5f64 6973 7420 6175 746f  the sd_dist auto
+00009760: 6d61 7469 6361 6c6c 7920 736f 2074 6861  matically so tha
+00009770: 7420 6974 2068 6173 2028 7369 7a65 2078  t it has (size x
+00009780: 206e 2920 696e 6465 7065 6e64 656e 740a   n) independent.
+00009790: 2020 2020 2020 2020 2320 6472 6177 7320          # draws 
+000097a0: 7768 6963 6820 6973 2077 6861 7420 7468  which is what th
+000097b0: 6520 605f 4c4b 4a43 686f 6c65 736b 7943  e `_LKJCholeskyC
+000097c0: 6f76 4261 7365 5256 2e72 6e67 5f66 6e60  ovBaseRV.rng_fn`
+000097d0: 2065 7870 6563 7473 2e20 5468 6973 206d   expects. This m
+000097e0: 616b 6573 2074 6865 0a20 2020 2020 2020  akes the.       
+000097f0: 2023 2072 616e 646f 6d20 616e 6420 6c6f   # random and lo
+00009800: 6770 206d 6574 686f 6473 2065 7175 6976  gp methods equiv
+00009810: 616c 656e 742c 2061 7320 7468 6520 6c61  alent, as the la
+00009820: 7474 6572 2061 6c73 6f20 6173 7375 6d65  tter also assume
+00009830: 7320 6120 756e 6971 7565 2076 616c 7565  s a unique value
+00009840: 0a20 2020 2020 2020 2023 2066 6f72 2065  .        # for e
+00009850: 6163 6820 6469 6167 6f6e 616c 2065 6c65  ach diagonal ele
+00009860: 6d65 6e74 2e0a 2020 2020 2020 2020 2320  ment..        # 
+00009870: 5369 6e63 6520 6065 7461 6020 616e 6420  Since `eta` and 
+00009880: 606e 6020 6172 6520 666f 7263 6564 2074  `n` are forced t
+00009890: 6f20 6265 2073 6361 6c61 7273 2077 6520  o be scalars we 
+000098a0: 646f 6e27 7420 6e65 6564 2074 6f20 776f  don't need to wo
+000098b0: 7272 7920 6162 6f75 740a 2020 2020 2020  rry about.      
+000098c0: 2020 2320 696d 706c 6965 6420 6261 7463    # implied batc
+000098d0: 6865 6420 6469 6d65 6e73 696f 6e73 2066  hed dimensions f
+000098e0: 726f 6d20 7468 6f73 6520 666f 7220 7468  rom those for th
+000098f0: 6520 7469 6d65 2062 6569 6e67 2e0a 2020  e time being..  
+00009900: 2020 2020 2020 6966 2073 697a 6520 6973        if size is
+00009910: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00009920: 2020 2073 697a 6520 3d20 7364 5f64 6973     size = sd_dis
+00009930: 742e 7368 6170 655b 3a2d 315d 0a20 2020  t.shape[:-1].   
+00009940: 2020 2020 2073 6861 7065 203d 2074 7570       shape = tup
+00009950: 6c65 2873 697a 6529 202b 2028 6e2c 290a  le(size) + (n,).
+00009960: 2020 2020 2020 2020 6966 2073 645f 6469          if sd_di
+00009970: 7374 2e6f 776e 6572 2e6f 702e 6e64 696d  st.owner.op.ndim
+00009980: 5f73 7570 7020 3d3d 2030 3a0a 2020 2020  _supp == 0:.    
+00009990: 2020 2020 2020 2020 7364 5f64 6973 7420          sd_dist 
+000099a0: 3d20 6368 616e 6765 5f64 6973 745f 7369  = change_dist_si
+000099b0: 7a65 2873 645f 6469 7374 2c20 7368 6170  ze(sd_dist, shap
+000099c0: 6529 0a20 2020 2020 2020 2065 6c73 653a  e).        else:
+000099d0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+000099e0: 6865 2073 7570 706f 7274 2073 6861 7065  he support shape
+000099f0: 206d 7573 7420 6265 2060 6e60 2062 7574   must be `n` but
+00009a00: 2077 6520 6861 7665 206e 6f20 7761 7920   we have no way 
+00009a10: 6f66 2063 6f6e 7472 6f6c 6c69 6e67 2069  of controlling i
+00009a20: 740a 2020 2020 2020 2020 2020 2020 7364  t.            sd
+00009a30: 5f64 6973 7420 3d20 6368 616e 6765 5f64  _dist = change_d
+00009a40: 6973 745f 7369 7a65 2873 645f 6469 7374  ist_size(sd_dist
+00009a50: 2c20 7368 6170 655b 3a2d 315d 290a 0a20  , shape[:-1]).. 
+00009a60: 2020 2020 2020 2023 2043 7265 6174 6520         # Create 
+00009a70: 6e65 7720 726e 6720 666f 7220 7468 6520  new rng for the 
+00009a80: 5f6c 6b6a 6368 6f6c 6573 6b79 636f 7620  _lkjcholeskycov 
+00009a90: 696e 7465 726e 616c 2052 560a 2020 2020  internal RV.    
+00009aa0: 2020 2020 726e 6720 3d20 7079 7465 6e73      rng = pytens
+00009ab0: 6f72 2e73 6861 7265 6428 6e70 2e72 616e  or.shared(np.ran
+00009ac0: 646f 6d2e 6465 6661 756c 745f 726e 6728  dom.default_rng(
+00009ad0: 2929 0a0a 2020 2020 2020 2020 726e 675f  ))..        rng_
+00009ae0: 2c20 6e5f 2c20 6574 615f 2c20 7364 5f64  , n_, eta_, sd_d
+00009af0: 6973 745f 203d 2072 6e67 2e74 7970 6528  ist_ = rng.type(
+00009b00: 292c 206e 2e74 7970 6528 292c 2065 7461  ), n.type(), eta
+00009b10: 2e74 7970 6528 292c 2073 645f 6469 7374  .type(), sd_dist
+00009b20: 2e74 7970 6528 290a 2020 2020 2020 2020  .type().        
+00009b30: 6e65 7874 5f72 6e67 5f2c 206c 6b6a 636f  next_rng_, lkjco
+00009b40: 765f 203d 205f 6c6a 6b5f 6368 6f6c 6573  v_ = _ljk_choles
+00009b50: 6b79 5f63 6f76 5f62 6173 6528 6e5f 2c20  ky_cov_base(n_, 
+00009b60: 6574 615f 2c20 7364 5f64 6973 745f 2c20  eta_, sd_dist_, 
+00009b70: 726e 673d 726e 675f 292e 6f77 6e65 722e  rng=rng_).owner.
+00009b80: 6f75 7470 7574 730a 0a20 2020 2020 2020  outputs..       
+00009b90: 2072 6574 7572 6e20 5f4c 4b4a 4368 6f6c   return _LKJChol
+00009ba0: 6573 6b79 436f 7652 5628 0a20 2020 2020  eskyCovRV(.     
+00009bb0: 2020 2020 2020 2069 6e70 7574 733d 5b72         inputs=[r
+00009bc0: 6e67 5f2c 206e 5f2c 2065 7461 5f2c 2073  ng_, n_, eta_, s
+00009bd0: 645f 6469 7374 5f5d 2c0a 2020 2020 2020  d_dist_],.      
+00009be0: 2020 2020 2020 6f75 7470 7574 733d 5b6e        outputs=[n
+00009bf0: 6578 745f 726e 675f 2c20 6c6b 6a63 6f76  ext_rng_, lkjcov
+00009c00: 5f5d 2c0a 2020 2020 2020 2020 2020 2020  _],.            
+00009c10: 6e64 696d 5f73 7570 703d 312c 0a20 2020  ndim_supp=1,.   
+00009c20: 2020 2020 2029 2872 6e67 2c20 6e2c 2065       )(rng, n, e
+00009c30: 7461 2c20 7364 5f64 6973 7429 0a0a 0a40  ta, sd_dist)...@
+00009c40: 5f63 6861 6e67 655f 6469 7374 5f73 697a  _change_dist_siz
+00009c50: 652e 7265 6769 7374 6572 285f 4c4b 4a43  e.register(_LKJC
+00009c60: 686f 6c65 736b 7943 6f76 5256 290a 6465  holeskyCovRV).de
+00009c70: 6620 6368 616e 6765 5f4c 4b4a 4368 6f6c  f change_LKJChol
+00009c80: 656b 7379 436f 7652 565f 7369 7a65 286f  eksyCovRV_size(o
+00009c90: 702c 2064 6973 742c 206e 6577 5f73 697a  p, dist, new_siz
+00009ca0: 652c 2065 7870 616e 643d 4661 6c73 6529  e, expand=False)
+00009cb0: 3a0a 2020 2020 6e2c 2065 7461 2c20 7364  :.    n, eta, sd
+00009cc0: 5f64 6973 7420 3d20 6469 7374 2e6f 776e  _dist = dist.own
+00009cd0: 6572 2e69 6e70 7574 735b 313a 5d0a 0a20  er.inputs[1:].. 
+00009ce0: 2020 2069 6620 6578 7061 6e64 3a0a 2020     if expand:.  
+00009cf0: 2020 2020 2020 6f6c 645f 7369 7a65 203d        old_size =
+00009d00: 2073 645f 6469 7374 2e73 6861 7065 5b3a   sd_dist.shape[:
+00009d10: 2d31 5d0a 2020 2020 2020 2020 6e65 775f  -1].        new_
+00009d20: 7369 7a65 203d 2074 7570 6c65 286e 6577  size = tuple(new
+00009d30: 5f73 697a 6529 202b 2074 7570 6c65 286f  _size) + tuple(o
+00009d40: 6c64 5f73 697a 6529 0a0a 2020 2020 7265  ld_size)..    re
+00009d50: 7475 726e 205f 4c4b 4a43 686f 6c65 736b  turn _LKJCholesk
+00009d60: 7943 6f76 2e72 765f 6f70 286e 2c20 6574  yCov.rv_op(n, et
+00009d70: 612c 2073 645f 6469 7374 2c20 7369 7a65  a, sd_dist, size
+00009d80: 3d6e 6577 5f73 697a 6529 0a0a 0a40 5f6d  =new_size)...@_m
+00009d90: 6f6d 656e 742e 7265 6769 7374 6572 285f  oment.register(_
+00009da0: 4c4b 4a43 686f 6c65 736b 7943 6f76 5256  LKJCholeskyCovRV
+00009db0: 290a 6465 6620 5f4c 4b4a 4368 6f6c 656b  ).def _LKJCholek
+00009dc0: 7379 436f 7652 565f 6d6f 6d65 6e74 286f  syCovRV_moment(o
+00009dd0: 702c 2072 762c 2072 6e67 2c20 6e2c 2065  p, rv, rng, n, e
+00009de0: 7461 2c20 7364 5f64 6973 7429 3a0a 2020  ta, sd_dist):.  
+00009df0: 2020 6469 6167 5f69 6478 7320 3d20 2870    diag_idxs = (p
+00009e00: 742e 6375 6d73 756d 2870 742e 6172 616e  t.cumsum(pt.aran
+00009e10: 6765 2831 2c20 6e20 2b20 3129 2920 2d20  ge(1, n + 1)) - 
+00009e20: 3129 2e61 7374 7970 6528 2269 6e74 3332  1).astype("int32
+00009e30: 2229 0a20 2020 206d 6f6d 656e 7420 3d20  ").    moment = 
+00009e40: 7074 2e7a 6572 6f73 5f6c 696b 6528 7276  pt.zeros_like(rv
+00009e50: 290a 2020 2020 6d6f 6d65 6e74 203d 2070  ).    moment = p
+00009e60: 742e 7365 745f 7375 6274 656e 736f 7228  t.set_subtensor(
+00009e70: 6d6f 6d65 6e74 5b2e 2e2e 2c20 6469 6167  moment[..., diag
+00009e80: 5f69 6478 735d 2c20 3129 0a20 2020 2072  _idxs], 1).    r
+00009e90: 6574 7572 6e20 6d6f 6d65 6e74 0a0a 0a40  eturn moment...@
+00009ea0: 5f64 6566 6175 6c74 5f74 7261 6e73 666f  _default_transfo
+00009eb0: 726d 2e72 6567 6973 7465 7228 5f4c 4b4a  rm.register(_LKJ
+00009ec0: 4368 6f6c 6573 6b79 436f 7652 5629 0a64  CholeskyCovRV).d
+00009ed0: 6566 205f 4c4b 4a43 686f 6c65 6b73 7943  ef _LKJCholeksyC
+00009ee0: 6f76 5256 5f64 6566 6175 6c74 5f74 7261  ovRV_default_tra
+00009ef0: 6e73 666f 726d 286f 702c 2072 7629 3a0a  nsform(op, rv):.
+00009f00: 2020 2020 5f2c 206e 2c20 5f2c 205f 203d      _, n, _, _ =
+00009f10: 2072 762e 6f77 6e65 722e 696e 7075 7473   rv.owner.inputs
+00009f20: 0a20 2020 2072 6574 7572 6e20 7472 616e  .    return tran
+00009f30: 7366 6f72 6d73 2e43 686f 6c65 736b 7943  sforms.CholeskyC
+00009f40: 6f76 5061 636b 6564 286e 290a 0a0a 405f  ovPacked(n)...@_
+00009f50: 6c6f 6770 726f 622e 7265 6769 7374 6572  logprob.register
+00009f60: 285f 4c4b 4a43 686f 6c65 736b 7943 6f76  (_LKJCholeskyCov
+00009f70: 5256 290a 6465 6620 5f4c 4b4a 4368 6f6c  RV).def _LKJChol
+00009f80: 656b 7379 436f 7652 565f 6c6f 6770 286f  eksyCovRV_logp(o
+00009f90: 702c 2076 616c 7565 732c 2072 6e67 2c20  p, values, rng, 
+00009fa0: 6e2c 2065 7461 2c20 7364 5f64 6973 742c  n, eta, sd_dist,
+00009fb0: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
+00009fc0: 2876 616c 7565 2c29 203d 2076 616c 7565  (value,) = value
+00009fd0: 730a 0a20 2020 2069 6620 7661 6c75 652e  s..    if value.
+00009fe0: 6e64 696d 203e 2031 3a0a 2020 2020 2020  ndim > 1:.      
+00009ff0: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+0000a000: 6f72 2822 5f4c 4b4a 4368 6f6c 6573 6b79  or("_LKJCholesky
+0000a010: 436f 7620 6c6f 6770 2069 7320 6f6e 6c79  Cov logp is only
+0000a020: 2069 6d70 6c65 6d65 6e74 6564 2066 6f72   implemented for
+0000a030: 2076 6563 746f 7220 7661 6c75 6573 2028   vector values (
+0000a040: 6e64 696d 3d31 2922 290a 0a20 2020 2064  ndim=1)")..    d
+0000a050: 6961 675f 6964 7873 203d 2070 742e 6375  iag_idxs = pt.cu
+0000a060: 6d73 756d 2870 742e 6172 616e 6765 2831  msum(pt.arange(1
+0000a070: 2c20 6e20 2b20 3129 2920 2d20 310a 2020  , n + 1)) - 1.  
+0000a080: 2020 6375 6d73 756d 203d 2070 742e 6375    cumsum = pt.cu
+0000a090: 6d73 756d 2876 616c 7565 2a2a 3229 0a20  msum(value**2). 
+0000a0a0: 2020 2076 6172 6961 6e63 6520 3d20 7074     variance = pt
+0000a0b0: 2e7a 6572 6f73 2870 742e 6174 6c65 6173  .zeros(pt.atleas
+0000a0c0: 745f 3164 286e 2929 0a20 2020 2076 6172  t_1d(n)).    var
+0000a0d0: 6961 6e63 6520 3d20 7074 2e69 6e63 5f73  iance = pt.inc_s
+0000a0e0: 7562 7465 6e73 6f72 2876 6172 6961 6e63  ubtensor(varianc
+0000a0f0: 655b 305d 2c20 7661 6c75 655b 305d 202a  e[0], value[0] *
+0000a100: 2a20 3229 0a20 2020 2076 6172 6961 6e63  * 2).    varianc
+0000a110: 6520 3d20 7074 2e69 6e63 5f73 7562 7465  e = pt.inc_subte
+0000a120: 6e73 6f72 2876 6172 6961 6e63 655b 313a  nsor(variance[1:
+0000a130: 5d2c 2063 756d 7375 6d5b 6469 6167 5f69  ], cumsum[diag_i
+0000a140: 6478 735b 313a 5d5d 202d 2063 756d 7375  dxs[1:]] - cumsu
+0000a150: 6d5b 6469 6167 5f69 6478 735b 3a2d 315d  m[diag_idxs[:-1]
+0000a160: 5d29 0a20 2020 2073 645f 7661 6c73 203d  ]).    sd_vals =
+0000a170: 2070 742e 7371 7274 2876 6172 6961 6e63   pt.sqrt(varianc
+0000a180: 6529 0a0a 2020 2020 6c6f 6770 5f73 6420  e)..    logp_sd 
+0000a190: 3d20 706d 2e6c 6f67 7028 7364 5f64 6973  = pm.logp(sd_dis
+0000a1a0: 742c 2073 645f 7661 6c73 292e 7375 6d28  t, sd_vals).sum(
+0000a1b0: 290a 2020 2020 636f 7272 5f64 6961 6720  ).    corr_diag 
+0000a1c0: 3d20 7661 6c75 655b 6469 6167 5f69 6478  = value[diag_idx
+0000a1d0: 735d 202f 2073 645f 7661 6c73 0a0a 2020  s] / sd_vals..  
+0000a1e0: 2020 6c6f 6770 5f6c 6b6a 203d 2028 3220    logp_lkj = (2 
+0000a1f0: 2a20 6574 6120 2d20 3320 2b20 6e20 2d20  * eta - 3 + n - 
+0000a200: 7074 2e61 7261 6e67 6528 6e29 2920 2a20  pt.arange(n)) * 
+0000a210: 7074 2e6c 6f67 2863 6f72 725f 6469 6167  pt.log(corr_diag
+0000a220: 290a 2020 2020 6c6f 6770 5f6c 6b6a 203d  ).    logp_lkj =
+0000a230: 2070 742e 7375 6d28 6c6f 6770 5f6c 6b6a   pt.sum(logp_lkj
+0000a240: 290a 0a20 2020 2023 2043 6f6d 7075 7465  )..    # Compute
+0000a250: 2074 6865 206c 6f67 2064 6574 206a 6163   the log det jac
+0000a260: 6f62 6961 6e20 6f66 2074 6865 2073 6563  obian of the sec
+0000a270: 6f6e 6420 7472 616e 7366 6f72 6d61 7469  ond transformati
+0000a280: 6f6e 0a20 2020 2023 2064 6573 6372 6962  on.    # describ
+0000a290: 6564 2069 6e20 7468 6520 646f 6373 7472  ed in the docstr
+0000a2a0: 696e 672e 0a20 2020 2069 6478 203d 2070  ing..    idx = p
+0000a2b0: 742e 6172 616e 6765 286e 290a 2020 2020  t.arange(n).    
+0000a2c0: 6465 745f 696e 766a 6163 203d 2070 742e  det_invjac = pt.
+0000a2d0: 6c6f 6728 636f 7272 5f64 6961 6729 202d  log(corr_diag) -
+0000a2e0: 2069 6478 202a 2070 742e 6c6f 6728 7364   idx * pt.log(sd
+0000a2f0: 5f76 616c 7329 0a20 2020 2064 6574 5f69  _vals).    det_i
+0000a300: 6e76 6a61 6320 3d20 6465 745f 696e 766a  nvjac = det_invj
+0000a310: 6163 2e73 756d 2829 0a0a 2020 2020 2320  ac.sum()..    # 
+0000a320: 544f 444f 3a20 5f6c 6b6a 5f6e 6f72 6d61  TODO: _lkj_norma
+0000a330: 6c69 7a69 6e67 5f63 6f6e 7374 616e 7420  lizing_constant 
+0000a340: 6375 7272 656e 746c 7920 7265 7175 6972  currently requir
+0000a350: 6573 2060 6574 6160 2061 6e64 2060 6e60  es `eta` and `n`
+0000a360: 2074 6f20 6265 2063 6f6e 7374 616e 7473   to be constants
+0000a370: 0a20 2020 2069 6620 6e6f 7420 6973 696e  .    if not isin
+0000a380: 7374 616e 6365 286e 2c20 436f 6e73 7461  stance(n, Consta
+0000a390: 6e74 293a 0a20 2020 2020 2020 2072 6169  nt):.        rai
+0000a3a0: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+0000a3b0: 6445 7272 6f72 2822 6c6f 6770 206f 6e6c  dError("logp onl
+0000a3c0: 7920 696d 706c 656d 656e 7465 6420 666f  y implemented fo
+0000a3d0: 7220 636f 6e73 7461 6e74 2060 6e60 2229  r constant `n`")
+0000a3e0: 0a20 2020 206e 203d 2069 6e74 286e 2e64  .    n = int(n.d
+0000a3f0: 6174 6129 0a0a 2020 2020 6966 206e 6f74  ata)..    if not
+0000a400: 2069 7369 6e73 7461 6e63 6528 6574 612c   isinstance(eta,
+0000a410: 2043 6f6e 7374 616e 7429 3a0a 2020 2020   Constant):.    
+0000a420: 2020 2020 7261 6973 6520 4e6f 7449 6d70      raise NotImp
+0000a430: 6c65 6d65 6e74 6564 4572 726f 7228 226c  lementedError("l
+0000a440: 6f67 7020 6f6e 6c79 2069 6d70 6c65 6d65  ogp only impleme
+0000a450: 6e74 6564 2066 6f72 2063 6f6e 7374 616e  nted for constan
+0000a460: 7420 6065 7461 6022 290a 2020 2020 6574  t `eta`").    et
+0000a470: 6120 3d20 666c 6f61 7428 6574 612e 6461  a = float(eta.da
+0000a480: 7461 290a 0a20 2020 206e 6f72 6d20 3d20  ta)..    norm = 
+0000a490: 5f6c 6b6a 5f6e 6f72 6d61 6c69 7a69 6e67  _lkj_normalizing
+0000a4a0: 5f63 6f6e 7374 616e 7428 6574 612c 206e  _constant(eta, n
+0000a4b0: 290a 0a20 2020 2072 6574 7572 6e20 6e6f  )..    return no
+0000a4c0: 726d 202b 206c 6f67 705f 6c6b 6a20 2b20  rm + logp_lkj + 
+0000a4d0: 6c6f 6770 5f73 6420 2b20 6465 745f 696e  logp_sd + det_in
+0000a4e0: 766a 6163 0a0a 0a63 6c61 7373 204c 4b4a  vjac...class LKJ
+0000a4f0: 4368 6f6c 6573 6b79 436f 763a 0a20 2020  CholeskyCov:.   
+0000a500: 2072 2222 2257 7261 7070 6572 2063 6c61   r"""Wrapper cla
+0000a510: 7373 2066 6f72 2063 6f76 6172 6961 6e63  ss for covarianc
+0000a520: 6520 6d61 7472 6978 2077 6974 6820 4c4b  e matrix with LK
+0000a530: 4a20 6469 7374 7269 6275 7465 6420 636f  J distributed co
+0000a540: 7272 656c 6174 696f 6e73 2e0a 0a20 2020  rrelations...   
+0000a550: 2054 6869 7320 6465 6669 6e65 7320 6120   This defines a 
+0000a560: 6469 7374 7269 6275 7469 6f6e 206f 7665  distribution ove
+0000a570: 7220 4368 6f6c 6573 6b79 2064 6563 6f6d  r Cholesky decom
+0000a580: 706f 7365 6420 636f 7661 7269 616e 6365  posed covariance
+0000a590: 0a20 2020 206d 6174 7269 6365 732c 2073  .    matrices, s
+0000a5a0: 7563 6820 7468 6174 2074 6865 2075 6e64  uch that the und
+0000a5b0: 6572 6c79 696e 6720 636f 7272 656c 6174  erlying correlat
+0000a5c0: 696f 6e20 6d61 7472 6963 6573 2066 6f6c  ion matrices fol
+0000a5d0: 6c6f 7720 616e 0a20 2020 204c 4b4a 2064  low an.    LKJ d
+0000a5e0: 6973 7472 6962 7574 696f 6e20 5b31 5d20  istribution [1] 
+0000a5f0: 616e 6420 7468 6520 7374 616e 6461 7264  and the standard
+0000a600: 2064 6576 6961 7469 6f6e 7320 666f 6c6c   deviations foll
+0000a610: 6f77 2061 6e20 6172 6269 7472 6172 790a  ow an arbitrary.
+0000a620: 2020 2020 6469 7374 7269 6275 7469 6f6e      distribution
+0000a630: 2073 7065 6369 6669 6564 2062 7920 7468   specified by th
+0000a640: 6520 7573 6572 2e0a 0a20 2020 2050 6172  e user...    Par
+0000a650: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0000a660: 2d2d 2d2d 2d2d 0a20 2020 206e 616d 6520  ------.    name 
+0000a670: 3a20 7374 720a 2020 2020 2020 2020 5468  : str.        Th
+0000a680: 6520 6e61 6d65 2067 6976 656e 2074 6f20  e name given to 
+0000a690: 7468 6520 7661 7269 6162 6c65 2069 6e20  the variable in 
+0000a6a0: 7468 6520 6d6f 6465 6c2e 0a20 2020 2065  the model..    e
+0000a6b0: 7461 203a 2074 656e 736f 725f 6c69 6b65  ta : tensor_like
+0000a6c0: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
+0000a6d0: 2020 5468 6520 7368 6170 6520 7061 7261    The shape para
+0000a6e0: 6d65 7465 7220 2865 7461 203e 2030 2920  meter (eta > 0) 
+0000a6f0: 6f66 2074 6865 204c 4b4a 2064 6973 7472  of the LKJ distr
+0000a700: 6962 7574 696f 6e2e 2065 7461 203d 2031  ibution. eta = 1
+0000a710: 0a20 2020 2020 2020 2069 6d70 6c69 6573  .        implies
+0000a720: 2061 2075 6e69 666f 726d 2064 6973 7472   a uniform distr
+0000a730: 6962 7574 696f 6e20 6f66 2074 6865 2063  ibution of the c
+0000a740: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
+0000a750: 6365 733b 0a20 2020 2020 2020 206c 6172  ces;.        lar
+0000a760: 6765 7220 7661 6c75 6573 2070 7574 206d  ger values put m
+0000a770: 6f72 6520 7765 6967 6874 206f 6e20 6d61  ore weight on ma
+0000a780: 7472 6963 6573 2077 6974 6820 6665 7720  trices with few 
+0000a790: 636f 7272 656c 6174 696f 6e73 2e0a 2020  correlations..  
+0000a7a0: 2020 6e20 3a20 7465 6e73 6f72 5f6c 696b    n : tensor_lik
+0000a7b0: 6520 6f66 2069 6e74 0a20 2020 2020 2020  e of int.       
+0000a7c0: 2044 696d 656e 7369 6f6e 206f 6620 7468   Dimension of th
+0000a7d0: 6520 636f 7661 7269 616e 6365 206d 6174  e covariance mat
+0000a7e0: 7269 7820 286e 203e 2031 292e 0a20 2020  rix (n > 1)..   
+0000a7f0: 2073 645f 6469 7374 203a 2044 6973 7472   sd_dist : Distr
+0000a800: 6962 7574 696f 6e0a 2020 2020 2020 2020  ibution.        
+0000a810: 4120 706f 7369 7469 7665 2073 6361 6c61  A positive scala
+0000a820: 7220 6f72 2076 6563 746f 7220 6469 7374  r or vector dist
+0000a830: 7269 6275 7469 6f6e 2066 6f72 2074 6865  ribution for the
+0000a840: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+0000a850: 696f 6e73 2c20 6372 6561 7465 640a 2020  ions, created.  
+0000a860: 2020 2020 2020 7769 7468 2074 6865 2060        with the `
+0000a870: 2e64 6973 7428 2960 2041 5049 2e20 5368  .dist()` API. Sh
+0000a880: 6f75 6c64 2068 6176 6520 6073 6861 7065  ould have `shape
+0000a890: 5b2d 315d 3d6e 602e 2053 6361 6c61 7220  [-1]=n`. Scalar 
+0000a8a0: 6469 7374 7269 6275 7469 6f6e 7320 7769  distributions wi
+0000a8b0: 6c6c 2062 650a 2020 2020 2020 2020 6175  ll be.        au
+0000a8c0: 746f 6d61 7469 6361 6c6c 7920 7265 7369  tomatically resi
+0000a8d0: 7a65 6420 746f 2065 6e73 7572 6520 7468  zed to ensure th
+0000a8e0: 6973 2e0a 0a20 2020 2020 2020 202e 2e20  is...        .. 
+0000a8f0: 7761 726e 696e 673a 3a20 7364 5f64 6973  warning:: sd_dis
+0000a900: 7420 7769 6c6c 2062 6520 636c 6f6e 6564  t will be cloned
+0000a910: 2c20 7265 6e64 6572 696e 6720 6974 2069  , rendering it i
+0000a920: 6e64 6570 656e 6465 6e74 206f 6620 7468  ndependent of th
+0000a930: 6520 6f6e 6520 7061 7373 6564 2061 7320  e one passed as 
+0000a940: 696e 7075 742e 0a0a 2020 2020 636f 6d70  input...    comp
+0000a950: 7574 655f 636f 7272 203a 2062 6f6f 6c2c  ute_corr : bool,
+0000a960: 2064 6566 6175 6c74 3d54 7275 650a 2020   default=True.  
+0000a970: 2020 2020 2020 4966 2060 5472 7565 602c        If `True`,
+0000a980: 2072 6574 7572 6e73 2074 6872 6565 2076   returns three v
+0000a990: 616c 7565 733a 2074 6865 2043 686f 6c65  alues: the Chole
+0000a9a0: 736b 7920 6465 636f 6d70 6f73 6974 696f  sky decompositio
+0000a9b0: 6e2c 2074 6865 2063 6f72 7265 6c61 7469  n, the correlati
+0000a9c0: 6f6e 730a 2020 2020 2020 2020 616e 6420  ons.        and 
+0000a9d0: 7468 6520 7374 616e 6461 7264 2064 6576  the standard dev
+0000a9e0: 6961 7469 6f6e 7320 6f66 2074 6865 2063  iations of the c
+0000a9f0: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000aa00: 2e20 4f74 6865 7277 6973 652c 206f 6e6c  . Otherwise, onl
+0000aa10: 7920 7265 7475 726e 730a 2020 2020 2020  y returns.      
+0000aa20: 2020 7468 6520 7061 636b 6564 2043 686f    the packed Cho
+0000aa30: 6c65 736b 7920 6465 636f 6d70 6f73 6974  lesky decomposit
+0000aa40: 696f 6e2e 2044 6566 6175 6c74 7320 746f  ion. Defaults to
+0000aa50: 2060 5472 7565 602e 0a20 2020 2020 2020   `True`..       
+0000aa60: 2063 6f6d 7061 7469 6269 6c69 7479 2e0a   compatibility..
+0000aa70: 2020 2020 7374 6f72 655f 696e 5f74 7261      store_in_tra
+0000aa80: 6365 203a 2062 6f6f 6c2c 2064 6566 6175  ce : bool, defau
+0000aa90: 6c74 3d54 7275 650a 2020 2020 2020 2020  lt=True.        
+0000aaa0: 5768 6574 6865 7220 746f 2073 746f 7265  Whether to store
+0000aab0: 2074 6865 2063 6f72 7265 6c61 7469 6f6e   the correlation
+0000aac0: 7320 616e 6420 7374 616e 6461 7264 2064  s and standard d
+0000aad0: 6576 6961 7469 6f6e 7320 6f66 2074 6865  eviations of the
+0000aae0: 2063 6f76 6172 6961 6e63 650a 2020 2020   covariance.    
+0000aaf0: 2020 2020 6d61 7472 6978 2069 6e20 7468      matrix in th
+0000ab00: 6520 706f 7374 6572 696f 7220 7472 6163  e posterior trac
+0000ab10: 652e 2049 6620 6054 7275 6560 2c20 7468  e. If `True`, th
+0000ab20: 6579 2077 696c 6c20 6175 746f 6d61 7469  ey will automati
+0000ab30: 6361 6c6c 7920 6265 206e 616d 6564 2061  cally be named a
+0000ab40: 730a 2020 2020 2020 2020 607b 6e61 6d65  s.        `{name
+0000ab50: 7d5f 636f 7272 6020 616e 6420 607b 6e61  }_corr` and `{na
+0000ab60: 6d65 7d5f 7374 6473 6020 7265 7370 6563  me}_stds` respec
+0000ab70: 7469 7665 6c79 2e20 4566 6665 6374 6976  tively. Effectiv
+0000ab80: 6520 6f6e 6c79 2077 6865 6e0a 2020 2020  e only when.    
+0000ab90: 2020 2020 6063 6f6d 7075 7465 5f63 6f72      `compute_cor
+0000aba0: 723d 5472 7565 602e 0a0a 2020 2020 5265  r=True`...    Re
+0000abb0: 7475 726e 730a 2020 2020 2d2d 2d2d 2d2d  turns.    ------
+0000abc0: 2d0a 2020 2020 6368 6f6c 203a 2020 5465  -.    chol :  Te
+0000abd0: 6e73 6f72 5661 7269 6162 6c65 0a20 2020  nsorVariable.   
+0000abe0: 2020 2020 2049 6620 6063 6f6d 7075 7465       If `compute
+0000abf0: 5f63 6f72 723d 5472 7565 602e 2054 6865  _corr=True`. The
+0000ac00: 2075 6e70 6163 6b65 6420 4368 6f6c 6573   unpacked Choles
+0000ac10: 6b79 2063 6f76 6172 6961 6e63 6520 6465  ky covariance de
+0000ac20: 636f 6d70 6f73 6974 696f 6e2e 0a20 2020  composition..   
+0000ac30: 2063 6f72 7220 3a20 5465 6e73 6f72 5661   corr : TensorVa
+0000ac40: 7269 6162 6c65 0a20 2020 2020 2020 2049  riable.        I
+0000ac50: 6620 6063 6f6d 7075 7465 5f63 6f72 723d  f `compute_corr=
+0000ac60: 5472 7565 602e 2054 6865 2063 6f72 7265  True`. The corre
+0000ac70: 6c61 7469 6f6e 7320 6f66 2074 6865 2063  lations of the c
+0000ac80: 6f76 6172 6961 6e63 6520 6d61 7472 6978  ovariance matrix
+0000ac90: 2e0a 2020 2020 7374 6473 203a 2054 656e  ..    stds : Ten
+0000aca0: 736f 7256 6172 6961 626c 650a 2020 2020  sorVariable.    
+0000acb0: 2020 2020 4966 2060 636f 6d70 7574 655f      If `compute_
+0000acc0: 636f 7272 3d54 7275 6560 2e20 5468 6520  corr=True`. The 
+0000acd0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+0000ace0: 6f6e 7320 6f66 2074 6865 2063 6f76 6172  ons of the covar
+0000acf0: 6961 6e63 6520 6d61 7472 6978 2e0a 2020  iance matrix..  
+0000ad00: 2020 7061 636b 6564 5f63 686f 6c20 3a20    packed_chol : 
+0000ad10: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
+0000ad20: 2020 2020 2020 2049 6620 6063 6f6d 7075         If `compu
+0000ad30: 7465 5f63 6f72 723d 4661 6c73 6560 2054  te_corr=False` T
+0000ad40: 6865 2070 6163 6b65 6420 4368 6f6c 6573  he packed Choles
+0000ad50: 6b79 2063 6f76 6172 6961 6e63 6520 6465  ky covariance de
+0000ad60: 636f 6d70 6f73 6974 696f 6e2e 0a0a 2020  composition...  
+0000ad70: 2020 4e6f 7465 730a 2020 2020 2d2d 2d2d    Notes.    ----
+0000ad80: 2d0a 2020 2020 5369 6e63 6520 7468 6520  -.    Since the 
+0000ad90: 4368 6f6c 6573 6b79 2066 6163 746f 7220  Cholesky factor 
+0000ada0: 6973 2061 206c 6f77 6572 2074 7269 616e  is a lower trian
+0000adb0: 6775 6c61 7220 6d61 7472 6978 2c20 7765  gular matrix, we
+0000adc0: 2075 7365 2070 6163 6b65 6420 7374 6f72   use packed stor
+0000add0: 6167 6520 666f 720a 2020 2020 7468 6520  age for.    the 
+0000ade0: 6d61 7472 6978 3a20 5765 2073 746f 7265  matrix: We store
+0000adf0: 2074 6865 2076 616c 7565 7320 6f66 2074   the values of t
+0000ae00: 6865 206c 6f77 6572 2074 7269 616e 6775  he lower triangu
+0000ae10: 6c61 7220 6d61 7472 6978 2069 6e20 6120  lar matrix in a 
+0000ae20: 6f6e 652d 6469 6d65 6e73 696f 6e61 6c0a  one-dimensional.
+0000ae30: 2020 2020 6172 7261 792c 206e 756d 6265      array, numbe
+0000ae40: 7265 6420 6279 2072 6f77 3a3a 0a0a 2020  red by row::..  
+0000ae50: 2020 2020 2020 5b5b 3020 2d20 2d20 2d5d        [[0 - - -]
+0000ae60: 0a20 2020 2020 2020 2020 5b31 2032 202d  .         [1 2 -
+0000ae70: 202d 5d0a 2020 2020 2020 2020 205b 3320   -].         [3 
+0000ae80: 3420 3520 2d5d 0a20 2020 2020 2020 2020  4 5 -].         
+0000ae90: 5b36 2037 2038 2039 5d5d 0a0a 2020 2020  [6 7 8 9]]..    
+0000aea0: 5468 6520 756e 7061 636b 6564 2043 686f  The unpacked Cho
+0000aeb0: 6c65 736b 7920 636f 7661 7269 616e 6365  lesky covariance
+0000aec0: 206d 6174 7269 7820 6973 2061 7574 6f6d   matrix is autom
+0000aed0: 6174 6963 616c 6c79 2063 6f6d 7075 7465  atically compute
+0000aee0: 6420 616e 6420 7265 7475 726e 6564 2077  d and returned w
+0000aef0: 6865 6e0a 2020 2020 796f 7520 7370 6563  hen.    you spec
+0000af00: 6966 7920 6063 6f6d 7075 7465 5f63 6f72  ify `compute_cor
+0000af10: 723d 5472 7565 6020 696e 2060 706d 2e4c  r=True` in `pm.L
+0000af20: 4b4a 4368 6f6c 6573 6b79 436f 7660 2028  KJCholeskyCov` (
+0000af30: 7365 6520 6578 616d 706c 6520 6265 6c6f  see example belo
+0000af40: 7729 2e0a 2020 2020 4f74 6865 7277 6973  w)..    Otherwis
+0000af50: 652c 2079 6f75 2063 616e 2075 7365 2060  e, you can use `
+0000af60: 706d 2e65 7870 616e 645f 7061 636b 6564  pm.expand_packed
+0000af70: 5f74 7269 616e 6775 6c61 7228 7061 636b  _triangular(pack
+0000af80: 6564 5f63 6f76 2c20 6c6f 7765 723d 5472  ed_cov, lower=Tr
+0000af90: 7565 2960 0a20 2020 2074 6f20 636f 6e76  ue)`.    to conv
+0000afa0: 6572 7420 7468 6520 7061 636b 6564 2043  ert the packed C
+0000afb0: 686f 6c65 736b 7920 6d61 7472 6978 2074  holesky matrix t
+0000afc0: 6f20 6120 7265 6775 6c61 7220 7477 6f2d  o a regular two-
+0000afd0: 6469 6d65 6e73 696f 6e61 6c20 6172 7261  dimensional arra
+0000afe0: 792e 0a0a 2020 2020 4578 616d 706c 6573  y...    Examples
+0000aff0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a 2020  .    --------.  
+0000b000: 2020 2e2e 2063 6f64 653a 3a20 7079 7468    .. code:: pyth
+0000b010: 6f6e 0a0a 2020 2020 2020 2020 7769 7468  on..        with
+0000b020: 2070 6d2e 4d6f 6465 6c28 2920 6173 206d   pm.Model() as m
+0000b030: 6f64 656c 3a0a 2020 2020 2020 2020 2020  odel:.          
+0000b040: 2020 2320 4e6f 7465 2074 6861 7420 7765    # Note that we
+0000b050: 2061 6363 6573 7320 7468 6520 6469 7374   access the dist
+0000b060: 7269 6275 7469 6f6e 2066 6f72 2074 6865  ribution for the
+0000b070: 2073 7461 6e64 6172 640a 2020 2020 2020   standard.      
+0000b080: 2020 2020 2020 2320 6465 7669 6174 696f        # deviatio
+0000b090: 6e73 2c20 616e 6420 646f 206e 6f74 2063  ns, and do not c
+0000b0a0: 7265 6174 6520 6120 6e65 7720 7261 6e64  reate a new rand
+0000b0b0: 6f6d 2076 6172 6961 626c 652e 0a20 2020  om variable..   
+0000b0c0: 2020 2020 2020 2020 2073 645f 6469 7374           sd_dist
+0000b0d0: 203d 2070 6d2e 4578 706f 6e65 6e74 6961   = pm.Exponentia
+0000b0e0: 6c2e 6469 7374 2831 2e30 2c20 7369 7a65  l.dist(1.0, size
+0000b0f0: 3d31 3029 0a20 2020 2020 2020 2020 2020  =10).           
+0000b100: 2063 686f 6c2c 2063 6f72 722c 2073 6967   chol, corr, sig
+0000b110: 6d61 7320 3d20 706d 2e4c 4b4a 4368 6f6c  mas = pm.LKJChol
+0000b120: 6573 6b79 436f 7628 0a20 2020 2020 2020  eskyCov(.       
+0000b130: 2020 2020 2020 2020 2027 6368 6f6c 5f63           'chol_c
+0000b140: 6f76 272c 2065 7461 3d34 2c20 6e3d 3130  ov', eta=4, n=10
+0000b150: 2c20 7364 5f64 6973 743d 7364 5f64 6973  , sd_dist=sd_dis
+0000b160: 740a 2020 2020 2020 2020 2020 2020 290a  t.            ).
+0000b170: 0a20 2020 2020 2020 2020 2020 2023 2069  .            # i
+0000b180: 6620 796f 7520 6f6e 6c79 2077 616e 7420  f you only want 
+0000b190: 7468 6520 7061 636b 6564 2043 686f 6c65  the packed Chole
+0000b1a0: 736b 793a 0a20 2020 2020 2020 2020 2020  sky:.           
+0000b1b0: 2023 2070 6163 6b65 645f 6368 6f6c 203d   # packed_chol =
+0000b1c0: 2070 6d2e 4c4b 4a43 686f 6c65 736b 7943   pm.LKJCholeskyC
+0000b1d0: 6f76 280a 2020 2020 2020 2020 2020 2020  ov(.            
+0000b1e0: 2020 2020 2763 686f 6c5f 636f 7627 2c20      'chol_cov', 
+0000b1f0: 6574 613d 342c 206e 3d31 302c 2073 645f  eta=4, n=10, sd_
+0000b200: 6469 7374 3d73 645f 6469 7374 2c20 636f  dist=sd_dist, co
+0000b210: 6d70 7574 655f 636f 7272 3d46 616c 7365  mpute_corr=False
+0000b220: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
+0000b230: 2020 2020 2020 2020 2020 2023 2063 686f             # cho
+0000b240: 6c20 3d20 706d 2e65 7870 616e 645f 7061  l = pm.expand_pa
+0000b250: 636b 6564 5f74 7269 616e 6775 6c61 7228  cked_triangular(
+0000b260: 3130 2c20 7061 636b 6564 5f63 686f 6c2c  10, packed_chol,
+0000b270: 206c 6f77 6572 3d54 7275 6529 0a0a 2020   lower=True)..  
+0000b280: 2020 2020 2020 2020 2020 2320 4465 6669            # Defi
+0000b290: 6e65 2061 206e 6577 204d 764e 6f72 6d61  ne a new MvNorma
+0000b2a0: 6c20 7769 7468 2074 6865 2067 6976 656e  l with the given
+0000b2b0: 2063 6f76 6172 6961 6e63 650a 2020 2020   covariance.    
+0000b2c0: 2020 2020 2020 2020 7661 6c73 203d 2070          vals = p
+0000b2d0: 6d2e 4d76 4e6f 726d 616c 2827 7661 6c73  m.MvNormal('vals
+0000b2e0: 272c 206d 753d 6e70 2e7a 6572 6f73 2831  ', mu=np.zeros(1
+0000b2f0: 3029 2c20 6368 6f6c 3d63 686f 6c2c 2073  0), chol=chol, s
+0000b300: 6861 7065 3d31 3029 0a0a 2020 2020 2020  hape=10)..      
+0000b310: 2020 2020 2020 2320 4f72 2074 7261 6e73        # Or trans
+0000b320: 666f 726d 2061 6e20 756e 636f 7272 656c  form an uncorrel
+0000b330: 6174 6564 206e 6f72 6d61 6c3a 0a20 2020  ated normal:.   
+0000b340: 2020 2020 2020 2020 2076 616c 735f 7261           vals_ra
+0000b350: 7720 3d20 706d 2e4e 6f72 6d61 6c28 2776  w = pm.Normal('v
+0000b360: 616c 735f 7261 7727 2c20 6d75 3d30 2c20  als_raw', mu=0, 
+0000b370: 7369 676d 613d 312c 2073 6861 7065 3d31  sigma=1, shape=1
+0000b380: 3029 0a20 2020 2020 2020 2020 2020 2076  0).            v
+0000b390: 616c 7320 3d20 7074 2e64 6f74 2863 686f  als = pt.dot(cho
+0000b3a0: 6c2c 2076 616c 735f 7261 7729 0a0a 2020  l, vals_raw)..  
+0000b3b0: 2020 2020 2020 2020 2020 2320 4f72 2063            # Or c
+0000b3c0: 6f6d 7075 7465 2074 6865 2063 6f76 6172  ompute the covar
+0000b3d0: 6961 6e63 6520 6d61 7472 6978 0a20 2020  iance matrix.   
+0000b3e0: 2020 2020 2020 2020 2063 6f76 203d 2070           cov = p
+0000b3f0: 742e 646f 7428 6368 6f6c 2c20 6368 6f6c  t.dot(chol, chol
+0000b400: 2e54 290a 0a20 2020 202a 2a49 6d70 6c65  .T)..    **Imple
+0000b410: 6d65 6e74 6174 696f 6e2a 2a20 496e 2074  mentation** In t
+0000b420: 6865 2075 6e63 6f6e 7374 7261 696e 6564  he unconstrained
+0000b430: 2073 7061 6365 2061 6c6c 2076 616c 7565   space all value
+0000b440: 7320 6f66 2074 6865 2063 686f 6c65 736b  s of the cholesk
+0000b450: 7920 6661 6374 6f72 0a20 2020 2061 7265  y factor.    are
+0000b460: 2073 746f 7265 6420 756e 7472 616e 7366   stored untransf
+0000b470: 6f72 6d65 642c 2065 7863 6570 7420 666f  ormed, except fo
+0000b480: 7220 7468 6520 6469 6167 6f6e 616c 2065  r the diagonal e
+0000b490: 6e74 7269 6573 2c20 7768 6572 650a 2020  ntries, where.  
+0000b4a0: 2020 7765 2075 7365 2061 206c 6f67 2d74    we use a log-t
+0000b4b0: 7261 6e73 666f 726d 2074 6f20 7265 7374  ransform to rest
+0000b4c0: 7269 6374 2074 6865 6d20 746f 2070 6f73  rict them to pos
+0000b4d0: 6974 6976 6520 7661 6c75 6573 2e0a 0a20  itive values... 
+0000b4e0: 2020 2054 6f20 636f 7272 6563 746c 7920     To correctly 
+0000b4f0: 636f 6d70 7574 6520 6c6f 672d 6c69 6b65  compute log-like
+0000b500: 6c69 686f 6f64 7320 666f 7220 7468 6520  lihoods for the 
+0000b510: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+0000b520: 6f6e 730a 2020 2020 616e 6420 7468 6520  ons.    and the 
+0000b530: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
+0000b540: 6978 2073 6570 6172 6174 656c 792c 2077  ix separately, w
+0000b550: 6520 6e65 6564 2074 6f20 636f 6e73 6964  e need to consid
+0000b560: 6572 2061 0a20 2020 2073 6563 6f6e 6420  er a.    second 
+0000b570: 7472 616e 7366 6f72 6d61 7469 6f6e 3a20  transformation: 
+0000b580: 4769 7665 6e20 6120 6368 6f6c 6573 6b79  Given a cholesky
+0000b590: 2066 6163 746f 7269 7a61 7469 6f6e 0a20   factorization. 
+0000b5a0: 2020 203a 6d61 7468 3a60 4c4c 5e54 203d     :math:`LL^T =
+0000b5b0: 205c 5369 676d 6160 206f 6620 6120 636f   \Sigma` of a co
+0000b5c0: 7661 7269 616e 6365 206d 6174 7269 7820  variance matrix 
+0000b5d0: 7765 2063 616e 2072 6563 6f76 6572 2074  we can recover t
+0000b5e0: 6865 0a20 2020 2073 7461 6e64 6172 6420  he.    standard 
+0000b5f0: 6465 7669 6174 696f 6e73 203a 6d61 7468  deviations :math
+0000b600: 3a60 5c73 6967 6d61 6020 6173 2074 6865  :`\sigma` as the
+0000b610: 2065 7563 6c69 6465 616e 206c 656e 6774   euclidean lengt
+0000b620: 6873 206f 660a 2020 2020 7468 6520 726f  hs of.    the ro
+0000b630: 7773 206f 6620 3a6d 6174 683a 604c 602c  ws of :math:`L`,
+0000b640: 2061 6e64 2074 6865 2063 686f 6c65 736b   and the cholesk
+0000b650: 7920 6661 6374 6f72 206f 6620 7468 650a  y factor of the.
+0000b660: 2020 2020 636f 7272 656c 6174 696f 6e20      correlation 
+0000b670: 6d61 7472 6978 2061 7320 3a6d 6174 683a  matrix as :math:
+0000b680: 6055 203d 205c 7465 7874 7b64 6961 677d  `U = \text{diag}
+0000b690: 285c 7369 676d 6129 5e7b 2d31 7d4c 602e  (\sigma)^{-1}L`.
+0000b6a0: 0a20 2020 2053 696e 6365 2065 6163 6820  .    Since each 
+0000b6b0: 726f 7720 6f66 203a 6d61 7468 3a60 5560  row of :math:`U`
+0000b6c0: 2068 6173 206c 656e 6774 6820 312c 2077   has length 1, w
+0000b6d0: 6520 646f 206e 6f74 206e 6565 6420 746f  e do not need to
+0000b6e0: 0a20 2020 2073 746f 7265 2074 6865 2064  .    store the d
+0000b6f0: 6961 676f 6e61 6c2e 2057 6520 6465 6669  iagonal. We defi
+0000b700: 6e65 2061 2074 7261 6e73 666f 726d 6174  ne a transformat
+0000b710: 696f 6e20 3a6d 6174 683a 605c 7068 6960  ion :math:`\phi`
+0000b720: 0a20 2020 2073 7563 6820 7468 6174 203a  .    such that :
+0000b730: 6d61 7468 3a60 5c70 6869 284c 2960 2069  math:`\phi(L)` i
+0000b740: 7320 7468 6520 6c6f 7765 7220 7472 6961  s the lower tria
+0000b750: 6e67 756c 6172 206d 6174 7269 7820 636f  ngular matrix co
+0000b760: 6e74 6169 6e69 6e67 0a20 2020 2074 6865  ntaining.    the
+0000b770: 2073 7461 6e64 6172 6420 6465 7669 6174   standard deviat
+0000b780: 696f 6e73 203a 6d61 7468 3a60 5c73 6967  ions :math:`\sig
+0000b790: 6d61 6020 6f6e 2074 6865 2064 6961 676f  ma` on the diago
+0000b7a0: 6e61 6c20 616e 6420 7468 650a 2020 2020  nal and the.    
+0000b7b0: 636f 7272 656c 6174 696f 6e20 6d61 7472  correlation matr
+0000b7c0: 6978 203a 6d61 7468 3a60 5560 2062 656c  ix :math:`U` bel
+0000b7d0: 6f77 2e20 496e 2074 6869 7320 666f 726d  ow. In this form
+0000b7e0: 2077 6520 6361 6e20 6561 7369 6c79 0a20   we can easily. 
+0000b7f0: 2020 2063 6f6d 7075 7465 2074 6865 2064     compute the d
+0000b800: 6966 6665 7265 6e74 206c 696b 656c 6968  ifferent likelih
+0000b810: 6f6f 6473 2073 6570 6172 6174 656c 792c  oods separately,
+0000b820: 2061 7320 7468 6520 6c69 6b65 6c69 686f   as the likeliho
+0000b830: 6f64 0a20 2020 206f 6620 7468 6520 636f  od.    of the co
+0000b840: 7272 656c 6174 696f 6e20 6d61 7472 6978  rrelation matrix
+0000b850: 206f 6e6c 7920 6465 7065 6e64 7320 6f6e   only depends on
+0000b860: 2074 6865 2076 616c 7565 7320 6265 6c6f   the values belo
+0000b870: 7720 7468 650a 2020 2020 6469 6167 6f6e  w the.    diagon
+0000b880: 616c 2c20 616e 6420 7468 6520 6c69 6b65  al, and the like
+0000b890: 6c69 686f 6f64 206f 6620 7468 6520 7374  lihood of the st
+0000b8a0: 616e 6461 7264 2064 6576 6961 7469 6f6e  andard deviation
+0000b8b0: 2064 6570 656e 6473 0a20 2020 206f 6e6c   depends.    onl
+0000b8c0: 7920 6f6e 2074 6865 2064 6961 676f 6e61  y on the diagona
+0000b8d0: 6c20 7661 6c75 6573 2e0a 0a20 2020 2057  l values...    W
+0000b8e0: 6520 7374 696c 6c20 6e65 6564 2074 6865  e still need the
+0000b8f0: 2064 6574 6572 6d69 6e61 6e74 206f 6620   determinant of 
+0000b900: 7468 6520 6a61 636f 6269 616e 206f 6620  the jacobian of 
+0000b910: 3a6d 6174 683a 605c 7068 695e 7b2d 317d  :math:`\phi^{-1}
+0000b920: 602e 0a20 2020 2049 6620 7765 2074 6869  `..    If we thi
+0000b930: 6e6b 206f 6620 3a6d 6174 683a 605c 7068  nk of :math:`\ph
+0000b940: 6960 2061 7320 616e 2061 7574 6f6d 6f72  i` as an automor
+0000b950: 7068 6973 6d20 6f6e 0a20 2020 203a 6d61  phism on.    :ma
+0000b960: 7468 3a60 5c6d 6174 6862 627b 527d 5e7b  th:`\mathbb{R}^{
+0000b970: 5c74 6672 6163 7b6e 286e 2b31 297d 7b32  \tfrac{n(n+1)}{2
+0000b980: 7d7d 602c 2077 6865 7265 2077 6520 6f72  }}`, where we or
+0000b990: 6465 720a 2020 2020 7468 6520 6469 6d65  der.    the dime
+0000b9a0: 6e73 696f 6e73 2061 7320 6465 7363 7269  nsions as descri
+0000b9b0: 6265 6420 696e 2074 6865 206e 6f74 6573  bed in the notes
+0000b9c0: 2061 626f 7665 2c20 7468 6520 6a61 636f   above, the jaco
+0000b9d0: 6269 616e 0a20 2020 2069 7320 6120 626c  bian.    is a bl
+0000b9e0: 6f63 6b2d 6469 6167 6f6e 616c 206d 6174  ock-diagonal mat
+0000b9f0: 7269 782c 2077 6865 7265 2065 6163 6820  rix, where each 
+0000ba00: 626c 6f63 6b20 636f 7272 6573 706f 6e64  block correspond
+0000ba10: 7320 746f 0a20 2020 206f 6e65 2072 6f77  s to.    one row
+0000ba20: 206f 6620 3a6d 6174 683a 6055 602e 2045   of :math:`U`. E
+0000ba30: 6163 6820 626c 6f63 6b20 6861 7320 6172  ach block has ar
+0000ba40: 726f 7768 6561 6420 7368 6170 652c 2061  rowhead shape, a
+0000ba50: 6e64 2077 650a 2020 2020 6361 6e20 636f  nd we.    can co
+0000ba60: 6d70 7574 6520 7468 6520 6465 7465 726d  mpute the determ
+0000ba70: 696e 616e 7420 6f66 2074 6861 7420 6173  inant of that as
+0000ba80: 2064 6573 6372 6962 6564 2069 6e20 5b32   described in [2
+0000ba90: 5d2e 2053 696e 6365 0a20 2020 2074 6865  ]. Since.    the
+0000baa0: 2064 6574 6572 6d69 6e61 6e74 206f 6620   determinant of 
+0000bab0: 6120 626c 6f63 6b2d 6469 6167 6f6e 616c  a block-diagonal
+0000bac0: 206d 6174 7269 7820 6973 2074 6865 2070   matrix is the p
+0000bad0: 726f 6475 6374 0a20 2020 206f 6620 7468  roduct.    of th
+0000bae0: 6520 6465 7465 726d 696e 616e 7473 206f  e determinants o
+0000baf0: 6620 7468 6520 626c 6f63 6b73 2c20 7765  f the blocks, we
+0000bb00: 2067 6574 0a0a 2020 2020 2e2e 206d 6174   get..    .. mat
+0000bb10: 683a 3a0a 0a20 2020 2020 2020 5c74 6578  h::..       \tex
+0000bb20: 747b 6465 747d 284a 5f7b 5c70 6869 5e7b  t{det}(J_{\phi^{
+0000bb30: 2d31 7d7d 2855 2929 203d 0a20 2020 2020  -1}}(U)) =.     
+0000bb40: 2020 5c6c 6566 745b 0a20 2020 2020 2020    \left[.       
+0000bb50: 2020 5c70 726f 645f 7b69 3d32 7d5e 4e20    \prod_{i=2}^N 
+0000bb60: 755f 7b69 697d 5e7b 6920 2d20 317d 204c  u_{ii}^{i - 1} L
+0000bb70: 5f7b 6969 7d0a 2020 2020 2020 205c 7269  _{ii}.       \ri
+0000bb80: 6768 745d 5e7b 2d31 7d0a 0a20 2020 2052  ght]^{-1}..    R
+0000bb90: 6566 6572 656e 6365 730a 2020 2020 2d2d  eferences.    --
+0000bba0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e 2e20  --------.    .. 
+0000bbb0: 5b31 5d20 4c65 7761 6e64 6f77 736b 692c  [1] Lewandowski,
+0000bbc0: 2044 2e2c 204b 7572 6f77 6963 6b61 2c20   D., Kurowicka, 
+0000bbd0: 442e 2061 6e64 204a 6f65 2c20 482e 2028  D. and Joe, H. (
+0000bbe0: 3230 3039 292e 0a20 2020 2020 2020 2247  2009)..       "G
+0000bbf0: 656e 6572 6174 696e 6720 7261 6e64 6f6d  enerating random
+0000bc00: 2063 6f72 7265 6c61 7469 6f6e 206d 6174   correlation mat
+0000bc10: 7269 6365 7320 6261 7365 6420 6f6e 2076  rices based on v
+0000bc20: 696e 6573 2061 6e64 0a20 2020 2020 2020  ines and.       
+0000bc30: 6578 7465 6e64 6564 206f 6e69 6f6e 206d  extended onion m
+0000bc40: 6574 686f 642e 2220 4a6f 7572 6e61 6c20  ethod." Journal 
+0000bc50: 6f66 206d 756c 7469 7661 7269 6174 6520  of multivariate 
+0000bc60: 616e 616c 7973 6973 2c0a 2020 2020 2020  analysis,.      
+0000bc70: 2031 3030 2839 292c 2070 702e 3139 3839   100(9), pp.1989
+0000bc80: 2d32 3030 312e 0a0a 2020 2020 2e2e 205b  -2001...    .. [
+0000bc90: 325d 204a 2e20 4d2e 2069 736e 2774 2061  2] J. M. isn't a
+0000bca0: 206d 6174 6865 6d61 7469 6369 616e 2028   mathematician (
+0000bcb0: 6874 7470 3a2f 2f6d 6174 682e 7374 6163  http://math.stac
+0000bcc0: 6b65 7863 6861 6e67 652e 636f 6d2f 7573  kexchange.com/us
+0000bcd0: 6572 732f 3439 382f 0a20 2020 2020 2020  ers/498/.       
+0000bce0: 6a2d 6d2d 6973 6e74 2d61 2d6d 6174 6865  j-m-isnt-a-mathe
+0000bcf0: 6d61 7469 6369 616e 292c 2044 6966 6665  matician), Diffe
+0000bd00: 7265 6e74 2061 7070 726f 6163 6865 7320  rent approaches 
+0000bd10: 746f 2065 7661 6c75 6174 6520 7468 6973  to evaluate this
+0000bd20: 0a20 2020 2020 2020 6465 7465 726d 696e  .       determin
+0000bd30: 616e 742c 2055 524c 2028 7665 7273 696f  ant, URL (versio
+0000bd40: 6e3a 2032 3031 322d 3034 2d31 3429 3a0a  n: 2012-04-14):.
+0000bd50: 2020 2020 2020 2068 7474 703a 2f2f 6d61         http://ma
+0000bd60: 7468 2e73 7461 636b 6578 6368 616e 6765  th.stackexchange
+0000bd70: 2e63 6f6d 2f71 2f31 3330 3032 360a 2020  .com/q/130026.  
+0000bd80: 2020 2222 220a 0a20 2020 2064 6566 205f    """..    def _
+0000bd90: 5f6e 6577 5f5f 2863 6c73 2c20 6e61 6d65  _new__(cls, name
+0000bda0: 2c20 6574 612c 206e 2c20 7364 5f64 6973  , eta, n, sd_dis
+0000bdb0: 742c 202a 2c20 636f 6d70 7574 655f 636f  t, *, compute_co
+0000bdc0: 7272 3d54 7275 652c 2073 746f 7265 5f69  rr=True, store_i
+0000bdd0: 6e5f 7472 6163 653d 5472 7565 2c20 2a2a  n_trace=True, **
+0000bde0: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+0000bdf0: 2070 6163 6b65 645f 6368 6f6c 203d 205f   packed_chol = _
+0000be00: 4c4b 4a43 686f 6c65 736b 7943 6f76 286e  LKJCholeskyCov(n
+0000be10: 616d 652c 2065 7461 3d65 7461 2c20 6e3d  ame, eta=eta, n=
+0000be20: 6e2c 2073 645f 6469 7374 3d73 645f 6469  n, sd_dist=sd_di
+0000be30: 7374 2c20 2a2a 6b77 6172 6773 290a 2020  st, **kwargs).  
+0000be40: 2020 2020 2020 6966 206e 6f74 2063 6f6d        if not com
+0000be50: 7075 7465 5f63 6f72 723a 0a20 2020 2020  pute_corr:.     
+0000be60: 2020 2020 2020 2072 6574 7572 6e20 7061         return pa
+0000be70: 636b 6564 5f63 686f 6c0a 2020 2020 2020  cked_chol.      
+0000be80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000be90: 2020 2020 6368 6f6c 2c20 636f 7272 2c20      chol, corr, 
+0000bea0: 7374 6473 203d 2063 6c73 2e68 656c 7065  stds = cls.helpe
+0000beb0: 725f 6465 7465 726d 696e 6973 7469 6373  r_deterministics
+0000bec0: 286e 2c20 7061 636b 6564 5f63 686f 6c29  (n, packed_chol)
+0000bed0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bee0: 7374 6f72 655f 696e 5f74 7261 6365 3a0a  store_in_trace:.
+0000bef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bf00: 636f 7272 203d 2070 6d2e 4465 7465 726d  corr = pm.Determ
+0000bf10: 696e 6973 7469 6328 6622 7b6e 616d 657d  inistic(f"{name}
+0000bf20: 5f63 6f72 7222 2c20 636f 7272 290a 2020  _corr", corr).  
+0000bf30: 2020 2020 2020 2020 2020 2020 2020 7374                st
+0000bf40: 6473 203d 2070 6d2e 4465 7465 726d 696e  ds = pm.Determin
+0000bf50: 6973 7469 6328 6622 7b6e 616d 657d 5f73  istic(f"{name}_s
+0000bf60: 7464 7322 2c20 7374 6473 290a 2020 2020  tds", stds).    
+0000bf70: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+0000bf80: 686f 6c2c 2063 6f72 722c 2073 7464 730a  hol, corr, stds.
+0000bf90: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
+0000bfa0: 640a 2020 2020 6465 6620 6469 7374 2863  d.    def dist(c
+0000bfb0: 6c73 2c20 6574 612c 206e 2c20 7364 5f64  ls, eta, n, sd_d
+0000bfc0: 6973 742c 202a 2c20 636f 6d70 7574 655f  ist, *, compute_
+0000bfd0: 636f 7272 3d54 7275 652c 202a 2a6b 7761  corr=True, **kwa
+0000bfe0: 7267 7329 3a0a 2020 2020 2020 2020 2320  rgs):.        # 
+0000bff0: 636f 6d70 7574 6520 4368 6f6c 6573 6b79  compute Cholesky
+0000c000: 2064 6563 6f6d 706f 7369 7469 6f6e 0a20   decomposition. 
+0000c010: 2020 2020 2020 2070 6163 6b65 645f 6368         packed_ch
+0000c020: 6f6c 203d 205f 4c4b 4a43 686f 6c65 736b  ol = _LKJCholesk
+0000c030: 7943 6f76 2e64 6973 7428 6574 613d 6574  yCov.dist(eta=et
+0000c040: 612c 206e 3d6e 2c20 7364 5f64 6973 743d  a, n=n, sd_dist=
+0000c050: 7364 5f64 6973 742c 202a 2a6b 7761 7267  sd_dist, **kwarg
+0000c060: 7329 0a20 2020 2020 2020 2069 6620 6e6f  s).        if no
+0000c070: 7420 636f 6d70 7574 655f 636f 7272 3a0a  t compute_corr:.
+0000c080: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c090: 726e 2070 6163 6b65 645f 6368 6f6c 0a20  rn packed_chol. 
+0000c0a0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000c0b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c0c0: 636c 732e 6865 6c70 6572 5f64 6574 6572  cls.helper_deter
+0000c0d0: 6d69 6e69 7374 6963 7328 6e2c 2070 6163  ministics(n, pac
+0000c0e0: 6b65 645f 6368 6f6c 290a 0a20 2020 2040  ked_chol)..    @
+0000c0f0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+0000c100: 6465 6620 6865 6c70 6572 5f64 6574 6572  def helper_deter
+0000c110: 6d69 6e69 7374 6963 7328 636c 732c 206e  ministics(cls, n
+0000c120: 2c20 7061 636b 6564 5f63 686f 6c29 3a0a  , packed_chol):.
+0000c130: 2020 2020 2020 2020 6368 6f6c 203d 2070          chol = p
+0000c140: 6d2e 6578 7061 6e64 5f70 6163 6b65 645f  m.expand_packed_
+0000c150: 7472 6961 6e67 756c 6172 286e 2c20 7061  triangular(n, pa
+0000c160: 636b 6564 5f63 686f 6c2c 206c 6f77 6572  cked_chol, lower
+0000c170: 3d54 7275 6529 0a20 2020 2020 2020 2023  =True).        #
+0000c180: 2063 6f6d 7075 7465 2063 6f76 6172 6961   compute covaria
+0000c190: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
+0000c1a0: 2020 2063 6f76 203d 2070 742e 646f 7428     cov = pt.dot(
+0000c1b0: 6368 6f6c 2c20 6368 6f6c 2e54 290a 2020  chol, chol.T).  
+0000c1c0: 2020 2020 2020 2320 6578 7472 6163 7420        # extract 
+0000c1d0: 7374 616e 6461 7264 2064 6576 6961 7469  standard deviati
+0000c1e0: 6f6e 7320 616e 6420 7268 6f0a 2020 2020  ons and rho.    
+0000c1f0: 2020 2020 7374 6473 203d 2070 742e 7371      stds = pt.sq
+0000c200: 7274 2870 742e 6469 6167 2863 6f76 2929  rt(pt.diag(cov))
+0000c210: 0a20 2020 2020 2020 2069 6e76 5f73 7464  .        inv_std
+0000c220: 7320 3d20 3120 2f20 7374 6473 0a20 2020  s = 1 / stds.   
+0000c230: 2020 2020 2063 6f72 7220 3d20 696e 765f       corr = inv_
+0000c240: 7374 6473 5b4e 6f6e 652c 203a 5d20 2a20  stds[None, :] * 
+0000c250: 636f 7620 2a20 696e 765f 7374 6473 5b3a  cov * inv_stds[:
+0000c260: 2c20 4e6f 6e65 5d0a 2020 2020 2020 2020  , None].        
+0000c270: 7265 7475 726e 2063 686f 6c2c 2063 6f72  return chol, cor
+0000c280: 722c 2073 7464 730a 0a0a 636c 6173 7320  r, stds...class 
+0000c290: 4c4b 4a43 6f72 7252 5628 5261 6e64 6f6d  LKJCorrRV(Random
+0000c2a0: 5661 7269 6162 6c65 293a 0a20 2020 206e  Variable):.    n
+0000c2b0: 616d 6520 3d20 226c 6b6a 636f 7272 220a  ame = "lkjcorr".
+0000c2c0: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
+0000c2d0: 310a 2020 2020 6e64 696d 735f 7061 7261  1.    ndims_para
+0000c2e0: 6d73 203d 205b 302c 2030 5d0a 2020 2020  ms = [0, 0].    
+0000c2f0: 6474 7970 6520 3d20 2266 6c6f 6174 5822  dtype = "floatX"
+0000c300: 0a20 2020 205f 7072 696e 745f 6e61 6d65  .    _print_name
+0000c310: 203d 2028 224c 4b4a 436f 7272 5256 222c   = ("LKJCorrRV",
+0000c320: 2022 5c5c 6f70 6572 6174 6f72 6e61 6d65   "\\operatorname
+0000c330: 7b4c 4b4a 436f 7272 5256 7d22 290a 0a20  {LKJCorrRV}").. 
+0000c340: 2020 2064 6566 206d 616b 655f 6e6f 6465     def make_node
+0000c350: 2873 656c 662c 2072 6e67 2c20 7369 7a65  (self, rng, size
+0000c360: 2c20 6474 7970 652c 206e 2c20 6574 6129  , dtype, n, eta)
+0000c370: 3a0a 2020 2020 2020 2020 6e20 3d20 7074  :.        n = pt
+0000c380: 2e61 735f 7465 6e73 6f72 5f76 6172 6961  .as_tensor_varia
+0000c390: 626c 6528 6e29 0a20 2020 2020 2020 2069  ble(n).        i
+0000c3a0: 6620 6e6f 7420 6e2e 6e64 696d 203d 3d20  f not n.ndim == 
+0000c3b0: 303a 0a20 2020 2020 2020 2020 2020 2072  0:.            r
+0000c3c0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000c3d0: 226e 206d 7573 7420 6265 2061 2073 6361  "n must be a sca
+0000c3e0: 6c61 7220 286e 6469 6d3d 3029 2e22 290a  lar (ndim=0).").
+0000c3f0: 0a20 2020 2020 2020 2065 7461 203d 2070  .        eta = p
+0000c400: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+0000c410: 6162 6c65 2865 7461 290a 2020 2020 2020  able(eta).      
+0000c420: 2020 6966 206e 6f74 2065 7461 2e6e 6469    if not eta.ndi
+0000c430: 6d20 3d3d 2030 3a0a 2020 2020 2020 2020  m == 0:.        
+0000c440: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+0000c450: 7272 6f72 2822 6574 6120 6d75 7374 2062  rror("eta must b
+0000c460: 6520 6120 7363 616c 6172 2028 6e64 696d  e a scalar (ndim
+0000c470: 3d30 292e 2229 0a0a 2020 2020 2020 2020  =0).")..        
+0000c480: 7265 7475 726e 2073 7570 6572 2829 2e6d  return super().m
+0000c490: 616b 655f 6e6f 6465 2872 6e67 2c20 7369  ake_node(rng, si
+0000c4a0: 7a65 2c20 6474 7970 652c 206e 2c20 6574  ze, dtype, n, et
+0000c4b0: 6129 0a0a 2020 2020 6465 6620 5f73 7570  a)..    def _sup
+0000c4c0: 705f 7368 6170 655f 6672 6f6d 5f70 6172  p_shape_from_par
+0000c4d0: 616d 7328 7365 6c66 2c20 6469 7374 5f70  ams(self, dist_p
+0000c4e0: 6172 616d 732c 202a 2a6b 7761 7267 7329  arams, **kwargs)
+0000c4f0: 3a0a 2020 2020 2020 2020 6e20 3d20 6469  :.        n = di
+0000c500: 7374 5f70 6172 616d 735b 305d 0a20 2020  st_params[0].   
+0000c510: 2020 2020 2064 6973 745f 7368 6170 6520       dist_shape 
+0000c520: 3d20 2828 6e20 2a20 286e 202d 2031 2929  = ((n * (n - 1))
+0000c530: 202f 2f20 322c 290a 2020 2020 2020 2020   // 2,).        
+0000c540: 7265 7475 726e 2064 6973 745f 7368 6170  return dist_shap
+0000c550: 650a 0a20 2020 2040 636c 6173 736d 6574  e..    @classmet
+0000c560: 686f 640a 2020 2020 6465 6620 726e 675f  hod.    def rng_
+0000c570: 666e 2863 6c73 2c20 726e 672c 206e 2c20  fn(cls, rng, n, 
+0000c580: 6574 612c 2073 697a 6529 3a0a 2020 2020  eta, size):.    
+0000c590: 2020 2020 2320 5765 2066 6c61 7474 656e      # We flatten
+0000c5a0: 2074 6865 2073 697a 6520 746f 206d 616b   the size to mak
+0000c5b0: 6520 6f70 6572 6174 696f 6e73 2065 6173  e operations eas
+0000c5c0: 6965 722c 2061 6e64 2074 6865 6e20 7265  ier, and then re
+0000c5d0: 6275 696c 6420 6974 0a20 2020 2020 2020  build it.       
+0000c5e0: 2069 6620 7369 7a65 2069 7320 4e6f 6e65   if size is None
+0000c5f0: 3a0a 2020 2020 2020 2020 2020 2020 666c  :.            fl
+0000c600: 6174 5f73 697a 6520 3d20 310a 2020 2020  at_size = 1.    
+0000c610: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000c620: 2020 2020 2020 666c 6174 5f73 697a 6520        flat_size 
+0000c630: 3d20 6e70 2e70 726f 6428 7369 7a65 290a  = np.prod(size).
+0000c640: 0a20 2020 2020 2020 2043 203d 2063 6c73  .        C = cls
+0000c650: 2e5f 7261 6e64 6f6d 5f63 6f72 725f 6d61  ._random_corr_ma
+0000c660: 7472 6978 2872 6e67 3d72 6e67 2c20 6e3d  trix(rng=rng, n=
+0000c670: 6e2c 2065 7461 3d65 7461 2c20 666c 6174  n, eta=eta, flat
+0000c680: 5f73 697a 653d 666c 6174 5f73 697a 6529  _size=flat_size)
+0000c690: 0a0a 2020 2020 2020 2020 7472 6975 5f69  ..        triu_i
+0000c6a0: 6478 203d 206e 702e 7472 6975 5f69 6e64  dx = np.triu_ind
+0000c6b0: 6963 6573 286e 2c20 6b3d 3129 0a20 2020  ices(n, k=1).   
+0000c6c0: 2020 2020 2073 616d 706c 6573 203d 2043       samples = C
+0000c6d0: 5b2e 2e2e 2c20 7472 6975 5f69 6478 5b30  [..., triu_idx[0
+0000c6e0: 5d2c 2074 7269 755f 6964 785b 315d 5d0a  ], triu_idx[1]].
+0000c6f0: 0a20 2020 2020 2020 2069 6620 7369 7a65  .        if size
+0000c700: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+0000c710: 2020 2020 2020 7361 6d70 6c65 7320 3d20        samples = 
+0000c720: 7361 6d70 6c65 735b 305d 0a20 2020 2020  samples[0].     
+0000c730: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000c740: 2020 2020 2064 6973 745f 7368 6170 6520       dist_shape 
+0000c750: 3d20 286e 202a 2028 6e20 2d20 3129 2920  = (n * (n - 1)) 
+0000c760: 2f2f 2032 0a20 2020 2020 2020 2020 2020  // 2.           
+0000c770: 2073 616d 706c 6573 203d 206e 702e 7265   samples = np.re
+0000c780: 7368 6170 6528 7361 6d70 6c65 732c 2028  shape(samples, (
+0000c790: 2a73 697a 652c 2064 6973 745f 7368 6170  *size, dist_shap
+0000c7a0: 6529 290a 2020 2020 2020 2020 7265 7475  e)).        retu
+0000c7b0: 726e 2073 616d 706c 6573 0a0a 2020 2020  rn samples..    
+0000c7c0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+0000c7d0: 2064 6566 205f 7261 6e64 6f6d 5f63 6f72   def _random_cor
+0000c7e0: 725f 6d61 7472 6978 2863 6c73 2c20 726e  r_matrix(cls, rn
+0000c7f0: 672c 206e 2c20 6574 612c 2066 6c61 745f  g, n, eta, flat_
+0000c800: 7369 7a65 293a 0a20 2020 2020 2020 2023  size):.        #
+0000c810: 206f 7269 6769 6e61 6c20 696d 706c 656d   original implem
+0000c820: 656e 7461 7469 6f6e 2069 6e20 5220 7365  entation in R se
+0000c830: 653a 0a20 2020 2020 2020 2023 2068 7474  e:.        # htt
+0000c840: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+0000c850: 726d 6365 6c72 6561 7468 2f72 6574 6869  rmcelreath/rethi
+0000c860: 6e6b 696e 672f 626c 6f62 2f6d 6173 7465  nking/blob/maste
+0000c870: 722f 522f 6469 7374 7269 6275 7469 6f6e  r/R/distribution
+0000c880: 732e 720a 2020 2020 2020 2020 6265 7461  s.r.        beta
+0000c890: 203d 2065 7461 202d 2031 2e30 202b 206e   = eta - 1.0 + n
+0000c8a0: 202f 2032 2e30 0a20 2020 2020 2020 2072   / 2.0.        r
+0000c8b0: 3132 203d 2032 2e30 202a 2073 7461 7473  12 = 2.0 * stats
+0000c8c0: 2e62 6574 612e 7276 7328 613d 6265 7461  .beta.rvs(a=beta
+0000c8d0: 2c20 623d 6265 7461 2c20 7369 7a65 3d66  , b=beta, size=f
+0000c8e0: 6c61 745f 7369 7a65 2c20 7261 6e64 6f6d  lat_size, random
+0000c8f0: 5f73 7461 7465 3d72 6e67 2920 2d20 312e  _state=rng) - 1.
+0000c900: 300a 2020 2020 2020 2020 5020 3d20 6e70  0.        P = np
+0000c910: 2e66 756c 6c28 2866 6c61 745f 7369 7a65  .full((flat_size
+0000c920: 2c20 6e2c 206e 292c 206e 702e 6579 6528  , n, n), np.eye(
+0000c930: 6e29 290a 2020 2020 2020 2020 505b 2e2e  n)).        P[..
+0000c940: 2e2c 2030 2c20 315d 203d 2072 3132 0a20  ., 0, 1] = r12. 
+0000c950: 2020 2020 2020 2050 5b2e 2e2e 2c20 312c         P[..., 1,
+0000c960: 2031 5d20 3d20 6e70 2e73 7172 7428 312e   1] = np.sqrt(1.
+0000c970: 3020 2d20 7231 322a 2a32 290a 2020 2020  0 - r12**2).    
+0000c980: 2020 2020 666f 7220 6d70 3120 696e 2072      for mp1 in r
+0000c990: 616e 6765 2832 2c20 6e29 3a0a 2020 2020  ange(2, n):.    
+0000c9a0: 2020 2020 2020 2020 6265 7461 202d 3d20          beta -= 
+0000c9b0: 302e 350a 2020 2020 2020 2020 2020 2020  0.5.            
+0000c9c0: 7920 3d20 7374 6174 732e 6265 7461 2e72  y = stats.beta.r
+0000c9d0: 7673 2861 3d6d 7031 202f 2032 2e30 2c20  vs(a=mp1 / 2.0, 
+0000c9e0: 623d 6265 7461 2c20 7369 7a65 3d66 6c61  b=beta, size=fla
+0000c9f0: 745f 7369 7a65 2c20 7261 6e64 6f6d 5f73  t_size, random_s
+0000ca00: 7461 7465 3d72 6e67 290a 2020 2020 2020  tate=rng).      
+0000ca10: 2020 2020 2020 7a20 3d20 7374 6174 732e        z = stats.
+0000ca20: 6e6f 726d 2e72 7673 286c 6f63 3d30 2c20  norm.rvs(loc=0, 
+0000ca30: 7363 616c 653d 312c 2073 697a 653d 2866  scale=1, size=(f
+0000ca40: 6c61 745f 7369 7a65 2c20 6d70 3129 2c20  lat_size, mp1), 
+0000ca50: 7261 6e64 6f6d 5f73 7461 7465 3d72 6e67  random_state=rng
+0000ca60: 290a 2020 2020 2020 2020 2020 2020 7a20  ).            z 
+0000ca70: 3d20 7a20 2f20 6e70 2e73 7172 7428 6e70  = z / np.sqrt(np
+0000ca80: 2e65 696e 7375 6d28 2269 6a2c 696a 2d3e  .einsum("ij,ij->
+0000ca90: 6922 2c20 7a2c 207a 2929 5b2e 2e2e 2c20  i", z, z))[..., 
+0000caa0: 6e70 2e6e 6577 6178 6973 5d0a 2020 2020  np.newaxis].    
+0000cab0: 2020 2020 2020 2020 505b 2e2e 2e2c 2030          P[..., 0
+0000cac0: 3a6d 7031 2c20 6d70 315d 203d 206e 702e  :mp1, mp1] = np.
+0000cad0: 7371 7274 2879 5b2e 2e2e 2c20 6e70 2e6e  sqrt(y[..., np.n
+0000cae0: 6577 6178 6973 5d29 202a 207a 0a20 2020  ewaxis]) * z.   
+0000caf0: 2020 2020 2020 2020 2050 5b2e 2e2e 2c20           P[..., 
+0000cb00: 6d70 312c 206d 7031 5d20 3d20 6e70 2e73  mp1, mp1] = np.s
+0000cb10: 7172 7428 312e 3020 2d20 7929 0a20 2020  qrt(1.0 - y).   
+0000cb20: 2020 2020 2043 203d 206e 702e 6569 6e73       C = np.eins
+0000cb30: 756d 2822 2e2e 2e6a 692c 2e2e 2e6a 6b2d  um("...ji,...jk-
+0000cb40: 3e2e 2e2e 696b 222c 2050 2c20 5029 0a20  >...ik", P, P). 
+0000cb50: 2020 2020 2020 2072 6574 7572 6e20 430a         return C.
+0000cb60: 0a0a 6c6b 6a63 6f72 7220 3d20 4c4b 4a43  ..lkjcorr = LKJC
+0000cb70: 6f72 7252 5628 290a 0a0a 636c 6173 7320  orrRV()...class 
+0000cb80: 4c4b 4a43 6f72 7228 426f 756e 6465 6443  LKJCorr(BoundedC
+0000cb90: 6f6e 7469 6e75 6f75 7329 3a0a 2020 2020  ontinuous):.    
+0000cba0: 7222 2222 0a20 2020 2054 6865 204c 4b4a  r""".    The LKJ
+0000cbb0: 2028 4c65 7761 6e64 6f77 736b 692c 204b   (Lewandowski, K
+0000cbc0: 7572 6f77 6963 6b61 2061 6e64 204a 6f65  urowicka and Joe
+0000cbd0: 2920 6c6f 672d 6c69 6b65 6c69 686f 6f64  ) log-likelihood
+0000cbe0: 2e0a 0a20 2020 2054 6865 204c 4b4a 2064  ...    The LKJ d
+0000cbf0: 6973 7472 6962 7574 696f 6e20 6973 2061  istribution is a
+0000cc00: 2070 7269 6f72 2064 6973 7472 6962 7574   prior distribut
+0000cc10: 696f 6e20 666f 7220 636f 7272 656c 6174  ion for correlat
+0000cc20: 696f 6e20 6d61 7472 6963 6573 2e0a 2020  ion matrices..  
+0000cc30: 2020 4966 2065 7461 203d 2031 2074 6869    If eta = 1 thi
+0000cc40: 7320 636f 7272 6573 706f 6e64 7320 746f  s corresponds to
+0000cc50: 2074 6865 2075 6e69 666f 726d 2064 6973   the uniform dis
+0000cc60: 7472 6962 7574 696f 6e20 6f76 6572 2063  tribution over c
+0000cc70: 6f72 7265 6c61 7469 6f6e 0a20 2020 206d  orrelation.    m
+0000cc80: 6174 7269 6365 732e 2046 6f72 2065 7461  atrices. For eta
+0000cc90: 202d 3e20 6f6f 2074 6865 204c 4b4a 2070   -> oo the LKJ p
+0000cca0: 7269 6f72 2061 7070 726f 6163 6865 7320  rior approaches 
+0000ccb0: 7468 6520 6964 656e 7469 7479 206d 6174  the identity mat
+0000ccc0: 7269 782e 0a0a 2020 2020 3d3d 3d3d 3d3d  rix...    ======
+0000ccd0: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+0000cce0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000ccf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cd00: 3d3d 0a20 2020 2053 7570 706f 7274 2020  ==.    Support  
+0000cd10: 2055 7070 6572 2074 7269 616e 6775 6c61   Upper triangula
+0000cd20: 7220 6d61 7472 6978 2077 6974 6820 7661  r matrix with va
+0000cd30: 6c75 6573 2069 6e20 5b2d 312c 2031 5d0a  lues in [-1, 1].
+0000cd40: 2020 2020 3d3d 3d3d 3d3d 3d3d 2020 3d3d      ========  ==
+0000cd50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cd60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000cd70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2020  ============..  
+0000cd80: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+0000cd90: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+0000cda0: 6e20 3a20 7465 6e73 6f72 5f6c 696b 6520  n : tensor_like 
+0000cdb0: 6f66 2069 6e74 0a20 2020 2020 2020 2044  of int.        D
+0000cdc0: 696d 656e 7369 6f6e 206f 6620 7468 6520  imension of the 
+0000cdd0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000cde0: 7820 286e 203e 2031 292e 0a20 2020 2065  x (n > 1)..    e
+0000cdf0: 7461 203a 2074 656e 736f 725f 6c69 6b65  ta : tensor_like
+0000ce00: 206f 6620 666c 6f61 740a 2020 2020 2020   of float.      
+0000ce10: 2020 5468 6520 7368 6170 6520 7061 7261    The shape para
+0000ce20: 6d65 7465 7220 2865 7461 203e 2030 2920  meter (eta > 0) 
+0000ce30: 6f66 2074 6865 204c 4b4a 2064 6973 7472  of the LKJ distr
+0000ce40: 6962 7574 696f 6e2e 2065 7461 203d 2031  ibution. eta = 1
+0000ce50: 0a20 2020 2020 2020 2069 6d70 6c69 6573  .        implies
+0000ce60: 2061 2075 6e69 666f 726d 2064 6973 7472   a uniform distr
+0000ce70: 6962 7574 696f 6e20 6f66 2074 6865 2063  ibution of the c
+0000ce80: 6f72 7265 6c61 7469 6f6e 206d 6174 7269  orrelation matri
+0000ce90: 6365 733b 0a20 2020 2020 2020 206c 6172  ces;.        lar
+0000cea0: 6765 7220 7661 6c75 6573 2070 7574 206d  ger values put m
+0000ceb0: 6f72 6520 7765 6967 6874 206f 6e20 6d61  ore weight on ma
+0000cec0: 7472 6963 6573 2077 6974 6820 6665 7720  trices with few 
+0000ced0: 636f 7272 656c 6174 696f 6e73 2e0a 0a20  correlations... 
+0000cee0: 2020 204e 6f74 6573 0a20 2020 202d 2d2d     Notes.    ---
+0000cef0: 2d2d 0a20 2020 2054 6869 7320 696d 706c  --.    This impl
+0000cf00: 656d 656e 7461 7469 6f6e 206f 6e6c 7920  ementation only 
+0000cf10: 7265 7475 726e 7320 7468 6520 7661 6c75  returns the valu
+0000cf20: 6573 206f 6620 7468 6520 7570 7065 7220  es of the upper 
+0000cf30: 7472 6961 6e67 756c 6172 0a20 2020 206d  triangular.    m
+0000cf40: 6174 7269 7820 6578 636c 7564 696e 6720  atrix excluding 
+0000cf50: 7468 6520 6469 6167 6f6e 616c 2e20 4865  the diagonal. He
+0000cf60: 7265 2069 7320 6120 7363 6865 6d61 7469  re is a schemati
+0000cf70: 6320 666f 7220 6e20 3d20 352c 2073 686f  c for n = 5, sho
+0000cf80: 7769 6e67 0a20 2020 2074 6865 2069 6e64  wing.    the ind
+0000cf90: 6578 6573 206f 6620 7468 6520 656c 656d  exes of the elem
+0000cfa0: 656e 7473 3a3a 0a0a 2020 2020 2020 2020  ents::..        
+0000cfb0: 5b5b 2d20 3020 3120 3220 335d 0a20 2020  [[- 0 1 2 3].   
+0000cfc0: 2020 2020 2020 5b2d 202d 2034 2035 2036        [- - 4 5 6
+0000cfd0: 5d0a 2020 2020 2020 2020 205b 2d20 2d20  ].         [- - 
+0000cfe0: 2d20 3720 385d 0a20 2020 2020 2020 2020  - 7 8].         
+0000cff0: 5b2d 202d 202d 202d 2039 5d0a 2020 2020  [- - - - 9].    
+0000d000: 2020 2020 205b 2d20 2d20 2d20 2d20 2d5d       [- - - - -]
+0000d010: 5d0a 0a0a 2020 2020 5265 6665 7265 6e63  ]...    Referenc
+0000d020: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  es.    ---------
+0000d030: 2d0a 2020 2020 2e2e 205b 4c4b 4a32 3030  -.    .. [LKJ200
+0000d040: 395d 204c 6577 616e 646f 7773 6b69 2c20  9] Lewandowski, 
+0000d050: 442e 2c20 4b75 726f 7769 636b 612c 2044  D., Kurowicka, D
+0000d060: 2e20 616e 6420 4a6f 652c 2048 2e20 2832  . and Joe, H. (2
+0000d070: 3030 3929 2e0a 2020 2020 2020 2020 2247  009)..        "G
+0000d080: 656e 6572 6174 696e 6720 7261 6e64 6f6d  enerating random
+0000d090: 2063 6f72 7265 6c61 7469 6f6e 206d 6174   correlation mat
+0000d0a0: 7269 6365 7320 6261 7365 6420 6f6e 2076  rices based on v
+0000d0b0: 696e 6573 2061 6e64 0a20 2020 2020 2020  ines and.       
+0000d0c0: 2065 7874 656e 6465 6420 6f6e 696f 6e20   extended onion 
+0000d0d0: 6d65 7468 6f64 2e22 204a 6f75 726e 616c  method." Journal
+0000d0e0: 206f 6620 6d75 6c74 6976 6172 6961 7465   of multivariate
+0000d0f0: 2061 6e61 6c79 7369 732c 0a20 2020 2020   analysis,.     
+0000d100: 2020 2031 3030 2839 292c 2070 702e 3139     100(9), pp.19
+0000d110: 3839 2d32 3030 312e 0a20 2020 2022 2222  89-2001..    """
+0000d120: 0a0a 2020 2020 7276 5f6f 7020 3d20 6c6b  ..    rv_op = lk
+0000d130: 6a63 6f72 720a 0a20 2020 2040 636c 6173  jcorr..    @clas
+0000d140: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+0000d150: 6469 7374 2863 6c73 2c20 6e2c 2065 7461  dist(cls, n, eta
+0000d160: 2c20 2a2a 6b77 6172 6773 293a 0a20 2020  , **kwargs):.   
+0000d170: 2020 2020 206e 203d 2070 742e 6173 5f74       n = pt.as_t
+0000d180: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
+0000d190: 6e74 5828 6e29 290a 2020 2020 2020 2020  ntX(n)).        
+0000d1a0: 6574 6120 3d20 7074 2e61 735f 7465 6e73  eta = pt.as_tens
+0000d1b0: 6f72 5f76 6172 6961 626c 6528 666c 6f61  or_variable(floa
+0000d1c0: 7458 2865 7461 2929 0a20 2020 2020 2020  tX(eta)).       
+0000d1d0: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+0000d1e0: 6469 7374 285b 6e2c 2065 7461 5d2c 202a  dist([n, eta], *
+0000d1f0: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+0000d200: 6620 6d6f 6d65 6e74 2872 762c 202a 6172  f moment(rv, *ar
+0000d210: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
+0000d220: 7572 6e20 7074 2e7a 6572 6f73 5f6c 696b  urn pt.zeros_lik
+0000d230: 6528 7276 290a 0a20 2020 2064 6566 206c  e(rv)..    def l
+0000d240: 6f67 7028 7661 6c75 652c 206e 2c20 6574  ogp(value, n, et
+0000d250: 6129 3a0a 2020 2020 2020 2020 2222 220a  a):.        """.
+0000d260: 2020 2020 2020 2020 4361 6c63 756c 6174          Calculat
+0000d270: 6520 6c6f 672d 7072 6f62 6162 696c 6974  e log-probabilit
+0000d280: 7920 6f66 204c 4b4a 2064 6973 7472 6962  y of LKJ distrib
+0000d290: 7574 696f 6e20 6174 2073 7065 6369 6669  ution at specifi
+0000d2a0: 6564 0a20 2020 2020 2020 2076 616c 7565  ed.        value
+0000d2b0: 2e0a 0a20 2020 2020 2020 2050 6172 616d  ...        Param
+0000d2c0: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
+0000d2d0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+0000d2e0: 2076 616c 7565 3a20 6e75 6d65 7269 630a   value: numeric.
+0000d2f0: 2020 2020 2020 2020 2020 2020 5661 6c75              Valu
+0000d300: 6520 666f 7220 7768 6963 6820 6c6f 672d  e for which log-
+0000d310: 7072 6f62 6162 696c 6974 7920 6973 2063  probability is c
+0000d320: 616c 6375 6c61 7465 642e 0a0a 2020 2020  alculated...    
+0000d330: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+0000d340: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+0000d350: 2020 2020 5465 6e73 6f72 5661 7269 6162      TensorVariab
+0000d360: 6c65 0a20 2020 2020 2020 2022 2222 0a0a  le.        """..
+0000d370: 2020 2020 2020 2020 2320 544f 444f 3a20          # TODO: 
+0000d380: 5079 5465 6e73 6f72 2064 6f65 7320 6e6f  PyTensor does no
+0000d390: 7420 6861 7665 2061 2060 7472 6975 5f69  t have a `triu_i
+0000d3a0: 6e64 6963 6573 602c 2073 6f20 7765 2063  ndices`, so we c
+0000d3b0: 616e 206f 6e6c 7920 776f 726b 2077 6974  an only work wit
+0000d3c0: 6820 636f 6e73 7461 6e74 0a20 2020 2020  h constant.     
+0000d3d0: 2020 2023 2020 6e20 286f 7220 656c 7365     #  n (or else
+0000d3e0: 2066 696e 6420 6120 6469 6666 6572 656e   find a differen
+0000d3f0: 7420 6578 7072 6573 7369 6f6e 290a 2020  t expression).  
+0000d400: 2020 2020 2020 6966 206e 6f74 2069 7369        if not isi
+0000d410: 6e73 7461 6e63 6528 6e2c 2043 6f6e 7374  nstance(n, Const
+0000d420: 616e 7429 3a0a 2020 2020 2020 2020 2020  ant):.          
+0000d430: 2020 7261 6973 6520 4e6f 7449 6d70 6c65    raise NotImple
+0000d440: 6d65 6e74 6564 4572 726f 7228 226c 6f67  mentedError("log
+0000d450: 7020 6f6e 6c79 2069 6d70 6c65 6d65 6e74  p only implement
+0000d460: 6564 2066 6f72 2063 6f6e 7374 616e 7420  ed for constant 
+0000d470: 606e 6022 290a 0a20 2020 2020 2020 206e  `n`")..        n
+0000d480: 203d 2069 6e74 286e 2e64 6174 6129 0a20   = int(n.data). 
+0000d490: 2020 2020 2020 2073 6861 7065 203d 206e         shape = n
+0000d4a0: 202a 2028 6e20 2d20 3129 202f 2f20 320a   * (n - 1) // 2.
+0000d4b0: 2020 2020 2020 2020 7472 695f 696e 6465          tri_inde
+0000d4c0: 7820 3d20 6e70 2e7a 6572 6f73 2828 6e2c  x = np.zeros((n,
+0000d4d0: 206e 292c 2064 7479 7065 3d22 696e 7433   n), dtype="int3
+0000d4e0: 3222 290a 2020 2020 2020 2020 7472 695f  2").        tri_
+0000d4f0: 696e 6465 785b 6e70 2e74 7269 755f 696e  index[np.triu_in
+0000d500: 6469 6365 7328 6e2c 206b 3d31 295d 203d  dices(n, k=1)] =
+0000d510: 206e 702e 6172 616e 6765 2873 6861 7065   np.arange(shape
+0000d520: 290a 2020 2020 2020 2020 7472 695f 696e  ).        tri_in
+0000d530: 6465 785b 6e70 2e74 7269 755f 696e 6469  dex[np.triu_indi
+0000d540: 6365 7328 6e2c 206b 3d31 295b 3a3a 2d31  ces(n, k=1)[::-1
+0000d550: 5d5d 203d 206e 702e 6172 616e 6765 2873  ]] = np.arange(s
+0000d560: 6861 7065 290a 0a20 2020 2020 2020 2076  hape)..        v
+0000d570: 616c 7565 203d 2070 742e 7461 6b65 2876  alue = pt.take(v
+0000d580: 616c 7565 2c20 7472 695f 696e 6465 7829  alue, tri_index)
+0000d590: 0a20 2020 2020 2020 2076 616c 7565 203d  .        value =
+0000d5a0: 2070 742e 6669 6c6c 5f64 6961 676f 6e61   pt.fill_diagona
+0000d5b0: 6c28 7661 6c75 652c 2031 290a 0a20 2020  l(value, 1)..   
+0000d5c0: 2020 2020 2023 2054 4f44 4f3a 205f 6c6b       # TODO: _lk
+0000d5d0: 6a5f 6e6f 726d 616c 697a 696e 675f 636f  j_normalizing_co
+0000d5e0: 6e73 7461 6e74 2063 7572 7265 6e74 6c79  nstant currently
+0000d5f0: 2072 6571 7569 7265 7320 6065 7461 6020   requires `eta` 
+0000d600: 616e 6420 606e 6020 746f 2062 6520 636f  and `n` to be co
+0000d610: 6e73 7461 6e74 730a 2020 2020 2020 2020  nstants.        
+0000d620: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+0000d630: 6528 6574 612c 2043 6f6e 7374 616e 7429  e(eta, Constant)
+0000d640: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000d650: 6973 6520 4e6f 7449 6d70 6c65 6d65 6e74  ise NotImplement
+0000d660: 6564 4572 726f 7228 226c 6f67 7020 6f6e  edError("logp on
+0000d670: 6c79 2069 6d70 6c65 6d65 6e74 6564 2066  ly implemented f
+0000d680: 6f72 2063 6f6e 7374 616e 7420 6065 7461  or constant `eta
+0000d690: 6022 290a 2020 2020 2020 2020 6574 6120  `").        eta 
+0000d6a0: 3d20 666c 6f61 7428 6574 612e 6461 7461  = float(eta.data
+0000d6b0: 290a 2020 2020 2020 2020 7265 7375 6c74  ).        result
+0000d6c0: 203d 205f 6c6b 6a5f 6e6f 726d 616c 697a   = _lkj_normaliz
+0000d6d0: 696e 675f 636f 6e73 7461 6e74 2865 7461  ing_constant(eta
+0000d6e0: 2c20 6e29 0a20 2020 2020 2020 2072 6573  , n).        res
+0000d6f0: 756c 7420 2b3d 2028 6574 6120 2d20 312e  ult += (eta - 1.
+0000d700: 3029 202a 2070 742e 6c6f 6728 6465 7428  0) * pt.log(det(
+0000d710: 7661 6c75 6529 290a 2020 2020 2020 2020  value)).        
+0000d720: 7265 7475 726e 2063 6865 636b 5f70 6172  return check_par
+0000d730: 616d 6574 6572 7328 0a20 2020 2020 2020  ameters(.       
+0000d740: 2020 2020 2072 6573 756c 742c 0a20 2020       result,.   
+0000d750: 2020 2020 2020 2020 2076 616c 7565 203e           value >
+0000d760: 3d20 2d31 2c0a 2020 2020 2020 2020 2020  = -1,.          
+0000d770: 2020 7661 6c75 6520 3c3d 2031 2c0a 2020    value <= 1,.  
+0000d780: 2020 2020 2020 2020 2020 6d61 7472 6978            matrix
+0000d790: 5f70 6f73 5f64 6566 2876 616c 7565 292c  _pos_def(value),
+0000d7a0: 0a20 2020 2020 2020 2020 2020 2065 7461  .            eta
+0000d7b0: 203e 2030 2c0a 2020 2020 2020 2020 290a   > 0,.        ).
+0000d7c0: 0a0a 405f 6465 6661 756c 745f 7472 616e  ..@_default_tran
+0000d7d0: 7366 6f72 6d2e 7265 6769 7374 6572 284c  sform.register(L
+0000d7e0: 4b4a 436f 7272 290a 6465 6620 6c6b 6a63  KJCorr).def lkjc
+0000d7f0: 6f72 725f 6465 6661 756c 745f 7472 616e  orr_default_tran
+0000d800: 7366 6f72 6d28 6f70 2c20 7276 293a 0a20  sform(op, rv):. 
+0000d810: 2020 2072 6574 7572 6e20 496e 7465 7276     return Interv
+0000d820: 616c 2866 6c6f 6174 5828 2d31 2e30 292c  al(floatX(-1.0),
+0000d830: 2066 6c6f 6174 5828 312e 3029 290a 0a0a   floatX(1.0))...
+0000d840: 636c 6173 7320 4d61 7472 6978 4e6f 726d  class MatrixNorm
+0000d850: 616c 5256 2852 616e 646f 6d56 6172 6961  alRV(RandomVaria
+0000d860: 626c 6529 3a0a 2020 2020 6e61 6d65 203d  ble):.    name =
+0000d870: 2022 6d61 7472 6978 6e6f 726d 616c 220a   "matrixnormal".
+0000d880: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
+0000d890: 320a 2020 2020 6e64 696d 735f 7061 7261  2.    ndims_para
+0000d8a0: 6d73 203d 205b 322c 2032 2c20 325d 0a20  ms = [2, 2, 2]. 
+0000d8b0: 2020 2064 7479 7065 203d 2022 666c 6f61     dtype = "floa
+0000d8c0: 7458 220a 2020 2020 5f70 7269 6e74 5f6e  tX".    _print_n
+0000d8d0: 616d 6520 3d20 2822 4d61 7472 6978 4e6f  ame = ("MatrixNo
+0000d8e0: 726d 616c 222c 2022 5c5c 6f70 6572 6174  rmal", "\\operat
+0000d8f0: 6f72 6e61 6d65 7b4d 6174 7269 784e 6f72  orname{MatrixNor
+0000d900: 6d61 6c7d 2229 0a0a 2020 2020 6465 6620  mal}")..    def 
+0000d910: 5f69 6e66 6572 5f73 6861 7065 2873 656c  _infer_shape(sel
+0000d920: 662c 2073 697a 652c 2064 6973 745f 7061  f, size, dist_pa
+0000d930: 7261 6d73 2c20 7061 7261 6d5f 7368 6170  rams, param_shap
+0000d940: 6573 3d4e 6f6e 6529 3a0a 2020 2020 2020  es=None):.      
+0000d950: 2020 7368 6170 6520 3d20 7475 706c 6528    shape = tuple(
+0000d960: 7369 7a65 2920 2b20 7475 706c 6528 6469  size) + tuple(di
+0000d970: 7374 5f70 6172 616d 735b 305d 2e73 6861  st_params[0].sha
+0000d980: 7065 5b2d 323a 5d29 0a20 2020 2020 2020  pe[-2:]).       
+0000d990: 2072 6574 7572 6e20 7368 6170 650a 0a20   return shape.. 
+0000d9a0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+0000d9b0: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
+0000d9c0: 6c73 2c20 726e 672c 206d 752c 2072 6f77  ls, rng, mu, row
+0000d9d0: 6368 6f6c 2c20 636f 6c63 686f 6c2c 2073  chol, colchol, s
+0000d9e0: 697a 653d 4e6f 6e65 293a 0a20 2020 2020  ize=None):.     
+0000d9f0: 2020 2073 697a 6520 3d20 746f 5f74 7570     size = to_tup
+0000da00: 6c65 2873 697a 6529 0a20 2020 2020 2020  le(size).       
+0000da10: 2064 6973 745f 7368 6170 6520 3d20 746f   dist_shape = to
+0000da20: 5f74 7570 6c65 285b 726f 7763 686f 6c2e  _tuple([rowchol.
+0000da30: 7368 6170 655b 305d 2c20 636f 6c63 686f  shape[0], colcho
+0000da40: 6c2e 7368 6170 655b 305d 5d29 0a20 2020  l.shape[0]]).   
+0000da50: 2020 2020 206f 7574 7075 745f 7368 6170       output_shap
+0000da60: 6520 3d20 7369 7a65 202b 2064 6973 745f  e = size + dist_
+0000da70: 7368 6170 650a 0a20 2020 2020 2020 2023  shape..        #
+0000da80: 2042 726f 6164 6361 7374 696e 6720 616c   Broadcasting al
+0000da90: 6c20 7061 7261 6d65 7465 7273 0a20 2020  l parameters.   
+0000daa0: 2020 2020 2073 6861 7065 7320 3d20 5b6d       shapes = [m
+0000dab0: 752e 7368 6170 652c 206f 7574 7075 745f  u.shape, output_
+0000dac0: 7368 6170 655d 0a20 2020 2020 2020 2062  shape].        b
+0000dad0: 726f 6164 6361 7374 6162 6c65 5f73 6861  roadcastable_sha
+0000dae0: 7065 203d 2062 726f 6164 6361 7374 5f64  pe = broadcast_d
+0000daf0: 6973 745f 7361 6d70 6c65 735f 7368 6170  ist_samples_shap
+0000db00: 6528 7368 6170 6573 2c20 7369 7a65 3d73  e(shapes, size=s
+0000db10: 697a 6529 0a20 2020 2020 2020 206d 7520  ize).        mu 
+0000db20: 3d20 6e70 2e62 726f 6164 6361 7374 5f74  = np.broadcast_t
+0000db30: 6f28 6d75 2c20 7368 6170 653d 6272 6f61  o(mu, shape=broa
+0000db40: 6463 6173 7461 626c 655f 7368 6170 6529  dcastable_shape)
+0000db50: 0a20 2020 2020 2020 2072 6f77 6368 6f6c  .        rowchol
+0000db60: 203d 206e 702e 6272 6f61 6463 6173 745f   = np.broadcast_
+0000db70: 746f 2872 6f77 6368 6f6c 2c20 7368 6170  to(rowchol, shap
+0000db80: 653d 7369 7a65 202b 2072 6f77 6368 6f6c  e=size + rowchol
+0000db90: 2e73 6861 7065 5b2d 323a 5d29 0a0a 2020  .shape[-2:])..  
+0000dba0: 2020 2020 2020 636f 6c63 686f 6c20 3d20        colchol = 
+0000dbb0: 6e70 2e62 726f 6164 6361 7374 5f74 6f28  np.broadcast_to(
+0000dbc0: 636f 6c63 686f 6c2c 2073 6861 7065 3d73  colchol, shape=s
+0000dbd0: 697a 6520 2b20 636f 6c63 686f 6c2e 7368  ize + colchol.sh
+0000dbe0: 6170 655b 2d32 3a5d 290a 2020 2020 2020  ape[-2:]).      
+0000dbf0: 2020 636f 6c63 686f 6c20 3d20 6e70 2e73    colchol = np.s
+0000dc00: 7761 7061 7865 7328 636f 6c63 686f 6c2c  wapaxes(colchol,
+0000dc10: 202d 312c 202d 3229 2020 2320 5461 6b65   -1, -2)  # Take
+0000dc20: 2074 7261 6e73 706f 7365 0a0a 2020 2020   transpose..    
+0000dc30: 2020 2020 7374 616e 6461 7264 5f6e 6f72      standard_nor
+0000dc40: 6d61 6c20 3d20 726e 672e 7374 616e 6461  mal = rng.standa
+0000dc50: 7264 5f6e 6f72 6d61 6c28 6f75 7470 7574  rd_normal(output
+0000dc60: 5f73 6861 7065 290a 2020 2020 2020 2020  _shape).        
+0000dc70: 7361 6d70 6c65 7320 3d20 6d75 202b 206e  samples = mu + n
+0000dc80: 702e 6d61 746d 756c 2872 6f77 6368 6f6c  p.matmul(rowchol
+0000dc90: 2c20 6e70 2e6d 6174 6d75 6c28 7374 616e  , np.matmul(stan
+0000dca0: 6461 7264 5f6e 6f72 6d61 6c2c 2063 6f6c  dard_normal, col
+0000dcb0: 6368 6f6c 2929 0a0a 2020 2020 2020 2020  chol))..        
+0000dcc0: 7265 7475 726e 2073 616d 706c 6573 0a0a  return samples..
+0000dcd0: 0a6d 6174 7269 786e 6f72 6d61 6c20 3d20  .matrixnormal = 
+0000dce0: 4d61 7472 6978 4e6f 726d 616c 5256 2829  MatrixNormalRV()
+0000dcf0: 0a0a 0a63 6c61 7373 204d 6174 7269 784e  ...class MatrixN
+0000dd00: 6f72 6d61 6c28 436f 6e74 696e 756f 7573  ormal(Continuous
+0000dd10: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
+0000dd20: 4d61 7472 6978 2d76 616c 7565 6420 6e6f  Matrix-valued no
+0000dd30: 726d 616c 206c 6f67 2d6c 696b 656c 6968  rmal log-likelih
+0000dd40: 6f6f 642e 0a0a 2020 2020 2e2e 206d 6174  ood...    .. mat
+0000dd50: 683a 3a0a 2020 2020 2020 2066 2878 205c  h::.       f(x \
+0000dd60: 6d69 6420 5c6d 752c 2055 2c20 5629 203d  mid \mu, U, V) =
+0000dd70: 0a20 2020 2020 2020 2020 2020 5c66 7261  .           \fra
+0000dd80: 637b 317d 7b28 325c 7069 5e7b 6d20 6e7d  c{1}{(2\pi^{m n}
+0000dd90: 207c 557c 5e6e 207c 567c 5e6d 295e 7b31   |U|^n |V|^m)^{1
+0000dda0: 2f32 7d7d 0a20 2020 2020 2020 2020 2020  /2}}.           
+0000ddb0: 5c65 7870 5c6c 6566 745c 7b0a 2020 2020  \exp\left\{.    
+0000ddc0: 2020 2020 2020 2020 2020 2020 2d5c 6672              -\fr
+0000ddd0: 6163 7b31 7d7b 327d 205c 6d61 7468 726d  ac{1}{2} \mathrm
+0000dde0: 7b54 727d 5b20 565e 7b2d 317d 2028 782d  {Tr}[ V^{-1} (x-
+0000ddf0: 5c6d 7529 5e7b 5c70 7269 6d65 7d20 555e  \mu)^{\prime} U^
+0000de00: 7b2d 317d 2028 782d 5c6d 7529 5d0a 2020  {-1} (x-\mu)].  
+0000de10: 2020 2020 2020 2020 2020 5c72 6967 6874            \right
+0000de20: 5c7d 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  \}..    ========
+0000de30: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
+0000de40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000de50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20  ==============. 
+0000de60: 2020 2053 7570 706f 7274 2020 2020 2020     Support      
+0000de70: 2020 2020 3a6d 6174 683a 6078 205c 696e      :math:`x \in
+0000de80: 205c 6d61 7468 6262 7b52 7d5e 7b6d 205c   \mathbb{R}^{m \
+0000de90: 7469 6d65 7320 6e7d 600a 2020 2020 4d65  times n}`.    Me
+0000dea0: 616e 2020 2020 2020 2020 2020 2020 203a  an             :
+0000deb0: 6d61 7468 3a60 5c6d 7560 0a20 2020 2052  math:`\mu`.    R
+0000dec0: 6f77 2056 6172 6961 6e63 6520 2020 2020  ow Variance     
+0000ded0: 3a6d 6174 683a 6055 600a 2020 2020 436f  :math:`U`.    Co
+0000dee0: 6c75 6d6e 2056 6172 6961 6e63 6520 203a  lumn Variance  :
+0000def0: 6d61 7468 3a60 5660 0a20 2020 203d 3d3d  math:`V`.    ===
+0000df00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d  ============  ==
+0000df10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000df20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000df30: 3d3d 3d0a 0a20 2020 2050 6172 616d 6574  ===..    Paramet
+0000df40: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
+0000df50: 2d2d 0a20 2020 206d 7520 3a20 7465 6e73  --.    mu : tens
+0000df60: 6f72 5f6c 696b 6520 6f66 2066 6c6f 6174  or_like of float
+0000df70: 0a20 2020 2020 2020 2041 7272 6179 206f  .        Array o
+0000df80: 6620 6d65 616e 732e 204d 7573 7420 6265  f means. Must be
+0000df90: 2062 726f 6164 6361 7374 6162 6c65 2077   broadcastable w
+0000dfa0: 6974 6820 7468 6520 7261 6e64 6f6d 2076  ith the random v
+0000dfb0: 6172 6961 626c 6520 5820 7375 6368 0a20  ariable X such. 
+0000dfc0: 2020 2020 2020 2074 6861 7420 7468 6520         that the 
+0000dfd0: 7368 6170 6520 6f66 206d 7520 2b20 5820  shape of mu + X 
+0000dfe0: 6973 2028 4d2c 204e 292e 0a20 2020 2072  is (M, N)..    r
+0000dff0: 6f77 636f 7620 3a20 284d 2c20 4d29 2074  owcov : (M, M) t
+0000e000: 656e 736f 725f 6c69 6b65 206f 6620 666c  ensor_like of fl
+0000e010: 6f61 742c 206f 7074 696f 6e61 6c0a 2020  oat, optional.  
+0000e020: 2020 2020 2020 416d 6f6e 672d 726f 7720        Among-row 
+0000e030: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000e040: 782e 2044 6566 696e 6573 2076 6172 6961  x. Defines varia
+0000e050: 6e63 6520 7769 7468 696e 0a20 2020 2020  nce within.     
+0000e060: 2020 2063 6f6c 756d 6e73 2e20 4578 6163     columns. Exac
+0000e070: 746c 7920 6f6e 6520 6f66 2072 6f77 636f  tly one of rowco
+0000e080: 7620 6f72 2072 6f77 6368 6f6c 2069 7320  v or rowchol is 
+0000e090: 6e65 6564 6564 2e0a 2020 2020 726f 7763  needed..    rowc
+0000e0a0: 686f 6c20 3a20 284d 2c20 4d29 2074 656e  hol : (M, M) ten
+0000e0b0: 736f 725f 6c69 6b65 206f 6620 666c 6f61  sor_like of floa
+0000e0c0: 742c 206f 7074 696f 6e61 6c0a 2020 2020  t, optional.    
+0000e0d0: 2020 2020 4368 6f6c 6573 6b79 2064 6563      Cholesky dec
+0000e0e0: 6f6d 706f 7369 7469 6f6e 206f 6620 616d  omposition of am
+0000e0f0: 6f6e 672d 726f 7720 636f 7661 7269 616e  ong-row covarian
+0000e100: 6365 206d 6174 7269 782e 2045 7861 6374  ce matrix. Exact
+0000e110: 6c79 206f 6e65 206f 660a 2020 2020 2020  ly one of.      
+0000e120: 2020 726f 7763 6f76 206f 7220 726f 7763    rowcov or rowc
+0000e130: 686f 6c20 6973 206e 6565 6465 642e 0a20  hol is needed.. 
+0000e140: 2020 2063 6f6c 636f 7620 3a20 284e 2c20     colcov : (N, 
+0000e150: 4e29 2074 656e 736f 725f 6c69 6b65 206f  N) tensor_like o
+0000e160: 6620 666c 6f61 742c 206f 7074 696f 6e61  f float, optiona
+0000e170: 6c0a 2020 2020 2020 2020 416d 6f6e 672d  l.        Among-
+0000e180: 636f 6c75 6d6e 2063 6f76 6172 6961 6e63  column covarianc
+0000e190: 6520 6d61 7472 6978 2e20 4966 2072 6f77  e matrix. If row
+0000e1a0: 636f 7620 6973 2074 6865 2069 6465 6e74  cov is the ident
+0000e1b0: 6974 7920 6d61 7472 6978 2c0a 2020 2020  ity matrix,.    
+0000e1c0: 2020 2020 7468 6973 2066 756e 6374 696f      this functio
+0000e1d0: 6e73 2061 7320 6063 6f76 6020 696e 204d  ns as `cov` in M
+0000e1e0: 764e 6f72 6d61 6c2e 0a20 2020 2020 2020  vNormal..       
+0000e1f0: 2045 7861 6374 6c79 206f 6e65 206f 6620   Exactly one of 
+0000e200: 636f 6c63 6f76 206f 7220 636f 6c63 686f  colcov or colcho
+0000e210: 6c20 6973 206e 6565 6465 642e 0a20 2020  l is needed..   
+0000e220: 2063 6f6c 6368 6f6c 203a 2028 4e2c 204e   colchol : (N, N
+0000e230: 2920 7465 6e73 6f72 5f6c 696b 6520 6f66  ) tensor_like of
+0000e240: 2066 6c6f 6174 2c20 6f70 7469 6f6e 616c   float, optional
+0000e250: 0a20 2020 2020 2020 2043 686f 6c65 736b  .        Cholesk
+0000e260: 7920 6465 636f 6d70 6f73 6974 696f 6e20  y decomposition 
+0000e270: 6f66 2061 6d6f 6e67 2d63 6f6c 756d 6e20  of among-column 
+0000e280: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+0000e290: 782e 2045 7861 6374 6c79 206f 6e65 0a20  x. Exactly one. 
+0000e2a0: 2020 2020 2020 206f 6620 636f 6c63 6f76         of colcov
+0000e2b0: 206f 7220 636f 6c63 686f 6c20 6973 206e   or colchol is n
+0000e2c0: 6565 6465 642e 0a0a 2020 2020 4578 616d  eeded...    Exam
+0000e2d0: 706c 6573 0a20 2020 202d 2d2d 2d2d 2d2d  ples.    -------
+0000e2e0: 2d0a 2020 2020 4465 6669 6e65 2061 206d  -.    Define a m
+0000e2f0: 6174 7269 7876 6172 6961 7465 206e 6f72  atrixvariate nor
+0000e300: 6d61 6c20 7661 7269 6162 6c65 2066 6f72  mal variable for
+0000e310: 2067 6976 656e 2072 6f77 2061 6e64 2063   given row and c
+0000e320: 6f6c 756d 6e20 636f 7661 7269 616e 6365  olumn covariance
+0000e330: 0a20 2020 206d 6174 7269 6365 733a 3a0a  .    matrices::.
+0000e340: 0a20 2020 2020 2020 2063 6f6c 636f 7620  .        colcov 
+0000e350: 3d20 6e70 2e61 7272 6179 285b 5b31 2e2c  = np.array([[1.,
+0000e360: 2030 2e35 5d2c 205b 302e 352c 2032 5d5d   0.5], [0.5, 2]]
+0000e370: 290a 2020 2020 2020 2020 726f 7763 6f76  ).        rowcov
+0000e380: 203d 206e 702e 6172 7261 7928 5b5b 312c   = np.array([[1,
+0000e390: 2030 2c20 305d 2c20 5b30 2c20 342c 2030   0, 0], [0, 4, 0
+0000e3a0: 5d2c 205b 302c 2030 2c20 3136 5d5d 290a  ], [0, 0, 16]]).
+0000e3b0: 2020 2020 2020 2020 6d20 3d20 726f 7763          m = rowc
+0000e3c0: 6f76 2e73 6861 7065 5b30 5d0a 2020 2020  ov.shape[0].    
+0000e3d0: 2020 2020 6e20 3d20 636f 6c63 6f76 2e73      n = colcov.s
+0000e3e0: 6861 7065 5b30 5d0a 2020 2020 2020 2020  hape[0].        
+0000e3f0: 6d75 203d 206e 702e 7a65 726f 7328 286d  mu = np.zeros((m
+0000e400: 2c20 6e29 290a 2020 2020 2020 2020 7661  , n)).        va
+0000e410: 6c73 203d 2070 6d2e 4d61 7472 6978 4e6f  ls = pm.MatrixNo
+0000e420: 726d 616c 2827 7661 6c73 272c 206d 753d  rmal('vals', mu=
+0000e430: 6d75 2c20 636f 6c63 6f76 3d63 6f6c 636f  mu, colcov=colco
+0000e440: 762c 0a20 2020 2020 2020 2020 2020 2020  v,.             
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 2020 726f 7763 6f76 3d72 6f77 636f 7629    rowcov=rowcov)
+0000e470: 0a0a 2020 2020 4162 6f76 652c 2074 6865  ..    Above, the
+0000e480: 2069 7468 2072 6f77 2069 6e20 7661 6c73   ith row in vals
+0000e490: 2068 6173 2061 2076 6172 6961 6e63 6520   has a variance 
+0000e4a0: 7468 6174 2069 7320 7363 616c 6564 2062  that is scaled b
+0000e4b0: 7920 345e 692e 0a20 2020 2041 6c74 6572  y 4^i..    Alter
+0000e4c0: 6e61 7469 7665 6c79 2c20 726f 7720 6f72  natively, row or
+0000e4d0: 2063 6f6c 756d 6e20 6368 6f6c 6573 6b79   column cholesky
+0000e4e0: 206d 6174 7269 6365 7320 636f 756c 6420   matrices could 
+0000e4f0: 6265 2073 7562 7374 6974 7574 6564 2066  be substituted f
+0000e500: 6f72 0a20 2020 2065 6974 6865 7220 636f  or.    either co
+0000e510: 7661 7269 616e 6365 206d 6174 7269 782e  variance matrix.
+0000e520: 2054 6865 204d 6174 7269 784e 6f72 6d61   The MatrixNorma
+0000e530: 6c20 6973 2071 7569 636b 6572 2077 6179  l is quicker way
+0000e540: 2063 6f6d 7075 7465 0a20 2020 204d 764e   compute.    MvN
+0000e550: 6f72 6d61 6c28 6d75 2c20 6e70 2e6b 726f  ormal(mu, np.kro
+0000e560: 6e28 726f 7763 6f76 2c20 636f 6c63 6f76  n(rowcov, colcov
+0000e570: 2929 2074 6861 7420 7461 6b65 7320 6164  )) that takes ad
+0000e580: 7661 6e74 6167 6520 6f66 206b 726f 6e65  vantage of krone
+0000e590: 636b 6572 2070 726f 6475 6374 0a20 2020  cker product.   
+0000e5a0: 2070 726f 7065 7274 6965 7320 666f 7220   properties for 
+0000e5b0: 696e 7665 7273 696f 6e2e 2046 6f72 2065  inversion. For e
+0000e5c0: 7861 6d70 6c65 2c20 6966 2064 7261 7773  xample, if draws
+0000e5d0: 2066 726f 6d20 4d76 4e6f 726d 616c 2068   from MvNormal h
+0000e5e0: 6164 2074 6865 2073 616d 650a 2020 2020  ad the same.    
+0000e5f0: 636f 7661 7269 616e 6365 2073 7472 7563  covariance struc
+0000e600: 7475 7265 2c20 6275 7420 7765 7265 2073  ture, but were s
+0000e610: 6361 6c65 6420 6279 2064 6966 6665 7265  caled by differe
+0000e620: 6e74 2070 6f77 6572 7320 6f66 2061 6e20  nt powers of an 
+0000e630: 756e 6b6e 6f77 6e0a 2020 2020 636f 6e73  unknown.    cons
+0000e640: 7461 6e74 2c20 626f 7468 2074 6865 2063  tant, both the c
+0000e650: 6f76 6172 6961 6e63 6520 616e 6420 7363  ovariance and sc
+0000e660: 616c 696e 6720 636f 756c 6420 6265 206c  aling could be l
+0000e670: 6561 726e 6564 2061 7320 666f 6c6c 6f77  earned as follow
+0000e680: 730a 2020 2020 2873 6565 2074 6865 2064  s.    (see the d
+0000e690: 6f63 7374 7269 6e67 206f 6620 604c 4b4a  ocstring of `LKJ
+0000e6a0: 4368 6f6c 6573 6b79 436f 7660 2066 6f72  CholeskyCov` for
+0000e6b0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+0000e6c0: 6e20 6162 6f75 7420 7468 6973 290a 0a20  n about this).. 
+0000e6d0: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
+0000e6e0: 686f 6e0a 0a20 2020 2020 2020 2023 2053  hon..        # S
+0000e6f0: 6574 7570 2064 6174 610a 2020 2020 2020  etup data.      
+0000e700: 2020 7472 7565 5f63 6f6c 636f 7620 3d20    true_colcov = 
+0000e710: 6e70 2e61 7272 6179 285b 5b31 2e30 2c20  np.array([[1.0, 
+0000e720: 302e 352c 2030 2e31 5d2c 0a20 2020 2020  0.5, 0.1],.     
+0000e730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e740: 2020 2020 2020 2020 2020 205b 302e 352c             [0.5,
+0000e750: 2031 2e30 2c20 302e 325d 2c0a 2020 2020   1.0, 0.2],.    
+0000e760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e770: 2020 2020 2020 2020 2020 2020 5b30 2e31              [0.1
+0000e780: 2c20 302e 322c 2031 2e30 5d5d 290a 2020  , 0.2, 1.0]]).  
+0000e790: 2020 2020 2020 6d20 3d20 330a 2020 2020        m = 3.    
+0000e7a0: 2020 2020 6e20 3d20 7472 7565 5f63 6f6c      n = true_col
+0000e7b0: 636f 762e 7368 6170 655b 305d 0a20 2020  cov.shape[0].   
+0000e7c0: 2020 2020 2074 7275 655f 7363 616c 6520       true_scale 
+0000e7d0: 3d20 330a 2020 2020 2020 2020 7472 7565  = 3.        true
+0000e7e0: 5f72 6f77 636f 7620 3d20 6e70 2e64 6961  _rowcov = np.dia
+0000e7f0: 6728 5b74 7275 655f 7363 616c 652a 2a28  g([true_scale**(
+0000e800: 322a 6929 2066 6f72 2069 2069 6e20 7261  2*i) for i in ra
+0000e810: 6e67 6528 6d29 5d29 0a20 2020 2020 2020  nge(m)]).       
+0000e820: 206d 7520 3d20 6e70 2e7a 6572 6f73 2828   mu = np.zeros((
+0000e830: 6d2c 206e 2929 0a20 2020 2020 2020 2074  m, n)).        t
+0000e840: 7275 655f 6b72 6f6e 203d 206e 702e 6b72  rue_kron = np.kr
+0000e850: 6f6e 2874 7275 655f 726f 7763 6f76 2c20  on(true_rowcov, 
+0000e860: 7472 7565 5f63 6f6c 636f 7629 0a20 2020  true_colcov).   
+0000e870: 2020 2020 2064 6174 6120 3d20 6e70 2e72       data = np.r
+0000e880: 616e 646f 6d2e 6d75 6c74 6976 6172 6961  andom.multivaria
+0000e890: 7465 5f6e 6f72 6d61 6c28 6d75 2e66 6c61  te_normal(mu.fla
+0000e8a0: 7474 656e 2829 2c20 7472 7565 5f6b 726f  tten(), true_kro
+0000e8b0: 6e29 0a20 2020 2020 2020 2064 6174 6120  n).        data 
+0000e8c0: 3d20 6461 7461 2e72 6573 6861 7065 286d  = data.reshape(m
+0000e8d0: 2c20 6e29 0a0a 2020 2020 2020 2020 7769  , n)..        wi
+0000e8e0: 7468 2070 6d2e 4d6f 6465 6c28 2920 6173  th pm.Model() as
+0000e8f0: 206d 6f64 656c 3a0a 2020 2020 2020 2020   model:.        
+0000e900: 2020 2020 2320 5365 7475 7020 7269 6768      # Setup righ
+0000e910: 7420 6368 6f6c 6573 6b79 206d 6174 7269  t cholesky matri
+0000e920: 780a 2020 2020 2020 2020 2020 2020 7364  x.            sd
+0000e930: 5f64 6973 7420 3d20 706d 2e48 616c 6643  _dist = pm.HalfC
+0000e940: 6175 6368 792e 6469 7374 2862 6574 613d  auchy.dist(beta=
+0000e950: 322e 352c 2073 6861 7065 3d33 290a 2020  2.5, shape=3).  
+0000e960: 2020 2020 2020 2020 2020 636f 6c63 686f            colcho
+0000e970: 6c5f 7061 636b 6564 203d 2070 6d2e 4c4b  l_packed = pm.LK
+0000e980: 4a43 686f 6c65 736b 7943 6f76 2827 636f  JCholeskyCov('co
+0000e990: 6c63 686f 6c70 6163 6b65 6427 2c20 6e3d  lcholpacked', n=
+0000e9a0: 332c 2065 7461 3d32 2c0a 2020 2020 2020  3, eta=2,.      
+0000e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e9d0: 2020 2020 2020 2020 2073 645f 6469 7374           sd_dist
+0000e9e0: 3d73 645f 6469 7374 290a 2020 2020 2020  =sd_dist).      
+0000e9f0: 2020 2020 2020 636f 6c63 686f 6c20 3d20        colchol = 
+0000ea00: 706d 2e65 7870 616e 645f 7061 636b 6564  pm.expand_packed
+0000ea10: 5f74 7269 616e 6775 6c61 7228 332c 2063  _triangular(3, c
+0000ea20: 6f6c 6368 6f6c 5f70 6163 6b65 6429 0a0a  olchol_packed)..
+0000ea30: 2020 2020 2020 2020 2020 2020 2320 5365              # Se
+0000ea40: 7475 7020 6c65 6674 2063 6f76 6172 6961  tup left covaria
+0000ea50: 6e63 6520 6d61 7472 6978 0a20 2020 2020  nce matrix.     
+0000ea60: 2020 2020 2020 2073 6361 6c65 203d 2070         scale = p
+0000ea70: 6d2e 4c6f 674e 6f72 6d61 6c28 2773 6361  m.LogNormal('sca
+0000ea80: 6c65 272c 206d 753d 6e70 2e6c 6f67 2874  le', mu=np.log(t
+0000ea90: 7275 655f 7363 616c 6529 2c20 7369 676d  rue_scale), sigm
+0000eaa0: 613d 302e 3529 0a20 2020 2020 2020 2020  a=0.5).         
+0000eab0: 2020 2072 6f77 636f 7620 3d20 7074 2e64     rowcov = pt.d
+0000eac0: 6961 6728 5b73 6361 6c65 2a2a 2832 2a69  iag([scale**(2*i
+0000ead0: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
+0000eae0: 286d 295d 290a 0a20 2020 2020 2020 2020  (m)])..         
+0000eaf0: 2020 2076 616c 7320 3d20 706d 2e4d 6174     vals = pm.Mat
+0000eb00: 7269 784e 6f72 6d61 6c28 2776 616c 7327  rixNormal('vals'
+0000eb10: 2c20 6d75 3d6d 752c 2063 6f6c 6368 6f6c  , mu=mu, colchol
+0000eb20: 3d63 6f6c 6368 6f6c 2c20 726f 7763 6f76  =colchol, rowcov
+0000eb30: 3d72 6f77 636f 762c 0a20 2020 2020 2020  =rowcov,.       
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb50: 2020 2020 2020 2020 2020 2020 6f62 7365              obse
+0000eb60: 7276 6564 3d64 6174 6129 0a20 2020 2022  rved=data).    "
+0000eb70: 2222 0a20 2020 2072 765f 6f70 203d 206d  "".    rv_op = m
+0000eb80: 6174 7269 786e 6f72 6d61 6c0a 0a20 2020  atrixnormal..   
+0000eb90: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+0000eba0: 2020 6465 6620 6469 7374 280a 2020 2020    def dist(.    
+0000ebb0: 2020 2020 636c 732c 0a20 2020 2020 2020      cls,.       
+0000ebc0: 206d 752c 0a20 2020 2020 2020 2072 6f77   mu,.        row
+0000ebd0: 636f 763d 4e6f 6e65 2c0a 2020 2020 2020  cov=None,.      
+0000ebe0: 2020 726f 7763 686f 6c3d 4e6f 6e65 2c0a    rowchol=None,.
+0000ebf0: 2020 2020 2020 2020 636f 6c63 6f76 3d4e          colcov=N
+0000ec00: 6f6e 652c 0a20 2020 2020 2020 2063 6f6c  one,.        col
+0000ec10: 6368 6f6c 3d4e 6f6e 652c 0a20 2020 2020  chol=None,.     
+0000ec20: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
+0000ec30: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
+0000ec40: 293a 0a20 2020 2020 2020 2063 686f 6c65  ):.        chole
+0000ec50: 736b 7920 3d20 4368 6f6c 6573 6b79 286c  sky = Cholesky(l
+0000ec60: 6f77 6572 3d54 7275 652c 206f 6e5f 6572  ower=True, on_er
+0000ec70: 726f 723d 2272 6169 7365 2229 0a0a 2020  ror="raise")..  
+0000ec80: 2020 2020 2020 2320 416d 6f6e 672d 726f        # Among-ro
+0000ec90: 7720 6d61 7472 6963 6573 0a20 2020 2020  w matrices.     
+0000eca0: 2020 2069 6620 6c65 6e28 5b69 2066 6f72     if len([i for
+0000ecb0: 2069 2069 6e20 5b72 6f77 636f 762c 2072   i in [rowcov, r
+0000ecc0: 6f77 6368 6f6c 5d20 6966 2069 2069 7320  owchol] if i is 
+0000ecd0: 6e6f 7420 4e6f 6e65 5d29 2021 3d20 313a  not None]) != 1:
+0000ece0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0000ecf0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000ed10: 496e 636f 6d70 6174 6962 6c65 2070 6172  Incompatible par
+0000ed20: 616d 6574 6572 697a 6174 696f 6e2e 2053  ameterization. S
+0000ed30: 7065 6369 6679 2065 7861 6374 6c79 206f  pecify exactly o
+0000ed40: 6e65 206f 6620 726f 7763 6f76 2c20 6f72  ne of rowcov, or
+0000ed50: 2072 6f77 6368 6f6c 2e22 0a20 2020 2020   rowchol.".     
+0000ed60: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+0000ed70: 2069 6620 726f 7763 6f76 2069 7320 6e6f   if rowcov is no
+0000ed80: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+0000ed90: 2020 2020 6966 2072 6f77 636f 762e 6e64      if rowcov.nd
+0000eda0: 696d 2021 3d20 323a 0a20 2020 2020 2020  im != 2:.       
+0000edb0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000edc0: 616c 7565 4572 726f 7228 2272 6f77 636f  alueError("rowco
+0000edd0: 7620 6d75 7374 2062 6520 7477 6f20 6469  v must be two di
+0000ede0: 6d65 6e73 696f 6e61 6c2e 2229 0a20 2020  mensional.").   
+0000edf0: 2020 2020 2020 2020 2072 6f77 6368 6f6c           rowchol
+0000ee00: 5f63 6f76 203d 2063 686f 6c65 736b 7928  _cov = cholesky(
+0000ee10: 726f 7763 6f76 290a 2020 2020 2020 2020  rowcov).        
+0000ee20: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000ee30: 2020 6966 2072 6f77 6368 6f6c 2e6e 6469    if rowchol.ndi
+0000ee40: 6d20 213d 2032 3a0a 2020 2020 2020 2020  m != 2:.        
+0000ee50: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000ee60: 6c75 6545 7272 6f72 2822 726f 7763 686f  lueError("rowcho
+0000ee70: 6c20 6d75 7374 2062 6520 7477 6f20 6469  l must be two di
+0000ee80: 6d65 6e73 696f 6e61 6c2e 2229 0a20 2020  mensional.").   
+0000ee90: 2020 2020 2020 2020 2072 6f77 6368 6f6c           rowchol
+0000eea0: 5f63 6f76 203d 2070 742e 6173 5f74 656e  _cov = pt.as_ten
+0000eeb0: 736f 725f 7661 7269 6162 6c65 2872 6f77  sor_variable(row
+0000eec0: 6368 6f6c 290a 0a20 2020 2020 2020 2023  chol)..        #
+0000eed0: 2041 6d6f 6e67 2d63 6f6c 756d 6e20 6d61   Among-column ma
+0000eee0: 7472 6963 6573 0a20 2020 2020 2020 2069  trices.        i
+0000eef0: 6620 6c65 6e28 5b69 2066 6f72 2069 2069  f len([i for i i
+0000ef00: 6e20 5b63 6f6c 636f 762c 2063 6f6c 6368  n [colcov, colch
+0000ef10: 6f6c 5d20 6966 2069 2069 7320 6e6f 7420  ol] if i is not 
+0000ef20: 4e6f 6e65 5d29 2021 3d20 313a 0a20 2020  None]) != 1:.   
+0000ef30: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000ef40: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+0000ef50: 2020 2020 2020 2020 2020 2022 496e 636f             "Inco
+0000ef60: 6d70 6174 6962 6c65 2070 6172 616d 6574  mpatible paramet
+0000ef70: 6572 697a 6174 696f 6e2e 2053 7065 6369  erization. Speci
+0000ef80: 6679 2065 7861 6374 6c79 206f 6e65 206f  fy exactly one o
+0000ef90: 6620 636f 6c63 6f76 2c20 6f72 2063 6f6c  f colcov, or col
+0000efa0: 6368 6f6c 2e22 0a20 2020 2020 2020 2020  chol.".         
+0000efb0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
+0000efc0: 636f 6c63 6f76 2069 7320 6e6f 7420 4e6f  colcov is not No
+0000efd0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000efe0: 636f 6c63 6f76 203d 2070 742e 6173 5f74  colcov = pt.as_t
+0000eff0: 656e 736f 725f 7661 7269 6162 6c65 2863  ensor_variable(c
+0000f000: 6f6c 636f 7629 0a20 2020 2020 2020 2020  olcov).         
+0000f010: 2020 2069 6620 636f 6c63 6f76 2e6e 6469     if colcov.ndi
+0000f020: 6d20 213d 2032 3a0a 2020 2020 2020 2020  m != 2:.        
+0000f030: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+0000f040: 6c75 6545 7272 6f72 2822 636f 6c63 6f76  lueError("colcov
+0000f050: 206d 7573 7420 6265 2074 776f 2064 696d   must be two dim
+0000f060: 656e 7369 6f6e 616c 2e22 290a 2020 2020  ensional.").    
+0000f070: 2020 2020 2020 2020 636f 6c63 686f 6c5f          colchol_
+0000f080: 636f 7620 3d20 6368 6f6c 6573 6b79 2863  cov = cholesky(c
+0000f090: 6f6c 636f 7629 0a20 2020 2020 2020 2065  olcov).        e
+0000f0a0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+0000f0b0: 2069 6620 636f 6c63 686f 6c2e 6e64 696d   if colchol.ndim
+0000f0c0: 2021 3d20 323a 0a20 2020 2020 2020 2020   != 2:.         
+0000f0d0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+0000f0e0: 7565 4572 726f 7228 2263 6f6c 6368 6f6c  ueError("colchol
+0000f0f0: 206d 7573 7420 6265 2074 776f 2064 696d   must be two dim
+0000f100: 656e 7369 6f6e 616c 2e22 290a 2020 2020  ensional.").    
+0000f110: 2020 2020 2020 2020 636f 6c63 686f 6c5f          colchol_
+0000f120: 636f 7620 3d20 7074 2e61 735f 7465 6e73  cov = pt.as_tens
+0000f130: 6f72 5f76 6172 6961 626c 6528 636f 6c63  or_variable(colc
+0000f140: 686f 6c29 0a0a 2020 2020 2020 2020 6469  hol)..        di
+0000f150: 7374 5f73 6861 7065 203d 2028 726f 7763  st_shape = (rowc
+0000f160: 686f 6c5f 636f 762e 7368 6170 655b 2d31  hol_cov.shape[-1
+0000f170: 5d2c 2063 6f6c 6368 6f6c 5f63 6f76 2e73  ], colchol_cov.s
+0000f180: 6861 7065 5b2d 315d 290a 0a20 2020 2020  hape[-1])..     
+0000f190: 2020 2023 2042 726f 6164 6361 7374 696e     # Broadcastin
+0000f1a0: 6720 6d75 0a20 2020 2020 2020 206d 7520  g mu.        mu 
+0000f1b0: 3d20 7074 2e65 7874 7261 5f6f 7073 2e62  = pt.extra_ops.b
+0000f1c0: 726f 6164 6361 7374 5f74 6f28 6d75 2c20  roadcast_to(mu, 
+0000f1d0: 7368 6170 653d 6469 7374 5f73 6861 7065  shape=dist_shape
+0000f1e0: 290a 2020 2020 2020 2020 6d75 203d 2070  ).        mu = p
+0000f1f0: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+0000f200: 6162 6c65 2866 6c6f 6174 5828 6d75 2929  able(floatX(mu))
+0000f210: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+0000f220: 2073 7570 6572 2829 2e64 6973 7428 5b6d   super().dist([m
+0000f230: 752c 2072 6f77 6368 6f6c 5f63 6f76 2c20  u, rowchol_cov, 
+0000f240: 636f 6c63 686f 6c5f 636f 765d 2c20 2a2a  colchol_cov], **
+0000f250: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
+0000f260: 206d 6f6d 656e 7428 7276 2c20 7369 7a65   moment(rv, size
+0000f270: 2c20 6d75 2c20 726f 7763 686f 6c2c 2063  , mu, rowchol, c
+0000f280: 6f6c 6368 6f6c 293a 0a20 2020 2020 2020  olchol):.       
+0000f290: 2072 6574 7572 6e20 7074 2e66 756c 6c5f   return pt.full_
+0000f2a0: 6c69 6b65 2872 762c 206d 7529 0a0a 2020  like(rv, mu)..  
+0000f2b0: 2020 6465 6620 6c6f 6770 2876 616c 7565    def logp(value
+0000f2c0: 2c20 6d75 2c20 726f 7763 686f 6c2c 2063  , mu, rowchol, c
+0000f2d0: 6f6c 6368 6f6c 293a 0a20 2020 2020 2020  olchol):.       
+0000f2e0: 2022 2222 0a20 2020 2020 2020 2043 616c   """.        Cal
+0000f2f0: 6375 6c61 7465 206c 6f67 2d70 726f 6261  culate log-proba
+0000f300: 6269 6c69 7479 206f 6620 4d61 7472 6978  bility of Matrix
+0000f310: 2d76 616c 7565 6420 4e6f 726d 616c 2064  -valued Normal d
+0000f320: 6973 7472 6962 7574 696f 6e0a 2020 2020  istribution.    
+0000f330: 2020 2020 6174 2073 7065 6369 6669 6564      at specified
+0000f340: 2076 616c 7565 2e0a 0a20 2020 2020 2020   value...       
+0000f350: 2050 6172 616d 6574 6572 730a 2020 2020   Parameters.    
+0000f360: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+0000f370: 2020 2020 2020 2076 616c 7565 3a20 6e75         value: nu
+0000f380: 6d65 7269 630a 2020 2020 2020 2020 2020  meric.          
+0000f390: 2020 5661 6c75 6520 666f 7220 7768 6963    Value for whic
+0000f3a0: 6820 6c6f 672d 7072 6f62 6162 696c 6974  h log-probabilit
+0000f3b0: 7920 6973 2063 616c 6375 6c61 7465 642e  y is calculated.
+0000f3c0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000f3d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+0000f3e0: 2d0a 2020 2020 2020 2020 5465 6e73 6f72  -.        Tensor
+0000f3f0: 5661 7269 6162 6c65 0a20 2020 2020 2020  Variable.       
+0000f400: 2022 2222 0a0a 2020 2020 2020 2020 6966   """..        if
+0000f410: 2076 616c 7565 2e6e 6469 6d20 213d 2032   value.ndim != 2
+0000f420: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000f430: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0000f440: 5661 6c75 6520 6d75 7374 2062 6520 7477  Value must be tw
+0000f450: 6f20 6469 6d65 6e73 696f 6e61 6c2e 2229  o dimensional.")
+0000f460: 0a0a 2020 2020 2020 2020 2320 436f 6d70  ..        # Comp
+0000f470: 7574 6520 5472 5b63 6f6c 636f 765e 2d31  ute Tr[colcov^-1
+0000f480: 2040 2028 7820 2d20 6d75 292e 5420 4020   @ (x - mu).T @ 
+0000f490: 726f 7763 6f76 5e2d 3120 4020 2878 202d  rowcov^-1 @ (x -
+0000f4a0: 206d 7529 5d20 616e 640a 2020 2020 2020   mu)] and.      
+0000f4b0: 2020 2320 7468 6520 6c6f 6764 6574 206f    # the logdet o
+0000f4c0: 6620 636f 6c63 6f76 2061 6e64 2072 6f77  f colcov and row
+0000f4d0: 636f 762e 0a20 2020 2020 2020 2064 656c  cov..        del
+0000f4e0: 7461 203d 2076 616c 7565 202d 206d 750a  ta = value - mu.
+0000f4f0: 0a20 2020 2020 2020 2023 2046 696e 6420  .        # Find 
+0000f500: 6578 706f 6e65 6e74 2070 6965 6365 2062  exponent piece b
+0000f510: 7920 7069 6563 650a 2020 2020 2020 2020  y piece.        
+0000f520: 7269 6768 745f 7175 6164 6469 7374 203d  right_quaddist =
+0000f530: 2073 6f6c 7665 5f6c 6f77 6572 2872 6f77   solve_lower(row
+0000f540: 6368 6f6c 2c20 6465 6c74 6129 0a20 2020  chol, delta).   
+0000f550: 2020 2020 2071 7561 6464 6973 7420 3d20       quaddist = 
+0000f560: 7074 2e6e 6c69 6e61 6c67 2e6d 6174 7269  pt.nlinalg.matri
+0000f570: 785f 646f 7428 7269 6768 745f 7175 6164  x_dot(right_quad
+0000f580: 6469 7374 2e54 2c20 7269 6768 745f 7175  dist.T, right_qu
+0000f590: 6164 6469 7374 290a 2020 2020 2020 2020  addist).        
+0000f5a0: 7175 6164 6469 7374 203d 2073 6f6c 7665  quaddist = solve
+0000f5b0: 5f6c 6f77 6572 2863 6f6c 6368 6f6c 2c20  _lower(colchol, 
+0000f5c0: 7175 6164 6469 7374 290a 2020 2020 2020  quaddist).      
+0000f5d0: 2020 7175 6164 6469 7374 203d 2073 6f6c    quaddist = sol
+0000f5e0: 7665 5f75 7070 6572 2863 6f6c 6368 6f6c  ve_upper(colchol
+0000f5f0: 2e54 2c20 7175 6164 6469 7374 290a 2020  .T, quaddist).  
+0000f600: 2020 2020 2020 7472 7175 6164 6469 7374        trquaddist
+0000f610: 203d 2070 742e 6e6c 696e 616c 672e 7472   = pt.nlinalg.tr
+0000f620: 6163 6528 7175 6164 6469 7374 290a 0a20  ace(quaddist).. 
+0000f630: 2020 2020 2020 2063 6f6c 6469 6167 203d         coldiag =
+0000f640: 2070 742e 6469 6167 2863 6f6c 6368 6f6c   pt.diag(colchol
+0000f650: 290a 2020 2020 2020 2020 726f 7764 6961  ).        rowdia
+0000f660: 6720 3d20 7074 2e64 6961 6728 726f 7763  g = pt.diag(rowc
+0000f670: 686f 6c29 0a20 2020 2020 2020 2068 616c  hol).        hal
+0000f680: 665f 636f 6c6c 6f67 6465 7420 3d20 7074  f_collogdet = pt
+0000f690: 2e73 756d 2870 742e 6c6f 6728 636f 6c64  .sum(pt.log(cold
+0000f6a0: 6961 6729 2920 2023 206c 6f67 6465 7428  iag))  # logdet(
+0000f6b0: 4d29 203d 2032 2a54 7228 6c6f 6728 4c29  M) = 2*Tr(log(L)
+0000f6c0: 290a 2020 2020 2020 2020 6861 6c66 5f72  ).        half_r
+0000f6d0: 6f77 6c6f 6764 6574 203d 2070 742e 7375  owlogdet = pt.su
+0000f6e0: 6d28 7074 2e6c 6f67 2872 6f77 6469 6167  m(pt.log(rowdiag
+0000f6f0: 2929 2020 2320 5573 696e 6720 4368 6f6c  ))  # Using Chol
+0000f700: 6573 6b79 3a20 4d20 3d20 4c20 4c5e 540a  esky: M = L L^T.
+0000f710: 0a20 2020 2020 2020 206d 203d 2072 6f77  .        m = row
+0000f720: 6368 6f6c 2e73 6861 7065 5b30 5d0a 2020  chol.shape[0].  
+0000f730: 2020 2020 2020 6e20 3d20 636f 6c63 686f        n = colcho
+0000f740: 6c2e 7368 6170 655b 305d 0a0a 2020 2020  l.shape[0]..    
+0000f750: 2020 2020 6e6f 726d 203d 202d 302e 3520      norm = -0.5 
+0000f760: 2a20 6d20 2a20 6e20 2a20 706d 2e66 6c6f  * m * n * pm.flo
+0000f770: 6174 5828 6e70 2e6c 6f67 2832 202a 206e  atX(np.log(2 * n
+0000f780: 702e 7069 2929 0a20 2020 2020 2020 2072  p.pi)).        r
+0000f790: 6574 7572 6e20 6e6f 726d 202d 2030 2e35  eturn norm - 0.5
+0000f7a0: 202a 2074 7271 7561 6464 6973 7420 2d20   * trquaddist - 
+0000f7b0: 6d20 2a20 6861 6c66 5f63 6f6c 6c6f 6764  m * half_collogd
+0000f7c0: 6574 202d 206e 202a 2068 616c 665f 726f  et - n * half_ro
+0000f7d0: 776c 6f67 6465 740a 0a0a 636c 6173 7320  wlogdet...class 
+0000f7e0: 4b72 6f6e 6563 6b65 724e 6f72 6d61 6c52  KroneckerNormalR
+0000f7f0: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
+0000f800: 293a 0a20 2020 206e 616d 6520 3d20 226b  ):.    name = "k
+0000f810: 726f 6e65 636b 6572 6e6f 726d 616c 220a  roneckernormal".
+0000f820: 2020 2020 6e64 696d 5f73 7570 7020 3d20      ndim_supp = 
+0000f830: 310a 2020 2020 6e64 696d 735f 7061 7261  1.    ndims_para
+0000f840: 6d73 203d 205b 312c 2030 2c20 325d 0a20  ms = [1, 0, 2]. 
+0000f850: 2020 2064 7479 7065 203d 2022 666c 6f61     dtype = "floa
+0000f860: 7458 220a 2020 2020 5f70 7269 6e74 5f6e  tX".    _print_n
+0000f870: 616d 6520 3d20 2822 4b72 6f6e 6563 6b65  ame = ("Kronecke
+0000f880: 724e 6f72 6d61 6c22 2c20 225c 5c6f 7065  rNormal", "\\ope
+0000f890: 7261 746f 726e 616d 657b 4b72 6f6e 6563  ratorname{Kronec
+0000f8a0: 6b65 724e 6f72 6d61 6c7d 2229 0a0a 2020  kerNormal}")..  
+0000f8b0: 2020 6465 6620 726e 675f 666e 2873 656c    def rng_fn(sel
+0000f8c0: 662c 2072 6e67 2c20 6d75 2c20 7369 676d  f, rng, mu, sigm
+0000f8d0: 612c 202a 636f 7673 2c20 7369 7a65 3d4e  a, *covs, size=N
+0000f8e0: 6f6e 6529 3a0a 2020 2020 2020 2020 7369  one):.        si
+0000f8f0: 7a65 203d 2073 697a 6520 6966 2073 697a  ze = size if siz
+0000f900: 6520 656c 7365 2063 6f76 735b 2d31 5d0a  e else covs[-1].
+0000f910: 2020 2020 2020 2020 636f 7673 203d 2063          covs = c
+0000f920: 6f76 735b 3a2d 315d 2069 6620 636f 7673  ovs[:-1] if covs
+0000f930: 5b2d 315d 203d 3d20 7369 7a65 2065 6c73  [-1] == size els
+0000f940: 6520 636f 7673 0a0a 2020 2020 2020 2020  e covs..        
+0000f950: 636f 7620 3d20 7265 6475 6365 286c 696e  cov = reduce(lin
+0000f960: 616c 672e 6b72 6f6e 2c20 636f 7673 290a  alg.kron, covs).
+0000f970: 0a20 2020 2020 2020 2069 6620 7369 676d  .        if sigm
+0000f980: 613a 0a20 2020 2020 2020 2020 2020 2063  a:.            c
+0000f990: 6f76 203d 2063 6f76 202b 2073 6967 6d61  ov = cov + sigma
+0000f9a0: 2a2a 3220 2a20 6e70 2e65 7965 2863 6f76  **2 * np.eye(cov
+0000f9b0: 2e73 6861 7065 5b30 5d29 0a0a 2020 2020  .shape[0])..    
+0000f9c0: 2020 2020 7820 3d20 6d75 6c74 6976 6172      x = multivar
+0000f9d0: 6961 7465 5f6e 6f72 6d61 6c2e 726e 675f  iate_normal.rng_
+0000f9e0: 666e 2872 6e67 3d72 6e67 2c20 6d65 616e  fn(rng=rng, mean
+0000f9f0: 3d6d 752c 2063 6f76 3d63 6f76 2c20 7369  =mu, cov=cov, si
+0000fa00: 7a65 3d73 697a 6529 0a20 2020 2020 2020  ze=size).       
+0000fa10: 2072 6574 7572 6e20 780a 0a0a 6b72 6f6e   return x...kron
+0000fa20: 6563 6b65 726e 6f72 6d61 6c20 3d20 4b72  eckernormal = Kr
+0000fa30: 6f6e 6563 6b65 724e 6f72 6d61 6c52 5628  oneckerNormalRV(
+0000fa40: 290a 0a0a 636c 6173 7320 4b72 6f6e 6563  )...class Kronec
+0000fa50: 6b65 724e 6f72 6d61 6c28 436f 6e74 696e  kerNormal(Contin
+0000fa60: 756f 7573 293a 0a20 2020 2072 2222 220a  uous):.    r""".
+0000fa70: 2020 2020 4d75 6c74 6976 6172 6961 7465      Multivariate
+0000fa80: 206e 6f72 6d61 6c20 6c6f 672d 6c69 6b65   normal log-like
+0000fa90: 6c69 686f 6f64 2077 6974 6820 4b72 6f6e  lihood with Kron
+0000faa0: 6563 6b65 722d 7374 7275 6374 7572 6564  ecker-structured
+0000fab0: 2063 6f76 6172 6961 6e63 652e 0a0a 2020   covariance...  
+0000fac0: 2020 2e2e 206d 6174 683a 3a0a 0a20 2020    .. math::..   
+0000fad0: 2020 2020 6628 7820 5c6d 6964 205c 6d75      f(x \mid \mu
+0000fae0: 2c20 4b29 203d 0a20 2020 2020 2020 2020  , K) =.         
+0000faf0: 2020 5c66 7261 637b 317d 7b28 325c 7069    \frac{1}{(2\pi
+0000fb00: 207c 4b7c 295e 7b31 2f32 7d7d 0a20 2020   |K|)^{1/2}}.   
+0000fb10: 2020 2020 2020 2020 5c65 7870 5c6c 6566          \exp\lef
+0000fb20: 745c 7b20 2d5c 6672 6163 7b31 7d7b 327d  t\{ -\frac{1}{2}
+0000fb30: 2028 782d 5c6d 7529 5e7b 5c70 7269 6d65   (x-\mu)^{\prime
+0000fb40: 7d20 4b5e 7b2d 317d 2028 782d 5c6d 7529  } K^{-1} (x-\mu)
+0000fb50: 205c 7269 6768 745c 7d0a 0a20 2020 203d   \right\}..    =
+0000fb60: 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d  =======  =======
+0000fb70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fb80: 3d3d 3d0a 2020 2020 5375 7070 6f72 7420  ===.    Support 
+0000fb90: 2020 3a6d 6174 683a 6078 205c 696e 205c    :math:`x \in \
+0000fba0: 6d61 7468 6262 7b52 7d5e 4e60 0a20 2020  mathbb{R}^N`.   
+0000fbb0: 204d 6561 6e20 2020 2020 203a 6d61 7468   Mean      :math
+0000fbc0: 3a60 5c6d 7560 0a20 2020 2056 6172 6961  :`\mu`.    Varia
+0000fbd0: 6e63 6520 203a 6d61 7468 3a60 4b20 3d20  nce  :math:`K = 
+0000fbe0: 5c62 6967 6f74 696d 6573 204b 5f69 202b  \bigotimes K_i +
+0000fbf0: 205c 7369 676d 615e 3220 495f 4e60 0a20   \sigma^2 I_N`. 
+0000fc00: 2020 203d 3d3d 3d3d 3d3d 3d20 203d 3d3d     ========  ===
+0000fc10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0000fc20: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
+0000fc30: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+0000fc40: 2d2d 2d2d 2d2d 0a20 2020 206d 7520 3a20  ------.    mu : 
+0000fc50: 7465 6e73 6f72 5f6c 696b 6520 6f66 2066  tensor_like of f
+0000fc60: 6c6f 6174 0a20 2020 2020 2020 2056 6563  loat.        Vec
+0000fc70: 746f 7220 6f66 206d 6561 6e73 2c20 6a75  tor of means, ju
+0000fc80: 7374 2061 7320 696e 2060 4d76 4e6f 726d  st as in `MvNorm
+0000fc90: 616c 602e 0a20 2020 2063 6f76 7320 3a20  al`..    covs : 
+0000fca0: 6c69 7374 206f 6620 6172 7261 7973 0a20  list of arrays. 
+0000fcb0: 2020 2020 2020 2054 6865 2073 6574 206f         The set o
+0000fcc0: 6620 636f 7661 7269 616e 6365 206d 6174  f covariance mat
+0000fcd0: 7269 6365 7320 3a6d 6174 683a 605b 4b5f  rices :math:`[K_
+0000fce0: 312c 204b 5f32 2c20 2e2e 2e5d 6020 746f  1, K_2, ...]` to
+0000fcf0: 2062 650a 2020 2020 2020 2020 4b72 6f6e   be.        Kron
+0000fd00: 6563 6b65 7265 6420 696e 2074 6865 206f  eckered in the o
+0000fd10: 7264 6572 2070 726f 7669 6465 6420 3a6d  rder provided :m
+0000fd20: 6174 683a 605c 6269 676f 7469 6d65 7320  ath:`\bigotimes 
+0000fd30: 4b5f 6960 2e0a 2020 2020 6368 6f6c 7320  K_i`..    chols 
+0000fd40: 3a20 6c69 7374 206f 6620 6172 7261 7973  : list of arrays
+0000fd50: 0a20 2020 2020 2020 2054 6865 2073 6574  .        The set
+0000fd60: 206f 6620 6c6f 7765 7220 6368 6f6c 6573   of lower choles
+0000fd70: 6b79 206d 6174 7269 6365 7320 3a6d 6174  ky matrices :mat
+0000fd80: 683a 605b 4c5f 312c 204c 5f32 2c20 2e2e  h:`[L_1, L_2, ..
+0000fd90: 2e5d 6020 7375 6368 2074 6861 740a 2020  .]` such that.  
+0000fda0: 2020 2020 2020 3a6d 6174 683a 604b 5f69        :math:`K_i
+0000fdb0: 203d 204c 5f69 204c 5f69 2760 2e0a 2020   = L_i L_i'`..  
+0000fdc0: 2020 6576 6473 203a 206c 6973 7420 6f66    evds : list of
+0000fdd0: 2074 7570 6c65 730a 2020 2020 2020 2020   tuples.        
+0000fde0: 5468 6520 7365 7420 6f66 2065 6967 656e  The set of eigen
+0000fdf0: 7661 6c75 652d 7665 6374 6f72 2c20 6569  value-vector, ei
+0000fe00: 6765 6e76 6563 746f 722d 6d61 7472 6978  genvector-matrix
+0000fe10: 2070 6169 7273 0a20 2020 2020 2020 203a   pairs.        :
+0000fe20: 6d61 7468 3a60 5b28 765f 312c 2051 5f31  math:`[(v_1, Q_1
+0000fe30: 292c 2028 765f 322c 2051 5f32 292c 202e  ), (v_2, Q_2), .
+0000fe40: 2e2e 5d60 2073 7563 6820 7468 6174 0a20  ..]` such that. 
+0000fe50: 2020 2020 2020 203a 6d61 7468 3a60 4b5f         :math:`K_
+0000fe60: 6920 3d20 515f 6920 5c74 6578 747b 6469  i = Q_i \text{di
+0000fe70: 6167 7d28 765f 6929 2051 5f69 2760 2e20  ag}(v_i) Q_i'`. 
+0000fe80: 466f 7220 6578 616d 706c 653a 3a0a 0a20  For example::.. 
+0000fe90: 2020 2020 2020 2020 2020 2076 5f69 2c20             v_i, 
+0000fea0: 515f 6920 3d20 7074 2e6e 6c69 6e61 6c67  Q_i = pt.nlinalg
+0000feb0: 2e65 6967 6828 4b5f 6929 0a20 2020 2073  .eigh(K_i).    s
+0000fec0: 6967 6d61 203a 2073 6361 6c61 722c 206f  igma : scalar, o
+0000fed0: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+0000fee0: 5374 616e 6461 7264 2064 6576 6961 7469  Standard deviati
+0000fef0: 6f6e 206f 6620 7468 6520 4761 7573 7369  on of the Gaussi
+0000ff00: 616e 2077 6869 7465 206e 6f69 7365 2e0a  an white noise..
+0000ff10: 0a20 2020 2045 7861 6d70 6c65 730a 2020  .    Examples.  
+0000ff20: 2020 2d2d 2d2d 2d2d 2d2d 0a20 2020 2044    --------.    D
+0000ff30: 6566 696e 6520 6120 6d75 6c74 6976 6172  efine a multivar
+0000ff40: 6961 7465 206e 6f72 6d61 6c20 7661 7269  iate normal vari
+0000ff50: 6162 6c65 2077 6974 6820 6120 636f 7661  able with a cova
+0000ff60: 7269 616e 6365 0a20 2020 203a 6d61 7468  riance.    :math
+0000ff70: 3a60 4b20 3d20 4b5f 3120 5c6f 7469 6d65  :`K = K_1 \otime
+0000ff80: 7320 4b5f 3260 0a0a 2020 2020 2e2e 2063  s K_2`..    .. c
+0000ff90: 6f64 653a 3a20 7079 7468 6f6e 0a0a 2020  ode:: python..  
+0000ffa0: 2020 2020 2020 4b31 203d 206e 702e 6172        K1 = np.ar
+0000ffb0: 7261 7928 5b5b 312e 2c20 302e 355d 2c20  ray([[1., 0.5], 
+0000ffc0: 5b30 2e35 2c20 325d 5d29 0a20 2020 2020  [0.5, 2]]).     
+0000ffd0: 2020 204b 3220 3d20 6e70 2e61 7272 6179     K2 = np.array
+0000ffe0: 285b 5b31 2e2c 2030 2e34 2c20 302e 325d  ([[1., 0.4, 0.2]
+0000fff0: 2c20 5b30 2e34 2c20 322c 2030 2e33 5d2c  , [0.4, 2, 0.3],
+00010000: 205b 302e 322c 2030 2e33 2c20 315d 5d29   [0.2, 0.3, 1]])
+00010010: 0a20 2020 2020 2020 2063 6f76 7320 3d20  .        covs = 
+00010020: 5b4b 312c 204b 325d 0a20 2020 2020 2020  [K1, K2].       
+00010030: 204e 203d 2036 0a20 2020 2020 2020 206d   N = 6.        m
+00010040: 7520 3d20 6e70 2e7a 6572 6f73 284e 290a  u = np.zeros(N).
+00010050: 2020 2020 2020 2020 7769 7468 2070 6d2e          with pm.
+00010060: 4d6f 6465 6c28 2920 6173 206d 6f64 656c  Model() as model
+00010070: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
+00010080: 6c73 203d 2070 6d2e 4b72 6f6e 6563 6b65  ls = pm.Kronecke
+00010090: 724e 6f72 6d61 6c28 2776 616c 7327 2c20  rNormal('vals', 
+000100a0: 6d75 3d6d 752c 2063 6f76 733d 636f 7673  mu=mu, covs=covs
+000100b0: 2c20 7368 6170 653d 4e29 0a0a 2020 2020  , shape=N)..    
+000100c0: 4566 6669 6369 656e 6379 2067 6169 6e73  Efficiency gains
+000100d0: 2061 7265 206d 6164 6520 6279 2063 686f   are made by cho
+000100e0: 6c65 736b 7920 6465 636f 6d70 6f73 696e  lesky decomposin
+000100f0: 6720 3a6d 6174 683a 604b 5f31 6020 616e  g :math:`K_1` an
+00010100: 640a 2020 2020 3a6d 6174 683a 604b 5f32  d.    :math:`K_2
+00010110: 6020 696e 6469 7669 6475 616c 6c79 2072  ` individually r
+00010120: 6174 6865 7220 7468 616e 2074 6865 206c  ather than the l
+00010130: 6172 6765 7220 3a6d 6174 683a 604b 6020  arger :math:`K` 
+00010140: 6d61 7472 6978 2e20 416c 7468 6f75 6768  matrix. Although
+00010150: 0a20 2020 206f 6e6c 7920 7477 6f20 6d61  .    only two ma
+00010160: 7472 6963 6573 203a 6d61 7468 3a60 4b5f  trices :math:`K_
+00010170: 3160 2061 6e64 203a 6d61 7468 3a60 4b5f  1` and :math:`K_
+00010180: 3260 2061 7265 2073 686f 776e 2068 6572  2` are shown her
+00010190: 652c 2061 6e20 6172 6269 7472 6172 790a  e, an arbitrary.
+000101a0: 2020 2020 6e75 6d62 6572 206f 6620 7375      number of su
+000101b0: 626d 6174 7269 6365 7320 6361 6e20 6265  bmatrices can be
+000101c0: 2063 6f6d 6269 6e65 6420 696e 2074 6869   combined in thi
+000101d0: 7320 7761 792e 2043 686f 6c65 736b 7973  s way. Choleskys
+000101e0: 2061 6e64 0a20 2020 2065 6967 656e 6465   and.    eigende
+000101f0: 636f 6d70 6f73 6974 696f 6e73 2063 616e  compositions can
+00010200: 2062 6520 7072 6f76 6964 6564 2069 6e73   be provided ins
+00010210: 7465 6164 0a0a 2020 2020 2e2e 2063 6f64  tead..    .. cod
+00010220: 653a 3a20 7079 7468 6f6e 0a0a 2020 2020  e:: python..    
+00010230: 2020 2020 6368 6f6c 7320 3d20 5b6e 702e      chols = [np.
+00010240: 6c69 6e61 6c67 2e63 686f 6c65 736b 7928  linalg.cholesky(
+00010250: 4b69 2920 666f 7220 4b69 2069 6e20 636f  Ki) for Ki in co
+00010260: 7673 5d0a 2020 2020 2020 2020 6576 6473  vs].        evds
+00010270: 203d 205b 6e70 2e6c 696e 616c 672e 6569   = [np.linalg.ei
+00010280: 6768 284b 6929 2066 6f72 204b 6920 696e  gh(Ki) for Ki in
+00010290: 2063 6f76 735d 0a20 2020 2020 2020 2077   covs].        w
+000102a0: 6974 6820 706d 2e4d 6f64 656c 2829 2061  ith pm.Model() a
+000102b0: 7320 6d6f 6465 6c3a 0a20 2020 2020 2020  s model:.       
+000102c0: 2020 2020 2076 616c 7332 203d 2070 6d2e       vals2 = pm.
+000102d0: 4b72 6f6e 6563 6b65 724e 6f72 6d61 6c28  KroneckerNormal(
+000102e0: 2776 616c 7332 272c 206d 753d 6d75 2c20  'vals2', mu=mu, 
+000102f0: 6368 6f6c 733d 6368 6f6c 732c 2073 6861  chols=chols, sha
+00010300: 7065 3d4e 290a 2020 2020 2020 2020 2020  pe=N).          
+00010310: 2020 2320 6f72 0a20 2020 2020 2020 2020    # or.         
+00010320: 2020 2076 616c 7333 203d 2070 6d2e 4b72     vals3 = pm.Kr
+00010330: 6f6e 6563 6b65 724e 6f72 6d61 6c28 2776  oneckerNormal('v
+00010340: 616c 7333 272c 206d 753d 6d75 2c20 6576  als3', mu=mu, ev
+00010350: 6473 3d65 7664 732c 2073 6861 7065 3d4e  ds=evds, shape=N
+00010360: 290a 0a20 2020 206e 6569 7468 6572 206f  )..    neither o
+00010370: 6620 7768 6963 6820 7769 6c6c 2062 6520  f which will be 
+00010380: 636f 6e76 6572 7465 642e 2044 6961 676f  converted. Diago
+00010390: 6e61 6c20 6e6f 6973 6520 6361 6e20 616c  nal noise can al
+000103a0: 736f 2062 6520 6164 6465 6420 746f 0a20  so be added to. 
+000103b0: 2020 2074 6865 2063 6f76 6172 6961 6e63     the covarianc
+000103c0: 6520 6d61 7472 6978 2c20 3a6d 6174 683a  e matrix, :math:
+000103d0: 604b 203d 204b 5f31 205c 6f74 696d 6573  `K = K_1 \otimes
+000103e0: 204b 5f32 202b 205c 7369 676d 615e 3220   K_2 + \sigma^2 
+000103f0: 495f 4e60 2e0a 2020 2020 4465 7370 6974  I_N`..    Despit
+00010400: 6520 7468 6520 6e6f 6973 6520 7265 6d6f  e the noise remo
+00010410: 7669 6e67 2074 6865 206f 7665 7261 6c6c  ving the overall
+00010420: 204b 726f 6e65 636b 6572 2073 7472 7563   Kronecker struc
+00010430: 7475 7265 206f 6620 7468 6520 6d61 7472  ture of the matr
+00010440: 6978 2c0a 2020 2020 604b 726f 6e65 636b  ix,.    `Kroneck
+00010450: 6572 4e6f 726d 616c 6020 6361 6e20 636f  erNormal` can co
+00010460: 6e74 696e 7565 2074 6f20 6d61 6b65 2065  ntinue to make e
+00010470: 6666 6963 6965 6e74 2063 616c 6375 6c61  fficient calcula
+00010480: 7469 6f6e 7320 6279 0a20 2020 2075 7469  tions by.    uti
+00010490: 6c69 7a69 6e67 2065 6967 656e 6465 636f  lizing eigendeco
+000104a0: 6d70 6f73 6974 6f6e 7320 6f66 2074 6865  mpositons of the
+000104b0: 2073 7562 6d61 7472 6963 6573 2062 6568   submatrices beh
+000104c0: 696e 6420 7468 6520 7363 656e 6573 205b  ind the scenes [
+000104d0: 315d 2e0a 2020 2020 5468 7573 2c0a 0a20  1]..    Thus,.. 
+000104e0: 2020 202e 2e20 636f 6465 3a3a 2070 7974     .. code:: pyt
+000104f0: 686f 6e0a 0a20 2020 2020 2020 2073 6967  hon..        sig
+00010500: 6d61 203d 2030 2e31 0a20 2020 2020 2020  ma = 0.1.       
+00010510: 2077 6974 6820 706d 2e4d 6f64 656c 2829   with pm.Model()
+00010520: 2061 7320 6e6f 6973 655f 6d6f 6465 6c3a   as noise_model:
+00010530: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+00010540: 7320 3d20 706d 2e4b 726f 6e65 636b 6572  s = pm.Kronecker
+00010550: 4e6f 726d 616c 2827 7661 6c73 272c 206d  Normal('vals', m
+00010560: 753d 6d75 2c20 636f 7673 3d63 6f76 732c  u=mu, covs=covs,
+00010570: 2073 6967 6d61 3d73 6967 6d61 2c20 7368   sigma=sigma, sh
+00010580: 6170 653d 4e29 0a20 2020 2020 2020 2020  ape=N).         
+00010590: 2020 2076 616c 7332 203d 2070 6d2e 4b72     vals2 = pm.Kr
+000105a0: 6f6e 6563 6b65 724e 6f72 6d61 6c28 2776  oneckerNormal('v
+000105b0: 616c 7332 272c 206d 753d 6d75 2c20 6368  als2', mu=mu, ch
+000105c0: 6f6c 733d 6368 6f6c 732c 2073 6967 6d61  ols=chols, sigma
+000105d0: 3d73 6967 6d61 2c20 7368 6170 653d 4e29  =sigma, shape=N)
+000105e0: 0a20 2020 2020 2020 2020 2020 2076 616c  .            val
+000105f0: 7333 203d 2070 6d2e 4b72 6f6e 6563 6b65  s3 = pm.Kronecke
+00010600: 724e 6f72 6d61 6c28 2776 616c 7333 272c  rNormal('vals3',
+00010610: 206d 753d 6d75 2c20 6576 6473 3d65 7664   mu=mu, evds=evd
+00010620: 732c 2073 6967 6d61 3d73 6967 6d61 2c20  s, sigma=sigma, 
+00010630: 7368 6170 653d 4e29 0a0a 2020 2020 6172  shape=N)..    ar
+00010640: 6520 6964 656e 7469 6361 6c2c 2077 6974  e identical, wit
+00010650: 6820 6063 6f76 7360 2061 6e64 2060 6368  h `covs` and `ch
+00010660: 6f6c 7360 2065 6163 6820 636f 6e76 6572  ols` each conver
+00010670: 7465 6420 746f 0a20 2020 2065 6967 656e  ted to.    eigen
+00010680: 6465 636f 6d70 6f73 6974 696f 6e73 2e0a  decompositions..
+00010690: 0a20 2020 2052 6566 6572 656e 6365 730a  .    References.
+000106a0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20      ----------. 
+000106b0: 2020 202e 2e20 5b31 5d20 5361 6174 6368     .. [1] Saatch
+000106c0: 692c 2059 2e20 2832 3031 3129 2e20 2253  i, Y. (2011). "S
+000106d0: 6361 6c61 626c 6520 696e 6665 7265 6e63  calable inferenc
+000106e0: 6520 666f 7220 7374 7275 6374 7572 6564  e for structured
+000106f0: 2047 6175 7373 6961 6e20 7072 6f63 6573   Gaussian proces
+00010700: 7320 6d6f 6465 6c73 220a 2020 2020 2222  s models".    ""
+00010710: 220a 2020 2020 7276 5f6f 7020 3d20 6b72  ".    rv_op = kr
+00010720: 6f6e 6563 6b65 726e 6f72 6d61 6c0a 0a20  oneckernormal.. 
+00010730: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00010740: 2020 2020 6465 6620 6469 7374 2863 6c73      def dist(cls
+00010750: 2c20 6d75 2c20 636f 7673 3d4e 6f6e 652c  , mu, covs=None,
+00010760: 2063 686f 6c73 3d4e 6f6e 652c 2065 7664   chols=None, evd
+00010770: 733d 4e6f 6e65 2c20 7369 676d 613d 4e6f  s=None, sigma=No
+00010780: 6e65 2c20 2a61 7267 732c 202a 2a6b 7761  ne, *args, **kwa
+00010790: 7267 7329 3a0a 2020 2020 2020 2020 6966  rgs):.        if
+000107a0: 206c 656e 285b 6920 666f 7220 6920 696e   len([i for i in
+000107b0: 205b 636f 7673 2c20 6368 6f6c 732c 2065   [covs, chols, e
+000107c0: 7664 735d 2069 6620 6920 6973 206e 6f74  vds] if i is not
+000107d0: 204e 6f6e 655d 2920 213d 2031 3a0a 2020   None]) != 1:.  
+000107e0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000107f0: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00010800: 2020 2020 2020 2020 2020 2020 2249 6e63              "Inc
+00010810: 6f6d 7061 7469 626c 6520 7061 7261 6d65  ompatible parame
+00010820: 7465 7269 7a61 7469 6f6e 2e20 5370 6563  terization. Spec
+00010830: 6966 7920 6578 6163 746c 7920 6f6e 6520  ify exactly one 
+00010840: 6f66 2063 6f76 732c 2063 686f 6c73 2c20  of covs, chols, 
+00010850: 6f72 2065 7664 732e 220a 2020 2020 2020  or evds.".      
+00010860: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00010870: 2073 6967 6d61 203d 2073 6967 6d61 2069   sigma = sigma i
+00010880: 6620 7369 676d 6120 656c 7365 2030 0a0a  f sigma else 0..
+00010890: 2020 2020 2020 2020 6966 2063 686f 6c73          if chols
+000108a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+000108b0: 2020 2020 2020 2020 2020 636f 7673 203d            covs =
+000108c0: 205b 6368 6f6c 2e64 6f74 2863 686f 6c2e   [chol.dot(chol.
+000108d0: 5429 2066 6f72 2063 686f 6c20 696e 2063  T) for chol in c
+000108e0: 686f 6c73 5d0a 2020 2020 2020 2020 656c  hols].        el
+000108f0: 6966 2065 7664 7320 6973 206e 6f74 204e  if evds is not N
+00010900: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00010910: 2065 6967 685f 6974 6572 6162 6c65 203d   eigh_iterable =
+00010920: 2065 7664 730a 2020 2020 2020 2020 2020   evds.          
+00010930: 2020 636f 7673 203d 205b 5d0a 2020 2020    covs = [].    
+00010940: 2020 2020 2020 2020 6569 6773 5f73 6570          eigs_sep
+00010950: 2c20 5173 203d 207a 6970 282a 6569 6768  , Qs = zip(*eigh
+00010960: 5f69 7465 7261 626c 6529 2020 2320 556e  _iterable)  # Un
+00010970: 7a69 700a 2020 2020 2020 2020 2020 2020  zip.            
+00010980: 666f 7220 6569 672c 2051 2069 6e20 7a69  for eig, Q in zi
+00010990: 7028 6569 6773 5f73 6570 2c20 5173 293a  p(eigs_sep, Qs):
+000109a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000109b0: 2063 6f76 5f69 203d 2070 742e 646f 7428   cov_i = pt.dot(
+000109c0: 512c 2070 742e 646f 7428 7074 2e64 6961  Q, pt.dot(pt.dia
+000109d0: 6728 6569 6729 2c20 512e 5429 290a 2020  g(eig), Q.T)).  
+000109e0: 2020 2020 2020 2020 2020 2020 2020 636f                co
+000109f0: 7673 2e61 7070 656e 6428 636f 765f 6929  vs.append(cov_i)
+00010a00: 0a0a 2020 2020 2020 2020 6d75 203d 2070  ..        mu = p
+00010a10: 742e 6173 5f74 656e 736f 725f 7661 7269  t.as_tensor_vari
+00010a20: 6162 6c65 286d 7529 0a0a 2020 2020 2020  able(mu)..      
+00010a30: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
+00010a40: 2e64 6973 7428 5b6d 752c 2073 6967 6d61  .dist([mu, sigma
+00010a50: 2c20 2a63 6f76 735d 2c20 2a2a 6b77 6172  , *covs], **kwar
+00010a60: 6773 290a 0a20 2020 2064 6566 206d 6f6d  gs)..    def mom
+00010a70: 656e 7428 7276 2c20 7369 7a65 2c20 6d75  ent(rv, size, mu
+00010a80: 2c20 636f 7673 2c20 6368 6f6c 732c 2065  , covs, chols, e
+00010a90: 7664 7329 3a0a 2020 2020 2020 2020 6d65  vds):.        me
+00010aa0: 616e 203d 206d 750a 2020 2020 2020 2020  an = mu.        
+00010ab0: 6966 206e 6f74 2072 765f 7369 7a65 5f69  if not rv_size_i
+00010ac0: 735f 6e6f 6e65 2873 697a 6529 3a0a 2020  s_none(size):.  
+00010ad0: 2020 2020 2020 2020 2020 6d6f 6d65 6e74            moment
+00010ae0: 5f73 697a 6520 3d20 7074 2e63 6f6e 6361  _size = pt.conca
+00010af0: 7465 6e61 7465 285b 7369 7a65 2c20 6d75  tenate([size, mu
+00010b00: 2e73 6861 7065 5d29 0a20 2020 2020 2020  .shape]).       
+00010b10: 2020 2020 206d 6561 6e20 3d20 7074 2e66       mean = pt.f
+00010b20: 756c 6c28 6d6f 6d65 6e74 5f73 697a 652c  ull(moment_size,
+00010b30: 206d 7529 0a20 2020 2020 2020 2072 6574   mu).        ret
+00010b40: 7572 6e20 6d65 616e 0a0a 2020 2020 6465  urn mean..    de
+00010b50: 6620 6c6f 6770 2876 616c 7565 2c20 6d75  f logp(value, mu
+00010b60: 2c20 7369 676d 612c 202a 636f 7673 293a  , sigma, *covs):
+00010b70: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00010b80: 2020 2020 2043 616c 6375 6c61 7465 206c       Calculate l
+00010b90: 6f67 2d70 726f 6261 6269 6c69 7479 206f  og-probability o
+00010ba0: 6620 4d75 6c74 6976 6172 6961 7465 204e  f Multivariate N
+00010bb0: 6f72 6d61 6c20 6469 7374 7269 6275 7469  ormal distributi
+00010bc0: 6f6e 0a20 2020 2020 2020 2077 6974 6820  on.        with 
+00010bd0: 4b72 6f6e 6563 6b65 722d 7374 7275 6374  Kronecker-struct
+00010be0: 7572 6564 2063 6f76 6172 6961 6e63 6520  ured covariance 
+00010bf0: 6174 2073 7065 6369 6669 6564 2076 616c  at specified val
+00010c00: 7565 2e0a 0a20 2020 2020 2020 2050 6172  ue...        Par
+00010c10: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00010c20: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00010c30: 2020 2076 616c 7565 3a20 6e75 6d65 7269     value: numeri
+00010c40: 630a 2020 2020 2020 2020 2020 2020 5661  c.            Va
+00010c50: 6c75 6520 666f 7220 7768 6963 6820 6c6f  lue for which lo
+00010c60: 672d 7072 6f62 6162 696c 6974 7920 6973  g-probability is
+00010c70: 2063 616c 6375 6c61 7465 642e 0a0a 2020   calculated...  
+00010c80: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
+00010c90: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
+00010ca0: 2020 2020 2020 5465 6e73 6f72 5661 7269        TensorVari
+00010cb0: 6162 6c65 0a20 2020 2020 2020 2022 2222  able.        """
+00010cc0: 0a20 2020 2020 2020 2023 2043 6f6d 7075  .        # Compu
+00010cd0: 7465 7320 7468 6520 7175 6164 7261 7469  tes the quadrati
+00010ce0: 6320 2878 2d6d 7529 5e54 2040 204b 5e2d  c (x-mu)^T @ K^-
+00010cf0: 3120 4020 2878 2d6d 7529 2061 6e64 206c  1 @ (x-mu) and l
+00010d00: 6f67 2864 6574 284b 2929 0a20 2020 2020  og(det(K)).     
+00010d10: 2020 2069 6620 7661 6c75 652e 6e64 696d     if value.ndim
+00010d20: 203e 2032 206f 7220 7661 6c75 652e 6e64   > 2 or value.nd
+00010d30: 696d 203d 3d20 303a 0a20 2020 2020 2020  im == 0:.       
+00010d40: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00010d50: 4572 726f 7228 6622 496e 7661 6c69 6420  Error(f"Invalid 
+00010d60: 6469 6d65 6e73 696f 6e20 666f 7220 7661  dimension for va
+00010d70: 6c75 653a 207b 7661 6c75 652e 6e64 696d  lue: {value.ndim
+00010d80: 7d22 290a 2020 2020 2020 2020 6966 2076  }").        if v
+00010d90: 616c 7565 2e6e 6469 6d20 3d3d 2031 3a0a  alue.ndim == 1:.
+00010da0: 2020 2020 2020 2020 2020 2020 6f6e 6564              oned
+00010db0: 696d 203d 2054 7275 650a 2020 2020 2020  im = True.      
+00010dc0: 2020 2020 2020 7661 6c75 6520 3d20 7661        value = va
+00010dd0: 6c75 655b 4e6f 6e65 2c20 3a5d 0a20 2020  lue[None, :].   
+00010de0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010df0: 2020 2020 2020 206f 6e65 6469 6d20 3d20         onedim = 
+00010e00: 4661 6c73 650a 0a20 2020 2020 2020 2064  False..        d
+00010e10: 656c 7461 203d 2076 616c 7565 202d 206d  elta = value - m
+00010e20: 750a 0a20 2020 2020 2020 2065 6967 685f  u..        eigh_
+00010e30: 6974 6572 6162 6c65 203d 206d 6170 2865  iterable = map(e
+00010e40: 6967 682c 2063 6f76 7329 0a20 2020 2020  igh, covs).     
+00010e50: 2020 2065 6967 735f 7365 702c 2051 7320     eigs_sep, Qs 
+00010e60: 3d20 7a69 7028 2a65 6967 685f 6974 6572  = zip(*eigh_iter
+00010e70: 6162 6c65 2920 2023 2055 6e7a 6970 0a20  able)  # Unzip. 
+00010e80: 2020 2020 2020 2051 7320 3d20 6c69 7374         Qs = list
+00010e90: 286d 6170 2870 742e 6173 5f74 656e 736f  (map(pt.as_tenso
+00010ea0: 725f 7661 7269 6162 6c65 2c20 5173 2929  r_variable, Qs))
+00010eb0: 0a20 2020 2020 2020 2051 5473 203d 206c  .        QTs = l
+00010ec0: 6973 7428 6d61 7028 7074 2e74 7261 6e73  ist(map(pt.trans
+00010ed0: 706f 7365 2c20 5173 2929 0a0a 2020 2020  pose, Qs))..    
+00010ee0: 2020 2020 6569 6773 5f73 6570 203d 206c      eigs_sep = l
+00010ef0: 6973 7428 6d61 7028 7074 2e61 735f 7465  ist(map(pt.as_te
+00010f00: 6e73 6f72 5f76 6172 6961 626c 652c 2065  nsor_variable, e
+00010f10: 6967 735f 7365 7029 290a 2020 2020 2020  igs_sep)).      
+00010f20: 2020 6569 6773 203d 206b 726f 6e5f 6469    eigs = kron_di
+00010f30: 6167 282a 6569 6773 5f73 6570 2920 2023  ag(*eigs_sep)  #
+00010f40: 2043 6f6d 6269 6e65 2073 6570 6172 6174   Combine separat
+00010f50: 6520 6569 6773 0a20 2020 2020 2020 2065  e eigs.        e
+00010f60: 6967 7320 2b3d 2073 6967 6d61 2a2a 320a  igs += sigma**2.
+00010f70: 2020 2020 2020 2020 4e20 3d20 6569 6773          N = eigs
+00010f80: 2e73 6861 7065 5b30 5d0a 0a20 2020 2020  .shape[0]..     
+00010f90: 2020 2073 7172 745f 7175 6164 203d 206b     sqrt_quad = k
+00010fa0: 726f 6e5f 646f 7428 5154 732c 2064 656c  ron_dot(QTs, del
+00010fb0: 7461 2e54 290a 2020 2020 2020 2020 7371  ta.T).        sq
+00010fc0: 7274 5f71 7561 6420 3d20 7371 7274 5f71  rt_quad = sqrt_q
+00010fd0: 7561 6420 2f20 7074 2e73 7172 7428 6569  uad / pt.sqrt(ei
+00010fe0: 6773 5b3a 2c20 4e6f 6e65 5d29 0a20 2020  gs[:, None]).   
+00010ff0: 2020 2020 206c 6f67 6465 7420 3d20 7074       logdet = pt
+00011000: 2e73 756d 2870 742e 6c6f 6728 6569 6773  .sum(pt.log(eigs
+00011010: 2929 0a0a 2020 2020 2020 2020 2320 5371  ))..        # Sq
+00011020: 7561 7265 2065 6163 6820 7361 6d70 6c65  uare each sample
+00011030: 0a20 2020 2020 2020 2071 7561 6420 3d20  .        quad = 
+00011040: 7074 2e62 6174 6368 6564 5f64 6f74 2873  pt.batched_dot(s
+00011050: 7172 745f 7175 6164 2e54 2c20 7371 7274  qrt_quad.T, sqrt
+00011060: 5f71 7561 642e 5429 0a20 2020 2020 2020  _quad.T).       
+00011070: 2069 6620 6f6e 6564 696d 3a0a 2020 2020   if onedim:.    
+00011080: 2020 2020 2020 2020 7175 6164 203d 2071          quad = q
+00011090: 7561 645b 305d 0a0a 2020 2020 2020 2020  uad[0]..        
+000110a0: 6120 3d20 2d28 7175 6164 202b 206c 6f67  a = -(quad + log
+000110b0: 6465 7420 2b20 4e20 2a20 7074 2e6c 6f67  det + N * pt.log
+000110c0: 2832 202a 206e 702e 7069 2929 202f 2032  (2 * np.pi)) / 2
+000110d0: 2e30 0a20 2020 2020 2020 2072 6574 7572  .0.        retur
+000110e0: 6e20 610a 0a0a 636c 6173 7320 4341 5252  n a...class CARR
+000110f0: 5628 5261 6e64 6f6d 5661 7269 6162 6c65  V(RandomVariable
+00011100: 293a 0a20 2020 206e 616d 6520 3d20 2263  ):.    name = "c
+00011110: 6172 220a 2020 2020 6e64 696d 5f73 7570  ar".    ndim_sup
+00011120: 7020 3d20 310a 2020 2020 6e64 696d 735f  p = 1.    ndims_
+00011130: 7061 7261 6d73 203d 205b 312c 2032 2c20  params = [1, 2, 
+00011140: 302c 2030 5d0a 2020 2020 6474 7970 6520  0, 0].    dtype 
+00011150: 3d20 2266 6c6f 6174 5822 0a20 2020 205f  = "floatX".    _
+00011160: 7072 696e 745f 6e61 6d65 203d 2028 2243  print_name = ("C
+00011170: 4152 222c 2022 5c5c 6f70 6572 6174 6f72  AR", "\\operator
+00011180: 6e61 6d65 7b43 4152 7d22 290a 0a20 2020  name{CAR}")..   
+00011190: 2064 6566 206d 616b 655f 6e6f 6465 2873   def make_node(s
+000111a0: 656c 662c 2072 6e67 2c20 7369 7a65 2c20  elf, rng, size, 
+000111b0: 6474 7970 652c 206d 752c 2057 2c20 616c  dtype, mu, W, al
+000111c0: 7068 612c 2074 6175 293a 0a20 2020 2020  pha, tau):.     
+000111d0: 2020 206d 7520 3d20 7074 2e61 735f 7465     mu = pt.as_te
+000111e0: 6e73 6f72 5f76 6172 6961 626c 6528 666c  nsor_variable(fl
+000111f0: 6f61 7458 286d 7529 290a 0a20 2020 2020  oatX(mu))..     
+00011200: 2020 2057 203d 2070 7974 656e 736f 722e     W = pytensor.
+00011210: 7370 6172 7365 2e61 735f 7370 6172 7365  sparse.as_sparse
+00011220: 5f6f 725f 7465 6e73 6f72 5f76 6172 6961  _or_tensor_varia
+00011230: 626c 6528 666c 6f61 7458 2857 2929 0a20  ble(floatX(W)). 
+00011240: 2020 2020 2020 2069 6620 6e6f 7420 572e         if not W.
+00011250: 6e64 696d 203d 3d20 323a 0a20 2020 2020  ndim == 2:.     
+00011260: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00011270: 7565 4572 726f 7228 2257 206d 7573 7420  ueError("W must 
+00011280: 6265 2061 206d 6174 7269 7820 286e 6469  be a matrix (ndi
+00011290: 6d3d 3229 2e22 290a 0a20 2020 2020 2020  m=2).")..       
+000112a0: 2073 7061 7273 6520 3d20 6973 696e 7374   sparse = isinst
+000112b0: 616e 6365 2857 2c20 7079 7465 6e73 6f72  ance(W, pytensor
+000112c0: 2e73 7061 7273 652e 5370 6172 7365 5661  .sparse.SparseVa
+000112d0: 7269 6162 6c65 290a 2020 2020 2020 2020  riable).        
+000112e0: 6d73 6720 3d20 2257 206d 7573 7420 6265  msg = "W must be
+000112f0: 2061 2073 796d 6d65 7472 6963 2061 646a   a symmetric adj
+00011300: 6163 656e 6379 206d 6174 7269 782e 220a  acency matrix.".
+00011310: 2020 2020 2020 2020 6966 2073 7061 7273          if spars
+00011320: 653a 0a20 2020 2020 2020 2020 2020 2061  e:.            a
+00011330: 6273 5f64 6966 6620 3d20 7079 7465 6e73  bs_diff = pytens
+00011340: 6f72 2e73 7061 7273 652e 6261 7369 632e  or.sparse.basic.
+00011350: 6d75 6c28 7079 7465 6e73 6f72 2e73 7061  mul(pytensor.spa
+00011360: 7273 652e 7369 676e 2857 202d 2057 2e54  rse.sign(W - W.T
+00011370: 292c 2057 202d 2057 2e54 290a 2020 2020  ), W - W.T).    
+00011380: 2020 2020 2020 2020 5720 3d20 4173 7365          W = Asse
+00011390: 7274 286d 7367 2928 572c 2070 742e 6973  rt(msg)(W, pt.is
+000113a0: 636c 6f73 6528 7079 7465 6e73 6f72 2e73  close(pytensor.s
+000113b0: 7061 7273 652e 7370 5f73 756d 2861 6273  parse.sp_sum(abs
+000113c0: 5f64 6966 6629 2c20 3029 290a 2020 2020  _diff), 0)).    
+000113d0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+000113e0: 2020 2020 2020 5720 3d20 4173 7365 7274        W = Assert
+000113f0: 286d 7367 2928 572c 2070 742e 616c 6c63  (msg)(W, pt.allc
+00011400: 6c6f 7365 2857 2c20 572e 5429 290a 0a20  lose(W, W.T)).. 
+00011410: 2020 2020 2020 2074 6175 203d 2070 742e         tau = pt.
+00011420: 6173 5f74 656e 736f 725f 7661 7269 6162  as_tensor_variab
+00011430: 6c65 2866 6c6f 6174 5828 7461 7529 290a  le(floatX(tau)).
+00011440: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
+00011450: 7074 2e61 735f 7465 6e73 6f72 5f76 6172  pt.as_tensor_var
+00011460: 6961 626c 6528 666c 6f61 7458 2861 6c70  iable(floatX(alp
+00011470: 6861 2929 0a0a 2020 2020 2020 2020 7265  ha))..        re
+00011480: 7475 726e 2073 7570 6572 2829 2e6d 616b  turn super().mak
+00011490: 655f 6e6f 6465 2872 6e67 2c20 7369 7a65  e_node(rng, size
+000114a0: 2c20 6474 7970 652c 206d 752c 2057 2c20  , dtype, mu, W, 
+000114b0: 616c 7068 612c 2074 6175 290a 0a20 2020  alpha, tau)..   
+000114c0: 2064 6566 205f 696e 6665 725f 7368 6170   def _infer_shap
+000114d0: 6528 7365 6c66 2c20 7369 7a65 2c20 6469  e(self, size, di
+000114e0: 7374 5f70 6172 616d 732c 2070 6172 616d  st_params, param
+000114f0: 5f73 6861 7065 733d 4e6f 6e65 293a 0a20  _shapes=None):. 
+00011500: 2020 2020 2020 2073 6861 7065 203d 2074         shape = t
+00011510: 7570 6c65 2873 697a 6529 202b 2028 6469  uple(size) + (di
+00011520: 7374 5f70 6172 616d 735b 305d 2e73 6861  st_params[0].sha
+00011530: 7065 5b2d 315d 2c29 0a20 2020 2020 2020  pe[-1],).       
+00011540: 2072 6574 7572 6e20 7368 6170 650a 0a20   return shape.. 
+00011550: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+00011560: 2020 2020 6465 6620 726e 675f 666e 2863      def rng_fn(c
+00011570: 6c73 2c20 726e 673a 206e 702e 7261 6e64  ls, rng: np.rand
+00011580: 6f6d 2e52 616e 646f 6d53 7461 7465 2c20  om.RandomState, 
+00011590: 6d75 2c20 572c 2061 6c70 6861 2c20 7461  mu, W, alpha, ta
+000115a0: 752c 2073 697a 6529 3a0a 2020 2020 2020  u, size):.      
+000115b0: 2020 2222 220a 2020 2020 2020 2020 496d    """.        Im
+000115c0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+000115d0: 616c 676f 7269 7468 6d20 6672 6f6d 2070  algorithm from p
+000115e0: 6170 6572 0a20 2020 2020 2020 2048 6176  aper.        Hav
+000115f0: 6172 6420 5275 652c 2032 3030 312e 2022  ard Rue, 2001. "
+00011600: 4661 7374 2073 616d 706c 696e 6720 6f66  Fast sampling of
+00011610: 2047 6175 7373 6961 6e20 4d61 726b 6f76   Gaussian Markov
+00011620: 2072 616e 646f 6d20 6669 656c 6473 2c22   random fields,"
+00011630: 0a20 2020 2020 2020 204a 6f75 726e 616c  .        Journal
+00011640: 206f 6620 7468 6520 526f 7961 6c20 5374   of the Royal St
+00011650: 6174 6973 7469 6361 6c20 536f 6369 6574  atistical Societ
+00011660: 7920 5365 7269 6573 2042 2c20 526f 7961  y Series B, Roya
+00011670: 6c20 5374 6174 6973 7469 6361 6c20 536f  l Statistical So
+00011680: 6369 6574 792c 0a20 2020 2020 2020 2076  ciety,.        v
+00011690: 6f6c 2e20 3633 2832 292c 2070 6167 6573  ol. 63(2), pages
+000116a0: 2033 3235 2d33 3338 2e20 444f 493a 2031   325-338. DOI: 1
+000116b0: 302e 3131 3131 2f31 3436 372d 3938 3638  0.1111/1467-9868
+000116c0: 2e30 3032 3838 0a20 2020 2020 2020 2022  .00288.        "
+000116d0: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+000116e0: 7420 7363 6970 792e 7370 6172 7365 2e69  t scipy.sparse.i
+000116f0: 7373 7061 7273 6528 5729 3a0a 2020 2020  ssparse(W):.    
+00011700: 2020 2020 2020 2020 5720 3d20 7363 6970          W = scip
+00011710: 792e 7370 6172 7365 2e63 7372 5f6d 6174  y.sparse.csr_mat
+00011720: 7269 7828 5729 0a20 2020 2020 2020 2073  rix(W).        s
+00011730: 203d 206e 702e 6173 6172 7261 7928 572e   = np.asarray(W.
+00011740: 7375 6d28 6178 6973 3d30 2929 5b30 5d0a  sum(axis=0))[0].
+00011750: 2020 2020 2020 2020 4420 3d20 7363 6970          D = scip
+00011760: 792e 7370 6172 7365 2e64 6961 6773 2873  y.sparse.diags(s
+00011770: 290a 2020 2020 2020 2020 7461 7520 3d20  ).        tau = 
+00011780: 7363 6970 792e 7370 6172 7365 2e63 7372  scipy.sparse.csr
+00011790: 5f6d 6174 7269 7828 7461 7529 0a20 2020  _matrix(tau).   
+000117a0: 2020 2020 2061 6c70 6861 203d 2073 6369       alpha = sci
+000117b0: 7079 2e73 7061 7273 652e 6373 725f 6d61  py.sparse.csr_ma
+000117c0: 7472 6978 2861 6c70 6861 290a 0a20 2020  trix(alpha)..   
+000117d0: 2020 2020 2051 203d 2074 6175 2e6d 756c       Q = tau.mul
+000117e0: 7469 706c 7928 4420 2d20 616c 7068 612e  tiply(D - alpha.
+000117f0: 6d75 6c74 6970 6c79 2857 2929 0a0a 2020  multiply(W))..  
+00011800: 2020 2020 2020 7065 726d 5f61 7272 6179        perm_array
+00011810: 203d 2073 6369 7079 2e73 7061 7273 652e   = scipy.sparse.
+00011820: 6373 6772 6170 682e 7265 7665 7273 655f  csgraph.reverse_
+00011830: 6375 7468 696c 6c5f 6d63 6b65 6528 512c  cuthill_mckee(Q,
+00011840: 2073 796d 6d65 7472 6963 5f6d 6f64 653d   symmetric_mode=
+00011850: 5472 7565 290a 2020 2020 2020 2020 696e  True).        in
+00011860: 765f 7065 726d 203d 206e 702e 6172 6773  v_perm = np.args
+00011870: 6f72 7428 7065 726d 5f61 7272 6179 290a  ort(perm_array).
+00011880: 0a20 2020 2020 2020 2051 203d 2051 5b70  .        Q = Q[p
+00011890: 6572 6d5f 6172 7261 792c 203a 5d5b 3a2c  erm_array, :][:,
+000118a0: 2070 6572 6d5f 6172 7261 795d 0a0a 2020   perm_array]..  
+000118b0: 2020 2020 2020 5162 203d 2051 2e64 6961        Qb = Q.dia
+000118c0: 676f 6e61 6c28 290a 2020 2020 2020 2020  gonal().        
+000118d0: 7520 3d20 310a 2020 2020 2020 2020 7768  u = 1.        wh
+000118e0: 696c 6520 6e70 2e63 6f75 6e74 5f6e 6f6e  ile np.count_non
+000118f0: 7a65 726f 2851 2e64 6961 676f 6e61 6c28  zero(Q.diagonal(
+00011900: 7529 2920 3e20 303a 0a20 2020 2020 2020  u)) > 0:.       
+00011910: 2020 2020 2051 6220 3d20 6e70 2e76 7374       Qb = np.vst
+00011920: 6163 6b28 286e 702e 7061 6428 512e 6469  ack((np.pad(Q.di
+00011930: 6167 6f6e 616c 2875 292c 2028 752c 2030  agonal(u), (u, 0
+00011940: 292c 2063 6f6e 7374 616e 745f 7661 6c75  ), constant_valu
+00011950: 6573 3d28 302c 2030 2929 2c20 5162 2929  es=(0, 0)), Qb))
+00011960: 0a20 2020 2020 2020 2020 2020 2075 202b  .            u +
+00011970: 3d20 310a 0a20 2020 2020 2020 204c 203d  = 1..        L =
+00011980: 2073 6369 7079 2e6c 696e 616c 672e 6368   scipy.linalg.ch
+00011990: 6f6c 6573 6b79 5f62 616e 6465 6428 5162  olesky_banded(Qb
+000119a0: 2c20 6c6f 7765 723d 4661 6c73 6529 0a0a  , lower=False)..
+000119b0: 2020 2020 2020 2020 7369 7a65 203d 2074          size = t
+000119c0: 7570 6c65 2873 697a 6520 6f72 2028 2929  uple(size or ())
+000119d0: 0a20 2020 2020 2020 2069 6620 7369 7a65  .        if size
+000119e0: 3a0a 2020 2020 2020 2020 2020 2020 6d75  :.            mu
+000119f0: 203d 206e 702e 6272 6f61 6463 6173 745f   = np.broadcast_
+00011a00: 746f 286d 752c 2073 697a 6520 2b20 286d  to(mu, size + (m
+00011a10: 752e 7368 6170 655b 2d31 5d2c 2929 0a20  u.shape[-1],)). 
+00011a20: 2020 2020 2020 207a 203d 2072 6e67 2e6e         z = rng.n
+00011a30: 6f72 6d61 6c28 7369 7a65 3d6d 752e 7368  ormal(size=mu.sh
+00011a40: 6170 6529 0a20 2020 2020 2020 2073 616d  ape).        sam
+00011a50: 706c 6573 203d 206e 702e 656d 7074 7928  ples = np.empty(
+00011a60: 7a2e 7368 6170 6529 0a20 2020 2020 2020  z.shape).       
+00011a70: 2066 6f72 2069 6478 2069 6e20 6e70 2e6e   for idx in np.n
+00011a80: 6469 6e64 6578 286d 752e 7368 6170 655b  dindex(mu.shape[
+00011a90: 3a2d 315d 293a 0a20 2020 2020 2020 2020  :-1]):.         
+00011aa0: 2020 2073 616d 706c 6573 5b69 6478 5d20     samples[idx] 
+00011ab0: 3d20 7363 6970 792e 6c69 6e61 6c67 2e63  = scipy.linalg.c
+00011ac0: 686f 5f73 6f6c 7665 5f62 616e 6465 6428  ho_solve_banded(
+00011ad0: 284c 2c20 4661 6c73 6529 2c20 7a5b 6964  (L, False), z[id
+00011ae0: 785d 2920 2b20 6d75 5b69 6478 5d5b 7065  x]) + mu[idx][pe
+00011af0: 726d 5f61 7272 6179 5d0a 2020 2020 2020  rm_array].      
+00011b00: 2020 7361 6d70 6c65 7320 3d20 7361 6d70    samples = samp
+00011b10: 6c65 735b 2e2e 2e2c 2069 6e76 5f70 6572  les[..., inv_per
+00011b20: 6d5d 0a20 2020 2020 2020 2072 6574 7572  m].        retur
+00011b30: 6e20 7361 6d70 6c65 730a 0a0a 6361 7220  n samples...car 
+00011b40: 3d20 4341 5252 5628 290a 0a0a 636c 6173  = CARRV()...clas
+00011b50: 7320 4341 5228 436f 6e74 696e 756f 7573  s CAR(Continuous
+00011b60: 293a 0a20 2020 2072 2222 220a 2020 2020  ):.    r""".    
+00011b70: 4c69 6b65 6c69 686f 6f64 2066 6f72 2061  Likelihood for a
+00011b80: 2063 6f6e 6469 7469 6f6e 616c 2061 7574   conditional aut
+00011b90: 6f72 6567 7265 7373 696f 6e2e 2054 6869  oregression. Thi
+00011ba0: 7320 6973 2061 2073 7065 6369 616c 2063  s is a special c
+00011bb0: 6173 6520 6f66 2074 6865 0a20 2020 206d  ase of the.    m
+00011bc0: 756c 7469 7661 7269 6174 6520 6e6f 726d  ultivariate norm
+00011bd0: 616c 2077 6974 6820 616e 2061 646a 6163  al with an adjac
+00011be0: 656e 6379 2d73 7472 7563 7475 7265 6420  ency-structured 
+00011bf0: 636f 7661 7269 616e 6365 206d 6174 7269  covariance matri
+00011c00: 782e 0a0a 2020 2020 2e2e 206d 6174 683a  x...    .. math:
+00011c10: 3a0a 0a20 2020 2020 2020 6628 7820 5c6d  :..       f(x \m
+00011c20: 6964 2057 2c20 5c61 6c70 6861 2c20 5c74  id W, \alpha, \t
+00011c30: 6175 2920 3d0a 2020 2020 2020 2020 2020  au) =.          
+00011c40: 205c 6672 6163 7b7c 547c 5e7b 312f 327d   \frac{|T|^{1/2}
+00011c50: 7d7b 2832 5c70 6929 5e7b 6b2f 327d 7d0a  }{(2\pi)^{k/2}}.
+00011c60: 2020 2020 2020 2020 2020 205c 6578 705c             \exp\
+00011c70: 6c65 6674 5c7b 202d 5c66 7261 637b 317d  left\{ -\frac{1}
+00011c80: 7b32 7d20 2878 2d5c 6d75 295e 7b5c 7072  {2} (x-\mu)^{\pr
+00011c90: 696d 657d 2054 5e7b 2d31 7d20 2878 2d5c  ime} T^{-1} (x-\
+00011ca0: 6d75 2920 5c72 6967 6874 5c7d 0a0a 2020  mu) \right\}..  
+00011cb0: 2020 7768 6572 6520 3a6d 6174 683a 6054    where :math:`T
+00011cc0: 203d 2028 5c74 6175 2044 2849 2d5c 616c   = (\tau D(I-\al
+00011cd0: 7068 6120 5729 295e 7b2d 317d 6020 616e  pha W))^{-1}` an
+00011ce0: 6420 3a6d 6174 683a 6044 203d 2064 6961  d :math:`D = dia
+00011cf0: 6728 5c73 756d 5f69 2057 5f7b 696a 7d29  g(\sum_i W_{ij})
+00011d00: 602e 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d  `...    ========
+00011d10: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    ==============
+00011d20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a20 2020  ============.   
+00011d30: 2053 7570 706f 7274 2020 203a 6d61 7468   Support   :math
+00011d40: 3a60 7820 5c69 6e20 5c6d 6174 6862 627b  :`x \in \mathbb{
+00011d50: 527d 5e6b 600a 2020 2020 4d65 616e 2020  R}^k`.    Mean  
+00011d60: 2020 2020 3a6d 6174 683a 605c 6d75 205c      :math:`\mu \
+00011d70: 696e 205c 6d61 7468 6262 7b52 7d5e 6b60  in \mathbb{R}^k`
+00011d80: 0a20 2020 2056 6172 6961 6e63 6520 203a  .    Variance  :
+00011d90: 6d61 7468 3a60 285c 7461 7520 4428 492d  math:`(\tau D(I-
+00011da0: 5c61 6c70 6861 2057 2929 5e7b 2d31 7d60  \alpha W))^{-1}`
+00011db0: 0a20 2020 203d 3d3d 3d3d 3d3d 3d20 203d  .    ========  =
+00011dc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00011dd0: 3d3d 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050  =========..    P
+00011de0: 6172 616d 6574 6572 730a 2020 2020 2d2d  arameters.    --
+00011df0: 2d2d 2d2d 2d2d 2d2d 0a20 2020 206d 7520  --------.    mu 
+00011e00: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+00011e10: 2066 6c6f 6174 0a20 2020 2020 2020 2052   float.        R
+00011e20: 6561 6c2d 7661 6c75 6564 206d 6561 6e20  eal-valued mean 
+00011e30: 7665 6374 6f72 0a20 2020 2057 203a 2028  vector.    W : (
+00011e40: 4d2c 204d 2920 7465 6e73 6f72 5f6c 696b  M, M) tensor_lik
+00011e50: 6520 6f66 2069 6e74 0a20 2020 2020 2020  e of int.       
+00011e60: 2053 796d 6d65 7472 6963 2061 646a 6163   Symmetric adjac
+00011e70: 656e 6379 206d 6174 7269 7820 6f66 2031  ency matrix of 1
+00011e80: 7320 616e 6420 3073 2069 6e64 6963 6174  s and 0s indicat
+00011e90: 696e 670a 2020 2020 2020 2020 6164 6a61  ing.        adja
+00011ea0: 6365 6e63 7920 6265 7477 6565 6e20 656c  cency between el
+00011eb0: 656d 656e 7473 2e20 4966 2070 6f73 7369  ements. If possi
+00011ec0: 626c 652c 202a 572a 2069 7320 636f 6e76  ble, *W* is conv
+00011ed0: 6572 7465 640a 2020 2020 2020 2020 746f  erted.        to
+00011ee0: 2061 2073 7061 7273 6520 6d61 7472 6978   a sparse matrix
+00011ef0: 2c20 6661 6c6c 696e 6720 6261 636b 2074  , falling back t
+00011f00: 6f20 6120 6465 6e73 6520 7661 7269 6162  o a dense variab
+00011f10: 6c65 2e0a 2020 2020 2020 2020 3a66 756e  le..        :fun
+00011f20: 633a 607e 7079 7465 6e73 6f72 2e73 7061  c:`~pytensor.spa
+00011f30: 7273 652e 6261 7369 632e 6173 5f73 7061  rse.basic.as_spa
+00011f40: 7273 655f 6f72 5f74 656e 736f 725f 7661  rse_or_tensor_va
+00011f50: 7269 6162 6c65 6020 6973 0a20 2020 2020  riable` is.     
+00011f60: 2020 2075 7365 6420 666f 7220 7468 6973     used for this
+00011f70: 2073 7061 7273 6520 6f72 2074 656e 736f   sparse or tenso
+00011f80: 7276 6172 6961 626c 6520 636f 6e76 6572  rvariable conver
+00011f90: 7369 6f6e 2e0a 2020 2020 616c 7068 6120  sion..    alpha 
+00011fa0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+00011fb0: 2066 6c6f 6174 0a20 2020 2020 2020 2041   float.        A
+00011fc0: 7574 6f72 6567 7265 7373 696f 6e20 7061  utoregression pa
+00011fd0: 7261 6d65 7465 7220 7461 6b69 6e67 2076  rameter taking v
+00011fe0: 616c 7565 7320 6265 7477 6565 6e20 2d31  alues between -1
+00011ff0: 2061 6e64 2031 2e20 5661 6c75 6573 2063   and 1. Values c
+00012000: 6c6f 7365 7220 746f 2030 2069 6e64 6963  loser to 0 indic
+00012010: 6174 6520 7765 616b 6572 0a20 2020 2020  ate weaker.     
+00012020: 2020 2063 6f72 7265 6c61 7469 6f6e 2061     correlation a
+00012030: 6e64 2076 616c 7565 7320 636c 6f73 6572  nd values closer
+00012040: 2074 6f20 3120 696e 6469 6361 7465 2068   to 1 indicate h
+00012050: 6967 6865 7220 6175 746f 636f 7272 656c  igher autocorrel
+00012060: 6174 696f 6e2e 2046 6f72 206d 6f73 7420  ation. For most 
+00012070: 7573 6520 6361 7365 732c 2074 6865 0a20  use cases, the. 
+00012080: 2020 2020 2020 2073 7570 706f 7274 206f         support o
+00012090: 6620 616c 7068 6120 7368 6f75 6c64 2062  f alpha should b
+000120a0: 6520 7265 7374 7269 6374 6564 2074 6f20  e restricted to 
+000120b0: 2830 2c20 3129 2e0a 2020 2020 7461 7520  (0, 1)..    tau 
+000120c0: 3a20 7465 6e73 6f72 5f6c 696b 6520 6f66  : tensor_like of
+000120d0: 2066 6c6f 6174 0a20 2020 2020 2020 2050   float.        P
+000120e0: 6f73 6974 6976 6520 7072 6563 6973 696f  ositive precisio
+000120f0: 6e20 7661 7269 6162 6c65 2063 6f6e 7472  n variable contr
+00012100: 6f6c 6c69 6e67 2074 6865 2073 6361 6c65  olling the scale
+00012110: 206f 6620 7468 6520 756e 6465 726c 7969   of the underlyi
+00012120: 6e67 206e 6f72 6d61 6c20 7661 7269 6174  ng normal variat
+00012130: 6573 2e0a 0a20 2020 2052 6566 6572 656e  es...    Referen
+00012140: 6365 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ces.    --------
+00012150: 2d2d 0a20 2020 202e 2e20 204a 696e 2c20  --.    ..  Jin, 
+00012160: 582e 2c20 4361 726c 696e 2c20 422e 2c20  X., Carlin, B., 
+00012170: 4261 6e65 726a 6565 2c20 532e 0a20 2020  Banerjee, S..   
+00012180: 2020 2020 2022 4765 6e65 7261 6c69 7a65       "Generalize
+00012190: 6420 4869 6572 6172 6368 6963 616c 204d  d Hierarchical M
+000121a0: 756c 7469 7661 7269 6174 6520 4341 5220  ultivariate CAR 
+000121b0: 4d6f 6465 6c73 2066 6f72 2041 7265 616c  Models for Areal
+000121c0: 2044 6174 6122 0a20 2020 2020 2020 2042   Data".        B
+000121d0: 696f 6d65 7472 6963 732c 2056 6f6c 2e20  iometrics, Vol. 
+000121e0: 3631 2c20 4e6f 2e20 3420 2844 6563 2e2c  61, No. 4 (Dec.,
+000121f0: 2032 3030 3529 2c20 7070 2e20 3935 302d   2005), pp. 950-
+00012200: 3936 310a 2020 2020 2222 220a 2020 2020  961.    """.    
+00012210: 7276 5f6f 7020 3d20 6361 720a 0a20 2020  rv_op = car..   
+00012220: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
+00012230: 2020 6465 6620 6469 7374 2863 6c73 2c20    def dist(cls, 
+00012240: 6d75 2c20 572c 2061 6c70 6861 2c20 7461  mu, W, alpha, ta
+00012250: 752c 202a 6172 6773 2c20 2a2a 6b77 6172  u, *args, **kwar
+00012260: 6773 293a 0a20 2020 2020 2020 2072 6574  gs):.        ret
+00012270: 7572 6e20 7375 7065 7228 292e 6469 7374  urn super().dist
+00012280: 285b 6d75 2c20 572c 2061 6c70 6861 2c20  ([mu, W, alpha, 
+00012290: 7461 755d 2c20 2a2a 6b77 6172 6773 290a  tau], **kwargs).
+000122a0: 0a20 2020 2064 6566 206d 6f6d 656e 7428  .    def moment(
+000122b0: 7276 2c20 7369 7a65 2c20 6d75 2c20 572c  rv, size, mu, W,
+000122c0: 2061 6c70 6861 2c20 7461 7529 3a0a 2020   alpha, tau):.  
+000122d0: 2020 2020 2020 7265 7475 726e 2070 742e        return pt.
+000122e0: 6675 6c6c 5f6c 696b 6528 7276 2c20 6d75  full_like(rv, mu
+000122f0: 290a 0a20 2020 2064 6566 206c 6f67 7028  )..    def logp(
+00012300: 7661 6c75 652c 206d 752c 2057 2c20 616c  value, mu, W, al
+00012310: 7068 612c 2074 6175 293a 0a20 2020 2020  pha, tau):.     
+00012320: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
+00012330: 616c 6375 6c61 7465 206c 6f67 2d70 726f  alculate log-pro
+00012340: 6261 6269 6c69 7479 206f 6620 6120 4341  bability of a CA
+00012350: 522d 6469 7374 7269 6275 7465 6420 7665  R-distributed ve
+00012360: 6374 6f72 0a20 2020 2020 2020 2061 7420  ctor.        at 
+00012370: 7370 6563 6966 6965 6420 7661 6c75 652e  specified value.
+00012380: 2054 6869 7320 6c6f 6720 7072 6f62 6162   This log probab
+00012390: 696c 6974 7920 6675 6e63 7469 6f6e 2064  ility function d
+000123a0: 6966 6665 7273 2066 726f 6d0a 2020 2020  iffers from.    
+000123b0: 2020 2020 7468 6520 7472 7565 2043 4152      the true CAR
+000123c0: 206c 6f67 2064 656e 7369 7479 2028 414b   log density (AK
+000123d0: 4120 6120 6d75 6c74 6976 6172 6961 7465  A a multivariate
+000123e0: 206e 6f72 6d61 6c20 7769 7468 2043 4152   normal with CAR
+000123f0: 2d73 7472 7563 7475 7265 640a 2020 2020  -structured.    
+00012400: 2020 2020 636f 7661 7269 616e 6365 206d      covariance m
+00012410: 6174 7269 7829 2062 7920 616e 2061 6464  atrix) by an add
+00012420: 6974 6976 6520 636f 6e73 7461 6e74 2e0a  itive constant..
+00012430: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00012440: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00012450: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 2076  ------.        v
+00012460: 616c 7565 3a20 6172 7261 790a 2020 2020  alue: array.    
+00012470: 2020 2020 2020 2020 5661 6c75 6520 666f          Value fo
+00012480: 7220 7768 6963 6820 6c6f 672d 7072 6f62  r which log-prob
+00012490: 6162 696c 6974 7920 6973 2063 616c 6375  ability is calcu
+000124a0: 6c61 7465 642e 0a0a 2020 2020 2020 2020  lated...        
+000124b0: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+000124c0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+000124d0: 5465 6e73 6f72 5661 7269 6162 6c65 0a20  TensorVariable. 
+000124e0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
+000124f0: 2020 2020 7370 6172 7365 203d 2069 7369      sparse = isi
+00012500: 6e73 7461 6e63 6528 572c 2028 7079 7465  nstance(W, (pyte
+00012510: 6e73 6f72 2e73 7061 7273 652e 5370 6172  nsor.sparse.Spar
+00012520: 7365 436f 6e73 7461 6e74 2c20 7079 7465  seConstant, pyte
+00012530: 6e73 6f72 2e73 7061 7273 652e 5370 6172  nsor.sparse.Spar
+00012540: 7365 5661 7269 6162 6c65 2929 0a0a 2020  seVariable))..  
+00012550: 2020 2020 2020 6966 2073 7061 7273 653a        if sparse:
+00012560: 0a20 2020 2020 2020 2020 2020 2044 203d  .            D =
+00012570: 2073 705f 7375 6d28 572c 2061 7869 733d   sp_sum(W, axis=
+00012580: 3029 0a20 2020 2020 2020 2020 2020 2044  0).            D
+00012590: 696e 765f 7371 7274 203d 2070 742e 6469  inv_sqrt = pt.di
+000125a0: 6167 2831 202f 2070 742e 7371 7274 2844  ag(1 / pt.sqrt(D
+000125b0: 2929 0a20 2020 2020 2020 2020 2020 2044  )).            D
+000125c0: 5744 203d 2070 742e 646f 7428 7079 7465  WD = pt.dot(pyte
+000125d0: 6e73 6f72 2e73 7061 7273 652e 646f 7428  nsor.sparse.dot(
+000125e0: 4469 6e76 5f73 7172 742c 2057 292c 2044  Dinv_sqrt, W), D
+000125f0: 696e 765f 7371 7274 290a 2020 2020 2020  inv_sqrt).      
+00012600: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012610: 2020 2020 4420 3d20 572e 7375 6d28 6178      D = W.sum(ax
+00012620: 6973 3d30 290a 2020 2020 2020 2020 2020  is=0).          
+00012630: 2020 4469 6e76 5f73 7172 7420 3d20 7074    Dinv_sqrt = pt
+00012640: 2e64 6961 6728 3120 2f20 7074 2e73 7172  .diag(1 / pt.sqr
+00012650: 7428 4429 290a 2020 2020 2020 2020 2020  t(D)).          
+00012660: 2020 4457 4420 3d20 7074 2e64 6f74 2870    DWD = pt.dot(p
+00012670: 742e 646f 7428 4469 6e76 5f73 7172 742c  t.dot(Dinv_sqrt,
+00012680: 2057 292c 2044 696e 765f 7371 7274 290a   W), Dinv_sqrt).
+00012690: 2020 2020 2020 2020 6c61 6d20 3d20 7074          lam = pt
+000126a0: 2e73 6c69 6e61 6c67 2e65 6967 7661 6c73  .slinalg.eigvals
+000126b0: 6828 4457 442c 2070 742e 6579 6528 4457  h(DWD, pt.eye(DW
+000126c0: 442e 7368 6170 655b 305d 2929 0a0a 2020  D.shape[0]))..  
+000126d0: 2020 2020 2020 642c 205f 203d 2057 2e73        d, _ = W.s
+000126e0: 6861 7065 0a0a 2020 2020 2020 2020 6966  hape..        if
+000126f0: 2076 616c 7565 2e6e 6469 6d20 3d3d 2031   value.ndim == 1
+00012700: 3a0a 2020 2020 2020 2020 2020 2020 7661  :.            va
+00012710: 6c75 6520 3d20 7661 6c75 655b 4e6f 6e65  lue = value[None
+00012720: 2c20 3a5d 0a0a 2020 2020 2020 2020 6c6f  , :]..        lo
+00012730: 6774 6175 203d 2064 202a 2070 742e 6c6f  gtau = d * pt.lo
+00012740: 6728 7461 7529 2e73 756d 2829 0a20 2020  g(tau).sum().   
+00012750: 2020 2020 206c 6f67 6465 7420 3d20 7074       logdet = pt
+00012760: 2e6c 6f67 2831 202d 2061 6c70 6861 2e54  .log(1 - alpha.T
+00012770: 202a 206c 616d 5b3a 2c20 4e6f 6e65 5d29   * lam[:, None])
+00012780: 2e73 756d 2829 0a20 2020 2020 2020 2064  .sum().        d
+00012790: 656c 7461 203d 2076 616c 7565 202d 206d  elta = value - m
+000127a0: 750a 0a20 2020 2020 2020 2069 6620 7370  u..        if sp
+000127b0: 6172 7365 3a0a 2020 2020 2020 2020 2020  arse:.          
+000127c0: 2020 5764 656c 7461 203d 2070 7974 656e    Wdelta = pyten
+000127d0: 736f 722e 7370 6172 7365 2e64 6f74 2864  sor.sparse.dot(d
+000127e0: 656c 7461 2c20 5729 0a20 2020 2020 2020  elta, W).       
+000127f0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00012800: 2020 2057 6465 6c74 6120 3d20 7074 2e64     Wdelta = pt.d
+00012810: 6f74 2864 656c 7461 2c20 5729 0a0a 2020  ot(delta, W)..  
+00012820: 2020 2020 2020 7461 755f 646f 745f 6465        tau_dot_de
+00012830: 6c74 6120 3d20 445b 4e6f 6e65 2c20 3a5d  lta = D[None, :]
+00012840: 202a 2064 656c 7461 202d 2061 6c70 6861   * delta - alpha
+00012850: 202a 2057 6465 6c74 610a 2020 2020 2020   * Wdelta.      
+00012860: 2020 6c6f 6771 7561 6420 3d20 2874 6175    logquad = (tau
+00012870: 202a 2064 656c 7461 202a 2074 6175 5f64   * delta * tau_d
+00012880: 6f74 5f64 656c 7461 292e 7375 6d28 6178  ot_delta).sum(ax
+00012890: 6973 3d2d 3129 0a20 2020 2020 2020 2072  is=-1).        r
+000128a0: 6574 7572 6e20 6368 6563 6b5f 7061 7261  eturn check_para
+000128b0: 6d65 7465 7273 280a 2020 2020 2020 2020  meters(.        
+000128c0: 2020 2020 302e 3520 2a20 286c 6f67 7461      0.5 * (logta
+000128d0: 7520 2b20 6c6f 6764 6574 202d 206c 6f67  u + logdet - log
+000128e0: 7175 6164 292c 0a20 2020 2020 2020 2020  quad),.         
+000128f0: 2020 202d 3120 3c3d 2061 6c70 6861 2c0a     -1 <= alpha,.
+00012900: 2020 2020 2020 2020 2020 2020 616c 7068              alph
+00012910: 6120 3c3d 2031 2c0a 2020 2020 2020 2020  a <= 1,.        
+00012920: 2020 2020 7461 7520 3e20 302c 0a20 2020      tau > 0,.   
+00012930: 2020 2020 2020 2020 206d 7367 3d22 2d31           msg="-1
+00012940: 203c 3d20 616c 7068 6120 3c3d 2031 2c20   <= alpha <= 1, 
+00012950: 7461 7520 3e20 3022 2c0a 2020 2020 2020  tau > 0",.      
+00012960: 2020 290a 0a0a 636c 6173 7320 5374 6963    )...class Stic
+00012970: 6b42 7265 616b 696e 6757 6569 6768 7473  kBreakingWeights
+00012980: 5256 2852 616e 646f 6d56 6172 6961 626c  RV(RandomVariabl
+00012990: 6529 3a0a 2020 2020 6e61 6d65 203d 2022  e):.    name = "
+000129a0: 7374 6963 6b5f 6272 6561 6b69 6e67 5f77  stick_breaking_w
+000129b0: 6569 6768 7473 220a 2020 2020 6e64 696d  eights".    ndim
+000129c0: 5f73 7570 7020 3d20 310a 2020 2020 6e64  _supp = 1.    nd
+000129d0: 696d 735f 7061 7261 6d73 203d 205b 302c  ims_params = [0,
+000129e0: 2030 5d0a 2020 2020 6474 7970 6520 3d20   0].    dtype = 
+000129f0: 2266 6c6f 6174 5822 0a20 2020 205f 7072  "floatX".    _pr
+00012a00: 696e 745f 6e61 6d65 203d 2028 2253 7469  int_name = ("Sti
+00012a10: 636b 4272 6561 6b69 6e67 5765 6967 6874  ckBreakingWeight
+00012a20: 7322 2c20 225c 5c6f 7065 7261 746f 726e  s", "\\operatorn
+00012a30: 616d 657b 5374 6963 6b42 7265 616b 696e  ame{StickBreakin
+00012a40: 6757 6569 6768 7473 7d22 290a 0a20 2020  gWeights}")..   
+00012a50: 2064 6566 206d 616b 655f 6e6f 6465 2873   def make_node(s
+00012a60: 656c 662c 2072 6e67 2c20 7369 7a65 2c20  elf, rng, size, 
+00012a70: 6474 7970 652c 2061 6c70 6861 2c20 4b29  dtype, alpha, K)
+00012a80: 3a0a 2020 2020 2020 2020 616c 7068 6120  :.        alpha 
+00012a90: 3d20 7074 2e61 735f 7465 6e73 6f72 5f76  = pt.as_tensor_v
+00012aa0: 6172 6961 626c 6528 616c 7068 6129 0a20  ariable(alpha). 
+00012ab0: 2020 2020 2020 204b 203d 2070 742e 6173         K = pt.as
+00012ac0: 5f74 656e 736f 725f 7661 7269 6162 6c65  _tensor_variable
+00012ad0: 2869 6e74 5828 4b29 290a 0a20 2020 2020  (intX(K))..     
+00012ae0: 2020 2069 6620 4b2e 6e64 696d 203e 2030     if K.ndim > 0
+00012af0: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00012b00: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00012b10: 4b20 6d75 7374 2062 6520 6120 7363 616c  K must be a scal
+00012b20: 6172 2e22 290a 0a20 2020 2020 2020 2072  ar.")..        r
+00012b30: 6574 7572 6e20 7375 7065 7228 292e 6d61  eturn super().ma
+00012b40: 6b65 5f6e 6f64 6528 726e 672c 2073 697a  ke_node(rng, siz
+00012b50: 652c 2064 7479 7065 2c20 616c 7068 612c  e, dtype, alpha,
+00012b60: 204b 290a 0a20 2020 2064 6566 205f 7375   K)..    def _su
+00012b70: 7070 5f73 6861 7065 5f66 726f 6d5f 7061  pp_shape_from_pa
+00012b80: 7261 6d73 2873 656c 662c 2064 6973 745f  rams(self, dist_
+00012b90: 7061 7261 6d73 2c20 2a2a 6b77 6172 6773  params, **kwargs
+00012ba0: 293a 0a20 2020 2020 2020 204b 203d 2064  ):.        K = d
+00012bb0: 6973 745f 7061 7261 6d73 5b31 5d0a 2020  ist_params[1].  
+00012bc0: 2020 2020 2020 7265 7475 726e 2028 4b20        return (K 
+00012bd0: 2b20 312c 290a 0a20 2020 2040 636c 6173  + 1,)..    @clas
+00012be0: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00012bf0: 726e 675f 666e 2863 6c73 2c20 726e 672c  rng_fn(cls, rng,
+00012c00: 2061 6c70 6861 2c20 4b2c 2073 697a 6529   alpha, K, size)
+00012c10: 3a0a 2020 2020 2020 2020 6966 204b 203c  :.        if K <
+00012c20: 2030 3a0a 2020 2020 2020 2020 2020 2020   0:.            
+00012c30: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00012c40: 2822 4b20 6e65 6564 7320 746f 2062 6520  ("K needs to be 
+00012c50: 706f 7369 7469 7665 2e22 290a 0a20 2020  positive.")..   
+00012c60: 2020 2020 2073 697a 6520 3d20 746f 5f74       size = to_t
+00012c70: 7570 6c65 2873 697a 6529 2069 6620 7369  uple(size) if si
+00012c80: 7a65 2069 7320 6e6f 7420 4e6f 6e65 2065  ze is not None e
+00012c90: 6c73 6520 616c 7068 612e 7368 6170 650a  lse alpha.shape.
+00012ca0: 2020 2020 2020 2020 7369 7a65 203d 2073          size = s
+00012cb0: 697a 6520 2b20 284b 2c29 0a20 2020 2020  ize + (K,).     
+00012cc0: 2020 2061 6c70 6861 203d 2061 6c70 6861     alpha = alpha
+00012cd0: 5b2e 2e2e 2c20 6e70 2e6e 6577 6178 6973  [..., np.newaxis
+00012ce0: 5d0a 0a20 2020 2020 2020 2062 6574 6173  ]..        betas
+00012cf0: 203d 2072 6e67 2e62 6574 6128 312c 2061   = rng.beta(1, a
+00012d00: 6c70 6861 2c20 7369 7a65 3d73 697a 6529  lpha, size=size)
+00012d10: 0a0a 2020 2020 2020 2020 7374 6963 6b73  ..        sticks
+00012d20: 203d 206e 702e 636f 6e63 6174 656e 6174   = np.concatenat
+00012d30: 6528 0a20 2020 2020 2020 2020 2020 2028  e(.            (
+00012d40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012d50: 206e 702e 6f6e 6573 2873 6861 7065 3d28   np.ones(shape=(
+00012d60: 7369 7a65 5b3a 2d31 5d20 2b20 2831 2c29  size[:-1] + (1,)
+00012d70: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
+00012d80: 2020 2020 6e70 2e63 756d 7072 6f64 2831      np.cumprod(1
+00012d90: 202d 2062 6574 6173 5b2e 2e2e 2c20 3a2d   - betas[..., :-
+00012da0: 315d 2c20 6178 6973 3d2d 3129 2c0a 2020  1], axis=-1),.  
+00012db0: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
+00012dc0: 2020 2020 2020 2020 2061 7869 733d 2d31           axis=-1
+00012dd0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00012de0: 2020 2020 2077 6569 6768 7473 203d 2073       weights = s
+00012df0: 7469 636b 7320 2a20 6265 7461 730a 2020  ticks * betas.  
+00012e00: 2020 2020 2020 7765 6967 6874 7320 3d20        weights = 
+00012e10: 6e70 2e63 6f6e 6361 7465 6e61 7465 280a  np.concatenate(.
+00012e20: 2020 2020 2020 2020 2020 2020 2877 6569              (wei
+00012e30: 6768 7473 2c20 3120 2d20 7765 6967 6874  ghts, 1 - weight
+00012e40: 732e 7375 6d28 6178 6973 3d2d 3129 5b2e  s.sum(axis=-1)[.
+00012e50: 2e2e 2c20 6e70 2e6e 6577 6178 6973 5d29  .., np.newaxis])
+00012e60: 2c0a 2020 2020 2020 2020 2020 2020 6178  ,.            ax
+00012e70: 6973 3d2d 312c 0a20 2020 2020 2020 2029  is=-1,.        )
+00012e80: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00012e90: 2077 6569 6768 7473 0a0a 0a73 7469 636b   weights...stick
+00012ea0: 6272 6561 6b69 6e67 7765 6967 6874 7320  breakingweights 
+00012eb0: 3d20 5374 6963 6b42 7265 616b 696e 6757  = StickBreakingW
+00012ec0: 6569 6768 7473 5256 2829 0a0a 0a63 6c61  eightsRV()...cla
+00012ed0: 7373 2053 7469 636b 4272 6561 6b69 6e67  ss StickBreaking
+00012ee0: 5765 6967 6874 7328 5369 6d70 6c65 7843  Weights(SimplexC
+00012ef0: 6f6e 7469 6e75 6f75 7329 3a0a 2020 2020  ontinuous):.    
+00012f00: 7222 2222 0a20 2020 204c 696b 656c 6968  r""".    Likelih
+00012f10: 6f6f 6420 6f66 2074 7275 6e63 6174 6564  ood of truncated
+00012f20: 2073 7469 636b 2d62 7265 616b 696e 6720   stick-breaking 
+00012f30: 7765 6967 6874 732e 2054 6865 2077 6569  weights. The wei
+00012f40: 6768 7473 2061 7265 2067 656e 6572 6174  ghts are generat
+00012f50: 6564 2066 726f 6d20 610a 2020 2020 7374  ed from a.    st
+00012f60: 6963 6b2d 6272 6561 6b69 6e67 2070 726f  ick-breaking pro
+00012f70: 6365 6475 6365 2077 6865 7265 203a 6d61  ceduce where :ma
+00012f80: 7468 3a60 785f 6b20 3d20 765f 6b20 5c70  th:`x_k = v_k \p
+00012f90: 726f 645f 7b5c 656c 6c20 3c20 6b7d 2028  rod_{\ell < k} (
+00012fa0: 3120 2d20 765f 5c65 6c6c 2960 2066 6f72  1 - v_\ell)` for
+00012fb0: 0a20 2020 203a 6d61 7468 3a60 6b20 5c69  .    :math:`k \i
+00012fc0: 6e20 5c7b 312c 205c 6c64 6f74 732c 204b  n \{1, \ldots, K
+00012fd0: 5c7d 6020 616e 6420 3a6d 6174 683a 6078  \}` and :math:`x
+00012fe0: 5f4b 203d 205c 7072 6f64 5f7b 5c65 6c6c  _K = \prod_{\ell
+00012ff0: 203d 2031 7d5e 7b4b 7d20 2831 202d 2076   = 1}^{K} (1 - v
+00013000: 5f5c 656c 6c29 203d 2031 202d 205c 7375  _\ell) = 1 - \su
+00013010: 6d5f 7b5c 656c 6c3d 317d 5e4b 2078 5f5c  m_{\ell=1}^K x_\
+00013020: 656c 6c60 0a20 2020 2077 6974 6820 3a6d  ell`.    with :m
+00013030: 6174 683a 6076 5f6b 205c 7374 6163 6b72  ath:`v_k \stackr
+00013040: 656c 7b5c 7465 7874 7b69 2e69 2e64 2e7d  el{\text{i.i.d.}
+00013050: 7d7b 5c73 696d 7d20 5c74 6578 747b 4265  }{\sim} \text{Be
+00013060: 7461 7d28 312c 205c 616c 7068 6129 602e  ta}(1, \alpha)`.
+00013070: 0a0a 2020 2020 2e2e 206d 6174 683a 0a0a  ..    .. math:..
+00013080: 2020 2020 2020 2020 6628 5c6d 6174 6862          f(\mathb
+00013090: 667b 787d 7c5c 616c 7068 612c 204b 2920  f{x}|\alpha, K) 
+000130a0: 3d0a 2020 2020 2020 2020 2020 2020 4228  =.            B(
+000130b0: 312c 205c 616c 7068 6129 5e7b 2d4b 7d78  1, \alpha)^{-K}x
+000130c0: 5f7b 4b2b 317d 5e5c 616c 7068 6120 5c70  _{K+1}^\alpha \p
+000130d0: 726f 645f 7b6b 3d31 7d5e 7b4b 2b31 7d5c  rod_{k=1}^{K+1}\
+000130e0: 6c65 6674 5c7b 5c73 756d 5f7b 6a3d 6b7d  left\{\sum_{j=k}
+000130f0: 5e7b 4b2b 317d 2078 5f6a 5c72 6967 6874  ^{K+1} x_j\right
+00013100: 5c7d 5e7b 2d31 7d0a 0a20 2020 203d 3d3d  \}^{-1}..    ===
+00013110: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
+00013120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00013140: 3d3d 3d3d 3d3d 0a20 2020 2053 7570 706f  ======.    Suppo
+00013150: 7274 2020 203a 6d61 7468 3a60 785f 6b20  rt   :math:`x_k 
+00013160: 5c69 6e20 2830 2c20 3129 6020 666f 7220  \in (0, 1)` for 
+00013170: 3a6d 6174 683a 606b 205c 696e 205c 7b31  :math:`k \in \{1
+00013180: 2c20 5c6c 646f 7473 2c20 4b2b 315c 7d60  , \ldots, K+1\}`
+00013190: 0a20 2020 2020 2020 2020 2020 2020 2073  .              s
+000131a0: 7563 6820 7468 6174 203a 6d61 7468 3a60  uch that :math:`
+000131b0: 5c73 756d 2078 5f6b 203d 2031 600a 2020  \sum x_k = 1`.  
+000131c0: 2020 4d65 616e 2020 2020 2020 3a6d 6174    Mean      :mat
+000131d0: 683a 605c 6d61 7468 6262 7b45 7d5b 785f  h:`\mathbb{E}[x_
+000131e0: 6b5d 203d 205c 6466 7261 637b 317d 7b31  k] = \dfrac{1}{1
+000131f0: 202b 205c 616c 7068 617d 5c6c 6566 7428   + \alpha}\left(
+00013200: 5c64 6672 6163 7b5c 616c 7068 617d 7b31  \dfrac{\alpha}{1
+00013210: 202b 205c 616c 7068 617d 5c72 6967 6874   + \alpha}\right
+00013220: 295e 7b6b 202d 2031 7d60 0a20 2020 2020  )^{k - 1}`.     
+00013230: 2020 2020 2020 2020 2066 6f72 203a 6d61           for :ma
+00013240: 7468 3a60 6b20 5c69 6e20 5c7b 312c 205c  th:`k \in \{1, \
+00013250: 6c64 6f74 732c 204b 5c7d 6020 616e 6420  ldots, K\}` and 
+00013260: 3a6d 6174 683a 605c 6d61 7468 6262 7b45  :math:`\mathbb{E
+00013270: 7d5b 785f 7b4b 2b31 7d5d 203d 205c 6c65  }[x_{K+1}] = \le
+00013280: 6674 285c 6466 7261 637b 5c61 6c70 6861  ft(\dfrac{\alpha
+00013290: 7d7b 3120 2b20 5c61 6c70 6861 7d5c 7269  }{1 + \alpha}\ri
+000132a0: 6768 7429 5e7b 4b7d 600a 2020 2020 3d3d  ght)^{K}`.    ==
+000132b0: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
+000132c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000132d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000132e0: 3d3d 3d3d 3d3d 3d0a 0a20 2020 2050 6172  =======..    Par
+000132f0: 616d 6574 6572 730a 2020 2020 2d2d 2d2d  ameters.    ----
+00013300: 2d2d 2d2d 2d2d 0a20 2020 2061 6c70 6861  ------.    alpha
+00013310: 203a 2074 656e 736f 725f 6c69 6b65 206f   : tensor_like o
+00013320: 6620 666c 6f61 740a 2020 2020 2020 2020  f float.        
+00013330: 436f 6e63 656e 7472 6174 696f 6e20 7061  Concentration pa
+00013340: 7261 6d65 7465 7220 2861 6c70 6861 203e  rameter (alpha >
+00013350: 2030 292e 0a20 2020 204b 203a 2074 656e   0)..    K : ten
+00013360: 736f 725f 6c69 6b65 206f 6620 696e 740a  sor_like of int.
+00013370: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
+00013380: 6572 206f 6620 2273 7469 636b 7322 2074  er of "sticks" t
+00013390: 6f20 6272 6561 6b20 6f66 6620 6672 6f6d  o break off from
+000133a0: 2061 6e20 696e 6974 6961 6c20 6f6e 652d   an initial one-
+000133b0: 756e 6974 2073 7469 636b 2e20 5468 6520  unit stick. The 
+000133c0: 6c65 6e67 7468 206f 6620 7468 6520 7765  length of the we
+000133d0: 6967 6874 0a20 2020 2020 2020 2076 6563  ight.        vec
+000133e0: 746f 7220 6973 204b 202b 2031 2c20 7768  tor is K + 1, wh
+000133f0: 6572 6520 7468 6520 6c61 7374 2077 6569  ere the last wei
+00013400: 6768 7420 6973 206f 6e65 206d 696e 7573  ght is one minus
+00013410: 2074 6865 2073 756d 206f 6620 616c 6c20   the sum of all 
+00013420: 7468 6520 6669 7273 7420 7374 6963 6b73  the first sticks
+00013430: 2e0a 0a20 2020 2052 6566 6572 656e 6365  ...    Reference
+00013440: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00013450: 0a20 2020 202e 2e20 5b31 5d20 4973 6877  .    .. [1] Ishw
+00013460: 6172 616e 2c20 482e 2c20 2620 4a61 6d65  aran, H., & Jame
+00013470: 732c 204c 2e20 462e 2028 3230 3031 292e  s, L. F. (2001).
+00013480: 2047 6962 6273 2073 616d 706c 696e 6720   Gibbs sampling 
+00013490: 6d65 7468 6f64 7320 666f 7220 7374 6963  methods for stic
+000134a0: 6b2d 6272 6561 6b69 6e67 2070 7269 6f72  k-breaking prior
+000134b0: 732e 0a20 2020 2020 2020 2020 2020 4a6f  s..           Jo
+000134c0: 7572 6e61 6c20 6f66 2074 6865 2041 6d65  urnal of the Ame
+000134d0: 7269 6361 6e20 5374 6174 6973 7469 6361  rican Statistica
+000134e0: 6c20 4173 736f 6369 6174 696f 6e2c 2039  l Association, 9
+000134f0: 3628 3435 3329 2c20 3136 312d 3137 332e  6(453), 161-173.
+00013500: 0a0a 2020 2020 2e2e 205b 325d 204d c3bc  ..    .. [2] M..
+00013510: 6c6c 6572 2c20 502e 2c20 5175 696e 7461  ller, P., Quinta
+00013520: 6e61 2c20 462e 2041 2e2c 204a 6172 612c  na, F. A., Jara,
+00013530: 2041 2e2c 2026 2048 616e 736f 6e2c 2054   A., & Hanson, T
+00013540: 2e20 2832 3031 3529 2e20 4261 7965 7369  . (2015). Bayesi
+00013550: 616e 206e 6f6e 7061 7261 6d65 7472 6963  an nonparametric
+00013560: 2064 6174 610a 2020 2020 2020 2020 2020   data.          
+00013570: 2061 6e61 6c79 7369 732e 204e 6577 2059   analysis. New Y
+00013580: 6f72 6b3a 2053 7072 696e 6765 722e 0a20  ork: Springer.. 
+00013590: 2020 2022 2222 0a20 2020 2072 765f 6f70     """.    rv_op
+000135a0: 203d 2073 7469 636b 6272 6561 6b69 6e67   = stickbreaking
+000135b0: 7765 6967 6874 730a 0a20 2020 2040 636c  weights..    @cl
+000135c0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+000135d0: 6620 6469 7374 2863 6c73 2c20 616c 7068  f dist(cls, alph
+000135e0: 612c 204b 2c20 2a61 7267 732c 202a 2a6b  a, K, *args, **k
+000135f0: 7761 7267 7329 3a0a 2020 2020 2020 2020  wargs):.        
+00013600: 616c 7068 6120 3d20 7074 2e61 735f 7465  alpha = pt.as_te
+00013610: 6e73 6f72 5f76 6172 6961 626c 6528 666c  nsor_variable(fl
+00013620: 6f61 7458 2861 6c70 6861 2929 0a20 2020  oatX(alpha)).   
+00013630: 2020 2020 204b 203d 2070 742e 6173 5f74       K = pt.as_t
+00013640: 656e 736f 725f 7661 7269 6162 6c65 2869  ensor_variable(i
+00013650: 6e74 5828 4b29 290a 0a20 2020 2020 2020  ntX(K))..       
+00013660: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00013670: 6469 7374 285b 616c 7068 612c 204b 5d2c  dist([alpha, K],
+00013680: 202a 2a6b 7761 7267 7329 0a0a 2020 2020   **kwargs)..    
+00013690: 6465 6620 6d6f 6d65 6e74 2872 762c 2073  def moment(rv, s
+000136a0: 697a 652c 2061 6c70 6861 2c20 4b29 3a0a  ize, alpha, K):.
+000136b0: 2020 2020 2020 2020 616c 7068 6120 3d20          alpha = 
+000136c0: 616c 7068 615b 2e2e 2e2c 206e 702e 6e65  alpha[..., np.ne
+000136d0: 7761 7869 735d 0a20 2020 2020 2020 206d  waxis].        m
+000136e0: 6f6d 656e 7420 3d20 2861 6c70 6861 202f  oment = (alpha /
+000136f0: 2028 3120 2b20 616c 7068 6129 2920 2a2a   (1 + alpha)) **
+00013700: 2070 742e 6172 616e 6765 284b 290a 2020   pt.arange(K).  
+00013710: 2020 2020 2020 6d6f 6d65 6e74 202a 3d20        moment *= 
+00013720: 3120 2f20 2831 202b 2061 6c70 6861 290a  1 / (1 + alpha).
+00013730: 2020 2020 2020 2020 6d6f 6d65 6e74 203d          moment =
+00013740: 2070 742e 636f 6e63 6174 656e 6174 6528   pt.concatenate(
+00013750: 5b6d 6f6d 656e 742c 2028 616c 7068 6120  [moment, (alpha 
+00013760: 2f20 2831 202b 2061 6c70 6861 2929 202a  / (1 + alpha)) *
+00013770: 2a20 4b5d 2c20 6178 6973 3d2d 3129 0a20  * K], axis=-1). 
+00013780: 2020 2020 2020 2069 6620 6e6f 7420 7276         if not rv
+00013790: 5f73 697a 655f 6973 5f6e 6f6e 6528 7369  _size_is_none(si
+000137a0: 7a65 293a 0a20 2020 2020 2020 2020 2020  ze):.           
+000137b0: 206d 6f6d 656e 745f 7369 7a65 203d 2070   moment_size = p
+000137c0: 742e 636f 6e63 6174 656e 6174 6528 0a20  t.concatenate(. 
+000137d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000137e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000137f0: 2020 2020 2073 697a 652c 0a20 2020 2020       size,.     
+00013800: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+00013810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013820: 2020 2020 2020 2020 204b 202b 2031 2c0a           K + 1,.
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 2020 2020 5d2c 0a20 2020 2020 2020 2020      ],.         
+00013850: 2020 2020 2020 205d 0a20 2020 2020 2020         ].       
+00013860: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
+00013870: 2020 206d 6f6d 656e 7420 3d20 7074 2e66     moment = pt.f
+00013880: 756c 6c28 6d6f 6d65 6e74 5f73 697a 652c  ull(moment_size,
+00013890: 206d 6f6d 656e 7429 0a0a 2020 2020 2020   moment)..      
+000138a0: 2020 7265 7475 726e 206d 6f6d 656e 740a    return moment.
+000138b0: 0a20 2020 2064 6566 206c 6f67 7028 7661  .    def logp(va
+000138c0: 6c75 652c 2061 6c70 6861 2c20 4b29 3a0a  lue, alpha, K):.
+000138d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000138e0: 2020 2020 4361 6c63 756c 6174 6520 6c6f      Calculate lo
+000138f0: 672d 7072 6f62 6162 696c 6974 7920 6f66  g-probability of
+00013900: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
+00013910: 6e20 696e 6475 6365 6420 6672 6f6d 2074  n induced from t
+00013920: 6865 2073 7469 636b 2d62 7265 616b 696e  he stick-breakin
+00013930: 6720 7072 6f63 6573 730a 2020 2020 2020  g process.      
+00013940: 2020 6174 2073 7065 6369 6669 6564 2076    at specified v
+00013950: 616c 7565 2e0a 0a20 2020 2020 2020 2050  alue...        P
+00013960: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00013970: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00013980: 2020 2020 2076 616c 7565 3a20 6e75 6d65       value: nume
+00013990: 7269 630a 2020 2020 2020 2020 2020 2020  ric.            
+000139a0: 5661 6c75 6520 666f 7220 7768 6963 6820  Value for which 
+000139b0: 6c6f 672d 7072 6f62 6162 696c 6974 7920  log-probability 
+000139c0: 6973 2063 616c 6375 6c61 7465 642e 0a0a  is calculated...
+000139d0: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
+000139e0: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
+000139f0: 2020 2020 2020 2020 5465 6e73 6f72 5661          TensorVa
+00013a00: 7269 6162 6c65 0a20 2020 2020 2020 2022  riable.        "
+00013a10: 2222 0a20 2020 2020 2020 206c 6f67 7020  "".        logp 
+00013a20: 3d20 2d70 742e 7375 6d28 0a20 2020 2020  = -pt.sum(.     
+00013a30: 2020 2020 2020 2070 742e 6c6f 6728 0a20         pt.log(. 
+00013a40: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00013a50: 742e 6375 6d73 756d 280a 2020 2020 2020  t.cumsum(.      
+00013a60: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00013a70: 6c75 655b 2e2e 2e2c 203a 3a2d 315d 2c0a  lue[..., ::-1],.
+00013a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a90: 2020 2020 6178 6973 3d2d 312c 0a20 2020      axis=-1,.   
+00013aa0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
+00013ab0: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
+00013ac0: 2020 2020 2020 2020 2020 6178 6973 3d2d            axis=-
+00013ad0: 312c 0a20 2020 2020 2020 2029 0a20 2020  1,.        ).   
+00013ae0: 2020 2020 206c 6f67 7020 2b3d 202d 4b20       logp += -K 
+00013af0: 2a20 6265 7461 6c6e 2831 2c20 616c 7068  * betaln(1, alph
+00013b00: 6129 0a20 2020 2020 2020 206c 6f67 7020  a).        logp 
+00013b10: 2b3d 2061 6c70 6861 202a 2070 742e 6c6f  += alpha * pt.lo
+00013b20: 6728 7661 6c75 655b 2e2e 2e2c 202d 315d  g(value[..., -1]
+00013b30: 290a 0a20 2020 2020 2020 206c 6f67 7020  )..        logp 
+00013b40: 3d20 7074 2e73 7769 7463 6828 0a20 2020  = pt.switch(.   
+00013b50: 2020 2020 2020 2020 2070 742e 6f72 5f28           pt.or_(
+00013b60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013b70: 2070 742e 616e 7928 0a20 2020 2020 2020   pt.any(.       
+00013b80: 2020 2020 2020 2020 2020 2020 2070 742e               pt.
+00013b90: 616e 645f 2870 742e 6c65 2876 616c 7565  and_(pt.le(value
+00013ba0: 2c20 3029 2c20 7074 2e67 6528 7661 6c75  , 0), pt.ge(valu
+00013bb0: 652c 2031 2929 2c0a 2020 2020 2020 2020  e, 1)),.        
+00013bc0: 2020 2020 2020 2020 2020 2020 6178 6973              axis
+00013bd0: 3d2d 312c 0a20 2020 2020 2020 2020 2020  =-1,.           
+00013be0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
+00013bf0: 2020 2020 2020 2020 7074 2e6f 725f 280a          pt.or_(.
+00013c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c10: 2020 2020 7074 2e62 6974 7769 7365 5f6e      pt.bitwise_n
+00013c20: 6f74 2870 742e 616c 6c63 6c6f 7365 2876  ot(pt.allclose(v
+00013c30: 616c 7565 2e73 756d 282d 3129 2c20 3129  alue.sum(-1), 1)
+00013c40: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00013c50: 2020 2020 2020 2070 742e 6e65 7128 7661         pt.neq(va
+00013c60: 6c75 652e 7368 6170 655b 2d31 5d2c 204b  lue.shape[-1], K
+00013c70: 202b 2031 292c 0a20 2020 2020 2020 2020   + 1),.         
+00013c80: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00013c90: 2020 2020 2020 292c 0a20 2020 2020 2020        ),.       
+00013ca0: 2020 2020 202d 6e70 2e69 6e66 2c0a 2020       -np.inf,.  
+00013cb0: 2020 2020 2020 2020 2020 6c6f 6770 2c0a            logp,.
+00013cc0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+00013cd0: 2020 2072 6574 7572 6e20 6368 6563 6b5f     return check_
+00013ce0: 7061 7261 6d65 7465 7273 280a 2020 2020  parameters(.    
+00013cf0: 2020 2020 2020 2020 6c6f 6770 2c0a 2020          logp,.  
+00013d00: 2020 2020 2020 2020 2020 616c 7068 6120            alpha 
+00013d10: 3e20 302c 0a20 2020 2020 2020 2020 2020  > 0,.           
+00013d20: 204b 203e 2030 2c0a 2020 2020 2020 2020   K > 0,.        
+00013d30: 2020 2020 6d73 673d 2261 6c70 6861 203e      msg="alpha >
+00013d40: 2030 2c20 4b20 3e20 3022 2c0a 2020 2020   0, K > 0",.    
+00013d50: 2020 2020 290a 0a0a 636c 6173 7320 5a65      )...class Ze
+00013d60: 726f 5375 6d4e 6f72 6d61 6c52 5628 5379  roSumNormalRV(Sy
+00013d70: 6d62 6f6c 6963 5261 6e64 6f6d 5661 7269  mbolicRandomVari
+00013d80: 6162 6c65 293a 0a20 2020 2022 2222 5a65  able):.    """Ze
+00013d90: 726f 5375 6d4e 6f72 6d61 6c20 7261 6e64  roSumNormal rand
+00013da0: 6f6d 2076 6172 6961 626c 6522 2222 0a0a  om variable"""..
+00013db0: 2020 2020 5f70 7269 6e74 5f6e 616d 6520      _print_name 
+00013dc0: 3d20 2822 5a65 726f 5375 6d4e 6f72 6d61  = ("ZeroSumNorma
+00013dd0: 6c22 2c20 225c 5c6f 7065 7261 746f 726e  l", "\\operatorn
+00013de0: 616d 657b 5a65 726f 5375 6d4e 6f72 6d61  ame{ZeroSumNorma
+00013df0: 6c7d 2229 0a20 2020 2064 6566 6175 6c74  l}").    default
+00013e00: 5f6f 7574 7075 7420 3d20 300a 0a0a 636c  _output = 0...cl
+00013e10: 6173 7320 5a65 726f 5375 6d4e 6f72 6d61  ass ZeroSumNorma
+00013e20: 6c28 4469 7374 7269 6275 7469 6f6e 293a  l(Distribution):
+00013e30: 0a20 2020 2072 2222 220a 2020 2020 5a65  .    r""".    Ze
+00013e40: 726f 5375 6d4e 6f72 6d61 6c20 6469 7374  roSumNormal dist
+00013e50: 7269 6275 7469 6f6e 2c20 692e 6520 4e6f  ribution, i.e No
+00013e60: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
+00013e70: 6e20 7768 6572 6520 6f6e 6520 6f72 0a20  n where one or. 
+00013e80: 2020 2073 6576 6572 616c 2061 7865 7320     several axes 
+00013e90: 6172 6520 636f 6e73 7472 6169 6e65 6420  are constrained 
+00013ea0: 746f 2073 756d 2074 6f20 7a65 726f 2e0a  to sum to zero..
+00013eb0: 2020 2020 4279 2064 6566 6175 6c74 2c20      By default, 
+00013ec0: 7468 6520 6c61 7374 2061 7869 7320 6973  the last axis is
+00013ed0: 2063 6f6e 7374 7261 696e 6564 2074 6f20   constrained to 
+00013ee0: 7375 6d20 746f 207a 6572 6f2e 0a20 2020  sum to zero..   
+00013ef0: 2053 6565 2060 6e5f 7a65 726f 7375 6d5f   See `n_zerosum_
+00013f00: 6178 6573 6020 6b77 6172 6720 666f 7220  axes` kwarg for 
+00013f10: 6d6f 7265 2064 6574 6169 6c73 2e0a 0a20  more details... 
+00013f20: 2020 202e 2e20 6d61 7468 3a3a 0a0a 2020     .. math::..  
+00013f30: 2020 2020 2020 5c62 6567 696e 7b61 6c69        \begin{ali
+00013f40: 676e 2a7d 0a20 2020 2020 2020 2020 2020  gn*}.           
+00013f50: 205a 534e 285c 7369 676d 6129 203d 204e   ZSN(\sigma) = N
+00013f60: 205c 4269 6728 2030 2c20 5c73 6967 6d61   \Big( 0, \sigma
+00013f70: 5e32 2028 4920 2d20 5c74 6672 6163 7b31  ^2 (I - \tfrac{1
+00013f80: 7d7b 6e7d 4a29 205c 4269 6729 205c 5c0a  }{n}J) \Big) \\.
+00013f90: 2020 2020 2020 2020 2020 2020 5c74 6578              \tex
+00013fa0: 747b 7768 6572 657d 205c 207e 204a 5f7b  t{where} \ ~ J_{
+00013fb0: 696a 7d20 3d20 3120 5c20 7e20 5c74 6578  ij} = 1 \ ~ \tex
+00013fc0: 747b 616e 647d 205c 5c0a 2020 2020 2020  t{and} \\.      
+00013fd0: 2020 2020 2020 6e20 3d20 5c74 6578 747b        n = \text{
+00013fe0: 6e62 7220 6f66 207a 6572 6f2d 7375 6d20  nbr of zero-sum 
+00013ff0: 6178 6573 7d0a 2020 2020 2020 2020 5c65  axes}.        \e
+00014000: 6e64 7b61 6c69 676e 2a7d 0a0a 2020 2020  nd{align*}..    
+00014010: 5061 7261 6d65 7465 7273 0a20 2020 202d  Parameters.    -
+00014020: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 7369  ---------.    si
+00014030: 676d 6120 3a20 7465 6e73 6f72 5f6c 696b  gma : tensor_lik
+00014040: 6520 6f66 2066 6c6f 6174 0a20 2020 2020  e of float.     
+00014050: 2020 2053 6361 6c65 2070 6172 616d 6574     Scale paramet
+00014060: 6572 2028 7369 676d 6120 3e20 3029 2e0a  er (sigma > 0)..
+00014070: 2020 2020 2020 2020 4974 2773 2061 6374          It's act
+00014080: 7561 6c6c 7920 7468 6520 7374 616e 6461  ually the standa
+00014090: 7264 2064 6576 6961 7469 6f6e 206f 6620  rd deviation of 
+000140a0: 7468 6520 756e 6465 726c 7969 6e67 2c20  the underlying, 
+000140b0: 756e 636f 6e73 7472 6169 6e65 6420 4e6f  unconstrained No
+000140c0: 726d 616c 2064 6973 7472 6962 7574 696f  rmal distributio
+000140d0: 6e2e 0a20 2020 2020 2020 2044 6566 6175  n..        Defau
+000140e0: 6c74 7320 746f 2031 2069 6620 6e6f 7420  lts to 1 if not 
+000140f0: 7370 6563 6966 6965 642e 0a20 2020 2020  specified..     
+00014100: 2020 2046 6f72 206e 6f77 2c20 6060 7369     For now, ``si
+00014110: 676d 6160 6020 6861 7320 746f 2062 6520  gma`` has to be 
+00014120: 6120 7363 616c 6172 2c20 746f 2065 6e73  a scalar, to ens
+00014130: 7572 6520 7468 6520 7a65 726f 2d73 756d  ure the zero-sum
+00014140: 2063 6f6e 7374 7261 696e 742e 0a20 2020   constraint..   
+00014150: 206e 5f7a 6572 6f73 756d 5f61 7865 733a   n_zerosum_axes:
+00014160: 2069 6e74 2c20 6465 6661 756c 7473 2074   int, defaults t
+00014170: 6f20 310a 2020 2020 2020 2020 4e75 6d62  o 1.        Numb
+00014180: 6572 206f 6620 6178 6573 2061 6c6f 6e67  er of axes along
+00014190: 2077 6869 6368 2074 6865 207a 6572 6f2d   which the zero-
+000141a0: 7375 6d20 636f 6e73 7472 6169 6e74 2069  sum constraint i
+000141b0: 7320 656e 666f 7263 6564 2c20 7374 6172  s enforced, star
+000141c0: 7469 6e67 2066 726f 6d20 7468 6520 7269  ting from the ri
+000141d0: 6768 746d 6f73 7420 706f 7369 7469 6f6e  ghtmost position
+000141e0: 2e0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
+000141f0: 7473 2074 6f20 312c 2069 2e65 2074 6865  ts to 1, i.e the
+00014200: 2072 6967 6874 6d6f 7374 2061 7869 732e   rightmost axis.
+00014210: 0a20 2020 207a 6572 6f73 756d 5f61 7865  .    zerosum_axe
+00014220: 733a 2069 6e74 2c20 6465 7072 6563 6174  s: int, deprecat
+00014230: 6564 2070 6c65 6173 6520 7573 6520 6e5f  ed please use n_
+00014240: 7a65 726f 7375 6d5f 6178 6573 2061 7320  zerosum_axes as 
+00014250: 6974 7320 7375 6363 6573 736f 720a 2020  its successor.  
+00014260: 2020 6469 6d73 3a20 7365 7175 656e 6365    dims: sequence
+00014270: 206f 6620 7374 7269 6e67 732c 206f 7074   of strings, opt
+00014280: 696f 6e61 6c0a 2020 2020 2020 2020 4469  ional.        Di
+00014290: 6d65 6e73 696f 6e20 6e61 6d65 7320 6f66  mension names of
+000142a0: 2074 6865 2064 6973 7472 6962 7574 696f   the distributio
+000142b0: 6e2e 2057 6f72 6b73 2074 6865 2073 616d  n. Works the sam
+000142c0: 6520 6173 2066 6f72 206f 7468 6572 2050  e as for other P
+000142d0: 794d 4320 6469 7374 7269 6275 7469 6f6e  yMC distribution
+000142e0: 732e 0a20 2020 2020 2020 204e 6563 6573  s..        Neces
+000142f0: 7361 7279 2069 6620 6060 7368 6170 6560  sary if ``shape`
+00014300: 6020 6973 206e 6f74 2070 6173 7365 642e  ` is not passed.
+00014310: 0a20 2020 2073 6861 7065 3a20 7475 706c  .    shape: tupl
+00014320: 6520 6f66 2069 6e74 6567 6572 732c 206f  e of integers, o
+00014330: 7074 696f 6e61 6c0a 2020 2020 2020 2020  ptional.        
+00014340: 5368 6170 6520 6f66 2074 6865 2064 6973  Shape of the dis
+00014350: 7472 6962 7574 696f 6e2e 2057 6f72 6b73  tribution. Works
+00014360: 2074 6865 2073 616d 6520 6173 2066 6f72   the same as for
+00014370: 206f 7468 6572 2050 794d 4320 6469 7374   other PyMC dist
+00014380: 7269 6275 7469 6f6e 732e 0a20 2020 2020  ributions..     
+00014390: 2020 204e 6563 6573 7361 7279 2069 6620     Necessary if 
+000143a0: 6060 6469 6d73 6060 206f 7220 6060 6f62  ``dims`` or ``ob
+000143b0: 7365 7276 6564 6060 2069 7320 6e6f 7420  served`` is not 
+000143c0: 7061 7373 6564 2e0a 0a20 2020 2057 6172  passed...    War
+000143d0: 6e69 6e67 730a 2020 2020 2d2d 2d2d 2d2d  nings.    ------
+000143e0: 2d2d 0a20 2020 2060 6073 6967 6d61 6060  --.    ``sigma``
+000143f0: 2068 6173 2074 6f20 6265 2061 2073 6361   has to be a sca
+00014400: 6c61 722c 2074 6f20 656e 7375 7265 2074  lar, to ensure t
+00014410: 6865 207a 6572 6f2d 7375 6d20 636f 6e73  he zero-sum cons
+00014420: 7472 6169 6e74 2e0a 2020 2020 5468 6520  traint..    The 
+00014430: 6162 696c 6974 7920 746f 2073 7065 6369  ability to speci
+00014440: 6679 2061 2076 6563 746f 7220 6f66 2060  fy a vector of `
+00014450: 6073 6967 6d61 6060 206d 6179 2062 6520  `sigma`` may be 
+00014460: 6164 6465 6420 696e 2066 7574 7572 6520  added in future 
+00014470: 7665 7273 696f 6e73 2e0a 0a20 2020 2060  versions...    `
+00014480: 606e 5f7a 6572 6f73 756d 5f61 7865 7360  `n_zerosum_axes`
+00014490: 6020 6861 7320 746f 2062 6520 3e20 302e  ` has to be > 0.
+000144a0: 2049 6620 796f 7520 7761 6e74 2074 6865   If you want the
+000144b0: 2062 6568 6176 696f 7220 6f66 2060 606e   behavior of ``n
+000144c0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
+000144d0: 3060 602c 0a20 2020 206a 7573 7420 7573  0``,.    just us
+000144e0: 6520 6060 706d 2e4e 6f72 6d61 6c60 602e  e ``pm.Normal``.
+000144f0: 0a0a 2020 2020 4578 616d 706c 6573 0a20  ..    Examples. 
+00014500: 2020 202d 2d2d 2d2d 2d2d 2d0a 2020 2020     --------.    
+00014510: 4465 6669 6e65 2061 2060 5a65 726f 5375  Define a `ZeroSu
+00014520: 6d4e 6f72 6d61 6c60 2076 6172 6961 626c  mNormal` variabl
+00014530: 652c 2077 6974 6820 6073 6967 6d61 3d31  e, with `sigma=1
+00014540: 6020 616e 640a 2020 2020 606e 5f7a 6572  ` and.    `n_zer
+00014550: 6f73 756d 5f61 7865 733d 3160 2020 6279  osum_axes=1`  by
+00014560: 2064 6566 6175 6c74 3a3a 0a0a 2020 2020   default::..    
+00014570: 2020 2020 434f 4f52 4453 203d 207b 0a20      COORDS = {. 
+00014580: 2020 2020 2020 2020 2020 2022 7265 6769             "regi
+00014590: 6f6e 7322 3a20 5b22 6122 2c20 2262 222c  ons": ["a", "b",
+000145a0: 2022 6322 5d2c 0a20 2020 2020 2020 2020   "c"],.         
+000145b0: 2020 2022 616e 7377 6572 7322 3a20 5b22     "answers": ["
+000145c0: 7965 7322 2c20 226e 6f22 2c20 2277 6861  yes", "no", "wha
+000145d0: 7465 7665 7222 2c20 2264 6f6e 2774 2075  tever", "don't u
+000145e0: 6e64 6572 7374 616e 6420 7175 6573 7469  nderstand questi
+000145f0: 6f6e 225d 2c0a 2020 2020 2020 2020 7d0a  on"],.        }.
+00014600: 2020 2020 2020 2020 7769 7468 2070 6d2e          with pm.
+00014610: 4d6f 6465 6c28 636f 6f72 6473 3d43 4f4f  Model(coords=COO
+00014620: 5244 5329 2061 7320 6d3a 0a20 2020 2020  RDS) as m:.     
+00014630: 2020 2020 2020 2023 2074 6865 207a 6572         # the zer
+00014640: 6f20 7375 6d20 6178 6973 2077 696c 6c20  o sum axis will 
+00014650: 6265 2027 616e 7377 6572 7327 0a20 2020  be 'answers'.   
+00014660: 2020 2020 2020 2020 2076 203d 2070 6d2e           v = pm.
+00014670: 5a65 726f 5375 6d4e 6f72 6d61 6c28 2276  ZeroSumNormal("v
+00014680: 222c 2064 696d 733d 2822 7265 6769 6f6e  ", dims=("region
+00014690: 7322 2c20 2261 6e73 7765 7273 2229 290a  s", "answers")).
+000146a0: 0a20 2020 2020 2020 2077 6974 6820 706d  .        with pm
+000146b0: 2e4d 6f64 656c 2863 6f6f 7264 733d 434f  .Model(coords=CO
+000146c0: 4f52 4453 2920 6173 206d 3a0a 2020 2020  ORDS) as m:.    
+000146d0: 2020 2020 2020 2020 2320 7468 6520 7a65          # the ze
+000146e0: 726f 2073 756d 2061 7865 7320 7769 6c6c  ro sum axes will
+000146f0: 2062 6520 2761 6e73 7765 7273 2720 616e   be 'answers' an
+00014700: 6420 2772 6567 696f 6e73 270a 2020 2020  d 'regions'.    
+00014710: 2020 2020 2020 2020 7620 3d20 706d 2e5a          v = pm.Z
+00014720: 6572 6f53 756d 4e6f 726d 616c 2822 7622  eroSumNormal("v"
+00014730: 2c20 6469 6d73 3d28 2272 6567 696f 6e73  , dims=("regions
+00014740: 222c 2022 616e 7377 6572 7322 292c 206e  ", "answers"), n
+00014750: 5f7a 6572 6f73 756d 5f61 7865 733d 3229  _zerosum_axes=2)
+00014760: 0a0a 2020 2020 2020 2020 7769 7468 2070  ..        with p
+00014770: 6d2e 4d6f 6465 6c28 636f 6f72 6473 3d43  m.Model(coords=C
+00014780: 4f4f 5244 5329 2061 7320 6d3a 0a20 2020  OORDS) as m:.   
+00014790: 2020 2020 2020 2020 2023 2074 6865 207a           # the z
+000147a0: 6572 6f20 7375 6d20 6178 6573 2077 696c  ero sum axes wil
+000147b0: 6c20 6265 2074 6865 206c 6173 7420 7477  l be the last tw
+000147c0: 6f0a 2020 2020 2020 2020 2020 2020 7620  o.            v 
+000147d0: 3d20 706d 2e5a 6572 6f53 756d 4e6f 726d  = pm.ZeroSumNorm
+000147e0: 616c 2822 7622 2c20 7368 6170 653d 2833  al("v", shape=(3
+000147f0: 2c20 342c 2035 292c 206e 5f7a 6572 6f73  , 4, 5), n_zeros
+00014800: 756d 5f61 7865 733d 3229 0a20 2020 2022  um_axes=2).    "
+00014810: 2222 0a20 2020 2072 765f 7479 7065 203d  "".    rv_type =
+00014820: 205a 6572 6f53 756d 4e6f 726d 616c 5256   ZeroSumNormalRV
+00014830: 0a0a 2020 2020 6465 6620 5f5f 6e65 775f  ..    def __new_
+00014840: 5f28 0a20 2020 2020 2020 2063 6c73 2c20  _(.        cls, 
+00014850: 2a61 7267 732c 207a 6572 6f73 756d 5f61  *args, zerosum_a
+00014860: 7865 733d 4e6f 6e65 2c20 6e5f 7a65 726f  xes=None, n_zero
+00014870: 7375 6d5f 6178 6573 3d4e 6f6e 652c 2073  sum_axes=None, s
+00014880: 7570 706f 7274 5f73 6861 7065 3d4e 6f6e  upport_shape=Non
+00014890: 652c 2064 696d 733d 4e6f 6e65 2c20 2a2a  e, dims=None, **
+000148a0: 6b77 6172 6773 0a20 2020 2029 3a0a 2020  kwargs.    ):.  
+000148b0: 2020 2020 2020 6966 207a 6572 6f73 756d        if zerosum
+000148c0: 5f61 7865 7320 6973 206e 6f74 204e 6f6e  _axes is not Non
+000148d0: 653a 0a20 2020 2020 2020 2020 2020 206e  e:.            n
+000148e0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
+000148f0: 7a65 726f 7375 6d5f 6178 6573 0a20 2020  zerosum_axes.   
+00014900: 2020 2020 2020 2020 2077 6172 6e69 6e67           warning
+00014910: 732e 7761 726e 280a 2020 2020 2020 2020  s.warn(.        
+00014920: 2020 2020 2020 2020 2254 6865 2027 7a65          "The 'ze
+00014930: 726f 7375 6d5f 6178 6573 2720 7061 7261  rosum_axes' para
+00014940: 6d65 7465 7220 6973 2064 6570 7265 6361  meter is depreca
+00014950: 7465 642e 2055 7365 2027 6e5f 7a65 726f  ted. Use 'n_zero
+00014960: 7375 6d5f 6178 6573 2720 696e 7374 6561  sum_axes' instea
+00014970: 642e 222c 0a20 2020 2020 2020 2020 2020  d.",.           
+00014980: 2020 2020 2044 6570 7265 6361 7469 6f6e       Deprecation
+00014990: 5761 726e 696e 672c 0a20 2020 2020 2020  Warning,.       
+000149a0: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+000149b0: 6620 6469 6d73 2069 7320 6e6f 7420 4e6f  f dims is not No
+000149c0: 6e65 206f 7220 6b77 6172 6773 2e67 6574  ne or kwargs.get
+000149d0: 2822 6f62 7365 7276 6564 2229 2069 7320  ("observed") is 
+000149e0: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+000149f0: 2020 2020 2020 6e5f 7a65 726f 7375 6d5f        n_zerosum_
+00014a00: 6178 6573 203d 2063 6c73 2e63 6865 636b  axes = cls.check
+00014a10: 5f7a 6572 6f73 756d 5f61 7865 7328 6e5f  _zerosum_axes(n_
+00014a20: 7a65 726f 7375 6d5f 6178 6573 290a 0a20  zerosum_axes).. 
+00014a30: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+00014a40: 7274 5f73 6861 7065 203d 2067 6574 5f73  rt_shape = get_s
+00014a50: 7570 706f 7274 5f73 6861 7065 280a 2020  upport_shape(.  
+00014a60: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00014a70: 7070 6f72 745f 7368 6170 653d 7375 7070  pport_shape=supp
+00014a80: 6f72 745f 7368 6170 652c 0a20 2020 2020  ort_shape,.     
+00014a90: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00014aa0: 3d4e 6f6e 652c 2020 2320 5368 6170 6520  =None,  # Shape 
+00014ab0: 7769 6c6c 2062 6520 6368 6563 6b65 6420  will be checked 
+00014ac0: 696e 2060 636c 732e 6469 7374 600a 2020  in `cls.dist`.  
+00014ad0: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00014ae0: 6d73 3d64 696d 732c 0a20 2020 2020 2020  ms=dims,.       
+00014af0: 2020 2020 2020 2020 206f 6273 6572 7665           observe
+00014b00: 643d 6b77 6172 6773 2e67 6574 2822 6f62  d=kwargs.get("ob
+00014b10: 7365 7276 6564 222c 204e 6f6e 6529 2c0a  served", None),.
+00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014b30: 6e64 696d 5f73 7570 703d 6e5f 7a65 726f  ndim_supp=n_zero
+00014b40: 7375 6d5f 6178 6573 2c0a 2020 2020 2020  sum_axes,.      
+00014b50: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
+00014b60: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00014b70: 5f5f 6e65 775f 5f28 0a20 2020 2020 2020  __new__(.       
+00014b80: 2020 2020 2063 6c73 2c0a 2020 2020 2020       cls,.      
+00014b90: 2020 2020 2020 2a61 7267 732c 0a20 2020        *args,.   
+00014ba0: 2020 2020 2020 2020 206e 5f7a 6572 6f73           n_zeros
+00014bb0: 756d 5f61 7865 733d 6e5f 7a65 726f 7375  um_axes=n_zerosu
+00014bc0: 6d5f 6178 6573 2c0a 2020 2020 2020 2020  m_axes,.        
+00014bd0: 2020 2020 7375 7070 6f72 745f 7368 6170      support_shap
+00014be0: 653d 7375 7070 6f72 745f 7368 6170 652c  e=support_shape,
+00014bf0: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
+00014c00: 733d 6469 6d73 2c0a 2020 2020 2020 2020  s=dims,.        
+00014c10: 2020 2020 2a2a 6b77 6172 6773 2c0a 2020      **kwargs,.  
+00014c20: 2020 2020 2020 290a 0a20 2020 2040 636c        )..    @cl
+00014c30: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00014c40: 6620 6469 7374 2863 6c73 2c20 7369 676d  f dist(cls, sigm
+00014c50: 613d 312c 206e 5f7a 6572 6f73 756d 5f61  a=1, n_zerosum_a
+00014c60: 7865 733d 4e6f 6e65 2c20 7375 7070 6f72  xes=None, suppor
+00014c70: 745f 7368 6170 653d 4e6f 6e65 2c20 2a2a  t_shape=None, **
+00014c80: 6b77 6172 6773 293a 0a20 2020 2020 2020  kwargs):.       
+00014c90: 206e 5f7a 6572 6f73 756d 5f61 7865 7320   n_zerosum_axes 
+00014ca0: 3d20 636c 732e 6368 6563 6b5f 7a65 726f  = cls.check_zero
+00014cb0: 7375 6d5f 6178 6573 286e 5f7a 6572 6f73  sum_axes(n_zeros
+00014cc0: 756d 5f61 7865 7329 0a0a 2020 2020 2020  um_axes)..      
+00014cd0: 2020 7369 676d 6120 3d20 7074 2e61 735f    sigma = pt.as_
+00014ce0: 7465 6e73 6f72 5f76 6172 6961 626c 6528  tensor_variable(
+00014cf0: 666c 6f61 7458 2873 6967 6d61 2929 0a20  floatX(sigma)). 
+00014d00: 2020 2020 2020 2069 6620 7369 676d 612e         if sigma.
+00014d10: 6e64 696d 203e 2030 3a0a 2020 2020 2020  ndim > 0:.      
+00014d20: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00014d30: 6545 7272 6f72 2822 7369 676d 6120 6861  eError("sigma ha
+00014d40: 7320 746f 2062 6520 6120 7363 616c 6172  s to be a scalar
+00014d50: 2229 0a0a 2020 2020 2020 2020 7375 7070  ")..        supp
+00014d60: 6f72 745f 7368 6170 6520 3d20 6765 745f  ort_shape = get_
+00014d70: 7375 7070 6f72 745f 7368 6170 6528 0a20  support_shape(. 
+00014d80: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+00014d90: 7274 5f73 6861 7065 3d73 7570 706f 7274  rt_shape=support
+00014da0: 5f73 6861 7065 2c0a 2020 2020 2020 2020  _shape,.        
+00014db0: 2020 2020 7368 6170 653d 6b77 6172 6773      shape=kwargs
+00014dc0: 2e67 6574 2822 7368 6170 6522 292c 0a20  .get("shape"),. 
+00014dd0: 2020 2020 2020 2020 2020 206e 6469 6d5f             ndim_
+00014de0: 7375 7070 3d6e 5f7a 6572 6f73 756d 5f61  supp=n_zerosum_a
+00014df0: 7865 732c 0a20 2020 2020 2020 2029 0a0a  xes,.        )..
+00014e00: 2020 2020 2020 2020 6966 2073 7570 706f          if suppo
+00014e10: 7274 5f73 6861 7065 2069 7320 4e6f 6e65  rt_shape is None
+00014e20: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00014e30: 206e 5f7a 6572 6f73 756d 5f61 7865 7320   n_zerosum_axes 
+00014e40: 3e20 303a 0a20 2020 2020 2020 2020 2020  > 0:.           
+00014e50: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
+00014e60: 4572 726f 7228 2259 6f75 206d 7573 7420  Error("You must 
+00014e70: 7370 6563 6966 7920 6469 6d73 2c20 7368  specify dims, sh
+00014e80: 6170 6520 6f72 2073 7570 706f 7274 5f73  ape or support_s
+00014e90: 6861 7065 2070 6172 616d 6574 6572 2229  hape parameter")
+00014ea0: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
+00014eb0: 4f44 4f3a 2065 6467 652d 6361 7365 2064  ODO: edge-case d
+00014ec0: 6f65 736e 2774 2077 6f72 6b20 666f 7220  oesn't work for 
+00014ed0: 6e6f 772c 2062 6563 6175 7365 2070 742e  now, because pt.
+00014ee0: 7374 6163 6b20 696e 2067 6574 5f73 7570  stack in get_sup
+00014ef0: 706f 7274 5f73 6861 7065 2066 6169 6c73  port_shape fails
+00014f00: 0a20 2020 2020 2020 2020 2020 2023 2065  .            # e
+00014f10: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00014f20: 2023 2020 2020 2073 7570 706f 7274 5f73   #     support_s
+00014f30: 6861 7065 203d 2028 2920 2320 6265 6361  hape = () # beca
+00014f40: 7573 6520 6974 2773 206a 7573 7420 6120  use it's just a 
+00014f50: 4e6f 726d 616c 2069 6e20 7468 6174 2063  Normal in that c
+00014f60: 6173 650a 2020 2020 2020 2020 7375 7070  ase.        supp
+00014f70: 6f72 745f 7368 6170 6520 3d20 7074 2e61  ort_shape = pt.a
+00014f80: 735f 7465 6e73 6f72 5f76 6172 6961 626c  s_tensor_variabl
+00014f90: 6528 696e 7458 2873 7570 706f 7274 5f73  e(intX(support_s
+00014fa0: 6861 7065 2929 0a0a 2020 2020 2020 2020  hape))..        
+00014fb0: 6173 7365 7274 206e 5f7a 6572 6f73 756d  assert n_zerosum
+00014fc0: 5f61 7865 7320 3d3d 2070 742e 6765 745f  _axes == pt.get_
+00014fd0: 7665 6374 6f72 5f6c 656e 6774 6828 0a20  vector_length(. 
+00014fe0: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+00014ff0: 7274 5f73 6861 7065 0a20 2020 2020 2020  rt_shape.       
+00015000: 2029 2c20 2273 7570 706f 7274 5f73 6861   ), "support_sha
+00015010: 7065 2068 6173 2074 6f20 6265 2061 7320  pe has to be as 
+00015020: 6c6f 6e67 2061 7320 6e5f 7a65 726f 7375  long as n_zerosu
+00015030: 6d5f 6178 6573 220a 0a20 2020 2020 2020  m_axes"..       
+00015040: 2072 6574 7572 6e20 7375 7065 7228 292e   return super().
+00015050: 6469 7374 280a 2020 2020 2020 2020 2020  dist(.          
+00015060: 2020 5b73 6967 6d61 5d2c 206e 5f7a 6572    [sigma], n_zer
+00015070: 6f73 756d 5f61 7865 733d 6e5f 7a65 726f  osum_axes=n_zero
+00015080: 7375 6d5f 6178 6573 2c20 7375 7070 6f72  sum_axes, suppor
+00015090: 745f 7368 6170 653d 7375 7070 6f72 745f  t_shape=support_
+000150a0: 7368 6170 652c 202a 2a6b 7761 7267 730a  shape, **kwargs.
+000150b0: 2020 2020 2020 2020 290a 0a20 2020 2040          )..    @
+000150c0: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+000150d0: 6465 6620 6368 6563 6b5f 7a65 726f 7375  def check_zerosu
+000150e0: 6d5f 6178 6573 2863 6c73 2c20 6e5f 7a65  m_axes(cls, n_ze
+000150f0: 726f 7375 6d5f 6178 6573 3a20 4f70 7469  rosum_axes: Opti
+00015100: 6f6e 616c 5b69 6e74 5d29 202d 3e20 696e  onal[int]) -> in
+00015110: 743a 0a20 2020 2020 2020 2069 6620 6e5f  t:.        if n_
+00015120: 7a65 726f 7375 6d5f 6178 6573 2069 7320  zerosum_axes is 
+00015130: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00015140: 2020 6e5f 7a65 726f 7375 6d5f 6178 6573    n_zerosum_axes
+00015150: 203d 2031 0a20 2020 2020 2020 2069 6620   = 1.        if 
+00015160: 6e6f 7420 6973 696e 7374 616e 6365 286e  not isinstance(n
+00015170: 5f7a 6572 6f73 756d 5f61 7865 732c 2069  _zerosum_axes, i
+00015180: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00015190: 2072 6169 7365 2054 7970 6545 7272 6f72   raise TypeError
+000151a0: 2822 6e5f 7a65 726f 7375 6d5f 6178 6573  ("n_zerosum_axes
+000151b0: 2068 6173 2074 6f20 6265 2061 6e20 696e   has to be an in
+000151c0: 7465 6765 7222 290a 2020 2020 2020 2020  teger").        
+000151d0: 6966 206e 6f74 206e 5f7a 6572 6f73 756d  if not n_zerosum
+000151e0: 5f61 7865 7320 3e20 303a 0a20 2020 2020  _axes > 0:.     
+000151f0: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00015200: 7565 4572 726f 7228 226e 5f7a 6572 6f73  ueError("n_zeros
+00015210: 756d 5f61 7865 7320 6861 7320 746f 2062  um_axes has to b
+00015220: 6520 3e20 3022 290a 2020 2020 2020 2020  e > 0").        
+00015230: 7265 7475 726e 206e 5f7a 6572 6f73 756d  return n_zerosum
+00015240: 5f61 7865 730a 0a20 2020 2040 636c 6173  _axes..    @clas
+00015250: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00015260: 7276 5f6f 7028 636c 732c 2073 6967 6d61  rv_op(cls, sigma
+00015270: 2c20 6e5f 7a65 726f 7375 6d5f 6178 6573  , n_zerosum_axes
+00015280: 2c20 7375 7070 6f72 745f 7368 6170 652c  , support_shape,
+00015290: 2073 697a 653d 4e6f 6e65 293a 0a20 2020   size=None):.   
+000152a0: 2020 2020 2073 6861 7065 203d 2074 6f5f       shape = to_
+000152b0: 7475 706c 6528 7369 7a65 2920 2b20 7475  tuple(size) + tu
+000152c0: 706c 6528 7375 7070 6f72 745f 7368 6170  ple(support_shap
+000152d0: 6529 0a20 2020 2020 2020 206e 6f72 6d61  e).        norma
+000152e0: 6c5f 6469 7374 203d 2070 6d2e 4e6f 726d  l_dist = pm.Norm
+000152f0: 616c 2e64 6973 7428 7369 676d 613d 7369  al.dist(sigma=si
+00015300: 676d 612c 2073 6861 7065 3d73 6861 7065  gma, shape=shape
+00015310: 290a 0a20 2020 2020 2020 2069 6620 6e5f  )..        if n_
+00015320: 7a65 726f 7375 6d5f 6178 6573 203e 206e  zerosum_axes > n
+00015330: 6f72 6d61 6c5f 6469 7374 2e6e 6469 6d3a  ormal_dist.ndim:
+00015340: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00015350: 7365 2056 616c 7565 4572 726f 7228 2253  se ValueError("S
+00015360: 6861 7065 206f 6620 6469 7374 7269 6275  hape of distribu
+00015370: 7469 6f6e 2069 7320 746f 6f20 736d 616c  tion is too smal
+00015380: 6c20 666f 7220 7468 6520 6e75 6d62 6572  l for the number
+00015390: 206f 6620 7a65 726f 7375 6d20 6178 6573   of zerosum axes
+000153a0: 2229 0a0a 2020 2020 2020 2020 6e6f 726d  ")..        norm
+000153b0: 616c 5f64 6973 745f 2c20 7369 676d 615f  al_dist_, sigma_
+000153c0: 2c20 7375 7070 6f72 745f 7368 6170 655f  , support_shape_
+000153d0: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+000153e0: 206e 6f72 6d61 6c5f 6469 7374 2e74 7970   normal_dist.typ
+000153f0: 6528 292c 0a20 2020 2020 2020 2020 2020  e(),.           
+00015400: 2073 6967 6d61 2e74 7970 6528 292c 0a20   sigma.type(),. 
+00015410: 2020 2020 2020 2020 2020 2073 7570 706f             suppo
+00015420: 7274 5f73 6861 7065 2e74 7970 6528 292c  rt_shape.type(),
+00015430: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
+00015440: 2020 2020 2320 5a65 726f 7375 6d2d 6e6f      # Zerosum-no
+00015450: 726d 616c 696e 6720 6973 2061 6368 6965  rmaling is achie
+00015460: 7665 6420 6279 2073 7562 7472 6163 7469  ved by subtracti
+00015470: 6e67 2074 6865 206d 6561 6e20 616c 6f6e  ng the mean alon
+00015480: 6720 7468 6520 6769 7665 6e20 6e5f 7a65  g the given n_ze
+00015490: 726f 7375 6d5f 6178 6573 0a20 2020 2020  rosum_axes.     
+000154a0: 2020 207a 6572 6f73 756d 5f72 765f 203d     zerosum_rv_ =
+000154b0: 206e 6f72 6d61 6c5f 6469 7374 5f0a 2020   normal_dist_.  
+000154c0: 2020 2020 2020 666f 7220 6178 6973 2069        for axis i
+000154d0: 6e20 7261 6e67 6528 6e5f 7a65 726f 7375  n range(n_zerosu
+000154e0: 6d5f 6178 6573 293a 0a20 2020 2020 2020  m_axes):.       
+000154f0: 2020 2020 207a 6572 6f73 756d 5f72 765f       zerosum_rv_
+00015500: 202d 3d20 7a65 726f 7375 6d5f 7276 5f2e   -= zerosum_rv_.
+00015510: 6d65 616e 2861 7869 733d 2d61 7869 7320  mean(axis=-axis 
+00015520: 2d20 312c 206b 6565 7064 696d 733d 5472  - 1, keepdims=Tr
+00015530: 7565 290a 0a20 2020 2020 2020 2072 6574  ue)..        ret
+00015540: 7572 6e20 5a65 726f 5375 6d4e 6f72 6d61  urn ZeroSumNorma
+00015550: 6c52 5628 0a20 2020 2020 2020 2020 2020  lRV(.           
+00015560: 2069 6e70 7574 733d 5b6e 6f72 6d61 6c5f   inputs=[normal_
+00015570: 6469 7374 5f2c 2073 6967 6d61 5f2c 2073  dist_, sigma_, s
+00015580: 7570 706f 7274 5f73 6861 7065 5f5d 2c0a  upport_shape_],.
+00015590: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+000155a0: 7574 733d 5b7a 6572 6f73 756d 5f72 765f  uts=[zerosum_rv_
+000155b0: 2c20 7375 7070 6f72 745f 7368 6170 655f  , support_shape_
+000155c0: 5d2c 0a20 2020 2020 2020 2020 2020 206e  ],.            n
+000155d0: 6469 6d5f 7375 7070 3d6e 5f7a 6572 6f73  dim_supp=n_zeros
+000155e0: 756d 5f61 7865 732c 0a20 2020 2020 2020  um_axes,.       
+000155f0: 2029 286e 6f72 6d61 6c5f 6469 7374 2c20   )(normal_dist, 
+00015600: 7369 676d 612c 2073 7570 706f 7274 5f73  sigma, support_s
+00015610: 6861 7065 290a 0a0a 405f 6368 616e 6765  hape)...@_change
+00015620: 5f64 6973 745f 7369 7a65 2e72 6567 6973  _dist_size.regis
+00015630: 7465 7228 5a65 726f 5375 6d4e 6f72 6d61  ter(ZeroSumNorma
+00015640: 6c52 5629 0a64 6566 2063 6861 6e67 655f  lRV).def change_
+00015650: 7a65 726f 7375 6d5f 7369 7a65 286f 702c  zerosum_size(op,
+00015660: 206e 6f72 6d61 6c5f 6469 7374 2c20 6e65   normal_dist, ne
+00015670: 775f 7369 7a65 2c20 6578 7061 6e64 3d46  w_size, expand=F
+00015680: 616c 7365 293a 0a20 2020 206e 6f72 6d61  alse):.    norma
+00015690: 6c5f 6469 7374 2c20 7369 676d 612c 2073  l_dist, sigma, s
+000156a0: 7570 706f 7274 5f73 6861 7065 203d 206e  upport_shape = n
+000156b0: 6f72 6d61 6c5f 6469 7374 2e6f 776e 6572  ormal_dist.owner
+000156c0: 2e69 6e70 7574 730a 0a20 2020 2069 6620  .inputs..    if 
+000156d0: 6578 7061 6e64 3a0a 2020 2020 2020 2020  expand:.        
+000156e0: 6f72 6967 696e 616c 5f73 6861 7065 203d  original_shape =
+000156f0: 2074 7570 6c65 286e 6f72 6d61 6c5f 6469   tuple(normal_di
+00015700: 7374 2e73 6861 7065 290a 2020 2020 2020  st.shape).      
+00015710: 2020 6f6c 645f 7369 7a65 203d 206f 7269    old_size = ori
+00015720: 6769 6e61 6c5f 7368 6170 655b 3a20 6c65  ginal_shape[: le
+00015730: 6e28 6f72 6967 696e 616c 5f73 6861 7065  n(original_shape
+00015740: 2920 2d20 6f70 2e6e 6469 6d5f 7375 7070  ) - op.ndim_supp
+00015750: 5d0a 2020 2020 2020 2020 6e65 775f 7369  ].        new_si
+00015760: 7a65 203d 2074 7570 6c65 286e 6577 5f73  ze = tuple(new_s
+00015770: 697a 6529 202b 206f 6c64 5f73 697a 650a  ize) + old_size.
+00015780: 0a20 2020 2072 6574 7572 6e20 5a65 726f  .    return Zero
+00015790: 5375 6d4e 6f72 6d61 6c2e 7276 5f6f 7028  SumNormal.rv_op(
+000157a0: 0a20 2020 2020 2020 2073 6967 6d61 3d73  .        sigma=s
+000157b0: 6967 6d61 2c20 6e5f 7a65 726f 7375 6d5f  igma, n_zerosum_
+000157c0: 6178 6573 3d6f 702e 6e64 696d 5f73 7570  axes=op.ndim_sup
+000157d0: 702c 2073 7570 706f 7274 5f73 6861 7065  p, support_shape
+000157e0: 3d73 7570 706f 7274 5f73 6861 7065 2c20  =support_shape, 
+000157f0: 7369 7a65 3d6e 6577 5f73 697a 650a 2020  size=new_size.  
+00015800: 2020 290a 0a0a 405f 6d6f 6d65 6e74 2e72    )...@_moment.r
+00015810: 6567 6973 7465 7228 5a65 726f 5375 6d4e  egister(ZeroSumN
+00015820: 6f72 6d61 6c52 5629 0a64 6566 207a 6572  ormalRV).def zer
+00015830: 6f73 756d 6e6f 726d 616c 5f6d 6f6d 656e  osumnormal_momen
+00015840: 7428 6f70 2c20 7276 2c20 2a72 765f 696e  t(op, rv, *rv_in
+00015850: 7075 7473 293a 0a20 2020 2072 6574 7572  puts):.    retur
+00015860: 6e20 7074 2e7a 6572 6f73 5f6c 696b 6528  n pt.zeros_like(
+00015870: 7276 290a 0a0a 405f 6465 6661 756c 745f  rv)...@_default_
+00015880: 7472 616e 7366 6f72 6d2e 7265 6769 7374  transform.regist
+00015890: 6572 285a 6572 6f53 756d 4e6f 726d 616c  er(ZeroSumNormal
+000158a0: 5256 290a 6465 6620 7a65 726f 7375 6d5f  RV).def zerosum_
+000158b0: 6465 6661 756c 745f 7472 616e 7366 6f72  default_transfor
+000158c0: 6d28 6f70 2c20 7276 293a 0a20 2020 206e  m(op, rv):.    n
+000158d0: 5f7a 6572 6f73 756d 5f61 7865 7320 3d20  _zerosum_axes = 
+000158e0: 7475 706c 6528 6e70 2e61 7261 6e67 6528  tuple(np.arange(
+000158f0: 2d6f 702e 6e64 696d 5f73 7570 702c 2030  -op.ndim_supp, 0
+00015900: 2929 0a20 2020 2072 6574 7572 6e20 5a65  )).    return Ze
+00015910: 726f 5375 6d54 7261 6e73 666f 726d 286e  roSumTransform(n
+00015920: 5f7a 6572 6f73 756d 5f61 7865 7329 0a0a  _zerosum_axes)..
+00015930: 0a40 5f6c 6f67 7072 6f62 2e72 6567 6973  .@_logprob.regis
+00015940: 7465 7228 5a65 726f 5375 6d4e 6f72 6d61  ter(ZeroSumNorma
+00015950: 6c52 5629 0a64 6566 207a 6572 6f73 756d  lRV).def zerosum
+00015960: 6e6f 726d 616c 5f6c 6f67 7028 6f70 2c20  normal_logp(op, 
+00015970: 7661 6c75 6573 2c20 6e6f 726d 616c 5f64  values, normal_d
+00015980: 6973 742c 2073 6967 6d61 2c20 7375 7070  ist, sigma, supp
+00015990: 6f72 745f 7368 6170 652c 202a 2a6b 7761  ort_shape, **kwa
+000159a0: 7267 7329 3a0a 2020 2020 2876 616c 7565  rgs):.    (value
+000159b0: 2c29 203d 2076 616c 7565 730a 2020 2020  ,) = values.    
+000159c0: 7368 6170 6520 3d20 7661 6c75 652e 7368  shape = value.sh
+000159d0: 6170 650a 2020 2020 6e5f 7a65 726f 7375  ape.    n_zerosu
+000159e0: 6d5f 6178 6573 203d 206f 702e 6e64 696d  m_axes = op.ndim
+000159f0: 5f73 7570 700a 0a20 2020 205f 6465 675f  _supp..    _deg_
+00015a00: 6672 6565 5f73 7570 706f 7274 5f73 6861  free_support_sha
+00015a10: 7065 203d 2070 742e 696e 635f 7375 6274  pe = pt.inc_subt
+00015a20: 656e 736f 7228 7368 6170 655b 2d6e 5f7a  ensor(shape[-n_z
+00015a30: 6572 6f73 756d 5f61 7865 733a 5d2c 202d  erosum_axes:], -
+00015a40: 3129 0a20 2020 205f 6675 6c6c 5f73 697a  1).    _full_siz
+00015a50: 6520 3d20 7074 2e70 726f 6428 7368 6170  e = pt.prod(shap
+00015a60: 6529 0a20 2020 205f 6465 6772 6565 735f  e).    _degrees_
+00015a70: 6f66 5f66 7265 6564 6f6d 203d 2070 742e  of_freedom = pt.
+00015a80: 7072 6f64 285f 6465 675f 6672 6565 5f73  prod(_deg_free_s
+00015a90: 7570 706f 7274 5f73 6861 7065 290a 0a20  upport_shape).. 
+00015aa0: 2020 207a 6572 6f73 756d 7320 3d20 5b0a     zerosums = [.
+00015ab0: 2020 2020 2020 2020 7074 2e61 6c6c 2870          pt.all(p
+00015ac0: 742e 6973 636c 6f73 6528 7074 2e6d 6561  t.isclose(pt.mea
+00015ad0: 6e28 7661 6c75 652c 2061 7869 733d 2d61  n(value, axis=-a
+00015ae0: 7869 7320 2d20 3129 2c20 302c 2061 746f  xis - 1), 0, ato
+00015af0: 6c3d 3165 2d39 2929 0a20 2020 2020 2020  l=1e-9)).       
+00015b00: 2066 6f72 2061 7869 7320 696e 2072 616e   for axis in ran
+00015b10: 6765 286e 5f7a 6572 6f73 756d 5f61 7865  ge(n_zerosum_axe
+00015b20: 7329 0a20 2020 205d 0a0a 2020 2020 6f75  s).    ]..    ou
+00015b30: 7420 3d20 7074 2e73 756d 280a 2020 2020  t = pt.sum(.    
+00015b40: 2020 2020 706d 2e6c 6f67 7028 6e6f 726d      pm.logp(norm
+00015b50: 616c 5f64 6973 742c 2076 616c 7565 2920  al_dist, value) 
+00015b60: 2a20 5f64 6567 7265 6573 5f6f 665f 6672  * _degrees_of_fr
+00015b70: 6565 646f 6d20 2f20 5f66 756c 6c5f 7369  eedom / _full_si
+00015b80: 7a65 2c0a 2020 2020 2020 2020 6178 6973  ze,.        axis
+00015b90: 3d74 7570 6c65 286e 702e 6172 616e 6765  =tuple(np.arange
+00015ba0: 282d 6e5f 7a65 726f 7375 6d5f 6178 6573  (-n_zerosum_axes
+00015bb0: 2c20 3029 292c 0a20 2020 2029 0a0a 2020  , 0)),.    )..  
+00015bc0: 2020 7265 7475 726e 2063 6865 636b 5f70    return check_p
+00015bd0: 6172 616d 6574 6572 7328 6f75 742c 202a  arameters(out, *
+00015be0: 7a65 726f 7375 6d73 2c20 6d73 673d 226d  zerosums, msg="m
+00015bf0: 6561 6e28 7661 6c75 652c 2061 7869 733d  ean(value, axis=
+00015c00: 6e5f 7a65 726f 7375 6d5f 6178 6573 2920  n_zerosum_axes) 
+00015c10: 3d20 3022 290a                           = 0").
```

### Comparing `pymc-5.4.1/pymc/distributions/shape_utils.py` & `pymc-5.5.0/pymc/distributions/shape_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/simulator.py` & `pymc-5.5.0/pymc/distributions/simulator.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/timeseries.py` & `pymc-5.5.0/pymc/distributions/timeseries.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,14 @@
     change_dist_size,
     get_support_shape,
     get_support_shape_1d,
 )
 from pymc.exceptions import NotConstantValueError
 from pymc.logprob.abstract import _logprob
 from pymc.logprob.basic import logp
-from pymc.logprob.utils import ignore_logprob, reconsider_logprob
 from pymc.pytensorf import constant_fold, floatX, intX
 from pymc.util import check_dist_not_registered
 
 __all__ = [
     "RandomWalk",
     "GaussianRandomWalk",
     "MvGaussianRandomWalk",
@@ -107,19 +106,14 @@
                 "init_dist and innovation_dist must have the same support dimensionality"
             )
 
         # We need to check this, because we clone the variables when we ignore their logprob next
         if init_dist in ancestors([innovation_dist]) or innovation_dist in ancestors([init_dist]):
             raise ValueError("init_dist and innovation_dist must be completely independent")
 
-        # PyMC should not be concerned that these variables don't have values, as they will be
-        # accounted for in the logp of RandomWalk
-        init_dist = ignore_logprob(init_dist)
-        innovation_dist = ignore_logprob(innovation_dist)
-
         steps = cls.get_steps(
             innovation_dist=innovation_dist,
             steps=steps,
             shape=kwargs.get("shape"),
             dims=None,
             observed=None,
         )
@@ -231,22 +225,20 @@
     grw_moment = pt.cumsum(grw_moment, axis=0)
     # shape = (B, T, S)
     grw_moment = pt.moveaxis(grw_moment, 0, -op.ndim_supp)
     return grw_moment
 
 
 @_logprob.register(RandomWalkRV)
-def random_walk_logp(op, values, init_dist, innovation_dist, steps, **kwargs):
+def random_walk_logp(op, values, *inputs, **kwargs):
     # Although we can derive the logprob of random walks, it does not collapse
     # what we consider the core dimension of steps. We do it manually here.
     (value,) = values
     # Recreate RV and obtain inner graph
-    rv_node = op.make_node(
-        reconsider_logprob(init_dist), reconsider_logprob(innovation_dist), steps
-    )
+    rv_node = op.make_node(*inputs)
     rv = clone_replace(
         op.inner_outputs, replace={u: v for u, v in zip(op.inner_inputs, rv_node.inputs)}
     )[op.default_output]
     # Obtain logp of the inner graph and collapse steps dimension
     return logp(rv, value).sum(axis=-1)
 
 
@@ -567,17 +559,14 @@
                 "Initial distribution not specified, defaulting to "
                 "`Normal.dist(0, 100, shape=...)`. You can specify an init_dist "
                 "manually to suppress this warning.",
                 UserWarning,
             )
             init_dist = Normal.dist(0, 100, shape=(*sigma.shape, ar_order))
 
-        # We can ignore init_dist, as it will be accounted for in the logp term
-        init_dist = ignore_logprob(init_dist)
-
         return super().dist([rhos, sigma, init_dist, steps, ar_order, constant], **kwargs)
 
     @classmethod
     def _get_ar_order(cls, rhos: TensorVariable, ar_order: Optional[int], constant: bool) -> int:
         """Compute ar_order given inputs
 
         If ar_order is not specified we do constant folding on the shape of rhos
@@ -785,16 +774,14 @@
 
         omega = pt.as_tensor_variable(omega)
         alpha_1 = pt.as_tensor_variable(alpha_1)
         beta_1 = pt.as_tensor_variable(beta_1)
         initial_vol = pt.as_tensor_variable(initial_vol)
 
         init_dist = Normal.dist(0, initial_vol)
-        # We can ignore init_dist, as it will be accounted for in the logp term
-        init_dist = ignore_logprob(init_dist)
 
         return super().dist([omega, alpha_1, beta_1, initial_vol, init_dist, steps], **kwargs)
 
     @classmethod
     def rv_op(cls, omega, alpha_1, beta_1, initial_vol, init_dist, steps, size=None):
         if size is not None:
             batch_size = size
@@ -969,16 +956,14 @@
             warnings.warn(
                 "Initial distribution not specified, defaulting to "
                 "`Normal.dist(0, 100, shape=...)`. You can specify an init_dist "
                 "manually to suppress this warning.",
                 UserWarning,
             )
             init_dist = Normal.dist(0, 100, shape=sde_pars[0].shape)
-        # We can ignore init_dist, as it will be accounted for in the logp term
-        init_dist = ignore_logprob(init_dist)
 
         return super().dist([init_dist, steps, sde_pars, dt, sde_fn], **kwargs)
 
     @classmethod
     def rv_op(cls, init_dist, steps, sde_pars, dt, sde_fn, size=None):
         # Init dist should have shape (*size,)
         if size is not None:
```

### Comparing `pymc-5.4.1/pymc/distributions/transforms.py` & `pymc-5.5.0/pymc/distributions/transforms.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/distributions/truncated.py` & `pymc-5.5.0/pymc/distributions/truncated.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/exceptions.py` & `pymc-5.5.0/pymc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/func_utils.py` & `pymc-5.5.0/pymc/func_utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/gp/__init__.py` & `pymc-5.5.0/pymc/gp/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/gp/cov.py` & `pymc-5.5.0/pymc/gp/cov.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/gp/gp.py` & `pymc-5.5.0/pymc/gp/gp.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/gp/hsgp_approx.py` & `pymc-5.5.0/pymc/gp/hsgp_approx.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/gp/mean.py` & `pymc-5.5.0/pymc/gp/mean.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/gp/util.py` & `pymc-5.5.0/pymc/gp/util.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/initial_point.py` & `pymc-5.5.0/pymc/initial_point.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/logprob/__init__.py` & `pymc-5.5.0/pymc/logprob/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,21 @@
 #   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
 
-from pymc.logprob.basic import factorized_joint_logprob, icdf, joint_logp, logcdf, logp
+from pymc.logprob.basic import (
+    conditional_logp,
+    icdf,
+    logcdf,
+    logp,
+    transformed_conditional_logp,
+)
 
 # isort: off
 # Add rewrites to the DBs
 import pymc.logprob.binary
 import pymc.logprob.censoring
 import pymc.logprob.cumsum
 import pymc.logprob.checks
```

### Comparing `pymc-5.4.1/pymc/logprob/abstract.py` & `pymc-5.5.0/pymc/logprob/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -30,224 +30,284 @@
 #   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
 
-import abc
+import warnings
 
-from copy import copy
-from functools import singledispatch
-from typing import Callable, List, Sequence, Tuple
-
-from pytensor.graph.basic import Apply, Variable
-from pytensor.graph.op import Op
-from pytensor.graph.utils import MetaType
-from pytensor.tensor import TensorVariable
-from pytensor.tensor.elemwise import Elemwise
+from typing import (
+    Callable,
+    Container,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    Union,
+)
+
+import numpy as np
+
+from pytensor import Variable
+from pytensor import tensor as pt
+from pytensor.graph import Apply, Op
+from pytensor.graph.basic import Constant, clone_get_equiv, graph_inputs, walk
+from pytensor.graph.fg import FunctionGraph
+from pytensor.graph.op import HasInnerGraph
+from pytensor.link.c.type import CType
+from pytensor.raise_op import CheckAndRaise
 from pytensor.tensor.random.op import RandomVariable
+from pytensor.tensor.var import TensorVariable
 
+from pymc.logprob.abstract import MeasurableVariable, _logprob
+from pymc.util import makeiter
 
-@singledispatch
-def _logprob(
-    op: Op,
-    values: Sequence[TensorVariable],
-    *inputs: TensorVariable,
-    **kwargs,
-):
-    """Create a graph for the log-density/mass of a ``RandomVariable``.
 
-    This function dispatches on the type of ``op``, which should be a subclass
-    of ``RandomVariable``.  If you want to implement new density/mass graphs
-    for a ``RandomVariable``, register a new function on this dispatcher.
+def walk_model(
+    graphs: Iterable[TensorVariable],
+    walk_past_rvs: bool = False,
+    stop_at_vars: Optional[Set[TensorVariable]] = None,
+    expand_fn: Callable[[TensorVariable], List[TensorVariable]] = lambda var: [],
+) -> Generator[TensorVariable, None, None]:
+    """Walk model graphs and yield their nodes.
+
+    By default, these walks will not go past ``MeasurableVariable`` nodes.
 
+    Parameters
+    ----------
+    graphs
+        The graphs to walk.
+    walk_past_rvs
+        If ``True``, the walk will not terminate at ``MeasurableVariable``s.
+    stop_at_vars
+        A list of variables at which the walk will terminate.
+    expand_fn
+        A function that returns the next variable(s) to be traversed.
     """
-    raise NotImplementedError(f"Logprob method not implemented for {op}")
+    if stop_at_vars is None:
+        stop_at_vars = set()
 
+    def expand(var: TensorVariable, stop_at_vars=stop_at_vars) -> List[TensorVariable]:
+        new_vars = expand_fn(var)
 
-def _logprob_helper(rv, *values, **kwargs):
-    """Helper that calls `_logprob` dispatcher."""
-    logprob = _logprob(rv.owner.op, values, *rv.owner.inputs, **kwargs)
+        if (
+            var.owner
+            and (walk_past_rvs or not isinstance(var.owner.op, MeasurableVariable))
+            and (var not in stop_at_vars)
+        ):
+            new_vars.extend(reversed(var.owner.inputs))
+
+        return new_vars
+
+    yield from walk(graphs, expand, False)
+
+
+def replace_rvs_in_graphs(
+    graphs: Iterable[TensorVariable],
+    replacement_fn: Callable[
+        [TensorVariable, Dict[TensorVariable, TensorVariable]],
+        Dict[TensorVariable, TensorVariable],
+    ],
+    initial_replacements: Optional[Dict[TensorVariable, TensorVariable]] = None,
+    **kwargs,
+) -> Tuple[TensorVariable, Dict[TensorVariable, TensorVariable]]:
+    """Replace random variables in graphs.
+
+    This will *not* recompute test values.
 
-    for rv in values:
-        if rv.name:
-            logprob.name = f"{rv.name}_logprob"
-            break
+    Parameters
+    ----------
+    graphs
+        The graphs in which random variables are to be replaced.
 
-    return logprob
+    Returns
+    -------
+    A ``tuple`` containing the transformed graphs and a ``dict`` of the
+    replacements that were made.
+    """
+    replacements = {}
+    if initial_replacements:
+        replacements.update(initial_replacements)
 
+    def expand_replace(var: TensorVariable) -> List[TensorVariable]:
+        new_nodes: List[TensorVariable] = []
+        if var.owner and isinstance(var.owner.op, MeasurableVariable):
+            new_nodes.extend(replacement_fn(var, replacements))
+        return new_nodes
 
-@singledispatch
-def _logcdf(
-    op: Op,
-    value: TensorVariable,
-    *inputs: TensorVariable,
-    **kwargs,
-):
-    """Create a graph for the logcdf of a ``RandomVariable``.
+    for var in walk_model(graphs, expand_fn=expand_replace, **kwargs):
+        pass
 
-    This function dispatches on the type of ``op``, which should be a subclass
-    of ``RandomVariable``.  If you want to implement new logcdf graphs
-    for a ``RandomVariable``, register a new function on this dispatcher.
-    """
-    raise NotImplementedError(f"LogCDF method not implemented for {op}")
+    if replacements:
+        inputs = [i for i in graph_inputs(graphs) if not isinstance(i, Constant)]
+        equiv = {k: k for k in replacements.keys()}
+        equiv = clone_get_equiv(inputs, graphs, False, False, equiv)
 
+        fg = FunctionGraph(
+            [equiv[i] for i in inputs],
+            [equiv[o] for o in graphs],
+            clone=False,
+        )
 
-def _logcdf_helper(rv, value, **kwargs):
-    """Helper that calls `_logcdf` dispatcher."""
-    logcdf = _logcdf(rv.owner.op, value, *rv.owner.inputs, name=rv.name, **kwargs)
+        fg.replace_all(replacements.items(), import_missing=True)
 
-    if rv.name:
-        logcdf.name = f"{rv.name}_logcdf"
+        graphs = list(fg.outputs)
 
-    return logcdf
+    return graphs, replacements
 
 
-@singledispatch
-def _icdf(
-    op: Op,
-    value: TensorVariable,
-    *inputs: TensorVariable,
+def rvs_to_value_vars(
+    graphs: Iterable[TensorVariable],
+    initial_replacements: Optional[Dict[TensorVariable, TensorVariable]] = None,
     **kwargs,
-):
-    """Create a graph for the inverse CDF of a `RandomVariable`.
+) -> Tuple[TensorVariable, Dict[TensorVariable, TensorVariable]]:
+    """Replace random variables in graphs with their value variables.
 
-    This function dispatches on the type of `op`, which should be a subclass
-    of `RandomVariable`.
-    """
-    raise NotImplementedError(f"Inverse CDF method not implemented for {op}")
+    This will *not* recompute test values in the resulting graphs.
 
+    Parameters
+    ----------
+    graphs
+        The graphs in which to perform the replacements.
+    initial_replacements
+        A ``dict`` containing the initial replacements to be made.
 
-def _icdf_helper(rv, value, **kwargs):
-    """Helper that calls `_icdf` dispatcher."""
-    rv_icdf = _icdf(rv.owner.op, value, *rv.owner.inputs, **kwargs)
+    """
 
-    if rv.name:
-        rv_icdf.name = f"{rv.name}_icdf"
+    def replace_fn(var, replacements):
+        rv_value_var = replacements.get(var, None)
+        if rv_value_var is not None:
+            replacements[var] = rv_value_var
+            # In case the value variable is itself a graph, we walk it for
+            # potential replacements
+            return [rv_value_var]
+        return []
 
-    return rv_icdf
+    return replace_rvs_in_graphs(graphs, replace_fn, initial_replacements, **kwargs)
 
 
-class MeasurableVariable(abc.ABC):
-    """A variable that can be assigned a measure/log-probability"""
+def convert_indices(indices, entry):
+    if indices and isinstance(entry, CType):
+        rval = indices.pop(0)
+        return rval
+    elif isinstance(entry, slice):
+        return slice(
+            convert_indices(indices, entry.start),
+            convert_indices(indices, entry.stop),
+            convert_indices(indices, entry.step),
+        )
+    else:
+        return entry
 
 
-MeasurableVariable.register(RandomVariable)
+def indices_from_subtensor(idx_list, indices):
+    """Compute a useable index tuple from the inputs of a ``*Subtensor**`` ``Op``."""
+    return tuple(
+        tuple(convert_indices(list(indices), idx) for idx in idx_list) if idx_list else indices
+    )
 
 
-class UnmeasurableMeta(MetaType):
-    def __new__(cls, name, bases, dict):
-        if "id_obj" not in dict:
-            dict["id_obj"] = None
+def check_potential_measurability(
+    inputs: Tuple[TensorVariable], valued_rvs: Container[TensorVariable]
+) -> bool:
+    if any(
+        ancestor_var
+        for ancestor_var in walk_model(
+            inputs,
+            walk_past_rvs=False,
+            stop_at_vars=set(valued_rvs),
+        )
+        if (
+            ancestor_var.owner
+            and isinstance(ancestor_var.owner.op, MeasurableVariable)
+            and ancestor_var not in valued_rvs
+        )
+    ):
+        return True
+    return False
 
-        return super().__new__(cls, name, bases, dict)
 
-    def __eq__(self, other):
-        if isinstance(other, UnmeasurableMeta):
-            return hash(self.id_obj) == hash(other.id_obj)
-        return False
+class ParameterValueError(ValueError):
+    """Exception for invalid parameters values in logprob graphs"""
 
-    def __hash__(self):
-        return hash(self.id_obj)
 
+class CheckParameterValue(CheckAndRaise):
+    """Implements a parameter value check in a logprob graph.
 
-class UnmeasurableVariable(metaclass=UnmeasurableMeta):
-    """
-    id_obj is an attribute, i.e. tuple of length two, of the unmeasurable class object.
-    e.g. id_obj = (NormalRV, noop_measurable_outputs_fn)
+    Raises `ParameterValueError` if the check is not True.
     """
 
+    __props__ = ("msg", "exc_type", "can_be_replaced_by_ninf")
 
-def get_measurable_outputs(op: Op, node: Apply) -> List[Variable]:
-    """Return only the outputs that are measurable."""
-    if isinstance(op, MeasurableVariable):
-        return _get_measurable_outputs(op, node)
-    else:
-        return []
-
+    def __init__(self, msg: str = "", can_be_replaced_by_ninf: bool = False):
+        super().__init__(ParameterValueError, msg)
+        self.can_be_replaced_by_ninf = can_be_replaced_by_ninf
 
-@singledispatch
-def _get_measurable_outputs(op, node):
-    return node.outputs
+    def __str__(self):
+        return f"Check{{{self.msg}}}"
 
 
-@_get_measurable_outputs.register(RandomVariable)
-def _get_measurable_outputs_RandomVariable(op, node):
-    return node.outputs[1:]
+class DiracDelta(Op):
+    """An `Op` that represents a Dirac-delta distribution."""
 
+    __props__ = ("rtol", "atol")
 
-def noop_measurable_outputs_fn(*args, **kwargs):
-    return []
+    def __init__(self, rtol=1e-5, atol=1e-8):
+        self.rtol = rtol
+        self.atol = atol
 
+    def make_node(self, x):
+        x = pt.as_tensor(x)
+        return Apply(self, [x], [x.type()])
 
-def assign_custom_measurable_outputs(
-    node: Apply,
-    measurable_outputs_fn: Callable = noop_measurable_outputs_fn,
-    type_prefix: str = "Unmeasurable",
-) -> Apply:
-    """Assign a custom ``_get_measurable_outputs`` dispatch function to a measurable variable instance.
+    def do_constant_folding(self, fgraph, node):
+        # Without this, the `Op` would be removed from the graph during
+        # canonicalization
+        return False
 
-    The node is cloned and a custom `Op` that's a copy of the original node's
-    `Op` is created.  That custom `Op` replaces the old `Op` in the cloned
-    node, and then a custom dispatch implementation is created for the clone
-    `Op` in `_get_measurable_outputs`.
+    def perform(self, node, inp, out):
+        (x,) = inp
+        (z,) = out
+        warnings.warn("DiracDelta is a dummy Op that shouldn't be used in a compiled graph")
+        z[0] = x
 
-    If `measurable_outputs_fn` isn't specified, a no-op is used; the result is
-    a clone of `node` that will effectively be ignored by
-    `factorized_joint_logprob`.
+    def infer_shape(self, fgraph, node, input_shapes):
+        return input_shapes
 
-    Parameters
-    ----------
-    node
-        The node to recreate with a new cloned `Op`.
-    measurable_outputs_fn
-        The function that will be assigned to the new cloned `Op` in the
-        `_get_measurable_outputs` dispatcher.
-        The default is a no-op function (i.e. no measurable outputs)
-    type_prefix
-        The prefix used for the new type's name.
-        The default is ``"Unmeasurable"``, which matches the default
-        ``"measurable_outputs_fn"``.
-    """
 
-    new_node = node.clone()
-    op_type = type(new_node.op)
+MeasurableVariable.register(DiracDelta)
 
-    if op_type in _get_measurable_outputs.registry.keys() and isinstance(op_type, UnmeasurableMeta):
-        if _get_measurable_outputs.registry[op_type] != measurable_outputs_fn:
-            raise ValueError(
-                f"The type {op_type.__name__} with hash value {hash(op_type)} "
-                "has already been dispatched a measurable outputs function."
-            )
-        return node
-
-    new_op_dict = op_type.__dict__.copy()
-    new_op_dict["id_obj"] = (new_node.op, measurable_outputs_fn)
-    new_op_dict.setdefault("original_op_type", op_type)
 
-    new_op_type = type(
-        f"{type_prefix}{op_type.__name__}", (op_type, UnmeasurableVariable), new_op_dict
-    )
-    new_node.op = copy(new_node.op)
-    new_node.op.__class__ = new_op_type
+dirac_delta = DiracDelta()
 
-    _get_measurable_outputs.register(new_op_type)(measurable_outputs_fn)
 
-    return new_node
+@_logprob.register(DiracDelta)
+def diracdelta_logprob(op, values, *inputs, **kwargs):
+    (values,) = values
+    (const_value,) = inputs
+    values, const_value = pt.broadcast_arrays(values, const_value)
+    return pt.switch(pt.isclose(values, const_value, rtol=op.rtol, atol=op.atol), 0.0, -np.inf)
 
 
-class MeasurableElemwise(Elemwise):
-    """Base class for Measurable Elemwise variables"""
+def find_rvs_in_graph(vars: Union[Variable, Sequence[Variable]]) -> Set[Variable]:
+    """Assert that there are no `MeasurableVariable` nodes in a graph."""
 
-    valid_scalar_types: Tuple[MetaType, ...] = ()
+    def expand(r):
+        owner = r.owner
+        if owner:
+            inputs = list(reversed(owner.inputs))
 
-    def __init__(self, scalar_op, *args, **kwargs):
-        if not isinstance(scalar_op, self.valid_scalar_types):
-            raise TypeError(
-                f"scalar_op {scalar_op} is not valid for class {self.__class__}. "
-                f"Acceptable types are {self.valid_scalar_types}"
-            )
-        super().__init__(scalar_op, *args, **kwargs)
+            if isinstance(owner.op, HasInnerGraph):
+                inputs += owner.op.inner_outputs
 
+            return inputs
 
-MeasurableVariable.register(MeasurableElemwise)
+    return {
+        node
+        for node in walk(makeiter(vars), expand, False)
+        if node.owner and isinstance(node.owner.op, (RandomVariable, MeasurableVariable))
+    }
```

### Comparing `pymc-5.4.1/pymc/logprob/basic.py` & `pymc-5.5.0/pymc/logprob/basic.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,62 +36,69 @@
 
 import warnings
 
 from collections import deque
 from typing import Dict, List, Optional, Sequence, Union
 
 import numpy as np
-import pytensor
 import pytensor.tensor as pt
 
 from pytensor import config
 from pytensor.graph.basic import (
     Constant,
     Variable,
     ancestors,
     graph_inputs,
     io_toposort,
 )
 from pytensor.graph.op import compute_test_value
 from pytensor.graph.rewriting.basic import GraphRewriter, NodeRewriter
-from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.var import TensorVariable
 from typing_extensions import TypeAlias
 
 from pymc.logprob.abstract import (
+    MeasurableVariable,
     _icdf_helper,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
-    get_measurable_outputs,
 )
 from pymc.logprob.rewriting import cleanup_ir, construct_ir_fgraph
 from pymc.logprob.transforms import RVTransform, TransformValuesRewrite
-from pymc.logprob.utils import rvs_to_value_vars
+from pymc.logprob.utils import find_rvs_in_graph, rvs_to_value_vars
 
 TensorLike: TypeAlias = Union[Variable, float, np.ndarray]
 
 
-def _warn_rvs_in_inferred_graph(graph: Sequence[TensorVariable]):
+def _find_unallowed_rvs_in_graph(graph):
+    from pymc.data import MinibatchIndexRV
+    from pymc.distributions.simulator import SimulatorRV
+
+    return {
+        rv
+        for rv in find_rvs_in_graph(graph)
+        if not isinstance(rv.owner.op, (SimulatorRV, MinibatchIndexRV))
+    }
+
+
+def _warn_rvs_in_inferred_graph(graph: Union[TensorVariable, Sequence[TensorVariable]]):
     """Issue warning if any RVs are found in graph.
 
     RVs are usually an (implicit) conditional input of the derived probability expression,
     and meant to be replaced by respective value variables before evaluation.
     However, when the IR graph is built, any non-input nodes (including RVs) are cloned,
     breaking the link with the original ones.
     This makes it impossible (or difficult) to replace it by the respective values afterward,
     so we instruct users to do it beforehand.
     """
-    from pymc.testing import assert_no_rvs
 
-    try:
-        assert_no_rvs(graph)
-    except AssertionError:
+    rvs_in_graph = _find_unallowed_rvs_in_graph(graph)
+    if rvs_in_graph:
         warnings.warn(
-            "RandomVariables were found in the derived graph. "
+            f"RandomVariables {rvs_in_graph} were found in the derived graph. "
             "These variables are a clone and do not match the original ones on identity.\n"
             "If you are deriving a quantity that depends on model RVs, use `model.replace_rvs_by_values` first. For example: "
             "`logp(model.replace_rvs_by_values([rv])[0], value)`",
             stacklevel=3,
         )
 
 
@@ -145,23 +152,30 @@
         expr = _icdf_helper(ir_rv, value, **kwargs)
         cleanup_ir([expr])
         if warn_missing_rvs:
             _warn_rvs_in_inferred_graph(expr)
         return expr
 
 
-def factorized_joint_logprob(
+RVS_IN_JOINT_LOGP_GRAPH_MSG = (
+    "Random variables detected in the logp graph: %s.\n"
+    "This can happen when DensityDist logp or Interval transform functions reference nonlocal variables,\n"
+    "or when not all rvs have a corresponding value variable."
+)
+
+
+def conditional_logp(
     rv_values: Dict[TensorVariable, TensorVariable],
     warn_missing_rvs: bool = True,
     ir_rewriter: Optional[GraphRewriter] = None,
     extra_rewrites: Optional[Union[GraphRewriter, NodeRewriter]] = None,
     **kwargs,
 ) -> Dict[TensorVariable, TensorVariable]:
-    r"""Create a map between variables and their log-probabilities such that the
-    sum is their joint log-probability.
+    r"""Create a map between variables and conditional log-probabilities
+    such that the sum is their joint log-probability.
 
     The `rv_values` dictionary specifies a joint probability graph defined by
     pairs of random variables and respective measure-space input parameters
 
     For example, consider the following
 
     .. code-block:: python
@@ -171,49 +185,50 @@
         sigma2_rv = pt.random.invgamma(0.5, 0.5)
         Y_rv = pt.random.normal(0, pt.sqrt(sigma2_rv))
 
     This graph for ``Y_rv`` is equivalent to the following hierarchical model:
 
     .. math::
 
-        \sigma^2 \sim& \operatorname{InvGamma}(0.5, 0.5) \\
-        Y \sim& \operatorname{N}(0, \sigma^2)
+        \Sigma^2 \sim& \operatorname{InvGamma}(0.5, 0.5) \\
+        Y \sim& \operatorname{N}(0, \Sigma)
 
     If we create a value variable for ``Y_rv``, i.e. ``y_vv = pt.scalar("y")``,
-    the graph of ``factorized_joint_logprob({Y_rv: y_vv})`` is equivalent to the
-    conditional probability :math:`\log p(Y = y \mid \sigma^2)`, with a stochastic
+    the graph of ``conditional_logp({Y_rv: y_vv})`` is equivalent to the
+    conditional log-probability :math:`\log p(Y = y \mid \Sigma^2)`, with a stochastic
     ``sigma2_rv``. If we specify a value variable for ``sigma2_rv``, i.e.
-    ``s_vv = pt.scalar("s2")``, then ``factorized_joint_logprob({Y_rv: y_vv, sigma2_rv: s_vv})``
-    yields the joint log-probability of the two variables.
+    ``s_vv = pt.scalar("s2")``, then ``conditional_logp({Y_rv: y_vv, sigma2_rv: s_vv})``
+    yields the conditional log-probabilities of the two variables.
+    The sum of the two terms gives their joint log-probability.
 
     .. math::
 
-        \log p(Y = y, \sigma^2 = s) =
-            \log p(Y = y \mid \sigma^2 = s) + \log p(\sigma^2 = s)
+        \log p(Y = y, \Sigma^2 = \sigma^2) =
+            \log p(Y = y \mid \Sigma^2 = \sigma^2) + \log p(\Sigma^2 = \sigma^2)
 
 
     Parameters
     ----------
     rv_values
         A ``dict`` of variables that maps stochastic elements
         (e.g. `RandomVariable`\s) to symbolic `Variable`\s representing their
         values in a log-probability.
     warn_missing_rvs
         When ``True``, issue a warning when a `RandomVariable` is found in
-        the graph and doesn't have a corresponding value variable specified in
+        the logp graph and doesn't have a corresponding value variable specified in
         `rv_values`.
     ir_rewriter
         Rewriter that produces the intermediate representation of Measurable Variables.
     extra_rewrites
         Extra rewrites to be applied (e.g. reparameterizations, transforms,
         etc.)
 
     Returns
     -------
-    A ``dict`` that maps each value variable to the log-probability factor derived
+    A ``dict`` that maps each value variable to the conditional log-probability term derived
     from the respective `RandomVariable`.
 
     """
     fgraph, rv_values, _ = construct_ir_fgraph(rv_values, ir_rewriter=ir_rewriter)
 
     if extra_rewrites is not None:
         extra_rewrites.rewrite(fgraph)
@@ -250,68 +265,56 @@
             if (not isinstance(v, Constant) and v not in replacements)
         }
     )
 
     # Walk the graph from its inputs to its outputs and construct the
     # log-probability
     q = deque(fgraph.toposort())
-
     logprob_vars = {}
 
     while q:
         node = q.popleft()
 
-        outputs = get_measurable_outputs(node.op, node)
-
-        if not outputs:
-            continue
-
-        if any(o not in updated_rv_values for o in outputs):
-            if warn_missing_rvs:
-                warnings.warn(
-                    "Found a random variable that was neither among the observations "
-                    f"nor the conditioned variables: {outputs}.\n"
-                    "This variables is a clone and does not match the original one on identity."
-                )
+        if not isinstance(node.op, MeasurableVariable):
             continue
 
-        q_value_vars = [replacements[q_rv_var] for q_rv_var in outputs]
+        q_values = [replacements[q_rv] for q_rv in node.outputs if q_rv in updated_rv_values]
 
-        if not q_value_vars:
+        if not q_values:
             continue
 
         # Replace `RandomVariable`s in the inputs with value variables.
         # Also, store the results in the `replacements` map for the nodes
         # that follow.
         remapped_vars, _ = rvs_to_value_vars(
-            q_value_vars + list(node.inputs),
+            q_values + list(node.inputs),
             initial_replacements=replacements,
         )
-        q_value_vars = remapped_vars[: len(q_value_vars)]
-        q_rv_inputs = remapped_vars[len(q_value_vars) :]
+        q_values = remapped_vars[: len(q_values)]
+        q_rv_inputs = remapped_vars[len(q_values) :]
 
         q_logprob_vars = _logprob(
             node.op,
-            q_value_vars,
+            q_values,
             *q_rv_inputs,
             **kwargs,
         )
 
         if not isinstance(q_logprob_vars, (list, tuple)):
             q_logprob_vars = [q_logprob_vars]
 
-        for q_value_var, q_logprob_var in zip(q_value_vars, q_logprob_vars):
+        for q_value_var, q_logprob_var in zip(q_values, q_logprob_vars):
             q_value_var = original_values[q_value_var]
 
             if q_value_var.name:
                 q_logprob_var.name = f"{q_value_var.name}_logprob"
 
             if q_value_var in logprob_vars:
                 raise ValueError(
-                    f"More than one logprob factor was assigned to the value var {q_value_var}"
+                    f"More than one logprob term was assigned to the value var {q_value_var}"
                 )
 
             logprob_vars[q_value_var] = q_logprob_var
 
         # Recompute test values for the changes introduced by the
         # replacements above.
         if config.compute_test_value != "off":
@@ -320,73 +323,83 @@
 
     missing_value_terms = set(original_values.values()) - set(logprob_vars.keys())
     if missing_value_terms:
         raise RuntimeError(
             f"The logprob terms of the following value variables could not be derived: {missing_value_terms}"
         )
 
-    cleanup_ir(logprob_vars.values())
-
-    return logprob_vars
+    logprob_expressions = list(logprob_vars.values())
+    cleanup_ir(logprob_expressions)
 
+    if warn_missing_rvs:
+        rvs_in_logp_expressions = _find_unallowed_rvs_in_graph(logprob_expressions)
+        if rvs_in_logp_expressions:
+            warnings.warn(RVS_IN_JOINT_LOGP_GRAPH_MSG % rvs_in_logp_expressions, UserWarning)
 
-def _check_no_rvs(logp_terms: Sequence[TensorVariable]):
-    # Raise if there are unexpected RandomVariables in the logp graph
-    # Only SimulatorRVs MinibatchIndexRVs are allowed
-    from pymc.data import MinibatchIndexRV
-    from pymc.distributions.simulator import SimulatorRV
-
-    unexpected_rv_nodes = [
-        node
-        for node in pytensor.graph.ancestors(logp_terms)
-        if (
-            node.owner
-            and isinstance(node.owner.op, RandomVariable)
-            and not isinstance(node.owner.op, (SimulatorRV, MinibatchIndexRV))
-        )
-    ]
-    if unexpected_rv_nodes:
-        raise ValueError(
-            f"Random variables detected in the logp graph: {unexpected_rv_nodes}.\n"
-            "This can happen when DensityDist logp or Interval transform functions "
-            "reference nonlocal variables."
-        )
+    return logprob_vars
 
 
-def joint_logp(
+def transformed_conditional_logp(
     rvs: Sequence[TensorVariable],
     *,
     rvs_to_values: Dict[TensorVariable, TensorVariable],
     rvs_to_transforms: Dict[TensorVariable, RVTransform],
     jacobian: bool = True,
     **kwargs,
 ) -> List[TensorVariable]:
-    """Thin wrapper around pymc.logprob.factorized_joint_logprob, extended with Model
-    specific concerns such as transforms, jacobian, and scaling"""
+    """Thin wrapper around conditional_logprob, which creates a value transform rewrite.
+
+    This helper will only return the subset of logprob terms corresponding to `rvs`.
+    All rvs_to_values and rvs_to_transforms mappings are required.
+    """
 
     transform_rewrite = None
     values_to_transforms = {
         rvs_to_values[rv]: transform
         for rv, transform in rvs_to_transforms.items()
         if transform is not None
     }
     if values_to_transforms:
         # There seems to be an incorrect type hint in TransformValuesRewrite
         transform_rewrite = TransformValuesRewrite(values_to_transforms)  # type: ignore
 
-    temp_logp_terms = factorized_joint_logprob(
+    kwargs.setdefault("warn_missing_rvs", False)
+    temp_logp_terms = conditional_logp(
         rvs_to_values,
         extra_rewrites=transform_rewrite,
         use_jacobian=jacobian,
         **kwargs,
     )
 
     # The function returns the logp for every single value term we provided to it.
     # This includes the extra values we plugged in above, so we filter those we
     # actually wanted in the same order they were given in.
     logp_terms = {}
     for rv in rvs:
         value_var = rvs_to_values[rv]
         logp_terms[value_var] = temp_logp_terms[value_var]
 
-    _check_no_rvs(list(logp_terms.values()))
-    return list(logp_terms.values())
+    logp_terms_list = list(logp_terms.values())
+
+    rvs_in_logp_expressions = _find_unallowed_rvs_in_graph(logp_terms_list)
+    if rvs_in_logp_expressions:
+        raise ValueError(RVS_IN_JOINT_LOGP_GRAPH_MSG % rvs_in_logp_expressions)
+
+    return logp_terms_list
+
+
+def factorized_joint_logprob(*args, **kwargs):
+    warnings.warn(
+        "`factorized_joint_logprob` was renamed to `conditional_logp`. "
+        "The function will be removed in a future release",
+        FutureWarning,
+    )
+    return conditional_logp(*args, **kwargs)
+
+
+def joint_logp(*args, **kwargs):
+    warnings.warn(
+        "`joint_logp` was renamed to `transformed_conditional_logp`. "
+        "The function will be removed in a future release",
+        FutureWarning,
+    )
+    return transformed_conditional_logp(*args, **kwargs)
```

### Comparing `pymc-5.4.1/pymc/logprob/censoring.py` & `pymc-5.5.0/pymc/logprob/censoring.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,22 +43,17 @@
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.rewriting.basic import node_rewriter
 from pytensor.scalar.basic import Ceil, Clip, Floor, RoundHalfToEven
 from pytensor.scalar.basic import clip as scalar_clip
 from pytensor.tensor.math import ceil, clip, floor, round_half_to_even
 from pytensor.tensor.var import TensorConstant
 
-from pymc.logprob.abstract import (
-    MeasurableElemwise,
-    MeasurableVariable,
-    _logcdf,
-    _logprob,
-)
-from pymc.logprob.rewriting import measurable_ir_rewrites_db
-from pymc.logprob.utils import CheckParameterValue, ignore_logprob
+from pymc.logprob.abstract import MeasurableElemwise, _logcdf, _logprob
+from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
+from pymc.logprob.utils import CheckParameterValue
 
 
 class MeasurableClip(MeasurableElemwise):
     """A placeholder used to specify a log-likelihood for a clipped RV sub-graph."""
 
     valid_scalar_types = (Clip,)
 
@@ -66,44 +61,30 @@
 measurable_clip = MeasurableClip(scalar_clip)
 
 
 @node_rewriter(tracks=[clip])
 def find_measurable_clips(fgraph: FunctionGraph, node: Node) -> Optional[List[MeasurableClip]]:
     # TODO: Canonicalize x[x>ub] = ub -> clip(x, x, ub)
 
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    if isinstance(node.op, MeasurableClip):
-        return None  # pragma: no cover
+    if not rv_map_feature.request_measurable(node.inputs):
+        return None
 
-    clipped_var = node.outputs[0]
     base_var, lower_bound, upper_bound = node.inputs
 
-    if not (
-        base_var.owner
-        and isinstance(base_var.owner.op, MeasurableVariable)
-        and base_var not in rv_map_feature.rv_values
-    ):
-        return None
-
     # Replace bounds by `+-inf` if `y = clip(x, x, ?)` or `y=clip(x, ?, x)`
     # This is used in `clip_logprob` to generate a more succinct logprob graph
     # for one-sided clipped random variables
     lower_bound = lower_bound if (lower_bound is not base_var) else pt.constant(-np.inf)
     upper_bound = upper_bound if (upper_bound is not base_var) else pt.constant(np.inf)
 
-    # Make base_var unmeasurable
-    unmeasurable_base_var = ignore_logprob(base_var)
-    clipped_rv_node = measurable_clip.make_node(unmeasurable_base_var, lower_bound, upper_bound)
-    clipped_rv = clipped_rv_node.outputs[0]
-
-    clipped_rv.name = clipped_var.name
-
+    clipped_rv = measurable_clip.make_node(base_var, lower_bound, upper_bound).outputs[0]
     return [clipped_rv]
 
 
 measurable_ir_rewrites_db.register(
     "find_measurable_clips",
     find_measurable_clips,
     "basic",
@@ -173,39 +154,25 @@
     """A placeholder used to specify a log-likelihood for a clipped RV sub-graph."""
 
     valid_scalar_types = (RoundHalfToEven, Floor, Ceil)
 
 
 @node_rewriter(tracks=[ceil, floor, round_half_to_even])
 def find_measurable_roundings(fgraph: FunctionGraph, node: Node) -> Optional[List[MeasurableRound]]:
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    if isinstance(node.op, MeasurableRound):
-        return None  # pragma: no cover
-
-    (rounded_var,) = node.outputs
-    (base_var,) = node.inputs
-
-    if not (
-        base_var.owner
-        and isinstance(base_var.owner.op, MeasurableVariable)
-        and base_var not in rv_map_feature.rv_values
-        # Rounding only makes sense for continuous variables
-        and base_var.dtype.startswith("float")
-    ):
+    if not rv_map_feature.request_measurable(node.inputs):
         return None
 
-    # Make base_var unmeasurable
-    unmeasurable_base_var = ignore_logprob(base_var)
-
+    [base_var] = node.inputs
     rounded_op = MeasurableRound(node.op.scalar_op)
-    rounded_rv = rounded_op.make_node(unmeasurable_base_var).default_output()
-    rounded_rv.name = rounded_var.name
+    rounded_rv = rounded_op.make_node(base_var).default_output()
+    rounded_rv.name = node.outputs[0].name
     return [rounded_rv]
 
 
 measurable_ir_rewrites_db.register(
     "find_measurable_roundings",
     find_measurable_roundings,
     "basic",
```

### Comparing `pymc-5.4.1/pymc/logprob/checks.py` & `pymc-5.5.0/pymc/logprob/checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,20 +35,19 @@
 #   SOFTWARE.
 
 from typing import List, Optional
 
 import pytensor.tensor as pt
 
 from pytensor.graph.rewriting.basic import node_rewriter
-from pytensor.raise_op import CheckAndRaise, ExceptionType
+from pytensor.raise_op import CheckAndRaise
 from pytensor.tensor.shape import SpecifyShape
 
 from pymc.logprob.abstract import MeasurableVariable, _logprob, _logprob_helper
 from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
-from pymc.logprob.utils import ignore_logprob
 
 
 class MeasurableSpecifyShape(SpecifyShape):
     """A placeholder used to specify a log-likelihood for a specify-shape sub-graph."""
 
 
 MeasurableVariable.register(MeasurableSpecifyShape)
@@ -82,18 +81,15 @@
         base_rv.owner
         and isinstance(base_rv.owner.op, MeasurableVariable)
         and base_rv not in rv_map_feature.rv_values
     ):
         return None  # pragma: no cover
 
     new_op = MeasurableSpecifyShape()
-    # Make base_var unmeasurable
-    unmeasurable_base_rv = ignore_logprob(base_rv)
-    new_rv = new_op.make_node(unmeasurable_base_rv, *shape).default_output()
-    new_rv.name = rv.name
+    new_rv = new_op.make_node(base_rv, *shape).default_output()
 
     return [new_rv]
 
 
 measurable_ir_rewrites_db.register(
     "find_measurable_specify_shapes",
     find_measurable_specify_shapes,
@@ -106,53 +102,46 @@
     """A placeholder used to specify a log-likelihood for an assert sub-graph."""
 
 
 MeasurableVariable.register(MeasurableCheckAndRaise)
 
 
 @_logprob.register(MeasurableCheckAndRaise)
-def logprob_assert(op, values, inner_rv, *assertion, **kwargs):
+def logprob_check_and_raise(op, values, inner_rv, *assertions, **kwargs):
+    from pymc.pytensorf import replace_rvs_by_values
+
     (value,) = values
     # transfer assertion from rv to value
-    value = op(assertion, value)
+    assertions = replace_rvs_by_values(assertions, rvs_to_values={inner_rv: value})
+    value = op(value, *assertions)
     return _logprob_helper(inner_rv, value)
 
 
 @node_rewriter([CheckAndRaise])
-def find_measurable_asserts(fgraph, node) -> Optional[List[MeasurableCheckAndRaise]]:
+def find_measurable_check_and_raise(fgraph, node) -> Optional[List[MeasurableCheckAndRaise]]:
     r"""Finds `AssertOp`\s for which a `logprob` can be computed."""
 
     if isinstance(node.op, MeasurableCheckAndRaise):
         return None  # pragma: no cover
 
     rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    rv = node.outputs[0]
-
     base_rv, *conds = node.inputs
+    if not rv_map_feature.request_measurable([base_rv]):
+        return None
 
-    if not (
-        base_rv.owner
-        and isinstance(base_rv.owner.op, MeasurableVariable)
-        and base_rv not in rv_map_feature.rv_values
-    ):
-        return None  # pragma: no cover
-
-    exception_type = ExceptionType()
-    new_op = MeasurableCheckAndRaise(exc_type=exception_type)
-    # Make base_var unmeasurable
-    unmeasurable_base_rv = ignore_logprob(base_rv)
-    new_rv = new_op.make_node(unmeasurable_base_rv, *conds).default_output()
-    new_rv.name = rv.name
+    op = node.op
+    new_op = MeasurableCheckAndRaise(exc_type=op.exc_type, msg=op.msg)
+    new_rv = new_op.make_node(base_rv, *conds).default_output()
 
     return [new_rv]
 
 
 measurable_ir_rewrites_db.register(
-    "find_measurable_asserts",
-    find_measurable_asserts,
+    "find_measurable_check_and_raise",
+    find_measurable_check_and_raise,
     "basic",
     "assert",
 )
```

### Comparing `pymc-5.4.1/pymc/logprob/cumsum.py` & `pymc-5.5.0/pymc/logprob/cumsum.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 import pytensor.tensor as pt
 
 from pytensor.graph.rewriting.basic import node_rewriter
 from pytensor.tensor.extra_ops import CumOp
 
 from pymc.logprob.abstract import MeasurableVariable, _logprob, _logprob_helper
 from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
-from pymc.logprob.utils import ignore_logprob
 
 
 class MeasurableCumsum(CumOp):
     """A placeholder used to specify a log-likelihood for a cumsum sub-graph."""
 
 
 MeasurableVariable.register(MeasurableCumsum)
@@ -88,33 +87,25 @@
         return None  # pragma: no cover
 
     rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    rv = node.outputs[0]
-
     base_rv = node.inputs[0]
-    if not (
-        base_rv.owner
-        and isinstance(base_rv.owner.op, MeasurableVariable)
-        and base_rv not in rv_map_feature.rv_values
-    ):
-        return None  # pragma: no cover
 
     # Check that cumsum does not mix dimensions
     if base_rv.ndim > 1 and node.op.axis is None:
         return None
 
+    if not rv_map_feature.request_measurable(node.inputs):
+        return None
+
     new_op = MeasurableCumsum(axis=node.op.axis or 0, mode="add")
-    # Make base_var unmeasurable
-    unmeasurable_base_rv = ignore_logprob(base_rv)
-    new_rv = new_op.make_node(unmeasurable_base_rv).default_output()
-    new_rv.name = rv.name
+    new_rv = new_op.make_node(base_rv).default_output()
 
     return [new_rv]
 
 
 measurable_ir_rewrites_db.register(
     "find_measurable_cumsums",
     find_measurable_cumsums,
```

### Comparing `pymc-5.4.1/pymc/logprob/mixture.py` & `pymc-5.5.0/pymc/logprob/mixture.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,23 +38,17 @@
 
 import pytensor
 import pytensor.tensor as pt
 
 from pytensor.graph.basic import Apply, Constant, Variable
 from pytensor.graph.fg import FunctionGraph
 from pytensor.graph.op import Op, compute_test_value
-from pytensor.graph.rewriting.basic import (
-    EquilibriumGraphRewriter,
-    node_rewriter,
-    pre_greedy_node_rewriter,
-)
+from pytensor.graph.rewriting.basic import node_rewriter, pre_greedy_node_rewriter
 from pytensor.ifelse import IfElse, ifelse
-from pytensor.scalar.basic import Switch
-from pytensor.tensor.basic import Join, MakeVector
-from pytensor.tensor.elemwise import Elemwise
+from pytensor.tensor.basic import Join, MakeVector, switch
 from pytensor.tensor.random.rewriting import (
     local_dimshuffle_rv_lift,
     local_rv_size_lift,
     local_subtensor_rv_lift,
 )
 from pytensor.tensor.shape import shape_tuple
 from pytensor.tensor.subtensor import (
@@ -67,21 +61,22 @@
 )
 from pytensor.tensor.type import TensorType
 from pytensor.tensor.type_other import NoneConst, NoneTypeT, SliceConstant, SliceType
 from pytensor.tensor.var import TensorVariable
 
 from pymc.logprob.abstract import MeasurableVariable, _logprob, _logprob_helper
 from pymc.logprob.rewriting import (
+    PreserveRVMappings,
+    assume_measured_ir_outputs,
     local_lift_DiracDelta,
-    logprob_rewrites_db,
     measurable_ir_rewrites_db,
     subtensor_ops,
 )
 from pymc.logprob.tensor import naive_bcast_rv_lift
-from pymc.logprob.utils import ignore_logprob, ignore_logprob_multiple_vars
+from pymc.logprob.utils import check_potential_measurability
 
 
 def is_newaxis(x):
     return isinstance(x, type(None)) or isinstance(getattr(x, "type", None), NoneTypeT)
 
 
 def expand_indices(
@@ -268,137 +263,100 @@
 
         mixture_rvs = joined_rvs.owner.inputs[1:]
 
     return mixture_rvs, join_axis
 
 
 @node_rewriter(subtensor_ops)
-def mixture_replace(fgraph, node):
+def find_measurable_index_mixture(fgraph, node):
     r"""Identify mixture sub-graphs and replace them with a place-holder `Op`.
 
     The basic idea is to find ``stack(mixture_comps)[I_rv]``, where
     ``mixture_comps`` is a ``list`` of `MeasurableVariable`\s and ``I_rv`` is a
     `MeasurableVariable` with a discrete and finite support.
     From these terms, new terms ``Z_rv[i] = mixture_comps[i][i == I_rv]`` are
     created for each ``i`` in ``enumerate(mixture_comps)``.
     """
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    old_mixture_rv = node.default_output()
-
-    mixture_rvs, join_axis = get_stack_mixture_vars(node)
-
-    # We don't support symbolic join axis
-    if mixture_rvs is None or not isinstance(join_axis, (NoneTypeT, Constant)):
-        return None
-
-    # Check that all components are MeasurableVariables and none is already conditioned on
-    if not all(
-        (
-            rv.owner is not None
-            and isinstance(rv.owner.op, MeasurableVariable)
-            and rv not in rv_map_feature.rv_values
-        )
-        for rv in mixture_rvs
-    ):
-        return None  # pragma: no cover
-
     mixing_indices = node.inputs[1:]
 
     # TODO: Add check / test case for Advanced Boolean indexing
     if isinstance(node.op, (AdvancedSubtensor, AdvancedSubtensor1)):
         # We don't support (non-scalar) integer array indexing as it can pick repeated values,
         # but the Mixture logprob assumes all mixture values are independent
         if any(
             indices.dtype.startswith("int") and sum(1 - b for b in indices.type.broadcastable) > 0
             for indices in mixing_indices
             if not isinstance(indices, SliceConstant)
         ):
             return None
 
-    # We loop through mixture components and collect all the array elements
-    # that belong to each one (by way of their indices).
-    new_mixture_rvs = []
-    for i, component_rv in enumerate(mixture_rvs):
-        # We create custom types for the mixture components and assign them
-        # null `get_measurable_outputs` dispatches so that they aren't
-        # erroneously encountered in places like `factorized_joint_logprob`.
-        new_comp_rv = ignore_logprob(component_rv)
-        new_mixture_rvs.append(new_comp_rv)
+    old_mixture_rv = node.default_output()
+    mixture_rvs, join_axis = get_stack_mixture_vars(node)
+
+    # We don't support symbolic join axis
+    if mixture_rvs is None or not isinstance(join_axis, (NoneTypeT, Constant)):
+        return None
+
+    if rv_map_feature.request_measurable(mixture_rvs) != mixture_rvs:
+        return None
 
     # Replace this sub-graph with a `MixtureRV`
     mix_op = MixtureRV(
         1 + len(mixing_indices),
         old_mixture_rv.dtype,
         old_mixture_rv.broadcastable,
     )
-    new_node = mix_op.make_node(*([join_axis] + mixing_indices + new_mixture_rvs))
+    new_node = mix_op.make_node(*([join_axis] + mixing_indices + mixture_rvs))
 
     new_mixture_rv = new_node.default_output()
 
     if pytensor.config.compute_test_value != "off":
         # We can't use `MixtureRV` to compute a test value; instead, we'll use
         # the original node's test value.
         if not hasattr(old_mixture_rv.tag, "test_value"):
             compute_test_value(node)
 
         new_mixture_rv.tag.test_value = old_mixture_rv.tag.test_value
 
-    if old_mixture_rv.name:
-        new_mixture_rv.name = f"{old_mixture_rv.name}-mixture"
-
     return [new_mixture_rv]
 
 
-@node_rewriter((Elemwise,))
-def switch_mixture_replace(fgraph, node):
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+@node_rewriter([switch])
+def find_measurable_switch_mixture(fgraph, node):
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    if not isinstance(node.op.scalar_op, Switch):
-        return None  # pragma: no cover
-
     old_mixture_rv = node.default_output()
-    # idx, component_1, component_2 = node.inputs
-
-    mixture_rvs = []
+    idx, *components = node.inputs
 
-    for component_rv in node.inputs[1:]:
-        if not (
-            component_rv.owner
-            and isinstance(component_rv.owner.op, MeasurableVariable)
-            and component_rv not in rv_map_feature.rv_values
-        ):
-            return None
-        new_comp_rv = ignore_logprob(component_rv)
-        mixture_rvs.append(new_comp_rv)
+    if rv_map_feature.request_measurable(components) != components:
+        return None
 
     mix_op = MixtureRV(
         2,
         old_mixture_rv.dtype,
         old_mixture_rv.broadcastable,
     )
-    new_node = mix_op.make_node(*([NoneConst, as_nontensor_scalar(node.inputs[0])] + mixture_rvs))
-
-    new_mixture_rv = new_node.default_output()
+    new_mixture_rv = mix_op.make_node(
+        *([NoneConst, as_nontensor_scalar(node.inputs[0])] + components[::-1])
+    ).default_output()
 
     if pytensor.config.compute_test_value != "off":
         if not hasattr(old_mixture_rv.tag, "test_value"):
             compute_test_value(node)
 
         new_mixture_rv.tag.test_value = old_mixture_rv.tag.test_value
 
-    if old_mixture_rv.name:
-        new_mixture_rv.name = f"{old_mixture_rv.name}-mixture"
-
     return [new_mixture_rv]
 
 
 @_logprob.register(MixtureRV)
 def logprob_MixtureRV(
     op, values, *inputs: Optional[Union[TensorVariable, slice]], name=None, **kwargs
 ):
@@ -471,58 +429,96 @@
                 comp_logp,
                 pt.zeros_like(comp_logp),
             )
 
     return logp_val
 
 
-logprob_rewrites_db.register(
-    "mixture_replace",
-    EquilibriumGraphRewriter(
-        [mixture_replace, switch_mixture_replace],
-        max_use_ratio=pytensor.config.optdb__max_use_ratio,
-    ),
+measurable_ir_rewrites_db.register(
+    "find_measurable_index_mixture",
+    find_measurable_index_mixture,
+    "basic",
+    "mixture",
+)
+
+measurable_ir_rewrites_db.register(
+    "find_measurable_switch_mixture",
+    find_measurable_switch_mixture,
     "basic",
     "mixture",
 )
 
 
 class MeasurableIfElse(IfElse):
     """Measurable subclass of IfElse operator."""
 
 
 MeasurableVariable.register(MeasurableIfElse)
 
 
 @node_rewriter([IfElse])
+def useless_ifelse_outputs(fgraph, node):
+    """Remove outputs that are shared across the IfElse branches."""
+    # TODO: This should be a PyTensor canonicalization
+    op = node.op
+    if_var, *inputs = node.inputs
+    shared_inputs = set(inputs[op.n_outs :]).intersection(inputs[: op.n_outs])
+    if not shared_inputs:
+        return None
+
+    replacements = {}
+    for shared_inp in shared_inputs:
+        idx = inputs.index(shared_inp)
+        replacements[node.outputs[idx]] = shared_inp
+
+    # IfElse isn't needed at all
+    if len(shared_inputs) == op.n_outs:
+        return replacements
+
+    # Create subset IfElse with remaining nodes
+    remaining_inputs = [inp for inp in inputs if inp not in shared_inputs]
+    new_outs = (
+        IfElse(n_outs=len(remaining_inputs) // 2).make_node(if_var, *remaining_inputs).outputs
+    )
+    for inp, new_out in zip(remaining_inputs, new_outs):
+        idx = inputs.index(inp)
+        replacements[node.outputs[idx]] = new_out
+
+    return replacements
+
+
+@node_rewriter([IfElse])
 def find_measurable_ifelse_mixture(fgraph, node):
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    if isinstance(node.op, MeasurableIfElse):
+    op = node.op
+    if_var, *base_rvs = node.inputs
+
+    valued_rvs = rv_map_feature.rv_values.keys()
+    if not all(check_potential_measurability([base_var], valued_rvs) for base_var in base_rvs):
         return None
 
-    # Check if all components are unvalued measuarable variables
-    if_var, *base_rvs = node.inputs
+    base_rvs = assume_measured_ir_outputs(valued_rvs, base_rvs)
+    if len(base_rvs) != op.n_outs * 2:
+        return None
+    if not all(var.owner and isinstance(var.owner.op, MeasurableVariable) for var in base_rvs):
+        return None
 
-    if not all(
-        (
-            rv.owner is not None
-            and isinstance(rv.owner.op, MeasurableVariable)
-            and rv not in rv_map_feature.rv_values
-        )
-        for rv in base_rvs
-    ):
-        return None  # pragma: no cover
+    return MeasurableIfElse(n_outs=op.n_outs).make_node(if_var, *base_rvs).outputs
 
-    unmeasurable_base_rvs = ignore_logprob_multiple_vars(base_rvs, rv_map_feature.rv_values)
 
-    return MeasurableIfElse(n_outs=node.op.n_outs).make_node(if_var, *unmeasurable_base_rvs).outputs
+measurable_ir_rewrites_db.register(
+    "useless_ifelse_outputs",
+    useless_ifelse_outputs,
+    "basic",
+    "mixture",
+)
 
 
 measurable_ir_rewrites_db.register(
     "find_measurable_ifelse_mixture",
     find_measurable_ifelse_mixture,
     "basic",
     "mixture",
@@ -547,8 +543,11 @@
     ]
 
     # If the multiple variables depend on each other, we have to replace them
     # by the respective values
     logps_then = replace_rvs_by_values(logps_then, rvs_to_values=rvs_to_values_then)
     logps_else = replace_rvs_by_values(logps_else, rvs_to_values=rvs_to_values_else)
 
-    return ifelse(if_var, logps_then, logps_else)
+    logps = ifelse(if_var, logps_then, logps_else)
+    if len(logps) == 1:
+        return logps[0]
+    return logps
```

### Comparing `pymc-5.4.1/pymc/logprob/rewriting.py` & `pymc-5.5.0/pymc/logprob/rewriting.py`

 * *Files 17% similar despite different names*

```diff
@@ -29,27 +29,42 @@
 #   THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 #   IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 #   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
+import warnings
 
-from typing import Dict, Optional, Sequence, Tuple
+from collections import deque
+from typing import Dict, List, Optional, Sequence, Tuple
 
 import pytensor.tensor as pt
 
+from pytensor import config
 from pytensor.compile.mode import optdb
-from pytensor.graph.basic import Constant, Variable, ancestors
+from pytensor.graph.basic import (
+    Constant,
+    Variable,
+    ancestors,
+    io_toposort,
+    truncated_graph_inputs,
+)
 from pytensor.graph.features import Feature
 from pytensor.graph.fg import FunctionGraph
-from pytensor.graph.rewriting.basic import GraphRewriter, node_rewriter
+from pytensor.graph.replace import clone_replace
+from pytensor.graph.rewriting.basic import (
+    ChangeTracker,
+    EquilibriumGraphRewriter,
+    GraphRewriter,
+    node_rewriter,
+)
 from pytensor.graph.rewriting.db import (
-    EquilibriumDB,
     LocalGroupDB,
+    RewriteDatabase,
     RewriteDatabaseQuery,
     SequenceDB,
     TopoDB,
 )
 from pytensor.tensor.elemwise import DimShuffle, Elemwise
 from pytensor.tensor.extra_ops import BroadcastTo
 from pytensor.tensor.random.rewriting import local_subtensor_rv_lift
@@ -68,26 +83,111 @@
 from pymc.logprob.abstract import MeasurableVariable
 from pymc.logprob.utils import DiracDelta, indices_from_subtensor
 
 inc_subtensor_ops = (IncSubtensor, AdvancedIncSubtensor, AdvancedIncSubtensor1)
 subtensor_ops = (AdvancedSubtensor, AdvancedSubtensor1, Subtensor)
 
 
-class NoCallbackEquilibriumDB(EquilibriumDB):
-    r"""An `EquilibriumDB` that doesn't hide its exceptions.
+class MeasurableEquilibriumGraphRewriter(EquilibriumGraphRewriter):
+    """EquilibriumGraphRewriter focused on IR measurable rewrites.
+
+    This is a stripped down version of the EquilibriumGraphRewriter,
+    which specifically targets nodes in `PreserveRVMAppings.needs_measuring`
+    that are not yet measurable.
+
+    """
+
+    def apply(self, fgraph):
+        rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
+        if not rv_map_feature:
+            return None
+
+        change_tracker = ChangeTracker()
+        fgraph.attach_feature(change_tracker)
+
+        changed = True
+        max_use_abort = False
+        rewriter_name = None
+        global_process_count = {}
+
+        for rewriter in self.global_rewriters + list(self.get_node_rewriters()):
+            global_process_count.setdefault(rewriter, 0)
+
+        while changed and not max_use_abort:
+            changed = False
+            max_nb_nodes = len(fgraph.apply_nodes)
+            max_use = max_nb_nodes * self.max_use_ratio
+
+            # Apply global rewriters
+            for grewrite in self.global_rewriters:
+                change_tracker.reset()
+                grewrite.apply(fgraph)
+                if change_tracker.changed:
+                    global_process_count[grewrite] += 1
+                    changed = True
+                    if global_process_count[grewrite] > max_use:
+                        max_use_abort = True
+                        rewriter_name = getattr(grewrite, "name", None) or getattr(
+                            grewrite, "__name__", ""
+                        )
+
+            # Apply local node rewriters
+            q = deque(io_toposort(fgraph.inputs, fgraph.outputs))
+            while q:
+                node = q.pop()
+                if node not in fgraph.apply_nodes:
+                    continue
+                # This is where we filter only those nodes we care about:
+                # Nodes that have variables that we want to measure and are not yet measurable
+                if isinstance(node.op, MeasurableVariable):
+                    continue
+                if not any(out in rv_map_feature.needs_measuring for out in node.outputs):
+                    continue
+                for node_rewriter in self.node_tracker.get_trackers(node.op):
+                    node_rewriter_change = self.process_node(fgraph, node, node_rewriter)
+                    if not node_rewriter_change:
+                        continue
+                    global_process_count[node_rewriter] += 1
+                    changed = True
+                    if global_process_count[node_rewriter] > max_use:
+                        max_use_abort = True
+                        rewriter_name = getattr(node_rewriter, "name", None) or getattr(
+                            node_rewriter, "__name__", ""
+                        )
+                    # If we converted to a MeasurableVariable we're done here!
+                    if node not in fgraph.apply_nodes or isinstance(node.op, MeasurableVariable):
+                        # go to next node
+                        break
+
+        if max_use_abort:
+            msg = (
+                f"{type(self).__name__} max'ed out by {rewriter_name}."
+                "You can safely raise the current threshold of "
+                f"{config.optdb__max_use_ratio} with the option `optdb__max_use_ratio`."
+            )
+            if config.on_opt_error == "raise":
+                raise AssertionError(msg)
+            else:
+                warnings.warn(msg)
+        fgraph.remove_feature(change_tracker)
+
+
+class MeasurableEquilibriumDB(RewriteDatabase):
+    """A database of rewrites that should be applied until equilibrium is reached.
+
+    This will return a MeasurableEquilibriumGraphRewriter when queried.
 
-    By setting `failure_callback` to ``None`` in the `EquilibriumGraphRewriter`\s
-    that `EquilibriumDB` generates, we're able to directly emit the desired
-    exceptions from within the `NodeRewriter`\s themselves.
     """
 
     def query(self, *tags, **kwtags):
-        res = super().query(*tags, **kwtags)
-        res.failure_callback = None
-        return res
+        rewriters = super().query(*tags, **kwtags)
+        return MeasurableEquilibriumGraphRewriter(
+            rewriters,
+            max_use_ratio=config.optdb__max_use_ratio,
+        )
 
 
 class PreserveRVMappings(Feature):
     r"""Keeps track of random variables and their respective value variables during
     graph rewrites in `rv_values`
 
     When a random variable is replaced in a rewrite, this `Feature` automatically
@@ -112,15 +212,15 @@
         rv_values
             Mappings between random variables and their value variables.
             The keys of this map are what this `Feature` keeps updated.
             The ``dict`` is updated in-place.
         """
         self.rv_values = rv_values
         self.original_values = {v: v for v in rv_values.values()}
-        self.measurable_conversions: Dict[Variable, Variable] = {}
+        self.needs_measuring = set(rv_values.keys())
 
     def on_attach(self, fgraph):
         if hasattr(fgraph, "preserve_rv_mappings"):
             raise ValueError(f"{fgraph} already has the `PreserveRVMappings` feature attached.")
 
         fgraph.preserve_rv_mappings = self
 
@@ -159,22 +259,29 @@
         """
         Whenever a node is replaced during rewrite, we check if it had a value
         variable associated with it and map it to the new node.
         """
         r_value_var = self.rv_values.pop(r, None)
         if r_value_var is not None:
             self.rv_values[new_r] = r_value_var
-        elif (
-            new_r not in self.rv_values
-            and r.owner
-            and new_r.owner
-            and not isinstance(r.owner.op, MeasurableVariable)
-            and isinstance(new_r.owner.op, MeasurableVariable)
-        ):
-            self.measurable_conversions[r] = new_r
+            self.needs_measuring.add(new_r)
+            if new_r.name is None:
+                new_r.name = r.name
+
+    def request_measurable(self, vars: Sequence[Variable]) -> List[Variable]:
+        measurable = []
+        for var in vars:
+            # Input vars or valued vars can't be measured for derived expressions
+            if not var.owner or var in self.rv_values:
+                continue
+            if isinstance(var.owner.op, MeasurableVariable):
+                measurable.append(var)
+            else:
+                self.needs_measuring.add(var)
+        return measurable
 
 
 @register_canonicalize
 @node_rewriter((Elemwise, BroadcastTo, DimShuffle) + subtensor_ops)
 def local_lift_DiracDelta(fgraph, node):
     r"""Lift basic `Op`\s through `DiracDelta`\s."""
 
@@ -218,34 +325,27 @@
 
     In other words, the log-probability for an `*IncSubtensor*` is the log-probability
     of the underlying `RandomVariable` evaluated at ``data`` for the indices
     given by ``idx`` and at the value variable for ``~idx``.
 
     This provides a means of specifying "missing data", for instance.
     """
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    if not isinstance(node.op, inc_subtensor_ops):
-        return None  # pragma: no cover
-
     rv_var = node.outputs[0]
     if rv_var not in rv_map_feature.rv_values:
         return None  # pragma: no cover
 
     base_rv_var = node.inputs[0]
 
-    if not (
-        base_rv_var.owner
-        and isinstance(base_rv_var.owner.op, MeasurableVariable)
-        and base_rv_var not in rv_map_feature.rv_values
-    ):
-        return None  # pragma: no cover
+    if not rv_map_feature.request_measurable([base_rv_var]):
+        return None
 
     data = node.inputs[1]
     idx = indices_from_subtensor(getattr(node.op, "idx_list", None), node.inputs[2:])
 
     # Create a new value variable with the indices `idx` set to `data`
     value_var = rv_map_feature.rv_values[rv_var]
     new_value_var = pt.set_subtensor(value_var[idx], data)
@@ -258,15 +358,15 @@
 logprob_rewrites_db = SequenceDB()
 logprob_rewrites_db.name = "logprob_rewrites_db"
 logprob_rewrites_db.register("pre-canonicalize", optdb.query("+canonicalize"), "basic")
 
 # These rewrites convert un-measurable variables into their measurable forms,
 # but they need to be reapplied, because some of the measurable forms require
 # their inputs to be measurable.
-measurable_ir_rewrites_db = NoCallbackEquilibriumDB()
+measurable_ir_rewrites_db = MeasurableEquilibriumDB()
 measurable_ir_rewrites_db.name = "measurable_ir_rewrites_db"
 
 logprob_rewrites_db.register("measurable_ir_rewrites", measurable_ir_rewrites_db, "basic")
 
 # These rewrites push random/measurable variables "down", making them closer to
 # (or eventually) the graph outputs.  Often this is done by lifting other `Op`s
 # "up" through the random/measurable variables and into their inputs.
@@ -357,19 +457,45 @@
     rv_remapper = PreserveRVMappings(rv_values)
     fgraph.attach_feature(rv_remapper)
 
     if ir_rewriter is None:
         ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))
     ir_rewriter.rewrite(fgraph)
 
-    if rv_remapper.measurable_conversions:
-        # Undo un-valued measurable IR rewrites
-        new_to_old = tuple((v, k) for k, v in reversed(rv_remapper.measurable_conversions.items()))
-        fgraph.replace_all(new_to_old)
-
     return fgraph, rv_values, memo
 
 
 def cleanup_ir(vars: Sequence[Variable]) -> None:
     fgraph = FunctionGraph(outputs=vars, clone=False)
     ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["cleanup"]))
     ir_rewriter.rewrite(fgraph)
+
+
+def assume_measured_ir_outputs(
+    inputs: Sequence[TensorVariable], outputs: Sequence[TensorVariable]
+) -> Sequence[TensorVariable]:
+    """Run IR rewrite assuming each output is measured.
+
+    IR variables could depend on each other in a way that looks unmeasurable without a value variable assigned to each.
+    For instance `join([add(x, z), z])` is a potentially measurable join, but `add(x, z)` can look unmeasurable
+    because neither `x` and `z` are valued in the IR representation.
+    This helper runs an inner ir rewrite after giving each output a dummy value variable.
+    We replace inputs by dummies and then undo it so that any dependency on outer variables is preserved.
+    """
+    # Replace inputs by dummy variables
+    replaced_inputs = {
+        var: var.type()
+        for var in truncated_graph_inputs(outputs, ancestors_to_include=inputs)
+        if var in inputs
+    }
+    cloned_outputs = clone_replace(outputs, replace=replaced_inputs)
+
+    dummy_rv_values = {base_var: base_var.type() for base_var in cloned_outputs}
+    fgraph, *_ = construct_ir_fgraph(dummy_rv_values)
+
+    # Replace dummy variables by inputs
+    fgraph.replace_all(
+        tuple((repl, orig) for orig, repl in replaced_inputs.items()),
+        import_missing=True,
+    )
+
+    return fgraph.outputs
```

### Comparing `pymc-5.4.1/pymc/logprob/scan.py` & `pymc-5.5.0/pymc/logprob/scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 #   FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 #   AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 #   LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 #   OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 #   SOFTWARE.
 
 from copy import copy
-from typing import Callable, Dict, Iterable, List, Tuple, cast
+from typing import Callable, Dict, Iterable, List, Optional, Tuple, cast
 
 import numpy as np
 import pytensor
 import pytensor.tensor as pt
 
 from pytensor.graph.basic import Variable
 from pytensor.graph.op import compute_test_value
@@ -49,22 +49,18 @@
 from pytensor.scan.rewriting import scan_eqopt1, scan_eqopt2
 from pytensor.scan.utils import ScanArgs
 from pytensor.tensor.random.type import RandomType
 from pytensor.tensor.subtensor import Subtensor, indices_from_subtensor
 from pytensor.tensor.var import TensorVariable
 from pytensor.updates import OrderedUpdates
 
-from pymc.logprob.abstract import (
-    MeasurableVariable,
-    _get_measurable_outputs,
-    _logprob,
-    get_measurable_outputs,
-)
-from pymc.logprob.basic import factorized_joint_logprob
+from pymc.logprob.abstract import MeasurableVariable, _logprob
+from pymc.logprob.basic import conditional_logp
 from pymc.logprob.rewriting import (
+    PreserveRVMappings,
     construct_ir_fgraph,
     inc_subtensor_ops,
     logprob_rewrites_db,
     measurable_ir_rewrites_db,
 )
 from pymc.pytensorf import replace_rvs_by_values
 
@@ -310,15 +306,15 @@
     rv_outer_outs = get_random_outer_outputs(scan_args)
 
     var_indices, rv_vars, io_vars = zip(*rv_outer_outs)
     value_map = {_rv: _val for _rv, _val in zip(rv_vars, values)}
 
     def create_inner_out_logp(value_map: Dict[TensorVariable, TensorVariable]) -> TensorVariable:
         """Create a log-likelihood inner-output for a `Scan`."""
-        logp_parts = factorized_joint_logprob(value_map, warn_missing_rvs=False)
+        logp_parts = conditional_logp(value_map, warn_rvs=False)
         return logp_parts.values()
 
     logp_scan_args = convert_outer_out_to_in(
         scan_args,
         rv_vars,
         value_map,
         inner_out_fn=create_inner_out_logp,
@@ -352,66 +348,43 @@
     logp_outputs = logp_scan_out[-len(values) :]
 
     if len(logp_outputs) == 1:
         return logp_outputs[0]
     return logp_outputs
 
 
-@node_rewriter([Scan])
+@node_rewriter([Scan, Subtensor])
 def find_measurable_scans(fgraph, node):
     r"""Find `Scan`\s for which a `logprob` can be computed.
 
     This will convert said `Scan`\s into `MeasurableScan`\s.  It also updates
     random variable and value variable mappings that have been specified for
     parts of a `Scan`\s outputs (e.g. everything except the initial values).
     """
 
-    if not isinstance(node.op, Scan):
-        return None
-
-    if isinstance(node.op, MeasurableScan):
-        return None
-
     if not hasattr(fgraph, "shape_feature"):
         return None  # pragma: no cover
 
-    rv_map_feature = getattr(fgraph, "preserve_rv_mappings", None)
+    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
+    if isinstance(node.op, Subtensor):
+        node = node.inputs[0].owner
+        if not (node and isinstance(node.op, Scan)):
+            return None
+        if isinstance(node.op, MeasurableScan):
+            return None
+
     curr_scanargs = ScanArgs.from_node(node)
 
     # Find the un-output `MeasurableVariable`s created in the inner-graph
-    clients: Dict[Variable, List[Variable]] = {}
-
-    local_fgraph_topo = pytensor.graph.basic.io_toposort(
-        curr_scanargs.inner_inputs,
-        [o for o in curr_scanargs.inner_outputs if not isinstance(o.type, RandomType)],
-        clients=clients,
-    )
-    for n in local_fgraph_topo:
-        if isinstance(n.op, MeasurableVariable):
-            measurable_outputs = get_measurable_outputs(n.op, n)
-            # This variable's source of measure is used by another inner node,
-            # So we don't need it to be an output!
-            if not measurable_outputs:
-                continue
-
-            non_output_node_clients = [
-                c for c in clients[n] if c not in curr_scanargs.inner_outputs
-            ]
-
-            if non_output_node_clients:
-                # This node is a `MeasurableVariable`, but it depends on
-                # variable that's not being output?
-                # TODO: Why can't we make this a `MeasurableScan`?
-                return None
-
     if not any(out in rv_map_feature.rv_values for out in node.outputs):
+        # TODO: T
         # We need to remap user inputs that have been specified in terms of
         # `Subtensor`s of this `Scan`'s node's outputs.
         #
         # For example, the output that the user got was something like
         # `out[1:]` for `outputs_info = [{"initial": x0, "taps": [-1]}]`, so
         # they likely passed `{out[1:]: x_1T_vv}` to `joint_logprob`.
         # Since `out[1:]` isn't really the output of a `Scan`, but a
@@ -507,25 +480,28 @@
         mode=node.op.mode,
     )
     new_node = op.make_node(*curr_scanargs.outer_inputs)
 
     return dict(zip(node.outputs, new_node.outputs))
 
 
-@node_rewriter([Scan])
+@node_rewriter([Scan, Subtensor])
 def add_opts_to_inner_graphs(fgraph, node):
     """Update the `Mode`(s) used to compile the inner-graph of a `Scan` `Op`.
 
     This is how we add the measurable IR rewrites to the "body"
     (i.e. inner-graph) of a `Scan` loop.
     """
 
-    if not isinstance(node.op, Scan):
-        return None
+    if isinstance(node.op, Subtensor):
+        node = node.inputs[0].owner
+        if not (node and isinstance(node.op, Scan)):
+            return None
 
+    # TODO: This might not be needed now that we only target relevant nodes
     # Avoid unnecessarily re-applying this rewrite
     if getattr(node.op.mode, "had_logprob_rewrites", False):
         return None
 
     inner_rv_values = {out: out.type() for out in node.op.inner_outputs}
     ir_rewriter = logprob_rewrites_db.query(RewriteDatabaseQuery(include=["basic"]))
     inner_fgraph, rv_values, _ = construct_ir_fgraph(inner_rv_values, ir_rewriter=ir_rewriter)
@@ -538,40 +514,17 @@
 
     op = Scan(node.op.inner_inputs, new_outputs, node.op.info, mode=new_mode)
     new_node = op.make_node(*node.inputs)
 
     return dict(zip(node.outputs, new_node.outputs))
 
 
-@_get_measurable_outputs.register(MeasurableScan)
-def _get_measurable_outputs_MeasurableScan(op: Scan, node):
-    """Collect measurable outputs for Measurable Scans"""
-    inner_out_from_outer_out_map = op.get_oinp_iinp_iout_oout_mappings()["inner_out_from_outer_out"]
-    inner_outs = op.inner_outputs
-
-    # Measurable scan outputs are those whose inner scan output counterparts are also measurable
-    measurable_outputs = []
-    for out_idx, out in enumerate(node.outputs):
-        [inner_out_idx] = inner_out_from_outer_out_map[out_idx]
-        inner_out = inner_outs[inner_out_idx]
-        inner_out_node = inner_out.owner
-        if isinstance(
-            inner_out_node.op, MeasurableVariable
-        ) and inner_out in get_measurable_outputs(inner_out_node.op, inner_out_node):
-            measurable_outputs.append(out)
-
-    return measurable_outputs
-
-
 measurable_ir_rewrites_db.register(
     "add_opts_to_inner_graphs",
     add_opts_to_inner_graphs,
-    # out2in(
-    #     add_opts_to_inner_graphs, name="add_opts_to_inner_graphs", ignore_newtrees=True
-    # ),
     "basic",
     "scan",
 )
 
 measurable_ir_rewrites_db.register(
     "find_measurable_scans",
     find_measurable_scans,
```

### Comparing `pymc-5.4.1/pymc/logprob/tensor.py` & `pymc-5.5.0/pymc/logprob/tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,20 @@
 from pytensor.tensor.random.op import RandomVariable
 from pytensor.tensor.random.rewriting import (
     local_dimshuffle_rv_lift,
     local_rv_size_lift,
 )
 
 from pymc.logprob.abstract import MeasurableVariable, _logprob, _logprob_helper
-from pymc.logprob.rewriting import PreserveRVMappings, measurable_ir_rewrites_db
-from pymc.logprob.utils import ignore_logprob, ignore_logprob_multiple_vars
+from pymc.logprob.rewriting import (
+    PreserveRVMappings,
+    assume_measured_ir_outputs,
+    measurable_ir_rewrites_db,
+)
+from pymc.logprob.utils import check_potential_measurability
 
 
 @node_rewriter([BroadcastTo])
 def naive_bcast_rv_lift(fgraph, node):
     """Lift a ``BroadcastTo`` through a ``RandomVariable`` ``Op``.
 
     XXX: This implementation simply broadcasts the ``RandomVariable``'s
@@ -198,49 +202,38 @@
 
 @node_rewriter([MakeVector, Join])
 def find_measurable_stacks(
     fgraph, node
 ) -> Optional[List[Union[MeasurableMakeVector, MeasurableJoin]]]:
     r"""Finds `Joins`\s and `MakeVector`\s for which a `logprob` can be computed."""
 
-    if isinstance(node.op, (MeasurableMakeVector, MeasurableJoin)):
-        return None  # pragma: no cover
-
     rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
-    rvs_to_values = rv_map_feature.rv_values
-
-    stack_out = node.outputs[0]
-
     is_join = isinstance(node.op, Join)
 
     if is_join:
         axis, *base_vars = node.inputs
     else:
         base_vars = node.inputs
 
-    if not all(
-        base_var.owner
-        and isinstance(base_var.owner.op, MeasurableVariable)
-        and base_var not in rvs_to_values
-        for base_var in base_vars
-    ):
-        return None  # pragma: no cover
+    valued_rvs = rv_map_feature.rv_values.keys()
+    if not all(check_potential_measurability([base_var], valued_rvs) for base_var in base_vars):
+        return None
 
-    unmeasurable_base_vars = ignore_logprob_multiple_vars(base_vars, rvs_to_values)
+    base_vars = assume_measured_ir_outputs(valued_rvs, base_vars)
+    if not all(var.owner and isinstance(var.owner.op, MeasurableVariable) for var in base_vars):
+        return None
 
     if is_join:
-        measurable_stack = MeasurableJoin()(axis, *unmeasurable_base_vars)
+        measurable_stack = MeasurableJoin()(axis, *base_vars)
     else:
-        measurable_stack = MeasurableMakeVector(node.op.dtype)(*unmeasurable_base_vars)
-
-    measurable_stack.name = stack_out.name
+        measurable_stack = MeasurableMakeVector(node.op.dtype)(*base_vars)
 
     return [measurable_stack]
 
 
 class MeasurableDimShuffle(DimShuffle):
     """A placeholder used to specify a log-likelihood for a dimshuffle sub-graph."""
 
@@ -283,46 +276,38 @@
     return raw_logp.dimshuffle(redo_ds)
 
 
 @node_rewriter([DimShuffle])
 def find_measurable_dimshuffles(fgraph, node) -> Optional[List[MeasurableDimShuffle]]:
     r"""Finds `Dimshuffle`\s for which a `logprob` can be computed."""
 
-    if isinstance(node.op, MeasurableDimShuffle):
-        return None  # pragma: no cover
-
     rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
 
     if rv_map_feature is None:
         return None  # pragma: no cover
 
+    if not rv_map_feature.request_measurable(node.inputs):
+        return None
+
     base_var = node.inputs[0]
 
     # We can only apply this rewrite directly to `RandomVariable`s, as those are
     # the only `Op`s for which we always know the support axis. Other measurable
     # variables can have arbitrary support axes (e.g., if they contain separate
     # `MeasurableDimShuffle`s). Most measurable variables with `DimShuffle`s
     # should still be supported as long as the `DimShuffle`s can be merged/
     # lifted towards the base RandomVariable.
     # TODO: If we include the support axis as meta information in each
     # intermediate MeasurableVariable, we can lift this restriction.
-    if not (
-        base_var.owner
-        and isinstance(base_var.owner.op, RandomVariable)
-        and base_var not in rv_map_feature.rv_values
-    ):
+    if not isinstance(base_var.owner.op, RandomVariable):
         return None  # pragma: no cover
 
-    # Make base_vars unmeasurable
-    base_var = ignore_logprob(base_var)
-
     measurable_dimshuffle = MeasurableDimShuffle(node.op.input_broadcastable, node.op.new_order)(
         base_var
     )
-    measurable_dimshuffle.name = node.outputs[0].name
 
     return [measurable_dimshuffle]
 
 
 measurable_ir_rewrites_db.register("dimshuffle_lift", local_dimshuffle_rv_lift, "basic", "tensor")
```

### Comparing `pymc-5.4.1/pymc/logprob/transforms.py` & `pymc-5.5.0/pymc/logprob/transforms.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,28 +89,27 @@
     true_div,
 )
 from pytensor.tensor.var import TensorVariable
 
 from pymc.logprob.abstract import (
     MeasurableElemwise,
     MeasurableVariable,
-    _get_measurable_outputs,
     _icdf,
     _icdf_helper,
     _logcdf,
     _logcdf_helper,
     _logprob,
     _logprob_helper,
 )
 from pymc.logprob.rewriting import (
     PreserveRVMappings,
     cleanup_ir_rewrites_db,
     measurable_ir_rewrites_db,
 )
-from pymc.logprob.utils import check_potential_measurability, ignore_logprob
+from pymc.logprob.utils import check_potential_measurability
 
 
 class TransformedVariable(Op):
     """A no-op that identifies a transform and its un-transformed input."""
 
     view_map = {0: [0]}
 
@@ -220,15 +219,14 @@
     trans_node.op = new_op
 
     # We now assume that the old value variable represents the *transformed space*.
     # This means that we need to replace all instance of the old value variable
     # with "inversely/un-" transformed versions of itself.
     for rv_var, value_var, transform in zip(rv_vars, value_vars, transforms):
         rv_var_out_idx = node.outputs.index(rv_var)
-        trans_node.outputs[rv_var_out_idx].name = rv_var.name
 
         if transform is None:
             continue
 
         new_value_var = transformed_variable(
             transform.backward(value_var, *trans_node.inputs), value_var
         )
@@ -284,15 +282,14 @@
     trans_node.op = new_op
 
     # We now assume that the old value variable represents the *transformed space*.
     # This means that we need to replace all instance of the old value variable
     # with "inversely/un-" transformed versions of itself.
     for rv_var, value_var, transform in zip(rv_vars, value_vars, transforms):
         rv_var_out_idx = node.outputs.index(rv_var)
-        trans_node.outputs[rv_var_out_idx].name = rv_var.name
 
         if transform is None:
             continue
 
         # We access the original value variable and apply the transform to that
         original_value_var = rv_map_feature.original_values[value_var]
         trans_original_value_var = transform.backward(original_value_var, *trans_node.inputs)
@@ -381,19 +378,14 @@
 
     def __init__(self, *args, transform: RVTransform, measurable_input_idx: int, **kwargs):
         self.transform_elemwise = transform
         self.measurable_input_idx = measurable_input_idx
         super().__init__(*args, **kwargs)
 
 
-@_get_measurable_outputs.register(MeasurableTransform)
-def _get_measurable_outputs_Transform(op, node):
-    return [node.default_output()]
-
-
 @_logprob.register(MeasurableTransform)
 def measurable_transform_logprob(op: MeasurableTransform, values, *inputs, **kwargs):
     """Compute the log-probability graph for a `MeasurabeTransform`."""
     # TODO: Could other rewrites affect the order of inputs?
     (value,) = values
     other_inputs = list(inputs)
     measurable_input = other_inputs.pop(op.measurable_input_idx)
@@ -457,70 +449,33 @@
 
     return icdf
 
 
 @node_rewriter([reciprocal])
 def measurable_reciprocal_to_power(fgraph, node):
     """Convert reciprocal of `MeasurableVariable`s to power."""
-    inp = node.inputs[0]
-    if not (inp.owner and isinstance(inp.owner.op, MeasurableVariable)):
-        return None
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    if rv_map_feature is None:
-        return None  # pragma: no cover
-
-    # Only apply this rewrite if the variable is unvalued
-    if inp in rv_map_feature.rv_values:
-        return None  # pragma: no cover
-
+    [inp] = node.inputs
     return [pt.pow(inp, -1.0)]
 
 
 @node_rewriter([sqr, sqrt])
 def measurable_sqrt_sqr_to_power(fgraph, node):
     """Convert square root or square of `MeasurableVariable`s to power form."""
-
-    inp = node.inputs[0]
-    if not (inp.owner and isinstance(inp.owner.op, MeasurableVariable)):
-        return None
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    if rv_map_feature is None:
-        return None  # pragma: no cover
-
-    # Only apply this rewrite if the variable is unvalued
-    if inp in rv_map_feature.rv_values:
-        return None  # pragma: no cover
+    [inp] = node.inputs
 
     if isinstance(node.op.scalar_op, Sqr):
         return [pt.pow(inp, 2)]
 
     if isinstance(node.op.scalar_op, Sqrt):
         return [pt.pow(inp, 1 / 2)]
 
 
 @node_rewriter([true_div])
 def measurable_div_to_product(fgraph, node):
     """Convert divisions involving `MeasurableVariable`s to products."""
-
-    measurable_vars = [
-        var for var in node.inputs if (var.owner and isinstance(var.owner.op, MeasurableVariable))
-    ]
-    if not measurable_vars:
-        return None  # pragma: no cover
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    if rv_map_feature is None:
-        return None  # pragma: no cover
-
-    # Only apply this rewrite if there is one unvalued MeasurableVariable involved
-    if all(measurable_var in rv_map_feature.rv_values for measurable_var in measurable_vars):
-        return None  # pragma: no cover
-
     numerator, denominator = node.inputs
 
     # Check if numerator is 1
     try:
         if pt.get_scalar_constant_value(numerator) == 1:
             # We convert the denominator directly to a power transform as this
             # must be the measurable input
@@ -531,47 +486,21 @@
     # it might not be measurable (and therefore not needed)
     return [pt.mul(numerator, pt.reciprocal(denominator))]
 
 
 @node_rewriter([neg])
 def measurable_neg_to_product(fgraph, node):
     """Convert negation of `MeasurableVariable`s to product with `-1`."""
-
     inp = node.inputs[0]
-    if not (inp.owner and isinstance(inp.owner.op, MeasurableVariable)):
-        return None
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    if rv_map_feature is None:
-        return None  # pragma: no cover
-
-    # Only apply this rewrite if the variable is unvalued
-    if inp in rv_map_feature.rv_values:
-        return None  # pragma: no cover
-
     return [pt.mul(inp, -1.0)]
 
 
 @node_rewriter([sub])
 def measurable_sub_to_neg(fgraph, node):
     """Convert subtraction involving `MeasurableVariable`s to addition with neg"""
-    measurable_vars = [
-        var for var in node.inputs if (var.owner and isinstance(var.owner.op, MeasurableVariable))
-    ]
-    if not measurable_vars:
-        return None  # pragma: no cover
-
-    rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
-    if rv_map_feature is None:
-        return None  # pragma: no cover
-
-    # Only apply this rewrite if there is one unvalued MeasurableVariable involved
-    if all(measurable_var in rv_map_feature.rv_values for measurable_var in measurable_vars):
-        return None  # pragma: no cover
-
     minuend, subtrahend = node.inputs
     return [pt.add(minuend, pt.neg(subtrahend))]
 
 
 @node_rewriter([exp, log, add, mul, pow, abs, sinh, cosh, tanh, erf, erfc, erfcx])
 def find_measurable_transforms(fgraph: FunctionGraph, node: Node) -> Optional[List[Node]]:
     """Find measurable transformations from Elemwise operators."""
@@ -581,42 +510,32 @@
         return None  # pragma: no cover
 
     rv_map_feature: Optional[PreserveRVMappings] = getattr(fgraph, "preserve_rv_mappings", None)
     if rv_map_feature is None:
         return None  # pragma: no cover
 
     # Check that we have a single source of measurement
-    measurable_inputs = [
-        inp
-        for idx, inp in enumerate(node.inputs)
-        if inp.owner
-        and isinstance(inp.owner.op, MeasurableVariable)
-        and inp not in rv_map_feature.rv_values
-    ]
+    measurable_inputs = rv_map_feature.request_measurable(node.inputs)
 
     if len(measurable_inputs) != 1:
         return None
 
-    measurable_input: TensorVariable = measurable_inputs[0]
+    [measurable_input] = measurable_inputs
 
     # Do not apply rewrite to discrete variables
     if measurable_input.type.dtype.startswith("int"):
         return None
 
     # Check that other inputs are not potentially measurable, in which case this rewrite
     # would be invalid
     other_inputs = tuple(inp for inp in node.inputs if inp is not measurable_input)
 
-    if not check_potential_measurability(other_inputs, rv_map_feature):
+    if check_potential_measurability(other_inputs, rv_map_feature.rv_values.keys()):
         return None
 
-    # Make base_measure outputs unmeasurable
-    # This seems to be the only thing preventing nested rewrites from being erased
-    measurable_input = ignore_logprob(measurable_input)
-
     scalar_op = node.op.scalar_op
     measurable_input_idx = 0
     transform_inputs: Tuple[TensorVariable, ...] = (measurable_input,)
     transform: RVTransform
 
     transform_dict = {
         Exp: ExpTransform(),
@@ -655,16 +574,14 @@
 
     transform_op = MeasurableTransform(
         scalar_op=scalar_op,
         transform=transform,
         measurable_input_idx=measurable_input_idx,
     )
     transform_out = transform_op.make_node(*transform_inputs).default_output()
-    transform_out.name = node.outputs[0].name
-
     return [transform_out]
 
 
 measurable_ir_rewrites_db.register(
     "measurable_reciprocal_to_power",
     measurable_reciprocal_to_power,
     "basic",
```

### Comparing `pymc-5.4.1/pymc/math.py` & `pymc-5.5.0/pymc/math.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/model.py` & `pymc-5.5.0/pymc/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     BlockModelAccessError,
     ImputationWarning,
     SamplingError,
     ShapeError,
     ShapeWarning,
 )
 from pymc.initial_point import make_initial_point_fn
-from pymc.logprob.basic import joint_logp
+from pymc.logprob.basic import transformed_conditional_logp
 from pymc.logprob.utils import ParameterValueError
 from pymc.pytensorf import (
     PointFunc,
     SeedSequenceSeed,
     compile_pymc,
     convert_observed_data,
     gradient,
@@ -757,15 +757,15 @@
                 else:
                     raise ValueError(
                         f"Requested variable {var} not found among the model variables"
                     )
 
         rv_logps: List[TensorVariable] = []
         if rvs:
-            rv_logps = joint_logp(
+            rv_logps = transformed_conditional_logp(
                 rvs=rvs,
                 rvs_to_values=self.rvs_to_values,
                 rvs_to_transforms=self.rvs_to_transforms,
                 jacobian=jacobian,
             )
             assert isinstance(rv_logps, list)
```

### Comparing `pymc-5.4.1/pymc/model_graph.py` & `pymc-5.5.0/pymc/model_graph.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/ode/__init__.py` & `pymc-5.5.0/pymc/ode/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/ode/ode.py` & `pymc-5.5.0/pymc/ode/ode.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/ode/utils.py` & `pymc-5.5.0/pymc/ode/utils.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/plots/__init__.py` & `pymc-5.5.0/pymc/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/printing.py` & `pymc-5.5.0/pymc/printing.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/pytensorf.py` & `pymc-5.5.0/pymc/pytensorf.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 from pytensor.tensor.sharedvar import SharedVariable, TensorSharedVariable
 from pytensor.tensor.subtensor import AdvancedIncSubtensor, AdvancedIncSubtensor1
 from pytensor.tensor.var import TensorConstant, TensorVariable
 
 from pymc.exceptions import NotConstantValueError
 from pymc.logprob.transforms import RVTransform
 from pymc.logprob.utils import CheckParameterValue
+from pymc.util import makeiter
 from pymc.vartypes import continuous_types, isgenerator, typefilter
 
 PotentialShapeType = Union[int, np.ndarray, Sequence[Union[int, Variable]], TensorVariable]
 
 
 __all__ = [
     "gradient",
@@ -546,21 +547,14 @@
 
     if vars:
         return -pt.concatenate([hessian_diag1(f, v) for v in vars], axis=0)
     else:
         return empty_gradient
 
 
-def makeiter(a):
-    if isinstance(a, (tuple, list)):
-        return a
-    else:
-        return [a]
-
-
 class IdentityOp(scalar.UnaryScalarOp):
     @staticmethod
     def st_impl(x):
         return x
 
     def impl(self, x):
         return x
```

### Comparing `pymc-5.4.1/pymc/sampling/__init__.py` & `pymc-5.5.0/pymc/sampling/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/sampling/forward.py` & `pymc-5.5.0/pymc/sampling/forward.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/sampling/jax.py` & `pymc-5.5.0/pymc/sampling/jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/sampling/mcmc.py` & `pymc-5.5.0/pymc/sampling/mcmc.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,33 +16,36 @@
 
 import logging
 import pickle
 import sys
 import time
 import warnings
 
-from collections import defaultdict
 from typing import (
     Any,
     Dict,
     Iterator,
     List,
     Literal,
+    Mapping,
     Optional,
     Sequence,
+    Set,
     Tuple,
+    Type,
     Union,
     overload,
 )
 
 import numpy as np
 import pytensor.gradient as tg
 
 from arviz import InferenceData
 from fastprogress.fastprogress import progress_bar
+from pytensor.graph.basic import Variable
 from typing_extensions import Protocol, TypeAlias
 
 import pymc as pm
 
 from pymc.backends import RunType, TraceOrBackend, init_traces
 from pymc.backends.base import IBaseTrace, MultiTrace, _choose_chains
 from pymc.blocking import DictToArrayBijection
@@ -86,15 +89,18 @@
         pass
 
 
 _log = logging.getLogger(__name__)
 
 
 def instantiate_steppers(
-    model, steps: List[Step], selected_steps, step_kwargs=None
+    model: Model,
+    steps: List[Step],
+    selected_steps: Mapping[Type[BlockedStep], List[Any]],
+    step_kwargs: Optional[Dict[str, Dict]] = None,
 ) -> Union[Step, List[Step]]:
     """Instantiate steppers assigned to the model variables.
 
     This function is intended to be called automatically from ``sample()``, but
     may be called manually.
 
     Parameters
@@ -118,30 +124,44 @@
     """
     if step_kwargs is None:
         step_kwargs = {}
 
     used_keys = set()
     for step_class, vars in selected_steps.items():
         if vars:
-            args = step_kwargs.get(step_class.name, {})
-            used_keys.add(step_class.name)
+            name = getattr(step_class, "name")
+            args = step_kwargs.get(name, {})
+            used_keys.add(name)
             step = step_class(vars=vars, model=model, **args)
             steps.append(step)
 
     unused_args = set(step_kwargs).difference(used_keys)
     if unused_args:
-        raise ValueError("Unused step method arguments: %s" % unused_args)
+        s = "s" if len(unused_args) > 1 else ""
+        example_arg = sorted(unused_args)[0]
+        example_step = (list(selected_steps.keys()) or pm.STEP_METHODS)[0]
+        example_step_name = getattr(example_step, "name")
+        raise ValueError(
+            f"Invalid key{s} found in step_kwargs: {unused_args}. "
+            "Keys must be step names and values valid kwargs for that stepper. "
+            f'Did you mean {{"{example_step_name}": {{"{example_arg}": ...}}}}?'
+        )
 
     if len(steps) == 1:
         return steps[0]
 
     return steps
 
 
-def assign_step_methods(model, step=None, methods=None, step_kwargs=None):
+def assign_step_methods(
+    model: Model,
+    step: Optional[Union[Step, Sequence[Step]]] = None,
+    methods: Optional[Sequence[Type[BlockedStep]]] = None,
+    step_kwargs: Optional[Dict[str, Any]] = None,
+) -> Union[Step, List[Step]]:
     """Assign model variables to appropriate step methods.
 
     Passing a specified model will auto-assign its constituent stochastic
     variables to step methods based on the characteristics of the variables.
     This function is intended to be called automatically from ``sample()``, but
     may be called manually. Each step method passed should have a
     ``competence()`` method that returns an ordinal competence value
@@ -163,57 +183,56 @@
         the step method, values a dict of arguments.
 
     Returns
     -------
     methods : list
         List of step methods associated with the model's variables.
     """
-    steps = []
-    assigned_vars = set()
-
-    if methods is None:
-        methods = pm.STEP_METHODS
+    steps: List[Step] = []
+    assigned_vars: Set[Variable] = set()
 
     if step is not None:
-        try:
-            steps += list(step)
-        except TypeError:
+        if isinstance(step, (BlockedStep, CompoundStep)):
             steps.append(step)
+        else:
+            steps.extend(step)
         for step in steps:
             for var in step.vars:
                 if var not in model.value_vars:
                     raise ValueError(
-                        f"{var} assigned to {step} sampler is not a value variable in the model. You can use `util.get_value_vars_from_user_vars` to parse user provided variables."
+                        f"{var} assigned to {step} sampler is not a value variable in the model. "
+                        "You can use `util.get_value_vars_from_user_vars` to parse user provided variables."
                     )
             assigned_vars = assigned_vars.union(set(step.vars))
 
     # Use competence classmethods to select step methods for remaining
     # variables
-    selected_steps = defaultdict(list)
+    methods_list: List[Type[BlockedStep]] = list(methods or pm.STEP_METHODS)
+    selected_steps: Dict[Type[BlockedStep], List] = {}
     model_logp = model.logp()
 
     for var in model.value_vars:
         if var not in assigned_vars:
             # determine if a gradient can be computed
-            has_gradient = var.dtype not in discrete_types
+            has_gradient = getattr(var, "dtype") not in discrete_types
             if has_gradient:
                 try:
-                    tg.grad(model_logp, var)
+                    tg.grad(model_logp, var)  # type: ignore
                 except (NotImplementedError, tg.NullTypeGradError):
                     has_gradient = False
 
             # select the best method
             rv_var = model.values_to_rvs[var]
             selected = max(
-                methods,
-                key=lambda method, var=rv_var, has_gradient=has_gradient: method._competence(
+                methods_list,
+                key=lambda method, var=rv_var, has_gradient=has_gradient: method._competence(  # type: ignore
                     var, has_gradient
                 ),
             )
-            selected_steps[selected].append(var)
+            selected_steps.setdefault(selected, []).append(var)
 
     return instantiate_steppers(model, steps, selected_steps, step_kwargs)
 
 
 def _print_step_hierarchy(s: Step, level: int = 0) -> None:
     if isinstance(s, CompoundStep):
         _log.info(">" * level + "CompoundStep")
```

### Comparing `pymc-5.4.1/pymc/sampling/parallel.py` & `pymc-5.5.0/pymc/sampling/parallel.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/sampling/population.py` & `pymc-5.5.0/pymc/sampling/population.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/sampling_jax.py` & `pymc-5.5.0/pymc/sampling_jax.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/smc/__init__.py` & `pymc-5.5.0/pymc/smc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/smc/kernels.py` & `pymc-5.5.0/pymc/smc/kernels.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/smc/sampling.py` & `pymc-5.5.0/pymc/smc/sampling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/stats/__init__.py` & `pymc-5.5.0/pymc/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/stats/convergence.py` & `pymc-5.5.0/pymc/stats/convergence.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/stats/log_likelihood.py` & `pymc-5.5.0/pymc/stats/log_likelihood.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/__init__.py` & `pymc-5.5.0/pymc/step_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/arraystep.py` & `pymc-5.5.0/pymc/step_methods/arraystep.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/compound.py` & `pymc-5.5.0/pymc/step_methods/compound.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,15 @@
 
     def reset_tuning(self):
         for method in self.methods:
             if hasattr(method, "reset_tuning"):
                 method.reset_tuning()
 
     @property
-    def vars(self):
+    def vars(self) -> List[Variable]:
         return [var for method in self.methods for var in method.vars]
 
 
 def flatten_steps(step: Union[BlockedStep, CompoundStep]) -> List[BlockedStep]:
     """Flatten a hierarchy of step methods to a list."""
     if isinstance(step, BlockedStep):
         return [step]
```

### Comparing `pymc-5.4.1/pymc/step_methods/hmc/__init__.py` & `pymc-5.5.0/pymc/step_methods/hmc/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/hmc/base_hmc.py` & `pymc-5.5.0/pymc/step_methods/hmc/base_hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/hmc/hmc.py` & `pymc-5.5.0/pymc/step_methods/hmc/hmc.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/hmc/integration.py` & `pymc-5.5.0/pymc/step_methods/hmc/integration.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/hmc/nuts.py` & `pymc-5.5.0/pymc/step_methods/hmc/nuts.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/hmc/quadpotential.py` & `pymc-5.5.0/pymc/step_methods/hmc/quadpotential.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/metropolis.py` & `pymc-5.5.0/pymc/step_methods/metropolis.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/slicer.py` & `pymc-5.5.0/pymc/step_methods/slicer.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/step_methods/step_sizes.py` & `pymc-5.5.0/pymc/step_methods/step_sizes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/testing.py` & `pymc-5.5.0/pymc/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,40 +10,37 @@
 #   distributed under the License is distributed on an "AS IS" BASIS,
 #   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #   See the License for the specific language governing permissions and
 #   limitations under the License.
 import functools as ft
 import itertools as it
 
-from typing import Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Sequence, Tuple, Union
 
 import numpy as np
 import pytensor
 import pytensor.tensor as pt
 import pytest
 
 from numpy import random as nr
 from numpy import testing as npt
 from pytensor.compile.mode import Mode
-from pytensor.graph.basic import walk
-from pytensor.graph.op import HasInnerGraph
+from pytensor.graph.basic import Variable
 from pytensor.graph.rewriting.basic import in2out
 from pytensor.tensor import TensorVariable
-from pytensor.tensor.random.op import RandomVariable
 from scipy import special as sp
 from scipy import stats as st
 
 import pymc as pm
 
 from pymc.distributions.distribution import Distribution
 from pymc.distributions.shape_utils import change_dist_size
 from pymc.initial_point import make_initial_point_fn
-from pymc.logprob.abstract import MeasurableVariable
-from pymc.logprob.basic import icdf, joint_logp, logcdf, logp
-from pymc.logprob.utils import ParameterValueError
+from pymc.logprob.basic import icdf, logcdf, logp, transformed_conditional_logp
+from pymc.logprob.utils import ParameterValueError, find_rvs_in_graph
 from pymc.pytensorf import (
     compile_pymc,
     floatX,
     inputvars,
     intX,
     local_check_parameter_to_ninf_switch,
 )
@@ -672,15 +669,15 @@
 
     assert moment.shape == expected.shape
     assert expected.shape == random_draw.shape
     assert np.allclose(moment, expected)
 
     if check_finite_logp:
         logp_moment = (
-            joint_logp(
+            transformed_conditional_logp(
                 (model["x"],),
                 rvs_to_values={model["x"]: pt.constant(moment)},
                 rvs_to_transforms={},
             )[0]
             .sum()
             .eval()
         )
@@ -959,23 +956,13 @@
 
 def seeded_numpy_distribution_builder(dist_name: str) -> Callable:
     return lambda self: ft.partial(
         getattr(np.random.RandomState, dist_name), self.get_random_state()
     )
 
 
-def assert_no_rvs(var):
+def assert_no_rvs(vars: Sequence[Variable]) -> None:
     """Assert that there are no `MeasurableVariable` nodes in a graph."""
 
-    def expand(r):
-        owner = r.owner
-        if owner:
-            inputs = list(reversed(owner.inputs))
-
-            if isinstance(owner.op, HasInnerGraph):
-                inputs += owner.op.inner_outputs
-
-            return inputs
-
-    for v in walk([var], expand, False):
-        if v.owner and isinstance(v.owner.op, (RandomVariable, MeasurableVariable)):
-            raise AssertionError(f"RV found in graph: {v}")
+    rvs = find_rvs_in_graph(vars)
+    if rvs:
+        raise AssertionError(f"RV found in graph: {rvs}")
```

### Comparing `pymc-5.4.1/pymc/tuning/__init__.py` & `pymc-5.5.0/pymc/tuning/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/tuning/scaling.py` & `pymc-5.5.0/pymc/tuning/scaling.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/tuning/starting.py` & `pymc-5.5.0/pymc/tuning/starting.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/util.py` & `pymc-5.5.0/pymc/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -506,7 +506,14 @@
 def _add_future_warning_tag(var) -> None:
     old_tag = var.tag
     if not isinstance(old_tag, _FutureWarningValidatingScratchpad):
         new_tag = _FutureWarningValidatingScratchpad("test_value", var.type.filter)
         for k, v in old_tag.__dict__.items():
             new_tag.__dict__.setdefault(k, v)
         var.tag = new_tag
+
+
+def makeiter(a):
+    if isinstance(a, (tuple, list)):
+        return a
+    else:
+        return [a]
```

### Comparing `pymc-5.4.1/pymc/variational/__init__.py` & `pymc-5.5.0/pymc/variational/__init__.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/variational/approximations.py` & `pymc-5.5.0/pymc/variational/approximations.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from pytensor.graph.basic import Variable
 from pytensor.tensor.var import TensorVariable
 
 import pymc as pm
 
 from pymc.blocking import DictToArrayBijection
 from pymc.distributions.dist_math import rho2sigma
-from pymc.pytensorf import makeiter
+from pymc.util import makeiter
 from pymc.variational import opvi
 from pymc.variational.opvi import (
     Approximation,
     Group,
     NotImplementedInference,
     _known_scan_ignored_inputs,
     node_property,
```

### Comparing `pymc-5.4.1/pymc/variational/callbacks.py` & `pymc-5.5.0/pymc/variational/callbacks.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/variational/inference.py` & `pymc-5.5.0/pymc/variational/inference.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/variational/minibatch_rv.py` & `pymc-5.5.0/pymc/variational/minibatch_rv.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,21 +15,15 @@
 
 import pytensor.tensor as pt
 
 from pytensor import Variable, config
 from pytensor.graph import Apply, Op
 from pytensor.tensor import NoneConst, TensorVariable, as_tensor_variable
 
-from pymc.logprob.abstract import (
-    MeasurableVariable,
-    _get_measurable_outputs,
-    _logprob,
-    _logprob_helper,
-)
-from pymc.logprob.utils import ignore_logprob
+from pymc.logprob.abstract import MeasurableVariable, _logprob, _logprob_helper
 
 
 class MinibatchRandomVariable(Op):
     """RV whose logprob should be rescaled to match total_size"""
 
     __props__ = ()
     view_map = {0: [0]}
@@ -77,16 +71,14 @@
             missing_ndims = max((rv.ndim - len(begin) - len(end), 0))
             total_size = begin + [None] * missing_ndims + end
         if len(total_size) > rv.ndim:
             raise ValueError(f"Length of total_size {total_size} is langer than RV ndim {rv.ndim}")
     else:
         raise TypeError(f"Invalid type for total_size: {total_size}")
 
-    rv = ignore_logprob(rv)
-
     return cast(TensorVariable, minibatch_rv(rv, *total_size))
 
 
 def get_scaling(total_size: Sequence[Variable], shape: TensorVariable) -> TensorVariable:
     """Gets scaling constant for logp."""
 
     # mypy doesn't understand we can convert a shape TensorVariable into a tuple
@@ -101,17 +93,12 @@
 
     return pt.cast(coef, dtype=config.floatX)
 
 
 MeasurableVariable.register(MinibatchRandomVariable)
 
 
-@_get_measurable_outputs.register(MinibatchRandomVariable)
-def _get_measurable_outputs_minibatch_random_variable(op, node):
-    return [node.outputs[0]]
-
-
 @_logprob.register(MinibatchRandomVariable)
 def minibatch_rv_logprob(op, values, *inputs, **kwargs):
     [value] = values
     rv, *total_size = inputs
     return _logprob_helper(rv, value, **kwargs) * get_scaling(total_size, value.shape)
```

### Comparing `pymc-5.4.1/pymc/variational/operators.py` & `pymc-5.5.0/pymc/variational/operators.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/variational/opvi.py` & `pymc-5.5.0/pymc/variational/opvi.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -68,22 +68,22 @@
 from pymc.initial_point import make_initial_point_fn
 from pymc.model import modelcontext
 from pymc.pytensorf import (
     SeedSequenceSeed,
     compile_pymc,
     find_rng_nodes,
     identity,
-    makeiter,
     reseed_rngs,
 )
 from pymc.util import (
     RandomState,
     WithMemoization,
     _get_seeds_per_chain,
     locally_cachedmethod,
+    makeiter,
 )
 from pymc.variational.minibatch_rv import MinibatchRandomVariable, get_scaling
 from pymc.variational.updates import adagrad_window
 from pymc.vartypes import discrete_types
 
 __all__ = ["ObjectiveFunction", "Operator", "TestFunction", "Group", "Approximation"]
```

### Comparing `pymc-5.4.1/pymc/variational/stein.py` & `pymc-5.5.0/pymc/variational/stein.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/variational/test_functions.py` & `pymc-5.5.0/pymc/variational/test_functions.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/variational/updates.py` & `pymc-5.5.0/pymc/variational/updates.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc/vartypes.py` & `pymc-5.5.0/pymc/vartypes.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/pymc.egg-info/PKG-INFO` & `pymc-5.5.0/pymc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymc
-Version: 5.4.1
+Version: 5.5.0
 Summary: Probabilistic Programming in Python: Bayesian Modeling and Probabilistic Machine Learning with PyTensor
 Home-page: http://github.com/pymc-devs/pymc
 Maintainer: PyMC Developers
 Maintainer-email: pymc.devs@gmail.com
 License: Apache License, Version 2.0
 Description: .. image:: https://cdn.rawgit.com/pymc-devs/pymc/main/docs/logos/svg/PyMC_banner.svg
             :height: 100px
```

### Comparing `pymc-5.4.1/pymc.egg-info/SOURCES.txt` & `pymc-5.5.0/pymc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/scripts/docker_container.sh` & `pymc-5.5.0/scripts/docker_container.sh`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/setup.py` & `pymc-5.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymc-5.4.1/versioneer.py` & `pymc-5.5.0/versioneer.py`

 * *Files identical despite different names*

