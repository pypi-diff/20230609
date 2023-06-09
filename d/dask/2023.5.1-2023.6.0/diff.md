# Comparing `tmp/dask-2023.5.1.tar.gz` & `tmp/dask-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-2023.5.1.tar", last modified: Fri May 26 20:09:35 2023, max compression
+gzip compressed data, was "dask-2023.6.0.tar", last modified: Fri Jun  9 16:34:13 2023, max compression
```

## Comparing `dask-2023.5.1.tar` & `dask-2023.6.0.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.479508 dask-2023.5.1/
--rw-r--r--   0 james      (501) staff       (20)     1531 2022-10-24 20:44:15.000000 dask-2023.5.1/LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)      325 2022-11-09 22:20:24.000000 dask-2023.5.1/MANIFEST.in
--rw-r--r--   0 james      (501) staff       (20)     2532 2023-05-26 20:09:35.478474 dask-2023.5.1/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1291 2022-11-09 22:20:24.000000 dask-2023.5.1/README.rst
--rw-r--r--   0 james      (501) staff       (20)     2397 2023-05-24 20:58:41.000000 dask-2023.5.1/conftest.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.480087 dask-2023.5.1/dask/
--rw-r--r--   0 james      (501) staff       (20)      464 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      133 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/__main__.py
--rw-r--r--   0 james      (501) staff       (20)      643 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/_compatibility.py
--rw-r--r--   0 james      (501) staff       (20)      500 2023-05-26 20:09:35.480178 dask-2023.5.1/dask/_version.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.814626 dask-2023.5.1/dask/array/
--rw-r--r--   0 james      (501) staff       (20)     1543 2021-06-08 02:50:30.000000 dask-2023.5.1/dask/array/NUMPY_LICENSE.txt
--rw-r--r--   0 james      (501) staff       (20)     5413 2023-05-24 21:26:44.000000 dask-2023.5.1/dask/array/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12600 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/backends.py
--rw-r--r--   0 james      (501) staff       (20)     9983 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/blockwise.py
--rw-r--r--   0 james      (501) staff       (20)    12304 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/chunk.py
--rw-r--r--   0 james      (501) staff       (20)     5066 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/chunk_types.py
--rw-r--r--   0 james      (501) staff       (20)   190916 2023-05-19 15:53:47.000000 dask-2023.5.1/dask/array/core.py
--rw-r--r--   0 james      (501) staff       (20)    40564 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/array/creation.py
--rw-r--r--   0 james      (501) staff       (20)     2114 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/cupy_entry_point.py
--rw-r--r--   0 james      (501) staff       (20)      526 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     9189 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/einsumfuncs.py
--rw-r--r--   0 james      (501) staff       (20)     7252 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/fft.py
--rw-r--r--   0 james      (501) staff       (20)    32656 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/gufunc.py
--rw-r--r--   0 james      (501) staff       (20)     1996 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/image.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.815913 dask-2023.5.1/dask/array/lib/
--rw-r--r--   0 james      (501) staff       (20)       77 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/lib/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      101 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/lib/stride_tricks.py
--rw-r--r--   0 james      (501) staff       (20)    53335 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/linalg.py
--rw-r--r--   0 james      (501) staff       (20)     6363 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/ma.py
--rw-r--r--   0 james      (501) staff       (20)     5699 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/numpy_compat.py
--rw-r--r--   0 james      (501) staff       (20)    12838 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/optimization.py
--rw-r--r--   0 james      (501) staff       (20)    28480 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/overlap.py
--rw-r--r--   0 james      (501) staff       (20)    10652 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/percentile.py
--rw-r--r--   0 james      (501) staff       (20)    40604 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/random.py
--rw-r--r--   0 james      (501) staff       (20)    28023 2023-05-24 22:18:59.000000 dask-2023.5.1/dask/array/rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    57287 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/reductions.py
--rw-r--r--   0 james      (501) staff       (20)    10765 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/reshape.py
--rw-r--r--   0 james      (501) staff       (20)    81988 2023-05-19 15:53:47.000000 dask-2023.5.1/dask/array/routines.py
--rw-r--r--   0 james      (501) staff       (20)    72631 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/slicing.py
--rw-r--r--   0 james      (501) staff       (20)    14613 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/stats.py
--rw-r--r--   0 james      (501) staff       (20)     8048 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/svg.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.882922 dask-2023.5.1/dask/array/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.5.1/dask/array/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)   161461 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_array_core.py
--rw-r--r--   0 james      (501) staff       (20)     6689 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_array_function.py
--rw-r--r--   0 james      (501) staff       (20)     3159 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_array_utils.py
--rw-r--r--   0 james      (501) staff       (20)    23222 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_atop.py
--rw-r--r--   0 james      (501) staff       (20)     3304 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_chunk.py
--rw-r--r--   0 james      (501) staff       (20)    31150 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_creation.py
--rw-r--r--   0 james      (501) staff       (20)    19888 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_core.py
--rw-r--r--   0 james      (501) staff       (20)     6456 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_creation.py
--rw-r--r--   0 james      (501) staff       (20)      594 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_gufunc.py
--rw-r--r--   0 james      (501) staff       (20)    13412 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_linalg.py
--rw-r--r--   0 james      (501) staff       (20)     4303 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_overlap.py
--rw-r--r--   0 james      (501) staff       (20)     2862 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_percentile.py
--rw-r--r--   0 james      (501) staff       (20)     9219 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_random.py
--rw-r--r--   0 james      (501) staff       (20)     2224 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_reductions.py
--rw-r--r--   0 james      (501) staff       (20)     7437 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_routines.py
--rw-r--r--   0 james      (501) staff       (20)     4877 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_slicing.py
--rw-r--r--   0 james      (501) staff       (20)     2982 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_cupy_sparse.py
--rw-r--r--   0 james      (501) staff       (20)     8865 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_dispatch.py
--rw-r--r--   0 james      (501) staff       (20)     8437 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_fft.py
--rw-r--r--   0 james      (501) staff       (20)    21013 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_gufunc.py
--rw-r--r--   0 james      (501) staff       (20)     1482 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_image.py
--rw-r--r--   0 james      (501) staff       (20)    36448 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_linalg.py
--rw-r--r--   0 james      (501) staff       (20)    15635 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_masked.py
--rw-r--r--   0 james      (501) staff       (20)     1087 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_numpy_compat.py
--rw-r--r--   0 james      (501) staff       (20)    17446 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_optimization.py
--rw-r--r--   0 james      (501) staff       (20)    26718 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_overlap.py
--rw-r--r--   0 james      (501) staff       (20)     3443 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_percentiles.py
--rw-r--r--   0 james      (501) staff       (20)    15353 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_random.py
--rw-r--r--   0 james      (501) staff       (20)    36341 2023-05-24 21:57:25.000000 dask-2023.5.1/dask/array/tests/test_rechunk.py
--rw-r--r--   0 james      (501) staff       (20)    32756 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_reductions.py
--rw-r--r--   0 james      (501) staff       (20)     7289 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_reshape.py
--rw-r--r--   0 james      (501) staff       (20)    83849 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_routines.py
--rw-r--r--   0 james      (501) staff       (20)    32302 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_slicing.py
--rw-r--r--   0 james      (501) staff       (20)     6592 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_sparse.py
--rw-r--r--   0 james      (501) staff       (20)     5489 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_stats.py
--rw-r--r--   0 james      (501) staff       (20)     2740 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_svg.py
--rw-r--r--   0 james      (501) staff       (20)      525 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_testing.py
--rw-r--r--   0 james      (501) staff       (20)    17390 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_ufunc.py
--rw-r--r--   0 james      (501) staff       (20)     2706 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_wrap.py
--rw-r--r--   0 james      (501) staff       (20)     1317 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tests/test_xarray.py
--rw-r--r--   0 james      (501) staff       (20)     4737 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/tiledb_io.py
--rw-r--r--   0 james      (501) staff       (20)     9943 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/ufunc.py
--rw-r--r--   0 james      (501) staff       (20)    18674 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/utils.py
--rw-r--r--   0 james      (501) staff       (20)     6906 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/array/wrap.py
--rw-r--r--   0 james      (501) staff       (20)     4936 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/backends.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.888761 dask-2023.5.1/dask/bag/
--rw-r--r--   0 james      (501) staff       (20)      903 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     9111 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/avro.py
--rw-r--r--   0 james      (501) staff       (20)      763 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/chunk.py
--rw-r--r--   0 james      (501) staff       (20)    84784 2023-05-24 15:39:04.000000 dask-2023.5.1/dask/bag/core.py
--rw-r--r--   0 james      (501) staff       (20)     5464 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/random.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.892166 dask-2023.5.1/dask/bag/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.5.1/dask/bag/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     3808 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/tests/test_avro.py
--rw-r--r--   0 james      (501) staff       (20)    50747 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/tests/test_bag.py
--rw-r--r--   0 james      (501) staff       (20)     6528 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/tests/test_random.py
--rw-r--r--   0 james      (501) staff       (20)     5049 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/tests/test_text.py
--rw-r--r--   0 james      (501) staff       (20)     6765 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/text.py
--rw-r--r--   0 james      (501) staff       (20)      241 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bag/utils.py
--rw-r--r--   0 james      (501) staff       (20)    52086 2023-05-26 16:18:40.000000 dask-2023.5.1/dask/base.py
--rw-r--r--   0 james      (501) staff       (20)    53252 2023-05-19 15:53:47.000000 dask-2023.5.1/dask/blockwise.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.894508 dask-2023.5.1/dask/bytes/
--rw-r--r--   0 james      (501) staff       (20)       75 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6933 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/core.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.900449 dask-2023.5.1/dask/bytes/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.5.1/dask/bytes/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     5158 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/tests/test_bytes_utils.py
--rw-r--r--   0 james      (501) staff       (20)      530 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/tests/test_compression.py
--rw-r--r--   0 james      (501) staff       (20)     6657 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/bytes/tests/test_http.py
--rw-r--r--   0 james      (501) staff       (20)    11476 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/tests/test_local.py
--rw-r--r--   0 james      (501) staff       (20)    19667 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/tests/test_s3.py
--rw-r--r--   0 james      (501) staff       (20)      500 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/bytes/utils.py
--rw-r--r--   0 james      (501) staff       (20)     2001 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/cache.py
--rw-r--r--   0 james      (501) staff       (20)     4067 2022-10-24 20:44:15.000000 dask-2023.5.1/dask/callbacks.py
--rw-r--r--   0 james      (501) staff       (20)     3064 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/cli.py
--rw-r--r--   0 james      (501) staff       (20)      523 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/compatibility.py
--rw-r--r--   0 james      (501) staff       (20)    21645 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/config.py
--rw-r--r--   0 james      (501) staff       (20)     1756 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/context.py
--rw-r--r--   0 james      (501) staff       (20)    14833 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/core.py
--rw-r--r--   0 james      (501) staff       (20)     6944 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/dask-schema.yaml
--rw-r--r--   0 james      (501) staff       (20)     1498 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/dask.yaml
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.925194 dask-2023.5.1/dask/dataframe/
--rw-r--r--   0 james      (501) staff       (20)     1812 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7496 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/_compat.py
--rw-r--r--   0 james      (501) staff       (20)     2171 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/_dtypes.py
--rw-r--r--   0 james      (501) staff       (20)     3219 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/_pyarrow.py
--rw-r--r--   0 james      (501) staff       (20)     1936 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/_pyarrow_compat.py
--rw-r--r--   0 james      (501) staff       (20)    12101 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/dataframe/accessor.py
--rw-r--r--   0 james      (501) staff       (20)    24298 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/backends.py
--rw-r--r--   0 james      (501) staff       (20)     9507 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/categorical.py
--rw-r--r--   0 james      (501) staff       (20)   302228 2023-05-26 16:32:18.000000 dask-2023.5.1/dask/dataframe/core.py
--rw-r--r--   0 james      (501) staff       (20)     4473 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/dispatch.py
--rw-r--r--   0 james      (501) staff       (20)      552 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/extensions.py
--rw-r--r--   0 james      (501) staff       (20)   114780 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/groupby.py
--rw-r--r--   0 james      (501) staff       (20)     2463 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/hyperloglog.py
--rw-r--r--   0 james      (501) staff       (20)    13412 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/indexing.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.933555 dask-2023.5.1/dask/dataframe/io/
--rw-r--r--   0 james      (501) staff       (20)      706 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    33811 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/csv.py
--rw-r--r--   0 james      (501) staff       (20)     5781 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/demo.py
--rw-r--r--   0 james      (501) staff       (20)    18079 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/hdf.py
--rw-r--r--   0 james      (501) staff       (20)    38487 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/io.py
--rw-r--r--   0 james      (501) staff       (20)    11163 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/json.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.937064 dask-2023.5.1/dask/dataframe/io/orc/
--rw-r--r--   0 james      (501) staff       (20)       92 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/orc/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     4487 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/orc/arrow.py
--rw-r--r--   0 james      (501) staff       (20)     7098 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/orc/core.py
--rw-r--r--   0 james      (501) staff       (20)      510 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/orc/utils.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.948404 dask-2023.5.1/dask/dataframe/io/parquet/
--rw-r--r--   0 james      (501) staff       (20)      166 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/parquet/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    71237 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/parquet/arrow.py
--rw-r--r--   0 james      (501) staff       (20)    66556 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/dataframe/io/parquet/core.py
--rw-r--r--   0 james      (501) staff       (20)    52426 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/parquet/fastparquet.py
--rw-r--r--   0 james      (501) staff       (20)    32896 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/parquet/utils.py
--rw-r--r--   0 james      (501) staff       (20)    21108 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/sql.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.963708 dask-2023.5.1/dask/dataframe/io/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-03-07 20:03:52.000000 dask-2023.5.1/dask/dataframe/io/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    59231 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_csv.py
--rw-r--r--   0 james      (501) staff       (20)     5036 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_demo.py
--rw-r--r--   0 james      (501) staff       (20)    27232 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_hdf.py
--rw-r--r--   0 james      (501) staff       (20)    34438 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_io.py
--rw-r--r--   0 james      (501) staff       (20)     8625 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_json.py
--rw-r--r--   0 james      (501) staff       (20)     5238 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_orc.py
--rw-r--r--   0 james      (501) staff       (20)   164976 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_parquet.py
--rw-r--r--   0 james      (501) staff       (20)    17632 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/tests/test_sql.py
--rw-r--r--   0 james      (501) staff       (20)     7899 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/io/utils.py
--rw-r--r--   0 james      (501) staff       (20)    14015 2023-05-26 19:43:33.000000 dask-2023.5.1/dask/dataframe/methods.py
--rw-r--r--   0 james      (501) staff       (20)    53884 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/multi.py
--rw-r--r--   0 james      (501) staff       (20)     1600 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/numeric.py
--rw-r--r--   0 james      (501) staff       (20)     8778 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/optimize.py
--rw-r--r--   0 james      (501) staff       (20)    20044 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/partitionquantiles.py
--rw-r--r--   0 james      (501) staff       (20)    11825 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/reshape.py
--rw-r--r--   0 james      (501) staff       (20)    22185 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/rolling.py
--rw-r--r--   0 james      (501) staff       (20)    37975 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/shuffle.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.998479 dask-2023.5.1/dask/dataframe/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.5.1/dask/dataframe/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    10633 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_accessors.py
--rw-r--r--   0 james      (501) staff       (20)    67628 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_arithmetics_reduction.py
--rw-r--r--   0 james      (501) staff       (20)      942 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_boolean.py
--rw-r--r--   0 james      (501) staff       (20)    16678 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_categorical.py
--rw-r--r--   0 james      (501) staff       (20)   192106 2023-05-26 16:32:18.000000 dask-2023.5.1/dask/dataframe/tests/test_dataframe.py
--rw-r--r--   0 james      (501) staff       (20)     1456 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_extensions.py
--rw-r--r--   0 james      (501) staff       (20)    14743 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_format.py
--rw-r--r--   0 james      (501) staff       (20)   120823 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_groupby.py
--rw-r--r--   0 james      (501) staff       (20)     2702 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_hashing.py
--rw-r--r--   0 james      (501) staff       (20)     2897 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_hyperloglog.py
--rw-r--r--   0 james      (501) staff       (20)    22382 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_indexing.py
--rw-r--r--   0 james      (501) staff       (20)     7034 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_merge_column_and_index.py
--rw-r--r--   0 james      (501) staff       (20)      463 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_methods.py
--rw-r--r--   0 james      (501) staff       (20)    91017 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_multi.py
--rw-r--r--   0 james      (501) staff       (20)     2120 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_numeric.py
--rw-r--r--   0 james      (501) staff       (20)     1067 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_optimize_dataframe.py
--rw-r--r--   0 james      (501) staff       (20)     6662 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_pyarrow.py
--rw-r--r--   0 james      (501) staff       (20)     4550 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_pyarrow_compat.py
--rw-r--r--   0 james      (501) staff       (20)    11571 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_reshape.py
--rw-r--r--   0 james      (501) staff       (20)    17524 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_rolling.py
--rw-r--r--   0 james      (501) staff       (20)    53386 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_shuffle.py
--rw-r--r--   0 james      (501) staff       (20)    16595 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_ufunc.py
--rw-r--r--   0 james      (501) staff       (20)    21288 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tests/test_utils_dataframe.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.000059 dask-2023.5.1/dask/dataframe/tseries/
--rw-r--r--   0 james      (501) staff       (20)        0 2021-06-08 02:50:30.000000 dask-2023.5.1/dask/dataframe/tseries/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     7664 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tseries/resample.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.001222 dask-2023.5.1/dask/dataframe/tseries/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.5.1/dask/dataframe/tseries/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     6866 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/tseries/tests/test_resample.py
--rw-r--r--   0 james      (501) staff       (20)    27404 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/dataframe/utils.py
--rw-r--r--   0 james      (501) staff       (20)     5314 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/datasets.py
--rw-r--r--   0 james      (501) staff       (20)    24389 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/delayed.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.003784 dask-2023.5.1/dask/diagnostics/
--rw-r--r--   0 james      (501) staff       (20)      258 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/diagnostics/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12136 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/diagnostics/profile.py
--rw-r--r--   0 james      (501) staff       (20)    16332 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/diagnostics/profile_visualize.py
--rw-r--r--   0 james      (501) staff       (20)     5001 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/diagnostics/progress.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.006323 dask-2023.5.1/dask/diagnostics/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.5.1/dask/diagnostics/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)    12045 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/diagnostics/tests/test_profiler.py
--rw-r--r--   0 james      (501) staff       (20)     3388 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/diagnostics/tests/test_progress.py
--rw-r--r--   0 james      (501) staff       (20)      715 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/distributed.py
--rw-r--r--   0 james      (501) staff       (20)    16587 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/dot.py
--rw-r--r--   0 james      (501) staff       (20)    19595 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/graph_manipulation.py
--rw-r--r--   0 james      (501) staff       (20)     2492 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/hashing.py
--rw-r--r--   0 james      (501) staff       (20)    34771 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/highlevelgraph.py
--rw-r--r--   0 james      (501) staff       (20)    46007 2023-05-03 18:02:08.000000 dask-2023.5.1/dask/layers.py
--rw-r--r--   0 james      (501) staff       (20)    18888 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/local.py
--rw-r--r--   0 james      (501) staff       (20)      487 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/ml.py
--rw-r--r--   0 james      (501) staff       (20)     8466 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/multiprocessing.py
--rw-r--r--   0 james      (501) staff       (20)    35638 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/optimization.py
--rw-r--r--   0 james      (501) staff       (20)    45768 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/order.py
--rw-r--r--   0 james      (501) staff       (20)        0 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/py.typed
--rw-r--r--   0 james      (501) staff       (20)    12597 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/rewrite.py
--rw-r--r--   0 james      (501) staff       (20)     7298 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/sizeof.py
--rw-r--r--   0 james      (501) staff       (20)     1510 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/system.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.045470 dask-2023.5.1/dask/tests/
--rw-r--r--   0 james      (501) staff       (20)        0 2023-03-07 20:04:31.000000 dask-2023.5.1/dask/tests/__init__.py
--rw-r--r--   0 james      (501) staff       (20)      742 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_backends.py
--rw-r--r--   0 james      (501) staff       (20)    51124 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_base.py
--rw-r--r--   0 james      (501) staff       (20)     1613 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_cache.py
--rw-r--r--   0 james      (501) staff       (20)     2570 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_callbacks.py
--rw-r--r--   0 james      (501) staff       (20)     1199 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_ci.py
--rw-r--r--   0 james      (501) staff       (20)     3266 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_cli.py
--rw-r--r--   0 james      (501) staff       (20)      379 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_compatibility.py
--rw-r--r--   0 james      (501) staff       (20)    17846 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_config.py
--rw-r--r--   0 james      (501) staff       (20)     1137 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_context.py
--rw-r--r--   0 james      (501) staff       (20)     7422 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_core.py
--rw-r--r--   0 james      (501) staff       (20)     1112 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_datasets.py
--rw-r--r--   0 james      (501) staff       (20)    22989 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_delayed.py
--rw-r--r--   0 james      (501) staff       (20)    31293 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_distributed.py
--rw-r--r--   0 james      (501) staff       (20)      925 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_docs.py
--rw-r--r--   0 james      (501) staff       (20)    12271 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_dot.py
--rw-r--r--   0 james      (501) staff       (20)    15070 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_graph_manipulation.py
--rw-r--r--   0 james      (501) staff       (20)     1095 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_hashing.py
--rw-r--r--   0 james      (501) staff       (20)     8363 2023-05-26 16:18:40.000000 dask-2023.5.1/dask/tests/test_highgraph.py
--rw-r--r--   0 james      (501) staff       (20)     9341 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_layers.py
--rw-r--r--   0 james      (501) staff       (20)     5008 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_local.py
--rw-r--r--   0 james      (501) staff       (20)      419 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_ml.py
--rw-r--r--   0 james      (501) staff       (20)     8457 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_multiprocessing.py
--rw-r--r--   0 james      (501) staff       (20)    45227 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_optimization.py
--rw-r--r--   0 james      (501) staff       (20)    28229 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_order.py
--rw-r--r--   0 james      (501) staff       (20)     4684 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_rewrite.py
--rw-r--r--   0 james      (501) staff       (20)     7518 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_sizeof.py
--rw-r--r--   0 james      (501) staff       (20)     7154 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_spark_compat.py
--rw-r--r--   0 james      (501) staff       (20)     1397 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_system.py
--rw-r--r--   0 james      (501) staff       (20)     4749 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_threaded.py
--rw-r--r--   0 james      (501) staff       (20)     5670 2023-04-25 18:34:46.000000 dask-2023.5.1/dask/tests/test_typing.py
--rw-r--r--   0 james      (501) staff       (20)    22705 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_utils.py
--rw-r--r--   0 james      (501) staff       (20)     1598 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/test_utils_test.py
--rw-r--r--   0 james      (501) staff       (20)      211 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/tests/warning_aliases.py
--rw-r--r--   0 james      (501) staff       (20)     2993 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/threaded.py
--rw-r--r--   0 james      (501) staff       (20)    14538 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/typing.py
--rw-r--r--   0 james      (501) staff       (20)    56051 2023-05-24 15:39:04.000000 dask-2023.5.1/dask/utils.py
--rw-r--r--   0 james      (501) staff       (20)     4825 2023-04-11 17:13:14.000000 dask-2023.5.1/dask/utils_test.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.046630 dask-2023.5.1/dask/widgets/
--rw-r--r--   0 james      (501) staff       (20)      792 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/widgets/__init__.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.051499 dask-2023.5.1/dask/widgets/templates/
--rw-r--r--   0 james      (501) staff       (20)     1295 2023-03-13 17:40:25.000000 dask-2023.5.1/dask/widgets/templates/array.html.j2
--rw-r--r--   0 james      (501) staff       (20)      124 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/widgets/templates/dataframe.html.j2
--rw-r--r--   0 james      (501) staff       (20)     2579 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/widgets/templates/highlevelgraph.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1981 2022-11-09 22:20:24.000000 dask-2023.5.1/dask/widgets/templates/highlevelgraph_layer.html.j2
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.052781 dask-2023.5.1/dask/widgets/tests/
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.056871 dask-2023.5.1/dask/widgets/tests/templates/
--rw-r--r--   0 james      (501) staff       (20)       38 2022-10-24 20:44:15.000000 dask-2023.5.1/dask/widgets/tests/templates/bytes.html.j2
--rw-r--r--   0 james      (501) staff       (20)       39 2022-10-24 20:44:15.000000 dask-2023.5.1/dask/widgets/tests/templates/custom_filter.html.j2
--rw-r--r--   0 james      (501) staff       (20)       30 2022-10-24 20:44:15.000000 dask-2023.5.1/dask/widgets/tests/templates/example.html.j2
--rw-r--r--   0 james      (501) staff       (20)     1401 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/widgets/tests/test_widgets.py
--rw-r--r--   0 james      (501) staff       (20)     1120 2023-05-24 20:58:41.000000 dask-2023.5.1/dask/widgets/widgets.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:34.772426 dask-2023.5.1/dask.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2532 2023-05-26 20:09:34.000000 dask-2023.5.1/dask.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)    13939 2023-05-26 20:09:34.000000 dask-2023.5.1/dask.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-26 20:09:34.000000 dask-2023.5.1/dask.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)      124 2023-05-26 20:09:34.000000 dask-2023.5.1/dask.egg-info/entry_points.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-05-26 20:09:33.000000 dask-2023.5.1/dask.egg-info/not-zip-safe
--rw-r--r--   0 james      (501) staff       (20)      454 2023-05-26 20:09:34.000000 dask-2023.5.1/dask.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)        5 2023-05-26 20:09:34.000000 dask-2023.5.1/dask.egg-info/top_level.txt
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.061375 dask-2023.5.1/docs/
--rw-r--r--   0 james      (501) staff       (20)     5741 2023-03-22 19:03:53.000000 dask-2023.5.1/docs/Makefile
--rw-r--r--   0 james      (501) staff       (20)     5186 2022-08-08 20:45:08.000000 dask-2023.5.1/docs/make.bat
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.301131 dask-2023.5.1/docs/source/
--rw-r--r--   0 james      (501) staff       (20)    17598 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/10-minutes-to-dask.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.315722 dask-2023.5.1/docs/source/_static/
--rw-r--r--   0 james      (501) staff       (20)    10187 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/_static/config_converter.js
--rw-r--r--   0 james      (501) staff       (20)    11021 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/_static/dask-simple.png
--rw-r--r--   0 james      (501) staff       (20)     2375 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/_static/main-page.css
--rw-r--r--   0 james      (501) staff       (20)    15598 2022-08-08 20:45:08.000000 dask-2023.5.1/docs/source/_static/profile.html
--rw-r--r--   0 james      (501) staff       (20)    65304 2022-08-08 20:45:08.000000 dask-2023.5.1/docs/source/_static/stacked_profile.html
--rw-r--r--   0 james      (501) staff       (20)      523 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/_static/style.css
--rw-r--r--   0 james      (501) staff       (20)      365 2021-06-16 20:41:28.000000 dask-2023.5.1/docs/source/_static/theme_overrides.css
--rw-r--r--   0 james      (501) staff       (20)   292662 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/_static/transpose_cyto.html
--rw-r--r--   0 james      (501) staff       (20)    49423 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/_static/yaml.min.js
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.317827 dask-2023.5.1/docs/source/_templates/
--rw-r--r--   0 james      (501) staff       (20)      180 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/_templates/layout.html
--rw-r--r--   0 james      (501) staff       (20)     2235 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/api.rst
--rw-r--r--   0 james      (501) staff       (20)     6968 2023-05-24 15:39:04.000000 dask-2023.5.1/docs/source/array-api.rst
--rw-r--r--   0 james      (501) staff       (20)     2943 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/array-assignment.rst
--rw-r--r--   0 james      (501) staff       (20)     4740 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/array-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)    13035 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array-chunks.rst
--rw-r--r--   0 james      (501) staff       (20)    18437 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array-creation.rst
--rw-r--r--   0 james      (501) staff       (20)     5885 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array-design.rst
--rw-r--r--   0 james      (501) staff       (20)     2857 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array-gufunc.rst
--rw-r--r--   0 james      (501) staff       (20)     6069 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/array-overlap.rst
--rw-r--r--   0 james      (501) staff       (20)     3924 2023-05-19 15:53:47.000000 dask-2023.5.1/docs/source/array-random.rst
--rw-r--r--   0 james      (501) staff       (20)     4137 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/array-slicing.rst
--rw-r--r--   0 james      (501) staff       (20)     3291 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array-sparse.rst
--rw-r--r--   0 james      (501) staff       (20)     2018 2022-10-07 21:37:36.000000 dask-2023.5.1/docs/source/array-stack.rst
--rw-r--r--   0 james      (501) staff       (20)     1140 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array-stats.rst
--rw-r--r--   0 james      (501) staff       (20)     4121 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/array.rst
--rw-r--r--   0 james      (501) staff       (20)     1574 2022-08-08 20:45:08.000000 dask-2023.5.1/docs/source/bag-api.rst
--rw-r--r--   0 james      (501) staff       (20)     4557 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/bag-creation.rst
--rw-r--r--   0 james      (501) staff       (20)     4068 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/bag.rst
--rw-r--r--   0 james      (501) staff       (20)    14050 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     5553 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/caching.rst
--rw-r--r--   0 james      (501) staff       (20)   305185 2023-05-26 20:04:56.000000 dask-2023.5.1/docs/source/changelog.rst
--rw-r--r--   0 james      (501) staff       (20)      211 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/cheatsheet.rst
--rw-r--r--   0 james      (501) staff       (20)     4047 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/cli.rst
--rw-r--r--   0 james      (501) staff       (20)    15465 2023-03-13 20:41:19.000000 dask-2023.5.1/docs/source/conf.py
--rw-r--r--   0 james      (501) staff       (20)    16654 2023-04-06 21:35:01.000000 dask-2023.5.1/docs/source/configuration.rst
--rw-r--r--   0 james      (501) staff       (20)    18651 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/custom-collections.rst
--rw-r--r--   0 james      (501) staff       (20)     3604 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/custom-graphs.rst
--rw-r--r--   0 james      (501) staff       (20)      932 2023-05-24 20:58:41.000000 dask-2023.5.1/docs/source/dashboard-progress-script.py
--rw-r--r--   0 james      (501) staff       (20)    15045 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/dashboard.rst
--rw-r--r--   0 james      (501) staff       (20)   203552 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/daskcheatsheet.pdf
--rw-r--r--   0 james      (501) staff       (20)    13693 2023-05-19 15:53:47.000000 dask-2023.5.1/docs/source/dataframe-api.rst
--rw-r--r--   0 james      (501) staff       (20)     9611 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/dataframe-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     3951 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/dataframe-categoricals.rst
--rw-r--r--   0 james      (501) staff       (20)     5967 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/dataframe-create.rst
--rw-r--r--   0 james      (501) staff       (20)     5002 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/dataframe-design.rst
--rw-r--r--   0 james      (501) staff       (20)     6224 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/dataframe-extend.rst
--rw-r--r--   0 james      (501) staff       (20)     8050 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/dataframe-groupby.rst
--rw-r--r--   0 james      (501) staff       (20)     6115 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/dataframe-indexing.rst
--rw-r--r--   0 james      (501) staff       (20)     3454 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/dataframe-joins.rst
--rw-r--r--   0 james      (501) staff       (20)    10952 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/dataframe-parquet.rst
--rw-r--r--   0 james      (501) staff       (20)    12661 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/dataframe-sql.rst
--rw-r--r--   0 james      (501) staff       (20)     7772 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/dataframe.rst
--rw-r--r--   0 james      (501) staff       (20)      363 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/debugging-performance.rst
--rw-r--r--   0 james      (501) staff       (20)     1696 2022-08-08 20:45:08.000000 dask-2023.5.1/docs/source/delayed-api.rst
--rw-r--r--   0 james      (501) staff       (20)    17616 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/delayed-best-practices.rst
--rw-r--r--   0 james      (501) staff       (20)     1497 2022-10-07 21:37:36.000000 dask-2023.5.1/docs/source/delayed-collections.rst
--rw-r--r--   0 james      (501) staff       (20)     6357 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/delayed.rst
--rw-r--r--   0 james      (501) staff       (20)     3620 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/deploying-cli.rst
--rw-r--r--   0 james      (501) staff       (20)     3012 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/deploying-cloud.rst
--rw-r--r--   0 james      (501) staff       (20)     2868 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/deploying-docker.rst
--rw-r--r--   0 james      (501) staff       (20)     9939 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/deploying-hpc.rst
--rw-r--r--   0 james      (501) staff       (20)     4001 2023-05-19 15:53:47.000000 dask-2023.5.1/docs/source/deploying-kubernetes.rst
--rw-r--r--   0 james      (501) staff       (20)     5823 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/deploying-python-advanced.rst
--rw-r--r--   0 james      (501) staff       (20)     2839 2023-04-25 18:34:46.000000 dask-2023.5.1/docs/source/deploying-python.rst
--rw-r--r--   0 james      (501) staff       (20)     1619 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/deploying-ssh.rst
--rw-r--r--   0 james      (501) staff       (20)     7348 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/deploying.rst
--rw-r--r--   0 james      (501) staff       (20)    10873 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/deployment-considerations.rst
--rw-r--r--   0 james      (501) staff       (20)    13144 2023-05-24 20:58:41.000000 dask-2023.5.1/docs/source/develop.rst
--rw-r--r--   0 james      (501) staff       (20)     4442 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/diagnostics-distributed.rst
--rw-r--r--   0 james      (501) staff       (20)    10407 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/diagnostics-local.rst
--rw-r--r--   0 james      (501) staff       (20)     4364 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/ecosystem.rst
--rw-r--r--   0 james      (501) staff       (20)    19999 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/faq.rst
--rw-r--r--   0 james      (501) staff       (20)    25569 2023-05-19 15:53:47.000000 dask-2023.5.1/docs/source/futures.rst
--rw-r--r--   0 james      (501) staff       (20)     5820 2022-10-07 21:37:14.000000 dask-2023.5.1/docs/source/gpu.rst
--rw-r--r--   0 james      (501) staff       (20)     2541 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/graph_manipulation.rst
--rw-r--r--   0 james      (501) staff       (20)     5433 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/graphs.rst
--rw-r--r--   0 james      (501) staff       (20)     5399 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/graphviz.rst
--rw-r--r--   0 james      (501) staff       (20)     6946 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/high-level-graphs.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.332580 dask-2023.5.1/docs/source/how-to/
--rw-r--r--   0 james      (501) staff       (20)     4364 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/how-to/adaptive.rst
--rw-r--r--   0 james      (501) staff       (20)    15360 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/how-to/connect-to-remote-data.rst
--rw-r--r--   0 james      (501) staff       (20)     4209 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/how-to/customize-initialization.rst
--rw-r--r--   0 james      (501) staff       (20)    10859 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/how-to/debug.rst
--rw-r--r--   0 james      (501) staff       (20)     1722 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/how-to/extend-sizeof.rst
--rw-r--r--   0 james      (501) staff       (20)      433 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/how-to/index.rst
--rw-r--r--   0 james      (501) staff       (20)     4562 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/how-to/manage-environments.rst
--rw-r--r--   0 james      (501) staff       (20)     6680 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/how-to/selecting-the-collection-backend.rst
--rw-r--r--   0 james      (501) staff       (20)      902 2023-04-25 18:34:46.000000 dask-2023.5.1/docs/source/how-to/setup-prometheus.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.475904 dask-2023.5.1/docs/source/images/
--rw-r--r--   0 james      (501) staff       (20)    99565 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/10_minutes_array_graph.png
--rw-r--r--   0 james      (501) staff       (20)    22442 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/10_minutes_bag_graph.png
--rw-r--r--   0 james      (501) staff       (20)    56229 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/10_minutes_dataframe_graph.png
--rw-r--r--   0 james      (501) staff       (20)     4059 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/HHMI_Janelia_Color.png
--rw-r--r--   0 james      (501) staff       (20)    18406 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/array.svg
--rw-r--r--   0 james      (501) staff       (20)  1620104 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/async-embarrassing.gif
--rw-r--r--   0 james      (501) staff       (20)    10752 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/concurrent-futures-threaded.webp
--rw-r--r--   0 james      (501) staff       (20)   135129 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/crosstalk.svg
--rw-r--r--   0 james      (501) staff       (20)  2367087 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dashboard_jupyterlab.png
--rw-r--r--   0 james      (501) staff       (20)    37971 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dashboard_link.png
--rw-r--r--   0 james      (501) staff       (20)    68712 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dashboard_memory.png
--rw-r--r--   0 james      (501) staff       (20)   281018 2023-04-25 18:34:46.000000 dask-2023.5.1/docs/source/images/dashboard_memory_new.gif
--rw-r--r--   0 james      (501) staff       (20)    25435 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/images/dashboard_progress.png
--rw-r--r--   0 james      (501) staff       (20)   276928 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/images/dashboard_status.png
--rw-r--r--   0 james      (501) staff       (20)    12009 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/images/dashboard_task_processing.png
--rw-r--r--   0 james      (501) staff       (20)    58238 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dashboard_task_stream_unhealthy.png
--rw-r--r--   0 james      (501) staff       (20)   103654 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dashboard_taskstream_healthy.png
--rw-r--r--   0 james      (501) staff       (20)   112822 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/dask-adaptive.svg
--rw-r--r--   0 james      (501) staff       (20)    14645 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/dask-array.svg
--rw-r--r--   0 james      (501) staff       (20)   222084 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/dask-cluster-manager.svg
--rw-r--r--   0 james      (501) staff       (20)    18782 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/dask-dataframe.svg
--rw-r--r--   0 james      (501) staff       (20)   381903 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask-overview-distributed-callout.svg
--rw-r--r--   0 james      (501) staff       (20)   357643 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask-overview-schedulers.svg
--rw-r--r--   0 james      (501) staff       (20)    97471 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/dask-overview.svg
--rw-r--r--   0 james      (501) staff       (20)     3022 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_horizontal.svg
--rw-r--r--   0 james      (501) staff       (20)     3651 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_horizontal_black.svg
--rw-r--r--   0 james      (501) staff       (20)     3767 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_horizontal_on_blue.svg
--rw-r--r--   0 james      (501) staff       (20)     3738 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_horizontal_on_pink.svg
--rw-r--r--   0 james      (501) staff       (20)     3738 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_horizontal_white.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_icon.svg
--rw-r--r--   0 james      (501) staff       (20)     1571 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_icon_black.svg
--rw-r--r--   0 james      (501) staff       (20)     1607 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_icon_on_pink.svg
--rw-r--r--   0 james      (501) staff       (20)     1609 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/dask_icon_white.svg
--rw-r--r--   0 james      (501) staff       (20)    20216 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/delayed-inc-double-add.svg
--rw-r--r--   0 james      (501) staff       (20)   104628 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/distributed-overview.svg
--rw-r--r--   0 james      (501) staff       (20)    18297 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/frame-shuffle.svg
--rw-r--r--   0 james      (501) staff       (20)    22979 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/frame-sort.svg
--rw-r--r--   0 james      (501) staff       (20)    12181 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/frame.svg
--rw-r--r--   0 james      (501) staff       (20)    41828 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/gputester-msg.png
--rw-r--r--   0 james      (501) staff       (20)   210392 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/growth_of_languages.png
--rw-r--r--   0 james      (501) staff       (20)   167834 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/growth_of_libraries.png
--rw-r--r--   0 james      (501) staff       (20)     4097 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/inc-add.svg
--rw-r--r--   0 james      (501) staff       (20)   123010 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/map-reduce-task-scheduling.svg
--rw-r--r--   0 james      (501) staff       (20)   482302 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/map_blocks_drop_axis.png
--rw-r--r--   0 james      (501) staff       (20)   113067 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/merge_chunks.png
--rw-r--r--   0 james      (501) staff       (20)    63244 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/merge_chunks_false.png
--rw-r--r--   0 james      (501) staff       (20)    13024 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/optimize_dask1.svg
--rw-r--r--   0 james      (501) staff       (20)     8803 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/optimize_dask2.svg
--rw-r--r--   0 james      (501) staff       (20)     5198 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/optimize_dask3.svg
--rw-r--r--   0 james      (501) staff       (20)     4104 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/optimize_dask4.svg
--rw-r--r--   0 james      (501) staff       (20)     2738 2021-11-11 17:33:01.000000 dask-2023.5.1/docs/source/images/optimize_dask5.svg
--rw-r--r--   0 james      (501) staff       (20)   292827 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/order-failure.png
--rw-r--r--   0 james      (501) staff       (20)   239828 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/order-success.png
--rw-r--r--   0 james      (501) staff       (20)    40833 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/overlap.svg
--rw-r--r--   0 james      (501) staff       (20)    18785 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/overlapping-blocks.svg
--rw-r--r--   0 james      (501) staff       (20)     4537 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/overlapping-neighbors.svg
--rw-r--r--   0 james      (501) staff       (20)    20533 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/pipeline.svg
--rw-r--r--   0 james      (501) staff       (20)    31576 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/reshape.png
--rw-r--r--   0 james      (501) staff       (20)    31410 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/reshape_problem.png
--rw-r--r--   0 james      (501) staff       (20)    33288 2021-11-11 20:27:17.000000 dask-2023.5.1/docs/source/images/reshape_rechunked.png
--rw-r--r--   0 james      (501) staff       (20)    50209 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/scaling-edges.png
--rw-r--r--   0 james      (501) staff       (20)    68476 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/scaling-nodes.png
--rw-r--r--   0 james      (501) staff       (20)    21294 2021-06-08 02:50:31.000000 dask-2023.5.1/docs/source/images/simple-dask.png
--rw-r--r--   0 james      (501) staff       (20)    27572 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/transpose-hlg-hovertooltip.png
--rw-r--r--   0 james      (501) staff       (20)    84492 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/images/transpose-hlg-html-repr.png
--rw-r--r--   0 james      (501) staff       (20)    39365 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/transpose.svg
--rw-r--r--   0 james      (501) staff       (20)    22446 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/transpose_opt.svg
--rw-r--r--   0 james      (501) staff       (20)   115022 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/images/trivial.svg
--rw-r--r--   0 james      (501) staff       (20)     2451 2021-06-08 02:51:08.000000 dask-2023.5.1/docs/source/images/unoverlapping-neighbors.svg
--rw-r--r--   0 james      (501) staff       (20)     6237 2023-03-13 17:40:25.000000 dask-2023.5.1/docs/source/index.rst
--rw-r--r--   0 james      (501) staff       (20)    15235 2023-05-24 20:58:41.000000 dask-2023.5.1/docs/source/install.rst
--rw-r--r--   0 james      (501) staff       (20)      341 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/internals.rst
--rw-r--r--   0 james      (501) staff       (20)      868 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/logos.rst
--rw-r--r--   0 james      (501) staff       (20)     3573 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/maintainers.rst
--rw-r--r--   0 james      (501) staff       (20)    12200 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/optimize.rst
--rw-r--r--   0 james      (501) staff       (20)     7119 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/order.rst
--rw-r--r--   0 james      (501) staff       (20)     4810 2022-10-07 21:37:14.000000 dask-2023.5.1/docs/source/phases-of-computation.rst
--rw-r--r--   0 james      (501) staff       (20)     5089 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/presentations.rst
--rw-r--r--   0 james      (501) staff       (20)     6010 2022-10-07 21:37:14.000000 dask-2023.5.1/docs/source/scheduler-overview.rst
--rw-r--r--   0 james      (501) staff       (20)     4493 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/scheduling-policy.rst
--rw-r--r--   0 james      (501) staff       (20)    11015 2023-05-24 20:58:41.000000 dask-2023.5.1/docs/source/scheduling.rst
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-05-26 20:09:35.477147 dask-2023.5.1/docs/source/scripts/
--rw-r--r--   0 james      (501) staff       (20)     3294 2023-05-24 20:58:41.000000 dask-2023.5.1/docs/source/scripts/scheduling.py
--rw-r--r--   0 james      (501) staff       (20)     6104 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/shared.rst
--rw-r--r--   0 james      (501) staff       (20)     9342 2022-11-09 22:20:24.000000 dask-2023.5.1/docs/source/spark.rst
--rw-r--r--   0 james      (501) staff       (20)     3966 2022-10-07 21:37:14.000000 dask-2023.5.1/docs/source/spec.rst
--rw-r--r--   0 james      (501) staff       (20)     4754 2023-05-22 17:52:26.000000 dask-2023.5.1/docs/source/support.rst
--rw-r--r--   0 james      (501) staff       (20)     1831 2021-06-16 20:41:28.000000 dask-2023.5.1/docs/source/understanding-performance.rst
--rw-r--r--   0 james      (501) staff       (20)    12205 2023-05-03 18:02:08.000000 dask-2023.5.1/docs/source/user-interfaces.rst
--rw-r--r--   0 james      (501) staff       (20)    11744 2022-10-24 20:44:15.000000 dask-2023.5.1/docs/source/why.rst
--rw-r--r--   0 james      (501) staff       (20)     5713 2023-05-26 19:49:48.000000 dask-2023.5.1/pyproject.toml
--rw-r--r--   0 james      (501) staff       (20)       38 2023-05-26 20:09:35.479697 dask-2023.5.1/setup.cfg
--rwxr-xr-x   0 james      (501) staff       (20)      194 2023-05-03 18:02:08.000000 dask-2023.5.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.358937 dask-2023.6.0/
+-rw-r--r--   0 james      (501) staff       (20)     1531 2022-10-24 20:44:15.000000 dask-2023.6.0/LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)      325 2022-11-09 22:20:24.000000 dask-2023.6.0/MANIFEST.in
+-rw-r--r--   0 james      (501) staff       (20)     2532 2023-06-09 16:34:13.358263 dask-2023.6.0/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1291 2022-11-09 22:20:24.000000 dask-2023.6.0/README.rst
+-rw-r--r--   0 james      (501) staff       (20)     2397 2023-05-31 15:34:32.000000 dask-2023.6.0/conftest.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.359490 dask-2023.6.0/dask/
+-rw-r--r--   0 james      (501) staff       (20)      464 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      133 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/__main__.py
+-rw-r--r--   0 james      (501) staff       (20)      643 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/_compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2023-06-09 16:34:13.359618 dask-2023.6.0/dask/_version.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.897849 dask-2023.6.0/dask/array/
+-rw-r--r--   0 james      (501) staff       (20)     1543 2021-06-08 02:50:30.000000 dask-2023.6.0/dask/array/NUMPY_LICENSE.txt
+-rw-r--r--   0 james      (501) staff       (20)     5413 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12600 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/backends.py
+-rw-r--r--   0 james      (501) staff       (20)     9983 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/blockwise.py
+-rw-r--r--   0 james      (501) staff       (20)    12304 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/chunk.py
+-rw-r--r--   0 james      (501) staff       (20)     5066 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/chunk_types.py
+-rw-r--r--   0 james      (501) staff       (20)   190916 2023-05-31 19:49:19.000000 dask-2023.6.0/dask/array/core.py
+-rw-r--r--   0 james      (501) staff       (20)    40564 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/array/creation.py
+-rw-r--r--   0 james      (501) staff       (20)     2114 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/cupy_entry_point.py
+-rw-r--r--   0 james      (501) staff       (20)      526 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     9189 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/einsumfuncs.py
+-rw-r--r--   0 james      (501) staff       (20)     7252 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/fft.py
+-rw-r--r--   0 james      (501) staff       (20)    32656 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     1996 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/image.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.898543 dask-2023.6.0/dask/array/lib/
+-rw-r--r--   0 james      (501) staff       (20)       77 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/lib/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      101 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/lib/stride_tricks.py
+-rw-r--r--   0 james      (501) staff       (20)    53335 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/linalg.py
+-rw-r--r--   0 james      (501) staff       (20)     6363 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/ma.py
+-rw-r--r--   0 james      (501) staff       (20)     5699 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/numpy_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    12838 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    28480 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/overlap.py
+-rw-r--r--   0 james      (501) staff       (20)    10652 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/percentile.py
+-rw-r--r--   0 james      (501) staff       (20)    40604 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/random.py
+-rw-r--r--   0 james      (501) staff       (20)    28023 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    57287 2023-06-01 20:02:33.000000 dask-2023.6.0/dask/array/reductions.py
+-rw-r--r--   0 james      (501) staff       (20)    10765 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    81988 2023-05-19 15:53:47.000000 dask-2023.6.0/dask/array/routines.py
+-rw-r--r--   0 james      (501) staff       (20)    72631 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/slicing.py
+-rw-r--r--   0 james      (501) staff       (20)    14613 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/stats.py
+-rw-r--r--   0 james      (501) staff       (20)     8048 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/svg.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.916697 dask-2023.6.0/dask/array/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.6.0/dask/array/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)   161461 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_array_core.py
+-rw-r--r--   0 james      (501) staff       (20)     6689 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_array_function.py
+-rw-r--r--   0 james      (501) staff       (20)     3159 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_array_utils.py
+-rw-r--r--   0 james      (501) staff       (20)    23222 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_atop.py
+-rw-r--r--   0 james      (501) staff       (20)     3304 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_chunk.py
+-rw-r--r--   0 james      (501) staff       (20)    31150 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_creation.py
+-rw-r--r--   0 james      (501) staff       (20)    19888 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_core.py
+-rw-r--r--   0 james      (501) staff       (20)     6456 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_creation.py
+-rw-r--r--   0 james      (501) staff       (20)      594 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    13412 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_linalg.py
+-rw-r--r--   0 james      (501) staff       (20)     4303 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_overlap.py
+-rw-r--r--   0 james      (501) staff       (20)     2862 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_percentile.py
+-rw-r--r--   0 james      (501) staff       (20)     9219 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_random.py
+-rw-r--r--   0 james      (501) staff       (20)     2224 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)     7437 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_routines.py
+-rw-r--r--   0 james      (501) staff       (20)     4877 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_slicing.py
+-rw-r--r--   0 james      (501) staff       (20)     2982 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_cupy_sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     8865 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)     8437 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_fft.py
+-rw-r--r--   0 james      (501) staff       (20)    21013 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_gufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     1482 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_image.py
+-rw-r--r--   0 james      (501) staff       (20)    36448 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_linalg.py
+-rw-r--r--   0 james      (501) staff       (20)    15635 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_masked.py
+-rw-r--r--   0 james      (501) staff       (20)     1087 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_numpy_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    17446 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    26718 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_overlap.py
+-rw-r--r--   0 james      (501) staff       (20)     3443 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_percentiles.py
+-rw-r--r--   0 james      (501) staff       (20)    15353 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_random.py
+-rw-r--r--   0 james      (501) staff       (20)    36341 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_rechunk.py
+-rw-r--r--   0 james      (501) staff       (20)    32756 2023-06-01 20:02:33.000000 dask-2023.6.0/dask/array/tests/test_reductions.py
+-rw-r--r--   0 james      (501) staff       (20)     7289 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    83849 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_routines.py
+-rw-r--r--   0 james      (501) staff       (20)    32302 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_slicing.py
+-rw-r--r--   0 james      (501) staff       (20)     6592 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_sparse.py
+-rw-r--r--   0 james      (501) staff       (20)     5489 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_stats.py
+-rw-r--r--   0 james      (501) staff       (20)     2740 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_svg.py
+-rw-r--r--   0 james      (501) staff       (20)      525 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_testing.py
+-rw-r--r--   0 james      (501) staff       (20)    17390 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)     2706 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_wrap.py
+-rw-r--r--   0 james      (501) staff       (20)     1317 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tests/test_xarray.py
+-rw-r--r--   0 james      (501) staff       (20)     4737 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/tiledb_io.py
+-rw-r--r--   0 james      (501) staff       (20)     9943 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    18674 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     6906 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/array/wrap.py
+-rw-r--r--   0 james      (501) staff       (20)     4936 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/backends.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.918953 dask-2023.6.0/dask/bag/
+-rw-r--r--   0 james      (501) staff       (20)      903 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     9111 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/avro.py
+-rw-r--r--   0 james      (501) staff       (20)      763 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/chunk.py
+-rw-r--r--   0 james      (501) staff       (20)    84784 2023-05-24 15:39:04.000000 dask-2023.6.0/dask/bag/core.py
+-rw-r--r--   0 james      (501) staff       (20)     5464 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/random.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.920979 dask-2023.6.0/dask/bag/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.6.0/dask/bag/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     3808 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/tests/test_avro.py
+-rw-r--r--   0 james      (501) staff       (20)    50747 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/tests/test_bag.py
+-rw-r--r--   0 james      (501) staff       (20)     6528 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/tests/test_random.py
+-rw-r--r--   0 james      (501) staff       (20)     5049 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/tests/test_text.py
+-rw-r--r--   0 james      (501) staff       (20)     6765 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/text.py
+-rw-r--r--   0 james      (501) staff       (20)      241 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bag/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    52086 2023-06-01 18:18:40.000000 dask-2023.6.0/dask/base.py
+-rw-r--r--   0 james      (501) staff       (20)    53252 2023-05-19 15:53:47.000000 dask-2023.6.0/dask/blockwise.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.922026 dask-2023.6.0/dask/bytes/
+-rw-r--r--   0 james      (501) staff       (20)       75 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6933 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/core.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.924679 dask-2023.6.0/dask/bytes/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.6.0/dask/bytes/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     5158 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/tests/test_bytes_utils.py
+-rw-r--r--   0 james      (501) staff       (20)      530 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/tests/test_compression.py
+-rw-r--r--   0 james      (501) staff       (20)     6657 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/bytes/tests/test_http.py
+-rw-r--r--   0 james      (501) staff       (20)    11476 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/tests/test_local.py
+-rw-r--r--   0 james      (501) staff       (20)    19667 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/tests/test_s3.py
+-rw-r--r--   0 james      (501) staff       (20)      500 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/bytes/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     2001 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/cache.py
+-rw-r--r--   0 james      (501) staff       (20)     4067 2022-10-24 20:44:15.000000 dask-2023.6.0/dask/callbacks.py
+-rw-r--r--   0 james      (501) staff       (20)     3064 2023-06-09 16:12:58.000000 dask-2023.6.0/dask/cli.py
+-rw-r--r--   0 james      (501) staff       (20)      523 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)    21645 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/config.py
+-rw-r--r--   0 james      (501) staff       (20)     1756 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/context.py
+-rw-r--r--   0 james      (501) staff       (20)    14833 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/core.py
+-rw-r--r--   0 james      (501) staff       (20)     6944 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/dask-schema.yaml
+-rw-r--r--   0 james      (501) staff       (20)     1498 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/dask.yaml
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.936339 dask-2023.6.0/dask/dataframe/
+-rw-r--r--   0 james      (501) staff       (20)     1812 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7496 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/_compat.py
+-rw-r--r--   0 james      (501) staff       (20)     2171 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/_dtypes.py
+-rw-r--r--   0 james      (501) staff       (20)     3219 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/_pyarrow.py
+-rw-r--r--   0 james      (501) staff       (20)     1936 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/_pyarrow_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    12101 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/dataframe/accessor.py
+-rw-r--r--   0 james      (501) staff       (20)    24298 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/backends.py
+-rw-r--r--   0 james      (501) staff       (20)     9507 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   302228 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/core.py
+-rw-r--r--   0 james      (501) staff       (20)     4473 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/dispatch.py
+-rw-r--r--   0 james      (501) staff       (20)      552 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/extensions.py
+-rw-r--r--   0 james      (501) staff       (20)   114809 2023-06-01 18:18:42.000000 dask-2023.6.0/dask/dataframe/groupby.py
+-rw-r--r--   0 james      (501) staff       (20)     2463 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/hyperloglog.py
+-rw-r--r--   0 james      (501) staff       (20)    13412 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/indexing.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.942878 dask-2023.6.0/dask/dataframe/io/
+-rw-r--r--   0 james      (501) staff       (20)      706 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    33811 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/csv.py
+-rw-r--r--   0 james      (501) staff       (20)     5781 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/demo.py
+-rw-r--r--   0 james      (501) staff       (20)    18079 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    38487 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/io.py
+-rw-r--r--   0 james      (501) staff       (20)    11163 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/json.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.944402 dask-2023.6.0/dask/dataframe/io/orc/
+-rw-r--r--   0 james      (501) staff       (20)       92 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/orc/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     4487 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/orc/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)     7098 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/orc/core.py
+-rw-r--r--   0 james      (501) staff       (20)      510 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/orc/utils.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.947088 dask-2023.6.0/dask/dataframe/io/parquet/
+-rw-r--r--   0 james      (501) staff       (20)      166 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/parquet/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    71237 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/parquet/arrow.py
+-rw-r--r--   0 james      (501) staff       (20)    67219 2023-06-01 18:18:42.000000 dask-2023.6.0/dask/dataframe/io/parquet/core.py
+-rw-r--r--   0 james      (501) staff       (20)    52426 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/parquet/fastparquet.py
+-rw-r--r--   0 james      (501) staff       (20)    32896 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/parquet/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    21108 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/sql.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.952834 dask-2023.6.0/dask/dataframe/io/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-03-07 20:03:52.000000 dask-2023.6.0/dask/dataframe/io/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    59231 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_csv.py
+-rw-r--r--   0 james      (501) staff       (20)     5036 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_demo.py
+-rw-r--r--   0 james      (501) staff       (20)    27232 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_hdf.py
+-rw-r--r--   0 james      (501) staff       (20)    34438 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_io.py
+-rw-r--r--   0 james      (501) staff       (20)     8625 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_json.py
+-rw-r--r--   0 james      (501) staff       (20)     5238 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_orc.py
+-rw-r--r--   0 james      (501) staff       (20)   165615 2023-06-01 18:18:42.000000 dask-2023.6.0/dask/dataframe/io/tests/test_parquet.py
+-rw-r--r--   0 james      (501) staff       (20)    17632 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/tests/test_sql.py
+-rw-r--r--   0 james      (501) staff       (20)     7899 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/io/utils.py
+-rw-r--r--   0 james      (501) staff       (20)    14019 2023-06-01 18:18:40.000000 dask-2023.6.0/dask/dataframe/methods.py
+-rw-r--r--   0 james      (501) staff       (20)    53884 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/multi.py
+-rw-r--r--   0 james      (501) staff       (20)     1600 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/numeric.py
+-rw-r--r--   0 james      (501) staff       (20)     8778 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/optimize.py
+-rw-r--r--   0 james      (501) staff       (20)    20044 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/partitionquantiles.py
+-rw-r--r--   0 james      (501) staff       (20)    11825 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    22185 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    37975 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/shuffle.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.964979 dask-2023.6.0/dask/dataframe/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.6.0/dask/dataframe/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    10633 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_accessors.py
+-rw-r--r--   0 james      (501) staff       (20)    67628 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_arithmetics_reduction.py
+-rw-r--r--   0 james      (501) staff       (20)      942 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_boolean.py
+-rw-r--r--   0 james      (501) staff       (20)    16678 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_categorical.py
+-rw-r--r--   0 james      (501) staff       (20)   192106 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_dataframe.py
+-rw-r--r--   0 james      (501) staff       (20)     1456 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_extensions.py
+-rw-r--r--   0 james      (501) staff       (20)    14743 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_format.py
+-rw-r--r--   0 james      (501) staff       (20)   121269 2023-06-01 18:18:42.000000 dask-2023.6.0/dask/dataframe/tests/test_groupby.py
+-rw-r--r--   0 james      (501) staff       (20)     2702 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_hashing.py
+-rw-r--r--   0 james      (501) staff       (20)     2897 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_hyperloglog.py
+-rw-r--r--   0 james      (501) staff       (20)    22382 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_indexing.py
+-rw-r--r--   0 james      (501) staff       (20)     7034 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_merge_column_and_index.py
+-rw-r--r--   0 james      (501) staff       (20)      463 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_methods.py
+-rw-r--r--   0 james      (501) staff       (20)    91017 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_multi.py
+-rw-r--r--   0 james      (501) staff       (20)     2120 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_numeric.py
+-rw-r--r--   0 james      (501) staff       (20)     1067 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_optimize_dataframe.py
+-rw-r--r--   0 james      (501) staff       (20)     6662 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_pyarrow.py
+-rw-r--r--   0 james      (501) staff       (20)     4550 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_pyarrow_compat.py
+-rw-r--r--   0 james      (501) staff       (20)    11571 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_reshape.py
+-rw-r--r--   0 james      (501) staff       (20)    17524 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_rolling.py
+-rw-r--r--   0 james      (501) staff       (20)    53386 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_shuffle.py
+-rw-r--r--   0 james      (501) staff       (20)    16595 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_ufunc.py
+-rw-r--r--   0 james      (501) staff       (20)    21288 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tests/test_utils_dataframe.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.965894 dask-2023.6.0/dask/dataframe/tseries/
+-rw-r--r--   0 james      (501) staff       (20)        0 2021-06-08 02:50:30.000000 dask-2023.6.0/dask/dataframe/tseries/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     7664 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tseries/resample.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.966782 dask-2023.6.0/dask/dataframe/tseries/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.6.0/dask/dataframe/tseries/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     6866 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/tseries/tests/test_resample.py
+-rw-r--r--   0 james      (501) staff       (20)    27404 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/dataframe/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     5314 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/datasets.py
+-rw-r--r--   0 james      (501) staff       (20)    24389 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/delayed.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.968757 dask-2023.6.0/dask/diagnostics/
+-rw-r--r--   0 james      (501) staff       (20)      258 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/diagnostics/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12136 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/diagnostics/profile.py
+-rw-r--r--   0 james      (501) staff       (20)    16332 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/diagnostics/profile_visualize.py
+-rw-r--r--   0 james      (501) staff       (20)     5001 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/diagnostics/progress.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.970032 dask-2023.6.0/dask/diagnostics/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-02-04 20:18:56.000000 dask-2023.6.0/dask/diagnostics/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)    12045 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/diagnostics/tests/test_profiler.py
+-rw-r--r--   0 james      (501) staff       (20)     3388 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/diagnostics/tests/test_progress.py
+-rw-r--r--   0 james      (501) staff       (20)      715 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/distributed.py
+-rw-r--r--   0 james      (501) staff       (20)    16587 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/dot.py
+-rw-r--r--   0 james      (501) staff       (20)    19595 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/graph_manipulation.py
+-rw-r--r--   0 james      (501) staff       (20)     2492 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/hashing.py
+-rw-r--r--   0 james      (501) staff       (20)    34771 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/highlevelgraph.py
+-rw-r--r--   0 james      (501) staff       (20)    46007 2023-05-03 18:02:08.000000 dask-2023.6.0/dask/layers.py
+-rw-r--r--   0 james      (501) staff       (20)    18888 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/local.py
+-rw-r--r--   0 james      (501) staff       (20)      487 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/ml.py
+-rw-r--r--   0 james      (501) staff       (20)     8466 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/multiprocessing.py
+-rw-r--r--   0 james      (501) staff       (20)    35638 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    45768 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/order.py
+-rw-r--r--   0 james      (501) staff       (20)        0 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/py.typed
+-rw-r--r--   0 james      (501) staff       (20)    12597 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/rewrite.py
+-rw-r--r--   0 james      (501) staff       (20)     7298 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)     1510 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/system.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.990899 dask-2023.6.0/dask/tests/
+-rw-r--r--   0 james      (501) staff       (20)        0 2023-03-07 20:04:31.000000 dask-2023.6.0/dask/tests/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)      742 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_backends.py
+-rw-r--r--   0 james      (501) staff       (20)    51124 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_base.py
+-rw-r--r--   0 james      (501) staff       (20)     1613 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_cache.py
+-rw-r--r--   0 james      (501) staff       (20)     2570 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_callbacks.py
+-rw-r--r--   0 james      (501) staff       (20)     1199 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_ci.py
+-rw-r--r--   0 james      (501) staff       (20)     3266 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_cli.py
+-rw-r--r--   0 james      (501) staff       (20)      379 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_compatibility.py
+-rw-r--r--   0 james      (501) staff       (20)    17846 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_config.py
+-rw-r--r--   0 james      (501) staff       (20)     1137 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_context.py
+-rw-r--r--   0 james      (501) staff       (20)     7422 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_core.py
+-rw-r--r--   0 james      (501) staff       (20)     1112 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_datasets.py
+-rw-r--r--   0 james      (501) staff       (20)    22989 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_delayed.py
+-rw-r--r--   0 james      (501) staff       (20)    31293 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_distributed.py
+-rw-r--r--   0 james      (501) staff       (20)      925 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_docs.py
+-rw-r--r--   0 james      (501) staff       (20)    12271 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_dot.py
+-rw-r--r--   0 james      (501) staff       (20)    15070 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_graph_manipulation.py
+-rw-r--r--   0 james      (501) staff       (20)     1095 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_hashing.py
+-rw-r--r--   0 james      (501) staff       (20)     8363 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_highgraph.py
+-rw-r--r--   0 james      (501) staff       (20)     9341 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_layers.py
+-rw-r--r--   0 james      (501) staff       (20)     5008 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_local.py
+-rw-r--r--   0 james      (501) staff       (20)      419 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_ml.py
+-rw-r--r--   0 james      (501) staff       (20)     8457 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_multiprocessing.py
+-rw-r--r--   0 james      (501) staff       (20)    45227 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_optimization.py
+-rw-r--r--   0 james      (501) staff       (20)    28229 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_order.py
+-rw-r--r--   0 james      (501) staff       (20)     4684 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_rewrite.py
+-rw-r--r--   0 james      (501) staff       (20)     7518 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_sizeof.py
+-rw-r--r--   0 james      (501) staff       (20)     7154 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_spark_compat.py
+-rw-r--r--   0 james      (501) staff       (20)     1397 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_system.py
+-rw-r--r--   0 james      (501) staff       (20)     4749 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_threaded.py
+-rw-r--r--   0 james      (501) staff       (20)     5670 2023-04-25 18:34:46.000000 dask-2023.6.0/dask/tests/test_typing.py
+-rw-r--r--   0 james      (501) staff       (20)    22705 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_utils.py
+-rw-r--r--   0 james      (501) staff       (20)     1598 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/test_utils_test.py
+-rw-r--r--   0 james      (501) staff       (20)      211 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/tests/warning_aliases.py
+-rw-r--r--   0 james      (501) staff       (20)     2993 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/threaded.py
+-rw-r--r--   0 james      (501) staff       (20)    14538 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/typing.py
+-rw-r--r--   0 james      (501) staff       (20)    56051 2023-05-24 15:39:04.000000 dask-2023.6.0/dask/utils.py
+-rw-r--r--   0 james      (501) staff       (20)     4825 2023-04-11 17:13:14.000000 dask-2023.6.0/dask/utils_test.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.992306 dask-2023.6.0/dask/widgets/
+-rw-r--r--   0 james      (501) staff       (20)      792 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/widgets/__init__.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.998932 dask-2023.6.0/dask/widgets/templates/
+-rw-r--r--   0 james      (501) staff       (20)     1295 2023-03-13 17:40:25.000000 dask-2023.6.0/dask/widgets/templates/array.html.j2
+-rw-r--r--   0 james      (501) staff       (20)      124 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/widgets/templates/dataframe.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     2579 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/widgets/templates/highlevelgraph.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1981 2022-11-09 22:20:24.000000 dask-2023.6.0/dask/widgets/templates/highlevelgraph_layer.html.j2
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.000053 dask-2023.6.0/dask/widgets/tests/
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.008194 dask-2023.6.0/dask/widgets/tests/templates/
+-rw-r--r--   0 james      (501) staff       (20)       38 2022-10-24 20:44:15.000000 dask-2023.6.0/dask/widgets/tests/templates/bytes.html.j2
+-rw-r--r--   0 james      (501) staff       (20)       39 2022-10-24 20:44:15.000000 dask-2023.6.0/dask/widgets/tests/templates/custom_filter.html.j2
+-rw-r--r--   0 james      (501) staff       (20)       30 2022-10-24 20:44:15.000000 dask-2023.6.0/dask/widgets/tests/templates/example.html.j2
+-rw-r--r--   0 james      (501) staff       (20)     1401 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/widgets/tests/test_widgets.py
+-rw-r--r--   0 james      (501) staff       (20)     1120 2023-05-31 15:34:32.000000 dask-2023.6.0/dask/widgets/widgets.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:12.879917 dask-2023.6.0/dask.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2532 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)    13939 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)      124 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/entry_points.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/not-zip-safe
+-rw-r--r--   0 james      (501) staff       (20)      454 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)        5 2023-06-09 16:34:12.000000 dask-2023.6.0/dask.egg-info/top_level.txt
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.013377 dask-2023.6.0/docs/
+-rw-r--r--   0 james      (501) staff       (20)     5741 2023-03-22 19:03:53.000000 dask-2023.6.0/docs/Makefile
+-rw-r--r--   0 james      (501) staff       (20)     5186 2022-08-08 20:45:08.000000 dask-2023.6.0/docs/make.bat
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.195237 dask-2023.6.0/docs/source/
+-rw-r--r--   0 james      (501) staff       (20)    17598 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/10-minutes-to-dask.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.212434 dask-2023.6.0/docs/source/_static/
+-rw-r--r--   0 james      (501) staff       (20)    10187 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/_static/config_converter.js
+-rw-r--r--   0 james      (501) staff       (20)    11021 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/_static/dask-simple.png
+-rw-r--r--   0 james      (501) staff       (20)     2375 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/_static/main-page.css
+-rw-r--r--   0 james      (501) staff       (20)    15598 2022-08-08 20:45:08.000000 dask-2023.6.0/docs/source/_static/profile.html
+-rw-r--r--   0 james      (501) staff       (20)    65304 2022-08-08 20:45:08.000000 dask-2023.6.0/docs/source/_static/stacked_profile.html
+-rw-r--r--   0 james      (501) staff       (20)      523 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/_static/style.css
+-rw-r--r--   0 james      (501) staff       (20)      365 2021-06-16 20:41:28.000000 dask-2023.6.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 james      (501) staff       (20)   292662 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/_static/transpose_cyto.html
+-rw-r--r--   0 james      (501) staff       (20)    49423 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/_static/yaml.min.js
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.213730 dask-2023.6.0/docs/source/_templates/
+-rw-r--r--   0 james      (501) staff       (20)      180 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/_templates/layout.html
+-rw-r--r--   0 james      (501) staff       (20)     2235 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/api.rst
+-rw-r--r--   0 james      (501) staff       (20)     6968 2023-05-24 15:39:04.000000 dask-2023.6.0/docs/source/array-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     2943 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/array-assignment.rst
+-rw-r--r--   0 james      (501) staff       (20)     4740 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/array-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)    13035 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array-chunks.rst
+-rw-r--r--   0 james      (501) staff       (20)    18437 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array-creation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5885 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array-design.rst
+-rw-r--r--   0 james      (501) staff       (20)     2857 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array-gufunc.rst
+-rw-r--r--   0 james      (501) staff       (20)     6069 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/array-overlap.rst
+-rw-r--r--   0 james      (501) staff       (20)     3924 2023-05-19 15:53:47.000000 dask-2023.6.0/docs/source/array-random.rst
+-rw-r--r--   0 james      (501) staff       (20)     4137 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/array-slicing.rst
+-rw-r--r--   0 james      (501) staff       (20)     3291 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array-sparse.rst
+-rw-r--r--   0 james      (501) staff       (20)     2018 2022-10-07 21:37:36.000000 dask-2023.6.0/docs/source/array-stack.rst
+-rw-r--r--   0 james      (501) staff       (20)     1140 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array-stats.rst
+-rw-r--r--   0 james      (501) staff       (20)     4121 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/array.rst
+-rw-r--r--   0 james      (501) staff       (20)     1574 2022-08-08 20:45:08.000000 dask-2023.6.0/docs/source/bag-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     4557 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/bag-creation.rst
+-rw-r--r--   0 james      (501) staff       (20)     4068 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/bag.rst
+-rw-r--r--   0 james      (501) staff       (20)    14050 2023-05-22 17:52:26.000000 dask-2023.6.0/docs/source/best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     5553 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/caching.rst
+-rw-r--r--   0 james      (501) staff       (20)   305883 2023-06-09 16:25:33.000000 dask-2023.6.0/docs/source/changelog.rst
+-rw-r--r--   0 james      (501) staff       (20)      211 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/cheatsheet.rst
+-rw-r--r--   0 james      (501) staff       (20)     4047 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/cli.rst
+-rw-r--r--   0 james      (501) staff       (20)    15465 2023-03-13 20:41:19.000000 dask-2023.6.0/docs/source/conf.py
+-rw-r--r--   0 james      (501) staff       (20)    16654 2023-04-06 21:35:01.000000 dask-2023.6.0/docs/source/configuration.rst
+-rw-r--r--   0 james      (501) staff       (20)    18651 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/custom-collections.rst
+-rw-r--r--   0 james      (501) staff       (20)     3604 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/custom-graphs.rst
+-rw-r--r--   0 james      (501) staff       (20)      932 2023-05-31 15:34:32.000000 dask-2023.6.0/docs/source/dashboard-progress-script.py
+-rw-r--r--   0 james      (501) staff       (20)    15045 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/dashboard.rst
+-rw-r--r--   0 james      (501) staff       (20)   203552 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/daskcheatsheet.pdf
+-rw-r--r--   0 james      (501) staff       (20)    13693 2023-05-19 15:53:47.000000 dask-2023.6.0/docs/source/dataframe-api.rst
+-rw-r--r--   0 james      (501) staff       (20)     9611 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/dataframe-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     3951 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/dataframe-categoricals.rst
+-rw-r--r--   0 james      (501) staff       (20)     5967 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/dataframe-create.rst
+-rw-r--r--   0 james      (501) staff       (20)     5002 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/dataframe-design.rst
+-rw-r--r--   0 james      (501) staff       (20)     6224 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/dataframe-extend.rst
+-rw-r--r--   0 james      (501) staff       (20)     8050 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/dataframe-groupby.rst
+-rw-r--r--   0 james      (501) staff       (20)     6115 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/dataframe-indexing.rst
+-rw-r--r--   0 james      (501) staff       (20)     3454 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/dataframe-joins.rst
+-rw-r--r--   0 james      (501) staff       (20)    10952 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/dataframe-parquet.rst
+-rw-r--r--   0 james      (501) staff       (20)    12661 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/dataframe-sql.rst
+-rw-r--r--   0 james      (501) staff       (20)     7772 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/dataframe.rst
+-rw-r--r--   0 james      (501) staff       (20)      363 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/debugging-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)     1696 2022-08-08 20:45:08.000000 dask-2023.6.0/docs/source/delayed-api.rst
+-rw-r--r--   0 james      (501) staff       (20)    17616 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/delayed-best-practices.rst
+-rw-r--r--   0 james      (501) staff       (20)     1497 2022-10-07 21:37:36.000000 dask-2023.6.0/docs/source/delayed-collections.rst
+-rw-r--r--   0 james      (501) staff       (20)     6357 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/delayed.rst
+-rw-r--r--   0 james      (501) staff       (20)     3620 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/deploying-cli.rst
+-rw-r--r--   0 james      (501) staff       (20)     3012 2023-05-22 17:52:26.000000 dask-2023.6.0/docs/source/deploying-cloud.rst
+-rw-r--r--   0 james      (501) staff       (20)     2868 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/deploying-docker.rst
+-rw-r--r--   0 james      (501) staff       (20)     9939 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/deploying-hpc.rst
+-rw-r--r--   0 james      (501) staff       (20)     4001 2023-05-19 15:53:47.000000 dask-2023.6.0/docs/source/deploying-kubernetes.rst
+-rw-r--r--   0 james      (501) staff       (20)     5823 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/deploying-python-advanced.rst
+-rw-r--r--   0 james      (501) staff       (20)     2839 2023-04-25 18:34:46.000000 dask-2023.6.0/docs/source/deploying-python.rst
+-rw-r--r--   0 james      (501) staff       (20)     1619 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/deploying-ssh.rst
+-rw-r--r--   0 james      (501) staff       (20)     7356 2023-06-06 17:26:06.000000 dask-2023.6.0/docs/source/deploying.rst
+-rw-r--r--   0 james      (501) staff       (20)    10873 2023-05-22 17:52:26.000000 dask-2023.6.0/docs/source/deployment-considerations.rst
+-rw-r--r--   0 james      (501) staff       (20)    13144 2023-05-31 15:34:32.000000 dask-2023.6.0/docs/source/develop.rst
+-rw-r--r--   0 james      (501) staff       (20)     4442 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/diagnostics-distributed.rst
+-rw-r--r--   0 james      (501) staff       (20)    10407 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/diagnostics-local.rst
+-rw-r--r--   0 james      (501) staff       (20)     4364 2023-05-22 17:52:26.000000 dask-2023.6.0/docs/source/ecosystem.rst
+-rw-r--r--   0 james      (501) staff       (20)    19999 2023-05-22 17:52:26.000000 dask-2023.6.0/docs/source/faq.rst
+-rw-r--r--   0 james      (501) staff       (20)    25569 2023-05-19 15:53:47.000000 dask-2023.6.0/docs/source/futures.rst
+-rw-r--r--   0 james      (501) staff       (20)     5820 2022-10-07 21:37:14.000000 dask-2023.6.0/docs/source/gpu.rst
+-rw-r--r--   0 james      (501) staff       (20)     2541 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/graph_manipulation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5433 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/graphs.rst
+-rw-r--r--   0 james      (501) staff       (20)     5399 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/graphviz.rst
+-rw-r--r--   0 james      (501) staff       (20)     6946 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/high-level-graphs.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.222336 dask-2023.6.0/docs/source/how-to/
+-rw-r--r--   0 james      (501) staff       (20)     4364 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/how-to/adaptive.rst
+-rw-r--r--   0 james      (501) staff       (20)    15360 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/how-to/connect-to-remote-data.rst
+-rw-r--r--   0 james      (501) staff       (20)     4209 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/how-to/customize-initialization.rst
+-rw-r--r--   0 james      (501) staff       (20)    10859 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/how-to/debug.rst
+-rw-r--r--   0 james      (501) staff       (20)     1722 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/how-to/extend-sizeof.rst
+-rw-r--r--   0 james      (501) staff       (20)      433 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/how-to/index.rst
+-rw-r--r--   0 james      (501) staff       (20)     4562 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/how-to/manage-environments.rst
+-rw-r--r--   0 james      (501) staff       (20)     6680 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/how-to/selecting-the-collection-backend.rst
+-rw-r--r--   0 james      (501) staff       (20)      902 2023-04-25 18:34:46.000000 dask-2023.6.0/docs/source/how-to/setup-prometheus.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.356478 dask-2023.6.0/docs/source/images/
+-rw-r--r--   0 james      (501) staff       (20)    99565 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/10_minutes_array_graph.png
+-rw-r--r--   0 james      (501) staff       (20)    22442 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/10_minutes_bag_graph.png
+-rw-r--r--   0 james      (501) staff       (20)    56229 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/10_minutes_dataframe_graph.png
+-rw-r--r--   0 james      (501) staff       (20)     4059 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/HHMI_Janelia_Color.png
+-rw-r--r--   0 james      (501) staff       (20)    18406 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/array.svg
+-rw-r--r--   0 james      (501) staff       (20)  1620104 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/async-embarrassing.gif
+-rw-r--r--   0 james      (501) staff       (20)    10752 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/concurrent-futures-threaded.webp
+-rw-r--r--   0 james      (501) staff       (20)   135129 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/crosstalk.svg
+-rw-r--r--   0 james      (501) staff       (20)  2367087 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dashboard_jupyterlab.png
+-rw-r--r--   0 james      (501) staff       (20)    37971 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dashboard_link.png
+-rw-r--r--   0 james      (501) staff       (20)    68712 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dashboard_memory.png
+-rw-r--r--   0 james      (501) staff       (20)   281018 2023-04-25 18:34:46.000000 dask-2023.6.0/docs/source/images/dashboard_memory_new.gif
+-rw-r--r--   0 james      (501) staff       (20)    25435 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/images/dashboard_progress.png
+-rw-r--r--   0 james      (501) staff       (20)   276928 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/images/dashboard_status.png
+-rw-r--r--   0 james      (501) staff       (20)    12009 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/images/dashboard_task_processing.png
+-rw-r--r--   0 james      (501) staff       (20)    58238 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dashboard_task_stream_unhealthy.png
+-rw-r--r--   0 james      (501) staff       (20)   103654 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dashboard_taskstream_healthy.png
+-rw-r--r--   0 james      (501) staff       (20)   112822 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/dask-adaptive.svg
+-rw-r--r--   0 james      (501) staff       (20)    14645 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/dask-array.svg
+-rw-r--r--   0 james      (501) staff       (20)   222084 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/dask-cluster-manager.svg
+-rw-r--r--   0 james      (501) staff       (20)    18782 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/dask-dataframe.svg
+-rw-r--r--   0 james      (501) staff       (20)   381903 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask-overview-distributed-callout.svg
+-rw-r--r--   0 james      (501) staff       (20)   357643 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask-overview-schedulers.svg
+-rw-r--r--   0 james      (501) staff       (20)    97471 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/dask-overview.svg
+-rw-r--r--   0 james      (501) staff       (20)     3022 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_horizontal.svg
+-rw-r--r--   0 james      (501) staff       (20)     3651 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_horizontal_black.svg
+-rw-r--r--   0 james      (501) staff       (20)     3767 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_horizontal_on_blue.svg
+-rw-r--r--   0 james      (501) staff       (20)     3738 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_horizontal_on_pink.svg
+-rw-r--r--   0 james      (501) staff       (20)     3738 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_horizontal_white.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_icon.svg
+-rw-r--r--   0 james      (501) staff       (20)     1571 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_icon_black.svg
+-rw-r--r--   0 james      (501) staff       (20)     1607 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_icon_on_pink.svg
+-rw-r--r--   0 james      (501) staff       (20)     1609 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/dask_icon_white.svg
+-rw-r--r--   0 james      (501) staff       (20)    20216 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/delayed-inc-double-add.svg
+-rw-r--r--   0 james      (501) staff       (20)   104628 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/distributed-overview.svg
+-rw-r--r--   0 james      (501) staff       (20)    18297 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/frame-shuffle.svg
+-rw-r--r--   0 james      (501) staff       (20)    22979 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/frame-sort.svg
+-rw-r--r--   0 james      (501) staff       (20)    12181 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/frame.svg
+-rw-r--r--   0 james      (501) staff       (20)    41828 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/gputester-msg.png
+-rw-r--r--   0 james      (501) staff       (20)   210392 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/growth_of_languages.png
+-rw-r--r--   0 james      (501) staff       (20)   167834 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/growth_of_libraries.png
+-rw-r--r--   0 james      (501) staff       (20)     4097 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/inc-add.svg
+-rw-r--r--   0 james      (501) staff       (20)   123010 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/map-reduce-task-scheduling.svg
+-rw-r--r--   0 james      (501) staff       (20)   482302 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/map_blocks_drop_axis.png
+-rw-r--r--   0 james      (501) staff       (20)   113067 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/merge_chunks.png
+-rw-r--r--   0 james      (501) staff       (20)    63244 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/merge_chunks_false.png
+-rw-r--r--   0 james      (501) staff       (20)    13024 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/optimize_dask1.svg
+-rw-r--r--   0 james      (501) staff       (20)     8803 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/optimize_dask2.svg
+-rw-r--r--   0 james      (501) staff       (20)     5198 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/optimize_dask3.svg
+-rw-r--r--   0 james      (501) staff       (20)     4104 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/optimize_dask4.svg
+-rw-r--r--   0 james      (501) staff       (20)     2738 2021-11-11 17:33:01.000000 dask-2023.6.0/docs/source/images/optimize_dask5.svg
+-rw-r--r--   0 james      (501) staff       (20)   292827 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/order-failure.png
+-rw-r--r--   0 james      (501) staff       (20)   239828 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/order-success.png
+-rw-r--r--   0 james      (501) staff       (20)    40833 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/overlap.svg
+-rw-r--r--   0 james      (501) staff       (20)    18785 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/overlapping-blocks.svg
+-rw-r--r--   0 james      (501) staff       (20)     4537 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/overlapping-neighbors.svg
+-rw-r--r--   0 james      (501) staff       (20)    20533 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/pipeline.svg
+-rw-r--r--   0 james      (501) staff       (20)    31576 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/reshape.png
+-rw-r--r--   0 james      (501) staff       (20)    31410 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/reshape_problem.png
+-rw-r--r--   0 james      (501) staff       (20)    33288 2021-11-11 20:27:17.000000 dask-2023.6.0/docs/source/images/reshape_rechunked.png
+-rw-r--r--   0 james      (501) staff       (20)    50209 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/scaling-edges.png
+-rw-r--r--   0 james      (501) staff       (20)    68476 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/scaling-nodes.png
+-rw-r--r--   0 james      (501) staff       (20)    21294 2021-06-08 02:50:31.000000 dask-2023.6.0/docs/source/images/simple-dask.png
+-rw-r--r--   0 james      (501) staff       (20)    27572 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/transpose-hlg-hovertooltip.png
+-rw-r--r--   0 james      (501) staff       (20)    84492 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/images/transpose-hlg-html-repr.png
+-rw-r--r--   0 james      (501) staff       (20)    39365 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/transpose.svg
+-rw-r--r--   0 james      (501) staff       (20)    22446 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/transpose_opt.svg
+-rw-r--r--   0 james      (501) staff       (20)   115022 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/images/trivial.svg
+-rw-r--r--   0 james      (501) staff       (20)     2451 2021-06-08 02:51:08.000000 dask-2023.6.0/docs/source/images/unoverlapping-neighbors.svg
+-rw-r--r--   0 james      (501) staff       (20)     6237 2023-03-13 17:40:25.000000 dask-2023.6.0/docs/source/index.rst
+-rw-r--r--   0 james      (501) staff       (20)    15235 2023-05-31 15:34:32.000000 dask-2023.6.0/docs/source/install.rst
+-rw-r--r--   0 james      (501) staff       (20)      341 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/internals.rst
+-rw-r--r--   0 james      (501) staff       (20)      868 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/logos.rst
+-rw-r--r--   0 james      (501) staff       (20)     3573 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/maintainers.rst
+-rw-r--r--   0 james      (501) staff       (20)    12200 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/optimize.rst
+-rw-r--r--   0 james      (501) staff       (20)     7119 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/order.rst
+-rw-r--r--   0 james      (501) staff       (20)     4810 2022-10-07 21:37:14.000000 dask-2023.6.0/docs/source/phases-of-computation.rst
+-rw-r--r--   0 james      (501) staff       (20)     5089 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/presentations.rst
+-rw-r--r--   0 james      (501) staff       (20)     6010 2022-10-07 21:37:14.000000 dask-2023.6.0/docs/source/scheduler-overview.rst
+-rw-r--r--   0 james      (501) staff       (20)     4493 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/scheduling-policy.rst
+-rw-r--r--   0 james      (501) staff       (20)    11015 2023-05-31 15:34:32.000000 dask-2023.6.0/docs/source/scheduling.rst
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-09 16:34:13.357454 dask-2023.6.0/docs/source/scripts/
+-rw-r--r--   0 james      (501) staff       (20)     3294 2023-05-31 15:34:32.000000 dask-2023.6.0/docs/source/scripts/scheduling.py
+-rw-r--r--   0 james      (501) staff       (20)     6104 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/shared.rst
+-rw-r--r--   0 james      (501) staff       (20)     9342 2022-11-09 22:20:24.000000 dask-2023.6.0/docs/source/spark.rst
+-rw-r--r--   0 james      (501) staff       (20)     3966 2022-10-07 21:37:14.000000 dask-2023.6.0/docs/source/spec.rst
+-rw-r--r--   0 james      (501) staff       (20)     4754 2023-05-22 17:52:26.000000 dask-2023.6.0/docs/source/support.rst
+-rw-r--r--   0 james      (501) staff       (20)     1831 2021-06-16 20:41:28.000000 dask-2023.6.0/docs/source/understanding-performance.rst
+-rw-r--r--   0 james      (501) staff       (20)    12205 2023-05-03 18:02:08.000000 dask-2023.6.0/docs/source/user-interfaces.rst
+-rw-r--r--   0 james      (501) staff       (20)    11744 2022-10-24 20:44:15.000000 dask-2023.6.0/docs/source/why.rst
+-rw-r--r--   0 james      (501) staff       (20)     5526 2023-06-09 16:15:33.000000 dask-2023.6.0/pyproject.toml
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-09 16:34:13.359097 dask-2023.6.0/setup.cfg
+-rwxr-xr-x   0 james      (501) staff       (20)      194 2023-05-03 18:02:08.000000 dask-2023.6.0/setup.py
```

### Comparing `dask-2023.5.1/LICENSE.txt` & `dask-2023.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/PKG-INFO` & `dask-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask
-Version: 2023.5.1
+Version: 2023.6.0
 Summary: Parallel PyData with Task Scheduling
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Homepage, https://github.com/dask/dask/
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-2023.5.1/README.rst` & `dask-2023.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/conftest.py` & `dask-2023.6.0/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/_compatibility.py` & `dask-2023.6.0/dask/_compatibility.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/NUMPY_LICENSE.txt` & `dask-2023.6.0/dask/array/NUMPY_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/__init__.py` & `dask-2023.6.0/dask/array/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/backends.py` & `dask-2023.6.0/dask/array/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/blockwise.py` & `dask-2023.6.0/dask/array/blockwise.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/chunk.py` & `dask-2023.6.0/dask/array/chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/chunk_types.py` & `dask-2023.6.0/dask/array/chunk_types.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/core.py` & `dask-2023.6.0/dask/array/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/creation.py` & `dask-2023.6.0/dask/array/creation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/cupy_entry_point.py` & `dask-2023.6.0/dask/array/cupy_entry_point.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/dispatch.py` & `dask-2023.6.0/dask/array/dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/einsumfuncs.py` & `dask-2023.6.0/dask/array/einsumfuncs.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/fft.py` & `dask-2023.6.0/dask/array/fft.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/gufunc.py` & `dask-2023.6.0/dask/array/gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/image.py` & `dask-2023.6.0/dask/array/image.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/linalg.py` & `dask-2023.6.0/dask/array/linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/ma.py` & `dask-2023.6.0/dask/array/ma.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/numpy_compat.py` & `dask-2023.6.0/dask/array/numpy_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/optimization.py` & `dask-2023.6.0/dask/array/optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/overlap.py` & `dask-2023.6.0/dask/array/overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/percentile.py` & `dask-2023.6.0/dask/array/percentile.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/random.py` & `dask-2023.6.0/dask/array/random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/rechunk.py` & `dask-2023.6.0/dask/array/rechunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/reductions.py` & `dask-2023.6.0/dask/array/reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/reshape.py` & `dask-2023.6.0/dask/array/reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/routines.py` & `dask-2023.6.0/dask/array/routines.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/slicing.py` & `dask-2023.6.0/dask/array/slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/stats.py` & `dask-2023.6.0/dask/array/stats.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/svg.py` & `dask-2023.6.0/dask/array/svg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_array_core.py` & `dask-2023.6.0/dask/array/tests/test_array_core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_array_function.py` & `dask-2023.6.0/dask/array/tests/test_array_function.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_array_utils.py` & `dask-2023.6.0/dask/array/tests/test_array_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_atop.py` & `dask-2023.6.0/dask/array/tests/test_atop.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_chunk.py` & `dask-2023.6.0/dask/array/tests/test_chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_creation.py` & `dask-2023.6.0/dask/array/tests/test_creation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_core.py` & `dask-2023.6.0/dask/array/tests/test_cupy_core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_creation.py` & `dask-2023.6.0/dask/array/tests/test_cupy_creation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_gufunc.py` & `dask-2023.6.0/dask/array/tests/test_cupy_gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_linalg.py` & `dask-2023.6.0/dask/array/tests/test_cupy_linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_overlap.py` & `dask-2023.6.0/dask/array/tests/test_cupy_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_percentile.py` & `dask-2023.6.0/dask/array/tests/test_cupy_percentile.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_random.py` & `dask-2023.6.0/dask/array/tests/test_cupy_random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_reductions.py` & `dask-2023.6.0/dask/array/tests/test_cupy_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_routines.py` & `dask-2023.6.0/dask/array/tests/test_cupy_routines.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_slicing.py` & `dask-2023.6.0/dask/array/tests/test_cupy_slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_cupy_sparse.py` & `dask-2023.6.0/dask/array/tests/test_cupy_sparse.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_dispatch.py` & `dask-2023.6.0/dask/array/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_fft.py` & `dask-2023.6.0/dask/array/tests/test_fft.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_gufunc.py` & `dask-2023.6.0/dask/array/tests/test_gufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_image.py` & `dask-2023.6.0/dask/array/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_linalg.py` & `dask-2023.6.0/dask/array/tests/test_linalg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_masked.py` & `dask-2023.6.0/dask/array/tests/test_masked.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_numpy_compat.py` & `dask-2023.6.0/dask/array/tests/test_numpy_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_optimization.py` & `dask-2023.6.0/dask/array/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_overlap.py` & `dask-2023.6.0/dask/array/tests/test_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_percentiles.py` & `dask-2023.6.0/dask/array/tests/test_percentiles.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_random.py` & `dask-2023.6.0/dask/array/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_rechunk.py` & `dask-2023.6.0/dask/array/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_reductions.py` & `dask-2023.6.0/dask/array/tests/test_reductions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_reshape.py` & `dask-2023.6.0/dask/array/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_routines.py` & `dask-2023.6.0/dask/array/tests/test_routines.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_slicing.py` & `dask-2023.6.0/dask/array/tests/test_slicing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_sparse.py` & `dask-2023.6.0/dask/array/tests/test_sparse.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_stats.py` & `dask-2023.6.0/dask/array/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_svg.py` & `dask-2023.6.0/dask/array/tests/test_svg.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_testing.py` & `dask-2023.6.0/dask/array/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_ufunc.py` & `dask-2023.6.0/dask/array/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_wrap.py` & `dask-2023.6.0/dask/array/tests/test_wrap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tests/test_xarray.py` & `dask-2023.6.0/dask/array/tests/test_xarray.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/tiledb_io.py` & `dask-2023.6.0/dask/array/tiledb_io.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/ufunc.py` & `dask-2023.6.0/dask/array/ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/utils.py` & `dask-2023.6.0/dask/array/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/array/wrap.py` & `dask-2023.6.0/dask/array/wrap.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/backends.py` & `dask-2023.6.0/dask/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/__init__.py` & `dask-2023.6.0/dask/bag/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/avro.py` & `dask-2023.6.0/dask/bag/avro.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/chunk.py` & `dask-2023.6.0/dask/bag/chunk.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/core.py` & `dask-2023.6.0/dask/bag/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/random.py` & `dask-2023.6.0/dask/bag/random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/tests/test_avro.py` & `dask-2023.6.0/dask/bag/tests/test_avro.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/tests/test_bag.py` & `dask-2023.6.0/dask/bag/tests/test_bag.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/tests/test_random.py` & `dask-2023.6.0/dask/bag/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/tests/test_text.py` & `dask-2023.6.0/dask/bag/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bag/text.py` & `dask-2023.6.0/dask/bag/text.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/base.py` & `dask-2023.6.0/dask/base.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/blockwise.py` & `dask-2023.6.0/dask/blockwise.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bytes/core.py` & `dask-2023.6.0/dask/bytes/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bytes/tests/test_bytes_utils.py` & `dask-2023.6.0/dask/bytes/tests/test_bytes_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bytes/tests/test_compression.py` & `dask-2023.6.0/dask/bytes/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bytes/tests/test_http.py` & `dask-2023.6.0/dask/bytes/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bytes/tests/test_local.py` & `dask-2023.6.0/dask/bytes/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/bytes/tests/test_s3.py` & `dask-2023.6.0/dask/bytes/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/cache.py` & `dask-2023.6.0/dask/cache.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/callbacks.py` & `dask-2023.6.0/dask/callbacks.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/cli.py` & `dask-2023.6.0/dask/cli.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/compatibility.py` & `dask-2023.6.0/dask/compatibility.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/config.py` & `dask-2023.6.0/dask/config.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/context.py` & `dask-2023.6.0/dask/context.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/core.py` & `dask-2023.6.0/dask/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dask-schema.yaml` & `dask-2023.6.0/dask/dask-schema.yaml`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dask.yaml` & `dask-2023.6.0/dask/dask.yaml`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/__init__.py` & `dask-2023.6.0/dask/dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/_compat.py` & `dask-2023.6.0/dask/dataframe/_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/_dtypes.py` & `dask-2023.6.0/dask/dataframe/_dtypes.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/_pyarrow.py` & `dask-2023.6.0/dask/dataframe/_pyarrow.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/_pyarrow_compat.py` & `dask-2023.6.0/dask/dataframe/_pyarrow_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/accessor.py` & `dask-2023.6.0/dask/dataframe/accessor.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/backends.py` & `dask-2023.6.0/dask/dataframe/backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/categorical.py` & `dask-2023.6.0/dask/dataframe/categorical.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/core.py` & `dask-2023.6.0/dask/dataframe/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/dispatch.py` & `dask-2023.6.0/dask/dataframe/dispatch.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/extensions.py` & `dask-2023.6.0/dask/dataframe/extensions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/groupby.py` & `dask-2023.6.0/dask/dataframe/groupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -3118,18 +3118,20 @@
     else:
         return x.value_counts(**kwargs)
 
 
 def _value_counts_aggregate(series_gb):
     data = {k: v.groupby(level=-1).sum() for k, v in series_gb}
     res = pd.concat(data, names=series_gb.obj.index.names)
