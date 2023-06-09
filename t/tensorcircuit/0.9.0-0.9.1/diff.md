# Comparing `tmp/tensorcircuit-0.9.0.tar.gz` & `tmp/tensorcircuit-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tensorcircuit-0.9.0.tar", last modified: Fri May  5 09:12:51 2023, max compression
+gzip compressed data, was "dist/tensorcircuit-0.9.1.tar", last modified: Mon May 15 03:15:29 2023, max compression
```

## Comparing `tensorcircuit-0.9.0.tar` & `tensorcircuit-0.9.1.tar`

### file list

```diff
@@ -1,169 +1,170 @@
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.252808 tensorcircuit-0.9.0/
--rw-r--r--   0 shixin     (501) staff       (20)    23650 2023-05-05 09:07:43.000000 tensorcircuit-0.9.0/CHANGELOG.md
--rw-r--r--   0 shixin     (501) staff       (20)     1023 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/HISTORY.md
--rw-r--r--   0 shixin     (501) staff       (20)    11358 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/LICENSE
--rw-r--r--   0 shixin     (501) staff       (20)      132 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/MANIFEST.in
--rw-r--r--   0 shixin     (501) staff       (20)    18126 2023-05-05 09:12:51.252232 tensorcircuit-0.9.0/PKG-INFO
--rw-r--r--   0 shixin     (501) staff       (20)    17577 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/README.md
--rw-r--r--   0 shixin     (501) staff       (20)     5352 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/README_cn.md
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:50.834058 tensorcircuit-0.9.0/docs/
--rw-r--r--   0 shixin     (501) staff       (20)      614 2020-04-19 06:32:37.000000 tensorcircuit-0.9.0/docs/Makefile
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:50.876685 tensorcircuit-0.9.0/docs/source/
--rw-r--r--   0 shixin     (501) staff       (20)     6148 2022-06-10 06:25:56.000000 tensorcircuit-0.9.0/docs/source/.DS_Store
--rw-r--r--   0 shixin     (501) staff       (20)     6332 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/advance.rst
--rw-r--r--   0 shixin     (501) staff       (20)     6308 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/cnconf.py
--rw-r--r--   0 shixin     (501) staff       (20)     6367 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/conf.py
--rw-r--r--   0 shixin     (501) staff       (20)     8192 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/contribution.rst
--rw-r--r--   0 shixin     (501) staff       (20)    10971 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/faq.rst
--rw-r--r--   0 shixin     (501) staff       (20)     3677 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/generate_rst.py
--rw-r--r--   0 shixin     (501) staff       (20)     2551 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/index.rst
--rw-r--r--   0 shixin     (501) staff       (20)      374 2022-05-17 08:27:32.000000 tensorcircuit-0.9.0/docs/source/index_cn.rst.disable
--rw-r--r--   0 shixin     (501) staff       (20)     8413 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/infras.rst
--rw-r--r--   0 shixin     (501) staff       (20)      660 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/docs/source/modules.rst
--rw-r--r--   0 shixin     (501) staff       (20)     4334 2022-04-13 08:43:33.000000 tensorcircuit-0.9.0/docs/source/modules.rst.backup
--rw-r--r--   0 shixin     (501) staff       (20)    27390 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/docs/source/quickstart.rst
--rw-r--r--   0 shixin     (501) staff       (20)     8223 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/docs/source/sharpbits.rst
--rw-r--r--   0 shixin     (501) staff       (20)      226 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/docs/source/textbooktoc.rst
--rw-r--r--   0 shixin     (501) staff       (20)      674 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/docs/source/tutorial.rst
--rw-r--r--   0 shixin     (501) staff       (20)      669 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/docs/source/tutorial_cn.rst
--rw-r--r--   0 shixin     (501) staff       (20)      509 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/docs/source/whitepapertoc.rst
--rw-r--r--   0 shixin     (501) staff       (20)      531 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/docs/source/whitepapertoc_cn.rst
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.003783 tensorcircuit-0.9.0/examples/
--rw-r--r--   0 shixin     (501) staff       (20)     2173 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/GHZ_DQAS.py
--rw-r--r--   0 shixin     (501) staff       (20)    61992 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/H6_hamiltonian.npy
--rw-r--r--   0 shixin     (501) staff       (20)     3984 2023-04-21 04:22:17.000000 tensorcircuit-0.9.0/examples/QAOA_DQAS.py
--rw-r--r--   0 shixin     (501) staff       (20)     1304 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/QEM_DQAS.py
--rw-r--r--   0 shixin     (501) staff       (20)     3346 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/adiabatic_vqnhe.py
--rw-r--r--   0 shixin     (501) staff       (20)     2574 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/chaotic_behavior.py
--rw-r--r--   0 shixin     (501) staff       (20)     2760 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/checkpoint_memsave.py
--rw-r--r--   0 shixin     (501) staff       (20)     6713 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/gradient_benchmark.py
--rw-r--r--   0 shixin     (501) staff       (20)      950 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/hamiltonian_building.py
--rw-r--r--   0 shixin     (501) staff       (20)     1729 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/hchainhamiltonian.py
--rw-r--r--   0 shixin     (501) staff       (20)     1885 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/incremental_twoqubit.py
--rw-r--r--   0 shixin     (501) staff       (20)     2593 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/mcnoise_boost.py
--rw-r--r--   0 shixin     (501) staff       (20)     1676 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/mcnoise_check.py
--rw-r--r--   0 shixin     (501) staff       (20)     2399 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/mpsvsexact.py
--rw-r--r--   0 shixin     (501) staff       (20)     5217 2023-04-21 04:23:12.000000 tensorcircuit-0.9.0/examples/noisy_qml.py
--rw-r--r--   0 shixin     (501) staff       (20)     2290 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/optperformance_comparison.py
--rw-r--r--   0 shixin     (501) staff       (20)      971 2021-11-17 07:46:30.000000 tensorcircuit-0.9.0/examples/qaoa_block.result
--rw-r--r--   0 shixin     (501) staff       (20)      736 2022-02-17 02:39:55.000000 tensorcircuit-0.9.0/examples/qaoa_graph.py.outdated
--rw-r--r--   0 shixin     (501) staff       (20)     1145 2022-02-17 02:39:48.000000 tensorcircuit-0.9.0/examples/qaoa_micro.py.outdated
--rw-r--r--   0 shixin     (501) staff       (20)      814 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/qaoa_parallel_opt.py
--rw-r--r--   0 shixin     (501) staff       (20)     2523 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/quantumng.py
--rw-r--r--   0 shixin     (501) staff       (20)     2201 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/simple_qaoa.py
--rw-r--r--   0 shixin     (501) staff       (20)     2628 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/examples/universal_lr.py
--rw-r--r--   0 shixin     (501) staff       (20)     3412 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/variational_dynamics.py
--rw-r--r--   0 shixin     (501) staff       (20)     3533 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqe_extra.py
--rw-r--r--   0 shixin     (501) staff       (20)     3989 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqe_extra_mpo.py
--rw-r--r--   0 shixin     (501) staff       (20)     4094 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqe_extra_mpo_spopt.py
--rw-r--r--   0 shixin     (501) staff       (20)     4004 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/examples/vqeh2o_benchmark.py
--rw-r--r--   0 shixin     (501) staff       (20)     1006 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/examples/vqnhe_h6.py
--rw-r--r--   0 shixin     (501) staff       (20)       38 2023-05-05 09:12:51.253770 tensorcircuit-0.9.0/setup.cfg
--rw-r--r--   0 shixin     (501) staff       (20)      968 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/setup.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.116136 tensorcircuit-0.9.0/tensorcircuit/
--rw-r--r--   0 shixin     (501) staff       (20)     1395 2023-05-05 09:07:31.000000 tensorcircuit-0.9.0/tensorcircuit/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     2901 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/about.py
--rw-r--r--   0 shixin     (501) staff       (20)    39188 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/abstractcircuit.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.132756 tensorcircuit-0.9.0/tensorcircuit/applications/
--rw-r--r--   0 shixin     (501) staff       (20)      234 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/tensorcircuit/applications/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)    34460 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/dqas.py
--rw-r--r--   0 shixin     (501) staff       (20)    15348 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/applications/graphdata.py
--rw-r--r--   0 shixin     (501) staff       (20)    18124 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/layers.py
--rw-r--r--   0 shixin     (501) staff       (20)    14032 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/utils.py
--rw-r--r--   0 shixin     (501) staff       (20)    36391 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/vags.py
--rw-r--r--   0 shixin     (501) staff       (20)    15117 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/van.py
--rw-r--r--   0 shixin     (501) staff       (20)    23156 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/applications/vqes.py
--rw-r--r--   0 shixin     (501) staff       (20)     8235 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/asciiart.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.160683 tensorcircuit-0.9.0/tensorcircuit/backends/
--rw-r--r--   0 shixin     (501) staff       (20)       80 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/backends/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)    57621 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/abstract_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     1713 2023-04-11 04:16:09.000000 tensorcircuit-0.9.0/tensorcircuit/backends/backend_factory.py
--rw-r--r--   0 shixin     (501) staff       (20)    14928 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/cupy_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)    24925 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/jax_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     4008 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/backends/jax_ops.py
--rw-r--r--   0 shixin     (501) staff       (20)    13813 2023-04-21 07:14:14.000000 tensorcircuit-0.9.0/tensorcircuit/backends/numpy_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)    24148 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     3825 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_ops.py
--rw-r--r--   0 shixin     (501) staff       (20)    31112 2023-05-05 08:09:14.000000 tensorcircuit-0.9.0/tensorcircuit/backends/tensorflow_backend.py
--rw-r--r--   0 shixin     (501) staff       (20)     3377 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/backends/tf_ops.py
--rw-r--r--   0 shixin     (501) staff       (20)    34020 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/basecircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)    28637 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/channels.py
--rw-r--r--   0 shixin     (501) staff       (20)    36220 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/circuit.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.177968 tensorcircuit-0.9.0/tensorcircuit/cloud/
--rw-r--r--   0 shixin     (501) staff       (20)        0 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)    14582 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/abstraction.py
--rw-r--r--   0 shixin     (501) staff       (20)    17577 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/apis.py
--rw-r--r--   0 shixin     (501) staff       (20)       60 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/config.py
--rw-r--r--   0 shixin     (501) staff       (20)     2252 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/local.py
--rw-r--r--   0 shixin     (501) staff       (20)     2238 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/quafu_provider.py
--rw-r--r--   0 shixin     (501) staff       (20)    14212 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/tencent.py
--rw-r--r--   0 shixin     (501) staff       (20)     3622 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/utils.py
--rw-r--r--   0 shixin     (501) staff       (20)     5764 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tensorcircuit/cloud/wrapper.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.181850 tensorcircuit-0.9.0/tensorcircuit/compiler/
--rw-r--r--   0 shixin     (501) staff       (20)      165 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/compiler/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     1490 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/compiler/composed_compiler.py
--rw-r--r--   0 shixin     (501) staff       (20)     5215 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/compiler/qiskit_compiler.py
--rw-r--r--   0 shixin     (501) staff       (20)    28754 2023-04-10 07:26:28.000000 tensorcircuit-0.9.0/tensorcircuit/cons.py
--rw-r--r--   0 shixin     (501) staff       (20)    13806 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/densitymatrix.py
--rw-r--r--   0 shixin     (501) staff       (20)    15210 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/experimental.py
--rw-r--r--   0 shixin     (501) staff       (20)    29016 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/gates.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.189430 tensorcircuit-0.9.0/tensorcircuit/interfaces/
--rw-r--r--   0 shixin     (501) staff       (20)      469 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     1439 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/numpy.py
--rw-r--r--   0 shixin     (501) staff       (20)     3402 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/scipy.py
--rw-r--r--   0 shixin     (501) staff       (20)     3355 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/tensorflow.py
--rw-r--r--   0 shixin     (501) staff       (20)    10364 2023-04-27 04:12:44.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/tensortrans.py
--rw-r--r--   0 shixin     (501) staff       (20)     5030 2023-04-27 04:52:54.000000 tensorcircuit-0.9.0/tensorcircuit/interfaces/torch.py
--rw-r--r--   0 shixin     (501) staff       (20)     9959 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/keras.py
--rw-r--r--   0 shixin     (501) staff       (20)    15270 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/mps_base.py
--rw-r--r--   0 shixin     (501) staff       (20)    34350 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/mpscircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)    11861 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/noisemodel.py
--rw-r--r--   0 shixin     (501) staff       (20)    82850 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tensorcircuit/quantum.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.193887 tensorcircuit-0.9.0/tensorcircuit/results/
--rw-r--r--   0 shixin     (501) staff       (20)       89 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/results/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     3366 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/results/counts.py
--rw-r--r--   0 shixin     (501) staff       (20)    31362 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/results/readout_mitigation.py
--rw-r--r--   0 shixin     (501) staff       (20)     9413 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/simplify.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.203609 tensorcircuit-0.9.0/tensorcircuit/templates/
--rw-r--r--   0 shixin     (501) staff       (20)      111 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/tensorcircuit/templates/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     6158 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/templates/blocks.py
--rw-r--r--   0 shixin     (501) staff       (20)     1061 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/templates/chems.py
--rw-r--r--   0 shixin     (501) staff       (20)     1933 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/templates/dataset.py
--rw-r--r--   0 shixin     (501) staff       (20)     5811 2023-04-11 04:19:05.000000 tensorcircuit-0.9.0/tensorcircuit/templates/ensemble.py
--rw-r--r--   0 shixin     (501) staff       (20)     3934 2022-07-06 06:14:53.000000 tensorcircuit-0.9.0/tensorcircuit/templates/graphs.py
--rw-r--r--   0 shixin     (501) staff       (20)    10942 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/templates/measurements.py
--rw-r--r--   0 shixin     (501) staff       (20)     3552 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/torchnn.py
--rw-r--r--   0 shixin     (501) staff       (20)    27335 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/translation.py
--rw-r--r--   0 shixin     (501) staff       (20)     7060 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tensorcircuit/utils.py
--rw-r--r--   0 shixin     (501) staff       (20)    12195 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tensorcircuit/vis.py
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.120831 tensorcircuit-0.9.0/tensorcircuit.egg-info/
--rw-r--r--   0 shixin     (501) staff       (20)    18126 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/PKG-INFO
--rw-r--r--   0 shixin     (501) staff       (20)     4367 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/SOURCES.txt
--rw-r--r--   0 shixin     (501) staff       (20)        1 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/dependency_links.txt
--rw-r--r--   0 shixin     (501) staff       (20)      133 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/requires.txt
--rw-r--r--   0 shixin     (501) staff       (20)       20 2023-05-05 09:12:50.000000 tensorcircuit-0.9.0/tensorcircuit.egg-info/top_level.txt
-drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-05 09:12:51.251106 tensorcircuit-0.9.0/tests/
--rw-r--r--   0 shixin     (501) staff       (20)        0 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/tests/__init__.py
--rw-r--r--   0 shixin     (501) staff       (20)     1457 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tests/conftest.py
--rw-r--r--   0 shixin     (501) staff       (20)    33394 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tests/test_backends.py
--rw-r--r--   0 shixin     (501) staff       (20)     3805 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_calibrating.py
--rw-r--r--   0 shixin     (501) staff       (20)    11237 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_channels.py
--rw-r--r--   0 shixin     (501) staff       (20)    46467 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tests/test_circuit.py
--rw-r--r--   0 shixin     (501) staff       (20)     4204 2023-05-05 09:07:02.000000 tensorcircuit-0.9.0/tests/test_cloud.py
--rw-r--r--   0 shixin     (501) staff       (20)     2518 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_compiler.py
--rw-r--r--   0 shixin     (501) staff       (20)    17232 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_dmcircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)     1974 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_ensemble.py
--rw-r--r--   0 shixin     (501) staff       (20)     4593 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_gates.py
--rw-r--r--   0 shixin     (501) staff       (20)    13220 2023-04-25 09:21:10.000000 tensorcircuit-0.9.0/tests/test_interfaces.py
--rw-r--r--   0 shixin     (501) staff       (20)     4656 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_keras.py
--rw-r--r--   0 shixin     (501) staff       (20)     6639 2023-04-17 12:12:38.000000 tensorcircuit-0.9.0/tests/test_miscs.py
--rw-r--r--   0 shixin     (501) staff       (20)    10552 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_mpscircuit.py
--rw-r--r--   0 shixin     (501) staff       (20)     5637 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_noisemodel.py
--rw-r--r--   0 shixin     (501) staff       (20)      753 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_qaoa.py
--rw-r--r--   0 shixin     (501) staff       (20)    16823 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_quantum.py
--rw-r--r--   0 shixin     (501) staff       (20)     1245 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_quantum_attr.py
--rw-r--r--   0 shixin     (501) staff       (20)    11050 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_results.py
--rw-r--r--   0 shixin     (501) staff       (20)     1175 2021-12-08 02:25:17.000000 tensorcircuit-0.9.0/tests/test_simplify.py
--rw-r--r--   0 shixin     (501) staff       (20)     5962 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_templates.py
--rw-r--r--   0 shixin     (501) staff       (20)     2039 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_torchnn.py
--rw-r--r--   0 shixin     (501) staff       (20)     3163 2023-04-10 07:26:29.000000 tensorcircuit-0.9.0/tests/test_van.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.403403 tensorcircuit-0.9.1/
+-rw-r--r--   0 shixin     (501) staff       (20)    24590 2023-05-15 03:10:39.000000 tensorcircuit-0.9.1/CHANGELOG.md
+-rw-r--r--   0 shixin     (501) staff       (20)     1023 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/HISTORY.md
+-rw-r--r--   0 shixin     (501) staff       (20)    11358 2021-12-08 02:25:17.000000 tensorcircuit-0.9.1/LICENSE
+-rw-r--r--   0 shixin     (501) staff       (20)      132 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/MANIFEST.in
+-rw-r--r--   0 shixin     (501) staff       (20)    18909 2023-05-15 03:15:29.402958 tensorcircuit-0.9.1/PKG-INFO
+-rw-r--r--   0 shixin     (501) staff       (20)    18360 2023-05-12 05:45:29.000000 tensorcircuit-0.9.1/README.md
+-rw-r--r--   0 shixin     (501) staff       (20)     6097 2023-05-12 05:45:29.000000 tensorcircuit-0.9.1/README_cn.md
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.245179 tensorcircuit-0.9.1/docs/
+-rw-r--r--   0 shixin     (501) staff       (20)      614 2020-04-19 06:32:37.000000 tensorcircuit-0.9.1/docs/Makefile
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.261998 tensorcircuit-0.9.1/docs/source/
+-rw-r--r--   0 shixin     (501) staff       (20)     6148 2022-06-10 06:25:56.000000 tensorcircuit-0.9.1/docs/source/.DS_Store
+-rw-r--r--   0 shixin     (501) staff       (20)     6332 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/docs/source/advance.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     6308 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/docs/source/cnconf.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6440 2023-05-10 13:16:21.000000 tensorcircuit-0.9.1/docs/source/conf.py
+-rw-r--r--   0 shixin     (501) staff       (20)     8192 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/docs/source/contribution.rst
+-rw-r--r--   0 shixin     (501) staff       (20)    10971 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/docs/source/faq.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     3677 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/docs/source/generate_rst.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3326 2023-05-12 05:45:29.000000 tensorcircuit-0.9.1/docs/source/index.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      374 2022-05-17 08:27:32.000000 tensorcircuit-0.9.1/docs/source/index_cn.rst.disable
+-rw-r--r--   0 shixin     (501) staff       (20)    10071 2023-05-12 06:36:49.000000 tensorcircuit-0.9.1/docs/source/infras.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      680 2023-05-09 08:00:01.000000 tensorcircuit-0.9.1/docs/source/modules.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     4334 2022-04-13 08:43:33.000000 tensorcircuit-0.9.1/docs/source/modules.rst.backup
+-rw-r--r--   0 shixin     (501) staff       (20)    27533 2023-05-06 08:44:28.000000 tensorcircuit-0.9.1/docs/source/quickstart.rst
+-rw-r--r--   0 shixin     (501) staff       (20)     8223 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/docs/source/sharpbits.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      226 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/docs/source/textbooktoc.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      674 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/docs/source/tutorial.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      669 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/docs/source/tutorial_cn.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      509 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/docs/source/whitepapertoc.rst
+-rw-r--r--   0 shixin     (501) staff       (20)      531 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/docs/source/whitepapertoc_cn.rst
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.292939 tensorcircuit-0.9.1/examples/
+-rw-r--r--   0 shixin     (501) staff       (20)     2173 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/GHZ_DQAS.py
+-rw-r--r--   0 shixin     (501) staff       (20)    61992 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/H6_hamiltonian.npy
+-rw-r--r--   0 shixin     (501) staff       (20)     3984 2023-04-21 04:22:17.000000 tensorcircuit-0.9.1/examples/QAOA_DQAS.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1304 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/QEM_DQAS.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3346 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/adiabatic_vqnhe.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2574 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/chaotic_behavior.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2760 2023-05-05 15:08:03.000000 tensorcircuit-0.9.1/examples/checkpoint_memsave.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6713 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/gradient_benchmark.py
+-rw-r--r--   0 shixin     (501) staff       (20)      950 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/hamiltonian_building.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1729 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/hchainhamiltonian.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1885 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/incremental_twoqubit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2593 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/mcnoise_boost.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1676 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/mcnoise_check.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2399 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/mpsvsexact.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5217 2023-04-21 04:23:12.000000 tensorcircuit-0.9.1/examples/noisy_qml.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2290 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/optperformance_comparison.py
+-rw-r--r--   0 shixin     (501) staff       (20)      971 2021-11-17 07:46:30.000000 tensorcircuit-0.9.1/examples/qaoa_block.result
+-rw-r--r--   0 shixin     (501) staff       (20)      736 2022-02-17 02:39:55.000000 tensorcircuit-0.9.1/examples/qaoa_graph.py.outdated
+-rw-r--r--   0 shixin     (501) staff       (20)     1145 2022-02-17 02:39:48.000000 tensorcircuit-0.9.1/examples/qaoa_micro.py.outdated
+-rw-r--r--   0 shixin     (501) staff       (20)      814 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/qaoa_parallel_opt.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2523 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/quantumng.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2201 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/simple_qaoa.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2628 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/examples/universal_lr.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3412 2023-05-05 15:08:04.000000 tensorcircuit-0.9.1/examples/variational_dynamics.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3533 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/vqe_extra.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3989 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/vqe_extra_mpo.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4094 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/examples/vqe_extra_mpo_spopt.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4004 2023-05-05 15:08:04.000000 tensorcircuit-0.9.1/examples/vqeh2o_benchmark.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1006 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/examples/vqnhe_h6.py
+-rw-r--r--   0 shixin     (501) staff       (20)       38 2023-05-15 03:15:29.403600 tensorcircuit-0.9.1/setup.cfg
+-rw-r--r--   0 shixin     (501) staff       (20)      968 2023-05-05 09:07:02.000000 tensorcircuit-0.9.1/setup.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.317794 tensorcircuit-0.9.1/tensorcircuit/
+-rw-r--r--   0 shixin     (501) staff       (20)     1448 2023-05-15 03:10:53.000000 tensorcircuit-0.9.1/tensorcircuit/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2901 2023-04-17 12:12:38.000000 tensorcircuit-0.9.1/tensorcircuit/about.py
+-rw-r--r--   0 shixin     (501) staff       (20)    39188 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/tensorcircuit/abstractcircuit.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.332834 tensorcircuit-0.9.1/tensorcircuit/applications/
+-rw-r--r--   0 shixin     (501) staff       (20)      234 2021-12-08 02:25:17.000000 tensorcircuit-0.9.1/tensorcircuit/applications/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)    34460 2023-04-11 04:19:05.000000 tensorcircuit-0.9.1/tensorcircuit/applications/dqas.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15348 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/tensorcircuit/applications/graphdata.py
+-rw-r--r--   0 shixin     (501) staff       (20)    18124 2023-04-11 04:19:05.000000 tensorcircuit-0.9.1/tensorcircuit/applications/layers.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14032 2023-05-05 15:08:05.000000 tensorcircuit-0.9.1/tensorcircuit/applications/utils.py
+-rw-r--r--   0 shixin     (501) staff       (20)    36391 2023-05-05 15:08:08.000000 tensorcircuit-0.9.1/tensorcircuit/applications/vags.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15117 2023-05-05 15:08:05.000000 tensorcircuit-0.9.1/tensorcircuit/applications/van.py
+-rw-r--r--   0 shixin     (501) staff       (20)    23416 2023-05-12 06:36:49.000000 tensorcircuit-0.9.1/tensorcircuit/applications/vqes.py
+-rw-r--r--   0 shixin     (501) staff       (20)     8235 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/tensorcircuit/asciiart.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.345689 tensorcircuit-0.9.1/tensorcircuit/backends/
+-rw-r--r--   0 shixin     (501) staff       (20)       80 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/tensorcircuit/backends/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)    57621 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/backends/abstract_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1713 2023-04-11 04:16:09.000000 tensorcircuit-0.9.1/tensorcircuit/backends/backend_factory.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14928 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/backends/cupy_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)    24925 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/backends/jax_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4024 2023-05-08 09:14:10.000000 tensorcircuit-0.9.1/tensorcircuit/backends/jax_ops.py
+-rw-r--r--   0 shixin     (501) staff       (20)    13813 2023-04-21 07:14:14.000000 tensorcircuit-0.9.1/tensorcircuit/backends/numpy_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)    24148 2023-04-17 12:12:38.000000 tensorcircuit-0.9.1/tensorcircuit/backends/pytorch_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3825 2023-04-17 12:12:38.000000 tensorcircuit-0.9.1/tensorcircuit/backends/pytorch_ops.py
+-rw-r--r--   0 shixin     (501) staff       (20)    31112 2023-05-05 08:09:14.000000 tensorcircuit-0.9.1/tensorcircuit/backends/tensorflow_backend.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3377 2023-04-11 04:19:05.000000 tensorcircuit-0.9.1/tensorcircuit/backends/tf_ops.py
+-rw-r--r--   0 shixin     (501) staff       (20)    34020 2023-04-10 07:26:28.000000 tensorcircuit-0.9.1/tensorcircuit/basecircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)    28637 2023-05-05 15:08:07.000000 tensorcircuit-0.9.1/tensorcircuit/channels.py
+-rw-r--r--   0 shixin     (501) staff       (20)    36220 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/circuit.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.355278 tensorcircuit-0.9.1/tensorcircuit/cloud/
+-rw-r--r--   0 shixin     (501) staff       (20)       67 2023-05-06 08:44:28.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14582 2023-05-05 09:07:02.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/abstraction.py
+-rw-r--r--   0 shixin     (501) staff       (20)    17866 2023-05-08 09:14:10.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/apis.py
+-rw-r--r--   0 shixin     (501) staff       (20)       60 2023-05-05 09:07:02.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/config.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2252 2023-05-05 09:07:02.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/local.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2238 2023-05-05 09:07:02.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/quafu_provider.py
+-rw-r--r--   0 shixin     (501) staff       (20)    14222 2023-05-12 06:36:49.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/tencent.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3622 2023-05-05 09:07:02.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/utils.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10718 2023-05-12 06:36:49.000000 tensorcircuit-0.9.1/tensorcircuit/cloud/wrapper.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.360610 tensorcircuit-0.9.1/tensorcircuit/compiler/
+-rw-r--r--   0 shixin     (501) staff       (20)      241 2023-05-10 13:16:21.000000 tensorcircuit-0.9.1/tensorcircuit/compiler/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3258 2023-05-10 13:16:21.000000 tensorcircuit-0.9.1/tensorcircuit/compiler/composed_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6032 2023-05-09 08:50:24.000000 tensorcircuit-0.9.1/tensorcircuit/compiler/qiskit_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)     9595 2023-05-12 06:36:49.000000 tensorcircuit-0.9.1/tensorcircuit/compiler/simple_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)    29573 2023-05-08 09:14:10.000000 tensorcircuit-0.9.1/tensorcircuit/cons.py
+-rw-r--r--   0 shixin     (501) staff       (20)    13806 2023-05-05 15:08:07.000000 tensorcircuit-0.9.1/tensorcircuit/densitymatrix.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15210 2023-04-11 04:19:05.000000 tensorcircuit-0.9.1/tensorcircuit/experimental.py
+-rw-r--r--   0 shixin     (501) staff       (20)    29016 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/gates.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.366567 tensorcircuit-0.9.1/tensorcircuit/interfaces/
+-rw-r--r--   0 shixin     (501) staff       (20)      469 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/interfaces/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1439 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/interfaces/numpy.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3402 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/interfaces/scipy.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3355 2023-04-11 04:19:05.000000 tensorcircuit-0.9.1/tensorcircuit/interfaces/tensorflow.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10364 2023-04-27 04:12:44.000000 tensorcircuit-0.9.1/tensorcircuit/interfaces/tensortrans.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5030 2023-04-27 04:52:54.000000 tensorcircuit-0.9.1/tensorcircuit/interfaces/torch.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10126 2023-05-08 09:14:10.000000 tensorcircuit-0.9.1/tensorcircuit/keras.py
+-rw-r--r--   0 shixin     (501) staff       (20)    15270 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/mps_base.py
+-rw-r--r--   0 shixin     (501) staff       (20)    34350 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tensorcircuit/mpscircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)    11861 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/noisemodel.py
+-rw-r--r--   0 shixin     (501) staff       (20)    82850 2023-04-17 12:12:38.000000 tensorcircuit-0.9.1/tensorcircuit/quantum.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.369595 tensorcircuit-0.9.1/tensorcircuit/results/
+-rw-r--r--   0 shixin     (501) staff       (20)       89 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/results/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3366 2023-05-05 15:08:06.000000 tensorcircuit-0.9.1/tensorcircuit/results/counts.py
+-rw-r--r--   0 shixin     (501) staff       (20)    31362 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tensorcircuit/results/readout_mitigation.py
+-rw-r--r--   0 shixin     (501) staff       (20)     9413 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/simplify.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.376559 tensorcircuit-0.9.1/tensorcircuit/templates/
+-rw-r--r--   0 shixin     (501) staff       (20)      111 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/tensorcircuit/templates/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6158 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/templates/blocks.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1061 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/templates/chems.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1933 2023-05-05 15:08:06.000000 tensorcircuit-0.9.1/tensorcircuit/templates/dataset.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5811 2023-04-11 04:19:05.000000 tensorcircuit-0.9.1/tensorcircuit/templates/ensemble.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3934 2022-07-06 06:14:53.000000 tensorcircuit-0.9.1/tensorcircuit/templates/graphs.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10942 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/templates/measurements.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4621 2023-05-08 09:14:10.000000 tensorcircuit-0.9.1/tensorcircuit/torchnn.py
+-rw-r--r--   0 shixin     (501) staff       (20)    27335 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tensorcircuit/translation.py
+-rw-r--r--   0 shixin     (501) staff       (20)     7060 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tensorcircuit/utils.py
+-rw-r--r--   0 shixin     (501) staff       (20)    12195 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tensorcircuit/vis.py
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.323008 tensorcircuit-0.9.1/tensorcircuit.egg-info/
+-rw-r--r--   0 shixin     (501) staff       (20)    18909 2023-05-15 03:15:29.000000 tensorcircuit-0.9.1/tensorcircuit.egg-info/PKG-INFO
+-rw-r--r--   0 shixin     (501) staff       (20)     4409 2023-05-15 03:15:29.000000 tensorcircuit-0.9.1/tensorcircuit.egg-info/SOURCES.txt
+-rw-r--r--   0 shixin     (501) staff       (20)        1 2023-05-15 03:15:29.000000 tensorcircuit-0.9.1/tensorcircuit.egg-info/dependency_links.txt
+-rw-r--r--   0 shixin     (501) staff       (20)      133 2023-05-15 03:15:29.000000 tensorcircuit-0.9.1/tensorcircuit.egg-info/requires.txt
+-rw-r--r--   0 shixin     (501) staff       (20)       20 2023-05-15 03:15:29.000000 tensorcircuit-0.9.1/tensorcircuit.egg-info/top_level.txt
+drwxr-xr-x   0 shixin     (501) staff       (20)        0 2023-05-15 03:15:29.401984 tensorcircuit-0.9.1/tests/
+-rw-r--r--   0 shixin     (501) staff       (20)        0 2021-12-08 02:25:17.000000 tensorcircuit-0.9.1/tests/__init__.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1457 2023-04-17 12:12:38.000000 tensorcircuit-0.9.1/tests/conftest.py
+-rw-r--r--   0 shixin     (501) staff       (20)    33394 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tests/test_backends.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3805 2023-05-05 15:08:07.000000 tensorcircuit-0.9.1/tests/test_calibrating.py
+-rw-r--r--   0 shixin     (501) staff       (20)    11237 2023-05-05 15:08:08.000000 tensorcircuit-0.9.1/tests/test_channels.py
+-rw-r--r--   0 shixin     (501) staff       (20)    46467 2023-04-25 09:21:10.000000 tensorcircuit-0.9.1/tests/test_circuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5445 2023-05-12 06:36:49.000000 tensorcircuit-0.9.1/tests/test_cloud.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3419 2023-05-09 09:21:16.000000 tensorcircuit-0.9.1/tests/test_compiler.py
+-rw-r--r--   0 shixin     (501) staff       (20)    17232 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_dmcircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1974 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_ensemble.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4593 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_gates.py
+-rw-r--r--   0 shixin     (501) staff       (20)    13220 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tests/test_interfaces.py
+-rw-r--r--   0 shixin     (501) staff       (20)     4656 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tests/test_keras.py
+-rw-r--r--   0 shixin     (501) staff       (20)     6639 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tests/test_miscs.py
+-rw-r--r--   0 shixin     (501) staff       (20)    10552 2023-05-05 15:08:09.000000 tensorcircuit-0.9.1/tests/test_mpscircuit.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5637 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_noisemodel.py
+-rw-r--r--   0 shixin     (501) staff       (20)      753 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_qaoa.py
+-rw-r--r--   0 shixin     (501) staff       (20)    16823 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_quantum.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1245 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_quantum_attr.py
+-rw-r--r--   0 shixin     (501) staff       (20)    11050 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_results.py
+-rw-r--r--   0 shixin     (501) staff       (20)     1175 2021-12-08 02:25:17.000000 tensorcircuit-0.9.1/tests/test_simplify.py
+-rw-r--r--   0 shixin     (501) staff       (20)     5962 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_templates.py
+-rw-r--r--   0 shixin     (501) staff       (20)     2823 2023-05-08 09:14:10.000000 tensorcircuit-0.9.1/tests/test_torchnn.py
+-rw-r--r--   0 shixin     (501) staff       (20)     3163 2023-04-10 07:26:29.000000 tensorcircuit-0.9.1/tests/test_van.py
```

### Comparing `tensorcircuit-0.9.0/CHANGELOG.md` & `tensorcircuit-0.9.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,35 @@
 # Change Log
 
 ## Unreleased
 
