# Comparing `tmp/mpi4jax-0.3.8.tar.gz` & `tmp/mpi4jax-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpi4jax-0.3.8.tar", last modified: Thu Apr 28 08:34:27 2022, max compression
+gzip compressed data, was "mpi4jax-0.3.9.tar", last modified: Tue Aug  9 12:11:55 2022, max compression
```

## Comparing `mpi4jax-0.3.8.tar` & `mpi4jax-0.3.9.tar`

### file list

```diff
@@ -1,77 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.349418 mpi4jax-0.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)    16700 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/examples/shallow_water.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/mpi4jax/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.349418 mpi4jax-0.3.8/mpi4jax/_src/
--rw-r--r--   0 runner    (1001) docker     (121)     1107 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.349418 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4904 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/allgather.py
--rw-r--r--   0 runner    (1001) docker     (121)     6268 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/allreduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     4702 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/alltoall.py
--rw-r--r--   0 runner    (1001) docker     (121)     3430 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/barrier.py
--rw-r--r--   0 runner    (1001) docker     (121)     4797 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/bcast.py
--rw-r--r--   0 runner    (1001) docker     (121)     5722 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/gather.py
--rw-r--r--   0 runner    (1001) docker     (121)     5268 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/recv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5048 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/reduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     4208 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     5546 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4055 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/send.py
--rw-r--r--   0 runner    (1001) docker     (121)    10361 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/collective_ops/sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (121)      207 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/comm.py
--rw-r--r--   0 runner    (1001) docker     (121)     2983 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/flush.py
--rw-r--r--   0 runner    (1001) docker     (121)     1010 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/jax_compat.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.349418 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/
--rw-r--r--   0 runner    (1001) docker     (121)      720 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      626 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    11582 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     7985 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
--rw-r--r--   0 runner    (1001) docker     (121)    28140 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/mpi4jax/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.349418 mpi4jax-0.3.8/mpi4jax/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/experimental/register_overrides.py
--rw-r--r--   0 runner    (1001) docker     (121)     7493 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/mpi4jax/experimental/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.349418 mpi4jax-0.3.8/mpi4jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5095 2022-04-28 08:34:27.000000 mpi4jax-0.3.8/mpi4jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2042 2022-04-28 08:34:27.000000 mpi4jax-0.3.8/mpi4jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 08:34:27.000000 mpi4jax-0.3.8/mpi4jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-04-28 08:34:27.000000 mpi4jax-0.3.8/mpi4jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-04-28 08:34:27.000000 mpi4jax-0.3.8/mpi4jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6214 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/tests/collective_ops/
--rw-r--r--   0 runner    (1001) docker     (121)      916 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_allgather.py
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_allreduce.py
--rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_allreduce_matvec.py
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_alltoall.py
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_barrier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_bcast.py
--rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (121)      884 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_scatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     4337 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_send_and_recv.py
--rw-r--r--   0 runner    (1001) docker     (121)     5331 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/collective_ops/test_sendrecv.py
--rw-r--r--   0 runner    (1001) docker     (121)      376 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 08:34:27.353418 mpi4jax-0.3.8/tests/experimental/
--rw-r--r--   0 runner    (1001) docker     (121)    12611 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/experimental/test_auto_tokenize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/test_flush.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/test_has_cuda.py
--rw-r--r--   0 runner    (1001) docker     (121)      913 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/test_invalid_jaxlib.py
--rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (121)    70144 2022-04-28 08:32:47.000000 mpi4jax-0.3.8/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1085 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.727733 mpi4jax-0.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)    16700 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/examples/shallow_water.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/mpi4jax/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.727733 mpi4jax-0.3.9/mpi4jax/_src/
+-rw-r--r--   0 runner    (1001) docker     (121)     1207 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       77 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/_latest_jax_version.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.727733 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4934 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/allgather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6298 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4732 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3460 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/barrier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4827 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/bcast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5752 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/gather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/recv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5078 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4238 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5576 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4085 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/send.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10391 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/collective_ops/sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      207 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/comm.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2741 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      335 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/flush.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3037 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      626 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)     2164 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)    11582 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     7985 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)    28140 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/mpi4jax/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/mpi4jax/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)       73 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3623 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/experimental/register_overrides.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7261 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/mpi4jax/experimental/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.727733 mpi4jax-0.3.9/mpi4jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-08-09 12:11:55.000000 mpi4jax-0.3.9/mpi4jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-08-09 12:11:55.000000 mpi4jax-0.3.9/mpi4jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 12:11:55.000000 mpi4jax-0.3.9/mpi4jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-08-09 12:11:55.000000 mpi4jax-0.3.9/mpi4jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-08-09 12:11:55.000000 mpi4jax-0.3.9/mpi4jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      703 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6322 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/tests/collective_ops/
+-rw-r--r--   0 runner    (1001) docker     (121)      916 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_allgather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_allreduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5273 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_allreduce_matvec.py
+-rw-r--r--   0 runner    (1001) docker     (121)      834 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_alltoall.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_barrier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1249 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_bcast.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4127 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1216 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (121)      884 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4337 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_send_and_recv.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5331 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/collective_ops/test_sendrecv.py
+-rw-r--r--   0 runner    (1001) docker     (121)      376 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 12:11:55.731733 mpi4jax-0.3.9/tests/experimental/
+-rw-r--r--   0 runner    (1001) docker     (121)    10689 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/experimental/test_auto_tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      494 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/test_flush.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/test_has_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1387 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/test_jax_compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    70144 2022-08-09 12:10:34.000000 mpi4jax-0.3.9/versioneer.py
```

### Comparing `mpi4jax-0.3.8/LICENSE.md` & `mpi4jax-0.3.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/PKG-INFO` & `mpi4jax-0.3.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.3.8
+Version: 0.3.9
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE.md
 
 mpi4jax
 =======
 
 |JOSS paper| |PyPI Version| |Conda Version| |Tests| |codecov| |Documentation Status|