-    levels = {i: level for i, level in enumerate(series_gb.obj.index.levels)}
-    # verify_integrity=False to preserve index codes
+    typed_levels = {
+        i: res.index.levels[i].astype(series_gb.obj.index.levels[i].dtype)
+        for i in range(len(res.index.levels))
+    }
     res.index = res.index.set_levels(
-        levels.values(), level=levels.keys(), verify_integrity=False
+        typed_levels.values(), level=typed_levels.keys(), verify_integrity=False
     )
     return res
 
 
 def _tail_chunk(series_gb, **kwargs):
     keys, groups = zip(*series_gb) if len(series_gb) else ((True,), (series_gb,))
     return pd.concat([group.tail(**kwargs) for group in groups], keys=keys)
```

### Comparing `dask-2023.5.1/dask/dataframe/hyperloglog.py` & `dask-2023.6.0/dask/dataframe/hyperloglog.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/indexing.py` & `dask-2023.6.0/dask/dataframe/indexing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/__init__.py` & `dask-2023.6.0/dask/dataframe/io/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/csv.py` & `dask-2023.6.0/dask/dataframe/io/csv.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/demo.py` & `dask-2023.6.0/dask/dataframe/io/demo.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/hdf.py` & `dask-2023.6.0/dask/dataframe/io/hdf.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/io.py` & `dask-2023.6.0/dask/dataframe/io/io.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/json.py` & `dask-2023.6.0/dask/dataframe/io/json.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/orc/arrow.py` & `dask-2023.6.0/dask/dataframe/io/orc/arrow.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/orc/core.py` & `dask-2023.6.0/dask/dataframe/io/orc/core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/parquet/arrow.py` & `dask-2023.6.0/dask/dataframe/io/parquet/arrow.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/parquet/core.py` & `dask-2023.6.0/dask/dataframe/io/parquet/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1343,17 +1343,39 @@
         Note that the "fastparquet" engine does not currently support DNF for
         the filtering of partitioned columns (List[Tuple] is required).
     Returns
     -------
     parts, statistics: the same as the input, but possibly a subset
     """
 
+    # Supported predicate operators
+    _supported_operators = {
+        "=",
+        "==",
+        "!=",
+        "<",
+        "<=",
+        ">",
+        ">=",
+        "is",
+        "is not",
+        "in",
+        "not in",
+    }
+
     def apply_conjunction(parts, statistics, conjunction):
         for column, operator, value in conjunction:
-            if operator == "in" and not isinstance(value, (list, set, tuple)):
+            if operator not in _supported_operators:
+                # Use same error message as `_filters_to_expression`
+                raise ValueError(
+                    f'"{(column, operator, value)}" is not a valid operator in predicates.'
+                )
+            elif operator in ("in", "not in") and not isinstance(
+                value, (list, set, tuple)
+            ):
                 raise TypeError("Value of 'in' filter must be a list, set, or tuple.")
             out_parts = []
             out_statistics = []
             for part, stats in zip(parts, statistics):
                 if "filter" in stats and stats["filter"]:
                     continue  # Filtered by engine
                 try:
@@ -1390,14 +1412,16 @@
                         and min <= value
                         or operator == ">"
                         and max > value
                         or operator == ">="
                         and max >= value
                         or operator == "in"
                         and any(min <= item <= max for item in value)
+                        or operator == "not in"
+                        and not any(min == max == item for item in value)
                     ):
                         out_parts.append(part)
                         out_statistics.append(stats)
 
             parts, statistics = out_parts, out_statistics
 
         return parts, statistics
```

### Comparing `dask-2023.5.1/dask/dataframe/io/parquet/fastparquet.py` & `dask-2023.6.0/dask/dataframe/io/parquet/fastparquet.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/parquet/utils.py` & `dask-2023.6.0/dask/dataframe/io/parquet/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/sql.py` & `dask-2023.6.0/dask/dataframe/io/sql.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_csv.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_csv.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_demo.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_demo.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_hdf.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_hdf.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_io.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_json.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_orc.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_orc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_parquet.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_parquet.py`

 * *Files 0% similar despite different names*

```diff
@@ -4535,14 +4535,30 @@
     path = tmp_path / "in_predicate_iterable_dask.parquet"
     ddf.to_parquet(path, engine=engine)
     result = dd.read_parquet(path, engine=engine, filters=filters)
     expected = pd.read_parquet(path, engine=engine, filters=filters)
     assert_eq(result, expected, check_index=False)
 
 
+def test_not_in_predicate(tmp_path, engine):
+    ddf = dd.from_dict(
+        {"A": range(8), "B": [1, 1, 2, 2, 3, 3, 4, 4]},
+        npartitions=4,
+    )
+    ddf.to_parquet(tmp_path, engine=engine)
+    filters = [[("B", "not in", (1, 2))]]
+    result = dd.read_parquet(tmp_path, engine=engine, filters=filters)
+    expected = pd.read_parquet(tmp_path, engine=engine, filters=filters)
+    assert_eq(result, expected, check_index=False)
+
+    with pytest.raises(ValueError, match="not a valid operator in predicates"):
+        unsupported_op = [[("B", "not eq", 1)]]
+        dd.read_parquet(tmp_path, engine=engine, filters=unsupported_op)
+
+
 # Non-iterable filter value with `in` predicate
 # Test single nested and double nested lists of filters, as well as having multiple
 # filters to test against.
 @pytest.mark.parametrize(
     "filter_value",
     (
         [("B", "in", 10)],
```

### Comparing `dask-2023.5.1/dask/dataframe/io/tests/test_sql.py` & `dask-2023.6.0/dask/dataframe/io/tests/test_sql.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/io/utils.py` & `dask-2023.6.0/dask/dataframe/io/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/methods.py` & `dask-2023.6.0/dask/dataframe/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -262,15 +262,15 @@
         nunique, count, top_freq, min_ts, max_ts = stats
 
     # input was empty dataframe/series
     if len(top_freq) == 0:
         data = [0, 0]
         index = ["count", "unique"]
         dtype = None
-        data.extend([None, None])
+        data.extend([np.nan, np.nan])
         index.extend(["top", "freq"])
         dtype = object
         result = pd.Series(data, index=index, dtype=dtype, name=name)
         return result
 
     top = top_freq.index[0]
     freq = top_freq.iloc[0]
```

### Comparing `dask-2023.5.1/dask/dataframe/multi.py` & `dask-2023.6.0/dask/dataframe/multi.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/numeric.py` & `dask-2023.6.0/dask/dataframe/numeric.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/optimize.py` & `dask-2023.6.0/dask/dataframe/optimize.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/partitionquantiles.py` & `dask-2023.6.0/dask/dataframe/partitionquantiles.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/reshape.py` & `dask-2023.6.0/dask/dataframe/reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/rolling.py` & `dask-2023.6.0/dask/dataframe/rolling.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/shuffle.py` & `dask-2023.6.0/dask/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_accessors.py` & `dask-2023.6.0/dask/dataframe/tests/test_accessors.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_arithmetics_reduction.py` & `dask-2023.6.0/dask/dataframe/tests/test_arithmetics_reduction.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_boolean.py` & `dask-2023.6.0/dask/dataframe/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_categorical.py` & `dask-2023.6.0/dask/dataframe/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_dataframe.py` & `dask-2023.6.0/dask/dataframe/tests/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_extensions.py` & `dask-2023.6.0/dask/dataframe/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_format.py` & `dask-2023.6.0/dask/dataframe/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_groupby.py` & `dask-2023.6.0/dask/dataframe/tests/test_groupby.py`

 * *Files 1% similar despite different names*

```diff
@@ -2546,14 +2546,28 @@
     ddf = dd.from_pandas(df, npartitions=2)
 
     pd_gb = df.groupby(by).baz.value_counts()
     dd_gb = ddf.groupby(by).baz.value_counts()
     assert_eq(dd_gb, pd_gb)
 
 
+def test_groupby_value_counts_10322():
+    """Repro case for https://github.com/dask/dask/issues/10322."""
+    df = pd.DataFrame(
+        {
+            "x": [10] * 5 + [6] * 5 + [3] * 5,
+            "y": [1] * 3 + [2] * 3 + [4] * 3 + [5] * 3 + [2] * 3,
+        }
+    )
+    counts = df.groupby("x")["y"].value_counts()
+    ddf = dd.from_pandas(df, npartitions=3)
+    dcounts = ddf.groupby("x")["y"].value_counts()
+    assert_eq(counts, dcounts)
+
+
 @contextlib.contextmanager
 def groupby_axis_and_meta():
     # Because we're checking for multiple warnings, we need to record
     # all warnings and inspect them after the fact
     with pytest.warns() as record:
         yield
     assert len(record) == 2 if PANDAS_GT_210 else 1, [x.message for x in record.list]