+## 0.9.1
+
+### Added
+
+- Add `tc.TorchHardwarLayer` for shortcut layer construction of quantum hardware experiments
+
+- Add cotengra contractor setup shortcut
+
+- Add simplecompiler module to assite qiskit compile for better performance when targeting rz native basis
+
+### Changed
+
+- Add compiler and cloud namespace to the global tensorcircuit namespace
+
+- Refactor composed compiler pipeline interface to include simple_compiler, using `DefaultCompiler` for now (breaking)
+
+- Refactor `batch_submit_template` wrapper to make it a standard abstraction layer between tc cloud infras and `batch_expectation_ps` abstraction, providing another way to adpot other cloud providers with only `batch_submit_template` implemented
+
+### Fixed
+
+- `submit_task` return (list of dict vs dict) follows the data type of provided circuit instead of the number of circuits
+
+- Fix qubit mapping related bug when using `batch_expectation_ps` or `simple_compile`
+
 ## 0.9.0
 
 ### Added
 
 - Cloud module for Tencent QCloud is now merged into the master branch and ready to release
 
 - Add `tc.about()` to print related software versions and configs
```

### Comparing `tensorcircuit-0.9.0/HISTORY.md` & `tensorcircuit-0.9.1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/LICENSE` & `tensorcircuit-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/PKG-INFO` & `tensorcircuit-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: tensorcircuit
-Version: 0.9.0
-Summary: Quantum circuits on top of tensor network
-Home-page: https://github.com/tencent-quantum-lab/tensorcircuit
-Author: TensorCircuit Authors
-Author-email: shixinzhang@tencent.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-Provides-Extra: tensorflow
-Provides-Extra: jax
-Provides-Extra: torch
-Provides-Extra: qiskit
-Provides-Extra: cloud
-License-File: LICENSE
-
 <p align="center">
   <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
     <img width=90% src="docs/source/statics/logov2.jpg">
   </a>
 </p>
 
 <p align="center">