@@ -139,9 +138,7 @@
    :target: https://pypi.org/project/mpi4jax/
 .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/mpi4jax.svg
    :target: https://anaconda.org/conda-forge/mpi4jax
 .. |Documentation Status| image:: https://readthedocs.org/projects/mpi4jax/badge/?version=latest
    :target: https://mpi4jax.readthedocs.io/en/latest/?badge=latest
 .. |JOSS paper| image:: https://joss.theoj.org/papers/10.21105/joss.03419/status.svg
    :target: https://doi.org/10.21105/joss.03419
-
-
```

### Comparing `mpi4jax-0.3.8/README.rst` & `mpi4jax-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/examples/shallow_water.py` & `mpi4jax-0.3.9/examples/shallow_water.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/__init__.py` & `mpi4jax-0.3.9/mpi4jax/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/__init__.py` & `mpi4jax-0.3.9/mpi4jax/_src/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # make sure to import mpi4py before anything else
 # this calls MPI_Init and registers mpi4py's atexit handler
 from mpi4py import MPI
 
-# this registers our custom XLA functions
-from . import xla_bridge
+# check version of JAX and jaxlib
+from . import jax_compat
 
-# import public API
-from .collective_ops.allgather import allgather  # noqa: F401
-from .collective_ops.allreduce import allreduce  # noqa: F401
-from .collective_ops.alltoall import alltoall  # noqa: F401
-from .collective_ops.barrier import barrier  # noqa: F401
-from .collective_ops.bcast import bcast  # noqa: F401
-from .collective_ops.gather import gather  # noqa: F401
-from .collective_ops.recv import recv  # noqa: F401
-from .collective_ops.reduce import reduce  # noqa: F401
-from .collective_ops.scan import scan  # noqa: F401
-from .collective_ops.scatter import scatter  # noqa: F401
-from .collective_ops.send import send  # noqa: F401
-from .collective_ops.sendrecv import sendrecv  # noqa: F401
+jax_compat.check_jax_version()  # noqa: F401
 
-from .utils import has_cuda_support  # noqa: F401
+# this registers our custom XLA functions
+from . import xla_bridge  # noqa: E402
 
-# check version of jaxlib
-from . import jax_compat
+# import public API
+from .collective_ops.allgather import allgather  # noqa: F401, E402
+from .collective_ops.allreduce import allreduce  # noqa: F401, E402
+from .collective_ops.alltoall import alltoall  # noqa: F401, E402
+from .collective_ops.barrier import barrier  # noqa: F401, E402
+from .collective_ops.bcast import bcast  # noqa: F401, E402
+from .collective_ops.gather import gather  # noqa: F401, E402
+from .collective_ops.recv import recv  # noqa: F401, E402
+from .collective_ops.reduce import reduce  # noqa: F401, E402
+from .collective_ops.scan import scan  # noqa: F401, E402
+from .collective_ops.scatter import scatter  # noqa: F401, E402
+from .collective_ops.send import send  # noqa: F401, E402
+from .collective_ops.sendrecv import sendrecv  # noqa: F401, E402
 
-jax_compat.check_jax_version()  # noqa: F401
+from .utils import has_cuda_support  # noqa: F401, E402
 
 # sanitize namespace
 del jax_compat, xla_bridge, MPI
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/allgather.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/allgather.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_allgather_p = Primitive("allgather_mpi")  # Create the primitive
 mpi_allgather_impl = default_primitive_impl(mpi_allgather_p)
 
 
 # This function applies the primitive to an AST
@@ -172,12 +172,12 @@
         abstract_arrays.ShapedArray(out_shape, x.dtype),
         core.abstract_token,
     )
 
 
 mpi_allgather_p.multiple_results = True
 mpi_allgather_p.def_impl(mpi_allgather_impl)
-mpi_allgather_p.def_abstract_eval(mpi_allgather_abstract_eval)
+register_abstract_eval(mpi_allgather_p, mpi_allgather_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_allgather_p] = mpi_allgather_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_allgather_p] = mpi_allgather_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/allreduce.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/allreduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import ad, xla, batching
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_allreduce_p = Primitive("allreduce_mpi")  # Create the primitive
 mpi_allreduce_impl = default_primitive_impl(mpi_allreduce_p)
 
 
 # This function applies the primitive to an AST
@@ -192,15 +192,15 @@
         x_tan, token, op=op, comm=comm, transpose=(not transpose)
     )
     return res, token_tan
 
 
 mpi_allreduce_p.multiple_results = True
 mpi_allreduce_p.def_impl(mpi_allreduce_impl)
-mpi_allreduce_p.def_abstract_eval(mpi_allreduce_abstract_eval)
+register_abstract_eval(mpi_allreduce_p, mpi_allreduce_abstract_eval)
 
 batching.primitive_batchers[mpi_allreduce_p] = mpi_allreduce_batch_eval
 
 ad.primitive_jvps[mpi_allreduce_p] = mpi_allreduce_value_and_jvp
 ad.primitive_transposes[mpi_allreduce_p] = mpi_allreduce_transpose_rule
 
 # assign to the primitive the correct encoder
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/alltoall.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/alltoall.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_alltoall_p = Primitive("alltoall_mpi")  # Create the primitive
 mpi_alltoall_impl = default_primitive_impl(mpi_alltoall_p)
 
 
 # This function applies the primitive to an AST
@@ -169,12 +169,12 @@
         abstract_arrays.ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     )
 
 
 mpi_alltoall_p.multiple_results = True
 mpi_alltoall_p.def_impl(mpi_alltoall_impl)