```

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_hashing.py` & `dask-2023.6.0/dask/dataframe/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_hyperloglog.py` & `dask-2023.6.0/dask/dataframe/tests/test_hyperloglog.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_indexing.py` & `dask-2023.6.0/dask/dataframe/tests/test_indexing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_merge_column_and_index.py` & `dask-2023.6.0/dask/dataframe/tests/test_merge_column_and_index.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_multi.py` & `dask-2023.6.0/dask/dataframe/tests/test_multi.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_numeric.py` & `dask-2023.6.0/dask/dataframe/tests/test_numeric.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_optimize_dataframe.py` & `dask-2023.6.0/dask/dataframe/tests/test_optimize_dataframe.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_pyarrow.py` & `dask-2023.6.0/dask/dataframe/tests/test_pyarrow.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_pyarrow_compat.py` & `dask-2023.6.0/dask/dataframe/tests/test_pyarrow_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_reshape.py` & `dask-2023.6.0/dask/dataframe/tests/test_reshape.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_rolling.py` & `dask-2023.6.0/dask/dataframe/tests/test_rolling.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_shuffle.py` & `dask-2023.6.0/dask/dataframe/tests/test_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_ufunc.py` & `dask-2023.6.0/dask/dataframe/tests/test_ufunc.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tests/test_utils_dataframe.py` & `dask-2023.6.0/dask/dataframe/tests/test_utils_dataframe.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tseries/resample.py` & `dask-2023.6.0/dask/dataframe/tseries/resample.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/tseries/tests/test_resample.py` & `dask-2023.6.0/dask/dataframe/tseries/tests/test_resample.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dataframe/utils.py` & `dask-2023.6.0/dask/dataframe/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/datasets.py` & `dask-2023.6.0/dask/datasets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/delayed.py` & `dask-2023.6.0/dask/delayed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/diagnostics/profile.py` & `dask-2023.6.0/dask/diagnostics/profile.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/diagnostics/profile_visualize.py` & `dask-2023.6.0/dask/diagnostics/profile_visualize.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/diagnostics/progress.py` & `dask-2023.6.0/dask/diagnostics/progress.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/diagnostics/tests/test_profiler.py` & `dask-2023.6.0/dask/diagnostics/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/diagnostics/tests/test_progress.py` & `dask-2023.6.0/dask/diagnostics/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/distributed.py` & `dask-2023.6.0/dask/distributed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/dot.py` & `dask-2023.6.0/dask/dot.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/graph_manipulation.py` & `dask-2023.6.0/dask/graph_manipulation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/hashing.py` & `dask-2023.6.0/dask/hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/highlevelgraph.py` & `dask-2023.6.0/dask/highlevelgraph.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/layers.py` & `dask-2023.6.0/dask/layers.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/local.py` & `dask-2023.6.0/dask/local.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/multiprocessing.py` & `dask-2023.6.0/dask/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/optimization.py` & `dask-2023.6.0/dask/optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/order.py` & `dask-2023.6.0/dask/order.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/rewrite.py` & `dask-2023.6.0/dask/rewrite.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/sizeof.py` & `dask-2023.6.0/dask/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/system.py` & `dask-2023.6.0/dask/system.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_backends.py` & `dask-2023.6.0/dask/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_base.py` & `dask-2023.6.0/dask/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_cache.py` & `dask-2023.6.0/dask/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_callbacks.py` & `dask-2023.6.0/dask/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_ci.py` & `dask-2023.6.0/dask/tests/test_ci.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_cli.py` & `dask-2023.6.0/dask/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_config.py` & `dask-2023.6.0/dask/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_context.py` & `dask-2023.6.0/dask/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_core.py` & `dask-2023.6.0/dask/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_datasets.py` & `dask-2023.6.0/dask/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_delayed.py` & `dask-2023.6.0/dask/tests/test_delayed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_distributed.py` & `dask-2023.6.0/dask/tests/test_distributed.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_docs.py` & `dask-2023.6.0/dask/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_dot.py` & `dask-2023.6.0/dask/tests/test_dot.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_graph_manipulation.py` & `dask-2023.6.0/dask/tests/test_graph_manipulation.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_hashing.py` & `dask-2023.6.0/dask/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_highgraph.py` & `dask-2023.6.0/dask/tests/test_highgraph.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_layers.py` & `dask-2023.6.0/dask/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_local.py` & `dask-2023.6.0/dask/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_multiprocessing.py` & `dask-2023.6.0/dask/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_optimization.py` & `dask-2023.6.0/dask/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_order.py` & `dask-2023.6.0/dask/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_rewrite.py` & `dask-2023.6.0/dask/tests/test_rewrite.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_sizeof.py` & `dask-2023.6.0/dask/tests/test_sizeof.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_spark_compat.py` & `dask-2023.6.0/dask/tests/test_spark_compat.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_system.py` & `dask-2023.6.0/dask/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_threaded.py` & `dask-2023.6.0/dask/tests/test_threaded.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_typing.py` & `dask-2023.6.0/dask/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_utils.py` & `dask-2023.6.0/dask/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/tests/test_utils_test.py` & `dask-2023.6.0/dask/tests/test_utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/threaded.py` & `dask-2023.6.0/dask/threaded.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/typing.py` & `dask-2023.6.0/dask/typing.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/utils.py` & `dask-2023.6.0/dask/utils.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/utils_test.py` & `dask-2023.6.0/dask/utils_test.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/widgets/__init__.py` & `dask-2023.6.0/dask/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/widgets/templates/array.html.j2` & `dask-2023.6.0/dask/widgets/templates/array.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/widgets/templates/highlevelgraph.html.j2` & `dask-2023.6.0/dask/widgets/templates/highlevelgraph.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/widgets/templates/highlevelgraph_layer.html.j2` & `dask-2023.6.0/dask/widgets/templates/highlevelgraph_layer.html.j2`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/widgets/tests/test_widgets.py` & `dask-2023.6.0/dask/widgets/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask/widgets/widgets.py` & `dask-2023.6.0/dask/widgets/widgets.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/dask.egg-info/PKG-INFO` & `dask-2023.6.0/dask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask
-Version: 2023.5.1
+Version: 2023.6.0
 Summary: Parallel PyData with Task Scheduling
 Maintainer-email: Matthew Rocklin <mrocklin@gmail.com>
 License: BSD
 Project-URL: Homepage, https://github.com/dask/dask/
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `dask-2023.5.1/dask.egg-info/SOURCES.txt` & `dask-2023.6.0/dask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/Makefile` & `dask-2023.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/make.bat` & `dask-2023.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/10-minutes-to-dask.rst` & `dask-2023.6.0/docs/source/10-minutes-to-dask.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/config_converter.js` & `dask-2023.6.0/docs/source/_static/config_converter.js`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/dask-simple.png` & `dask-2023.6.0/docs/source/_static/dask-simple.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/main-page.css` & `dask-2023.6.0/docs/source/_static/main-page.css`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/profile.html` & `dask-2023.6.0/docs/source/_static/profile.html`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/stacked_profile.html` & `dask-2023.6.0/docs/source/_static/stacked_profile.html`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/style.css` & `dask-2023.6.0/docs/source/_static/style.css`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/transpose_cyto.html` & `dask-2023.6.0/docs/source/_static/transpose_cyto.html`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/_static/yaml.min.js` & `dask-2023.6.0/docs/source/_static/yaml.min.js`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/api.rst` & `dask-2023.6.0/docs/source/api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-api.rst` & `dask-2023.6.0/docs/source/array-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-assignment.rst` & `dask-2023.6.0/docs/source/array-assignment.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-best-practices.rst` & `dask-2023.6.0/docs/source/array-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-chunks.rst` & `dask-2023.6.0/docs/source/array-chunks.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-creation.rst` & `dask-2023.6.0/docs/source/array-creation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-design.rst` & `dask-2023.6.0/docs/source/array-design.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-gufunc.rst` & `dask-2023.6.0/docs/source/array-gufunc.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-overlap.rst` & `dask-2023.6.0/docs/source/array-overlap.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-random.rst` & `dask-2023.6.0/docs/source/array-random.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-slicing.rst` & `dask-2023.6.0/docs/source/array-slicing.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-sparse.rst` & `dask-2023.6.0/docs/source/array-sparse.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-stack.rst` & `dask-2023.6.0/docs/source/array-stack.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array-stats.rst` & `dask-2023.6.0/docs/source/array-stats.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/array.rst` & `dask-2023.6.0/docs/source/array.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/bag-api.rst` & `dask-2023.6.0/docs/source/bag-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/bag-creation.rst` & `dask-2023.6.0/docs/source/bag-creation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/bag.rst` & `dask-2023.6.0/docs/source/bag.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/best-practices.rst` & `dask-2023.6.0/docs/source/best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/caching.rst` & `dask-2023.6.0/docs/source/caching.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/changelog.rst` & `dask-2023.6.0/docs/source/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,37 @@
 Changelog
 =========
 