@@ -44,17 +25,17 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
 
-TensorCircuit is the next generation of quantum circuit simulators with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
 
-TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms.
+TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
 
 ## Getting Started
 
 Please begin with [Quick Start](/docs/source/quickstart.rst).
 
 For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
 
@@ -105,30 +86,32 @@
 
 We recommend you install this package with tensorflow also installed as:
 
 ```python
 pip install tensorcircuit[tensorflow]
 ```
 
-Other optional dependencies include `[torch]`, `[jax]` and `[qiskit]`.
+Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
 
 For the nightly build of tensorcircuit with new features, try:
 
 ```python
 pip uninstall tensorcircuit
 pip install tensorcircuit-nightly
 ```
 
 We also have [Docker support](/docker).
 
 ## Advantages
 
 - Tensor network simulation engine based
 
-- JIT, AD, vectorized parallelism compatible, GPU support
+- JIT, AD, vectorized parallelism compatible
+
+- GPU support, quantum device access support, hybrid deployment support
 
 - Efficiency
 
   - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
 
   - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
 
@@ -154,14 +137,18 @@
 
 ### Guidelines
 
 For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
 
 We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
 
+### License
+
+TensorCircuit is open source, released under the Apache License, Version 2.0.
+
 ### Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
@@ -209,25 +196,39 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## Research and Applications
 
 ### DQAS
 
 For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2010.08561.pdf (published in QST).