-mpi_alltoall_p.def_abstract_eval(mpi_alltoall_abstract_eval)
+register_abstract_eval(mpi_alltoall_p, mpi_alltoall_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_alltoall_p] = mpi_alltoall_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_alltoall_p] = mpi_alltoall_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/barrier.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/barrier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from mpi4py import MPI as _MPI
 
 from jax import core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla, batching
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -13,15 +13,15 @@
     unpack_hashable,
     wrap_as_hashable,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_barrier_p = Primitive("barrier_mpi")  # Create the primitive
 mpi_barrier_impl = default_primitive_impl(mpi_barrier_p)
 
 
 # This function applies the primitive to an AST
@@ -110,14 +110,14 @@
 def mpi_barrier_batch_eval(in_args, batch_axes, comm):
     token = in_args[0]
     res = mpi_barrier_p.bind(token, comm=comm)
     return res, batch_axes
 
 
 mpi_barrier_p.def_impl(mpi_barrier_impl)
-mpi_barrier_p.def_abstract_eval(mpi_barrier_abstract_eval)
+register_abstract_eval(mpi_barrier_p, mpi_barrier_abstract_eval)
 
 batching.primitive_batchers[mpi_barrier_p] = mpi_barrier_batch_eval
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_barrier_p] = mpi_barrier_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_barrier_p] = mpi_barrier_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/bcast.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/bcast.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lib import xla_client
 from jax.lax import create_token
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_bcast_p = Primitive("bcast_mpi")  # Create the primitive
 mpi_bcast_impl = default_primitive_impl(mpi_bcast_p)
 
 
 # This function applies the primitive to an AST
@@ -167,12 +167,12 @@
         abstract_arrays.ShapedArray(dims, xs.dtype),
         core.abstract_token,
     )
 
 
 mpi_bcast_p.multiple_results = True
 mpi_bcast_p.def_impl(mpi_bcast_impl)
-mpi_bcast_p.def_abstract_eval(mpi_bcast_abstract_eval)
+register_abstract_eval(mpi_bcast_p, mpi_bcast_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_bcast_p] = mpi_bcast_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_bcast_p] = mpi_bcast_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/gather.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/gather.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_gather_p = Primitive("gather_mpi")  # Create the primitive
 mpi_gather_impl = default_primitive_impl(mpi_gather_p)
 
 
 # This function applies the primitive to an AST
@@ -206,12 +206,12 @@
         abstract_arrays.ShapedArray(out_shape, x.dtype),
         core.abstract_token,
     )
 
 
 mpi_gather_p.multiple_results = True
 mpi_gather_p.def_impl(mpi_gather_impl)
-mpi_gather_p.def_abstract_eval(mpi_gather_abstract_eval)
+register_abstract_eval(mpi_gather_p, mpi_gather_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_gather_p] = mpi_gather_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_gather_p] = mpi_gather_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/recv.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/recv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -17,15 +17,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_recv_p = Primitive("recv_mpi")  # Create the primitive
 mpi_recv_impl = default_primitive_impl(mpi_recv_p)
 
 
 # This function applies the primitive to an AST
@@ -182,12 +182,12 @@
         abstract_arrays.ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     )
 
 
 mpi_recv_p.multiple_results = True
 mpi_recv_p.def_impl(mpi_recv_impl)
-mpi_recv_p.def_abstract_eval(mpi_recv_abstract_eval)
+register_abstract_eval(mpi_recv_p, mpi_recv_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_recv_p] = mpi_recv_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_recv_p] = mpi_recv_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/reduce.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/reduce.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lib import xla_client
 from jax.lax import create_token
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_reduce_p = Primitive("reduce_mpi")  # Create the primitive
 mpi_reduce_impl = default_primitive_impl(mpi_reduce_p)
 
 
 # This function applies the primitive to an AST
@@ -180,12 +180,12 @@
         abstract_arrays.ShapedArray(dims, xs.dtype),
         core.abstract_token,
     )
 
 
 mpi_reduce_p.multiple_results = True
 mpi_reduce_p.def_impl(mpi_reduce_impl)
-mpi_reduce_p.def_abstract_eval(mpi_reduce_abstract_eval)
+register_abstract_eval(mpi_reduce_p, mpi_reduce_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_reduce_p] = mpi_reduce_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_reduce_p] = mpi_reduce_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/scan.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/scan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lib import xla_client
 from jax.lax import create_token
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_scan_p = Primitive("scan_mpi")  # Create the primitive
 mpi_scan_impl = default_primitive_impl(mpi_scan_p)
 
 
 # This function applies the primitive to an AST
@@ -142,12 +142,12 @@
         abstract_arrays.ShapedArray(xs.shape, xs.dtype),
         core.abstract_token,
     )
 
 
 mpi_scan_p.multiple_results = True
 mpi_scan_p.def_impl(mpi_scan_impl)
-mpi_scan_p.def_abstract_eval(mpi_scan_abstract_eval)
+register_abstract_eval(mpi_scan_p, mpi_scan_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_scan_p] = mpi_scan_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_scan_p] = mpi_scan_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/scatter.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/scatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_scatter_p = Primitive("scatter_mpi")  # Create the primitive
 mpi_scatter_impl = default_primitive_impl(mpi_scatter_p)
 
 
 # This function applies the primitive to an AST
@@ -200,12 +200,12 @@
         abstract_arrays.ShapedArray(out_shape, x.dtype),
         core.abstract_token,
     )
 
 
 mpi_scatter_p.multiple_results = True
 mpi_scatter_p.def_impl(mpi_scatter_impl)
-mpi_scatter_p.def_abstract_eval(mpi_scatter_abstract_eval)
+register_abstract_eval(mpi_scatter_p, mpi_scatter_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_scatter_p] = mpi_scatter_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_scatter_p] = mpi_scatter_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/send.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/send.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import xla
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -16,15 +16,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_send_p = Primitive("send_mpi")  # Create the primitive
 mpi_send_impl = default_primitive_impl(mpi_send_p)
 
 
 # This function applies the primitive to an AST