+.. _v2023.6.0:
+
+2023.6.0
+--------
+
+Released on June 9, 2023
+
+Enhancements
+^^^^^^^^^^^^
+- Add missing ``not in`` predicate support to ``read_parquet`` (:pr:`10320`) `Richard (Rick) Zamora`_
+
+Bug Fixes
+^^^^^^^^^
+- Fix for incorrect ``value_counts`` (:pr:`10323`) `Irina Truong`_
+- Update empty ``describe`` top and freq values (:pr:`10319`) `James Bourbeau`_
+
+Documentation
+^^^^^^^^^^^^^
+- Fix hetzner typo (:pr:`10332`) `Sarah Charlotte Johnson`_
+
+Maintenance
+^^^^^^^^^^^
+- Test with ``numba`` and ``sparse`` on Python 3.11 (:pr:`10329`) `Thomas Grainger`_
+- Remove ``numpy.find_common_type`` warning ignore (:pr:`10311`) `James Bourbeau`_
+- Update gpuCI ``RAPIDS_VER`` to ``23.08`` (:pr:`10310`)
+
+
 .. _v2023.5.1:
 
 2023.5.1
 --------
 
 Released on May 26, 2023
```

### Comparing `dask-2023.5.1/docs/source/cli.rst` & `dask-2023.6.0/docs/source/cli.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/conf.py` & `dask-2023.6.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/configuration.rst` & `dask-2023.6.0/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/custom-collections.rst` & `dask-2023.6.0/docs/source/custom-collections.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/custom-graphs.rst` & `dask-2023.6.0/docs/source/custom-graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dashboard-progress-script.py` & `dask-2023.6.0/docs/source/dashboard-progress-script.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dashboard.rst` & `dask-2023.6.0/docs/source/dashboard.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/daskcheatsheet.pdf` & `dask-2023.6.0/docs/source/daskcheatsheet.pdf`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-api.rst` & `dask-2023.6.0/docs/source/dataframe-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-best-practices.rst` & `dask-2023.6.0/docs/source/dataframe-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-categoricals.rst` & `dask-2023.6.0/docs/source/dataframe-categoricals.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-create.rst` & `dask-2023.6.0/docs/source/dataframe-create.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-design.rst` & `dask-2023.6.0/docs/source/dataframe-design.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-extend.rst` & `dask-2023.6.0/docs/source/dataframe-extend.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-groupby.rst` & `dask-2023.6.0/docs/source/dataframe-groupby.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-indexing.rst` & `dask-2023.6.0/docs/source/dataframe-indexing.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-joins.rst` & `dask-2023.6.0/docs/source/dataframe-joins.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-parquet.rst` & `dask-2023.6.0/docs/source/dataframe-parquet.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe-sql.rst` & `dask-2023.6.0/docs/source/dataframe-sql.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/dataframe.rst` & `dask-2023.6.0/docs/source/dataframe.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/delayed-api.rst` & `dask-2023.6.0/docs/source/delayed-api.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/delayed-best-practices.rst` & `dask-2023.6.0/docs/source/delayed-best-practices.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/delayed-collections.rst` & `dask-2023.6.0/docs/source/delayed-collections.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/delayed.rst` & `dask-2023.6.0/docs/source/delayed.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-cli.rst` & `dask-2023.6.0/docs/source/deploying-cli.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-cloud.rst` & `dask-2023.6.0/docs/source/deploying-cloud.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-docker.rst` & `dask-2023.6.0/docs/source/deploying-docker.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-hpc.rst` & `dask-2023.6.0/docs/source/deploying-hpc.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-kubernetes.rst` & `dask-2023.6.0/docs/source/deploying-kubernetes.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-python-advanced.rst` & `dask-2023.6.0/docs/source/deploying-python-advanced.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-python.rst` & `dask-2023.6.0/docs/source/deploying-python.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying-ssh.rst` & `dask-2023.6.0/docs/source/deploying-ssh.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/deploying.rst` & `dask-2023.6.0/docs/source/deploying.rst`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
 ~~~~~
 
 See :doc:`deploying-cloud` for more details.
 
 - `Dask-Yarn <https://yarn.dask.org>`_
     Deploy Dask on YARN clusters, such as are found in traditional Hadoop installations.
 - `Dask Cloud Provider <https://cloudprovider.dask.org/en/latest/>`_