+
+Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
 
 ### VQNHE
 
 For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2106.05105.pdf (published in PRL) and https://arxiv.org/pdf/2112.10380.pdf.
 
-### VQEX - MBL
+Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
+
+### VQEX-MBL
 
 For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-Reference paper: https://arxiv.org/pdf/2111.13719.pdf (published in PRB).
 
-### Stark - DTC
+Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
+
+### Stark-DTC
 
 For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-Reference paper: https://arxiv.org/pdf/2208.02866.pdf (published in PRL).
 
+Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+
+### EMQAOA-DARBO
+
+For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+
+Reference paper: https://arxiv.org/abs/2303.14877.
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
 
+Reference paper: https://arxiv.org/abs/2303.10825.
```

### Comparing `tensorcircuit-0.9.0/README.md` & `tensorcircuit-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: tensorcircuit
+Version: 0.9.1
+Summary: Quantum circuits on top of tensor network
+Home-page: https://github.com/tencent-quantum-lab/tensorcircuit
+Author: TensorCircuit Authors
+Author-email: shixinzhang@tencent.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+Provides-Extra: tensorflow
+Provides-Extra: jax
+Provides-Extra: torch
+Provides-Extra: qiskit
+Provides-Extra: cloud
+License-File: LICENSE
+
 <p align="center">
   <a href="https://github.com/tencent-quantum-lab/tensorcircuit">
     <img width=90% src="docs/source/statics/logov2.jpg">
   </a>
 </p>
 
 <p align="center">
@@ -25,17 +44,17 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
 
-TensorCircuit is the next generation of quantum circuit simulators with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
 
-TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms.
+TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
 
 ## Getting Started
 
 Please begin with [Quick Start](/docs/source/quickstart.rst).
 
 For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
 
@@ -86,30 +105,32 @@
 
 We recommend you install this package with tensorflow also installed as:
 
 ```python
 pip install tensorcircuit[tensorflow]
 ```
 
-Other optional dependencies include `[torch]`, `[jax]` and `[qiskit]`.
+Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
 
 For the nightly build of tensorcircuit with new features, try:
 
 ```python
 pip uninstall tensorcircuit
 pip install tensorcircuit-nightly
 ```
 
 We also have [Docker support](/docker).
 
 ## Advantages
 
 - Tensor network simulation engine based
 
-- JIT, AD, vectorized parallelism compatible, GPU support
+- JIT, AD, vectorized parallelism compatible
+
+- GPU support, quantum device access support, hybrid deployment support
 
 - Efficiency
 
   - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
 
   - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
 
@@ -135,14 +156,18 @@
 
 ### Guidelines
 
 For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
 
 We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
 
+### License
+
+TensorCircuit is open source, released under the Apache License, Version 2.0.
+
 ### Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
@@ -190,23 +215,41 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## Research and Applications
 
 ### DQAS
 
 For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2010.08561.pdf (published in QST).
+
+Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
 
 ### VQNHE
 
 For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2106.05105.pdf (published in PRL) and https://arxiv.org/pdf/2112.10380.pdf.
 
-### VQEX - MBL
+Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
+
+### VQEX-MBL
 
 For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-Reference paper: https://arxiv.org/pdf/2111.13719.pdf (published in PRB).
 
-### Stark - DTC
+Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
+
+### Stark-DTC
 
 For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-Reference paper: https://arxiv.org/pdf/2208.02866.pdf (published in PRL).
+
+Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+
+### EMQAOA-DARBO
+
+For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+
+Reference paper: https://arxiv.org/abs/2303.14877.
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+
+Reference paper: https://arxiv.org/abs/2303.10825.
+
+
```

### Comparing `tensorcircuit-0.9.0/README_cn.md` & `tensorcircuit-0.9.1/README_cn.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,23 +21,25 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> <a href="README.md">English</a> |  简体中文 </p>
 
-TensorCircuit 是下一代量子电路模拟器，支持自动微分、即时编译、硬件加速和向量并行化。
+TensorCircuit 是下一代量子软件框架，支持自动微分、即时编译、硬件加速和向量并行化。
 
 TensorCircuit 建立在现代机器学习框架之上，并且与机器学习后端无关。 它特别适用于量子经典混合范式和变分量子算法的高效模拟。
 
+TensorCircuit 现在支持真实量子硬件连接和实验，并提供优雅的 CPU/GPU/QPU 混合部署方案（v0.9+）。
+
 ## 入门
 
 请从 [快速上手](/docs/source/quickstart.rst) 和 [Jupyter 教程](/docs/source/tutorials) 开始。
 