@@ -137,12 +137,12 @@
 
 # This function evaluates only the shapes during AST construction
 def mpi_send_abstract_eval(xs, token, dest, tag, comm):
     return core.abstract_token
 
 
 mpi_send_p.def_impl(mpi_send_impl)
-mpi_send_p.def_abstract_eval(mpi_send_abstract_eval)
+register_abstract_eval(mpi_send_p, mpi_send_abstract_eval)
 
 # assign to the primitive the correct encoder
 xla.backend_specific_translations["cpu"][mpi_send_p] = mpi_send_xla_encode_cpu
 xla.backend_specific_translations["gpu"][mpi_send_p] = mpi_send_xla_encode_gpu
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/collective_ops/sendrecv.py` & `mpi4jax-0.3.9/mpi4jax/_src/collective_ops/sendrecv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as _np
 from mpi4py import MPI as _MPI
 
 from jax import abstract_arrays, core
-from jax.core import Primitive
+from jax.core import Primitive, Tracer, Token
 from jax.interpreters import ad, xla, batching
 from jax.lax import create_token
 from jax.lib import xla_client
 
 from ..utils import (
     HashableMPIType,
     default_primitive_impl,
@@ -17,15 +17,15 @@
     wrap_as_hashable,
     xla_constant_intc,
     xla_constant_uintptr,
 )
 from ..decorators import translation_rule_cpu, translation_rule_gpu
 from ..validation import enforce_types
 from ..comm import get_default_comm
-from ..jax_compat import Tracer, Token
+from ..jax_compat import register_abstract_eval
 
 # The Jax primitive
 mpi_sendrecv_p = Primitive("sendrecv_mpi")  # Create the primitive
 mpi_sendrecv_impl = default_primitive_impl(mpi_sendrecv_p)
 
 
 # This function applies the primitive to an AST
@@ -383,15 +383,15 @@
         _must_transpose=not _must_transpose,
     )
     return res, ad.Zero.from_value(res), token_tan
 
 
 mpi_sendrecv_p.multiple_results = True
 mpi_sendrecv_p.def_impl(mpi_sendrecv_impl)
-mpi_sendrecv_p.def_abstract_eval(mpi_sendrecv_abstract_eval)
+register_abstract_eval(mpi_sendrecv_p, mpi_sendrecv_abstract_eval)
 
 batching.primitive_batchers[mpi_sendrecv_p] = mpi_sendrecv_batch_eval
 
 ad.primitive_jvps[mpi_sendrecv_p] = mpi_sendrecv_value_and_jvp
 ad.primitive_transposes[mpi_sendrecv_p] = mpi_sendrecv_transpose_rule
 
 # assign to the primitive the correct encoder
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/decorators.py` & `mpi4jax-0.3.9/mpi4jax/_src/decorators.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,21 +20,14 @@
 
     from .flush import flush
 
     flush_platform = functools.partial(flush, platform=platform)
     atexit.register(flush_platform)
 
 