-    Constructing and managing ephemeral Dask clusters on AWS, DigitalOcean, GCP, Azure, and Hertzner
+    Constructing and managing ephemeral Dask clusters on AWS, DigitalOcean, Google Cloud, Azure, and Hetzner
 - You can use `Coiled <https://coiled.io?utm_source=dask-docs&utm_medium=deploying>`_, a commercial Dask deployment option, to handle the creation and management of Dask clusters on cloud computing environments (AWS and GCP).
 
 Ad-hoc deployments
 ~~~~~~~~~~~~~~~~~~
 
 - :doc:`Manual Setup <deploying-cli>`
     The command line interface to set up ``dask-scheduler`` and ``dask-worker`` processes.
```

### Comparing `dask-2023.5.1/docs/source/deployment-considerations.rst` & `dask-2023.6.0/docs/source/deployment-considerations.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/develop.rst` & `dask-2023.6.0/docs/source/develop.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/diagnostics-distributed.rst` & `dask-2023.6.0/docs/source/diagnostics-distributed.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/diagnostics-local.rst` & `dask-2023.6.0/docs/source/diagnostics-local.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/ecosystem.rst` & `dask-2023.6.0/docs/source/ecosystem.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/faq.rst` & `dask-2023.6.0/docs/source/faq.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/futures.rst` & `dask-2023.6.0/docs/source/futures.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/gpu.rst` & `dask-2023.6.0/docs/source/gpu.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/graph_manipulation.rst` & `dask-2023.6.0/docs/source/graph_manipulation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/graphs.rst` & `dask-2023.6.0/docs/source/graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/graphviz.rst` & `dask-2023.6.0/docs/source/graphviz.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/high-level-graphs.rst` & `dask-2023.6.0/docs/source/high-level-graphs.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/adaptive.rst` & `dask-2023.6.0/docs/source/how-to/adaptive.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/connect-to-remote-data.rst` & `dask-2023.6.0/docs/source/how-to/connect-to-remote-data.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/customize-initialization.rst` & `dask-2023.6.0/docs/source/how-to/customize-initialization.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/debug.rst` & `dask-2023.6.0/docs/source/how-to/debug.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/extend-sizeof.rst` & `dask-2023.6.0/docs/source/how-to/extend-sizeof.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/manage-environments.rst` & `dask-2023.6.0/docs/source/how-to/manage-environments.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/selecting-the-collection-backend.rst` & `dask-2023.6.0/docs/source/how-to/selecting-the-collection-backend.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/how-to/setup-prometheus.rst` & `dask-2023.6.0/docs/source/how-to/setup-prometheus.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/10_minutes_array_graph.png` & `dask-2023.6.0/docs/source/images/10_minutes_array_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/10_minutes_bag_graph.png` & `dask-2023.6.0/docs/source/images/10_minutes_bag_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/10_minutes_dataframe_graph.png` & `dask-2023.6.0/docs/source/images/10_minutes_dataframe_graph.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/HHMI_Janelia_Color.png` & `dask-2023.6.0/docs/source/images/HHMI_Janelia_Color.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/array.svg` & `dask-2023.6.0/docs/source/images/array.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/async-embarrassing.gif` & `dask-2023.6.0/docs/source/images/async-embarrassing.gif`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/concurrent-futures-threaded.webp` & `dask-2023.6.0/docs/source/images/concurrent-futures-threaded.webp`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/crosstalk.svg` & `dask-2023.6.0/docs/source/images/crosstalk.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_jupyterlab.png` & `dask-2023.6.0/docs/source/images/dashboard_jupyterlab.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_link.png` & `dask-2023.6.0/docs/source/images/dashboard_link.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_memory.png` & `dask-2023.6.0/docs/source/images/dashboard_memory.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_memory_new.gif` & `dask-2023.6.0/docs/source/images/dashboard_memory_new.gif`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_progress.png` & `dask-2023.6.0/docs/source/images/dashboard_progress.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_status.png` & `dask-2023.6.0/docs/source/images/dashboard_status.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_task_processing.png` & `dask-2023.6.0/docs/source/images/dashboard_task_processing.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_task_stream_unhealthy.png` & `dask-2023.6.0/docs/source/images/dashboard_task_stream_unhealthy.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dashboard_taskstream_healthy.png` & `dask-2023.6.0/docs/source/images/dashboard_taskstream_healthy.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-adaptive.svg` & `dask-2023.6.0/docs/source/images/dask-adaptive.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-array.svg` & `dask-2023.6.0/docs/source/images/dask-array.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-cluster-manager.svg` & `dask-2023.6.0/docs/source/images/dask-cluster-manager.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-dataframe.svg` & `dask-2023.6.0/docs/source/images/dask-dataframe.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-overview-distributed-callout.svg` & `dask-2023.6.0/docs/source/images/dask-overview-distributed-callout.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-overview-schedulers.svg` & `dask-2023.6.0/docs/source/images/dask-overview-schedulers.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask-overview.svg` & `dask-2023.6.0/docs/source/images/dask-overview.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_horizontal.svg` & `dask-2023.6.0/docs/source/images/dask_horizontal.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_horizontal_black.svg` & `dask-2023.6.0/docs/source/images/dask_horizontal_black.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_horizontal_on_blue.svg` & `dask-2023.6.0/docs/source/images/dask_horizontal_on_blue.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_horizontal_on_pink.svg` & `dask-2023.6.0/docs/source/images/dask_horizontal_on_pink.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_horizontal_white.svg` & `dask-2023.6.0/docs/source/images/dask_horizontal_white.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_icon.svg` & `dask-2023.6.0/docs/source/images/dask_icon.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_icon_black.svg` & `dask-2023.6.0/docs/source/images/dask_icon_black.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_icon_on_pink.svg` & `dask-2023.6.0/docs/source/images/dask_icon_on_pink.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/dask_icon_white.svg` & `dask-2023.6.0/docs/source/images/dask_icon_white.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/delayed-inc-double-add.svg` & `dask-2023.6.0/docs/source/images/delayed-inc-double-add.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/distributed-overview.svg` & `dask-2023.6.0/docs/source/images/distributed-overview.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/frame-shuffle.svg` & `dask-2023.6.0/docs/source/images/frame-shuffle.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/frame-sort.svg` & `dask-2023.6.0/docs/source/images/frame-sort.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/frame.svg` & `dask-2023.6.0/docs/source/images/frame.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/gputester-msg.png` & `dask-2023.6.0/docs/source/images/gputester-msg.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/growth_of_languages.png` & `dask-2023.6.0/docs/source/images/growth_of_languages.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/growth_of_libraries.png` & `dask-2023.6.0/docs/source/images/growth_of_libraries.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/inc-add.svg` & `dask-2023.6.0/docs/source/images/inc-add.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/map-reduce-task-scheduling.svg` & `dask-2023.6.0/docs/source/images/map-reduce-task-scheduling.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/map_blocks_drop_axis.png` & `dask-2023.6.0/docs/source/images/map_blocks_drop_axis.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/merge_chunks.png` & `dask-2023.6.0/docs/source/images/merge_chunks.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/merge_chunks_false.png` & `dask-2023.6.0/docs/source/images/merge_chunks_false.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/optimize_dask1.svg` & `dask-2023.6.0/docs/source/images/optimize_dask1.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/optimize_dask2.svg` & `dask-2023.6.0/docs/source/images/optimize_dask2.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/optimize_dask3.svg` & `dask-2023.6.0/docs/source/images/optimize_dask3.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/optimize_dask4.svg` & `dask-2023.6.0/docs/source/images/optimize_dask4.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/optimize_dask5.svg` & `dask-2023.6.0/docs/source/images/optimize_dask5.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/order-failure.png` & `dask-2023.6.0/docs/source/images/order-failure.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/order-success.png` & `dask-2023.6.0/docs/source/images/order-success.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/overlap.svg` & `dask-2023.6.0/docs/source/images/overlap.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/overlapping-blocks.svg` & `dask-2023.6.0/docs/source/images/overlapping-blocks.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/overlapping-neighbors.svg` & `dask-2023.6.0/docs/source/images/overlapping-neighbors.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/pipeline.svg` & `dask-2023.6.0/docs/source/images/pipeline.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/reshape.png` & `dask-2023.6.0/docs/source/images/reshape.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/reshape_problem.png` & `dask-2023.6.0/docs/source/images/reshape_problem.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/reshape_rechunked.png` & `dask-2023.6.0/docs/source/images/reshape_rechunked.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/scaling-edges.png` & `dask-2023.6.0/docs/source/images/scaling-edges.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/scaling-nodes.png` & `dask-2023.6.0/docs/source/images/scaling-nodes.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/simple-dask.png` & `dask-2023.6.0/docs/source/images/simple-dask.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/transpose-hlg-hovertooltip.png` & `dask-2023.6.0/docs/source/images/transpose-hlg-hovertooltip.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/transpose-hlg-html-repr.png` & `dask-2023.6.0/docs/source/images/transpose-hlg-html-repr.png`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/transpose.svg` & `dask-2023.6.0/docs/source/images/transpose.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/transpose_opt.svg` & `dask-2023.6.0/docs/source/images/transpose_opt.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/trivial.svg` & `dask-2023.6.0/docs/source/images/trivial.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/images/unoverlapping-neighbors.svg` & `dask-2023.6.0/docs/source/images/unoverlapping-neighbors.svg`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/index.rst` & `dask-2023.6.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/install.rst` & `dask-2023.6.0/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/logos.rst` & `dask-2023.6.0/docs/source/logos.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/maintainers.rst` & `dask-2023.6.0/docs/source/maintainers.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/optimize.rst` & `dask-2023.6.0/docs/source/optimize.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/order.rst` & `dask-2023.6.0/docs/source/order.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/phases-of-computation.rst` & `dask-2023.6.0/docs/source/phases-of-computation.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/presentations.rst` & `dask-2023.6.0/docs/source/presentations.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/scheduler-overview.rst` & `dask-2023.6.0/docs/source/scheduler-overview.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/scheduling-policy.rst` & `dask-2023.6.0/docs/source/scheduling-policy.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/scheduling.rst` & `dask-2023.6.0/docs/source/scheduling.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/scripts/scheduling.py` & `dask-2023.6.0/docs/source/scripts/scheduling.py`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/shared.rst` & `dask-2023.6.0/docs/source/shared.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/spark.rst` & `dask-2023.6.0/docs/source/spark.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/spec.rst` & `dask-2023.6.0/docs/source/spec.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/support.rst` & `dask-2023.6.0/docs/source/support.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/understanding-performance.rst` & `dask-2023.6.0/docs/source/understanding-performance.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/user-interfaces.rst` & `dask-2023.6.0/docs/source/user-interfaces.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/docs/source/why.rst` & `dask-2023.6.0/docs/source/why.rst`

 * *Files identical despite different names*

### Comparing `dask-2023.5.1/pyproject.toml` & `dask-2023.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 array = ["numpy >= 1.21"]
 # keeping for backwards compatibility
 bag = []
 dataframe = [
     "numpy >= 1.21",
     "pandas >= 1.3",
 ]
