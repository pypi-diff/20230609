# Comparing `tmp/evadb-0.2.7.tar.gz` & `tmp/evadb-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evadb-0.2.7.tar", last modified: Thu Jun  8 00:40:00 2023, max compression
+gzip compressed data, was "evadb-0.2.8.tar", last modified: Fri Jun  9 04:10:28 2023, max compression
```

## Comparing `evadb-0.2.7.tar` & `evadb-0.2.8.tar`

### file list

```diff
@@ -1,469 +1,470 @@
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.974635 evadb-0.2.7/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2022-08-11 16:20:33.000000 evadb-0.2.7/LICENSE.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-08 00:40:00.974635 evadb-0.2.7/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13539 2023-06-07 03:30:14.000000 evadb-0.2.7/README.md
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.914633 evadb-0.2.7/evadb/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      903 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.914633 evadb-0.2.7/evadb/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8760 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/binder/binder_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15514 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/binder/statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7980 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/binder/statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.914633 evadb-0.2.7/evadb/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19315 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3322 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/catalog_type.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9335 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/catalog_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.918633 evadb-0.2.7/evadb/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1501 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/association_models.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4749 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/base_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4549 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/column_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2869 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/index_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2439 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/table_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3020 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/udf_cache_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3099 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/udf_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1802 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/udf_cost_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3921 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/udf_io_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2203 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/udf_metadata_catalog.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6787 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/models/utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2124 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/schema_utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.918633 evadb-0.2.7/evadb/catalog/services/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1289 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/base_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3375 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/column_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2968 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/index_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4959 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/table_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3997 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/udf_cache_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3247 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/udf_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3034 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/udf_cost_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2932 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/udf_io_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2224 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/services/udf_metadata_catalog_service.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2730 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/catalog/sql_config.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.918633 evadb-0.2.7/evadb/configuration/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/configuration/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5058 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/configuration/bootstrap_environment.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2501 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/configuration/configuration_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1017 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/configuration/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      882 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/constants.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1957 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/database.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2002 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2657 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/eva_server.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      566 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/evadb.yml
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3795 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2318 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/apply_and_merge_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2029 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/create_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5093 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1946 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/create_mat_view_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7178 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4734 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4993 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/drop_object_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3613 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/exchange_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3023 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5371 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/executor_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1590 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1999 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/function_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1891 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/groupby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1938 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/hash_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2241 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1682 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/join_build_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1837 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/lateral_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1649 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3078 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/load_csv_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1736 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5944 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/load_multimedia_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1610 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/nested_loop_join_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4257 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8302 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1710 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/pp_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1361 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/predicate_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1356 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/project_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2076 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/ray_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1261 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1479 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1912 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1840 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2616 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/storage_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1330 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/union_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4389 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/executor/vector_index_scan_executor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5559 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3977 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/aggregation_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1622 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/arithmetic_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4355 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/comparison_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2548 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/constant_value_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10443 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10044 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3057 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/logical_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4691 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/expression/tuple_value_expression.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/interfaces/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/interfaces/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/interfaces/relational/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/interfaces/relational/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11182 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/interfaces/relational/db.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7504 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/interfaces/relational/relation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4618 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/interfaces/relational/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      633 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1334 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/catalog/frame_info.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      857 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/catalog/properties.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/models/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1967 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/server/response.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.926633 evadb-0.2.7/evadb/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15328 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/models/storage/batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.930633 evadb-0.2.7/evadb/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      620 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3267 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2143 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3458 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2675 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/group_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4345 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    36733 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/operators.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4009 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      984 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/optimizer_task_stack.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12596 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/optimizer_tasks.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11288 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4275 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/plan_generator.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1169 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/property.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.930633 evadb-0.2.7/evadb/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1021 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/rules/pattern.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    49297 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/rules/rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7374 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/rules/rules_base.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7509 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/rules/rules_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13356 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/optimizer/statement_to_opr_converter.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.934633 evadb-0.2.7/evadb/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1360 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/alias.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2752 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/create_index_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2882 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/create_mat_view_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5322 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/create_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4434 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/create_udf_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2056 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2129 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/drop_object_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19687 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/evadb.lark
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1388 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2930 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/insert_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1720 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_parser.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.934633 evadb-0.2.7/evadb/parser/lark_visitor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2683 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2169 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_common_clauses_ids.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10838 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_create_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1408 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_delete_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_drop_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1008 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_explain_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4682 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_expressions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5778 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_functions.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2471 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_insert_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2245 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      936 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2147 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1116 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_show_statements.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9479 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/lark_visitor/_table_sources.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3222 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/load_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1231 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2013 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/rename_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6256 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/select_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1464 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/show_statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1428 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/statement.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8647 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/table_ref.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1868 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4269 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/parser/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1697 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/abstract_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3455 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/abstract_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1461 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/abstract_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1938 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/apply_and_merge_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2481 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/create_index_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2084 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/create_mat_view_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2208 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/create_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3611 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/create_udf_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1959 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/delete_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1497 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/drop_object_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2061 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/exchange_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1037 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/explain_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1761 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/function_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1505 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/groupby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1720 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/hash_join_build_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2189 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/hash_join_probe_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2031 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/insert_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1416 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/lateral_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1474 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/limit_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2718 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/load_data_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1518 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/nested_loop_join_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1568 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/orderby_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1183 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/pp_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1251 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/predicate_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1255 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/project_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1622 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/rename_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1475 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/sample_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1766 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/seq_scan_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1207 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/show_info_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4429 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/storage_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1406 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1249 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/union_plan.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2730 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/plan_nodes/vector_index_scan_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2326 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/abstract_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2654 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5999 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/readers/document/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/document/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1471 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/document/document_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1979 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/document/registry.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/readers/image/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/image/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1069 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/image/opencv_image_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2052 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/readers/pdf_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      623 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3464 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/server/command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3599 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/server/interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3347 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/server/server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6181 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/abstract_media_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2491 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/abstract_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1779 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/document_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1783 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/image_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1758 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/pdf_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9491 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2058 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2556 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/storage/video_storage_engine.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.942634 evadb-0.2.7/evadb/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      605 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.946634 evadb-0.2.7/evadb/third_party/huggingface/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      612 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/huggingface/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1426 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/huggingface/binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6481 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/huggingface/create.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2619 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/huggingface/model.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.946634 evadb-0.2.7/evadb/third_party/vector_stores/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/vector_stores/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3286 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/vector_stores/faiss.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2962 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/vector_stores/qdrant.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1376 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/vector_stores/types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1606 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/third_party/vector_stores/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.946634 evadb-0.2.7/evadb/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.950634 evadb-0.2.7/evadb/udfs/abstract/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/abstract/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2442 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/abstract/abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4046 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/abstract/hf_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3849 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/abstract/pytorch_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3922 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/abstract/tracker_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3466 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/asl_action_recognition.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3440 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/chatgpt.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.950634 evadb-0.2.7/evadb/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/decorators/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2190 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/decorators/decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.954634 evadb-0.2.7/evadb/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2759 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/decorators/io_descriptors/abstract_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3384 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/decorators/io_descriptors/data_types.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2071 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/decorators/utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5480 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2545 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/face_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6020 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1824 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1028 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/gpu_compatible.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3530 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/mnist_image_classifier.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2202 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/mvit_action_recognition.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.954634 evadb-0.2.7/evadb/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2480 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/annotate.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2570 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1649 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1181 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2208 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/gaussian_blur.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2210 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/horizontal_flip.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1559 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1784 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2147 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/to_grayscale.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2196 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ndarray/vertical_flip.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2754 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/ocr_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2703 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/saliency_feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2763 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/sentence_transformer_feature_extractor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2909 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/sift_feature_extractor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.954634 evadb-0.2.7/evadb/udfs/trackers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/trackers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2371 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/trackers/nor_fair.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.954634 evadb-0.2.7/evadb/udfs/tutorials/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      636 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/tutorials/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7899 2023-06-08 00:38:31.000000 evadb-0.2.7/evadb/udfs/udf_bootstrap_queries.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3869 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/udfs/yolo_object_detector.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.954634 evadb-0.2.7/evadb/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      611 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      909 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/errors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6759 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1956 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/kv_cache.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      985 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/logging_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1388 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/math_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1562 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/s3_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1694 2023-06-07 23:17:50.000000 evadb-0.2.7/evadb/utils/stats.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-08 00:39:58.000000 evadb-0.2.7/evadb/version.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.914633 evadb-0.2.7/evadb.egg-info/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14211 2023-06-08 00:40:00.000000 evadb-0.2.7/evadb.egg-info/PKG-INFO
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14182 2023-06-08 00:40:00.000000 evadb-0.2.7/evadb.egg-info/SOURCES.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-08 00:40:00.000000 evadb-0.2.7/evadb.egg-info/dependency_links.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       92 2023-06-08 00:40:00.000000 evadb-0.2.7/evadb.egg-info/entry_points.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1373 2023-06-08 00:40:00.000000 evadb-0.2.7/evadb.egg-info/requires.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       23 2023-06-08 00:40:00.000000 evadb-0.2.7/evadb.egg-info/top_level.txt
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2022-06-26 17:11:46.000000 evadb-0.2.7/pyproject.toml
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-08 00:40:00.974635 evadb-0.2.7/setup.cfg
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4617 2023-06-07 23:17:50.000000 evadb-0.2.7/setup.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.958634 evadb-0.2.7/test/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-09-30 14:20:49.000000 evadb-0.2.7/test/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.958634 evadb-0.2.7/test/benchmark_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:53.000000 evadb-0.2.7/test/benchmark_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1263 2023-06-07 23:17:50.000000 evadb-0.2.7/test/benchmark_tests/conftest.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6891 2023-06-07 23:17:50.000000 evadb-0.2.7/test/benchmark_tests/test_benchmark_pytorch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.958634 evadb-0.2.7/test/binder/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/binder/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14197 2023-06-07 23:17:50.000000 evadb-0.2.7/test/binder/test_statement_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8054 2023-06-07 23:17:50.000000 evadb-0.2.7/test/binder/test_statement_binder_context.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.958634 evadb-0.2.7/test/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/catalog/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.958634 evadb-0.2.7/test/catalog/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/catalog/models/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7246 2023-06-07 23:17:50.000000 evadb-0.2.7/test/catalog/models/test_models.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7353 2023-06-07 23:17:50.000000 evadb-0.2.7/test/catalog/test_catalog_manager.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1404 2023-06-07 23:17:50.000000 evadb-0.2.7/test/catalog/test_column_type.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.958634 evadb-0.2.7/test/executor/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/executor/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1108 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_abstract_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4079 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_create_udf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4271 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_execution_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4745 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_limit_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2934 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_orderby_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9931 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_plan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1865 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_sample_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3035 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/test_seq_scan_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      849 2023-06-07 23:17:50.000000 evadb-0.2.7/test/executor/utils.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.962634 evadb-0.2.7/test/expression/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/expression/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3732 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_abstract_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5157 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_aggregation.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2983 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_arithmetic.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5588 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_comparison.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2881 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_expression_tree.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7569 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_expression_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2699 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_function_expression.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10254 2023-06-07 23:17:50.000000 evadb-0.2.7/test/expression/test_logical.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/integration_tests/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/integration_tests/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3701 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6122 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_create_index_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3894 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_create_table_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5195 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_delete_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7099 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_drop_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2371 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_error_handling_with_ray.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3681 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_explain_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3264 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_fuzzy_join.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17569 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_huggingface_udfs.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3956 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_insert_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3092 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_like.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    21878 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2018 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_load_pdf_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7734 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_mat_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2665 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11067 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_optimizer_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15564 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_pytorch.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3081 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_rename_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10842 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_reuse.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5315 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_s3_load_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2349 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_saliency.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    31937 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_select_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3434 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_show_info_executor.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15007 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_similarity.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12509 2023-06-07 23:17:50.000000 evadb-0.2.7/test/integration_tests/test_udf_executor.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/interfaces/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 23:17:50.000000 evadb-0.2.7/test/interfaces/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/interfaces/relational/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-06-07 03:30:15.000000 evadb-0.2.7/test/interfaces/relational/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12369 2023-06-07 23:17:50.000000 evadb-0.2.7/test/interfaces/relational/test_relational_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1604 2023-06-07 23:17:50.000000 evadb-0.2.7/test/markers.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/models/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/models/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/models/catalog/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/models/catalog/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1014 2023-06-07 23:17:50.000000 evadb-0.2.7/test/models/catalog/test_frame_info.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/models/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/models/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5923 2023-06-07 23:17:50.000000 evadb-0.2.7/test/models/storage/test_batch.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/optimizer/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/optimizer/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.966635 evadb-0.2.7/test/optimizer/rules/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.7/test/optimizer/rules/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11752 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/rules/test_rules.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4244 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_binder.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2327 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_cascade_optimizer.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4510 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_cost_model.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2695 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_group.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2000 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_memo.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1051 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_optimizer_context.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5666 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_optimizer_task.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2006 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_optimizer_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13111 2023-06-07 23:17:50.000000 evadb-0.2.7/test/optimizer/test_statement_to_opr_converter.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/parser/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/parser/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35632 2023-06-07 23:17:50.000000 evadb-0.2.7/test/parser/test_parser.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7795 2023-06-07 23:17:50.000000 evadb-0.2.7/test/parser/test_parser_statements.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/plan_nodes/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-01-02 23:54:50.000000 evadb-0.2.7/test/plan_nodes/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5985 2023-06-07 23:17:50.000000 evadb-0.2.7/test/plan_nodes/test_plan.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/readers/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/readers/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1692 2023-06-07 23:17:50.000000 evadb-0.2.7/test/readers/test_csv_reader.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8120 2023-06-07 23:17:50.000000 evadb-0.2.7/test/readers/test_decord_reader.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/server/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-11-12 17:07:12.000000 evadb-0.2.7/test/server/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1276 2023-06-07 23:17:50.000000 evadb-0.2.7/test/server/test_command_handler.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5169 2023-06-07 23:17:50.000000 evadb-0.2.7/test/server/test_db_api.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2615 2023-06-07 23:17:50.000000 evadb-0.2.7/test/server/test_interpreter.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2078 2023-06-07 23:17:50.000000 evadb-0.2.7/test/server/test_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/storage/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/storage/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4510 2023-06-07 23:17:50.000000 evadb-0.2.7/test/storage/test_sqlite_storage_engine.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4163 2023-06-07 23:17:50.000000 evadb-0.2.7/test/storage/test_video_storage.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3321 2023-06-07 23:17:50.000000 evadb-0.2.7/test/test_eva_cmd_client.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1298 2023-06-07 23:17:50.000000 evadb-0.2.7/test/test_eva_imports.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1330 2023-06-07 23:17:50.000000 evadb-0.2.7/test/test_eva_server.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/udfs/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2022-08-08 22:30:00.000000 evadb-0.2.7/test/udfs/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/udfs/decorators/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.7/test/udfs/decorators/__init__.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.970635 evadb-0.2.7/test/udfs/decorators/io_descriptors/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2023-03-28 02:19:14.000000 evadb-0.2.7/test/udfs/decorators/io_descriptors/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7435 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/decorators/io_descriptors/test_descriptors.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2143 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/decorators/test_decorators.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.974635 evadb-0.2.7/test/udfs/ndarray/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      648 2022-10-16 04:44:32.000000 evadb-0.2.7/test/udfs/ndarray/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1846 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_annotate.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      851 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_array_count.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2412 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_crop.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2018 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_flips.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1661 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_gaussian_blur.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2262 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_open.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1654 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/ndarray/test_to_grayscale.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4422 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/test_abstract_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5405 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/test_chatgpt.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2158 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/test_emotion_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3357 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/test_facenet_udf.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2556 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/test_fastrcnn_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2772 2023-06-07 23:17:50.000000 evadb-0.2.7/test/udfs/test_yolo_object_detector.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17773 2023-06-07 23:17:50.000000 evadb-0.2.7/test/util.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.974635 evadb-0.2.7/test/utils/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      587 2022-08-08 22:30:00.000000 evadb-0.2.7/test/utils/__init__.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3871 2023-06-07 23:17:50.000000 evadb-0.2.7/test/utils/test_generic_utils.py
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2281 2023-06-07 23:17:50.000000 evadb-0.2.7/test/utils/test_timer.py
-drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 00:40:00.974635 evadb-0.2.7/third_party/
--rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2022-06-26 17:11:46.000000 evadb-0.2.7/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11357 2023-06-08 04:02:21.000000 evadb-0.2.8/LICENSE.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14468 2023-06-09 04:10:28.674551 evadb-0.2.8/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13794 2023-06-09 04:00:45.000000 evadb-0.2.8/README.md
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.630549 evadb-0.2.8/evadb/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      905 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.634549 evadb-0.2.8/evadb/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8762 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/binder/binder_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15520 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/binder/statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7982 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/binder/statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.634549 evadb-0.2.8/evadb/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19317 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3346 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/catalog_type.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9337 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/catalog_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.634549 evadb-0.2.8/evadb/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1503 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/association_models.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4751 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/base_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4551 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/column_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2871 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/index_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2441 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/table_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3022 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/udf_cache_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3101 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/udf_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1804 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/udf_cost_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3923 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/udf_io_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2205 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/udf_metadata_catalog.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6789 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/models/utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2126 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/schema_utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.634549 evadb-0.2.8/evadb/catalog/services/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1291 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/base_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3377 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/column_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2970 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/index_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4961 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/table_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3999 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/udf_cache_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3249 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/udf_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3036 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/udf_cost_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2934 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/udf_io_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2226 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/services/udf_metadata_catalog_service.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2732 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/catalog/sql_config.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.638550 evadb-0.2.8/evadb/configuration/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      622 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/configuration/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5035 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/configuration/bootstrap_environment.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2508 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/configuration/configuration_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1031 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/configuration/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      884 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/constants.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1964 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/database.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      568 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/evadb.yml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2018 2023-06-08 22:16:07.000000 evadb-0.2.8/evadb/evadb_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2023-06-08 22:16:07.000000 evadb-0.2.8/evadb/evadb_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      617 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3803 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2324 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/apply_and_merge_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2035 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/create_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5099 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1952 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/create_mat_view_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7186 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4740 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4999 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/drop_object_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3619 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/exchange_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3025 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5373 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/executor_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1596 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2005 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/function_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1897 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/groupby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1944 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/hash_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2247 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1688 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/join_build_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1843 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/lateral_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1655 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3084 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/load_csv_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1742 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5950 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/load_multimedia_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1616 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/nested_loop_join_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4263 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8310 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1716 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/pp_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1367 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/predicate_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1362 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/project_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2078 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/ray_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1267 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1485 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1918 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1846 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2622 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/storage_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1336 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/union_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4395 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/executor/vector_index_scan_executor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      619 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5561 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3979 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/aggregation_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1624 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/arithmetic_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4357 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/comparison_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2550 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/constant_value_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10445 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10046 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3059 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/logical_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4693 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/expression/tuple_value_expression.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/interfaces/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/interfaces/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/interfaces/relational/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/interfaces/relational/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12597 2023-06-09 01:44:52.000000 evadb-0.2.8/evadb/interfaces/relational/db.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7741 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/interfaces/relational/relation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4628 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/interfaces/relational/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      637 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1336 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/catalog/frame_info.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      859 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/catalog/properties.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/models/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1971 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/server/response.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.642550 evadb-0.2.8/evadb/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15330 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/models/storage/batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.646550 evadb-0.2.8/evadb/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      624 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3269 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2145 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3460 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2677 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/group_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4347 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    36735 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/operators.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4040 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      986 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/optimizer_task_stack.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12600 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/optimizer_tasks.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11290 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4281 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/plan_generator.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1171 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/property.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.646550 evadb-0.2.8/evadb/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1023 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/rules/pattern.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    49299 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/rules/rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7376 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/rules/rules_base.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7511 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/rules/rules_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13358 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/optimizer/statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.646550 evadb-0.2.8/evadb/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1362 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/alias.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2754 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/create_index_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2884 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/create_mat_view_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5324 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/create_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4436 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/create_udf_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2058 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2131 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/drop_object_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    19687 2023-06-08 15:06:21.000000 evadb-0.2.8/evadb/parser/evadb.lark
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1390 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2932 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/insert_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1724 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_parser.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.650550 evadb-0.2.8/evadb/parser/lark_visitor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2685 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2171 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_common_clauses_ids.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10840 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_create_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1410 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_delete_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2007 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_drop_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1010 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_explain_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4684 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_expressions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5780 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_functions.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2473 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_insert_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2247 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      938 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2149 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1118 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_show_statements.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9481 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/lark_visitor/_table_sources.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3224 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/load_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1233 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2015 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/rename_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6258 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/select_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1466 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/show_statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1430 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/statement.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8649 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/table_ref.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1892 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4271 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/parser/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      616 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1699 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/abstract_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3457 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/abstract_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1463 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/abstract_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1940 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/apply_and_merge_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2483 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/create_index_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2086 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/create_mat_view_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2210 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/create_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3483 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/create_udf_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1961 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/delete_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1499 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/drop_object_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2063 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/exchange_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1039 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/explain_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1763 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/function_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1507 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/groupby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1722 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/hash_join_build_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2191 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/hash_join_probe_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2033 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/insert_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1418 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/lateral_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1476 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/limit_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2720 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/load_data_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1520 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/nested_loop_join_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1570 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/orderby_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1185 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/pp_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1253 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/predicate_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1257 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/project_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1624 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/rename_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1477 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/sample_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1768 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/seq_scan_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1209 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/show_info_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4431 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/storage_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1408 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1251 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/union_plan.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2732 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/plan_nodes/vector_index_scan_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2328 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/abstract_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2656 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6001 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/readers/document/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/document/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1473 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/document/document_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1981 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/document/registry.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/readers/image/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/image/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1071 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/image/opencv_image_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2054 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/readers/pdf_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      625 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3474 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/server/command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3609 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/server/interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3357 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/server/server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6187 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/abstract_media_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2497 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/abstract_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1785 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/document_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1789 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/image_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1764 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/pdf_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9483 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2066 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2562 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/storage/video_storage_engine.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      607 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/third_party/huggingface/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      614 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/huggingface/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1428 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/huggingface/binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6485 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/huggingface/create.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2625 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/huggingface/model.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.654550 evadb-0.2.8/evadb/third_party/vector_stores/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      609 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/vector_stores/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3288 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/vector_stores/faiss.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2964 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/vector_stores/qdrant.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1378 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/vector_stores/types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1608 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/third_party/vector_stores/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.658550 evadb-0.2.8/evadb/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      618 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.658550 evadb-0.2.8/evadb/udfs/abstract/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      627 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/abstract/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2446 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/abstract/abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4058 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/abstract/hf_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3853 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/abstract/pytorch_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3928 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/abstract/tracker_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3468 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/asl_action_recognition.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3600 2023-06-09 01:44:52.000000 evadb-0.2.8/evadb/udfs/chatgpt.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.658550 evadb-0.2.8/evadb/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/decorators/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2192 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/decorators/decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.658550 evadb-0.2.8/evadb/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2761 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/decorators/io_descriptors/abstract_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3386 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/decorators/io_descriptors/data_types.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2073 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/decorators/utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5482 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2547 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/face_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6022 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1826 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1030 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/gpu_compatible.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3532 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/mnist_image_classifier.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2204 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/mvit_action_recognition.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/evadb/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      640 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2482 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2572 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1651 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1183 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2210 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2212 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/horizontal_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1561 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1786 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2149 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2198 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ndarray/vertical_flip.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2756 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/ocr_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2705 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/saliency_feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3214 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/sentence_feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2177 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/sentence_transformer_feature_extractor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2911 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/sift_feature_extractor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/evadb/udfs/trackers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/trackers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2377 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/trackers/nor_fair.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/evadb/udfs/tutorials/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      638 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/tutorials/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8636 2023-06-09 01:44:52.000000 evadb-0.2.8/evadb/udfs/udf_bootstrap_queries.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3871 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/udfs/yolo_object_detector.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/evadb/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      615 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      911 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/errors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6763 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1958 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/kv_cache.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      987 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/logging_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1390 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/math_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1564 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/s3_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1696 2023-06-08 22:16:06.000000 evadb-0.2.8/evadb/utils/stats.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      123 2023-06-09 04:10:26.000000 evadb-0.2.8/evadb/version.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.634549 evadb-0.2.8/evadb.egg-info/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14468 2023-06-09 04:10:28.000000 evadb-0.2.8/evadb.egg-info/PKG-INFO
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14227 2023-06-09 04:10:28.000000 evadb-0.2.8/evadb.egg-info/SOURCES.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        1 2023-06-09 04:10:28.000000 evadb-0.2.8/evadb.egg-info/dependency_links.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       96 2023-06-09 04:10:28.000000 evadb-0.2.8/evadb.egg-info/entry_points.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1423 2023-06-09 04:10:28.000000 evadb-0.2.8/evadb.egg-info/requires.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       23 2023-06-09 04:10:28.000000 evadb-0.2.8/evadb.egg-info/top_level.txt
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       90 2023-06-08 04:02:21.000000 evadb-0.2.8/pyproject.toml
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)       38 2023-06-09 04:10:28.674551 evadb-0.2.8/setup.cfg
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4702 2023-06-09 04:08:06.000000 evadb-0.2.8/setup.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/test/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/test/benchmark_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/benchmark_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1265 2023-06-08 22:16:06.000000 evadb-0.2.8/test/benchmark_tests/conftest.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6893 2023-06-08 22:16:06.000000 evadb-0.2.8/test/benchmark_tests/test_benchmark_pytorch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/test/binder/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/binder/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    14199 2023-06-08 22:16:06.000000 evadb-0.2.8/test/binder/test_statement_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8056 2023-06-08 22:16:06.000000 evadb-0.2.8/test/binder/test_statement_binder_context.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/test/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/catalog/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.662551 evadb-0.2.8/test/catalog/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/catalog/models/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7252 2023-06-08 22:16:06.000000 evadb-0.2.8/test/catalog/models/test_models.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7355 2023-06-08 22:16:06.000000 evadb-0.2.8/test/catalog/test_catalog_manager.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1406 2023-06-08 22:16:06.000000 evadb-0.2.8/test/catalog/test_column_type.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.666551 evadb-0.2.8/test/executor/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1110 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_abstract_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4081 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_create_udf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4273 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_execution_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4747 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_limit_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2936 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_orderby_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     9933 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_plan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1867 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_sample_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3037 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/test_seq_scan_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      851 2023-06-08 22:16:06.000000 evadb-0.2.8/test/executor/utils.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.666551 evadb-0.2.8/test/expression/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3734 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_abstract_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5159 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_aggregation.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2985 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_arithmetic.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5590 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_comparison.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2883 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_expression_tree.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7571 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_expression_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2701 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_function_expression.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10256 2023-06-08 22:16:06.000000 evadb-0.2.8/test/expression/test_logical.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/integration_tests/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3703 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     6124 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_create_index_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3900 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_create_table_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5205 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_delete_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7102 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_drop_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2373 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_error_handling_with_ray.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3683 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_explain_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2862 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_fuzzy_join.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17573 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_huggingface_udfs.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3964 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_insert_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3100 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_like.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    21912 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2024 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_load_pdf_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7740 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_mat_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2667 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11073 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_optimizer_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15580 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_pytorch.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3083 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_rename_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    10854 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_reuse.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5321 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_s3_load_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2361 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_saliency.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    31947 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_select_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3452 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_show_info_executor.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    15009 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_similarity.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12511 2023-06-08 22:16:06.000000 evadb-0.2.8/test/integration_tests/test_udf_executor.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/interfaces/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/interfaces/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/interfaces/relational/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/interfaces/relational/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    12386 2023-06-08 22:16:07.000000 evadb-0.2.8/test/interfaces/relational/test_relational_api.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1606 2023-06-08 22:16:06.000000 evadb-0.2.8/test/markers.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/models/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/models/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/models/catalog/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/models/catalog/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1016 2023-06-08 22:16:06.000000 evadb-0.2.8/test/models/catalog/test_frame_info.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/models/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/models/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5925 2023-06-08 22:16:06.000000 evadb-0.2.8/test/models/storage/test_batch.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/optimizer/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/optimizer/rules/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/rules/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    11754 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/rules/test_rules.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4246 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_binder.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2329 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_cascade_optimizer.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4512 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_cost_model.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2697 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_group.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2002 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_memo.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1053 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_optimizer_context.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5668 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_optimizer_task.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2008 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_optimizer_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    13113 2023-06-08 22:16:06.000000 evadb-0.2.8/test/optimizer/test_statement_to_opr_converter.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/parser/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/parser/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    35848 2023-06-08 22:16:06.000000 evadb-0.2.8/test/parser/test_parser.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7797 2023-06-08 22:16:06.000000 evadb-0.2.8/test/parser/test_parser_statements.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/plan_nodes/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/plan_nodes/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5987 2023-06-08 22:16:06.000000 evadb-0.2.8/test/plan_nodes/test_plan.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/readers/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/readers/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1694 2023-06-08 22:16:06.000000 evadb-0.2.8/test/readers/test_csv_reader.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     8128 2023-06-08 22:16:06.000000 evadb-0.2.8/test/readers/test_decord_reader.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.670551 evadb-0.2.8/test/server/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/server/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1278 2023-06-08 22:16:06.000000 evadb-0.2.8/test/server/test_command_handler.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     5221 2023-06-08 22:16:06.000000 evadb-0.2.8/test/server/test_db_api.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2617 2023-06-08 22:16:06.000000 evadb-0.2.8/test/server/test_interpreter.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2171 2023-06-08 22:16:06.000000 evadb-0.2.8/test/server/test_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/test/storage/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/storage/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4512 2023-06-08 22:16:06.000000 evadb-0.2.8/test/storage/test_sqlite_storage_engine.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4165 2023-06-08 22:16:06.000000 evadb-0.2.8/test/storage/test_video_storage.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3341 2023-06-08 22:16:06.000000 evadb-0.2.8/test/test_eva_cmd_client.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1310 2023-06-08 22:16:06.000000 evadb-0.2.8/test/test_eva_imports.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1427 2023-06-08 22:16:06.000000 evadb-0.2.8/test/test_eva_server.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/test/udfs/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      640 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/test/udfs/decorators/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/decorators/__init__.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/test/udfs/decorators/io_descriptors/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/decorators/io_descriptors/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     7437 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/decorators/io_descriptors/test_descriptors.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2145 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/decorators/test_decorators.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/test/udfs/ndarray/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      650 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1852 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_annotate.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      853 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_array_count.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2414 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_crop.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2026 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_flips.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1671 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_gaussian_blur.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2264 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_open.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     1668 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/ndarray/test_to_grayscale.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4424 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/test_abstract_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     4083 2023-06-09 01:44:52.000000 evadb-0.2.8/test/udfs/test_chatgpt.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2164 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/test_emotion_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3363 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/test_facenet_udf.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2558 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/test_fastrcnn_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2774 2023-06-08 22:16:06.000000 evadb-0.2.8/test/udfs/test_yolo_object_detector.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)    17789 2023-06-08 22:16:06.000000 evadb-0.2.8/test/util.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/test/utils/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)      589 2023-06-08 22:16:06.000000 evadb-0.2.8/test/utils/__init__.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     3939 2023-06-08 22:16:06.000000 evadb-0.2.8/test/utils/test_generic_utils.py
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)     2283 2023-06-08 22:16:06.000000 evadb-0.2.8/test/utils/test_timer.py
+drwxr-xr-x   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-09 04:10:28.674551 evadb-0.2.8/third_party/
+-rw-r--r--   0 jarulraj3 (347863) gtperson  (2626)        0 2023-06-08 04:02:21.000000 evadb-0.2.8/third_party/__init__.py
```

### Comparing `evadb-0.2.7/LICENSE.txt` & `evadb-0.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `evadb-0.2.7/PKG-INFO` & `evadb-0.2.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: evadb
-Version: 0.2.7
-Summary: EVA AI-Relational Database System
+Version: 0.2.8
+Summary: EvaDB AI-Relational Database System
 Home-page: https://github.com/georgia-tech-db/eva
 Download-URL: https://github.com/georgia-tech-db/eva
 Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu
 License: Apache License 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -13,19 +13,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE.txt
 
-# EVA AI-SQL Database System
+# EvaDB AI-SQL Database System
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EvaDB on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
         </a>          
         <a href="https://twitter.com/evadb_ai">
             <img alt="Twitter" src="https://img.shields.io/badge/twitter-eva-bde1ee.svg?logo=twitter">
         </a>  
@@ -37,21 +37,21 @@
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
         </a>
         <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
 </div>
 
-<p align="center"> <b><h3>EVA DB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+<p align="center"> <b><h3>EvaDB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
-EVA DB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (videos, text, podcasts, PDFs, etc.).
+EvaDB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (text documents, videos, PDFs, podcasts, etc.).
 
-EVA DB accelerates AI pipelines by 10-100x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
+EvaDB accelerates AI pipelines by 10x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EvaDB supports an AI-oriented query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
 
-The high-level SQL API allows even beginners to use EVA in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EVA DB is fully implemented in Python and licensed under the Apache license.
+The high-level Python and SQL APIs allows even beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under the Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
@@ -61,60 +61,60 @@
 - [Community and Support](#community-and-support)
 - [Twitter](https://twitter.com/evadb_ai)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
 
-- 🔮 Build simpler AI-powered applications using short SQL-like queries
-- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
+- 🔮 Build simpler AI-powered applications using short Python or SQL queries
+- ⚡️ 10x faster applications using AI-centric query optimization  
 - 💰 Save money spent on GPUs
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
 - ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Illustrative Applications
 
-Here are some illustrative EVA-powered applications (each Jupyter notebook can be opened on Google Colab):
+Here are some illustrative EvaDB-powered applications (each Jupyter notebook can be opened on Google Colab):
 
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
- * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Reddit Image Similarity Search</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">ChatGPT-based video question answering</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html">Quering PDF documents</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow with YOLO</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining emotion palette of a movie</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image segmentation with Hugging Face</a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates</a>
  * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
 
 ## Documentation
 
 * [Detailed Documentation](https://evadb.readthedocs.io/)
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI tasks and how you can easily extend EVA to support your custom deep learning model through user-defined functions.
-  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code yourself.
+  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EvaDB for different AI tasks and how you can easily extend EvaDB to support your custom deep learning model through user-defined functions.
+  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EvaDB. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 * [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html)
 
 ## Quick Start
 
-- Install EVA using the pip package manager. EVA supports Python versions >= 3.8:
+- Install EvaDB using the pip package manager. EvaDB supports Python versions >= 3.8:
 
 ```shell
 pip install evadb
 ```
 
-- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+- To launch and connect to an EvaDB server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
 ```shell
 cursor = connect_to_server()
 ```
 
-- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+- Load a video onto the EvaDB server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
 
 ```mysql
 LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
 ```
 
 - That's it! You can now run queries over the loaded video:
 
@@ -156,19 +156,19 @@
 ```mysql
    -- Analyse emotions of faces in a video
    SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
    FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
    WHERE id < 15;
 ```
 
-- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
+- **EvaDB runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
 
-   💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+   💾 **Caching**: EvaDB automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
 
-   🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+   🎯 **Predicate Reordering**: EvaDB optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
 
 Consider these two exploratory queries on a dataset of dog images:
 <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
 
 ```mysql
   -- Query 1: Find all images of black-colored dogs
   SELECT id, bbox FROM dogs 
@@ -180,32 +180,38 @@
   SELECT id, bbox FROM dogs 
   JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
   WHERE Obj.label = 'dog' 
     AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
     AND Color(Crop(data, bbox)) = 'black';
 ```
 
-By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+By reusing the results of the first query and reordering the predicates based on the available cached inference results, EvaDB runs the second query **10x faster**!
 
 ## Architecture Diagram
 
-This diagram presents the key components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+This diagram presents the key components of EvaDB. EvaDB's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
 1. Structured data (SQL database system connected via `sqlalchemy`).
 2. Unstructured media data (on cloud buckets or local filesystem).
 3. Vector data (vector database system).
 
 <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
 ## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
+### 🔮 [PDF Question Answering](https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html) (Question Answering Model)
+
+| App |
+|-----|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/pdf-qa.webp" width="400"> |
+
 ### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
 
 ### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
 
@@ -217,31 +223,31 @@
 
 | Query Result |
 |--------------|
 <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
 
 ## Community and Support
 
-👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on Twitter](https://twitter.com/evadb_ai).
+👋 If you have general questions about EvaDB, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) and to [follow us on Twitter](https://twitter.com/evadb_ai).
 
 <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EvaDB Slack Channel" width="500">
 </a>
 
 If you run into any problems or issues, please create a Github issue and we'll try our best to help.
 
 Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our [roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from you.
 
 ## Contributing
 
 [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
 [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
 [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=latest)](https://evadb.readthedocs.io/en/latest/index.html)
 
-EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+EvaDB is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EvaDB are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
 Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,71 +1,70 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.7 Summary: EVA AI-Relational
+Metadata-Version: 2.1 Name: evadb Version: 0.2.8 Summary: EvaDB AI-Relational
 Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
 https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
 Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE.txt # EVA AI-SQL
+text/markdown Provides-Extra: dev License-File: LICENSE.txt # EvaDB AI-SQL
 Database System
-[Open_EVA_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
+[Open_EvaDB_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
 Status] [Downloads] [Python Versions]
-**** EVA DB is a database system for building simpler and faster AI-powered
+**** EvaDB is a database system for building simpler and faster AI-powered
 applications. ****
-EVA DB is an AI-SQL database system for developing applications powered by AI
+EvaDB is an AI-SQL database system for developing applications powered by AI
 models. We aim to simplify the development and deployment of AI-powered
 applications that operate on structured (tables, feature stores) and
-unstructured data (videos, text, podcasts, PDFs, etc.). EVA DB accelerates AI
-pipelines by 10-100x using a collection of performance optimizations inspired
-by time-tested SQL database systems, including data-parallel query execution,
-function caching, sampling, and cost-based predicate reordering. EVA supports
-an AI-oriented SQL-like query language tailored for analyzing both structured
-and unstructured data. It has first-class support for PyTorch, Hugging Face,
-YOLO, and Open AI models. The high-level SQL API allows even beginners to use
-EVA in a few lines of code. Advanced users can define custom user-defined
-functions that wrap around any AI model or Python library. EVA DB is fully
-implemented in Python and licensed under the Apache license. ## Quick Links -
-[Features](#features) - [Quick Start](#quick-start) - [Documentation]
-(#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Architecture Diagram](#architecture-diagram) - [Illustrative
-Applications](#illustrative-applications) - [Screenshots](#screenshots) -
-[Community and Support](#community-and-support) - [Twitter](https://
-twitter.com/evadb_ai) - [Contributing](#contributing) - [License](#license) ##
-Features - ð® Build simpler AI-powered applications using short SQL-like
-queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+unstructured data (text documents, videos, PDFs, podcasts, etc.). EvaDB
+accelerates AI pipelines by 10x using a collection of performance optimizations
+inspired by time-tested SQL database systems, including data-parallel query
+execution, function caching, sampling, and cost-based predicate reordering.
+EvaDB supports an AI-oriented query language tailored for analyzing both
+structured and unstructured data. It has first-class support for PyTorch,
+Hugging Face, YOLO, and Open AI models. The high-level Python and SQL APIs
+allows even beginners to use EvaDB in a few lines of code. Advanced users can
+define custom user-defined functions that wrap around any AI model or Python
+library. EvaDB is fully implemented in Python and licensed under the Apache
+license. ## Quick Links - [Features](#features) - [Quick Start](#quick-start) -
+[Documentation](#documentation) - [Roadmap](https://github.com/orgs/georgia-
+tech-db/projects/3) - [Architecture Diagram](#architecture-diagram) -
+[Illustrative Applications](#illustrative-applications) - [Screenshots]
+(#screenshots) - [Community and Support](#community-and-support) - [Twitter]
+(https://twitter.com/evadb_ai) - [Contributing](#contributing) - [License]
+(#license) ## Features - ð® Build simpler AI-powered applications using short
+Python or SQL queries - â¡ï¸ 10x faster applications using AI-centric query
 optimization - ð° Save money spent on GPUs - ð First-class support for
 your custom deep learning models through user-defined functions - ð¦ Built-in
 caching to eliminate redundant model invocations across queries - â¨ï¸ First-
 class support for PyTorch, Hugging Face, YOLO, and Open AI models - ð
 Installable via pip and fully implemented in Python ## Illustrative
-Applications Here are some illustrative EVA-powered applications (each Jupyter
-notebook can be opened on Google Colab): * ð® Using_ChatGPT_to_ask_questions
-based_on_videos * ð® Analysing_traffic_flow_at_an_intersection * ð®
-Examining_the_emotion_palette_of_actors_in_a_movie * ð® Image_Similarity
-Search_on_Reddit_[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their
-content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
-plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
-[Detailed Documentation](https://evadb.readthedocs.io/) - The Getting_Started
-page shows how you can use EVA for different AI tasks and how you can easily
-extend EVA to support your custom deep learning model through user-defined
-functions. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EVA. Each notebook includes a link
-to Google Colab, where you can run the code yourself. * [Tutorials](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/
-evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/
-projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/
-08-chatgpt.html) ## Quick Start - Install EVA using the pip package manager.
-EVA supports Python versions >= 3.8: ```shell pip install evadb ``` - To launch
-and connect to an EVA server in a Jupyter notebook, check out this
-[illustrative emotion analysis notebook](https://github.com/georgia-tech-db/
-eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
-connect_to_server() ``` - Load a video onto the EVA server (we use
+Applications Here are some illustrative EvaDB-powered applications (each
+Jupyter notebook can be opened on Google Colab): * ð® Reddit_Image_Similarity
+Search * ð® ChatGPT-based_video_question_answering * ð® Quering_PDF
+documents * ð® Analysing_traffic_flow_with_YOLO * ð® Examining_emotion
+palette_of_a_movie * ð® Image_segmentation_with_Hugging_Face * ð®
+Recognizing_license_plates * ð® Analysing_toxicity_of_social_media_memes ##
+Documentation * [Detailed Documentation](https://evadb.readthedocs.io/) - The
+Getting_Started page shows how you can use EvaDB for different AI tasks and how
+you can easily extend EvaDB to support your custom deep learning model through
+user-defined functions. - The User_Guides section contains Jupyter Notebooks
+that demonstrate how to use various features of EvaDB. Each notebook includes a
+link to Google Colab, where you can run the code yourself. * [Tutorials](https:
+//github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb) * [Join us on Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter]
+(https://twitter.com/evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/
+georgia-tech-db/projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/
+source/tutorials/08-chatgpt.html) ## Quick Start - Install EvaDB using the pip
+package manager. EvaDB supports Python versions >= 3.8: ```shell pip install
+evadb ``` - To launch and connect to an EvaDB server in a Jupyter notebook,
+check out this [illustrative emotion analysis notebook](https://github.com/
+georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell
+cursor = connect_to_server() ``` - Load a video onto the EvaDB server (we use
 [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
 VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You
 can now run queries over the loaded video: ```mysql SELECT id, data FROM
 TrafficVideo WHERE id < 5; ``` - Search for frames in the video that contain a
 car: ```mysql SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo
 (data).labels; ``` | Source Video | Query Result | |---------------|-----------
 ---| |[Source Video] |[Query Result] | - Search for frames in the video that
@@ -74,65 +73,68 @@
 more than three cars: ```mysql SELECT id, data FROM TrafficVideo WHERE
 ArrayCount(Yolo(data).labels, 'car') > 3; ``` - **Use your custom deep learning
 model in queries** with a user-defined function (UDF): ```mysql CREATE UDF IF
 NOT EXISTS Yolo TYPE ultralytics 'model' 'yolov8m.pt'; ``` - **Chain multiple
 models in a single query** to set up useful AI pipelines. ```mysql -- Analyse
 emotions of faces in a video SELECT id, bbox, EmotionDetector(Crop(data, bbox))
 FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)
-WHERE id < 15; ``` - **EVA runs queries faster using its AI-centric query
-optimizer**. Two key optimizations are: ð¾ **Caching**: EVA automatically
+WHERE id < 15; ``` - **EvaDB runs queries faster using its AI-centric query
+optimizer**. Two key optimizations are: ð¾ **Caching**: EvaDB automatically
 caches and reuses previous query results (especially model inference results),
 eliminating redundant computation and reducing query processing time. ð¯
-**Predicate Reordering**: EVA optimizes the order in which the query predicates
-are evaluated (e.g., runs the faster, more selective model first), leading to
-faster queries and lower inference costs. Consider these two exploratory
-queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
-blob/master/data/assets/eva_performance_comparison.png?raw=true]
+**Predicate Reordering**: EvaDB optimizes the order in which the query
+predicates are evaluated (e.g., runs the faster, more selective model first),
+leading to faster queries and lower inference costs. Consider these two
+exploratory queries on a dataset of dog images: [https://github.com/georgia-
+tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
-predicates based on the available cached inference results, EVA runs the second
-query **10x faster**! ## Architecture Diagram This diagram presents the key
-components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as
-input and generates a query plan that is then executed by the Query Engine. The
-Query Engine hits multiple storage engines to retrieve the data required for
-efficiently running the query: 1. Structured data (SQL database system
-connected via `sqlalchemy`). 2. Unstructured media data (on cloud buckets or
-local filesystem). 3. Vector data (vector database system). [Architecture
-Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
+predicates based on the available cached inference results, EvaDB runs the
+second query **10x faster**! ## Architecture Diagram This diagram presents the
+key components of EvaDB. EvaDB's AI-centric Query Optimizer takes a parsed
+query as input and generates a query plan that is then executed by the Query
+Engine. The Query Engine hits multiple storage engines to retrieve the data
+required for efficiently running the query: 1. Structured data (SQL database
+system connected via `sqlalchemy`). 2. Unstructured media data (on cloud
+buckets or local filesystem). 3. Vector data (vector database system).
+[Architecture Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
-Classification Model) | Source Video | Query Result | |---------------|--------
-------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
-analysis.html) (Face Detection + Emotion Classification Models) | Source Video
-| Query Result | |---------------|--------------| |[Source Video] |[Query
-Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
-db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ## Community and Support ð If you
-have general questions about EVA, want to say hello or just follow along, we'd
-like to invite you to join our [Slack Community](https://join.slack.com/t/eva-
-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on
-Twitter](https://twitter.com/evadb_ai). [EVA_Slack_Channel] If you run into any
-problems or issues, please create a Github issue and we'll try our best to
-help. Don't see a feature in the list? Search our issue tracker if someone has
-already requested it and add a comment to it explaining your use-case, or open
-a new issue if not. We prioritize our [roadmap](https://github.com/orgs/
-georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from
-you. ## Contributing [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)]
-(https://pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-
-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
-[Documentation Status](https://readthedocs.org/projects/evadb/badge/
-?version=latest)](https://evadb.readthedocs.io/en/latest/index.html) EVA is the
-beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
-graphs/contributors). All kinds of contributions to EVA are appreciated. To
-file a bug or to request a feature, please use GitHub_issues. Pull_requests are
-welcome. For more information, see our [contribution guide](https://
-evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
+---------| |[Source Video] |[Query Result] | ### ð® [PDF Question Answering]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html)
+(Question Answering Model) | App | |-----| |[Source Video] | ### ð® [MNIST
+Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
+mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
+----------|--------------| |[Source Video] |[Query Result] | ### ð® [Movie
+Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-
+emotion-analysis.html) (Face Detection + Emotion Classification Models) |
+Source Video | Query Result | |---------------|--------------| |[Source Video]
+|[Query Result] | ### ð® [License Plate Recognition](https://github.com/
+georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction
+Models) | Query Result | |--------------| [Query Result] | ## Community and
+Support ð If you have general questions about EvaDB, want to say hello or
+just follow along, we'd like to invite you to join our [Slack Community](https:
+//join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+and to [follow us on Twitter](https://twitter.com/evadb_ai). [EvaDB_Slack
+Channel] If you run into any problems or issues, please create a Github issue
+and we'll try our best to help. Don't see a feature in the list? Search our
+issue tracker if someone has already requested it and add a comment to it
+explaining your use-case, or open a new issue if not. We prioritize our
+[roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user
+feedback, so we'd love to hear from you. ## Contributing [![PyPI Version]
+(https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [!
+[CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https:/
+/circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
+readthedocs.org/projects/evadb/badge/?version=latest)](https://
+evadb.readthedocs.io/en/latest/index.html) EvaDB is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EvaDB are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE).
```

### Comparing `evadb-0.2.7/README.md` & `evadb-0.2.8/evadb.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,31 @@
-# EVA AI-SQL Database System
+Metadata-Version: 2.1
+Name: evadb
+Version: 0.2.8
+Summary: EvaDB AI-Relational Database System
+Home-page: https://github.com/georgia-tech-db/eva
+Download-URL: https://github.com/georgia-tech-db/eva
+Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu
+License: Apache License 2.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# EvaDB AI-SQL Database System
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EvaDB on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
         </a>          
         <a href="https://twitter.com/evadb_ai">
             <img alt="Twitter" src="https://img.shields.io/badge/twitter-eva-bde1ee.svg?logo=twitter">
         </a>  
@@ -18,21 +37,21 @@
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
         </a>
         <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
 </div>
 
-<p align="center"> <b><h3>EVA DB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+<p align="center"> <b><h3>EvaDB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
-EVA DB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (videos, text, podcasts, PDFs, etc.).
+EvaDB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (text documents, videos, PDFs, podcasts, etc.).
 
-EVA DB accelerates AI pipelines by 10-100x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
+EvaDB accelerates AI pipelines by 10x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EvaDB supports an AI-oriented query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
 
-The high-level SQL API allows even beginners to use EVA in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EVA DB is fully implemented in Python and licensed under the Apache license.
+The high-level Python and SQL APIs allows even beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under the Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
@@ -42,60 +61,60 @@
 - [Community and Support](#community-and-support)
 - [Twitter](https://twitter.com/evadb_ai)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
 
-- 🔮 Build simpler AI-powered applications using short SQL-like queries
-- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
+- 🔮 Build simpler AI-powered applications using short Python or SQL queries
+- ⚡️ 10x faster applications using AI-centric query optimization  
 - 💰 Save money spent on GPUs
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
 - ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Illustrative Applications
 
-Here are some illustrative EVA-powered applications (each Jupyter notebook can be opened on Google Colab):
+Here are some illustrative EvaDB-powered applications (each Jupyter notebook can be opened on Google Colab):
 
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
- * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Reddit Image Similarity Search</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">ChatGPT-based video question answering</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html">Quering PDF documents</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow with YOLO</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining emotion palette of a movie</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image segmentation with Hugging Face</a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates</a>
  * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
 
 ## Documentation
 
 * [Detailed Documentation](https://evadb.readthedocs.io/)
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI tasks and how you can easily extend EVA to support your custom deep learning model through user-defined functions.
-  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code yourself.
+  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EvaDB for different AI tasks and how you can easily extend EvaDB to support your custom deep learning model through user-defined functions.
+  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EvaDB. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 * [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html)
 
 ## Quick Start
 
-- Install EVA using the pip package manager. EVA supports Python versions >= 3.8:
+- Install EvaDB using the pip package manager. EvaDB supports Python versions >= 3.8:
 
 ```shell
 pip install evadb
 ```
 
-- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+- To launch and connect to an EvaDB server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
 ```shell
 cursor = connect_to_server()
 ```
 
-- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+- Load a video onto the EvaDB server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
 
 ```mysql
 LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
 ```
 
 - That's it! You can now run queries over the loaded video:
 
@@ -137,19 +156,19 @@
 ```mysql
    -- Analyse emotions of faces in a video
    SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
    FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
    WHERE id < 15;
 ```
 
-- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
+- **EvaDB runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
 
-   💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+   💾 **Caching**: EvaDB automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
 
-   🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+   🎯 **Predicate Reordering**: EvaDB optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
 
 Consider these two exploratory queries on a dataset of dog images:
 <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
 
 ```mysql
   -- Query 1: Find all images of black-colored dogs
   SELECT id, bbox FROM dogs 
@@ -161,32 +180,38 @@
   SELECT id, bbox FROM dogs 
   JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
   WHERE Obj.label = 'dog' 
     AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
     AND Color(Crop(data, bbox)) = 'black';
 ```
 
-By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+By reusing the results of the first query and reordering the predicates based on the available cached inference results, EvaDB runs the second query **10x faster**!
 
 ## Architecture Diagram
 
-This diagram presents the key components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+This diagram presents the key components of EvaDB. EvaDB's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
 1. Structured data (SQL database system connected via `sqlalchemy`).
 2. Unstructured media data (on cloud buckets or local filesystem).
 3. Vector data (vector database system).
 
 <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
 ## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
+### 🔮 [PDF Question Answering](https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html) (Question Answering Model)
+
+| App |
+|-----|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/pdf-qa.webp" width="400"> |
+
 ### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
 
 ### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
 
@@ -198,31 +223,31 @@
 
 | Query Result |
 |--------------|
 <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
 
 ## Community and Support
 
-👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on Twitter](https://twitter.com/evadb_ai).
+👋 If you have general questions about EvaDB, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) and to [follow us on Twitter](https://twitter.com/evadb_ai).
 
 <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EvaDB Slack Channel" width="500">
 </a>
 
 If you run into any problems or issues, please create a Github issue and we'll try our best to help.
 
 Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our [roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from you.
 
 ## Contributing
 
 [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
 [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
 [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=latest)](https://evadb.readthedocs.io/en/latest/index.html)
 
-EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+EvaDB is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EvaDB are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
 Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,62 +1,70 @@
-# EVA AI-SQL Database System
-[Open_EVA_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
+Metadata-Version: 2.1 Name: evadb Version: 0.2.8 Summary: EvaDB AI-Relational
+Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
+https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
+Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
+Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
+:: Apache Software License Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
+text/markdown Provides-Extra: dev License-File: LICENSE.txt # EvaDB AI-SQL
+Database System
+[Open_EvaDB_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
 Status] [Downloads] [Python Versions]
-**** EVA DB is a database system for building simpler and faster AI-powered
+**** EvaDB is a database system for building simpler and faster AI-powered
 applications. ****
-EVA DB is an AI-SQL database system for developing applications powered by AI
+EvaDB is an AI-SQL database system for developing applications powered by AI
 models. We aim to simplify the development and deployment of AI-powered
 applications that operate on structured (tables, feature stores) and
-unstructured data (videos, text, podcasts, PDFs, etc.). EVA DB accelerates AI
-pipelines by 10-100x using a collection of performance optimizations inspired
-by time-tested SQL database systems, including data-parallel query execution,
-function caching, sampling, and cost-based predicate reordering. EVA supports
-an AI-oriented SQL-like query language tailored for analyzing both structured
-and unstructured data. It has first-class support for PyTorch, Hugging Face,
-YOLO, and Open AI models. The high-level SQL API allows even beginners to use
-EVA in a few lines of code. Advanced users can define custom user-defined
-functions that wrap around any AI model or Python library. EVA DB is fully
-implemented in Python and licensed under the Apache license. ## Quick Links -
-[Features](#features) - [Quick Start](#quick-start) - [Documentation]
-(#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Architecture Diagram](#architecture-diagram) - [Illustrative
-Applications](#illustrative-applications) - [Screenshots](#screenshots) -
-[Community and Support](#community-and-support) - [Twitter](https://
-twitter.com/evadb_ai) - [Contributing](#contributing) - [License](#license) ##
-Features - ð® Build simpler AI-powered applications using short SQL-like
-queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+unstructured data (text documents, videos, PDFs, podcasts, etc.). EvaDB
+accelerates AI pipelines by 10x using a collection of performance optimizations
+inspired by time-tested SQL database systems, including data-parallel query
+execution, function caching, sampling, and cost-based predicate reordering.
+EvaDB supports an AI-oriented query language tailored for analyzing both
+structured and unstructured data. It has first-class support for PyTorch,
+Hugging Face, YOLO, and Open AI models. The high-level Python and SQL APIs
+allows even beginners to use EvaDB in a few lines of code. Advanced users can
+define custom user-defined functions that wrap around any AI model or Python
+library. EvaDB is fully implemented in Python and licensed under the Apache
+license. ## Quick Links - [Features](#features) - [Quick Start](#quick-start) -
+[Documentation](#documentation) - [Roadmap](https://github.com/orgs/georgia-
+tech-db/projects/3) - [Architecture Diagram](#architecture-diagram) -
+[Illustrative Applications](#illustrative-applications) - [Screenshots]
+(#screenshots) - [Community and Support](#community-and-support) - [Twitter]
+(https://twitter.com/evadb_ai) - [Contributing](#contributing) - [License]
+(#license) ## Features - ð® Build simpler AI-powered applications using short
+Python or SQL queries - â¡ï¸ 10x faster applications using AI-centric query
 optimization - ð° Save money spent on GPUs - ð First-class support for
 your custom deep learning models through user-defined functions - ð¦ Built-in
 caching to eliminate redundant model invocations across queries - â¨ï¸ First-
 class support for PyTorch, Hugging Face, YOLO, and Open AI models - ð
 Installable via pip and fully implemented in Python ## Illustrative
-Applications Here are some illustrative EVA-powered applications (each Jupyter
-notebook can be opened on Google Colab): * ð® Using_ChatGPT_to_ask_questions
-based_on_videos * ð® Analysing_traffic_flow_at_an_intersection * ð®
-Examining_the_emotion_palette_of_actors_in_a_movie * ð® Image_Similarity
-Search_on_Reddit_[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their
-content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
-plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
-[Detailed Documentation](https://evadb.readthedocs.io/) - The Getting_Started
-page shows how you can use EVA for different AI tasks and how you can easily
-extend EVA to support your custom deep learning model through user-defined
-functions. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EVA. Each notebook includes a link
-to Google Colab, where you can run the code yourself. * [Tutorials](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/
-evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/
-projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/
-08-chatgpt.html) ## Quick Start - Install EVA using the pip package manager.
-EVA supports Python versions >= 3.8: ```shell pip install evadb ``` - To launch
-and connect to an EVA server in a Jupyter notebook, check out this
-[illustrative emotion analysis notebook](https://github.com/georgia-tech-db/
-eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
-connect_to_server() ``` - Load a video onto the EVA server (we use
+Applications Here are some illustrative EvaDB-powered applications (each
+Jupyter notebook can be opened on Google Colab): * ð® Reddit_Image_Similarity
+Search * ð® ChatGPT-based_video_question_answering * ð® Quering_PDF
+documents * ð® Analysing_traffic_flow_with_YOLO * ð® Examining_emotion
+palette_of_a_movie * ð® Image_segmentation_with_Hugging_Face * ð®
+Recognizing_license_plates * ð® Analysing_toxicity_of_social_media_memes ##
+Documentation * [Detailed Documentation](https://evadb.readthedocs.io/) - The
+Getting_Started page shows how you can use EvaDB for different AI tasks and how
+you can easily extend EvaDB to support your custom deep learning model through
+user-defined functions. - The User_Guides section contains Jupyter Notebooks
+that demonstrate how to use various features of EvaDB. Each notebook includes a
+link to Google Colab, where you can run the code yourself. * [Tutorials](https:
+//github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb) * [Join us on Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter]
+(https://twitter.com/evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/
+georgia-tech-db/projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/
+source/tutorials/08-chatgpt.html) ## Quick Start - Install EvaDB using the pip
+package manager. EvaDB supports Python versions >= 3.8: ```shell pip install
+evadb ``` - To launch and connect to an EvaDB server in a Jupyter notebook,
+check out this [illustrative emotion analysis notebook](https://github.com/
+georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell
+cursor = connect_to_server() ``` - Load a video onto the EvaDB server (we use
 [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
 VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You
 can now run queries over the loaded video: ```mysql SELECT id, data FROM
 TrafficVideo WHERE id < 5; ``` - Search for frames in the video that contain a
 car: ```mysql SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo
 (data).labels; ``` | Source Video | Query Result | |---------------|-----------
 ---| |[Source Video] |[Query Result] | - Search for frames in the video that
@@ -65,65 +73,68 @@
 more than three cars: ```mysql SELECT id, data FROM TrafficVideo WHERE
 ArrayCount(Yolo(data).labels, 'car') > 3; ``` - **Use your custom deep learning
 model in queries** with a user-defined function (UDF): ```mysql CREATE UDF IF
 NOT EXISTS Yolo TYPE ultralytics 'model' 'yolov8m.pt'; ``` - **Chain multiple
 models in a single query** to set up useful AI pipelines. ```mysql -- Analyse
 emotions of faces in a video SELECT id, bbox, EmotionDetector(Crop(data, bbox))
 FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)
-WHERE id < 15; ``` - **EVA runs queries faster using its AI-centric query
-optimizer**. Two key optimizations are: ð¾ **Caching**: EVA automatically
+WHERE id < 15; ``` - **EvaDB runs queries faster using its AI-centric query
+optimizer**. Two key optimizations are: ð¾ **Caching**: EvaDB automatically
 caches and reuses previous query results (especially model inference results),
 eliminating redundant computation and reducing query processing time. ð¯
-**Predicate Reordering**: EVA optimizes the order in which the query predicates
-are evaluated (e.g., runs the faster, more selective model first), leading to
-faster queries and lower inference costs. Consider these two exploratory
-queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
-blob/master/data/assets/eva_performance_comparison.png?raw=true]
+**Predicate Reordering**: EvaDB optimizes the order in which the query
+predicates are evaluated (e.g., runs the faster, more selective model first),
+leading to faster queries and lower inference costs. Consider these two
+exploratory queries on a dataset of dog images: [https://github.com/georgia-
+tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
-predicates based on the available cached inference results, EVA runs the second
-query **10x faster**! ## Architecture Diagram This diagram presents the key
-components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as
-input and generates a query plan that is then executed by the Query Engine. The
-Query Engine hits multiple storage engines to retrieve the data required for
-efficiently running the query: 1. Structured data (SQL database system
-connected via `sqlalchemy`). 2. Unstructured media data (on cloud buckets or
-local filesystem). 3. Vector data (vector database system). [Architecture
-Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
+predicates based on the available cached inference results, EvaDB runs the
+second query **10x faster**! ## Architecture Diagram This diagram presents the
+key components of EvaDB. EvaDB's AI-centric Query Optimizer takes a parsed
+query as input and generates a query plan that is then executed by the Query
+Engine. The Query Engine hits multiple storage engines to retrieve the data
+required for efficiently running the query: 1. Structured data (SQL database
+system connected via `sqlalchemy`). 2. Unstructured media data (on cloud
+buckets or local filesystem). 3. Vector data (vector database system).
+[Architecture Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
-Classification Model) | Source Video | Query Result | |---------------|--------
-------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
-analysis.html) (Face Detection + Emotion Classification Models) | Source Video
-| Query Result | |---------------|--------------| |[Source Video] |[Query
-Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
-db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ## Community and Support ð If you
-have general questions about EVA, want to say hello or just follow along, we'd
-like to invite you to join our [Slack Community](https://join.slack.com/t/eva-
-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on
-Twitter](https://twitter.com/evadb_ai). [EVA_Slack_Channel] If you run into any
-problems or issues, please create a Github issue and we'll try our best to
-help. Don't see a feature in the list? Search our issue tracker if someone has
-already requested it and add a comment to it explaining your use-case, or open
-a new issue if not. We prioritize our [roadmap](https://github.com/orgs/
-georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from
-you. ## Contributing [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)]
-(https://pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-
-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
-[Documentation Status](https://readthedocs.org/projects/evadb/badge/
-?version=latest)](https://evadb.readthedocs.io/en/latest/index.html) EVA is the
-beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
-graphs/contributors). All kinds of contributions to EVA are appreciated. To
-file a bug or to request a feature, please use GitHub_issues. Pull_requests are
-welcome. For more information, see our [contribution guide](https://
-evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
+---------| |[Source Video] |[Query Result] | ### ð® [PDF Question Answering]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html)
+(Question Answering Model) | App | |-----| |[Source Video] | ### ð® [MNIST
+Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
+mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
+----------|--------------| |[Source Video] |[Query Result] | ### ð® [Movie
+Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-
+emotion-analysis.html) (Face Detection + Emotion Classification Models) |
+Source Video | Query Result | |---------------|--------------| |[Source Video]
+|[Query Result] | ### ð® [License Plate Recognition](https://github.com/
+georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction
+Models) | Query Result | |--------------| [Query Result] | ## Community and
+Support ð If you have general questions about EvaDB, want to say hello or
+just follow along, we'd like to invite you to join our [Slack Community](https:
+//join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+and to [follow us on Twitter](https://twitter.com/evadb_ai). [EvaDB_Slack
+Channel] If you run into any problems or issues, please create a Github issue
+and we'll try our best to help. Don't see a feature in the list? Search our
+issue tracker if someone has already requested it and add a comment to it
+explaining your use-case, or open a new issue if not. We prioritize our
+[roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user
+feedback, so we'd love to hear from you. ## Contributing [![PyPI Version]
+(https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [!
+[CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https:/
+/circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
+readthedocs.org/projects/evadb/badge/?version=latest)](https://
+evadb.readthedocs.io/en/latest/index.html) EvaDB is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EvaDB are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE).
```

### Comparing `evadb-0.2.7/evadb/__init__.py` & `evadb-0.2.8/evadb/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from evadb.interfaces.relational.db import (  # noqa: E402,F401
-    EVADBConnection,
-    EVADBCursor,
+    EvaDBConnection,
+    EvaDBCursor,
     connect,
 )
-from evadb.interfaces.relational.relation import EVADBQuery  # noqa: E402,F401
+from evadb.interfaces.relational.relation import EvaDBQuery  # noqa: E402,F401
 
 from .version import VERSION as __version__  # noqa: E402,F401
 
 PYTHON_APIS = ["connect"]
 
 __all__ = list(PYTHON_APIS)
```

### Comparing `evadb-0.2.7/evadb/binder/__init__.py` & `evadb-0.2.8/evadb/binder/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/binder/binder_utils.py` & `evadb-0.2.8/evadb/binder/binder_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/binder/statement_binder.py` & `evadb-0.2.8/evadb/binder/statement_binder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,15 @@
     extend_star,
     handle_bind_extract_object_function,
     resolve_alias_table_value_expression,
 )
 from evadb.binder.statement_binder_context import StatementBinderContext
 from evadb.catalog.catalog_type import NdArrayType, TableType, VideoColumnName
 from evadb.catalog.catalog_utils import get_metadata_properties
-from evadb.configuration.constants import EVA_INSTALLATION_DIR
+from evadb.configuration.constants import EvaDB_INSTALLATION_DIR
 from evadb.expression.abstract_expression import AbstractExpression, ExpressionType
 from evadb.expression.function_expression import FunctionExpression
 from evadb.expression.tuple_value_expression import TupleValueExpression
 from evadb.parser.create_index_statement import CreateIndexStatement
 from evadb.parser.create_mat_view_statement import CreateMaterializedViewStatement
 from evadb.parser.create_statement import ColumnDefinition, CreateTableStatement
 from evadb.parser.delete_statement import DeleteTableStatement
@@ -306,15 +306,15 @@
         if udf_obj.type == "HuggingFace":
             node.function = assign_hf_udf(udf_obj)
 
         else:
             if udf_obj.type == "ultralytics":
                 # manually set the impl_path for yolo udfs we only handle object
                 # detection for now, hopefully this can be generalized
-                udf_dir = Path(EVA_INSTALLATION_DIR) / "udfs"
+                udf_dir = Path(EvaDB_INSTALLATION_DIR) / "udfs"
                 udf_obj.impl_file_path = (
                     Path(f"{udf_dir}/yolo_object_detector.py").absolute().as_posix()
                 )
 
             # Verify the consistency of the UDF. If the checksum of the UDF does not
             # match the one stored in the catalog, an error will be thrown and the user
             # will be asked to register the UDF again.
```

### Comparing `evadb-0.2.7/evadb/binder/statement_binder_context.py` & `evadb-0.2.8/evadb/binder/statement_binder_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/__init__.py` & `evadb-0.2.8/evadb/expression/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-catalog subdirectory
-"""
+"""expression subdirectory"""
```

### Comparing `evadb-0.2.7/evadb/catalog/catalog_manager.py` & `evadb-0.2.8/evadb/catalog/catalog_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/catalog_type.py` & `evadb-0.2.8/evadb/catalog/catalog_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,51 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from evadb.utils.generic_utils import EVAEnum
+from evadb.utils.generic_utils import EvaDBEnum
 
 
-class Dimension(EVAEnum):
+class Dimension(EvaDBEnum):
     ANYDIM  # noqa: F821
 
 
-class TableType(EVAEnum):
+class TableType(EvaDBEnum):
     STRUCTURED_DATA  # noqa: F821
     VIDEO_DATA  # noqa: F821
     IMAGE_DATA  # noqa: F821
     DOCUMENT_DATA  # noqa: F821
     PDF_DATA  # noqa: F821
 
     # reserved for system generated tables
     # cannot be accessed/modified directly by user
     SYSTEM_STRUCTURED_DATA  # noqa: F821
 
 
-class ColumnType(EVAEnum):
+class ColumnType(EvaDBEnum):
     BOOLEAN  # noqa: F821
     INTEGER  # noqa: F821
     FLOAT  # noqa: F821
     TEXT  # noqa: F821
     NDARRAY  # noqa: F821
     ANY  # noqa: F821
 
 
-class NdArrayType(EVAEnum):
+class NdArrayType(EvaDBEnum):
     INT8  # noqa: F821
     UINT8  # noqa: F821
     INT16  # noqa: F821
     INT32  # noqa: F821
     INT64  # noqa: F821
     UNICODE  # noqa: F821
     BOOL  # noqa: F821
@@ -90,45 +90,45 @@
             np_type = np.dtype(object)
         else:
             raise ValueError("Can not auto convert %s to numpy type" % t)
 
         return np_type
 
 
-class VectorStoreType(EVAEnum):
+class VectorStoreType(EvaDBEnum):
     FAISS  # noqa: F821
     QDRANT  # noqa: F821
 
 
-class VideoColumnName(EVAEnum):
+class VideoColumnName(EvaDBEnum):
     name  # noqa: F821
     id  # noqa: F821
     data  # noqa: F821
     seconds  # noqa: F821
     audio  # noqa: F821
 
     def __eq__(self, other):
         if isinstance(other, str):
             return self.name == other
 
-        if isinstance(other, EVAEnum):
+        if isinstance(other, EvaDBEnum):
             return self.value == other.value
 
         return False
 
 
-class ImageColumnName(EVAEnum):
+class ImageColumnName(EvaDBEnum):
     name  # noqa: F821
     data  # noqa: F821
 
 
-class DocumentColumnName(EVAEnum):
+class DocumentColumnName(EvaDBEnum):
     name  # noqa: F821
     data  # noqa: F821
     metadata  # noqa: F821
 
 
-class PDFColumnName(EVAEnum):
+class PDFColumnName(EvaDBEnum):
     name  # noqa: F821
     page  # noqa: F821
     paragraph  # noqa: F821
     data  # noqa: F821
```

### Comparing `evadb-0.2.7/evadb/catalog/catalog_utils.py` & `evadb-0.2.8/evadb/catalog/catalog_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/__init__.py` & `evadb-0.2.8/evadb/catalog/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/association_models.py` & `evadb-0.2.8/evadb/catalog/models/association_models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/base_model.py` & `evadb-0.2.8/evadb/catalog/models/base_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/column_catalog.py` & `evadb-0.2.8/evadb/catalog/models/column_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/index_catalog.py` & `evadb-0.2.8/evadb/catalog/models/index_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/table_catalog.py` & `evadb-0.2.8/evadb/catalog/models/table_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/udf_cache_catalog.py` & `evadb-0.2.8/evadb/catalog/models/udf_cache_catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/udf_catalog.py` & `evadb-0.2.8/evadb/catalog/models/udf_catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/udf_cost_catalog.py` & `evadb-0.2.8/evadb/catalog/models/udf_cost_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/udf_io_catalog.py` & `evadb-0.2.8/evadb/catalog/models/udf_io_catalog.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/udf_metadata_catalog.py` & `evadb-0.2.8/evadb/catalog/models/udf_metadata_catalog.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/models/utils.py` & `evadb-0.2.8/evadb/catalog/models/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -67,15 +67,15 @@
                 if table.name not in CATALOG_TABLES:
                     if insp.has_table(table.name):
                         table.drop(con)
             trans.commit()
 
 
 #####
-# Dataclass equivalents of catalog entires
+# Dataclass equivalents of catalog entries
 # This is done to ensure we don't expose the sqlalchemy dependencies beyond catalog
 # service. Further, sqlalchemy does not allow sharing of objects across threads.
 
 
 @dataclass(unsafe_hash=True)
 class UdfCacheCatalogEntry:
     """Dataclass representing an entry in the `UdfCatalog`."""
```

### Comparing `evadb-0.2.7/evadb/catalog/schema_utils.py` & `evadb-0.2.8/evadb/catalog/schema_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/__init__.py` & `evadb-0.2.8/evadb/catalog/services/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/base_service.py` & `evadb-0.2.8/evadb/catalog/services/base_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/column_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/column_catalog_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/index_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/index_catalog_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/table_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/table_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/udf_cache_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/udf_cache_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/udf_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/udf_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/udf_cost_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/udf_cost_catalog_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/udf_io_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/udf_io_catalog_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/services/udf_metadata_catalog_service.py` & `evadb-0.2.8/evadb/catalog/services/udf_metadata_catalog_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/catalog/sql_config.py` & `evadb-0.2.8/evadb/catalog/sql_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/configuration/__init__.py` & `evadb-0.2.8/evadb/configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/configuration/bootstrap_environment.py` & `evadb-0.2.8/evadb/configuration/bootstrap_environment.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -18,87 +18,86 @@
 from typing import Union
 
 import yaml
 
 from evadb.configuration.constants import (
     CACHE_DIR,
     DB_DEFAULT_NAME,
-    EVA_CONFIG_FILE,
-    EVA_DATASET_DIR,
     INDEX_DIR,
     S3_DOWNLOAD_DIR,
     TMP_DIR,
     UDF_DIR,
+    EvaDB_CONFIG_FILE,
+    EvaDB_DATASET_DIR,
 )
-from evadb.utils.logging_manager import logger as eva_logger
+from evadb.utils.logging_manager import logger as evadb_logger
 
 
-def get_base_config(eva_installation_dir: Path) -> Path:
+def get_base_config(evadb_installation_dir: Path) -> Path:
     """
     Get path to .evadb.yml source path.
-    This file will be copied to user's .eva directory.
     """
-    # if eva package is installed into environment
-    if importlib_resources.is_resource("evadb", EVA_CONFIG_FILE):
-        with importlib_resources.path("evadb", EVA_CONFIG_FILE) as yml_path:
+    # if evadb package is installed in environment
+    if importlib_resources.is_resource("evadb", EvaDB_CONFIG_FILE):
+        with importlib_resources.path("evadb", EvaDB_CONFIG_FILE) as yml_path:
             return yml_path
     else:
         # For local dev environments without package installed
-        return eva_installation_dir / EVA_CONFIG_FILE
+        return evadb_installation_dir / EvaDB_CONFIG_FILE
 
 
-def get_default_db_uri(eva_db_dir: Path):
-    return f"sqlite:///{eva_db_dir.resolve()}/{DB_DEFAULT_NAME}"
+def get_default_db_uri(evadb_dir: Path):
+    return f"sqlite:///{evadb_dir.resolve()}/{DB_DEFAULT_NAME}"
 
 
-def bootstrap_environment(eva_db_dir: Path, eva_installation_dir: Path):
+def bootstrap_environment(evadb_dir: Path, evadb_installation_dir: Path):
     """
-    Populates necessary configuration for EVA to be able to run.
+    Populates necessary configuration for EvaDB to be able to run.
 
     Arguments:
-        eva_db_dir: path to eva database directory
-        eva_installation_dir: path to eva module
+        evadb_dir: path to evadb database directory
+        evadb_installation_dir: path to evadb package
     """
 
-    default_config_path = get_base_config(eva_installation_dir).resolve()
+    default_config_path = get_base_config(evadb_installation_dir).resolve()
 
     # creates necessary directories
     config_default_dict = create_directories_and_get_default_config_values(
-        Path(eva_db_dir), Path(eva_installation_dir)
+        Path(evadb_dir), Path(evadb_installation_dir)
     )
 
-    assert eva_db_dir.exists(), f"{eva_db_dir} does not exist"
-    assert eva_installation_dir.exists(), f"{eva_installation_dir} does not exist"
+    assert evadb_dir.exists(), f"{evadb_dir} does not exist"
+    assert evadb_installation_dir.exists(), f"{evadb_installation_dir} does not exist"
     config_obj = {}
     with default_config_path.open("r") as yml_file:
         config_obj = yaml.load(yml_file, Loader=yaml.FullLoader)
     config_obj = merge_dict_of_dicts(config_obj, config_default_dict)
     mode = config_obj["core"]["mode"]
 
     # set logger to appropriate level (debug or release)
     level = logging.WARN if mode == "release" else logging.DEBUG
-    eva_logger.setLevel(level)
-    eva_logger.debug(f"Setting logging level to: {str(level)}")
+    evadb_logger.setLevel(level)
+    evadb_logger.debug(f"Setting logging level to: {str(level)}")
 
     return config_obj
 
 
 def create_directories_and_get_default_config_values(
-    eva_db_dir: Path, eva_installation_dir: Path, category: str = None, key: str = None
+    evadb_dir: Path, evadb_installation_dir: Path, category: str = None, key: str = None
 ) -> Union[dict, str]:
-    default_install_dir = eva_installation_dir
-    dataset_location = eva_db_dir / EVA_DATASET_DIR
-    index_dir = eva_db_dir / INDEX_DIR
-    cache_dir = eva_db_dir / CACHE_DIR
-    s3_dir = eva_db_dir / S3_DOWNLOAD_DIR
-    tmp_dir = eva_db_dir / TMP_DIR
-    udf_dir = eva_db_dir / UDF_DIR
+    default_install_dir = evadb_installation_dir
+    dataset_location = evadb_dir / EvaDB_DATASET_DIR
+    index_dir = evadb_dir / INDEX_DIR
+    cache_dir = evadb_dir / CACHE_DIR
+    s3_dir = evadb_dir / S3_DOWNLOAD_DIR
+    tmp_dir = evadb_dir / TMP_DIR
+    udf_dir = evadb_dir / UDF_DIR
 
-    if not eva_db_dir.exists():
-        eva_db_dir.mkdir(parents=True, exist_ok=True)
+    if not evadb_dir.exists():
+        evadb_dir.mkdir(parents=True, exist_ok=True)
     if not dataset_location.exists():
         dataset_location.mkdir(parents=True, exist_ok=True)
     if not index_dir.exists():
         index_dir.mkdir(parents=True, exist_ok=True)
     if not cache_dir.exists():
         cache_dir.mkdir(parents=True, exist_ok=True)
     if not s3_dir.exists():
@@ -107,17 +106,17 @@
         tmp_dir.mkdir(parents=True, exist_ok=True)
     if not udf_dir.exists():
         udf_dir.mkdir(parents=True, exist_ok=True)
 
     config_obj = {}
     config_obj["core"] = {}
     config_obj["storage"] = {}
-    config_obj["core"]["eva_installation_dir"] = str(default_install_dir.resolve())
+    config_obj["core"]["evadb_installation_dir"] = str(default_install_dir.resolve())
     config_obj["core"]["datasets_dir"] = str(dataset_location.resolve())
-    config_obj["core"]["catalog_database_uri"] = get_default_db_uri(eva_db_dir)
+    config_obj["core"]["catalog_database_uri"] = get_default_db_uri(evadb_dir)
     config_obj["storage"]["index_dir"] = str(index_dir.resolve())
     config_obj["storage"]["cache_dir"] = str(cache_dir.resolve())
     config_obj["storage"]["s3_download_dir"] = str(s3_dir.resolve())
     config_obj["storage"]["tmp_dir"] = str(tmp_dir.resolve())
     config_obj["storage"]["udf_dir"] = str(udf_dir.resolve())
     if category and key:
         return config_obj.get(category, {}).get(key, None)
```

### Comparing `evadb-0.2.7/evadb/configuration/configuration_manager.py` & `evadb-0.2.8/evadb/configuration/configuration_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,27 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import Any
 
 from evadb.configuration.bootstrap_environment import bootstrap_environment
-from evadb.configuration.constants import EVA_DATABASE_DIR, EVA_INSTALLATION_DIR
+from evadb.configuration.constants import EvaDB_DATABASE_DIR, EvaDB_INSTALLATION_DIR
 from evadb.utils.logging_manager import logger
 
 
 class ConfigurationManager(object):
-    def __init__(self, eva_db_dir: str = None) -> None:
-        self._eva_db_dir = eva_db_dir or EVA_DATABASE_DIR
+    def __init__(self, evadb_dir: str = None) -> None:
+        self._evadb_dir = evadb_dir or EvaDB_DATABASE_DIR
         self._config_obj = self._create_if_not_exists()
 
     def _create_if_not_exists(self):
         config_obj = bootstrap_environment(
-            eva_db_dir=Path(self._eva_db_dir),
-            eva_installation_dir=Path(EVA_INSTALLATION_DIR),
+            evadb_dir=Path(self._evadb_dir),
+            evadb_installation_dir=Path(EvaDB_INSTALLATION_DIR),
         )
         return config_obj
 
     def _get(self, category: str, key: str) -> Any:
         """Retrieve a configuration value based on the category and key.
 
         Args:
```

### Comparing `evadb-0.2.7/evadb/configuration/constants.py` & `evadb-0.2.8/evadb/configuration/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,20 +12,20 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 
 import evadb
 
-EVA_INSTALLATION_DIR = Path(evadb.__file__).parent
-EVA_ROOT_DIR = Path(evadb.__file__).parent.parent
-EVA_DATABASE_DIR = "evadb_data"
-EVA_DATASET_DIR = "evadb_datasets"
-EVA_CONFIG_FILE = "evadb.yml"
+EvaDB_INSTALLATION_DIR = Path(evadb.__file__).parent
+EvaDB_ROOT_DIR = Path(evadb.__file__).parent.parent
+EvaDB_DATABASE_DIR = "evadb_data"
+EvaDB_DATASET_DIR = "evadb_datasets"
+EvaDB_CONFIG_FILE = "evadb.yml"
 UDF_DIR = "udfs"
 CATALOG_DIR = "catalog"
 INDEX_DIR = "index"
 CACHE_DIR = "cache"
 DATASET_DATAFRAME_NAME = "dataset"
-DB_DEFAULT_NAME = "eva.db"
+DB_DEFAULT_NAME = "evadb.db"
 S3_DOWNLOAD_DIR = "s3_downloads"
 TMP_DIR = "tmp"
```

### Comparing `evadb-0.2.7/evadb/constants.py` & `evadb-0.2.8/evadb/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/database.py` & `evadb-0.2.8/evadb/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,41 +14,41 @@
 # limitations under the License.
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TYPE_CHECKING, Callable
 
 from evadb.catalog.catalog_utils import get_catalog_instance
 from evadb.configuration.configuration_manager import ConfigurationManager
-from evadb.configuration.constants import DB_DEFAULT_NAME, EVA_DATABASE_DIR
+from evadb.configuration.constants import DB_DEFAULT_NAME, EvaDB_DATABASE_DIR
 
 if TYPE_CHECKING:
     from evadb.catalog.catalog_manager import CatalogManager
 
 
 @dataclass
-class EVADatabase:
+class EvaDBDatabase:
     db_uri: str
     config: ConfigurationManager
     catalog_uri: str
     catalog_func: Callable
 
     def catalog(self) -> "CatalogManager":
         """
         Note: Generating an object on demand plays a crucial role in ensuring that different threads do not share the same catalog object, as it can result in serialization issues and incorrect behavior with SQLAlchemy. Refer to get_catalog_instance()
         """
         return self.catalog_func(self.catalog_uri, self.config)
 
 
-def get_default_db_uri(eva_db_dir: Path):
-    return f"sqlite:///{eva_db_dir.resolve()}/{DB_DEFAULT_NAME}"
+def get_default_db_uri(evadb_dir: Path):
+    return f"sqlite:///{evadb_dir.resolve()}/{DB_DEFAULT_NAME}"
 
 
-def init_eva_db_instance(
+def init_evadb_instance(
     db_dir: str, host: str = None, port: int = None, custom_db_uri: str = None
 ):
     if db_dir is None:
-        db_dir = EVA_DATABASE_DIR
+        db_dir = EvaDB_DATABASE_DIR
     config = ConfigurationManager(db_dir)
 
     catalog_uri = custom_db_uri or get_default_db_uri(Path(db_dir))
 
-    return EVADatabase(db_dir, config, catalog_uri, get_catalog_instance)
+    return EvaDBDatabase(db_dir, config, catalog_uri, get_catalog_instance)
```

### Comparing `evadb-0.2.7/evadb/eva_cmd_client.py` & `evadb-0.2.8/evadb/evadb_cmd_client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,41 +16,41 @@
 import asyncio
 import sys
 from os.path import abspath, dirname, join
 
 from evadb.utils.logging_manager import logger
 
 """
-To allow running eva_server from any location
+To allow running evadb_server from any location
 """
 THIS_DIR = dirname(__file__)
-EVA_CODE_DIR = abspath(join(THIS_DIR, ".."))
-sys.path.append(EVA_CODE_DIR)
+EvaDB_CODE_DIR = abspath(join(THIS_DIR, ".."))
+sys.path.append(EvaDB_CODE_DIR)
 
 from evadb.configuration.configuration_manager import ConfigurationManager  # noqa: E402
 from evadb.server.interpreter import start_cmd_client  # noqa: E402
 
 
-async def eva_client(host: str, port: int):
+async def evadb_client(host: str, port: int):
     """
-    Start the eva client
+    Start the evadb client
     """
 
     # Launch client
     try:
         await start_cmd_client(host, port)
     except KeyboardInterrupt:
         pass
     except Exception as e:
         logger.critical(e)
         raise e
 
 
 def main():
-    parser = argparse.ArgumentParser(description="EVA Client")
+    parser = argparse.ArgumentParser(description="EvaDB Client")
 
     parser.add_argument(
         "--host",
         help="Specify the host address of the server you want to connect to.",
     )
 
     parser.add_argument(
@@ -64,12 +64,12 @@
     host = (
         args.host if args.host else ConfigurationManager().get_value("server", "host")
     )
 
     port = (
         args.port if args.port else ConfigurationManager().get_value("server", "port")
     )
-    asyncio.run(eva_client(host, port))
+    asyncio.run(evadb_client(host, port))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `evadb-0.2.7/evadb/eva_server.py` & `evadb-0.2.8/evadb/evadb_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,57 +17,57 @@
 import sys
 from os.path import abspath, dirname, join
 from signal import SIGTERM
 
 from psutil import process_iter
 
 """
-To allow running eva_server from any location
+To allow running evadb_server from any location
 """
 THIS_DIR = dirname(__file__)
-EVA_CODE_DIR = abspath(join(THIS_DIR, ".."))
-sys.path.append(EVA_CODE_DIR)
+EvaDB_CODE_DIR = abspath(join(THIS_DIR, ".."))
+sys.path.append(EvaDB_CODE_DIR)
 
 from evadb.server.server import EvaServer  # noqa: E402
 
 
-async def start_eva_server(
+async def start_evadb_server(
     db_dir: str, host: str, port: str, custom_db_uri: str = None
 ):
-    """Start the eva server"""
-    eva_server = EvaServer()
-    await eva_server.start_eva_server(db_dir, host, port, custom_db_uri)
+    """Start the evadb server"""
+    evadb_server = EvaServer()
+    await evadb_server.start_evadb_server(db_dir, host, port, custom_db_uri)
 
 
 def stop_server():
     """
-    Stop the eva server
+    Stop the evadb server
     """
     for proc in process_iter():
-        if proc.name() == "eva_server":
+        if proc.name() == "evadb_server":
             proc.send_signal(SIGTERM)
 
     return 0
 
 
 def main():
-    parser = argparse.ArgumentParser(description="EVA Server")
+    parser = argparse.ArgumentParser(description="EvaDB Server")
 
     parser.add_argument(
         "--host",
         help="Specify the host address on which the server will start.",
     )
 
     parser.add_argument(
         "--port",
         help="Specify the port number on which the server will start.",
     )
 
     parser.add_argument(
-        "--db_dir", help="Specify the eva directory which the server should access."
+        "--db_dir", help="Specify the evadb directory which the server should access."
     )
 
     parser.add_argument(
         "--sql_backend",
         help="Specify the custom sql database to use for structured data.",
     )
 
@@ -93,14 +93,14 @@
     # Stop server
     if args.stop:
         return stop_server()
 
     # Start server
     if args.start:
         asyncio.run(
-            start_eva_server(args.db_dir, args.host, args.port, args.sql_backend)
+            start_evadb_server(args.db_dir, args.host, args.port, args.sql_backend)
         )
 
 
 if __name__ == "__main__":
     # execute only if run as the entry point into the program
     main()
```

### Comparing `evadb-0.2.7/evadb/evadb.yml` & `evadb-0.2.8/evadb/evadb.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-00000000: 636f 7265 3a0a 2020 6576 615f 696e 7374  core:.  eva_inst
-00000010: 616c 6c61 7469 6f6e 5f64 6972 3a20 2222  allation_dir: ""
-00000020: 0a20 2064 6174 6173 6574 735f 6469 723a  .  datasets_dir:
-00000030: 2022 220a 2020 6361 7461 6c6f 675f 6461   "".  catalog_da
-00000040: 7461 6261 7365 5f75 7269 3a20 2222 0a20  tabase_uri: "". 
-00000050: 2061 7070 6c69 6361 7469 6f6e 3a20 2265   application: "e
-00000060: 7661 6462 220a 2020 6d6f 6465 3a20 2272  vadb".  mode: "r
-00000070: 656c 6561 7365 2220 2372 656c 6561 7365  elease" #release
-00000080: 206f 7220 6465 6275 670a 0a65 7865 6375   or debug..execu
-00000090: 746f 723a 0a20 2023 2062 6174 6368 5f6d  tor:.  # batch_m
-000000a0: 656d 5f73 697a 6520 636f 6e66 6967 7572  em_size configur
-000000b0: 6573 2074 6865 206e 756d 6265 7220 6f66  es the number of
-000000c0: 2072 6f77 7320 7072 6f63 6573 7365 6420   rows processed 
-000000d0: 6279 2074 6865 2065 7865 6375 7469 6f6e  by the execution
-000000e0: 2065 6e67 696e 6520 696e 206f 6e65 2069   engine in one i
-000000f0: 7465 7261 7469 6f6e 0a20 2023 2072 6f77  teration.  # row
-00000100: 7320 3d20 6d61 7828 312c 2072 6f77 5f6d  s = max(1, row_m
-00000110: 656d 5f73 697a 6520 2f20 6261 7463 685f  em_size / batch_
-00000120: 6d65 6d5f 7369 7a65 290a 2020 6261 7463  mem_size).  batc
-00000130: 685f 6d65 6d5f 7369 7a65 3a20 3330 3030  h_mem_size: 3000
-00000140: 3030 3030 0a0a 2020 2320 6261 7463 6820  0000..  # batch 
-00000150: 7369 7a65 2075 7365 6420 666f 7220 6770  size used for gp
-00000160: 755f 6f70 6572 6174 696f 6e73 0a20 2067  u_operations.  g
-00000170: 7075 5f62 6174 6368 5f73 697a 653a 2031  pu_batch_size: 1
-00000180: 0a0a 2020 6770 755f 6964 733a 205b 305d  ..  gpu_ids: [0]
-00000190: 0a0a 7374 6f72 6167 653a 0a20 2074 6d70  ..storage:.  tmp
-000001a0: 5f64 6972 3a20 2222 0a20 2073 335f 646f  _dir: "".  s3_do
-000001b0: 776e 6c6f 6164 5f64 6972 3a20 2222 0a0a  wnload_dir: ""..
-000001c0: 7365 7276 6572 3a0a 2020 686f 7374 3a20  server:.  host: 
-000001d0: 2230 2e30 2e30 2e30 220a 2020 706f 7274  "0.0.0.0".  port
-000001e0: 3a20 3838 3033 0a20 2073 6f63 6b65 745f  : 8803.  socket_
-000001f0: 7469 6d65 6f75 743a 2036 300a 0a65 7870  timeout: 60..exp
-00000200: 6572 696d 656e 7461 6c3a 0a20 2072 6179  erimental:.  ray
-00000210: 3a20 5472 7565 0a0a 7468 6972 645f 7061  : True..third_pa
-00000220: 7274 793a 0a20 204f 5045 4e41 495f 4b45  rty:.  OPENAI_KE
-00000230: 593a 2022 220a                           Y: "".
+00000000: 636f 7265 3a0a 2020 6576 6164 625f 696e  core:.  evadb_in
+00000010: 7374 616c 6c61 7469 6f6e 5f64 6972 3a20  stallation_dir: 
+00000020: 2222 0a20 2064 6174 6173 6574 735f 6469  "".  datasets_di
+00000030: 723a 2022 220a 2020 6361 7461 6c6f 675f  r: "".  catalog_
+00000040: 6461 7461 6261 7365 5f75 7269 3a20 2222  database_uri: ""
+00000050: 0a20 2061 7070 6c69 6361 7469 6f6e 3a20  .  application: 
+00000060: 2265 7661 6462 220a 2020 6d6f 6465 3a20  "evadb".  mode: 
+00000070: 2272 656c 6561 7365 2220 2372 656c 6561  "release" #relea
+00000080: 7365 206f 7220 6465 6275 670a 0a65 7865  se or debug..exe
+00000090: 6375 746f 723a 0a20 2023 2062 6174 6368  cutor:.  # batch
+000000a0: 5f6d 656d 5f73 697a 6520 636f 6e66 6967  _mem_size config
+000000b0: 7572 6573 2074 6865 206e 756d 6265 7220  ures the number 
+000000c0: 6f66 2072 6f77 7320 7072 6f63 6573 7365  of rows processe
+000000d0: 6420 6279 2074 6865 2065 7865 6375 7469  d by the executi
+000000e0: 6f6e 2065 6e67 696e 6520 696e 206f 6e65  on engine in one
+000000f0: 2069 7465 7261 7469 6f6e 0a20 2023 2072   iteration.  # r
+00000100: 6f77 7320 3d20 6d61 7828 312c 2072 6f77  ows = max(1, row
+00000110: 5f6d 656d 5f73 697a 6520 2f20 6261 7463  _mem_size / batc
+00000120: 685f 6d65 6d5f 7369 7a65 290a 2020 6261  h_mem_size).  ba
+00000130: 7463 685f 6d65 6d5f 7369 7a65 3a20 3330  tch_mem_size: 30
+00000140: 3030 3030 3030 0a0a 2020 2320 6261 7463  000000..  # batc
+00000150: 6820 7369 7a65 2075 7365 6420 666f 7220  h size used for 
+00000160: 6770 755f 6f70 6572 6174 696f 6e73 0a20  gpu_operations. 
+00000170: 2067 7075 5f62 6174 6368 5f73 697a 653a   gpu_batch_size:
+00000180: 2031 0a0a 2020 6770 755f 6964 733a 205b   1..  gpu_ids: [
+00000190: 305d 0a0a 7374 6f72 6167 653a 0a20 2074  0]..storage:.  t
+000001a0: 6d70 5f64 6972 3a20 2222 0a20 2073 335f  mp_dir: "".  s3_
+000001b0: 646f 776e 6c6f 6164 5f64 6972 3a20 2222  download_dir: ""
+000001c0: 0a0a 7365 7276 6572 3a0a 2020 686f 7374  ..server:.  host
+000001d0: 3a20 2230 2e30 2e30 2e30 220a 2020 706f  : "0.0.0.0".  po
+000001e0: 7274 3a20 3838 3033 0a20 2073 6f63 6b65  rt: 8803.  socke
+000001f0: 745f 7469 6d65 6f75 743a 2036 300a 0a65  t_timeout: 60..e
+00000200: 7870 6572 696d 656e 7461 6c3a 0a20 2072  xperimental:.  r
+00000210: 6179 3a20 5472 7565 0a0a 7468 6972 645f  ay: True..third_
+00000220: 7061 7274 793a 0a20 204f 5045 4e41 495f  party:.  OPENAI_
+00000230: 4b45 593a 2022 220a                      KEY: "".
```

### Comparing `evadb-0.2.7/evadb/executor/__init__.py` & `evadb-0.2.8/evadb/plan_nodes/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""executor subdirectory"""
+"""planner subdirectory"""
```

### Comparing `evadb-0.2.7/evadb/executor/abstract_executor.py` & `evadb-0.2.8/evadb/executor/abstract_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,29 +15,29 @@
 from abc import ABC, abstractmethod
 from collections import deque
 from typing import TYPE_CHECKING, Any, Generator, Iterable, List, TypeVar
 
 if TYPE_CHECKING:
     from evadb.catalog.catalog_manager import CatalogManager
 from evadb.configuration.configuration_manager import ConfigurationManager
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.abstract_plan import AbstractPlan
 
 AbstractExecutor = TypeVar("AbstractExecutor")
 
 
 class AbstractExecutor(ABC):
     """
     An abstract class for the executor engine
     Arguments:
         node (AbstractPlan): Plan node corresponding to this executor
     """
 
-    def __init__(self, db: EVADatabase, node: AbstractPlan):
+    def __init__(self, db: EvaDBDatabase, node: AbstractPlan):
         self._db = db
         self._node = node
         self._config: ConfigurationManager = db.config if db else None
         self._children = []
 
     def catalog(self) -> "CatalogManager":
         """The object is intentionally generated on demand to prevent serialization issues. Having a SQLAlchemy object as a member variable can cause problems with multiprocessing. See get_catalog_instance()"""
@@ -66,15 +66,15 @@
         self._children = children
 
     @property
     def node(self) -> AbstractPlan:
         return self._node
 
     @property
-    def db(self) -> EVADatabase:
+    def db(self) -> EvaDBDatabase:
         return self._db
 
     @property
     def config(self) -> ConfigurationManager:
         return self._config
 
     @abstractmethod
@@ -99,20 +99,20 @@
         queue = deque([self])
         while queue:
             node = queue.popleft()
             yield node
             for child in node.children:
                 queue.append(child)
 
-    def find_all(self, exceution_type: Any):
-        """Returns a generator which visits all the nodes in execution tree and yields one that matches the passed `exceution_type`.
+    def find_all(self, execution_type: Any):
+        """Returns a generator which visits all the nodes in execution tree and yields one that matches the passed `execution_type`.
 
         Args:
-            exceution_type (Any): execution type to match with
+            execution_type (Any): execution type to match with
 
         Returns:
             the generator object.
         """
 
         for node in self.bfs():
-            if isinstance(node, exceution_type):
+            if isinstance(node, execution_type):
                 yield node
```

### Comparing `evadb-0.2.7/evadb/executor/apply_and_merge_executor.py` & `evadb-0.2.8/evadb/executor/apply_and_merge_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.apply_and_merge_plan import ApplyAndMergePlan
 
 
 class ApplyAndMergeExecutor(AbstractExecutor):
     """
@@ -27,15 +27,15 @@
     assumes an inner join while merging. Therefore, if the function does not return any
     output, the input rows are dropped.
     Arguments:
         node (AbstractPlan): ApplyAndMergePlan
 
     """
 
-    def __init__(self, db: EVADatabase, node: ApplyAndMergePlan):
+    def __init__(self, db: EvaDBDatabase, node: ApplyAndMergePlan):
         super().__init__(db, node)
         self.func_expr = node.func_expr
         self.do_unnest = node.do_unnest
         self.alias = node.alias
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
```

### Comparing `evadb-0.2.7/evadb/executor/create_executor.py` & `evadb-0.2.8/evadb/executor/create_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import handle_if_not_exists
 from evadb.plan_nodes.create_plan import CreatePlan
 from evadb.storage.storage_engine import StorageEngine
 from evadb.utils.logging_manager import logger
 
 
 class CreateExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: CreatePlan):
+    def __init__(self, db: EvaDBDatabase, node: CreatePlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         if not handle_if_not_exists(
             self.catalog(), self.node.table_info, self.node.if_not_exists
         ):
             logger.debug(f"Creating table {self.node.table_info}")
```

### Comparing `evadb-0.2.7/evadb/executor/create_index_executor.py` & `evadb-0.2.8/evadb/executor/create_index_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,27 +13,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 
 import pandas as pd
 
 from evadb.catalog.sql_config import IDENTIFIER_COLUMN
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError, handle_vector_store_params
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.create_index_plan import CreateIndexPlan
 from evadb.storage.storage_engine import StorageEngine
 from evadb.third_party.vector_stores.types import FeaturePayload
 from evadb.third_party.vector_stores.utils import VectorStoreFactory
 from evadb.utils.logging_manager import logger
 
 
 class CreateIndexExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: CreateIndexPlan):
+    def __init__(self, db: EvaDBDatabase, node: CreateIndexPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         if self.catalog().get_index_catalog_entry_by_name(self.node.name):
             msg = f"Index {self.node.name} already exists."
             logger.error(msg)
             raise ExecutorError(msg)
```

### Comparing `evadb-0.2.7/evadb/executor/create_mat_view_executor.py` & `evadb-0.2.8/evadb/executor/create_mat_view_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import handle_if_not_exists
 from evadb.plan_nodes.create_mat_view_plan import CreateMaterializedViewPlan
 from evadb.storage.storage_engine import StorageEngine
 
 
 class CreateMaterializedViewExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: CreateMaterializedViewPlan):
+    def __init__(self, db: EvaDBDatabase, node: CreateMaterializedViewPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         """Create materialized view executor"""
         if not handle_if_not_exists(
             self.catalog(), self.node.view, self.node.if_not_exists
         ):
```

### Comparing `evadb-0.2.7/evadb/executor/create_udf_executor.py` & `evadb-0.2.8/evadb/executor/create_udf_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,30 +16,30 @@
 from typing import Dict, List
 
 import pandas as pd
 
 from evadb.catalog.catalog_utils import get_metadata_properties
 from evadb.catalog.models.udf_catalog import UdfCatalogEntry
 from evadb.catalog.models.udf_io_catalog import UdfIOCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.create_udf_plan import CreateUDFPlan
 from evadb.third_party.huggingface.create import gen_hf_io_catalog_entries
 from evadb.udfs.decorators.utils import load_io_from_udf_decorators
 from evadb.utils.errors import UDFIODefinitionError
 from evadb.utils.generic_utils import load_udf_class_from_file
 from evadb.utils.logging_manager import logger
 
 
 class CreateUDFExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: CreateUDFPlan):
+    def __init__(self, db: EvaDBDatabase, node: CreateUDFPlan):
         super().__init__(db, node)
         self.udf_dir = (
-            Path(self.config.get_value("core", "eva_installation_dir")) / "udfs"
+            Path(self.config.get_value("core", "evadb_installation_dir")) / "udfs"
         )
 
     def handle_huggingface_udf(self):
         """Handle HuggingFace UDFs
 
         HuggingFace UDFs are special UDFs that are not loaded from a file.
         So we do not need to call the setup method on them like we do for other UDFs.
```

### Comparing `evadb-0.2.7/evadb/executor/delete_executor.py` & `evadb-0.2.8/evadb/executor/delete_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,30 +15,30 @@
 from typing import Iterator
 
 import pandas as pd
 from sqlalchemy import and_, or_
 
 from evadb.catalog.catalog_type import TableType
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.expression.abstract_expression import ExpressionType
 from evadb.expression.comparison_expression import ComparisonExpression
 from evadb.expression.constant_value_expression import ConstantValueExpression
 from evadb.expression.logical_expression import LogicalExpression
 from evadb.expression.tuple_value_expression import TupleValueExpression
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.project_plan import ProjectPlan
 from evadb.storage.storage_engine import StorageEngine
 
 
 class DeleteExecutor(AbstractExecutor):
     """ """
 
-    def __init__(self, db: EVADatabase, node: ProjectPlan):
+    def __init__(self, db: EvaDBDatabase, node: ProjectPlan):
         super().__init__(db, node)
         self.predicate = node.where_clause
 
     def predicate_node_to_filter_clause(
         self, table: TableCatalogEntry, predicate_node: ComparisonExpression
     ):
         filter_clause = None
```

### Comparing `evadb-0.2.7/evadb/executor/drop_object_executor.py` & `evadb-0.2.8/evadb/executor/drop_object_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,27 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import pandas as pd
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError, handle_vector_store_params
 from evadb.models.storage.batch import Batch
 from evadb.parser.types import ObjectType
 from evadb.plan_nodes.drop_object_plan import DropObjectPlan
 from evadb.storage.storage_engine import StorageEngine
 from evadb.third_party.vector_stores.utils import VectorStoreFactory
 from evadb.utils.logging_manager import logger
 
 
 class DropObjectExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: DropObjectPlan):
+    def __init__(self, db: EvaDBDatabase, node: DropObjectPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         """Drop Object executor"""
 
         if self.node.object_type == ObjectType.TABLE:
             yield self._handle_drop_table(self.node.name, self.node.if_exists)
```

### Comparing `evadb-0.2.7/evadb/executor/exchange_executor.py` & `evadb-0.2.8/evadb/executor/exchange_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
 from ray.util.queue import Queue
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError
 from evadb.executor.ray_utils import (
     StageCompleteSignal,
     ray_parallel,
     ray_pull,
     ray_wait_and_alert,
@@ -49,15 +49,15 @@
                 input_queue.put(next_item)
                 raise next_item
             else:
                 yield next_item
 
 
 class ExchangeExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: ExchangePlan):
+    def __init__(self, db: EvaDBDatabase, node: ExchangePlan):
         self.inner_plan = node.inner_plan
         self.parallelism = node.parallelism
         self.ray_pull_env_conf_dict = node.ray_pull_env_conf_dict
         self.ray_parallel_env_conf_dict = node.ray_parallel_env_conf_dict
         super().__init__(db, node)
 
     def build_inner_executor(self, inner_executor):
```

### Comparing `evadb-0.2.7/evadb/executor/execution_context.py` & `evadb-0.2.8/evadb/executor/execution_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/executor/executor_utils.py` & `evadb-0.2.8/evadb/executor/executor_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/executor/explain_executor.py` & `evadb-0.2.8/evadb/executor/explain_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pandas as pd
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.abstract_plan import AbstractPlan
 from evadb.plan_nodes.explain_plan import ExplainPlan
 
 
 class ExplainExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: ExplainPlan):
+    def __init__(self, db: EvaDBDatabase, node: ExplainPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         # Traverse optimized physical plan, which is commonly supported.
         # Logical plan can be also printed by passing explainable_opr
         # attribute of the node, but is not done for now.
         plan_str = self._exec(self._node.children[0], 0)
```

### Comparing `evadb-0.2.7/evadb/executor/function_scan_executor.py` & `evadb-0.2.8/evadb/executor/function_scan_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.function_scan_plan import FunctionScanPlan
 
 
 class FunctionScanExecutor(AbstractExecutor):
     """
     Executes functional expression which yields a table of rows
     Arguments:
         node (AbstractPlan): FunctionScanPlan
 
     """
 
-    def __init__(self, db: EVADatabase, node: FunctionScanPlan):
+    def __init__(self, db: EvaDBDatabase, node: FunctionScanPlan):
         super().__init__(db, node)
         self.func_expr = node.func_expr
         self.do_unnest = node.do_unnest
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         assert (
             "lateral_input" in kwargs
```

### Comparing `evadb-0.2.7/evadb/executor/groupby_executor.py` & `evadb-0.2.8/evadb/executor/groupby_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import re
 from typing import Iterator
 
 import pandas as pd
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.groupby_plan import GroupByPlan
 
 
 class GroupByExecutor(AbstractExecutor):
     """
@@ -29,15 +29,15 @@
     E.g., "GROUP BY '8 frames'" groups every 8 frames into one segment
 
     Arguments:
         node (AbstractPlan): The GroupBy Plan
 
     """
 
-    def __init__(self, db: EVADatabase, node: GroupByPlan):
+    def __init__(self, db: EvaDBDatabase, node: GroupByPlan):
         super().__init__(db, node)
         numbers_only = re.sub(r"\D", "", node.groupby_clause.value)
         self._segment_length = int(numbers_only)
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
```

### Comparing `evadb-0.2.7/evadb/executor/hash_join_executor.py` & `evadb-0.2.8/evadb/executor/hash_join_executor.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import apply_predicate, apply_project
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.hash_join_probe_plan import HashJoinProbePlan
 
 
 class HashJoinExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: HashJoinProbePlan):
+    def __init__(self, db: EvaDBDatabase, node: HashJoinProbePlan):
         super().__init__(db, node)
         self.predicate = node.join_predicate
         self.join_type = node.join_type
         self.probe_keys = node.probe_keys
         self.join_project = node.join_project
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
```

### Comparing `evadb-0.2.7/evadb/executor/insert_executor.py` & `evadb-0.2.8/evadb/executor/insert_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,23 +11,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pandas as pd
 
 from evadb.catalog.catalog_type import TableType
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.insert_plan import InsertPlan
 from evadb.storage.storage_engine import StorageEngine
 
 
 class InsertExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: InsertPlan):
+    def __init__(self, db: EvaDBDatabase, node: InsertPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         storage_engine = None
         table_catalog_entry = None
 
         # Get catalog entry
```

### Comparing `evadb-0.2.7/evadb/executor/join_build_executor.py` & `evadb-0.2.8/evadb/executor/join_build_executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.hash_join_build_plan import HashJoinBuildPlan
 
 
 class BuildJoinExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: HashJoinBuildPlan):
+    def __init__(self, db: EvaDBDatabase, node: HashJoinBuildPlan):
         super().__init__(db, node)
         self.predicate = None  # node.join_predicate
         self.join_type = node.join_type
         self.build_keys = node.build_keys
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
```

### Comparing `evadb-0.2.7/evadb/executor/lateral_join_executor.py` & `evadb-0.2.8/evadb/executor/lateral_join_executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import apply_predicate, apply_project
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.lateral_join_plan import LateralJoinPlan
 
 
 class LateralJoinExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: LateralJoinPlan):
+    def __init__(self, db: EvaDBDatabase, node: LateralJoinPlan):
         super().__init__(db, node)
         self.predicate = node.join_predicate
         self.join_project = node.join_project
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         outer = self.children[0]
         inner = self.children[1]
```

### Comparing `evadb-0.2.7/evadb/executor/limit_executor.py` & `evadb-0.2.8/evadb/executor/limit_executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.limit_plan import LimitPlan
 
 
 class LimitExecutor(AbstractExecutor):
     """
     Limits the number of rows returned
 
     Arguments:
         node (AbstractPlan): The Limit Plan
 
     """
 
-    def __init__(self, db: EVADatabase, node: LimitPlan):
+    def __init__(self, db: EvaDBDatabase, node: LimitPlan):
         super().__init__(db, node)
         self._limit_count = node.limit_value
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         remaining_tuples = self._limit_count
         # aggregates the batches into one large batch
```

### Comparing `evadb-0.2.7/evadb/executor/load_csv_executor.py` & `evadb-0.2.8/evadb/executor/load_csv_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pandas as pd
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError
 from evadb.expression.tuple_value_expression import TupleValueExpression
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.load_data_plan import LoadDataPlan
 from evadb.readers.csv_reader import CSVReader
 from evadb.storage.storage_engine import StorageEngine
 from evadb.utils.logging_manager import logger
 
 
 class LoadCSVExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: LoadDataPlan):
+    def __init__(self, db: EvaDBDatabase, node: LoadDataPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         """
         Read the input csv file using pandas and persist data
         using storage engine
         """
```

### Comparing `evadb-0.2.7/evadb/executor/load_executor.py` & `evadb-0.2.8/evadb/executor/load_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.load_csv_executor import LoadCSVExecutor
 from evadb.executor.load_multimedia_executor import LoadMultimediaExecutor
 from evadb.parser.types import FileFormatType
 from evadb.plan_nodes.load_data_plan import LoadDataPlan
 
 
 class LoadDataExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: LoadDataPlan):
+    def __init__(self, db: EvaDBDatabase, node: LoadDataPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         """
         Use TYPE to determine the type of data to load.
         """
```

### Comparing `evadb-0.2.7/evadb/executor/load_multimedia_executor.py` & `evadb-0.2.8/evadb/executor/load_multimedia_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,28 +15,28 @@
 import multiprocessing as mp
 from multiprocessing import Pool
 from pathlib import Path
 
 import pandas as pd
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError, iter_path_regex, validate_media
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.load_data_plan import LoadDataPlan
 from evadb.storage.abstract_storage_engine import AbstractStorageEngine
 from evadb.storage.storage_engine import StorageEngine
 from evadb.utils.errors import DatasetFileNotFoundError
 from evadb.utils.logging_manager import logger
 from evadb.utils.s3_utils import download_from_s3
 
 
 class LoadMultimediaExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: LoadDataPlan):
+    def __init__(self, db: EvaDBDatabase, node: LoadDataPlan):
         super().__init__(db, node)
         self.media_type = self.node.file_options["file_format"]
 
     def exec(self, *args, **kwargs):
         storage_engine = None
         table_obj = None
         try:
```

### Comparing `evadb-0.2.7/evadb/executor/nested_loop_join_executor.py` & `evadb-0.2.8/evadb/executor/nested_loop_join_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import apply_predicate
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.nested_loop_join_plan import NestedLoopJoinPlan
 
 
 class NestedLoopJoinExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: NestedLoopJoinPlan):
+    def __init__(self, db: EvaDBDatabase, node: NestedLoopJoinPlan):
         super().__init__(db, node)
         self.predicate = node.join_predicate
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         outer = self.children[0]
         inner = self.children[1]
         for row1 in outer.exec(**kwargs):
```

### Comparing `evadb-0.2.7/evadb/executor/orderby_executor.py` & `evadb-0.2.8/evadb/executor/orderby_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError
 from evadb.expression.function_expression import FunctionExpression
 from evadb.expression.tuple_value_expression import TupleValueExpression
 from evadb.models.storage.batch import Batch
 from evadb.parser.types import ParserOrderBySortType
 from evadb.plan_nodes.orderby_plan import OrderByPlan
@@ -29,15 +29,15 @@
     Sort the frames which satisfy the condition
 
     Arguments:
         node (AbstractPlan): The OrderBy Plan
 
     """
 
-    def __init__(self, db: EVADatabase, node: OrderByPlan):
+    def __init__(self, db: EvaDBDatabase, node: OrderByPlan):
         super().__init__(db, node)
         self._orderby_list = node.orderby_list
         self._columns = node.columns
         self._sort_types = node.sort_types
         self.batch_sizes = []
 
     def _extract_column_name(self, col):
```

### Comparing `evadb-0.2.7/evadb/executor/plan_executor.py` & `evadb-0.2.8/evadb/executor/plan_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.apply_and_merge_executor import ApplyAndMergeExecutor
 from evadb.executor.create_executor import CreateExecutor
 from evadb.executor.create_index_executor import CreateIndexExecutor
 from evadb.executor.create_mat_view_executor import CreateMaterializedViewExecutor
 from evadb.executor.create_udf_executor import CreateUDFExecutor
 from evadb.executor.delete_executor import DeleteExecutor
@@ -55,18 +55,18 @@
 class PlanExecutor:
     """
     This is an interface between plan tree and execution tree.
     We traverse the plan tree and build execution tree from it
 
     Arguments:
         plan (AbstractPlan): Physical plan tree which needs to be executed
-        evadb (EVADatabase): database to execute the query on
+        evadb (EvaDBDatabase): database to execute the query on
     """
 
-    def __init__(self, evadb: EVADatabase, plan: AbstractPlan):
+    def __init__(self, evadb: EvaDBDatabase, plan: AbstractPlan):
         self._db = evadb
         self._plan = plan
 
     def _build_execution_tree(self, plan: AbstractPlan) -> AbstractExecutor:
         """build the execution tree from plan tree
 
         Arguments:
```

### Comparing `evadb-0.2.7/evadb/executor/pp_executor.py` & `evadb-0.2.8/evadb/executor/pp_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.pp_plan import PPScanPlan
 
 
 class PPExecutor(AbstractExecutor):
     """
@@ -27,15 +27,15 @@
         node (AbstractPlan): ...
 
     Note: This look kind of redundant. This logic for now is similar to that
     of sequential scan executor. Will decide to delete it depending on how
     sequential scan evolves.
     """
 
-    def __init__(self, db: EVADatabase, node: PPScanPlan):
+    def __init__(self, db: EvaDBDatabase, node: PPScanPlan):
         super().__init__(db, node)
         self.predicate = node.predicate
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         for batch in child_executor.exec():
             outcomes = self.predicate.evaluate(batch)
```

### Comparing `evadb-0.2.7/evadb/executor/predicate_executor.py` & `evadb-0.2.8/evadb/executor/predicate_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import apply_predicate
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.predicate_plan import PredicatePlan
 
 
 class PredicateExecutor(AbstractExecutor):
     """ """
 
-    def __init__(self, db: EVADatabase, node: PredicatePlan):
+    def __init__(self, db: EvaDBDatabase, node: PredicatePlan):
         super().__init__(db, node)
         self.predicate = node.predicate
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         for batch in child_executor.exec(**kwargs):
             batch = apply_predicate(batch, self.predicate, self.catalog())
```

### Comparing `evadb-0.2.7/evadb/executor/project_executor.py` & `evadb-0.2.8/evadb/executor/project_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import apply_project
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.project_plan import ProjectPlan
 
 
 class ProjectExecutor(AbstractExecutor):
     """ """
 
-    def __init__(self, db: EVADatabase, node: ProjectPlan):
+    def __init__(self, db: EvaDBDatabase, node: ProjectPlan):
         super().__init__(db, node)
         self.target_list = node.target_list
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
         for batch in child_executor.exec(**kwargs):
             batch = apply_project(batch, self.target_list, self.catalog())
```

### Comparing `evadb-0.2.7/evadb/executor/ray_utils.py` & `evadb-0.2.8/evadb/executor/ray_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/executor/rename_executor.py` & `evadb-0.2.8/evadb/executor/rename_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.plan_nodes.rename_plan import RenamePlan
 from evadb.storage.storage_engine import StorageEngine
 
 
 class RenameExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: RenamePlan):
+    def __init__(self, db: EvaDBDatabase, node: RenamePlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         """rename table executor
 
         Calls the catalog to modified catalog entry corresponding to the table.
         """
```

### Comparing `evadb-0.2.7/evadb/executor/sample_executor.py` & `evadb-0.2.8/evadb/executor/sample_executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.sample_plan import SamplePlan
 
 
 class SampleExecutor(AbstractExecutor):
     """
     Samples uniformly from the rows.
 
     Arguments:
         node (AbstractPlan): The Sample Plan
 
     """
 
-    def __init__(self, db: EVADatabase, node: SamplePlan):
+    def __init__(self, db: EvaDBDatabase, node: SamplePlan):
         super().__init__(db, node)
         self._sample_freq = node.sample_freq.value
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
 
         current = 0
```

### Comparing `evadb-0.2.7/evadb/executor/seq_scan_executor.py` & `evadb-0.2.8/evadb/executor/seq_scan_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import apply_predicate, apply_project
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.seq_scan_plan import SeqScanPlan
 
 
 class SequentialScanExecutor(AbstractExecutor):
     """
     Applies predicates to filter the frames which satisfy the condition
     Arguments:
         node (AbstractPlan): The SequentialScanPlan
 
     """
 
-    def __init__(self, db: EVADatabase, node: SeqScanPlan):
+    def __init__(self, db: EvaDBDatabase, node: SeqScanPlan):
         super().__init__(db, node)
         self.predicate = node.predicate
         self.project_expr = node.columns
         self.alias = node.alias
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         child_executor = self.children[0]
```

### Comparing `evadb-0.2.7/evadb/executor/show_info_executor.py` & `evadb-0.2.8/evadb/executor/show_info_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,23 +11,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import pandas as pd
 
 from evadb.catalog.catalog_type import TableType
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.parser.types import ShowType
 from evadb.plan_nodes.show_info_plan import ShowInfoPlan
 
 
 class ShowInfoExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: ShowInfoPlan):
+    def __init__(self, db: EvaDBDatabase, node: ShowInfoPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs):
         show_entries = []
 
         assert (
             self.node.show_type is ShowType.UDFS or ShowType.TABLES
```

### Comparing `evadb-0.2.7/evadb/executor/storage_executor.py` & `evadb-0.2.8/evadb/executor/storage_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,25 +11,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
 from evadb.catalog.catalog_type import TableType
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import ExecutorError
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.storage_plan import StoragePlan
 from evadb.storage.storage_engine import StorageEngine
 from evadb.utils.logging_manager import logger
 
 
 class StorageExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: StoragePlan):
+    def __init__(self, db: EvaDBDatabase, node: StoragePlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         try:
             storage_engine = StorageEngine.factory(self.db, self.node.table)
 
             if self.node.table.table_type == TableType.VIDEO_DATA:
```

### Comparing `evadb-0.2.7/evadb/executor/union_executor.py` & `evadb-0.2.8/evadb/executor/union_executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.union_plan import UnionPlan
 
 
 class UnionExecutor(AbstractExecutor):
     """
     Merge the seq scan queries
     Arguments:
         node (AbstractPlan): The UnionPlan
 
     """
 
-    def __init__(self, db: EVADatabase, node: UnionPlan):
+    def __init__(self, db: EvaDBDatabase, node: UnionPlan):
         super().__init__(db, node)
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
         assert self.node.all is True, "Only UNION ALL is supported now."
 
         # We should have only two children
         for child in self.children:
```

### Comparing `evadb-0.2.7/evadb/executor/vector_index_scan_executor.py` & `evadb-0.2.8/evadb/executor/vector_index_scan_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Iterator
 
 import pandas as pd
 
 from evadb.catalog.sql_config import IDENTIFIER_COLUMN
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.abstract_executor import AbstractExecutor
 from evadb.executor.executor_utils import handle_vector_store_params
 from evadb.models.storage.batch import Batch
 from evadb.plan_nodes.vector_index_scan_plan import VectorIndexScanPlan
 from evadb.third_party.vector_stores.types import VectorIndexQuery
 from evadb.third_party.vector_stores.utils import VectorStoreFactory
 from evadb.utils.logging_manager import logger
@@ -32,15 +32,15 @@
     for column in column_list:
         alias, col_name = column.split(".")
         if col_name == IDENTIFIER_COLUMN:
             return alias
 
 
 class VectorIndexScanExecutor(AbstractExecutor):
-    def __init__(self, db: EVADatabase, node: VectorIndexScanPlan):
+    def __init__(self, db: EvaDBDatabase, node: VectorIndexScanPlan):
         super().__init__(db, node)
 
         self.index_name = node.index_name
         self.limit_count = node.limit_count
         self.search_query_expr = node.search_query_expr
 
     def exec(self, *args, **kwargs) -> Iterator[Batch]:
```

### Comparing `evadb-0.2.7/evadb/expression/__init__.py` & `evadb-0.2.8/evadb/interfaces/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""expression subdirectory"""
```

### Comparing `evadb-0.2.7/evadb/expression/abstract_expression.py` & `evadb-0.2.8/evadb/expression/abstract_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/aggregation_expression.py` & `evadb-0.2.8/evadb/expression/aggregation_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/arithmetic_expression.py` & `evadb-0.2.8/evadb/expression/arithmetic_expression.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/comparison_expression.py` & `evadb-0.2.8/evadb/expression/comparison_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/constant_value_expression.py` & `evadb-0.2.8/evadb/expression/constant_value_expression.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/expression_utils.py` & `evadb-0.2.8/evadb/expression/expression_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/function_expression.py` & `evadb-0.2.8/evadb/expression/function_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/logical_expression.py` & `evadb-0.2.8/evadb/expression/logical_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/expression/tuple_value_expression.py` & `evadb-0.2.8/evadb/expression/tuple_value_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/interfaces/__init__.py` & `evadb-0.2.8/evadb/interfaces/relational/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/interfaces/relational/__init__.py` & `evadb-0.2.8/evadb/models/catalog/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/interfaces/relational/db.py` & `evadb-0.2.8/evadb/interfaces/relational/db.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,18 +12,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 
 import pandas
 
-from evadb.configuration.constants import EVA_DATABASE_DIR
-from evadb.database import EVADatabase, init_eva_db_instance
+from evadb.configuration.constants import EvaDB_DATABASE_DIR
+from evadb.database import EvaDBDatabase, init_evadb_instance
 from evadb.expression.tuple_value_expression import TupleValueExpression
-from evadb.interfaces.relational.relation import EVADBQuery
+from evadb.interfaces.relational.relation import EvaDBQuery
 from evadb.interfaces.relational.utils import execute_statement, try_binding
 from evadb.models.server.response import Response
 from evadb.models.storage.batch import Batch
 from evadb.parser.alias import Alias
 from evadb.parser.select_statement import SelectStatement
 from evadb.parser.utils import (
     parse_create_udf,
@@ -35,54 +35,54 @@
     parse_query,
     parse_table_clause,
 )
 from evadb.udfs.udf_bootstrap_queries import init_builtin_udfs
 from evadb.utils.logging_manager import logger
 
 
-class EVADBConnection:
-    def __init__(self, evadb: EVADatabase, reader, writer):
+class EvaDBConnection:
+    def __init__(self, evadb: EvaDBDatabase, reader, writer):
         self._reader = reader
         self._writer = writer
         self._cursor = None
         self._result: Batch = None
         self._evadb = evadb
 
     def cursor(self):
         """Retrieves a cursor associated with the connection.
 
         Returns:
-            EVADBCursor: The cursor object used to execute queries.
+            EvaDBCursor: The cursor object used to execute queries.
 
 
         Examples:
-            >>> from eva import connect
-            >>> conn = connect()
-            >>> cursor = conn.cursor()
+            >>> import evadb
+            >>> connection = connect()
+            >>> cursor = connection.cursor()
         """
         # One unique cursor for one connection
         if self._cursor is None:
-            self._cursor = EVADBCursor(self)
+            self._cursor = EvaDBCursor(self)
         return self._cursor
 
 
-class EVADBCursor(object):
+class EvaDBCursor(object):
     def __init__(self, connection):
         self._connection = connection
         self._evadb = connection._evadb
         self._pending_query = False
         self._result = None
 
     async def execute_async(self, query: str):
         """
-        Send query to the EVA server.
+        Send query to the EvaDB server.
         """
         if self._pending_query:
             raise SystemError(
-                "EVA does not support concurrent queries. \
+                "EvaDB does not support concurrent queries. \
                     Call fetch_all() to complete the pending query"
             )
         query = self._multiline_query_transformation(query)
         self._connection._writer.write((query + "\n").encode())
         await self._connection._writer.drain()
         self._pending_query = True
         return self
@@ -130,194 +130,240 @@
         def func_sync(*args, **kwargs):
             loop = asyncio.get_event_loop()
             res = loop.run_until_complete(func(*args, **kwargs))
             return res
 
         return func_sync
 
-    def table(self, table_name: str) -> EVADBQuery:
+    def table(self, table_name: str) -> EvaDBQuery:
         """
         Retrieves data from a table in the database.
 
         Args:
             table_name (str): Name of the table.
 
         Returns:
-            EVADBQuery: The EVADBQuery object representing the table query.
+            EvaDBQuery: The EvaDBQuery object representing the table query.
+
+        Examples:
+            >>> relation = conn.table("sample_table")
         """
         table = parse_table_clause(table_name)
         # SELECT * FROM table
         select_stmt = SelectStatement(
             target_list=[TupleValueExpression(col_name="*")], from_table=table
         )
         try_binding(self._evadb.catalog, select_stmt)
-        return EVADBQuery(self._evadb, select_stmt, alias=Alias(table_name.lower()))
+        return EvaDBQuery(self._evadb, select_stmt, alias=Alias(table_name.lower()))
 
     def df(self) -> pandas.DataFrame:
         """
         Returns the result as a pandas DataFrame.
 
         Returns:
             pandas.DataFrame: The result as a DataFrame.
 
         Raises:
             Exception: If no valid result is available with the current connection.
+
+        Examples:
+            >>> result = conn.query("CREATE TABLE IF NOT EXISTS youtube_video_text AS SELECT SpeechRecognizer(audio) FROM youtube_video;").df()
         """
         if not self._result:
             raise Exception("No valid result with the current cursor")
         return self._result.frames
 
     def create_vector_index(
         self, index_name: str, table_name: str, expr: str, using: str
-    ) -> "EVADBCursor":
+    ) -> "EvaDBCursor":
         """
         Creates a vector index using the provided expr on the table.
 
         Args:
             index_name (str): Name of the index.
             table_name (str): Name of the table.
             expr (str): Expression used to build the vector index.
             using (str): Method used for indexing, can be `FAISS` or `QDRANT`.
 
         Returns:
-            EVADBCursor: The EVADBCursor object.
+            EvaDBCursor: The EvaDBCursor object.
 
+        Examples:
+            Create a Vector Index using QDRANT
+
+            >>> conn.create_vector_index(
+                    "faiss_index",
+                    table_name="meme_images",
+                    expr="SiftFeatureExtractor(data)",
+                    using="QDRANT"
+                )
         """
         stmt = parse_create_vector_index(index_name, table_name, expr, using)
         self._result = execute_statement(self._evadb, stmt)
         return self
 
     def load(
         self, file_regex: str, table_name: str, format: str, **kwargs
-    ) -> EVADBQuery:
+    ) -> EvaDBQuery:
         """
         Loads data from files into a table.
 
         Args:
             file_regex (str): Regular expression specifying the files to load.
             table_name (str): Name of the table.
             format (str): File format of the data.
             **kwargs: Additional keyword arguments for configuring the load operation.
 
         Returns:
-            EVADBQuery: The EVADBQuery object representing the load query.
+            EvaDBQuery: The EvaDBQuery object representing the load query.
+
+        Examples:
+            Load the online_video.mp4 file into table named 'youtube_video'.
+
+            >>> conn.load("online_video.mp4", "youtube_video", "video")
         """
         # LOAD {FORMAT} file_regex INTO table_name
         stmt = parse_load(table_name, file_regex, format, **kwargs)
-        return EVADBQuery(self._evadb, stmt)
+        return EvaDBQuery(self._evadb, stmt)
 
-    def drop_table(self, table_name: str, if_exists: bool = True) -> "EVADBQuery":
+    def drop_table(self, table_name: str, if_exists: bool = True) -> "EvaDBQuery":
         """
         Drop a table in the database.
 
         Args:
             table_name (str): Name of the table to be dropped.
-            if_exists (bool): If True, do not raise an error if the Tabel does not already exist. If False, raise an error.
+            if_exists (bool): If True, do not raise an error if the Table does not already exist. If False, raise an error.
+
+        Returns:
+            EvaDBQuery: The EvaDBQuery object representing the DROP TABLE.
 
-        Returns
-            EVADBQuery: The EVADBQuery object representing the DROP TABLE.
+        Examples:
+            Drop table 'sample_table'
+
+            >>> conn.drop_table("sample_table", if_exists = True)
         """
         stmt = parse_drop_table(table_name, if_exists)
-        return EVADBQuery(self._evadb, stmt)
+        return EvaDBQuery(self._evadb, stmt)
 
-    def drop_udf(self, udf_name: str, if_exists: bool = True) -> "EVADBQuery":
+    def drop_udf(self, udf_name: str, if_exists: bool = True) -> "EvaDBQuery":
         """
         Drop a udf in the database.
 
         Args:
             udf_name (str): Name of the udf to be dropped.
             if_exists (bool): If True, do not raise an error if the UDF does not already exist. If False, raise an error.
 
-        Returns
-            EVADBQuery: The EVADBQuery object representing the DROP UDF.
+        Returns:
+            EvaDBQuery: The EvaDBQuery object representing the DROP UDF.
+
+        Examples:
+            Drop UDF 'ObjectDetector'
+
+            >>> conn.drop_udf("ObjectDetector", if_exists = True)
         """
         stmt = parse_drop_udf(udf_name, if_exists)
-        return EVADBQuery(self._evadb, stmt)
+        return EvaDBQuery(self._evadb, stmt)
 
-    def drop_index(self, index_name: str, if_exists: bool = True) -> "EVADBQuery":
+    def drop_index(self, index_name: str, if_exists: bool = True) -> "EvaDBQuery":
         """
         Drop an index in the database.
 
         Args:
             index_name (str): Name of the index to be dropped.
             if_exists (bool): If True, do not raise an error if the index does not already exist. If False, raise an error.
 
-        Returns
-            EVADBQuery: The EVADBQuery object representing the DROP INDEX.
+        Returns:
+            EvaDBQuery: The EvaDBQuery object representing the DROP INDEX.
+
+        Examples:
+            Drop the index with name 'faiss_index'
+
+            >>> conn.drop_index("faiss_index", if_exists = True)
         """
         stmt = parse_drop_index(index_name, if_exists)
-        return EVADBQuery(self._evadb, stmt)
+        return EvaDBQuery(self._evadb, stmt)
 
     def create_udf(
         self,
         udf_name: str,
         if_not_exists: bool = True,
         impl_path: str = None,
         type: str = None,
         **kwargs
-    ) -> "EVADBQuery":
+    ) -> "EvaDBQuery":
         """
         Create a udf in the database.
 
         Args:
             udf_name (str): Name of the udf to be created.
             if_not_exists (bool): If True, do not raise an error if the UDF already exist. If False, raise an error.
             impl_path (str): Path string to udf's implementation.
             type (str): Type of the udf (e.g. HuggingFace).
             **kwargs: Additional keyword arguments for configuring the create udf operation.
 
-        Returns
-            EVADBQuery: The EVADBQuery object representing the UDF created.
+        Returns:
+            EvaDBQuery: The EvaDBQuery object representing the UDF created.
+
+        Examples:
+            >>> conn.create_udf("MnistImageClassifier", if_exists = True, 'mnist_image_classifier.py')
         """
         stmt = parse_create_udf(udf_name, if_not_exists, impl_path, type, **kwargs)
-        return EVADBQuery(self._evadb, stmt)
+        return EvaDBQuery(self._evadb, stmt)
 
-    def query(self, sql_query: str) -> EVADBQuery:
+    def query(self, sql_query: str) -> EvaDBQuery:
         """
         Executes a SQL query.
 
         Args:
             sql_query (str): The SQL query to be executed
+
         Returns:
-            EVADBQuery: The EVADBQuery object.
+            EvaDBQuery: The EvaDBQuery object.
+
+        Examples:
+            >>> conn.query("DROP UDF IF EXISTS SentenceFeatureExtractor;")
         """
         stmt = parse_query(sql_query)
-        return EVADBQuery(self._evadb, stmt)
+        return EvaDBQuery(self._evadb, stmt)
 
 
 def connect(
-    eva_dir: str = EVA_DATABASE_DIR, sql_backend: str = None
-) -> EVADBConnection:
+    evadb_dir: str = EvaDB_DATABASE_DIR, sql_backend: str = None
+) -> EvaDBConnection:
     """
-    Connects to the EVA server and returns a connection object.
+    Connects to the EvaDB server and returns a connection object.
 
     Args:
-        eva_dir (str): The directory used by EVA to store database-related content. Default is "eva_db".
+        evadb_dir (str): The directory used by EvaDB to store database-related content. Default is "evadb".
         sql_backend (str): Custom database URI to be used. We follow the SQLAlchemy database URL format.
-            Default is SQLite in the EVA directory. See https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls.
+            Default is SQLite in the EvaDB directory. See https://docs.sqlalchemy.org/en/20/core/engines.html#database-urls.
 
     Returns:
-        EVADBConnection: A connection object representing the connection to the EVA database.
+        EvaDBConnection: A connection object representing the connection to the EvaDB database.
+
+    Examples:
+        >>> from evadb import connect
+        >>> conn = connect()
     """
 
     # As we are not employing a client-server approach for the Pythonic interface, the
-    # host and port parameters are irrelevant. Additionally, for the EVADBConnection, the
+    # host and port parameters are irrelevant. Additionally, for the EvaDBConnection, the
     # reader and writer parameters are not relevant in the serverless approach.
-    evadb = init_eva_db_instance(eva_dir, custom_db_uri=sql_backend)
+    evadb = init_evadb_instance(evadb_dir, custom_db_uri=sql_backend)
     init_builtin_udfs(evadb, mode="release")
-    return EVADBConnection(evadb, None, None)
+    return EvaDBConnection(evadb, None, None)
 
 
 # WIP
 # support remote connections from pythonic APIs
 
 
-async def get_connection(host: str, port: int) -> EVADBConnection:
+async def get_connection(host: str, port: int) -> EvaDBConnection:
     reader, writer = await asyncio.open_connection(host, port)
     # no db required for remote connection
-    connection = EVADBConnection(None, reader, writer)
+    connection = EvaDBConnection(None, reader, writer)
     return connection
 
 
-def connect_remote(host: str, port: int) -> EVADBConnection:
+def connect_remote(host: str, port: int) -> EvaDBConnection:
     connection = asyncio.run(get_connection(host, port))
     return connection
```

### Comparing `evadb-0.2.7/evadb/interfaces/relational/relation.py` & `evadb-0.2.8/evadb/interfaces/relational/relation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from typing import Union
 
 import pandas
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.interfaces.relational.utils import (
     create_limit_expression,
     create_star_expression,
     execute_statement,
     handle_select_clause,
     sql_predicate_to_expresssion_tree,
     sql_string_to_expresssion_list,
@@ -32,49 +32,49 @@
 from evadb.parser.select_statement import SelectStatement
 from evadb.parser.statement import AbstractStatement
 from evadb.parser.table_ref import JoinNode, TableRef
 from evadb.parser.types import JoinType
 from evadb.parser.utils import parse_sql_orderby_expr
 
 
-class EVADBQuery:
+class EvaDBQuery:
     def __init__(
         self,
-        evadb: EVADatabase,
+        evadb: EvaDBDatabase,
         query_node: Union[AbstractStatement, TableRef],
         alias: Alias = None,
     ):
         self._evadb = evadb
         self._query_node = query_node
         self._alias = alias
 
-    def alias(self, alias: str) -> "EVADBQuery":
+    def alias(self, alias: str) -> "EvaDBQuery":
         """Returns a new Relation with an alias set.
 
         Args:
             alias (str): an alias name to be set for the Relation.
 
         Returns:
-            EVADBQuery: Aliased Relation.
+            EvaDBQuery: Aliased Relation.
 
         Examples:
             >>> relation = conn.table("sample_table")
             >>> relation.alias('table')
         """
         self._alias = Alias(alias)
 
-    def cross_apply(self, expr: str, alias: str) -> "EVADBQuery":
+    def cross_apply(self, expr: str, alias: str) -> "EvaDBQuery":
         """Execute a expr on all the rows of the relation
 
         Args:
             expr (str): sql expression
             alias (str): alias of the output of the expr
 
         Returns:
-            `EVADBQuery`: relation
+            `EvaDBQuery`: relation
 
         Examples:
 
             Runs Yolo on all the frames of the input table
 
             >>> relation = conn.table("videos")
             >>> relation.cross_apply("Yolo(data)", "objs(labels, bboxes, scores)")
@@ -111,29 +111,29 @@
         assert batch is not None, "relation execute failed"
         return batch.frames
 
     def execute(self) -> Batch:
         """Transform the relation into a result set
 
         Returns:
-            Batch: result as eva Batch
+            Batch: result as evadb Batch
         """
         result = execute_statement(self._evadb, self._query_node.copy())
         assert result.frames is not None
         return result
 
-    def filter(self, expr: str) -> "EVADBQuery":
+    def filter(self, expr: str) -> "EvaDBQuery":
         """
-        Filters rows using the given condition. Multiple chained filters results in `AND`
+        Filters rows using the given condition. Multiple filters can be chained using `AND`
 
         Parameters:
             expr (str): The filter expression.
 
         Returns:
-            EVADBQuery : Filtered EVADBQuery.
+            EvaDBQuery : Filtered EvaDBQuery.
         Examples:
             >>> relation = conn.table("sample_table")
             >>> relation.filter("col1 > 10")
 
             Filter by sql string
 
             >>> relation.filter("col1 > 10 AND col1 < 20")
@@ -145,22 +145,22 @@
             self._query_node, self._alias, "where_clause", parsed_expr
         )
 
         try_binding(self._evadb.catalog, self._query_node)
 
         return self
 
-    def limit(self, num: int) -> "EVADBQuery":
+    def limit(self, num: int) -> "EvaDBQuery":
         """Limits the result count to the number specified.
 
         Args:
             num (int): Number of records to return. Will return num records or all records if the Relation contains fewer records.
 
         Returns:
-            EVADBQuery: Relation with subset of records
+            EvaDBQuery: Relation with subset of records
 
         Examples:
             >>> relation = conn.table("sample_table")
             >>> relation.limit(10)
 
         """
 
@@ -169,51 +169,56 @@
             self._query_node, self._alias, "limit_count", limit_expr
         )
 
         try_binding(self._evadb.catalog, self._query_node)
 
         return self
 
-    def order(self, order_expr: str) -> "EVADBQuery":
+    def order(self, order_expr: str) -> "EvaDBQuery":
         """Reorder the relation based on the order_expr
 
         Args:
             order_expr (str): sql expression to order the relation
 
         Returns:
-            EVADBQuery: A EVADBQuery ordered based on the order_expr.
+            EvaDBQuery: A EvaDBQuery ordered based on the order_expr.
+
+        Examples:
+            >>> relation = conn.table("PDFs")
+            >>> relation.order("Similarity(SentenceTransformerFeatureExtractor('When was the NATO created?'), SentenceTransformerFeatureExtractor(data) ) DESC")
+
         """
 
         parsed_expr = parse_sql_orderby_expr(order_expr)
         self._query_node = handle_select_clause(
             self._query_node, self._alias, "orderby_list", parsed_expr
         )
 
         try_binding(self._evadb.catalog, self._query_node)
 
         return self
 
-    def select(self, expr: str) -> "EVADBQuery":
+    def select(self, expr: str) -> "EvaDBQuery":
         """
-        Projects a set of expressions and returns a new EVADBQuery.
+        Projects a set of expressions and returns a new EvaDBQuery.
 
         Parameters:
-            exprs (Union[str, List[str]]): The expression(s) to be selected. If '*' is provided, it expands to all columns in the current EVADBQuery.
+            exprs (Union[str, List[str]]): The expression(s) to be selected. If '*' is provided, it expands to all columns in the current EvaDBQuery.
 
         Returns:
-            EVADBQuery: A EVADBQuery with subset (or all) of columns.
+            EvaDBQuery: A EvaDBQuery with subset (or all) of columns.
 
         Examples:
             >>> relation = conn.table("sample_table")
 
-            Select all columns in the EVADBQuery.
+            Select all columns in the EvaDBQuery.
 
             >>> relation.select("*")
 
-            Select all subset of columns in the EVADBQuery.
+            Select all subset of columns in the EvaDBQuery.
 
             >>> relation.select("col1")
             >>> relation.select("col1, col2")
         """
 
         parsed_exprs = sql_string_to_expresssion_list(expr)
```

### Comparing `evadb-0.2.7/evadb/interfaces/relational/utils.py` & `evadb-0.2.8/evadb/interfaces/relational/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 from typing import Callable, List, Union
 
 from evadb.binder.statement_binder import StatementBinder
 from evadb.binder.statement_binder_context import StatementBinderContext
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.plan_executor import PlanExecutor
 from evadb.expression.abstract_expression import AbstractExpression
 from evadb.expression.constant_value_expression import ConstantValueExpression
 from evadb.expression.tuple_value_expression import TupleValueExpression
 from evadb.models.storage.batch import Batch
 from evadb.optimizer.plan_generator import PlanGenerator
 from evadb.optimizer.statement_to_opr_converter import StatementToPlanConverter
@@ -32,31 +32,31 @@
     parse_expression,
     parse_lateral_join,
     parse_predicate_expression,
 )
 
 
 def sql_string_to_expresssion_list(expr: str) -> List[AbstractExpression]:
-    """Converts the sql expression to list of eva abstract expressions
+    """Converts the sql expression to list of evadb abstract expressions
 
     Args:
         expr (str): the expr to convert
 
     Returns:
-        List[AbstractExpression]: list of eva abstract expressions
+        List[AbstractExpression]: list of evadb abstract expressions
 
     """
     return parse_expression(expr)
 
 
 def sql_predicate_to_expresssion_tree(expr: str) -> AbstractExpression:
     return parse_predicate_expression(expr)
 
 
-def execute_statement(evadb: EVADatabase, statement: AbstractStatement) -> Batch:
+def execute_statement(evadb: EvaDBDatabase, statement: AbstractStatement) -> Batch:
     StatementBinder(StatementBinderContext(evadb.catalog)).bind(statement)
     l_plan = StatementToPlanConverter().visit(statement)
     p_plan = asyncio.run(PlanGenerator(evadb).build(l_plan))
     output = PlanExecutor(evadb, p_plan).execute_plan()
     if output:
         batch_list = list(output)
         return Batch.concat(batch_list, copy=False)
```

### Comparing `evadb-0.2.7/evadb/models/__init__.py` & `evadb-0.2.8/evadb/models/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""builds the different models used in eva"""
+"""builds the different models used in evadb"""
```

### Comparing `evadb-0.2.7/evadb/models/catalog/__init__.py` & `evadb-0.2.8/evadb/models/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/models/catalog/frame_info.py` & `evadb-0.2.8/evadb/models/catalog/frame_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/models/catalog/properties.py` & `evadb-0.2.8/evadb/models/catalog/properties.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/models/server/__init__.py` & `evadb-0.2.8/evadb/models/storage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/models/server/response.py` & `evadb-0.2.8/evadb/models/server/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -25,15 +25,15 @@
     FAIL = -1
     SUCCESS = 0
 
 
 @dataclass(frozen=True)
 class Response:
     """
-    Data model for EVA server response
+    Data model for EvaDB server response
     """
 
     status: ResponseStatus = ResponseStatus.FAIL
     batch: Batch = None
     error: Optional[str] = None
     query_time: Optional[float] = None
```

### Comparing `evadb-0.2.7/evadb/models/storage/__init__.py` & `evadb-0.2.8/evadb/optimizer/rules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/models/storage/batch.py` & `evadb-0.2.8/evadb/models/storage/batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/__init__.py` & `evadb-0.2.8/test/udfs/ndarray/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""general optimizers for eva"""
+"""user defined test functions operating on ndarrays udfs"""
```

### Comparing `evadb-0.2.7/evadb/optimizer/binder.py` & `evadb-0.2.8/evadb/optimizer/binder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/cost_model.py` & `evadb-0.2.8/evadb/optimizer/cost_model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/group.py` & `evadb-0.2.8/evadb/optimizer/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/group_expression.py` & `evadb-0.2.8/evadb/optimizer/group_expression.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/memo.py` & `evadb-0.2.8/evadb/optimizer/memo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/operators.py` & `evadb-0.2.8/evadb/optimizer/operators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/optimizer_context.py` & `evadb-0.2.8/evadb/optimizer/optimizer_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import copy
 
 from evadb.constants import UNDEFINED_GROUP_ID
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.optimizer.cost_model import CostModel
 from evadb.optimizer.group_expression import GroupExpression
 from evadb.optimizer.memo import Memo
 from evadb.optimizer.operators import Dummy, Operator
 from evadb.optimizer.optimizer_task_stack import OptimizerTaskStack
 from evadb.optimizer.rules.rules_manager import RulesManager
 
@@ -30,15 +30,18 @@
 
     Arguments:
         _task_queue(OptimizerTaskStack):
             stack to keep track outstanding tasks
     """
 
     def __init__(
-        self, db: EVADatabase, cost_model: CostModel, rules_manager: RulesManager = None
+        self,
+        db: EvaDBDatabase,
+        cost_model: CostModel,
+        rules_manager: RulesManager = None,
     ):
         self._db = db
         self._task_stack = OptimizerTaskStack()
         self._memo = Memo()
         self._cost_model = cost_model
         self._rules_manager = rules_manager or RulesManager(db.config)
```

### Comparing `evadb-0.2.7/evadb/optimizer/optimizer_task_stack.py` & `evadb-0.2.8/evadb/optimizer/optimizer_task_stack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/optimizer_tasks.py` & `evadb-0.2.8/evadb/optimizer/optimizer_tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -289,15 +289,15 @@
     def execute(self):
         cost = 0
         memo = self.optimizer_context.memo
         grp = memo.get_group_by_id(self.root_expr.group_id)
         for child_id in self.root_expr.children:
             child_grp = memo.get_group_by_id(child_id)
             if child_grp.get_best_expr(PropertyType.DEFAULT):
-                # Note: May never get hit when using EVA on Ray
+                # Note: May never get hit when using EvaDB on Ray
                 cost += child_grp.get_best_expr_cost(PropertyType.DEFAULT)
             else:
                 self.optimizer_context.task_stack.push(
                     OptimizeInputs(self.root_expr, self.optimizer_context)
                 )
                 self.optimizer_context.task_stack.push(
                     OptimizeGroup(child_grp, self.optimizer_context)
```

### Comparing `evadb-0.2.7/evadb/optimizer/optimizer_utils.py` & `evadb-0.2.8/evadb/optimizer/optimizer_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/plan_generator.py` & `evadb-0.2.8/evadb/optimizer/plan_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 
 import nest_asyncio
 
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.optimizer.cost_model import CostModel
 from evadb.optimizer.operators import Operator
 from evadb.optimizer.optimizer_context import OptimizerContext
 from evadb.optimizer.optimizer_task_stack import OptimizerTaskStack
 from evadb.optimizer.optimizer_tasks import (
     BottomUpRewrite,
     OptimizeGroup,
@@ -35,15 +35,15 @@
 class PlanGenerator:
     """
     Used for building Physical Plan from Logical Plan.
     """
 
     def __init__(
         self,
-        db: EVADatabase,
+        db: EvaDBDatabase,
         rules_manager: RulesManager = None,
         cost_model: CostModel = None,
     ) -> None:
         self.db = db
         self.rules_manager = rules_manager or RulesManager(db.config)
         self.cost_model = cost_model or CostModel()
```

### Comparing `evadb-0.2.7/evadb/optimizer/property.py` & `evadb-0.2.8/evadb/optimizer/property.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/rules/__init__.py` & `evadb-0.2.8/evadb/parser/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/rules/pattern.py` & `evadb-0.2.8/evadb/optimizer/rules/pattern.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/rules/rules.py` & `evadb-0.2.8/evadb/optimizer/rules/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/rules/rules_base.py` & `evadb-0.2.8/evadb/optimizer/rules/rules_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/rules/rules_manager.py` & `evadb-0.2.8/evadb/optimizer/rules/rules_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/optimizer/statement_to_opr_converter.py` & `evadb-0.2.8/evadb/optimizer/statement_to_opr_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/__init__.py` & `evadb-0.2.8/evadb/readers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/alias.py` & `evadb-0.2.8/evadb/parser/alias.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/create_index_statement.py` & `evadb-0.2.8/evadb/parser/create_index_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/create_mat_view_statement.py` & `evadb-0.2.8/evadb/parser/create_mat_view_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/create_statement.py` & `evadb-0.2.8/evadb/parser/create_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/create_udf_statement.py` & `evadb-0.2.8/evadb/parser/create_udf_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/delete_statement.py` & `evadb-0.2.8/evadb/parser/delete_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/drop_object_statement.py` & `evadb-0.2.8/evadb/parser/drop_object_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/evadb.lark` & `evadb-0.2.8/evadb/parser/evadb.lark`

 * *Files identical despite different names*

### Comparing `evadb-0.2.7/evadb/parser/explain_statement.py` & `evadb-0.2.8/evadb/parser/explain_statement.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/insert_statement.py` & `evadb-0.2.8/evadb/parser/insert_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_parser.py` & `evadb-0.2.8/evadb/parser/lark_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -17,15 +17,15 @@
 from lark import Lark
 
 from evadb.parser.lark_visitor import LarkInterpreter
 
 
 class LarkParser(object):
     """
-    Parser for EVA QL based on Lark
+    Parser for EvaDB QL based on Lark
     """
 
     _parser = None
 
     def __new__(cls):
         if not hasattr(cls, "_instance"):
             cls._instance = super(LarkParser, cls).__new__(cls)
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/__init__.py` & `evadb-0.2.8/evadb/parser/lark_visitor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_common_clauses_ids.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_common_clauses_ids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_create_statements.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_create_statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_delete_statement.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_delete_statement.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_drop_statement.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_drop_statement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_explain_statement.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_explain_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_expressions.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_functions.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_insert_statements.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_insert_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_load_statement.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_load_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_rename_statement.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_rename_statement.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_select_statement.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_select_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_show_statements.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_show_statements.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/lark_visitor/_table_sources.py` & `evadb-0.2.8/evadb/parser/lark_visitor/_table_sources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/load_statement.py` & `evadb-0.2.8/evadb/parser/load_statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/parser.py` & `evadb-0.2.8/evadb/parser/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,15 +13,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from evadb.parser.lark_parser import LarkParser
 
 
 class Parser(object):
     """
-    Parser based on EVAQL grammar: evadb.lark
+    Parser based on EvaDB grammar: evadb.lark
     """
 
     _lark_parser = None
 
     def __new__(cls):
         if not hasattr(cls, "_instance"):
             cls._instance = super(Parser, cls).__new__(cls)
```

### Comparing `evadb-0.2.7/evadb/parser/rename_statement.py` & `evadb-0.2.8/evadb/parser/rename_statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/select_statement.py` & `evadb-0.2.8/evadb/parser/select_statement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/show_statement.py` & `evadb-0.2.8/evadb/parser/show_statement.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/statement.py` & `evadb-0.2.8/evadb/parser/statement.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/table_ref.py` & `evadb-0.2.8/evadb/parser/table_ref.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/parser/types.py` & `evadb-0.2.8/evadb/parser/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from evadb.utils.generic_utils import EVAEnum
+from evadb.utils.generic_utils import EvaDBEnum
 
 
-class ColumnConstraintEnum(EVAEnum):
+class ColumnConstraintEnum(EvaDBEnum):
     NOTNULL  # noqa: F821
     DEFAULT  # noqa: F821
     PRIMARY  # noqa: F821
     UNIQUE  # noqa: F821
 
 
-class StatementType(EVAEnum):
+class StatementType(EvaDBEnum):
     """
-    Manages EVAEnums for all the sql-like statements supported
+    Manages EvaDBEnums for all the sql-like statements supported
     """
 
     SELECT  # noqa: F821
     CREATE  # noqa: F821
     RENAME  # noqa: F821
     DROP_OBJECT  # noqa: F821
     INSERT  # noqa: F821
@@ -39,42 +39,42 @@
     CREATE_MATERIALIZED_VIEW  # noqa: F821
     SHOW  # noqa: F821
     EXPLAIN  # noqa: F821
     CREATE_INDEX  # noqa: F821
     # add other types
 
 
-class ParserOrderBySortType(EVAEnum):
+class ParserOrderBySortType(EvaDBEnum):
     """
-    Manages EVAEnums for all order by sort types
+    Manages EvaDBEnums for all order by sort types
     """
 
     ASC  # noqa: F821
     DESC  # noqa: F821
 
 
-class JoinType(EVAEnum):
+class JoinType(EvaDBEnum):
     LATERAL_JOIN  # noqa: F821
     INNER_JOIN  # noqa: F821
 
 
-class FileFormatType(EVAEnum):
+class FileFormatType(EvaDBEnum):
     VIDEO  # noqa: F821
     CSV  # noqa: F821
     IMAGE  # noqa: F821
     DOCUMENT  # noqa: F821
     PDF  # noqa: F821
 
 
-class ShowType(EVAEnum):
+class ShowType(EvaDBEnum):
     UDFS  # noqa: F821
     TABLES  # noqa: F821
 
 
-class UDFType(EVAEnum):
+class UDFType(EvaDBEnum):
     EXTRACT_OBJECT  # noqa: F821
 
 
-class ObjectType(EVAEnum):
+class ObjectType(EvaDBEnum):
     TABLE  # noqa: F821
     UDF  # noqa: F821
     INDEX  # noqa: F821
```

### Comparing `evadb-0.2.7/evadb/parser/utils.py` & `evadb-0.2.8/evadb/parser/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/__init__.py` & `evadb-0.2.8/evadb/readers/document/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""planner subdirectory"""
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/abstract_join_plan.py` & `evadb-0.2.8/evadb/plan_nodes/abstract_join_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/abstract_plan.py` & `evadb-0.2.8/evadb/plan_nodes/abstract_plan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/abstract_scan_plan.py` & `evadb-0.2.8/evadb/plan_nodes/abstract_scan_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/apply_and_merge_plan.py` & `evadb-0.2.8/evadb/plan_nodes/apply_and_merge_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/create_index_plan.py` & `evadb-0.2.8/evadb/plan_nodes/create_index_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/create_mat_view_plan.py` & `evadb-0.2.8/evadb/plan_nodes/create_mat_view_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/create_plan.py` & `evadb-0.2.8/evadb/plan_nodes/create_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/create_udf_plan.py` & `evadb-0.2.8/evadb/plan_nodes/create_udf_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -33,16 +33,14 @@
             else will replace the existing
         inputs: List[UdfIOCatalogEntry]
             udf inputs, annotated list similar to table columns
         outputs: List[UdfIOCatalogEntry]
             udf outputs, annotated list similar to table columns
         impl_file_path: Path
             file path which holds the implementation of the udf.
-            This file should be placed in the data directory and
-            the path provided should be relative to the eva dir.
         udf_type: str
             udf type. it ca be object detection, classification etc.
     """
 
     def __init__(
         self,
         name: str,
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/delete_plan.py` & `evadb-0.2.8/evadb/plan_nodes/delete_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/drop_object_plan.py` & `evadb-0.2.8/evadb/plan_nodes/drop_object_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/exchange_plan.py` & `evadb-0.2.8/evadb/plan_nodes/exchange_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/explain_plan.py` & `evadb-0.2.8/evadb/plan_nodes/explain_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/function_scan_plan.py` & `evadb-0.2.8/evadb/plan_nodes/function_scan_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/groupby_plan.py` & `evadb-0.2.8/evadb/plan_nodes/groupby_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/hash_join_build_plan.py` & `evadb-0.2.8/evadb/plan_nodes/hash_join_build_plan.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/hash_join_probe_plan.py` & `evadb-0.2.8/evadb/plan_nodes/hash_join_probe_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/insert_plan.py` & `evadb-0.2.8/evadb/plan_nodes/insert_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/lateral_join_plan.py` & `evadb-0.2.8/evadb/plan_nodes/lateral_join_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/limit_plan.py` & `evadb-0.2.8/evadb/plan_nodes/limit_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/load_data_plan.py` & `evadb-0.2.8/evadb/plan_nodes/load_data_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/nested_loop_join_plan.py` & `evadb-0.2.8/evadb/plan_nodes/nested_loop_join_plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/orderby_plan.py` & `evadb-0.2.8/evadb/plan_nodes/orderby_plan.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/pp_plan.py` & `evadb-0.2.8/evadb/plan_nodes/pp_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/predicate_plan.py` & `evadb-0.2.8/evadb/plan_nodes/predicate_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/project_plan.py` & `evadb-0.2.8/evadb/plan_nodes/project_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/rename_plan.py` & `evadb-0.2.8/evadb/plan_nodes/rename_plan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/sample_plan.py` & `evadb-0.2.8/evadb/plan_nodes/sample_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/seq_scan_plan.py` & `evadb-0.2.8/evadb/plan_nodes/seq_scan_plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/show_info_plan.py` & `evadb-0.2.8/evadb/plan_nodes/show_info_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/storage_plan.py` & `evadb-0.2.8/evadb/plan_nodes/storage_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/types.py` & `evadb-0.2.8/evadb/plan_nodes/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/union_plan.py` & `evadb-0.2.8/evadb/plan_nodes/union_plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/plan_nodes/vector_index_scan_plan.py` & `evadb-0.2.8/evadb/plan_nodes/vector_index_scan_plan.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/__init__.py` & `evadb-0.2.8/evadb/readers/image/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/abstract_reader.py` & `evadb-0.2.8/evadb/readers/abstract_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/csv_reader.py` & `evadb-0.2.8/evadb/readers/csv_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/decord_reader.py` & `evadb-0.2.8/evadb/readers/decord_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/document/__init__.py` & `evadb-0.2.8/evadb/udfs/decorators/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/document/document_reader.py` & `evadb-0.2.8/evadb/readers/document/document_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/document/registry.py` & `evadb-0.2.8/evadb/readers/document/registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/image/__init__.py` & `evadb-0.2.8/evadb/udfs/decorators/io_descriptors/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/image/opencv_image_reader.py` & `evadb-0.2.8/evadb/readers/image/opencv_image_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/readers/pdf_reader.py` & `evadb-0.2.8/evadb/readers/pdf_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/server/__init__.py` & `evadb-0.2.8/evadb/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/server/command_handler.py` & `evadb-0.2.8/evadb/server/command_handler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,27 +13,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 from typing import Iterator, Optional
 
 from evadb.binder.statement_binder import StatementBinder
 from evadb.binder.statement_binder_context import StatementBinderContext
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.executor.plan_executor import PlanExecutor
 from evadb.models.server.response import Response, ResponseStatus
 from evadb.models.storage.batch import Batch
 from evadb.optimizer.plan_generator import PlanGenerator
 from evadb.optimizer.statement_to_opr_converter import StatementToPlanConverter
 from evadb.parser.parser import Parser
 from evadb.utils.logging_manager import logger
 from evadb.utils.stats import Timer
 
 
 def execute_query(
-    evadb: EVADatabase, query, report_time: bool = False, **kwargs
+    evadb: EvaDBDatabase, query, report_time: bool = False, **kwargs
 ) -> Iterator[Batch]:
     """
     Execute the query and return a result generator.
     """
     query_compile_time = Timer()
     plan_generator = kwargs.pop("plan_generator", PlanGenerator(evadb))
     with query_compile_time:
@@ -44,26 +44,26 @@
         output = PlanExecutor(evadb, p_plan).execute_plan()
 
     query_compile_time.log_elapsed_time("Query Compile Time")
     return output
 
 
 def execute_query_fetch_all(
-    evadb: EVADatabase, query=None, **kwargs
+    evadb: EvaDBDatabase, query=None, **kwargs
 ) -> Optional[Batch]:
     """
     Execute the query and fetch all results into one Batch object.
     """
     output = execute_query(evadb, query, report_time=True, **kwargs)
     if output:
         batch_list = list(output)
         return Batch.concat(batch_list, copy=False)
 
 
-async def handle_request(evadb: EVADatabase, client_writer, request_message):
+async def handle_request(evadb: EvaDBDatabase, client_writer, request_message):
     """
     Reads a request from a client and processes it
 
     If user inputs 'quit' stops the event loop
     otherwise just echoes user input
     """
     logger.debug("Receive request: --|" + str(request_message) + "|--")
```

### Comparing `evadb-0.2.7/evadb/server/interpreter.py` & `evadb-0.2.8/evadb/server/interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,15 +15,15 @@
 import asyncio
 import os
 import sys
 from asyncio import StreamReader, StreamWriter
 from collections import deque
 from typing import Dict
 
-from evadb.interfaces.relational.db import EVADBConnection
+from evadb.interfaces.relational.db import EvaDBConnection
 from evadb.utils.logging_manager import logger
 
 # version.py defines the VERSION and VERSION_SHORT variables
 VERSION_DICT: Dict[str, str] = {}
 
 current_file_dir = os.path.dirname(__file__)
 current_file_parent_dir = os.path.join(current_file_dir, os.pardir)
@@ -52,24 +52,24 @@
     return stream_reader
 
 
 async def read_from_client_and_send_to_server(
     stdin_reader: StreamReader, writer: StreamWriter, server_reader: StreamReader
 ):
     VERSION = VERSION_DICT["VERSION"]
-    intro = f"eva (v{VERSION})\nType 'EXIT;' to exit the client \n"
+    intro = f"evadb (v{VERSION})\nType 'EXIT;' to exit the client \n"
     print(intro, flush=True)
 
-    prompt = "eva=#"
+    prompt = "evadb=#"
 
-    # The EVADatabase object is not passed from the command line client.
+    # The EvaDBDatabase object is not passed from the command line client.
     # The concept is to always send a SQL query to the server, which is responsible for
     # executing it and returning the results. However, in the Pythonic interface, we
-    # adopt a serverless approach and don't rely on the EVADatabase object.
-    connection = EVADBConnection(None, server_reader, writer)
+    # adopt a serverless approach and don't rely on the EvaDBDatabase object.
+    connection = EvaDBConnection(None, server_reader, writer)
     cursor = connection.cursor()
 
     while True:
         sys.stdout.write(prompt)
         sys.stdout.flush()
         query = await read_line(stdin_reader)
         logger.debug("Query: --|" + query + "|--")
```

### Comparing `evadb-0.2.7/evadb/server/server.py` & `evadb-0.2.8/evadb/server/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,55 +12,55 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import asyncio
 import string
 from asyncio import StreamReader, StreamWriter
 
-from evadb.database import init_eva_db_instance
+from evadb.database import init_evadb_instance
 from evadb.udfs.udf_bootstrap_queries import init_builtin_udfs
 from evadb.utils.logging_manager import logger
 
 
 class EvaServer:
     """
     Receives messages and offloads them to another task for processing them.
     """
 
     def __init__(self):
         self._server = None
         self._clients = {}  # client -> (reader, writer)
         self._evadb = None
 
-    async def start_eva_server(
+    async def start_evadb_server(
         self, db_dir: str, host: string, port: int, custom_db_uri: str = None
     ):
         """
         Start the server
         Server objects are asynchronous context managers.
 
         hostname: hostname of the server
         port: port of the server
         """
-        print(f"EVA server started at host {host} and port {port}")
-        self._evadb = init_eva_db_instance(db_dir, host, port, custom_db_uri)
+        print(f"EvaDB server started at host {host} and port {port}")
+        self._evadb = init_evadb_instance(db_dir, host, port, custom_db_uri)
 
         self._server = await asyncio.start_server(self.accept_client, host, port)
 
         # load built-in udfs
         mode = self._evadb.config.get_value("core", "mode")
         init_builtin_udfs(self._evadb, mode=mode)
 
         async with self._server:
             await self._server.serve_forever()
 
-        logger.warn("EVA server stopped")
+        logger.warn("EvaDB server stopped")
 
-    async def stop_eva_server(self):
-        logger.warn("EVA server stopped")
+    async def stop_evadb_server(self):
+        logger.warn("EvaDB server stopped")
         if self._server is not None:
             await self._server.close()
 
     async def accept_client(
         self, client_reader: StreamReader, client_writer: StreamWriter
     ):
         task = asyncio.Task(self.handle_client(client_reader, client_writer))
```

### Comparing `evadb-0.2.7/evadb/storage/__init__.py` & `evadb-0.2.8/evadb/executor/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-storage subdirectory
-"""
+"""executor subdirectory"""
```

### Comparing `evadb-0.2.7/evadb/storage/abstract_media_storage_engine.py` & `evadb-0.2.8/evadb/storage/abstract_media_storage_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,24 +16,24 @@
 import re
 import shutil
 from pathlib import Path
 
 import pandas as pd
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.models.storage.batch import Batch
 from evadb.parser.table_ref import TableInfo
 from evadb.storage.abstract_storage_engine import AbstractStorageEngine
 from evadb.storage.sqlite_storage_engine import SQLStorageEngine
 from evadb.utils.logging_manager import logger
 
 
 class AbstractMediaStorageEngine(AbstractStorageEngine):
-    def __init__(self, db: EVADatabase):
+    def __init__(self, db: EvaDBDatabase):
         super().__init__(db)
         self._rdb_handler: SQLStorageEngine = SQLStorageEngine(db)
 
     def _get_metadata_table(self, table: TableCatalogEntry):
         return self.db.catalog().get_multimedia_metadata_table_catalog_entry(table)
 
     def _create_metadata_table(self, table: TableCatalogEntry):
```

### Comparing `evadb-0.2.7/evadb/storage/abstract_storage_engine.py` & `evadb-0.2.8/evadb/storage/abstract_storage_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,28 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from abc import ABCMeta, abstractmethod
 from typing import Iterator
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.expression.abstract_expression import AbstractExpression
 from evadb.models.storage.batch import Batch
 
 
 class AbstractStorageEngine(metaclass=ABCMeta):
     """
     Abstract class for defining storage engine. Storage engine is responsible
     for handling data storage and retrieval tasks.
     This contains a minimal set of APIs that each engine should implement
 
     """
 
-    def __init__(self, db: EVADatabase):
+    def __init__(self, db: EvaDBDatabase):
         self.db = db
 
     @abstractmethod
     def create(self, table: TableCatalogEntry):
         """Interface that implements all the necessary task required for
             creating the basic unit of storage(table or dataframe)
```

### Comparing `evadb-0.2.7/evadb/storage/document_storage_engine.py` & `evadb-0.2.8/evadb/storage/document_storage_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,22 +12,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import Iterator
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.models.storage.batch import Batch
 from evadb.readers.document.document_reader import DocumentReader
 from evadb.storage.abstract_media_storage_engine import AbstractMediaStorageEngine
 
 
 class DocumentStorageEngine(AbstractMediaStorageEngine):
-    def __init__(self, db: EVADatabase):
+    def __init__(self, db: EvaDBDatabase):
         super().__init__(db)
 
     def read(self, table: TableCatalogEntry) -> Iterator[Batch]:
         for doc_files in self._rdb_handler.read(self._get_metadata_table(table), 12):
             for _, (row_id, file_name) in doc_files.iterrows():
                 system_file_name = self._xform_file_url_to_file_name(file_name)
                 doc_file = Path(table.file_url) / system_file_name
```

### Comparing `evadb-0.2.7/evadb/storage/image_storage_engine.py` & `evadb-0.2.8/evadb/storage/pdf_storage_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,28 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import Iterator
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.models.storage.batch import Batch
-from evadb.readers.image.opencv_image_reader import CVImageReader
+from evadb.readers.pdf_reader import PDFReader
 from evadb.storage.abstract_media_storage_engine import AbstractMediaStorageEngine
 
 
-class ImageStorageEngine(AbstractMediaStorageEngine):
-    def __init__(self, db: EVADatabase):
+class PDFStorageEngine(AbstractMediaStorageEngine):
+    def __init__(self, db: EvaDBDatabase):
         super().__init__(db)
 
     def read(self, table: TableCatalogEntry) -> Iterator[Batch]:
         for image_files in self._rdb_handler.read(self._get_metadata_table(table), 12):
             for _, (row_id, file_name) in image_files.iterrows():
                 system_file_name = self._xform_file_url_to_file_name(file_name)
                 image_file = Path(table.file_url) / system_file_name
                 # setting batch_mem_size = 1, we need fix it
-                reader = CVImageReader(str(image_file), batch_mem_size=1)
+                reader = PDFReader(str(image_file), batch_mem_size=1)
                 for batch in reader.read():
                     batch.frames[table.columns[0].name] = row_id
                     batch.frames[table.columns[1].name] = str(file_name)
                     yield batch
```

### Comparing `evadb-0.2.7/evadb/storage/pdf_storage_engine.py` & `evadb-0.2.8/evadb/storage/image_storage_engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,28 +12,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from pathlib import Path
 from typing import Iterator
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.models.storage.batch import Batch
-from evadb.readers.pdf_reader import PDFReader
+from evadb.readers.image.opencv_image_reader import CVImageReader
 from evadb.storage.abstract_media_storage_engine import AbstractMediaStorageEngine
 
 
-class PDFStorageEngine(AbstractMediaStorageEngine):
-    def __init__(self, db: EVADatabase):
+class ImageStorageEngine(AbstractMediaStorageEngine):
+    def __init__(self, db: EvaDBDatabase):
         super().__init__(db)
 
     def read(self, table: TableCatalogEntry) -> Iterator[Batch]:
         for image_files in self._rdb_handler.read(self._get_metadata_table(table), 12):
             for _, (row_id, file_name) in image_files.iterrows():
                 system_file_name = self._xform_file_url_to_file_name(file_name)
                 image_file = Path(table.file_url) / system_file_name
                 # setting batch_mem_size = 1, we need fix it
-                reader = PDFReader(str(image_file), batch_mem_size=1)
+                reader = CVImageReader(str(image_file), batch_mem_size=1)
                 for batch in reader.read():
                     batch.frames[table.columns[0].name] = row_id
                     batch.frames[table.columns[1].name] = str(file_name)
                     yield batch
```

### Comparing `evadb-0.2.7/evadb/storage/sqlite_storage_engine.py` & `evadb-0.2.8/evadb/storage/sqlite_storage_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,27 +21,27 @@
 
 from evadb.catalog.catalog_type import ColumnType
 from evadb.catalog.models.base_model import BaseModel
 from evadb.catalog.models.column_catalog import ColumnCatalogEntry
 from evadb.catalog.models.table_catalog import TableCatalogEntry
 from evadb.catalog.schema_utils import SchemaUtils
 from evadb.catalog.sql_config import IDENTIFIER_COLUMN
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.models.storage.batch import Batch
 from evadb.parser.table_ref import TableInfo
 from evadb.storage.abstract_storage_engine import AbstractStorageEngine
 from evadb.utils.generic_utils import PickleSerializer, get_size
 from evadb.utils.logging_manager import logger
 
 # Leveraging Dynamic schema in SQLAlchemy
 # https://sparrigan.github.io/sql/sqla/2016/01/03/dynamic-tables.html
 
 
 class SQLStorageEngine(AbstractStorageEngine):
-    def __init__(self, db: EVADatabase):
+    def __init__(self, db: EvaDBDatabase):
         """
         Grab the existing sql session
         """
         super().__init__(db)
         self._sql_session = db.catalog().sql_config.session
         self._sql_engine = db.catalog().sql_config.engine
         self._serializer = PickleSerializer
@@ -96,15 +96,15 @@
         # the sqlalchemy engine.
         table_columns = [col for col in table.columns if col.name != IDENTIFIER_COLUMN]
         sqlalchemy_schema = SchemaUtils.xform_to_sqlalchemy_schema(table_columns)
         attr_dict.update(sqlalchemy_schema)
 
         insp = inspect(self._sql_engine)
         if insp.has_table(table.name):
-            logger.warning("Trying to create an exsiting table {table.name}")
+            logger.warning("Table {table.name} already exists")
             return BaseModel.metadata.tables[table.name]
 
         # dynamic schema generation
         # https://sparrigan.github.io/sql/sqla/2016/01/03/dynamic-tables.html
         new_table = type(
             f"__placeholder_class_name__{table.name}", (BaseModel,), attr_dict
         )()
```

### Comparing `evadb-0.2.7/evadb/storage/storage_engine.py` & `evadb-0.2.8/evadb/storage/storage_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from evadb.catalog.catalog_type import TableType
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.storage.abstract_storage_engine import AbstractStorageEngine
 from evadb.storage.document_storage_engine import DocumentStorageEngine
 from evadb.storage.image_storage_engine import ImageStorageEngine
 from evadb.storage.pdf_storage_engine import PDFStorageEngine
 from evadb.storage.sqlite_storage_engine import SQLStorageEngine
 from evadb.storage.video_storage_engine import DecordStorageEngine
 
 
 class StorageEngine:
     storages = None
 
     @classmethod
-    def _lazy_initialize_storages(cls, db: EVADatabase):
+    def _lazy_initialize_storages(cls, db: EvaDBDatabase):
         if not cls.storages:
             cls.storages = {
                 TableType.STRUCTURED_DATA: SQLStorageEngine,
                 TableType.VIDEO_DATA: DecordStorageEngine,
                 TableType.IMAGE_DATA: ImageStorageEngine,
                 TableType.DOCUMENT_DATA: DocumentStorageEngine,
                 TableType.PDF_DATA: PDFStorageEngine,
             }
 
     @classmethod
     def factory(
-        cls, db: EVADatabase, table: TableCatalogEntry
+        cls, db: EvaDBDatabase, table: TableCatalogEntry
     ) -> AbstractStorageEngine:
         cls._lazy_initialize_storages(db)
         if table is None:
             raise ValueError("Expected TableCatalogEntry, got None")
         if table.table_type in cls.storages:
             return cls.storages[table.table_type](db)
```

### Comparing `evadb-0.2.7/evadb/storage/video_storage_engine.py` & `evadb-0.2.8/evadb/storage/video_storage_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,23 +13,23 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import sys
 from pathlib import Path
 from typing import Iterator
 
 from evadb.catalog.models.table_catalog import TableCatalogEntry
-from evadb.database import EVADatabase
+from evadb.database import EvaDBDatabase
 from evadb.expression.abstract_expression import AbstractExpression
 from evadb.models.storage.batch import Batch
 from evadb.readers.decord_reader import DecordReader
 from evadb.storage.abstract_media_storage_engine import AbstractMediaStorageEngine
 
 
 class DecordStorageEngine(AbstractMediaStorageEngine):
-    def __init__(self, db: EVADatabase):
+    def __init__(self, db: EvaDBDatabase):
         super().__init__(db)
 
     def read(
         self,
         table: TableCatalogEntry,
         batch_mem_size: int,
         predicate: AbstractExpression = None,
```

### Comparing `evadb-0.2.7/evadb/third_party/__init__.py` & `evadb-0.2.8/evadb/third_party/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/huggingface/__init__.py` & `evadb-0.2.8/evadb/third_party/huggingface/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/huggingface/binder.py` & `evadb-0.2.8/evadb/third_party/huggingface/binder.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/huggingface/create.py` & `evadb-0.2.8/evadb/third_party/huggingface/create.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -108,15 +108,15 @@
     """
     Infer the name and type for each output of the HuggingFace UDF
     """
     assert "task" in pipeline_args, "Task Not Found In Model Definition"
     task = pipeline_args["task"]
     assert (
         task in INPUT_TYPE_FOR_SUPPORTED_TASKS
-    ), f"Task {task} not supported in EVA currently"
+    ), f"Task {task} not supported in EvaDB currently"
 
     # Construct the pipeline
     pipe = pipeline(**pipeline_args)
 
     # Run the pipeline through a dummy input to get a sample output
     input_type = INPUT_TYPE_FOR_SUPPORTED_TASKS[task]
     model_input = gen_sample_input(input_type)
```

### Comparing `evadb-0.2.7/evadb/third_party/huggingface/model.py` & `evadb-0.2.8/evadb/third_party/huggingface/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,18 +15,18 @@
 from typing import Any
 
 import decord
 import numpy as np
 from PIL import Image
 
 from evadb.udfs.abstract.hf_abstract_udf import AbstractHFUdf
-from evadb.utils.generic_utils import EVAEnum
+from evadb.utils.generic_utils import EvaDBEnum
 
 
-class HFInputTypes(EVAEnum):
+class HFInputTypes(EvaDBEnum):
     TEXT  # noqa: F821
     IMAGE  # noqa: F821
     AUDIO  # noqa: F821
     VIDEO  # noqa: F821
     MULTIMODAL_TEXT_IMAGE  # noqa: F821
```

### Comparing `evadb-0.2.7/evadb/third_party/vector_stores/__init__.py` & `evadb-0.2.8/evadb/third_party/vector_stores/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/vector_stores/faiss.py` & `evadb-0.2.8/evadb/third_party/vector_stores/faiss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/vector_stores/qdrant.py` & `evadb-0.2.8/evadb/third_party/vector_stores/qdrant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/vector_stores/types.py` & `evadb-0.2.8/evadb/third_party/vector_stores/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/third_party/vector_stores/utils.py` & `evadb-0.2.8/evadb/third_party/vector_stores/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/__init__.py` & `evadb-0.2.8/evadb/udfs/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/abstract/__init__.py` & `evadb-0.2.8/evadb/udfs/abstract/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/abstract/abstract_udf.py` & `evadb-0.2.8/evadb/udfs/abstract/abstract_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,15 +19,15 @@
 from numpy.typing import ArrayLike
 
 InputType = Union[pd.DataFrame, ArrayLike]
 
 
 class AbstractUDF(metaclass=ABCMeta):
     """
-    Abstract class for UDFs. All the UDFs in EVA will inherit from this.
+    Abstract class for UDFs. All the UDFs in EvaDB will inherit from this.
 
     Load and initialize the machine learning model in the __init__.
 
     """
 
     def __init__(self, *args, **kwargs):
         self.setup(*args, **kwargs)
```

### Comparing `evadb-0.2.7/evadb/udfs/abstract/hf_abstract_udf.py` & `evadb-0.2.8/evadb/udfs/abstract/hf_abstract_udf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -23,15 +23,15 @@
 
 
 class AbstractHFUdf(AbstractUDF, GPUCompatible):
     """
     An abstract class for all HuggingFace models.
 
     This is implemented using the pipeline API from HuggingFace. pipeline is an
-    easy way to use a huggingface model for inference. In EVA, we require users
+    easy way to use a huggingface model for inference. In EvaDB, we require users
     to mention the task they want to perform for simplicity. A HuggingFace task
     is different from a model(pytorch). There are a large number of models on HuggingFace
     hub that can be used for a particular task. The user can specify the model or a default
     model will be used.
 
     Refer to https://huggingface.co/transformers/main_classes/pipelines.html for more details
     on pipelines.
@@ -61,21 +61,21 @@
         Arguments that will be passed to the pipeline by default.
         User provided arguments override the default arguments
         """
         return {}
 
     def input_formatter(self, inputs: Any):
         """
-        Function that formats input from EVA format to HuggingFace format for that particular HF model
+        Function that formats input from EvaDB format to HuggingFace format for that particular HF model
         """
         return inputs
 
     def output_formatter(self, outputs: Any):
         """
-        Function that formats output from HuggingFace format to EVA format (pandas dataframe)
+        Function that formats output from HuggingFace format to EvaDB format (pandas dataframe)
         The output can be in various formats, depending on the model. For example:
             {'text' : 'transcript from video'}
             [[{'score': 0.25, 'label': 'bridge'}, {'score': 0.50, 'label': 'car'}]]
         """
         if isinstance(outputs, dict):
             return pd.DataFrame(outputs, index=[0])
         # PERF: Can improve performance by avoiding redundant list creation
@@ -91,13 +91,13 @@
 
         result_df = pd.DataFrame(result_list)
         return result_df
 
     def forward(self, inputs, *args, **kwargs) -> pd.DataFrame:
         hf_input = self.input_formatter(inputs)
         hf_output = self.hf_udf_obj(hf_input, *args, **kwargs)
-        eva_output = self.output_formatter(hf_output)
-        return eva_output
+        evadb_output = self.output_formatter(hf_output)
+        return evadb_output
 
     def to_device(self, device: str) -> GPUCompatible:
         self.hf_udf_obj = pipeline(**self.pipeline_args, device=device)
         return self
```

### Comparing `evadb-0.2.7/evadb/udfs/abstract/pytorch_abstract_udf.py` & `evadb-0.2.8/evadb/udfs/abstract/pytorch_abstract_udf.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -92,15 +92,15 @@
         Required to make class a member of GPUCompatible Protocol.
         """
         return self.to(torch.device("cuda:{}".format(device)))
 
 
 class PytorchAbstractTransformationUDF(AbstractTransformationUDF, Compose):
     """
-    Use PyTorch torchvision transforms as EVA transforms.
+    Use PyTorch torchvision transforms as EvaDB transforms.
     """
 
     def __init__(self, transforms):
         Compose.__init__(self, transforms)
 
     def transform(self, frames: ArrayLike) -> ArrayLike:
         return Compose.__call__(self, frames)
```

### Comparing `evadb-0.2.7/evadb/udfs/abstract/tracker_abstract_udf.py` & `evadb-0.2.8/evadb/udfs/abstract/tracker_abstract_udf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,17 +19,17 @@
 
 from evadb.catalog.catalog_type import NdArrayType
 from evadb.udfs.abstract.abstract_udf import AbstractUDF
 from evadb.udfs.decorators.decorators import forward, setup
 from evadb.udfs.decorators.io_descriptors.data_types import PandasDataframe
 
 
-class EVATrackerAbstractUDF(AbstractUDF):
+class EvaDBTrackerAbstractUDF(AbstractUDF):
     """
-    An abstract class for all EVA object trackers.
+    An abstract class for all EvaDB object trackers.
     """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @setup(cacheable=False, udf_type="object_tracker", batchable=False)
     def setup(self, *args, **kwargs):
```

### Comparing `evadb-0.2.7/evadb/udfs/asl_action_recognition.py` & `evadb-0.2.8/evadb/udfs/asl_action_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/chatgpt.py` & `evadb-0.2.8/evadb/udfs/chatgpt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 
 import os
 
 import openai
 import pandas as pd
+from retry import retry
 
 from evadb.catalog.catalog_type import NdArrayType
 from evadb.configuration.configuration_manager import ConfigurationManager
 from evadb.udfs.abstract.abstract_udf import AbstractUDF
 from evadb.udfs.decorators.decorators import forward, setup
 from evadb.udfs.decorators.io_descriptors.data_types import PandasDataframe
 
@@ -31,36 +32,31 @@
     "gpt-4-32k",
     "gpt-4-32k-0314",
     "gpt-3.5-turbo",
     "gpt-3.5-turbo-0301",
 ]
 
 
+@retry(tries=6, delay=10)
+def completion_with_backoff(**kwargs):
+    return openai.ChatCompletion.create(**kwargs)
+
+
 class ChatGPT(AbstractUDF):
     @property
     def name(self) -> str:
         return "ChatGPT"
 
     @setup(cacheable=False, udf_type="chat-completion", batchable=True)
     def setup(
         self,
         model="gpt-3.5-turbo",
         temperature: float = 0,
     ) -> None:
-        # Try Configuration Manager
-        openai.api_key = ConfigurationManager().get_value("third_party", "OPENAI_KEY")
-        # If not found, try OS Environment Variable
-        if len(openai.api_key) == 0:
-            openai.api_key = os.environ.get("OPENAI_KEY", "")
-        assert (
-            len(openai.api_key) != 0
-        ), "Please set your OpenAI API key in evadb.yml file (third_party, open_api_key) or environment variable (OPENAI_KEY)"
-
         assert model in _VALID_CHAT_COMPLETION_MODEL, f"Unsupported ChatGPT {model}"
-
         self.model = model
         self.temperature = temperature
 
     @forward(
         input_signatures=[
             PandasDataframe(
                 columns=["prompt", "query"],
@@ -78,20 +74,28 @@
                     NdArrayType.STR,
                 ],
                 column_shapes=[(1,)],
             )
         ],
     )
     def forward(self, text_df):
+        # Register API key, try configuration manager first
+        openai.api_key = ConfigurationManager().get_value("third_party", "OPENAI_KEY")
+        # If not found, try OS Environment Variable
+        if len(openai.api_key) == 0:
+            openai.api_key = os.environ.get("OPENAI_KEY", "")
+        assert (
+            len(openai.api_key) != 0
+        ), "Please set your OpenAI API key in evadb.yml file (third_party, open_api_key) or environment variable (OPENAI_KEY)"
+
         prompts = text_df[text_df.columns[0]]
         queries = text_df[text_df.columns[1]]
 
         # openai api currently supports answers to a single prompt only
-        # so this udf is designed such that
-
+        # so this udf is designed for that
         results = []
 
         for prompt, query in zip(prompts, queries):
             if prompt != "None":
                 query = prompt + ": " + query
 
             params = {
@@ -100,13 +104,14 @@
                 "messages": [
                     {
                         "role": "user",
                         "content": query,
                     }
                 ],
             }
-            response = openai.ChatCompletion.create(**params)
+
+            response = completion_with_backoff(**params)
             results.append(response.choices[0].message.content)
 
         df = pd.DataFrame({"response": results})
 
         return df
```

### Comparing `evadb-0.2.7/evadb/udfs/decorators/__init__.py` & `evadb-0.2.8/test/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/decorators/decorators.py` & `evadb-0.2.8/evadb/udfs/decorators/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/decorators/io_descriptors/__init__.py` & `evadb-0.2.8/test/benchmark_tests/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/decorators/io_descriptors/abstract_types.py` & `evadb-0.2.8/evadb/udfs/decorators/io_descriptors/abstract_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/decorators/io_descriptors/data_types.py` & `evadb-0.2.8/evadb/udfs/decorators/io_descriptors/data_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/decorators/utils.py` & `evadb-0.2.8/evadb/udfs/decorators/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/emotion_detector.py` & `evadb-0.2.8/evadb/udfs/emotion_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/face_detector.py` & `evadb-0.2.8/evadb/udfs/face_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/fastrcnn_object_detector.py` & `evadb-0.2.8/evadb/udfs/fastrcnn_object_detector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/feature_extractor.py` & `evadb-0.2.8/evadb/udfs/feature_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/gpu_compatible.py` & `evadb-0.2.8/evadb/udfs/gpu_compatible.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/mnist_image_classifier.py` & `evadb-0.2.8/evadb/udfs/mnist_image_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/mvit_action_recognition.py` & `evadb-0.2.8/evadb/udfs/mvit_action_recognition.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/__init__.py` & `evadb-0.2.8/evadb/udfs/ndarray/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/annotate.py` & `evadb-0.2.8/evadb/udfs/ndarray/annotate.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/array_count.py` & `evadb-0.2.8/evadb/udfs/ndarray/array_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/crop.py` & `evadb-0.2.8/evadb/udfs/ndarray/crop.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/fuzzy_join.py` & `evadb-0.2.8/evadb/udfs/ndarray/fuzzy_join.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/gaussian_blur.py` & `evadb-0.2.8/evadb/udfs/ndarray/gaussian_blur.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/horizontal_flip.py` & `evadb-0.2.8/evadb/udfs/ndarray/horizontal_flip.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/open.py` & `evadb-0.2.8/evadb/udfs/ndarray/open.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/similarity.py` & `evadb-0.2.8/evadb/udfs/ndarray/similarity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/to_grayscale.py` & `evadb-0.2.8/evadb/udfs/ndarray/to_grayscale.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ndarray/vertical_flip.py` & `evadb-0.2.8/evadb/udfs/ndarray/vertical_flip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/ocr_extractor.py` & `evadb-0.2.8/evadb/udfs/ocr_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/saliency_feature_extractor.py` & `evadb-0.2.8/evadb/udfs/saliency_feature_extractor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -57,22 +57,22 @@
         ],
     )
     def forward(self, df: pd.DataFrame) -> pd.DataFrame:
         def _forward(row: pd.Series) -> np.ndarray:
             rgb_img = row[0]
 
             composed = Compose([Resize((224, 224)), ToTensor()])
-            transfromed_img = composed(Image.fromarray(rgb_img[:, :, ::-1])).unsqueeze(
+            transformed_img = composed(Image.fromarray(rgb_img[:, :, ::-1])).unsqueeze(
                 0
             )
-            transfromed_img.requires_grad_()
-            outputs = self.model(transfromed_img)
+            transformed_img.requires_grad_()
+            outputs = self.model(transformed_img)
             score_max_index = outputs.argmax()
             score_max = outputs[0, score_max_index]
             score_max.backward()
-            saliency, _ = torch.max(transfromed_img.grad.data.abs(), dim=1)
+            saliency, _ = torch.max(transformed_img.grad.data.abs(), dim=1)
 
             return saliency
 
         ret = pd.DataFrame()
         ret["saliency"] = df.apply(_forward, axis=1)
         return ret
```

### Comparing `evadb-0.2.7/evadb/udfs/sentence_transformer_feature_extractor.py` & `evadb-0.2.8/evadb/udfs/sentence_transformer_feature_extractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
-#
-# Licensed under the Apache License, Version 2.0 (the "License");
-# you may not use this file except in compliance with the License.
-# You may obtain a copy of the License at
-#
-#     http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing, software
-# distributed under the License is distributed on an "AS IS" BASIS,
-# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-# See the License for the specific language governing permissions and
-# limitations under the License.
-
-# coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -40,15 +25,15 @@
 
 class SentenceTransformerFeatureExtractor(AbstractUDF, GPUCompatible):
     @setup(cacheable=False, udf_type="FeatureExtraction", batchable=False)
     def setup(self):
         self.model = SentenceTransformer("all-MiniLM-L6-v2")
 
     def to_device(self, device: str) -> GPUCompatible:
-        self.modle = self.model.to(device)
+        self.model = self.model.to(device)
         return self
 
     @property
     def name(self) -> str:
         return "SentenceTransformerFeatureExtractor"
 
     @forward(
```

### Comparing `evadb-0.2.7/evadb/udfs/sift_feature_extractor.py` & `evadb-0.2.8/evadb/udfs/sift_feature_extractor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/trackers/__init__.py` & `evadb-0.2.8/evadb/udfs/trackers/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/trackers/nor_fair.py` & `evadb-0.2.8/evadb/udfs/trackers/nor_fair.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,21 +11,21 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import numpy as np
 from norfair import Detection, Tracker
 
-from evadb.udfs.abstract.tracker_abstract_udf import EVATrackerAbstractUDF
+from evadb.udfs.abstract.tracker_abstract_udf import EvaDBTrackerAbstractUDF
 from evadb.utils.math_utils import get_centroid
 
 DISTANCE_THRESHOLD_CENTROID: int = 30
 
 
-class NorFairTracker(EVATrackerAbstractUDF):
+class NorFairTracker(EvaDBTrackerAbstractUDF):
     @property
     def name(self) -> str:
         return "NorFairTracker"
 
     def setup(self, distance_threshold=DISTANCE_THRESHOLD_CENTROID) -> None:
         # https://github.com/tryolabs/norfair/blob/74b11edde83941dd6e32bcccd5fa849e16bf8564/norfair/tracker.py#L18
         self.tracker = Tracker(
```

### Comparing `evadb-0.2.7/evadb/udfs/tutorials/__init__.py` & `evadb-0.2.8/evadb/udfs/tutorials/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/udfs/udf_bootstrap_queries.py` & `evadb-0.2.8/evadb/udfs/udf_bootstrap_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,183 +1,204 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from evadb.configuration.constants import EVA_INSTALLATION_DIR
-from evadb.database import EVADatabase
+from evadb.configuration.constants import EvaDB_INSTALLATION_DIR
+from evadb.database import EvaDBDatabase
 from evadb.server.command_handler import execute_query_fetch_all
 
 NDARRAY_DIR = "ndarray"
 TUTORIALS_DIR = "tutorials"
 
 DummyObjectDetector_udf_query = """CREATE UDF IF NOT EXISTS DummyObjectDetector
                   INPUT  (Frame_Array NDARRAY INT8(3, ANYDIM, ANYDIM))
                   OUTPUT (label NDARRAY STR(1))
                   TYPE  Classification
                   IMPL  '{}/../test/util.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 DummyMultiObjectDetector_udf_query = """CREATE UDF
                   IF NOT EXISTS  DummyMultiObjectDetector
                   INPUT  (Frame_Array NDARRAY INT8(3, ANYDIM, ANYDIM))
                   OUTPUT (labels NDARRAY STR(2))
                   TYPE  Classification
                   IMPL  '{}/../test/util.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 DummyFeatureExtractor_udf_query = """CREATE UDF
                   IF NOT EXISTS DummyFeatureExtractor
                   INPUT (Frame_Array NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (features NDARRAY FLOAT32(1, ANYDIM))
                   TYPE Classification
                   IMPL '{}/../test/util.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
+)
+
+fuzzy_udf_query = """CREATE UDF IF NOT EXISTS FuzzDistance
+                    INPUT (Input_Array1 NDARRAY ANYTYPE, Input_Array2 NDARRAY ANYTYPE)
+                    OUTPUT (distance FLOAT(32, 7))
+                    TYPE NdarrayUDF
+                    IMPL "{}/udfs/{}/fuzzy_join.py";
+        """.format(
+    EvaDB_INSTALLATION_DIR, NDARRAY_DIR
 )
 
 ArrayCount_udf_query = """CREATE UDF
             IF NOT EXISTS  ArrayCount
             INPUT (Input_Array NDARRAY ANYTYPE, Search_Key ANYTYPE)
             OUTPUT (key_count INTEGER)
             TYPE NdarrayUDF
             IMPL "{}/udfs/{}/array_count.py";
         """.format(
-    EVA_INSTALLATION_DIR, NDARRAY_DIR
+    EvaDB_INSTALLATION_DIR, NDARRAY_DIR
 )
 
 Crop_udf_query = """CREATE UDF IF NOT EXISTS Crop
                 INPUT  (Frame_Array NDARRAY UINT8(3, ANYDIM, ANYDIM),
                         bboxes NDARRAY FLOAT32(ANYDIM, 4))
                 OUTPUT (Cropped_Frame_Array NDARRAY UINT8(3, ANYDIM, ANYDIM))
                 TYPE  NdarrayUDF
                 IMPL  "{}/udfs/{}/crop.py";
         """.format(
-    EVA_INSTALLATION_DIR, NDARRAY_DIR
+    EvaDB_INSTALLATION_DIR, NDARRAY_DIR
 )
 
 Open_udf_query = """CREATE UDF IF NOT EXISTS Open
                 INPUT (img_path TEXT(1000))
                 OUTPUT (data NDARRAY UINT8(3, ANYDIM, ANYDIM))
                 TYPE NdarrayUDF
                 IMPL "{}/udfs/{}/open.py";
         """.format(
-    EVA_INSTALLATION_DIR, NDARRAY_DIR
+    EvaDB_INSTALLATION_DIR, NDARRAY_DIR
 )
 
 Similarity_udf_query = """CREATE UDF IF NOT EXISTS Similarity
                     INPUT (Frame_Array_Open NDARRAY UINT8(3, ANYDIM, ANYDIM),
                            Frame_Array_Base NDARRAY UINT8(3, ANYDIM, ANYDIM),
                            Feature_Extractor_Name TEXT(100))
                     OUTPUT (distance FLOAT(32, 7))
                     TYPE NdarrayUDF
                     IMPL "{}/udfs/{}/similarity.py";
         """.format(
-    EVA_INSTALLATION_DIR, NDARRAY_DIR
+    EvaDB_INSTALLATION_DIR, NDARRAY_DIR
 )
 
 Unnest_udf_query = """CREATE UDF IF NOT EXISTS Unnest
                 INPUT  (inp NDARRAY ANYTYPE)
                 OUTPUT (out ANYTYPE)
                 TYPE  NdarrayUDF
                 IMPL  "{}/udfs/{}/unnest.py";
         """.format(
-    EVA_INSTALLATION_DIR, NDARRAY_DIR
+    EvaDB_INSTALLATION_DIR, NDARRAY_DIR
 )
 
 Fastrcnn_udf_query = """CREATE UDF IF NOT EXISTS FastRCNNObjectDetector
       INPUT  (Frame_Array NDARRAY UINT8(3, ANYDIM, ANYDIM))
       OUTPUT (labels NDARRAY STR(ANYDIM), bboxes NDARRAY FLOAT32(ANYDIM, 4),
                 scores NDARRAY FLOAT32(ANYDIM))
       TYPE  Classification
       IMPL  '{}/udfs/fastrcnn_object_detector.py';
       """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 Yolo_udf_query = """CREATE UDF IF NOT EXISTS Yolo
       TYPE  ultralytics
       'model' 'yolov8m.pt';
       """
 
 ocr_udf_query = """CREATE UDF IF NOT EXISTS OCRExtractor
       INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
       OUTPUT (labels NDARRAY STR(10), bboxes NDARRAY FLOAT32(ANYDIM, 4),
                 scores NDARRAY FLOAT32(ANYDIM))
       TYPE  OCRExtraction
       IMPL  '{}/udfs/ocr_extractor.py';
       """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 face_detection_udf_query = """CREATE UDF IF NOT EXISTS FaceDetector
                   INPUT  (frame NDARRAY UINT8(3, ANYDIM, ANYDIM))
                   OUTPUT (bboxes NDARRAY FLOAT32(ANYDIM, 4),
                           scores NDARRAY FLOAT32(ANYDIM))
                   TYPE  FaceDetection
                   IMPL  '{}/udfs/face_detector.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 Mvit_udf_query = """CREATE UDF IF NOT EXISTS MVITActionRecognition
         INPUT  (Frame_Array NDARRAY UINT8(3, 16, 224, 224))
         OUTPUT (labels NDARRAY STR(ANYDIM))
         TYPE  Classification
         IMPL  '{}/udfs/mvit_action_recognition.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 Asl_udf_query = """CREATE UDF IF NOT EXISTS ASLActionRecognition
         INPUT  (Frame_Array NDARRAY UINT8(3, 16, 224, 224))
         OUTPUT (labels NDARRAY STR(ANYDIM))
         TYPE  Classification
         IMPL  '{}/udfs/asl_action_recognition.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 norfair_obj_tracker_query = """CREATE UDF IF NOT EXISTS NorFairTracker
                   IMPL  '{}/udfs/trackers/nor_fair.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
 )
 
 Sift_udf_query = """CREATE UDF IF NOT EXISTS SiftFeatureExtractor
         IMPL  '{}/udfs/sift_feature_extractor.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
+)
+
+Text_feat_udf_query = """CREATE UDF IF NOT EXISTS SentenceFeatureExtractor
+        IMPL  '{}/udfs/sentence_feature_extractor.py';
+        """.format(
+    EvaDB_INSTALLATION_DIR
 )
 
 mnistcnn_udf_query = """CREATE UDF IF NOT EXISTS MnistImageClassifier
         INPUT  (data NDARRAY (3, 28, 28))
         OUTPUT (label TEXT(2))
         TYPE  Classification
         IMPL  '{}/udfs/mnist_image_classifier.py';
         """.format(
-    EVA_INSTALLATION_DIR
+    EvaDB_INSTALLATION_DIR
+)
+
+chatgpt_udf_query = """CREATE UDF IF NOT EXISTS ChatGPT
+        IMPL '{}/udfs/chatgpt.py';
+        """.format(
+    EvaDB_INSTALLATION_DIR
 )
 
 
-def init_builtin_udfs(db: EVADatabase, mode: str = "debug") -> None:
+def init_builtin_udfs(db: EvaDBDatabase, mode: str = "debug") -> None:
     """Load the built-in UDFs into the system during system bootstrapping.
 
     The function loads a set of pre-defined UDF queries based on the `mode` argument.
     In 'debug' mode, the function loads debug UDFs along with release UDFs.
     In 'release' mode, only release UDFs are loaded. In addition, in 'debug' mode,
     the function loads a smaller model to accelerate the test suite time.
 
@@ -191,14 +212,15 @@
         Fastrcnn_udf_query,
         ArrayCount_udf_query,
         Crop_udf_query,
         Open_udf_query,
         Similarity_udf_query,
         norfair_obj_tracker_query,
         mnistcnn_udf_query,
+        chatgpt_udf_query,
         # Disabled because required packages (eg., easy_ocr might not be preinstalled)
         # face_detection_udf_query,
         # ocr_udf_query,
         # Mvit_udf_query, - Disabled as it requires specific pytorch package
         # Sift_udf_query, - requires package kornia
     ]
```

### Comparing `evadb-0.2.7/evadb/udfs/yolo_object_detector.py` & `evadb-0.2.8/evadb/udfs/yolo_object_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/utils/__init__.py` & `evadb-0.2.8/evadb/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""general eva utils"""
+"""general evadb utils"""
```

### Comparing `evadb-0.2.7/evadb/utils/errors.py` & `evadb-0.2.8/evadb/utils/errors.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/utils/generic_utils.py` & `evadb-0.2.8/evadb/utils/generic_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -198,15 +198,15 @@
 
     @classmethod
     def deserialize(cls, data):
         return pickle.loads(data)
 
 
 @unique
-class EVAEnum(AutoEnum):
+class EvaDBEnum(AutoEnum):
     def __str__(self):
         return self.name
 
 
 def remove_directory_contents(dir_path):
     if os.path.exists(dir_path):
         for filename in os.listdir(dir_path):
```

### Comparing `evadb-0.2.7/evadb/utils/kv_cache.py` & `evadb-0.2.8/evadb/utils/kv_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/utils/logging_manager.py` & `evadb-0.2.8/evadb/utils/logging_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/utils/math_utils.py` & `evadb-0.2.8/evadb/utils/math_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/utils/s3_utils.py` & `evadb-0.2.8/evadb/utils/s3_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb/utils/stats.py` & `evadb-0.2.8/evadb/utils/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/evadb.egg-info/PKG-INFO` & `evadb-0.2.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,12 @@
-Metadata-Version: 2.1
-Name: evadb
-Version: 0.2.7
-Summary: EVA AI-Relational Database System
-Home-page: https://github.com/georgia-tech-db/eva
-Download-URL: https://github.com/georgia-tech-db/eva
-Author: Georgia Tech Database Group
-Author-email: arulraj@gatech.edu
-License: Apache License 2.0
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# EVA AI-SQL Database System
+# EvaDB AI-SQL Database System
 
 <div>
         <a href="https://colab.research.google.com/github/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb">
-            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EVA on Colab"/>
+            <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open EvaDB on Colab"/>
         </a>
         <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">
             <img alt="Slack" src="https://img.shields.io/badge/slack-eva-ff69b4.svg?logo=slack">
         </a>          
         <a href="https://twitter.com/evadb_ai">
             <img alt="Twitter" src="https://img.shields.io/badge/twitter-eva-bde1ee.svg?logo=twitter">
         </a>  
@@ -37,21 +18,21 @@
         <img alt="Coverage Status" src="https://coveralls.io/repos/github/georgia-tech-db/eva/badge.svg?branch=master"/>     
         <a href="https://pepy.tech/project/evadb">
           <img alt="Downloads" src="https://static.pepy.tech/badge/evadb/month"/>
         </a>
         <img alt="Python Versions" src="https://img.shields.io/badge/Python--versions-3.8%20|%203.9%20|%203.10-brightgreen"/>       
 </div>
 
-<p align="center"> <b><h3>EVA DB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
+<p align="center"> <b><h3>EvaDB is a database system for building simpler and faster AI-powered applications.</b></h3> </p>
 
-EVA DB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (videos, text, podcasts, PDFs, etc.).
+EvaDB is an AI-SQL database system for developing applications powered by AI models. We aim to simplify the development and deployment of AI-powered applications that operate on structured (tables, feature stores) and unstructured data (text documents, videos, PDFs, podcasts, etc.).
 
-EVA DB accelerates AI pipelines by 10-100x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EVA supports an AI-oriented SQL-like query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
+EvaDB accelerates AI pipelines by 10x using a collection of performance optimizations inspired by time-tested SQL database systems, including data-parallel query execution, function caching, sampling, and cost-based predicate reordering. EvaDB supports an AI-oriented query language tailored for analyzing both structured and unstructured data. It has first-class support for PyTorch, Hugging Face, YOLO, and Open AI models.
 
-The high-level SQL API allows even beginners to use EVA in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EVA DB is fully implemented in Python and licensed under the Apache license.
+The high-level Python and SQL APIs allows even beginners to use EvaDB in a few lines of code. Advanced users can define custom user-defined functions that wrap around any AI model or Python library. EvaDB is fully implemented in Python and licensed under the Apache license.
 
 ## Quick Links
 
 - [Features](#features)
 - [Quick Start](#quick-start)
 - [Documentation](#documentation)
 - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
@@ -61,60 +42,60 @@
 - [Community and Support](#community-and-support)
 - [Twitter](https://twitter.com/evadb_ai)
 - [Contributing](#contributing)
 - [License](#license)
 
 ## Features
 
-- 🔮 Build simpler AI-powered applications using short SQL-like queries
-- ⚡️ 10-100x faster AI pipelines using AI-centric query optimization  
+- 🔮 Build simpler AI-powered applications using short Python or SQL queries
+- ⚡️ 10x faster applications using AI-centric query optimization  
 - 💰 Save money spent on GPUs
 - 🚀 First-class support for your custom deep learning models through user-defined functions
 - 📦 Built-in caching to eliminate redundant model invocations across queries
 - ⌨️ First-class support for PyTorch, Hugging Face, YOLO, and Open AI models
 - 🐍 Installable via pip and fully implemented in Python
 
 ## Illustrative Applications
 
-Here are some illustrative EVA-powered applications (each Jupyter notebook can be opened on Google Colab):
+Here are some illustrative EvaDB-powered applications (each Jupyter notebook can be opened on Google Colab):
 
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">Using ChatGPT to ask questions based on videos</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow at an intersection</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining the emotion palette of actors in a movie</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Image Similarity Search on Reddit [FAISS + Qdrant]</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html">Classifying images based on their content</a>
- * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image Segmentation using Hugging Face</a>
- * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates </a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/11-similarity-search-for-motif-mining.html">Reddit Image Similarity Search</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html">ChatGPT-based video question answering</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html">Quering PDF documents</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html">Analysing traffic flow with YOLO</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html">Examining emotion palette of a movie</a>
+ * 🔮 <a href="https://evadb.readthedocs.io/en/stable/source/tutorials/07-object-segmentation-huggingface.html">Image segmentation with Hugging Face</a>
+ * 🔮 <a href="https://github.com/georgia-tech-db/license-plate-recognition">Recognizing license plates</a>
  * 🔮 <a href="https://github.com/georgia-tech-db/toxicity-classification">Analysing toxicity of social media memes </a>
 
 ## Documentation
 
 * [Detailed Documentation](https://evadb.readthedocs.io/)
-  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EVA for different AI tasks and how you can easily extend EVA to support your custom deep learning model through user-defined functions.
-  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EVA. Each notebook includes a link to Google Colab, where you can run the code yourself.
+  - The <a href="https://evadb.readthedocs.io/en/stable/source/overview/installation.html">Getting Started</a> page shows how you can use EvaDB for different AI tasks and how you can easily extend EvaDB to support your custom deep learning model through user-defined functions.
+  - The <a href="https://evadb.readthedocs.io/en/latest/source/tutorials/11-similarity-search-for-motif-mining.html">User Guides</a> section contains Jupyter Notebooks that demonstrate how to use various features of EvaDB. Each notebook includes a link to Google Colab, where you can run the code yourself.
 * [Tutorials](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
 * [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
 * [Follow us on Twitter](https://twitter.com/evadb_ai)
 * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/projects/3)
 * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/08-chatgpt.html)
 
 ## Quick Start
 
-- Install EVA using the pip package manager. EVA supports Python versions >= 3.8:
+- Install EvaDB using the pip package manager. EvaDB supports Python versions >= 3.8:
 
 ```shell
 pip install evadb
 ```
 
-- To launch and connect to an EVA server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
+- To launch and connect to an EvaDB server in a Jupyter notebook, check out this [illustrative emotion analysis notebook](https://github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb):
 ```shell
 cursor = connect_to_server()
 ```
 
-- Load a video onto the EVA server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
+- Load a video onto the EvaDB server (we use [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration):
 
 ```mysql
 LOAD VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo;
 ```
 
 - That's it! You can now run queries over the loaded video:
 
@@ -156,19 +137,19 @@
 ```mysql
    -- Analyse emotions of faces in a video
    SELECT id, bbox, EmotionDetector(Crop(data, bbox)) 
    FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)  
    WHERE id < 15;
 ```
 
-- **EVA runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
+- **EvaDB runs queries faster using its AI-centric query optimizer**. Two key optimizations are:
 
-   💾 **Caching**: EVA automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
+   💾 **Caching**: EvaDB automatically caches and reuses previous query results (especially model inference results), eliminating redundant computation and reducing query processing time.
 
-   🎯 **Predicate Reordering**: EVA optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
+   🎯 **Predicate Reordering**: EvaDB optimizes the order in which the query predicates are evaluated (e.g., runs the faster, more selective model first), leading to faster queries and lower inference costs.
 
 Consider these two exploratory queries on a dataset of dog images:
 <img align="right" style="display:inline;" width="40%" src="https://github.com/georgia-tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true"></a>
 
 ```mysql
   -- Query 1: Find all images of black-colored dogs
   SELECT id, bbox FROM dogs 
@@ -180,32 +161,38 @@
   SELECT id, bbox FROM dogs 
   JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) 
   WHERE Obj.label = 'dog' 
     AND DogBreedClassifier(Crop(data, bbox)) = 'great dane' 
     AND Color(Crop(data, bbox)) = 'black';
 ```
 
-By reusing the results of the first query and reordering the predicates based on the available cached inference results, EVA runs the second query **10x faster**!
+By reusing the results of the first query and reordering the predicates based on the available cached inference results, EvaDB runs the second query **10x faster**!
 
 ## Architecture Diagram
 
-This diagram presents the key components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
+This diagram presents the key components of EvaDB. EvaDB's AI-centric Query Optimizer takes a parsed query as input and generates a query plan that is then executed by the Query Engine. The Query Engine hits multiple storage engines to retrieve the data required for efficiently running the query:
 1. Structured data (SQL database system connected via `sqlalchemy`).
 2. Unstructured media data (on cloud buckets or local filesystem).
 3. Vector data (vector database system).
 
 <img width="700" alt="Architecture Diagram" src="https://github.com/georgia-tech-db/eva/assets/5521975/01452ec9-87d9-4d27-90b2-c0b1ab29b16c">
 
 ## Screenshots
 
 ### 🔮 [Traffic Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html) (Object Detection Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-input.webp" width="300"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/traffic-output.webp" width="300"> |
 
+### 🔮 [PDF Question Answering](https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html) (Question Answering Model)
+
+| App |
+|-----|
+|<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/pdf-qa.webp" width="400"> |
+
 ### 🔮 [MNIST Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image Classification Model)
 | Source Video  | Query Result |
 |---------------|--------------|
 |<img alt="Source Video" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-input.webp" width="150"> |<img alt="Query Result" src="https://github.com/georgia-tech-db/eva/releases/download/v0.1.0/mnist-output.webp" width="150"> |
 
 ### 🔮 [Movie Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-analysis.html) (Face Detection + Emotion Classification Models)
 
@@ -217,31 +204,31 @@
 
 | Query Result |
 |--------------|
 <img alt="Query Result" src="https://github.com/georgia-tech-db/license-plate-recognition/blob/main/README_files/README_12_3.png" width="300"> |
 
 ## Community and Support
 
-👋 If you have general questions about EVA, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on Twitter](https://twitter.com/evadb_ai).
+👋 If you have general questions about EvaDB, want to say hello or just follow along, we'd like to invite you to join our [Slack Community](https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) and to [follow us on Twitter](https://twitter.com/evadb_ai).
 
 <a href="https://join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg">              
-    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EVA Slack Channel" width="500">
+    <img src="https://raw.githubusercontent.com/georgia-tech-db/eva/master/docs/images/eva/eva-slack.png" alt="EvaDB Slack Channel" width="500">
 </a>
 
 If you run into any problems or issues, please create a Github issue and we'll try our best to help.
 
 Don't see a feature in the list? Search our issue tracker if someone has already requested it and add a comment to it explaining your use-case, or open a new issue if not. We prioritize our [roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from you.
 
 ## Contributing
 
 [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb)
 [![CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva)
 [![Documentation Status](https://readthedocs.org/projects/evadb/badge/?version=latest)](https://evadb.readthedocs.io/en/latest/index.html)
 
-EVA is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EVA are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
+EvaDB is the beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All kinds of contributions to EvaDB are appreciated. To file a bug or to request a feature, please use <a href="https://github.com/georgia-tech-db/eva/issues">GitHub issues</a>. <a href="https://github.com/georgia-tech-db/eva/pulls">Pull requests</a> are welcome.
 
 For more information, see our
 [contribution guide](https://evadb.readthedocs.io/en/stable/source/contribute/index.html).
 
 ## License
 Copyright (c) 2018-present [Georgia Tech Database Group](http://db.cc.gatech.edu/).
 Licensed under [Apache License](LICENSE).
```

#### html2text {}

```diff
@@ -1,71 +1,61 @@
-Metadata-Version: 2.1 Name: evadb Version: 0.2.7 Summary: EVA AI-Relational
-Database System Home-page: https://github.com/georgia-tech-db/eva Download-URL:
-https://github.com/georgia-tech-db/eva Author: Georgia Tech Database Group
-Author-email: arulraj@gatech.edu License: Apache License 2.0 Classifier:
-Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
-:: Apache Software License Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
-Language :: Python :: 3.10 Requires-Python: >=3.8 Description-Content-Type:
-text/markdown Provides-Extra: dev License-File: LICENSE.txt # EVA AI-SQL
-Database System
-[Open_EVA_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
+# EvaDB AI-SQL Database System
+[Open_EvaDB_on_Colab] [Slack] [Twitter] [Roadmap] [PyPI] [License] [Coverage
 Status] [Downloads] [Python Versions]
-**** EVA DB is a database system for building simpler and faster AI-powered
+**** EvaDB is a database system for building simpler and faster AI-powered
 applications. ****
-EVA DB is an AI-SQL database system for developing applications powered by AI
+EvaDB is an AI-SQL database system for developing applications powered by AI
 models. We aim to simplify the development and deployment of AI-powered
 applications that operate on structured (tables, feature stores) and
-unstructured data (videos, text, podcasts, PDFs, etc.). EVA DB accelerates AI
-pipelines by 10-100x using a collection of performance optimizations inspired
-by time-tested SQL database systems, including data-parallel query execution,
-function caching, sampling, and cost-based predicate reordering. EVA supports
-an AI-oriented SQL-like query language tailored for analyzing both structured
-and unstructured data. It has first-class support for PyTorch, Hugging Face,
-YOLO, and Open AI models. The high-level SQL API allows even beginners to use
-EVA in a few lines of code. Advanced users can define custom user-defined
-functions that wrap around any AI model or Python library. EVA DB is fully
-implemented in Python and licensed under the Apache license. ## Quick Links -
-[Features](#features) - [Quick Start](#quick-start) - [Documentation]
-(#documentation) - [Roadmap](https://github.com/orgs/georgia-tech-db/projects/
-3) - [Architecture Diagram](#architecture-diagram) - [Illustrative
-Applications](#illustrative-applications) - [Screenshots](#screenshots) -
-[Community and Support](#community-and-support) - [Twitter](https://
-twitter.com/evadb_ai) - [Contributing](#contributing) - [License](#license) ##
-Features - ð® Build simpler AI-powered applications using short SQL-like
-queries - â¡ï¸ 10-100x faster AI pipelines using AI-centric query
+unstructured data (text documents, videos, PDFs, podcasts, etc.). EvaDB
+accelerates AI pipelines by 10x using a collection of performance optimizations
+inspired by time-tested SQL database systems, including data-parallel query
+execution, function caching, sampling, and cost-based predicate reordering.
+EvaDB supports an AI-oriented query language tailored for analyzing both
+structured and unstructured data. It has first-class support for PyTorch,
+Hugging Face, YOLO, and Open AI models. The high-level Python and SQL APIs
+allows even beginners to use EvaDB in a few lines of code. Advanced users can
+define custom user-defined functions that wrap around any AI model or Python
+library. EvaDB is fully implemented in Python and licensed under the Apache
+license. ## Quick Links - [Features](#features) - [Quick Start](#quick-start) -
+[Documentation](#documentation) - [Roadmap](https://github.com/orgs/georgia-
+tech-db/projects/3) - [Architecture Diagram](#architecture-diagram) -
+[Illustrative Applications](#illustrative-applications) - [Screenshots]
+(#screenshots) - [Community and Support](#community-and-support) - [Twitter]
+(https://twitter.com/evadb_ai) - [Contributing](#contributing) - [License]
+(#license) ## Features - ð® Build simpler AI-powered applications using short
+Python or SQL queries - â¡ï¸ 10x faster applications using AI-centric query
 optimization - ð° Save money spent on GPUs - ð First-class support for
 your custom deep learning models through user-defined functions - ð¦ Built-in
 caching to eliminate redundant model invocations across queries - â¨ï¸ First-
 class support for PyTorch, Hugging Face, YOLO, and Open AI models - ð
 Installable via pip and fully implemented in Python ## Illustrative
-Applications Here are some illustrative EVA-powered applications (each Jupyter
-notebook can be opened on Google Colab): * ð® Using_ChatGPT_to_ask_questions
-based_on_videos * ð® Analysing_traffic_flow_at_an_intersection * ð®
-Examining_the_emotion_palette_of_actors_in_a_movie * ð® Image_Similarity
-Search_on_Reddit_[FAISS_+_Qdrant] * ð® Classifying_images_based_on_their
-content * ð® Image_Segmentation_using_Hugging_Face * ð® Recognizing_license
-plates * ð® Analysing_toxicity_of_social_media_memes ## Documentation *
-[Detailed Documentation](https://evadb.readthedocs.io/) - The Getting_Started
-page shows how you can use EVA for different AI tasks and how you can easily
-extend EVA to support your custom deep learning model through user-defined
-functions. - The User_Guides section contains Jupyter Notebooks that
-demonstrate how to use various features of EVA. Each notebook includes a link
-to Google Colab, where you can run the code yourself. * [Tutorials](https://
-github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb)
-* [Join us on Slack](https://join.slack.com/t/eva-db/shared_invite/zt-
-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter](https://twitter.com/
-evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/georgia-tech-db/
-projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/source/tutorials/
-08-chatgpt.html) ## Quick Start - Install EVA using the pip package manager.
-EVA supports Python versions >= 3.8: ```shell pip install evadb ``` - To launch
-and connect to an EVA server in a Jupyter notebook, check out this
-[illustrative emotion analysis notebook](https://github.com/georgia-tech-db/
-eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell cursor =
-connect_to_server() ``` - Load a video onto the EVA server (we use
+Applications Here are some illustrative EvaDB-powered applications (each
+Jupyter notebook can be opened on Google Colab): * ð® Reddit_Image_Similarity
+Search * ð® ChatGPT-based_video_question_answering * ð® Quering_PDF
+documents * ð® Analysing_traffic_flow_with_YOLO * ð® Examining_emotion
+palette_of_a_movie * ð® Image_segmentation_with_Hugging_Face * ð®
+Recognizing_license_plates * ð® Analysing_toxicity_of_social_media_memes ##
+Documentation * [Detailed Documentation](https://evadb.readthedocs.io/) - The
+Getting_Started page shows how you can use EvaDB for different AI tasks and how
+you can easily extend EvaDB to support your custom deep learning model through
+user-defined functions. - The User_Guides section contains Jupyter Notebooks
+that demonstrate how to use various features of EvaDB. Each notebook includes a
+link to Google Colab, where you can run the code yourself. * [Tutorials](https:
+//github.com/georgia-tech-db/eva/blob/master/tutorials/03-emotion-
+analysis.ipynb) * [Join us on Slack](https://join.slack.com/t/eva-db/
+shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg) * [Follow us on Twitter]
+(https://twitter.com/evadb_ai) * [Medium-Term Roadmap](https://github.com/orgs/
+georgia-tech-db/projects/3) * [Demo](https://evadb.readthedocs.io/en/stable/
+source/tutorials/08-chatgpt.html) ## Quick Start - Install EvaDB using the pip
+package manager. EvaDB supports Python versions >= 3.8: ```shell pip install
+evadb ``` - To launch and connect to an EvaDB server in a Jupyter notebook,
+check out this [illustrative emotion analysis notebook](https://github.com/
+georgia-tech-db/eva/blob/master/tutorials/03-emotion-analysis.ipynb): ```shell
+cursor = connect_to_server() ``` - Load a video onto the EvaDB server (we use
 [ua_detrac.mp4](data/ua_detrac/ua_detrac.mp4) for illustration): ```mysql LOAD
 VIDEO "data/ua_detrac/ua_detrac.mp4" INTO TrafficVideo; ``` - That's it! You
 can now run queries over the loaded video: ```mysql SELECT id, data FROM
 TrafficVideo WHERE id < 5; ``` - Search for frames in the video that contain a
 car: ```mysql SELECT id, data FROM TrafficVideo WHERE ['car'] <@ Yolo
 (data).labels; ``` | Source Video | Query Result | |---------------|-----------
 ---| |[Source Video] |[Query Result] | - Search for frames in the video that
@@ -74,65 +64,68 @@
 more than three cars: ```mysql SELECT id, data FROM TrafficVideo WHERE
 ArrayCount(Yolo(data).labels, 'car') > 3; ``` - **Use your custom deep learning
 model in queries** with a user-defined function (UDF): ```mysql CREATE UDF IF
 NOT EXISTS Yolo TYPE ultralytics 'model' 'yolov8m.pt'; ``` - **Chain multiple
 models in a single query** to set up useful AI pipelines. ```mysql -- Analyse
 emotions of faces in a video SELECT id, bbox, EmotionDetector(Crop(data, bbox))
 FROM MovieVideo JOIN LATERAL UNNEST(FaceDetector(data)) AS Face(bbox, conf)
-WHERE id < 15; ``` - **EVA runs queries faster using its AI-centric query
-optimizer**. Two key optimizations are: ð¾ **Caching**: EVA automatically
+WHERE id < 15; ``` - **EvaDB runs queries faster using its AI-centric query
+optimizer**. Two key optimizations are: ð¾ **Caching**: EvaDB automatically
 caches and reuses previous query results (especially model inference results),
 eliminating redundant computation and reducing query processing time. ð¯
-**Predicate Reordering**: EVA optimizes the order in which the query predicates
-are evaluated (e.g., runs the faster, more selective model first), leading to
-faster queries and lower inference costs. Consider these two exploratory
-queries on a dataset of dog images: [https://github.com/georgia-tech-db/eva/
-blob/master/data/assets/eva_performance_comparison.png?raw=true]
+**Predicate Reordering**: EvaDB optimizes the order in which the query
+predicates are evaluated (e.g., runs the faster, more selective model first),
+leading to faster queries and lower inference costs. Consider these two
+exploratory queries on a dataset of dog images: [https://github.com/georgia-
+tech-db/eva/blob/master/data/assets/eva_performance_comparison.png?raw=true]
  ```mysql -- Query 1: Find all images of black-colored dogs SELECT id, bbox
 FROM dogs JOIN LATERAL UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE
 Obj.label = 'dog' AND Color(Crop(data, bbox)) = 'black'; -- Query 2: Find all
 Great Danes that are black-colored SELECT id, bbox FROM dogs JOIN LATERAL
 UNNEST(Yolo(data)) AS Obj(label, bbox, score) WHERE Obj.label = 'dog' AND
 DogBreedClassifier(Crop(data, bbox)) = 'great dane' AND Color(Crop(data, bbox))
 = 'black'; ``` By reusing the results of the first query and reordering the
-predicates based on the available cached inference results, EVA runs the second
-query **10x faster**! ## Architecture Diagram This diagram presents the key
-components of EVA DB. EVA's AI-centric Query Optimizer takes a parsed query as
-input and generates a query plan that is then executed by the Query Engine. The
-Query Engine hits multiple storage engines to retrieve the data required for
-efficiently running the query: 1. Structured data (SQL database system
-connected via `sqlalchemy`). 2. Unstructured media data (on cloud buckets or
-local filesystem). 3. Vector data (vector database system). [Architecture
-Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
+predicates based on the available cached inference results, EvaDB runs the
+second query **10x faster**! ## Architecture Diagram This diagram presents the
+key components of EvaDB. EvaDB's AI-centric Query Optimizer takes a parsed
+query as input and generates a query plan that is then executed by the Query
+Engine. The Query Engine hits multiple storage engines to retrieve the data
+required for efficiently running the query: 1. Structured data (SQL database
+system connected via `sqlalchemy`). 2. Unstructured media data (on cloud
+buckets or local filesystem). 3. Vector data (vector database system).
+[Architecture Diagram] ## Screenshots ### ð® [Traffic Analysis](https://
 evadb.readthedocs.io/en/stable/source/tutorials/02-object-detection.html)
 (Object Detection Model) | Source Video | Query Result | |---------------|-----
----------| |[Source Video] |[Query Result] | ### ð® [MNIST Digit Recognition]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/01-mnist.html) (Image
-Classification Model) | Source Video | Query Result | |---------------|--------
-------| |[Source Video] |[Query Result] | ### ð® [Movie Emotion Analysis]
-(https://evadb.readthedocs.io/en/stable/source/tutorials/03-emotion-
-analysis.html) (Face Detection + Emotion Classification Models) | Source Video
-| Query Result | |---------------|--------------| |[Source Video] |[Query
-Result] | ### ð® [License Plate Recognition](https://github.com/georgia-tech-
-db/eva-application-template) (Plate Detection + OCR Extraction Models) | Query
-Result | |--------------| [Query Result] | ## Community and Support ð If you
-have general questions about EVA, want to say hello or just follow along, we'd
-like to invite you to join our [Slack Community](https://join.slack.com/t/eva-
-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)and to [follow us on
-Twitter](https://twitter.com/evadb_ai). [EVA_Slack_Channel] If you run into any
-problems or issues, please create a Github issue and we'll try our best to
-help. Don't see a feature in the list? Search our issue tracker if someone has
-already requested it and add a comment to it explaining your use-case, or open
-a new issue if not. We prioritize our [roadmap](https://github.com/orgs/
-georgia-tech-db/projects/3) based on user feedback, so we'd love to hear from
-you. ## Contributing [![PyPI Version](https://img.shields.io/pypi/v/evadb.svg)]
-(https://pypi.org/project/evadb) [![CI Status](https://circleci.com/gh/georgia-
-tech-db/eva.svg?style=svg)](https://circleci.com/gh/georgia-tech-db/eva) [!
-[Documentation Status](https://readthedocs.org/projects/evadb/badge/
-?version=latest)](https://evadb.readthedocs.io/en/latest/index.html) EVA is the
-beneficiary of many [contributors](https://github.com/georgia-tech-db/eva/
-graphs/contributors). All kinds of contributions to EVA are appreciated. To
-file a bug or to request a feature, please use GitHub_issues. Pull_requests are
-welcome. For more information, see our [contribution guide](https://
-evadb.readthedocs.io/en/stable/source/contribute/index.html). ## License
-Copyright (c) 2018-present [Georgia Tech Database Group](http://
-db.cc.gatech.edu/). Licensed under [Apache License](LICENSE).
+---------| |[Source Video] |[Query Result] | ### ð® [PDF Question Answering]
+(https://evadb.readthedocs.io/en/stable/source/tutorials/12-query-pdf.html)
+(Question Answering Model) | App | |-----| |[Source Video] | ### ð® [MNIST
+Digit Recognition](https://evadb.readthedocs.io/en/stable/source/tutorials/01-
+mnist.html) (Image Classification Model) | Source Video | Query Result | |-----
+----------|--------------| |[Source Video] |[Query Result] | ### ð® [Movie
+Emotion Analysis](https://evadb.readthedocs.io/en/stable/source/tutorials/03-
+emotion-analysis.html) (Face Detection + Emotion Classification Models) |
+Source Video | Query Result | |---------------|--------------| |[Source Video]
+|[Query Result] | ### ð® [License Plate Recognition](https://github.com/
+georgia-tech-db/eva-application-template) (Plate Detection + OCR Extraction
+Models) | Query Result | |--------------| [Query Result] | ## Community and
+Support ð If you have general questions about EvaDB, want to say hello or
+just follow along, we'd like to invite you to join our [Slack Community](https:
+//join.slack.com/t/eva-db/shared_invite/zt-1i10zyddy-PlJ4iawLdurDv~aIAq90Dg)
+and to [follow us on Twitter](https://twitter.com/evadb_ai). [EvaDB_Slack
+Channel] If you run into any problems or issues, please create a Github issue
+and we'll try our best to help. Don't see a feature in the list? Search our
+issue tracker if someone has already requested it and add a comment to it
+explaining your use-case, or open a new issue if not. We prioritize our
+[roadmap](https://github.com/orgs/georgia-tech-db/projects/3) based on user
+feedback, so we'd love to hear from you. ## Contributing [![PyPI Version]
+(https://img.shields.io/pypi/v/evadb.svg)](https://pypi.org/project/evadb) [!
+[CI Status](https://circleci.com/gh/georgia-tech-db/eva.svg?style=svg)](https:/
+/circleci.com/gh/georgia-tech-db/eva) [![Documentation Status](https://
+readthedocs.org/projects/evadb/badge/?version=latest)](https://
+evadb.readthedocs.io/en/latest/index.html) EvaDB is the beneficiary of many
+[contributors](https://github.com/georgia-tech-db/eva/graphs/contributors). All
+kinds of contributions to EvaDB are appreciated. To file a bug or to request a
+feature, please use GitHub_issues. Pull_requests are welcome. For more
+information, see our [contribution guide](https://evadb.readthedocs.io/en/
+stable/source/contribute/index.html). ## License Copyright (c) 2018-present
+[Georgia Tech Database Group](http://db.cc.gatech.edu/). Licensed under [Apache
+License](LICENSE).
```

### Comparing `evadb-0.2.7/evadb.egg-info/SOURCES.txt` & `evadb-0.2.8/evadb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.py
 evadb/__init__.py
 evadb/constants.py
 evadb/database.py
-evadb/eva_cmd_client.py
-evadb/eva_server.py
 evadb/evadb.yml
+evadb/evadb_cmd_client.py
+evadb/evadb_server.py
 evadb/version.py
 evadb.egg-info/PKG-INFO
 evadb.egg-info/SOURCES.txt
 evadb.egg-info/dependency_links.txt
 evadb.egg-info/entry_points.txt
 evadb.egg-info/requires.txt
 evadb.egg-info/top_level.txt
@@ -240,14 +240,15 @@
 evadb/udfs/fastrcnn_object_detector.py
 evadb/udfs/feature_extractor.py
 evadb/udfs/gpu_compatible.py
 evadb/udfs/mnist_image_classifier.py
 evadb/udfs/mvit_action_recognition.py
 evadb/udfs/ocr_extractor.py
 evadb/udfs/saliency_feature_extractor.py
+evadb/udfs/sentence_feature_extractor.py
 evadb/udfs/sentence_transformer_feature_extractor.py
 evadb/udfs/sift_feature_extractor.py
 evadb/udfs/udf_bootstrap_queries.py
 evadb/udfs/yolo_object_detector.py
 evadb/udfs/abstract/__init__.py
 evadb/udfs/abstract/abstract_udf.py
 evadb/udfs/abstract/hf_abstract_udf.py
```

### Comparing `evadb-0.2.7/evadb.egg-info/requires.txt` & `evadb-0.2.8/evadb.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 opencv-contrib-python-headless>=4.6.0.66
 Pillow>=8.4.0
 sqlalchemy<2.0.0,>=1.4.0
 sqlalchemy-utils>=0.36.6
 lark>=1.0.0
 pyyaml>=5.1
 importlib-metadata<5.0
-ray>=1.13.0
+ray<2.5.0,>=1.13.0
 aenum>=2.2.0
 diskcache>=5.4.0
 eva-decord>=0.6.1
 boto3
 nest_asyncio
 langchain
 pymupdf
@@ -22,28 +22,29 @@
 faiss-cpu
 facenet-pytorch>=2.5.2
 ipython<8.13.0
 thefuzz
 ultralytics>=8.0.93
 transformers>=4.27.4
 openai>=0.27.4
+retry>=0.9.2
 timm>=0.6.13
 norfair>=2.2.0
 
 [dev]
 numpy>=1.19.5
 pandas>=1.1.5
 opencv-contrib-python-headless>=4.6.0.66
 Pillow>=8.4.0
 sqlalchemy<2.0.0,>=1.4.0
 sqlalchemy-utils>=0.36.6
 lark>=1.0.0
 pyyaml>=5.1
 importlib-metadata<5.0
-ray>=1.13.0
+ray<2.5.0,>=1.13.0
 aenum>=2.2.0
 diskcache>=5.4.0
 eva-decord>=0.6.1
 boto3
 nest_asyncio
 langchain
 pymupdf
@@ -54,14 +55,15 @@
 faiss-cpu
 facenet-pytorch>=2.5.2
 ipython<8.13.0
 thefuzz
 ultralytics>=8.0.93
 transformers>=4.27.4
 openai>=0.27.4
+retry>=0.9.2
 timm>=0.6.13
 norfair>=2.2.0
 black>=23.1.0
 isort>=5.10.1
 pytest>=6.1.2
 pytest-cov>=2.11.1
 pytest-random-order>=1.0.4
@@ -79,10 +81,11 @@
 codespell
 pylint
 pymysql>=0.10.1
 wheel>=0.37.1
 semantic_version
 PyGithub
 twine
+PyDriller
 qdrant-client>=1.1.7
 kornia
 langchain>=0.0.177
```

### Comparing `evadb-0.2.7/setup.py` & `evadb-0.2.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ###############################
-### EVA PACKAGAGING
+### EvaDB PACKAGAGING
 ###############################
 
 import io
 import os
 
 # to read contents of README file
 from pathlib import Path
@@ -12,15 +12,15 @@
 from setuptools import find_packages, setup
 from setuptools.command.install import install
 from subprocess import check_call
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-DESCRIPTION = "EVA AI-Relational Database System"
+DESCRIPTION = "EvaDB AI-Relational Database System"
 NAME = "evadb"
 AUTHOR = "Georgia Tech Database Group"
 AUTHOR_EMAIL = "arulraj@gatech.edu"
 URL = "https://github.com/georgia-tech-db/eva"
 
 
 def read(path, encoding="utf-8"):
@@ -44,15 +44,15 @@
     "opencv-contrib-python-headless>=4.6.0.66",
     "Pillow>=8.4.0",
     "sqlalchemy>=1.4.0,<2.0.0",  # major changes in 2.0.0
     "sqlalchemy-utils>=0.36.6",
     "lark>=1.0.0",
     "pyyaml>=5.1",
     "importlib-metadata<5.0",
-    "ray>=1.13.0",
+    "ray>=1.13.0,<2.5.0", # breaking change in 2.5.0
     "aenum>=2.2.0",
     "diskcache>=5.4.0",
     "eva-decord>=0.6.1",
     "boto3",
     "nest_asyncio",
     "langchain",
     "pymupdf",
@@ -92,31 +92,33 @@
 benchmark_libs = [
     "pytest-benchmark",
 ]
 
 doc_libs = ["codespell", "pylint"]
 
 dist_libs = [
-    "wheel>=0.37.1", 
-    "semantic_version", 
-    "PyGithub", 
-    "twine"
+    "wheel>=0.37.1",
+    "semantic_version",
+    "PyGithub",
+    "twine",
+    "PyDriller"
 ]
 
 ### NEEDED FOR AN ALTERNATE DATA SYSTEM OTHER THAN SQLITE
 database_libs = ["pymysql>=0.10.1"]
 
 ### NEEDED FOR A BATTERIES-LOADED EXPERIENCE
 udf_libs = [
     "facenet-pytorch>=2.5.2",  # FACE DETECTION
     "ipython<8.13.0",  # NOTEBOOKS
     "thefuzz",  # FUZZY STRING MATCHING
     "ultralytics>=8.0.93",  # OBJECT DETECTION
     "transformers>=4.27.4",  # HUGGINGFACE
     "openai>=0.27.4",  # CHATGPT
+    "retry>=0.9.2", #CHATGPT
     "timm>=0.6.13",  # HUGGINGFACE VISION TASKS
     "norfair>=2.2.0",  # OBJECT TRACKING
 ]
 
 ### NEEDED FOR EXPERIMENTAL FEATURES
 third_party_libs = [
     "qdrant-client>=1.1.7",  # Qdrant vector store client
@@ -163,16 +165,16 @@
         "Programming Language :: Python :: 3.10",
         # "Programming Language :: Python :: 3.11",
     ],
     packages=find_packages(exclude=["tests", "tests.*"]),
     # https://python-packaging.readthedocs.io/en/latest/command-line-scripts.html#the-console-scripts-entry-point
     entry_points={
         "console_scripts": [
-            "eva_server=evadb.eva_server:main",
-            "eva_client=evadb.eva_cmd_client:main",
+            "eva_server=evadb.evadb_server:main",
+            "eva_client=evadb.evadb_cmd_client:main",
         ]
     },
     python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require=EXTRA_REQUIRES,
     include_package_data=True,
     package_data={"evadb": ["evadb.yml", "parser/evadb.lark"]},
```

### Comparing `evadb-0.2.7/test/__init__.py` & `evadb-0.2.8/evadb/catalog/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+catalog subdirectory
+"""
```

### Comparing `evadb-0.2.7/test/benchmark_tests/__init__.py` & `evadb-0.2.8/test/binder/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/benchmark_tests/conftest.py` & `evadb-0.2.8/test/benchmark_tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/benchmark_tests/test_benchmark_pytorch.py` & `evadb-0.2.8/test/benchmark_tests/test_benchmark_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/binder/__init__.py` & `evadb-0.2.8/test/catalog/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/binder/test_statement_binder.py` & `evadb-0.2.8/test/binder/test_statement_binder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/binder/test_statement_binder_context.py` & `evadb-0.2.8/test/binder/test_statement_binder_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/catalog/__init__.py` & `evadb-0.2.8/test/catalog/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/catalog/models/__init__.py` & `evadb-0.2.8/test/executor/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/catalog/models/test_models.py` & `evadb-0.2.8/test/catalog/models/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -63,20 +63,20 @@
         self.assertNotEqual(df_col, df_col1)
 
     def test_table_catalog_entry_equality(self):
         column_1 = ColumnCatalogEntry("frame_id", ColumnType.INTEGER, False)
         column_2 = ColumnCatalogEntry("frame_label", ColumnType.INTEGER, False)
         col_list = [column_1, column_2]
         table_catalog_entry = TableCatalogEntry(
-            "name", "eva_dataset", table_type=TableType.VIDEO_DATA, columns=col_list
+            "name", "evadb_dataset", table_type=TableType.VIDEO_DATA, columns=col_list
         )
         self.assertEqual(table_catalog_entry, table_catalog_entry)
 
         table_catalog_entry1 = TableCatalogEntry(
-            "name2", "eva_dataset", table_type=TableType.VIDEO_DATA, columns=col_list
+            "name2", "evadb_dataset", table_type=TableType.VIDEO_DATA, columns=col_list
         )
 
         self.assertNotEqual(table_catalog_entry, table_catalog_entry1)
 
     def test_udf(self):
         udf = UdfCatalogEntry("udf", "fasterRCNN", "ObjectDetection", "checksum")
         self.assertEqual(udf.row_id, None)
```

### Comparing `evadb-0.2.7/test/catalog/test_catalog_manager.py` & `evadb-0.2.8/test/catalog/test_catalog_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/catalog/test_column_type.py` & `evadb-0.2.8/test/catalog/test_column_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/__init__.py` & `evadb-0.2.8/test/expression/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_abstract_executor.py` & `evadb-0.2.8/test/executor/test_abstract_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_create_udf_executor.py` & `evadb-0.2.8/test/executor/test_create_udf_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_execution_context.py` & `evadb-0.2.8/test/executor/test_execution_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_limit_executor.py` & `evadb-0.2.8/test/executor/test_limit_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_orderby_executor.py` & `evadb-0.2.8/test/executor/test_orderby_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_plan_executor.py` & `evadb-0.2.8/test/executor/test_plan_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_sample_executor.py` & `evadb-0.2.8/test/executor/test_sample_executor.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/test_seq_scan_executor.py` & `evadb-0.2.8/test/executor/test_seq_scan_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/executor/utils.py` & `evadb-0.2.8/test/executor/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/__init__.py` & `evadb-0.2.8/test/integration_tests/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_abstract_expression.py` & `evadb-0.2.8/test/expression/test_abstract_expression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_aggregation.py` & `evadb-0.2.8/test/expression/test_aggregation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_arithmetic.py` & `evadb-0.2.8/test/expression/test_arithmetic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_comparison.py` & `evadb-0.2.8/test/expression/test_comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_expression_tree.py` & `evadb-0.2.8/test/expression/test_expression_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_expression_utils.py` & `evadb-0.2.8/test/expression/test_expression_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_function_expression.py` & `evadb-0.2.8/test/expression/test_function_expression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/expression/test_logical.py` & `evadb-0.2.8/test/expression/test_logical.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/__init__.py` & `evadb-0.2.8/test/interfaces/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_array_count.py` & `evadb-0.2.8/test/integration_tests/test_array_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_create_index_executor.py` & `evadb-0.2.8/test/integration_tests/test_create_index_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_create_table_executor.py` & `evadb-0.2.8/test/integration_tests/test_create_table_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
     load_udfs_for_testing,
     shutdown_ray,
 )
 
 import pandas as pd
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.executor.executor_utils import ExecutorError
 from evadb.models.storage.batch import Batch
 from evadb.server.command_handler import execute_query_fetch_all
 
 NUM_FRAMES = 10
 
 
@@ -38,15 +38,15 @@
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
         # reset the catalog manager before running each test
         cls.evadb.catalog().reset()
         video_file_path = create_sample_video()
         load_query = f"LOAD VIDEO '{video_file_path}' INTO MyVideo;"
         execute_query_fetch_all(cls.evadb, load_query)
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{ua_detrac}' INTO UATRAC;")
         load_udfs_for_testing(cls.evadb)
 
     @classmethod
     def tearDownClass(cls):
         file_remove("dummy.avi")
         file_remove("ua_detrac.mp4")
```

### Comparing `evadb-0.2.7/test/integration_tests/test_delete_executor.py` & `evadb-0.2.8/test/integration_tests/test_delete_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -19,15 +19,15 @@
     load_udfs_for_testing,
     shutdown_ray,
 )
 
 import numpy as np
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 @pytest.mark.notparallel
 class DeleteExecutorTest(unittest.TestCase):
     def setUp(self):
         self.evadb = get_evadb_for_testing()
@@ -61,26 +61,26 @@
         """
         execute_query_fetch_all(self.evadb, insert_query3)
 
         ####################################################
         # Create a table for testing Delete with Video Data#
         ####################################################
 
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/1/*.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/1/*.mp4"
         query = f'LOAD VIDEO "{path}" INTO TestDeleteVideos;'
         _ = execute_query_fetch_all(self.evadb, query)
 
     def tearDown(self):
         shutdown_ray()
         file_remove("dummy.avi")
 
     # integration test
     @unittest.skip("Not supported in current version")
     def test_should_delete_single_video_in_table(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/1/2.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/1/2.mp4"
         delete_query = f"""DELETE FROM TestDeleteVideos WHERE name="{path}";"""
         batch = execute_query_fetch_all(self.evadb, delete_query)
 
         query = "SELECT name FROM MyVideo"
         batch = execute_query_fetch_all(self.evadb, query)
         self.assertIsNone(
             np.testing.assert_array_equal(
@@ -96,15 +96,15 @@
                 batch.frames["data"][0],
                 np.array([[[41, 41, 41], [41, 41, 41]], [[41, 41, 41], [41, 41, 41]]]),
             )
         )
 
     @unittest.skip("Not supported in current version")
     def test_should_delete_single_image_in_table(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/1/2.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/1/2.mp4"
         delete_query = f"""DELETE FROM TestDeleteVideos WHERE name="{path}";"""
         batch = execute_query_fetch_all(self.evadb, delete_query)
 
         query = "SELECT name FROM MyVideo"
         batch = execute_query_fetch_all(self.evadb, query)
         self.assertIsNone(
             np.testing.assert_array_equal(
```

### Comparing `evadb-0.2.7/test/integration_tests/test_drop_executor.py` & `evadb-0.2.8/test/integration_tests/test_drop_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -157,15 +157,15 @@
         index_name = "index_name"
         self._create_index(index_name)
 
         index_obj = self.evadb.catalog().get_index_catalog_entry_by_name(index_name)
         self.assertTrue(index_obj is not None)
 
         # Test that dropping the wrong Index:
-        # - does not affect Indexs in the catalog
+        # - does not affect Indexes in the catalog
         # - raises an appropriate exception
         wrong_udf_name = "wrong_udf_name"
         drop_query = f"DROP INDEX {wrong_udf_name};"
         with self.assertRaises(ExecutorError):
             execute_query_fetch_all(self.evadb, drop_query)
         obj = self.evadb.catalog().get_index_catalog_entry_by_name(index_name)
         self.assertTrue(obj is not None)
```

### Comparing `evadb-0.2.7/test/integration_tests/test_error_handling_with_ray.py` & `evadb-0.2.8/test/integration_tests/test_error_handling_with_ray.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_explain_executor.py` & `evadb-0.2.8/test/integration_tests/test_explain_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_fuzzy_join.py` & `evadb-0.2.8/test/integration_tests/test_fuzzy_join.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,26 +20,27 @@
     file_remove,
     get_evadb_for_testing,
     shutdown_ray,
 )
 
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.server.command_handler import execute_query_fetch_all
+from evadb.udfs.udf_bootstrap_queries import fuzzy_udf_query
 
 
 @pytest.mark.notparallel
 class FuzzyJoinTests(unittest.TestCase):
     def setUp(self):
         self.evadb = get_evadb_for_testing()
         self.evadb.catalog().reset()
         self.video_file_path = create_sample_video()
         self.image_files_path = Path(
-            f"{EVA_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/*.jpg"
+            f"{EvaDB_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/*.jpg"
         )
         self.csv_file_path = create_sample_csv()
 
         # Prepare needed UDFs and data.
         # loading a csv requires a table to be created first
         create_table_query = """
             CREATE TABLE IF NOT EXISTS MyVideoCSV (
@@ -68,25 +69,14 @@
         file_remove("dummy.avi")
         file_remove("dummy.csv")
         # clean up
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS MyVideo;")
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS MyVideoCSV;")
 
     def test_fuzzyjoin(self):
-        EVA_INSTALLATION_DIR = self.evadb.config.get_value(
-            "core", "eva_installation_dir"
-        )
-        fuzzy_udf = """CREATE UDF IF NOT EXISTS FuzzDistance
-                    INPUT (Input_Array1 NDARRAY ANYTYPE, Input_Array2 NDARRAY ANYTYPE)
-                    OUTPUT (distance FLOAT(32, 7))
-                    TYPE NdarrayUDF
-                    IMPL "{}/udfs/{}/fuzzy_join.py";
-        """.format(
-            EVA_INSTALLATION_DIR, "ndarray"
-        )
-        execute_query_fetch_all(self.evadb, fuzzy_udf)
+        execute_query_fetch_all(self.evadb, fuzzy_udf_query)
 
         fuzzy_join_query = """SELECT * FROM MyVideo a JOIN MyVideoCSV b
                       ON FuzzDistance(a.id, b.id) = 100;"""
 
         actual_batch = execute_query_fetch_all(self.evadb, fuzzy_join_query)
         self.assertEqual(len(actual_batch), 10)
```

### Comparing `evadb-0.2.7/test/integration_tests/test_huggingface_udfs.py` & `evadb-0.2.8/test/integration_tests/test_huggingface_udfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -82,15 +82,15 @@
             'task' '{task}'
         """
         # catch an assert
 
         with self.assertRaises(ExecutorError) as exc_info:
             execute_query_fetch_all(self.evadb, create_udf_query)
         self.assertIn(
-            f"Task {task} not supported in EVA currently", str(exc_info.exception)
+            f"Task {task} not supported in EvaDB currently", str(exc_info.exception)
         )
 
     def test_object_detection(self):
         udf_name = "HFObjectDetector"
         create_udf_query = f"""CREATE UDF {udf_name}
             TYPE HuggingFace
             'task' 'object-detection'
```

### Comparing `evadb-0.2.7/test/integration_tests/test_insert_executor.py` & `evadb-0.2.8/test/integration_tests/test_insert_executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -96,17 +96,17 @@
         logger.info(batch)
 
         self.assertIsNone(
             np.testing.assert_array_equal(
                 batch.frames["csvtable.name"].array,
                 np.array(
                     [
-                        "test_eva/similarity/data/sad.jpg",
-                        "test_eva/similarity/data/happy.jpg",
-                        "test_eva/similarity/data/angry.jpg",
+                        "test_evadb/similarity/data/sad.jpg",
+                        "test_evadb/similarity/data/happy.jpg",
+                        "test_evadb/similarity/data/angry.jpg",
                     ]
                 ),
             )
         )
 
         query = """SELECT name FROM CSVTable WHERE name LIKE '.*(sad|happy)';"""
         batch = execute_query_fetch_all(self.evadb, query)
```

### Comparing `evadb-0.2.7/test/integration_tests/test_like.py` & `evadb-0.2.8/test/integration_tests/test_like.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,25 +12,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from test.markers import ocr_skip_marker
 from test.util import get_evadb_for_testing, shutdown_ray
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 class LikeTest(unittest.TestCase):
     def setUp(self):
         self.evadb = get_evadb_for_testing()
         # reset the catalog manager before running each test
         self.evadb.catalog().reset()
-        meme1 = f"{EVA_ROOT_DIR}/data/detoxify/meme1.jpg"
-        meme2 = f"{EVA_ROOT_DIR}/data/detoxify/meme2.jpg"
+        meme1 = f"{EvaDB_ROOT_DIR}/data/detoxify/meme1.jpg"
+        meme2 = f"{EvaDB_ROOT_DIR}/data/detoxify/meme2.jpg"
 
         execute_query_fetch_all(self.evadb, f"LOAD IMAGE '{meme1}' INTO MemeImages;")
         execute_query_fetch_all(self.evadb, f"LOAD IMAGE '{meme2}' INTO MemeImages;")
 
     def tearDown(self):
         shutdown_ray()
         # clean up
```

### Comparing `evadb-0.2.7/test/integration_tests/test_load_executor.py` & `evadb-0.2.8/test/integration_tests/test_load_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -31,30 +31,30 @@
 )
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from evadb.binder.binder_utils import BinderError
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.executor.executor_utils import ExecutorError
 from evadb.models.storage.batch import Batch
 from evadb.parser.types import FileFormatType
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 @pytest.mark.notparallel
 class LoadExecutorTest(unittest.TestCase):
     def setUp(self):
         self.evadb = get_evadb_for_testing()
         # reset the catalog manager before running each test
         self.evadb.catalog().reset()
         self.video_file_path = create_sample_video()
         self.image_files_path = Path(
-            f"{EVA_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/*.jpg"
+            f"{EvaDB_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/*.jpg"
         )
         self.csv_file_path = create_sample_csv()
 
     def tearDown(self):
         shutdown_ray()
 
         file_remove("dummy.avi")
@@ -114,25 +114,25 @@
             "The dataset file could not be found. Please verify that the file exists in the specified path.",
         )
 
         # create the file again for other test cases
         create_sample_video()
 
     def test_should_load_videos_in_table(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/1/*.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/1/*.mp4"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         result = execute_query_fetch_all(self.evadb, query)
         expected = Batch(
             pd.DataFrame([f"Number of loaded {FileFormatType.VIDEO.name}: 2"])
         )
         self.assertEqual(result, expected)
 
     def test_should_form_symlink_to_multiple_videos(self):
         catalog_manager = self.evadb.catalog()
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/1/*.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/1/*.mp4"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         execute_query_fetch_all(self.evadb, query)
 
         table_catalog_entry = catalog_manager.get_table_catalog_entry("MyVideos")
         video_dir = table_catalog_entry.file_url
 
         # the video directory would have two files
@@ -140,56 +140,56 @@
         video_files = os.listdir(video_dir)
         # check that the files are symlinks to the original videos
         for video_file in video_files:
             video_file_path = os.path.join(video_dir, video_file)
             self.assertTrue(os.path.islink(video_file_path))
             self.assertTrue(
                 os.readlink(video_file_path).startswith(
-                    f"{EVA_ROOT_DIR}/data/sample_videos/1"
+                    f"{EvaDB_ROOT_DIR}/data/sample_videos/1"
                 )
             )
 
     def test_should_load_videos_with_same_name_but_different_path(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/**/*.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/**/*.mp4"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         result = execute_query_fetch_all(self.evadb, query)
         expected = Batch(
             pd.DataFrame([f"Number of loaded {FileFormatType.VIDEO.name}: 4"])
         )
         self.assertEqual(result, expected)
 
     def test_should_fail_to_load_videos_with_same_path(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/2/*.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/2/*.mp4"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         result = execute_query_fetch_all(self.evadb, query)
         expected = Batch(
             pd.DataFrame([f"Number of loaded {FileFormatType.VIDEO.name}: 1"])
         )
         self.assertEqual(result, expected)
 
         # original file should be preserved
         expected_output = execute_query_fetch_all(
             self.evadb, "SELECT id FROM MyVideos;"
         )
 
         # try adding duplicate files to the table
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/**/*.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/**/*.mp4"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         with self.assertRaises(ExecutorError):
             execute_query_fetch_all(self.evadb, query)
 
         # original data should be preserved
         after_load_fail = execute_query_fetch_all(
             self.evadb, "SELECT id FROM MyVideos;"
         )
 
         self.assertEqual(expected_output, after_load_fail)
 
     def test_should_fail_to_load_missing_video(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_videos/missing.mp4"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_videos/missing.mp4"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         with self.assertRaises(ExecutorError) as exc_info:
             execute_query_fetch_all(self.evadb, query)
         self.assertIn(
             "Load VIDEO failed due to no valid files found on path",
             str(exc_info.exception),
         )
@@ -200,23 +200,23 @@
         tempfile_path = os.path.join(tempfile.gettempdir(), tempfile_name)
         with open(tempfile_path, "wb") as tmp:
             query = f"""LOAD VIDEO "{tmp.name}" INTO MyVideos;"""
             with self.assertRaises(Exception):
                 execute_query_fetch_all(self.evadb, query)
 
     def test_should_fail_to_load_invalid_files_as_video(self):
-        path = f"{EVA_ROOT_DIR}/data/**"
+        path = f"{EvaDB_ROOT_DIR}/data/**"
         query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
         with self.assertRaises(Exception):
             execute_query_fetch_all(self.evadb, query)
         with self.assertRaises(BinderError):
             execute_query_fetch_all(self.evadb, "SELECT name FROM MyVideos")
 
     def test_should_rollback_if_video_load_fails(self):
-        path_regex = Path(f"{EVA_ROOT_DIR}/data/sample_videos/1/*.mp4")
+        path_regex = Path(f"{EvaDB_ROOT_DIR}/data/sample_videos/1/*.mp4")
         valid_videos = glob.glob(str(path_regex.expanduser()), recursive=True)
 
         tempfile_name = os.urandom(24).hex()
         tempfile_path = os.path.join(tempfile.gettempdir(), tempfile_name)
         with open(tempfile_path, "wb") as empty_file:
             # Load one correct file and one empty file
             # nothing should be added
@@ -240,19 +240,19 @@
                 query = f"""LOAD VIDEO "{path}" INTO MyVideos;"""
                 with self.assertRaises(Exception):
                     execute_query_fetch_all(self.evadb, query)
                 with self.assertRaises(BinderError):
                     execute_query_fetch_all(self.evadb, "SELECT name FROM MyVideos")
 
     def test_should_rollback_and_preserve_previous_state(self):
-        path_regex = Path(f"{EVA_ROOT_DIR}/data/sample_videos/1/*.mp4")
+        path_regex = Path(f"{EvaDB_ROOT_DIR}/data/sample_videos/1/*.mp4")
         valid_videos = glob.glob(str(path_regex.expanduser()), recursive=True)
         # Load one correct file
         # commit
-        load_file = f"{EVA_ROOT_DIR}/data/sample_videos/1/1.mp4"
+        load_file = f"{EvaDB_ROOT_DIR}/data/sample_videos/1/1.mp4"
         execute_query_fetch_all(
             self.evadb, f"""LOAD VIDEO "{load_file}" INTO MyVideos;"""
         )
 
         # Load one correct file and one empty file
         # original file should remain
         tempfile_name = os.urandom(24).hex()
@@ -281,15 +281,15 @@
         result = execute_query_fetch_all(self.evadb, query)
         expected = Batch(
             pd.DataFrame([f"Number of loaded {FileFormatType.IMAGE.name}: {num_files}"])
         )
         self.assertEqual(result, expected)
 
     def test_should_fail_to_load_missing_image(self):
-        path = f"{EVA_ROOT_DIR}/data/sample_images/missing.jpg"
+        path = f"{EvaDB_ROOT_DIR}/data/sample_images/missing.jpg"
         query = f"""LOAD IMAGE "{path}" INTO MyImages;"""
         with self.assertRaises(ExecutorError) as exc_info:
             execute_query_fetch_all(self.evadb, query)
         self.assertIn(
             "Load IMAGE failed due to no valid files found on path",
             str(exc_info.exception),
         )
@@ -328,15 +328,15 @@
         tempfile_path = os.path.join(tempfile.gettempdir(), tempfile_name)
         with open(tempfile_path, "wb") as tmp:
             query = f"""LOAD IMAGE "{tmp.name}" INTO MyImages;"""
             with self.assertRaises(Exception):
                 execute_query_fetch_all(self.evadb, query)
 
     def test_should_fail_to_load_invalid_files_as_image(self):
-        path = f"{EVA_ROOT_DIR}/data/**"
+        path = f"{EvaDB_ROOT_DIR}/data/**"
         query = f"""LOAD IMAGE "{path}" INTO MyImages;"""
         with self.assertRaises(Exception):
             execute_query_fetch_all(self.evadb, query)
         with self.assertRaises(BinderError):
             execute_query_fetch_all(self.evadb, "SELECT name FROM MyImages;")
 
     def test_should_rollback_if_image_load_fails(self):
@@ -512,15 +512,15 @@
 
         # Clean up large scale image directory.
         shutil.rmtree(large_scale_image_files_path)
 
     def test_load_pdfs(self):
         execute_query_fetch_all(
             self.evadb,
-            f"""LOAD DOCUMENT '{EVA_ROOT_DIR}/data/documents/*.pdf' INTO pdfs;""",
+            f"""LOAD DOCUMENT '{EvaDB_ROOT_DIR}/data/documents/*.pdf' INTO pdfs;""",
         )
         result = execute_query_fetch_all(self.evadb, "SELECT * from pdfs;")
         self.assertEqual(len(result.columns), 3)
         self.assertEqual(len(result), 4)
 
 
 if __name__ == "__main__":
```

### Comparing `evadb-0.2.7/test/integration_tests/test_load_pdf_executor.py` & `evadb-0.2.8/test/integration_tests/test_load_pdf_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,30 +13,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from test.util import get_evadb_for_testing
 
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 @pytest.mark.notparallel
 class LoadExecutorTest(unittest.TestCase):
     def setUp(self):
         self.evadb = get_evadb_for_testing()
         # reset the catalog manager before running each test
         self.evadb.catalog().reset()
 
     def tearDown(self):
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS MyPDFs;")
 
     def test_load_pdfs(self):
-        pdf_path = f"{EVA_ROOT_DIR}/data/documents/pdf_sample1.pdf"
+        pdf_path = f"{EvaDB_ROOT_DIR}/data/documents/pdf_sample1.pdf"
 
         import fitz
 
         doc = fitz.open(pdf_path)
         number_of_paragraphs = 0
         for page in doc:
             blocks = page.get_text("dict")["blocks"]
```

### Comparing `evadb-0.2.7/test/integration_tests/test_mat_executor.py` & `evadb-0.2.8/test/integration_tests/test_mat_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -21,15 +21,15 @@
     load_udfs_for_testing,
     shutdown_ray,
 )
 
 import pandas as pd
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.models.storage.batch import Batch
 from evadb.server.command_handler import execute_query_fetch_all
 
 NUM_FRAMES = 10
 
 
 @pytest.mark.notparallel
@@ -41,15 +41,15 @@
         ray.init(num_cpus=1)
         cls.evadb = get_evadb_for_testing()
         # reset the catalog manager before running each test
         cls.evadb.catalog().reset()
         video_file_path = create_sample_video()
         load_query = f"LOAD VIDEO '{video_file_path}' INTO MyVideo;"
         execute_query_fetch_all(cls.evadb, load_query)
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{ua_detrac}' INTO UATRAC;")
         load_udfs_for_testing(cls.evadb)
 
     @classmethod
     def tearDownClass(cls):
         shutdown_ray()
         file_remove("dummy.avi")
```

### Comparing `evadb-0.2.7/test/integration_tests/test_open.py` & `evadb-0.2.8/test/integration_tests/test_open.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_optimizer_rules.py` & `evadb-0.2.8/test/integration_tests/test_optimizer_rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,15 +22,15 @@
 )
 
 import numpy as np
 import pandas as pd
 import pytest
 from mock import MagicMock, patch
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.expression.comparison_expression import ComparisonExpression
 from evadb.models.storage.batch import Batch
 from evadb.optimizer.plan_generator import PlanGenerator
 from evadb.optimizer.rules.rules import (
     PushDownFilterThroughApplyAndMerge,
     PushDownFilterThroughJoin,
     ReorderPredicates,
@@ -45,15 +45,15 @@
 @pytest.mark.notparallel
 @ray_skip_marker
 class OptimizerRulesTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
         cls.evadb.catalog().reset()
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{ua_detrac}' INTO MyVideo;")
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{ua_detrac}' INTO MyVideo2;")
         load_udfs_for_testing(cls.evadb, mode="debug")
 
     @classmethod
     def tearDownClass(cls):
         shutdown_ray()
```

### Comparing `evadb-0.2.7/test/integration_tests/test_pytorch.py` & `evadb-0.2.8/test/integration_tests/test_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,35 +24,35 @@
 )
 
 import cv2
 import numpy as np
 import pandas.testing as pd_testing
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.executor.executor_utils import ExecutorError
 from evadb.models.storage.batch import Batch
 from evadb.server.command_handler import execute_query_fetch_all
 from evadb.udfs.udf_bootstrap_queries import Asl_udf_query, Mvit_udf_query
 
 
 @pytest.mark.notparallel
 class PytorchTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
         cls.evadb.catalog().reset()
         os.environ["ray"] = str(cls.evadb.config.get_value("experimental", "ray"))
 
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
-        mnist = f"{EVA_ROOT_DIR}/data/mnist/mnist.mp4"
-        actions = f"{EVA_ROOT_DIR}/data/actions/actions.mp4"
-        asl_actions = f"{EVA_ROOT_DIR}/data/actions/computer_asl.mp4"
-        meme1 = f"{EVA_ROOT_DIR}/data/detoxify/meme1.jpg"
-        meme2 = f"{EVA_ROOT_DIR}/data/detoxify/meme2.jpg"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        mnist = f"{EvaDB_ROOT_DIR}/data/mnist/mnist.mp4"
+        actions = f"{EvaDB_ROOT_DIR}/data/actions/actions.mp4"
+        asl_actions = f"{EvaDB_ROOT_DIR}/data/actions/computer_asl.mp4"
+        meme1 = f"{EvaDB_ROOT_DIR}/data/detoxify/meme1.jpg"
+        meme2 = f"{EvaDB_ROOT_DIR}/data/detoxify/meme2.jpg"
 
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{ua_detrac}' INTO MyVideo;")
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{mnist}' INTO MNIST;")
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{actions}' INTO Actions;")
         execute_query_fetch_all(
             cls.evadb, f"LOAD VIDEO '{asl_actions}' INTO Asl_actions;"
         )
```

### Comparing `evadb-0.2.7/test/integration_tests/test_rename_executor.py` & `evadb-0.2.8/test/integration_tests/test_rename_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_reuse.py` & `evadb-0.2.8/test/integration_tests/test_reuse.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,15 +20,15 @@
 from test.util import (
     get_evadb_for_testing,
     get_logical_query_plan,
     load_udfs_for_testing,
     shutdown_ray,
 )
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.optimizer.operators import LogicalFunctionScan
 from evadb.optimizer.plan_generator import PlanGenerator
 from evadb.optimizer.rules.rules import (
     CacheFunctionExpressionInApply,
     CacheFunctionExpressionInFilter,
     CacheFunctionExpressionInProject,
 )
@@ -46,15 +46,15 @@
             'model' 'facebook/detr-resnet-50';
         """
         execute_query_fetch_all(self.evadb, create_udf_query)
 
     def setUp(self):
         self.evadb = get_evadb_for_testing()
         self.evadb.catalog().reset()
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         execute_query_fetch_all(self.evadb, f"LOAD VIDEO '{ua_detrac}' INTO DETRAC;")
         load_udfs_for_testing(self.evadb)
         self._load_hf_model()
 
     def tearDown(self):
         shutdown_ray()
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS DETRAC;")
@@ -189,25 +189,25 @@
     @windows_skip_marker
     def test_reuse_after_server_shutdown(self):
         select_query = """SELECT id, label FROM DETRAC JOIN
             LATERAL Yolo(data) AS Obj(label, bbox, conf) WHERE id < 4;"""
         execute_query_fetch_all(self.evadb, select_query)
 
         # Stop and restart server
-        os.system("nohup eva_server --stop")
-        os.system("nohup eva_server --start &")
+        os.system("nohup evadb_server --stop")
+        os.system("nohup evadb_server --start &")
 
         select_query = """SELECT id, label FROM DETRAC JOIN
             LATERAL Yolo(data) AS Obj(label, bbox, conf) WHERE id < 6;"""
 
         reuse_batch = execute_query_fetch_all(self.evadb, select_query)
         self._verify_reuse_correctness(select_query, reuse_batch)
 
         # stop the server
-        os.system("nohup eva_server --stop")
+        os.system("nohup evadb_server --stop")
 
     def test_drop_udf_should_remove_cache(self):
         select_query = """SELECT id, label FROM DETRAC JOIN
             LATERAL Yolo(data) AS Obj(label, bbox, conf) WHERE id < 5;"""
         execute_query_fetch_all(self.evadb, select_query)
 
         plan = next(
```

### Comparing `evadb-0.2.7/test/integration_tests/test_s3_load_executor.py` & `evadb-0.2.8/test/integration_tests/test_s3_load_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -24,30 +24,30 @@
 )
 
 import boto3
 import pandas as pd
 import pytest
 from moto import mock_s3
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.models.storage.batch import Batch
 from evadb.parser.types import FileFormatType
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 @pytest.mark.notparallel
 class S3LoadExecutorTest(unittest.TestCase):
     mock_s3 = mock_s3()
 
     def setUp(self):
         self.evadb = get_evadb_for_testing()
         # reset the catalog manager before running each test
         self.evadb.catalog().reset()
         self.video_file_path = create_sample_video()
-        self.multiple_video_file_path = f"{EVA_ROOT_DIR}/data/sample_videos/1"
+        self.multiple_video_file_path = f"{EvaDB_ROOT_DIR}/data/sample_videos/1"
         self.s3_download_dir = self.evadb.config.get_value("storage", "s3_download_dir")
 
         """Mocked AWS Credentials for moto."""
         os.environ["AWS_ACCESS_KEY_ID"] = "testing"
         os.environ["AWS_SECRET_ACCESS_KEY"] = "testing"
         os.environ["AWS_SECURITY_TOKEN"] = "testing"
         os.environ["AWS_SESSION_TOKEN"] = "testing"
```

### Comparing `evadb-0.2.7/test/integration_tests/test_saliency.py` & `evadb-0.2.8/test/integration_tests/test_saliency.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -13,47 +13,47 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from test.util import shutdown_ray, suffix_pytest_xdist_worker_id_to_dir
 
 import pytest
 
-from evadb.configuration.constants import EVA_DATABASE_DIR, EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_DATABASE_DIR, EvaDB_ROOT_DIR
 from evadb.interfaces.relational.db import connect
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 @pytest.mark.notparallel
 class SaliencyTests(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
-        cls.db_dir = suffix_pytest_xdist_worker_id_to_dir(EVA_DATABASE_DIR)
+        cls.db_dir = suffix_pytest_xdist_worker_id_to_dir(EvaDB_DATABASE_DIR)
         cls.conn = connect(cls.db_dir)
         cls.evadb = cls.conn._evadb
 
     @classmethod
     def tearDownClass(cls):
         shutdown_ray()
         # execute_query_fetch_all("DROP TABLE IF EXISTS MyVideo;")
         execute_query_fetch_all(cls.evadb, "DROP TABLE IF EXISTS SALIENCY;")
         # file_remove("dummy.avi")
 
     def test_saliency(self):
-        Saliency1 = f"{EVA_ROOT_DIR}/data/saliency/test1.jpeg"
+        Saliency1 = f"{EvaDB_ROOT_DIR}/data/saliency/test1.jpeg"
         create_udf_query = f"LOAD IMAGE '{Saliency1}' INTO SALIENCY;"
 
         execute_query_fetch_all(self.evadb, "DROP TABLE IF EXISTS SALIENCY;")
 
         execute_query_fetch_all(self.evadb, create_udf_query)
         execute_query_fetch_all(
             self.evadb, "DROP UDF IF EXISTS SaliencyFeatureExtractor"
         )
 
         create_udf_query = f"""CREATE UDF IF NOT EXISTS SaliencyFeatureExtractor
-                    IMPL  '{EVA_ROOT_DIR}/evadb/udfs/saliency_feature_extractor.py';
+                    IMPL  '{EvaDB_ROOT_DIR}/evadb/udfs/saliency_feature_extractor.py';
         """
         execute_query_fetch_all(self.evadb, create_udf_query)
 
         select_query_saliency = """SELECT data, SaliencyFeatureExtractor(data)
                   FROM SALIENCY
         """
         actual_batch_saliency = execute_query_fetch_all(
```

### Comparing `evadb-0.2.7/test/integration_tests/test_select_executor.py` & `evadb-0.2.8/test/integration_tests/test_select_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,15 +26,15 @@
 )
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from evadb.binder.binder_utils import BinderError
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.models.storage.batch import Batch
 from evadb.readers.decord_reader import DecordReader
 from evadb.server.command_handler import execute_query_fetch_all
 
 NUM_FRAMES = 10
 
 
@@ -43,24 +43,24 @@
     @classmethod
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
         cls.evadb.catalog().reset()
         video_file_path = create_sample_video(NUM_FRAMES)
         load_query = f"LOAD VIDEO '{video_file_path}' INTO MyVideo;"
         execute_query_fetch_all(cls.evadb, load_query)
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
         load_query = f"LOAD VIDEO '{ua_detrac}' INTO DETRAC;"
         execute_query_fetch_all(cls.evadb, load_query)
         load_udfs_for_testing(cls.evadb)
         cls.table1 = create_table(cls.evadb, "table1", 100, 3)
         cls.table2 = create_table(cls.evadb, "table2", 500, 3)
         cls.table3 = create_table(cls.evadb, "table3", 1000, 3)
 
-        cls.meme1 = f"{EVA_ROOT_DIR}/data/detoxify/meme1.jpg"
-        cls.meme2 = f"{EVA_ROOT_DIR}/data/detoxify/meme2.jpg"
+        cls.meme1 = f"{EvaDB_ROOT_DIR}/data/detoxify/meme1.jpg"
+        cls.meme2 = f"{EvaDB_ROOT_DIR}/data/detoxify/meme2.jpg"
 
         execute_query_fetch_all(cls.evadb, f"LOAD IMAGE '{cls.meme1}' INTO MemeImages;")
         execute_query_fetch_all(cls.evadb, f"LOAD IMAGE '{cls.meme2}' INTO MemeImages;")
 
     @classmethod
     def tearDownClass(cls):
         shutdown_ray()
```

### Comparing `evadb-0.2.7/test/integration_tests/test_show_info_executor.py` & `evadb-0.2.8/test/integration_tests/test_show_info_executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 import unittest
 from test.markers import windows_skip_marker
 from test.util import get_evadb_for_testing
 
 import pandas as pd
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.models.storage.batch import Batch
 from evadb.server.command_handler import execute_query_fetch_all
 from evadb.udfs.udf_bootstrap_queries import ArrayCount_udf_query, Fastrcnn_udf_query
 
 NUM_FRAMES = 10
 
 
@@ -34,17 +34,17 @@
     def setUpClass(cls):
         cls.evadb = get_evadb_for_testing()
         cls.evadb.catalog().reset()
         queries = [Fastrcnn_udf_query, ArrayCount_udf_query]
         for query in queries:
             execute_query_fetch_all(cls.evadb, query)
 
-        ua_detrac = f"{EVA_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
-        mnist = f"{EVA_ROOT_DIR}/data/mnist/mnist.mp4"
-        actions = f"{EVA_ROOT_DIR}/data/actions/actions.mp4"
+        ua_detrac = f"{EvaDB_ROOT_DIR}/data/ua_detrac/ua_detrac.mp4"
+        mnist = f"{EvaDB_ROOT_DIR}/data/mnist/mnist.mp4"
+        actions = f"{EvaDB_ROOT_DIR}/data/actions/actions.mp4"
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{ua_detrac}' INTO MyVideo;")
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{mnist}' INTO MNIST;")
         execute_query_fetch_all(cls.evadb, f"LOAD VIDEO '{actions}' INTO Actions;")
 
     @classmethod
     def tearDownClass(cls):
         execute_query_fetch_all(cls.evadb, "DROP TABLE IF EXISTS Actions;")
@@ -62,26 +62,26 @@
         }
         expected_df = pd.DataFrame(expected)
         self.assertTrue(all(expected_df.name == result.frames.name))
         self.assertTrue(all(expected_df.type == result.frames.type))
 
     @windows_skip_marker
     def test_show_tables(self):
-        # Note this test can causes sqlalchemy issues if the eva_server is not stopped
+        # Note this test can causes sqlalchemy issues if the evadb_server is not stopped
         result = execute_query_fetch_all(self.evadb, "SHOW TABLES;")
         self.assertEqual(len(result), 3)
         expected = {"name": ["MyVideo", "MNIST", "Actions"]}
         expected_df = pd.DataFrame(expected)
         self.assertEqual(result, Batch(expected_df))
 
         # Stop and restart server
-        os.system("nohup eva_server --stop")
-        os.system("nohup eva_server --start &")
+        os.system("nohup evadb_server --stop")
+        os.system("nohup evadb_server --start &")
 
         result = execute_query_fetch_all(self.evadb, "SHOW TABLES;")
         self.assertEqual(len(result), 3)
         expected = {"name": ["MyVideo", "MNIST", "Actions"]}
         expected_df = pd.DataFrame(expected)
         self.assertEqual(result, Batch(expected_df))
 
         # stop the server
-        os.system("nohup eva_server --stop")
+        os.system("nohup evadb_server --stop")
```

### Comparing `evadb-0.2.7/test/integration_tests/test_similarity.py` & `evadb-0.2.8/test/integration_tests/test_similarity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/integration_tests/test_udf_executor.py` & `evadb-0.2.8/test/integration_tests/test_udf_executor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/interfaces/__init__.py` & `evadb-0.2.8/test/interfaces/relational/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/interfaces/relational/__init__.py` & `evadb-0.2.8/test/models/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/interfaces/relational/test_relational_api.py` & `evadb-0.2.8/test/interfaces/relational/test_relational_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -22,38 +22,38 @@
 )
 
 import numpy as np
 import pandas as pd
 from pandas.testing import assert_frame_equal
 
 from evadb.binder.binder_utils import BinderError
-from evadb.configuration.constants import EVA_DATABASE_DIR, EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_DATABASE_DIR, EvaDB_ROOT_DIR
 from evadb.executor.executor_utils import ExecutorError
 from evadb.interfaces.relational.db import connect
 from evadb.models.storage.batch import Batch
 from evadb.server.command_handler import execute_query_fetch_all
 
 
 class RelationalAPI(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     @classmethod
     def setUpClass(cls):
-        cls.db_dir = suffix_pytest_xdist_worker_id_to_dir(EVA_DATABASE_DIR)
+        cls.db_dir = suffix_pytest_xdist_worker_id_to_dir(EvaDB_DATABASE_DIR)
         cls.conn = connect(cls.db_dir)
         cls.evadb = cls.conn._evadb
 
     def setUp(self):
         self.evadb.catalog().reset()
-        self.mnist_path = f"{EVA_ROOT_DIR}/data/mnist/mnist.mp4"
+        self.mnist_path = f"{EvaDB_ROOT_DIR}/data/mnist/mnist.mp4"
         load_udfs_for_testing(
             self.evadb,
         )
-        self.images = f"{EVA_ROOT_DIR}/data/detoxify/*.jpg"
+        self.images = f"{EvaDB_ROOT_DIR}/data/detoxify/*.jpg"
 
     def tearDown(self):
         shutdown_ray()
         # todo: move these to relational apis as well
         execute_query_fetch_all(self.evadb, """DROP TABLE IF EXISTS mnist_video;""")
         execute_query_fetch_all(self.evadb, """DROP TABLE IF EXISTS meme_images;""")
 
@@ -171,27 +171,27 @@
             format="image",
         )
         rel.execute()
 
         # todo support register udf
         cursor.query(
             f"""CREATE UDF IF NOT EXISTS SiftFeatureExtractor
-                IMPL  '{EVA_ROOT_DIR}/evadb/udfs/sift_feature_extractor.py'"""
+                IMPL  '{EvaDB_ROOT_DIR}/evadb/udfs/sift_feature_extractor.py'"""
         ).df()
 
         # create a vector index using QDRANT
         cursor.create_vector_index(
             "faiss_index",
             table_name="meme_images",
             expr="SiftFeatureExtractor(data)",
             using="QDRANT",
         ).df()
 
         # do similarity search
-        base_image = f"{EVA_ROOT_DIR}/data/detoxify/meme1.jpg"
+        base_image = f"{EvaDB_ROOT_DIR}/data/detoxify/meme1.jpg"
         rel = (
             cursor.table("meme_images")
             .order(
                 f"Similarity(SiftFeatureExtractor(Open('{base_image}')), SiftFeatureExtractor(data))"
             )
             .limit(1)
             .select("name")
@@ -321,47 +321,47 @@
         drop_table = cursor.drop_table("dummy_video", if_exists=False)
         with self.assertRaises(ExecutorError):
             drop_table.execute()
 
     def test_pdf_similarity_search(self):
         conn = connect()
         cursor = conn.cursor()
-        pdf_path1 = f"{EVA_ROOT_DIR}/data/documents/state_of_the_union.pdf"
-        pdf_path2 = f"{EVA_ROOT_DIR}/data/documents/layout-parser-paper.pdf"
+        pdf_path1 = f"{EvaDB_ROOT_DIR}/data/documents/state_of_the_union.pdf"
+        pdf_path2 = f"{EvaDB_ROOT_DIR}/data/documents/layout-parser-paper.pdf"
 
-        load_pdf = cursor.load(file_regex=pdf_path1, format="PDF", table_name="PDFss")
+        load_pdf = cursor.load(file_regex=pdf_path1, format="PDF", table_name="PDFs")
         load_pdf.execute()
 
-        load_pdf = cursor.load(file_regex=pdf_path2, format="PDF", table_name="PDFss")
+        load_pdf = cursor.load(file_regex=pdf_path2, format="PDF", table_name="PDFs")
         load_pdf.execute()
 
         udf_check = cursor.drop_udf("SentenceTransformerFeatureExtractor")
         udf_check.df()
         udf = cursor.create_udf(
             "SentenceTransformerFeatureExtractor",
             True,
-            f"{EVA_ROOT_DIR}/evadb/udfs/sentence_transformer_feature_extractor.py",
+            f"{EvaDB_ROOT_DIR}/evadb/udfs/sentence_transformer_feature_extractor.py",
         )
         udf.execute()
 
         cursor.create_vector_index(
             "faiss_index",
-            table_name="PDFss",
+            table_name="PDFs",
             expr="SentenceTransformerFeatureExtractor(data)",
             using="QDRANT",
         ).df()
 
         query = (
-            cursor.table("PDFss")
+            cursor.table("PDFs")
             .order(
                 """Similarity(
                     SentenceTransformerFeatureExtractor('When was the NATO created?'), SentenceTransformerFeatureExtractor(data)
                 ) DESC"""
             )
             .limit(3)
             .select("data")
         )
         output = query.df()
         self.assertEqual(len(output), 3)
-        self.assertTrue("pdfss.data" in output.columns)
+        self.assertTrue("pdfs.data" in output.columns)
 
         cursor.drop_index("faiss_index").df()
```

### Comparing `evadb-0.2.7/test/markers.py` & `evadb-0.2.8/test/markers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/models/__init__.py` & `evadb-0.2.8/test/models/catalog/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/models/catalog/__init__.py` & `evadb-0.2.8/test/models/storage/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/models/catalog/test_frame_info.py` & `evadb-0.2.8/test/models/catalog/test_frame_info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/models/storage/__init__.py` & `evadb-0.2.8/test/optimizer/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/models/storage/test_batch.py` & `evadb-0.2.8/test/models/storage/test_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/__init__.py` & `evadb-0.2.8/test/optimizer/rules/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/rules/__init__.py` & `evadb-0.2.8/test/parser/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/rules/test_rules.py` & `evadb-0.2.8/test/optimizer/rules/test_rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_binder.py` & `evadb-0.2.8/test/optimizer/test_binder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_cascade_optimizer.py` & `evadb-0.2.8/test/optimizer/test_cascade_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_cost_model.py` & `evadb-0.2.8/test/optimizer/test_cost_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_group.py` & `evadb-0.2.8/test/optimizer/test_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_memo.py` & `evadb-0.2.8/test/optimizer/test_memo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_optimizer_context.py` & `evadb-0.2.8/test/optimizer/test_optimizer_context.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_optimizer_task.py` & `evadb-0.2.8/test/optimizer/test_optimizer_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_optimizer_utils.py` & `evadb-0.2.8/test/optimizer/test_optimizer_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/optimizer/test_statement_to_opr_converter.py` & `evadb-0.2.8/test/optimizer/test_statement_to_opr_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/parser/__init__.py` & `evadb-0.2.8/test/plan_nodes/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/parser/test_parser.py` & `evadb-0.2.8/test/parser/test_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -51,55 +51,55 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def test_create_index_statement(self):
         parser = Parser()
 
         create_index_query = "CREATE INDEX testindex ON MyVideo (featCol) USING FAISS;"
-        eva_stmt_list = parser.parse(create_index_query)
+        evadb_stmt_list = parser.parse(create_index_query)
 
         # check stmt itself
-        self.assertIsInstance(eva_stmt_list, list)
-        self.assertEqual(len(eva_stmt_list), 1)
-        self.assertEqual(eva_stmt_list[0].stmt_type, StatementType.CREATE_INDEX)
+        self.assertIsInstance(evadb_stmt_list, list)
+        self.assertEqual(len(evadb_stmt_list), 1)
+        self.assertEqual(evadb_stmt_list[0].stmt_type, StatementType.CREATE_INDEX)
 
         expected_stmt = CreateIndexStatement(
             "testindex",
             TableRef(TableInfo("MyVideo")),
             [
                 ColumnDefinition("featCol", None, None, None),
             ],
             VectorStoreType.FAISS,
         )
-        actual_stmt = eva_stmt_list[0]
+        actual_stmt = evadb_stmt_list[0]
         self.assertEqual(actual_stmt, expected_stmt)
 
         # create index on UDF expression
         create_index_query = (
             "CREATE INDEX testindex ON MyVideo (FeatureExtractor(featCol)) USING FAISS;"
         )
-        eva_stmt_list = parser.parse(create_index_query)
+        evadb_stmt_list = parser.parse(create_index_query)
 
         # check stmt itself
-        self.assertIsInstance(eva_stmt_list, list)
-        self.assertEqual(len(eva_stmt_list), 1)
-        self.assertEqual(eva_stmt_list[0].stmt_type, StatementType.CREATE_INDEX)
+        self.assertIsInstance(evadb_stmt_list, list)
+        self.assertEqual(len(evadb_stmt_list), 1)
+        self.assertEqual(evadb_stmt_list[0].stmt_type, StatementType.CREATE_INDEX)
 
         func_expr = FunctionExpression(None, "FeatureExtractor")
         func_expr.append_child(TupleValueExpression("featCol"))
         expected_stmt = CreateIndexStatement(
             "testindex",
             TableRef(TableInfo("MyVideo")),
             [
                 ColumnDefinition("featCol", None, None, None),
             ],
             VectorStoreType.FAISS,
             func_expr,
         )
-        actual_stmt = eva_stmt_list[0]
+        actual_stmt = evadb_stmt_list[0]
         self.assertEqual(actual_stmt, expected_stmt)
 
     @unittest.skip("Skip parser exception handling testcase, moved to binder")
     def test_create_index_exception_statement(self):
         parser = Parser()
 
         create_index_query = (
@@ -109,23 +109,23 @@
         with self.assertRaises(Exception):
             parser.parse(create_index_query)
 
     def test_explain_dml_statement(self):
         parser = Parser()
 
         explain_query = "EXPLAIN SELECT CLASS FROM TAIPAI;"
-        eva_statement_list = parser.parse(explain_query)
+        evadb_statement_list = parser.parse(explain_query)
 
         # check explain stmt itself
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.EXPLAIN)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.EXPLAIN)
 
         # check inner stmt
-        inner_stmt = eva_statement_list[0].explainable_stmt
+        inner_stmt = evadb_statement_list[0].explainable_stmt
         self.assertEqual(inner_stmt.stmt_type, StatementType.SELECT)
 
         # check inner stmt from
         self.assertIsNotNone(inner_stmt.from_table)
         self.assertIsInstance(inner_stmt.from_table, TableRef)
         self.assertEqual(inner_stmt.from_table.table.table_name, "TAIPAI")
 
@@ -134,23 +134,23 @@
 
         select_query = """SELECT id, Yolo(frame).labels FROM MyVideo
                         WHERE id<5; """
         explain_query = "EXPLAIN CREATE MATERIALIZED VIEW uadtrac_fastRCNN (id, labels) AS {}".format(
             select_query
         )
 
-        eva_statement_list = parser.parse(explain_query)
+        evadb_statement_list = parser.parse(explain_query)
 
         # check explain stmt itself
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.EXPLAIN)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.EXPLAIN)
 
         # check inner stmt
-        inner_stmt = eva_statement_list[0].explainable_stmt
+        inner_stmt = evadb_statement_list[0].explainable_stmt
         self.assertEqual(inner_stmt.stmt_type, StatementType.CREATE_MATERIALIZED_VIEW)
 
         # check inner stmt from
         self.assertIsNotNone(
             inner_stmt.view_info, TableRef(TableInfo("uadetrac_fastRCNN"))
         )
 
@@ -190,19 +190,19 @@
                     (5, 100, 2432, 4324, 100),
                     expected_cci,
                 ),
             ],
         )
 
         for query in single_queries:
-            eva_statement_list = parser.parse(query)
-            self.assertIsInstance(eva_statement_list, list)
-            self.assertEqual(len(eva_statement_list), 1)
-            self.assertIsInstance(eva_statement_list[0], AbstractStatement)
-            self.assertEqual(eva_statement_list[0], expected_stmt)
+            evadb_statement_list = parser.parse(query)
+            self.assertIsInstance(evadb_statement_list, list)
+            self.assertEqual(len(evadb_statement_list), 1)
+            self.assertIsInstance(evadb_statement_list[0], AbstractStatement)
+            self.assertEqual(evadb_statement_list[0], expected_stmt)
 
     def test_create_table_statement_with_rare_datatypes(self):
         parser = Parser()
         query = """CREATE TABLE IF NOT EXISTS Dummy (
                   C NDARRAY UINT8(5),
                   D NDARRAY INT16(5),
                   E NDARRAY INT32(5),
@@ -210,18 +210,18 @@
                   G NDARRAY UNICODE(5),
                   H NDARRAY BOOLEAN(5),
                   I NDARRAY FLOAT64(5),
                   J NDARRAY DECIMAL(5),
                   K NDARRAY DATETIME(5)
             );"""
 
-        eva_statement_list = parser.parse(query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertIsInstance(eva_statement_list[0], AbstractStatement)
+        evadb_statement_list = parser.parse(query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertIsInstance(evadb_statement_list[0], AbstractStatement)
 
     def test_create_table_statement_without_proper_datatype(self):
         parser = Parser()
         query = """CREATE TABLE IF NOT EXISTS Dummy (
                   C NDARRAY INT(5)
                 );"""
 
@@ -238,31 +238,31 @@
 
     def test_rename_table_statement(self):
         parser = Parser()
         rename_queries = "RENAME TABLE student TO student_info"
         expected_stmt = RenameTableStatement(
             TableRef(TableInfo("student")), TableInfo("student_info")
         )
-        eva_statement_list = parser.parse(rename_queries)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.RENAME)
+        evadb_statement_list = parser.parse(rename_queries)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.RENAME)
 
-        rename_stmt = eva_statement_list[0]
+        rename_stmt = evadb_statement_list[0]
         self.assertEqual(rename_stmt, expected_stmt)
 
     def test_drop_table_statement(self):
         parser = Parser()
         drop_queries = "DROP TABLE student_info"
         expected_stmt = DropObjectStatement(ObjectType.TABLE, "student_info", False)
-        eva_statement_list = parser.parse(drop_queries)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.DROP_OBJECT)
-        drop_stmt = eva_statement_list[0]
+        evadb_statement_list = parser.parse(drop_queries)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.DROP_OBJECT)
+        drop_stmt = evadb_statement_list[0]
         self.assertEqual(drop_stmt, expected_stmt)
 
     def test_drop_udf_statement_str(self):
         drop_udf_query1 = """DROP UDF MyUDF;"""
         drop_udf_query2 = """DROP UDF IF EXISTS MyUDF;"""
         expected_stmt1 = DropObjectStatement(ObjectType.UDF, "MyUDF", False)
         expected_stmt2 = DropObjectStatement(ObjectType.UDF, "MyUDF", True)
@@ -285,48 +285,48 @@
         )
         single_queries.append(
             "SELECT CLASS FROM TAIPAI \
             WHERE (CLASS = 'VAN' AND REDNESS < 300 ) OR REDNESS > 500;"
         )
 
         for query in single_queries:
-            eva_statement_list = parser.parse(query)
+            evadb_statement_list = parser.parse(query)
 
-            self.assertIsInstance(eva_statement_list, list)
-            self.assertEqual(len(eva_statement_list), 1)
-            self.assertIsInstance(eva_statement_list[0], AbstractStatement)
+            self.assertIsInstance(evadb_statement_list, list)
+            self.assertEqual(len(evadb_statement_list), 1)
+            self.assertIsInstance(evadb_statement_list[0], AbstractStatement)
 
     def test_multiple_statement_queries(self):
         parser = Parser()
 
         multiple_queries = []
         multiple_queries.append(
             "SELECT CLASS FROM TAIPAI \
                 WHERE (CLASS != 'VAN' AND REDNESS < 300)  OR REDNESS > 500; \
                 SELECT REDNESS FROM TAIPAI \
                 WHERE (CLASS = 'VAN' AND REDNESS = 300)"
         )
 
         for query in multiple_queries:
-            eva_statement_list = parser.parse(query)
-            self.assertIsInstance(eva_statement_list, list)
-            self.assertEqual(len(eva_statement_list), 2)
-            self.assertIsInstance(eva_statement_list[0], AbstractStatement)
-            self.assertIsInstance(eva_statement_list[1], AbstractStatement)
+            evadb_statement_list = parser.parse(query)
+            self.assertIsInstance(evadb_statement_list, list)
+            self.assertEqual(len(evadb_statement_list), 2)
+            self.assertIsInstance(evadb_statement_list[0], AbstractStatement)
+            self.assertIsInstance(evadb_statement_list[1], AbstractStatement)
 
     def test_select_statement(self):
         parser = Parser()
         select_query = "SELECT CLASS, REDNESS FROM TAIPAI \
                 WHERE (CLASS = 'VAN' AND REDNESS < 300 ) OR REDNESS > 500;"
-        eva_statement_list = parser.parse(select_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.SELECT)
+        evadb_statement_list = parser.parse(select_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.SELECT)
 
-        select_stmt = eva_statement_list[0]
+        select_stmt = evadb_statement_list[0]
 
         # target List
         self.assertIsNotNone(select_stmt.target_list)
         self.assertEqual(len(select_stmt.target_list), 2)
         self.assertEqual(select_stmt.target_list[0].etype, ExpressionType.TUPLE_VALUE)
         self.assertEqual(select_stmt.target_list[1].etype, ExpressionType.TUPLE_VALUE)
 
@@ -340,25 +340,25 @@
         # other tests should go in expression testing
 
     def test_select_with_empty_string_literal(self):
         parser = Parser()
 
         select_query = """SELECT '' FROM TAIPAI;"""
 
-        eva_statement_list = parser.parse(select_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.SELECT)
+        evadb_statement_list = parser.parse(select_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.SELECT)
 
     def test_select_union_statement(self):
         parser = Parser()
         select_union_query = "SELECT CLASS, REDNESS FROM TAIPAI \
             UNION ALL SELECT CLASS, REDNESS FROM SHANGHAI;"
-        eva_statement_list = parser.parse(select_union_query)
-        select_stmt = eva_statement_list[0]
+        evadb_statement_list = parser.parse(select_union_query)
+        select_stmt = evadb_statement_list[0]
         self.assertIsNotNone(select_stmt.union_link)
         self.assertEqual(select_stmt.union_all, True)
         second_select_stmt = select_stmt.union_link
         self.assertIsNone(second_select_stmt.union_link)
 
     def test_select_statement_class(self):
         """Testing setting different clauses for Select
@@ -366,16 +366,16 @@
         Class: SelectStatement"""
 
         select_stmt_new = SelectStatement()
         parser = Parser()
 
         select_query_new = "SELECT CLASS, REDNESS FROM TAIPAI \
             WHERE (CLASS = 'VAN' AND REDNESS < 400 ) OR REDNESS > 700;"
-        eva_statement_list = parser.parse(select_query_new)
-        select_stmt = eva_statement_list[0]
+        evadb_statement_list = parser.parse(select_query_new)
+        select_stmt = evadb_statement_list[0]
 
         select_stmt_new.where_clause = select_stmt.where_clause
         select_stmt_new.target_list = select_stmt.target_list
         select_stmt_new.from_table = select_stmt.from_table
 
         self.assertEqual(select_stmt_new.where_clause, select_stmt.where_clause)
         self.assertEqual(select_stmt_new.target_list, select_stmt.target_list)
@@ -385,20 +385,20 @@
     def test_select_statement_groupby_class(self):
         """Testing sample frequency"""
 
         parser = Parser()
 
         select_query = "SELECT FIRST(id) FROM TAIPAI GROUP BY '8 frames';"
 
-        eva_statement_list = parser.parse(select_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.SELECT)
+        evadb_statement_list = parser.parse(select_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.SELECT)
 
-        select_stmt = eva_statement_list[0]
+        select_stmt = evadb_statement_list[0]
 
         # target List
         self.assertIsNotNone(select_stmt.target_list)
         self.assertEqual(len(select_stmt.target_list), 1)
         self.assertEqual(
             select_stmt.target_list[0].etype, ExpressionType.AGGREGATION_FIRST
         )
@@ -421,20 +421,20 @@
         parser = Parser()
 
         select_query = "SELECT CLASS, REDNESS FROM TAIPAI \
                     WHERE (CLASS = 'VAN' AND REDNESS < 400 ) OR REDNESS > 700 \
                     ORDER BY CLASS, REDNESS DESC;"
         # if orderby sort_type (ASC/DESC) not provided, should default to ASC
 
-        eva_statement_list = parser.parse(select_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.SELECT)
+        evadb_statement_list = parser.parse(select_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.SELECT)
 
-        select_stmt = eva_statement_list[0]
+        select_stmt = evadb_statement_list[0]
 
         # target List
         self.assertIsNotNone(select_stmt.target_list)
         self.assertEqual(len(select_stmt.target_list), 2)
         self.assertEqual(select_stmt.target_list[0].etype, ExpressionType.TUPLE_VALUE)
         self.assertEqual(select_stmt.target_list[1].etype, ExpressionType.TUPLE_VALUE)
 
@@ -460,20 +460,20 @@
 
         parser = Parser()
 
         select_query = "SELECT CLASS, REDNESS FROM TAIPAI \
                     WHERE (CLASS = 'VAN' AND REDNESS < 400 ) OR REDNESS > 700 \
                     ORDER BY CLASS, REDNESS DESC LIMIT 3;"
 
-        eva_statement_list = parser.parse(select_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.SELECT)
+        evadb_statement_list = parser.parse(select_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.SELECT)
 
-        select_stmt = eva_statement_list[0]
+        select_stmt = evadb_statement_list[0]
 
         # target List
         self.assertIsNotNone(select_stmt.target_list)
         self.assertEqual(len(select_stmt.target_list), 2)
         self.assertEqual(select_stmt.target_list[0].etype, ExpressionType.TUPLE_VALUE)
         self.assertEqual(select_stmt.target_list[1].etype, ExpressionType.TUPLE_VALUE)
 
@@ -500,20 +500,20 @@
     def test_select_statement_sample_class(self):
         """Testing sample frequency"""
 
         parser = Parser()
 
         select_query = "SELECT CLASS, REDNESS FROM TAIPAI SAMPLE 5;"
 
-        eva_statement_list = parser.parse(select_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.SELECT)
+        evadb_statement_list = parser.parse(select_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.SELECT)
 
-        select_stmt = eva_statement_list[0]
+        select_stmt = evadb_statement_list[0]
 
         # target List
         self.assertIsNotNone(select_stmt.target_list)
         self.assertEqual(len(select_stmt.target_list), 2)
         self.assertEqual(select_stmt.target_list[0].etype, ExpressionType.TUPLE_VALUE)
         self.assertEqual(select_stmt.target_list[1].etype, ExpressionType.TUPLE_VALUE)
 
@@ -549,32 +549,32 @@
                 TupleValueExpression("Frame_Path"),
             ],
             [
                 ConstantValueExpression(1),
                 ConstantValueExpression("/mnt/frames/1.png", ColumnType.TEXT),
             ],
         )
-        eva_statement_list = parser.parse(insert_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.INSERT)
+        evadb_statement_list = parser.parse(insert_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.INSERT)
 
-        insert_stmt = eva_statement_list[0]
+        insert_stmt = evadb_statement_list[0]
         self.assertEqual(insert_stmt, expected_stmt)
 
     def test_delete_statement(self):
         parser = Parser()
         delete_statement = """DELETE FROM Foo WHERE id > 5"""
 
-        eva_statement_list = parser.parse(delete_statement)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.DELETE)
+        evadb_statement_list = parser.parse(delete_statement)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.DELETE)
 
-        delete_stmt = eva_statement_list[0]
+        delete_stmt = evadb_statement_list[0]
 
         expected_stmt = DeleteTableStatement(
             TableRef(TableInfo("Foo")),
             ComparisonExpression(
                 ExpressionType.COMPARE_GREATER,
                 TupleValueExpression("id"),
                 ConstantValueExpression(5),
@@ -615,21 +615,21 @@
                 ColumnDefinition(
                     "Bbox", ColumnType.NDARRAY, NdArrayType.UINT8, (10, 4), expected_cci
                 ),
             ],
             "Classification",
             [("KEY", "VALUE")],
         )
-        eva_statement_list = parser.parse(create_udf_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.CREATE_UDF)
-        self.assertEqual(str(eva_statement_list[0]), str(expected_stmt))
+        evadb_statement_list = parser.parse(create_udf_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.CREATE_UDF)
+        self.assertEqual(str(evadb_statement_list[0]), str(expected_stmt))
 
-        create_udf_stmt = eva_statement_list[0]
+        create_udf_stmt = evadb_statement_list[0]
 
         self.assertEqual(create_udf_stmt, expected_stmt)
 
     def test_load_video_data_statement(self):
         parser = Parser()
         load_data_query = """LOAD VIDEO 'data/video.mp4'
                              INTO MyVideo"""
@@ -638,20 +638,20 @@
         column_list = None
         expected_stmt = LoadDataStatement(
             TableInfo("MyVideo"),
             Path("data/video.mp4"),
             column_list,
             file_options,
         )
-        eva_statement_list = parser.parse(load_data_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.LOAD_DATA)
+        evadb_statement_list = parser.parse(load_data_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.LOAD_DATA)
 
-        load_data_stmt = eva_statement_list[0]
+        load_data_stmt = evadb_statement_list[0]
         self.assertEqual(load_data_stmt, expected_stmt)
 
     def test_load_csv_data_statement(self):
         parser = Parser()
         load_data_query = """LOAD CSV 'data/meta.csv'
                              INTO
                              MyMeta (id, frame_id, video_id, label);"""
@@ -664,20 +664,20 @@
                 TupleValueExpression("id"),
                 TupleValueExpression("frame_id"),
                 TupleValueExpression("video_id"),
                 TupleValueExpression("label"),
             ],
             file_options,
         )
-        eva_statement_list = parser.parse(load_data_query)
-        self.assertIsInstance(eva_statement_list, list)
-        self.assertEqual(len(eva_statement_list), 1)
-        self.assertEqual(eva_statement_list[0].stmt_type, StatementType.LOAD_DATA)
+        evadb_statement_list = parser.parse(load_data_query)
+        self.assertIsInstance(evadb_statement_list, list)
+        self.assertEqual(len(evadb_statement_list), 1)
+        self.assertEqual(evadb_statement_list[0].stmt_type, StatementType.LOAD_DATA)
 
-        load_data_stmt = eva_statement_list[0]
+        load_data_stmt = evadb_statement_list[0]
         self.assertEqual(load_data_stmt, expected_stmt)
 
     def test_nested_select_statement(self):
         parser = Parser()
         sub_query = """SELECT CLASS FROM TAIPAI WHERE CLASS = 'VAN'"""
         nested_query = """SELECT ID FROM ({}) AS T;""".format(sub_query)
         parsed_sub_query = parser.parse(sub_query)[0]
```

### Comparing `evadb-0.2.7/test/parser/test_parser_statements.py` & `evadb-0.2.8/test/parser/test_parser_statements.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/plan_nodes/__init__.py` & `evadb-0.2.8/test/readers/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/plan_nodes/test_plan.py` & `evadb-0.2.8/test/plan_nodes/test_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/readers/__init__.py` & `evadb-0.2.8/test/server/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/readers/test_csv_reader.py` & `evadb-0.2.8/test/readers/test_csv_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/readers/test_decord_reader.py` & `evadb-0.2.8/test/readers/test_decord_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -20,15 +20,15 @@
     create_sample_video,
     file_remove,
 )
 
 import numpy as np
 import pytest
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.constants import AUDIORATE, IFRAMES
 from evadb.expression.abstract_expression import ExpressionType
 from evadb.expression.comparison_expression import ComparisonExpression
 from evadb.expression.constant_value_expression import ConstantValueExpression
 from evadb.expression.logical_expression import LogicalExpression
 from evadb.expression.tuple_value_expression import TupleValueExpression
 from evadb.readers.decord_reader import DecordReader
@@ -36,20 +36,20 @@
 
 @pytest.mark.notparallel
 class DecordLoaderTest(unittest.TestCase):
     @classmethod
     def setUpClass(self):
         self.video_file_url = create_sample_video()
         self.video_with_audio_file_url = (
-            f"{EVA_ROOT_DIR}/data/sample_videos/touchdown.mp4"
+            f"{EvaDB_ROOT_DIR}/data/sample_videos/touchdown.mp4"
         )
         self.frame_size = FRAME_SIZE[0] * FRAME_SIZE[1] * 3
         self.audio_frames = []
         for line in open(
-            f"{EVA_ROOT_DIR}/test/data/touchdown_audio_frames.csv"
+            f"{EvaDB_ROOT_DIR}/test/data/touchdown_audio_frames.csv"
         ).readlines():
             self.audio_frames.append(np.fromstring(line, sep=","))
 
     @classmethod
     def tearDownClass(self):
         file_remove("dummy.avi")
```

### Comparing `evadb-0.2.7/test/server/__init__.py` & `evadb-0.2.8/test/storage/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/server/test_command_handler.py` & `evadb-0.2.8/test/server/test_command_handler.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/server/test_db_api.py` & `evadb-0.2.8/test/server/test_db_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,15 +16,15 @@
 import os
 import sys
 import unittest
 from test.util import suffix_pytest_xdist_worker_id_to_dir
 
 from mock import MagicMock, patch
 
-from evadb.interfaces.relational.db import EVADBCursor, connect_remote
+from evadb.interfaces.relational.db import EvaDBCursor, connect_remote
 from evadb.models.server.response import Response
 
 # Check for Python 3.8+ for IsolatedAsyncioTestCase support
 if sys.version_info >= (3, 8):
     from unittest.mock import AsyncMock
 
     class DBAPITests(unittest.IsolatedAsyncioTestCase):
@@ -39,98 +39,98 @@
             return super().setUp()
 
         def tearDown(self) -> None:
             print("tearDown")
             os.remove(suffix_pytest_xdist_worker_id_to_dir("upload.txt"))
             return super().tearDown()
 
-        def test_eva_cursor_execute_async(self):
+        def test_evadb_cursor_execute_async(self):
             connection = AsyncMock()
-            eva_cursor = EVADBCursor(connection)
+            evadb_cursor = EvaDBCursor(connection)
             query = "test_query"
-            asyncio.run(eva_cursor.execute_async(query))
-            self.assertEqual(eva_cursor._pending_query, True)
+            asyncio.run(evadb_cursor.execute_async(query))
+            self.assertEqual(evadb_cursor._pending_query, True)
 
             # concurrent queries not allowed
             with self.assertRaises(SystemError):
-                asyncio.run(eva_cursor.execute_async(query))
+                asyncio.run(evadb_cursor.execute_async(query))
 
-        def test_eva_cursor_fetch_all_async(self):
+        def test_evadb_cursor_fetch_all_async(self):
             connection = AsyncMock()
-            eva_cursor = EVADBCursor(connection)
+            evadb_cursor = EvaDBCursor(connection)
             message = "test_response"
             serialized_message = Response.serialize("test_response")
             serialized_message_length = b"%d" % len(serialized_message)
             connection._reader.readline.side_effect = [serialized_message_length]
             connection._reader.readexactly.side_effect = [serialized_message]
-            response = asyncio.run(eva_cursor.fetch_all_async())
-            self.assertEqual(eva_cursor._pending_query, False)
+            response = asyncio.run(evadb_cursor.fetch_all_async())
+            self.assertEqual(evadb_cursor._pending_query, False)
             self.assertEqual(message, response)
 
-        def test_eva_cursor_fetch_one_sync(self):
+        def test_evadb_cursor_fetch_one_sync(self):
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
 
             connection = AsyncMock()
-            eva_cursor = EVADBCursor(connection)
+            evadb_cursor = EvaDBCursor(connection)
 
             message = "test_response"
             serialized_message = Response.serialize("test_response")
             serialized_message_length = b"%d" % len(serialized_message)
             connection._reader.readline.side_effect = [serialized_message_length]
             connection._reader.readexactly.side_effect = [serialized_message]
 
-            response = eva_cursor.fetch_one()
-            self.assertEqual(eva_cursor._pending_query, False)
+            response = evadb_cursor.fetch_one()
+            self.assertEqual(evadb_cursor._pending_query, False)
             self.assertEqual(message, response)
 
-        def test_eva_connection(self):
+        def test_evadb_connection(self):
             hostname = "localhost"
 
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
 
             connection = AsyncMock()
-            eva_cursor = EVADBCursor(connection)
+            evadb_cursor = EvaDBCursor(connection)
 
             # test attr
             with self.assertRaises(AttributeError):
-                eva_cursor.__getattr__("foo")
+                evadb_cursor.__getattr__("foo")
 
             # test connection error with incorrect port
             with self.assertRaises(OSError):
                 connect_remote(hostname, port=1)
 
-        async def test_eva_signal(self):
+        async def test_evadb_signal(self):
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
 
             connection = AsyncMock()
-            eva_cursor = EVADBCursor(connection)
+            evadb_cursor = EvaDBCursor(connection)
 
             query = "test_query"
-            await eva_cursor.execute_async(query)
+            await evadb_cursor.execute_async(query)
 
         def test_client_stop_query(self):
             connection = AsyncMock()
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
             connection.protocol.loop = loop
 
-            eva_cursor = EVADBCursor(connection)
-            eva_cursor.execute("test_query")
-            eva_cursor.stop_query()
-            self.assertEqual(eva_cursor._pending_query, False)
+            evadb_cursor = EvaDBCursor(connection)
+            evadb_cursor.execute("test_query")
+            evadb_cursor.stop_query()
+            self.assertEqual(evadb_cursor._pending_query, False)
 
         def test_get_attr(self):
             connection = AsyncMock()
 
-            eva_cursor = EVADBCursor(connection)
+            evadb_cursor = EvaDBCursor(connection)
             with self.assertRaises(AttributeError):
-                eva_cursor.missing_function()
+                evadb_cursor.missing_function()
 
         @patch("asyncio.open_connection")
         def test_get_connection(self, mock_open):
             server_reader = asyncio.StreamReader()
             server_writer = MagicMock()
             mock_open.return_value = (server_reader, server_writer)
```

### Comparing `evadb-0.2.7/test/server/test_interpreter.py` & `evadb-0.2.8/test/server/test_interpreter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -26,16 +26,16 @@
 
     class InterpreterTests(unittest.IsolatedAsyncioTestCase):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         @patch("asyncio.open_connection")
         @patch("evadb.server.interpreter.create_stdin_reader")
-        @patch("evadb.interfaces.relational.db.EVADBCursor.execute_async")
-        @patch("evadb.interfaces.relational.db.EVADBCursor.fetch_all_async")
+        @patch("evadb.interfaces.relational.db.EvaDBCursor.execute_async")
+        @patch("evadb.interfaces.relational.db.EvaDBCursor.fetch_all_async")
         async def test_start_cmd_client(
             self, mock_fetch, mock_execute, mock_stdin_reader, mock_open
         ):
             host = "localhost"
             port = find_free_port()
 
             server_reader = asyncio.StreamReader()
```

### Comparing `evadb-0.2.7/test/server/test_server.py` & `evadb-0.2.8/test/server/test_server.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,47 +14,48 @@
 # limitations under the License.
 import asyncio
 import sys
 import unittest
 
 from mock import MagicMock, patch
 
+from evadb.configuration.constants import EvaDB_DATABASE_DIR
 from evadb.server.server import EvaServer
 
 # Check for Python 3.8+ for IsolatedAsyncioTestCase support
 if sys.version_info >= (3, 8):
 
     class ServerTests(unittest.IsolatedAsyncioTestCase):
         def __init__(self, *args, **kwargs):
             super().__init__(*args, **kwargs)
 
         @patch("asyncio.start_server")
         async def test_server_functions(self, mock_start):
-            eva_server = EvaServer()
+            evadb_server = EvaServer()
             host = "localhost"
             port = 8803
 
-            await eva_server.start_eva_server("eva_db", host, port)
+            await evadb_server.start_evadb_server(EvaDB_DATABASE_DIR, host, port)
 
             # connection made
             client_reader1 = asyncio.StreamReader()
             client_writer1 = MagicMock()
             client_reader2 = asyncio.StreamReader()
             client_writer2 = MagicMock()
 
             # first client
             client_reader1.feed_data(b"SHOW UDFS;\n")
             client_reader1.feed_data(b"EXIT;\n")
 
-            await eva_server.accept_client(client_reader1, client_writer1)
-            assert len(eva_server._clients) == 1
+            await evadb_server.accept_client(client_reader1, client_writer1)
+            assert len(evadb_server._clients) == 1
 
             # another client
             client_reader2.feed_data(b"\xC4pple")  # trigger UnicodeDecodeError
             client_reader2.feed_eof()
 
-            await eva_server.accept_client(client_reader2, client_writer2)
-            assert len(eva_server._clients) == 2
+            await evadb_server.accept_client(client_reader2, client_writer2)
+            assert len(evadb_server._clients) == 2
 
-            await eva_server.handle_client(client_reader2, client_writer2)
+            await evadb_server.handle_client(client_reader2, client_writer2)
 
-            await eva_server.stop_eva_server()
+            await evadb_server.stop_evadb_server()
```

### Comparing `evadb-0.2.7/test/storage/__init__.py` & `evadb-0.2.8/test/udfs/decorators/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/storage/test_sqlite_storage_engine.py` & `evadb-0.2.8/test/storage/test_sqlite_storage_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/storage/test_video_storage.py` & `evadb-0.2.8/test/storage/test_video_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/test_eva_cmd_client.py` & `evadb-0.2.8/test/test_eva_cmd_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,65 +15,65 @@
 import argparse
 import asyncio
 import unittest
 
 from mock import call, patch
 
 from evadb.configuration.configuration_manager import ConfigurationManager
-from evadb.eva_cmd_client import eva_client, main
+from evadb.evadb_cmd_client import evadb_client, main
 
 
 class CMDClientTest(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get_mock_stdin_reader(self) -> asyncio.StreamReader:
         stdin_reader = asyncio.StreamReader()
         stdin_reader.feed_data(b"EXIT;\n")
         stdin_reader.feed_eof()
         return stdin_reader
 
-    @patch("evadb.eva_cmd_client.start_cmd_client")
+    @patch("evadb.evadb_cmd_client.start_cmd_client")
     @patch("evadb.server.interpreter.create_stdin_reader")
-    def test_eva_client(self, mock_stdin_reader, mock_client):
+    def test_evadb_client(self, mock_stdin_reader, mock_client):
         mock_stdin_reader.return_value = self.get_mock_stdin_reader()
         mock_client.side_effect = Exception("Test")
 
         async def test():
             with self.assertRaises(Exception):
-                await eva_client("0.0.0.0", 8803)
+                await evadb_client("0.0.0.0", 8803)
 
         asyncio.run(test())
 
         mock_client.reset_mock()
         mock_client.side_effect = KeyboardInterrupt
 
         async def test2():
             # Pass exception
-            await eva_client("0.0.0.0", 8803)
+            await evadb_client("0.0.0.0", 8803)
 
         asyncio.run(test2())
 
     @patch("argparse.ArgumentParser.parse_known_args")
-    @patch("evadb.eva_cmd_client.start_cmd_client")
-    def test_eva_client_with_cmd_arguments(
+    @patch("evadb.evadb_cmd_client.start_cmd_client")
+    def test_evadb_client_with_cmd_arguments(
         self, mock_start_cmd_client, mock_parse_known_args
     ):
         # Set up the mock to simulate command-line arguments
         mock_parse_known_args.return_value = (
             argparse.Namespace(host="127.0.0.1", port="8800"),
             [],
         )
 
         # Call the function under test
         main()
         mock_start_cmd_client.assert_called_once_with("127.0.0.1", "8800")
 
     @patch("argparse.ArgumentParser.parse_known_args")
-    @patch("evadb.eva_cmd_client.start_cmd_client")
+    @patch("evadb.evadb_cmd_client.start_cmd_client")
     def test_main_without_cmd_arguments(
         self, mock_start_cmd_client, mock_parse_known_args
     ):
         # Set up the mock to simulate missing command-line arguments
         mock_parse_known_args.return_value = (
             argparse.Namespace(host=None, port=None),
             [],
```

### Comparing `evadb-0.2.7/test/test_eva_imports.py` & `evadb-0.2.8/test/test_eva_imports.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -14,25 +14,25 @@
 # limitations under the License.
 import importlib
 import os
 import shutil
 import unittest
 
 
-class EVAImportTest(unittest.TestCase):
+class EvaDBImportTest(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    def test_eva_cli_imports(self):
+    def test_evadb_cli_imports(self):
         """
         Testing imports for running client and server packages,
         when current working directory is changed.
         """
         cur_dir = os.getcwd()
-        new_dir = os.path.join("test_eva", "test")
+        new_dir = os.path.join("test_evadb", "test")
         if not os.path.exists(new_dir):
             os.makedirs(new_dir)
         os.chdir(new_dir)
-        _ = importlib.import_module("evadb.eva_cmd_client")
-        _ = importlib.import_module("evadb.eva_server")
+        _ = importlib.import_module("evadb.evadb_cmd_client")
+        _ = importlib.import_module("evadb.evadb_server")
         os.chdir(cur_dir)
         shutil.rmtree(new_dir)
```

### Comparing `evadb-0.2.7/test/test_eva_server.py` & `evadb-0.2.8/test/test_eva_server.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,26 +12,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 
 from mock import patch
 
-from evadb.eva_server import main, start_eva_server
+from evadb.configuration.constants import EvaDB_DATABASE_DIR
+from evadb.evadb_server import main, start_evadb_server
 
 
-class EVAServerTest(unittest.IsolatedAsyncioTestCase):
+class EvaDBServerTest(unittest.IsolatedAsyncioTestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-    @patch("evadb.eva_server.start_eva_server")
+    @patch("evadb.evadb_server.start_evadb_server")
     @patch("asyncio.run")
-    def test_main(self, mock_run, mock_start_eva_server):
+    def test_main(self, mock_run, mock_start_evadb_server):
         main()
-        mock_start_eva_server.assert_called_once()
+        mock_start_evadb_server.assert_called_once()
         mock_run.assert_called_once()
 
-    @patch("evadb.eva_server.start_eva_server")
+    @patch("evadb.evadb_server.start_evadb_server")
     @patch("asyncio.start_server")
-    async def test_start_eva_server(self, mock_start_eva_server, mock_start):
-        await start_eva_server("eva_data", "0.0.0.0", 8803)
-        mock_start_eva_server.assert_called_once()
+    async def test_start_evadb_server(self, mock_start_evadb_server, mock_start):
+        await start_evadb_server(EvaDB_DATABASE_DIR, "0.0.0.0", 8803)
+        mock_start_evadb_server.assert_called_once()
```

### Comparing `evadb-0.2.7/test/udfs/__init__.py` & `evadb-0.2.8/test/udfs/decorators/io_descriptors/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""user defined functions operating on ndarrays"""
```

### Comparing `evadb-0.2.7/test/udfs/decorators/__init__.py` & `evadb-0.2.8/test/utils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/decorators/io_descriptors/test_descriptors.py` & `evadb-0.2.8/test/udfs/decorators/io_descriptors/test_descriptors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/decorators/test_decorators.py` & `evadb-0.2.8/test/udfs/decorators/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/__init__.py` & `evadb-0.2.8/test/udfs/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding=utf-8
-# Copyright 2018-2022 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""user defined test functions operating on ndarrays udfs"""
+"""user defined functions operating on ndarrays"""
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_annotate.py` & `evadb-0.2.8/test/udfs/ndarray/test_annotate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,28 +15,28 @@
 import unittest
 
 import numpy as np
 import pandas as pd
 from numpy import asarray
 from PIL import Image
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.udfs.ndarray.annotate import Annotate
 
 
 class AnnotateTests(unittest.TestCase):
     def setUp(self):
         self.annotate_instance = Annotate()
 
     def test_annotate_name_exists(self):
         assert hasattr(self.annotate_instance, "name")
 
     def test_should_annotate(self):
         img = Image.open(
-            f"{EVA_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/img00001.jpg"
+            f"{EvaDB_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/img00001.jpg"
         )
         arr = asarray(img)
         arr_copy = 0 + arr
         object_type = np.array(["object"])
         bbox = np.array([[50, 50, 70, 70]])
         df = pd.DataFrame([[arr, object_type, bbox]])
         modified_arr = self.annotate_instance(df)["annotated_frame_array"]
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_array_count.py` & `evadb-0.2.8/test/udfs/ndarray/test_array_count.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_crop.py` & `evadb-0.2.8/test/udfs/ndarray/test_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_flips.py` & `evadb-0.2.8/test/udfs/ndarray/test_flips.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -15,15 +15,15 @@
 import unittest
 
 import numpy as np
 import pandas as pd
 from numpy import asarray
 from PIL import Image
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.udfs.ndarray.horizontal_flip import HorizontalFlip
 from evadb.udfs.ndarray.vertical_flip import VerticalFlip
 
 
 class FlipTests(unittest.TestCase):
     def setUp(self):
         self.horizontal_flip_instance = HorizontalFlip()
@@ -31,26 +31,26 @@
 
     def test_flip_name_exists(self):
         assert hasattr(self.horizontal_flip_instance, "name")
         assert hasattr(self.vertical_flip_instance, "name")
 
     def test_should_flip_horizontally(self):
         img = Image.open(
-            f"{EVA_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/img00001.jpg"
+            f"{EvaDB_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/img00001.jpg"
         )
         arr = asarray(img)
         df = pd.DataFrame([[arr]])
         flipped_arr = self.horizontal_flip_instance(df)[
             "horizontally_flipped_frame_array"
         ]
 
         self.assertEqual(np.sum(arr[:, 0] - np.flip(flipped_arr[0][:, -1], 1)), 0)
 
     def test_should_flip_vertically(self):
         img = Image.open(
-            f"{EVA_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/img00001.jpg"
+            f"{EvaDB_ROOT_DIR}/test/data/uadetrac/small-data/MVI_20011/img00001.jpg"
         )
         arr = asarray(img)
         df = pd.DataFrame([[arr]])
         flipped_arr = self.vertical_flip_instance(df)["vertically_flipped_frame_array"]
 
         self.assertEqual(np.sum(arr[0, :] - np.flip(flipped_arr[0][-1, :], 1)), 0)
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_gaussian_blur.py` & `evadb-0.2.8/test/udfs/ndarray/test_gaussian_blur.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,32 +16,32 @@
 from pathlib import Path
 from test.util import file_remove
 
 import cv2
 import numpy as np
 import pandas as pd
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.udfs.ndarray.gaussian_blur import GaussianBlur
 
 
 class GaussianBlurTests(unittest.TestCase):
     def setUp(self):
         self.gb_instance = GaussianBlur()
-        self.tmp_file = f"{EVA_ROOT_DIR}/test/udfs/data/tmp.jpeg"
+        self.tmp_file = f"{EvaDB_ROOT_DIR}/test/udfs/data/tmp.jpeg"
 
     def test_gb_name_exists(self):
         assert hasattr(self.gb_instance, "name")
 
     def test_should_blur_image(self):
-        arr = cv2.imread(f"{EVA_ROOT_DIR}/test/udfs/data/dog.jpeg")
+        arr = cv2.imread(f"{EvaDB_ROOT_DIR}/test/udfs/data/dog.jpeg")
         df = pd.DataFrame([[arr]])
         modified_arr = self.gb_instance(df)["blurred_frame_array"]
         cv2.imwrite(
             self.tmp_file,
             cv2.cvtColor(modified_arr[0], cv2.COLOR_RGB2BGR),
         )
 
         actual_array = cv2.imread(self.tmp_file)
-        expected_array = cv2.imread(f"{EVA_ROOT_DIR}/test/udfs/data/blurred_dog.jpeg")
+        expected_array = cv2.imread(f"{EvaDB_ROOT_DIR}/test/udfs/data/blurred_dog.jpeg")
         self.assertEqual(np.sum(actual_array - expected_array), 0)
         file_remove(Path(self.tmp_file))
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_open.py` & `evadb-0.2.8/test/udfs/ndarray/test_open.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/ndarray/test_to_grayscale.py` & `evadb-0.2.8/test/udfs/ndarray/test_to_grayscale.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -16,27 +16,27 @@
 from pathlib import Path
 from test.util import file_remove
 
 import cv2
 import numpy as np
 import pandas as pd
 
-from evadb.configuration.constants import EVA_ROOT_DIR
+from evadb.configuration.constants import EvaDB_ROOT_DIR
 from evadb.udfs.ndarray.to_grayscale import ToGrayscale
 
 
 class ToGrayscaleTests(unittest.TestCase):
     def setUp(self):
         self.to_grayscale_instance = ToGrayscale()
 
     def test_gray_scale_name_exists(self):
         assert hasattr(self.to_grayscale_instance, "name")
 
     def test_should_convert_to_grayscale(self):
-        arr = cv2.imread(f"{EVA_ROOT_DIR}/test/udfs/data/dog.jpeg")
+        arr = cv2.imread(f"{EvaDB_ROOT_DIR}/test/udfs/data/dog.jpeg")
         df = pd.DataFrame([[arr]])
         modified_arr = self.to_grayscale_instance(df)["grayscale_frame_array"]
-        cv2.imwrite(f"{EVA_ROOT_DIR}/test/udfs/data/tmp.jpeg", modified_arr[0])
-        actual_array = cv2.imread(f"{EVA_ROOT_DIR}/test/udfs/data/tmp.jpeg")
-        expected_arr = cv2.imread(f"{EVA_ROOT_DIR}/test/udfs/data/grayscale_dog.jpeg")
+        cv2.imwrite(f"{EvaDB_ROOT_DIR}/test/udfs/data/tmp.jpeg", modified_arr[0])
+        actual_array = cv2.imread(f"{EvaDB_ROOT_DIR}/test/udfs/data/tmp.jpeg")
+        expected_arr = cv2.imread(f"{EvaDB_ROOT_DIR}/test/udfs/data/grayscale_dog.jpeg")
         self.assertEqual(np.sum(actual_array - expected_arr), 0)
-        file_remove(Path(f"{EVA_ROOT_DIR}/test/udfs/data/tmp.jpeg"))
+        file_remove(Path(f"{EvaDB_ROOT_DIR}/test/udfs/data/tmp.jpeg"))
```

### Comparing `evadb-0.2.7/test/udfs/test_abstract_udf.py` & `evadb-0.2.8/test/udfs/test_abstract_udf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/test_emotion_detector.py` & `evadb-0.2.8/test/udfs/test_emotion_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,26 +11,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 from pathlib import Path
-from test.util import EVA_TEST_DATA_DIR
+from test.util import EvaDB_TEST_DATA_DIR
 
 import cv2
 import pandas as pd
 
 from evadb.models.storage.batch import Batch
 
 
 class EmotionDetector(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.base_path = Path(EVA_TEST_DATA_DIR) / "data" / "emotion_detector"
+        self.base_path = Path(EvaDB_TEST_DATA_DIR) / "data" / "emotion_detector"
 
     def _load_image(self, path):
         assert path.exists(), f"File does not exist at the path {str(path)}"
         img = cv2.imread(str(path))
         return cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
     @unittest.skip("disable test due to model downloading time")
```

### Comparing `evadb-0.2.7/test/udfs/test_facenet_udf.py` & `evadb-0.2.8/test/udfs/test_facenet_udf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -11,29 +11,29 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import unittest
 from pathlib import Path
 from test.markers import windows_skip_marker
-from test.util import EVA_TEST_DATA_DIR
+from test.util import EvaDB_TEST_DATA_DIR
 from unittest.mock import patch
 
 import cv2
 import pandas as pd
 
 from evadb.models.storage.batch import Batch
 
 NUM_FRAMES = 10
 
 
 class FaceNet(unittest.TestCase):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self.base_path = Path(EVA_TEST_DATA_DIR) / "data" / "facenet"
+        self.base_path = Path(EvaDB_TEST_DATA_DIR) / "data" / "facenet"
 
     def _load_image(self, path):
         assert path.exists(), f"File does not exist at the path {str(path)}"
         img = cv2.imread(str(path))
         return cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
 
     @windows_skip_marker
```

### Comparing `evadb-0.2.7/test/udfs/test_fastrcnn_object_detector.py` & `evadb-0.2.8/test/udfs/test_fastrcnn_object_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/udfs/test_yolo_object_detector.py` & `evadb-0.2.8/test/udfs/test_yolo_object_detector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `evadb-0.2.7/test/util.py` & `evadb-0.2.8/test/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -30,16 +30,16 @@
 import ray
 from mock import MagicMock
 
 from evadb.binder.statement_binder import StatementBinder
 from evadb.binder.statement_binder_context import StatementBinderContext
 from evadb.catalog.catalog_type import NdArrayType
 from evadb.configuration.configuration_manager import ConfigurationManager
-from evadb.configuration.constants import EVA_DATABASE_DIR, EVA_INSTALLATION_DIR
-from evadb.database import init_eva_db_instance
+from evadb.configuration.constants import EvaDB_DATABASE_DIR, EvaDB_INSTALLATION_DIR
+from evadb.database import init_evadb_instance
 from evadb.expression.function_expression import FunctionExpression
 from evadb.models.storage.batch import Batch
 from evadb.optimizer.operators import LogicalFilter, Operator
 from evadb.optimizer.plan_generator import PlanGenerator
 from evadb.optimizer.statement_to_opr_converter import StatementToPlanConverter
 from evadb.parser.parser import Parser
 from evadb.plan_nodes.abstract_plan import AbstractPlan
@@ -60,41 +60,41 @@
         path = Path(str(worker_id) + "_" + path)
     except KeyError:
         pass
     return path
 
 
 def get_evadb_for_testing(uri: str = None):
-    db_dir = suffix_pytest_xdist_worker_id_to_dir(EVA_DATABASE_DIR)
+    db_dir = suffix_pytest_xdist_worker_id_to_dir(EvaDB_DATABASE_DIR)
     remove_directory_contents(db_dir)
     gc.collect()
-    return init_eva_db_instance(db_dir, custom_db_uri=uri)
+    return init_evadb_instance(db_dir, custom_db_uri=uri)
 
 
 def get_tmp_dir():
-    db_dir = suffix_pytest_xdist_worker_id_to_dir(EVA_DATABASE_DIR)
+    db_dir = suffix_pytest_xdist_worker_id_to_dir(EvaDB_DATABASE_DIR)
     config = ConfigurationManager(Path(db_dir))
     return config.get_value("storage", "tmp_dir")
 
 
 def s3_dir():
-    db_dir = suffix_pytest_xdist_worker_id_to_dir(EVA_DATABASE_DIR)
+    db_dir = suffix_pytest_xdist_worker_id_to_dir(EvaDB_DATABASE_DIR)
     config = ConfigurationManager(Path(db_dir))
     return config.get_value("storage", "s3_download_dir")
 
 
-EVA_TEST_DATA_DIR = Path(EVA_INSTALLATION_DIR).parent
+EvaDB_TEST_DATA_DIR = Path(EvaDB_INSTALLATION_DIR).parent
 
 
 def is_ray_stage_running():
     return "ray::ray_stage" in (p.name() for p in psutil.process_iter())
 
 
 def shutdown_ray():
-    db_dir = suffix_pytest_xdist_worker_id_to_dir(EVA_DATABASE_DIR)
+    db_dir = suffix_pytest_xdist_worker_id_to_dir(EvaDB_DATABASE_DIR)
     config = ConfigurationManager(Path(db_dir))
     if config.get_value("experimental", "ray"):
         ray.shutdown()
 
 
 # Ref: https://stackoverflow.com/a/63851681
 def get_all_subclasses(cls):
```

### Comparing `evadb-0.2.7/test/utils/test_generic_utils.py` & `evadb-0.2.8/test/utils/test_generic_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,14 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 from test.markers import windows_skip_marker
 
+from evadb.configuration.constants import EvaDB_DATASET_DIR
 from evadb.readers.decord_reader import DecordReader
 from evadb.utils.generic_utils import (
     generate_file_path,
     is_gpu_available,
     load_udf_class_from_file,
     str_to_class,
     validate_kwargs,
@@ -81,11 +82,11 @@
 
         # Switch back to builtin import
         builtins.__import__ = realimport
         is_gpu_available()
 
     @windows_skip_marker
     def test_should_return_a_random_full_path(self):
-        actual = generate_file_path("eva_datasets", "test")
+        actual = generate_file_path(EvaDB_DATASET_DIR, "test")
         self.assertTrue(actual.is_absolute())
         # Root directory must be the same, filename is random
-        self.assertTrue("eva_datasets" in str(actual.parent))
+        self.assertTrue(EvaDB_DATASET_DIR in str(actual.parent))
```

### Comparing `evadb-0.2.7/test/utils/test_timer.py` & `evadb-0.2.8/test/utils/test_timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-# Copyright 2018-2023 EVA
+# Copyright 2018-2023 EvaDB
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