-def ensure_omnistaging():
-    import jax.config
-
-    if not jax.config.omnistaging_enabled:
-        raise RuntimeError("mpi4jax requires JAX omnistaging to be enabled.")
-
-
 def ensure_gpu_ext():
     from .xla_bridge import HAS_GPU_EXT
 
     if not HAS_GPU_EXT:
         raise ImportError(
             "The mpi4jax GPU extensions could not be imported. "
             "Please re-build mpi4jax with CUDA support and try again."
@@ -80,18 +73,15 @@
 
 def translation_rule_cpu(func):
     """XLA primitive translation rule on CPU for mpi4jax custom calls.
 
     This runs generic setup and boilerplate functions.
     """
     # functions to call before running the translation rule
-    setup_funcs = (
-        functools.partial(ensure_platform_flush, "cpu"),
-        ensure_omnistaging,
-    )
+    setup_funcs = (functools.partial(ensure_platform_flush, "cpu"),)
 
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
         for f in setup_funcs:
             f()
         return func(*args, **kwargs)
 
@@ -103,15 +93,14 @@
 
     This runs generic setup and boilerplate functions.
     """
     # functions to call before running the translation rule
     setup_funcs = (
         ensure_gpu_ext,
         functools.partial(ensure_platform_flush, "gpu"),
-        ensure_omnistaging,
         setup_cuda_mpi,
     )
 
     @functools.wraps(func)
     def wrapped(*args, **kwargs):
         for f in setup_funcs:
             f()
```

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/utils.py` & `mpi4jax-0.3.9/mpi4jax/_src/utils.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/validation.py` & `mpi4jax-0.3.9/mpi4jax/_src/validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/__init__.py` & `mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd` & `mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/cuda_runtime_api.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd` & `mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pxd`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx` & `mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx` & `mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge_cpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx` & `mpi4jax-0.3.9/mpi4jax/_src/xla_bridge/mpi_xla_bridge_gpu.pyx`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/experimental/register_overrides.py` & `mpi4jax-0.3.9/mpi4jax/experimental/register_overrides.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/mpi4jax/experimental/tokenizer.py` & `mpi4jax-0.3.9/mpi4jax/experimental/tokenizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,11 @@
 import jax
 from jax import linear_util as lu
 from jax.interpreters import xla
 
-from .._src.jax_compat import versiontuple
-
-MINIMUM_JAX_VERSION = "0.2.27"
-
-if versiontuple(jax.__version__) < versiontuple(MINIMUM_JAX_VERSION):
-    raise RuntimeError(
-        f"auto_tokenize requires jax>={MINIMUM_JAX_VERSION}, but you have {jax.__version__}. "
-        "Consider upgrading JAX via `pip install -U jax`."
-    )
-
 # registry for wrapped mpi4jax ops
 from .register_overrides import token_override_registry  # noqa: E402
 
 # registry for wrapped JAX primitives
 recursive_token_forwarding_registry = {}
 
 
@@ -125,15 +115,19 @@
         else:
             return env[v]
 
     def write(v, val):
         env[v] = val
 
     env = {}
-    write(jax.core.unitvar, jax.core.unit)
+
+    # compatibility with jax<0.3.10
+    if hasattr(jax.core, "unitvar"):
+        write(jax.core.unitvar, jax.core.unit)
+
     safe_map(write, jaxpr.constvars, consts)
     safe_map(write, jaxpr.invars, args)
     for eqn in jaxpr.eqns:
         # Here, we override the original primatives with our own
         # token forcing method.
         if eqn.primitive in token_override_registry:
             token_override = token_override_registry[eqn.primitive]
@@ -199,12 +193,12 @@
         >>> arr = jnp.ones((3, 2))
         >>> res = f(arr)
 
     """
 
     def wrapper(*args, **kwargs):
         jaxpr, pytree = jax.make_jaxpr(f, return_shape=True)(*args, **kwargs)
-        _, pytree = jax.tree_flatten(pytree)
+        _, pytree = jax.tree_util.tree_flatten(pytree)
         res = _override_tokens(jaxpr.jaxpr, jaxpr.consts, None, *args, **kwargs)
-        return jax.tree_unflatten(pytree, res[1:])  # Drop the token.
+        return jax.tree_util.tree_unflatten(pytree, res[1:])  # Drop the token.
 
     return wrapper
```

### Comparing `mpi4jax-0.3.8/mpi4jax.egg-info/PKG-INFO` & `mpi4jax-0.3.9/mpi4jax.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: mpi4jax
-Version: 0.3.8
+Version: 0.3.9
 Summary: Zero-copy MPI communication of JAX arrays, for turbo-charged HPC applications in Python ⚡
 Home-page: https://github.com/mpi4jax/mpi4jax
 Author: Filippo Vicentini
 Author-email: filippovicentini@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Provides-Extra: dev
 License-File: LICENSE.md
 
 mpi4jax
 =======
 
 |JOSS paper| |PyPI Version| |Conda Version| |Tests| |codecov| |Documentation Status|
@@ -139,9 +138,7 @@
    :target: https://pypi.org/project/mpi4jax/
 .. |Conda Version| image:: https://img.shields.io/conda/vn/conda-forge/mpi4jax.svg
    :target: https://anaconda.org/conda-forge/mpi4jax
 .. |Documentation Status| image:: https://readthedocs.org/projects/mpi4jax/badge/?version=latest
    :target: https://mpi4jax.readthedocs.io/en/latest/?badge=latest
 .. |JOSS paper| image:: https://joss.theoj.org/papers/10.21105/joss.03419/status.svg
    :target: https://doi.org/10.21105/joss.03419
-
-
```

### Comparing `mpi4jax-0.3.8/mpi4jax.egg-info/SOURCES.txt` & `mpi4jax-0.3.9/mpi4jax.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 mpi4jax/_version.py
 mpi4jax.egg-info/PKG-INFO
 mpi4jax.egg-info/SOURCES.txt
 mpi4jax.egg-info/dependency_links.txt
 mpi4jax.egg-info/requires.txt
 mpi4jax.egg-info/top_level.txt
 mpi4jax/_src/__init__.py
+mpi4jax/_src/_latest_jax_version.txt
 mpi4jax/_src/comm.py
 mpi4jax/_src/decorators.py
 mpi4jax/_src/flush.py
 mpi4jax/_src/jax_compat.py
 mpi4jax/_src/utils.py
 mpi4jax/_src/validation.py
 mpi4jax/_src/collective_ops/__init__.py
@@ -43,15 +44,15 @@
 mpi4jax/experimental/register_overrides.py
 mpi4jax/experimental/tokenizer.py
 tests/conftest.py
 tests/test_decorators.py
 tests/test_examples.py
 tests/test_flush.py
 tests/test_has_cuda.py
-tests/test_invalid_jaxlib.py
+tests/test_jax_compat.py
 tests/test_validation.py
 tests/collective_ops/test_allgather.py
 tests/collective_ops/test_allreduce.py
 tests/collective_ops/test_allreduce_matvec.py
 tests/collective_ops/test_alltoall.py
 tests/collective_ops/test_barrier.py
 tests/collective_ops/test_bcast.py
```

### Comparing `mpi4jax-0.3.8/pyproject.toml` & `mpi4jax-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/setup.py` & `mpi4jax-0.3.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 import sys
+import shlex
 
 from setuptools import setup, find_packages
 from setuptools.extension import Extension
+from setuptools.command.build_ext import build_ext
 
 # ensure vendored versioneer is on path
 sys.path.append(os.path.dirname(__file__))
 import versioneer  # noqa: E402
 
 try:
     from Cython.Build import cythonize
@@ -18,28 +20,33 @@
 try:
     import mpi4py
 except ImportError:
     HAS_MPI4PY = False
 else:
     HAS_MPI4PY = True
 
+
+here = os.path.abspath(os.path.dirname(__file__))
+
 ##############
 # Requirements
 
-BASE_DEPENDENCIES = ["jax>=0.2.9", "mpi4py>=3.0.1", "numpy"]
+JAX_MINIMUM_VERSION = "0.3.0"
+
+BASE_DEPENDENCIES = ["mpi4py>=3.0.1", "numpy", f"jax>={JAX_MINIMUM_VERSION}"]
+
 DEV_DEPENDENCIES = [
     "pytest>=6",
     "pytest-cov>=2.10.1",
     "coverage[toml]>=5",
     "pre-commit",
     "black==21.6b0",
     "flake8==3.9.2",
 ]
 
-
 CYTHON_SUBMODULE_NAME = "mpi4jax._src.xla_bridge"
 CYTHON_SUBMODULE_PATH = "mpi4jax/_src/xla_bridge"
 
 
 #######
 # Utils
 def search_on_path(filenames):
@@ -61,34 +68,26 @@
     print("**************************************************")
 
 
 # /end Utils
 ############
 
 
-def mpi_info(cmd):
-    config = mpi4py.get_config()
-    cmd_compile = " ".join([config["mpicc"], "-show"])
-    out_stream = os.popen(cmd_compile)
-    flags = out_stream.read().strip()
-    flags = flags.replace(",", " ").split()
-
-    if cmd == "compile":
-        startwith = "-I"
-    elif cmd == "libdirs":
-        startwith = "-L"
-    elif cmd == "libs":
-        startwith = "-l"
-
-    out = []
-    for flag in flags:
-        if flag.startswith(startwith):
-            out.append(flag[2:])
+class custom_build_ext(build_ext):
+    def build_extensions(self):
+        config = mpi4py.get_config()
+
+        # on some platforms, mpi4py's compiler config includes flags
+        mpi_compiler = shlex.split(config["mpicc"])
+
+        for exe in ("compiler", "compiler_so", "compiler_cxx", "linker_so"):
+            current_flags = getattr(self.compiler, exe)[1:]
+            self.compiler.set_executable(exe, [*mpi_compiler, *current_flags])
 
-    return out
+        build_ext.build_extensions(self)
 
 
 ################
 # Cuda detection
 
 # Taken from CUPY (MIT License)
 def get_cuda_path():
@@ -118,36 +117,35 @@
         _cuda_path = "/usr/local/cuda"
     else:
         _cuda_path = None
 
     return _cuda_path
 
 
-def cuda_info(cmd):
+def get_cuda_info():
+    cuda_info = {"compile": [], "libdirs": [], "libs": []}
     cuda_path = get_cuda_path()
     if not cuda_path:
-        return []
+        return cuda_info
 
-    if cmd == "compile":
-        incdir = os.path.join(cuda_path, "include")
-        if os.path.isdir(incdir):
-            return [incdir]
-
-    if cmd == "libdirs":
-        for libdir in ("lib64", "lib"):
-            full_dir = os.path.join(cuda_path, libdir)
-            if os.path.isdir(full_dir):
-                return [full_dir]
+    incdir = os.path.join(cuda_path, "include")
+    if os.path.isdir(incdir):
+        cuda_info["compile"].append(incdir)
 
-    if cmd == "libs":
-        return ["cudart"]
+    for libdir in ("lib64", "lib"):
+        full_dir = os.path.join(cuda_path, libdir)
+        if os.path.isdir(full_dir):
+            cuda_info["libdirs"].append(full_dir)
 
-    return []
+    cuda_info["libs"].append("cudart")
+    return cuda_info
 
 
+cuda_info = get_cuda_info()
+
 # /end Cuda detection
 #####################
 
 
 def get_extensions():
     cmd = sys.argv[1]
     require_extensions = any(
@@ -162,75 +160,75 @@
         else:
             return []
 
     extensions = [
         Extension(
             name=f"{CYTHON_SUBMODULE_NAME}.{mod}",
             sources=[f"{CYTHON_SUBMODULE_PATH}/{mod}.pyx"],
-            include_dirs=mpi_info("compile"),
-            library_dirs=mpi_info("libdirs"),
-            libraries=mpi_info("libs"),
         )
         for mod in ("mpi_xla_bridge", "mpi_xla_bridge_cpu")
     ]
 
-    if cuda_info("compile"):
+    if cuda_info["compile"] and cuda_info["libdirs"]:
         extensions.append(
             Extension(
                 name=f"{CYTHON_SUBMODULE_NAME}.mpi_xla_bridge_gpu",
                 sources=[f"{CYTHON_SUBMODULE_PATH}/mpi_xla_bridge_gpu.pyx"],
-                include_dirs=mpi_info("compile") + cuda_info("compile"),
-                library_dirs=mpi_info("libdirs") + cuda_info("libdirs"),
-                libraries=mpi_info("libs") + cuda_info("libs"),
+                include_dirs=cuda_info["compile"],
+                library_dirs=cuda_info["libdirs"],
+                libraries=cuda_info["libs"],
             )
         )
     else:
         print_warning("CUDA path not found", "(GPU extensions will not be built)")
 
     if HAS_CYTHON:
         extensions = cythonize(
             extensions,
             language_level=3,
         )
 
     return extensions
 
 
-here = os.path.abspath(os.path.dirname(__file__))
-
 # get the long description from the README file
 with open(os.path.join(here, "README.rst"), encoding="utf-8") as f:
     long_description = f.read()
 
+
+cmdclass = versioneer.get_cmdclass()
+cmdclass.update(build_ext=custom_build_ext)
+
 setup(
     name="mpi4jax",
     author="Filippo Vicentini",
     author_email="filippovicentini@gmail.com",
     description=(
         "Zero-copy MPI communication of JAX arrays, "
         "for turbo-charged HPC applications in Python ⚡"
     ),
     long_description=long_description,
     url="https://github.com/mpi4jax/mpi4jax",
     license="MIT",
     version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
+    cmdclass=cmdclass,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Cython",
         "Development Status :: 3 - Alpha",
         "Environment :: GPU :: NVIDIA CUDA",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Unix",
         "Topic :: Scientific/Engineering",
     ],
     packages=find_packages(),
     ext_modules=get_extensions(),
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     install_requires=BASE_DEPENDENCIES,
     extras_require={
         "dev": DEV_DEPENDENCIES,
     },
+    package_data={"mpi4jax": ["_src/_latest_jax_version.txt"]},
 )
```

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_allgather.py` & `mpi4jax-0.3.9/tests/collective_ops/test_allgather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_allreduce.py` & `mpi4jax-0.3.9/tests/collective_ops/test_allreduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_allreduce_matvec.py` & `mpi4jax-0.3.9/tests/collective_ops/test_allreduce_matvec.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_alltoall.py` & `mpi4jax-0.3.9/tests/collective_ops/test_alltoall.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_barrier.py` & `mpi4jax-0.3.9/tests/collective_ops/test_barrier.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_bcast.py` & `mpi4jax-0.3.9/tests/collective_ops/test_bcast.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_common.py` & `mpi4jax-0.3.9/tests/collective_ops/test_common.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -79,16 +79,16 @@
             send(x, dest=100, comm=comm)
 
         send_jit(jnp.ones(10))
     """
     )
 
     proc = run_in_subprocess(test_script, tmp_path / "abort.py")
-    assert proc.returncode != 0
     print(proc.stderr)
+    assert proc.returncode != 0
     assert "r0 | MPI_Send returned error code" in proc.stderr
 
 
 @pytest.mark.skipif(rank > 0, reason="Runs only on rank 0")
 def test_deadlock_on_exit(tmp_path):
     from textwrap import dedent
```

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_gather.py` & `mpi4jax-0.3.9/tests/collective_ops/test_gather.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_reduce.py` & `mpi4jax-0.3.9/tests/collective_ops/test_reduce.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_scan.py` & `mpi4jax-0.3.9/tests/collective_ops/test_scan.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_scatter.py` & `mpi4jax-0.3.9/tests/collective_ops/test_scatter.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_send_and_recv.py` & `mpi4jax-0.3.9/tests/collective_ops/test_send_and_recv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/collective_ops/test_sendrecv.py` & `mpi4jax-0.3.9/tests/collective_ops/test_sendrecv.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/tests/experimental/test_auto_tokenize.py` & `mpi4jax-0.3.9/tests/experimental/test_auto_tokenize.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,20 @@
-import importlib
 import pytest
 
 from mpi4py import MPI
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
-from mpi4jax._src.jax_compat import versiontuple
-
 comm = MPI.COMM_WORLD
 rank = comm.Get_rank()
 size = comm.Get_size()
 
-jax_version = versiontuple(jax.__version__)
-min_version = versiontuple("0.2.27")
-
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_allreduce():
     from mpi4jax import allreduce
     from mpi4jax.experimental import auto_tokenize
 
     arr = jnp.ones((3, 2))
 
     def f(a):
@@ -29,15 +22,14 @@
         res, _ = allreduce(res, op=MPI.SUM)
         return res
 
     res = auto_tokenize(f)(arr)
     np.testing.assert_allclose(res, arr * size**2)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_nested_jits():
     from mpi4jax import allreduce
     from mpi4jax.experimental import auto_tokenize
 
     arr = jnp.ones((3, 2))
 
     @jax.jit
@@ -54,15 +46,14 @@
         res = g(res)
         return res
 
     res = auto_tokenize(f)(arr)
     np.testing.assert_allclose(res, arr * size**5)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 @pytest.mark.skipif(size < 2, reason="need 2 processes")
 def test_send_recv_tokenizer():
     from mpi4jax import recv, send
     from mpi4jax.experimental import auto_tokenize
 
     def simple_message_pass(arr):
         if rank == 0:
@@ -77,15 +68,14 @@
     res = jax.jit(auto_tokenize(simple_message_pass))(jnp.zeros((2, 2)))
     if rank == 0:
         np.testing.assert_allclose(res, jnp.ones((2, 2)))
     if rank == 1:
         np.testing.assert_allclose(res, jnp.zeros((2, 2)))
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 @pytest.mark.skipif(size < 2, reason="need 2 processes")
 def test_send_recv_hotpotato_tokenizer():
     from mpi4jax import recv, send, barrier
     from mpi4jax.experimental import auto_tokenize
 
     def hot_potato(arr):
         # Here, we test a send/recv pattern that is extremely likely to return the
@@ -133,15 +123,14 @@
     # Assert to ourselves the results are correct.
     if rank == 0:
         np.testing.assert_allclose(jitted_tokenized, jnp.ones((2, 2)) * -4)
     if rank == 1:
         np.testing.assert_allclose(jitted_tokenized, jnp.ones((2, 2)) * 11)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_fori_loop_tokenizer():
     from mpi4jax import allreduce
     from mpi4jax.experimental import auto_tokenize
 
     NUM_LOOPS = 6
 
     def sum_loop(i, args):
@@ -152,15 +141,14 @@
     def my_method(arr):
         return jax.lax.fori_loop(0, NUM_LOOPS, sum_loop, [arr])
 
     res = jax.jit(auto_tokenize(my_method))(jnp.ones((2, 2)))
     np.testing.assert_allclose(res[0], np.ones((2, 2)) * size**NUM_LOOPS)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_while_loop_tokenizer():
     from mpi4jax import allreduce
     from mpi4jax.experimental import auto_tokenize
 
     def sum_loop(arr):
         res, _ = allreduce(arr, op=MPI.SUM)
         res = res + 1
@@ -172,15 +160,14 @@
     def my_method(arr):
         return jax.lax.while_loop(cond, sum_loop, arr)
 
     res = jax.jit(auto_tokenize(my_method))(jnp.ones((2, 2)))
     assert (res >= np.ones((2, 2)) * 1000).all()
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_cond_tokenizer():
     from mpi4jax import allreduce
     from mpi4jax.experimental import auto_tokenize
 
     def branch1(arr):
         res, _ = allreduce(arr, op=MPI.PROD)
         return res
@@ -198,42 +185,39 @@
     res2 = jax.jit(auto_tokenize(my_method))(
         jnp.asarray(False), jnp.ones((2, 2), dtype=jnp.int32)
     ).block_until_ready()
     assert (res1 == 1).all()
     assert (res2 == size).all()
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_allgather_scalar():
     from mpi4jax import allgather
     from mpi4jax.experimental import auto_tokenize
 
     @jax.jit
     @auto_tokenize
     def f(arr):
         res, _ = allgather(arr)
         return res
 
     res = f(jnp.asarray(rank))
     assert jnp.array_equal(res, jnp.arange(size))
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_alltoall_jit():
     from mpi4jax import alltoall
     from mpi4jax.experimental import auto_tokenize
 
     arr = jnp.ones((size, 3, 2)) * rank
 
     res = jax.jit(auto_tokenize(lambda x: alltoall(x)[0]))(arr)
     for p in range(size):
         assert jnp.array_equal(res[p], jnp.ones((3, 2)) * p)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_bcast_scalar_jit():
     from mpi4jax import bcast
     from mpi4jax.experimental import auto_tokenize
 
     arr = 1
     _arr = 1
 
@@ -242,65 +226,60 @@
 
     res = jax.jit(auto_tokenize(lambda x: bcast(x, root=0)[0]))(_arr)
     assert jnp.array_equal(res, arr)
     if rank == 0:
         assert jnp.array_equal(_arr, arr)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_gather_scalar_jit():
     from mpi4jax import gather
     from mpi4jax.experimental import auto_tokenize
 
     arr = rank
     res = jax.jit(auto_tokenize(lambda x: gather(x, root=0)[0]))(arr)
     if rank == 0:
         assert jnp.array_equal(res, jnp.arange(size))
     else:
         assert jnp.array_equal(res, arr)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_reduce_scalar_jit():
     from mpi4jax import reduce
     from mpi4jax.experimental import auto_tokenize
 
     arr = rank
     res = jax.jit(auto_tokenize(lambda x: reduce(x, op=MPI.SUM, root=0)[0]))(arr)
     if rank == 0:
         assert jnp.array_equal(res, sum(range(size)))
     else:
         assert jnp.array_equal(res, arr)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_scan_scalar_jit():
     from mpi4jax import scan
     from mpi4jax.experimental import auto_tokenize
 
     arr = rank
     res = jax.jit(auto_tokenize(lambda x: scan(x, op=MPI.SUM)[0]))(arr)
     assert jnp.array_equal(res, sum(range(rank + 1)))
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 def test_scatter_jit():
     from mpi4jax import scatter
     from mpi4jax.experimental import auto_tokenize
 
     if rank == 0:
         arr = jnp.stack([jnp.ones((3, 2)) * r for r in range(size)], axis=0)
     else:
         arr = jnp.ones((3, 2)) * rank
 
     res = jax.jit(auto_tokenize(lambda x: scatter(x, root=0)[0]))(arr)
     assert jnp.array_equal(res, jnp.ones((3, 2)) * rank)
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 @pytest.mark.skipif(size < 2 or rank > 1, reason="Runs only on rank 0 and 1")
 def test_sendrecv_status_jit():
     from mpi4jax import sendrecv
     from mpi4jax.experimental import auto_tokenize
 
     arr = jnp.ones((3, 2)) * rank
     _arr = arr.copy()
@@ -315,15 +294,14 @@
     )(arr, arr)
 
     assert jnp.array_equal(res, jnp.ones_like(arr) * other)
     assert jnp.array_equal(_arr, arr)
     assert status.Get_source() == other
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 @pytest.mark.skipif(size < 2 or rank > 1, reason="Runs only on rank 0 and 1")
 def test_while_loop_consistency():
     from mpi4jax import allreduce, sendrecv, barrier
     from mpi4jax.experimental import auto_tokenize
 
     def cond(value):
         barrier()