-distributed = ["distributed == 2023.5.1"]
+distributed = ["distributed == 2023.6.0"]
 diagnostics = [
     "bokeh >= 2.4.2",
     "jinja2 >= 2.10.3",
 ]
 # keeping for backwards compatibility
 delayed = []
 complete = [
@@ -134,17 +134,14 @@
     'ignore:The distutils\.sysconfig module is deprecated, use sysconfig instead:DeprecationWarning:numpy',
     # With no network access, distributed raises a warning when detecting local IP address
     "ignore:Couldn't detect a suitable IP address:RuntimeWarning:distributed",
     # Ignore FutureWarning for change in group_keys behavior: no changes required on the dask side.
     # https://pandas.pydata.org/docs/dev/whatsnew/v1.5.0.html#using-group-keys-with-transformers-in-groupby-apply
     "ignore:Not prepending group keys:FutureWarning",
     "ignore:.*:dask.tests.warning_aliases.RemovedIn20Warning",
-    # This is coming from pandas use of np.find_common_type
-    # See https://github.com/pandas-dev/pandas/issues/53236
-    "ignore:np.find_common_type is deprecated:DeprecationWarning",
 ]
 xfail_strict = true
 
 [tool.mypy]
 # Silence errors about Python 3.9-style delayed type annotations on Python 3.8
 python_version = "3.9"
 # See https://github.com/python/mypy/issues/12286 for automatic multi-platform support
```