-有关更多信息和介绍，请参阅有用的 [示例脚本](/examples) 和 [完整文档](https://tensorcircuit.readthedocs.io/zh/latest/)。 [测试](/tests) 中的 API docstring 和测试用例也提供了丰富的信息。
+有关更多信息和介绍，请参阅有用的 [示例脚本](/examples) 和 [完整文档](https://tensorcircuit.readthedocs.io/zh/latest/)。 [测试](/tests)用例和 API docstring 也提供了丰富的使用信息。
 
 以下是一些最简易的演示。
 
 - 电路操作:
 
 ```python
 import tensorcircuit as tc
@@ -82,30 +84,32 @@
 
 我们推荐安装时同时安装 TensorFlow，这可以通过以下安装可选项实现：
 
 ```python
 pip install tensorcircuit[tensorflow]
 ```
 
-其他安装选项包括： `[torch]`, `[jax]` and `[qiskit]`。
+其他安装选项包括： `[torch]`, `[jax]`, `[qiskit]` 和 `[cloud]`。
 
 此外我们有每日发布的最新版本 pip package，可以尝鲜开发的最新功能，请通过以下方式安装:
 
 ```python
 pip uninstall tensorcircuit
 pip install tensorcircuit-nightly
 ```
 
 我们也有 [Docker 支持](/docker)。
 
 ## 优势
 
 - 基于张量网络模拟引擎
 
-- 即时编译、自动微分、向量并行化兼容，GPU 支持
+- 即时编译、自动微分、向量并行化兼容
+
+- GPU 支持、量子硬件支持、混合部署方案支持
 
 - 效率
 
   - 时间：与 TFQ, Pennylane, 或 Qiskit 相比，加速 10 到 10^6+ 倍
 
   - 空间：600+ qubits 1D VQE 工作流（收敛能量误差：< 1%）
 
@@ -129,28 +133,48 @@
 
 ### 说明
 
 有关贡献指南和说明，请参阅 [贡献](/CONTRIBUTING.md)。
 
 我们欢迎大家提出 [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PR](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), 和 [讨论](https://github.com/tencent-quantum-lab/tensorcircuit/discussions)，这些都托管在 GitHub 上。
 
+### 协议
+
+TensorCircuit 是基于 Apache License 2.0 的开源软件。
+
 ## 研究和应用
 
 ### DQAS
 
 可微量子架构搜索的应用见 [应用](/tensorcircuit/applications)。
-参考论文：https://arxiv.org/pdf/2010.08561.pdf (QST)。
+
+参考论文：https://arxiv.org/abs/2010.08561 (QST)。
 
 ### VQNHE
 
 关于变分量子神经混合本征求解器的应用，请参见 [应用](tensorcircuit/applications)。
-参考论文：https://arxiv.org/pdf/2106.05105.pdf (PRL) 和 https://arxiv.org/pdf/2112.10380.pdf 。
 
-### VQEX - MBL
+参考论文：https://arxiv.org/abs/2106.05105 (PRL) 和 https://arxiv.org/abs/2112.10380 。
+
+### VQEX-MBL
 
 VQEX 在 MBL 相位识别上的应用见 [教程](/docs/source/tutorials/vqex_mbl.ipynb)。
-参考论文: https://arxiv.org/pdf/2111.13719.pdf (PRB)。
 
-### Stark - DTC
+参考论文: https://arxiv.org/abs/2111.13719 (PRB)。
+
+### Stark-DTC
+
+数值验证 Stark 多体局域化稳定的离散时间晶体，类似的 Floquet 系统模拟请参考 [例子](/examples/timeevolution_trotter.py)。
+
+参考论文: https://arxiv.org/abs/2208.02866 (PRL)。
+
+### EMQAOA-DARBO
+
+数值模拟和带错误消除的真实量子硬件实验验证 QAOA 优化的代码请参考 [项目](https://github.com/sherrylixuecheng/EMQAOA-DARBO)。
+
+参考论文: https://arxiv.org/abs/2303.14877。
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) 是高效的，专注于处理和计算分子性质的量子计算软件。其基于 TensorCircuit 并为量子化学任务进行了专门的优化。
 
-数值验证 Stark 多体局域化稳定的离散时间晶体，类似的 Floquet 系统模拟请参考 [例子](/examples/timeevolution_trotter.py).
-参考论文: https://arxiv.org/pdf/2208.02866.pdf (PRL).
+参考论文: https://arxiv.org/abs/2303.10825。
```

### Comparing `tensorcircuit-0.9.0/docs/Makefile` & `tensorcircuit-0.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/.DS_Store` & `tensorcircuit-0.9.1/docs/source/.DS_Store`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/advance.rst` & `tensorcircuit-0.9.1/docs/source/advance.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/cnconf.py` & `tensorcircuit-0.9.1/docs/source/cnconf.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/conf.py` & `tensorcircuit-0.9.1/docs/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,16 @@
     "sphinx_copybutton",
     "nbsphinx",
     "toctree_filter",
     "sphinx.ext.napoleon",
     "myst_parser",
 ]
 
+nbsphinx_allow_errors = True
+
 autosectionlabel_prefix_document = True
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
@@ -140,14 +142,15 @@
 
 
 # -- Options for HTMLHelp output ---------------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = "tensorcircuitdoc"
 
+html_title = "TensorCircuit Documentation"
 
 # -- Options for LaTeX output ------------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
```

### Comparing `tensorcircuit-0.9.0/docs/source/contribution.rst` & `tensorcircuit-0.9.1/docs/source/contribution.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/faq.rst` & `tensorcircuit-0.9.1/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/generate_rst.py` & `tensorcircuit-0.9.1/docs/source/generate_rst.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/index.rst` & `tensorcircuit-0.9.1/docs/source/index.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,64 @@
-Guide to TensorCircuit
-==================================
+TensorCircuit Documentation
+===========================================================
 
 .. image:: https://github.com/tencent-quantum-lab/tensorcircuit/blob/master/docs/source/statics/logov2.jpg?raw=true
     :target: https://github.com/tencent-quantum-lab/tensorcircuit
 
-TensorCircuit is an open source quantum circuit and algorithm simulation framework.
 
-* It is built for human beings. 👽
+**Welcome and congratulations! You have found TensorCircuit.** 👏 
+
+TensorCircuit is an open-source high-performance quantum computing software framework in Python.
+
+* It is built for humans. 👽
 
 * It is designed for speed, flexibility and elegance. 🚀
 
 * It is empowered by advanced tensor network simulator engine. 🔋
 
+* It is ready for quantum hardware access with CPU/GPU/QPU (local/cloud) hybrid solutions. 🖥
+
 * It is implemented with industry-standard machine learning frameworks: TensorFlow, JAX, and PyTorch. 🤖
 
 * It is compatible with machine learning engineering paradigms: automatic differentiation, just-in-time compilation, vectorized parallelism and GPU acceleration. 🛠
 
-Links
-----------
+With the help of TensorCircuit, now get ready to efficiently and elegantly solve interesting and challenging quantum computing problems: from academic research prototype to industry application deployment.
+
+
+
+Relevant Links
+--------------------
+
+TensorCircuit is created and maintained by `Shi-Xin Zhang <https://github.com/refraction-ray>`_ and this version is released by `Tencent Quantum Lab <https://quantum.tencent.com/>`_.
 
-TensorCircuit is created and maintained by `Shi-Xin Zhang <https://github.com/refraction-ray>`_ and this version of the software is released by `Tencent Quantum Lab <https://quantum.tencent.com/>`_.
 The current core authors of TensorCircuit are `Shi-Xin Zhang <https://github.com/refraction-ray>`_ and `Yu-Qin Chen <https://github.com/yutuer21>`_.
 We also thank `contributions <https://github.com/tencent-quantum-lab/tensorcircuit/graphs/contributors>`_ from the lab and the open source community.
 
-* Source code: https://github.com/tencent-quantum-lab/tensorcircuit
+If you have any further questions or collaboration ideas, please use the issue tracker or forum below, or send email to shixinzhang#tencent.com.
+
 
-* Software Whitepaper in Quantum: https://quantum-journal.org/papers/q-2023-02-02-912/
+* Source code: https://github.com/tencent-quantum-lab/tensorcircuit
 
 * Documentation: https://tensorcircuit.readthedocs.io 
 
+* Software Whitepaper (published in Quantum): https://quantum-journal.org/papers/q-2023-02-02-912/
+
 * Issue Tracker: https://github.com/tencent-quantum-lab/tensorcircuit/issues
 
 * Forum: https://github.com/tencent-quantum-lab/tensorcircuit/discussions
 
 * PyPI page: https://pypi.org/project/tensorcircuit
 
 * DockerHub page: https://hub.docker.com/repository/docker/tensorcircuit/tensorcircuit
 
+* Research and projects based on TensorCircuit: https://github.com/tencent-quantum-lab/tensorcircuit#research-and-applications
+
+* Tencent Quantum Cloud Service: https://quantum.tencent.com/cloud/
+
+
 
 
 Reference Documentation
 ----------------------------
 
 The following documentation sections briefly introduce TensorCircuit to the users and developpers.
```

### Comparing `tensorcircuit-0.9.0/docs/source/infras.rst` & `tensorcircuit-0.9.1/docs/source/infras.rst`

 * *Files 11% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 - :py:mod:`tensorcircuit.densitymatrix`: Referenced and highly efficient implementation of ``tc.DMCircuit`` class, with similar set API of ``tc.Circuit`` while simulating the noise in the full form of the density matrix.
 
 - :py:mod:`tensorcircuit.noisemodel`: The global noise configuration and circuit noisy method APIs
 
 **ML Interfaces Related Modules:**
 
-- :py:mod:`tensorcircuit.interfaces`: Provide interfaces when quantum simulation backend is different from neural libraries. Currently include PyTorch and scipy optimizer interfaces.
+- :py:mod:`tensorcircuit.interfaces`: Provide interfaces when quantum simulation backend is different from neural libraries. Currently include PyTorch, TensorFlow, NumPy and SciPy optimizer interfaces.
 
 - :py:mod:`tensorcircuit.keras`: Provide TensorFlow Keras layers, as well as wrappers of jitted function, save/load from tf side.
 
 - :py:mod:`tensorcircuit.torchnn`: Provide PyTorch nn Modules.
 
 **MPS and MPO Utiliy Modules:**
 
@@ -58,15 +58,21 @@
 
 - :py:mod:`tensorcircuit.vis`: Visualization code for circuit drawing.
 
 - :py:mod:`tensorcircuit.translation`: Translate circuit object to circuit object in other quantum packages.
 
 **Processing and error mitigation on sample results:**
 
-- :py:mod:`tensorcircuit.results`: Provide tools to process count dict and to apply error mitigation
+- :py:mod:`tensorcircuit.results`: Provide tools to process count dict and to apply error mitigation.
+
+**Cloud quantum hardware access module:**
+
+- :py:mod:`tensorcircuit.cloud`: Provide quantum cloud SDK that can access and program the real quantum hardware.
+
+- :py:mod:`tensorcircuit.compiler`: Provide compiler chains to compile and transform quantum circuits.
 
 **Shortcuts and Templates for Circuit Manipulation:**
 
 - :py:mod:`tensorcircuit.templates`: provide handy shortcuts functions for expectation or circuit building patterns.
 
 **Applications:**
 
@@ -145,8 +151,33 @@
 Note how in this example, ``matrix`` is not a typical MPO but still can be expressed as ``QuOperator``. Indeed, any tensor network with two sets of dangling edges of the same dimension can be treated as ``QuOperator``. ``QuVector`` is even more flexible since we can treat all dangling edges as the vector dimension.
 
 Also, note how ``^`` is overloaded as ``tn.connect`` to connect edges between different nodes in TensorNetwork. And indexing the node gives the edges of the node, eg. ``n1[0]`` means the first edge of node ``n1``.
 
 The convention to define the ``QuOperator`` is firstly giving ``out_edges`` (left index or row index of the matrix) and then giving ``in_edges`` (right index or column index of the matrix). The edges list contains edge objects from the TensorNetwork library.
 
 Such QuOperator/QuVector abstraction support various calculations only possible on matrix/vectors, such as matmul (``@``), adjoint (``.adjoint()``), scalar multiplication (``*``), tensor product (``|``), and partial trace (``.partial_trace(subsystems_to_trace_out)``).
-To extract the matrix information of these objects, we can use ``.eval()`` or ``.eval_matrix()``, the former keeps the shape information of the tensor network while the latter gives the matrix representation with shape rank 2.
+To extract the matrix information of these objects, we can use ``.eval()`` or ``.eval_matrix()``, the former keeps the shape information of the tensor network while the latter gives the matrix representation with shape rank 2.
+
+
+Quantum Cloud SDK: Layerwise API design
+-----------------------------------------------------
+
+From lower level to higher level, a view of API layers invoking QPU calls
+
+- Vendor specific implementation of functional API in, e.g., :py:mod:`tensorcircuit.cloud.tencent`
+
+- Provider agnostic functional lower level API for task/device management in :py:mod:`tensorcircuit.cloud.apis`
+
+- Object oriented abstraction for Provider/Device/Task in :py:mod:`tensorcircuit.cloud.abstraction`
+
+- Unified batch submission interface as standarized in :py:meth:`tensorcircuit.cloud.wrapper.batch_submit_template`
+
+- Numerical and experimental unified all-in-one interface as :py:meth:`tensorcircuit.cloud.wrapper.batch_expectation_ps`
+
+- Application level code with QPU calls built directly on ``batch_expectation_ps`` or more fancy algorithms can be built on ``batch_submit_func`` so that these algorithms can be reused as long as one function ``batch_submit_func`` is defined for a given vendor (cheaper than defining a new provider from lower level).
+
+
+.. Note::
+
+    For compiler, error mitigation and results post-processing parts, they can be carefully designed to decouple with the QPU calls,
+    so they are separately implemented in :py:mod:`tensorcircuit.compiler` and :py:mod:`tensorcircuit.results`, 
+    and they can be independently useful even without tc's cloud access.
```

### Comparing `tensorcircuit-0.9.0/docs/source/modules.rst` & `tensorcircuit-0.9.1/docs/source/modules.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     ./api/about.rst
     ./api/abstractcircuit.rst
     ./api/applications.rst
     ./api/backends.rst
     ./api/basecircuit.rst
     ./api/channels.rst
     ./api/circuit.rst
+    ./api/cloud.rst
     ./api/compiler.rst
     ./api/cons.rst
     ./api/densitymatrix.rst
     ./api/experimental.rst
     ./api/gates.rst
     ./api/interfaces.rst
     ./api/keras.rst
```

### Comparing `tensorcircuit-0.9.0/docs/source/modules.rst.backup` & `tensorcircuit-0.9.1/docs/source/modules.rst.backup`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/quickstart.rst` & `tensorcircuit-0.9.1/docs/source/quickstart.rst`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 `Jax <https://github.com/google/jax#pip-installation-gpu-cuda>`_, 
 or `PyTorch <https://pytorch.org/get-started/locally/>`_.
 
 Docker is also recommended (especially Linux + Nvidia GPU setup): 
 
 ``sudo docker run -it --network host --gpus all tensorcircuit/tensorcircuit``.
 
+For more details on docker setup, please refer to `docker readme <https://github.com/tencent-quantum-lab/tensorcircuit/tree/master/docker>`_.
+
 - For Windows, due to the lack of support for Jax, we recommend to use docker or WSL, please refer to `TC via windows docker <contribs/development_windows.html>`_ or `TC via WSL <contribs/development_wsl2.html>`_.
 
 - For Mac with M series chips (arm architecture), please refer to `TC on Mac M series <contribs/development_MacARM.html>`_.
 
 Overall, the installation of TensorCircuit is simple, since it is purely in Python and hence very portable. 
 As long as the users can take care of the installation of ML frameworks on the corresponding system, TensorCircuit will work as expected.
```

### Comparing `tensorcircuit-0.9.0/docs/source/sharpbits.rst` & `tensorcircuit-0.9.1/docs/source/sharpbits.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/tutorial.rst` & `tensorcircuit-0.9.1/docs/source/tutorial.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/tutorial_cn.rst` & `tensorcircuit-0.9.1/docs/source/tutorial_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/docs/source/whitepapertoc_cn.rst` & `tensorcircuit-0.9.1/docs/source/whitepapertoc_cn.rst`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/GHZ_DQAS.py` & `tensorcircuit-0.9.1/examples/GHZ_DQAS.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/H6_hamiltonian.npy` & `tensorcircuit-0.9.1/examples/H6_hamiltonian.npy`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/QAOA_DQAS.py` & `tensorcircuit-0.9.1/examples/QAOA_DQAS.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/QEM_DQAS.py` & `tensorcircuit-0.9.1/examples/QEM_DQAS.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/adiabatic_vqnhe.py` & `tensorcircuit-0.9.1/examples/adiabatic_vqnhe.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/chaotic_behavior.py` & `tensorcircuit-0.9.1/examples/chaotic_behavior.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/checkpoint_memsave.py` & `tensorcircuit-0.9.1/examples/checkpoint_memsave.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/gradient_benchmark.py` & `tensorcircuit-0.9.1/examples/gradient_benchmark.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/hamiltonian_building.py` & `tensorcircuit-0.9.1/examples/hamiltonian_building.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/hchainhamiltonian.py` & `tensorcircuit-0.9.1/examples/hchainhamiltonian.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/incremental_twoqubit.py` & `tensorcircuit-0.9.1/examples/incremental_twoqubit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/mcnoise_boost.py` & `tensorcircuit-0.9.1/examples/mcnoise_boost.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/mcnoise_check.py` & `tensorcircuit-0.9.1/examples/mcnoise_check.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/mpsvsexact.py` & `tensorcircuit-0.9.1/examples/mpsvsexact.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/noisy_qml.py` & `tensorcircuit-0.9.1/examples/noisy_qml.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/optperformance_comparison.py` & `tensorcircuit-0.9.1/examples/optperformance_comparison.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/qaoa_block.result` & `tensorcircuit-0.9.1/examples/qaoa_block.result`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/qaoa_graph.py.outdated` & `tensorcircuit-0.9.1/examples/qaoa_graph.py.outdated`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/qaoa_micro.py.outdated` & `tensorcircuit-0.9.1/examples/qaoa_micro.py.outdated`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/qaoa_parallel_opt.py` & `tensorcircuit-0.9.1/examples/qaoa_parallel_opt.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/quantumng.py` & `tensorcircuit-0.9.1/examples/quantumng.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/simple_qaoa.py` & `tensorcircuit-0.9.1/examples/simple_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/universal_lr.py` & `tensorcircuit-0.9.1/examples/universal_lr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/variational_dynamics.py` & `tensorcircuit-0.9.1/examples/variational_dynamics.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/vqe_extra.py` & `tensorcircuit-0.9.1/examples/vqe_extra.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/vqe_extra_mpo.py` & `tensorcircuit-0.9.1/examples/vqe_extra_mpo.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/vqe_extra_mpo_spopt.py` & `tensorcircuit-0.9.1/examples/vqe_extra_mpo_spopt.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/vqeh2o_benchmark.py` & `tensorcircuit-0.9.1/examples/vqeh2o_benchmark.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/examples/vqnhe_h6.py` & `tensorcircuit-0.9.1/examples/vqnhe_h6.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/setup.py` & `tensorcircuit-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/__init__.py` & `tensorcircuit-0.9.1/tensorcircuit/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 __author__ = "TensorCircuit Authors"
 __creator__ = "refraction-ray"
 
 from .utils import gpu_memory_share
 
 gpu_memory_share()
 
@@ -34,22 +34,24 @@
 from .gates import num_to_tensor, array_to_tensor
 from .vis import qir2tex, render_pdf
 from . import interfaces
 from . import templates
 from . import results
 from . import quantum
 from .quantum import QuOperator, QuVector, QuAdjointVector, QuScalar
+from . import compiler
+from . import cloud
 
 try:
     from . import keras
-    from .keras import QuantumLayer as KerasLayer
+    from .keras import KerasLayer, KerasHardwareLayer
 except ModuleNotFoundError:
     pass  # in case tf is not installed
 
 try:
     from . import torchnn
-    from .torchnn import QuantumNet as TorchLayer
+    from .torchnn import TorchLayer, TorchHardwareLayer
 except ModuleNotFoundError:
     pass  # in case torch is not installed
 
 # just for fun
 from .asciiart import set_ascii
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/about.py` & `tensorcircuit-0.9.1/tensorcircuit/about.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/abstractcircuit.py` & `tensorcircuit-0.9.1/tensorcircuit/abstractcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/dqas.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/dqas.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/graphdata.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/graphdata.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/layers.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/layers.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/utils.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/vags.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/vags.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/van.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/van.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/applications/vqes.py` & `tensorcircuit-0.9.1/tensorcircuit/applications/vqes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 
 Tensor = Any
 Array = Any
 Model = Any
 dtype = np.complex128
 # only guarantee compatible with float64 mode
 # only support tf backend
+# i.e. use the following setup in the code
+# tc.set_backend("tensorflow")
+# tc.set_dtype("complex128")
 
 x = np.array([[0, 1.0], [1.0, 0]], dtype=dtype)
 y = np.array([[0, -1j], [1j, 0]], dtype=dtype)
 z = np.array([[1, 0], [0, -1]], dtype=dtype)
 xx = np.array([[0, 0, 0, 1], [0, 0, 1, 0], [0, 1, 0, 0], [1, 0, 0, 0]], dtype=dtype)
 yy = np.array([[0, 0, 0, -1], [0, 0, 1, 0], [0, 1, 0, 0], [-1, 0, 0, 0]], dtype=dtype)
 zz = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, -1, 0], [0, 0, 0, 1]], dtype=dtype)
@@ -372,15 +375,19 @@
     ) -> Callable[[Tensor], Tensor]:
         if choose == "hea":
             return self.create_hea_circuit(**kws)
         if choose == "hea2":
             return self.create_hea2_circuit(**kws)
         if choose == "hn":
             return self.create_hn_circuit(**kws)
-        raise ValueError("no such choose option: %s" % choose)
+        return self.create_functional_circuit(**kws)  # type: ignore
+
+    def create_functional_circuit(self, **kws: Any) -> Callable[[Tensor], Tensor]:
+        func = kws.get("func")
+        return func  # type: ignore
 
     def create_hn_circuit(self, **kws: Any) -> Callable[[Tensor], Tensor]:
         def circuit(a: Tensor) -> Tensor:
             c = Circuit(self.n)
             for i in range(self.n):
                 c.H(i)  # type: ignore
             return c
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/asciiart.py` & `tensorcircuit-0.9.1/tensorcircuit/asciiart.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/abstract_backend.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/abstract_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/backend_factory.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/backend_factory.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/cupy_backend.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/jax_backend.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/jax_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/jax_ops.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/jax_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 def jaxqr_bwd(res: Sequence[Array], tangents: Sequence[Array]) -> Tuple[Array]:
     a, q, r = res
     dq, dr = tangents
     dq = dq.conj()
     dr = dr.conj()
 
     def _TriangularSolve(x: Array, r: Array) -> Array:
-        return jax.scipy.linalg.solve_triangular(
+        return jax.scipy.linalg.solve_triangular(  # type: ignore
             r, x.T.conj(), lower=False, trans=0
         ).T.conj()
 
     def _QrGradSquareAndDeepMatrices(q: Array, r: Array, dq: Array, dr: Array) -> Array:
         # Modification begins
         rdiag = jnp.diag(r)
         rdiag = (jnp.abs(rdiag) < qr_epsilon) * qr_epsilon + (
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/numpy_backend.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_backend.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/pytorch_ops.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/pytorch_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/tensorflow_backend.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/backends/tf_ops.py` & `tensorcircuit-0.9.1/tensorcircuit/backends/tf_ops.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/basecircuit.py` & `tensorcircuit-0.9.1/tensorcircuit/basecircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/channels.py` & `tensorcircuit-0.9.1/tensorcircuit/channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/circuit.py` & `tensorcircuit-0.9.1/tensorcircuit/circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cloud/abstraction.py` & `tensorcircuit-0.9.1/tensorcircuit/cloud/abstraction.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cloud/apis.py` & `tensorcircuit-0.9.1/tensorcircuit/cloud/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 default_provider = Provider.from_name("tencent")
 avail_providers = ["tencent", "local"]
 
 
 def list_providers() -> List[Provider]:
     """
-    list all providers that tensorcircuit supports
+    list all cloud providers that tensorcircuit supports
 
     :return: _description_
     :rtype: List[Provider]
     """
     return [get_provider(s) for s in avail_providers]
 
 
@@ -81,15 +81,15 @@
 
 def set_device(
     provider: Optional[Union[str, Provider]] = None,
     device: Optional[Union[str, Device]] = None,
     set_global: bool = True,
 ) -> Device:
     """
-    _summary_
+    set the default device
 
     :param provider: provider of the device, defaults to None
     :type provider: Optional[Union[str, Provider]], optional
     :param device: the device, defaults to None
     :type device: Optional[Union[str, Device]], optional
     :param set_global: whether set, defaults to True,
         if False, equivalent to ``get_device``, defaults to True
@@ -201,18 +201,22 @@
     homedir = os.path.expanduser("~")
     authpath = os.path.join(homedir, ".tc.auth.json")
     # provider, device = _preprocess(provider, device)
     if clear is True:
         saved_token = {}
     if token is None:
         if cached and os.path.exists(authpath):
-            with open(authpath, "r") as f:
-                file_token = json.load(f)
-                file_token = {k: b64decode_s(v) for k, v in file_token.items()}
-                # file_token = backend.tree_map(b64decode_s, file_token)
+            try:
+                with open(authpath, "r") as f:
+                    file_token = json.load(f)
+                    file_token = {k: b64decode_s(v) for k, v in file_token.items()}
+                    # file_token = backend.tree_map(b64decode_s, file_token)
+            except json.JSONDecodeError:
+                logger.warning("token file loading failure, set empty token instead")
+                file_token = {}
         else:
             file_token = {}
         file_token.update(saved_token)
         saved_token = file_token
     else:  # with token
         if isinstance(provider, str):
             provider = Provider.from_name(provider)
@@ -409,14 +413,18 @@
     device: Optional[Union[str, Device]] = None,
     token: Optional[str] = None,
     **task_kws: Any,
 ) -> List[Task]:
     """
     submit task to the cloud platform, batch submission default enabled
 
+    .. seealso::
+
+        :py:meth:`tensorcircuit.cloud.tencent.submit_task`
+
     :param provider: _description_, defaults to None
     :type provider: Optional[Union[str, Provider]], optional
     :param device: _description_, defaults to None
     :type device: Optional[Union[str, Device]], optional
     :param token: _description_, defaults to None
     :type token: Optional[str], optional
     :param task_kws: all necessary keywords arguments for task submission,
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cloud/local.py` & `tensorcircuit-0.9.1/tensorcircuit/cloud/local.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cloud/quafu_provider.py` & `tensorcircuit-0.9.1/tensorcircuit/cloud/quafu_provider.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cloud/tencent.py` & `tensorcircuit-0.9.1/tensorcircuit/cloud/tencent.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,15 +284,15 @@
             if "err" in t:
                 logger.warning(t["err"])
             else:
                 logger.warning("unsuccessful submission of the task:\n" + dumps(r))
         else:
             ti = Task(id_=t["id"], device=device)
             rtn.append(ti)
-    if len(rtn) == 1:
+    if not is_sequence(source):
         return rtn[0]  # type: ignore
     elif len(rtn) == 0:
         raise ValueError("All tasks submitted failed")
     else:
         return rtn
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cloud/utils.py` & `tensorcircuit-0.9.1/tensorcircuit/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/compiler/composed_compiler.py` & `tensorcircuit-0.9.1/tensorcircuit/compiler/composed_compiler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """
 object oriented compiler pipeline
 """
 
-from typing import Any, Callable, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from ..utils import is_sequence
 from ..abstractcircuit import AbstractCircuit
 from .qiskit_compiler import qiskit_compile
+from .simple_compiler import simple_compile
 
 
 class Compiler:
     def __init__(
         self,
         compile_funcs: Union[Callable[..., Any], List[Callable[..., Any]]],
         compiled_options: Optional[List[Dict[str, Any]]] = None,
@@ -20,24 +21,64 @@
         else:
             self.compile_funcs = list(compile_funcs)  # type: ignore
         self.add_options(compiled_options)
 
     def add_options(
         self, compiled_options: Optional[List[Dict[str, Any]]] = None
     ) -> None:
-        if not is_sequence(compiled_options):
-            self.compiled_options = [compiled_options for _ in self.compile_funcs]
+        if compiled_options is None:
+            self.compiled_options = [{} for _ in range(len(self.compile_funcs))]  # type: ignore
+        elif not is_sequence(compiled_options):
+            self.compiled_options = [compiled_options for _ in self.compile_funcs]  # type: ignore
         else:
             assert len(compiled_options) == len(  # type: ignore
                 self.compile_funcs
             ), "`compiled_options` must have the same list length as `compile_funcs`"
             self.compiled_options = list(compiled_options)  # type: ignore
+            for i, c in enumerate(self.compiled_options):
+                if c is None:
+                    self.compiled_options[i] = {}
 
     def __call__(
         self, circuit: AbstractCircuit, info: Optional[Dict[str, Any]] = None
     ) -> Any:
         for f, d in zip(self.compile_funcs, self.compiled_options):
-            circuit, info = f(circuit, info, compiled_options=d)  # type: ignore
+            result = f(circuit, info, compiled_options=d)  # type: ignore
+            if not isinstance(result, tuple):
+                result = (result, info)
+            circuit, info = result
         return circuit, info
 
 
-default_compiler = Compiler(qiskit_compile)
+class DefaultCompiler(Compiler):
+    def __init__(self, qiskit_compiled_options: Optional[Dict[str, Any]] = None):
+        """
+        A fallback choice to compile circuit running on tencent quantum cloud with rz as native gate
+
+        :param qiskit_compiled_options: qiskit compiled options to be added
+            options documented in `qiskit.transpile` method,
+            to use tencent quantum cloud, `{"coupling_map": d.topology()}` is in general enough,
+            where d is a device object,
+            defaults to None, i.e. no qubit mapping is applied
+        :type qiskit_compiled_options: Optional[Dict[str, Any]], optional
+        """
+        compiled_options = {
+            "optimization_level": 3,
+            "basis_gates": ["u3", "h", "cx", "cz"],
+        }
+        # rz target is bad for qiskit
+        if qiskit_compiled_options:
+            compiled_options.update(qiskit_compiled_options)
+        super().__init__(
+            [qiskit_compile, simple_compile],
+            [compiled_options, None],  # type: ignore
+        )
+
+
+def default_compile(
+    circuit: AbstractCircuit,
+    info: Optional[Dict[str, Any]] = None,
+    compiled_options: Optional[Dict[str, Any]] = None,
+) -> Tuple[AbstractCircuit, Dict[str, Any]]:
+    dc = DefaultCompiler(compiled_options)
+    c, info = dc(circuit, info)
+    return c, info  # type: ignore
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/compiler/qiskit_compiler.py` & `tensorcircuit-0.9.1/tensorcircuit/compiler/qiskit_compiler.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,18 @@
     for r in s.split("\n"):
         inc = re.search(r"\(.*\)", r)
         if inc is None:
             rs.append(r)
         else:
             v = r[inc.start() : inc.end()]
             v = eval(v)
-            r = r[: inc.start()] + "(" + str(v) + ")" + r[inc.end() :]
+            if not isinstance(v, tuple):
+                r = r[: inc.start()] + "(" + str(v) + ")" + r[inc.end() :]
+            else:  # u gate case
+                r = r[: inc.start()] + str(v) + r[inc.end() :]
             rs.append(r)
     return "\n".join(rs)
 
 
 def _comment_qasm(s: str) -> str:
     """
     return the qasm str in comment format
@@ -116,27 +119,41 @@
 
 def qiskit_compile(
     circuit: Any,
     info: Optional[Dict[str, Any]] = None,
     output: str = "tc",
     compiled_options: Optional[Dict[str, Any]] = None,
 ) -> Any:
+    """
+    compile the circuit using ``qiskit.transpile`` method with some tricks and hacks
+
+    :param circuit: circuit in ``tc.Circuit`` or ``qiskit.QuantumCircuit`` form
+    :type circuit: Any
+    :param info: info for qubit mappings, defaults to None
+    :type info: Optional[Dict[str, Any]], optional
+    :param output: output circuit format, defaults to "tc"
+    :type output: str, optional
+    :param compiled_options: ``qiskit.transpile`` options in a dict, defaults to None
+    :type compiled_options: Optional[Dict[str, Any]], optional
+    :return: Tuple containing the output circuit and the qubit mapping info dict
+    :rtype: Any
+    """
     from qiskit.compiler import transpile
     from qiskit.transpiler.passes import RemoveBarriers
 
     if isinstance(circuit, AbstractCircuit):
         circuit = circuit.to_qiskit(enable_instruction=True)
     elif isinstance(circuit, str):
         circuit = qiskit_from_qasm_str_ordered_measure(circuit)
     # else qiskit circuit
     circuit = _add_measure_all_if_none(circuit)
     if compiled_options is None:
         compiled_options = {
             "basis_gates": ["h", "rz", "cx"],
-            "optimization_level": 2,
+            "optimization_level": 2,  # 3 can induce bugs...
         }
     ncircuit = transpile(circuit, **compiled_options)
     ncircuit = RemoveBarriers()(ncircuit)
 
     if output.lower() in ["qasm", "openqasm"]:
         r0 = ncircuit.qasm()
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/cons.py` & `tensorcircuit-0.9.1/tensorcircuit/cons.py`

 * *Files 1% similar despite different names*

```diff
@@ -754,14 +754,40 @@
     :return: The new tensornetwork with its contractor set.
     :rtype: tn.Node
     """
     if not method:
         method = "greedy"
         # auto for small size fallbacks to dp, which has bug for now
         # see: https://github.com/dgasmith/opt_einsum/issues/172
+    if method.startswith("cotengra"):
+        # cotengra shortcut
+        import cotengra
+
+        if method == "cotengra":
+            method = "custom"
+            optimizer = cotengra.ReusableHyperOptimizer(
+                methods=["greedy", "kahypar"],
+                parallel=True,
+                minimize="combo",
+                max_time=30,
+                max_repeats=64,
+                progbar=True,
+            )
+        else:  # "cotengra-30-64"
+            _, mt, mr = method.split("-")
+            method = "custom"
+            optimizer = cotengra.ReusableHyperOptimizer(
+                methods=["greedy", "kahypar"],
+                parallel=True,
+                minimize="combo",
+                max_time=int(mt),
+                max_repeats=int(mr),
+                progbar=True,
+            )
+
     if method == "plain":
         cf = plain_contractor
     elif method == "plain-experimental":
         cf = partial(experimental_contractor, local_steps=kws.get("local_steps", 2))
     elif method == "tng":  # don't use, deprecated, no guarantee
         if has_ps:
             cf = tn_greedy_contractor
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/densitymatrix.py` & `tensorcircuit-0.9.1/tensorcircuit/densitymatrix.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/experimental.py` & `tensorcircuit-0.9.1/tensorcircuit/experimental.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/gates.py` & `tensorcircuit-0.9.1/tensorcircuit/gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/interfaces/numpy.py` & `tensorcircuit-0.9.1/tensorcircuit/interfaces/numpy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/interfaces/scipy.py` & `tensorcircuit-0.9.1/tensorcircuit/interfaces/scipy.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/interfaces/tensorflow.py` & `tensorcircuit-0.9.1/tensorcircuit/interfaces/tensorflow.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/interfaces/tensortrans.py` & `tensorcircuit-0.9.1/tensorcircuit/interfaces/tensortrans.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/interfaces/torch.py` & `tensorcircuit-0.9.1/tensorcircuit/interfaces/torch.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/keras.py` & `tensorcircuit-0.9.1/tensorcircuit/keras.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,19 @@
     #     return dict(list(base_config.items()) + list(config.items()))
 
 
 KerasLayer = QuantumLayer
 
 
 class HardwareLayer(QuantumLayer):
+    """
+    Keras Layer wrapping quantum function with cloud qpu access
+    (using :py:mod:`tensorcircuit.cloud` module)
+    """
+
     @tf.autograph.experimental.do_not_convert  # type: ignore
     def call(
         self,
         inputs: tf.Tensor,
         training: Optional[bool] = None,
         mask: Optional[tf.Tensor] = None,
         **kwargs: Any
@@ -166,14 +171,17 @@
             result = []
             for inp in inputs:
                 result.append(self.f(inp, *self.pqc_weights, **kwargs))
             result = tf.stack(result)
         return result
 
 
+KerasHardwareLayer = HardwareLayer
+
+
 def output_asis_loss(y_true: tf.Tensor, y_pred: tf.Tensor) -> tf.Tensor:
     """
     The keras loss function that directly taking the model output as the loss.
 
     :param y_true: Ignoring this parameter.
     :type y_true: tf.Tensor
     :param y_pred: Model output.
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/mps_base.py` & `tensorcircuit-0.9.1/tensorcircuit/mps_base.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/mpscircuit.py` & `tensorcircuit-0.9.1/tensorcircuit/mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/noisemodel.py` & `tensorcircuit-0.9.1/tensorcircuit/noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/quantum.py` & `tensorcircuit-0.9.1/tensorcircuit/quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/results/counts.py` & `tensorcircuit-0.9.1/tensorcircuit/results/counts.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/results/readout_mitigation.py` & `tensorcircuit-0.9.1/tensorcircuit/results/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/simplify.py` & `tensorcircuit-0.9.1/tensorcircuit/simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/templates/blocks.py` & `tensorcircuit-0.9.1/tensorcircuit/templates/blocks.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/templates/chems.py` & `tensorcircuit-0.9.1/tensorcircuit/templates/chems.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/templates/dataset.py` & `tensorcircuit-0.9.1/tensorcircuit/templates/dataset.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/templates/ensemble.py` & `tensorcircuit-0.9.1/tensorcircuit/templates/ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/templates/graphs.py` & `tensorcircuit-0.9.1/tensorcircuit/templates/graphs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/templates/measurements.py` & `tensorcircuit-0.9.1/tensorcircuit/templates/measurements.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/torchnn.py` & `tensorcircuit-0.9.1/tensorcircuit/torchnn.py`

 * *Files 23% similar despite different names*

```diff
@@ -93,7 +93,46 @@
 
     def forward(self, *inputs: Tensor) -> Tensor:
         ypred = self.f(*inputs, *self.q_weights)
         return ypred
 
 
 TorchLayer = QuantumNet
+
+
+class HardwareNet(QuantumNet):
+    """
+    PyTorch Layer wrapping quantum function with cloud qpu access
+    (using :py:mod:`tensorcircuit.cloud` module)
+    """
+
+    def __init__(
+        self,
+        f: Callable[..., Any],
+        weights_shape: Sequence[Tuple[int, ...]],
+        initializer: Union[Any, Sequence[Any]] = None,
+        use_vmap: bool = True,
+    ):
+        super().__init__(
+            f,
+            weights_shape,
+            initializer,
+            use_vmap=False,
+            use_interface=False,
+            use_jit=False,
+        )
+        self.batch_support = use_vmap
+
+    def forward(self, *inputs: Tensor) -> Tensor:
+        if self.batch_support:
+            ypred = []
+            batch = inputs[0].shape[0]
+            for i in range(batch):
+                inp = tuple([a[i] for a in inputs])
+                ypred.append(self.f(*inp, *self.q_weights))
+            ypred = torch.stack(ypred)  # type: ignore
+        else:
+            ypred = self.f(*inputs, *self.q_weights)
+        return ypred
+
+
+TorchHardwareLayer = HardwareNet
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit/translation.py` & `tensorcircuit-0.9.1/tensorcircuit/translation.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/utils.py` & `tensorcircuit-0.9.1/tensorcircuit/utils.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit/vis.py` & `tensorcircuit-0.9.1/tensorcircuit/vis.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tensorcircuit.egg-info/PKG-INFO` & `tensorcircuit-0.9.1/tensorcircuit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorcircuit
-Version: 0.9.0
+Version: 0.9.1
 Summary: Quantum circuits on top of tensor network
 Home-page: https://github.com/tencent-quantum-lab/tensorcircuit
 Author: TensorCircuit Authors
 Author-email: shixinzhang@tencent.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -44,17 +44,17 @@
   <a href="./LICENSE">
     <img src="https://img.shields.io/badge/license-Apache%202.0-blue.svg?logo=apache"/>
   </a>
 </p>
 
 <p align="center"> English | <a href="README_cn.md"> 简体中文 </a></p>
 
-TensorCircuit is the next generation of quantum circuit simulators with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
+TensorCircuit is the next generation of quantum software framework with support for automatic differentiation, just-in-time compiling, hardware acceleration, and vectorized parallelism.
 
-TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms.
+TensorCircuit is built on top of modern machine learning frameworks and is machine learning backend agnostic. It is specifically suitable for highly efficient simulations of quantum-classical hybrid paradigm and variational quantum algorithms. It also supports real quantum hardware access and provides CPU/GPU/QPU hybrid deployment solutions since v0.9.
 
 ## Getting Started
 
 Please begin with [Quick Start](/docs/source/quickstart.rst).
 
 For more information and introductions, please refer to helpful [example scripts](/examples) and [full documentation](https://tensorcircuit.readthedocs.io/). API docstrings and test cases in [tests](/tests) are also informative.
 
@@ -105,30 +105,32 @@
 
 We recommend you install this package with tensorflow also installed as:
 
 ```python
 pip install tensorcircuit[tensorflow]
 ```
 
-Other optional dependencies include `[torch]`, `[jax]` and `[qiskit]`.
+Other optional dependencies include `[torch]`, `[jax]`, `[qiskit]` and `[cloud]`.
 
 For the nightly build of tensorcircuit with new features, try:
 
 ```python
 pip uninstall tensorcircuit
 pip install tensorcircuit-nightly
 ```
 
 We also have [Docker support](/docker).
 
 ## Advantages
 
 - Tensor network simulation engine based
 
-- JIT, AD, vectorized parallelism compatible, GPU support
+- JIT, AD, vectorized parallelism compatible
+
+- GPU support, quantum device access support, hybrid deployment support
 
 - Efficiency
 
   - Time: 10 to 10^6+ times acceleration compared to TensorFlow Quantum, Pennylane or Qiskit
 
   - Space: 600+ qubits 1D VQE workflow (converged energy inaccuracy: < 1%)
 
@@ -154,14 +156,18 @@
 
 ### Guidelines
 
 For contribution guidelines and notes, see [CONTRIBUTING](/CONTRIBUTING.md).
 
 We welcome [issues](https://github.com/tencent-quantum-lab/tensorcircuit/issues), [PRs](https://github.com/tencent-quantum-lab/tensorcircuit/pulls), and [discussions](https://github.com/tencent-quantum-lab/tensorcircuit/discussions) from everyone, and these are all hosted on GitHub.
 
+### License
+
+TensorCircuit is open source, released under the Apache License, Version 2.0.
+
 ### Contributors
 
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
 <!-- prettier-ignore-start -->
 <!-- markdownlint-disable -->
 <table>
   <tbody>
@@ -209,25 +215,41 @@
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 ## Research and Applications
 
 ### DQAS
 
 For the application of Differentiable Quantum Architecture Search, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2010.08561.pdf (published in QST).
+
+Reference paper: https://arxiv.org/abs/2010.08561 (published in QST).
 
 ### VQNHE
 
 For the application of Variational Quantum-Neural Hybrid Eigensolver, see [applications](/tensorcircuit/applications).
-Reference paper: https://arxiv.org/pdf/2106.05105.pdf (published in PRL) and https://arxiv.org/pdf/2112.10380.pdf.
 
-### VQEX - MBL
+Reference paper: https://arxiv.org/abs/2106.05105 (published in PRL) and https://arxiv.org/abs/2112.10380.
+
+### VQEX-MBL
 
 For the application of VQEX on MBL phase identification, see the [tutorial](/docs/source/tutorials/vqex_mbl.ipynb).
-Reference paper: https://arxiv.org/pdf/2111.13719.pdf (published in PRB).
 
-### Stark - DTC
+Reference paper: https://arxiv.org/abs/2111.13719 (published in PRB).
+
+### Stark-DTC
 
 For the numerical demosntration of discrete time crystal enabled by Stark many-body localization, see the Floquet simulation [demo](/examples/timeevolution_trotter.py).
-Reference paper: https://arxiv.org/pdf/2208.02866.pdf (published in PRL).
+
+Reference paper: https://arxiv.org/abs/2208.02866 (published in PRL).
+
+### EMQAOA-DARBO
+
+For the numerical simulation and hardware experiments with error mitigation on QAOA, see the [project repo](https://github.com/sherrylixuecheng/EMQAOA-DARBO).
+
+Reference paper: https://arxiv.org/abs/2303.14877.
+
+### TenCirChem
+
+[TenCirChem](https://github.com/tencent-quantum-lab/TenCirChem) is an efficient and versatile quantum computation package for molecular properties. TenCirChem is based on TensorCircuit and is optimized for chemistry applications.
+
+Reference paper: https://arxiv.org/abs/2303.10825.
```

### Comparing `tensorcircuit-0.9.0/tensorcircuit.egg-info/SOURCES.txt` & `tensorcircuit-0.9.1/tensorcircuit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
 tensorcircuit/cloud/quafu_provider.py
 tensorcircuit/cloud/tencent.py
 tensorcircuit/cloud/utils.py
 tensorcircuit/cloud/wrapper.py
 tensorcircuit/compiler/__init__.py
 tensorcircuit/compiler/composed_compiler.py
 tensorcircuit/compiler/qiskit_compiler.py
+tensorcircuit/compiler/simple_compiler.py
 tensorcircuit/interfaces/__init__.py
 tensorcircuit/interfaces/numpy.py
 tensorcircuit/interfaces/scipy.py
 tensorcircuit/interfaces/tensorflow.py
 tensorcircuit/interfaces/tensortrans.py
 tensorcircuit/interfaces/torch.py
 tensorcircuit/results/__init__.py
```

### Comparing `tensorcircuit-0.9.0/tests/conftest.py` & `tensorcircuit-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_backends.py` & `tensorcircuit-0.9.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_calibrating.py` & `tensorcircuit-0.9.1/tests/test_calibrating.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_channels.py` & `tensorcircuit-0.9.1/tests/test_channels.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_circuit.py` & `tensorcircuit-0.9.1/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_compiler.py` & `tensorcircuit-0.9.1/tests/test_compiler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import os
 import pytest
+import numpy as np
 
 # from pytest_lazyfixture import lazy_fixture as lf
 
 
 thisfile = os.path.abspath(__file__)
 modulepath = os.path.dirname(os.path.dirname(thisfile))
 
@@ -69,31 +70,78 @@
         },
     )
     assert info2["positional_logical_mapping"] == {0: 1}
     print(c2.draw())
 
 
 def test_composed_compiler():