@@ -343,15 +321,14 @@
     def run(value):
         return jax.lax.while_loop(cond, loop, value)
 
     res = run(1.0)
     assert res >= 10
 
 
-@pytest.mark.skipif(jax_version < min_version, reason="Requires more recent JAX")
 @pytest.mark.skipif(size < 2 or rank > 1, reason="Runs only on rank 0 and 1")
 def test_cond_consistency():
     from mpi4jax import recv, send
     from mpi4jax.experimental import auto_tokenize
 
     def hot_potato_right(args):
         arr, t = args
@@ -393,20 +370,7 @@
 
     if rank == 0:
         expected = -4
     else:
         expected = 11
 
     np.testing.assert_allclose(res, jnp.ones((2, 2)) * expected)
-
-
-def test_error_on_old_jax(monkeypatch):
-    with monkeypatch.context() as m:
-        fake_version = "0.0.0"
-        m.setattr(jax, "__version__", fake_version)
-
-        with pytest.raises(RuntimeError) as excinfo:
-            import mpi4jax.experimental.tokenizer
-
-            importlib.reload(mpi4jax.experimental.tokenizer)
-
-        assert fake_version in str(excinfo.value)
```

### Comparing `mpi4jax-0.3.8/tests/test_decorators.py` & `mpi4jax-0.3.9/tests/test_decorators.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,27 +10,14 @@
     assert not _is_truthy("false")
     assert _is_falsy("false")
 
     assert not _is_truthy("foo")
     assert not _is_falsy("foo")
 
 
-def test_missing_omnistaging(monkeypatch):
-    import jax
-    from mpi4jax._src.decorators import ensure_omnistaging
-
-    with monkeypatch.context() as m:
-        m.setattr(jax.config, "omnistaging_enabled", False)
-
-        with pytest.raises(RuntimeError) as excinfo:
-            ensure_omnistaging()
-
-        assert "omnistaging" in str(excinfo.value)
-
-
 def test_ensure_gpu_ext(monkeypatch):
     from mpi4jax._src import xla_bridge
     from mpi4jax._src.decorators import ensure_gpu_ext
 
     with monkeypatch.context() as m:
         m.setattr(xla_bridge, "HAS_GPU_EXT", False)
```

### Comparing `mpi4jax-0.3.8/tests/test_validation.py` & `mpi4jax-0.3.9/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `mpi4jax-0.3.8/versioneer.py` & `mpi4jax-0.3.9/versioneer.py`

 * *Files identical despite different names*

