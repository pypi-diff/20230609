# Comparing `tmp/polars_lts_cpu-0.18.1.tar.gz` & `tmp/polars_lts_cpu-0.18.2.tar.gz`

## Comparing `polars_lts_cpu-0.18.1.tar` & `polars_lts_cpu-0.18.2.tar`

### file list

```diff
@@ -1,1240 +1,1240 @@
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123      142 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-algo/README.md
--rw-r--r--   0     1001      123     7548 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      132 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/README.md
--rw-r--r--   0     1001      123     2382 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
--rw-r--r--   0     1001      123      267 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     1512 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
--rw-r--r--   0     1001      123     4108 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
--rw-r--r--   0     1001      123      234 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1687 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2419 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19010 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     7633 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      545 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9452 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8409 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123      439 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/sum.rs
--rw-r--r--   0     1001      123     2486 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18232 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      237 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11866 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3688 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     5245 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/fused.rs
--rw-r--r--   0     1001      123     3423 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1187 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/LICENSE
--rw-r--r--   0     1001      123    16770 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/json/deserialize.rs
--rw-r--r--   0     1001      123     6564 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/json/infer_schema.rs
--rw-r--r--   0     1001      123      189 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/json/mod.rs
--rw-r--r--   0     1001      123       30 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/lib.rs
--rw-r--r--   0     1001      123     1198 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/ndjson/deserialize.rs
--rw-r--r--   0     1001      123     4808 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/ndjson/file.rs
--rw-r--r--   0     1001      123      143 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/ndjson/mod.rs
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123      144 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/README.md
--rw-r--r--   0     1001      123     1975 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     1791 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
--rw-r--r--   0     1001      123     3773 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6664 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     8165 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     2252 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      370 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
--rw-r--r--   0     1001      123     2181 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
--rw-r--r--   0     1001      123     1482 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
--rw-r--r--   0     1001      123     1028 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
--rw-r--r--   0     1001      123     1177 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
--rw-r--r--   0     1001      123      508 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
--rw-r--r--   0     1001      123       51 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
--rw-r--r--   0     1001      123        1 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arity.rs
--rw-r--r--   0     1001      123      727 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/bitwise.rs
--rw-r--r--   0     1001      123     1206 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123     3964 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/decimal.rs
--rw-r--r--   0     1001      123     1250 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123      391 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
--rw-r--r--   0     1001      123     2767 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123     3487 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
--rw-r--r--   0     1001      123    25289 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123      797 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/tile.rs
--rw-r--r--   0     1001      123     1102 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      984 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4783 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1074 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/comparison.rs
--rw-r--r--   0     1001      123     1068 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1885 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9783 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3923 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2105 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    19032 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3970 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11693 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5616 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     9545 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1879 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14722 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123    10034 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11643 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4821 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8687 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4344 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     3672 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      496 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      183 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2821 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2052 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5232 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123      138 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/README.md
--rw-r--r--   0     1001      123     2383 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3608 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28133 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1815 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19446 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    22226 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10846 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13938 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    30724 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    24531 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    14759 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7586 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9227 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8287 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123    11044 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/json/mod.rs
--rw-r--r--   0     1001      123     4771 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7155 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ndjson/buffer.rs
--rw-r--r--   0     1001      123    11979 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ndjson/core.rs
--rw-r--r--   0     1001      123       37 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ndjson/mod.rs
--rw-r--r--   0     1001      123      273 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7360 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4784 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9623 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10052 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      621 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4374 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17253 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123     3992 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/arity.rs
--rw-r--r--   0     1001      123     1278 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/array.rs
--rw-r--r--   0     1001      123      935 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123    10228 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123     9538 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123     6441 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
--rw-r--r--   0     1001      123      753 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1074 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
--rw-r--r--   0     1001      123     1327 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123      257 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
--rw-r--r--   0     1001      123     6261 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
--rw-r--r--   0     1001      123     1593 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123     9597 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      673 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     2567 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123      992 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
--rw-r--r--   0     1001      123     8119 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    21034 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    14242 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    21047 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     5509 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123     1155 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/arity.rs
--rw-r--r--   0     1001      123      611 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
--rw-r--r--   0     1001      123     2717 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/concat.rs
--rw-r--r--   0     1001      123     4525 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
--rw-r--r--   0     1001      123     8736 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
--rw-r--r--   0     1001      123     1044 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/index.rs
--rw-r--r--   0     1001      123      968 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/mod.rs
--rw-r--r--   0     1001      123     9827 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/range.rs
--rw-r--r--   0     1001      123     1308 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
--rw-r--r--   0     1001      123     1973 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
--rw-r--r--   0     1001      123    11328 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
--rw-r--r--   0     1001      123    10213 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     3772 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    61334 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2658 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123     1068 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/selector.rs
--rw-r--r--   0     1001      123    17095 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     8318 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11742 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25683 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    24898 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29993 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15470 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    11905 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123    10140 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10559 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8072 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15277 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     2889 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14479 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6017 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
--rw-r--r--   0     1001      123     6774 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28901 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15756 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15752 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     3707 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27269 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13786 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     4181 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    20215 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10545 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    18601 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     6144 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13026 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      832 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11871 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123      358 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/README.md
--rw-r--r--   0     1001      123     1796 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4479 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     5127 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6754 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9278 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    48867 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     2734 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1555 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3986 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     4125 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13580 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4883 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     5859 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     6753 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2854 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4303 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1209 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     2015 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     4041 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1335 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21959 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    18331 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    17197 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     2583 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
--rw-r--r--   0     1001      123     3153 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     1996 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    23566 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     4332 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    13549 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31558 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2039 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      414 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    24050 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    20552 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9647 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123     2535 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
--rw-r--r--   0     1001      123     9227 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
--rw-r--r--   0     1001      123    15835 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
--rw-r--r--   0     1001      123      116 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     5827 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7066 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12759 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4166 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4273 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    15680 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6772 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3165 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47687 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     9513 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2893 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1028 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123      165 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/README.md
--rw-r--r--   0     1001      123       98 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      266 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      682 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/pass.rs
--rw-r--r--   0     1001      123      548 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3553 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     3559 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    11288 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     7500 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13819 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     3243 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2767 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     6311 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123     3116 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
--rw-r--r--   0     1001      123    11009 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2119 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4695 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     1887 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20783 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23420 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     9239 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5451 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2241 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     6787 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     7279 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3908 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5984 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      366 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     4335 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      514 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    21304 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    18204 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1155 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123      137 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/README.md
--rw-r--r--   0     1001      123     8985 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13676 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123      143 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/README.md
--rw-r--r--   0     1001      123     3565 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    11031 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     6408 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     2372 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    18180 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    18997 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     3975 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123    10548 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     3442 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    34469 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      621 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123     2976 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/month_end.rs
--rw-r--r--   0     1001      123     3365 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/month_start.rs
--rw-r--r--   0     1001      123      274 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1381 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     3992 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12787 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1443 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     6845 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2511 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2672 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    25015 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    21244 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    23652 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11666 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123      144 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/README.md
--rw-r--r--   0     1001      123     5125 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
--rw-r--r--   0     1001      123     8275 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
--rw-r--r--   0     1001      123     9406 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
--rw-r--r--   0     1001      123     3588 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
--rw-r--r--   0     1001      123     2551 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/array/mod.rs
--rw-r--r--   0     1001      123     6448 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     4311 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
--rw-r--r--   0     1001      123     1556 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    20366 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8969 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    16475 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    49461 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123    10060 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     7175 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    42339 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1453 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2347 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7963 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     3242 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19830 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10219 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6417 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2556 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    15982 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23389 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4806 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2956 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32691 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123    10025 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2880 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123    10551 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2820 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    28256 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6214 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123      908 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
--rw-r--r--   0     1001      123     7056 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    19463 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8691 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
--rw-r--r--   0     1001      123     8866 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     6323 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     5876 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    16797 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123     2658 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
--rw-r--r--   0     1001      123    23276 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     4375 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     2771 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10266 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     7391 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5528 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7543 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    31164 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    22078 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     7848 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123      301 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5810 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6072 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123      459 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
--rw-r--r--   0     1001      123    11626 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     8427 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1875 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2826 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    10497 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      595 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     3042 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25939 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7944 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2509 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42658 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    13349 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5609 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     8059 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      263 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36432 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     9916 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    35761 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6973 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5181 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16760 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    19219 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4113 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7749 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    40369 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5634 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    22901 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14380 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39516 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10637 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    19780 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123     5406 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/args.rs
--rw-r--r--   0     1001      123    13329 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22364 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    17372 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     4608 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6434 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4564 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    12313 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123     3865 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
--rw-r--r--   0     1001      123   126128 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27652 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     5183 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5976 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     9875 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2811 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10198 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17611 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15733 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2423 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123    17006 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     1094 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/df.rs
--rw-r--r--   0     1001      123     6559 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18543 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28755 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    19293 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    29575 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     6080 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/array.rs
--rw-r--r--   0     1001      123     9089 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10835 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12800 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    18214 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15034 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     7981 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    14734 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14063 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6078 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18396 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5522 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7939 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11788 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9607 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4471 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6241 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    38559 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5814 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4620 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5073 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18408 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2912 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     7077 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123     2492 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/flatten.rs
--rw-r--r--   0     1001      123    30596 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1600 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13201 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123      141 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/README.md
--rw-r--r--   0     1001      123      151 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/aliases.rs
--rw-r--r--   0     1001      123     2862 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123     2709 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      490 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     2336 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1115 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123      466 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123    22794 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    20710 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123     2098 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/keywords.rs
--rw-r--r--   0     1001      123      239 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123    19192 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     4572 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0     1001      123     1682 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_cumulative.rs
--rw-r--r--   0     1001      123     3063 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_io.rs
--rw-r--r--   0     1001      123     1539 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_math.rs
--rw-r--r--   0     1001      123      860 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_meta.rs
--rw-r--r--   0     1001      123     2982 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_string.rs
--rw-r--r--   0     1001      123     1056 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_7436.rs
--rw-r--r--   0     1001      123      888 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_7437.rs
--rw-r--r--   0     1001      123      652 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_7440.rs
--rw-r--r--   0     1001      123      700 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_8395.rs
--rw-r--r--   0     1001      123     1062 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_8419.rs
--rw-r--r--   0     1001      123      982 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/ops_distinct_on.rs
--rw-r--r--   0     1001      123    15418 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/simple_exprs.rs
--rw-r--r--   0     1001      123     2985 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/statements.rs
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123      145 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-error/README.md
--rw-r--r--   0     1001      123     6584 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3570 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8794 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20213 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       54 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17836 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      198 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123       24 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/ops/mod.rs
--rw-r--r--   0     1001      123      457 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/ops/take.rs
--rw-r--r--   0     1001      123     6259 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    11091 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30423 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7043 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      531 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      709 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10285 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1065 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10657 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1635 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5614 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4483 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6584 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123    12591 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     4393 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/.gitignore
--rw-r--r--   0     1001      123     1055 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/LICENSE
--rw-r--r--   0     1001      123     2414 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/Makefile
--rw-r--r--   0     1001      123    11998 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/README.md
--rw-r--r--   0     1001      123      651 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/build.rs
--rw-r--r--   0     1001      123       32 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      491 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1164 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/run_live_docs_server.py
--rw-r--r--   0     1001      123     1567 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7297 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1694 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1538 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      673 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      267 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/array.rst
--rw-r--r--   0     1001      123      309 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1130 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      470 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      722 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      432 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      159 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      951 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123     1036 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      683 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      405 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1294 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      277 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1013 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123     3316 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/selectors.rst
--rw-r--r--   0     1001      123      358 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      277 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/array.rst
--rw-r--r--   0     1001      123      257 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      744 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      437 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      776 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123     1021 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      421 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1192 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      503 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123     8067 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6161 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/__init__.py
--rw-r--r--   0     1001      123      280 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/_reexport.py
--rw-r--r--   0     1001      123    13229 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/api.py
--rw-r--r--   0     1001      123    28746 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/config.py
--rw-r--r--   0     1001      123    28105 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5227 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   315508 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    40637 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2692 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    16199 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1603 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4701 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    15739 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/dependencies.py
--rw-r--r--   0     1001      123     3573 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/__init__.py
--rw-r--r--   0     1001      123     3020 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/array.py
--rw-r--r--   0     1001      123     2704 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/binary.py
--rw-r--r--   0     1001      123     1698 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/categorical.py
--rw-r--r--   0     1001      123    77598 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/datetime.py
--rw-r--r--   0     1001      123   261537 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/expr.py
--rw-r--r--   0     1001      123    23905 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/list.py
--rw-r--r--   0     1001      123     4050 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/meta.py
--rw-r--r--   0     1001      123    58339 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/string.py
--rw-r--r--   0     1001      123     5426 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/expr/struct.py
--rw-r--r--   0     1001      123     2068 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/__init__.py
--rw-r--r--   0     1001      123    16541 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/as_datatype.py
--rw-r--r--   0     1001      123    18358 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/eager.py
--rw-r--r--   0     1001      123    72401 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/lazy.py
--rw-r--r--   0     1001      123    16227 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/range.py
--rw-r--r--   0     1001      123     6027 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/repeat.py
--rw-r--r--   0     1001      123     6139 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      952 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/_utils.py
--rw-r--r--   0     1001      123      861 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1072 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4681 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35482 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     5627 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/database.py
--rw-r--r--   0     1001      123    11047 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18449 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     6466 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1227 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5804 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      502 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/json.py
--rw-r--r--   0     1001      123     2207 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1259 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7177 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2291 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3601 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   168214 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24078 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/py.typed
--rw-r--r--   0     1001      123    32340 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/selectors.py
--rw-r--r--   0     1001      123       69 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/__init__.py
--rw-r--r--   0     1001      123     1572 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/_numpy.py
--rw-r--r--   0     1001      123     2515 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/array.py
--rw-r--r--   0     1001      123     1913 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/binary.py
--rw-r--r--   0     1001      123     1692 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/categorical.py
--rw-r--r--   0     1001      123    51711 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/datetime.py
--rw-r--r--   0     1001      123    13196 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/list.py
--rw-r--r--   0     1001      123   170010 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/series.py
--rw-r--r--   0     1001      123    37766 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/string.py
--rw-r--r--   0     1001      123     2542 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/struct.py
--rw-r--r--   0     1001      123     5361 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/series/utils.py
--rw-r--r--   0     1001      123     7559 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/sql/__init__.py
--rw-r--r--   0     1001      123    17409 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/__init__.py
--rw-r--r--   0     1001      123     1060 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/_private.py
--rw-r--r--   0     1001      123    16425 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/asserts.py
--rw-r--r--   0     1001      123      898 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    26833 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     3409 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/parametric/profiles.py
--rw-r--r--   0     1001      123    12132 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     6214 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/type_aliases.py
--rw-r--r--   0     1001      123     1169 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/__init__.py
--rw-r--r--   0     1001      123    54269 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/_construction.py
--rw-r--r--   0     1001      123     3902 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      711 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/_scan.py
--rw-r--r--   0     1001      123      579 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/build_info.py
--rw-r--r--   0     1001      123     8609 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/convert.py
--rw-r--r--   0     1001      123     6132 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2673 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    12905 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/polars/utils/various.py
--rw-r--r--   0     1001      123     5375 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/pyproject.toml
--rw-r--r--   0     1001      123      697 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/requirements-dev.txt
--rw-r--r--   0     1001      123       71 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10980 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     7448 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/apply/lazy.rs
--rw-r--r--   0     1001      123     8402 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/apply/mod.rs
--rw-r--r--   0     1001      123    90009 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3902 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5250 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/batched_csv.rs
--rw-r--r--   0     1001      123    48675 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/conversion.rs
--rw-r--r--   0     1001      123    45928 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/dataframe.rs
--rw-r--r--   0     1001      123     3950 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/error.rs
--rw-r--r--   0     1001      123      570 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/array.rs
--rw-r--r--   0     1001      123     2080 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/binary.rs
--rw-r--r--   0     1001      123      274 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/categorical.rs
--rw-r--r--   0     1001      123     5935 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/datetime.rs
--rw-r--r--   0     1001      123    34247 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/general.rs
--rw-r--r--   0     1001      123     3937 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/list.rs
--rw-r--r--   0     1001      123     2907 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/meta.rs
--rw-r--r--   0     1001      123      870 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/mod.rs
--rw-r--r--   0     1001      123     8677 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/string.rs
--rw-r--r--   0     1001      123      467 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/expr/struct.rs
--rw-r--r--   0     1001      123     9482 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/file.rs
--rw-r--r--   0     1001      123     3307 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/eager.rs
--rw-r--r--   0     1001      123     1657 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/io.rs
--rw-r--r--   0     1001      123    11835 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/lazy.rs
--rw-r--r--   0     1001      123     1312 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/meta.rs
--rw-r--r--   0     1001      123      217 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/misc.rs
--rw-r--r--   0     1001      123       87 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/mod.rs
--rw-r--r--   0     1001      123     1474 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/functions/whenthen.rs
--rw-r--r--   0     1001      123    30767 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/lazyframe.rs
--rw-r--r--   0     1001      123     2670 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/lazygroupby.rs
--rw-r--r--   0     1001      123     8268 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/lib.rs
--rw-r--r--   0     1001      123     1029 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/object.rs
--rw-r--r--   0     1001      123      122 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/py_modules.rs
--rw-r--r--   0     1001      123     1964 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/aggregation.rs
--rw-r--r--   0     1001      123     5406 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/arithmetic.rs
--rw-r--r--   0     1001      123     5138 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/comparison.rs
--rw-r--r--   0     1001      123     9077 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/construction.rs
--rw-r--r--   0     1001      123     8971 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/export.rs
--rw-r--r--   0     1001      123    26521 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/mod.rs
--rw-r--r--   0     1001      123     4569 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/numpy_ufunc.rs
--rw-r--r--   0     1001      123     4046 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/series/set_at_idx.rs
--rw-r--r--   0     1001      123     1036 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7963 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     6530 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123      179 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/parametric/conftest.py
--rw-r--r--   0     1001      123     3856 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     6897 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     8299 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      973 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_array.py
--rw-r--r--   0     1001      123      847 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    13603 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     5222 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      549 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123      423 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_integer.py
--rw-r--r--   0     1001      123    13216 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    27749 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    87542 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      418 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/datatypes/test_time.py
--rw-r--r--   0     1001      123        0 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/functions/__init__.py
--rw-r--r--   0     1001      123    13970 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/functions/test_as_datatype.py
--rw-r--r--   0     1001      123      480 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/functions/test_concat.py
--rw-r--r--   0     1001      123    15610 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/functions/test_functions.py
--rw-r--r--   0     1001      123    18470 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/functions/test_range.py
--rw-r--r--   0     1001      123     3724 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/functions/test_repeat.py
--rw-r--r--   0     1001      123      218 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1884 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39230 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6336 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     6172 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11169 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5483 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3986 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     7379 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2867 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11145 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13739 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3686 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123      589 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_array.py
--rw-r--r--   0     1001      123     3218 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    19585 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    14067 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1829 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23544 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    17964 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     7755 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123    10643 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     6932 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123     4631 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     3275 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     8813 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3664 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    24998 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123     7649 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_groupby_rolling.py
--rw-r--r--   0     1001      123     2983 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_is_in.py
--rw-r--r--   0     1001      123    18169 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    14612 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    19818 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123     1917 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_select.py
--rw-r--r--   0     1001      123    20578 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     4273 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     4130 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123    11694 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     5401 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/operations/test_with_columns.py
--rw-r--r--   0     1001      123        0 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/streaming/__init__.py
--rw-r--r--   0     1001      123      196 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/streaming/conftest.py
--rw-r--r--   0     1001      123      839 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/streaming/test_ooc.py
--rw-r--r--   0     1001      123    16053 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/streaming/test_streaming.py
--rw-r--r--   0     1001      123     4775 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19865 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    41129 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     5198 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   119415 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_df.py
--rw-r--r--   0     1001      123     2151 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    18790 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2741 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    34736 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3516 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123     3763 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    38286 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    47730 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2463 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4610 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     7073 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11551 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    13394 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     7231 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_selectors.py
--rw-r--r--   0     1001      123     2823 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83729 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_series.py
--rw-r--r--   0     1001      123      657 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_single.py
--rw-r--r--   0     1001      123     6747 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    12957 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123     2784 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/utils/test_parse_expr_input.py
--rw-r--r--   0     1001      123      247 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     5026 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    63894 2023-06-07 16:53:55.000000 polars_lts_cpu-0.18.1/Cargo.lock
--rw-r--r--   0        0        0    14545 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123      165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/README.md
+-rw-r--r--   0     1001      123       98 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      266 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      682 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/pass.rs
+-rw-r--r--   0     1001      123      548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3553 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     3559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    11288 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     3030 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     7500 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    13819 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     3243 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     6311 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123     3116 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs
+-rw-r--r--   0     1001      123    11264 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2119 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4695 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     1887 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20783 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23420 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     9239 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5451 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     6787 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     7279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      635 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5984 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     4335 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      514 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    21304 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    18204 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     5971 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123      358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/README.md
+-rw-r--r--   0     1001      123     1796 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4479 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     5127 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9278 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    48867 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     2734 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1555 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3986 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     4125 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13580 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4883 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     5859 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     6753 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2854 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4303 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1209 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     2015 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     4041 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1335 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21959 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    18331 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17197 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     2583 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs
+-rw-r--r--   0     1001      123     3153 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     1996 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    23566 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     4332 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    13549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31558 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    24050 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    20552 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9647 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123     2535 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs
+-rw-r--r--   0     1001      123     9227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs
+-rw-r--r--   0     1001      123    15835 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs
+-rw-r--r--   0     1001      123      116 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     5827 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7066 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12759 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4166 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    15680 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6772 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47687 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     9513 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2893 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0    10560 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3472 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8794 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       54 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17836 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123       24 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/ops/mod.rs
+-rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/ops/take.rs
+-rw-r--r--   0     1001      123     6259 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    11096 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7043 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      531 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      709 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1065 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10657 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1635 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5614 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4483 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6584 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0     2037 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123      143 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/README.md
+-rw-r--r--   0     1001      123     3565 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    11101 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     6408 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2372 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    18180 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    18997 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     3975 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123    10548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     3442 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    34469 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      621 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123     2976 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_end.rs
+-rw-r--r--   0     1001      123     3365 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_start.rs
+-rw-r--r--   0     1001      123      274 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1381 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     3992 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12787 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1443 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     6845 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2511 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2672 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    25015 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    21244 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    23652 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11666 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0     3439 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/README.md
+-rw-r--r--   0     1001      123     2382 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs
+-rw-r--r--   0     1001      123      267 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     1512 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs
+-rw-r--r--   0     1001      123     4108 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs
+-rw-r--r--   0     1001      123      234 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1687 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2419 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19010 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     7633 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      545 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9452 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8409 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123      439 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/sum.rs
+-rw-r--r--   0     1001      123     2486 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18232 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      237 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11866 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3688 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     5245 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/fused.rs
+-rw-r--r--   0     1001      123     3423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1187 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0     4397 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123      138 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/README.md
+-rw-r--r--   0     1001      123     2383 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28133 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1815 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19446 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    22226 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10846 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13938 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    30724 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    24531 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    14759 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8287 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11044 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/json/mod.rs
+-rw-r--r--   0     1001      123     4771 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/buffer.rs
+-rw-r--r--   0     1001      123    11979 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/core.rs
+-rw-r--r--   0     1001      123       37 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/mod.rs
+-rw-r--r--   0     1001      123      273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9623 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10052 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      621 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4374 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0      569 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123      141 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/README.md
+-rw-r--r--   0     1001      123      151 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/aliases.rs
+-rw-r--r--   0     1001      123     2862 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123     2709 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      490 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     2336 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123      466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/README.md
+-rw-r--r--   0     1001      123    22794 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    20710 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     2098 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123      239 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    19192 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0     1001      123     1682 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_cumulative.rs
+-rw-r--r--   0     1001      123     3063 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_io.rs
+-rw-r--r--   0     1001      123     1539 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_math.rs
+-rw-r--r--   0     1001      123      860 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_meta.rs
+-rw-r--r--   0     1001      123     2982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_string.rs
+-rw-r--r--   0     1001      123     1056 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7436.rs
+-rw-r--r--   0     1001      123      888 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7437.rs
+-rw-r--r--   0     1001      123      652 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7440.rs
+-rw-r--r--   0     1001      123      700 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8395.rs
+-rw-r--r--   0     1001      123     1062 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8419.rs
+-rw-r--r--   0     1001      123      982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/ops_distinct_on.rs
+-rw-r--r--   0     1001      123    15418 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/simple_exprs.rs
+-rw-r--r--   0     1001      123     2985 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/statements.rs
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/README.md
+-rw-r--r--   0     1001      123     8985 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13676 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0     1353 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/LICENSE
+-rw-r--r--   0     1001      123    16770 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/deserialize.rs
+-rw-r--r--   0     1001      123     6564 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/infer_schema.rs
+-rw-r--r--   0     1001      123      189 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/mod.rs
+-rw-r--r--   0     1001      123       30 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/lib.rs
+-rw-r--r--   0     1001      123     1198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/deserialize.rs
+-rw-r--r--   0     1001      123     4808 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/file.rs
+-rw-r--r--   0     1001      123      143 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/mod.rs
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123      144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/README.md
+-rw-r--r--   0     1001      123     1975 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     1791 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/fixed_size_list.rs
+-rw-r--r--   0     1001      123     3773 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6664 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     8165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     2252 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      370 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/add.rs
+-rw-r--r--   0     1001      123     2181 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs
+-rw-r--r--   0     1001      123     1482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs
+-rw-r--r--   0     1001      123     1028 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs
+-rw-r--r--   0     1001      123     1177 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs
+-rw-r--r--   0     1001      123      508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/sub.rs
+-rw-r--r--   0     1001      123       51 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/mod.rs
+-rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arity.rs
+-rw-r--r--   0     1001      123      727 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/bitwise.rs
+-rw-r--r--   0     1001      123     1206 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123     3964 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/decimal.rs
+-rw-r--r--   0     1001      123     1250 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123      391 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/bitmap.rs
+-rw-r--r--   0     1001      123     2767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123     3487 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs
+-rw-r--r--   0     1001      123    25289 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123      797 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/tile.rs
+-rw-r--r--   0     1001      123     1102 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      984 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4783 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1074 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/comparison.rs
+-rw-r--r--   0     1001      123     1068 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1885 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9783 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3923 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2019 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    16191 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3839 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11729 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5684 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     9609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1879 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14722 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123    10055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11643 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4821 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8687 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4344 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     3672 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      496 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      183 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2052 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5232 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123      145 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/README.md
+-rw-r--r--   0     1001      123     6584 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123      142 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/README.md
+-rw-r--r--   0     1001      123     7548 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123      144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/README.md
+-rw-r--r--   0     1001      123     5125 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs
+-rw-r--r--   0     1001      123     8275 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     9406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs
+-rw-r--r--   0     1001      123     3588 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/iterator.rs
+-rw-r--r--   0     1001      123     2551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/mod.rs
+-rw-r--r--   0     1001      123     6448 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     4311 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs
+-rw-r--r--   0     1001      123     1556 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8969 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    16475 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    49461 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123    10060 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     7175 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    42339 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1453 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2347 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     3242 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19830 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10219 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6417 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2556 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23389 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4806 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2956 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32691 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123    10025 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2880 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123    10551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2820 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    28256 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123      908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs
+-rw-r--r--   0     1001      123     7056 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    19463 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8691 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs
+-rw-r--r--   0     1001      123     8866 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     6323 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     5876 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    16797 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123     2658 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs
+-rw-r--r--   0     1001      123    23276 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     4375 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     2771 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10266 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     7391 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5528 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7543 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    31164 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    22078 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     7848 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123      301 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5810 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6072 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123      459 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/tile.rs
+-rw-r--r--   0     1001      123    11626 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     8427 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1875 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2826 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    10497 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      595 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     3042 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25939 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7944 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42658 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    13349 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     8059 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      263 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36432 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     9916 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    35761 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6973 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5181 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16760 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    19219 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4113 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7749 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    40369 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5634 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    22901 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14380 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39516 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10637 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    19780 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123     5406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/args.rs
+-rw-r--r--   0     1001      123    13329 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22364 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    17372 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4608 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6434 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4564 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    12313 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123     3865 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs
+-rw-r--r--   0     1001      123   126128 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27652 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     5183 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     9875 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2811 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17611 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    17006 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     1094 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/df.rs
+-rw-r--r--   0     1001      123     6559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18543 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28755 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    19293 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    29575 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     6080 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/array.rs
+-rw-r--r--   0     1001      123     9089 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10835 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12800 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15034 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     7981 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    14734 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14063 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6078 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18396 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5522 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     7939 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11788 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9607 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    38559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5814 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4620 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5073 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18408 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2912 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     7077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     2492 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    30596 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1600 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13201 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     5152 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17253 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123     3992 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arity.rs
+-rw-r--r--   0     1001      123     1278 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/array.rs
+-rw-r--r--   0     1001      123      935 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123    10228 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123     9538 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123     6441 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs
+-rw-r--r--   0     1001      123      753 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1074 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/array.rs
+-rw-r--r--   0     1001      123     1327 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123      257 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/concat.rs
+-rw-r--r--   0     1001      123     6261 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs
+-rw-r--r--   0     1001      123     1593 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123     9597 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      782 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2567 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123      992 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs
+-rw-r--r--   0     1001      123     8119 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    21146 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    14453 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    21047 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     5509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123     1155 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/arity.rs
+-rw-r--r--   0     1001      123      611 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/coerce.rs
+-rw-r--r--   0     1001      123     2717 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/concat.rs
+-rw-r--r--   0     1001      123     4525 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/correlation.rs
+-rw-r--r--   0     1001      123     8736 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs
+-rw-r--r--   0     1001      123     1044 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/index.rs
+-rw-r--r--   0     1001      123      968 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/mod.rs
+-rw-r--r--   0     1001      123     9827 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/range.rs
+-rw-r--r--   0     1001      123     1308 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/selectors.rs
+-rw-r--r--   0     1001      123     1973 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs
+-rw-r--r--   0     1001      123    11328 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/temporal.rs
+-rw-r--r--   0     1001      123    10213 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     3772 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    61431 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2658 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123     1068 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/selector.rs
+-rw-r--r--   0     1001      123    17095 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     8318 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11742 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25683 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29993 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15470 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123    10140 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8072 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     2889 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6017 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs
+-rw-r--r--   0     1001      123     6774 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28901 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15756 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15752 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26507 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     3707 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27269 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13786 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     4181 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    20215 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10545 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    18601 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     6144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13026 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      832 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11871 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0     4393 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/Makefile
+-rw-r--r--   0     1001      123    11998 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/README.md
+-rw-r--r--   0     1001      123      651 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/build.rs
+-rw-r--r--   0     1001      123       32 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      491 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1164 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/run_live_docs_server.py
+-rw-r--r--   0     1001      123     1567 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7297 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     2069 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1538 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      673 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      267 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/array.rst
+-rw-r--r--   0     1001      123      309 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1130 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      470 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      722 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      432 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      159 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      951 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123     1036 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      836 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      405 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1294 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      277 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1013 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123     3279 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/selectors.rst
+-rw-r--r--   0     1001      123      358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      277 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/array.rst
+-rw-r--r--   0     1001      123      257 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      437 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      776 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123     1021 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      421 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1192 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      503 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123     8067 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6161 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/__init__.py
+-rw-r--r--   0     1001      123      280 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/_reexport.py
+-rw-r--r--   0     1001      123    13229 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/api.py
+-rw-r--r--   0     1001      123    29008 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/config.py
+-rw-r--r--   0     1001      123    28105 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   315508 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    40637 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2692 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    16199 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1603 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4701 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    15739 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/dependencies.py
+-rw-r--r--   0     1001      123     3573 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     3020 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/array.py
+-rw-r--r--   0     1001      123     2704 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1698 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    77598 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   261537 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/expr.py
+-rw-r--r--   0     1001      123    23905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/list.py
+-rw-r--r--   0     1001      123     4050 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/meta.py
+-rw-r--r--   0     1001      123    59014 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/string.py
+-rw-r--r--   0     1001      123     5426 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/expr/struct.py
+-rw-r--r--   0     1001      123     2068 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    16541 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/as_datatype.py
+-rw-r--r--   0     1001      123    18358 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/eager.py
+-rw-r--r--   0     1001      123    72401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/lazy.py
+-rw-r--r--   0     1001      123    16227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/range.py
+-rw-r--r--   0     1001      123     6027 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/repeat.py
+-rw-r--r--   0     1001      123     6139 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      952 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/_utils.py
+-rw-r--r--   0     1001      123      861 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1072 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4681 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     5627 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/database.py
+-rw-r--r--   0     1001      123    11047 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18449 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6466 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1227 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5804 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      502 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/json.py
+-rw-r--r--   0     1001      123     2207 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1259 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7177 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2291 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3601 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   168214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24078 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/py.typed
+-rw-r--r--   0     1001      123    32502 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/selectors.py
+-rw-r--r--   0     1001      123       69 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1572 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     2515 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/array.py
+-rw-r--r--   0     1001      123     1913 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/binary.py
+-rw-r--r--   0     1001      123     1692 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/categorical.py
+-rw-r--r--   0     1001      123    51711 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/datetime.py
+-rw-r--r--   0     1001      123    13196 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/list.py
+-rw-r--r--   0     1001      123   170010 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/series.py
+-rw-r--r--   0     1001      123    37808 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/string.py
+-rw-r--r--   0     1001      123     2542 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/struct.py
+-rw-r--r--   0     1001      123     5361 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/series/utils.py
+-rw-r--r--   0     1001      123     7559 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/sql/__init__.py
+-rw-r--r--   0     1001      123    17409 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/sql/context.py
+-rw-r--r--   0     1001      123     4793 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/__init__.py
+-rw-r--r--   0     1001      123     1060 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/_private.py
+-rw-r--r--   0     1001      123    16425 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      898 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    26833 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     3409 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/profiles.py
+-rw-r--r--   0     1001      123    12132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     6214 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    54302 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     3902 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      711 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      579 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     8609 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/convert.py
+-rw-r--r--   0     1001      123     6132 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2673 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    12905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/polars/utils/various.py
+-rw-r--r--   0     1001      123     5375 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/pyproject.toml
+-rw-r--r--   0     1001      123      697 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/requirements-dev.txt
+-rw-r--r--   0     1001      123       68 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    10980 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     7448 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/lazy.rs
+-rw-r--r--   0     1001      123     8402 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/mod.rs
+-rw-r--r--   0     1001      123    90009 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/batched_csv.rs
+-rw-r--r--   0     1001      123    48675 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/conversion.rs
+-rw-r--r--   0     1001      123    45928 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/dataframe.rs
+-rw-r--r--   0     1001      123     3950 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/error.rs
+-rw-r--r--   0     1001      123      570 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/array.rs
+-rw-r--r--   0     1001      123     2080 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/binary.rs
+-rw-r--r--   0     1001      123      274 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/categorical.rs
+-rw-r--r--   0     1001      123     5935 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/datetime.rs
+-rw-r--r--   0     1001      123    34040 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/general.rs
+-rw-r--r--   0     1001      123     3937 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/list.rs
+-rw-r--r--   0     1001      123     2907 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/meta.rs
+-rw-r--r--   0     1001      123      870 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/mod.rs
+-rw-r--r--   0     1001      123     8677 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/string.rs
+-rw-r--r--   0     1001      123      467 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/expr/struct.rs
+-rw-r--r--   0     1001      123     9482 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/file.rs
+-rw-r--r--   0     1001      123     3307 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/eager.rs
+-rw-r--r--   0     1001      123     1657 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/io.rs
+-rw-r--r--   0     1001      123    11835 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/lazy.rs
+-rw-r--r--   0     1001      123     1312 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/meta.rs
+-rw-r--r--   0     1001      123      217 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/misc.rs
+-rw-r--r--   0     1001      123       87 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/mod.rs
+-rw-r--r--   0     1001      123     1474 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/functions/whenthen.rs
+-rw-r--r--   0     1001      123    30767 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/lazyframe.rs
+-rw-r--r--   0     1001      123     2670 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/lazygroupby.rs
+-rw-r--r--   0     1001      123     8268 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/lib.rs
+-rw-r--r--   0     1001      123     1029 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/py_modules.rs
+-rw-r--r--   0     1001      123     1964 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/aggregation.rs
+-rw-r--r--   0     1001      123     5406 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/arithmetic.rs
+-rw-r--r--   0     1001      123     5138 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/comparison.rs
+-rw-r--r--   0     1001      123     9077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/construction.rs
+-rw-r--r--   0     1001      123     8971 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/export.rs
+-rw-r--r--   0     1001      123    26521 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/mod.rs
+-rw-r--r--   0     1001      123     4569 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/numpy_ufunc.rs
+-rw-r--r--   0     1001      123     4046 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/series/set_at_idx.rs
+-rw-r--r--   0     1001      123     1036 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7963 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     6530 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123      179 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3856 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     6897 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      973 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_array.py
+-rw-r--r--   0     1001      123      847 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    13228 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     5222 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      549 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123      423 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_integer.py
+-rw-r--r--   0     1001      123    13216 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    27749 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    87542 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/__init__.py
+-rw-r--r--   0     1001      123    13970 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_as_datatype.py
+-rw-r--r--   0     1001      123      480 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_concat.py
+-rw-r--r--   0     1001      123    15610 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_functions.py
+-rw-r--r--   0     1001      123    18470 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_range.py
+-rw-r--r--   0     1001      123     3724 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/functions/test_repeat.py
+-rw-r--r--   0     1001      123      218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1884 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39230 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6336 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     6172 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5483 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3986 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     7379 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2867 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11145 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13738 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3686 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123      589 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_array.py
+-rw-r--r--   0     1001      123     3218 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    19585 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    14067 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1829 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23544 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    17964 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     7755 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123    10643 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     6932 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123     4631 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     3275 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8813 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    24998 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     7649 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby_rolling.py
+-rw-r--r--   0     1001      123     2983 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    18169 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    14612 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    19818 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123     1917 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_select.py
+-rw-r--r--   0     1001      123    20578 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     4273 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     4130 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123    11694 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     5401 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/operations/test_with_columns.py
+-rw-r--r--   0     1001      123        0 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/__init__.py
+-rw-r--r--   0     1001      123      196 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/conftest.py
+-rw-r--r--   0     1001      123      908 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/test_ooc.py
+-rw-r--r--   0     1001      123    16053 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/streaming/test_streaming.py
+-rw-r--r--   0     1001      123     4775 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    20002 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    42513 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     5198 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   119414 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     2151 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    18790 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2741 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    34736 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3516 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123     3763 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    38286 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    47730 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2463 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4610 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     7073 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11551 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13394 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     7419 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_selectors.py
+-rw-r--r--   0     1001      123     2823 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83729 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_series.py
+-rw-r--r--   0     1001      123      657 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_single.py
+-rw-r--r--   0     1001      123     6747 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    12957 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123     2784 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_parse_expr_input.py
+-rw-r--r--   0     1001      123      247 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     5026 2023-06-09 08:24:59.000000 polars_lts_cpu-0.18.2/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    63894 2023-06-09 08:26:02.000000 polars_lts_cpu-0.18.2/Cargo.lock
+-rw-r--r--   0        0        0    14545 1970-01-01 00:00:00.000000 polars_lts_cpu-0.18.2/PKG-INFO
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/array/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/fused.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-json/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-json/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-json/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/json/deserialize.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/json/infer_schema.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/json/infer_schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/ndjson/deserialize.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/deserialize.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-json/src/ndjson/file.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-json/src/ndjson/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/fixed_size_list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/null.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/commutative.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/div.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/arithmetics/decimal/mul.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/bitwise.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/cast.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/decimal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/compute/tile.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/compute/tile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/comparison.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,573 +1,487 @@
-use no_nulls;
-use no_nulls::{rolling_apply_agg_window, RollingAggWindowNoNulls};
+use std::sync::Arc;
 
-use super::*;
-
-pub struct SortedMinMax<'a, T: NativeType> {
-    slice: &'a [T],
-}
-
-impl<'a, T: NativeType> RollingAggWindowNoNulls<'a, T> for SortedMinMax<'a, T> {
-    fn new(slice: &'a [T], _start: usize, _end: usize, _params: DynArgs) -> Self {
-        Self { slice }
-    }
-
-    #[inline]
-    unsafe fn update(&mut self, start: usize, _end: usize) -> T {
-        *self.slice.get_unchecked(start)
+use polars_core::frame::groupby::GroupsProxy;
+use polars_core::prelude::*;
+use polars_core::POOL;
+
+use crate::physical_plan::state::ExecutionState;
+use crate::prelude::*;
+
+pub struct BinaryExpr {
+    pub(crate) left: Arc<dyn PhysicalExpr>,
+    pub(crate) op: Operator,
+    pub(crate) right: Arc<dyn PhysicalExpr>,
+    expr: Expr,
+}
+
+impl BinaryExpr {
+    pub fn new(
+        left: Arc<dyn PhysicalExpr>,
+        op: Operator,
+        right: Arc<dyn PhysicalExpr>,
+        expr: Expr,
+    ) -> Self {
+        Self {
+            left,
+            op,
+            right,
+            expr,
+        }
     }
 }
 
-pub struct MinWindow<'a, T: NativeType + PartialOrd + IsFloat> {
-    slice: &'a [T],
-    min: T,
-    last_start: usize,
-    last_end: usize,
+/// Can partially do operations in place.
+fn apply_operator_owned(left: Series, right: Series, op: Operator) -> PolarsResult<Series> {
+    match op {
+        Operator::Plus => Ok(left + right),
+        Operator::Minus => Ok(left - right),
+        Operator::Multiply => Ok(left * right),
+        _ => apply_operator(&left, &right, op),
+    }
 }
 
-impl<'a, T: NativeType + IsFloat + PartialOrd> RollingAggWindowNoNulls<'a, T> for MinWindow<'a, T> {
-    fn new(slice: &'a [T], start: usize, end: usize, _params: DynArgs) -> Self {
-        let min = *slice[start..end]
-            .iter()
-            .min_by(|a, b| compare_fn_nan_min(*a, *b))
-            .unwrap_or(&slice[start]);
-        Self {
-            slice,
-            min,
-            last_start: start,
-            last_end: end,
+pub fn apply_operator(left: &Series, right: &Series, op: Operator) -> PolarsResult<Series> {
+    use DataType::*;
+    match op {
+        Operator::Gt => ChunkCompare::<&Series>::gt(left, right).map(|ca| ca.into_series()),
+        Operator::GtEq => ChunkCompare::<&Series>::gt_eq(left, right).map(|ca| ca.into_series()),
+        Operator::Lt => ChunkCompare::<&Series>::lt(left, right).map(|ca| ca.into_series()),
+        Operator::LtEq => ChunkCompare::<&Series>::lt_eq(left, right).map(|ca| ca.into_series()),
+        Operator::Eq => ChunkCompare::<&Series>::equal(left, right).map(|ca| ca.into_series()),
+        Operator::NotEq => {
+            ChunkCompare::<&Series>::not_equal(left, right).map(|ca| ca.into_series())
+        }
+        Operator::Plus => Ok(left + right),
+        Operator::Minus => Ok(left - right),
+        Operator::Multiply => Ok(left * right),
+        Operator::Divide => Ok(left / right),
+        Operator::TrueDivide => match left.dtype() {
+            #[cfg(feature = "dtype-decimal")]
+            Decimal(_, _) => Ok(left / right),
+            Date | Datetime(_, _) | Float32 | Float64 => Ok(left / right),
+            _ => Ok(&left.cast(&Float64)? / &right.cast(&Float64)?),
+        },
+        Operator::FloorDivide => {
+            #[cfg(feature = "round_series")]
+            {
+                floor_div_series(left, right)
+            }
+            #[cfg(not(feature = "round_series"))]
+            {
+                panic!("activate 'round_series' feature")
+            }
         }
+        Operator::And => left.bitand(right),
+        Operator::Or => left.bitor(right),
+        Operator::Xor => left.bitxor(right),
+        Operator::Modulus => Ok(left % right),
+        Operator::EqValidity => left.equal_missing(right).map(|ca| ca.into_series()),
+        Operator::NotEqValidity => left.not_equal_missing(right).map(|ca| ca.into_series()),
     }
+}
+
+impl BinaryExpr {
+    fn apply_elementwise<'a>(
+        &self,
+        mut ac_l: AggregationContext<'a>,
+        ac_r: AggregationContext,
+        aggregated: bool,
+    ) -> PolarsResult<AggregationContext<'a>> {
+        // we want to be able to mutate in place
+        // so we take the lhs to make sure that we drop
+        let lhs = ac_l.series().clone();
+        let rhs = ac_r.series().clone();
 
-    unsafe fn update(&mut self, start: usize, end: usize) -> T {
-        // recompute min
-        if start >= self.last_end
-            // the window only got smaller
-            || end == self.last_end
+        // drop lhs so that we might operate in place
         {
-            self.min = *self
-                .slice
-                .get_unchecked(start..end)
-                .iter()
-                .min_by(|a, b| compare_fn_nan_min(*a, *b))
-                .unwrap_or(self.slice.get_unchecked(start));
-
-            self.last_start = start;
-            self.last_end = end;
-
-            return self.min;
-        }
-
-        let mut recompute_min = false;
-        // remove elements that should leave the window
-        for idx in self.last_start..start {
-            // safety
-            // we are in bounds
-            let leaving_value = self.slice.get_unchecked(idx);
-
-            // if the leaving value is the
-            // max value, we need to recompute the max.
-            if matches!(
-                compare_fn_nan_min(leaving_value, &self.min),
-                Ordering::Equal
-            ) {
-                recompute_min = true;
-                break;
-            }
+            let _ = ac_l.take();
         }
 
-        let entering_min = self
-            .slice
-            .get_unchecked(self.last_end..end)
-            .iter()
-            .min_by(|a, b| compare_fn_nan_min(*a, *b))
-            .unwrap_or(self.slice.get_unchecked(std::cmp::min(
-                self.last_start,
-                self.last_end.saturating_sub(1),
-            )));
-
-        if recompute_min {
-            match compare_fn_nan_min(&self.min, entering_min) {
-                // do nothing
-                Ordering::Equal => {}
-                // leaving < entering
-                Ordering::Less => {
-                    // leaving value could be the smallest, we might need to recompute
-
-                    // check the values in between the window we did not yet
-                    // compute to find the max there. We compare that with the `entering_max`
-                    // if any value is equal to equal to `self.max` of previous window we can break
-                    // early
-                    let mut min_in_between = self.slice.get_unchecked(start);
-                    for idx in (start + 1)..self.last_end {
-                        // safety
-                        // we are in bounds
-                        let value = self.slice.get_unchecked(idx);
-
-                        if matches!(compare_fn_nan_min(value, min_in_between), Ordering::Less) {
-                            min_in_between = value;
-                        }
+        let out = apply_operator_owned(lhs, rhs, self.op)?;
 
-                        // the min is also in the in between values
-                        if matches!(compare_fn_nan_min(value, &self.min), Ordering::Equal) {
-                            self.last_start = start;
-                            self.last_end = end;
-                            return self.min;
-                        }
-                    }
+        ac_l.with_series(out, aggregated, Some(&self.expr))?;
+        Ok(ac_l)
+    }
 
-                    if matches!(
-                        compare_fn_nan_min(min_in_between, entering_min),
-                        Ordering::Less
-                    ) {
-                        self.min = *min_in_between
-                    } else {
-                        self.min = *entering_min
-                    }
-                }
-                // leaving > entering
-                Ordering::Greater => {
-                    if matches!(compare_fn_nan_min(entering_min, &self.min), Ordering::Less) {
-                        self.min = *entering_min
+    fn apply_group_aware<'a>(
+        &self,
+        mut ac_l: AggregationContext<'a>,
+        mut ac_r: AggregationContext<'a>,
+    ) -> PolarsResult<AggregationContext<'a>> {
+        let name = ac_l.series().name().to_string();
+        let mut ca: ListChunked = ac_l
+            .iter_groups(false)
+            .zip(ac_r.iter_groups(false))
+            .map(|(l, r)| {
+                match (l, r) {
+                    (Some(l), Some(r)) => {
+                        let l = l.as_ref();
+                        let r = r.as_ref();
+                        Some(apply_operator(l, r, self.op))
                     }
+                    _ => None,
                 }
+                .transpose()
+            })
+            .collect::<PolarsResult<_>>()?;
+        ca.rename(&name);
+
+        // try if we can reuse the groups
+        use AggState::*;
+        match (ac_l.agg_state(), ac_r.agg_state()) {
+            // no need to change update groups
+            (AggregatedList(_), _) => {}
+            // we can take the groups of the rhs
+            (_, AggregatedList(_)) if matches!(ac_r.update_groups, UpdateGroups::No) => {
+                ac_l.groups = ac_r.groups
+            }
+            // we must update the groups
+            _ => {
+                ac_l.with_update_groups(UpdateGroups::WithSeriesLen);
             }
-        } else if matches!(compare_fn_nan_min(entering_min, &self.min), Ordering::Less) {
-            self.min = *entering_min
         }
 
-        self.last_start = start;
-        self.last_end = end;
-        self.min
+        ac_l.with_series(ca.into_series(), true, Some(&self.expr))?;
+        Ok(ac_l)
     }
 }
 
-pub struct MaxWindow<'a, T: NativeType> {
-    slice: &'a [T],
-    max: T,
-    last_start: usize,
-    last_end: usize,
-}
+impl PhysicalExpr for BinaryExpr {
+    fn as_expression(&self) -> Option<&Expr> {
+        Some(&self.expr)
+    }
 
-impl<'a, T: NativeType + IsFloat + PartialOrd> RollingAggWindowNoNulls<'a, T> for MaxWindow<'a, T> {
-    fn new(slice: &'a [T], start: usize, end: usize, _params: DynArgs) -> Self {
-        let max = *slice[start..end]
-            .iter()
-            .max_by(|a, b| compare_fn_nan_max(*a, *b))
-            .unwrap_or(&slice[start]);
-        Self {
-            slice,
-            max,
-            last_start: start,
-            last_end: end,
-        }
+    fn evaluate(&self, df: &DataFrame, state: &ExecutionState) -> PolarsResult<Series> {
+        // window functions may set a global state that determine their output
+        // state, so we don't let them run in parallel as they race
+        // they also saturate the thread pool by themselves, so that's fine
+        let (lhs, rhs) = if state.has_window() {
+            let mut state = state.split();
+            state.remove_cache_window_flag();
+            (
+                self.left.evaluate(df, &state),
+                self.right.evaluate(df, &state),
+            )
+        } else {
+            POOL.install(|| {
+                rayon::join(
+                    || self.left.evaluate(df, state),
+                    || self.right.evaluate(df, state),
+                )
+            })
+        };
+        let lhs = lhs?;
+        let rhs = rhs?;
+        polars_ensure!(
+            lhs.len() == rhs.len() || lhs.len() == 1 || rhs.len() == 1,
+            expr = self.expr,
+            ComputeError: "cannot evaluate two series of different lengths ({} and {})",
+            lhs.len(), rhs.len(),
+        );
+        apply_operator_owned(lhs, rhs, self.op)
     }
 
-    unsafe fn update(&mut self, start: usize, end: usize) -> T {
-        // recompute max
-        if start >= self.last_end
-            // the window only got smaller
-            || end == self.last_end
-        {
-            self.max = *self
-                .slice
-                .get_unchecked(start..end)
-                .iter()
-                .max_by(|a, b| compare_fn_nan_max(*a, *b))
-                .unwrap_or(self.slice.get_unchecked(start));
-
-            self.last_start = start;
-            self.last_end = end;
-
-            return self.max;
-        }
-
-        let mut recompute_max = false;
-        for idx in self.last_start..start {
-            // safety
-            // we are in bounds
-            let leaving_value = self.slice.get_unchecked(idx);
-            // if the leaving value is the max value, we need to recompute the max.
-            if matches!(
-                compare_fn_nan_max(leaving_value, &self.max),
-                Ordering::Equal
-            ) {
-                recompute_max = true;
-                break;
+    #[allow(clippy::ptr_arg)]
+    fn evaluate_on_groups<'a>(
+        &self,
+        df: &DataFrame,
+        groups: &'a GroupsProxy,
+        state: &ExecutionState,
+    ) -> PolarsResult<AggregationContext<'a>> {
+        let (result_a, result_b) = POOL.install(|| {
+            rayon::join(
+                || self.left.evaluate_on_groups(df, groups, state),
+                || self.right.evaluate_on_groups(df, groups, state),
+            )
+        });
+        let mut ac_l = result_a?;
+        let ac_r = result_b?;
+
+        match (ac_l.agg_state(), ac_r.agg_state()) {
+            (
+                AggState::Literal(_) | AggState::NotAggregated(_),
+                AggState::Literal(_) | AggState::NotAggregated(_),
+            ) => self.apply_elementwise(ac_l, ac_r, false),
+            (
+                AggState::AggregatedFlat(_) | AggState::Literal(_),
+                AggState::AggregatedFlat(_) | AggState::Literal(_),
+            ) => self.apply_elementwise(ac_l, ac_r, true),
+            (AggState::AggregatedFlat(_), AggState::NotAggregated(_))
+            | (AggState::NotAggregated(_), AggState::AggregatedFlat(_)) => {
+                self.apply_group_aware(ac_l, ac_r)
+            }
+            (AggState::AggregatedList(lhs), AggState::AggregatedList(rhs)) => {
+                let lhs = lhs.list().unwrap();
+                let rhs = rhs.list().unwrap();
+                let out =
+                    lhs.apply_to_inner(&|lhs| apply_operator(&lhs, &rhs.get_inner(), self.op))?;
+                ac_l.with_series(out.into_series(), true, Some(&self.expr))?;
+                Ok(ac_l)
             }
+            _ => self.apply_group_aware(ac_l, ac_r),
         }
+    }
 
-        let entering_max = self
-            .slice
-            .get_unchecked(self.last_end..end)
-            .iter()
-            .max_by(|a, b| compare_fn_nan_max(*a, *b))
-            .unwrap_or(self.slice.get_unchecked(std::cmp::max(
-                self.last_start,
-                self.last_end.saturating_sub(1),
-            )));
-
-        if recompute_max {
-            match compare_fn_nan_max(&self.max, entering_max) {
-                // do nothing
-                Ordering::Equal => {}
-                // leaving < entering
-                Ordering::Less => {
-                    if matches!(
-                        compare_fn_nan_max(entering_max, &self.max),
-                        Ordering::Greater
-                    ) {
-                        self.max = *entering_max
-                    }
-                }
-                // leaving > entering
-                Ordering::Greater => {
-                    // leaving value could be the largest, we might need to recompute
-
-                    // check the values in between the window we did not yet
-                    // compute to find the max there. We compare that with the `entering_max`
-                    // if any value is equal to equal to `self.max` of previous window we can break
-                    // early
-                    let mut max_in_between = self.slice.get_unchecked(start);
-                    for idx in (start + 1)..self.last_end {
-                        // safety
-                        // we are in bounds
-                        let value = self.slice.get_unchecked(idx);
+    fn to_field(&self, input_schema: &Schema) -> PolarsResult<Field> {
+        self.expr.to_field(input_schema, Context::Default)
+    }
 
-                        if matches!(compare_fn_nan_max(value, max_in_between), Ordering::Greater) {
-                            max_in_between = value;
-                        }
+    fn as_partitioned_aggregator(&self) -> Option<&dyn PartitionedAggregation> {
+        Some(self)
+    }
 
-                        // the max is also in the in between values
-                        if matches!(compare_fn_nan_max(value, &self.max), Ordering::Equal) {
-                            self.last_start = start;
-                            self.last_end = end;
-                            return self.max;
-                        }
-                    }
+    #[cfg(feature = "parquet")]
+    fn as_stats_evaluator(&self) -> Option<&dyn polars_io::predicates::StatsEvaluator> {
+        Some(self)
+    }
 
-                    if matches!(
-                        compare_fn_nan_max(max_in_between, entering_max),
-                        Ordering::Greater
-                    ) {
-                        self.max = *max_in_between
-                    } else {
-                        self.max = *entering_max
-                    }
-                }
-            }
-        } else if matches!(
-            compare_fn_nan_max(entering_max, &self.max),
-            Ordering::Greater
-        ) {
-            self.max = *entering_max
-        }
-        self.last_start = start;
-        self.last_end = end;
-        self.max
+    fn is_valid_aggregation(&self) -> bool {
+        // we don't want:
+        // col(a) == lit(1)
+
+        // we do want
+        // col(a).sum() == lit(1)
+        (!self.left.is_literal() && self.left.is_valid_aggregation())
+            | (!self.right.is_literal() && self.right.is_valid_aggregation())
     }
 }
 
-pub(crate) fn compute_min_weights<T>(values: &[T], weights: &[T]) -> T
-where
-    T: NativeType + PartialOrd + std::ops::Mul<Output = T>,
-{
-    values
-        .iter()
-        .zip(weights)
-        .map(|(v, w)| *v * *w)
-        .min_by(|a, b| a.partial_cmp(b).unwrap())
-        .unwrap()
-}
+#[cfg(feature = "parquet")]
+mod stats {
+    use polars_io::parquet::predicates::BatchStats;
+    use polars_io::predicates::StatsEvaluator;
 
-pub(crate) fn compute_max_weights<T>(values: &[T], weights: &[T]) -> T
-where
-    T: NativeType + PartialOrd + IsFloat + Bounded + Mul<Output = T>,
-{
-    let mut max = T::min_value();
-    for v in values.iter().zip(weights).map(|(v, w)| *v * *w) {
-        if T::is_float() && v.is_nan() {
-            return v;
-        }
-        if v > max {
-            max = v
+    use super::*;
+
+    fn apply_operator_stats_eq(min_max: &Series, literal: &Series) -> bool {
+        // literal is greater than max, don't need to read
+        if ChunkCompare::<&Series>::gt(literal, min_max)
+            .ok()
+            .map(|s| s.all())
+            == Some(true)
+        {
+            return false;
         }
-    }
 
-    max
-}
+        // literal is smaller than min, don't need to read
+        if ChunkCompare::<&Series>::lt(literal, min_max)
+            .ok()
+            .map(|s| s.all())
+            == Some(true)
+        {
+            return false;
+        }
 
-pub fn is_reverse_sorted_max<T: NativeType + PartialOrd + IsFloat>(values: &[T]) -> bool {
-    values
-        .windows(2)
-        .all(|w| match compare_fn_nan_min(&w[0], &w[1]) {
-            Ordering::Equal => true,
-            Ordering::Greater => true,
-            Ordering::Less => false,
-        })
-}
+        true
+    }
 
-pub fn rolling_max<T>(
-    values: &[T],
-    window_size: usize,
-    min_periods: usize,
-    center: bool,
-    weights: Option<&[f64]>,
-    _params: DynArgs,
-) -> ArrayRef
-where
-    T: NativeType + PartialOrd + IsFloat + Bounded + NumCast + Mul<Output = T>,
-{
-    match (center, weights) {
-        (true, None) => {
-            // will be O(n2) if we don't take this path we hope that we hit an early return on not sorted data
-            if is_reverse_sorted_max(values) {
-                rolling_apply_agg_window::<SortedMinMax<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets_center,
-                    None,
-                )
-            } else {
-                rolling_apply_agg_window::<MaxWindow<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets_center,
-                    None,
-                )
+    fn apply_operator_stats_rhs_lit(min_max: &Series, literal: &Series, op: Operator) -> bool {
+        match op {
+            Operator::Eq => apply_operator_stats_eq(min_max, literal),
+            // col > lit
+            // e.g.
+            // [min,
+            // max] > 0
+            //
+            // [-1,
+            // 2] > 0
+            //
+            // [false, true] -> true -> read
+            Operator::Gt => {
+                // literal is bigger than max value
+                // selection needs all rows
+                ChunkCompare::<&Series>::gt(min_max, literal)
+                    .ok()
+                    .map(|s| s.any())
+                    == Some(true)
             }
-        }
-        (false, None) => {
-            if is_reverse_sorted_max(values) {
-                rolling_apply_agg_window::<SortedMinMax<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets,
-                    None,
-                )
-            } else {
-                rolling_apply_agg_window::<MaxWindow<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets,
-                    None,
-                )
+            // col >= lit
+            Operator::GtEq => {
+                // literal is bigger than max value
+                // selection needs all rows
+                ChunkCompare::<&Series>::gt_eq(min_max, literal)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
             }
+            // col < lit
+            Operator::Lt => {
+                // literal is smaller than min value
+                // selection needs all rows
+                ChunkCompare::<&Series>::lt(min_max, literal)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
+            }
+            // col <= lit
+            Operator::LtEq => {
+                // literal is smaller than min value
+                // selection needs all rows
+                ChunkCompare::<&Series>::lt_eq(min_max, literal)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
+            }
+            // default: read the file
+            _ => true,
         }
-        (true, Some(weights)) => {
-            assert!(
-                T::is_float(),
-                "implementation error, should only be reachable by float types"
-            );
-            let weights = weights
-                .iter()
-                .map(|v| NumCast::from(*v).unwrap())
-                .collect::<Vec<_>>();
-            no_nulls::rolling_apply_weights(
-                values,
-                window_size,
-                min_periods,
-                det_offsets_center,
-                compute_max_weights,
-                &weights,
-            )
-        }
-        (false, Some(weights)) => {
-            assert!(
-                T::is_float(),
-                "implementation error, should only be reachable by float types"
-            );
-            let weights = weights
-                .iter()
-                .map(|v| NumCast::from(*v).unwrap())
-                .collect::<Vec<_>>();
-            no_nulls::rolling_apply_weights(
-                values,
-                window_size,
-                min_periods,
-                det_offsets,
-                compute_max_weights,
-                &weights,
-            )
+    }
+
+    fn apply_operator_stats_lhs_lit(literal: &Series, min_max: &Series, op: Operator) -> bool {
+        match op {
+            Operator::Eq => apply_operator_stats_eq(min_max, literal),
+            Operator::Gt => {
+                // literal is bigger than max value
+                // selection needs all rows
+                ChunkCompare::<&Series>::gt(literal, min_max)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
+            }
+            Operator::GtEq => {
+                // literal is bigger than max value
+                // selection needs all rows
+                ChunkCompare::<&Series>::gt_eq(literal, min_max)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
+            }
+            Operator::Lt => {
+                // literal is smaller than min value
+                // selection needs all rows
+                ChunkCompare::<&Series>::lt(literal, min_max)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
+            }
+            Operator::LtEq => {
+                // literal is smaller than min value
+                // selection needs all rows
+                ChunkCompare::<&Series>::lt_eq(literal, min_max)
+                    .ok()
+                    .map(|ca| ca.any())
+                    == Some(true)
+            }
+            // default: read the file
+            _ => true,
         }
     }
-}
 
-pub fn is_sorted_min<T: NativeType + PartialOrd + IsFloat>(values: &[T]) -> bool {
-    values
-        .windows(2)
-        .all(|w| match compare_fn_nan_min(&w[0], &w[1]) {
-            Ordering::Equal => true,
-            Ordering::Less => true,
-            Ordering::Greater => false,
-        })
-}
+    impl BinaryExpr {
+        fn impl_should_read(&self, stats: &BatchStats) -> PolarsResult<bool> {
+            // See: #5864 for the rationale behind this.
+            use Expr::*;
+            use Operator::*;
+            if !self.expr.into_iter().all(|e| match e {
+                BinaryExpr { op, .. } => !matches!(
+                    op,
+                    Multiply | Divide | TrueDivide | FloorDivide | Modulus | NotEq
+                ),
+                Column(_) | Literal(_) | Alias(_, _) => true,
+                _ => false,
+            }) {
+                return Ok(true);
+            }
 
-pub fn rolling_min<T>(
-    values: &[T],
-    window_size: usize,
-    min_periods: usize,
-    center: bool,
-    weights: Option<&[f64]>,
-    _params: DynArgs,
-) -> ArrayRef
-where
-    T: NativeType + PartialOrd + NumCast + Mul<Output = T> + Bounded + IsFloat,
-{
-    match (center, weights) {
-        (true, None) => {
-            // will be O(n2) if we don't take this path we hope that we hit an early return on not sorted data
-            if is_sorted_min(values) {
-                rolling_apply_agg_window::<SortedMinMax<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets_center,
-                    None,
-                )
-            } else {
-                rolling_apply_agg_window::<MinWindow<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets_center,
-                    None,
-                )
+            let schema = stats.schema();
+            let fld_l = self.left.to_field(schema)?;
+            let fld_r = self.right.to_field(schema)?;
+
+            #[cfg(debug_assertions)]
+            {
+                match (fld_l.data_type(), fld_r.data_type()) {
+                    #[cfg(feature = "dtype-categorical")]
+                    (DataType::Utf8, DataType::Categorical(_)) => {}
+                    #[cfg(feature = "dtype-categorical")]
+                    (DataType::Categorical(_), DataType::Utf8) => {}
+                    (l, r) if l != r => panic!("implementation error: {l:?}, {r:?}"),
+                    _ => {}
+                }
             }
+
+            let dummy = DataFrame::new_no_checks(vec![]);
+            let state = ExecutionState::new();
+
+            let out = match (self.left.is_literal(), self.right.is_literal()) {
+                (false, true) => {
+                    let l = stats.get_stats(fld_l.name())?;
+                    match l.to_min_max() {
+                        None => Ok(true),
+                        Some(min_max_s) => {
+                            // will be incorrect if not
+                            debug_assert_eq!(min_max_s.null_count(), 0);
+                            let lit_s = self.right.evaluate(&dummy, &state).unwrap();
+                            Ok(apply_operator_stats_rhs_lit(&min_max_s, &lit_s, self.op))
+                        }
+                    }
+                }
+                (true, false) => {
+                    let r = stats.get_stats(fld_r.name())?;
+                    match r.to_min_max() {
+                        None => Ok(true),
+                        Some(min_max_s) => {
+                            // will be incorrect if not
+                            debug_assert_eq!(min_max_s.null_count(), 0);
+                            let lit_s = self.left.evaluate(&dummy, &state).unwrap();
+                            Ok(apply_operator_stats_lhs_lit(&lit_s, &min_max_s, self.op))
+                        }
+                    }
+                }
+                // default: read the file
+                _ => Ok(true),
+            };
+            out.map(|read| {
+                if state.verbose() && read {
+                    eprintln!("parquet file must be read, statistics not sufficient for predicate.")
+                } else if state.verbose() && !read {
+                    eprintln!("parquet file can be skipped, the statistics were sufficient to apply the predicate.")
+                };
+                read
+            })
         }
-        (false, None) => {
-            // will be O(n2)
-            if is_sorted_min(values) {
-                rolling_apply_agg_window::<SortedMinMax<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets,
-                    None,
-                )
-            } else {
-                rolling_apply_agg_window::<MinWindow<_>, _, _>(
-                    values,
-                    window_size,
-                    min_periods,
-                    det_offsets,
-                    None,
-                )
+    }
+
+    impl StatsEvaluator for BinaryExpr {
+        fn should_read(&self, stats: &BatchStats) -> PolarsResult<bool> {
+            if std::env::var("POLARS_NO_PARQUET_STATISTICS").is_ok() {
+                return Ok(true);
+            }
+
+            match (
+                self.left.as_stats_evaluator(),
+                self.right.as_stats_evaluator(),
+            ) {
+                (Some(l), Some(r)) => match self.op {
+                    Operator::And => Ok(l.should_read(stats)? && r.should_read(stats)?),
+                    Operator::Or => Ok(l.should_read(stats)? || r.should_read(stats)?),
+                    _ => Ok(true),
+                },
+                _ => self.impl_should_read(stats),
             }
-        }
-        (true, Some(weights)) => {
-            assert!(
-                T::is_float(),
-                "implementation error, should only be reachable by float types"
-            );
-            let weights = weights
-                .iter()
-                .map(|v| NumCast::from(*v).unwrap())
-                .collect::<Vec<_>>();
-            no_nulls::rolling_apply_weights(
-                values,
-                window_size,
-                min_periods,
-                det_offsets_center,
-                compute_min_weights,
-                &weights,
-            )
-        }
-        (false, Some(weights)) => {
-            assert!(
-                T::is_float(),
-                "implementation error, should only be reachable by float types"
-            );
-            let weights = weights
-                .iter()
-                .map(|v| NumCast::from(*v).unwrap())
-                .collect::<Vec<_>>();
-            no_nulls::rolling_apply_weights(
-                values,
-                window_size,
-                min_periods,
-                det_offsets,
-                compute_min_weights,
-                &weights,
-            )
         }
     }
 }
 
-#[cfg(test)]
-mod test {
-    use super::*;
-
-    #[test]
-    fn test_rolling_min_max() {
-        let values = &[1.0f64, 5.0, 3.0, 4.0];
-
-        let out = rolling_min(values, 2, 2, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        assert_eq!(out, &[None, Some(1.0), Some(3.0), Some(3.0)]);
-        let out = rolling_max(values, 2, 2, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        assert_eq!(out, &[None, Some(5.0), Some(5.0), Some(4.0)]);
-
-        let out = rolling_min(values, 2, 1, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        assert_eq!(out, &[Some(1.0), Some(1.0), Some(3.0), Some(3.0)]);
-        let out = rolling_max(values, 2, 1, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        assert_eq!(out, &[Some(1.0), Some(5.0), Some(5.0), Some(4.0)]);
-
-        let out = rolling_max(values, 3, 1, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        assert_eq!(out, &[Some(1.0), Some(5.0), Some(5.0), Some(5.0)]);
-
-        // test nan handling.
-        let values = &[1.0, 2.0, 3.0, f64::nan(), 5.0, 6.0, 7.0];
-        let out = rolling_min(values, 3, 3, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        // we cannot compare nans, so we compare the string values
-        assert_eq!(
-            format!("{:?}", out.as_slice()),
-            format!(
-                "{:?}",
-                &[
-                    None,
-                    None,
-                    Some(1.0),
-                    Some(f64::nan()),
-                    Some(f64::nan()),
-                    Some(f64::nan()),
-                    Some(5.0)
-                ]
-            )
-        );
+impl PartitionedAggregation for BinaryExpr {
+    fn evaluate_partitioned(
+        &self,
+        df: &DataFrame,
+        groups: &GroupsProxy,
+        state: &ExecutionState,
+    ) -> PolarsResult<Series> {
+        let left = self.left.as_partitioned_aggregator().unwrap();
+        let right = self.right.as_partitioned_aggregator().unwrap();
+        let left = left.evaluate_partitioned(df, groups, state)?;
+        let right = right.evaluate_partitioned(df, groups, state)?;
+        apply_operator(&left, &right, self.op)
+    }
 
-        let out = rolling_max(values, 3, 3, false, None, None);
-        let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
-        let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
-        assert_eq!(
-            format!("{:?}", out.as_slice()),
-            format!(
-                "{:?}",
-                &[
-                    None,
-                    None,
-                    Some(3.0),
-                    Some(f64::nan()),
-                    Some(f64::nan()),
-                    Some(f64::nan()),
-                    Some(7.0)
-                ]
-            )
-        );
+    fn finalize(
+        &self,
+        partitioned: Series,
+        _groups: &GroupsProxy,
+        _state: &ExecutionState,
+    ) -> PolarsResult<Series> {
+        Ok(partitioned)
     }
 }
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 pub use quantile::*;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 pub use sum::*;
 pub use variance::*;
 
 use super::*;
+use crate::error::{polars_bail, PolarsResult};
 use crate::utils::CustomIterTools;
 
 pub trait RollingAggWindowNoNulls<'a, T: NativeType> {
     fn new(slice: &'a [T], start: usize, end: usize, params: DynArgs) -> Self;
 
     /// Update and recompute the window
     /// # Safety
@@ -33,15 +34,15 @@
 // Use an aggregation window that maintains the state
 pub(super) fn rolling_apply_agg_window<'a, Agg, T, Fo>(
     values: &'a [T],
     window_size: usize,
     min_periods: usize,
     det_offsets_fn: Fo,
     params: DynArgs,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     Fo: Fn(Idx, WindowSize, Len) -> (Start, End),
     Agg: RollingAggWindowNoNulls<'a, T>,
     T: Debug + IsFloat + NativeType,
 {
     let len = values.len();
     let (start, end) = det_offsets_fn(0, window_size, len);
@@ -53,19 +54,19 @@
             // safety:
             // we are in bounds
             unsafe { agg_window.update(start, end) }
         })
         .collect_trusted::<Vec<_>>();
 
     let validity = create_validity(min_periods, len, window_size, det_offsets_fn);
-    Box::new(PrimitiveArray::new(
+    Ok(Box::new(PrimitiveArray::new(
         T::PRIMITIVE.into(),
         out.into(),
         validity.map(|b| b.into()),
-    ))
+    )))
 }
 
 #[derive(Clone, Copy, PartialEq, Eq, Debug, Default)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub enum QuantileInterpolOptions {
     #[default]
     Nearest,
@@ -78,15 +79,15 @@
 pub(super) fn rolling_apply_weights<T, Fo, Fa>(
     values: &[T],
     window_size: usize,
     min_periods: usize,
     det_offsets_fn: Fo,
     aggregator: Fa,
     weights: &[T],
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType,
     Fo: Fn(Idx, WindowSize, Len) -> (Start, End),
     Fa: Fn(&[T], &[T]) -> T,
 {
     assert_eq!(weights.len(), window_size);
     let len = values.len();
@@ -96,19 +97,19 @@
             let vals = unsafe { values.get_unchecked(start..end) };
 
             aggregator(vals, weights)
         })
         .collect_trusted::<Vec<T>>();
 
     let validity = create_validity(min_periods, len, window_size, det_offsets_fn);
-    Box::new(PrimitiveArray::new(
+    Ok(Box::new(PrimitiveArray::new(
         DataType::from(T::PRIMITIVE),
         out.into(),
         validity.map(|b| b.into()),
-    ))
+    )))
 }
 
 fn compute_var_weights<T>(vals: &[T], weights: &[T]) -> T
 where
     T: Float + std::ops::AddAssign,
 {
     let weighted_iter = vals.iter().zip(weights).map(|(x, y)| *x * *y);
@@ -123,21 +124,14 @@
     let count = NumCast::from(vals.len()).unwrap();
 
     let mean = sum / count;
     // apply Bessel's correction
     ((sum_of_squares / count) - mean * mean) / (count - T::one()) * count
 }
 
-pub(crate) fn compute_mean_weights<T>(values: &[T], weights: &[T]) -> T
-where
-    T: Float + std::iter::Sum<T>,
-{
-    values.iter().zip(weights).map(|(v, w)| *v * *w).sum::<T>() / T::from(values.len()).unwrap()
-}
-
 pub(crate) fn compute_sum_weights<T>(values: &[T], weights: &[T]) -> T
 where
     T: std::iter::Sum<T> + Copy + std::ops::Mul<Output = T>,
 {
     values.iter().zip(weights).map(|(v, w)| *v * *w).sum()
 }
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files 2% similar despite different names*

```diff
@@ -121,37 +121,37 @@
 pub fn rolling_median<T>(
     values: &[T],
     window_size: usize,
     min_periods: usize,
     center: bool,
     weights: Option<&[f64]>,
     _params: DynArgs,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType
         + std::iter::Sum<T>
         + PartialOrd
         + ToPrimitive
         + NumCast
         + Add<Output = T>
         + Sub<Output = T>
         + Div<Output = T>
         + Mul<Output = T>
         + Zero
         + IsFloat,
 {
-    rolling_quantile(
+    Ok(rolling_quantile(
         values,
         0.5,
         QuantileInterpolOptions::Linear,
         window_size,
         min_periods,
         center,
         weights,
-    )
+    ))
 }
 
 pub fn rolling_quantile<T>(
     values: &[T],
     quantile: f64,
     interpolation: QuantileInterpolOptions,
     window_size: usize,
@@ -375,23 +375,23 @@
             QuantileInterpolOptions::Higher,
             QuantileInterpolOptions::Nearest,
             QuantileInterpolOptions::Midpoint,
             QuantileInterpolOptions::Linear,
         ];
 
         for interpol in interpol_options {
-            let out1 = rolling_min(values, 2, 2, false, None, None);
+            let out1 = rolling_min(values, 2, 2, false, None, None).unwrap();
             let out1 = out1.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
             let out1 = out1.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
             let out2 = rolling_quantile(values, 0.0, interpol, 2, 2, false, None);
             let out2 = out2.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
             let out2 = out2.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
             assert_eq!(out1, out2);
 
-            let out1 = rolling_max(values, 2, 2, false, None, None);
+            let out1 = rolling_max(values, 2, 2, false, None, None).unwrap();
             let out1 = out1.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
             let out1 = out1.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
             let out2 = rolling_quantile(values, 1.0, interpol, 2, 2, false, None);
             let out2 = out2.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
             let out2 = out2.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
             assert_eq!(out1, out2);
         }
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files 7% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 pub fn rolling_sum<T>(
     values: &[T],
     window_size: usize,
     min_periods: usize,
     center: bool,
     weights: Option<&[f64]>,
     _params: DynArgs,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType + std::iter::Sum + NumCast + Mul<Output = T> + AddAssign + SubAssign + IsFloat,
 {
     match (center, weights) {
         (true, None) => rolling_apply_agg_window::<SumWindow<_>, _, _>(
             values,
             window_size,
@@ -121,42 +121,42 @@
 #[cfg(test)]
 mod test {
     use super::*;
     #[test]
     fn test_rolling_sum() {
         let values = &[1.0f64, 2.0, 3.0, 4.0];
 
-        let out = rolling_sum(values, 2, 2, false, None, None);
+        let out = rolling_sum(values, 2, 2, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[None, Some(3.0), Some(5.0), Some(7.0)]);
 
-        let out = rolling_sum(values, 2, 1, false, None, None);
+        let out = rolling_sum(values, 2, 1, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[Some(1.0), Some(3.0), Some(5.0), Some(7.0)]);
 
-        let out = rolling_sum(values, 4, 1, false, None, None);
+        let out = rolling_sum(values, 4, 1, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[Some(1.0), Some(3.0), Some(6.0), Some(10.0)]);
 
-        let out = rolling_sum(values, 4, 1, true, None, None);
+        let out = rolling_sum(values, 4, 1, true, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[Some(3.0), Some(6.0), Some(10.0), Some(9.0)]);
 
-        let out = rolling_sum(values, 4, 4, true, None, None);
+        let out = rolling_sum(values, 4, 4, true, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[None, None, Some(10.0), None]);
 
         // test nan handling.
         let values = &[1.0, 2.0, 3.0, f64::nan(), 5.0, 6.0, 7.0];
-        let out = rolling_sum(values, 3, 3, false, None, None);
+        let out = rolling_sum(values, 3, 3, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
 
         assert_eq!(
             format!("{:?}", out.as_slice()),
             format!(
                 "{:?}",
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 pub fn rolling_var<T>(
     values: &[T],
     window_size: usize,
     min_periods: usize,
     center: bool,
     weights: Option<&[f64]>,
     params: DynArgs,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType
         + Float
         + IsFloat
         + std::iter::Sum
         + AddAssign
         + SubAssign
@@ -234,15 +234,15 @@
 pub fn rolling_std<T>(
     values: &[T],
     window_size: usize,
     min_periods: usize,
     center: bool,
     weights: Option<&[f64]>,
     params: DynArgs,
-) -> ArrayRef
+) -> PolarsResult<ArrayRef>
 where
     T: NativeType
         + Float
         + IsFloat
         + std::iter::Sum
         + AddAssign
         + SubAssign
@@ -278,39 +278,39 @@
 mod test {
     use super::*;
 
     #[test]
     fn test_rolling_var() {
         let values = &[1.0f64, 5.0, 3.0, 4.0];
 
-        let out = rolling_var(values, 2, 2, false, None, None);
+        let out = rolling_var(values, 2, 2, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[None, Some(8.0), Some(2.0), Some(0.5)]);
 
         let testpars = Some(Arc::new(RollingVarParams { ddof: 0 }) as Arc<dyn Any + Send + Sync>);
-        let out = rolling_var(values, 2, 2, false, None, testpars);
+        let out = rolling_var(values, 2, 2, false, None, testpars).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[None, Some(4.0), Some(1.0), Some(0.25)]);
 
-        let out = rolling_var(values, 2, 1, false, None, None);
+        let out = rolling_var(values, 2, 1, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out
             .into_iter()
             .map(|v| v.copied().unwrap())
             .collect::<Vec<_>>();
         // we cannot compare nans, so we compare the string values
         assert_eq!(
             format!("{:?}", out.as_slice()),
             format!("{:?}", &[0.0, 8.0, 2.0, 0.5])
         );
         // test nan handling.
         let values = &[-10.0, 2.0, 3.0, f64::nan(), 5.0, 6.0, 7.0];
-        let out = rolling_var(values, 3, 3, false, None, None);
+        let out = rolling_var(values, 3, 3, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         // we cannot compare nans, so we compare the string values
         assert_eq!(
             format!("{:?}", out.as_slice()),
             format!(
                 "{:?}",
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,16 @@
             Some(Bitmap::from(&[true, true, true, true])),
         );
         let out = rolling_max(arr, 2, 1, false, None, None);
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[Some(4.0), Some(4.0), Some(3.0), Some(2.0)]);
 
-        let out = super::no_nulls::rolling_max(arr.values().as_slice(), 2, 1, false, None, None);
+        let out =
+            super::no_nulls::rolling_max(arr.values().as_slice(), 2, 1, false, None, None).unwrap();
         let out = out.as_any().downcast_ref::<PrimitiveArray<f64>>().unwrap();
         let out = out.into_iter().map(|v| v.copied()).collect::<Vec<_>>();
         assert_eq!(out, &[Some(4.0), Some(4.0), Some(3.0), Some(2.0)]);
     }
 
     #[test]
     fn test_rolling_extrema_nulls() {
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/json/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/json/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ndjson/buffer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/ndjson/core.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/ndjson/core.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/arity.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/array.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/expr_dyn_fn.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/array.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files 16% similar despite different names*

```diff
@@ -18,7 +18,11 @@
     s.diff(n, null_behavior)
 }
 
 #[cfg(feature = "interpolate")]
 pub(super) fn interpolate(s: &Series, method: InterpolationMethod) -> PolarsResult<Series> {
     Ok(polars_ops::prelude::interpolate(s, method))
 }
+
+pub(super) fn to_physical(s: &Series) -> PolarsResult<Series> {
+    Ok(s.to_physical_repr().into_owned())
+}
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
     #[cfg(feature = "fused")]
     Fused(fused::FusedOperator),
     ConcatExpr(bool),
     Correlation {
         method: correlation::CorrelationMethod,
         ddof: u8,
     },
+    ToPhysical,
 }
 
 impl Display for FunctionExpr {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         use FunctionExpr::*;
 
         let s = match self {
@@ -274,14 +275,15 @@
             LowerBound => "lower_bound",
             #[cfg(feature = "fused")]
             Fused(fused) => return Display::fmt(fused, f),
             #[cfg(feature = "dtype-array")]
             ArrayExpr(af) => return Display::fmt(af, f),
             ConcatExpr(_) => "concat_expr",
             Correlation { method, .. } => return Display::fmt(method, f),
+            ToPhysical => "to_physical",
         };
         write!(f, "{s}")
     }
 }
 
 #[macro_export]
 macro_rules! wrap {
@@ -492,14 +494,15 @@
             Ceil => map!(round::ceil),
             UpperBound => map!(bounds::upper_bound),
             LowerBound => map!(bounds::lower_bound),
             #[cfg(feature = "fused")]
             Fused(op) => map_as_slice!(fused::fused, op),
             ConcatExpr(rechunk) => map_as_slice!(concat::concat_expr, rechunk),
             Correlation { method, ddof } => map_as_slice!(correlation::corr, ddof, method),
+            ToPhysical => map!(dispatch::to_physical),
         }
     }
 }
 
 #[cfg(feature = "strings")]
 impl From<StringFunction> for SpecialEq<Arc<dyn SeriesUdf>> {
     fn from(func: StringFunction) -> Self {
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files 2% similar despite different names*

```diff
@@ -198,14 +198,15 @@
             #[cfg(feature = "round_series")]
             Round { .. } | Floor | Ceil => mapper.with_same_dtype(),
             UpperBound | LowerBound => mapper.with_same_dtype(),
             #[cfg(feature = "fused")]
             Fused(_) => mapper.map_to_supertype(),
             ConcatExpr(_) => mapper.map_to_supertype(),
             Correlation { .. } => mapper.map_to_float_dtype(),
+            ToPhysical => mapper.to_physical_type(),
         }
     }
 }
 
 pub(super) struct FieldsMapper<'a> {
     fields: &'a [Field],
 }
@@ -231,14 +232,19 @@
     pub(super) fn map_to_float_dtype(&self) -> PolarsResult<Field> {
         self.map_dtype(|dtype| match dtype {
             DataType::Float32 => DataType::Float32,
             _ => DataType::Float64,
         })
     }
 
+    /// Map to a physical type.
+    pub(super) fn to_physical_type(&self) -> PolarsResult<Field> {
+        self.map_dtype(|dtype| dtype.to_physical())
+    }
+
     /// Map a single dtype with a potentially failing mapper function.
     #[cfg(any(feature = "timezones", feature = "dtype-array"))]
     pub(super) fn try_map_dtype(
         &self,
         func: impl Fn(&DataType) -> PolarsResult<DataType>,
     ) -> PolarsResult<Field> {
         let dtype = func(self.fields[0].data_type())?;
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/arity.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/coerce.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/coerce.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/concat.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/concat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/correlation.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/correlation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/horizontal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/index.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/range.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/selectors.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/selectors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/syntactic_sugar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/functions/temporal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/functions/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1763,14 +1763,18 @@
 
     #[cfg(feature = "row_hash")]
     /// Compute the hash of every element
     pub fn hash(self, k0: u64, k1: u64, k2: u64, k3: u64) -> Expr {
         self.map_private(FunctionExpr::Hash(k0, k1, k2, k3))
     }
 
+    pub fn to_physical(self) -> Expr {
+        self.map_private(FunctionExpr::ToPhysical)
+    }
+
     #[cfg(feature = "strings")]
     pub fn str(self) -> string::StringNameSpace {
         string::StringNameSpace(self)
     }
 
     pub fn binary(self) -> binary::BinaryNameSpace {
         binary::BinaryNameSpace(self)
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/selector.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/selector.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/fused.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,487 +1,557 @@
+use std::any::Any;
+use std::borrow::Cow;
+#[cfg(feature = "temporal")]
 use std::sync::Arc;
 
-use polars_core::frame::groupby::GroupsProxy;
-use polars_core::prelude::*;
-use polars_core::POOL;
+use polars_arrow::prelude::QuantileInterpolOptions;
 
-use crate::physical_plan::state::ExecutionState;
+#[cfg(feature = "object")]
+use crate::chunked_array::object::PolarsObjectSafe;
+pub use crate::prelude::ChunkCompare;
 use crate::prelude::*;
 
-pub struct BinaryExpr {
-    pub(crate) left: Arc<dyn PhysicalExpr>,
-    pub(crate) op: Operator,
-    pub(crate) right: Arc<dyn PhysicalExpr>,
-    expr: Expr,
+#[derive(Debug, Copy, Clone, Eq, PartialEq)]
+pub enum IsSorted {
+    Ascending,
+    Descending,
+    Not,
 }
 
-impl BinaryExpr {
-    pub fn new(
-        left: Arc<dyn PhysicalExpr>,
-        op: Operator,
-        right: Arc<dyn PhysicalExpr>,
-        expr: Expr,
-    ) -> Self {
-        Self {
-            left,
-            op,
-            right,
-            expr,
+impl IsSorted {
+    pub(crate) fn reverse(self) -> Self {
+        use IsSorted::*;
+        match self {
+            Ascending => Descending,
+            Descending => Ascending,
+            Not => Not,
         }
     }
 }
 
-/// Can partially do operations in place.
-fn apply_operator_owned(left: Series, right: Series, op: Operator) -> PolarsResult<Series> {
-    match op {
-        Operator::Plus => Ok(left + right),
-        Operator::Minus => Ok(left - right),
-        Operator::Multiply => Ok(left * right),
-        _ => apply_operator(&left, &right, op),
-    }
+macro_rules! invalid_operation_panic {
+    ($op:ident, $s:expr) => {
+        panic!(
+            "`{}` operation not supported for dtype `{}`",
+            stringify!($op),
+            $s._dtype()
+        )
+    };
 }
 
-pub fn apply_operator(left: &Series, right: &Series, op: Operator) -> PolarsResult<Series> {
-    use DataType::*;
-    match op {
-        Operator::Gt => ChunkCompare::<&Series>::gt(left, right).map(|ca| ca.into_series()),
-        Operator::GtEq => ChunkCompare::<&Series>::gt_eq(left, right).map(|ca| ca.into_series()),
-        Operator::Lt => ChunkCompare::<&Series>::lt(left, right).map(|ca| ca.into_series()),
-        Operator::LtEq => ChunkCompare::<&Series>::lt_eq(left, right).map(|ca| ca.into_series()),
-        Operator::Eq => ChunkCompare::<&Series>::equal(left, right).map(|ca| ca.into_series()),
-        Operator::NotEq => {
-            ChunkCompare::<&Series>::not_equal(left, right).map(|ca| ca.into_series())
-        }
-        Operator::Plus => Ok(left + right),
-        Operator::Minus => Ok(left - right),
-        Operator::Multiply => Ok(left * right),
-        Operator::Divide => Ok(left / right),
-        Operator::TrueDivide => match left.dtype() {
-            #[cfg(feature = "dtype-decimal")]
-            Decimal(_, _) => Ok(left / right),
-            Date | Datetime(_, _) | Float32 | Float64 => Ok(left / right),
-            _ => Ok(&left.cast(&Float64)? / &right.cast(&Float64)?),
-        },
-        Operator::FloorDivide => {
-            #[cfg(feature = "round_series")]
-            {
-                floor_div_series(left, right)
-            }
-            #[cfg(not(feature = "round_series"))]
-            {
-                panic!("activate 'round_series' feature")
-            }
-        }
-        Operator::And => left.bitand(right),
-        Operator::Or => left.bitor(right),
-        Operator::Xor => left.bitxor(right),
-        Operator::Modulus => Ok(left % right),
-        Operator::EqValidity => left.equal_missing(right).map(|ca| ca.into_series()),
-        Operator::NotEqValidity => left.not_equal_missing(right).map(|ca| ca.into_series()),
+pub(crate) mod private {
+    use ahash::RandomState;
+
+    use super::*;
+    use crate::chunked_array::ops::compare_inner::{PartialEqInner, PartialOrdInner};
+    #[cfg(feature = "rows")]
+    use crate::frame::groupby::GroupsProxy;
+
+    pub trait PrivateSeriesNumeric {
+        fn bit_repr_is_large(&self) -> bool {
+            false
+        }
+        fn bit_repr_large(&self) -> UInt64Chunked {
+            unimplemented!()
+        }
+        fn bit_repr_small(&self) -> UInt32Chunked {
+            unimplemented!()
+        }
     }
-}
 
-impl BinaryExpr {
-    fn apply_elementwise<'a>(
-        &self,
-        mut ac_l: AggregationContext<'a>,
-        ac_r: AggregationContext,
-        aggregated: bool,
-    ) -> PolarsResult<AggregationContext<'a>> {
-        // we want to be able to mutate in place
-        // so we take the lhs to make sure that we drop
-        let lhs = ac_l.series().clone();
-        let rhs = ac_r.series().clone();
+    pub trait PrivateSeries {
+        #[cfg(feature = "object")]
+        fn get_list_builder(
+            &self,
+            _name: &str,
+            _values_capacity: usize,
+            _list_capacity: usize,
+        ) -> Box<dyn ListBuilderTrait> {
+            invalid_operation_panic!(get_list_builder, self)
+        }
+
+        /// Get field (used in schema)
+        fn _field(&self) -> Cow<Field>;
+
+        fn _dtype(&self) -> &DataType;
+
+        fn compute_len(&mut self);
 
-        // drop lhs so that we might operate in place
-        {
-            let _ = ac_l.take();
+        fn explode_by_offsets(&self, _offsets: &[i64]) -> Series {
+            invalid_operation_panic!(explode_by_offsets, self)
         }
 
-        let out = apply_operator_owned(lhs, rhs, self.op)?;
+        /// Get an array with the cumulative max computed at every element
+        #[cfg(feature = "cum_agg")]
+        fn _cummax(&self, _reverse: bool) -> Series {
+            panic!("operation cummax not supported for this dtype")
+        }
 
-        ac_l.with_series(out, aggregated, Some(&self.expr))?;
-        Ok(ac_l)
-    }
+        /// Get an array with the cumulative min computed at every element
+        #[cfg(feature = "cum_agg")]
+        fn _cummin(&self, _reverse: bool) -> Series {
+            panic!("operation cummin not supported for this dtype")
+        }
 
-    fn apply_group_aware<'a>(
-        &self,
-        mut ac_l: AggregationContext<'a>,
-        mut ac_r: AggregationContext<'a>,
-    ) -> PolarsResult<AggregationContext<'a>> {
-        let name = ac_l.series().name().to_string();
-        let mut ca: ListChunked = ac_l
-            .iter_groups(false)
-            .zip(ac_r.iter_groups(false))
-            .map(|(l, r)| {
-                match (l, r) {
-                    (Some(l), Some(r)) => {
-                        let l = l.as_ref();
-                        let r = r.as_ref();
-                        Some(apply_operator(l, r, self.op))
-                    }
-                    _ => None,
-                }
-                .transpose()
-            })
-            .collect::<PolarsResult<_>>()?;
-        ca.rename(&name);
-
-        // try if we can reuse the groups
-        use AggState::*;
-        match (ac_l.agg_state(), ac_r.agg_state()) {
-            // no need to change update groups
-            (AggregatedList(_), _) => {}
-            // we can take the groups of the rhs
-            (_, AggregatedList(_)) if matches!(ac_r.update_groups, UpdateGroups::No) => {
-                ac_l.groups = ac_r.groups
-            }
-            // we must update the groups
-            _ => {
-                ac_l.with_update_groups(UpdateGroups::WithSeriesLen);
-            }
+        fn _set_sorted_flag(&mut self, _is_sorted: IsSorted) {
+            // ignore
         }
 
-        ac_l.with_series(ca.into_series(), true, Some(&self.expr))?;
-        Ok(ac_l)
+        unsafe fn equal_element(
+            &self,
+            _idx_self: usize,
+            _idx_other: usize,
+            _other: &Series,
+        ) -> bool {
+            invalid_operation_panic!(equal_element, self)
+        }
+        #[allow(clippy::wrong_self_convention)]
+        fn into_partial_eq_inner<'a>(&'a self) -> Box<dyn PartialEqInner + 'a> {
+            invalid_operation_panic!(into_partial_eq_inner, self)
+        }
+        #[allow(clippy::wrong_self_convention)]
+        fn into_partial_ord_inner<'a>(&'a self) -> Box<dyn PartialOrdInner + 'a> {
+            invalid_operation_panic!(into_partial_ord_inner, self)
+        }
+        fn vec_hash(&self, _build_hasher: RandomState, _buf: &mut Vec<u64>) -> PolarsResult<()> {
+            polars_bail!(opq = vec_hash, self._dtype());
+        }
+        fn vec_hash_combine(
+            &self,
+            _build_hasher: RandomState,
+            _hashes: &mut [u64],
+        ) -> PolarsResult<()> {
+            polars_bail!(opq = vec_hash_combine, self._dtype());
+        }
+        unsafe fn agg_min(&self, groups: &GroupsProxy) -> Series {
+            Series::full_null(self._field().name(), groups.len(), self._dtype())
+        }
+        unsafe fn agg_max(&self, groups: &GroupsProxy) -> Series {
+            Series::full_null(self._field().name(), groups.len(), self._dtype())
+        }
+        /// If the [`DataType`] is one of `{Int8, UInt8, Int16, UInt16}` the `Series` is
+        /// first cast to `Int64` to prevent overflow issues.
+        unsafe fn agg_sum(&self, groups: &GroupsProxy) -> Series {
+            Series::full_null(self._field().name(), groups.len(), self._dtype())
+        }
+        unsafe fn agg_std(&self, groups: &GroupsProxy, _ddof: u8) -> Series {
+            Series::full_null(self._field().name(), groups.len(), self._dtype())
+        }
+        unsafe fn agg_var(&self, groups: &GroupsProxy, _ddof: u8) -> Series {
+            Series::full_null(self._field().name(), groups.len(), self._dtype())
+        }
+        unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
+            Series::full_null(self._field().name(), groups.len(), self._dtype())
+        }
+
+        fn zip_outer_join_column(
+            &self,
+            _right_column: &Series,
+            _opt_join_tuples: &[(Option<IdxSize>, Option<IdxSize>)],
+        ) -> Series {
+            invalid_operation_panic!(zip_outer_join_column, self)
+        }
+
+        fn subtract(&self, _rhs: &Series) -> PolarsResult<Series> {
+            invalid_operation_panic!(sub, self)
+        }
+        fn add_to(&self, _rhs: &Series) -> PolarsResult<Series> {
+            invalid_operation_panic!(add, self)
+        }
+        fn multiply(&self, _rhs: &Series) -> PolarsResult<Series> {
+            invalid_operation_panic!(mul, self)
+        }
+        fn divide(&self, _rhs: &Series) -> PolarsResult<Series> {
+            invalid_operation_panic!(div, self)
+        }
+        fn remainder(&self, _rhs: &Series) -> PolarsResult<Series> {
+            invalid_operation_panic!(rem, self)
+        }
+        fn group_tuples(&self, _multithreaded: bool, _sorted: bool) -> PolarsResult<GroupsProxy> {
+            invalid_operation_panic!(group_tuples, self)
+        }
+        #[cfg(feature = "zip_with")]
+        fn zip_with_same_type(
+            &self,
+            _mask: &BooleanChunked,
+            _other: &Series,
+        ) -> PolarsResult<Series> {
+            invalid_operation_panic!(zip_with_same_type, self)
+        }
+
+        fn arg_sort_multiple(&self, _options: &SortMultipleOptions) -> PolarsResult<IdxCa> {
+            polars_bail!(opq = arg_sort_multiple, self._dtype());
+        }
     }
 }
 
-impl PhysicalExpr for BinaryExpr {
-    fn as_expression(&self) -> Option<&Expr> {
-        Some(&self.expr)
-    }
-
-    fn evaluate(&self, df: &DataFrame, state: &ExecutionState) -> PolarsResult<Series> {
-        // window functions may set a global state that determine their output
-        // state, so we don't let them run in parallel as they race
-        // they also saturate the thread pool by themselves, so that's fine
-        let (lhs, rhs) = if state.has_window() {
-            let mut state = state.split();
-            state.remove_cache_window_flag();
-            (
-                self.left.evaluate(df, &state),
-                self.right.evaluate(df, &state),
-            )
-        } else {
-            POOL.install(|| {
-                rayon::join(
-                    || self.left.evaluate(df, state),
-                    || self.right.evaluate(df, state),
-                )
-            })
-        };
-        let lhs = lhs?;
-        let rhs = rhs?;
-        polars_ensure!(
-            lhs.len() == rhs.len() || lhs.len() == 1 || rhs.len() == 1,
-            expr = self.expr,
-            ComputeError: "cannot evaluate two series of different lengths ({} and {})",
-            lhs.len(), rhs.len(),
-        );
-        apply_operator_owned(lhs, rhs, self.op)
+pub trait SeriesTrait:
+    Send + Sync + private::PrivateSeries + private::PrivateSeriesNumeric
+{
+    /// Check if [`Series`] is sorted.
+    fn is_sorted_flag(&self) -> IsSorted {
+        IsSorted::Not
     }
 
-    #[allow(clippy::ptr_arg)]
-    fn evaluate_on_groups<'a>(
-        &self,
-        df: &DataFrame,
-        groups: &'a GroupsProxy,
-        state: &ExecutionState,
-    ) -> PolarsResult<AggregationContext<'a>> {
-        let (result_a, result_b) = POOL.install(|| {
-            rayon::join(
-                || self.left.evaluate_on_groups(df, groups, state),
-                || self.right.evaluate_on_groups(df, groups, state),
-            )
-        });
-        let mut ac_l = result_a?;
-        let ac_r = result_b?;
-
-        match (ac_l.agg_state(), ac_r.agg_state()) {
-            (
-                AggState::Literal(_) | AggState::NotAggregated(_),
-                AggState::Literal(_) | AggState::NotAggregated(_),
-            ) => self.apply_elementwise(ac_l, ac_r, false),
-            (
-                AggState::AggregatedFlat(_) | AggState::Literal(_),
-                AggState::AggregatedFlat(_) | AggState::Literal(_),
-            ) => self.apply_elementwise(ac_l, ac_r, true),
-            (AggState::AggregatedFlat(_), AggState::NotAggregated(_))
-            | (AggState::NotAggregated(_), AggState::AggregatedFlat(_)) => {
-                self.apply_group_aware(ac_l, ac_r)
-            }
-            (AggState::AggregatedList(lhs), AggState::AggregatedList(rhs)) => {
-                let lhs = lhs.list().unwrap();
-                let rhs = rhs.list().unwrap();
-                let out =
-                    lhs.apply_to_inner(&|lhs| apply_operator(&lhs, &rhs.get_inner(), self.op))?;
-                ac_l.with_series(out.into_series(), true, Some(&self.expr))?;
-                Ok(ac_l)
-            }
-            _ => self.apply_group_aware(ac_l, ac_r),
-        }
+    /// Rename the Series.
+    fn rename(&mut self, name: &str);
+
+    fn bitand(&self, _other: &Series) -> PolarsResult<Series> {
+        polars_bail!(opq = bitand, self._dtype());
     }
 
-    fn to_field(&self, input_schema: &Schema) -> PolarsResult<Field> {
-        self.expr.to_field(input_schema, Context::Default)
-    }
-
-    fn as_partitioned_aggregator(&self) -> Option<&dyn PartitionedAggregation> {
-        Some(self)
-    }
-
-    #[cfg(feature = "parquet")]
-    fn as_stats_evaluator(&self) -> Option<&dyn polars_io::predicates::StatsEvaluator> {
-        Some(self)
-    }
-
-    fn is_valid_aggregation(&self) -> bool {
-        // we don't want:
-        // col(a) == lit(1)
-
-        // we do want
-        // col(a).sum() == lit(1)
-        (!self.left.is_literal() && self.left.is_valid_aggregation())
-            | (!self.right.is_literal() && self.right.is_valid_aggregation())
+    fn bitor(&self, _other: &Series) -> PolarsResult<Series> {
+        polars_bail!(opq = bitor, self._dtype());
     }
-}
 
-#[cfg(feature = "parquet")]
-mod stats {
-    use polars_io::parquet::predicates::BatchStats;
-    use polars_io::predicates::StatsEvaluator;
+    fn bitxor(&self, _other: &Series) -> PolarsResult<Series> {
+        polars_bail!(opq = bitxor, self._dtype());
+    }
 
-    use super::*;
+    /// Get the lengths of the underlying chunks
+    fn chunk_lengths(&self) -> ChunkIdIter;
+
+    /// Name of series.
+    fn name(&self) -> &str;
+
+    /// Get field (used in schema)
+    fn field(&self) -> Cow<Field> {
+        self._field()
+    }
+
+    /// Get datatype of series.
+    fn dtype(&self) -> &DataType {
+        self._dtype()
+    }
+
+    /// Underlying chunks.
+    fn chunks(&self) -> &Vec<ArrayRef>;
+
+    /// Number of chunks in this Series
+    fn n_chunks(&self) -> usize {
+        self.chunks().len()
+    }
+
+    /// Shrink the capacity of this array to fit its length.
+    fn shrink_to_fit(&mut self) {
+        invalid_operation_panic!(shrink_to_fit, self);
+    }
+
+    /// Take `num_elements` from the top as a zero copy view.
+    fn limit(&self, num_elements: usize) -> Series {
+        self.slice(0, num_elements)
+    }
+
+    /// Get a zero copy view of the data.
+    ///
+    /// When offset is negative the offset is counted from the
+    /// end of the array
+    fn slice(&self, _offset: i64, _length: usize) -> Series;
+
+    #[doc(hidden)]
+    fn append(&mut self, _other: &Series) -> PolarsResult<()>;
+
+    #[doc(hidden)]
+    fn extend(&mut self, _other: &Series) -> PolarsResult<()>;
+
+    /// Filter by boolean mask. This operation clones data.
+    fn filter(&self, _filter: &BooleanChunked) -> PolarsResult<Series>;
+
+    #[doc(hidden)]
+    #[cfg(feature = "chunked_ids")]
+    unsafe fn _take_chunked_unchecked(&self, by: &[ChunkId], sorted: IsSorted) -> Series;
 
-    fn apply_operator_stats_eq(min_max: &Series, literal: &Series) -> bool {
-        // literal is greater than max, don't need to read
-        if ChunkCompare::<&Series>::gt(literal, min_max)
-            .ok()
-            .map(|s| s.all())
-            == Some(true)
-        {
-            return false;
-        }
-
-        // literal is smaller than min, don't need to read
-        if ChunkCompare::<&Series>::lt(literal, min_max)
-            .ok()
-            .map(|s| s.all())
-            == Some(true)
-        {
-            return false;
-        }
-
-        true
-    }
-
-    fn apply_operator_stats_rhs_lit(min_max: &Series, literal: &Series, op: Operator) -> bool {
-        match op {
-            Operator::Eq => apply_operator_stats_eq(min_max, literal),
-            // col > lit
-            // e.g.
-            // [min,
-            // max] > 0
-            //
-            // [-1,
-            // 2] > 0
-            //
-            // [false, true] -> true -> read
-            Operator::Gt => {
-                // literal is bigger than max value
-                // selection needs all rows
-                ChunkCompare::<&Series>::gt(min_max, literal)
-                    .ok()
-                    .map(|s| s.any())
-                    == Some(true)
-            }
-            // col >= lit
-            Operator::GtEq => {
-                // literal is bigger than max value
-                // selection needs all rows
-                ChunkCompare::<&Series>::gt_eq(min_max, literal)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            // col < lit
-            Operator::Lt => {
-                // literal is smaller than min value
-                // selection needs all rows
-                ChunkCompare::<&Series>::lt(min_max, literal)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            // col <= lit
-            Operator::LtEq => {
-                // literal is smaller than min value
-                // selection needs all rows
-                ChunkCompare::<&Series>::lt_eq(min_max, literal)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            // default: read the file
-            _ => true,
-        }
-    }
-
-    fn apply_operator_stats_lhs_lit(literal: &Series, min_max: &Series, op: Operator) -> bool {
-        match op {
-            Operator::Eq => apply_operator_stats_eq(min_max, literal),
-            Operator::Gt => {
-                // literal is bigger than max value
-                // selection needs all rows
-                ChunkCompare::<&Series>::gt(literal, min_max)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            Operator::GtEq => {
-                // literal is bigger than max value
-                // selection needs all rows
-                ChunkCompare::<&Series>::gt_eq(literal, min_max)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            Operator::Lt => {
-                // literal is smaller than min value
-                // selection needs all rows
-                ChunkCompare::<&Series>::lt(literal, min_max)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            Operator::LtEq => {
-                // literal is smaller than min value
-                // selection needs all rows
-                ChunkCompare::<&Series>::lt_eq(literal, min_max)
-                    .ok()
-                    .map(|ca| ca.any())
-                    == Some(true)
-            }
-            // default: read the file
-            _ => true,
-        }
-    }
-
-    impl BinaryExpr {
-        fn impl_should_read(&self, stats: &BatchStats) -> PolarsResult<bool> {
-            // See: #5864 for the rationale behind this.
-            use Expr::*;
-            use Operator::*;
-            if !self.expr.into_iter().all(|e| match e {
-                BinaryExpr { op, .. } => !matches!(
-                    op,
-                    Multiply | Divide | TrueDivide | FloorDivide | Modulus | NotEq
-                ),
-                Column(_) | Literal(_) | Alias(_, _) => true,
-                _ => false,
-            }) {
-                return Ok(true);
-            }
-
-            let schema = stats.schema();
-            let fld_l = self.left.to_field(schema)?;
-            let fld_r = self.right.to_field(schema)?;
-
-            #[cfg(debug_assertions)]
-            {
-                match (fld_l.data_type(), fld_r.data_type()) {
-                    #[cfg(feature = "dtype-categorical")]
-                    (DataType::Utf8, DataType::Categorical(_)) => {}
-                    #[cfg(feature = "dtype-categorical")]
-                    (DataType::Categorical(_), DataType::Utf8) => {}
-                    (l, r) if l != r => panic!("implementation error: {l:?}, {r:?}"),
-                    _ => {}
-                }
-            }
-
-            let dummy = DataFrame::new_no_checks(vec![]);
-            let state = ExecutionState::new();
-
-            let out = match (self.left.is_literal(), self.right.is_literal()) {
-                (false, true) => {
-                    let l = stats.get_stats(fld_l.name())?;
-                    match l.to_min_max() {
-                        None => Ok(true),
-                        Some(min_max_s) => {
-                            // will be incorrect if not
-                            debug_assert_eq!(min_max_s.null_count(), 0);
-                            let lit_s = self.right.evaluate(&dummy, &state).unwrap();
-                            Ok(apply_operator_stats_rhs_lit(&min_max_s, &lit_s, self.op))
-                        }
-                    }
-                }
-                (true, false) => {
-                    let r = stats.get_stats(fld_r.name())?;
-                    match r.to_min_max() {
-                        None => Ok(true),
-                        Some(min_max_s) => {
-                            // will be incorrect if not
-                            debug_assert_eq!(min_max_s.null_count(), 0);
-                            let lit_s = self.left.evaluate(&dummy, &state).unwrap();
-                            Ok(apply_operator_stats_lhs_lit(&lit_s, &min_max_s, self.op))
-                        }
-                    }
-                }
-                // default: read the file
-                _ => Ok(true),
-            };
-            out.map(|read| {
-                if state.verbose() && read {
-                    eprintln!("parquet file must be read, statistics not sufficient for predicate.")
-                } else if state.verbose() && !read {
-                    eprintln!("parquet file can be skipped, the statistics were sufficient to apply the predicate.")
-                };
-                read
-            })
-        }
-    }
-
-    impl StatsEvaluator for BinaryExpr {
-        fn should_read(&self, stats: &BatchStats) -> PolarsResult<bool> {
-            if std::env::var("POLARS_NO_PARQUET_STATISTICS").is_ok() {
-                return Ok(true);
-            }
-
-            match (
-                self.left.as_stats_evaluator(),
-                self.right.as_stats_evaluator(),
-            ) {
-                (Some(l), Some(r)) => match self.op {
-                    Operator::And => Ok(l.should_read(stats)? && r.should_read(stats)?),
-                    Operator::Or => Ok(l.should_read(stats)? || r.should_read(stats)?),
-                    _ => Ok(true),
-                },
-                _ => self.impl_should_read(stats),
-            }
+    #[doc(hidden)]
+    #[cfg(feature = "chunked_ids")]
+    unsafe fn _take_opt_chunked_unchecked(&self, by: &[Option<ChunkId>]) -> Series;
+
+    /// Take by index from an iterator. This operation clones the data.
+    fn take_iter(&self, _iter: &mut dyn TakeIterator) -> PolarsResult<Series>;
+
+    /// Take by index from an iterator. This operation clones the data.
+    ///
+    /// # Safety
+    ///
+    /// - This doesn't check any bounds.
+    /// - Iterator must be TrustedLen
+    unsafe fn take_iter_unchecked(&self, _iter: &mut dyn TakeIterator) -> Series;
+
+    /// Take by index if ChunkedArray contains a single chunk.
+    ///
+    /// # Safety
+    /// This doesn't check any bounds.
+    unsafe fn take_unchecked(&self, _idx: &IdxCa) -> PolarsResult<Series>;
+
+    /// Take by index from an iterator. This operation clones the data.
+    ///
+    /// # Safety
+    ///
+    /// - This doesn't check any bounds.
+    /// - Iterator must be TrustedLen
+    unsafe fn take_opt_iter_unchecked(&self, _iter: &mut dyn TakeIteratorNulls) -> Series;
+
+    /// Take by index from an iterator. This operation clones the data.
+    /// todo! remove?
+    #[cfg(feature = "take_opt_iter")]
+    fn take_opt_iter(&self, _iter: &mut dyn TakeIteratorNulls) -> PolarsResult<Series> {
+        invalid_operation_panic!(take_opt_iter, self)
+    }
+
+    /// Take by index. This operation is clone.
+    fn take(&self, _indices: &IdxCa) -> PolarsResult<Series>;
+
+    /// Get length of series.
+    fn len(&self) -> usize;
+
+    /// Check if Series is empty.
+    fn is_empty(&self) -> bool {
+        self.len() == 0
+    }
+
+    /// Aggregate all chunks to a contiguous array of memory.
+    fn rechunk(&self) -> Series;
+
+    /// Drop all null values and return a new Series.
+    fn drop_nulls(&self) -> Series {
+        if self.null_count() == 0 {
+            Series(self.clone_inner())
+        } else {
+            self.filter(&self.is_not_null()).unwrap()
         }
     }
-}
 
-impl PartitionedAggregation for BinaryExpr {
-    fn evaluate_partitioned(
+    /// Returns the mean value in the array
+    /// Returns an option because the array is nullable.
+    fn mean(&self) -> Option<f64> {
+        None
+    }
+
+    /// Returns the median value in the array
+    /// Returns an option because the array is nullable.
+    fn median(&self) -> Option<f64> {
+        None
+    }
+
+    /// Create a new Series filled with values from the given index.
+    ///
+    /// # Example
+    ///
+    /// ```rust
+    /// use polars_core::prelude::*;
+    /// let s = Series::new("a", [0i32, 1, 8]);
+    /// let s2 = s.new_from_index(2, 4);
+    /// assert_eq!(Vec::from(s2.i32().unwrap()), &[Some(8), Some(8), Some(8), Some(8)])
+    /// ```
+    fn new_from_index(&self, _index: usize, _length: usize) -> Series;
+
+    fn cast(&self, _data_type: &DataType) -> PolarsResult<Series>;
+
+    /// Get a single value by index. Don't use this operation for loops as a runtime cast is
+    /// needed for every iteration.
+    fn get(&self, _index: usize) -> PolarsResult<AnyValue>;
+
+    /// Get a single value by index. Don't use this operation for loops as a runtime cast is
+    /// needed for every iteration.
+    ///
+    /// This may refer to physical types
+    ///
+    /// # Safety
+    /// Does not do any bounds checking
+    unsafe fn get_unchecked(&self, _index: usize) -> AnyValue {
+        invalid_operation_panic!(get_unchecked, self)
+    }
+
+    fn sort_with(&self, _options: SortOptions) -> Series {
+        invalid_operation_panic!(sort_with, self)
+    }
+
+    /// Retrieve the indexes needed for a sort.
+    #[allow(unused)]
+    fn arg_sort(&self, options: SortOptions) -> IdxCa {
+        invalid_operation_panic!(arg_sort, self)
+    }
+
+    /// Count the null values.
+    fn null_count(&self) -> usize;
+
+    /// Return if any the chunks in this `[ChunkedArray]` have a validity bitmap.
+    /// no bitmap means no null values.
+    fn has_validity(&self) -> bool;
+
+    /// Get unique values in the Series.
+    fn unique(&self) -> PolarsResult<Series> {
+        polars_bail!(opq = unique, self._dtype());
+    }
+
+    /// Get unique values in the Series.
+    fn n_unique(&self) -> PolarsResult<usize> {
+        polars_bail!(opq = n_unique, self._dtype());
+    }
+
+    /// Get first indexes of unique values.
+    fn arg_unique(&self) -> PolarsResult<IdxCa> {
+        polars_bail!(opq = arg_unique, self._dtype());
+    }
+
+    /// Get a mask of the null values.
+    fn is_null(&self) -> BooleanChunked;
+
+    /// Get a mask of the non-null values.
+    fn is_not_null(&self) -> BooleanChunked;
+
+    /// return a Series in reversed order
+    fn reverse(&self) -> Series;
+
+    /// Rechunk and return a pointer to the start of the Series.
+    /// Only implemented for numeric types
+    fn as_single_ptr(&mut self) -> PolarsResult<usize> {
+        polars_bail!(opq = as_single_ptr, self._dtype());
+    }
+
+    /// Shift the values by a given period and fill the parts that will be empty due to this operation
+    /// with `Nones`.
+    ///
+    /// *NOTE: If you want to fill the Nones with a value use the
+    /// [`shift` operation on `ChunkedArray<T>`](../chunked_array/ops/trait.ChunkShift.html).*
+    ///
+    /// # Example
+    ///
+    /// ```rust
+    /// # use polars_core::prelude::*;
+    /// fn example() -> PolarsResult<()> {
+    ///     let s = Series::new("series", &[1, 2, 3]);
+    ///
+    ///     let shifted = s.shift(1);
+    ///     assert_eq!(Vec::from(shifted.i32()?), &[None, Some(1), Some(2)]);
+    ///
+    ///     let shifted = s.shift(-1);
+    ///     assert_eq!(Vec::from(shifted.i32()?), &[Some(2), Some(3), None]);
+    ///
+    ///     let shifted = s.shift(2);
+    ///     assert_eq!(Vec::from(shifted.i32()?), &[None, None, Some(1)]);
+    ///
+    ///     Ok(())
+    /// }
+    /// example();
+    /// ```
+    fn shift(&self, _periods: i64) -> Series;
+
+    /// Get the sum of the Series as a new Series of length 1.
+    ///
+    /// If the [`DataType`] is one of `{Int8, UInt8, Int16, UInt16}` the `Series` is
+    /// first cast to `Int64` to prevent overflow issues.
+    fn _sum_as_series(&self) -> Series {
+        Series::full_null(self.name(), 1, self.dtype())
+    }
+    /// Get the max of the Series as a new Series of length 1.
+    fn max_as_series(&self) -> Series {
+        Series::full_null(self.name(), 1, self.dtype())
+    }
+    /// Get the min of the Series as a new Series of length 1.
+    fn min_as_series(&self) -> Series {
+        Series::full_null(self.name(), 1, self.dtype())
+    }
+    /// Get the median of the Series as a new Series of length 1.
+    fn median_as_series(&self) -> Series {
+        Series::full_null(self.name(), 1, self.dtype())
+    }
+    /// Get the variance of the Series as a new Series of length 1.
+    fn var_as_series(&self, _ddof: u8) -> Series {
+        Series::full_null(self.name(), 1, self.dtype())
+    }
+    /// Get the standard deviation of the Series as a new Series of length 1.
+    fn std_as_series(&self, _ddof: u8) -> Series {
+        Series::full_null(self.name(), 1, self.dtype())
+    }
+    /// Get the quantile of the ChunkedArray as a new Series of length 1.
+    fn quantile_as_series(
         &self,
-        df: &DataFrame,
-        groups: &GroupsProxy,
-        state: &ExecutionState,
+        _quantile: f64,
+        _interpol: QuantileInterpolOptions,
     ) -> PolarsResult<Series> {
-        let left = self.left.as_partitioned_aggregator().unwrap();
-        let right = self.right.as_partitioned_aggregator().unwrap();
-        let left = left.evaluate_partitioned(df, groups, state)?;
-        let right = right.evaluate_partitioned(df, groups, state)?;
-        apply_operator(&left, &right, self.op)
+        Ok(Series::full_null(self.name(), 1, self.dtype()))
+    }
+
+    /// Clone inner ChunkedArray and wrap in a new Arc
+    fn clone_inner(&self) -> Arc<dyn SeriesTrait>;
+
+    #[cfg(feature = "object")]
+    /// Get the value at this index as a downcastable Any trait ref.
+    fn get_object(&self, _index: usize) -> Option<&dyn PolarsObjectSafe> {
+        invalid_operation_panic!(get_object, self)
+    }
+
+    /// Get a hold to self as `Any` trait reference.
+    /// Only implemented for ObjectType
+    fn as_any(&self) -> &dyn Any {
+        invalid_operation_panic!(as_any, self)
+    }
+
+    /// Get a hold to self as `Any` trait reference.
+    /// Only implemented for ObjectType
+    fn as_any_mut(&mut self) -> &mut dyn Any {
+        invalid_operation_panic!(as_any_mut, self)
+    }
+
+    /// Get a boolean mask of the local maximum peaks.
+    fn peak_max(&self) -> BooleanChunked {
+        invalid_operation_panic!(peak_max, self)
+    }
+
+    /// Get a boolean mask of the local minimum peaks.
+    fn peak_min(&self) -> BooleanChunked {
+        invalid_operation_panic!(peak_min, self)
     }
 
-    fn finalize(
+    /// Check if elements of this Series are in the right Series, or List values of the right Series.
+    #[cfg(feature = "is_in")]
+    fn is_in(&self, _other: &Series) -> PolarsResult<BooleanChunked> {
+        polars_bail!(opq = is_in, self._dtype());
+    }
+    #[cfg(feature = "repeat_by")]
+    fn repeat_by(&self, _by: &IdxCa) -> PolarsResult<ListChunked> {
+        polars_bail!(opq = repeat_by, self._dtype());
+    }
+    #[cfg(feature = "checked_arithmetic")]
+    fn checked_div(&self, _rhs: &Series) -> PolarsResult<Series> {
+        polars_bail!(opq = checked_div, self._dtype());
+    }
+
+    #[cfg(feature = "mode")]
+    /// Compute the most occurring element in the array.
+    fn mode(&self) -> PolarsResult<Series> {
+        polars_bail!(opq = mode, self._dtype());
+    }
+
+    #[cfg(feature = "rolling_window")]
+    /// Apply a custom function over a rolling/ moving window of the array.
+    /// This has quite some dynamic dispatch, so prefer rolling_min, max, mean, sum over this.
+    fn rolling_apply(
         &self,
-        partitioned: Series,
-        _groups: &GroupsProxy,
-        _state: &ExecutionState,
+        _f: &dyn Fn(&Series) -> Series,
+        _options: RollingOptionsFixedWindow,
     ) -> PolarsResult<Series> {
-        Ok(partitioned)
+        polars_bail!(opq = rolling_apply, self._dtype());
+    }
+    #[cfg(feature = "concat_str")]
+    /// Concat the values into a string array.
+    /// # Arguments
+    ///
+    /// * `delimiter` - A string that will act as delimiter between values.
+    fn str_concat(&self, _delimiter: &str) -> Utf8Chunked {
+        invalid_operation_panic!(str_concat, self);
+    }
+
+    fn tile(&self, _n: usize) -> Series {
+        invalid_operation_panic!(tile, self);
+    }
+}
+
+impl<'a> (dyn SeriesTrait + 'a) {
+    pub fn unpack<N: 'static>(&self) -> PolarsResult<&ChunkedArray<N>>
+    where
+        N: PolarsDataType,
+    {
+        polars_ensure!(&N::get_dtype() == self.dtype(), unpack);
+        Ok(self.as_ref())
     }
 }
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/construct_pipeline.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/convert_alp.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-lazy/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/pass.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/pass.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+use once_cell::sync::Lazy;
+use polars_core::export::once_cell;
+
 use super::*;
 use crate::pipeline::PARTITION_SIZE;
 
 const OB_SIZE: usize = 2048;
 
+static SPILL_SIZE: Lazy<usize> = Lazy::new(|| {
+    std::env::var("POLARS_STREAMING_GROUPBY_SPILL_SIZE")
+        .map(|v| v.parse::<usize>().unwrap())
+        .unwrap_or(10_000)
+});
+
 #[derive(Clone)]
 struct SpillPartitions {
     // outer vec: partitions (factor of 2)
     // inner vec: number of keys + number of aggregated columns
     keys_aggs_partitioned: PartitionVec<Vec<AnyValueBufferTrusted<'static>>>,
     hash_partitioned: PartitionVec<Vec<u64>>,
     chunk_index_partitioned: PartitionVec<Vec<IdxSize>>,
@@ -254,15 +263,15 @@
             SpillPartitions::new(key_dtypes.clone(), agg_dtypes, output_schema.clone());
 
         Self {
             inner_map: AggHashTable::new(
                 agg_constructors,
                 key_dtypes.as_ref(),
                 output_schema,
-                Some(256),
+                Some(*SPILL_SIZE),
             ),
             spill_partitions,
         }
     }
 
     pub(super) fn split(&self) -> Self {
         // should be called before any chunk is processed
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/operator.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/operator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-json/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -223,15 +223,22 @@
 }
 
 #[cfg(feature = "rolling_window")]
 #[allow(clippy::type_complexity)]
 fn rolling_agg<T>(
     ca: &ChunkedArray<T>,
     options: RollingOptionsImpl,
-    rolling_agg_fn: &dyn Fn(&[T::Native], usize, usize, bool, Option<&[f64]>, DynArgs) -> ArrayRef,
+    rolling_agg_fn: &dyn Fn(
+        &[T::Native],
+        usize,
+        usize,
+        bool,
+        Option<&[f64]>,
+        DynArgs,
+    ) -> PolarsResult<ArrayRef>,
     rolling_agg_fn_nulls: &dyn Fn(
         &PrimitiveArray<T::Native>,
         usize,
         usize,
         bool,
         Option<&[f64]>,
         DynArgs,
@@ -267,15 +274,15 @@
             0 => rolling_agg_fn(
                 arr.values().as_slice(),
                 options.window_size,
                 options.min_periods,
                 options.center,
                 options.weights.as_deref(),
                 options.fn_params,
-            ),
+            )?,
             _ => rolling_agg_fn_nulls(
                 arr,
                 options.window_size,
                 options.min_periods,
                 options.center,
                 options.weights.as_deref(),
                 options.fn_params,
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/time.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/month_end.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_end.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/month_start.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/month_start.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/arithmetic/numeric.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/array/iterator.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/array/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/fixed_size_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/explode_and_offsets.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/min_max_binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/args.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/args.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/hash_join/zip_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -289,15 +289,15 @@
             Utf8 => AnyValueBuffer::Utf8(Utf8ChunkedBuilder::new("", len, len * 5)),
             // Struct and List can be recursive so use anyvalues for that
             dt => AnyValueBuffer::All(dt.clone(), Vec::with_capacity(len)),
         }
     }
 }
 
-/// An `AnyValyeBuffer` that should be used when we trust the builder
+/// An `AnyValueBuffer` that should be used when we trust the builder
 #[derive(Clone)]
 pub enum AnyValueBufferTrusted<'a> {
     Boolean(BooleanChunkedBuilder),
     #[cfg(feature = "dtype-i8")]
     Int8(PrimitiveChunkedBuilder<Int8Type>),
     #[cfg(feature = "dtype-i16")]
     Int16(PrimitiveChunkedBuilder<Int16Type>),
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/named_from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/schema.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/df.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/df.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/array.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/into.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/flatten.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/flatten.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/macros.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/sync.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/keywords.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/keywords.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_cumulative.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_cumulative.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_io.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_math.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_math.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_meta.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/functions_string.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/functions_string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_7436.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7436.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_7437.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7437.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_7440.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_7440.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_8395.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8395.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/iss_8419.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/iss_8419.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/ops_distinct_on.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/ops_distinct_on.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/simple_exprs.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/simple_exprs.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-sql/tests/statements.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-sql/tests/statements.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars-error/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.18.2/local_dependencies/polars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.18.2/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.18.2/local_dependencies/polars/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -38,50 +38,48 @@
 		-p polars-sql \
 		-p polars-json
 
 clippy-default:
 	cargo clippy
 
 test:  ## Run tests
-	POLARS_NO_STREAMING_GROUPBY=1 POLARS_MAX_THREADS=4 cargo t -p polars-core test_4_threads
 	cargo test --all-features \
 		-p polars-lazy \
 		-p polars-io \
 		-p polars-core \
 		-p polars-arrow \
 		-p polars-time \
 		-p polars-utils \
 		-p polars-row \
 		-p polars-sql \
 		-- \
 		--test-threads=2
 
 integration-tests:
-	cargo t --all-features --test it -- --test-threads=2
+	cargo test --all-features --test it -- --test-threads=2
 
 miri:
 	# not tested on all features because miri does not support SIMD
 	# some tests are also filtered, because miri cannot deal with the rayon threadpool
 	# we ignore leaks because the thread pool of rayon is never killed.
 	MIRIFLAGS="-Zmiri-disable-isolation -Zmiri-ignore-leaks -Zmiri-disable-stacked-borrows" \
 	POLARS_ALLOW_EXTENSION=1 \
 	cargo miri test \
 	    --no-default-features \
 	    --features object \
 	    -p polars-core \
-	    -p polars-arrow \
-	    --
+	    -p polars-arrow
 
 test-doc:
 	cargo test --doc \
 	    -p polars-lazy \
 	    -p polars-io \
 	    -p polars-core \
 	    -p polars-arrow \
-			-p polars-sql
+		-p polars-sql
 
 pre-commit: fmt clippy clippy-default  ## Run autoformatting and linting
 
 
 check-features:
 	cargo hack check --each-feature --no-dev-deps
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 //! standard for columnar data.
 //!
 //! ## Quickstart
 //! We recommend to build your queries directly with polars-lazy. This allows you to combine
 //! expression into powerful aggregations and column selections. All expressions are evaluated
 //! in parallel and your queries are optimized just in time.
 //!
-//! ```rust no_run
+//! ```no_run
 //! use polars::prelude::*;
 //! # fn example() -> PolarsResult<()> {
 //!
 //! let lf1 = LazyFrame::scan_parquet("myfile_1.parquet", Default::default())?
 //!     .groupby([col("ham")])
 //!     .agg([
 //!         // expressions can be combined into powerful aggregations
@@ -301,30 +301,32 @@
 //! #### Usage
 //! ```ignore
 //! use mimalloc::MiMalloc;
 //!
 //! #[global_allocator]
 //! static GLOBAL: MiMalloc = MiMalloc;
 //! ```
+//!
 //! ```ignore
 //! use jemallocator::Jemalloc;
 //!
 //! #[global_allocator]
 //! static GLOBAL: Jemalloc = Jemalloc;
 //! ```
 //!
 //! #### Notes
 //! [Benchmarks](https://github.com/pola-rs/polars/pull/3108) have shown that on Linux JeMalloc
 //! outperforms Mimalloc on all tasks and is therefor the default Linux allocator used for the Python bindings.
 //!
 //! #### Cargo.toml
-//! ```ignore
+//! ```toml
 //! [dependencies]
 //! mimalloc = { version = "*", default-features = false }
 //! ```
+//!
 //! ## Config with ENV vars
 //!
 //! * `POLARS_FMT_TABLE_FORMATTING` -> define styling of tables using any of the following options (default = UTF8_FULL_CONDENSED):
 //!
 //!                                    ASCII_FULL
 //!                                    ASCII_FULL_CONDENSED
 //!                                    ASCII_NO_BORDERS
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files 0% similar despite different names*

```diff
@@ -265,31 +265,31 @@
             min_periods: 3,
             center: true,
             ..Default::default()
         })
         .unwrap();
     let out = out.f64().unwrap().to_vec();
 
-    let expres = &[
+    let exp_res = &[
         None,
         Some(17.333333333333332),
         Some(11.583333333333334),
         Some(21.583333333333332),
         Some(24.666666666666668),
         Some(34.33333333333334),
     ];
-    let testres = out.iter().zip(expres.iter()).all(|(&a, &b)| match (a, b) {
+    let test_res = out.iter().zip(exp_res.iter()).all(|(&a, &b)| match (a, b) {
         (None, None) => true,
         (Some(a), Some(b)) => (a - b).abs() < 1e-12,
         (_, _) => false,
     });
     assert!(
-        testres,
+        test_res,
         "{:?} is not approximately equal to {:?}",
-        out, expres
+        out, exp_res
     );
 }
 
 #[test]
 fn test_median_quantile_types() {
     let s = Int32Chunked::new("foo", &[1, 2, 3, 2, 1]).into_series();
     let rol_med = s
```

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/local_dependencies/polars/tests/it/schema.rs` & `polars_lts_cpu-0.18.2/local_dependencies/polars/tests/it/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/Cargo.toml` & `polars_lts_cpu-0.18.2/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.18.1"
+version = "0.18.2"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
```

### Comparing `polars_lts_cpu-0.18.1/LICENSE` & `polars_lts_cpu-0.18.2/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/Makefile` & `polars_lts_cpu-0.18.2/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/README.md` & `polars_lts_cpu-0.18.2/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/build.rs` & `polars_lts_cpu-0.18.2/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/Makefile` & `polars_lts_cpu-0.18.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.18.2/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/run_live_docs_server.py` & `polars_lts_cpu-0.18.2/docs/run_live_docs_server.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.18.2/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/conf.py` & `polars_lts_cpu-0.18.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/api.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/config.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/config.rst`

 * *Files 14% similar despite different names*

```diff
@@ -51,14 +51,28 @@
 
     with pl.Config() as cfg:
         cfg.set_verbose(True)
         do_various_things()
 
     # on scope exit any modified settings are restored to their previous state
 
-...or by setting the options in the ``Config`` init directly (optionally
-omitting the "set\_" prefix for brevity):
+...or, often cleaner, by setting the options in the ``Config`` init directly
+(optionally omitting the "set\_" prefix for brevity):
 
 .. code-block:: python
 
     with pl.Config(verbose=True):
         do_various_things()
+
+Use as a function decorator
+---------------------------
+
+In the same vein, you can also use ``Config`` as a function decorator to
+temporarily set options for the duration of the function call:
+
+.. code-block:: python
+
+    @pl.Config(set_ascii_tables=True)
+    def write_ascii_frame_to_stdout(df: pl.DataFrame) -> None:
+        sys.stdout.write(str(df))
+
+"""
```

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/io.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/selectors.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/selectors.rst`

 * *Files 2% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 the :meth:`col` expression and can also broadcast expressions over the selected
 columns.
 
 Importing
 ---------
 
 * Selectors are available as functions imported from ``polars.selectors``
-* Typical usage is to import the module as ``cs`` and employ selectors from there.
+* Typical/recommended usage is to import the module as ``cs`` and employ selectors from there.
 
   .. code-block:: python
 
       import polars.selectors as cs
       import polars as pl
 
       df = pl.DataFrame(
           {
               "w": ["xx", "yy", "xx", "yy", "xx"],
               "x": [1, 2, 1, 4, -2],
               "y": [3.0, 4.5, 1.0, 2.5, -2.0],
               "z": ["a", "b", "a", "b", "b"],
           },
       )
-      df.groupby(by=cs.string()).agg(s.numeric().sum())
+      df.groupby(by=cs.string()).agg(cs.numeric().sum())
 
 Set operations
 --------------
 
 Selectors support ``set`` operations such as:
 
 - UNION:        ``A | B``
@@ -41,77 +41,80 @@
 - DIFFERENCE:   ``A - B``
 - COMPLEMENT:   ``~A``
 
 
 Examples
 ========
 
-  .. code-block:: python
-
-      import polars.selectors as cs
-      import polars as pl
+.. code-block:: python
 
-      # set up an empty dataframe with plenty of columns of various dtypes
-      df = pl.DataFrame(
-          schema={
-              "abc": pl.UInt16,
-              "bbb": pl.UInt32,
-              "cde": pl.Float64,
-              "def": pl.Float32,
-              "eee": pl.Boolean,
-              "fgg": pl.Boolean,
-              "ghi": pl.Time,
-              "JJK": pl.Date,
-              "Lmn": pl.Duration,
-              "opp": pl.Datetime("ms"),
-              "qqR": pl.Utf8,
-          },
-      )
+    import polars.selectors as cs
+    import polars as pl
 
-      # Select the UNION of temporal, strings and columns that start with "e"
-      assert df.select(cs.temporal() | cs.string() | cs.starts_with("e")).schema == {
-          "eee": pl.Boolean,
-          "ghi": pl.Time,
-          "JJK": pl.Date,
-          "Lmn": pl.Duration,
-          "opp": pl.Datetime("ms"),
-          "qqR": pl.Utf8,
-      }
-
-      # Select the INTERSECTION of temporal and column names that match "opp" OR "JJK"
-      assert df.select(cs.temporal() & cs.matches("opp|JJK")).schema == {
-          "JJK": pl.Date,
-          "opp": pl.Datetime("ms"),
-      }
-
-      # Select the DIFFERENCE of temporal columns and columns that contain the name "opp" OR "JJK"
-      assert df.select(cs.temporal() - cs.matches("opp|JJK")).schema == {
-          "ghi": pl.Time,
-          "Lmn": pl.Duration,
-      }
-
-      # Select the COMPLEMENT of all columns of dtypes Duration and Time
-      assert df.select(~cs.by_dtype([pl.Duration, pl.Time])).schema == {
-          "abc": pl.UInt16,
-          "bbb": pl.UInt32,
-          "cde": pl.Float64,
-          "def": pl.Float32,
-          "eee": pl.Boolean,
-          "fgg": pl.Boolean,
-          "JJK": pl.Date,
-          "opp": pl.Datetime("ms"),
-          "qqR": pl.Utf8,
-      }
+    # set up an empty dataframe with plenty of columns of various dtypes
+    df = pl.DataFrame(
+        schema={
+            "abc": pl.UInt16,
+            "bbb": pl.UInt32,
+            "cde": pl.Float64,
+            "def": pl.Float32,
+            "eee": pl.Boolean,
+            "fgg": pl.Boolean,
+            "ghi": pl.Time,
+            "JJK": pl.Date,
+            "Lmn": pl.Duration,
+            "opp": pl.Datetime("ms"),
+            "qqR": pl.Utf8,
+        },
+    )
+
+    # Select the UNION of temporal, strings and columns that start with "e"
+    assert df.select(cs.temporal() | cs.string() | cs.starts_with("e")).schema == {
+        "eee": pl.Boolean,
+        "ghi": pl.Time,
+        "JJK": pl.Date,
+        "Lmn": pl.Duration,
+        "opp": pl.Datetime("ms"),
+        "qqR": pl.Utf8,
+    }
+
+    # Select the INTERSECTION of temporal and column names that match "opp" OR "JJK"
+    assert df.select(cs.temporal() & cs.matches("opp|JJK")).schema == {
+        "JJK": pl.Date,
+        "opp": pl.Datetime("ms"),
+    }
+
+    # Select the DIFFERENCE of temporal columns and columns that contain the name "opp" OR "JJK"
+    assert df.select(cs.temporal() - cs.matches("opp|JJK")).schema == {
+        "ghi": pl.Time,
+        "Lmn": pl.Duration,
+    }
+
+    # Select the COMPLEMENT of all columns of dtypes Duration and Time
+    assert df.select(~cs.by_dtype([pl.Duration, pl.Time])).schema == {
+        "abc": pl.UInt16,
+        "bbb": pl.UInt32,
+        "cde": pl.Float64,
+        "def": pl.Float32,
+        "eee": pl.Boolean,
+        "fgg": pl.Boolean,
+        "JJK": pl.Date,
+        "opp": pl.Datetime("ms"),
+        "qqR": pl.Utf8,
+    }
 
 
 .. note::
 
-    If you don't want to use the set operations on the ``selector``s, you can materialize them as ``expressions``
-    by calling ``as_expr``. This ensures the operations ``OR, AND, etc`` are dispatched to the expressions.
+    If you don't want to use the set operations on the selectors, you can materialize them as ``expressions``
+    by calling ``as_expr``. This ensures the operations ``OR, AND, etc`` are dispatched to the underlying
+    expressions instead.
 
 Functions
 ---------
 
+Available selector functions:
+
 .. automodule:: polars.selectors
     :members:
     :autosummary:
     :autosummary-no-titles:
```

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/series/descriptive.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/docs/source/reference/testing.rst` & `polars_lts_cpu-0.18.2/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/__init__.py` & `polars_lts_cpu-0.18.2/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/api.py` & `polars_lts_cpu-0.18.2/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/config.py` & `polars_lts_cpu-0.18.2/polars/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,22 +53,22 @@
 }
 
 # vars that set the rust env directly should declare themselves here as the Config
 # method name paired with a callable that returns the current state of that value:
 _POLARS_CFG_DIRECT_VARS = {"set_fmt_float": _get_float_fmt}
 
 
-class Config:
+class Config(contextlib.ContextDecorator):
     """
     Configure polars; offers options for table formatting and more.
 
     Notes
     -----
-    Can also be used as a context manager in order to temporarily scope
-    the lifetime of specific options. For example:
+    Can also be used as a context manager OR a function decorator in order to
+    temporarily scope the lifetime of specific options. For example:
 
     >>> with pl.Config() as cfg:
     ...     # set verbose for more detailed output within the scope
     ...     cfg.set_verbose(True)  # doctest: +IGNORE_RESULT
     ...
     >>> # scope exit - no longer in verbose mode
 
@@ -76,14 +76,22 @@
 
     >>> with pl.Config(verbose=True):
     ...     pass
     ...
 
     (The compact format is available for all `Config` methods that take a single value).
 
+    Alternatively, you can use as a decorator in order to scope the duration of the
+    selected options to a specific function:
+
+    >>> @pl.Config(verbose=True)
+    ... def test():
+    ...     pass
+    ...
+
     """
 
     _original_state: str = ""
 
     def __init__(self, *, restore_defaults: bool = False, **options: Any) -> None:
         """
         Initialise a Config object instance for context manager usage.
```

### Comparing `polars_lts_cpu-0.18.1/polars/convert.py` & `polars_lts_cpu-0.18.2/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/dataframe/_html.py` & `polars_lts_cpu-0.18.2/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/dataframe/frame.py` & `polars_lts_cpu-0.18.2/polars/dataframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/dataframe/groupby.py` & `polars_lts_cpu-0.18.2/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/datatypes/__init__.py` & `polars_lts_cpu-0.18.2/polars/datatypes/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/datatypes/classes.py` & `polars_lts_cpu-0.18.2/polars/datatypes/classes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/datatypes/constants.py` & `polars_lts_cpu-0.18.2/polars/datatypes/constants.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/datatypes/constructor.py` & `polars_lts_cpu-0.18.2/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/datatypes/convert.py` & `polars_lts_cpu-0.18.2/polars/datatypes/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/dependencies.py` & `polars_lts_cpu-0.18.2/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/exceptions.py` & `polars_lts_cpu-0.18.2/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/array.py` & `polars_lts_cpu-0.18.2/polars/expr/array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/binary.py` & `polars_lts_cpu-0.18.2/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/categorical.py` & `polars_lts_cpu-0.18.2/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/datetime.py` & `polars_lts_cpu-0.18.2/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/expr.py` & `polars_lts_cpu-0.18.2/polars/expr/expr.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/list.py` & `polars_lts_cpu-0.18.2/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/meta.py` & `polars_lts_cpu-0.18.2/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/expr/string.py` & `polars_lts_cpu-0.18.2/polars/expr/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,39 +500,52 @@
         characters
             The set of characters to be removed. All combinations of this set of
             characters will be stripped. If set to None (default), all whitespace is
             removed instead.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"foo": [" hello ", "\tworld"]})
+        >>> df = pl.DataFrame({"foo": [" hello", "\nworld"]})
+        >>> df
+        shape: (2, 1)
+        ┌────────┐
+        │ foo    │
+        │ ---    │
+        │ str    │
+        ╞════════╡
+        │  hello │
+        │        │
+        │ world  │
+        └────────┘
+
         >>> df.select(pl.col("foo").str.strip())
         shape: (2, 1)
         ┌───────┐
         │ foo   │
         │ ---   │
         │ str   │
         ╞═══════╡
         │ hello │
         │ world │
         └───────┘
 
         Characters can be stripped by passing a string as argument. Note that whitespace
-        will not be stripped automatically when doing so.
+        will not be stripped automatically when doing so, unless that whitespace is
+        also included in the string.
 
-        >>> df.select(pl.col("foo").str.strip("od\t"))
+        >>> df.select(pl.col("foo").str.strip("ow\n"))
         shape: (2, 1)
-        ┌─────────┐
-        │ foo     │
-        │ ---     │
-        │ str     │
-        ╞═════════╡
-        │  hello  │
-        │ worl    │
-        └─────────┘
+        ┌───────┐
+        │ foo   │
+        │ ---   │
+        │ str   │
+        ╞═══════╡
+        │  hell │
+        │ rld   │
+        └───────┘
 
         """
         return wrap_expr(self._pyexpr.str_strip(characters))
 
     def lstrip(self, characters: str | None = None) -> Expr:
         r"""
         Remove leading characters.
@@ -584,39 +597,52 @@
         characters
             The set of characters to be removed. All combinations of this set of
             characters will be stripped. If set to None (default), all whitespace is
             removed instead.
 
         Examples
         --------
-        >>> df = pl.DataFrame({"foo": [" hello ", "world\t"]})
+        >>> df = pl.DataFrame({"foo": [" hello", "world\n"]})
+        >>> df
+        shape: (2, 1)
+        ┌────────┐
+        │ foo    │
+        │ ---    │
+        │ str    │
+        ╞════════╡
+        │  hello │
+        │ world  │
+        │        │
+        └────────┘
         >>> df.select(pl.col("foo").str.rstrip())
         shape: (2, 1)
         ┌────────┐
         │ foo    │
         │ ---    │
         │ str    │
         ╞════════╡
         │  hello │
         │ world  │
         └────────┘
 
         Characters can be stripped by passing a string as argument. Note that whitespace
-        will not be stripped automatically when doing so.
+        will not be stripped automatically when doing so, unless that whitespace is
+        also included in the string.
 
-        >>> df.select(pl.col("foo").str.rstrip("wod\t"))
+        >>> df.select(pl.col("foo").str.rstrip("oldw "))
         shape: (2, 1)
-        ┌─────────┐
-        │ foo     │
-        │ ---     │
-        │ str     │
-        ╞═════════╡
-        │  hello  │
-        │ worl    │
-        └─────────┘
+        ┌───────┐
+        │ foo   │
+        │ ---   │
+        │ str   │
+        ╞═══════╡
+        │  he   │
+        │ world │
+        │       │
+        └───────┘
 
         """
         return wrap_expr(self._pyexpr.str_rstrip(characters))
 
     def zfill(self, alignment: int) -> Expr:
         """
         Fills the string with zeroes.
```

### Comparing `polars_lts_cpu-0.18.1/polars/expr/struct.py` & `polars_lts_cpu-0.18.2/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/__init__.py` & `polars_lts_cpu-0.18.2/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/as_datatype.py` & `polars_lts_cpu-0.18.2/polars/functions/as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/eager.py` & `polars_lts_cpu-0.18.2/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/lazy.py` & `polars_lts_cpu-0.18.2/polars/functions/lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/range.py` & `polars_lts_cpu-0.18.2/polars/functions/range.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/repeat.py` & `polars_lts_cpu-0.18.2/polars/functions/repeat.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/functions/whenthen.py` & `polars_lts_cpu-0.18.2/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/__init__.py` & `polars_lts_cpu-0.18.2/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/_utils.py` & `polars_lts_cpu-0.18.2/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/avro.py` & `polars_lts_cpu-0.18.2/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/csv/_utils.py` & `polars_lts_cpu-0.18.2/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.18.2/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/csv/functions.py` & `polars_lts_cpu-0.18.2/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/database.py` & `polars_lts_cpu-0.18.2/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/delta.py` & `polars_lts_cpu-0.18.2/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.18.2/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/excel/functions.py` & `polars_lts_cpu-0.18.2/polars/io/excel/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.18.2/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/ipc/functions.py` & `polars_lts_cpu-0.18.2/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/ndjson.py` & `polars_lts_cpu-0.18.2/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.18.2/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/parquet/functions.py` & `polars_lts_cpu-0.18.2/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.18.2/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/lazyframe/frame.py` & `polars_lts_cpu-0.18.2/polars/lazyframe/frame.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.18.2/polars/lazyframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/selectors.py` & `polars_lts_cpu-0.18.2/polars/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,24 +131,26 @@
         This ensures that the operators ``|``, ``&``, ``~`` and ``-``
         are applied on the data and not no the selector sets.
         """
         return Expr._from_pyexpr(self._pyexpr)
 
 
 def _re_string(string: str | Collection[str]) -> str:
+    """Return escaped regex, potentially representing multiple string fragments."""
     if isinstance(string, str):
-        return re.escape(string)
+        rx = f"{re.escape(string)}"
     else:
         strings: list[str] = []
         for st in string:
-            if isinstance(st, Collection):
+            if isinstance(st, Collection) and not isinstance(st, str):  # type: ignore[redundant-expr]
                 strings.extend(st)
             else:
                 strings.append(st)
-        return "|".join(re.escape(x) for x in strings)
+        rx = "|".join(re.escape(x) for x in strings)
+    return f"({rx})"
 
 
 def all() -> Expr:
     """
     Select all columns.
 
     Examples
@@ -565,15 +567,15 @@
     --------
     contains : Select columns that contain the given literal substring(s).
     matches : Select all columns that match the given regex pattern.
     starts_with : Select columns that start with the given substring(s).
 
     """
     escaped_suffix = _re_string(suffix)
-    raw_params = f"^.*({escaped_suffix})$"
+    raw_params = f"^.*{escaped_suffix}$"
 
     return _selector_proxy_(
         F.col(raw_params),
         name="ends_with",
         parameters={"suffix": escaped_suffix},
         raw_parameters=[raw_params],
     )
@@ -963,15 +965,15 @@
     --------
     contains : Select all columns that contain the given substring.
     ends_with : Select all columns that end with the given substring(s).
     matches : Select all columns that match the given regex pattern.
 
     """
     escaped_prefix = _re_string(prefix)
-    raw_params = f"^({escaped_prefix}).*$"
+    raw_params = f"^{escaped_prefix}.*$"
 
     return _selector_proxy_(
         F.col(raw_params),
         name="starts_with",
         parameters={"prefix": prefix},
         raw_parameters=[raw_params],
     )
```

### Comparing `polars_lts_cpu-0.18.1/polars/series/_numpy.py` & `polars_lts_cpu-0.18.2/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/array.py` & `polars_lts_cpu-0.18.2/polars/series/array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/binary.py` & `polars_lts_cpu-0.18.2/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/categorical.py` & `polars_lts_cpu-0.18.2/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/datetime.py` & `polars_lts_cpu-0.18.2/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/list.py` & `polars_lts_cpu-0.18.2/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/series.py` & `polars_lts_cpu-0.18.2/polars/series/series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/string.py` & `polars_lts_cpu-0.18.2/polars/series/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -1034,22 +1034,23 @@
         Series: '' [str]
         [
                 "hello"
                 "world"
         ]
 
         Characters can be stripped by passing a string as argument. Note that whitespace
-        will not be stripped automatically when doing so.
+        will not be stripped automatically when doing so, unless that whitespace is
+        also included in the string.
 
-        >>> s.str.strip("od\t")
+        >>> s.str.strip("o ")
         shape: (2,)
         Series: '' [str]
         [
-                " hello "
-                "worl"
+            "hell"
+            "	world"
         ]
 
         """
 
     def lstrip(self, characters: str | None = None) -> Series:
         r"""
         Remove leading characters.
@@ -1106,20 +1107,20 @@
                 " hello"
                 "world"
         ]
 
         Characters can be stripped by passing a string as argument. Note that whitespace
         will not be stripped automatically when doing so.
 
-        >>> s.str.rstrip("wod\t")
+        >>> s.str.rstrip("orld\t")
         shape: (2,)
         Series: '' [str]
         [
-                " hello "
-                "worl"
+            " hello "
+            "w"
         ]
 
         """
 
     def zfill(self, alignment: int) -> Series:
         """
         Fills the string with zeroes.
```

### Comparing `polars_lts_cpu-0.18.1/polars/series/struct.py` & `polars_lts_cpu-0.18.2/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/series/utils.py` & `polars_lts_cpu-0.18.2/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/slice.py` & `polars_lts_cpu-0.18.2/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/sql/context.py` & `polars_lts_cpu-0.18.2/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/string_cache.py` & `polars_lts_cpu-0.18.2/polars/string_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     from polars.polars import enable_string_cache as _enable_string_cache
     from polars.polars import using_string_cache as _using_string_cache
 
 if TYPE_CHECKING:
     from types import TracebackType
 
 
-class StringCache:
+class StringCache(contextlib.ContextDecorator):
     """
     Context manager that allows data sources to share the same categorical features.
 
     This will temporarily cache the string categories until the context manager is
     finished. If StringCaches are nested, the global cache will only be invalidated
     when the outermost context exits.
```

### Comparing `polars_lts_cpu-0.18.1/polars/testing/_private.py` & `polars_lts_cpu-0.18.2/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/testing/asserts.py` & `polars_lts_cpu-0.18.2/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/testing/parametric/__init__.py` & `polars_lts_cpu-0.18.2/polars/testing/parametric/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/testing/parametric/primitives.py` & `polars_lts_cpu-0.18.2/polars/testing/parametric/primitives.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/testing/parametric/profiles.py` & `polars_lts_cpu-0.18.2/polars/testing/parametric/profiles.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/testing/parametric/strategies.py` & `polars_lts_cpu-0.18.2/polars/testing/parametric/strategies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/type_aliases.py` & `polars_lts_cpu-0.18.2/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/__init__.py` & `polars_lts_cpu-0.18.2/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/_construction.py` & `polars_lts_cpu-0.18.2/polars/utils/_construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1122,15 +1122,15 @@
             col: schema_overrides.get(col, Unknown) for col in column_names
         }
     else:
         column_names = []
         schema_override = {
             col: (py_type_to_dtype(tp, raise_unmatched=False) or Unknown)
             for col, tp in type_hints(first_element.__class__).items()
-            if col != "__slots__"
+            if col not in ("__slots__", "__pydantic_root_model__")
         }
         if schema_overrides:
             schema_override.update(schema_overrides)
         elif not from_model:
             dc_fields = set(asdict(first_element))
             schema_overrides = schema_override = {
                 nm: tp for nm, tp in schema_override.items() if nm in dc_fields
```

### Comparing `polars_lts_cpu-0.18.1/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.18.2/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/_scan.py` & `polars_lts_cpu-0.18.2/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/_wrap.py` & `polars_lts_cpu-0.18.2/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/build_info.py` & `polars_lts_cpu-0.18.2/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/convert.py` & `polars_lts_cpu-0.18.2/polars/utils/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/decorators.py` & `polars_lts_cpu-0.18.2/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/meta.py` & `polars_lts_cpu-0.18.2/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/polars_version.py` & `polars_lts_cpu-0.18.2/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/show_versions.py` & `polars_lts_cpu-0.18.2/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/polars/utils/various.py` & `polars_lts_cpu-0.18.2/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/pyproject.toml` & `polars_lts_cpu-0.18.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/requirements-dev.txt` & `polars_lts_cpu-0.18.2/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/scripts/check_stacklevels.py` & `polars_lts_cpu-0.18.2/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/apply/dataframe.rs` & `polars_lts_cpu-0.18.2/src/apply/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/apply/lazy.rs` & `polars_lts_cpu-0.18.2/src/apply/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/apply/mod.rs` & `polars_lts_cpu-0.18.2/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/apply/series.rs` & `polars_lts_cpu-0.18.2/src/apply/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.18.2/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.18.2/src/arrow_interop/to_rust.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/batched_csv.rs` & `polars_lts_cpu-0.18.2/src/batched_csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/conversion.rs` & `polars_lts_cpu-0.18.2/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/dataframe.rs` & `polars_lts_cpu-0.18.2/src/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/datatypes.rs` & `polars_lts_cpu-0.18.2/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/error.rs` & `polars_lts_cpu-0.18.2/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/array.rs` & `polars_lts_cpu-0.18.2/src/expr/array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/binary.rs` & `polars_lts_cpu-0.18.2/src/expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/datetime.rs` & `polars_lts_cpu-0.18.2/src/expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/general.rs` & `polars_lts_cpu-0.18.2/src/expr/general.rs`

 * *Files 0% similar despite different names*

```diff
@@ -960,22 +960,15 @@
     }
 
     fn cumcount(&self, reverse: bool) -> Self {
         self.inner.clone().cumcount(reverse).into()
     }
 
     fn to_physical(&self) -> Self {
-        self.inner
-            .clone()
-            .map(
-                |s| Ok(Some(s.to_physical_repr().into_owned())),
-                GetOutput::map_dtype(|dt| dt.to_physical()),
-            )
-            .with_fmt("to_physical")
-            .into()
+        self.inner.clone().to_physical().into()
     }
 
     fn shuffle(&self, seed: Option<u64>) -> Self {
         self.inner.clone().shuffle(seed).into()
     }
 
     fn sample_n(&self, n: usize, with_replacement: bool, shuffle: bool, seed: Option<u64>) -> Self {
```

### Comparing `polars_lts_cpu-0.18.1/src/expr/list.rs` & `polars_lts_cpu-0.18.2/src/expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/meta.rs` & `polars_lts_cpu-0.18.2/src/expr/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/mod.rs` & `polars_lts_cpu-0.18.2/src/expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/expr/string.rs` & `polars_lts_cpu-0.18.2/src/expr/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/file.rs` & `polars_lts_cpu-0.18.2/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/functions/eager.rs` & `polars_lts_cpu-0.18.2/src/functions/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/functions/io.rs` & `polars_lts_cpu-0.18.2/src/functions/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/functions/lazy.rs` & `polars_lts_cpu-0.18.2/src/functions/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/functions/meta.rs` & `polars_lts_cpu-0.18.2/src/functions/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/functions/whenthen.rs` & `polars_lts_cpu-0.18.2/src/functions/whenthen.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/lazyframe.rs` & `polars_lts_cpu-0.18.2/src/lazyframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/lazygroupby.rs` & `polars_lts_cpu-0.18.2/src/lazygroupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/lib.rs` & `polars_lts_cpu-0.18.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/object.rs` & `polars_lts_cpu-0.18.2/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/aggregation.rs` & `polars_lts_cpu-0.18.2/src/series/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/arithmetic.rs` & `polars_lts_cpu-0.18.2/src/series/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/comparison.rs` & `polars_lts_cpu-0.18.2/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/construction.rs` & `polars_lts_cpu-0.18.2/src/series/construction.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/export.rs` & `polars_lts_cpu-0.18.2/src/series/export.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/mod.rs` & `polars_lts_cpu-0.18.2/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/numpy_ufunc.rs` & `polars_lts_cpu-0.18.2/src/series/numpy_ufunc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/series/set_at_idx.rs` & `polars_lts_cpu-0.18.2/src/series/set_at_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/sql.rs` & `polars_lts_cpu-0.18.2/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/src/utils.rs` & `polars_lts_cpu-0.18.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/README.md` & `polars_lts_cpu-0.18.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.18.2/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.18.2/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/benchmark/test_release.py` & `polars_lts_cpu-0.18.2/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/docs/run_doctest.py` & `polars_lts_cpu-0.18.2/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.18.2/tests/parametric/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.18.2/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/parametric/test_series.py` & `polars_lts_cpu-0.18.2/tests/parametric/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/parametric/test_testing.py` & `polars_lts_cpu-0.18.2/tests/parametric/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/conftest.py` & `polars_lts_cpu-0.18.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_array.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_binary.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_categorical.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,56 +3,56 @@
 import io
 import typing
 from typing import Any
 
 import pytest
 
 import polars as pl
+from polars import StringCache
 from polars.testing import assert_frame_equal
 
 
+@StringCache()
 def test_categorical_outer_join() -> None:
-    with pl.StringCache():
-        df1 = pl.DataFrame(
-            [
-                pl.Series("key1", [42]),
-                pl.Series("key2", ["bar"], dtype=pl.Categorical),
-                pl.Series("val1", [1]),
-            ]
-        ).lazy()
-
-        df2 = pl.DataFrame(
-            [
-                pl.Series("key1", [42]),
-                pl.Series("key2", ["bar"], dtype=pl.Categorical),
-                pl.Series("val2", [2]),
-            ]
-        ).lazy()
-
-        expected = pl.DataFrame(
-            {"key1": [42], "key2": ["bar"], "val1": [1], "val2": [2]},
-            schema_overrides={"key2": pl.Categorical},
-        )
+    df1 = pl.DataFrame(
+        [
+            pl.Series("key1", [42]),
+            pl.Series("key2", ["bar"], dtype=pl.Categorical),
+            pl.Series("val1", [1]),
+        ]
+    ).lazy()
+
+    df2 = pl.DataFrame(
+        [
+            pl.Series("key1", [42]),
+            pl.Series("key2", ["bar"], dtype=pl.Categorical),
+            pl.Series("val2", [2]),
+        ]
+    ).lazy()
+
+    expected = pl.DataFrame(
+        {"key1": [42], "key2": ["bar"], "val1": [1], "val2": [2]},
+        schema_overrides={"key2": pl.Categorical},
+    )
 
     out = df1.join(df2, on=["key1", "key2"], how="outer").collect()
     assert_frame_equal(out, expected)
 
-    with pl.StringCache():
-        dfa = pl.DataFrame(
-            [
-                pl.Series("key", ["foo", "bar"], dtype=pl.Categorical),
-                pl.Series("val1", [3, 1]),
-            ]
-        )
-        dfb = pl.DataFrame(
-            [
-                pl.Series("key", ["bar", "baz"], dtype=pl.Categorical),
-                pl.Series("val2", [6, 8]),
-            ]
-        )
+    dfa = pl.DataFrame(
+        [
+            pl.Series("key", ["foo", "bar"], dtype=pl.Categorical),
+            pl.Series("val1", [3, 1]),
+        ]
+    )
+    dfb = pl.DataFrame(
+        [
+            pl.Series("key", ["bar", "baz"], dtype=pl.Categorical),
+            pl.Series("val2", [6, 8]),
+        ]
+    )
 
     df = dfa.join(dfb, on="key", how="outer")
     # the cast is important to test the rev map
     assert df["key"].cast(pl.Utf8).to_list() == ["bar", "baz", "foo"]
 
 
 def test_read_csv_categorical() -> None:
@@ -94,46 +94,46 @@
 def test_categorical_describe_3487() -> None:
     # test if we don't err
     df = pl.DataFrame({"cats": ["a", "b"]})
     df = df.with_columns(pl.col("cats").cast(pl.Categorical))
     df.describe()
 
 
+@StringCache()
 def test_categorical_is_in_list() -> None:
     # this requires type coercion to cast.
     # we should not cast within the function as this would be expensive within a groupby
     # context that would be a cast per group
-    with pl.StringCache():
-        df = pl.DataFrame(
-            {"a": [1, 2, 3, 1, 2], "b": ["a", "b", "c", "d", "e"]}
-        ).with_columns(pl.col("b").cast(pl.Categorical))
-
-        cat_list = ("a", "b", "c")
-        assert df.filter(pl.col("b").is_in(cat_list)).to_dict(False) == {
-            "a": [1, 2, 3],
-            "b": ["a", "b", "c"],
-        }
+    df = pl.DataFrame(
+        {"a": [1, 2, 3, 1, 2], "b": ["a", "b", "c", "d", "e"]}
+    ).with_columns(pl.col("b").cast(pl.Categorical))
+
+    cat_list = ("a", "b", "c")
+    assert df.filter(pl.col("b").is_in(cat_list)).to_dict(False) == {
+        "a": [1, 2, 3],
+        "b": ["a", "b", "c"],
+    }
 
 
+@StringCache()
 def test_unset_sorted_on_append() -> None:
-    with pl.StringCache():
-        df1 = pl.DataFrame(
-            [
-                pl.Series("key", ["a", "b", "a", "b"], dtype=pl.Categorical),
-                pl.Series("val", [1, 2, 3, 4]),
-            ]
-        ).sort("key")
-        df2 = pl.DataFrame(
-            [
-                pl.Series("key", ["a", "b", "a", "b"], dtype=pl.Categorical),
-                pl.Series("val", [5, 6, 7, 8]),
-            ]
-        ).sort("key")
-        df = pl.concat([df1, df2], rechunk=False)
-        assert df.groupby("key").count()["count"].to_list() == [4, 4]
+    df1 = pl.DataFrame(
+        [
+            pl.Series("key", ["a", "b", "a", "b"], dtype=pl.Categorical),
+            pl.Series("val", [1, 2, 3, 4]),
+        ]
+    ).sort("key")
+    df2 = pl.DataFrame(
+        [
+            pl.Series("key", ["a", "b", "a", "b"], dtype=pl.Categorical),
+            pl.Series("val", [5, 6, 7, 8]),
+        ]
+    ).sort("key")
+    df = pl.concat([df1, df2], rechunk=False)
+    assert df.groupby("key").count()["count"].to_list() == [4, 4]
 
 
 def test_categorical_error_on_local_cmp() -> None:
     df_cat = pl.DataFrame(
         [
             pl.Series("a_cat", ["c", "a", "b", "c", "b"], dtype=pl.Categorical),
             pl.Series("b_cat", ["F", "G", "E", "G", "G"], dtype=pl.Categorical),
@@ -161,40 +161,40 @@
     )
 
     s = df.with_columns(pl.col("a").shift_and_fill("c", periods=1))["a"]
     assert s.dtype == pl.Categorical
     assert s.to_list() == ["c", "a"]
 
 
+@StringCache()
 def test_merge_lit_under_global_cache_4491() -> None:
-    with pl.StringCache():
-        df = pl.DataFrame(
-            [
-                pl.Series("label", ["foo", "bar"], dtype=pl.Categorical),
-                pl.Series("value", [3, 9]),
-            ]
-        )
-        assert df.with_columns(
-            pl.when(pl.col("value") > 5)
-            .then(pl.col("label"))
-            .otherwise(pl.lit(None, pl.Categorical))
-        ).to_dict(False) == {"label": [None, "bar"], "value": [3, 9]}
+    df = pl.DataFrame(
+        [
+            pl.Series("label", ["foo", "bar"], dtype=pl.Categorical),
+            pl.Series("value", [3, 9]),
+        ]
+    )
+    assert df.with_columns(
+        pl.when(pl.col("value") > 5)
+        .then(pl.col("label"))
+        .otherwise(pl.lit(None, pl.Categorical))
+    ).to_dict(False) == {"label": [None, "bar"], "value": [3, 9]}
 
 
 def test_nested_cache_composition() -> None:
     # very artificial example/test, but validates the behaviour
-    # of  ested StringCache scopes, which we want to play well
+    # of nested StringCache scopes, which we want to play well
     # with each other when composing more complex pipelines.
 
     assert pl.using_string_cache() is False
 
     # function representing a composable stage of a pipeline; it implements
     # an inner scope for the case where it is called by itself, but when
     # called as part of a larger series of ops it should not invalidate
-    # the string cache (the outermost scope should be respected).
+    # the string cache (eg: the outermost scope should be respected).
     def create_lazy(data: dict) -> pl.LazyFrame:  # type: ignore[type-arg]
         with pl.StringCache():
             df = pl.DataFrame({"a": ["foo", "bar", "ham"], "b": [1, 2, 3]})
             lf = df.with_columns(pl.col("a").cast(pl.Categorical)).lazy()
 
         # confirm that scope-exit does NOT invalidate the
         # cache yet, as an outer context is still active
@@ -247,34 +247,34 @@
         )
 
 
 @pytest.mark.slow()
 def test_stringcache() -> None:
     N = 1_500
     with pl.StringCache():
-        # create a reasonable sized columns so the categorical map is reallocated
+        # create a large enough column that the categorical map is reallocated
         df = pl.DataFrame({"cats": pl.arange(0, N, eager=True)}).select(
             [pl.col("cats").cast(pl.Utf8).cast(pl.Categorical)]
         )
         assert df.filter(pl.col("cats").is_in(["1", "2"])).to_dict(False) == {
             "cats": ["1", "2"]
         }
 
 
+@StringCache()
 def test_categorical_sort_order(monkeypatch: Any) -> None:
-    with pl.StringCache():
-        # create the categorical ordering first
-        pl.Series(["foo", "bar", "baz"], dtype=pl.Categorical)
-        df = pl.DataFrame(
-            {
-                "n": [0, 0, 0],
-                # use same categories in different order
-                "x": pl.Series(["baz", "bar", "foo"], dtype=pl.Categorical),
-            }
-        )
+    # create the categorical ordering first
+    pl.Series(["foo", "bar", "baz"], dtype=pl.Categorical)
+    df = pl.DataFrame(
+        {
+            "n": [0, 0, 0],
+            # use same categories in different order
+            "x": pl.Series(["baz", "bar", "foo"], dtype=pl.Categorical),
+        }
+    )
 
     assert df.sort(["n", "x"])["x"].to_list() == ["foo", "bar", "baz"]
     assert df.with_columns(pl.col("x").cat.set_ordering("lexical")).sort(["n", "x"])[
         "x"
     ].to_list() == ["bar", "baz", "foo"]
     monkeypatch.setenv("POLARS_ROW_FMT_SORT", "1")
     assert df.sort(["n", "x"])["x"].to_list() == ["foo", "bar", "baz"]
@@ -367,21 +367,21 @@
         False
     ) == {
         "col": ["a", "a", "a"],
         "code": [0, 0, 0],
     }
 
 
+@StringCache()
 def test_categorical_fill_null_stringcache() -> None:
-    with pl.StringCache():
-        df = pl.LazyFrame(
-            {"index": [1, 2, 3], "cat": ["a", "b", None]},
-            schema={"index": pl.Int64(), "cat": pl.Categorical()},
-        )
-        a = df.select(pl.col("cat").fill_null("hi")).collect()
+    df = pl.LazyFrame(
+        {"index": [1, 2, 3], "cat": ["a", "b", None]},
+        schema={"index": pl.Int64(), "cat": pl.Categorical()},
+    )
+    a = df.select(pl.col("cat").fill_null("hi")).collect()
 
     assert a.to_dict(False) == {"cat": ["a", "b", "hi"]}
     assert a.dtypes == [pl.Categorical]
 
 
 @typing.no_type_check
 def test_fast_unique_flag_from_arrow() -> None:
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_duration.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_duration.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.18.2/tests/unit/datatypes/test_temporal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/functions/test_as_datatype.py` & `polars_lts_cpu-0.18.2/tests/unit/functions/test_as_datatype.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/functions/test_functions.py` & `polars_lts_cpu-0.18.2/tests/unit/functions/test_functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/functions/test_range.py` & `polars_lts_cpu-0.18.2/tests/unit/functions/test_range.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/functions/test_repeat.py` & `polars_lts_cpu-0.18.2/tests/unit/functions/test_repeat.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.18.2/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.18.2/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.18.2/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.18.2/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.18.2/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_database.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_excel.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_json.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_other.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,16 +134,16 @@
         "datetime": [  # unix timestamp in ms
             1618354800000,
             1618354740000,
             1618354680000,
             1618354620000,
             1618354560000,
         ],
-        "laf_max": [73.1999969482, 71.0999984741, 74.5, 69.5999984741, 69.6999969482],
-        "laf_eq": [59.5999984741, 61.0, 62.2999992371, 56.9000015259, 60.0],
+        "value1": [73.1999969482, 71.0999984741, 74.5, 69.5999984741, 69.6999969482],
+        "value2": [59.5999984741, 61.0, 62.2999992371, 56.9000015259, 60.0],
     }
     df = pl.DataFrame(data)
     df = df.with_columns(df["datetime"].cast(pl.Datetime))
 
     df.write_parquet(f, use_pyarrow=use_pyarrow, compression=compression)
     f.seek(0)
     read = pl.read_parquet(f)
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.18.2/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_array.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_array.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_string.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,16 +185,16 @@
 
 
 def test_str_strip() -> None:
     s = pl.Series([" hello ", "world\t "])
     expected = pl.Series(["hello", "world"])
     assert_series_equal(s.str.strip(), expected)
 
-    expected = pl.Series(["hello", "worl"])
-    assert_series_equal(s.str.strip().str.strip("d"), expected)
+    expected = pl.Series(["hell", "world"])
+    assert_series_equal(s.str.strip().str.strip("o"), expected)
 
     expected = pl.Series(["ell", "rld\t"])
     assert_series_equal(s.str.strip(" hwo"), expected)
 
 
 def test_str_lstrip() -> None:
     s = pl.Series([" hello ", "\t world"])
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_strptime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.18.2/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_explode.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_filter.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_groupby_rolling.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_groupby_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_is_in.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_is_in.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_select.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_select.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/operations/test_with_columns.py` & `polars_lts_cpu-0.18.2/tests/unit/operations/test_with_columns.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/streaming/test_ooc.py` & `polars_lts_cpu-0.18.2/tests/unit/streaming/test_ooc.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 @pytest.mark.slow()
 def test_streaming_out_of_core_unique(
     io_files_path: Path, monkeypatch: Any, capfd: Any
 ) -> None:
     monkeypatch.setenv("POLARS_FORCE_OOC", "1")
     monkeypatch.setenv("POLARS_VERBOSE", "1")
+    monkeypatch.setenv("POLARS_STREAMING_GROUPBY_SPILL_SIZE", "256")
     df = pl.read_csv(io_files_path / "foods*.csv")
     # this creates 10M rows
     q = df.lazy()
     q = q.join(q, how="cross").select(df.columns).head(10_000)
 
     # uses out-of-core unique
     df1 = q.join(q.head(1000), how="cross").unique().collect(streaming=True)
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/streaming/test_streaming.py` & `polars_lts_cpu-0.18.2/tests/unit/streaming/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_api.py` & `polars_lts_cpu-0.18.2/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_arity.py` & `polars_lts_cpu-0.18.2/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_cfg.py` & `polars_lts_cpu-0.18.2/tests/unit/test_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,43 +16,50 @@
     with pl.StringCache(), pl.Config(restore_defaults=True):
         yield
 
 
 def test_ascii_tables() -> None:
     df = pl.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6], "c": [7, 8, 9]})
 
+    ascii_table_repr = (
+        "shape: (3, 3)\n"
+        "+-----+-----+-----+\n"
+        "| a   | b   | c   |\n"
+        "| --- | --- | --- |\n"
+        "| i64 | i64 | i64 |\n"
+        "+=================+\n"
+        "| 1   | 4   | 7   |\n"
+        "| 2   | 5   | 8   |\n"
+        "| 3   | 6   | 9   |\n"
+        "+-----+-----+-----+"
+    )
     # note: expect to render ascii only within the given scope
     with pl.Config(set_ascii_tables=True):
-        assert (
-            str(df) == "shape: (3, 3)\n"
-            "+-----+-----+-----+\n"
-            "| a   | b   | c   |\n"
-            "| --- | --- | --- |\n"
-            "| i64 | i64 | i64 |\n"
-            "+=================+\n"
-            "| 1   | 4   | 7   |\n"
-            "| 2   | 5   | 8   |\n"
-            "| 3   | 6   | 9   |\n"
-            "+-----+-----+-----+"
-        )
+        assert repr(df) == ascii_table_repr
 
     # confirm back to utf8 default after scope-exit
     assert (
-        str(df) == "shape: (3, 3)\n"
+        repr(df) == "shape: (3, 3)\n"
         "┌─────┬─────┬─────┐\n"
         "│ a   ┆ b   ┆ c   │\n"
         "│ --- ┆ --- ┆ --- │\n"
         "│ i64 ┆ i64 ┆ i64 │\n"
         "╞═════╪═════╪═════╡\n"
         "│ 1   ┆ 4   ┆ 7   │\n"
         "│ 2   ┆ 5   ┆ 8   │\n"
         "│ 3   ┆ 6   ┆ 9   │\n"
         "└─────┴─────┴─────┘"
     )
 
+    @pl.Config(set_ascii_tables=True)
+    def ascii_table() -> str:
+        return repr(df)
+
+    assert ascii_table() == ascii_table_repr
+
 
 def test_hide_header_elements() -> None:
     df = pl.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6], "c": [7, 8, 9]})
 
     pl.Config.set_tbl_hide_column_data_types(True)
     assert (
         str(df) == "shape: (3, 3)\n"
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_constructors.py` & `polars_lts_cpu-0.18.2/tests/unit/test_constructors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import sys
-import typing
 from datetime import date, datetime, timedelta, timezone
 from decimal import Decimal
 from random import shuffle
-from typing import TYPE_CHECKING, Any, NamedTuple
+from typing import TYPE_CHECKING, Any, NamedTuple, no_type_check
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pytest
 
 import polars as pl
@@ -17,14 +16,19 @@
 from polars.exceptions import TimeZoneAwareConstructorWarning
 from polars.testing import assert_frame_equal, assert_series_equal
 from polars.utils._construction import type_hints
 
 if TYPE_CHECKING:
     from polars.datatypes import PolarsDataType
 
+    if sys.version_info >= (3, 8):
+        from typing import Literal
+    else:
+        from typing_extensions import Literal
+
 if sys.version_info >= (3, 9):
     from zoneinfo import ZoneInfo
 elif _ZONEINFO_AVAILABLE:
     # Import from submodule due to typing issue with backports.zoneinfo package:
     # https://github.com/pganssle/zoneinfo/issues/125
     from backports.zoneinfo._zoneinfo import ZoneInfo
 
@@ -251,14 +255,51 @@
         }
         assert df.rows() == raw_data
 
         # cover a miscellaneous edge-case when detecting the annotations
         assert type_hints(obj=type(None)) == {}
 
 
+@pytest.mark.skipif(pydantic.__version__ < "2.0", reason="requires pydantic 2.x")
+@no_type_check
+def test_init_pydantic_2x() -> None:
+    from pydantic import BaseModel, Field
+
+    class PageView(BaseModel):
+        user_id: str
+        ts: datetime = Field(alias=["ts", "$date"])  # type: ignore[literal-required]
+        path: str = Field("?", alias=["url", "path"])  # type: ignore[literal-required]
+        referer: str = Field("?", alias="referer")
+        event: Literal["leave", "enter"] = Field("enter")
+        time_on_page: int = Field(0, serialization_alias="top")
+
+    if sys.version_info > (3, 7):
+        data_json = """
+        [{
+            "user_id": "x",
+            "ts": {"$date": "2021-01-01T00:00:00.000Z"},
+            "url": "/latest/foobar",
+            "referer": "https://google.com",
+            "event": "enter",
+            "top": 123
+        }]
+        """
+        at = pydantic.TypeAdapter(list[PageView])
+        models = at.validate_json(data_json)
+
+        assert pl.DataFrame(models).to_dict(False) == {
+            "user_id": ["x"],
+            "ts": [datetime(2021, 1, 1, 0, 0)],
+            "path": ["?"],
+            "referer": ["https://google.com"],
+            "event": ["enter"],
+            "time_on_page": [0],
+        }
+
+
 def test_init_structured_objects_unhashable() -> None:
     # cover an edge-case with namedtuple fields that aren't hashable
 
     class Test(NamedTuple):
         dt: datetime
         info: dict[str, int]
 
@@ -899,15 +940,15 @@
         {"a": 1},
         {"b": 2},
     ]
 
     assert pl.from_dicts(data).to_dict(False) == {"a": [1, None], "b": [None, 2]}
 
 
-@typing.no_type_check
+@no_type_check
 def test_from_rows_dtype() -> None:
     # 50 is the default inference length
     # 5182
     df = pl.DataFrame(
         data=[(None, None)] * 50 + [("1.23", None)],
         schema=[("foo", pl.Utf8), ("bar", pl.Utf8)],
         orient="row",
@@ -1029,15 +1070,15 @@
                 {"some_text_here": "text", "list_": []},
                 {"some_text_here": "text", "list_": []},
             ],
         ],
     }
 
 
-@typing.no_type_check
+@no_type_check
 def test_from_records_nullable_structs() -> None:
     records = [
         {"id": 1, "items": [{"item_id": 100, "description": None}]},
         {"id": 1, "items": [{"item_id": 100, "description": "hi"}]},
     ]
 
     schema = [
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_cse.py` & `polars_lts_cpu-0.18.2/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.18.2/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_df.py` & `polars_lts_cpu-0.18.2/tests/unit/test_df.py`

 * *Files 0% similar despite different names*

```diff
@@ -1570,15 +1570,15 @@
         "<td>3</td>",
     ):
         assert match in html, f"Expected to find {match!r} in html repr"
 
 
 def test_rename(df: pl.DataFrame) -> None:
     out = df.rename({"strings": "bars", "int": "foos"})
-    # check if wel can select these new columns
+    # check if we can select these new columns
     _ = out[["foos", "bars"]]
 
 
 def test_write_csv() -> None:
     df = pl.DataFrame(
         {
             "foo": [1, 2, 3, 4, 5],
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_empty.py` & `polars_lts_cpu-0.18.2/tests/unit/test_empty.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_errors.py` & `polars_lts_cpu-0.18.2/tests/unit/test_errors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.18.2/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_exprs.py` & `polars_lts_cpu-0.18.2/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_fmt.py` & `polars_lts_cpu-0.18.2/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_interchange.py` & `polars_lts_cpu-0.18.2/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_interop.py` & `polars_lts_cpu-0.18.2/tests/unit/test_interop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_lazy.py` & `polars_lts_cpu-0.18.2/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.18.2/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_predicates.py` & `polars_lts_cpu-0.18.2/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_projections.py` & `polars_lts_cpu-0.18.2/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_queries.py` & `polars_lts_cpu-0.18.2/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_rows.py` & `polars_lts_cpu-0.18.2/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_schema.py` & `polars_lts_cpu-0.18.2/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_selectors.py` & `polars_lts_cpu-0.18.2/tests/unit/test_selectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,26 +72,28 @@
     ]
     assert df.select(~cs.contains(("b", "e", "g"))).columns == [
         "JJK",
         "Lmn",
         "opp",
         "qqR",
     ]
+    assert df.select(cs.contains(("ee", "x"))).columns == ["eee"]
 
 
 def test_selector_datetime(df: pl.DataFrame) -> None:
     assert df.select(cs.datetime()).schema == {"opp": pl.Datetime("ms")}
     assert df.select(cs.datetime("ns")).schema == {}
 
     all_columns = set(df.columns)
     assert set(df.select(~cs.datetime()).columns) == all_columns - {"opp"}
 
 
 def test_selector_ends_with(df: pl.DataFrame) -> None:
     assert df.select(cs.ends_with("e")).columns == ["cde", "eee"]
+    assert df.select(cs.ends_with("ee")).columns == ["eee"]
     assert df.select(cs.ends_with("e", "g", "i", "n", "p")).columns == [
         "cde",
         "eee",
         "fgg",
         "ghi",
         "Lmn",
         "opp",
@@ -161,14 +163,15 @@
     assert set(df.select(~cs.numeric()).columns) == (
         all_columns - {"abc", "bbb", "cde", "def"}
     )
 
 
 def test_selector_startswith(df: pl.DataFrame) -> None:
     assert df.select(cs.starts_with("a")).columns == ["abc"]
+    assert df.select(cs.starts_with("ee")).columns == ["eee"]
     assert df.select(cs.starts_with("d", "e", "f", "g", "h", "i", "j")).columns == [
         "def",
         "eee",
         "fgg",
         "ghi",
     ]
     assert df.select(~cs.starts_with("d", "e", "f", "g", "h", "i", "j")).columns == [
```

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_serde.py` & `polars_lts_cpu-0.18.2/tests/unit/test_serde.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_series.py` & `polars_lts_cpu-0.18.2/tests/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_single.py` & `polars_lts_cpu-0.18.2/tests/unit/test_single.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_sql.py` & `polars_lts_cpu-0.18.2/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/test_testing.py` & `polars_lts_cpu-0.18.2/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/utils/test_parse_expr_input.py` & `polars_lts_cpu-0.18.2/tests/unit/utils/test_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.18.2/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.18.1/Cargo.lock` & `polars_lts_cpu-0.18.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1678,15 +1678,15 @@
 checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.18.1"
+version = "0.18.2"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
```

### Comparing `polars_lts_cpu-0.18.1/PKG-INFO` & `polars_lts_cpu-0.18.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.18.1
+Version: 0.18.2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.18.1 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.18.2 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
```