-    from tensorcircuit.compiler import default_compiler
+    from tensorcircuit.compiler import DefaultCompiler
 
     c = tc.Circuit(3)
     c.rx(0)
     c.cx(0, 1)
     c.cz(1, 0)
     c.rxx(0, 2, theta=0.2)
     c.measure_instruction(2)
     c.measure_instruction(0)
+    default_compiler = DefaultCompiler()
     c1, info = default_compiler(c)
     print(c1.draw())
-    assert c1.gate_count_by_condition(lambda qir: qir["name"] == "cnot") == 4
+    assert c1.gate_count_by_condition(lambda qir: qir["name"] == "cnot") == 3
     assert info["positional_logical_mapping"][0] == 2
 
-    default_compiler.add_options(
+    default_compiler = DefaultCompiler(
         {
             "basis_gates": ["h", "rz", "cz"],
             "optimization_level": 2,
             "coupling_map": [[0, 1], [1, 2]],
         }
     )
+
     c1, info = default_compiler(c)
     assert c1.gate_count_by_condition(lambda qir: qir["name"] == "cnot") == 0
     print(info)
+
+
+def test_replace_r():
+    c = tc.Circuit(3)
+    c.rz(0, theta=0.1)
+    c.cx(0, 2)
+    c.ry(1)
+    c.rxx(1, 0, theta=0.2)
+    c.rx(0, theta=3.9)
+    c.ry(1, theta=-0.2)
+    c.rzz(1, 0, theta=-0.3)
+    c.ryy(1, 0, theta=-0.6)
+    c.rx(2)
+
+    print(c.draw())
+    c1 = tc.compiler.simple_compiler.replace_r(c)
+    print(c1.draw())
+    np.testing.assert_allclose(c.matrix(), c1.matrix(), atol=1e-5)
+
+
+def test_default_compiler():
+    c = tc.Circuit(3)
+    c.cx(0, 1)
+    c.rx(0, theta=1e-5)
+    c.x(1)
+    c.y(1)
+    c.z(1)
+    c.h(1)
+    c.cz(2, 0)
+    c.h(1)
+    c.cz(2, 0)
+    c.s(2)
+    c.sd(2)
+    c.s(2)
+    c.s(2)
+    c.y(2)
+    c.ry(2, theta=0.1)
+    c.t(2)
+    c.td(2)
+    c.ry(2, theta=-0.1)
+    c.rz(1, theta=0.3)
+
+    c1, _ = tc.compiler.simple_compiler.simple_compile(c)
+    print(c1.draw())
+    assert c1.gate_count() == 3
```

### Comparing `tensorcircuit-0.9.0/tests/test_dmcircuit.py` & `tensorcircuit-0.9.1/tests/test_dmcircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_ensemble.py` & `tensorcircuit-0.9.1/tests/test_ensemble.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_gates.py` & `tensorcircuit-0.9.1/tests/test_gates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_interfaces.py` & `tensorcircuit-0.9.1/tests/test_interfaces.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_keras.py` & `tensorcircuit-0.9.1/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_miscs.py` & `tensorcircuit-0.9.1/tests/test_miscs.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_mpscircuit.py` & `tensorcircuit-0.9.1/tests/test_mpscircuit.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_noisemodel.py` & `tensorcircuit-0.9.1/tests/test_noisemodel.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_qaoa.py` & `tensorcircuit-0.9.1/tests/test_qaoa.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_quantum.py` & `tensorcircuit-0.9.1/tests/test_quantum.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_quantum_attr.py` & `tensorcircuit-0.9.1/tests/test_quantum_attr.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_results.py` & `tensorcircuit-0.9.1/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_simplify.py` & `tensorcircuit-0.9.1/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_templates.py` & `tensorcircuit-0.9.1/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `tensorcircuit-0.9.0/tests/test_torchnn.py` & `tensorcircuit-0.9.1/tests/test_torchnn.py`

 * *Files 24% similar despite different names*

```diff
@@ -70,7 +70,30 @@
     noise = 0.2 * torchb.ones([2, n], dtype="float32")
     l = layer(state, noise)
     lsum = torchb.sum(l)
     print(l)
     lsum.backward()
     for p in layer.parameters():
         print(p.grad)
+
+
+@pytest.mark.parametrize("backend", [lf("tfb"), lf("jaxb"), lf("torchb")])
+def test_torchnn_hardware(backend):
+    n = 2
+
+    def qf(inputs, param):
+        inputs = tc.backend.convert_to_tensor(tc.get_backend("pytorch").numpy(inputs))
+        param = tc.backend.convert_to_tensor(tc.get_backend("pytorch").numpy(param))
+
+        c = tc.Circuit(n)
+        c.rx(0, theta=inputs[0])
+        c.rx(1, theta=inputs[1])
+        c.h(1)
+        c.rzz(0, 1, theta=param[0])
+        r = tc.backend.stack([c.expectation_ps(z=[i]) for i in range(n)])
+
+        r = tc.get_backend("pytorch").convert_to_tensor(tc.backend.numpy(r))
+        return torch.real(r)
+
+    ql = tc.torchnn.HardwareNet(qf, [1])
+    qnet = torch.nn.Sequential(ql, torch.nn.Linear(2, 1))
+    print(qnet(torch.ones([5, 2])))
```

### Comparing `tensorcircuit-0.9.0/tests/test_van.py` & `tensorcircuit-0.9.1/tests/test_van.py`

 * *Files identical despite different names*

